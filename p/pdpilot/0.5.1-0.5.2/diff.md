# Comparing `tmp/pdpilot-0.5.1.tar.gz` & `tmp/pdpilot-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdpilot-0.5.1.tar", last modified: Tue Jul 25 00:54:45 2023, max compression
+gzip compressed data, was "pdpilot-0.5.2.tar", last modified: Mon Jul 31 13:51:55 2023, max compression
```

## Comparing `pdpilot-0.5.1.tar` & `pdpilot-0.5.2.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.828879 pdpilot-0.5.1/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1499 2022-09-20 18:55:54.000000 pdpilot-0.5.1/LICENSE.txt
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      656 2023-06-30 20:13:32.000000 pdpilot-0.5.1/MANIFEST.in
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1574 2023-07-25 00:54:45.828951 pdpilot-0.5.1/PKG-INFO
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      449 2023-06-30 20:13:32.000000 pdpilot-0.5.1/README.md
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.810268 pdpilot-0.5.1/docs/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      637 2023-02-22 20:30:48.000000 pdpilot-0.5.1/docs/Makefile
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      132 2023-06-30 20:13:32.000000 pdpilot-0.5.1/docs/environment.yml
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      763 2022-12-02 20:03:10.000000 pdpilot-0.5.1/docs/make.bat
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.811794 pdpilot-0.5.1/docs/source/
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.812050 pdpilot-0.5.1/docs/source/_static/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)   290478 2023-07-25 00:53:40.000000 pdpilot-0.5.1/docs/source/_static/embed-bundle.js
--rw-r--r--   0 danielkerrigan   (501) staff       (20)       92 2023-06-30 20:13:32.000000 pdpilot-0.5.1/docs/source/api.rst
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1410 2023-06-30 20:13:32.000000 pdpilot-0.5.1/docs/source/conf.py
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1336 2023-07-19 18:02:43.000000 pdpilot-0.5.1/docs/source/developer-installation.rst
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     2114 2023-06-30 20:13:32.000000 pdpilot-0.5.1/docs/source/index.rst
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1600 2023-06-30 20:13:32.000000 pdpilot-0.5.1/docs/source/installation.rst
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      506 2023-07-25 00:11:37.000000 pdpilot-0.5.1/docs/source/release.rst
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.816625 pdpilot-0.5.1/docs/source/screenshots/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)   339104 2023-06-30 20:13:32.000000 pdpilot-0.5.1/docs/source/screenshots/detailed-plot-one-way-clusters.png
--rw-r--r--   0 danielkerrigan   (501) staff       (20)   436887 2023-06-30 20:13:32.000000 pdpilot-0.5.1/docs/source/screenshots/detailed-plot-one-way-ground-truth.png
--rw-r--r--   0 danielkerrigan   (501) staff       (20)   361453 2023-06-30 20:13:32.000000 pdpilot-0.5.1/docs/source/screenshots/detailed-plot-two-way.png
--rw-r--r--   0 danielkerrigan   (501) staff       (20)   892581 2023-06-30 20:13:32.000000 pdpilot-0.5.1/docs/source/screenshots/one-way-plots.png
--rw-r--r--   0 danielkerrigan   (501) staff       (20)   358077 2023-06-30 20:13:32.000000 pdpilot-0.5.1/docs/source/screenshots/two-way-plots.png
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     7961 2023-06-30 20:13:32.000000 pdpilot-0.5.1/docs/source/ui.rst
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.818466 pdpilot-0.5.1/examples/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     7373 2023-07-19 21:09:14.000000 pdpilot-0.5.1/examples/bike-rentals-regression.ipynb
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     5568 2023-07-12 22:50:00.000000 pdpilot-0.5.1/examples/churn-classification.ipynb
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     7720 2023-06-30 20:13:32.000000 pdpilot-0.5.1/examples/colab-example.ipynb
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      175 2023-06-30 20:13:32.000000 pdpilot-0.5.1/install.json
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     3027 2023-07-25 00:52:56.000000 pdpilot-0.5.1/package.json
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.820520 pdpilot-0.5.1/pdpilot/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1838 2023-06-30 20:13:32.000000 pdpilot-0.5.1/pdpilot/__init__.py
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      153 2023-07-25 00:10:54.000000 pdpilot-0.5.1/pdpilot/_frontend.py
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      111 2023-07-25 00:11:08.000000 pdpilot-0.5.1/pdpilot/_version.py
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.821353 pdpilot-0.5.1/pdpilot/labextension/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     3143 2023-07-25 00:53:45.000000 pdpilot-0.5.1/pdpilot/labextension/package.json
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.822321 pdpilot-0.5.1/pdpilot/labextension/static/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)   290502 2023-07-25 00:53:45.000000 pdpilot-0.5.1/pdpilot/labextension/static/568.fc735409708fd22de78c.js
--rw-r--r--   0 danielkerrigan   (501) staff       (20)   186042 2023-07-25 00:53:45.000000 pdpilot-0.5.1/pdpilot/labextension/static/713.5fb1220914a3fc9b6db7.js
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      475 2023-07-25 00:53:45.000000 pdpilot-0.5.1/pdpilot/labextension/static/713.5fb1220914a3fc9b6db7.js.LICENSE.txt
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     7007 2023-07-25 00:53:45.000000 pdpilot-0.5.1/pdpilot/labextension/static/remoteEntry.7d03101ac0d410913165.js
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      118 2023-07-25 00:53:41.000000 pdpilot-0.5.1/pdpilot/labextension/static/style.js
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     7709 2023-07-25 00:53:45.000000 pdpilot-0.5.1/pdpilot/labextension/static/third-party-licenses.json
--rw-r--r--   0 danielkerrigan   (501) staff       (20)       95 2023-06-30 20:13:32.000000 pdpilot-0.5.1/pdpilot/logging.py
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     7936 2023-07-19 18:52:22.000000 pdpilot-0.5.1/pdpilot/metadata.py
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.822677 pdpilot-0.5.1/pdpilot/nbextension/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      362 2023-06-30 20:13:32.000000 pdpilot-0.5.1/pdpilot/nbextension/extension.js
--rw-r--r--   0 danielkerrigan   (501) staff       (20)   290582 2023-07-25 00:53:40.000000 pdpilot-0.5.1/pdpilot/nbextension/index.js
--rw-r--r--   0 danielkerrigan   (501) staff       (20)    21526 2023-07-21 02:10:50.000000 pdpilot-0.5.1/pdpilot/pdp.py
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      755 2023-06-30 20:13:32.000000 pdpilot-0.5.1/pdpilot/tqdm_joblib.py
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      372 2023-07-06 17:58:51.000000 pdpilot-0.5.1/pdpilot/utils.py
--rw-r--r--   0 danielkerrigan   (501) staff       (20)    10649 2023-07-21 01:34:49.000000 pdpilot-0.5.1/pdpilot/widget.py
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.821226 pdpilot-0.5.1/pdpilot.egg-info/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1574 2023-07-25 00:54:45.000000 pdpilot-0.5.1/pdpilot.egg-info/PKG-INFO
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     3183 2023-07-25 00:54:45.000000 pdpilot-0.5.1/pdpilot.egg-info/SOURCES.txt
--rw-r--r--   0 danielkerrigan   (501) staff       (20)        1 2023-07-25 00:54:45.000000 pdpilot-0.5.1/pdpilot.egg-info/dependency_links.txt
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      200 2023-07-25 00:54:45.000000 pdpilot-0.5.1/pdpilot.egg-info/requires.txt
--rw-r--r--   0 danielkerrigan   (501) staff       (20)        8 2023-07-25 00:54:45.000000 pdpilot-0.5.1/pdpilot.egg-info/top_level.txt
--rw-r--r--   0 danielkerrigan   (501) staff       (20)       61 2023-06-30 20:13:32.000000 pdpilot-0.5.1/pdpilot.json
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      153 2023-02-23 21:00:34.000000 pdpilot-0.5.1/pyproject.toml
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      187 2023-07-25 00:54:45.829200 pdpilot-0.5.1/setup.cfg
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     3078 2023-07-11 14:54:54.000000 pdpilot-0.5.1/setup.py
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.824169 pdpilot-0.5.1/src/
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.826242 pdpilot-0.5.1/src/components/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     6438 2023-07-13 03:58:39.000000 pdpilot-0.5.1/src/components/DetailedPlot.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     3466 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/FeatureKindFilter.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     2819 2023-07-14 14:19:36.000000 pdpilot-0.5.1/src/components/FeatureNameFilter.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     2681 2023-07-25 00:31:46.000000 pdpilot-0.5.1/src/components/InfoTooltip.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     6143 2023-07-13 03:59:02.000000 pdpilot-0.5.1/src/components/OneWayDetailedPlot.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      952 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/OneWayGridContainer.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     2963 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/OneWayGridFilters.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1607 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/PDP.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)    15455 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/PDPGrid.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1595 2023-07-13 13:18:02.000000 pdpilot-0.5.1/src/components/SegmentedButton.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1223 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/Tabs.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1245 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/ToggleHeader.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     3128 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/TwoWayDetailedPlot.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1417 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/TwoWayGridContainer.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     3137 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/TwoWayGridFilters.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     3527 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/Widget.svelte
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.807939 pdpilot-0.5.1/src/components/vis/
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.826641 pdpilot-0.5.1/src/components/vis/axis/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      978 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/axis/Label.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     3217 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/axis/XAxis.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     3422 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/axis/YAxis.svelte
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.826776 pdpilot-0.5.1/src/components/vis/distribution/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)    14072 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/distribution/Scatterplot.svelte
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.826911 pdpilot-0.5.1/src/components/vis/ice-clusters/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)    13593 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/ice-clusters/ClusterDescriptions.svelte
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.827181 pdpilot-0.5.1/src/components/vis/legends/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1646 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/legends/CategoricalColorLegend.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     3150 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/legends/QuantitativeColorLegend.svelte
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.827590 pdpilot-0.5.1/src/components/vis/marginal/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     2302 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/marginal/MarginalBarChart.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     2204 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/marginal/MarginalHistogram.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1219 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/marginal/MarginalPDP.svelte
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.828256 pdpilot-0.5.1/src/components/vis/one-way/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     3753 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/one-way/ClusterCenters.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)    16759 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/one-way/ClusterLines.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)    10574 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/one-way/FeatureVsLabels.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)    11146 2023-07-20 20:14:13.000000 pdpilot-0.5.1/src/components/vis/one-way/Lines.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1384 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/one-way/OneWayChart.svelte
-drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-25 00:54:45.828757 pdpilot-0.5.1/src/components/vis/two-way/
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     7200 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/two-way/FeatureVsFeature.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1122 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/two-way/TwoWayChart.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     7993 2023-07-19 18:02:51.000000 pdpilot-0.5.1/src/components/vis/two-way/TwoWayHeatmap.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     6797 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/components/vis/two-way/TwoWayLines.svelte
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     8243 2023-07-19 18:04:28.000000 pdpilot-0.5.1/src/drawing.ts
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      513 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/extension.ts
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      163 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/fast-kde.d.ts
--rw-r--r--   0 danielkerrigan   (501) staff       (20)       53 2022-09-20 18:55:54.000000 pdpilot-0.5.1/src/index.ts
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1030 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/plugin.ts
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     4804 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/sorting.ts
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     8855 2023-07-21 02:20:21.000000 pdpilot-0.5.1/src/stores.ts
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     4609 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/types.ts
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1718 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/utils.ts
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      481 2023-06-01 22:05:36.000000 pdpilot-0.5.1/src/version.ts
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     7282 2023-07-21 02:17:43.000000 pdpilot-0.5.1/src/vis-utils.ts
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     1766 2023-06-30 20:13:32.000000 pdpilot-0.5.1/src/widget.ts
--rw-r--r--   0 danielkerrigan   (501) staff       (20)      540 2023-07-15 15:06:52.000000 pdpilot-0.5.1/tsconfig.json
--rw-r--r--   0 danielkerrigan   (501) staff       (20)     3097 2023-07-25 00:46:46.000000 pdpilot-0.5.1/webpack.config.js
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.128179 pdpilot-0.5.2/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1499 2022-09-20 18:55:54.000000 pdpilot-0.5.2/LICENSE.txt
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      656 2023-06-30 20:13:32.000000 pdpilot-0.5.2/MANIFEST.in
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1574 2023-07-31 13:51:55.128250 pdpilot-0.5.2/PKG-INFO
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      449 2023-06-30 20:13:32.000000 pdpilot-0.5.2/README.md
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.110057 pdpilot-0.5.2/docs/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      637 2023-02-22 20:30:48.000000 pdpilot-0.5.2/docs/Makefile
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      132 2023-06-30 20:13:32.000000 pdpilot-0.5.2/docs/environment.yml
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      763 2022-12-02 20:03:10.000000 pdpilot-0.5.2/docs/make.bat
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.111602 pdpilot-0.5.2/docs/source/
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.111857 pdpilot-0.5.2/docs/source/_static/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)   291593 2023-07-31 13:51:10.000000 pdpilot-0.5.2/docs/source/_static/embed-bundle.js
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)       92 2023-06-30 20:13:32.000000 pdpilot-0.5.2/docs/source/api.rst
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1410 2023-06-30 20:13:32.000000 pdpilot-0.5.2/docs/source/conf.py
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1336 2023-07-19 18:02:43.000000 pdpilot-0.5.2/docs/source/developer-installation.rst
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     2114 2023-06-30 20:13:32.000000 pdpilot-0.5.2/docs/source/index.rst
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1600 2023-06-30 20:13:32.000000 pdpilot-0.5.2/docs/source/installation.rst
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      506 2023-07-31 13:49:28.000000 pdpilot-0.5.2/docs/source/release.rst
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.116309 pdpilot-0.5.2/docs/source/screenshots/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)   339104 2023-06-30 20:13:32.000000 pdpilot-0.5.2/docs/source/screenshots/detailed-plot-one-way-clusters.png
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)   436887 2023-06-30 20:13:32.000000 pdpilot-0.5.2/docs/source/screenshots/detailed-plot-one-way-ground-truth.png
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)   361453 2023-06-30 20:13:32.000000 pdpilot-0.5.2/docs/source/screenshots/detailed-plot-two-way.png
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)   892581 2023-06-30 20:13:32.000000 pdpilot-0.5.2/docs/source/screenshots/one-way-plots.png
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)   358077 2023-06-30 20:13:32.000000 pdpilot-0.5.2/docs/source/screenshots/two-way-plots.png
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     7975 2023-07-30 23:45:37.000000 pdpilot-0.5.2/docs/source/ui.rst
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.117831 pdpilot-0.5.2/examples/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     7373 2023-07-31 13:47:58.000000 pdpilot-0.5.2/examples/bike-rentals-regression.ipynb
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     5568 2023-07-31 13:47:48.000000 pdpilot-0.5.2/examples/churn-classification.ipynb
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     7720 2023-06-30 20:13:32.000000 pdpilot-0.5.2/examples/colab-example.ipynb
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      175 2023-06-30 20:13:32.000000 pdpilot-0.5.2/install.json
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     3027 2023-07-31 13:48:30.000000 pdpilot-0.5.2/package.json
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.119942 pdpilot-0.5.2/pdpilot/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1838 2023-06-30 20:13:32.000000 pdpilot-0.5.2/pdpilot/__init__.py
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      153 2023-07-31 13:48:47.000000 pdpilot-0.5.2/pdpilot/_frontend.py
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      111 2023-07-31 13:48:41.000000 pdpilot-0.5.2/pdpilot/_version.py
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.120777 pdpilot-0.5.2/pdpilot/labextension/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     3143 2023-07-31 13:51:15.000000 pdpilot-0.5.2/pdpilot/labextension/package.json
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.121757 pdpilot-0.5.2/pdpilot/labextension/static/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)   291617 2023-07-31 13:51:15.000000 pdpilot-0.5.2/pdpilot/labextension/static/568.be4561957748b400120d.js
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)   186042 2023-07-31 13:51:15.000000 pdpilot-0.5.2/pdpilot/labextension/static/713.5fb1220914a3fc9b6db7.js
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      475 2023-07-31 13:51:15.000000 pdpilot-0.5.2/pdpilot/labextension/static/713.5fb1220914a3fc9b6db7.js.LICENSE.txt
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     7007 2023-07-31 13:51:15.000000 pdpilot-0.5.2/pdpilot/labextension/static/remoteEntry.93d73cafbbe8e20d7f23.js
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      118 2023-07-31 13:51:12.000000 pdpilot-0.5.2/pdpilot/labextension/static/style.js
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     7709 2023-07-31 13:51:15.000000 pdpilot-0.5.2/pdpilot/labextension/static/third-party-licenses.json
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)       95 2023-06-30 20:13:32.000000 pdpilot-0.5.2/pdpilot/logging.py
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     7936 2023-07-19 18:52:22.000000 pdpilot-0.5.2/pdpilot/metadata.py
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.122092 pdpilot-0.5.2/pdpilot/nbextension/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      362 2023-06-30 20:13:32.000000 pdpilot-0.5.2/pdpilot/nbextension/extension.js
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)   291697 2023-07-31 13:51:11.000000 pdpilot-0.5.2/pdpilot/nbextension/index.js
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)    21526 2023-07-31 13:41:02.000000 pdpilot-0.5.2/pdpilot/pdp.py
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      755 2023-06-30 20:13:32.000000 pdpilot-0.5.2/pdpilot/tqdm_joblib.py
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      372 2023-07-06 17:58:51.000000 pdpilot-0.5.2/pdpilot/utils.py
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)    10649 2023-07-21 01:34:49.000000 pdpilot-0.5.2/pdpilot/widget.py
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.120661 pdpilot-0.5.2/pdpilot.egg-info/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1574 2023-07-31 13:51:55.000000 pdpilot-0.5.2/pdpilot.egg-info/PKG-INFO
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     3183 2023-07-31 13:51:55.000000 pdpilot-0.5.2/pdpilot.egg-info/SOURCES.txt
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)        1 2023-07-31 13:51:55.000000 pdpilot-0.5.2/pdpilot.egg-info/dependency_links.txt
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      200 2023-07-31 13:51:55.000000 pdpilot-0.5.2/pdpilot.egg-info/requires.txt
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)        8 2023-07-31 13:51:55.000000 pdpilot-0.5.2/pdpilot.egg-info/top_level.txt
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)       61 2023-06-30 20:13:32.000000 pdpilot-0.5.2/pdpilot.json
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      153 2023-02-23 21:00:34.000000 pdpilot-0.5.2/pyproject.toml
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      187 2023-07-31 13:51:55.128503 pdpilot-0.5.2/setup.cfg
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     3078 2023-07-11 14:54:54.000000 pdpilot-0.5.2/setup.py
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.123563 pdpilot-0.5.2/src/
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.125306 pdpilot-0.5.2/src/components/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     6438 2023-07-13 03:58:39.000000 pdpilot-0.5.2/src/components/DetailedPlot.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     3466 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/FeatureKindFilter.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     2819 2023-07-14 14:19:36.000000 pdpilot-0.5.2/src/components/FeatureNameFilter.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     2681 2023-07-30 23:50:56.000000 pdpilot-0.5.2/src/components/InfoTooltip.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     6143 2023-07-31 04:26:27.000000 pdpilot-0.5.2/src/components/OneWayDetailedPlot.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      952 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/OneWayGridContainer.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     2963 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/OneWayGridFilters.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1607 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/PDP.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)    15489 2023-07-31 12:00:16.000000 pdpilot-0.5.2/src/components/PDPGrid.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1595 2023-07-13 13:18:02.000000 pdpilot-0.5.2/src/components/SegmentedButton.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1223 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/Tabs.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1245 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/ToggleHeader.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     3128 2023-07-31 03:16:47.000000 pdpilot-0.5.2/src/components/TwoWayDetailedPlot.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1417 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/TwoWayGridContainer.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     3137 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/TwoWayGridFilters.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     3527 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/Widget.svelte
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.107896 pdpilot-0.5.2/src/components/vis/
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.125670 pdpilot-0.5.2/src/components/vis/axis/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      978 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/vis/axis/Label.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     3217 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/vis/axis/XAxis.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     3422 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/vis/axis/YAxis.svelte
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.125805 pdpilot-0.5.2/src/components/vis/distribution/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)    14072 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/vis/distribution/Scatterplot.svelte
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.125938 pdpilot-0.5.2/src/components/vis/ice-clusters/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)    13593 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/vis/ice-clusters/ClusterDescriptions.svelte
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.126231 pdpilot-0.5.2/src/components/vis/legends/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1646 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/vis/legends/CategoricalColorLegend.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     3150 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/vis/legends/QuantitativeColorLegend.svelte
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.126680 pdpilot-0.5.2/src/components/vis/marginal/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     2302 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/vis/marginal/MarginalBarChart.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     2204 2023-07-30 23:27:51.000000 pdpilot-0.5.2/src/components/vis/marginal/MarginalHistogram.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1557 2023-07-31 11:58:45.000000 pdpilot-0.5.2/src/components/vis/marginal/MarginalPDP.svelte
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.127487 pdpilot-0.5.2/src/components/vis/one-way/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     3753 2023-07-31 03:15:21.000000 pdpilot-0.5.2/src/components/vis/one-way/ClusterCenters.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)    16759 2023-07-31 03:15:26.000000 pdpilot-0.5.2/src/components/vis/one-way/ClusterLines.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)    10574 2023-07-31 03:17:00.000000 pdpilot-0.5.2/src/components/vis/one-way/FeatureVsLabels.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)    11146 2023-07-31 03:53:55.000000 pdpilot-0.5.2/src/components/vis/one-way/Lines.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1384 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/vis/one-way/OneWayChart.svelte
+drwxr-xr-x   0 danielkerrigan   (501) staff       (20)        0 2023-07-31 13:51:55.128053 pdpilot-0.5.2/src/components/vis/two-way/
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     7200 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/vis/two-way/FeatureVsFeature.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1122 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/vis/two-way/TwoWayChart.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     7993 2023-07-31 13:22:49.000000 pdpilot-0.5.2/src/components/vis/two-way/TwoWayHeatmap.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     6797 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/components/vis/two-way/TwoWayLines.svelte
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     8243 2023-07-31 03:48:06.000000 pdpilot-0.5.2/src/drawing.ts
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      513 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/extension.ts
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      163 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/fast-kde.d.ts
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)       53 2022-09-20 18:55:54.000000 pdpilot-0.5.2/src/index.ts
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1030 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/plugin.ts
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     4819 2023-07-31 13:41:00.000000 pdpilot-0.5.2/src/sorting.ts
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     8855 2023-07-21 02:20:21.000000 pdpilot-0.5.2/src/stores.ts
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     4609 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/types.ts
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1718 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/utils.ts
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      481 2023-06-01 22:05:36.000000 pdpilot-0.5.2/src/version.ts
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     7282 2023-07-31 12:42:42.000000 pdpilot-0.5.2/src/vis-utils.ts
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     1766 2023-06-30 20:13:32.000000 pdpilot-0.5.2/src/widget.ts
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)      540 2023-07-15 15:06:52.000000 pdpilot-0.5.2/tsconfig.json
+-rw-r--r--   0 danielkerrigan   (501) staff       (20)     3097 2023-07-25 00:46:46.000000 pdpilot-0.5.2/webpack.config.js
```

### Comparing `pdpilot-0.5.1/LICENSE.txt` & `pdpilot-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/MANIFEST.in` & `pdpilot-0.5.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/PKG-INFO` & `pdpilot-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdpilot
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Jupyter widget for exploring PDP and ICE plots.
 Home-page: https://github.com/DanielKerrigan/PDPilot
 Author: Daniel Kerrigan
 Author-email: kerrigan.d@northeastern.edu
 License: BSD
 Keywords: Jupyter,Widgets,IPython,PDP,ICE
 Platform: Linux
```

### Comparing `pdpilot-0.5.1/docs/Makefile` & `pdpilot-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/docs/make.bat` & `pdpilot-0.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/docs/source/_static/embed-bundle.js` & `pdpilot-0.5.2/docs/source/_static/embed-bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -453,15 +453,15 @@
             },
             146: e => {
                 "use strict";
                 e.exports = t
             },
             147: t => {
                 "use strict";
-                t.exports = JSON.parse('{"name":"pdpilot","version":"0.5.1","description":"A Jupyter widget for exploring PDP and ICE plots.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/DanielKerrigan/PDPilot","bugs":{"url":"https://github.com/DanielKerrigan/PDPilot/issues"},"license":"BSD-3-Clause","author":{"name":"Daniel Kerrigan","email":"kerrigan.d@northeastern.edu"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/DanielKerrigan/PDPilot"},"scripts":{"build":"webpack --mode=development && jupyter labextension build --development=True .","build:prod":"webpack --mode=production && jupyter labextension build .","clean":"npm run clean:lib && npm run clean:nbextension && npm run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf pdpilot/labextension","clean:nbextension":"rimraf pdpilot/nbextension/static/index.js","fix":"prettier --plugin-search-dir . --write src && eslint . --ext .ts,.tsx,.svelte --fix","check":"prettier --plugin-search-dir . --check src && eslint . --ext .ts,.tsx,.svelte && svelte-check","prepack":"npm run build:prod","watch":"npm run watch:nbextension","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch .","test":"uvu -r tsm tests"},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","d3":"^7.8.5","fast-kde":"^0.2.1","lodash.clonedeep":"^4.5.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3 || ^4","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@tsconfig/svelte":"^5.0.0","@types/d3":"^7.4.0","@types/lodash.clonedeep":"^4.5.7","@types/node":"^20.2.5","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.45.0","@typescript-eslint/parser":"^5.45.0","acorn":"^7.2.0","css-loader":"^6.7.0","eslint":"^8.28.0","eslint-config-prettier":"^8.5.0","eslint-plugin-svelte":"^2.30.0","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.8.0","prettier-plugin-svelte":"^2.10.1","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^3.0.0","svelte":"^4.0.0","svelte-check":"^3.4.6","svelte-loader":"^3.1.8","svelte-preprocess":"^5.0.4","ts-loader":"^9.0.0","tslib":"^2.4.1","tsm":"^2.2.1","typescript":"^5.1.6","uvu":"^0.5.3","webpack":">=5.76.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":true,"outputDir":"pdpilot/labextension/"}}')
+                t.exports = JSON.parse('{"name":"pdpilot","version":"0.5.2","description":"A Jupyter widget for exploring PDP and ICE plots.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/DanielKerrigan/PDPilot","bugs":{"url":"https://github.com/DanielKerrigan/PDPilot/issues"},"license":"BSD-3-Clause","author":{"name":"Daniel Kerrigan","email":"kerrigan.d@northeastern.edu"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/DanielKerrigan/PDPilot"},"scripts":{"build":"webpack --mode=development && jupyter labextension build --development=True .","build:prod":"webpack --mode=production && jupyter labextension build .","clean":"npm run clean:lib && npm run clean:nbextension && npm run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf pdpilot/labextension","clean:nbextension":"rimraf pdpilot/nbextension/static/index.js","fix":"prettier --plugin-search-dir . --write src && eslint . --ext .ts,.tsx,.svelte --fix","check":"prettier --plugin-search-dir . --check src && eslint . --ext .ts,.tsx,.svelte && svelte-check","prepack":"npm run build:prod","watch":"npm run watch:nbextension","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch .","test":"uvu -r tsm tests"},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","d3":"^7.8.5","fast-kde":"^0.2.1","lodash.clonedeep":"^4.5.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3 || ^4","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@tsconfig/svelte":"^5.0.0","@types/d3":"^7.4.0","@types/lodash.clonedeep":"^4.5.7","@types/node":"^20.2.5","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.45.0","@typescript-eslint/parser":"^5.45.0","acorn":"^7.2.0","css-loader":"^6.7.0","eslint":"^8.28.0","eslint-config-prettier":"^8.5.0","eslint-plugin-svelte":"^2.30.0","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.8.0","prettier-plugin-svelte":"^2.10.1","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^3.0.0","svelte":"^4.0.0","svelte-check":"^3.4.6","svelte-loader":"^3.1.8","svelte-preprocess":"^5.0.4","ts-loader":"^9.0.0","tslib":"^2.4.1","tsm":"^2.2.1","typescript":"^5.1.6","uvu":"^0.5.3","webpack":">=5.76.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":true,"outputDir":"pdpilot/labextension/"}}')
             }
         },
         n = {};
 
     function r(t) {
         var i = n[t];
         if (void 0 !== i) return i.exports;
@@ -498,16 +498,16 @@
     }, r.nmd = t => (t.paths = [], t.children || (t.children = []), t);
     var i = {};
     return (() => {
         "use strict";
         r.r(i), r.d(i, {
             MODULE_NAME: () => n,
             MODULE_VERSION: () => e,
-            PDPilotModel: () => Zf,
-            PDPilotView: () => Qf
+            PDPilotModel: () => eh,
+            PDPilotView: () => nh
         });
         const t = r(147),
             e = t.version,
             n = t.name;
         var o = r(146);
         new Set;
         const l = "undefined" != typeof window ? window : "undefined" != typeof globalThis ? globalThis : global;
@@ -6259,15 +6259,15 @@
 
         function Ls(t) {
             let e, n, r, i, o, l, a, s, u, h, p, v, b = t[62].filteredIndices.length + "";
             return a = new Va({
                 props: {
                     scale: t[12],
                     x: t[25].left,
-                    label: "centered prediction"
+                    label: "Centered prediction"
                 }
             }), s = new Ma({
                 props: {
                     scale: t[13],
                     y: t[11] - t[25].bottom,
                     showTickLabels: t[62].id === t[16][t[16].length - 1],
                     showAxisLabel: t[62].id === t[16][t[16].length - 1],
@@ -6788,15 +6788,15 @@
                     integerOnly: "discrete" === t[9].subkind,
                     value_map: "value_map" in t[9] ? t[9].value_map : {}
                 }
             }), l = new Va({
                 props: {
                     scale: t[5],
                     x: t[7].left,
-                    label: "centered prediction"
+                    label: "Centered prediction"
                 }
             });
             let h = t[3] && Is(t);
             return {
                 c() {
                     e = g("svg"), s && s.c(), n = g("path"), u && u.c(), i = b(), bt(o.$$.fragment), bt(l.$$.fragment), h && h.c(), $(n, "d", r = t[11](t[0].ice.centered_pdp)), $(n, "stroke", "var(--black)"), $(n, "stroke-width", "2"), $(n, "fill", "none"), $(e, "width", t[1]), $(e, "height", t[2])
                 },
@@ -7117,15 +7117,15 @@
                     integerOnly: "discrete" === t[11].subkind,
                     value_map: "value_map" in t[11] ? t[11].value_map : {}
                 }
             }), a = new Va({
                 props: {
                     scale: t[13],
                     x: t[12].left,
-                    label: t[7] ? "centered prediction" : "prediction"
+                    label: t[7] ? "Centered prediction" : "Prediction"
                 }
             });
             let h = t[3] && Ks(t),
                 m = t[6] && t[18] === t[0].x_feature && Zs(t);
             return {
                 c() {
                     e = p("div"), n = p("canvas"), r = v(), i = g("svg"), o = g("g"), bt(l.$$.fragment), bt(a.$$.fragment), h && h.c(), s = b(), m && m.c(), $(n, "class", "svelte-hmor8t"), $(i, "width", t[1]), $(i, "height", t[2]), $(i, "class", "svelte-hmor8t"), $(e, "class", "pdpilot-plot-container svelte-hmor8t")
@@ -7133,15 +7133,15 @@
                 m(f, p) {
                     d(f, e, p), c(e, n), t[41](n), c(e, r), c(e, i), c(i, o), yt(l, o, null), yt(a, o, null), h && h.m(o, null), c(o, s), m && m.m(o, null), t[42](o), u = !0
                 },
                 p(t, e) {
                     const n = {};
                     16384 & e[0] && (n.scale = t[14]), 4100 & e[0] && (n.y = t[2] - t[12].bottom), 1 & e[0] && (n.label = t[0].x_feature), 2048 & e[0] && (n.integerOnly = "discrete" === t[11].subkind), 2048 & e[0] && (n.value_map = "value_map" in t[11] ? t[11].value_map : {}), l.$set(n);
                     const r = {};
-                    8192 & e[0] && (r.scale = t[13]), 4096 & e[0] && (r.x = t[12].left), 128 & e[0] && (r.label = t[7] ? "centered prediction" : "prediction"), a.$set(r), t[3] ? h ? (h.p(t, e), 8 & e[0] && dt(h, 1)) : (h = Ks(t), h.c(), dt(h, 1), h.m(o, s)) : h && (ct(), ft(h, 1, 1, (() => {
+                    8192 & e[0] && (r.scale = t[13]), 4096 & e[0] && (r.x = t[12].left), 128 & e[0] && (r.label = t[7] ? "Centered prediction" : "Prediction"), a.$set(r), t[3] ? h ? (h.p(t, e), 8 & e[0] && dt(h, 1)) : (h = Ks(t), h.c(), dt(h, 1), h.m(o, s)) : h && (ct(), ft(h, 1, 1, (() => {
                         h = null
                     })), ut()), t[6] && t[18] === t[0].x_feature ? m ? m.p(t, e) : (m = Zs(t), m.c(), m.m(o, null)) : m && (m.d(1), m = null), (!u || 2 & e[0]) && $(i, "width", t[1]), (!u || 4 & e[0]) && $(i, "height", t[2])
                 },
                 i(t) {
                     u || (dt(l.$$.fragment, t), dt(a.$$.fragment, t), dt(h), u = !0)
                 },
                 o(t) {
@@ -7573,15 +7573,15 @@
                         c = on().domain([0, 1]).range([0, n.bandwidth()]);
                     for (let d = 0; d < i.length; d++) {
                         const p = s(a[d].x),
                             g = c(a[d].y);
                         t.strokeStyle = r(l[d]), t.beginPath(), t.arc((null !== (f = e(i[d])) && void 0 !== f ? f : 0) + p, (null !== (h = n(o[d])) && void 0 !== h ? h : 0) + g, u, 0, 2 * Math.PI), t.stroke()
                     }
                 } else if ("bandwidth" in e && !("bandwidth" in n))
-                    if (e.bandwidth() >= 40) $n(Ln(i, o, l), (t => t[0])).forEach((([i, o]) => {
+                    if (e.bandwidth() >= 20) $n(Ln(i, o, l), (t => t[0])).forEach((([i, o]) => {
                         var l, a;
                         t.translate(null !== (l = e(i)) && void 0 !== l ? l : 0, 0),
                             function(t, e, n, r, i, o, l, a, s) {
                                 var c;
                                 if (!e) return;
                                 const u = on().domain([0, null !== (c = sc(t.densities, (t => t.density))) && void 0 !== c ? c : 0]).range([r / 2 - 2, 0]),
                                     d = cc().x0((t => {
@@ -7595,15 +7595,15 @@
                                     e.beginPath(), e.strokeStyle = "function" == typeof s ? s(i) : s, e.moveTo(r / 2 + 2, n(t)), e.lineTo(r, n(t)), e.stroke()
                                 })), e.globalAlpha = 1, e.fillStyle = "black", e.strokeStyle = "white", e.beginPath(), e.arc(r / 2, n(t.mean), 5, 0, 2 * Math.PI), e.fill(), e.stroke(), e.restore()
                             }(Fn(o.map((t => t[1])), o.map((t => t[2]))), t, n, e.bandwidth(), c, d, 0, 0, r), t.translate(-(null !== (a = e(i)) && void 0 !== a ? a : 0), 0)
                     }));
                     else
                         for (let a = 0; a < i.length; a++) t.strokeStyle = r(l[a]), t.beginPath(), t.moveTo(null !== (p = e(i[a])) && void 0 !== p ? p : 0, n(o[a])), t.lineTo((null !== (g = e(i[a])) && void 0 !== g ? g : 0) + e.bandwidth(), n(o[a])), t.stroke();
                 else if (!("bandwidth" in e) && "bandwidth" in n)
-                    if (n.bandwidth() >= 40) $n(Ln(i, o, l), (t => t[1])).forEach((([i, o]) => {
+                    if (n.bandwidth() >= 20) $n(Ln(i, o, l), (t => t[1])).forEach((([i, o]) => {
                         var l, a;
                         t.translate(0, null !== (l = n(i)) && void 0 !== l ? l : 0), fc(Fn(o.map((t => t[0])), o.map((t => t[2]))), t, e, s, n.bandwidth(), d, "rgb(145, 145, 145)", "black", r), t.translate(0, -(null !== (a = n(i)) && void 0 !== a ? a : 0))
                     }));
                     else
                         for (let a = 0; a < i.length; a++) t.strokeStyle = r(l[a]), t.beginPath(), t.moveTo(e(i[a]), null !== (m = n(o[a])) && void 0 !== m ? m : 0), t.lineTo(e(i[a]), (null !== (v = n(o[a])) && void 0 !== v ? v : 0) + n.bandwidth()), t.stroke();
                 else if (!("bandwidth" in e) && !("bandwidth" in n)) {
                     t.globalAlpha = d;
@@ -7760,86 +7760,139 @@
                     marginRight: 10,
                     marginLeft: 11,
                     title: 2
                 }, hc)
             }
         };
 
-        function xc(t) {
-            let e, n, r, i;
+        function xc(t, e, n) {
+            const r = t.slice();
+            return r[13] = e[n], r
+        }
+
+        function _c(t) {
+            let e, n = ht(t[8]),
+                r = [];
+            for (let e = 0; e < n.length; e += 1) r[e] = kc(xc(t, n, e));
             return {
                 c() {
-                    e = g("g"), n = g("path"), $(n, "d", r = t[2](t[3])), $(n, "stroke", t[1]), $(n, "fill", "none"), $(e, "transform", i = "translate(" + t[0] + ")")
+                    for (let t = 0; t < r.length; t += 1) r[t].c();
+                    e = b()
+                },
+                m(t, n) {
+                    for (let e = 0; e < r.length; e += 1) r[e] && r[e].m(t, n);
+                    d(t, e, n)
+                },
+                p(t, i) {
+                    if (377 & i) {
+                        let o;
+                        for (n = ht(t[8]), o = 0; o < n.length; o += 1) {
+                            const l = xc(t, n, o);
+                            r[o] ? r[o].p(l, i) : (r[o] = kc(l), r[o].c(), r[o].m(e.parentNode, e))
+                        }
+                        for (; o < r.length; o += 1) r[o].d(1);
+                        r.length = n.length
+                    }
+                },
+                d(t) {
+                    t && f(e), h(r, t)
+                }
+            }
+        }
+
+        function kc(t) {
+            let e, n, r;
+            return {
+                c() {
+                    e = g("circle"), $(e, "cx", n = "horizontal" === t[0] ? t[4](t[13]) : t[5](t[13])), $(e, "cy", r = "horizontal" === t[0] ? t[5](t[13]) : t[4](t[13])), $(e, "r", t[6]), $(e, "fill", t[3])
+                },
+                m(t, n) {
+                    d(t, e, n)
+                },
+                p(t, i) {
+                    305 & i && n !== (n = "horizontal" === t[0] ? t[4](t[13]) : t[5](t[13])) && $(e, "cx", n), 305 & i && r !== (r = "horizontal" === t[0] ? t[5](t[13]) : t[4](t[13])) && $(e, "cy", r), 64 & i && $(e, "r", t[6]), 8 & i && $(e, "fill", t[3])
+                },
+                d(t) {
+                    t && f(e)
+                }
+            }
+        }
+
+        function Mc(t) {
+            let e, n, r, i, o = "bandwidth" in t[1] && _c(t);
+            return {
+                c() {
+                    e = g("g"), n = g("path"), o && o.c(), $(n, "d", r = t[7](t[8])), $(n, "stroke", t[3]), $(n, "fill", "none"), $(e, "transform", i = "translate(" + t[2] + ")")
                 },
                 m(t, r) {
-                    d(t, e, r), c(e, n)
+                    d(t, e, r), c(e, n), o && o.m(e, null)
                 },
-                p(t, [o]) {
-                    12 & o && r !== (r = t[2](t[3])) && $(n, "d", r), 2 & o && $(n, "stroke", t[1]), 1 & o && i !== (i = "translate(" + t[0] + ")") && $(e, "transform", i)
+                p(t, [l]) {
+                    384 & l && r !== (r = t[7](t[8])) && $(n, "d", r), 8 & l && $(n, "stroke", t[3]), "bandwidth" in t[1] ? o ? o.p(t, l) : (o = _c(t), o.c(), o.m(e, null)) : o && (o.d(1), o = null), 4 & l && i !== (i = "translate(" + t[2] + ")") && $(e, "transform", i)
                 },
                 i: T,
                 o: T,
                 d(t) {
-                    t && f(e)
+                    t && f(e), o && o.d()
                 }
             }
         }
 
-        function _c(t, e, n) {
-            let r, i, o, l, a, s;
-            E(t, ar, (t => n(11, s = t)));
+        function Lc(t, e, n) {
+            let r, i, o, l, a, s, c;
+            E(t, ar, (t => n(12, c = t)));
             let {
-                pd: c
+                pd: u
             } = e, {
-                height: u
+                height: d
             } = e, {
-                direction: d
+                direction: f
             } = e, {
-                x: f
+                x: h
             } = e, {
-                translate: h = [0, 0]
+                translate: p = [0, 0]
             } = e, {
-                stroke: p = "black"
+                stroke: g = "black"
             } = e;
             return t.$$set = t => {
-                "pd" in t && n(4, c = t.pd), "height" in t && n(5, u = t.height), "direction" in t && n(6, d = t.direction), "x" in t && n(7, f = t.x), "translate" in t && n(0, h = t.translate), "stroke" in t && n(1, p = t.stroke)
+                "pd" in t && n(9, u = t.pd), "height" in t && n(10, d = t.height), "direction" in t && n(0, f = t.direction), "x" in t && n(1, h = t.x), "translate" in t && n(2, p = t.translate), "stroke" in t && n(3, g = t.stroke)
             }, t.$$.update = () => {
-                16 & t.$$.dirty && n(3, r = _n(c.x_values.length)), 2144 & t.$$.dirty && n(10, i = on().domain(s).range("horizontal" === d ? [u, 0] : [0, u])), 144 & t.$$.dirty && n(8, o = t => {
+                512 & t.$$.dirty && n(8, r = _n(u.x_values.length)), 5121 & t.$$.dirty && n(11, i = on().domain(c).range("horizontal" === f ? [d, 0] : [0, d])), 514 & t.$$.dirty && n(4, o = t => {
                     var e;
-                    return "bandwidth" in f ? (null !== (e = f(c.x_values[t])) && void 0 !== e ? e : 0) + f.bandwidth() / 2 : f(c.x_values[t])
-                }), 1040 & t.$$.dirty && n(9, l = t => i(c.mean_predictions[t])), 832 & t.$$.dirty && n(2, a = ei().x("horizontal" === d ? o : l).y("horizontal" === d ? l : o))
-            }, [h, p, a, r, c, u, d, f, o, l, i, s]
+                    return "bandwidth" in h ? (null !== (e = h(u.x_values[t])) && void 0 !== e ? e : 0) + h.bandwidth() / 2 : h(u.x_values[t])
+                }), 2560 & t.$$.dirty && n(5, l = t => i(u.mean_predictions[t])), 49 & t.$$.dirty && n(7, a = ei().x("horizontal" === f ? o : l).y("horizontal" === f ? l : o)), 2 & t.$$.dirty && n(6, s = "bandwidth" in h ? Math.min(2, h.bandwidth() / 2) : 0)
+            }, [f, h, p, g, o, l, s, a, r, u, d, i, c]
         }
-        const kc = class extends _t {
+        const Ac = class extends _t {
             constructor(t) {
-                super(), wt(this, t, _c, xc, j, {
-                    pd: 4,
-                    height: 5,
-                    direction: 6,
-                    x: 7,
-                    translate: 0,
-                    stroke: 1
+                super(), wt(this, t, Lc, Mc, j, {
+                    pd: 9,
+                    height: 10,
+                    direction: 0,
+                    x: 1,
+                    translate: 2,
+                    stroke: 3
                 })
             }
         };
 
-        function Mc(t) {
+        function Pc(t) {
             u(t, "svelte-crr1ai", ".two-way-container.svelte-crr1ai{position:relative;width:100%;height:100%}svg.svelte-crr1ai,canvas.svelte-crr1ai{position:absolute;top:var(--top);left:0}")
         }
 
-        function Lc(t) {
+        function Sc(t) {
             let e, n, r, i = t[12].left - t[21] + "px",
                 o = `${t[15]}px`;
             return n = new wc({
                 props: {
                     width: t[17] + t[20],
                     height: t[16],
                     color: t[8],
-                    marginLeft: Oc,
-                    marginRight: Oc,
+                    marginLeft: Bc,
+                    marginRight: Bc,
                     title: t[4]
                 }
             }), {
                 c() {
                     e = p("div"), bt(n.$$.fragment), M(e, "margin-left", i), M(e, "padding-top", o)
                 },
                 m(t, i) {
@@ -7857,25 +7910,25 @@
                 },
                 d(t) {
                     t && f(e), $t(n)
                 }
             }
         }
 
-        function Ac(t) {
+        function zc(t) {
             let e, n, r;
-            return e = new kc({
+            return e = new Ac({
                 props: {
                     pd: t[19],
                     height: t[6],
                     direction: "horizontal",
                     x: t[10],
                     translate: [0, t[12].top - t[6]]
                 }
-            }), n = new kc({
+            }), n = new Ac({
                 props: {
                     pd: t[18],
                     height: t[6],
                     direction: "vertical",
                     x: t[9],
                     translate: [t[1] - t[12].right, 0]
                 }
@@ -7900,24 +7953,24 @@
                 },
                 d(t) {
                     $t(e, t), $t(n, t)
                 }
             }
         }
 
-        function Pc(t) {
+        function Tc(t) {
             let e, n, r, i, o, l, a;
-            const s = [zc, Sc],
+            const s = [Cc, Nc],
                 c = [];
 
             function u(t, e) {
                 return "bandwidth" in t[10] ? 0 : 1
             }
             e = u(t), n = c[e] = s[e](t);
-            const h = [Nc, Tc],
+            const h = [Dc, Oc],
                 p = [];
 
             function g(t, e) {
                 return "bandwidth" in t[9] ? 0 : 1
             }
             return i = g(t), o = p[i] = h[i](t), {
                 c() {
@@ -7944,15 +7997,15 @@
                 },
                 d(t) {
                     t && (f(r), f(l)), c[e].d(t), p[i].d(t)
                 }
             }
         }
 
-        function Sc(t) {
+        function Nc(t) {
             let e, n;
             return e = new Qa({
                 props: {
                     data: t[14].distribution,
                     x: t[10],
                     height: t[6],
                     direction: "horizontal",
@@ -7977,15 +8030,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function zc(t) {
+        function Cc(t) {
             let e, n;
             return e = new ds({
                 props: {
                     data: t[14].distribution,
                     x: t[10],
                     height: t[6],
                     direction: "horizontal",
@@ -8010,15 +8063,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Tc(t) {
+        function Oc(t) {
             let e, n;
             return e = new Qa({
                 props: {
                     data: t[13].distribution,
                     x: t[9],
                     height: t[6],
                     direction: "vertical",
@@ -8043,15 +8096,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Nc(t) {
+        function Dc(t) {
             let e, n;
             return e = new ds({
                 props: {
                     data: t[13].distribution,
                     x: t[9],
                     height: t[6],
                     direction: "vertical",
@@ -8076,17 +8129,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Cc(t) {
+        function jc(t) {
             let e, n, r, i, o, l, a, s, u, h, m = `${t[16]+t[15]}px`,
-                b = t[5] && Lc(t);
+                b = t[5] && Sc(t);
             l = new Ma({
                 props: {
                     scale: t[10],
                     y: t[11] - t[12].bottom,
                     label: t[0].x_feature,
                     integerOnly: "discrete" === t[14].subkind,
                     value_map: "value_map" in t[14] ? t[14].value_map : {}
@@ -8096,29 +8149,29 @@
                     scale: t[9],
                     x: t[12].left,
                     label: t[0].y_feature,
                     integerOnly: "discrete" === t[13].subkind,
                     value_map: "value_map" in t[13] ? t[13].value_map : {}
                 }
             });
-            const y = [Pc, Ac],
+            const y = [Tc, zc],
                 w = [];
 
             function x(t, e) {
                 return t[2] ? 0 : t[3] && t[19] && t[18] ? 1 : -1
             }
             return ~(s = x(t)) && (u = w[s] = y[s](t)), {
                 c() {
                     e = p("div"), b && b.c(), n = v(), r = p("canvas"), i = v(), o = g("svg"), bt(l.$$.fragment), bt(a.$$.fragment), u && u.c(), $(r, "class", "svelte-crr1ai"), $(o, "width", t[1]), $(o, "height", t[11]), $(o, "class", "svelte-crr1ai"), $(e, "class", "two-way-container svelte-crr1ai"), M(e, "--top", m)
                 },
                 m(u, f) {
                     d(u, e, f), b && b.m(e, null), c(e, n), c(e, r), t[51](r), c(e, i), c(e, o), yt(l, o, null), yt(a, o, null), ~s && w[s].m(o, null), h = !0
                 },
                 p(t, r) {
-                    t[5] ? b ? (b.p(t, r), 32 & r[0] && dt(b, 1)) : (b = Lc(t), b.c(), dt(b, 1), b.m(e, n)) : b && (ct(), ft(b, 1, 1, (() => {
+                    t[5] ? b ? (b.p(t, r), 32 & r[0] && dt(b, 1)) : (b = Sc(t), b.c(), dt(b, 1), b.m(e, n)) : b && (ct(), ft(b, 1, 1, (() => {
                         b = null
                     })), ut());
                     const i = {};
                     1024 & r[0] && (i.scale = t[10]), 6144 & r[0] && (i.y = t[11] - t[12].bottom), 1 & r[0] && (i.label = t[0].x_feature), 16384 & r[0] && (i.integerOnly = "discrete" === t[14].subkind), 16384 & r[0] && (i.value_map = "value_map" in t[14] ? t[14].value_map : {}), l.$set(i);
                     const c = {};
                     512 & r[0] && (c.scale = t[9]), 4096 & r[0] && (c.x = t[12].left), 1 & r[0] && (c.label = t[0].y_feature), 8192 & r[0] && (c.integerOnly = "discrete" === t[13].subkind), 8192 & r[0] && (c.value_map = "value_map" in t[13] ? t[13].value_map : {}), a.$set(c);
                     let d = s;
@@ -8133,17 +8186,17 @@
                     ft(b), ft(l.$$.fragment, t), ft(a.$$.fragment, t), ft(u), h = !1
                 },
                 d(n) {
                     n && f(e), b && b.d(), t[51](null), $t(l), $t(a), ~s && w[s].d()
                 }
             }
         }
-        const Oc = 10;
+        const Bc = 10;
 
-        function Dc(t, e, n) {
+        function Ec(t, e, n) {
             let r, i, o, l, a, s, c, u, d, f, h, p, g, m, v, b, y, $, w, x, _, k, M, L, A, P, S, z, T;
             var N, C, O, D, j, B, I, R;
             E(t, mr, (t => n(47, P = t))), E(t, Sr, (t => n(48, S = t))), E(t, zr, (t => n(49, z = t))), E(t, Zn, (t => n(50, T = t)));
             let V, H, {
                     pd: q
                 } = e,
                 {
@@ -8190,66 +8243,66 @@
                     bottom: 35,
                     left: 50
                 }), 4259842 & t.$$.dirty[0] | 16384 & t.$$.dirty[1] && n(17, o = Math.min(W - i.left - i.right, K - r - i.top - i.bottom)), 131074 & t.$$.dirty[0] | 16384 & t.$$.dirty[1] && n(44, l = (W - o - i.left - i.right) / 2), 4390912 & t.$$.dirty[0] | 16384 & t.$$.dirty[1] && n(46, a = (K - r - o - i.top - i.bottom) / 2), 32 & t.$$.dirty[0] | 32768 & t.$$.dirty[1] && n(15, s = Q ? a : 0), 32768 & t.$$.dirty[0] | 57344 & t.$$.dirty[1] && n(12, c = {
                     top: i.top + a - s,
                     right: i.right + l,
                     bottom: i.bottom + a,
                     left: i.left + l
-                }), 4292608 & t.$$.dirty[0] && n(11, u = K - r - s), 1 & t.$$.dirty[0] | 524288 & t.$$.dirty[1] && n(14, d = T[q.x_feature]), 1 & t.$$.dirty[0] | 524288 & t.$$.dirty[1] && n(13, f = T[q.y_feature]), 1 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(42, h = S.copy().domain([q.pdp_min, q.pdp_max])), 1 & t.$$.dirty[0] | 262144 & t.$$.dirty[1] && n(43, p = z.copy().domain([q.interaction_min, 0, q.interaction_max])), 25165824 & t.$$.dirty[0] | 399360 & t.$$.dirty[1] && n(8, g = "interactions" === J ? U ? p : z : U ? h : S), 1 & t.$$.dirty[0] && n(37, m = Wn(q.x_axis)), 1 & t.$$.dirty[0] && n(36, v = Wn(q.y_axis)), 402653185 & t.$$.dirty[0] | 64 & t.$$.dirty[1] && n(41, b = q.x_axis[0] - (null !== n(28, C = null === n(27, N = m.get(q.x_axis[0])) || void 0 === N ? void 0 : N.before) && void 0 !== C ? C : 0)), 1610612737 & t.$$.dirty[0] | 64 & t.$$.dirty[1] && n(40, y = q.x_axis[q.x_axis.length - 1] + (null !== n(30, D = null === n(29, O = m.get(q.x_axis[q.x_axis.length - 1])) || void 0 === O ? void 0 : O.after) && void 0 !== D ? D : 0)), 1 & t.$$.dirty[0] | 35 & t.$$.dirty[1] && n(39, $ = q.y_axis[0] - (null !== n(32, B = null === n(31, j = v.get(q.y_axis[0])) || void 0 === j ? void 0 : j.before) && void 0 !== B ? B : 0)), 1 & t.$$.dirty[0] | 44 & t.$$.dirty[1] && n(38, w = q.y_axis[q.y_axis.length - 1] + (null !== n(34, R = null === n(33, I = v.get(q.y_axis[q.y_axis.length - 1])) || void 0 === I ? void 0 : I.after) && void 0 !== R ? R : 0)), 20483 & t.$$.dirty[0] | 1536 & t.$$.dirty[1] && n(10, x = "quantitative" === d.kind ? on().domain([b, y]).range([c.left, W - c.right]) : Ir().domain(q.x_axis).range([c.left, W - c.right])), 14337 & t.$$.dirty[0] | 384 & t.$$.dirty[1] && n(9, _ = "quantitative" === f.kind ? on().domain([$, w]).range([u - c.bottom, c.top]) : Ir().domain(q.y_axis).range([u - c.bottom, c.top])), 2178 & t.$$.dirty[0] | 16 & t.$$.dirty[1] && H && (En(V, H, W, u), H && null != x && null != _ && uc(q, H, W, u, x, _, g, J, m, v)), 16781059 & t.$$.dirty[0] | 112 & t.$$.dirty[1] && H && null != x && null != _ && uc(q, H, W, u, x, _, g, J, m, v), 16 & t.$$.dirty[0] && n(21, k = "" === Z ? Oc : 0), 16 & t.$$.dirty[0] && n(20, M = "" === Z ? 2 * Oc : Oc), 1 & t.$$.dirty[0] | 65536 & t.$$.dirty[1] && n(19, L = P.get(q.x_feature)), 1 & t.$$.dirty[0] | 65536 & t.$$.dirty[1] && n(18, A = P.get(q.y_feature))
+                }), 4292608 & t.$$.dirty[0] && n(11, u = K - r - s), 1 & t.$$.dirty[0] | 524288 & t.$$.dirty[1] && n(14, d = T[q.x_feature]), 1 & t.$$.dirty[0] | 524288 & t.$$.dirty[1] && n(13, f = T[q.y_feature]), 1 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(42, h = S.copy().domain([q.pdp_min, q.pdp_max])), 1 & t.$$.dirty[0] | 262144 & t.$$.dirty[1] && n(43, p = z.copy().domain([q.interaction_min, 0, q.interaction_max])), 25165824 & t.$$.dirty[0] | 399360 & t.$$.dirty[1] && n(8, g = "interactions" === J ? U ? p : z : U ? h : S), 1 & t.$$.dirty[0] && n(37, m = Wn(q.x_axis)), 1 & t.$$.dirty[0] && n(36, v = Wn(q.y_axis)), 402653185 & t.$$.dirty[0] | 64 & t.$$.dirty[1] && n(41, b = q.x_axis[0] - (null !== n(28, C = null === n(27, N = m.get(q.x_axis[0])) || void 0 === N ? void 0 : N.before) && void 0 !== C ? C : 0)), 1610612737 & t.$$.dirty[0] | 64 & t.$$.dirty[1] && n(40, y = q.x_axis[q.x_axis.length - 1] + (null !== n(30, D = null === n(29, O = m.get(q.x_axis[q.x_axis.length - 1])) || void 0 === O ? void 0 : O.after) && void 0 !== D ? D : 0)), 1 & t.$$.dirty[0] | 35 & t.$$.dirty[1] && n(39, $ = q.y_axis[0] - (null !== n(32, B = null === n(31, j = v.get(q.y_axis[0])) || void 0 === j ? void 0 : j.before) && void 0 !== B ? B : 0)), 1 & t.$$.dirty[0] | 44 & t.$$.dirty[1] && n(38, w = q.y_axis[q.y_axis.length - 1] + (null !== n(34, R = null === n(33, I = v.get(q.y_axis[q.y_axis.length - 1])) || void 0 === I ? void 0 : I.after) && void 0 !== R ? R : 0)), 20483 & t.$$.dirty[0] | 1536 & t.$$.dirty[1] && n(10, x = "quantitative" === d.kind ? on().domain([b, y]).range([c.left, W - c.right]) : Ir().domain(q.x_axis).range([c.left, W - c.right])), 14337 & t.$$.dirty[0] | 384 & t.$$.dirty[1] && n(9, _ = "quantitative" === f.kind ? on().domain([$, w]).range([u - c.bottom, c.top]) : Ir().domain(q.y_axis).range([u - c.bottom, c.top])), 2178 & t.$$.dirty[0] | 16 & t.$$.dirty[1] && H && (En(V, H, W, u), H && null != x && null != _ && uc(q, H, W, u, x, _, g, J, m, v)), 16781059 & t.$$.dirty[0] | 112 & t.$$.dirty[1] && H && null != x && null != _ && uc(q, H, W, u, x, _, g, J, m, v), 16 & t.$$.dirty[0] && n(21, k = "" === Z ? Bc : 0), 16 & t.$$.dirty[0] && n(20, M = "" === Z ? 2 * Bc : Bc), 1 & t.$$.dirty[0] | 65536 & t.$$.dirty[1] && n(19, L = P.get(q.x_feature)), 1 & t.$$.dirty[0] | 65536 & t.$$.dirty[1] && n(18, A = P.get(q.y_feature))
             }, [q, W, Y, G, Z, Q, nt, V, g, _, x, u, c, f, d, s, r, o, A, L, M, k, K, U, J, tt, et, N, C, O, D, j, B, I, R, H, v, m, w, $, y, b, h, p, l, i, a, P, S, z, T, function(t) {
                 X[t ? "unshift" : "push"]((() => {
                     V = t, n(7, V)
                 }))
             }]
         }
-        const jc = class extends _t {
+        const Ic = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Dc, Cc, j, {
+                super(), wt(this, t, Ec, jc, j, {
                     pd: 0,
                     width: 1,
                     height: 22,
                     scaleLocally: 23,
                     showMarginalDistribution: 2,
                     showMarginalPdp: 3,
                     colorShows: 24,
                     colorLegendTitle: 4,
                     showColorLegend: 5,
                     marginTop: 25,
                     marginRight: 26,
                     marginalPlotHeight: 6
-                }, Mc, [-1, -1])
+                }, Pc, [-1, -1])
             }
         };
 
-        function Bc(t, e) {
+        function Rc(t, e) {
             for (var n = new Array(e), r = 0; r < e; ++r) n[r] = t(r / (e - 1));
             return n
         }
 
-        function Ec(t) {
+        function Vc(t) {
             var e = t.length;
             return function(n) {
                 return t[Math.max(0, Math.min(e - 1, Math.floor(n * e)))]
             }
         }
-        const Ic = Ec(cn("44015444025645045745055946075a46085c460a5d460b5e470d60470e6147106347116447136548146748166848176948186a481a6c481b6d481c6e481d6f481f70482071482173482374482475482576482677482878482979472a7a472c7a472d7b472e7c472f7d46307e46327e46337f463480453581453781453882443983443a83443b84433d84433e85423f854240864241864142874144874045884046883f47883f48893e49893e4a893e4c8a3d4d8a3d4e8a3c4f8a3c508b3b518b3b528b3a538b3a548c39558c39568c38588c38598c375a8c375b8d365c8d365d8d355e8d355f8d34608d34618d33628d33638d32648e32658e31668e31678e31688e30698e306a8e2f6b8e2f6c8e2e6d8e2e6e8e2e6f8e2d708e2d718e2c718e2c728e2c738e2b748e2b758e2a768e2a778e2a788e29798e297a8e297b8e287c8e287d8e277e8e277f8e27808e26818e26828e26828e25838e25848e25858e24868e24878e23888e23898e238a8d228b8d228c8d228d8d218e8d218f8d21908d21918c20928c20928c20938c1f948c1f958b1f968b1f978b1f988b1f998a1f9a8a1e9b8a1e9c891e9d891f9e891f9f881fa0881fa1881fa1871fa28720a38620a48621a58521a68522a78522a88423a98324aa8325ab8225ac8226ad8127ad8128ae8029af7f2ab07f2cb17e2db27d2eb37c2fb47c31b57b32b67a34b67935b77937b87838b9773aba763bbb753dbc743fbc7340bd7242be7144bf7046c06f48c16e4ac16d4cc26c4ec36b50c46a52c56954c56856c66758c7655ac8645cc8635ec96260ca6063cb5f65cb5e67cc5c69cd5b6ccd5a6ece5870cf5773d05675d05477d1537ad1517cd2507fd34e81d34d84d44b86d54989d5488bd6468ed64590d74393d74195d84098d83e9bd93c9dd93ba0da39a2da37a5db36a8db34aadc32addc30b0dd2fb2dd2db5de2bb8de29bade28bddf26c0df25c2df23c5e021c8e020cae11fcde11dd0e11cd2e21bd5e21ad8e219dae319dde318dfe318e2e418e5e419e7e419eae51aece51befe51cf1e51df4e61ef6e620f8e621fbe723fde725"));
-        Ec(cn("00000401000501010601010802010902020b02020d03030f03031204041405041606051806051a07061c08071e0907200a08220b09240c09260d0a290e0b2b100b2d110c2f120d31130d34140e36150e38160f3b180f3d19103f1a10421c10441d11471e114920114b21114e22115024125325125527125829115a2a115c2c115f2d11612f116331116533106734106936106b38106c390f6e3b0f703d0f713f0f72400f74420f75440f764510774710784910784a10794c117a4e117b4f127b51127c52137c54137d56147d57157e59157e5a167e5c167f5d177f5f187f601880621980641a80651a80671b80681c816a1c816b1d816d1d816e1e81701f81721f817320817521817621817822817922827b23827c23827e24828025828125818326818426818627818827818928818b29818c29818e2a81902a81912b81932b80942c80962c80982d80992d809b2e7f9c2e7f9e2f7fa02f7fa1307ea3307ea5317ea6317da8327daa337dab337cad347cae347bb0357bb2357bb3367ab5367ab73779b83779ba3878bc3978bd3977bf3a77c03a76c23b75c43c75c53c74c73d73c83e73ca3e72cc3f71cd4071cf4070d0416fd2426fd3436ed5446dd6456cd8456cd9466bdb476adc4869de4968df4a68e04c67e24d66e34e65e44f64e55064e75263e85362e95462ea5661eb5760ec5860ed5a5fee5b5eef5d5ef05f5ef1605df2625df2645cf3655cf4675cf4695cf56b5cf66c5cf66e5cf7705cf7725cf8745cf8765cf9785df9795df97b5dfa7d5efa7f5efa815ffb835ffb8560fb8761fc8961fc8a62fc8c63fc8e64fc9065fd9266fd9467fd9668fd9869fd9a6afd9b6bfe9d6cfe9f6dfea16efea36ffea571fea772fea973feaa74feac76feae77feb078feb27afeb47bfeb67cfeb77efeb97ffebb81febd82febf84fec185fec287fec488fec68afec88cfeca8dfecc8ffecd90fecf92fed194fed395fed597fed799fed89afdda9cfddc9efddea0fde0a1fde2a3fde3a5fde5a7fde7a9fde9aafdebacfcecaefceeb0fcf0b2fcf2b4fcf4b6fcf6b8fcf7b9fcf9bbfcfbbdfcfdbf")), Ec(cn("00000401000501010601010802010a02020c02020e03021004031204031405041706041907051b08051d09061f0a07220b07240c08260d08290e092b10092d110a30120a32140b34150b37160b39180c3c190c3e1b0c411c0c431e0c451f0c48210c4a230c4c240c4f260c51280b53290b552b0b572d0b592f0a5b310a5c320a5e340a5f3609613809623909633b09643d09653e0966400a67420a68440a68450a69470b6a490b6a4a0c6b4c0c6b4d0d6c4f0d6c510e6c520e6d540f6d550f6d57106e59106e5a116e5c126e5d126e5f136e61136e62146e64156e65156e67166e69166e6a176e6c186e6d186e6f196e71196e721a6e741a6e751b6e771c6d781c6d7a1d6d7c1d6d7d1e6d7f1e6c801f6c82206c84206b85216b87216b88226a8a226a8c23698d23698f24699025689225689326679526679727669827669a28659b29649d29649f2a63a02a63a22b62a32c61a52c60a62d60a82e5fa92e5eab2f5ead305dae305cb0315bb1325ab3325ab43359b63458b73557b93556ba3655bc3754bd3853bf3952c03a51c13a50c33b4fc43c4ec63d4dc73e4cc83f4bca404acb4149cc4248ce4347cf4446d04545d24644d34743d44842d54a41d74b3fd84c3ed94d3dda4e3cdb503bdd513ade5238df5337e05536e15635e25734e35933e45a31e55c30e65d2fe75e2ee8602de9612bea632aeb6429eb6628ec6726ed6925ee6a24ef6c23ef6e21f06f20f1711ff1731df2741cf3761bf37819f47918f57b17f57d15f67e14f68013f78212f78410f8850ff8870ef8890cf98b0bf98c0af98e09fa9008fa9207fa9407fb9606fb9706fb9906fb9b06fb9d07fc9f07fca108fca309fca50afca60cfca80dfcaa0ffcac11fcae12fcb014fcb216fcb418fbb61afbb81dfbba1ffbbc21fbbe23fac026fac228fac42afac62df9c72ff9c932f9cb35f8cd37f8cf3af7d13df7d340f6d543f6d746f5d949f5db4cf4dd4ff4df53f4e156f3e35af3e55df2e661f2e865f2ea69f1ec6df1ed71f1ef75f1f179f2f27df2f482f3f586f3f68af4f88ef5f992f6fa96f8fb9af9fc9dfafda1fcffa4"));
-        var Rc = Ec(cn("0d088710078813078916078a19068c1b068d1d068e20068f2206902406912605912805922a05932c05942e05952f059631059733059735049837049938049a3a049a3c049b3e049c3f049c41049d43039e44039e46039f48039f4903a04b03a14c02a14e02a25002a25102a35302a35502a45601a45801a45901a55b01a55c01a65e01a66001a66100a76300a76400a76600a76700a86900a86a00a86c00a86e00a86f00a87100a87201a87401a87501a87701a87801a87a02a87b02a87d03a87e03a88004a88104a78305a78405a78606a68707a68808a68a09a58b0aa58d0ba58e0ca48f0da4910ea3920fa39410a29511a19613a19814a099159f9a169f9c179e9d189d9e199da01a9ca11b9ba21d9aa31e9aa51f99a62098a72197a82296aa2395ab2494ac2694ad2793ae2892b02991b12a90b22b8fb32c8eb42e8db52f8cb6308bb7318ab83289ba3388bb3488bc3587bd3786be3885bf3984c03a83c13b82c23c81c33d80c43e7fc5407ec6417dc7427cc8437bc9447aca457acb4679cc4778cc4977cd4a76ce4b75cf4c74d04d73d14e72d24f71d35171d45270d5536fd5546ed6556dd7566cd8576bd9586ada5a6ada5b69db5c68dc5d67dd5e66de5f65de6164df6263e06363e16462e26561e26660e3685fe4695ee56a5de56b5de66c5ce76e5be76f5ae87059e97158e97257ea7457eb7556eb7655ec7754ed7953ed7a52ee7b51ef7c51ef7e50f07f4ff0804ef1814df1834cf2844bf3854bf3874af48849f48948f58b47f58c46f68d45f68f44f79044f79143f79342f89441f89540f9973ff9983ef99a3efa9b3dfa9c3cfa9e3bfb9f3afba139fba238fca338fca537fca636fca835fca934fdab33fdac33fdae32fdaf31fdb130fdb22ffdb42ffdb52efeb72dfeb82cfeba2cfebb2bfebd2afebe2afec029fdc229fdc328fdc527fdc627fdc827fdca26fdcb26fccd25fcce25fcd025fcd225fbd324fbd524fbd724fad824fada24f9dc24f9dd25f8df25f8e125f7e225f7e425f6e626f6e826f5e926f5eb27f4ed27f3ee27f3f027f2f227f1f426f1f525f0f724f0f921"));
-        const Vc = cn("4e79a7f28e2ce1575976b7b259a14fedc949af7aa1ff9da79c755fbab0ab");
+        const Hc = Vc(cn("44015444025645045745055946075a46085c460a5d460b5e470d60470e6147106347116447136548146748166848176948186a481a6c481b6d481c6e481d6f481f70482071482173482374482475482576482677482878482979472a7a472c7a472d7b472e7c472f7d46307e46327e46337f463480453581453781453882443983443a83443b84433d84433e85423f854240864241864142874144874045884046883f47883f48893e49893e4a893e4c8a3d4d8a3d4e8a3c4f8a3c508b3b518b3b528b3a538b3a548c39558c39568c38588c38598c375a8c375b8d365c8d365d8d355e8d355f8d34608d34618d33628d33638d32648e32658e31668e31678e31688e30698e306a8e2f6b8e2f6c8e2e6d8e2e6e8e2e6f8e2d708e2d718e2c718e2c728e2c738e2b748e2b758e2a768e2a778e2a788e29798e297a8e297b8e287c8e287d8e277e8e277f8e27808e26818e26828e26828e25838e25848e25858e24868e24878e23888e23898e238a8d228b8d228c8d228d8d218e8d218f8d21908d21918c20928c20928c20938c1f948c1f958b1f968b1f978b1f988b1f998a1f9a8a1e9b8a1e9c891e9d891f9e891f9f881fa0881fa1881fa1871fa28720a38620a48621a58521a68522a78522a88423a98324aa8325ab8225ac8226ad8127ad8128ae8029af7f2ab07f2cb17e2db27d2eb37c2fb47c31b57b32b67a34b67935b77937b87838b9773aba763bbb753dbc743fbc7340bd7242be7144bf7046c06f48c16e4ac16d4cc26c4ec36b50c46a52c56954c56856c66758c7655ac8645cc8635ec96260ca6063cb5f65cb5e67cc5c69cd5b6ccd5a6ece5870cf5773d05675d05477d1537ad1517cd2507fd34e81d34d84d44b86d54989d5488bd6468ed64590d74393d74195d84098d83e9bd93c9dd93ba0da39a2da37a5db36a8db34aadc32addc30b0dd2fb2dd2db5de2bb8de29bade28bddf26c0df25c2df23c5e021c8e020cae11fcde11dd0e11cd2e21bd5e21ad8e219dae319dde318dfe318e2e418e5e419e7e419eae51aece51befe51cf1e51df4e61ef6e620f8e621fbe723fde725"));
+        Vc(cn("00000401000501010601010802010902020b02020d03030f03031204041405041606051806051a07061c08071e0907200a08220b09240c09260d0a290e0b2b100b2d110c2f120d31130d34140e36150e38160f3b180f3d19103f1a10421c10441d11471e114920114b21114e22115024125325125527125829115a2a115c2c115f2d11612f116331116533106734106936106b38106c390f6e3b0f703d0f713f0f72400f74420f75440f764510774710784910784a10794c117a4e117b4f127b51127c52137c54137d56147d57157e59157e5a167e5c167f5d177f5f187f601880621980641a80651a80671b80681c816a1c816b1d816d1d816e1e81701f81721f817320817521817621817822817922827b23827c23827e24828025828125818326818426818627818827818928818b29818c29818e2a81902a81912b81932b80942c80962c80982d80992d809b2e7f9c2e7f9e2f7fa02f7fa1307ea3307ea5317ea6317da8327daa337dab337cad347cae347bb0357bb2357bb3367ab5367ab73779b83779ba3878bc3978bd3977bf3a77c03a76c23b75c43c75c53c74c73d73c83e73ca3e72cc3f71cd4071cf4070d0416fd2426fd3436ed5446dd6456cd8456cd9466bdb476adc4869de4968df4a68e04c67e24d66e34e65e44f64e55064e75263e85362e95462ea5661eb5760ec5860ed5a5fee5b5eef5d5ef05f5ef1605df2625df2645cf3655cf4675cf4695cf56b5cf66c5cf66e5cf7705cf7725cf8745cf8765cf9785df9795df97b5dfa7d5efa7f5efa815ffb835ffb8560fb8761fc8961fc8a62fc8c63fc8e64fc9065fd9266fd9467fd9668fd9869fd9a6afd9b6bfe9d6cfe9f6dfea16efea36ffea571fea772fea973feaa74feac76feae77feb078feb27afeb47bfeb67cfeb77efeb97ffebb81febd82febf84fec185fec287fec488fec68afec88cfeca8dfecc8ffecd90fecf92fed194fed395fed597fed799fed89afdda9cfddc9efddea0fde0a1fde2a3fde3a5fde5a7fde7a9fde9aafdebacfcecaefceeb0fcf0b2fcf2b4fcf4b6fcf6b8fcf7b9fcf9bbfcfbbdfcfdbf")), Vc(cn("00000401000501010601010802010a02020c02020e03021004031204031405041706041907051b08051d09061f0a07220b07240c08260d08290e092b10092d110a30120a32140b34150b37160b39180c3c190c3e1b0c411c0c431e0c451f0c48210c4a230c4c240c4f260c51280b53290b552b0b572d0b592f0a5b310a5c320a5e340a5f3609613809623909633b09643d09653e0966400a67420a68440a68450a69470b6a490b6a4a0c6b4c0c6b4d0d6c4f0d6c510e6c520e6d540f6d550f6d57106e59106e5a116e5c126e5d126e5f136e61136e62146e64156e65156e67166e69166e6a176e6c186e6d186e6f196e71196e721a6e741a6e751b6e771c6d781c6d7a1d6d7c1d6d7d1e6d7f1e6c801f6c82206c84206b85216b87216b88226a8a226a8c23698d23698f24699025689225689326679526679727669827669a28659b29649d29649f2a63a02a63a22b62a32c61a52c60a62d60a82e5fa92e5eab2f5ead305dae305cb0315bb1325ab3325ab43359b63458b73557b93556ba3655bc3754bd3853bf3952c03a51c13a50c33b4fc43c4ec63d4dc73e4cc83f4bca404acb4149cc4248ce4347cf4446d04545d24644d34743d44842d54a41d74b3fd84c3ed94d3dda4e3cdb503bdd513ade5238df5337e05536e15635e25734e35933e45a31e55c30e65d2fe75e2ee8602de9612bea632aeb6429eb6628ec6726ed6925ee6a24ef6c23ef6e21f06f20f1711ff1731df2741cf3761bf37819f47918f57b17f57d15f67e14f68013f78212f78410f8850ff8870ef8890cf98b0bf98c0af98e09fa9008fa9207fa9407fb9606fb9706fb9906fb9b06fb9d07fc9f07fca108fca309fca50afca60cfca80dfcaa0ffcac11fcae12fcb014fcb216fcb418fbb61afbb81dfbba1ffbbc21fbbe23fac026fac228fac42afac62df9c72ff9c932f9cb35f8cd37f8cf3af7d13df7d340f6d543f6d746f5d949f5db4cf4dd4ff4df53f4e156f3e35af3e55df2e661f2e865f2ea69f1ec6df1ed71f1ef75f1f179f2f27df2f482f3f586f3f68af4f88ef5f992f6fa96f8fb9af9fc9dfafda1fcffa4"));
+        var qc = Vc(cn("0d088710078813078916078a19068c1b068d1d068e20068f2206902406912605912805922a05932c05942e05952f059631059733059735049837049938049a3a049a3c049b3e049c3f049c41049d43039e44039e46039f48039f4903a04b03a14c02a14e02a25002a25102a35302a35502a45601a45801a45901a55b01a55c01a65e01a66001a66100a76300a76400a76600a76700a86900a86a00a86c00a86e00a86f00a87100a87201a87401a87501a87701a87801a87a02a87b02a87d03a87e03a88004a88104a78305a78405a78606a68707a68808a68a09a58b0aa58d0ba58e0ca48f0da4910ea3920fa39410a29511a19613a19814a099159f9a169f9c179e9d189d9e199da01a9ca11b9ba21d9aa31e9aa51f99a62098a72197a82296aa2395ab2494ac2694ad2793ae2892b02991b12a90b22b8fb32c8eb42e8db52f8cb6308bb7318ab83289ba3388bb3488bc3587bd3786be3885bf3984c03a83c13b82c23c81c33d80c43e7fc5407ec6417dc7427cc8437bc9447aca457acb4679cc4778cc4977cd4a76ce4b75cf4c74d04d73d14e72d24f71d35171d45270d5536fd5546ed6556dd7566cd8576bd9586ada5a6ada5b69db5c68dc5d67dd5e66de5f65de6164df6263e06363e16462e26561e26660e3685fe4695ee56a5de56b5de66c5ce76e5be76f5ae87059e97158e97257ea7457eb7556eb7655ec7754ed7953ed7a52ee7b51ef7c51ef7e50f07f4ff0804ef1814df1834cf2844bf3854bf3874af48849f48948f58b47f58c46f68d45f68f44f79044f79143f79342f89441f89540f9973ff9983ef99a3efa9b3dfa9c3cfa9e3bfb9f3afba139fba238fca338fca537fca636fca835fca934fdab33fdac33fdae32fdaf31fdb130fdb22ffdb42ffdb52efeb72dfeb82cfeba2cfebb2bfebd2afebe2afec029fdc229fdc328fdc527fdc627fdc827fdca26fdcb26fccd25fcce25fcd025fcd225fbd324fbd524fbd724fad824fada24f9dc24f9dd25f8df25f8e125f7e225f7e425f6e626f6e826f5e926f5eb27f4ed27f3ee27f3f027f2f227f1f426f1f525f0f724f0f921"));
+        const Fc = cn("4e79a7f28e2ce1575976b7b259a14fedc949af7aa1ff9da79c755fbab0ab");
 
-        function Hc(t) {
+        function Wc(t) {
             u(t, "svelte-1pgkml6", ".color-container.svelte-1pgkml6{display:flex;align-items:center;gap:1em}.swatches.svelte-1pgkml6{flex:1;display:flex;gap:1em}.swatch-cell.svelte-1pgkml6{display:flex;align-items:center}.swatch-square.svelte-1pgkml6{min-width:var(--size);min-height:var(--size);margin-right:0.25em}")
         }
 
-        function qc(t, e, n) {
+        function Kc(t, e, n) {
             const r = t.slice();
             return r[10] = e[n], r
         }
 
-        function Fc(t) {
+        function Xc(t) {
             let e, n, r;
             return {
                 c() {
                     e = p("div"), n = m(t[5]), r = m(":"), $(e, "class", "pdpilot-small pdpilot-bold")
                 },
                 m(t, i) {
                     d(t, e, i), c(e, n), c(e, r)
@@ -8259,16 +8312,16 @@
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Wc(t) {
-            let e, n, r, i, o, l, a = `${Xc}px`,
+        function Uc(t) {
+            let e, n, r, i, o, l, a = `${Gc}px`,
                 s = (t[6][t[10]] ?? t[10]) + "";
             return {
                 c() {
                     e = p("div"), n = p("div"), r = v(), i = p("div"), o = m(s), l = v(), $(n, "class", "swatch-square svelte-1pgkml6"), M(n, "--size", a), M(n, "background-color", t[2](t[10])), $(i, "class", "swatch-label pdpilot-small"), $(e, "class", "swatch-cell svelte-1pgkml6")
                 },
                 m(t, a) {
                     d(t, e, a), c(e, n), c(e, r), c(e, i), c(i, o), c(e, l)
@@ -8278,57 +8331,57 @@
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Kc(t) {
+        function Yc(t) {
             let e, n, r, i, o = `${t[8]}px`,
                 l = `${t[1]}px`,
                 a = `${t[0]}px`,
                 s = `${t[3]}px`,
                 u = `${t[4]}px`,
-                g = "" !== t[5] && Fc(t),
+                g = "" !== t[5] && Xc(t),
                 m = ht(t[2].domain()),
                 b = [];
-            for (let e = 0; e < m.length; e += 1) b[e] = Wc(qc(t, m, e));
+            for (let e = 0; e < m.length; e += 1) b[e] = Uc(Kc(t, m, e));
             return {
                 c() {
                     e = p("div"), g && g.c(), n = v(), r = p("div");
                     for (let t = 0; t < b.length; t += 1) b[t].c();
                     $(r, "class", "swatches svelte-1pgkml6"), M(r, "max-width", o), $(e, "class", "color-container svelte-1pgkml6"), M(e, "max-height", l), M(e, "max-width", a), M(e, "margin-left", s), M(e, "margin-right", u)
                 },
                 m(o, l) {
                     d(o, e, l), g && g.m(e, null), c(e, n), c(e, r);
                     for (let t = 0; t < b.length; t += 1) b[t] && b[t].m(r, null);
                     i = S.observe(r, t[9].bind(r))
                 },
                 p(t, [i]) {
-                    if ("" !== t[5] ? g ? g.p(t, i) : (g = Fc(t), g.c(), g.m(e, n)) : g && (g.d(1), g = null), 68 & i) {
+                    if ("" !== t[5] ? g ? g.p(t, i) : (g = Xc(t), g.c(), g.m(e, n)) : g && (g.d(1), g = null), 68 & i) {
                         let e;
                         for (m = ht(t[2].domain()), e = 0; e < m.length; e += 1) {
-                            const n = qc(t, m, e);
-                            b[e] ? b[e].p(n, i) : (b[e] = Wc(n), b[e].c(), b[e].m(r, null))
+                            const n = Kc(t, m, e);
+                            b[e] ? b[e].p(n, i) : (b[e] = Uc(n), b[e].c(), b[e].m(r, null))
                         }
                         for (; e < b.length; e += 1) b[e].d(1);
                         b.length = m.length
                     }
                     256 & i && o !== (o = `${t[8]}px`) && M(r, "max-width", o), 2 & i && l !== (l = `${t[1]}px`) && M(e, "max-height", l), 1 & i && a !== (a = `${t[0]}px`) && M(e, "max-width", a), 8 & i && s !== (s = `${t[3]}px`) && M(e, "margin-left", s), 16 & i && u !== (u = `${t[4]}px`) && M(e, "margin-right", u)
                 },
                 i: T,
                 o: T,
                 d(t) {
                     t && f(e), g && g.d(), h(b, t), i()
                 }
             }
         }
-        const Xc = 12;
+        const Gc = 12;
 
-        function Uc(t, e, n) {
+        function Jc(t, e, n) {
             let r, {
                     width: i
                 } = e,
                 {
                     height: o
                 } = e,
                 {
@@ -8351,35 +8404,35 @@
                 "width" in t && n(0, i = t.width), "height" in t && n(1, o = t.height), "color" in t && n(2, l = t.color), "marginLeft" in t && n(3, s = t.marginLeft), "marginRight" in t && n(4, c = t.marginRight), "title" in t && n(5, u = t.title), "value_map" in t && n(6, d = t.value_map)
             }, t.$$.update = () => {
                 128 & t.$$.dirty && n(8, f = r ? r[0].inlineSize : 0)
             }, [i, o, l, s, c, u, d, r, f, function() {
                 r = a.entries.get(this)?.borderBoxSize, n(7, r)
             }]
         }
-        const Yc = class extends _t {
+        const Zc = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Uc, Kc, j, {
+                super(), wt(this, t, Jc, Yc, j, {
                     width: 0,
                     height: 1,
                     color: 2,
                     marginLeft: 3,
                     marginRight: 4,
                     title: 5,
                     value_map: 6
-                }, Hc)
+                }, Wc)
             }
         };
 
-        function Gc(t) {
+        function Qc(t) {
             u(t, "svelte-crr1ai", ".two-way-container.svelte-crr1ai{position:relative;width:100%;height:100%}svg.svelte-crr1ai,canvas.svelte-crr1ai{position:absolute;top:var(--top);left:0}")
         }
 
-        function Jc(t) {
+        function tu(t) {
             let e, n, r, i, o = `${t[9].left}px`;
-            const l = [Qc, Zc],
+            const l = [nu, eu],
                 a = [];
 
             function s(t, e) {
                 return "interpolator" in t[4] ? 0 : 1
             }
             return n = s(t), r = a[n] = l[n](t), {
                 c() {
@@ -8402,17 +8455,17 @@
                 },
                 d(t) {
                     t && f(e), a[n].d()
                 }
             }
         }
 
-        function Zc(t) {
+        function eu(t) {
             let e, n;
-            return e = new Yc({
+            return e = new Zc({
                 props: {
                     width: t[1] - t[9].left - t[9].right,
                     height: t[11],
                     color: t[4],
                     value_map: "value_map" in t[8] ? t[8].value_map : {},
                     title: t[0].y_feature,
                     marginLeft: 10,
@@ -8437,15 +8490,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Qc(t) {
+        function nu(t) {
             let e, n;
             return e = new wc({
                 props: {
                     width: t[1] - t[9].left - t[9].right,
                     height: t[11],
                     color: t[4],
                     title: t[0].y_feature,
@@ -8471,16 +8524,16 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function tu(t) {
-            let e, n, r, i, o, l, a, s, u = t[2] && Jc(t);
+        function ru(t) {
+            let e, n, r, i, o, l, a, s, u = t[2] && tu(t);
             return l = new Ma({
                 props: {
                     scale: t[6],
                     y: t[7] - t[9].bottom,
                     label: t[0].x_feature,
                     integerOnly: "discrete" === t[10].subkind,
                     value_map: "value_map" in t[10] ? t[10].value_map : {}
@@ -8497,15 +8550,15 @@
                 c() {
                     e = p("div"), u && u.c(), n = v(), r = p("canvas"), i = v(), o = g("svg"), bt(l.$$.fragment), bt(a.$$.fragment), $(r, "class", "svelte-crr1ai"), $(o, "width", t[1]), $(o, "height", t[7]), $(o, "class", "svelte-crr1ai"), $(e, "class", "two-way-container svelte-crr1ai"), M(e, "--top", t[11])
                 },
                 m(f, h) {
                     d(f, e, h), u && u.m(e, null), c(e, n), c(e, r), t[23](r), c(e, i), c(e, o), yt(l, o, null), yt(a, o, null), s = !0
                 },
                 p(t, [r]) {
-                    t[2] ? u ? (u.p(t, r), 4 & r && dt(u, 1)) : (u = Jc(t), u.c(), dt(u, 1), u.m(e, n)) : u && (ct(), ft(u, 1, 1, (() => {
+                    t[2] ? u ? (u.p(t, r), 4 & r && dt(u, 1)) : (u = tu(t), u.c(), dt(u, 1), u.m(e, n)) : u && (ct(), ft(u, 1, 1, (() => {
                         u = null
                     })), ut());
                     const i = {};
                     64 & r && (i.scale = t[6]), 640 & r && (i.y = t[7] - t[9].bottom), 1 & r && (i.label = t[0].x_feature), 1024 & r && (i.integerOnly = "discrete" === t[10].subkind), 1024 & r && (i.value_map = "value_map" in t[10] ? t[10].value_map : {}), l.$set(i);
                     const c = {};
                     32 & r && (c.scale = t[5]), 512 & r && (c.x = t[9].left), 256 & r && (c.integerOnly = "discrete" === t[8].subkind), 256 & r && (c.value_map = "value_map" in t[8] ? t[8].value_map : {}), a.$set(c), (!s || 2 & r) && $(o, "width", t[1]), (!s || 128 & r) && $(o, "height", t[7]), 2048 & r && M(e, "--top", t[11])
                 },
@@ -8517,15 +8570,15 @@
                 },
                 d(n) {
                     n && f(e), u && u.d(), t[23](null), $t(l), $t(a)
                 }
             }
         }
 
-        function eu(t, e, n) {
+        function iu(t, e, n) {
             let r, i, o, l, a, s, c, u, d, f, h, p, g, m;
             E(t, or, (t => n(21, g = t))), E(t, Zn, (t => n(22, m = t)));
             let v, b, {
                     pd: y
                 } = e,
                 {
                     width: $
@@ -8561,21 +8614,21 @@
             }, t.$$.update = () => {
                 4 & t.$$.dirty && n(11, r = _ ? 24 : 0), 6144 & t.$$.dirty && n(7, i = w - r), 49152 & t.$$.dirty && n(9, o = {
                     top: k,
                     right: M,
                     bottom: 35,
                     left: 50
                 }), 4194305 & t.$$.dirty && n(10, l = m[y.x_feature]), 4194305 & t.$$.dirty && n(8, a = m[y.y_feature]), 641 & t.$$.dirty && n(20, s = on().domain([y.pdp_min, y.pdp_max]).range([i - o.bottom, o.top])), 2097792 & t.$$.dirty && n(19, c = on().domain(g).range([i - o.bottom, o.top])), 1581056 & t.$$.dirty && n(5, u = x ? s : c), 1539 & t.$$.dirty && n(6, d = "quantitative" === l.kind ? on().domain([y.x_values[0], y.x_values[y.x_values.length - 1]]).range([o.left, $ - o.right]) : Vr().domain(y.x_values).range([o.left, $ - o.right]).padding(.5)), 256 & t.$$.dirty && n(4, f = function(t) {
-                    if ("quantitative" === t.kind) return an().domain([t.values[0], t.values[t.values.length - 1]]).interpolator((t => Ic(1 - t)));
+                    if ("quantitative" === t.kind) return an().domain([t.values[0], t.values[t.values.length - 1]]).interpolator((t => Hc(1 - t)));
                     if ("categorical" !== t.kind || "nominal" !== t.subkind && "one_hot" !== t.subkind) {
                         const e = t.values.length;
-                        return Er().domain(t.values).range(Bc(Ic, e).reverse())
+                        return Er().domain(t.values).range(Rc(Hc, e).reverse())
                     } {
                         const e = t.values.length;
-                        return Er().domain(t.values).range(e <= 10 ? Vc : Bc(Ic, e).reverse())
+                        return Er().domain(t.values).range(e <= 10 ? Fc : Rc(Hc, e).reverse())
                     }
                 }(a)), 65632 & t.$$.dirty && n(17, h = ei().x((t => {
                     var e;
                     return null !== (e = d(t.x)) && void 0 !== e ? e : 0
                 })).y((t => u(t.prediction))).context(b)), 1 & t.$$.dirty && n(18, p = function(t) {
                     var e;
                     const n = new Map;
@@ -8596,31 +8649,31 @@
                 }(y)), 65674 & t.$$.dirty && b && (En(v, b, $, i), b && null != d && null != u && null != h && L(p, b, h, f)), 458864 & t.$$.dirty && b && null != d && null != u && null != h && L(p, b, h, f)
             }, [y, $, _, v, f, u, d, i, a, o, l, r, w, x, k, M, b, h, p, c, s, g, m, function(t) {
                 X[t ? "unshift" : "push"]((() => {
                     v = t, n(3, v)
                 }))
             }]
         }
-        const nu = class extends _t {
+        const ou = class extends _t {
             constructor(t) {
-                super(), wt(this, t, eu, tu, j, {
+                super(), wt(this, t, iu, ru, j, {
                     pd: 0,
                     width: 1,
                     height: 12,
                     scaleLocally: 13,
                     showColorLegend: 2,
                     marginTop: 14,
                     marginRight: 15
-                }, Gc)
+                }, Qc)
             }
         };
 
-        function ru(t) {
+        function lu(t) {
             let e, n;
-            return e = new nu({
+            return e = new ou({
                 props: {
                     pd: t[0],
                     width: t[1],
                     height: t[2],
                     scaleLocally: t[3],
                     showColorLegend: t[7],
                     marginTop: t[9],
@@ -8645,17 +8698,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function iu(t) {
+        function au(t) {
             let e, n;
-            return e = new jc({
+            return e = new Ic({
                 props: {
                     pd: t[0],
                     width: t[1],
                     height: t[2],
                     scaleLocally: t[3],
                     showMarginalDistribution: t[4],
                     showMarginalPdp: t[5],
@@ -8685,17 +8738,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function ou(t) {
+        function su(t) {
             let e, n, r, i;
-            const o = [iu, ru],
+            const o = [au, lu],
                 l = [];
 
             function a(t, e) {
                 return "heatmap" === t[12] ? 0 : 1
             }
             return e = a(t), n = l[e] = o[e](t), {
                 c() {
@@ -8718,15 +8771,15 @@
                 },
                 d(t) {
                     t && f(r), l[e].d(t)
                 }
             }
         }
 
-        function lu(t, e, n) {
+        function cu(t, e, n) {
             let {
                 pd: r
             } = e, {
                 width: i
             } = e, {
                 height: o
             } = e, {
@@ -8750,17 +8803,17 @@
             } = e, {
                 twoWayKind: g = "heatmap"
             } = e;
             return t.$$set = t => {
                 "pd" in t && n(0, r = t.pd), "width" in t && n(1, i = t.width), "height" in t && n(2, o = t.height), "scaleLocally" in t && n(3, l = t.scaleLocally), "showMarginalDistribution" in t && n(4, a = t.showMarginalDistribution), "showMarginalPdp" in t && n(5, s = t.showMarginalPdp), "colorShows" in t && n(6, c = t.colorShows), "showColorLegend" in t && n(7, u = t.showColorLegend), "colorLegendTitle" in t && n(8, d = t.colorLegendTitle), "marginTop" in t && n(9, f = t.marginTop), "marginRight" in t && n(10, h = t.marginRight), "marginalPlotHeight" in t && n(11, p = t.marginalPlotHeight), "twoWayKind" in t && n(12, g = t.twoWayKind)
             }, [r, i, o, l, a, s, c, u, d, f, h, p, g]
         }
-        const au = class extends _t {
+        const uu = class extends _t {
             constructor(t) {
-                super(), wt(this, t, lu, ou, j, {
+                super(), wt(this, t, cu, su, j, {
                     pd: 0,
                     width: 1,
                     height: 2,
                     scaleLocally: 3,
                     showMarginalDistribution: 4,
                     showMarginalPdp: 5,
                     colorShows: 6,
@@ -8770,17 +8823,17 @@
                     marginRight: 10,
                     marginalPlotHeight: 11,
                     twoWayKind: 12
                 })
             }
         };
 
-        function su(t) {
+        function du(t) {
             let e, n, r, i;
-            const o = [uu, cu],
+            const o = [hu, fu],
                 l = [];
 
             function a(t, e) {
                 return 1 === t[0].num_features ? 0 : 2 === t[0].num_features ? 1 : -1
             }
             return ~(e = a(t)) && (n = l[e] = o[e](t)), {
                 c() {
@@ -8803,17 +8856,17 @@
                 },
                 d(t) {
                     t && f(r), ~e && l[e].d(t)
                 }
             }
         }
 
-        function cu(t) {
+        function fu(t) {
             let e, n;
-            return e = new au({
+            return e = new uu({
                 props: {
                     width: t[1],
                     height: t[2],
                     pd: t[0],
                     scaleLocally: t[3],
                     colorShows: t[4],
                     showColorLegend: t[5],
@@ -8844,15 +8897,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function uu(t) {
+        function hu(t) {
             let e, n;
             return e = new ac({
                 props: {
                     width: t[1],
                     height: t[2],
                     pd: t[0],
                     scaleLocally: t[3],
@@ -8884,25 +8937,25 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function du(t) {
-            let e, n, r = t[1] > 0 && t[2] > 0 && su(t);
+        function pu(t) {
+            let e, n, r = t[1] > 0 && t[2] > 0 && du(t);
             return {
                 c() {
                     r && r.c(), e = b()
                 },
                 m(t, i) {
                     r && r.m(t, i), d(t, e, i), n = !0
                 },
                 p(t, [n]) {
-                    t[1] > 0 && t[2] > 0 ? r ? (r.p(t, n), 6 & n && dt(r, 1)) : (r = su(t), r.c(), dt(r, 1), r.m(e.parentNode, e)) : r && (ct(), ft(r, 1, 1, (() => {
+                    t[1] > 0 && t[2] > 0 ? r ? (r.p(t, n), 6 & n && dt(r, 1)) : (r = du(t), r.c(), dt(r, 1), r.m(e.parentNode, e)) : r && (ct(), ft(r, 1, 1, (() => {
                         r = null
                     })), ut())
                 },
                 i(t) {
                     n || (dt(r), n = !0)
                 },
                 o(t) {
@@ -8910,15 +8963,15 @@
                 },
                 d(t) {
                     t && f(e), r && r.d(t)
                 }
             }
         }
 
-        function fu(t, e, n) {
+        function gu(t, e, n) {
             let {
                 pd: r
             } = e, {
                 width: i
             } = e, {
                 height: o
             } = e, {
@@ -8952,17 +9005,17 @@
             } = e, {
                 twoWayKind: $ = "heatmap"
             } = e;
             return t.$$set = t => {
                 "pd" in t && n(0, r = t.pd), "width" in t && n(1, i = t.width), "height" in t && n(2, o = t.height), "scaleLocally" in t && n(3, l = t.scaleLocally), "colorShows" in t && n(4, a = t.colorShows), "showColorLegend" in t && n(5, s = t.showColorLegend), "colorLegendTitle" in t && n(6, c = t.colorLegendTitle), "iceLevel" in t && n(7, u = t.iceLevel), "indices" in t && n(8, d = t.indices), "showMarginalDistribution" in t && n(9, f = t.showMarginalDistribution), "showMarginalPdp" in t && n(10, h = t.showMarginalPdp), "marginTop" in t && n(11, p = t.marginTop), "marginRight" in t && n(12, g = t.marginRight), "marginalPlotHeight" in t && n(13, m = t.marginalPlotHeight), "allowBrushing" in t && n(14, v = t.allowBrushing), "showBrushedBorder" in t && n(15, b = t.showBrushedBorder), "iceLineWidth" in t && n(16, y = t.iceLineWidth), "twoWayKind" in t && n(17, $ = t.twoWayKind)
             }, [r, i, o, l, a, s, c, u, d, f, h, p, g, m, v, b, y, $]
         }
-        const hu = class extends _t {
+        const mu = class extends _t {
             constructor(t) {
-                super(), wt(this, t, fu, du, j, {
+                super(), wt(this, t, gu, pu, j, {
                     pd: 0,
                     width: 1,
                     height: 2,
                     scaleLocally: 3,
                     colorShows: 4,
                     showColorLegend: 5,
                     colorLegendTitle: 6,
@@ -8977,69 +9030,69 @@
                     showBrushedBorder: 15,
                     iceLineWidth: 16,
                     twoWayKind: 17
                 })
             }
         };
 
-        function pu(t, e) {
+        function vu(t, e) {
             if ((i = t.length) > 1)
                 for (var n, r, i, o = 1, l = t[e[0]], a = l.length; o < i; ++o)
                     for (r = l, l = t[e[o]], n = 0; n < a; ++n) l[n][1] += l[n][0] = isNaN(r[n][1]) ? r[n][0] : r[n][1]
         }
 
-        function gu(t) {
+        function bu(t) {
             for (var e = t.length, n = new Array(e); --e >= 0;) n[e] = e;
             return n
         }
 
-        function mu(t, e) {
+        function yu(t, e) {
             return t[e]
         }
 
-        function vu(t) {
+        function $u(t) {
             const e = [];
             return e.key = t, e
         }
 
-        function bu(t, e) {
+        function wu(t, e) {
             if ((r = t.length) > 0) {
                 for (var n, r, i, o = 0, l = t[0].length; o < l; ++o) {
                     for (i = n = 0; n < r; ++n) i += t[n][o][1] || 0;
                     if (i)
                         for (n = 0; n < r; ++n) t[n][o][1] /= i
                 }
-                pu(t, e)
+                vu(t, e)
             }
         }
 
-        function yu(t) {
-            return gu(t).reverse()
+        function xu(t) {
+            return bu(t).reverse()
         }
 
-        function $u(t) {
+        function _u(t) {
             u(t, "svelte-1gasvv0", ".distributions-container.svelte-1gasvv0{width:100%;height:100%;display:flex;flex-direction:column;gap:0.5em}.distributions-settings.svelte-1gasvv0{display:flex;align-items:center;gap:1em}.distribution-plots.svelte-1gasvv0{flex:1;overflow-y:auto;position:relative}.label-and-input.svelte-1gasvv0{display:flex;align-items:center;gap:0.25em}svg.svelte-1gasvv0,canvas.svelte-1gasvv0{position:absolute;left:0}")
         }
 
-        function wu(t, e, n) {
+        function ku(t, e, n) {
             const r = t.slice();
             return r[39] = e[n], r
         }
 
-        function xu(t, e, n) {
+        function Mu(t, e, n) {
             const r = t.slice();
             return r[42] = e[n], r[44] = n, r
         }
 
-        function _u(t, e, n) {
+        function Lu(t, e, n) {
             const r = t.slice();
             return r[45] = e[n], r
         }
 
-        function ku(t) {
+        function Au(t) {
             let e, n, r, i, o;
             return {
                 c() {
                     e = p("label"), n = p("input"), r = m("Normalize bar charts"), $(n, "type", "checkbox"), $(e, "class", "label-and-input svelte-1gasvv0")
                 },
                 m(l, a) {
                     d(l, e, a), c(e, n), n.checked = t[2], c(e, r), i || (o = y(n, "change", t[27]), i = !0)
@@ -9049,18 +9102,18 @@
                 },
                 d(t) {
                     t && f(e), i = !1, o()
                 }
             }
         }
 
-        function Mu(t) {
+        function Pu(t) {
             let e, n, r, i = ht(t[39].data),
                 o = [];
-            for (let e = 0; e < i.length; e += 1) o[e] = Pu(xu(t, i, e));
+            for (let e = 0; e < i.length; e += 1) o[e] = Tu(Mu(t, i, e));
             return n = new Va({
                 props: {
                     scale: t[12],
                     x: t[14].left,
                     label: t[2] ? "percent" : "count",
                     format: t[2] ? Qe("~%") : In
                 }
@@ -9075,16 +9128,16 @@
                     for (let t = 0; t < o.length; t += 1) o[t] && o[t].m(e, null);
                     yt(n, t, i), r = !0
                 },
                 p(t, r) {
                     if (4744 & r[0]) {
                         let n;
                         for (i = ht(t[39].data), n = 0; n < i.length; n += 1) {
-                            const l = xu(t, i, n);
-                            o[n] ? o[n].p(l, r) : (o[n] = Pu(l), o[n].c(), o[n].m(e, null))
+                            const l = Mu(t, i, n);
+                            o[n] ? o[n].p(l, r) : (o[n] = Tu(l), o[n].c(), o[n].m(e, null))
                         }
                         for (; n < o.length; n += 1) o[n].d(1);
                         o.length = i.length
                     }
                     const l = {};
                     4096 & r[0] && (l.scale = t[12]), 4 & r[0] && (l.label = t[2] ? "percent" : "count"), 4 & r[0] && (l.format = t[2] ? Qe("~%") : In), n.$set(l)
                 },
@@ -9096,128 +9149,128 @@
                 },
                 d(t) {
                     t && f(e), h(o, t), $t(n, t)
                 }
             }
         }
 
-        function Lu(t) {
+        function Su(t) {
             let e, n, r, i, o;
             return {
                 c() {
-                    e = g("rect"), $(e, "x", n = Ou(t[45].data[0], t[9][t[39].feature]) + 1), $(e, "width", r = Cu(t[9][t[39].feature]) - 2), $(e, "y", i = t[12](t[45][1])), $(e, "height", o = t[12](t[45][0]) - t[12](t[45][1]))
+                    e = g("rect"), $(e, "x", n = Bu(t[45].data[0], t[9][t[39].feature]) + 1), $(e, "width", r = ju(t[9][t[39].feature]) - 2), $(e, "y", i = t[12](t[45][1])), $(e, "height", o = t[12](t[45][0]) - t[12](t[45][1]))
                 },
                 m(t, n) {
                     d(t, e, n)
                 },
                 p(t, l) {
-                    520 & l[0] && n !== (n = Ou(t[45].data[0], t[9][t[39].feature]) + 1) && $(e, "x", n), 520 & l[0] && r !== (r = Cu(t[9][t[39].feature]) - 2) && $(e, "width", r), 4104 & l[0] && i !== (i = t[12](t[45][1])) && $(e, "y", i), 4104 & l[0] && o !== (o = t[12](t[45][0]) - t[12](t[45][1])) && $(e, "height", o)
+                    520 & l[0] && n !== (n = Bu(t[45].data[0], t[9][t[39].feature]) + 1) && $(e, "x", n), 520 & l[0] && r !== (r = ju(t[9][t[39].feature]) - 2) && $(e, "width", r), 4104 & l[0] && i !== (i = t[12](t[45][1])) && $(e, "y", i), 4104 & l[0] && o !== (o = t[12](t[45][0]) - t[12](t[45][1])) && $(e, "height", o)
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Au(t) {
-            let e, n = t[45][0] !== t[45][1] && Lu(t);
+        function zu(t) {
+            let e, n = t[45][0] !== t[45][1] && Su(t);
             return {
                 c() {
                     n && n.c(), e = b()
                 },
                 m(t, r) {
                     n && n.m(t, r), d(t, e, r)
                 },
                 p(t, r) {
-                    t[45][0] !== t[45][1] ? n ? n.p(t, r) : (n = Lu(t), n.c(), n.m(e.parentNode, e)) : n && (n.d(1), n = null)
+                    t[45][0] !== t[45][1] ? n ? n.p(t, r) : (n = Su(t), n.c(), n.m(e.parentNode, e)) : n && (n.d(1), n = null)
                 },
                 d(t) {
                     t && f(e), n && n.d(t)
                 }
             }
         }
 
-        function Pu(t) {
+        function Tu(t) {
             let e, n, r = ht(t[42]),
                 i = [];
-            for (let e = 0; e < r.length; e += 1) i[e] = Au(_u(t, r, e));
+            for (let e = 0; e < r.length; e += 1) i[e] = zu(Lu(t, r, e));
             return {
                 c() {
                     e = g("g");
                     for (let t = 0; t < i.length; t += 1) i[t].c();
                     $(e, "fill", n = t[7](t[44]))
                 },
                 m(t, n) {
                     d(t, e, n);
                     for (let t = 0; t < i.length; t += 1) i[t] && i[t].m(e, null)
                 },
                 p(t, o) {
                     if (4616 & o[0]) {
                         let n;
                         for (r = ht(t[42]), n = 0; n < r.length; n += 1) {
-                            const l = _u(t, r, n);
-                            i[n] ? i[n].p(l, o) : (i[n] = Au(l), i[n].c(), i[n].m(e, null))
+                            const l = Lu(t, r, n);
+                            i[n] ? i[n].p(l, o) : (i[n] = zu(l), i[n].c(), i[n].m(e, null))
                         }
                         for (; n < i.length; n += 1) i[n].d(1);
                         i.length = r.length
                     }
                     128 & o[0] && n !== (n = t[7](t[44])) && $(e, "fill", n)
                 },
                 d(t) {
                     t && f(e), h(i, t)
                 }
             }
         }
 
-        function Su(t) {
-            let e, n, r, i, o, l, a = "categorical" === t[39].kind && Mu(t);
+        function Nu(t) {
+            let e, n, r, i, o, l, a = "categorical" === t[39].kind && Pu(t);
             return r = new Ma({
                 props: {
                     scale: t[9][t[39].feature],
                     y: t[8].bandwidth() - t[14].bottom,
                     showBaseline: !0,
                     baselineColor: "var(--gray-6)",
                     tickColor: "var(--gray-6)",
                     integerOnly: "discrete" === t[11][t[39].feature].subkind,
-                    value_map: Nu(t[11][t[39].feature]),
+                    value_map: Du(t[11][t[39].feature]),
                     label: t[39].feature
                 }
             }), {
                 c() {
                     e = g("g"), a && a.c(), n = g("g"), bt(r.$$.fragment), $(n, "class", "x-axis"), $(n, "id", i = "axis-" + t[39].feature), $(e, "transform", o = "translate(0," + t[8](t[39].feature) + ")")
                 },
                 m(t, i) {
                     d(t, e, i), a && a.m(e, null), c(e, n), yt(r, n, null), l = !0
                 },
                 p(t, s) {
-                    "categorical" === t[39].kind ? a ? (a.p(t, s), 8 & s[0] && dt(a, 1)) : (a = Mu(t), a.c(), dt(a, 1), a.m(e, n)) : a && (ct(), ft(a, 1, 1, (() => {
+                    "categorical" === t[39].kind ? a ? (a.p(t, s), 8 & s[0] && dt(a, 1)) : (a = Pu(t), a.c(), dt(a, 1), a.m(e, n)) : a && (ct(), ft(a, 1, 1, (() => {
                         a = null
                     })), ut());
                     const c = {};
-                    520 & s[0] && (c.scale = t[9][t[39].feature]), 256 & s[0] && (c.y = t[8].bandwidth() - t[14].bottom), 2056 & s[0] && (c.integerOnly = "discrete" === t[11][t[39].feature].subkind), 2056 & s[0] && (c.value_map = Nu(t[11][t[39].feature])), 8 & s[0] && (c.label = t[39].feature), r.$set(c), (!l || 8 & s[0] && i !== (i = "axis-" + t[39].feature)) && $(n, "id", i), (!l || 264 & s[0] && o !== (o = "translate(0," + t[8](t[39].feature) + ")")) && $(e, "transform", o)
+                    520 & s[0] && (c.scale = t[9][t[39].feature]), 256 & s[0] && (c.y = t[8].bandwidth() - t[14].bottom), 2056 & s[0] && (c.integerOnly = "discrete" === t[11][t[39].feature].subkind), 2056 & s[0] && (c.value_map = Du(t[11][t[39].feature])), 8 & s[0] && (c.label = t[39].feature), r.$set(c), (!l || 8 & s[0] && i !== (i = "axis-" + t[39].feature)) && $(n, "id", i), (!l || 264 & s[0] && o !== (o = "translate(0," + t[8](t[39].feature) + ")")) && $(e, "transform", o)
                 },
                 i(t) {
                     l || (dt(a), dt(r.$$.fragment, t), l = !0)
                 },
                 o(t) {
                     ft(a), ft(r.$$.fragment, t), l = !1
                 },
                 d(t) {
                     t && f(e), a && a.d(), $t(r)
                 }
             }
         }
 
-        function zu(t) {
+        function Cu(t) {
             let e, n, r, i, o, l, a, s, u, b, y, w, x, k, M, L, A = t[10].length + "",
                 S = 1 === t[10].length ? "instance" : "instances",
-                z = t[13].length > 0 && ku(t),
+                z = t[13].length > 0 && Au(t),
                 T = ht(t[3]),
                 N = [];
-            for (let e = 0; e < T.length; e += 1) N[e] = Su(wu(t, T, e));
+            for (let e = 0; e < T.length; e += 1) N[e] = Nu(ku(t, T, e));
             const C = t => ft(N[t], 1, 1, (() => {
                 N[t] = null
             }));
             return {
                 c() {
                     e = p("div"), n = p("div"), z && z.c(), r = v(), i = p("div"), o = m(A), l = v(), a = m(S), s = m(" selected"), u = v(), b = p("div"), y = p("canvas"), w = v(), x = g("svg"), k = g("g");
                     for (let t = 0; t < N.length; t += 1) N[t].c();
@@ -9225,19 +9278,19 @@
                 },
                 m(f, h) {
                     d(f, e, h), c(e, n), z && z.m(n, null), c(n, r), c(n, i), c(i, o), c(i, l), c(i, a), c(i, s), c(e, u), c(e, b), c(b, y), t[28](y), c(b, w), c(b, x), c(x, k);
                     for (let t = 0; t < N.length; t += 1) N[t] && N[t].m(k, null);
                     t[29](k), M = P.observe(b, t[30].bind(b)), L = !0
                 },
                 p(t, e) {
-                    if (t[13].length > 0 ? z ? z.p(t, e) : (z = ku(t), z.c(), z.m(n, r)) : z && (z.d(1), z = null), (!L || 1024 & e[0]) && A !== (A = t[10].length + "") && _(o, A), (!L || 1024 & e[0]) && S !== (S = 1 === t[10].length ? "instance" : "instances") && _(a, S), 23436 & e[0]) {
+                    if (t[13].length > 0 ? z ? z.p(t, e) : (z = Au(t), z.c(), z.m(n, r)) : z && (z.d(1), z = null), (!L || 1024 & e[0]) && A !== (A = t[10].length + "") && _(o, A), (!L || 1024 & e[0]) && S !== (S = 1 === t[10].length ? "instance" : "instances") && _(a, S), 23436 & e[0]) {
                         let n;
                         for (T = ht(t[3]), n = 0; n < T.length; n += 1) {
-                            const r = wu(t, T, n);
-                            N[n] ? (N[n].p(r, e), dt(N[n], 1)) : (N[n] = Su(r), N[n].c(), dt(N[n], 1), N[n].m(k, null))
+                            const r = ku(t, T, n);
+                            N[n] ? (N[n].p(r, e), dt(N[n], 1)) : (N[n] = Nu(r), N[n].c(), dt(N[n], 1), N[n].m(k, null))
                         }
                         for (ct(), n = T.length; n < N.length; n += 1) C(n);
                         ut()
                     }(!L || 1 & e[0]) && $(x, "width", t[0]), (!L || 64 & e[0]) && $(x, "height", t[6])
                 },
                 i(t) {
                     if (!L) {
@@ -9252,32 +9305,32 @@
                 },
                 d(n) {
                     n && f(e), z && z.d(), t[28](null), h(N, n), t[29](null), M()
                 }
             }
         }
 
-        function Tu(t) {
+        function Ou(t) {
             return "categorical" === t.kind
         }
 
-        function Nu(t) {
+        function Du(t) {
             return "value_map" in t ? t.value_map : {}
         }
 
-        function Cu(t) {
+        function ju(t) {
             return t && "bandwidth" in t ? t.bandwidth() : 0
         }
 
-        function Ou(t, e) {
+        function Bu(t, e) {
             var n;
             return e && null !== (n = e(t)) && void 0 !== n ? n : 0
         }
 
-        function Du(t, e, n) {
+        function Eu(t, e, n) {
             let r, i, o, l, s, c, u, d, f, h, p, g, m, v, b, y, $;
             E(t, Qn, (t => n(25, b = t))), E(t, Zn, (t => n(11, y = t))), E(t, er, (t => n(26, $ = t)));
             let {
                 pd: w
             } = e, {
                 features: x
             } = e;
@@ -9361,40 +9414,40 @@
             return F((() => {
                 O && n(18, D = O.getContext("2d"))
             })), t.$$set = t => {
                 "pd" in t && n(15, w = t.pd), "features" in t && n(16, x = t.features)
             }, t.$$.update = () => {
                 2 & t.$$.dirty[0] && n(0, M = k ? k.width : 0), 2 & t.$$.dirty[0] && n(17, L = k ? k.height : 0), 229376 & t.$$.dirty[0] && n(6, r = Math.max(L, x.length * (30 * w.ice.num_clusters + _.top + _.bottom))), 32768 & t.$$.dirty[0] && n(23, i = zn(w).cluster_labels), 32768 & t.$$.dirty[0] && n(21, o = _n(w.ice.num_clusters)), 67584 & t.$$.dirty[0] && n(13, l = x.filter((t => "categorical" === y[t].kind))), 2097152 & t.$$.dirty[0] && n(7, s = Er().domain(o).range(Un)), 65600 & t.$$.dirty[0] && n(8, c = Ir().domain(x).range([0, r])), 67108864 & t.$$.dirty[0] && (u = _n($)), 67108864 & t.$$.dirty[0] && n(10, d = _n($)), 2097156 & t.$$.dirty[0] && n(24, f = function() {
                     var t = Gr([]),
-                        e = gu,
-                        n = pu,
-                        r = mu;
+                        e = bu,
+                        n = vu,
+                        r = yu;
 
                     function i(i) {
-                        var o, l, a = Array.from(t.apply(this, arguments), vu),
+                        var o, l, a = Array.from(t.apply(this, arguments), $u),
                             s = a.length,
                             c = -1;
                         for (const t of i)
                             for (o = 0, ++c; o < s; ++o)(a[o][c] = [0, +r(t, a[o].key, c, i)]).data = t;
                         for (o = 0, l = Yr(e(a)); o < s; ++o) a[l[o]].index = o;
                         return n(a, l), a
                     }
                     return i.keys = function(e) {
                         return arguments.length ? (t = "function" == typeof e ? e : Gr(Array.from(e)), i) : t
                     }, i.value = function(t) {
                         return arguments.length ? (r = "function" == typeof t ? t : Gr(+t), i) : r
                     }, i.order = function(t) {
-                        return arguments.length ? (e = null == t ? gu : "function" == typeof t ? t : Gr(Array.from(t)), i) : e
+                        return arguments.length ? (e = null == t ? bu : "function" == typeof t ? t : Gr(Array.from(t)), i) : e
                     }, i.offset = function(t) {
-                        return arguments.length ? (n = null == t ? pu : t, i) : n
+                        return arguments.length ? (n = null == t ? vu : t, i) : n
                     }, i
                 }().keys(o).value(((t, e) => {
                     var n;
                     return null !== (n = t[1].get(e)) && void 0 !== n ? n : 0
-                })).offset(A ? bu : pu).order(yu)), 67585 & t.$$.dirty[0] && n(9, h = Object.fromEntries(x.map((t => {
+                })).offset(A ? wu : vu).order(xu)), 67585 & t.$$.dirty[0] && n(9, h = Object.fromEntries(x.map((t => {
                     const e = y[t];
                     return [t, "quantitative" === e.kind ? on().domain([e.values[0], e.values[e.values.length - 1]]).range([_.left, M - _.right]) : Ir().domain(e.values).range([_.left, M - _.right])]
                 })))), 58788864 & t.$$.dirty[0] && n(3, P = x.map((t => {
                     if ("categorical" === y[t].kind) {
                         const e = wn(d, (t => t.length), (e => b[t][e]), (t => i[t]));
                         return {
                             feature: t,
@@ -9408,15 +9461,15 @@
                             kind: "quantitative",
                             data: Array.from(e, (([t, e]) => ({
                                 cluster: t,
                                 raincloud: e
                             })))
                         }
                     }
-                }))), 8 & t.$$.dirty[0] && n(22, p = Math.max(...P.filter(Tu).map((t => t.data)).flat(3))), 4194564 & t.$$.dirty[0] && n(12, g = on().domain([0, A ? 1 : p]).range([c.bandwidth() - _.bottom, _.top])), 2097408 & t.$$.dirty[0] && n(19, m = Ir().domain(o).range([_.top, c.bandwidth() - _.bottom]).paddingInner(.2).paddingOuter(.1)), 257 & t.$$.dirty[0] && n(20, v = ia().extent([
+                }))), 8 & t.$$.dirty[0] && n(22, p = Math.max(...P.filter(Ou).map((t => t.data)).flat(3))), 4194564 & t.$$.dirty[0] && n(12, g = on().domain([0, A ? 1 : p]).range([c.bandwidth() - _.bottom, _.top])), 2097408 & t.$$.dirty[0] && n(19, m = Ir().domain(o).range([_.top, c.bandwidth() - _.bottom]).paddingInner(.2).paddingOuter(.1)), 257 & t.$$.dirty[0] && n(20, v = ia().extent([
                     [_.left, -4 + c.bandwidth() - _.bottom],
                     [M - _.right, 4 + c.bandwidth() - _.bottom]
                 ]).on("start brush end", T)), 1114129 & t.$$.dirty[0] && N && x && M > 0 && async function(t) {
                     N && (await Q(), C = wo(N).selectAll(".x-axis"), C.call(t), C.call(t.clear))
                 }(v), 262241 & t.$$.dirty[0] && O && D && (En(O, D, M, r), j(D, h, c, m, s, P, M, r)), 787401 & t.$$.dirty[0] && j(D, h, c, m, s, P, M, r)
             }, [M, k, A, P, N, O, r, s, c, h, d, y, g, l, _, w, x, L, D, m, v, o, p, i, f, b, $, function() {
                 A = this.checked, n(2, A)
@@ -9428,31 +9481,31 @@
                 X[t ? "unshift" : "push"]((() => {
                     N = t, n(4, N)
                 }))
             }, function() {
                 k = a.entries.get(this)?.contentRect, n(1, k)
             }]
         }
-        const ju = class extends _t {
+        const Iu = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Du, zu, j, {
+                super(), wt(this, t, Eu, Cu, j, {
                     pd: 15,
                     features: 16
-                }, $u, [-1, -1])
+                }, _u, [-1, -1])
             }
         };
 
-        function Bu(t) {
+        function Ru(t) {
             u(t, "svelte-2s8sz0", ".pdpilot-plot-container.svelte-2s8sz0{width:100%;height:100%;position:relative}svg.svelte-2s8sz0,canvas.svelte-2s8sz0{position:absolute;top:var(--top);left:0}")
         }
 
-        function Eu(t) {
+        function Vu(t) {
             let e, n, r, i, o = t[21].left - t[28] + "px",
                 l = `${t[22]}px`;
-            const a = [Ru, Iu],
+            const a = [qu, Hu],
                 s = [];
 
             function c(t, e) {
                 return "interpolator" in t[18] ? 0 : 1
             }
             return n = c(t), r = s[n] = a[n](t), {
                 c() {
@@ -9475,23 +9528,23 @@
                 },
                 d(t) {
                     t && f(e), s[n].d()
                 }
             }
         }
 
-        function Iu(t) {
+        function Hu(t) {
             let e, n;
-            return e = new Yc({
+            return e = new Zc({
                 props: {
                     width: t[23] + t[27],
-                    height: Zu,
+                    height: ed,
                     color: t[18],
-                    marginLeft: Qu,
-                    marginRight: Qu,
+                    marginLeft: nd,
+                    marginRight: nd,
                     title: t[3]
                 }
             }), {
                 c() {
                     bt(e.$$.fragment)
                 },
                 m(t, r) {
@@ -9509,23 +9562,23 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Ru(t) {
+        function qu(t) {
             let e, n;
             return e = new wc({
                 props: {
                     width: t[23] + t[27],
-                    height: Zu,
+                    height: ed,
                     color: t[18],
-                    marginLeft: Qu,
-                    marginRight: Qu,
+                    marginLeft: nd,
+                    marginRight: nd,
                     title: t[3]
                 }
             }), {
                 c() {
                     bt(e.$$.fragment)
                 },
                 m(t, r) {
@@ -9543,31 +9596,31 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Vu(t) {
-            let e, n, r, i, o = t[16] && t[24].length > 0 && Hu(t),
-                l = t[8] && Wu(t),
-                a = t[9] && Uu(t);
+        function Fu(t) {
+            let e, n, r, i, o = t[16] && t[24].length > 0 && Wu(t),
+                l = t[8] && Uu(t),
+                a = t[9] && Ju(t);
             return {
                 c() {
                     o && o.c(), e = b(), l && l.c(), n = b(), a && a.c(), r = b()
                 },
                 m(t, s) {
                     o && o.m(t, s), d(t, e, s), l && l.m(t, s), d(t, n, s), a && a.m(t, s), d(t, r, s), i = !0
                 },
                 p(t, i) {
-                    t[16] && t[24].length > 0 ? o ? (o.p(t, i), 16842752 & i[0] && dt(o, 1)) : (o = Hu(t), o.c(), dt(o, 1), o.m(e.parentNode, e)) : o && (ct(), ft(o, 1, 1, (() => {
+                    t[16] && t[24].length > 0 ? o ? (o.p(t, i), 16842752 & i[0] && dt(o, 1)) : (o = Wu(t), o.c(), dt(o, 1), o.m(e.parentNode, e)) : o && (ct(), ft(o, 1, 1, (() => {
                         o = null
-                    })), ut()), t[8] ? l ? (l.p(t, i), 256 & i[0] && dt(l, 1)) : (l = Wu(t), l.c(), dt(l, 1), l.m(n.parentNode, n)) : l && (ct(), ft(l, 1, 1, (() => {
+                    })), ut()), t[8] ? l ? (l.p(t, i), 256 & i[0] && dt(l, 1)) : (l = Uu(t), l.c(), dt(l, 1), l.m(n.parentNode, n)) : l && (ct(), ft(l, 1, 1, (() => {
                         l = null
-                    })), ut()), t[9] ? a ? (a.p(t, i), 512 & i[0] && dt(a, 1)) : (a = Uu(t), a.c(), dt(a, 1), a.m(r.parentNode, r)) : a && (ct(), ft(a, 1, 1, (() => {
+                    })), ut()), t[9] ? a ? (a.p(t, i), 512 & i[0] && dt(a, 1)) : (a = Ju(t), a.c(), dt(a, 1), a.m(r.parentNode, r)) : a && (ct(), ft(a, 1, 1, (() => {
                         a = null
                     })), ut())
                 },
                 i(t) {
                     i || (dt(o), dt(l), dt(a), i = !0)
                 },
                 o(t) {
@@ -9575,17 +9628,17 @@
                 },
                 d(t) {
                     t && (f(e), f(n), f(r)), o && o.d(t), l && l.d(t), a && a.d(t)
                 }
             }
         }
 
-        function Hu(t) {
+        function Wu(t) {
             let e, n, r, i;
-            const o = [Fu, qu],
+            const o = [Xu, Ku],
                 l = [];
 
             function a(t, e) {
                 return "bandwidth" in t[20] ? 0 : 1
             }
             return e = a(t), n = l[e] = o[e](t), {
                 c() {
@@ -9608,15 +9661,15 @@
                 },
                 d(t) {
                     t && f(r), l[e].d(t)
                 }
             }
         }
 
-        function qu(t) {
+        function Ku(t) {
             let e, n;
             return e = new Qa({
                 props: {
                     data: t[16],
                     fill: Kn,
                     x: t[20],
                     height: t[13],
@@ -9644,15 +9697,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Fu(t) {
+        function Xu(t) {
             let e, n;
             return e = new ds({
                 props: {
                     data: t[16],
                     fill: Kn,
                     x: t[20],
                     height: t[13],
@@ -9680,17 +9733,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Wu(t) {
+        function Uu(t) {
             let e, n, r, i;
-            const o = [Xu, Ku],
+            const o = [Gu, Yu],
                 l = [];
 
             function a(t, e) {
                 return "bandwidth" in t[20] ? 0 : 1
             }
             return e = a(t), n = l[e] = o[e](t), {
                 c() {
@@ -9713,15 +9766,15 @@
                 },
                 d(t) {
                     t && f(r), l[e].d(t)
                 }
             }
         }
 
-        function Ku(t) {
+        function Yu(t) {
             let e, n;
             return e = new Qa({
                 props: {
                     data: t[8],
                     fill: t[26] ? "none" : "var(--gray-3)",
                     stroke: t[26] ? "var(--black)" : "none",
                     x: t[20],
@@ -9750,15 +9803,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Xu(t) {
+        function Gu(t) {
             let e, n;
             return e = new ds({
                 props: {
                     data: t[8],
                     fill: t[26] ? "none" : "var(--gray-3)",
                     stroke: t[26] ? "var(--black)" : "none",
                     x: t[20],
@@ -9787,17 +9840,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Uu(t) {
+        function Ju(t) {
             let e, n, r, i;
-            const o = [Gu, Yu],
+            const o = [Qu, Zu],
                 l = [];
 
             function a(t, e) {
                 return "bandwidth" in t[19] ? 0 : 1
             }
             return e = a(t), n = l[e] = o[e](t), {
                 c() {
@@ -9820,15 +9873,15 @@
                 },
                 d(t) {
                     t && f(r), l[e].d(t)
                 }
             }
         }
 
-        function Yu(t) {
+        function Zu(t) {
             let e, n;
             return e = new Qa({
                 props: {
                     data: t[9],
                     x: t[19],
                     height: t[13],
                     direction: "vertical",
@@ -9853,15 +9906,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Gu(t) {
+        function Qu(t) {
             let e, n;
             return e = new ds({
                 props: {
                     data: t[9],
                     x: t[19],
                     height: t[13],
                     direction: "vertical",
@@ -9886,17 +9939,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Ju(t) {
-            let e, n, r, i, o, l, a, s, u, h = `${Zu+t[22]}px`,
-                m = "" !== t[3] && Eu(t);
+        function td(t) {
+            let e, n, r, i, o, l, a, s, u, h = `${ed+t[22]}px`,
+                m = "" !== t[3] && Vu(t);
             l = new Ma({
                 props: {
                     scale: t[20],
                     y: t[17] - t[21].bottom,
                     label: t[1],
                     integerOnly: t[4],
                     value_map: t[6]
@@ -9906,48 +9959,48 @@
                     scale: t[19],
                     x: t[21].left,
                     label: t[2],
                     integerOnly: t[5],
                     value_map: t[7]
                 }
             });
-            let b = t[10] && Vu(t);
+            let b = t[10] && Fu(t);
             return {
                 c() {
                     e = p("div"), m && m.c(), n = v(), r = p("canvas"), i = v(), o = g("svg"), bt(l.$$.fragment), bt(a.$$.fragment), s = g("g"), b && b.c(), $(r, "class", "svelte-2s8sz0"), $(o, "width", t[0]), $(o, "height", t[17]), $(o, "class", "svelte-2s8sz0"), $(e, "class", "pdpilot-plot-container svelte-2s8sz0"), M(e, "--top", h)
                 },
                 m(f, h) {
                     d(f, e, h), m && m.m(e, null), c(e, n), c(e, r), t[53](r), c(e, i), c(e, o), yt(l, o, null), yt(a, o, null), c(o, s), t[54](s), b && b.m(o, null), u = !0
                 },
                 p(t, r) {
-                    "" !== t[3] ? m ? (m.p(t, r), 8 & r[0] && dt(m, 1)) : (m = Eu(t), m.c(), dt(m, 1), m.m(e, n)) : m && (ct(), ft(m, 1, 1, (() => {
+                    "" !== t[3] ? m ? (m.p(t, r), 8 & r[0] && dt(m, 1)) : (m = Vu(t), m.c(), dt(m, 1), m.m(e, n)) : m && (ct(), ft(m, 1, 1, (() => {
                         m = null
                     })), ut());
                     const i = {};
                     1048576 & r[0] && (i.scale = t[20]), 2228224 & r[0] && (i.y = t[17] - t[21].bottom), 2 & r[0] && (i.label = t[1]), 16 & r[0] && (i.integerOnly = t[4]), 64 & r[0] && (i.value_map = t[6]), l.$set(i);
                     const s = {};
-                    524288 & r[0] && (s.scale = t[19]), 2097152 & r[0] && (s.x = t[21].left), 4 & r[0] && (s.label = t[2]), 32 & r[0] && (s.integerOnly = t[5]), 128 & r[0] && (s.value_map = t[7]), a.$set(s), t[10] ? b ? (b.p(t, r), 1024 & r[0] && dt(b, 1)) : (b = Vu(t), b.c(), dt(b, 1), b.m(o, null)) : b && (ct(), ft(b, 1, 1, (() => {
+                    524288 & r[0] && (s.scale = t[19]), 2097152 & r[0] && (s.x = t[21].left), 4 & r[0] && (s.label = t[2]), 32 & r[0] && (s.integerOnly = t[5]), 128 & r[0] && (s.value_map = t[7]), a.$set(s), t[10] ? b ? (b.p(t, r), 1024 & r[0] && dt(b, 1)) : (b = Fu(t), b.c(), dt(b, 1), b.m(o, null)) : b && (ct(), ft(b, 1, 1, (() => {
                         b = null
-                    })), ut()), (!u || 1 & r[0]) && $(o, "width", t[0]), (!u || 131072 & r[0]) && $(o, "height", t[17]), 4194304 & r[0] && h !== (h = `${Zu+t[22]}px`) && M(e, "--top", h)
+                    })), ut()), (!u || 1 & r[0]) && $(o, "width", t[0]), (!u || 131072 & r[0]) && $(o, "height", t[17]), 4194304 & r[0] && h !== (h = `${ed+t[22]}px`) && M(e, "--top", h)
                 },
                 i(t) {
                     u || (dt(m), dt(l.$$.fragment, t), dt(a.$$.fragment, t), dt(b), u = !0)
                 },
                 o(t) {
                     ft(m), ft(l.$$.fragment, t), ft(a.$$.fragment, t), ft(b), u = !1
                 },
                 d(n) {
                     n && f(e), m && m.d(), t[53](null), $t(l), $t(a), t[54](null), b && b.d()
                 }
             }
         }
-        const Zu = 24,
-            Qu = 10;
+        const ed = 24,
+            nd = 10;
 
-        function td(t, e, n) {
+        function rd(t, e, n) {
             let r, i, o, l, a, s, c, u, d, f, h, p, g, m, v, b, y, $, w, x, _;
             E(t, kr, (t => n(50, y = t))), E(t, fr, (t => n(24, $ = t))), E(t, Pr, (t => n(51, w = t))), E(t, Mr, (t => n(52, x = t))), E(t, Lr, (t => n(56, _ = t)));
             let k, M, {
                     width: L
                 } = e,
                 {
                     height: A
@@ -10088,36 +10141,36 @@
                 "width" in t && n(0, L = t.width), "height" in t && n(29, A = t.height), "xValues" in t && n(30, P = t.xValues), "yValues" in t && n(31, S = t.yValues), "colorValues" in t && n(32, z = t.colorValues), "xKind" in t && n(33, T = t.xKind), "yKind" in t && n(34, N = t.yKind), "colorKind" in t && n(35, C = t.colorKind), "xDomain" in t && n(36, O = t.xDomain), "yDomain" in t && n(37, D = t.yDomain), "colorDomain" in t && n(38, j = t.colorDomain), "colorScheme" in t && n(39, B = t.colorScheme), "xLabel" in t && n(1, I = t.xLabel), "yLabel" in t && n(2, V = t.yLabel), "colorLabel" in t && n(3, H = t.colorLabel), "xAxisIntegerOnly" in t && n(4, q = t.xAxisIntegerOnly), "yAxisIntegerOnly" in t && n(5, W = t.yAxisIntegerOnly), "xAxisValueMap" in t && n(6, K = t.xAxisValueMap), "yAxisValueMap" in t && n(7, U = t.yAxisValueMap), "xDistribution" in t && n(8, Y = t.xDistribution), "yDistribution" in t && n(9, G = t.yDistribution), "opacity" in t && n(40, J = t.opacity), "allowBrushing" in t && n(41, Z = t.allowBrushing), "showMarginalDistribution" in t && n(10, Q = t.showMarginalDistribution), "marginTop" in t && n(11, tt = t.marginTop), "marginRight" in t && n(12, et = t.marginRight), "marginalPlotHeight" in t && n(13, nt = t.marginalPlotHeight)
             }, t.$$.update = () => {
                 6144 & t.$$.dirty[0] && n(48, r = {
                     top: tt,
                     right: et,
                     bottom: 35,
                     left: 50
-                }), 536870913 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(23, i = Math.min(L - r.left - r.right, A - Zu - r.top - r.bottom)), 8388609 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(47, o = (L - i - r.left - r.right) / 2), 545259520 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(49, l = (A - Zu - i - r.top - r.bottom) / 2), 8 & t.$$.dirty[0] && n(28, a = "" === H ? Qu : 0), 8 & t.$$.dirty[0] && n(27, s = "" === H ? 2 * Qu : Qu), 8 & t.$$.dirty[0] | 262144 & t.$$.dirty[1] && n(22, c = "" !== H ? l : 0), 4194304 & t.$$.dirty[0] | 458752 & t.$$.dirty[1] && n(21, u = {
+                }), 536870913 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(23, i = Math.min(L - r.left - r.right, A - ed - r.top - r.bottom)), 8388609 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(47, o = (L - i - r.left - r.right) / 2), 545259520 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(49, l = (A - ed - i - r.top - r.bottom) / 2), 8 & t.$$.dirty[0] && n(28, a = "" === H ? nd : 0), 8 & t.$$.dirty[0] && n(27, s = "" === H ? 2 * nd : nd), 8 & t.$$.dirty[0] | 262144 & t.$$.dirty[1] && n(22, c = "" !== H ? l : 0), 4194304 & t.$$.dirty[0] | 458752 & t.$$.dirty[1] && n(21, u = {
                     top: r.top + l - c,
                     right: r.right + o,
                     bottom: r.bottom + l,
                     left: r.left + o
-                }), 541065216 & t.$$.dirty[0] && n(17, d = Math.max(A - Zu - c, 0)), 2097153 & t.$$.dirty[0] | 36 & t.$$.dirty[1] && n(20, f = "quantitative" === T ? on().domain(O).range([u.left, L - u.right]) : Ir().domain(O).paddingInner(.25).range([u.left, L - u.right])), 2228224 & t.$$.dirty[0] | 72 & t.$$.dirty[1] && n(19, h = "quantitative" === N ? on().domain(D).range([d - u.bottom, u.top]) : Ir().domain(D).paddingInner(.25).range([d - u.bottom, u.top])), 400 & t.$$.dirty[1] && n(18, p = "quantitative" === C ? an().domain(j).interpolator((t => Rc(rt(t)))) : Er().domain(j).range("highlight" === B ? ["rgb(145, 145, 145)", Kn] : ["#db5c39", "#5c39db"])), 1073741824 & t.$$.dirty[0] && (g = _n(P.length)), 2228225 & t.$$.dirty[0] && n(46, m = oa().extent([
+                }), 541065216 & t.$$.dirty[0] && n(17, d = Math.max(A - ed - c, 0)), 2097153 & t.$$.dirty[0] | 36 & t.$$.dirty[1] && n(20, f = "quantitative" === T ? on().domain(O).range([u.left, L - u.right]) : Ir().domain(O).paddingInner(.25).range([u.left, L - u.right])), 2228224 & t.$$.dirty[0] | 72 & t.$$.dirty[1] && n(19, h = "quantitative" === N ? on().domain(D).range([d - u.bottom, u.top]) : Ir().domain(D).paddingInner(.25).range([d - u.bottom, u.top])), 400 & t.$$.dirty[1] && n(18, p = "quantitative" === C ? an().domain(j).interpolator((t => qc(rt(t)))) : Er().domain(j).range("highlight" === B ? ["rgb(145, 145, 145)", Kn] : ["#db5c39", "#5c39db"])), 1073741824 & t.$$.dirty[0] && (g = _n(P.length)), 2228225 & t.$$.dirty[0] && n(46, m = oa().extent([
                     [u.left - 2, u.top - 2],
                     [L - u.right + 2, d - u.bottom + 2]
                 ]).on("start", ct).on("brush", ut).on("end", dt)), 163841 & t.$$.dirty[0] | 50176 & t.$$.dirty[1] && it && Z && L > 0 && d > 0 && (n(45, ot = wo(it)), ot.call(m)), 2158592 & t.$$.dirty[1] && ot && x && at && !st && ot.call(m.clear), 2 & t.$$.dirty[0] | 1049600 & t.$$.dirty[1] && n(16, lt = Z ? w.get(I) : void 0), 16842752 & t.$$.dirty[0] && n(26, v = lt && $.length > 0), 65792 & t.$$.dirty[0] && n(25, b = Y ? Hn(Y, lt) : 0), 147457 & t.$$.dirty[0] | 2048 & t.$$.dirty[1] && k && M && (En(k, M, L, d), dc(M, f, h, p, P, S, z, y, L, d, 2, J)), 1075707905 & t.$$.dirty[0] | 526851 & t.$$.dirty[1] && dc(M, f, h, p, P, S, z, y, L, d, 2, J)
             }, [L, I, V, H, q, W, K, U, Y, G, Q, tt, et, nt, k, it, lt, d, p, h, f, u, c, i, $, b, v, s, a, A, P, S, z, T, N, C, O, D, j, B, J, Z, M, at, st, ot, m, o, r, l, y, w, x, function(t) {
                 X[t ? "unshift" : "push"]((() => {
                     k = t, n(14, k)
                 }))
             }, function(t) {
                 X[t ? "unshift" : "push"]((() => {
                     it = t, n(15, it)
                 }))
             }]
         }
-        const ed = class extends _t {
+        const id = class extends _t {
             constructor(t) {
-                super(), wt(this, t, td, Ju, j, {
+                super(), wt(this, t, rd, td, j, {
                     width: 0,
                     height: 29,
                     xValues: 30,
                     yValues: 31,
                     colorValues: 32,
                     xKind: 33,
                     yKind: 34,
@@ -10137,28 +10190,28 @@
                     yDistribution: 9,
                     opacity: 40,
                     allowBrushing: 41,
                     showMarginalDistribution: 10,
                     marginTop: 11,
                     marginRight: 12,
                     marginalPlotHeight: 13
-                }, Bu, [-1, -1])
+                }, Ru, [-1, -1])
             }
         };
 
-        function nd(t) {
+        function od(t) {
             u(t, "svelte-tm4cy6", ".segmented-control-container.svelte-tm4cy6.svelte-tm4cy6{display:flex;gap:0.25em;align-items:center}.segmented-control-buttons-row.svelte-tm4cy6.svelte-tm4cy6{display:inline-grid;grid-auto-columns:1fr;grid-auto-flow:column}.segmented-control-buttons-row.svelte-tm4cy6 button.svelte-tm4cy6{border-radius:0;border-left:none;padding:0.0625em 0.125em}.segmented-control-buttons-row.svelte-tm4cy6 button.svelte-tm4cy6:first-child{border-top-left-radius:0.25em;border-bottom-left-radius:0.25em;border-left:1px solid var(--blue)}.segmented-control-buttons-row.svelte-tm4cy6 button.svelte-tm4cy6:last-child{border-top-right-radius:0.25em;border-bottom-right-radius:0.25em}.segmented-control-buttons-row.svelte-tm4cy6 button.selected-segment.svelte-tm4cy6{color:white;background-color:var(--blue)}.segmented-control-buttons-row.svelte-tm4cy6 button.selected-segment.svelte-tm4cy6:active{color:white;background-color:var(--dark-blue);border-color:var(--dark-blue)}")
         }
 
-        function rd(t, e, n) {
+        function ld(t, e, n) {
             const r = t.slice();
             return r[5] = e[n].value, r[6] = e[n].label, r[7] = e[n].enabled, r
         }
 
-        function id(t) {
+        function ad(t) {
             let e, n;
             return {
                 c() {
                     e = p("div"), n = m(t[2]), $(e, "class", "pdpilot-bold")
                 },
                 m(t, r) {
                     d(t, e, r), c(e, n)
@@ -10168,15 +10221,15 @@
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function od(t) {
+        function sd(t) {
             let e, n, r, i, o, l = t[6] + "";
 
             function a() {
                 return t[4](t[5])
             }
             return {
                 c() {
@@ -10190,49 +10243,49 @@
                 },
                 d(t) {
                     t && f(e), i = !1, o()
                 }
             }
         }
 
-        function ld(t) {
-            let e, n, r, i = t[2] && id(t),
+        function cd(t) {
+            let e, n, r, i = t[2] && ad(t),
                 o = ht(t[1]),
                 l = [];
-            for (let e = 0; e < o.length; e += 1) l[e] = od(rd(t, o, e));
+            for (let e = 0; e < o.length; e += 1) l[e] = sd(ld(t, o, e));
             return {
                 c() {
                     e = p("div"), i && i.c(), n = v(), r = p("div");
                     for (let t = 0; t < l.length; t += 1) l[t].c();
                     $(r, "class", "segmented-control-buttons-row svelte-tm4cy6"), $(e, "class", "segmented-control-container svelte-tm4cy6")
                 },
                 m(t, o) {
                     d(t, e, o), i && i.m(e, null), c(e, n), c(e, r);
                     for (let t = 0; t < l.length; t += 1) l[t] && l[t].m(r, null)
                 },
                 p(t, [a]) {
-                    if (t[2] ? i ? i.p(t, a) : (i = id(t), i.c(), i.m(e, n)) : i && (i.d(1), i = null), 11 & a) {
+                    if (t[2] ? i ? i.p(t, a) : (i = ad(t), i.c(), i.m(e, n)) : i && (i.d(1), i = null), 11 & a) {
                         let e;
                         for (o = ht(t[1]), e = 0; e < o.length; e += 1) {
-                            const n = rd(t, o, e);
-                            l[e] ? l[e].p(n, a) : (l[e] = od(n), l[e].c(), l[e].m(r, null))
+                            const n = ld(t, o, e);
+                            l[e] ? l[e].p(n, a) : (l[e] = sd(n), l[e].c(), l[e].m(r, null))
                         }
                         for (; e < l.length; e += 1) l[e].d(1);
                         l.length = o.length
                     }
                 },
                 i: T,
                 o: T,
                 d(t) {
                     t && f(e), i && i.d(), h(l, t)
                 }
             }
         }
 
-        function ad(t, e, n) {
+        function ud(t, e, n) {
             let {
                 segments: r
             } = e, {
                 selectedValue: i
             } = e, {
                 title: o = ""
             } = e;
@@ -10240,46 +10293,46 @@
             function l(t) {
                 n(0, i = t)
             }
             return t.$$set = t => {
                 "segments" in t && n(1, r = t.segments), "selectedValue" in t && n(0, i = t.selectedValue), "title" in t && n(2, o = t.title)
             }, [i, r, o, l, t => l(t)]
         }
-        const sd = class extends _t {
+        const dd = class extends _t {
             constructor(t) {
-                super(), wt(this, t, ad, ld, j, {
+                super(), wt(this, t, ud, cd, j, {
                     segments: 1,
                     selectedValue: 0,
                     title: 2
-                }, nd)
+                }, od)
             }
         };
 
-        function cd(t) {
+        function fd(t) {
             u(t, "svelte-a1f3se", ".one-way-detailed-pdp-container.svelte-a1f3se{display:flex;width:100%;height:100%}.pdpilot-no-clusters-message.svelte-a1f3se{flex:1;text-align:center;align-self:center}.pdpilot-half.svelte-a1f3se{flex:1;display:flex;flex-direction:column}.pdpilot-half-vis.svelte-a1f3se{flex:1}.pdpilot-vertical-divider.svelte-a1f3se{width:1px;margin:0 1em;background-color:var(--gray-1)}")
         }
 
-        function ud(t) {
+        function hd(t) {
             let e, n, r, i, o, l, a, s, u, h, g, m, b, y, w, x, _, k, L, A, S, z = ("cluster-lines" === t[5] ? .25 : .5) + "em",
                 T = ("cluster-descriptions" === t[4] ? .25 : .5) + "em";
 
             function N(e) {
                 t[21](e)
             }
             let C = {
                 segments: t[19],
                 title: "ICE Plot"
             };
 
             function O(e) {
                 t[23](e)
             }
-            void 0 !== t[5] && (C.selectedValue = t[5]), r = new sd({
+            void 0 !== t[5] && (C.selectedValue = t[5]), r = new dd({
                 props: C
-            }), X.push((() => vt(r, "selectedValue", N))), a = new hu({
+            }), X.push((() => vt(r, "selectedValue", N))), a = new mu({
                 props: {
                     pd: t[0],
                     width: t[11],
                     height: t[10],
                     scaleLocally: t[12],
                     showMarginalDistribution: !1,
                     marginTop: "cluster-lines" === t[5] ? 0 : 10,
@@ -10290,18 +10343,18 @@
                     showColorLegend: !1
                 }
             });
             let D = {
                 segments: t[6],
                 title: "Context"
             };
-            void 0 !== t[4] && (D.selectedValue = t[4]), y = new sd({
+            void 0 !== t[4] && (D.selectedValue = t[4]), y = new dd({
                 props: D
             }), X.push((() => vt(y, "selectedValue", O)));
-            const j = [hd, fd],
+            const j = [md, gd],
                 B = [];
 
             function E(t, e) {
                 return "cluster-descriptions" === t[4] ? 0 : "scatterplot" === t[4] ? 1 : -1
             }
             return ~(k = E(t)) && (L = B[k] = j[k](t)), {
                 c() {
@@ -10330,15 +10383,15 @@
                 },
                 d(t) {
                     t && (f(e), f(u), f(h), f(g), f(m)), $t(r), $t(a), s(), $t(y), ~k && B[k].d(), A()
                 }
             }
         }
 
-        function dd(t) {
+        function pd(t) {
             let e;
             return {
                 c() {
                     e = p("div"), e.textContent = "This feature does not have enough distinct clusters of ICE lines.", $(e, "class", "pdpilot-no-clusters-message svelte-a1f3se")
                 },
                 m(t, n) {
                     d(t, e, n)
@@ -10348,17 +10401,17 @@
                 o: T,
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function fd(t) {
+        function gd(t) {
             let e, n;
-            return e = new ed({
+            return e = new id({
                 props: {
                     width: t[9],
                     height: t[8],
                     xValues: t[13][t[0].x_feature],
                     yValues: t[14],
                     colorValues: Array.from({
                         length: t[15]
@@ -10367,28 +10420,28 @@
                     yKind: t[17] ? "categorical" : "quantitative",
                     colorKind: "categorical",
                     xDomain: "categorical" === t[1].kind ? t[0].x_values : [t[0].x_values[0], t[0].x_values[t[0].x_values.length - 1]],
                     yDomain: t[18],
                     colorDomain: [0, 1],
                     colorScheme: "highlight",
                     xLabel: t[0].x_feature,
-                    yLabel: "Ground Truth",
+                    yLabel: "Ground truth",
                     colorLabel: "",
                     xAxisIntegerOnly: "discrete" === t[1].subkind,
                     yAxisIntegerOnly: !1,
                     xAxisValueMap: "value_map" in t[1] ? t[1].value_map : {},
                     yAxisValueMap: {},
                     xDistribution: t[1].distribution,
                     yDistribution: null,
                     opacity: .5,
                     allowBrushing: !0,
                     showMarginalDistribution: !0,
-                    marginTop: gd + 3,
-                    marginRight: gd + 3,
-                    marginalPlotHeight: gd
+                    marginTop: bd + 3,
+                    marginRight: bd + 3,
+                    marginalPlotHeight: bd
                 }
             }), {
                 c() {
                     bt(e.$$.fragment)
                 },
                 m(t, r) {
                     yt(e, t, r), n = !0
@@ -10407,17 +10460,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function hd(t) {
+        function md(t) {
             let e, n;
-            return e = new ju({
+            return e = new Iu({
                 props: {
                     pd: t[0],
                     features: zn(t[0]).interacting_features
                 }
             }), e.$on("filter", t[20]), {
                 c() {
                     bt(e.$$.fragment)
@@ -10437,17 +10490,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function pd(t) {
+        function vd(t) {
             let e, n, r, i;
-            const o = [dd, ud],
+            const o = [pd, hd],
                 l = [];
 
             function a(t, e) {
                 return "cluster-lines" === t[5] && 1 === t[0].ice.num_clusters ? 0 : 1
             }
             return n = a(t), r = l[n] = o[n](t), {
                 c() {
@@ -10469,17 +10522,17 @@
                     ft(r), i = !1
                 },
                 d(t) {
                     t && f(e), l[n].d()
                 }
             }
         }
-        const gd = 50;
+        const bd = 50;
 
-        function md(t, e, n) {
+        function yd(t, e, n) {
             let r, i, o, l, s, c, u, d, f, h, p, g, m;
             E(t, xr, (t => n(4, s = t))), E(t, wr, (t => n(5, c = t))), E(t, _r, (t => n(12, u = t))), E(t, Qn, (t => n(13, d = t))), E(t, tr, (t => n(14, f = t))), E(t, er, (t => n(15, h = t))), E(t, Ar, (t => n(16, p = t))), E(t, vr, (t => n(17, g = t))), E(t, br, (t => n(18, m = t)));
             let v, b, {
                     pd: y
                 } = e,
                 {
                     featureInfo: $
@@ -10518,59 +10571,59 @@
                 v = a.entries.get(this)?.contentRect, n(2, v)
             }, function(t) {
                 s = t, xr.set(s)
             }, (t, e) => p.has(e) ? 1 : 0, function() {
                 b = a.entries.get(this)?.contentRect, n(3, b)
             }]
         }
-        const vd = class extends _t {
+        const $d = class extends _t {
             constructor(t) {
-                super(), wt(this, t, md, pd, j, {
+                super(), wt(this, t, yd, vd, j, {
                     pd: 0,
                     featureInfo: 1
-                }, cd)
+                }, fd)
             }
         };
 
-        function bd(t) {
+        function wd(t) {
             u(t, "svelte-jg5wjz", ".two-way-pdp-grid.svelte-jg5wjz{display:grid;width:100%;height:100%;grid-template-columns:1fr 1fr 1fr;grid-template-areas:'two-way-interaction two-way-pdp scatter'}")
         }
 
-        function yd(t) {
+        function xd(t) {
             let e, n, r, i, o, l, a, s, u, h, g;
-            return r = new hu({
+            return r = new mu({
                 props: {
                     pd: t[0],
                     width: t[4],
                     height: t[5],
                     scaleLocally: t[6],
                     showMarginalPdp: !0,
-                    marginTop: $d + 1,
-                    marginRight: $d + 1,
-                    marginalPlotHeight: $d,
+                    marginTop: _d + 1,
+                    marginRight: _d + 1,
+                    marginalPlotHeight: _d,
                     iceLevel: "lines",
                     colorShows: "interactions",
                     showColorLegend: !0,
                     colorLegendTitle: "Interactions"
                 }
-            }), l = new hu({
+            }), l = new mu({
                 props: {
                     pd: t[0],
                     width: t[4],
                     height: t[5],
                     scaleLocally: t[6],
                     showMarginalPdp: !0,
-                    marginTop: $d + 1,
-                    marginRight: $d + 1,
-                    marginalPlotHeight: $d,
+                    marginTop: _d + 1,
+                    marginRight: _d + 1,
+                    marginalPlotHeight: _d,
                     iceLevel: "lines",
                     showColorLegend: !0,
                     colorLegendTitle: "Predictions"
                 }
-            }), u = new ed({
+            }), u = new id({
                 props: {
                     width: t[4],
                     height: t[5],
                     xValues: t[7][t[0].x_feature],
                     yValues: t[7][t[0].y_feature],
                     colorValues: t[8],
                     xKind: t[1].kind,
@@ -10578,27 +10631,27 @@
                     colorKind: t[9] ? "categorical" : "quantitative",
                     xDomain: "categorical" === t[1].kind ? t[0].x_axis : [t[0].x_axis[0], t[0].x_axis[t[0].x_axis.length - 1]],
                     yDomain: "categorical" === t[10][t[0].y_feature].kind ? t[0].y_axis : [t[0].y_axis[0], t[0].y_axis[t[0].y_axis.length - 1]],
                     colorDomain: t[11],
                     colorScheme: t[9] ? "classes" : "sequential",
                     xLabel: t[0].x_feature,
                     yLabel: t[0].y_feature,
-                    colorLabel: "Ground Truth",
+                    colorLabel: "Ground truth",
                     xAxisIntegerOnly: "discrete" === t[1].subkind,
                     yAxisIntegerOnly: "discrete" === t[2].subkind,
                     xAxisValueMap: "value_map" in t[1] ? t[1].value_map : {},
                     yAxisValueMap: "value_map" in t[2] ? t[2].value_map : {},
                     xDistribution: t[1].distribution,
                     yDistribution: t[2].distribution,
                     opacity: 1,
                     allowBrushing: !1,
                     showMarginalDistribution: !0,
-                    marginTop: $d + 3,
-                    marginRight: $d + 3,
-                    marginalPlotHeight: $d
+                    marginTop: _d + 3,
+                    marginRight: _d + 3,
+                    marginalPlotHeight: _d
                 }
             }), {
                 c() {
                     e = p("div"), n = p("div"), bt(r.$$.fragment), i = v(), o = p("div"), bt(l.$$.fragment), a = v(), s = p("div"), bt(u.$$.fragment), M(n, "grid-area", "two-way-interaction"), M(o, "grid-area", "two-way-pdp"), M(s, "grid-area", "scatter"), $(e, "class", "two-way-pdp-grid svelte-jg5wjz")
                 },
                 m(f, p) {
                     d(f, e, p), c(e, n), yt(r, n, null), c(e, i), c(e, o), yt(l, o, null), c(e, a), c(e, s), yt(u, s, null), h = P.observe(e, t[13].bind(e)), g = !0
@@ -10618,17 +10671,17 @@
                     ft(r.$$.fragment, t), ft(l.$$.fragment, t), ft(u.$$.fragment, t), g = !1
                 },
                 d(t) {
                     t && f(e), $t(r), $t(l), $t(u), h()
                 }
             }
         }
-        const $d = 50;
+        const _d = 50;
 
-        function wd(t, e, n) {
+        function kd(t, e, n) {
             let r, i, o, l, s, c, u, d, f;
             E(t, _r, (t => n(6, l = t))), E(t, Qn, (t => n(7, s = t))), E(t, tr, (t => n(8, c = t))), E(t, vr, (t => n(9, u = t))), E(t, Zn, (t => n(10, d = t))), E(t, br, (t => n(11, f = t)));
             let h, {
                     pd: p
                 } = e,
                 {
                     xFeatureInfo: g
@@ -10640,39 +10693,39 @@
                 "pd" in t && n(0, p = t.pd), "xFeatureInfo" in t && n(1, g = t.xFeatureInfo), "yFeatureInfo" in t && n(2, m = t.yFeatureInfo)
             }, t.$$.update = () => {
                 8 & t.$$.dirty && n(12, r = h ? h.width : 0), 8 & t.$$.dirty && n(5, i = h ? h.height : 0), 4096 & t.$$.dirty && n(4, o = r / 3)
             }, [p, g, m, h, o, i, l, s, c, u, d, f, r, function() {
                 h = a.entries.get(this)?.contentRect, n(3, h)
             }]
         }
-        const xd = class extends _t {
+        const Md = class extends _t {
             constructor(t) {
-                super(), wt(this, t, wd, yd, j, {
+                super(), wt(this, t, kd, xd, j, {
                     pd: 0,
                     xFeatureInfo: 1,
                     yFeatureInfo: 2
-                }, bd)
+                }, wd)
             }
         };
 
-        function _d(t) {
+        function Ld(t) {
             u(t, "svelte-1oprcpz", ".zoomed-pdp-container.svelte-1oprcpz.svelte-1oprcpz{width:100%;height:100%;display:flex;flex-direction:column}.zoomed-pdp-header.svelte-1oprcpz.svelte-1oprcpz{height:2em;display:flex;align-items:center;background-color:white;gap:1.5em;padding-left:0.5em;padding-right:0.5em;border-bottom:1px solid var(--gray-1)}.feature-selects.svelte-1oprcpz.svelte-1oprcpz{flex:0 1 auto;min-width:0;display:flex;align-items:center;gap:0.5em}.feature-selects.svelte-1oprcpz label.svelte-1oprcpz{flex:0 1 auto;display:flex;align-items:center;gap:0.25em;min-width:0}.feature-selects.svelte-1oprcpz label span.svelte-1oprcpz{flex:0 0 auto}.feature-selects.svelte-1oprcpz label select.svelte-1oprcpz{flex:0 1 auto;min-width:0;text-overflow:ellipsis}.zoomed-pdp-content.svelte-1oprcpz.svelte-1oprcpz{flex:1;padding:0.5em;min-height:0px}.label-and-input.svelte-1oprcpz.svelte-1oprcpz{flex:0 0 auto;display:flex;align-items:center;gap:0.25em}.detailed-plot-message-container.svelte-1oprcpz.svelte-1oprcpz{height:100%;width:100%;align-items:center;justify-content:center;display:flex}.detailed-plot-message-content.svelte-1oprcpz.svelte-1oprcpz{width:40em;display:flex;flex-direction:column;justify-content:center;gap:1em}.detailed-plot-message-content.svelte-1oprcpz>button.svelte-1oprcpz{margin:auto}")
         }
 
-        function kd(t, e, n) {
+        function Ad(t, e, n) {
             const r = t.slice();
             return r[18] = e[n], r
         }
 
-        function Md(t, e, n) {
+        function Pd(t, e, n) {
             const r = t.slice();
             return r[18] = e[n], r
         }
 
-        function Ld(t) {
+        function Sd(t) {
             let e, n, r, i = t[18] + "";
             return {
                 c() {
                     e = p("option"), n = m(i), e.__value = r = t[18], k(e, e.__value)
                 },
                 m(t, r) {
                     d(t, e, r), c(e, n)
@@ -10682,15 +10735,15 @@
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Ad(t) {
+        function zd(t) {
             let e, n, r, i = t[18] + "";
             return {
                 c() {
                     e = p("option"), n = m(i), e.__value = r = t[18], k(e, e.__value)
                 },
                 m(t, r) {
                     d(t, e, r), c(e, n)
@@ -10700,33 +10753,33 @@
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Pd(t) {
-            let e, n, r, i, o, l, a, s = 2 === t[0].num_features && Sd(t);
+        function Td(t) {
+            let e, n, r, i, o, l, a, s = 2 === t[0].num_features && Nd(t);
             return {
                 c() {
                     e = p("label"), n = p("input"), r = m("Scale\n        locally"), i = v(), s && s.c(), o = b(), $(n, "type", "checkbox"), $(e, "class", "label-and-input svelte-1oprcpz")
                 },
                 m(u, f) {
                     d(u, e, f), c(e, n), n.checked = t[7], c(e, r), d(u, i, f), s && s.m(u, f), d(u, o, f), l || (a = y(n, "change", t[15]), l = !0)
                 },
                 p(t, e) {
-                    128 & e && (n.checked = t[7]), 2 === t[0].num_features ? s ? s.p(t, e) : (s = Sd(t), s.c(), s.m(o.parentNode, o)) : s && (s.d(1), s = null)
+                    128 & e && (n.checked = t[7]), 2 === t[0].num_features ? s ? s.p(t, e) : (s = Nd(t), s.c(), s.m(o.parentNode, o)) : s && (s.d(1), s = null)
                 },
                 d(t) {
                     t && (f(e), f(i), f(o)), s && s.d(t), l = !1, a()
                 }
             }
         }
 
-        function Sd(t) {
+        function Nd(t) {
             let e, n, r;
             return {
                 c() {
                     e = p("button"), e.textContent = "Swap Axes", $(e, "title", "Swap x and y axes")
                 },
                 m(i, o) {
                     d(i, e, o), n || (r = y(e, "click", t[9]), n = !0)
@@ -10734,17 +10787,17 @@
                 p: T,
                 d(t) {
                     t && f(e), n = !1, r()
                 }
             }
         }
 
-        function zd(t) {
+        function Cd(t) {
             let e, n;
-            return e = new xd({
+            return e = new Md({
                 props: {
                     pd: t[0],
                     xFeatureInfo: t[4],
                     yFeatureInfo: t[3]
                 }
             }), {
                 c() {
@@ -10765,17 +10818,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Td(t) {
+        function Od(t) {
             let e, n;
-            return e = new vd({
+            return e = new $d({
                 props: {
                     pd: t[0],
                     featureInfo: t[4]
                 }
             }), {
                 c() {
                     bt(e.$$.fragment)
@@ -10795,19 +10848,19 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Nd(t) {
+        function Dd(t) {
             let e, n;
 
             function r(t, e) {
-                return "" === t[2] && "" === t[1] ? Od : Cd
+                return "" === t[2] && "" === t[1] ? Bd : jd
             }
             let i = r(t),
                 o = i(t);
             return {
                 c() {
                     e = p("div"), n = p("div"), o.c(), $(n, "class", "detailed-plot-message-content svelte-1oprcpz"), $(e, "class", "detailed-plot-message-container svelte-1oprcpz")
                 },
@@ -10821,15 +10874,15 @@
                 o: T,
                 d(t) {
                     t && f(e), o.d()
                 }
             }
         }
 
-        function Cd(t) {
+        function jd(t) {
             let e, n, r, i, o, l, a, s, u, h, g, b, w = 2 === t[5].length ? "Computing..." : "Compute Now";
             return {
                 c() {
                     e = p("div"), n = m("The two-way PDP between "), r = m(t[2]), i = m(" and "), o = m(t[1]), l = m("\n              was not pre-computed, since we did not detect a likely interaction\n              between the two features."), a = v(), s = p("button"), u = m(w), s.disabled = h = 2 === t[5].length, $(s, "class", "svelte-1oprcpz")
                 },
                 m(f, h) {
                     d(f, e, h), c(e, n), c(e, r), c(e, i), c(e, o), c(e, l), d(f, a, h), d(f, s, h), c(s, u), g || (b = y(s, "click", t[8]), g = !0)
@@ -10839,15 +10892,15 @@
                 },
                 d(t) {
                     t && (f(e), f(a), f(s)), g = !1, b()
                 }
             }
         }
 
-        function Od(t) {
+        function Bd(t) {
             let e;
             return {
                 c() {
                     e = p("div"), e.textContent = "Select one or two features above.", M(e, "text-align", "center")
                 },
                 m(t, n) {
                     d(t, e, n)
@@ -10855,23 +10908,23 @@
                 p: T,
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Dd(t) {
+        function Ed(t) {
             let e, n, r, i, o, l, a, s, u, g, m, b, w, x, _, M, A, P, S, z, T, N, C = ht(t[6]),
                 D = [];
-            for (let e = 0; e < C.length; e += 1) D[e] = Ld(Md(t, C, e));
+            for (let e = 0; e < C.length; e += 1) D[e] = Sd(Pd(t, C, e));
             let j = ht(t[6]),
                 B = [];
-            for (let e = 0; e < j.length; e += 1) B[e] = Ad(kd(t, j, e));
-            let E = t[0] && Pd(t);
-            const I = [Nd, Td, zd],
+            for (let e = 0; e < j.length; e += 1) B[e] = zd(Ad(t, j, e));
+            let E = t[0] && Td(t);
+            const I = [Dd, Od, Cd],
                 R = [];
 
             function V(t, e) {
                 return null === t[0] ? 0 : 1 === t[0].num_features && t[4] ? 1 : 2 === t[0].num_features && t[4] && t[3] ? 2 : -1
             }
             return ~(P = V(t)) && (S = R[P] = I[P](t)), {
                 c() {
@@ -10888,30 +10941,30 @@
                     for (let t = 0; t < B.length; t += 1) B[t] && B[t].m(w, null);
                     L(w, t[1], !0), c(n, _), E && E.m(n, null), c(e, M), c(e, A), ~P && R[P].m(A, null), z = !0, T || (N = [y(a, "change", t[13]), y(w, "change", t[14])], T = !0)
                 },
                 p(t, [e]) {
                     if (64 & e) {
                         let n;
                         for (C = ht(t[6]), n = 0; n < C.length; n += 1) {
-                            const r = Md(t, C, n);
-                            D[n] ? D[n].p(r, e) : (D[n] = Ld(r), D[n].c(), D[n].m(a, null))
+                            const r = Pd(t, C, n);
+                            D[n] ? D[n].p(r, e) : (D[n] = Sd(r), D[n].c(), D[n].m(a, null))
                         }
                         for (; n < D.length; n += 1) D[n].d(1);
                         D.length = C.length
                     }
                     if (68 & e && L(a, t[2]), 64 & e) {
                         let n;
                         for (j = ht(t[6]), n = 0; n < j.length; n += 1) {
-                            const r = kd(t, j, n);
-                            B[n] ? B[n].p(r, e) : (B[n] = Ad(r), B[n].c(), B[n].m(w, null))
+                            const r = Ad(t, j, n);
+                            B[n] ? B[n].p(r, e) : (B[n] = zd(r), B[n].c(), B[n].m(w, null))
                         }
                         for (; n < B.length; n += 1) B[n].d(1);
                         B.length = j.length
                     }
-                    66 & e && L(w, t[1]), t[0] ? E ? E.p(t, e) : (E = Pd(t), E.c(), E.m(n, null)) : E && (E.d(1), E = null);
+                    66 & e && L(w, t[1]), t[0] ? E ? E.p(t, e) : (E = Td(t), E.c(), E.m(n, null)) : E && (E.d(1), E = null);
                     let r = P;
                     P = V(t), P === r ? ~P && R[P].p(t, e) : (S && (ct(), ft(R[r], 1, 1, (() => {
                         R[r] = null
                     })), ut()), ~P ? (S = R[P], S ? S.p(t, e) : (S = R[P] = I[P](t), S.c()), dt(S, 1), S.m(A, null)) : S = null)
                 },
                 i(t) {
                     z || (dt(S), z = !0)
@@ -10921,15 +10974,15 @@
                 },
                 d(t) {
                     t && f(e), h(D, t), h(B, t), E && E.d(), ~P && R[P].d(), T = !1, O(N)
                 }
             }
         }
 
-        function jd(t, e, n) {
+        function Id(t, e, n) {
             let r, i, o, l, a, s, c, u, d, f;
             E(t, ir, (t => n(10, o = t))), E(t, Zn, (t => n(11, l = t))), E(t, mr, (t => n(12, a = t))), E(t, $r, (t => n(1, s = t))), E(t, yr, (t => n(2, c = t))), E(t, hr, (t => n(5, u = t))), E(t, Jn, (t => n(6, d = t))), E(t, _r, (t => n(7, f = t)));
             let h = null;
             return t.$$.update = () => {
                 var e, d;
                 4102 & t.$$.dirty && (c === s && R($r, s = "", s), "" === c && "" !== s && (R(yr, c = s, c), R($r, s = "", s)), n(0, h = "" === s ? null !== (e = a.get(c)) && void 0 !== e ? e : null : null !== (d = o.find((t => t.x_feature === c && t.y_feature === s || t.x_feature === s && t.y_feature === c))) && void 0 !== d ? d : null)), 1024 & t.$$.dirty && o && function() {
                     const t = o.find((t => t.x_feature === u[0] && t.y_feature === u[1] || t.x_feature === u[1] && t.y_feature === u[0]));
@@ -10950,30 +11003,30 @@
                 c = A(this), yr.set(c)
             }, function() {
                 s = A(this), $r.set(s)
             }, function() {
                 f = this.checked, _r.set(f)
             }]
         }
-        const Bd = class extends _t {
+        const Rd = class extends _t {
             constructor(t) {
-                super(), wt(this, t, jd, Dd, j, {}, _d)
+                super(), wt(this, t, Id, Ed, j, {}, Ld)
             }
         };
 
-        function Ed(t) {
+        function Vd(t) {
             u(t, "svelte-1ps68ru", ".controls-features.svelte-1ps68ru.svelte-1ps68ru{display:flex;flex-direction:column;max-height:100%;row-gap:0.25em}ul.svelte-1ps68ru.svelte-1ps68ru{list-style:none}.fs-row.svelte-1ps68ru.svelte-1ps68ru{display:flex;align-items:center;column-gap:0.25em}input.svelte-1ps68ru.svelte-1ps68ru{min-width:0}.fs-row.svelte-1ps68ru label.svelte-1ps68ru{flex:1}.individual-features.svelte-1ps68ru.svelte-1ps68ru{flex:0 1 auto;overflow-y:auto;min-height:0}.hidden.svelte-1ps68ru.svelte-1ps68ru{display:none}.disabled-feature-label.svelte-1ps68ru.svelte-1ps68ru{color:var(--gray-5);cursor:not-allowed}")
         }
 
-        function Id(t, e, n) {
+        function Hd(t, e, n) {
             const r = t.slice();
             return r[13] = e[n].feature, r[14] = e[n].hidden, r[15] = e[n].disabled, r
         }
 
-        function Rd(t, e) {
+        function qd(t, e) {
             let n, r, i, o, l, a, s, u, h, g, b, w, M, L, A = !1,
                 P = e[13] + "";
             return w = x(e[9][0]), {
                 key: t,
                 first: null,
                 c() {
                     n = p("li"), r = p("input"), a = v(), s = p("label"), u = m(P), b = v(), $(r, "id", i = e[0] + "-" + e[13] + "-checkbox"), $(r, "type", "checkbox"), $(r, "name", "features"), r.__value = o = e[13], k(r, r.__value), r.disabled = l = e[15], $(r, "class", "svelte-1ps68ru"), $(s, "class", "pdpilot-cutoff svelte-1ps68ru"), $(s, "for", h = e[0] + "-" + e[13] + "-checkbox"), $(s, "title", g = e[13]), z(s, "disabled-feature-label", e[15]), $(n, "class", "fs-row svelte-1ps68ru"), z(n, "hidden", e[14]), w.p(r), this.first = n
@@ -10986,49 +11039,49 @@
                 },
                 d(t) {
                     t && f(n), w.r(), M = !1, L()
                 }
             }
         }
 
-        function Vd(t) {
+        function Fd(t) {
             let e, n, r, i, o, l, a, s, u = [],
                 h = new Map,
                 g = ht(t[3]);
             const b = t => t[13];
             for (let e = 0; e < g.length; e += 1) {
-                let n = Id(t, g, e),
+                let n = Hd(t, g, e),
                     r = b(n);
-                h.set(r, u[e] = Rd(r, n))
+                h.set(r, u[e] = qd(r, n))
             }
             return {
                 c() {
                     e = p("div"), n = p("label"), r = m("Search\n    "), i = p("input"), o = v(), l = p("ul");
                     for (let t = 0; t < u.length; t += 1) u[t].c();
                     $(i, "class", "svelte-1ps68ru"), $(n, "class", "fs-row svelte-1ps68ru"), $(l, "class", "individual-features svelte-1ps68ru"), $(e, "class", "controls-features svelte-1ps68ru")
                 },
                 m(f, h) {
                     d(f, e, h), c(e, n), c(n, r), c(n, i), k(i, t[1]), c(e, o), c(e, l);
                     for (let t = 0; t < u.length; t += 1) u[t] && u[t].m(l, null);
                     a || (s = y(i, "input", t[7]), a = !0)
                 },
                 p(t, [e]) {
-                    2 & e && i.value !== t[1] && k(i, t[1]), 13 & e && (g = ht(t[3]), u = mt(u, e, b, 1, t, g, h, l, pt, Rd, null, Id))
+                    2 & e && i.value !== t[1] && k(i, t[1]), 13 & e && (g = ht(t[3]), u = mt(u, e, b, 1, t, g, h, l, pt, qd, null, Hd))
                 },
                 i: T,
                 o: T,
                 d(t) {
                     t && f(e);
                     for (let t = 0; t < u.length; t += 1) u[t].d();
                     a = !1, s()
                 }
             }
         }
 
-        function Hd(t, e, n) {
+        function Wd(t, e, n) {
             let r, i;
             E(t, Jn, (t => n(6, i = t)));
             let {
                 enabledFeatures: o
             } = e, {
                 idPrefix: l
             } = e;
@@ -11057,32 +11110,32 @@
                 n(2, c = [])
             }, i, function() {
                 s = this.value, n(1, s)
             }, function() {
                 c = w(d[0], this.__value, this.checked), n(2, c), n(6, i)
             }, d]
         }
-        const qd = class extends _t {
+        const Kd = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Hd, Vd, j, {
+                super(), wt(this, t, Wd, Fd, j, {
                     enabledFeatures: 4,
                     idPrefix: 0,
                     clear: 5
-                }, Ed)
+                }, Vd)
             }
             get clear() {
                 return this.$$.ctx[5]
             }
         };
 
-        function Fd(t) {
+        function Xd(t) {
             u(t, "svelte-zyfurg", "ul.svelte-zyfurg.svelte-zyfurg{list-style:none}.label-and-input.svelte-zyfurg.svelte-zyfurg{display:flex;align-items:center;gap:0.25em}ul.svelte-zyfurg ul.svelte-zyfurg{margin-left:1em}")
         }
 
-        function Wd(t) {
+        function Ud(t) {
             let e, n, r, i, o, l, a, s, u, h, g, m, b, w, _, M, L, A, P, S, z, N, C, D, j, B, E, I, R;
             return E = x(t[7][0]), {
                 c() {
                     e = p("div"), n = p("ul"), r = p("li"), i = p("label"), o = p("input"), a = p("span"), a.textContent = "Ordered", s = v(), u = p("ul"), h = p("li"), g = p("label"), m = p("input"), b = p("span"), b.textContent = "Increasing", w = v(), _ = p("label"), M = p("input"), L = p("span"), L.textContent = "Decreasing", A = v(), P = p("label"), S = p("input"), z = p("span"), z.textContent = "Mixed", N = v(), C = p("li"), D = p("label"), j = p("input"), B = p("span"), B.textContent = "Nominal", $(o, "type", "checkbox"), o.indeterminate = l = t[0].ordered.shapes.length > 0 && t[0].ordered.shapes.length < t[1].length, $(i, "class", "label-and-input svelte-zyfurg"), $(m, "type", "checkbox"), m.__value = "increasing", k(m, m.__value), $(g, "class", "label-and-input svelte-zyfurg"), $(M, "type", "checkbox"), M.__value = "decreasing", k(M, M.__value), $(_, "class", "label-and-input svelte-zyfurg"), $(S, "type", "checkbox"), S.__value = "mixed", k(S, S.__value), $(P, "class", "label-and-input svelte-zyfurg"), $(u, "class", "svelte-zyfurg"), $(j, "type", "checkbox"), $(D, "class", "label-and-input svelte-zyfurg"), $(n, "class", "svelte-zyfurg"), E.p(m, M, S)
                 },
                 m(l, f) {
                     d(l, e, f), c(e, n), c(n, r), c(r, i), c(i, o), o.checked = t[0].ordered.checked, c(i, a), c(r, s), c(r, u), c(u, h), c(h, g), c(g, m), m.checked = ~(t[0].ordered.shapes || []).indexOf(m.__value), c(g, b), c(h, w), c(h, _), c(_, M), M.checked = ~(t[0].ordered.shapes || []).indexOf(M.__value), c(_, L), c(h, A), c(h, P), c(P, S), S.checked = ~(t[0].ordered.shapes || []).indexOf(S.__value), c(P, z), c(n, N), c(n, C), c(C, D), c(D, j), j.checked = t[0].nominal.checked, c(D, B), I || (R = [y(o, "change", t[5]), y(o, "change", t[2]), y(m, "change", t[6]), y(m, "change", t[3]), y(M, "change", t[8]), y(M, "change", t[3]), y(S, "change", t[9]), y(S, "change", t[3]), y(j, "change", t[10])], I = !0)
@@ -11094,15 +11147,15 @@
                 o: T,
                 d(t) {
                     t && f(e), E.r(), I = !1, O(R)
                 }
             }
         }
 
-        function Kd(t, e, n) {
+        function Yd(t, e, n) {
             let r = ["increasing", "decreasing", "mixed"];
             const i = {
                 ordered: {
                     checked: !0,
                     shapes: r
                 },
                 nominal: {
@@ -11161,103 +11214,103 @@
                 o.ordered.shapes = w(s[0], this.__value, this.checked), n(0, o), n(1, r)
             }, function() {
                 o.ordered.shapes = w(s[0], this.__value, this.checked), n(0, o), n(1, r)
             }, function() {
                 o.nominal.checked = this.checked, n(0, o), n(1, r)
             }]
         }
-        const Xd = class extends _t {
+        const Gd = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Kd, Wd, j, {
+                super(), wt(this, t, Yd, Ud, j, {
                     clear: 4
-                }, Fd)
+                }, Xd)
             }
             get clear() {
                 return this.$$.ctx[4]
             }
         };
 
-        function Ud(t) {
+        function Jd(t) {
             u(t, "svelte-2uqume", ".toggle-and-title.svelte-2uqume.svelte-2uqume{display:flex;align-items:center;gap:0.25em}.icon-tabler-chevron-down.svelte-2uqume polyline.svelte-2uqume{transition:transform 150ms}.rotate-polyline.svelte-2uqume.svelte-2uqume{transform-origin:50% 50%;transform:rotate(-90deg)}")
         }
 
-        function Yd(t) {
-            let e, n, r, i, o, l, a, s, u, h, b, w = `${Gd}px`,
-                x = `${Gd}px`;
+        function Zd(t) {
+            let e, n, r, i, o, l, a, s, u, h, b, w = `${Qd}px`,
+                x = `${Qd}px`;
             return {
                 c() {
-                    e = p("div"), n = p("button"), r = g("svg"), i = g("path"), o = g("polyline"), a = v(), s = p("div"), u = m(t[1]), $(i, "stroke", "none"), $(i, "d", "M0 0h24v24H0z"), $(i, "fill", "none"), $(o, "points", l = "2 12 12 22 22 12"), $(o, "class", "svelte-2uqume"), z(o, "rotate-polyline", !t[0]), $(r, "xmlns", "http://www.w3.org/2000/svg"), $(r, "class", "icon-tabler icon-tabler-chevron-down svelte-2uqume"), $(r, "width", Gd), $(r, "height", Gd), $(r, "viewBox", "0 0 24 24"), $(r, "stroke-width", "4"), $(r, "stroke", "currentColor"), $(r, "fill", "none"), $(r, "stroke-linecap", "round"), $(r, "stroke-linejoin", "round"), M(n, "border", "none"), M(n, "width", w), M(n, "height", x), M(n, "padding", "0"), M(n, "color", "var(--black)"), M(n, "background-color", "white"), $(s, "class", "pdpilot-bold"), $(e, "class", "toggle-and-title svelte-2uqume")
+                    e = p("div"), n = p("button"), r = g("svg"), i = g("path"), o = g("polyline"), a = v(), s = p("div"), u = m(t[1]), $(i, "stroke", "none"), $(i, "d", "M0 0h24v24H0z"), $(i, "fill", "none"), $(o, "points", l = "2 12 12 22 22 12"), $(o, "class", "svelte-2uqume"), z(o, "rotate-polyline", !t[0]), $(r, "xmlns", "http://www.w3.org/2000/svg"), $(r, "class", "icon-tabler icon-tabler-chevron-down svelte-2uqume"), $(r, "width", Qd), $(r, "height", Qd), $(r, "viewBox", "0 0 24 24"), $(r, "stroke-width", "4"), $(r, "stroke", "currentColor"), $(r, "fill", "none"), $(r, "stroke-linecap", "round"), $(r, "stroke-linejoin", "round"), M(n, "border", "none"), M(n, "width", w), M(n, "height", x), M(n, "padding", "0"), M(n, "color", "var(--black)"), M(n, "background-color", "white"), $(s, "class", "pdpilot-bold"), $(e, "class", "toggle-and-title svelte-2uqume")
                 },
                 m(l, f) {
                     d(l, e, f), c(e, n), c(n, r), c(r, i), c(r, o), c(e, a), c(e, s), c(s, u), h || (b = y(n, "click", t[2]), h = !0)
                 },
                 p(t, [e]) {
                     1 & e && z(o, "rotate-polyline", !t[0]), 2 & e && _(u, t[1])
                 },
                 i: T,
                 o: T,
                 d(t) {
                     t && f(e), h = !1, b()
                 }
             }
         }
-        const Gd = 8;
+        const Qd = 8;
 
-        function Jd(t, e, n) {
+        function tf(t, e, n) {
             let {
                 expanded: r = !1
             } = e, {
                 title: i
             } = e;
             return t.$$set = t => {
                 "expanded" in t && n(0, r = t.expanded), "title" in t && n(1, i = t.title)
             }, [r, i, () => n(0, r = !r)]
         }
-        const Zd = class extends _t {
+        const ef = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Jd, Yd, j, {
+                super(), wt(this, t, tf, Zd, j, {
                     expanded: 0,
                     title: 1
-                }, Ud)
+                }, Jd)
             }
         };
 
-        function Qd(t) {
+        function nf(t) {
             u(t, "svelte-1mkvanr", ".controls-container.svelte-1mkvanr.svelte-1mkvanr{height:100%;flex:0 0 200px;min-width:200px;max-width:200px;padding:0.25em;border-right:1px solid var(--gray-1);display:flex;flex-direction:column;gap:0.5em}.feature-selector-wrapper-outer.svelte-1mkvanr.svelte-1mkvanr{flex:0 1 auto;min-height:0;display:flex;flex-direction:column}.feature-selector-wrapper-inner.svelte-1mkvanr.svelte-1mkvanr{flex:1;min-height:0}.filter-header.svelte-1mkvanr+.filter-content.svelte-1mkvanr{margin-top:0.25em}.filter-content.svelte-1mkvanr.svelte-1mkvanr{margin-left:0.75em}")
         }
 
-        function tf(t) {
+        function rf(t) {
             let e, n, r, i, o, l, a, s, u, h, g, m, b, w, x, _, k, L, A, P, S, T, N;
 
             function C(e) {
                 t[11](e)
             }
             let O = {
                 title: "Type"
             };
 
             function D(e) {
                 t[13](e)
             }
-            void 0 !== t[2] && (O.expanded = t[2]), s = new Zd({
+            void 0 !== t[2] && (O.expanded = t[2]), s = new ef({
                 props: O
-            }), X.push((() => vt(s, "expanded", C))), m = new Xd({
+            }), X.push((() => vt(s, "expanded", C))), m = new Gd({
                 props: {}
             }), t[12](m), m.$on("changeKindFilters", t[5]);
             let j = {
                 title: "Name"
             };
-            void 0 !== t[3] && (j.expanded = t[3]), _ = new Zd({
+            void 0 !== t[3] && (j.expanded = t[3]), _ = new ef({
                 props: j
             }), X.push((() => vt(_, "expanded", D)));
             let B = {
                 enabledFeatures: t[4],
                 idPrefix: "pdpilot-one"
             };
-            return P = new qd({
+            return P = new Kd({
                 props: B
             }), t[14](P), P.$on("changeNameFilters", t[6]), {
                 c() {
                     e = p("div"), n = p("div"), n.textContent = "Feature Filters", r = v(), i = p("button"), i.textContent = "Clear Filters", o = v(), l = p("div"), a = p("div"), bt(s.$$.fragment), h = v(), g = p("div"), bt(m.$$.fragment), b = v(), w = p("div"), x = p("div"), bt(_.$$.fragment), L = v(), A = p("div"), bt(P.$$.fragment), $(n, "class", "pdpilot-bold"), M(i, "align-self", "start"), $(a, "class", "filter-header svelte-1mkvanr"), $(g, "class", "filter-content svelte-1mkvanr"), z(g, "pdp-hide", !t[2]), $(x, "class", "filter-header svelte-1mkvanr"), $(A, "class", "filter-content feature-selector-wrapper-inner svelte-1mkvanr"), z(A, "pdp-hide", !t[3]), $(w, "class", "filter-container feature-selector-wrapper-outer svelte-1mkvanr"), $(e, "class", "controls-container svelte-1mkvanr")
                 },
                 m(u, f) {
                     d(u, e, f), c(e, n), c(e, r), c(e, i), c(e, o), c(e, l), c(l, a), yt(s, a, null), c(l, h), c(l, g), yt(m, g, null), c(e, b), c(e, w), c(w, x), yt(_, x, null), c(w, L), c(w, A), yt(P, A, null), S = !0, T || (N = y(i, "click", t[7]), T = !0)
@@ -11278,15 +11331,15 @@
                 },
                 d(n) {
                     n && f(e), $t(s), t[12](null), $t(m), $t(_), t[14](null), $t(P), T = !1, N()
                 }
             }
         }
 
-        function ef(t, e, n) {
+        function of(t, e, n) {
             let r, i, o;
             E(t, mr, (t => n(9, i = t))), E(t, Jn, (t => n(10, o = t)));
             const l = W();
             let a, s, c, u = !0,
                 d = !0;
             return t.$$.update = () => {
                 1792 & t.$$.dirty && n(4, r = o.filter((t => {
@@ -11309,29 +11362,29 @@
                 d = t, n(3, d)
             }, function(t) {
                 X[t ? "unshift" : "push"]((() => {
                     s = t, n(1, s)
                 }))
             }]
         }
-        const nf = class extends _t {
+        const lf = class extends _t {
             constructor(t) {
-                super(), wt(this, t, ef, tf, j, {}, Qd)
+                super(), wt(this, t, of, rf, j, {}, nf)
             }
         };
 
-        function rf(t) {
+        function af(t) {
             return 0 === t.length || 1 === t[0].num_features
         }
 
-        function of(t) {
+        function sf(t) {
             u(t, "svelte-19snser", ".tooltip-container.svelte-19snser{position:relative;display:flex;align-items:center}.tooltip-content.svelte-19snser{position:absolute;padding:5px;border-radius:5px;max-width:30em;border:1px solid black;color:black;background-color:white;z-index:1;pointer-events:none}")
         }
 
-        function lf(t) {
+        function cf(t) {
             let e, n, r, i, o, l, a;
             return {
                 c() {
                     e = g("svg"), n = g("path"), r = g("circle"), i = g("line"), o = g("path"), $(n, "stroke", "none"), $(n, "d", "M0 0h24v24H0z"), $(r, "cx", "12"), $(r, "cy", "12"), $(r, "r", "9"), $(i, "x1", "12"), $(i, "y1", "17"), $(i, "x2", "12"), $(i, "y2", "17.01"), $(o, "d", "M12 13.5a1.5 1.5 0 0 1 1 -1.5a2.6 2.6 0 1 0 -3 -4"), $(e, "xmlns", "http://www.w3.org/2000/svg"), $(e, "class", "pdpilot-icon icon-tabler icon-tabler-help"), $(e, "width", "24"), $(e, "height", "24"), $(e, "viewBox", "0 0 24 24"), $(e, "stroke-width", "2"), $(e, "stroke", "currentColor"), $(e, "fill", "none"), $(e, "stroke-linecap", "round"), $(e, "stroke-linejoin", "round")
                 },
                 m(s, u) {
                     d(s, e, u), c(e, n), c(e, r), c(e, i), c(e, o), l || (a = [y(e, "mouseenter", t[15]), y(e, "mouseleave", t[16])], l = !0)
@@ -11339,15 +11392,15 @@
                 p: T,
                 d(t) {
                     t && f(e), l = !1, O(a)
                 }
             }
         }
 
-        function af(t) {
+        function uf(t) {
             let e, n, r, i, o, l, a;
             return {
                 c() {
                     e = g("svg"), n = g("path"), r = g("circle"), i = g("line"), o = g("line"), $(n, "stroke", "none"), $(n, "d", "M0 0h24v24H0z"), $(n, "fill", "none"), $(r, "cx", "12"), $(r, "cy", "12"), $(r, "r", "9"), $(i, "x1", "12"), $(i, "y1", "8"), $(i, "x2", "12"), $(i, "y2", "12"), $(o, "x1", "12"), $(o, "y1", "16"), $(o, "x2", "12.01"), $(o, "y2", "16"), $(e, "xmlns", "http://www.w3.org/2000/svg"), $(e, "class", "pdpilot-icon icon-tabler icon-tabler-alert-circle"), $(e, "width", "24"), $(e, "height", "24"), $(e, "viewBox", "0 0 24 24"), $(e, "stroke-width", "2"), $(e, "stroke", "currentColor"), $(e, "fill", "none"), $(e, "stroke-linecap", "round"), $(e, "stroke-linejoin", "round")
                 },
                 m(s, u) {
                     d(s, e, u), c(e, n), c(e, r), c(e, i), c(e, o), l || (a = [y(e, "mouseenter", t[13]), y(e, "mouseleave", t[14])], l = !0)
@@ -11355,15 +11408,15 @@
                 p: T,
                 d(t) {
                     t && f(e), l = !1, O(a)
                 }
             }
         }
 
-        function sf(t) {
+        function df(t) {
             let e, n, r = `${t[5]}\n      ${t[6]}\n      ${t[7]}\n      ${t[8]}`;
             const i = t[12].default,
                 o = function(t, e, n, r) {
                     if (t) {
                         const r = I(t, e, n, null);
                         return t[0](r)
                     }
@@ -11412,32 +11465,32 @@
                 },
                 d(t) {
                     t && f(e), o && o.d(t)
                 }
             }
         }
 
-        function cf(t) {
+        function ff(t) {
             let e, n, r;
 
             function i(t, e) {
-                return "alert" === t[0] ? af : lf
+                return "alert" === t[0] ? uf : cf
             }
             let o = i(t),
                 l = o(t),
-                a = t[10] && sf(t);
+                a = t[10] && df(t);
             return {
                 c() {
                     e = p("div"), l.c(), n = v(), a && a.c(), $(e, "class", "tooltip-container svelte-19snser")
                 },
                 m(t, i) {
                     d(t, e, i), l.m(e, null), c(e, n), a && a.m(e, null), r = !0
                 },
                 p(t, [r]) {
-                    o === (o = i(t)) && l ? l.p(t, r) : (l.d(1), l = o(t), l && (l.c(), l.m(e, n))), t[10] ? a ? (a.p(t, r), 1024 & r && dt(a, 1)) : (a = sf(t), a.c(), dt(a, 1), a.m(e, null)) : a && (ct(), ft(a, 1, 1, (() => {
+                    o === (o = i(t)) && l ? l.p(t, r) : (l.d(1), l = o(t), l && (l.c(), l.m(e, n))), t[10] ? a ? (a.p(t, r), 1024 & r && dt(a, 1)) : (a = df(t), a.c(), dt(a, 1), a.m(e, null)) : a && (ct(), ft(a, 1, 1, (() => {
                         a = null
                     })), ut())
                 },
                 i(t) {
                     r || (dt(a), r = !0)
                 },
                 o(t) {
@@ -11445,15 +11498,15 @@
                 },
                 d(t) {
                     t && f(e), l.d(), a && a.d()
                 }
             }
         }
 
-        function uf(t, e, n) {
+        function hf(t, e, n) {
             let {
                 $$slots: r = {},
                 $$scope: i
             } = e, {
                 kind: o = "help"
             } = e, {
                 top: l = "auto"
@@ -11474,51 +11527,51 @@
             } = e, {
                 width: p = "30em"
             } = e, g = !1;
             return t.$$set = t => {
                 "kind" in t && n(0, o = t.kind), "top" in t && n(1, l = t.top), "left" in t && n(2, a = t.left), "right" in t && n(3, s = t.right), "bottom" in t && n(4, c = t.bottom), "marginTop" in t && n(5, u = t.marginTop), "marginRight" in t && n(6, d = t.marginRight), "marginBottom" in t && n(7, f = t.marginBottom), "marginLeft" in t && n(8, h = t.marginLeft), "width" in t && n(9, p = t.width), "$$scope" in t && n(11, i = t.$$scope)
             }, [o, l, a, s, c, u, d, f, h, p, g, i, r, () => n(10, g = !0), () => n(10, g = !1), () => n(10, g = !0), () => n(10, g = !1)]
         }
-        const df = class extends _t {
+        const pf = class extends _t {
             constructor(t) {
-                super(), wt(this, t, uf, cf, j, {
+                super(), wt(this, t, hf, ff, j, {
                     kind: 0,
                     top: 1,
                     left: 2,
                     right: 3,
                     bottom: 4,
                     marginTop: 5,
                     marginRight: 6,
                     marginBottom: 7,
                     marginLeft: 8,
                     width: 9
-                }, of)
+                }, sf)
             }
         };
 
-        function ff(t) {
+        function gf(t) {
             u(t, "svelte-alv95s", ".group-container.svelte-alv95s.svelte-alv95s{height:100%;width:100%;display:flex;flex-direction:column;min-height:2em}.pdp-grid-container.svelte-alv95s.svelte-alv95s{flex:1;min-height:0;padding:1px}.pdpilot-no-plots-container.svelte-alv95s.svelte-alv95s{width:100%;height:100%;display:flex;align-items:center;justify-content:center}.pdpilot-no-plots-message.svelte-alv95s.svelte-alv95s{max-width:28em}.pdp-grid.svelte-alv95s.svelte-alv95s{height:100%;display:grid}.group-header.svelte-alv95s.svelte-alv95s{height:2em;display:flex;align-items:center;gap:1em;border-bottom:1px solid var(--gray-1);padding-left:0.5em;padding-right:0.5em}.two-way-color-container.svelte-alv95s.svelte-alv95s{flex:1;margin-left:auto;display:flex;align-items:center}.two-way-color-legend.svelte-alv95s.svelte-alv95s{flex:1}.page-change.svelte-alv95s.svelte-alv95s{display:flex;align-items:center}.current-page-number.svelte-alv95s.svelte-alv95s{width:2em;text-align:center}.label-and-input.svelte-alv95s.svelte-alv95s{display:flex;align-items:center;gap:0.25em}.pdp-grid-element.svelte-alv95s.svelte-alv95s{position:relative}.pdp-grid-element.svelte-alv95s:hover .expand-pdp-button.svelte-alv95s{display:block}.expand-pdp-button.svelte-alv95s.svelte-alv95s{position:absolute;display:none;bottom:2px;left:2px}.dont-shrink.svelte-alv95s.svelte-alv95s{flex:0 0 auto}.dont-show.svelte-alv95s.svelte-alv95s{display:none}ul.svelte-alv95s.svelte-alv95s{list-style:none}li.svelte-alv95s+li.svelte-alv95s{margin-top:0.5em}")
         }
 
-        function hf(t, e, n) {
+        function mf(t, e, n) {
             const r = t.slice();
             return r[51] = e[n], r
         }
 
-        function pf(t, e, n) {
+        function vf(t, e, n) {
             const r = t.slice();
             return r[54] = e[n].value, r[55] = e[n].title, r
         }
 
-        function gf(t, e, n) {
+        function bf(t, e, n) {
             const r = t.slice();
             return r[58] = e[n], r
         }
 
-        function mf(t) {
+        function yf(t) {
             let e, n, r, i = t[58].name + "";
             return {
                 c() {
                     e = p("option"), n = m(i), e.__value = r = t[58], k(e, e.__value)
                 },
                 m(t, r) {
                     d(t, e, r), c(e, n)
@@ -11528,49 +11581,49 @@
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function vf(t) {
+        function $f(t) {
             let e;
             return {
                 c() {
                     e = p("ul"), e.innerHTML = '<li class="svelte-alv95s"><span class="pdpilot-bold">Interaction:</span> Plots for feature\n                pairs with more interaction are ranked higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Variance:</span> Plots that have more\n                variation in their average predictions are ranked higher.</li>', $(e, "class", "svelte-alv95s")
                 },
                 m(t, n) {
                     d(t, e, n)
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function bf(t) {
+        function wf(t) {
             let e;
             return {
                 c() {
-                    e = p("ul"), e.innerHTML = '<li class="svelte-alv95s"><span class="pdpilot-bold">Variance:</span> Plots that have more\n                variance in their ICE lines are ranked higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Cluster difference:</span> Plots that\n                have ICE clusters farther from the partial dependence line are ranked\n                higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Highlighted similarity:</span> Plots where\n                the highlighted lines are closer together and farther from the partial\n                dependence line are ranked higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Highlighted distribution:</span> Plots\n                for features whose distributions of highlighted instances are more\n                different from the overall distributions are ranked higher.</li>', $(e, "class", "svelte-alv95s")
+                    e = p("ul"), e.innerHTML = '<li class="svelte-alv95s"><span class="pdpilot-bold">Importance:</span> Plots that have more\n                variance in their ICE lines are ranked higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Cluster difference:</span> Plots that\n                have ICE clusters farther from the partial dependence line are ranked\n                higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Highlighted line similarity:</span> Plots\n                where the highlighted lines are closer together and farther from\n                the partial dependence line are ranked higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Highlighted histogram difference:</span> Plots for features whose distributions of highlighted instances\n                are more different from the overall distributions are ranked higher.</li>', $(e, "class", "svelte-alv95s")
                 },
                 m(t, n) {
                     d(t, e, n)
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function yf(t) {
+        function xf(t) {
             let e;
 
             function n(t, e) {
-                return 1 === t[17] ? bf : vf
+                return 1 === t[17] ? wf : $f
             }
             let r = n(t),
                 i = r(t);
             return {
                 c() {
                     e = p("div"), i.c()
                 },
@@ -11582,15 +11635,15 @@
                 },
                 d(t) {
                     t && f(e), i.d()
                 }
             }
         }
 
-        function $f(t) {
+        function _f(t) {
             let e, n, r, i, o, l, a, s;
             return {
                 c() {
                     e = p("button"), n = g("svg"), r = g("path"), i = g("path"), o = g("path"), $(r, "stroke", "none"), $(r, "d", "M0 0h24v24H0z"), $(r, "fill", "none"), $(i, "d", "M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4"), $(o, "d", "M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4"), $(n, "xmlns", "http://www.w3.org/2000/svg"), $(n, "class", "pdpilot-icon icon-tabler icon-tabler-refresh"), $(n, "width", "24"), $(n, "height", "24"), $(n, "viewBox", "0 0 24 24"), $(n, "stroke-width", "2"), $(n, "stroke", "currentColor"), $(n, "fill", "none"), $(n, "stroke-linecap", "round"), $(n, "stroke-linejoin", "round"), $(e, "title", "Update sorting"), e.disabled = l = !t[13]
                 },
                 m(l, u) {
                     d(l, e, u), c(e, n), c(n, r), c(n, i), c(n, o), a || (s = y(e, "click", t[33]), a = !0)
@@ -11600,18 +11653,18 @@
                 },
                 d(t) {
                     t && f(e), a = !1, s()
                 }
             }
         }
 
-        function wf(t) {
+        function kf(t) {
             let e, n, r, i, o, l = ht(t[21]),
                 a = [];
-            for (let e = 0; e < l.length; e += 1) a[e] = xf(pf(t, l, e));
+            for (let e = 0; e < l.length; e += 1) a[e] = Mf(vf(t, l, e));
             return {
                 c() {
                     e = p("label"), n = m("Plot\n        "), r = p("select");
                     for (let t = 0; t < a.length; t += 1) a[t].c();
                     void 0 === t[9] && tt((() => t[34].call(r))), $(e, "class", "label-and-input dont-shrink svelte-alv95s")
                 },
                 m(l, s) {
@@ -11619,29 +11672,29 @@
                     for (let t = 0; t < a.length; t += 1) a[t] && a[t].m(r, null);
                     L(r, t[9], !0), i || (o = y(r, "change", t[34]), i = !0)
                 },
                 p(t, e) {
                     if (2097152 & e[0]) {
                         let n;
                         for (l = ht(t[21]), n = 0; n < l.length; n += 1) {
-                            const i = pf(t, l, n);
-                            a[n] ? a[n].p(i, e) : (a[n] = xf(i), a[n].c(), a[n].m(r, null))
+                            const i = vf(t, l, n);
+                            a[n] ? a[n].p(i, e) : (a[n] = Mf(i), a[n].c(), a[n].m(r, null))
                         }
                         for (; n < a.length; n += 1) a[n].d(1);
                         a.length = l.length
                     }
                     2097664 & e[0] && L(r, t[9])
                 },
                 d(t) {
                     t && f(e), h(a, t), i = !1, o()
                 }
             }
         }
 
-        function xf(t) {
+        function Mf(t) {
             let e, n, r, i = t[55] + "";
             return {
                 c() {
                     e = p("option"), n = m(i), e.__value = r = t[54], k(e, e.__value)
                 },
                 m(t, r) {
                     d(t, e, r), c(e, n)
@@ -11649,34 +11702,34 @@
                 p: T,
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function _f(t) {
+        function Lf(t) {
             let e, n, r, i, o, l, a, s, u, h, g;
-            return s = new df({
+            return s = new pf({
                 props: {
                     kind: "help",
                     right: "0",
                     top: "0",
                     marginRight: "1em",
                     marginTop: "1.5em",
                     width: "30em",
                     $$slots: {
-                        default: [Lf]
+                        default: [Sf]
                     },
                     $$scope: {
                         ctx: t
                     }
                 }
             }), {
                 c() {
-                    e = p("div"), n = p("label"), r = m("Color\n            "), i = p("select"), o = p("option"), o.textContent = "interactions", l = p("option"), l.textContent = "predictions", a = v(), bt(s.$$.fragment), o.__value = "interactions", k(o, o.__value), l.__value = "predictions", k(l, l.__value), void 0 === t[10] && tt((() => t[36].call(i))), $(n, "class", "label-and-input svelte-alv95s"), $(e, "class", "label-and-input dont-shrink svelte-alv95s")
+                    e = p("div"), n = p("label"), r = m("Color\n            "), i = p("select"), o = p("option"), o.textContent = "Predictions", l = p("option"), l.textContent = "Interactions", a = v(), bt(s.$$.fragment), o.__value = "predictions", k(o, o.__value), l.__value = "interactions", k(l, l.__value), void 0 === t[10] && tt((() => t[36].call(i))), $(n, "class", "label-and-input svelte-alv95s"), $(e, "class", "label-and-input dont-shrink svelte-alv95s")
                 },
                 m(f, p) {
                     d(f, e, p), c(e, n), c(n, r), c(n, i), c(i, o), c(i, l), L(i, t[10], !0), c(e, a), yt(s, e, null), u = !0, h || (g = y(i, "change", t[36]), h = !0)
                 },
                 p(t, e) {
                     1024 & e[0] && L(i, t[10]);
                     const n = {};
@@ -11693,15 +11746,15 @@
                 },
                 d(t) {
                     t && f(e), $t(s), h = !1, g()
                 }
             }
         }
 
-        function kf(t) {
+        function Af(t) {
             let e;
             return {
                 c() {
                     e = m("This color scale is for a standard two-way PDP. The color of a\n                cell represents the model's average prediction when setting the\n                instances to have the given values for pair of features.")
                 },
                 m(t, n) {
                     d(t, e, n)
@@ -11709,15 +11762,15 @@
                 p: T,
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Mf(t) {
+        function Pf(t) {
             let e, n, r, i, o;
             return {
                 c() {
                     e = m("This color scale shows the difference between the value in a\n                two-way PDP and the expected value if there was no interaction\n                between the pair of features. It indicates whether the\n                interaction between the two features makes the model's average\n                prediction for the given values "), n = p("span"), n.textContent = "lower", r = m("\n                or\n                "), i = p("span"), i.textContent = "higher", o = m(". The units are the same as your target variable."), M(n, "background", t[19].interpolator()(.1)), M(n, "border-radius", "4px"), M(n, "padding", "0.125em 0.25em"), M(n, "color", "white"), M(i, "background", t[19].interpolator()(.9)), M(i, "border-radius", "4px"), M(i, "padding", "0.125em 0.25em"), M(i, "color", "white")
                 },
                 m(t, l) {
                     d(t, e, l), d(t, n, l), d(t, r, l), d(t, i, l), d(t, o, l)
@@ -11727,19 +11780,19 @@
                 },
                 d(t) {
                     t && (f(e), f(n), f(r), f(i), f(o))
                 }
             }
         }
 
-        function Lf(t) {
+        function Sf(t) {
             let e;
 
             function n(t, e) {
-                return "interactions" === t[10] ? Mf : kf
+                return "interactions" === t[10] ? Pf : Af
             }
             let r = n(t),
                 i = r(t);
             return {
                 c() {
                     e = p("div"), i.c()
                 },
@@ -11751,39 +11804,39 @@
                 },
                 d(t) {
                     t && f(e), i.d()
                 }
             }
         }
 
-        function Af(t) {
+        function zf(t) {
             let e, n, r = [],
                 i = new Map,
                 o = `repeat(${t[8]}, minmax(0,${t[11]}px))`,
                 l = `repeat(${t[7]}, minmax(0,${t[12]}px))`,
                 a = ht(t[16]);
             const s = t => t[51].id;
             for (let e = 0; e < a.length; e += 1) {
-                let n = hf(t, a, e),
+                let n = mf(t, a, e),
                     o = s(n);
-                i.set(o, r[e] = Sf(o, n))
+                i.set(o, r[e] = Nf(o, n))
             }
             return {
                 c() {
                     e = p("div");
                     for (let t = 0; t < r.length; t += 1) r[t].c();
                     $(e, "class", "pdp-grid svelte-alv95s"), M(e, "grid-template-columns", o), M(e, "grid-template-rows", l)
                 },
                 m(t, i) {
                     d(t, e, i);
                     for (let t = 0; t < r.length; t += 1) r[t] && r[t].m(e, null);
                     n = !0
                 },
                 p(t, n) {
-                    16997888 & n[0] && (a = ht(t[16]), ct(), r = mt(r, n, s, 1, t, a, i, e, gt, Sf, null, hf), ut()), 2304 & n[0] && o !== (o = `repeat(${t[8]}, minmax(0,${t[11]}px))`) && M(e, "grid-template-columns", o), 4224 & n[0] && l !== (l = `repeat(${t[7]}, minmax(0,${t[12]}px))`) && M(e, "grid-template-rows", l)
+                    16997888 & n[0] && (a = ht(t[16]), ct(), r = mt(r, n, s, 1, t, a, i, e, gt, Nf, null, mf), ut()), 2304 & n[0] && o !== (o = `repeat(${t[8]}, minmax(0,${t[11]}px))`) && M(e, "grid-template-columns", o), 4224 & n[0] && l !== (l = `repeat(${t[7]}, minmax(0,${t[12]}px))`) && M(e, "grid-template-rows", l)
                 },
                 i(t) {
                     if (!n) {
                         for (let t = 0; t < a.length; t += 1) dt(r[t]);
                         n = !0
                     }
                 },
@@ -11794,15 +11847,15 @@
                 d(t) {
                     t && f(e);
                     for (let t = 0; t < r.length; t += 1) r[t].d()
                 }
             }
         }
 
-        function Pf(t) {
+        function Tf(t) {
             let e, n, r;
             return {
                 c() {
                     e = p("div"), n = p("div"), r = m(t[2]), $(n, "class", "pdpilot-no-plots-message svelte-alv95s"), $(e, "class", "pdpilot-no-plots-container svelte-alv95s")
                 },
                 m(t, i) {
                     d(t, e, i), c(e, n), c(n, r)
@@ -11814,22 +11867,22 @@
                 o: T,
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Sf(t, e) {
+        function Nf(t, e) {
             let n, r, i, o, l, a, s, u, h = `${e[11]}px`,
                 g = `${e[12]}px`;
 
             function m() {
                 return e[38](e[51])
             }
-            return r = new hu({
+            return r = new mu({
                 props: {
                     pd: e[51],
                     width: e[11],
                     height: e[12],
                     scaleLocally: e[14],
                     colorShows: e[10],
                     showMarginalDistribution: !0,
@@ -11864,47 +11917,47 @@
                 },
                 d(t) {
                     t && f(n), $t(r), s = !1, u()
                 }
             }
         }
 
-        function zf(t) {
+        function Cf(t) {
             let e, n, r, i, o, l, a, s, u, b, w, x, k, M, A, S, T, N, C, D, j, B, E, I, R, V, H, q, F, W, K, X, U, Y, G, J, Z, Q, et, nt, rt, it, ot, lt, at, st, pt, gt, mt = ht(t[1]),
                 vt = [];
-            for (let e = 0; e < mt.length; e += 1) vt[e] = mf(gf(t, mt, e));
-            q = new df({
+            for (let e = 0; e < mt.length; e += 1) vt[e] = yf(bf(t, mt, e));
+            q = new pf({
                 props: {
                     kind: "help",
                     left: "0",
                     top: "0",
                     marginRight: "1em",
                     marginTop: "1.5em",
-                    width: "30em",
+                    width: "25em",
                     $$slots: {
-                        default: [yf]
+                        default: [xf]
                     },
                     $$scope: {
                         ctx: t
                     }
                 }
             });
-            let wt = 1 === t[17] && t[5].forBrushing && $f(t),
-                xt = 1 === t[17] && wf(t),
-                _t = 2 === t[17] && _f(t);
+            let wt = 1 === t[17] && t[5].forBrushing && _f(t),
+                xt = 1 === t[17] && kf(t),
+                _t = 2 === t[17] && Lf(t);
             et = new wc({
                 props: {
                     width: t[18],
-                    height: Tf,
+                    height: Of,
                     color: "interactions" === t[10] ? t[19] : t[20],
                     marginLeft: 15,
                     marginRight: 15
                 }
             });
-            const kt = [Pf, Af],
+            const kt = [Tf, zf],
                 Mt = [];
 
             function Lt(t, e) {
                 return 0 === t[16].length ? 0 : 1
             }
             return ot = Lt(t), lt = Mt[ot] = kt[ot](t), {
                 c() {
@@ -11917,26 +11970,26 @@
                     for (let t = 0; t < vt.length; t += 1) vt[t] && vt[t].m(V, null);
                     L(V, t[5], !0), c(E, H), yt(q, E, null), c(n, F), wt && wt.m(n, null), c(n, W), xt && xt.m(n, null), c(n, K), c(n, X), c(X, U), U.checked = t[14], c(X, Y), c(n, G), c(n, J), _t && _t.m(J, null), c(J, Z), c(J, Q), yt(et, Q, null), nt = P.observe(Q, t[37].bind(Q)), c(e, rt), c(e, it), Mt[ot].m(it, null), at = P.observe(it, t[39].bind(it)), st = !0, pt || (gt = [y(i, "click", t[30]), y(A, "click", t[31]), y(V, "change", t[32]), y(U, "change", t[35])], pt = !0)
                 },
                 p(t, e) {
                     if ((!st || 64 & e[0] && b !== (b = t[6] <= 1)) && (i.disabled = b), (!st || 64 & e[0]) && _(k, t[6]), (!st || 32832 & e[0] && j !== (j = t[6] >= t[15])) && (A.disabled = j), 2 & e[0]) {
                         let n;
                         for (mt = ht(t[1]), n = 0; n < mt.length; n += 1) {
-                            const r = gf(t, mt, n);
-                            vt[n] ? vt[n].p(r, e) : (vt[n] = mf(r), vt[n].c(), vt[n].m(V, null))
+                            const r = bf(t, mt, n);
+                            vt[n] ? vt[n].p(r, e) : (vt[n] = yf(r), vt[n].c(), vt[n].m(V, null))
                         }
                         for (; n < vt.length; n += 1) vt[n].d(1);
                         vt.length = mt.length
                     }
                     34 & e[0] && L(V, t[5]);
                     const r = {};
                     131072 & e[0] | 1073741824 & e[1] && (r.$$scope = {
                         dirty: e,
                         ctx: t
-                    }), q.$set(r), 1 === t[17] && t[5].forBrushing ? wt ? wt.p(t, e) : (wt = $f(t), wt.c(), wt.m(n, W)) : wt && (wt.d(1), wt = null), 1 === t[17] ? xt ? xt.p(t, e) : (xt = wf(t), xt.c(), xt.m(n, K)) : xt && (xt.d(1), xt = null), 16384 & e[0] && (U.checked = t[14]), 2 === t[17] ? _t ? (_t.p(t, e), 131072 & e[0] && dt(_t, 1)) : (_t = _f(t), _t.c(), dt(_t, 1), _t.m(J, Z)) : _t && (ct(), ft(_t, 1, 1, (() => {
+                    }), q.$set(r), 1 === t[17] && t[5].forBrushing ? wt ? wt.p(t, e) : (wt = _f(t), wt.c(), wt.m(n, W)) : wt && (wt.d(1), wt = null), 1 === t[17] ? xt ? xt.p(t, e) : (xt = kf(t), xt.c(), xt.m(n, K)) : xt && (xt.d(1), xt = null), 16384 & e[0] && (U.checked = t[14]), 2 === t[17] ? _t ? (_t.p(t, e), 131072 & e[0] && dt(_t, 1)) : (_t = Lf(t), _t.c(), dt(_t, 1), _t.m(J, Z)) : _t && (ct(), ft(_t, 1, 1, (() => {
                         _t = null
                     })), ut());
                     const o = {};
                     262144 & e[0] && (o.width = t[18]), 1573888 & e[0] && (o.color = "interactions" === t[10] ? t[19] : t[20]), et.$set(o), (!st || 147456 & e[0]) && z(Q, "dont-show", 1 === t[17] || t[14]);
                     let l = ot;
                     ot = Lt(t), ot === l ? Mt[ot].p(t, e) : (ct(), ft(Mt[l], 1, 1, (() => {
                         Mt[l] = null
@@ -11949,17 +12002,17 @@
                     ft(q.$$.fragment, t), ft(_t), ft(et.$$.fragment, t), ft(lt), st = !1
                 },
                 d(t) {
                     t && f(e), h(vt, t), $t(q), wt && wt.d(), xt && xt.d(), _t && _t.d(), $t(et), nt(), Mt[ot].d(), at(), pt = !1, O(gt)
                 }
             }
         }
-        const Tf = 24;
+        const Of = 24;
 
-        function Nf(t, e, n) {
+        function Df(t, e, n) {
             let r, i, o, l, s, c, u, d, f, h, p, g, m, v, b, y, $, w, x, _, k, M;
             E(t, gr, (t => n(40, h = t))), E(t, xr, (t => n(41, p = t))), E(t, wr, (t => n(42, g = t))), E(t, _r, (t => n(43, m = t))), E(t, $r, (t => n(44, v = t))), E(t, yr, (t => n(45, b = t))), E(t, Mr, (t => n(29, y = t))), E(t, rr, (t => n(46, $ = t))), E(t, Zn, (t => n(47, w = t))), E(t, Pr, (t => n(48, x = t))), E(t, fr, (t => n(49, _ = t))), E(t, zr, (t => n(19, k = t))), E(t, Sr, (t => n(20, M = t)));
             let L, {
                     data: P
                 } = e,
                 {
                     sortingOptions: S
@@ -11974,15 +12027,15 @@
                 value: "centered-lines",
                 title: "Centered"
             }, {
                 value: "cluster-centers",
                 title: "Clusters"
             }];
             let N, C, O, D, j = "lines",
-                B = "interactions",
+                B = "predictions",
                 I = !1,
                 V = S[0];
 
             function H(t) {
                 n(13, I = !1), n(25, L = V.sort(t, {
                     highlightedIndices: _,
                     highlightedDistributions: x,
@@ -11999,15 +12052,15 @@
 
             function K(t) {
                 R(yr, b = t.x_feature, b), R($r, v = 2 === t.num_features ? t.y_feature : "", v), R(_r, m = W, m), 1 === t.num_features && (R(wr, g = "cluster-centers" === j ? "cluster-lines" : j, g), R(xr, p = "cluster-centers" === j ? "cluster-descriptions" : "scatterplot", p)), R(gr, h = "detailed-plot", h)
             }
             return t.$$set = t => {
                 "data" in t && n(0, P = t.data), "sortingOptions" in t && n(1, S = t.sortingOptions), "noPlotsMessage" in t && n(2, z = t.noPlotsMessage)
             }, t.$$.update = () => {
-                1 & t.$$.dirty[0] && n(17, r = rf(P) ? 1 : 2), 8 & t.$$.dirty[0] && n(28, i = N ? N.width : 0), 8 & t.$$.dirty[0] && n(27, o = N ? N.height : 0), 16 & t.$$.dirty[0] && n(18, l = C ? C.width : 140), 1 & t.$$.dirty[0] && n(26, s = Math.min(P.length, 12)), 67108864 & t.$$.dirty[0] && n(7, [c, u] = function(t) {
+                1 & t.$$.dirty[0] && n(17, r = af(P) ? 1 : 2), 8 & t.$$.dirty[0] && n(28, i = N ? N.width : 0), 8 & t.$$.dirty[0] && n(27, o = N ? N.height : 0), 16 & t.$$.dirty[0] && n(18, l = C ? C.width : 140), 1 & t.$$.dirty[0] && n(26, s = Math.min(P.length, 12)), 67108864 & t.$$.dirty[0] && n(7, [c, u] = function(t) {
                     const e = Math.ceil(Math.sqrt(t)),
                         n = Math.ceil(t / e);
                     return 1 === r ? [e, n] : [n, e]
                 }(s), c, (n(8, u), n(26, s), n(0, P))), 268435712 & t.$$.dirty[0] && n(11, O = Math.floor(i / u)), 134217856 & t.$$.dirty[0] && n(12, D = Math.floor(o / c)), 33 & t.$$.dirty[0] && (V.forBrushing || (n(25, L = V.sort(P)), F(1))), 33 & t.$$.dirty[0] && V.forBrushing && H(P), 536870912 & t.$$.dirty[0] && y && n(13, I = !0), 67108865 & t.$$.dirty[0] && n(15, d = Math.ceil(P.length / s)), 100663360 & t.$$.dirty[0] && n(16, f = L.slice((q - 1) * s, q * s))
             }, [P, S, z, N, C, V, q, c, u, j, B, O, D, I, W, d, f, r, l, k, M, T, H, F, K, L, s, o, i, y, () => F(q - 1), () => F(q + 1), function() {
                 V = A(this), n(5, V), n(1, S)
             }, () => H(P), function() {
@@ -12018,45 +12071,45 @@
                 B = A(this), n(10, B)
             }, function() {
                 C = a.entries.get(this)?.contentRect, n(4, C)
             }, t => K(t), function() {
                 N = a.entries.get(this)?.contentRect, n(3, N)
             }]
         }
-        const Cf = class extends _t {
+        const jf = class extends _t {
                 constructor(t) {
-                    super(), wt(this, t, Nf, zf, j, {
+                    super(), wt(this, t, Df, Cf, j, {
                         data: 0,
                         sortingOptions: 1,
                         noPlotsMessage: 2
-                    }, ff, [-1, -1])
+                    }, gf, [-1, -1])
                 }
             },
-            Of = [{
-                name: "Variance",
+            Bf = [{
+                name: "Importance",
                 forBrushing: !1,
                 sort: function(t) {
-                    return 0 !== t.length && rf(t) ? t.sort(((t, e) => ke(t.deviation, e.deviation))) : t
+                    return 0 !== t.length && af(t) ? t.sort(((t, e) => ke(t.deviation, e.deviation))) : t
                 }
             }, {
                 name: "Cluster difference",
                 forBrushing: !1,
                 sort: function(t) {
-                    if (0 === t.length || !rf(t)) return t;
+                    if (0 === t.length || !af(t)) return t;
 
                     function e(t) {
                         return 1 === t.ice.num_clusters ? -1 / 0 : zn(t).cluster_distance
                     }
                     return t.sort(((t, n) => ke(e(t), e(n))))
                 }
             }, {
-                name: "Highlighted similarity",
+                name: "Highlighted line similarity",
                 forBrushing: !0,
                 sort: function(t, e) {
-                    if (0 === t.length || !rf(t) || !e || !e.highlightedIndices || e.highlightedIndices.length <= 1 || !e.featureToIceLines) return t;
+                    if (0 === t.length || !af(t) || !e || !e.highlightedIndices || e.highlightedIndices.length <= 1 || !e.featureToIceLines) return t;
                     const n = e.highlightedIndices,
                         r = e.featureToIceLines,
                         i = Object.fromEntries(t.map((t => {
                             var e;
                             const i = r[t.x_feature],
                                 o = Tn(n.map((t => i[t]))),
                                 l = kn(o).map((t => {
@@ -12072,56 +12125,56 @@
                                     }))
                                 }(o, l, t.ice.centered_pdp);
                             return [t.x_feature, null !== (e = An(a)) && void 0 !== e ? e : 0]
                         })));
                     return t.sort(((t, e) => ke(i[t.x_feature], i[e.x_feature])))
                 }
             }, {
-                name: "Highlighted distribution",
+                name: "Highlighted histogram difference",
                 forBrushing: !0,
                 sort: function(t, e) {
-                    if (!(0 !== t.length && rf(t) && e && e.highlightedDistributions && e.featureInfo)) return t;
+                    if (!(0 !== t.length && af(t) && e && e.highlightedDistributions && e.featureInfo)) return t;
                     const n = e.highlightedDistributions,
                         r = e.featureInfo,
                         i = Object.fromEntries(t.map((t => {
                             const e = n.get(t.x_feature);
                             if (!e) return [t.x_feature, 0];
                             const i = r[t.x_feature].distribution.percents,
                                 o = e.percents;
                             let l = 0;
                             for (let t = 0; t < i.length; t++) l += Math.abs(o[t] - i[t]);
                             return [t.x_feature, l]
                         })));
                     return t.sort(((t, e) => ke(i[t.x_feature], i[e.x_feature])))
                 }
             }],
-            Df = [{
+            Ef = [{
                 name: "Interaction",
                 forBrushing: !1,
                 sort: function(t) {
-                    return 0 === t.length || rf(t) ? t : t.sort(((t, e) => ke(t.H, e.H)))
+                    return 0 === t.length || af(t) ? t : t.sort(((t, e) => ke(t.H, e.H)))
                 }
             }, {
                 name: "Variance",
                 forBrushing: !1,
                 sort: function(t) {
-                    return 0 === t.length || rf(t) ? t : t.sort(((t, e) => ke(t.deviation, e.deviation)))
+                    return 0 === t.length || af(t) ? t : t.sort(((t, e) => ke(t.deviation, e.deviation)))
                 }
             }];
 
-        function jf(t) {
+        function If(t) {
             u(t, "svelte-cuqal2", ".one-way-grid-container.svelte-cuqal2{height:100%;display:flex}.pdp-grid-wrapper.svelte-cuqal2{flex:1;min-width:0}")
         }
 
-        function Bf(t) {
+        function Rf(t) {
             let e, n, r, i, o, l, a;
-            return r = new nf({}), r.$on("changeFilters", t[1]), l = new Cf({
+            return r = new lf({}), r.$on("changeFilters", t[1]), l = new jf({
                 props: {
                     data: t[0],
-                    sortingOptions: Of,
+                    sortingOptions: Bf,
                     noPlotsMessage: "No plots to show."
                 }
             }), {
                 c() {
                     e = p("div"), n = p("div"), bt(r.$$.fragment), i = v(), o = p("div"), bt(l.$$.fragment), $(o, "class", "pdp-grid-wrapper svelte-cuqal2"), $(e, "class", "one-way-grid-container svelte-cuqal2")
                 },
                 m(t, s) {
@@ -12139,51 +12192,51 @@
                 },
                 d(t) {
                     t && f(e), $t(r), $t(l)
                 }
             }
         }
 
-        function Ef(t, e, n) {
+        function Vf(t, e, n) {
             let r, i, o;
             E(t, nr, (t => n(3, i = t))), E(t, Jn, (t => n(4, o = t)));
             let l = o;
             return t.$$.update = () => {
                 12 & t.$$.dirty && n(0, r = i.filter((t => l.includes(t.x_feature))))
             }, [r, function(t) {
                 n(2, l = t.detail)
             }, l, i]
         }
-        const If = class extends _t {
+        const Hf = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Ef, Bf, j, {}, jf)
+                super(), wt(this, t, Vf, Rf, j, {}, If)
             }
         };
 
-        function Rf(t) {
+        function qf(t) {
             u(t, "svelte-fnunp4", ".controls-container.svelte-fnunp4.svelte-fnunp4{height:100%;flex:0 0 200px;min-width:200px;max-width:200px;padding:0.25em;border-right:1px solid var(--gray-1);display:flex;flex-direction:column;gap:0.5em}.feature-selector-wrapper-outer.svelte-fnunp4.svelte-fnunp4{flex:0 1 auto;min-height:0;display:flex;flex-direction:column}.feature-selector-wrapper-middle.svelte-fnunp4.svelte-fnunp4{flex:1;min-height:0;display:flex;flex-direction:column}.feature-selector-wrapper-inner.svelte-fnunp4.svelte-fnunp4{flex:1;min-height:0}.filter-header.svelte-fnunp4+.filter-content.svelte-fnunp4{margin-top:0.25em}.filter-content.svelte-fnunp4.svelte-fnunp4{margin-left:0.75em}hr.svelte-fnunp4.svelte-fnunp4{margin:0.75em 0;border:0;height:1px;background:var(--gray-2)}.two-way-filter-radio.svelte-fnunp4.svelte-fnunp4{display:flex;flex-direction:column}")
         }
 
-        function Vf(t) {
+        function Ff(t) {
             let e, n, r, i, o, l, a, s, u, h, g, b, w, _, L, A, P, S, T, N, C, D, j, B, E, I, R, V, H, q;
 
             function F(e) {
                 t[7](e)
             }
             let W = {
                 title: "Name"
             };
-            void 0 !== t[1] && (W.expanded = t[1]), s = new Zd({
+            void 0 !== t[1] && (W.expanded = t[1]), s = new ef({
                 props: W
             }), X.push((() => vt(s, "expanded", F)));
             let K = {
                 enabledFeatures: t[3],
                 idPrefix: "pdpilot-two"
             };
-            return I = new qd({
+            return I = new Kd({
                 props: K
             }), t[11](I), I.$on("changeNameFilters", t[4]), V = x(t[9][0]), {
                 c() {
                     e = p("div"), n = p("div"), n.textContent = "Feature Filters", r = v(), i = p("button"), i.textContent = "Clear Filters", o = v(), l = p("div"), a = p("div"), bt(s.$$.fragment), h = v(), g = p("div"), b = p("div"), w = p("div"), w.textContent = "Plots must contain", _ = v(), L = p("label"), A = p("input"), P = m("\n          1+ selected feature"), S = v(), T = p("label"), N = p("input"), C = m("\n          2 selected features"), D = v(), j = p("hr"), B = v(), E = p("div"), bt(I.$$.fragment), $(n, "class", "pdpilot-bold"), M(i, "align-self", "start"), $(a, "class", "filter-header svelte-fnunp4"), $(A, "type", "radio"), $(A, "name", "op"), A.__value = "or", k(A, A.__value), $(N, "type", "radio"), $(N, "name", "op"), N.__value = "and", k(N, N.__value), $(b, "class", "two-way-filter-radio svelte-fnunp4"), $(j, "class", "svelte-fnunp4"), $(E, "class", "feature-selector-wrapper-inner svelte-fnunp4"), $(g, "class", "filter-content feature-selector-wrapper-middle svelte-fnunp4"), z(g, "pdp-hide", !t[1]), $(l, "class", "filter-container feature-selector-wrapper-outer svelte-fnunp4"), $(e, "class", "controls-container svelte-fnunp4"), V.p(A, N)
                 },
                 m(u, f) {
                     d(u, e, f), c(e, n), c(e, r), c(e, i), c(e, o), c(e, l), c(l, a), yt(s, a, null), c(l, h), c(l, g), c(g, b), c(b, w), c(b, _), c(b, L), c(L, A), A.checked = A.__value === t[2], c(L, P), c(b, S), c(b, T), c(T, N), N.checked = N.__value === t[2], c(T, C), c(g, D), c(g, j), c(g, B), c(g, E), yt(I, E, null), R = !0, H || (q = [y(i, "click", t[6]), y(A, "change", t[8]), y(A, "change", t[5]), y(N, "change", t[10]), y(N, "change", t[5])], H = !0)
@@ -12202,15 +12255,15 @@
                 },
                 d(n) {
                     n && f(e), $t(s), t[11](null), $t(I), V.r(), H = !1, O(q)
                 }
             }
         }
 
-        function Hf(t, e, n) {
+        function Wf(t, e, n) {
             let r;
             E(t, Jn, (t => n(3, r = t)));
             const i = W();
             let o, l = !0,
                 a = "and",
                 s = r;
             return [o, l, a, r, function(t) {
@@ -12239,30 +12292,30 @@
                 function(t) {
                     X[t ? "unshift" : "push"]((() => {
                         o = t, n(0, o)
                     }))
                 }
             ]
         }
-        const qf = class extends _t {
+        const Kf = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Hf, Vf, j, {}, Rf)
+                super(), wt(this, t, Wf, Ff, j, {}, qf)
             }
         };
 
-        function Ff(t) {
+        function Xf(t) {
             u(t, "svelte-1akrxps", ".two-way-grid-container.svelte-1akrxps{height:100%;display:flex}.pdp-grid-wrapper.svelte-1akrxps{flex:1;min-width:0}")
         }
 
-        function Wf(t) {
+        function Uf(t) {
             let e, n, r, i, o, l, a;
-            return r = new qf({}), r.$on("changeFilters", t[3]), l = new Cf({
+            return r = new Kf({}), r.$on("changeFilters", t[3]), l = new jf({
                 props: {
                     data: t[2],
-                    sortingOptions: Df,
+                    sortingOptions: Ef,
                     noPlotsMessage: 1 === t[0].length && "and" === t[1] ? "No plots to show." : "No plots to show. PDPilot only pre-computes two-way PDPs when it detects likely interaction between the pair of features."
                 }
             }), {
                 c() {
                     e = p("div"), n = p("div"), bt(r.$$.fragment), i = v(), o = p("div"), bt(l.$$.fragment), $(o, "class", "pdp-grid-wrapper svelte-1akrxps"), $(e, "class", "two-way-grid-container svelte-1akrxps")
                 },
                 m(t, s) {
@@ -12280,38 +12333,38 @@
                 },
                 d(t) {
                     t && f(e), $t(r), $t(l)
                 }
             }
         }
 
-        function Kf(t, e, n) {
+        function Yf(t, e, n) {
             let r, i, o;
             E(t, ir, (t => n(4, i = t))), E(t, Jn, (t => n(5, o = t)));
             let l = o,
                 a = "and";
             return t.$$.update = () => {
                 19 & t.$$.dirty && n(2, r = i.filter((t => "and" === a ? l.includes(t.x_feature) && l.includes(t.y_feature) : l.includes(t.x_feature) || l.includes(t.y_feature))))
             }, [l, a, r, function(t) {
                 n(0, l = t.detail.features), n(1, a = t.detail.op)
             }, i]
         }
-        const Xf = class extends _t {
+        const Gf = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Kf, Wf, j, {}, Ff)
+                super(), wt(this, t, Yf, Uf, j, {}, Xf)
             }
         };
 
-        function Uf(t) {
+        function Jf(t) {
             u(t, "svelte-mtrl6h", ".pdpilot-widget-container.svelte-mtrl6h{box-sizing:border-box;width:100%;display:flex;flex-direction:column;font-size:16px;border:1px solid var(--gray-1);background-color:white;color:black;--magenta:rgb(121, 35, 103);--blue:rgb(0, 95, 204);--dark-blue:rgb(1, 51, 104);--gray-0:rgb(247, 247, 247);--gray-1:rgb(226, 226, 226);--gray-2:rgb(198, 198, 198);--gray-3:rgb(171, 171, 171);--gray-4:rgb(145, 145, 145);--gray-5:rgb(119, 119, 119);--gray-6:rgb(94, 94, 94);--gray-7:rgb(71, 71, 71);--gray-8:rgb(48, 48, 48);--gray-9:rgb(27, 27, 27);--black:black;--red:#d62728;--light-red:#fc655a}.pdp-tab-content.svelte-mtrl6h{flex:1;min-height:0}.pdpilot-widget-container.svelte-mtrl6h .pdp-hide{display:none}.pdpilot-widget-container.svelte-mtrl6h canvas,.pdpilot-widget-container.svelte-mtrl6h svg{display:block}.pdpilot-widget-container.svelte-mtrl6h *{box-sizing:border-box;margin:0;padding:0;line-height:1.2}.pdpilot-widget-container.svelte-mtrl6h button{color:var(--blue);background-color:white;border:1px solid var(--blue);border-radius:0.25em;text-align:center;cursor:pointer;font-size:1em;line-height:1em;padding:0.0625em 0.0625em;font-family:inherit}.pdpilot-widget-container.svelte-mtrl6h button:hover:enabled{color:white;background-color:var(--blue)}.pdpilot-widget-container.svelte-mtrl6h button:active:enabled{color:white;background-color:var(--dark-blue);border-color:var(--dark-blue)}.pdpilot-widget-container.svelte-mtrl6h button:disabled{cursor:not-allowed;background-color:transparent;color:var(--gray-4);border-color:var(--gray-4)}.pdpilot-widget-container.svelte-mtrl6h h1{font-size:1.125em;font-weight:500}.pdpilot-widget-container.svelte-mtrl6h h2{font-size:1.0625em;font-weight:500}.pdpilot-widget-container.svelte-mtrl6h .pdpilot-large{font-size:1.125em}.pdpilot-widget-container.svelte-mtrl6h .pdpilot-small{font-size:0.875em}.pdpilot-widget-container.svelte-mtrl6h .pdpilot-bold{font-weight:500}.pdpilot-widget-container.svelte-mtrl6h .pdpilot-icon{width:1em;height:1em}.pdpilot-widget-container.svelte-mtrl6h .pdpilot-cutoff{overflow:hidden;white-space:nowrap;text-overflow:ellipsis}.pdpilot-widget-container.svelte-mtrl6h .icon-tabler{-webkit-transform:translate(0px, 0px);transform:translate(0px, 0px)}")
         }
 
-        function Yf(t) {
+        function Zf(t) {
             let e, n, r, i, o, l, a, s, u, h, g, m, b = `${t[0]}px`;
-            return n = new jr({}), o = new If({}), s = new Xf({}), g = new Bd({}), {
+            return n = new jr({}), o = new Hf({}), s = new Gf({}), g = new Rd({}), {
                 c() {
                     e = p("div"), bt(n.$$.fragment), r = v(), i = p("div"), bt(o.$$.fragment), l = v(), a = p("div"), bt(s.$$.fragment), u = v(), h = p("div"), bt(g.$$.fragment), $(i, "class", "pdp-tab-content svelte-mtrl6h"), z(i, "pdp-hide", "one-way-plots" !== t[1]), $(a, "class", "pdp-tab-content svelte-mtrl6h"), z(a, "pdp-hide", "two-way-plots" !== t[1]), $(h, "class", "pdp-tab-content svelte-mtrl6h"), z(h, "pdp-hide", "detailed-plot" !== t[1]), $(e, "class", "pdpilot-widget-container svelte-mtrl6h"), M(e, "height", b)
                 },
                 m(t, f) {
                     d(t, e, f), yt(n, e, null), c(e, r), c(e, i), yt(o, i, null), c(e, l), c(e, a), yt(s, a, null), c(e, u), c(e, h), yt(g, h, null), m = !0
                 },
                 p(t, [n]) {
@@ -12325,32 +12378,32 @@
                 },
                 d(t) {
                     t && f(e), $t(n), $t(o), $t(s), $t(g)
                 }
             }
         }
 
-        function Gf(t, e, n) {
+        function Qf(t, e, n) {
             let r, i;
             return E(t, dr, (t => n(0, r = t))), E(t, gr, (t => n(1, i = t))), [r, i]
         }
-        const Jf = class extends _t {
+        const th = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Gf, Yf, j, {}, Uf)
+                super(), wt(this, t, Qf, Zf, j, {}, Jf)
             }
         };
-        class Zf extends o.DOMWidgetModel {
+        class eh extends o.DOMWidgetModel {
             defaults() {
                 return Object.assign(Object.assign({}, super.defaults()), {
-                    _model_name: Zf.model_name,
-                    _model_module: Zf.model_module,
-                    _model_module_version: Zf.model_module_version,
-                    _view_name: Zf.view_name,
-                    _view_module: Zf.view_module,
-                    _view_module_version: Zf.view_module_version,
+                    _model_name: eh.model_name,
+                    _model_module: eh.model_module,
+                    _model_module_version: eh.model_module_version,
+                    _view_name: eh.view_name,
+                    _view_module: eh.view_module,
+                    _view_module_version: eh.view_module_version,
                     feature_names: [],
                     feature_info: {},
                     dataset: {},
                     labels: [],
                     num_instances: 0,
                     one_way_pds: [],
                     feature_to_ice_lines: {},
@@ -12364,16 +12417,16 @@
                     height: 600,
                     highlighted_indices: [],
                     two_way_to_calculate: [],
                     cluster_update: {}
                 })
             }
         }
-        Zf.serializers = Object.assign({}, o.DOMWidgetModel.serializers), Zf.model_name = "PDPilotModel", Zf.model_module = n, Zf.model_module_version = e, Zf.view_name = "PDPilotView", Zf.view_module = n, Zf.view_module_version = e;
-        class Qf extends o.DOMWidgetView {
+        eh.serializers = Object.assign({}, o.DOMWidgetModel.serializers), eh.model_name = "PDPilotModel", eh.model_module = n, eh.model_module_version = e, eh.view_name = "PDPilotView", eh.view_module = n, eh.view_module_version = e;
+        class nh extends o.DOMWidgetView {
             render() {
                 (function(t) {
                     Jn = Gn("feature_names", [], t), Zn = Gn("feature_info", {}, t), Qn = Gn("dataset", {}, t), tr = Gn("labels", [], t), er = Gn("num_instances", 0, t), nr = Gn("one_way_pds", [], t), rr = Gn("feature_to_ice_lines", {}, t), ir = Gn("two_way_pds", [], t), or = Gn("two_way_pdp_extent", [0, 0], t), lr = Gn("two_way_interaction_extent", [0, 0], t), ar = Gn("one_way_pdp_extent", [0, 0], t), sr = Gn("ice_line_extent", [0, 0], t), cr = Gn("ice_cluster_center_extent", [0, 0], t), ur = Gn("centered_ice_line_extent", [0, 0], t), dr = Gn("height", 600, t), fr = Gn("highlighted_indices", [], t), hr = Gn("two_way_to_calculate", [], t), pr = Gn("cluster_update", {}, t), gr = Mt("one-way-plots"), mr = Lt(nr, (t => new Map(t.map((t => [t.x_feature, t]))))), vr = Lt(tr, (t => 2 === new Set(t).size)), br = Lt([tr, vr], (([t, e]) => {
                         const n = [Math.min(...t), Math.max(...t)];
                         return e ? n : qn(n)
                     }));
                     const e = t.get("one_way_pds"),
@@ -12383,14 +12436,14 @@
                     }, ((t, e) => ({
                         x: (.5 + .7548776662466927 * e) % 1,
                         y: (.5 + .5698402909980532 * e) % 1
                     }))))), Mr = Mt(!1), Lr = Mt(""), Ar = Lt(fr, (t => new Set(t))), Pr = Lt([Zn, Qn, fr], (([t, e, n]) => new Map(Object.entries(t).map((([t, r]) => [t, Vn(r, e[t], n)]))))), Sr = Lt(or, (t => an().domain(qn(t)).interpolator(dn).unknown("black"))), zr = Lt(lr, (t => {
                         const e = qn([0, t[1]])[1];
                         return sn().domain([-e, 0, e]).interpolator(fn).unknown("black")
                     }))
-                })(this.model), new Jf({
+                })(this.model), new th({
                     target: this.el
                 })
             }
         }
     })(), i
 })()));
```

### Comparing `pdpilot-0.5.1/docs/source/conf.py` & `pdpilot-0.5.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/docs/source/developer-installation.rst` & `pdpilot-0.5.2/docs/source/developer-installation.rst`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/docs/source/index.rst` & `pdpilot-0.5.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/docs/source/installation.rst` & `pdpilot-0.5.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/docs/source/screenshots/detailed-plot-one-way-clusters.png` & `pdpilot-0.5.2/docs/source/screenshots/detailed-plot-one-way-clusters.png`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/docs/source/screenshots/detailed-plot-one-way-ground-truth.png` & `pdpilot-0.5.2/docs/source/screenshots/detailed-plot-one-way-ground-truth.png`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/docs/source/screenshots/detailed-plot-two-way.png` & `pdpilot-0.5.2/docs/source/screenshots/detailed-plot-two-way.png`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/docs/source/screenshots/one-way-plots.png` & `pdpilot-0.5.2/docs/source/screenshots/one-way-plots.png`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/docs/source/screenshots/two-way-plots.png` & `pdpilot-0.5.2/docs/source/screenshots/two-way-plots.png`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/docs/source/ui.rst` & `pdpilot-0.5.2/docs/source/ui.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 The One-way Plots tab shows a grid of `PDP <https://christophm.github.io/interpretable-ml-book/pdp.html>`_ + `ICE <https://christophm.github.io/interpretable-ml-book/ice.html>`_ plots, each containing one feature. Each plot shows the ICE lines in gray and the partial dependence line in black. Above each plot is a histogram showing the distribution of the feature's values in the dataset. In the row of controls at the top, the arrow buttons allow you to change pages. The “ICE” dropdown menu controls the type of visualization shown. The default is the standard ICE plot. Alternatively, you can show centered ICE plots, where all of the lines start at y = 0. Lastly, you can cluster the ICE lines and show the mean of each cluster. The “Scale locally” checkbox determines whether each plot has the same y-axis or each plot has its y-axis scaled to fit its own data. For normal ICE plots, scaling locally may not have any effect if the ICE lines already take up the full range of y-values.
 
 Brushing the lines on an ICE plot highlights the lines for those instances across all of the plots. When you brush lines, the histograms update to show both the distribution of the highlighted instances and the distribution of the entire dataset. The green bars show the distribution of the highlighted instances. The transparent bars with black outline show the distribution of the entire dataset. The two plots are overlaid so that you can compare the highlighted distribution to the overall distribution.
 
 The “Sort” dropdown menu controls how the plots are sorted. The one-way plots can be ranked according to one of several metrics:
 
-* **Variance**: Ranks the plots in descending order of the average amount of variance in the y-values (prediction target) of their ICE lines. The plots that have more variation are ranked higher.
+* **Importance**: Ranks the plots in descending order of the average amount of variance in the y-values (model prediction) of their ICE lines. The plots that have more variation are ranked higher.
 * **Cluster difference**: Ranks the plots in descending order of the total distance from the centers of the ICE line clusters to the partial dependence line. The plots that have more different clusters are ranked higher. This metric is paired best with the centered or clusters visualizations.
-* **Highlighted similarity**: Used in coordination with brushing ICE lines. This metric can be useful to identify if a cluster of instances in one plot is also a cluster in any others. Plots where the highlighted lines are closer together and farther from the partial dependence line are ranked first. The distances are computed on the centered ICE lines, so this metric is best paired with the centered ICE lines visualization. If you change the highlighted instances after selecting this metric, then clicking the refresh button next to the drop-down menu will update the rankings.
-* **Highlighted distribution**: Used in coordination with brushing ICE lines. For each plot, this metric measures the distance between the distribution of feature values for the highlighted instances to the distribution for all instances. The plots are sorted in descending order so that the features whose highlighted distributions are most different from the overall distributions are ranked higher. If you change the highlighted instances after selecting this metric, then clicking the refresh button next to the drop-down menu will update the rankings.
+* **Highlighted line similarity**: Used in coordination with brushing ICE lines. This metric can be useful to identify if a cluster of instances in one plot is also a cluster in any others. Plots where the highlighted lines are closer together and farther from the partial dependence line are ranked first. The distances are computed on the centered ICE lines, so this metric is best paired with the centered ICE lines visualization. If you change the highlighted instances after selecting this metric, then clicking the refresh button next to the drop-down menu will update the rankings.
+* **Highlighted histogram difference**: Used in coordination with brushing ICE lines. For each plot, this metric measures the distance between the distribution of feature values for the highlighted instances to the distribution for all instances. The plots are sorted in descending order so that the features whose highlighted distributions are most different from the overall distributions are ranked higher. If you change the highlighted instances after selecting this metric, then clicking the refresh button next to the drop-down menu will update the rankings.
 
 On the left sidebar, you can filter the plots by the type of the feature, by the shape of the PDP, and by feature name. Ordered features have values with defined orders, such as temperature or day of the week. Nominal features have values without defined orders. For ordered features, you can filter by whether the feature's PDP is generally increasing, decreasing, or sometimes increasing and sometimes decreasing.
 
 Two-way Plots
 -------------
 
 .. image:: screenshots/two-way-plots.png
```

### Comparing `pdpilot-0.5.1/examples/bike-rentals-regression.ipynb` & `pdpilot-0.5.2/examples/bike-rentals-regression.ipynb`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/examples/churn-classification.ipynb` & `pdpilot-0.5.2/examples/churn-classification.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970202494873548%*

 * *Differences: {"'cells'": '{15: {\'source\': {insert: [(4, "    ordinal_features={\'number customer service '*

 * *            'calls\'},\\n"), (5, "    nominal_features={\'area code\', \'international plan\', '*

 * *            '\'voice mail plan\'},\\n")], delete: [5, 4]}}, 18: {\'id\': \'0b46ed32\'}}',*

 * * "'metadata'": "{'language_info': {'version': '3.8.17'}}"}*

```diff
@@ -155,16 +155,16 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "pd_data = partial_dependence(\n",
                 "    predict=predict,\n",
                 "    df=subset,\n",
                 "    features=features,\n",
-                "    ordinal_features={'international plan', 'voice mail plan', 'number customer service calls'},\n",
-                "    nominal_features={'area code'},\n",
+                "    ordinal_features={'number customer service calls'},\n",
+                "    nominal_features={'area code', 'international plan', 'voice mail plan'},\n",
                 "    resolution=20,\n",
                 "    n_jobs=4,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
@@ -191,15 +191,15 @@
                 "\n",
                 "w"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a10b5c84",
+            "id": "0b46ed32",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
@@ -213,13 +213,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.16"
+            "version": "3.8.17"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pdpilot-0.5.1/examples/colab-example.ipynb` & `pdpilot-0.5.2/examples/colab-example.ipynb`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/package.json` & `pdpilot-0.5.2/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.5.2'"}*

```diff
@@ -87,9 +87,9 @@
         "prepack": "npm run build:prod",
         "test": "uvu -r tsm tests",
         "watch": "npm run watch:nbextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.5.1"
+    "version": "0.5.2"
 }
```

### Comparing `pdpilot-0.5.1/pdpilot/__init__.py` & `pdpilot-0.5.2/pdpilot/__init__.py`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/pdpilot/labextension/package.json` & `pdpilot-0.5.2/pdpilot/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9674479166666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.93d73cafbbe8e20d7f23.js'}}",*

 * * "'version'": "'0.5.2'"}*

```diff
@@ -57,15 +57,15 @@
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/DanielKerrigan/PDPilot",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.7d03101ac0d410913165.js"
+            "load": "static/remoteEntry.93d73cafbbe8e20d7f23.js"
         },
         "extension": true,
         "outputDir": "pdpilot/labextension/"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -91,9 +91,9 @@
         "prepack": "npm run build:prod",
         "test": "uvu -r tsm tests",
         "watch": "npm run watch:nbextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.5.1"
+    "version": "0.5.2"
 }
```

### Comparing `pdpilot-0.5.1/pdpilot/labextension/static/568.fc735409708fd22de78c.js` & `pdpilot-0.5.2/pdpilot/labextension/static/568.be4561957748b400120d.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -457,15 +457,15 @@
                         },
                         146: e => {
                             "use strict";
                             e.exports = t
                         },
                         147: t => {
                             "use strict";
-                            t.exports = JSON.parse('{"name":"pdpilot","version":"0.5.1","description":"A Jupyter widget for exploring PDP and ICE plots.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/DanielKerrigan/PDPilot","bugs":{"url":"https://github.com/DanielKerrigan/PDPilot/issues"},"license":"BSD-3-Clause","author":{"name":"Daniel Kerrigan","email":"kerrigan.d@northeastern.edu"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/DanielKerrigan/PDPilot"},"scripts":{"build":"webpack --mode=development && jupyter labextension build --development=True .","build:prod":"webpack --mode=production && jupyter labextension build .","clean":"npm run clean:lib && npm run clean:nbextension && npm run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf pdpilot/labextension","clean:nbextension":"rimraf pdpilot/nbextension/static/index.js","fix":"prettier --plugin-search-dir . --write src && eslint . --ext .ts,.tsx,.svelte --fix","check":"prettier --plugin-search-dir . --check src && eslint . --ext .ts,.tsx,.svelte && svelte-check","prepack":"npm run build:prod","watch":"npm run watch:nbextension","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch .","test":"uvu -r tsm tests"},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","d3":"^7.8.5","fast-kde":"^0.2.1","lodash.clonedeep":"^4.5.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3 || ^4","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@tsconfig/svelte":"^5.0.0","@types/d3":"^7.4.0","@types/lodash.clonedeep":"^4.5.7","@types/node":"^20.2.5","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.45.0","@typescript-eslint/parser":"^5.45.0","acorn":"^7.2.0","css-loader":"^6.7.0","eslint":"^8.28.0","eslint-config-prettier":"^8.5.0","eslint-plugin-svelte":"^2.30.0","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.8.0","prettier-plugin-svelte":"^2.10.1","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^3.0.0","svelte":"^4.0.0","svelte-check":"^3.4.6","svelte-loader":"^3.1.8","svelte-preprocess":"^5.0.4","ts-loader":"^9.0.0","tslib":"^2.4.1","tsm":"^2.2.1","typescript":"^5.1.6","uvu":"^0.5.3","webpack":">=5.76.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":true,"outputDir":"pdpilot/labextension/"}}')
+                            t.exports = JSON.parse('{"name":"pdpilot","version":"0.5.2","description":"A Jupyter widget for exploring PDP and ICE plots.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/DanielKerrigan/PDPilot","bugs":{"url":"https://github.com/DanielKerrigan/PDPilot/issues"},"license":"BSD-3-Clause","author":{"name":"Daniel Kerrigan","email":"kerrigan.d@northeastern.edu"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/DanielKerrigan/PDPilot"},"scripts":{"build":"webpack --mode=development && jupyter labextension build --development=True .","build:prod":"webpack --mode=production && jupyter labextension build .","clean":"npm run clean:lib && npm run clean:nbextension && npm run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf pdpilot/labextension","clean:nbextension":"rimraf pdpilot/nbextension/static/index.js","fix":"prettier --plugin-search-dir . --write src && eslint . --ext .ts,.tsx,.svelte --fix","check":"prettier --plugin-search-dir . --check src && eslint . --ext .ts,.tsx,.svelte && svelte-check","prepack":"npm run build:prod","watch":"npm run watch:nbextension","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch .","test":"uvu -r tsm tests"},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","d3":"^7.8.5","fast-kde":"^0.2.1","lodash.clonedeep":"^4.5.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3 || ^4","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@tsconfig/svelte":"^5.0.0","@types/d3":"^7.4.0","@types/lodash.clonedeep":"^4.5.7","@types/node":"^20.2.5","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.45.0","@typescript-eslint/parser":"^5.45.0","acorn":"^7.2.0","css-loader":"^6.7.0","eslint":"^8.28.0","eslint-config-prettier":"^8.5.0","eslint-plugin-svelte":"^2.30.0","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.8.0","prettier-plugin-svelte":"^2.10.1","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^3.0.0","svelte":"^4.0.0","svelte-check":"^3.4.6","svelte-loader":"^3.1.8","svelte-preprocess":"^5.0.4","ts-loader":"^9.0.0","tslib":"^2.4.1","tsm":"^2.2.1","typescript":"^5.1.6","uvu":"^0.5.3","webpack":">=5.76.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":true,"outputDir":"pdpilot/labextension/"}}')
                         }
                     },
                     r = {};
 
                 function i(t) {
                     var n = r[t];
                     if (void 0 !== n) return n.exports;
@@ -500,20 +500,20 @@
                         value: !0
                     })
                 }, i.nmd = t => (t.paths = [], t.children || (t.children = []), t);
                 var o = {};
                 return (() => {
                     "use strict";
                     i.r(o), i.d(o, {
-                        default: () => th
+                        default: () => rh
                     });
                     var t = {};
                     i.r(t), i.d(t, {
-                        PDPilotModel: () => Zf,
-                        PDPilotView: () => Qf
+                        PDPilotModel: () => eh,
+                        PDPilotView: () => nh
                     });
                     var e = i(146);
                     new Set;
                     const r = "undefined" != typeof window ? window : "undefined" != typeof globalThis ? globalThis : n.g;
                     class l {
                         _listeners = "WeakMap" in r ? new WeakMap : void 0;
                         _observer = void 0;
@@ -6259,15 +6259,15 @@
 
                     function Ls(t) {
                         let e, n, r, i, o, l, a, c, f, h, m, v, b = t[62].filteredIndices.length + "";
                         return a = new Va({
                             props: {
                                 scale: t[12],
                                 x: t[25].left,
-                                label: "centered prediction"
+                                label: "Centered prediction"
                             }
                         }), c = new Ma({
                             props: {
                                 scale: t[13],
                                 y: t[11] - t[25].bottom,
                                 showTickLabels: t[62].id === t[16][t[16].length - 1],
                                 showAxisLabel: t[62].id === t[16][t[16].length - 1],
@@ -6788,15 +6788,15 @@
                                 integerOnly: "discrete" === t[9].subkind,
                                 value_map: "value_map" in t[9] ? t[9].value_map : {}
                             }
                         }), l = new Va({
                             props: {
                                 scale: t[5],
                                 x: t[7].left,
-                                label: "centered prediction"
+                                label: "Centered prediction"
                             }
                         });
                         let h = t[3] && Is(t);
                         return {
                             c() {
                                 e = p("svg"), c && c.c(), n = p("path"), f && f.c(), i = v(), vt(o.$$.fragment), vt(l.$$.fragment), h && h.c(), y(n, "d", r = t[11](t[0].ice.centered_pdp)), y(n, "stroke", "var(--black)"), y(n, "stroke-width", "2"), y(n, "fill", "none"), y(e, "width", t[1]), y(e, "height", t[2])
                             },
@@ -7117,15 +7117,15 @@
                                 integerOnly: "discrete" === t[11].subkind,
                                 value_map: "value_map" in t[11] ? t[11].value_map : {}
                             }
                         }), a = new Va({
                             props: {
                                 scale: t[13],
                                 x: t[12].left,
-                                label: t[7] ? "centered prediction" : "prediction"
+                                label: t[7] ? "Centered prediction" : "Prediction"
                             }
                         });
                         let g = t[3] && Ks(t),
                             b = t[6] && t[18] === t[0].x_feature && Zs(t);
                         return {
                             c() {
                                 e = h("div"), n = h("canvas"), r = m(), i = p("svg"), o = p("g"), vt(l.$$.fragment), vt(a.$$.fragment), g && g.c(), c = v(), b && b.c(), y(n, "class", "svelte-hmor8t"), y(i, "width", t[1]), y(i, "height", t[2]), y(i, "class", "svelte-hmor8t"), y(e, "class", "pdpilot-plot-container svelte-hmor8t")
@@ -7133,15 +7133,15 @@
                             m(d, h) {
                                 u(d, e, h), s(e, n), t[41](n), s(e, r), s(e, i), s(i, o), bt(l, o, null), bt(a, o, null), g && g.m(o, null), s(o, c), b && b.m(o, null), t[42](o), f = !0
                             },
                             p(t, e) {
                                 const n = {};
                                 16384 & e[0] && (n.scale = t[14]), 4100 & e[0] && (n.y = t[2] - t[12].bottom), 1 & e[0] && (n.label = t[0].x_feature), 2048 & e[0] && (n.integerOnly = "discrete" === t[11].subkind), 2048 & e[0] && (n.value_map = "value_map" in t[11] ? t[11].value_map : {}), l.$set(n);
                                 const r = {};
-                                8192 & e[0] && (r.scale = t[13]), 4096 & e[0] && (r.x = t[12].left), 128 & e[0] && (r.label = t[7] ? "centered prediction" : "prediction"), a.$set(r), t[3] ? g ? (g.p(t, e), 8 & e[0] && ut(g, 1)) : (g = Ks(t), g.c(), ut(g, 1), g.m(o, c)) : g && (st(), dt(g, 1, 1, (() => {
+                                8192 & e[0] && (r.scale = t[13]), 4096 & e[0] && (r.x = t[12].left), 128 & e[0] && (r.label = t[7] ? "Centered prediction" : "Prediction"), a.$set(r), t[3] ? g ? (g.p(t, e), 8 & e[0] && ut(g, 1)) : (g = Ks(t), g.c(), ut(g, 1), g.m(o, c)) : g && (st(), dt(g, 1, 1, (() => {
                                     g = null
                                 })), ct()), t[6] && t[18] === t[0].x_feature ? b ? b.p(t, e) : (b = Zs(t), b.c(), b.m(o, null)) : b && (b.d(1), b = null), (!f || 2 & e[0]) && y(i, "width", t[1]), (!f || 4 & e[0]) && y(i, "height", t[2])
                             },
                             i(t) {
                                 f || (ut(l.$$.fragment, t), ut(a.$$.fragment, t), ut(g), f = !0)
                             },
                             o(t) {
@@ -7573,15 +7573,15 @@
                                     c = rn().domain([0, 1]).range([0, n.bandwidth()]);
                                 for (let d = 0; d < i.length; d++) {
                                     const p = s(a[d].x),
                                         g = c(a[d].y);
                                     t.strokeStyle = r(l[d]), t.beginPath(), t.arc((null !== (f = e(i[d])) && void 0 !== f ? f : 0) + p, (null !== (h = n(o[d])) && void 0 !== h ? h : 0) + g, u, 0, 2 * Math.PI), t.stroke()
                                 }
                             } else if ("bandwidth" in e && !("bandwidth" in n))
-                                if (e.bandwidth() >= 40) yn(Mn(i, o, l), (t => t[0])).forEach((([i, o]) => {
+                                if (e.bandwidth() >= 20) yn(Mn(i, o, l), (t => t[0])).forEach((([i, o]) => {
                                     var l, a;
                                     t.translate(null !== (l = e(i)) && void 0 !== l ? l : 0, 0),
                                         function(t, e, n, r, i, o, l, a, s) {
                                             var c;
                                             if (!e) return;
                                             const u = rn().domain([0, null !== (c = sc(t.densities, (t => t.density))) && void 0 !== c ? c : 0]).range([r / 2 - 2, 0]),
                                                 d = cc().x0((t => {
@@ -7595,15 +7595,15 @@
                                                 e.beginPath(), e.strokeStyle = "function" == typeof s ? s(i) : s, e.moveTo(r / 2 + 2, n(t)), e.lineTo(r, n(t)), e.stroke()
                                             })), e.globalAlpha = 1, e.fillStyle = "black", e.strokeStyle = "white", e.beginPath(), e.arc(r / 2, n(t.mean), 5, 0, 2 * Math.PI), e.fill(), e.stroke(), e.restore()
                                         }(Hn(o.map((t => t[1])), o.map((t => t[2]))), t, n, e.bandwidth(), c, d, 0, 0, r), t.translate(-(null !== (a = e(i)) && void 0 !== a ? a : 0), 0)
                                 }));
                                 else
                                     for (let a = 0; a < i.length; a++) t.strokeStyle = r(l[a]), t.beginPath(), t.moveTo(null !== (p = e(i[a])) && void 0 !== p ? p : 0, n(o[a])), t.lineTo((null !== (g = e(i[a])) && void 0 !== g ? g : 0) + e.bandwidth(), n(o[a])), t.stroke();
                             else if (!("bandwidth" in e) && "bandwidth" in n)
-                                if (n.bandwidth() >= 40) yn(Mn(i, o, l), (t => t[1])).forEach((([i, o]) => {
+                                if (n.bandwidth() >= 20) yn(Mn(i, o, l), (t => t[1])).forEach((([i, o]) => {
                                     var l, a;
                                     t.translate(0, null !== (l = n(i)) && void 0 !== l ? l : 0), fc(Hn(o.map((t => t[0])), o.map((t => t[2]))), t, e, s, n.bandwidth(), d, "rgb(145, 145, 145)", "black", r), t.translate(0, -(null !== (a = n(i)) && void 0 !== a ? a : 0))
                                 }));
                                 else
                                     for (let a = 0; a < i.length; a++) t.strokeStyle = r(l[a]), t.beginPath(), t.moveTo(e(i[a]), null !== (m = n(o[a])) && void 0 !== m ? m : 0), t.lineTo(e(i[a]), (null !== (v = n(o[a])) && void 0 !== v ? v : 0) + n.bandwidth()), t.stroke();
                             else if (!("bandwidth" in e) && !("bandwidth" in n)) {
                                 t.globalAlpha = d;
@@ -7760,86 +7760,139 @@
                                 marginRight: 10,
                                 marginLeft: 11,
                                 title: 2
                             }, hc)
                         }
                     };
 
-                    function xc(t) {
-                        let e, n, r, i;
+                    function xc(t, e, n) {
+                        const r = t.slice();
+                        return r[13] = e[n], r
+                    }
+
+                    function _c(t) {
+                        let e, n = ft(t[8]),
+                            r = [];
+                        for (let e = 0; e < n.length; e += 1) r[e] = kc(xc(t, n, e));
                         return {
                             c() {
-                                e = p("g"), n = p("path"), y(n, "d", r = t[2](t[3])), y(n, "stroke", t[1]), y(n, "fill", "none"), y(e, "transform", i = "translate(" + t[0] + ")")
+                                for (let t = 0; t < r.length; t += 1) r[t].c();
+                                e = v()
+                            },
+                            m(t, n) {
+                                for (let e = 0; e < r.length; e += 1) r[e] && r[e].m(t, n);
+                                u(t, e, n)
+                            },
+                            p(t, i) {
+                                if (377 & i) {
+                                    let o;
+                                    for (n = ft(t[8]), o = 0; o < n.length; o += 1) {
+                                        const l = xc(t, n, o);
+                                        r[o] ? r[o].p(l, i) : (r[o] = kc(l), r[o].c(), r[o].m(e.parentNode, e))
+                                    }
+                                    for (; o < r.length; o += 1) r[o].d(1);
+                                    r.length = n.length
+                                }
+                            },
+                            d(t) {
+                                t && d(e), f(r, t)
+                            }
+                        }
+                    }
+
+                    function kc(t) {
+                        let e, n, r;
+                        return {
+                            c() {
+                                e = p("circle"), y(e, "cx", n = "horizontal" === t[0] ? t[4](t[13]) : t[5](t[13])), y(e, "cy", r = "horizontal" === t[0] ? t[5](t[13]) : t[4](t[13])), y(e, "r", t[6]), y(e, "fill", t[3])
+                            },
+                            m(t, n) {
+                                u(t, e, n)
+                            },
+                            p(t, i) {
+                                305 & i && n !== (n = "horizontal" === t[0] ? t[4](t[13]) : t[5](t[13])) && y(e, "cx", n), 305 & i && r !== (r = "horizontal" === t[0] ? t[5](t[13]) : t[4](t[13])) && y(e, "cy", r), 64 & i && y(e, "r", t[6]), 8 & i && y(e, "fill", t[3])
+                            },
+                            d(t) {
+                                t && d(e)
+                            }
+                        }
+                    }
+
+                    function Mc(t) {
+                        let e, n, r, i, o = "bandwidth" in t[1] && _c(t);
+                        return {
+                            c() {
+                                e = p("g"), n = p("path"), o && o.c(), y(n, "d", r = t[7](t[8])), y(n, "stroke", t[3]), y(n, "fill", "none"), y(e, "transform", i = "translate(" + t[2] + ")")
                             },
                             m(t, r) {
-                                u(t, e, r), s(e, n)
+                                u(t, e, r), s(e, n), o && o.m(e, null)
                             },
-                            p(t, [o]) {
-                                12 & o && r !== (r = t[2](t[3])) && y(n, "d", r), 2 & o && y(n, "stroke", t[1]), 1 & o && i !== (i = "translate(" + t[0] + ")") && y(e, "transform", i)
+                            p(t, [l]) {
+                                384 & l && r !== (r = t[7](t[8])) && y(n, "d", r), 8 & l && y(n, "stroke", t[3]), "bandwidth" in t[1] ? o ? o.p(t, l) : (o = _c(t), o.c(), o.m(e, null)) : o && (o.d(1), o = null), 4 & l && i !== (i = "translate(" + t[2] + ")") && y(e, "transform", i)
                             },
                             i: z,
                             o: z,
                             d(t) {
-                                t && d(e)
+                                t && d(e), o && o.d()
                             }
                         }
                     }
 
-                    function _c(t, e, n) {
-                        let r, i, o, l, a, s;
-                        j(t, or, (t => n(11, s = t)));
+                    function Lc(t, e, n) {
+                        let r, i, o, l, a, s, c;
+                        j(t, or, (t => n(12, c = t)));
                         let {
-                            pd: c
+                            pd: u
                         } = e, {
-                            height: u
+                            height: d
                         } = e, {
-                            direction: d
+                            direction: f
                         } = e, {
-                            x: f
+                            x: h
                         } = e, {
-                            translate: h = [0, 0]
+                            translate: p = [0, 0]
                         } = e, {
-                            stroke: p = "black"
+                            stroke: g = "black"
                         } = e;
                         return t.$$set = t => {
-                            "pd" in t && n(4, c = t.pd), "height" in t && n(5, u = t.height), "direction" in t && n(6, d = t.direction), "x" in t && n(7, f = t.x), "translate" in t && n(0, h = t.translate), "stroke" in t && n(1, p = t.stroke)
+                            "pd" in t && n(9, u = t.pd), "height" in t && n(10, d = t.height), "direction" in t && n(0, f = t.direction), "x" in t && n(1, h = t.x), "translate" in t && n(2, p = t.translate), "stroke" in t && n(3, g = t.stroke)
                         }, t.$$.update = () => {
-                            16 & t.$$.dirty && n(3, r = xn(c.x_values.length)), 2144 & t.$$.dirty && n(10, i = rn().domain(s).range("horizontal" === d ? [u, 0] : [0, u])), 144 & t.$$.dirty && n(8, o = t => {
+                            512 & t.$$.dirty && n(8, r = xn(u.x_values.length)), 5121 & t.$$.dirty && n(11, i = rn().domain(c).range("horizontal" === f ? [d, 0] : [0, d])), 514 & t.$$.dirty && n(4, o = t => {
                                 var e;
-                                return "bandwidth" in f ? (null !== (e = f(c.x_values[t])) && void 0 !== e ? e : 0) + f.bandwidth() / 2 : f(c.x_values[t])
-                            }), 1040 & t.$$.dirty && n(9, l = t => i(c.mean_predictions[t])), 832 & t.$$.dirty && n(2, a = ni().x("horizontal" === d ? o : l).y("horizontal" === d ? l : o))
-                        }, [h, p, a, r, c, u, d, f, o, l, i, s]
+                                return "bandwidth" in h ? (null !== (e = h(u.x_values[t])) && void 0 !== e ? e : 0) + h.bandwidth() / 2 : h(u.x_values[t])
+                            }), 2560 & t.$$.dirty && n(5, l = t => i(u.mean_predictions[t])), 49 & t.$$.dirty && n(7, a = ni().x("horizontal" === f ? o : l).y("horizontal" === f ? l : o)), 2 & t.$$.dirty && n(6, s = "bandwidth" in h ? Math.min(2, h.bandwidth() / 2) : 0)
+                        }, [f, h, p, g, o, l, s, a, r, u, d, i, c]
                     }
-                    const kc = class extends xt {
+                    const Ac = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, _c, xc, D, {
-                                pd: 4,
-                                height: 5,
-                                direction: 6,
-                                x: 7,
-                                translate: 0,
-                                stroke: 1
+                            super(), $t(this, t, Lc, Mc, D, {
+                                pd: 9,
+                                height: 10,
+                                direction: 0,
+                                x: 1,
+                                translate: 2,
+                                stroke: 3
                             })
                         }
                     };
 
-                    function Mc(t) {
+                    function Pc(t) {
                         c(t, "svelte-crr1ai", ".two-way-container.svelte-crr1ai{position:relative;width:100%;height:100%}svg.svelte-crr1ai,canvas.svelte-crr1ai{position:absolute;top:var(--top);left:0}")
                     }
 
-                    function Lc(t) {
+                    function Sc(t) {
                         let e, n, r, i = t[12].left - t[21] + "px",
                             o = `${t[15]}px`;
                         return n = new wc({
                             props: {
                                 width: t[17] + t[20],
                                 height: t[16],
                                 color: t[8],
-                                marginLeft: Oc,
-                                marginRight: Oc,
+                                marginLeft: jc,
+                                marginRight: jc,
                                 title: t[4]
                             }
                         }), {
                             c() {
                                 e = h("div"), vt(n.$$.fragment), k(e, "margin-left", i), k(e, "padding-top", o)
                             },
                             m(t, i) {
@@ -7857,25 +7910,25 @@
                             },
                             d(t) {
                                 t && d(e), yt(n)
                             }
                         }
                     }
 
-                    function Ac(t) {
+                    function zc(t) {
                         let e, n, r;
-                        return e = new kc({
+                        return e = new Ac({
                             props: {
                                 pd: t[19],
                                 height: t[6],
                                 direction: "horizontal",
                                 x: t[10],
                                 translate: [0, t[12].top - t[6]]
                             }
-                        }), n = new kc({
+                        }), n = new Ac({
                             props: {
                                 pd: t[18],
                                 height: t[6],
                                 direction: "vertical",
                                 x: t[9],
                                 translate: [t[1] - t[12].right, 0]
                             }
@@ -7900,24 +7953,24 @@
                             },
                             d(t) {
                                 yt(e, t), yt(n, t)
                             }
                         }
                     }
 
-                    function Pc(t) {
+                    function Tc(t) {
                         let e, n, r, i, o, l, a;
-                        const s = [zc, Sc],
+                        const s = [Cc, Nc],
                             c = [];
 
                         function f(t, e) {
                             return "bandwidth" in t[10] ? 0 : 1
                         }
                         e = f(t), n = c[e] = s[e](t);
-                        const h = [Nc, Tc],
+                        const h = [Dc, Oc],
                             p = [];
 
                         function g(t, e) {
                             return "bandwidth" in t[9] ? 0 : 1
                         }
                         return i = g(t), o = p[i] = h[i](t), {
                             c() {
@@ -7944,15 +7997,15 @@
                             },
                             d(t) {
                                 t && (d(r), d(l)), c[e].d(t), p[i].d(t)
                             }
                         }
                     }
 
-                    function Sc(t) {
+                    function Nc(t) {
                         let e, n;
                         return e = new Qa({
                             props: {
                                 data: t[14].distribution,
                                 x: t[10],
                                 height: t[6],
                                 direction: "horizontal",
@@ -7977,15 +8030,15 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function zc(t) {
+                    function Cc(t) {
                         let e, n;
                         return e = new ds({
                             props: {
                                 data: t[14].distribution,
                                 x: t[10],
                                 height: t[6],
                                 direction: "horizontal",
@@ -8010,15 +8063,15 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function Tc(t) {
+                    function Oc(t) {
                         let e, n;
                         return e = new Qa({
                             props: {
                                 data: t[13].distribution,
                                 x: t[9],
                                 height: t[6],
                                 direction: "vertical",
@@ -8043,15 +8096,15 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function Nc(t) {
+                    function Dc(t) {
                         let e, n;
                         return e = new ds({
                             props: {
                                 data: t[13].distribution,
                                 x: t[9],
                                 height: t[6],
                                 direction: "vertical",
@@ -8076,17 +8129,17 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function Cc(t) {
+                    function Bc(t) {
                         let e, n, r, i, o, l, a, c, f, g, v = `${t[16]+t[15]}px`,
-                            b = t[5] && Lc(t);
+                            b = t[5] && Sc(t);
                         l = new Ma({
                             props: {
                                 scale: t[10],
                                 y: t[11] - t[12].bottom,
                                 label: t[0].x_feature,
                                 integerOnly: "discrete" === t[14].subkind,
                                 value_map: "value_map" in t[14] ? t[14].value_map : {}
@@ -8096,29 +8149,29 @@
                                 scale: t[9],
                                 x: t[12].left,
                                 label: t[0].y_feature,
                                 integerOnly: "discrete" === t[13].subkind,
                                 value_map: "value_map" in t[13] ? t[13].value_map : {}
                             }
                         });
-                        const $ = [Pc, Ac],
+                        const $ = [Tc, zc],
                             w = [];
 
                         function x(t, e) {
                             return t[2] ? 0 : t[3] && t[19] && t[18] ? 1 : -1
                         }
                         return ~(c = x(t)) && (f = w[c] = $[c](t)), {
                             c() {
                                 e = h("div"), b && b.c(), n = m(), r = h("canvas"), i = m(), o = p("svg"), vt(l.$$.fragment), vt(a.$$.fragment), f && f.c(), y(r, "class", "svelte-crr1ai"), y(o, "width", t[1]), y(o, "height", t[11]), y(o, "class", "svelte-crr1ai"), y(e, "class", "two-way-container svelte-crr1ai"), k(e, "--top", v)
                             },
                             m(d, f) {
                                 u(d, e, f), b && b.m(e, null), s(e, n), s(e, r), t[51](r), s(e, i), s(e, o), bt(l, o, null), bt(a, o, null), ~c && w[c].m(o, null), g = !0
                             },
                             p(t, r) {
-                                t[5] ? b ? (b.p(t, r), 32 & r[0] && ut(b, 1)) : (b = Lc(t), b.c(), ut(b, 1), b.m(e, n)) : b && (st(), dt(b, 1, 1, (() => {
+                                t[5] ? b ? (b.p(t, r), 32 & r[0] && ut(b, 1)) : (b = Sc(t), b.c(), ut(b, 1), b.m(e, n)) : b && (st(), dt(b, 1, 1, (() => {
                                     b = null
                                 })), ct());
                                 const i = {};
                                 1024 & r[0] && (i.scale = t[10]), 6144 & r[0] && (i.y = t[11] - t[12].bottom), 1 & r[0] && (i.label = t[0].x_feature), 16384 & r[0] && (i.integerOnly = "discrete" === t[14].subkind), 16384 & r[0] && (i.value_map = "value_map" in t[14] ? t[14].value_map : {}), l.$set(i);
                                 const s = {};
                                 512 & r[0] && (s.scale = t[9]), 4096 & r[0] && (s.x = t[12].left), 1 & r[0] && (s.label = t[0].y_feature), 8192 & r[0] && (s.integerOnly = "discrete" === t[13].subkind), 8192 & r[0] && (s.value_map = "value_map" in t[13] ? t[13].value_map : {}), a.$set(s);
                                 let u = c;
@@ -8133,17 +8186,17 @@
                                 dt(b), dt(l.$$.fragment, t), dt(a.$$.fragment, t), dt(f), g = !1
                             },
                             d(n) {
                                 n && d(e), b && b.d(), t[51](null), yt(l), yt(a), ~c && w[c].d()
                             }
                         }
                     }
-                    const Oc = 10;
+                    const jc = 10;
 
-                    function Dc(t, e, n) {
+                    function Ec(t, e, n) {
                         let r, i, o, l, a, s, c, u, d, f, h, p, g, m, v, b, y, $, w, x, _, k, M, L, A, P, S, z, T;
                         var N, C, O, D, B, E, I, R;
                         j(t, pr, (t => n(47, P = t))), j(t, Ar, (t => n(48, S = t))), j(t, Pr, (t => n(49, z = t))), j(t, Gn, (t => n(50, T = t)));
                         let V, H, {
                                 pd: F
                             } = e,
                             {
@@ -8190,66 +8243,66 @@
                                 bottom: 35,
                                 left: 50
                             }), 4259842 & t.$$.dirty[0] | 16384 & t.$$.dirty[1] && n(17, o = Math.min(W - i.left - i.right, X - r - i.top - i.bottom)), 131074 & t.$$.dirty[0] | 16384 & t.$$.dirty[1] && n(44, l = (W - o - i.left - i.right) / 2), 4390912 & t.$$.dirty[0] | 16384 & t.$$.dirty[1] && n(46, a = (X - r - o - i.top - i.bottom) / 2), 32 & t.$$.dirty[0] | 32768 & t.$$.dirty[1] && n(15, s = Q ? a : 0), 32768 & t.$$.dirty[0] | 57344 & t.$$.dirty[1] && n(12, c = {
                                 top: i.top + a - s,
                                 right: i.right + l,
                                 bottom: i.bottom + a,
                                 left: i.left + l
-                            }), 4292608 & t.$$.dirty[0] && n(11, u = X - r - s), 1 & t.$$.dirty[0] | 524288 & t.$$.dirty[1] && n(14, d = T[F.x_feature]), 1 & t.$$.dirty[0] | 524288 & t.$$.dirty[1] && n(13, f = T[F.y_feature]), 1 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(42, h = S.copy().domain([F.pdp_min, F.pdp_max])), 1 & t.$$.dirty[0] | 262144 & t.$$.dirty[1] && n(43, p = z.copy().domain([F.interaction_min, 0, F.interaction_max])), 25165824 & t.$$.dirty[0] | 399360 & t.$$.dirty[1] && n(8, g = "interactions" === J ? U ? p : z : U ? h : S), 1 & t.$$.dirty[0] && n(37, m = qn(F.x_axis)), 1 & t.$$.dirty[0] && n(36, v = qn(F.y_axis)), 402653185 & t.$$.dirty[0] | 64 & t.$$.dirty[1] && n(41, b = F.x_axis[0] - (null !== n(28, C = null === n(27, N = m.get(F.x_axis[0])) || void 0 === N ? void 0 : N.before) && void 0 !== C ? C : 0)), 1610612737 & t.$$.dirty[0] | 64 & t.$$.dirty[1] && n(40, y = F.x_axis[F.x_axis.length - 1] + (null !== n(30, D = null === n(29, O = m.get(F.x_axis[F.x_axis.length - 1])) || void 0 === O ? void 0 : O.after) && void 0 !== D ? D : 0)), 1 & t.$$.dirty[0] | 35 & t.$$.dirty[1] && n(39, $ = F.y_axis[0] - (null !== n(32, E = null === n(31, B = v.get(F.y_axis[0])) || void 0 === B ? void 0 : B.before) && void 0 !== E ? E : 0)), 1 & t.$$.dirty[0] | 44 & t.$$.dirty[1] && n(38, w = F.y_axis[F.y_axis.length - 1] + (null !== n(34, R = null === n(33, I = v.get(F.y_axis[F.y_axis.length - 1])) || void 0 === I ? void 0 : I.after) && void 0 !== R ? R : 0)), 20483 & t.$$.dirty[0] | 1536 & t.$$.dirty[1] && n(10, x = "quantitative" === d.kind ? rn().domain([b, y]).range([c.left, W - c.right]) : Rr().domain(F.x_axis).range([c.left, W - c.right])), 14337 & t.$$.dirty[0] | 384 & t.$$.dirty[1] && n(9, _ = "quantitative" === f.kind ? rn().domain([$, w]).range([u - c.bottom, c.top]) : Rr().domain(F.y_axis).range([u - c.bottom, c.top])), 2178 & t.$$.dirty[0] | 16 & t.$$.dirty[1] && H && (Bn(V, H, W, u), H && null != x && null != _ && uc(F, H, W, u, x, _, g, J, m, v)), 16781059 & t.$$.dirty[0] | 112 & t.$$.dirty[1] && H && null != x && null != _ && uc(F, H, W, u, x, _, g, J, m, v), 16 & t.$$.dirty[0] && n(21, k = "" === Z ? Oc : 0), 16 & t.$$.dirty[0] && n(20, M = "" === Z ? 2 * Oc : Oc), 1 & t.$$.dirty[0] | 65536 & t.$$.dirty[1] && n(19, L = P.get(F.x_feature)), 1 & t.$$.dirty[0] | 65536 & t.$$.dirty[1] && n(18, A = P.get(F.y_feature))
+                            }), 4292608 & t.$$.dirty[0] && n(11, u = X - r - s), 1 & t.$$.dirty[0] | 524288 & t.$$.dirty[1] && n(14, d = T[F.x_feature]), 1 & t.$$.dirty[0] | 524288 & t.$$.dirty[1] && n(13, f = T[F.y_feature]), 1 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(42, h = S.copy().domain([F.pdp_min, F.pdp_max])), 1 & t.$$.dirty[0] | 262144 & t.$$.dirty[1] && n(43, p = z.copy().domain([F.interaction_min, 0, F.interaction_max])), 25165824 & t.$$.dirty[0] | 399360 & t.$$.dirty[1] && n(8, g = "interactions" === J ? U ? p : z : U ? h : S), 1 & t.$$.dirty[0] && n(37, m = qn(F.x_axis)), 1 & t.$$.dirty[0] && n(36, v = qn(F.y_axis)), 402653185 & t.$$.dirty[0] | 64 & t.$$.dirty[1] && n(41, b = F.x_axis[0] - (null !== n(28, C = null === n(27, N = m.get(F.x_axis[0])) || void 0 === N ? void 0 : N.before) && void 0 !== C ? C : 0)), 1610612737 & t.$$.dirty[0] | 64 & t.$$.dirty[1] && n(40, y = F.x_axis[F.x_axis.length - 1] + (null !== n(30, D = null === n(29, O = m.get(F.x_axis[F.x_axis.length - 1])) || void 0 === O ? void 0 : O.after) && void 0 !== D ? D : 0)), 1 & t.$$.dirty[0] | 35 & t.$$.dirty[1] && n(39, $ = F.y_axis[0] - (null !== n(32, E = null === n(31, B = v.get(F.y_axis[0])) || void 0 === B ? void 0 : B.before) && void 0 !== E ? E : 0)), 1 & t.$$.dirty[0] | 44 & t.$$.dirty[1] && n(38, w = F.y_axis[F.y_axis.length - 1] + (null !== n(34, R = null === n(33, I = v.get(F.y_axis[F.y_axis.length - 1])) || void 0 === I ? void 0 : I.after) && void 0 !== R ? R : 0)), 20483 & t.$$.dirty[0] | 1536 & t.$$.dirty[1] && n(10, x = "quantitative" === d.kind ? rn().domain([b, y]).range([c.left, W - c.right]) : Rr().domain(F.x_axis).range([c.left, W - c.right])), 14337 & t.$$.dirty[0] | 384 & t.$$.dirty[1] && n(9, _ = "quantitative" === f.kind ? rn().domain([$, w]).range([u - c.bottom, c.top]) : Rr().domain(F.y_axis).range([u - c.bottom, c.top])), 2178 & t.$$.dirty[0] | 16 & t.$$.dirty[1] && H && (Bn(V, H, W, u), H && null != x && null != _ && uc(F, H, W, u, x, _, g, J, m, v)), 16781059 & t.$$.dirty[0] | 112 & t.$$.dirty[1] && H && null != x && null != _ && uc(F, H, W, u, x, _, g, J, m, v), 16 & t.$$.dirty[0] && n(21, k = "" === Z ? jc : 0), 16 & t.$$.dirty[0] && n(20, M = "" === Z ? 2 * jc : jc), 1 & t.$$.dirty[0] | 65536 & t.$$.dirty[1] && n(19, L = P.get(F.x_feature)), 1 & t.$$.dirty[0] | 65536 & t.$$.dirty[1] && n(18, A = P.get(F.y_feature))
                         }, [F, W, Y, G, Z, Q, nt, V, g, _, x, u, c, f, d, s, r, o, A, L, M, k, X, U, J, tt, et, N, C, O, D, B, E, I, R, H, v, m, w, $, y, b, h, p, l, i, a, P, S, z, T, function(t) {
                             K[t ? "unshift" : "push"]((() => {
                                 V = t, n(7, V)
                             }))
                         }]
                     }
-                    const Bc = class extends xt {
+                    const Ic = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, Dc, Cc, D, {
+                            super(), $t(this, t, Ec, Bc, D, {
                                 pd: 0,
                                 width: 1,
                                 height: 22,
                                 scaleLocally: 23,
                                 showMarginalDistribution: 2,
                                 showMarginalPdp: 3,
                                 colorShows: 24,
                                 colorLegendTitle: 4,
                                 showColorLegend: 5,
                                 marginTop: 25,
                                 marginRight: 26,
                                 marginalPlotHeight: 6
-                            }, Mc, [-1, -1])
+                            }, Pc, [-1, -1])
                         }
                     };
 
-                    function jc(t, e) {
+                    function Rc(t, e) {
                         for (var n = new Array(e), r = 0; r < e; ++r) n[r] = t(r / (e - 1));
                         return n
                     }
 
-                    function Ec(t) {
+                    function Vc(t) {
                         var e = t.length;
                         return function(n) {
                             return t[Math.max(0, Math.min(e - 1, Math.floor(n * e)))]
                         }
                     }
-                    const Ic = Ec(sn("44015444025645045745055946075a46085c460a5d460b5e470d60470e6147106347116447136548146748166848176948186a481a6c481b6d481c6e481d6f481f70482071482173482374482475482576482677482878482979472a7a472c7a472d7b472e7c472f7d46307e46327e46337f463480453581453781453882443983443a83443b84433d84433e85423f854240864241864142874144874045884046883f47883f48893e49893e4a893e4c8a3d4d8a3d4e8a3c4f8a3c508b3b518b3b528b3a538b3a548c39558c39568c38588c38598c375a8c375b8d365c8d365d8d355e8d355f8d34608d34618d33628d33638d32648e32658e31668e31678e31688e30698e306a8e2f6b8e2f6c8e2e6d8e2e6e8e2e6f8e2d708e2d718e2c718e2c728e2c738e2b748e2b758e2a768e2a778e2a788e29798e297a8e297b8e287c8e287d8e277e8e277f8e27808e26818e26828e26828e25838e25848e25858e24868e24878e23888e23898e238a8d228b8d228c8d228d8d218e8d218f8d21908d21918c20928c20928c20938c1f948c1f958b1f968b1f978b1f988b1f998a1f9a8a1e9b8a1e9c891e9d891f9e891f9f881fa0881fa1881fa1871fa28720a38620a48621a58521a68522a78522a88423a98324aa8325ab8225ac8226ad8127ad8128ae8029af7f2ab07f2cb17e2db27d2eb37c2fb47c31b57b32b67a34b67935b77937b87838b9773aba763bbb753dbc743fbc7340bd7242be7144bf7046c06f48c16e4ac16d4cc26c4ec36b50c46a52c56954c56856c66758c7655ac8645cc8635ec96260ca6063cb5f65cb5e67cc5c69cd5b6ccd5a6ece5870cf5773d05675d05477d1537ad1517cd2507fd34e81d34d84d44b86d54989d5488bd6468ed64590d74393d74195d84098d83e9bd93c9dd93ba0da39a2da37a5db36a8db34aadc32addc30b0dd2fb2dd2db5de2bb8de29bade28bddf26c0df25c2df23c5e021c8e020cae11fcde11dd0e11cd2e21bd5e21ad8e219dae319dde318dfe318e2e418e5e419e7e419eae51aece51befe51cf1e51df4e61ef6e620f8e621fbe723fde725"));
-                    Ec(sn("00000401000501010601010802010902020b02020d03030f03031204041405041606051806051a07061c08071e0907200a08220b09240c09260d0a290e0b2b100b2d110c2f120d31130d34140e36150e38160f3b180f3d19103f1a10421c10441d11471e114920114b21114e22115024125325125527125829115a2a115c2c115f2d11612f116331116533106734106936106b38106c390f6e3b0f703d0f713f0f72400f74420f75440f764510774710784910784a10794c117a4e117b4f127b51127c52137c54137d56147d57157e59157e5a167e5c167f5d177f5f187f601880621980641a80651a80671b80681c816a1c816b1d816d1d816e1e81701f81721f817320817521817621817822817922827b23827c23827e24828025828125818326818426818627818827818928818b29818c29818e2a81902a81912b81932b80942c80962c80982d80992d809b2e7f9c2e7f9e2f7fa02f7fa1307ea3307ea5317ea6317da8327daa337dab337cad347cae347bb0357bb2357bb3367ab5367ab73779b83779ba3878bc3978bd3977bf3a77c03a76c23b75c43c75c53c74c73d73c83e73ca3e72cc3f71cd4071cf4070d0416fd2426fd3436ed5446dd6456cd8456cd9466bdb476adc4869de4968df4a68e04c67e24d66e34e65e44f64e55064e75263e85362e95462ea5661eb5760ec5860ed5a5fee5b5eef5d5ef05f5ef1605df2625df2645cf3655cf4675cf4695cf56b5cf66c5cf66e5cf7705cf7725cf8745cf8765cf9785df9795df97b5dfa7d5efa7f5efa815ffb835ffb8560fb8761fc8961fc8a62fc8c63fc8e64fc9065fd9266fd9467fd9668fd9869fd9a6afd9b6bfe9d6cfe9f6dfea16efea36ffea571fea772fea973feaa74feac76feae77feb078feb27afeb47bfeb67cfeb77efeb97ffebb81febd82febf84fec185fec287fec488fec68afec88cfeca8dfecc8ffecd90fecf92fed194fed395fed597fed799fed89afdda9cfddc9efddea0fde0a1fde2a3fde3a5fde5a7fde7a9fde9aafdebacfcecaefceeb0fcf0b2fcf2b4fcf4b6fcf6b8fcf7b9fcf9bbfcfbbdfcfdbf")), Ec(sn("00000401000501010601010802010a02020c02020e03021004031204031405041706041907051b08051d09061f0a07220b07240c08260d08290e092b10092d110a30120a32140b34150b37160b39180c3c190c3e1b0c411c0c431e0c451f0c48210c4a230c4c240c4f260c51280b53290b552b0b572d0b592f0a5b310a5c320a5e340a5f3609613809623909633b09643d09653e0966400a67420a68440a68450a69470b6a490b6a4a0c6b4c0c6b4d0d6c4f0d6c510e6c520e6d540f6d550f6d57106e59106e5a116e5c126e5d126e5f136e61136e62146e64156e65156e67166e69166e6a176e6c186e6d186e6f196e71196e721a6e741a6e751b6e771c6d781c6d7a1d6d7c1d6d7d1e6d7f1e6c801f6c82206c84206b85216b87216b88226a8a226a8c23698d23698f24699025689225689326679526679727669827669a28659b29649d29649f2a63a02a63a22b62a32c61a52c60a62d60a82e5fa92e5eab2f5ead305dae305cb0315bb1325ab3325ab43359b63458b73557b93556ba3655bc3754bd3853bf3952c03a51c13a50c33b4fc43c4ec63d4dc73e4cc83f4bca404acb4149cc4248ce4347cf4446d04545d24644d34743d44842d54a41d74b3fd84c3ed94d3dda4e3cdb503bdd513ade5238df5337e05536e15635e25734e35933e45a31e55c30e65d2fe75e2ee8602de9612bea632aeb6429eb6628ec6726ed6925ee6a24ef6c23ef6e21f06f20f1711ff1731df2741cf3761bf37819f47918f57b17f57d15f67e14f68013f78212f78410f8850ff8870ef8890cf98b0bf98c0af98e09fa9008fa9207fa9407fb9606fb9706fb9906fb9b06fb9d07fc9f07fca108fca309fca50afca60cfca80dfcaa0ffcac11fcae12fcb014fcb216fcb418fbb61afbb81dfbba1ffbbc21fbbe23fac026fac228fac42afac62df9c72ff9c932f9cb35f8cd37f8cf3af7d13df7d340f6d543f6d746f5d949f5db4cf4dd4ff4df53f4e156f3e35af3e55df2e661f2e865f2ea69f1ec6df1ed71f1ef75f1f179f2f27df2f482f3f586f3f68af4f88ef5f992f6fa96f8fb9af9fc9dfafda1fcffa4"));
-                    var Rc = Ec(sn("0d088710078813078916078a19068c1b068d1d068e20068f2206902406912605912805922a05932c05942e05952f059631059733059735049837049938049a3a049a3c049b3e049c3f049c41049d43039e44039e46039f48039f4903a04b03a14c02a14e02a25002a25102a35302a35502a45601a45801a45901a55b01a55c01a65e01a66001a66100a76300a76400a76600a76700a86900a86a00a86c00a86e00a86f00a87100a87201a87401a87501a87701a87801a87a02a87b02a87d03a87e03a88004a88104a78305a78405a78606a68707a68808a68a09a58b0aa58d0ba58e0ca48f0da4910ea3920fa39410a29511a19613a19814a099159f9a169f9c179e9d189d9e199da01a9ca11b9ba21d9aa31e9aa51f99a62098a72197a82296aa2395ab2494ac2694ad2793ae2892b02991b12a90b22b8fb32c8eb42e8db52f8cb6308bb7318ab83289ba3388bb3488bc3587bd3786be3885bf3984c03a83c13b82c23c81c33d80c43e7fc5407ec6417dc7427cc8437bc9447aca457acb4679cc4778cc4977cd4a76ce4b75cf4c74d04d73d14e72d24f71d35171d45270d5536fd5546ed6556dd7566cd8576bd9586ada5a6ada5b69db5c68dc5d67dd5e66de5f65de6164df6263e06363e16462e26561e26660e3685fe4695ee56a5de56b5de66c5ce76e5be76f5ae87059e97158e97257ea7457eb7556eb7655ec7754ed7953ed7a52ee7b51ef7c51ef7e50f07f4ff0804ef1814df1834cf2844bf3854bf3874af48849f48948f58b47f58c46f68d45f68f44f79044f79143f79342f89441f89540f9973ff9983ef99a3efa9b3dfa9c3cfa9e3bfb9f3afba139fba238fca338fca537fca636fca835fca934fdab33fdac33fdae32fdaf31fdb130fdb22ffdb42ffdb52efeb72dfeb82cfeba2cfebb2bfebd2afebe2afec029fdc229fdc328fdc527fdc627fdc827fdca26fdcb26fccd25fcce25fcd025fcd225fbd324fbd524fbd724fad824fada24f9dc24f9dd25f8df25f8e125f7e225f7e425f6e626f6e826f5e926f5eb27f4ed27f3ee27f3f027f2f227f1f426f1f525f0f724f0f921"));
-                    const Vc = sn("4e79a7f28e2ce1575976b7b259a14fedc949af7aa1ff9da79c755fbab0ab");
+                    const Hc = Vc(sn("44015444025645045745055946075a46085c460a5d460b5e470d60470e6147106347116447136548146748166848176948186a481a6c481b6d481c6e481d6f481f70482071482173482374482475482576482677482878482979472a7a472c7a472d7b472e7c472f7d46307e46327e46337f463480453581453781453882443983443a83443b84433d84433e85423f854240864241864142874144874045884046883f47883f48893e49893e4a893e4c8a3d4d8a3d4e8a3c4f8a3c508b3b518b3b528b3a538b3a548c39558c39568c38588c38598c375a8c375b8d365c8d365d8d355e8d355f8d34608d34618d33628d33638d32648e32658e31668e31678e31688e30698e306a8e2f6b8e2f6c8e2e6d8e2e6e8e2e6f8e2d708e2d718e2c718e2c728e2c738e2b748e2b758e2a768e2a778e2a788e29798e297a8e297b8e287c8e287d8e277e8e277f8e27808e26818e26828e26828e25838e25848e25858e24868e24878e23888e23898e238a8d228b8d228c8d228d8d218e8d218f8d21908d21918c20928c20928c20938c1f948c1f958b1f968b1f978b1f988b1f998a1f9a8a1e9b8a1e9c891e9d891f9e891f9f881fa0881fa1881fa1871fa28720a38620a48621a58521a68522a78522a88423a98324aa8325ab8225ac8226ad8127ad8128ae8029af7f2ab07f2cb17e2db27d2eb37c2fb47c31b57b32b67a34b67935b77937b87838b9773aba763bbb753dbc743fbc7340bd7242be7144bf7046c06f48c16e4ac16d4cc26c4ec36b50c46a52c56954c56856c66758c7655ac8645cc8635ec96260ca6063cb5f65cb5e67cc5c69cd5b6ccd5a6ece5870cf5773d05675d05477d1537ad1517cd2507fd34e81d34d84d44b86d54989d5488bd6468ed64590d74393d74195d84098d83e9bd93c9dd93ba0da39a2da37a5db36a8db34aadc32addc30b0dd2fb2dd2db5de2bb8de29bade28bddf26c0df25c2df23c5e021c8e020cae11fcde11dd0e11cd2e21bd5e21ad8e219dae319dde318dfe318e2e418e5e419e7e419eae51aece51befe51cf1e51df4e61ef6e620f8e621fbe723fde725"));
+                    Vc(sn("00000401000501010601010802010902020b02020d03030f03031204041405041606051806051a07061c08071e0907200a08220b09240c09260d0a290e0b2b100b2d110c2f120d31130d34140e36150e38160f3b180f3d19103f1a10421c10441d11471e114920114b21114e22115024125325125527125829115a2a115c2c115f2d11612f116331116533106734106936106b38106c390f6e3b0f703d0f713f0f72400f74420f75440f764510774710784910784a10794c117a4e117b4f127b51127c52137c54137d56147d57157e59157e5a167e5c167f5d177f5f187f601880621980641a80651a80671b80681c816a1c816b1d816d1d816e1e81701f81721f817320817521817621817822817922827b23827c23827e24828025828125818326818426818627818827818928818b29818c29818e2a81902a81912b81932b80942c80962c80982d80992d809b2e7f9c2e7f9e2f7fa02f7fa1307ea3307ea5317ea6317da8327daa337dab337cad347cae347bb0357bb2357bb3367ab5367ab73779b83779ba3878bc3978bd3977bf3a77c03a76c23b75c43c75c53c74c73d73c83e73ca3e72cc3f71cd4071cf4070d0416fd2426fd3436ed5446dd6456cd8456cd9466bdb476adc4869de4968df4a68e04c67e24d66e34e65e44f64e55064e75263e85362e95462ea5661eb5760ec5860ed5a5fee5b5eef5d5ef05f5ef1605df2625df2645cf3655cf4675cf4695cf56b5cf66c5cf66e5cf7705cf7725cf8745cf8765cf9785df9795df97b5dfa7d5efa7f5efa815ffb835ffb8560fb8761fc8961fc8a62fc8c63fc8e64fc9065fd9266fd9467fd9668fd9869fd9a6afd9b6bfe9d6cfe9f6dfea16efea36ffea571fea772fea973feaa74feac76feae77feb078feb27afeb47bfeb67cfeb77efeb97ffebb81febd82febf84fec185fec287fec488fec68afec88cfeca8dfecc8ffecd90fecf92fed194fed395fed597fed799fed89afdda9cfddc9efddea0fde0a1fde2a3fde3a5fde5a7fde7a9fde9aafdebacfcecaefceeb0fcf0b2fcf2b4fcf4b6fcf6b8fcf7b9fcf9bbfcfbbdfcfdbf")), Vc(sn("00000401000501010601010802010a02020c02020e03021004031204031405041706041907051b08051d09061f0a07220b07240c08260d08290e092b10092d110a30120a32140b34150b37160b39180c3c190c3e1b0c411c0c431e0c451f0c48210c4a230c4c240c4f260c51280b53290b552b0b572d0b592f0a5b310a5c320a5e340a5f3609613809623909633b09643d09653e0966400a67420a68440a68450a69470b6a490b6a4a0c6b4c0c6b4d0d6c4f0d6c510e6c520e6d540f6d550f6d57106e59106e5a116e5c126e5d126e5f136e61136e62146e64156e65156e67166e69166e6a176e6c186e6d186e6f196e71196e721a6e741a6e751b6e771c6d781c6d7a1d6d7c1d6d7d1e6d7f1e6c801f6c82206c84206b85216b87216b88226a8a226a8c23698d23698f24699025689225689326679526679727669827669a28659b29649d29649f2a63a02a63a22b62a32c61a52c60a62d60a82e5fa92e5eab2f5ead305dae305cb0315bb1325ab3325ab43359b63458b73557b93556ba3655bc3754bd3853bf3952c03a51c13a50c33b4fc43c4ec63d4dc73e4cc83f4bca404acb4149cc4248ce4347cf4446d04545d24644d34743d44842d54a41d74b3fd84c3ed94d3dda4e3cdb503bdd513ade5238df5337e05536e15635e25734e35933e45a31e55c30e65d2fe75e2ee8602de9612bea632aeb6429eb6628ec6726ed6925ee6a24ef6c23ef6e21f06f20f1711ff1731df2741cf3761bf37819f47918f57b17f57d15f67e14f68013f78212f78410f8850ff8870ef8890cf98b0bf98c0af98e09fa9008fa9207fa9407fb9606fb9706fb9906fb9b06fb9d07fc9f07fca108fca309fca50afca60cfca80dfcaa0ffcac11fcae12fcb014fcb216fcb418fbb61afbb81dfbba1ffbbc21fbbe23fac026fac228fac42afac62df9c72ff9c932f9cb35f8cd37f8cf3af7d13df7d340f6d543f6d746f5d949f5db4cf4dd4ff4df53f4e156f3e35af3e55df2e661f2e865f2ea69f1ec6df1ed71f1ef75f1f179f2f27df2f482f3f586f3f68af4f88ef5f992f6fa96f8fb9af9fc9dfafda1fcffa4"));
+                    var qc = Vc(sn("0d088710078813078916078a19068c1b068d1d068e20068f2206902406912605912805922a05932c05942e05952f059631059733059735049837049938049a3a049a3c049b3e049c3f049c41049d43039e44039e46039f48039f4903a04b03a14c02a14e02a25002a25102a35302a35502a45601a45801a45901a55b01a55c01a65e01a66001a66100a76300a76400a76600a76700a86900a86a00a86c00a86e00a86f00a87100a87201a87401a87501a87701a87801a87a02a87b02a87d03a87e03a88004a88104a78305a78405a78606a68707a68808a68a09a58b0aa58d0ba58e0ca48f0da4910ea3920fa39410a29511a19613a19814a099159f9a169f9c179e9d189d9e199da01a9ca11b9ba21d9aa31e9aa51f99a62098a72197a82296aa2395ab2494ac2694ad2793ae2892b02991b12a90b22b8fb32c8eb42e8db52f8cb6308bb7318ab83289ba3388bb3488bc3587bd3786be3885bf3984c03a83c13b82c23c81c33d80c43e7fc5407ec6417dc7427cc8437bc9447aca457acb4679cc4778cc4977cd4a76ce4b75cf4c74d04d73d14e72d24f71d35171d45270d5536fd5546ed6556dd7566cd8576bd9586ada5a6ada5b69db5c68dc5d67dd5e66de5f65de6164df6263e06363e16462e26561e26660e3685fe4695ee56a5de56b5de66c5ce76e5be76f5ae87059e97158e97257ea7457eb7556eb7655ec7754ed7953ed7a52ee7b51ef7c51ef7e50f07f4ff0804ef1814df1834cf2844bf3854bf3874af48849f48948f58b47f58c46f68d45f68f44f79044f79143f79342f89441f89540f9973ff9983ef99a3efa9b3dfa9c3cfa9e3bfb9f3afba139fba238fca338fca537fca636fca835fca934fdab33fdac33fdae32fdaf31fdb130fdb22ffdb42ffdb52efeb72dfeb82cfeba2cfebb2bfebd2afebe2afec029fdc229fdc328fdc527fdc627fdc827fdca26fdcb26fccd25fcce25fcd025fcd225fbd324fbd524fbd724fad824fada24f9dc24f9dd25f8df25f8e125f7e225f7e425f6e626f6e826f5e926f5eb27f4ed27f3ee27f3f027f2f227f1f426f1f525f0f724f0f921"));
+                    const Fc = sn("4e79a7f28e2ce1575976b7b259a14fedc949af7aa1ff9da79c755fbab0ab");
 
-                    function Hc(t) {
+                    function Wc(t) {
                         c(t, "svelte-1pgkml6", ".color-container.svelte-1pgkml6{display:flex;align-items:center;gap:1em}.swatches.svelte-1pgkml6{flex:1;display:flex;gap:1em}.swatch-cell.svelte-1pgkml6{display:flex;align-items:center}.swatch-square.svelte-1pgkml6{min-width:var(--size);min-height:var(--size);margin-right:0.25em}")
                     }
 
-                    function qc(t, e, n) {
+                    function Kc(t, e, n) {
                         const r = t.slice();
                         return r[10] = e[n], r
                     }
 
-                    function Fc(t) {
+                    function Xc(t) {
                         let e, n, r;
                         return {
                             c() {
                                 e = h("div"), n = g(t[5]), r = g(":"), y(e, "class", "pdpilot-small pdpilot-bold")
                             },
                             m(t, i) {
                                 u(t, e, i), s(e, n), s(e, r)
@@ -8259,16 +8312,16 @@
                             },
                             d(t) {
                                 t && d(e)
                             }
                         }
                     }
 
-                    function Wc(t) {
-                        let e, n, r, i, o, l, a = `${Xc}px`,
+                    function Uc(t) {
+                        let e, n, r, i, o, l, a = `${Gc}px`,
                             c = (t[6][t[10]] ?? t[10]) + "";
                         return {
                             c() {
                                 e = h("div"), n = h("div"), r = m(), i = h("div"), o = g(c), l = m(), y(n, "class", "swatch-square svelte-1pgkml6"), k(n, "--size", a), k(n, "background-color", t[2](t[10])), y(i, "class", "swatch-label pdpilot-small"), y(e, "class", "swatch-cell svelte-1pgkml6")
                             },
                             m(t, a) {
                                 u(t, e, a), s(e, n), s(e, r), s(e, i), s(i, o), s(e, l)
@@ -8278,57 +8331,57 @@
                             },
                             d(t) {
                                 t && d(e)
                             }
                         }
                     }
 
-                    function Kc(t) {
+                    function Yc(t) {
                         let e, n, r, i, o = `${t[8]}px`,
                             l = `${t[1]}px`,
                             a = `${t[0]}px`,
                             c = `${t[3]}px`,
                             p = `${t[4]}px`,
-                            g = "" !== t[5] && Fc(t),
+                            g = "" !== t[5] && Xc(t),
                             v = ft(t[2].domain()),
                             b = [];
-                        for (let e = 0; e < v.length; e += 1) b[e] = Wc(qc(t, v, e));
+                        for (let e = 0; e < v.length; e += 1) b[e] = Uc(Kc(t, v, e));
                         return {
                             c() {
                                 e = h("div"), g && g.c(), n = m(), r = h("div");
                                 for (let t = 0; t < b.length; t += 1) b[t].c();
                                 y(r, "class", "swatches svelte-1pgkml6"), k(r, "max-width", o), y(e, "class", "color-container svelte-1pgkml6"), k(e, "max-height", l), k(e, "max-width", a), k(e, "margin-left", c), k(e, "margin-right", p)
                             },
                             m(o, l) {
                                 u(o, e, l), g && g.m(e, null), s(e, n), s(e, r);
                                 for (let t = 0; t < b.length; t += 1) b[t] && b[t].m(r, null);
                                 i = P.observe(r, t[9].bind(r))
                             },
                             p(t, [i]) {
-                                if ("" !== t[5] ? g ? g.p(t, i) : (g = Fc(t), g.c(), g.m(e, n)) : g && (g.d(1), g = null), 68 & i) {
+                                if ("" !== t[5] ? g ? g.p(t, i) : (g = Xc(t), g.c(), g.m(e, n)) : g && (g.d(1), g = null), 68 & i) {
                                     let e;
                                     for (v = ft(t[2].domain()), e = 0; e < v.length; e += 1) {
-                                        const n = qc(t, v, e);
-                                        b[e] ? b[e].p(n, i) : (b[e] = Wc(n), b[e].c(), b[e].m(r, null))
+                                        const n = Kc(t, v, e);
+                                        b[e] ? b[e].p(n, i) : (b[e] = Uc(n), b[e].c(), b[e].m(r, null))
                                     }
                                     for (; e < b.length; e += 1) b[e].d(1);
                                     b.length = v.length
                                 }
                                 256 & i && o !== (o = `${t[8]}px`) && k(r, "max-width", o), 2 & i && l !== (l = `${t[1]}px`) && k(e, "max-height", l), 1 & i && a !== (a = `${t[0]}px`) && k(e, "max-width", a), 8 & i && c !== (c = `${t[3]}px`) && k(e, "margin-left", c), 16 & i && p !== (p = `${t[4]}px`) && k(e, "margin-right", p)
                             },
                             i: z,
                             o: z,
                             d(t) {
                                 t && d(e), g && g.d(), f(b, t), i()
                             }
                         }
                     }
-                    const Xc = 12;
+                    const Gc = 12;
 
-                    function Uc(t, e, n) {
+                    function Jc(t, e, n) {
                         let r, {
                                 width: i
                             } = e,
                             {
                                 height: o
                             } = e,
                             {
@@ -8351,35 +8404,35 @@
                             "width" in t && n(0, i = t.width), "height" in t && n(1, o = t.height), "color" in t && n(2, a = t.color), "marginLeft" in t && n(3, s = t.marginLeft), "marginRight" in t && n(4, c = t.marginRight), "title" in t && n(5, u = t.title), "value_map" in t && n(6, d = t.value_map)
                         }, t.$$.update = () => {
                             128 & t.$$.dirty && n(8, f = r ? r[0].inlineSize : 0)
                         }, [i, o, a, s, c, u, d, r, f, function() {
                             r = l.entries.get(this)?.borderBoxSize, n(7, r)
                         }]
                     }
-                    const Yc = class extends xt {
+                    const Zc = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, Uc, Kc, D, {
+                            super(), $t(this, t, Jc, Yc, D, {
                                 width: 0,
                                 height: 1,
                                 color: 2,
                                 marginLeft: 3,
                                 marginRight: 4,
                                 title: 5,
                                 value_map: 6
-                            }, Hc)
+                            }, Wc)
                         }
                     };
 
-                    function Gc(t) {
+                    function Qc(t) {
                         c(t, "svelte-crr1ai", ".two-way-container.svelte-crr1ai{position:relative;width:100%;height:100%}svg.svelte-crr1ai,canvas.svelte-crr1ai{position:absolute;top:var(--top);left:0}")
                     }
 
-                    function Jc(t) {
+                    function tu(t) {
                         let e, n, r, i, o = `${t[9].left}px`;
-                        const l = [Qc, Zc],
+                        const l = [nu, eu],
                             a = [];
 
                         function s(t, e) {
                             return "interpolator" in t[4] ? 0 : 1
                         }
                         return n = s(t), r = a[n] = l[n](t), {
                             c() {
@@ -8402,17 +8455,17 @@
                             },
                             d(t) {
                                 t && d(e), a[n].d()
                             }
                         }
                     }
 
-                    function Zc(t) {
+                    function eu(t) {
                         let e, n;
-                        return e = new Yc({
+                        return e = new Zc({
                             props: {
                                 width: t[1] - t[9].left - t[9].right,
                                 height: t[11],
                                 color: t[4],
                                 value_map: "value_map" in t[8] ? t[8].value_map : {},
                                 title: t[0].y_feature,
                                 marginLeft: 10,
@@ -8437,15 +8490,15 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function Qc(t) {
+                    function nu(t) {
                         let e, n;
                         return e = new wc({
                             props: {
                                 width: t[1] - t[9].left - t[9].right,
                                 height: t[11],
                                 color: t[4],
                                 title: t[0].y_feature,
@@ -8471,16 +8524,16 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function tu(t) {
-                        let e, n, r, i, o, l, a, c, f = t[2] && Jc(t);
+                    function ru(t) {
+                        let e, n, r, i, o, l, a, c, f = t[2] && tu(t);
                         return l = new Ma({
                             props: {
                                 scale: t[6],
                                 y: t[7] - t[9].bottom,
                                 label: t[0].x_feature,
                                 integerOnly: "discrete" === t[10].subkind,
                                 value_map: "value_map" in t[10] ? t[10].value_map : {}
@@ -8497,15 +8550,15 @@
                             c() {
                                 e = h("div"), f && f.c(), n = m(), r = h("canvas"), i = m(), o = p("svg"), vt(l.$$.fragment), vt(a.$$.fragment), y(r, "class", "svelte-crr1ai"), y(o, "width", t[1]), y(o, "height", t[7]), y(o, "class", "svelte-crr1ai"), y(e, "class", "two-way-container svelte-crr1ai"), k(e, "--top", t[11])
                             },
                             m(d, h) {
                                 u(d, e, h), f && f.m(e, null), s(e, n), s(e, r), t[23](r), s(e, i), s(e, o), bt(l, o, null), bt(a, o, null), c = !0
                             },
                             p(t, [r]) {
-                                t[2] ? f ? (f.p(t, r), 4 & r && ut(f, 1)) : (f = Jc(t), f.c(), ut(f, 1), f.m(e, n)) : f && (st(), dt(f, 1, 1, (() => {
+                                t[2] ? f ? (f.p(t, r), 4 & r && ut(f, 1)) : (f = tu(t), f.c(), ut(f, 1), f.m(e, n)) : f && (st(), dt(f, 1, 1, (() => {
                                     f = null
                                 })), ct());
                                 const i = {};
                                 64 & r && (i.scale = t[6]), 640 & r && (i.y = t[7] - t[9].bottom), 1 & r && (i.label = t[0].x_feature), 1024 & r && (i.integerOnly = "discrete" === t[10].subkind), 1024 & r && (i.value_map = "value_map" in t[10] ? t[10].value_map : {}), l.$set(i);
                                 const s = {};
                                 32 & r && (s.scale = t[5]), 512 & r && (s.x = t[9].left), 256 & r && (s.integerOnly = "discrete" === t[8].subkind), 256 & r && (s.value_map = "value_map" in t[8] ? t[8].value_map : {}), a.$set(s), (!c || 2 & r) && y(o, "width", t[1]), (!c || 128 & r) && y(o, "height", t[7]), 2048 & r && k(e, "--top", t[11])
                             },
@@ -8517,15 +8570,15 @@
                             },
                             d(n) {
                                 n && d(e), f && f.d(), t[23](null), yt(l), yt(a)
                             }
                         }
                     }
 
-                    function eu(t, e, n) {
+                    function iu(t, e, n) {
                         let r, i, o, l, a, s, c, u, d, f, h, p, g, m;
                         j(t, rr, (t => n(21, g = t))), j(t, Gn, (t => n(22, m = t)));
                         let v, b, {
                                 pd: y
                             } = e,
                             {
                                 width: $
@@ -8561,21 +8614,21 @@
                         }, t.$$.update = () => {
                             4 & t.$$.dirty && n(11, r = _ ? 24 : 0), 6144 & t.$$.dirty && n(7, i = w - r), 49152 & t.$$.dirty && n(9, o = {
                                 top: k,
                                 right: M,
                                 bottom: 35,
                                 left: 50
                             }), 4194305 & t.$$.dirty && n(10, l = m[y.x_feature]), 4194305 & t.$$.dirty && n(8, a = m[y.y_feature]), 641 & t.$$.dirty && n(20, s = rn().domain([y.pdp_min, y.pdp_max]).range([i - o.bottom, o.top])), 2097792 & t.$$.dirty && n(19, c = rn().domain(g).range([i - o.bottom, o.top])), 1581056 & t.$$.dirty && n(5, u = x ? s : c), 1539 & t.$$.dirty && n(6, d = "quantitative" === l.kind ? rn().domain([y.x_values[0], y.x_values[y.x_values.length - 1]]).range([o.left, $ - o.right]) : Hr().domain(y.x_values).range([o.left, $ - o.right]).padding(.5)), 256 & t.$$.dirty && n(4, f = function(t) {
-                                if ("quantitative" === t.kind) return ln().domain([t.values[0], t.values[t.values.length - 1]]).interpolator((t => Ic(1 - t)));
+                                if ("quantitative" === t.kind) return ln().domain([t.values[0], t.values[t.values.length - 1]]).interpolator((t => Hc(1 - t)));
                                 if ("categorical" !== t.kind || "nominal" !== t.subkind && "one_hot" !== t.subkind) {
                                     const e = t.values.length;
-                                    return Ir().domain(t.values).range(jc(Ic, e).reverse())
+                                    return Ir().domain(t.values).range(Rc(Hc, e).reverse())
                                 } {
                                     const e = t.values.length;
-                                    return Ir().domain(t.values).range(e <= 10 ? Vc : jc(Ic, e).reverse())
+                                    return Ir().domain(t.values).range(e <= 10 ? Fc : Rc(Hc, e).reverse())
                                 }
                             }(a)), 65632 & t.$$.dirty && n(17, h = ni().x((t => {
                                 var e;
                                 return null !== (e = d(t.x)) && void 0 !== e ? e : 0
                             })).y((t => u(t.prediction))).context(b)), 1 & t.$$.dirty && n(18, p = function(t) {
                                 var e;
                                 const n = new Map;
@@ -8596,31 +8649,31 @@
                             }(y)), 65674 & t.$$.dirty && b && (Bn(v, b, $, i), b && null != d && null != u && null != h && L(p, b, h, f)), 458864 & t.$$.dirty && b && null != d && null != u && null != h && L(p, b, h, f)
                         }, [y, $, _, v, f, u, d, i, a, o, l, r, w, x, k, M, b, h, p, c, s, g, m, function(t) {
                             K[t ? "unshift" : "push"]((() => {
                                 v = t, n(3, v)
                             }))
                         }]
                     }
-                    const nu = class extends xt {
+                    const ou = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, eu, tu, D, {
+                            super(), $t(this, t, iu, ru, D, {
                                 pd: 0,
                                 width: 1,
                                 height: 12,
                                 scaleLocally: 13,
                                 showColorLegend: 2,
                                 marginTop: 14,
                                 marginRight: 15
-                            }, Gc)
+                            }, Qc)
                         }
                     };
 
-                    function ru(t) {
+                    function lu(t) {
                         let e, n;
-                        return e = new nu({
+                        return e = new ou({
                             props: {
                                 pd: t[0],
                                 width: t[1],
                                 height: t[2],
                                 scaleLocally: t[3],
                                 showColorLegend: t[7],
                                 marginTop: t[9],
@@ -8645,17 +8698,17 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function iu(t) {
+                    function au(t) {
                         let e, n;
-                        return e = new Bc({
+                        return e = new Ic({
                             props: {
                                 pd: t[0],
                                 width: t[1],
                                 height: t[2],
                                 scaleLocally: t[3],
                                 showMarginalDistribution: t[4],
                                 showMarginalPdp: t[5],
@@ -8685,17 +8738,17 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function ou(t) {
+                    function su(t) {
                         let e, n, r, i;
-                        const o = [iu, ru],
+                        const o = [au, lu],
                             l = [];
 
                         function a(t, e) {
                             return "heatmap" === t[12] ? 0 : 1
                         }
                         return e = a(t), n = l[e] = o[e](t), {
                             c() {
@@ -8718,15 +8771,15 @@
                             },
                             d(t) {
                                 t && d(r), l[e].d(t)
                             }
                         }
                     }
 
-                    function lu(t, e, n) {
+                    function cu(t, e, n) {
                         let {
                             pd: r
                         } = e, {
                             width: i
                         } = e, {
                             height: o
                         } = e, {
@@ -8750,17 +8803,17 @@
                         } = e, {
                             twoWayKind: g = "heatmap"
                         } = e;
                         return t.$$set = t => {
                             "pd" in t && n(0, r = t.pd), "width" in t && n(1, i = t.width), "height" in t && n(2, o = t.height), "scaleLocally" in t && n(3, l = t.scaleLocally), "showMarginalDistribution" in t && n(4, a = t.showMarginalDistribution), "showMarginalPdp" in t && n(5, s = t.showMarginalPdp), "colorShows" in t && n(6, c = t.colorShows), "showColorLegend" in t && n(7, u = t.showColorLegend), "colorLegendTitle" in t && n(8, d = t.colorLegendTitle), "marginTop" in t && n(9, f = t.marginTop), "marginRight" in t && n(10, h = t.marginRight), "marginalPlotHeight" in t && n(11, p = t.marginalPlotHeight), "twoWayKind" in t && n(12, g = t.twoWayKind)
                         }, [r, i, o, l, a, s, c, u, d, f, h, p, g]
                     }
-                    const au = class extends xt {
+                    const uu = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, lu, ou, D, {
+                            super(), $t(this, t, cu, su, D, {
                                 pd: 0,
                                 width: 1,
                                 height: 2,
                                 scaleLocally: 3,
                                 showMarginalDistribution: 4,
                                 showMarginalPdp: 5,
                                 colorShows: 6,
@@ -8770,17 +8823,17 @@
                                 marginRight: 10,
                                 marginalPlotHeight: 11,
                                 twoWayKind: 12
                             })
                         }
                     };
 
-                    function su(t) {
+                    function du(t) {
                         let e, n, r, i;
-                        const o = [uu, cu],
+                        const o = [hu, fu],
                             l = [];
 
                         function a(t, e) {
                             return 1 === t[0].num_features ? 0 : 2 === t[0].num_features ? 1 : -1
                         }
                         return ~(e = a(t)) && (n = l[e] = o[e](t)), {
                             c() {
@@ -8803,17 +8856,17 @@
                             },
                             d(t) {
                                 t && d(r), ~e && l[e].d(t)
                             }
                         }
                     }
 
-                    function cu(t) {
+                    function fu(t) {
                         let e, n;
-                        return e = new au({
+                        return e = new uu({
                             props: {
                                 width: t[1],
                                 height: t[2],
                                 pd: t[0],
                                 scaleLocally: t[3],
                                 colorShows: t[4],
                                 showColorLegend: t[5],
@@ -8844,15 +8897,15 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function uu(t) {
+                    function hu(t) {
                         let e, n;
                         return e = new ac({
                             props: {
                                 width: t[1],
                                 height: t[2],
                                 pd: t[0],
                                 scaleLocally: t[3],
@@ -8884,25 +8937,25 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function du(t) {
-                        let e, n, r = t[1] > 0 && t[2] > 0 && su(t);
+                    function pu(t) {
+                        let e, n, r = t[1] > 0 && t[2] > 0 && du(t);
                         return {
                             c() {
                                 r && r.c(), e = v()
                             },
                             m(t, i) {
                                 r && r.m(t, i), u(t, e, i), n = !0
                             },
                             p(t, [n]) {
-                                t[1] > 0 && t[2] > 0 ? r ? (r.p(t, n), 6 & n && ut(r, 1)) : (r = su(t), r.c(), ut(r, 1), r.m(e.parentNode, e)) : r && (st(), dt(r, 1, 1, (() => {
+                                t[1] > 0 && t[2] > 0 ? r ? (r.p(t, n), 6 & n && ut(r, 1)) : (r = du(t), r.c(), ut(r, 1), r.m(e.parentNode, e)) : r && (st(), dt(r, 1, 1, (() => {
                                     r = null
                                 })), ct())
                             },
                             i(t) {
                                 n || (ut(r), n = !0)
                             },
                             o(t) {
@@ -8910,15 +8963,15 @@
                             },
                             d(t) {
                                 t && d(e), r && r.d(t)
                             }
                         }
                     }
 
-                    function fu(t, e, n) {
+                    function gu(t, e, n) {
                         let {
                             pd: r
                         } = e, {
                             width: i
                         } = e, {
                             height: o
                         } = e, {
@@ -8952,17 +9005,17 @@
                         } = e, {
                             twoWayKind: $ = "heatmap"
                         } = e;
                         return t.$$set = t => {
                             "pd" in t && n(0, r = t.pd), "width" in t && n(1, i = t.width), "height" in t && n(2, o = t.height), "scaleLocally" in t && n(3, l = t.scaleLocally), "colorShows" in t && n(4, a = t.colorShows), "showColorLegend" in t && n(5, s = t.showColorLegend), "colorLegendTitle" in t && n(6, c = t.colorLegendTitle), "iceLevel" in t && n(7, u = t.iceLevel), "indices" in t && n(8, d = t.indices), "showMarginalDistribution" in t && n(9, f = t.showMarginalDistribution), "showMarginalPdp" in t && n(10, h = t.showMarginalPdp), "marginTop" in t && n(11, p = t.marginTop), "marginRight" in t && n(12, g = t.marginRight), "marginalPlotHeight" in t && n(13, m = t.marginalPlotHeight), "allowBrushing" in t && n(14, v = t.allowBrushing), "showBrushedBorder" in t && n(15, b = t.showBrushedBorder), "iceLineWidth" in t && n(16, y = t.iceLineWidth), "twoWayKind" in t && n(17, $ = t.twoWayKind)
                         }, [r, i, o, l, a, s, c, u, d, f, h, p, g, m, v, b, y, $]
                     }
-                    const hu = class extends xt {
+                    const mu = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, fu, du, D, {
+                            super(), $t(this, t, gu, pu, D, {
                                 pd: 0,
                                 width: 1,
                                 height: 2,
                                 scaleLocally: 3,
                                 colorShows: 4,
                                 showColorLegend: 5,
                                 colorLegendTitle: 6,
@@ -8977,69 +9030,69 @@
                                 showBrushedBorder: 15,
                                 iceLineWidth: 16,
                                 twoWayKind: 17
                             })
                         }
                     };
 
-                    function pu(t, e) {
+                    function vu(t, e) {
                         if ((i = t.length) > 1)
                             for (var n, r, i, o = 1, l = t[e[0]], a = l.length; o < i; ++o)
                                 for (r = l, l = t[e[o]], n = 0; n < a; ++n) l[n][1] += l[n][0] = isNaN(r[n][1]) ? r[n][0] : r[n][1]
                     }
 
-                    function gu(t) {
+                    function bu(t) {
                         for (var e = t.length, n = new Array(e); --e >= 0;) n[e] = e;
                         return n
                     }
 
-                    function mu(t, e) {
+                    function yu(t, e) {
                         return t[e]
                     }
 
-                    function vu(t) {
+                    function $u(t) {
                         const e = [];
                         return e.key = t, e
                     }
 
-                    function bu(t, e) {
+                    function wu(t, e) {
                         if ((r = t.length) > 0) {
                             for (var n, r, i, o = 0, l = t[0].length; o < l; ++o) {
                                 for (i = n = 0; n < r; ++n) i += t[n][o][1] || 0;
                                 if (i)
                                     for (n = 0; n < r; ++n) t[n][o][1] /= i
                             }
-                            pu(t, e)
+                            vu(t, e)
                         }
                     }
 
-                    function yu(t) {
-                        return gu(t).reverse()
+                    function xu(t) {
+                        return bu(t).reverse()
                     }
 
-                    function $u(t) {
+                    function _u(t) {
                         c(t, "svelte-1gasvv0", ".distributions-container.svelte-1gasvv0{width:100%;height:100%;display:flex;flex-direction:column;gap:0.5em}.distributions-settings.svelte-1gasvv0{display:flex;align-items:center;gap:1em}.distribution-plots.svelte-1gasvv0{flex:1;overflow-y:auto;position:relative}.label-and-input.svelte-1gasvv0{display:flex;align-items:center;gap:0.25em}svg.svelte-1gasvv0,canvas.svelte-1gasvv0{position:absolute;left:0}")
                     }
 
-                    function wu(t, e, n) {
+                    function ku(t, e, n) {
                         const r = t.slice();
                         return r[39] = e[n], r
                     }
 
-                    function xu(t, e, n) {
+                    function Mu(t, e, n) {
                         const r = t.slice();
                         return r[42] = e[n], r[44] = n, r
                     }
 
-                    function _u(t, e, n) {
+                    function Lu(t, e, n) {
                         const r = t.slice();
                         return r[45] = e[n], r
                     }
 
-                    function ku(t) {
+                    function Au(t) {
                         let e, n, r, i, o;
                         return {
                             c() {
                                 e = h("label"), n = h("input"), r = g("Normalize bar charts"), y(n, "type", "checkbox"), y(e, "class", "label-and-input svelte-1gasvv0")
                             },
                             m(l, a) {
                                 u(l, e, a), s(e, n), n.checked = t[2], s(e, r), i || (o = b(n, "change", t[27]), i = !0)
@@ -9049,18 +9102,18 @@
                             },
                             d(t) {
                                 t && d(e), i = !1, o()
                             }
                         }
                     }
 
-                    function Mu(t) {
+                    function Pu(t) {
                         let e, n, r, i = ft(t[39].data),
                             o = [];
-                        for (let e = 0; e < i.length; e += 1) o[e] = Pu(xu(t, i, e));
+                        for (let e = 0; e < i.length; e += 1) o[e] = Tu(Mu(t, i, e));
                         return n = new Va({
                             props: {
                                 scale: t[12],
                                 x: t[14].left,
                                 label: t[2] ? "percent" : "count",
                                 format: t[2] ? Ze("~%") : jn
                             }
@@ -9075,16 +9128,16 @@
                                 for (let t = 0; t < o.length; t += 1) o[t] && o[t].m(e, null);
                                 bt(n, t, i), r = !0
                             },
                             p(t, r) {
                                 if (4744 & r[0]) {
                                     let n;
                                     for (i = ft(t[39].data), n = 0; n < i.length; n += 1) {
-                                        const l = xu(t, i, n);
-                                        o[n] ? o[n].p(l, r) : (o[n] = Pu(l), o[n].c(), o[n].m(e, null))
+                                        const l = Mu(t, i, n);
+                                        o[n] ? o[n].p(l, r) : (o[n] = Tu(l), o[n].c(), o[n].m(e, null))
                                     }
                                     for (; n < o.length; n += 1) o[n].d(1);
                                     o.length = i.length
                                 }
                                 const l = {};
                                 4096 & r[0] && (l.scale = t[12]), 4 & r[0] && (l.label = t[2] ? "percent" : "count"), 4 & r[0] && (l.format = t[2] ? Ze("~%") : jn), n.$set(l)
                             },
@@ -9096,128 +9149,128 @@
                             },
                             d(t) {
                                 t && d(e), f(o, t), yt(n, t)
                             }
                         }
                     }
 
-                    function Lu(t) {
+                    function Su(t) {
                         let e, n, r, i, o;
                         return {
                             c() {
-                                e = p("rect"), y(e, "x", n = Ou(t[45].data[0], t[9][t[39].feature]) + 1), y(e, "width", r = Cu(t[9][t[39].feature]) - 2), y(e, "y", i = t[12](t[45][1])), y(e, "height", o = t[12](t[45][0]) - t[12](t[45][1]))
+                                e = p("rect"), y(e, "x", n = ju(t[45].data[0], t[9][t[39].feature]) + 1), y(e, "width", r = Bu(t[9][t[39].feature]) - 2), y(e, "y", i = t[12](t[45][1])), y(e, "height", o = t[12](t[45][0]) - t[12](t[45][1]))
                             },
                             m(t, n) {
                                 u(t, e, n)
                             },
                             p(t, l) {
-                                520 & l[0] && n !== (n = Ou(t[45].data[0], t[9][t[39].feature]) + 1) && y(e, "x", n), 520 & l[0] && r !== (r = Cu(t[9][t[39].feature]) - 2) && y(e, "width", r), 4104 & l[0] && i !== (i = t[12](t[45][1])) && y(e, "y", i), 4104 & l[0] && o !== (o = t[12](t[45][0]) - t[12](t[45][1])) && y(e, "height", o)
+                                520 & l[0] && n !== (n = ju(t[45].data[0], t[9][t[39].feature]) + 1) && y(e, "x", n), 520 & l[0] && r !== (r = Bu(t[9][t[39].feature]) - 2) && y(e, "width", r), 4104 & l[0] && i !== (i = t[12](t[45][1])) && y(e, "y", i), 4104 & l[0] && o !== (o = t[12](t[45][0]) - t[12](t[45][1])) && y(e, "height", o)
                             },
                             d(t) {
                                 t && d(e)
                             }
                         }
                     }
 
-                    function Au(t) {
-                        let e, n = t[45][0] !== t[45][1] && Lu(t);
+                    function zu(t) {
+                        let e, n = t[45][0] !== t[45][1] && Su(t);
                         return {
                             c() {
                                 n && n.c(), e = v()
                             },
                             m(t, r) {
                                 n && n.m(t, r), u(t, e, r)
                             },
                             p(t, r) {
-                                t[45][0] !== t[45][1] ? n ? n.p(t, r) : (n = Lu(t), n.c(), n.m(e.parentNode, e)) : n && (n.d(1), n = null)
+                                t[45][0] !== t[45][1] ? n ? n.p(t, r) : (n = Su(t), n.c(), n.m(e.parentNode, e)) : n && (n.d(1), n = null)
                             },
                             d(t) {
                                 t && d(e), n && n.d(t)
                             }
                         }
                     }
 
-                    function Pu(t) {
+                    function Tu(t) {
                         let e, n, r = ft(t[42]),
                             i = [];
-                        for (let e = 0; e < r.length; e += 1) i[e] = Au(_u(t, r, e));
+                        for (let e = 0; e < r.length; e += 1) i[e] = zu(Lu(t, r, e));
                         return {
                             c() {
                                 e = p("g");
                                 for (let t = 0; t < i.length; t += 1) i[t].c();
                                 y(e, "fill", n = t[7](t[44]))
                             },
                             m(t, n) {
                                 u(t, e, n);
                                 for (let t = 0; t < i.length; t += 1) i[t] && i[t].m(e, null)
                             },
                             p(t, o) {
                                 if (4616 & o[0]) {
                                     let n;
                                     for (r = ft(t[42]), n = 0; n < r.length; n += 1) {
-                                        const l = _u(t, r, n);
-                                        i[n] ? i[n].p(l, o) : (i[n] = Au(l), i[n].c(), i[n].m(e, null))
+                                        const l = Lu(t, r, n);
+                                        i[n] ? i[n].p(l, o) : (i[n] = zu(l), i[n].c(), i[n].m(e, null))
                                     }
                                     for (; n < i.length; n += 1) i[n].d(1);
                                     i.length = r.length
                                 }
                                 128 & o[0] && n !== (n = t[7](t[44])) && y(e, "fill", n)
                             },
                             d(t) {
                                 t && d(e), f(i, t)
                             }
                         }
                     }
 
-                    function Su(t) {
-                        let e, n, r, i, o, l, a = "categorical" === t[39].kind && Mu(t);
+                    function Nu(t) {
+                        let e, n, r, i, o, l, a = "categorical" === t[39].kind && Pu(t);
                         return r = new Ma({
                             props: {
                                 scale: t[9][t[39].feature],
                                 y: t[8].bandwidth() - t[14].bottom,
                                 showBaseline: !0,
                                 baselineColor: "var(--gray-6)",
                                 tickColor: "var(--gray-6)",
                                 integerOnly: "discrete" === t[11][t[39].feature].subkind,
-                                value_map: Nu(t[11][t[39].feature]),
+                                value_map: Du(t[11][t[39].feature]),
                                 label: t[39].feature
                             }
                         }), {
                             c() {
                                 e = p("g"), a && a.c(), n = p("g"), vt(r.$$.fragment), y(n, "class", "x-axis"), y(n, "id", i = "axis-" + t[39].feature), y(e, "transform", o = "translate(0," + t[8](t[39].feature) + ")")
                             },
                             m(t, i) {
                                 u(t, e, i), a && a.m(e, null), s(e, n), bt(r, n, null), l = !0
                             },
                             p(t, s) {
-                                "categorical" === t[39].kind ? a ? (a.p(t, s), 8 & s[0] && ut(a, 1)) : (a = Mu(t), a.c(), ut(a, 1), a.m(e, n)) : a && (st(), dt(a, 1, 1, (() => {
+                                "categorical" === t[39].kind ? a ? (a.p(t, s), 8 & s[0] && ut(a, 1)) : (a = Pu(t), a.c(), ut(a, 1), a.m(e, n)) : a && (st(), dt(a, 1, 1, (() => {
                                     a = null
                                 })), ct());
                                 const c = {};
-                                520 & s[0] && (c.scale = t[9][t[39].feature]), 256 & s[0] && (c.y = t[8].bandwidth() - t[14].bottom), 2056 & s[0] && (c.integerOnly = "discrete" === t[11][t[39].feature].subkind), 2056 & s[0] && (c.value_map = Nu(t[11][t[39].feature])), 8 & s[0] && (c.label = t[39].feature), r.$set(c), (!l || 8 & s[0] && i !== (i = "axis-" + t[39].feature)) && y(n, "id", i), (!l || 264 & s[0] && o !== (o = "translate(0," + t[8](t[39].feature) + ")")) && y(e, "transform", o)
+                                520 & s[0] && (c.scale = t[9][t[39].feature]), 256 & s[0] && (c.y = t[8].bandwidth() - t[14].bottom), 2056 & s[0] && (c.integerOnly = "discrete" === t[11][t[39].feature].subkind), 2056 & s[0] && (c.value_map = Du(t[11][t[39].feature])), 8 & s[0] && (c.label = t[39].feature), r.$set(c), (!l || 8 & s[0] && i !== (i = "axis-" + t[39].feature)) && y(n, "id", i), (!l || 264 & s[0] && o !== (o = "translate(0," + t[8](t[39].feature) + ")")) && y(e, "transform", o)
                             },
                             i(t) {
                                 l || (ut(a), ut(r.$$.fragment, t), l = !0)
                             },
                             o(t) {
                                 dt(a), dt(r.$$.fragment, t), l = !1
                             },
                             d(t) {
                                 t && d(e), a && a.d(), yt(r)
                             }
                         }
                     }
 
-                    function zu(t) {
+                    function Cu(t) {
                         let e, n, r, i, o, l, a, c, v, b, $, w, _, k, M, L, P = t[10].length + "",
                             S = 1 === t[10].length ? "instance" : "instances",
-                            z = t[13].length > 0 && ku(t),
+                            z = t[13].length > 0 && Au(t),
                             T = ft(t[3]),
                             N = [];
-                        for (let e = 0; e < T.length; e += 1) N[e] = Su(wu(t, T, e));
+                        for (let e = 0; e < T.length; e += 1) N[e] = Nu(ku(t, T, e));
                         const C = t => dt(N[t], 1, 1, (() => {
                             N[t] = null
                         }));
                         return {
                             c() {
                                 e = h("div"), n = h("div"), z && z.c(), r = m(), i = h("div"), o = g(P), l = m(), a = g(S), c = g(" selected"), v = m(), b = h("div"), $ = h("canvas"), w = m(), _ = p("svg"), k = p("g");
                                 for (let t = 0; t < N.length; t += 1) N[t].c();
@@ -9225,19 +9278,19 @@
                             },
                             m(d, f) {
                                 u(d, e, f), s(e, n), z && z.m(n, null), s(n, r), s(n, i), s(i, o), s(i, l), s(i, a), s(i, c), s(e, v), s(e, b), s(b, $), t[28]($), s(b, w), s(b, _), s(_, k);
                                 for (let t = 0; t < N.length; t += 1) N[t] && N[t].m(k, null);
                                 t[29](k), M = A.observe(b, t[30].bind(b)), L = !0
                             },
                             p(t, e) {
-                                if (t[13].length > 0 ? z ? z.p(t, e) : (z = ku(t), z.c(), z.m(n, r)) : z && (z.d(1), z = null), (!L || 1024 & e[0]) && P !== (P = t[10].length + "") && x(o, P), (!L || 1024 & e[0]) && S !== (S = 1 === t[10].length ? "instance" : "instances") && x(a, S), 23436 & e[0]) {
+                                if (t[13].length > 0 ? z ? z.p(t, e) : (z = Au(t), z.c(), z.m(n, r)) : z && (z.d(1), z = null), (!L || 1024 & e[0]) && P !== (P = t[10].length + "") && x(o, P), (!L || 1024 & e[0]) && S !== (S = 1 === t[10].length ? "instance" : "instances") && x(a, S), 23436 & e[0]) {
                                     let n;
                                     for (T = ft(t[3]), n = 0; n < T.length; n += 1) {
-                                        const r = wu(t, T, n);
-                                        N[n] ? (N[n].p(r, e), ut(N[n], 1)) : (N[n] = Su(r), N[n].c(), ut(N[n], 1), N[n].m(k, null))
+                                        const r = ku(t, T, n);
+                                        N[n] ? (N[n].p(r, e), ut(N[n], 1)) : (N[n] = Nu(r), N[n].c(), ut(N[n], 1), N[n].m(k, null))
                                     }
                                     for (st(), n = T.length; n < N.length; n += 1) C(n);
                                     ct()
                                 }(!L || 1 & e[0]) && y(_, "width", t[0]), (!L || 64 & e[0]) && y(_, "height", t[6])
                             },
                             i(t) {
                                 if (!L) {
@@ -9252,32 +9305,32 @@
                             },
                             d(n) {
                                 n && d(e), z && z.d(), t[28](null), f(N, n), t[29](null), M()
                             }
                         }
                     }
 
-                    function Tu(t) {
+                    function Ou(t) {
                         return "categorical" === t.kind
                     }
 
-                    function Nu(t) {
+                    function Du(t) {
                         return "value_map" in t ? t.value_map : {}
                     }
 
-                    function Cu(t) {
+                    function Bu(t) {
                         return t && "bandwidth" in t ? t.bandwidth() : 0
                     }
 
-                    function Ou(t, e) {
+                    function ju(t, e) {
                         var n;
                         return e && null !== (n = e(t)) && void 0 !== n ? n : 0
                     }
 
-                    function Du(t, e, n) {
+                    function Eu(t, e, n) {
                         let r, i, o, a, s, c, u, d, f, h, p, g, m, v, b, y, $;
                         j(t, Jn, (t => n(25, b = t))), j(t, Gn, (t => n(11, y = t))), j(t, Qn, (t => n(26, $ = t)));
                         let {
                             pd: w
                         } = e, {
                             features: x
                         } = e;
@@ -9361,40 +9414,40 @@
                         return q((() => {
                             O && n(18, D = O.getContext("2d"))
                         })), t.$$set = t => {
                             "pd" in t && n(15, w = t.pd), "features" in t && n(16, x = t.features)
                         }, t.$$.update = () => {
                             2 & t.$$.dirty[0] && n(0, M = k ? k.width : 0), 2 & t.$$.dirty[0] && n(17, L = k ? k.height : 0), 229376 & t.$$.dirty[0] && n(6, r = Math.max(L, x.length * (30 * w.ice.num_clusters + _.top + _.bottom))), 32768 & t.$$.dirty[0] && n(23, i = Sn(w).cluster_labels), 32768 & t.$$.dirty[0] && n(21, o = xn(w.ice.num_clusters)), 67584 & t.$$.dirty[0] && n(13, a = x.filter((t => "categorical" === y[t].kind))), 2097152 & t.$$.dirty[0] && n(7, s = Ir().domain(o).range(Kn)), 65600 & t.$$.dirty[0] && n(8, c = Rr().domain(x).range([0, r])), 67108864 & t.$$.dirty[0] && (u = xn($)), 67108864 & t.$$.dirty[0] && n(10, d = xn($)), 2097156 & t.$$.dirty[0] && n(24, f = function() {
                                 var t = Jr([]),
-                                    e = gu,
-                                    n = pu,
-                                    r = mu;
+                                    e = bu,
+                                    n = vu,
+                                    r = yu;
 
                                 function i(i) {
-                                    var o, l, a = Array.from(t.apply(this, arguments), vu),
+                                    var o, l, a = Array.from(t.apply(this, arguments), $u),
                                         s = a.length,
                                         c = -1;
                                     for (const t of i)
                                         for (o = 0, ++c; o < s; ++o)(a[o][c] = [0, +r(t, a[o].key, c, i)]).data = t;
                                     for (o = 0, l = Gr(e(a)); o < s; ++o) a[l[o]].index = o;
                                     return n(a, l), a
                                 }
                                 return i.keys = function(e) {
                                     return arguments.length ? (t = "function" == typeof e ? e : Jr(Array.from(e)), i) : t
                                 }, i.value = function(t) {
                                     return arguments.length ? (r = "function" == typeof t ? t : Jr(+t), i) : r
                                 }, i.order = function(t) {
-                                    return arguments.length ? (e = null == t ? gu : "function" == typeof t ? t : Jr(Array.from(t)), i) : e
+                                    return arguments.length ? (e = null == t ? bu : "function" == typeof t ? t : Jr(Array.from(t)), i) : e
                                 }, i.offset = function(t) {
-                                    return arguments.length ? (n = null == t ? pu : t, i) : n
+                                    return arguments.length ? (n = null == t ? vu : t, i) : n
                                 }, i
                             }().keys(o).value(((t, e) => {
                                 var n;
                                 return null !== (n = t[1].get(e)) && void 0 !== n ? n : 0
-                            })).offset(A ? bu : pu).order(yu)), 67585 & t.$$.dirty[0] && n(9, h = Object.fromEntries(x.map((t => {
+                            })).offset(A ? wu : vu).order(xu)), 67585 & t.$$.dirty[0] && n(9, h = Object.fromEntries(x.map((t => {
                                 const e = y[t];
                                 return [t, "quantitative" === e.kind ? rn().domain([e.values[0], e.values[e.values.length - 1]]).range([_.left, M - _.right]) : Rr().domain(e.values).range([_.left, M - _.right])]
                             })))), 58788864 & t.$$.dirty[0] && n(3, P = x.map((t => {
                                 if ("categorical" === y[t].kind) {
                                     const e = $n(d, (t => t.length), (e => b[t][e]), (t => i[t]));
                                     return {
                                         feature: t,
@@ -9408,15 +9461,15 @@
                                         kind: "quantitative",
                                         data: Array.from(e, (([t, e]) => ({
                                             cluster: t,
                                             raincloud: e
                                         })))
                                     }
                                 }
-                            }))), 8 & t.$$.dirty[0] && n(22, p = Math.max(...P.filter(Tu).map((t => t.data)).flat(3))), 4194564 & t.$$.dirty[0] && n(12, g = rn().domain([0, A ? 1 : p]).range([c.bandwidth() - _.bottom, _.top])), 2097408 & t.$$.dirty[0] && n(19, m = Rr().domain(o).range([_.top, c.bandwidth() - _.bottom]).paddingInner(.2).paddingOuter(.1)), 257 & t.$$.dirty[0] && n(20, v = la(Kl).extent([
+                            }))), 8 & t.$$.dirty[0] && n(22, p = Math.max(...P.filter(Ou).map((t => t.data)).flat(3))), 4194564 & t.$$.dirty[0] && n(12, g = rn().domain([0, A ? 1 : p]).range([c.bandwidth() - _.bottom, _.top])), 2097408 & t.$$.dirty[0] && n(19, m = Rr().domain(o).range([_.top, c.bandwidth() - _.bottom]).paddingInner(.2).paddingOuter(.1)), 257 & t.$$.dirty[0] && n(20, v = la(Kl).extent([
                                 [_.left, -4 + c.bandwidth() - _.bottom],
                                 [M - _.right, 4 + c.bandwidth() - _.bottom]
                             ]).on("start brush end", T)), 1114129 & t.$$.dirty[0] && N && x && M > 0 && async function(t) {
                                 N && (await Z(), C = xo(N).selectAll(".x-axis"), C.call(t), C.call(t.clear))
                             }(v), 262241 & t.$$.dirty[0] && O && D && (Bn(O, D, M, r), B(D, h, c, m, s, P, M, r)), 787401 & t.$$.dirty[0] && B(D, h, c, m, s, P, M, r)
                         }, [M, k, A, P, N, O, r, s, c, h, d, y, g, a, _, w, x, L, D, m, v, o, p, i, f, b, $, function() {
                             A = this.checked, n(2, A)
@@ -9428,31 +9481,31 @@
                             K[t ? "unshift" : "push"]((() => {
                                 N = t, n(4, N)
                             }))
                         }, function() {
                             k = l.entries.get(this)?.contentRect, n(1, k)
                         }]
                     }
-                    const Bu = class extends xt {
+                    const Iu = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, Du, zu, D, {
+                            super(), $t(this, t, Eu, Cu, D, {
                                 pd: 15,
                                 features: 16
-                            }, $u, [-1, -1])
+                            }, _u, [-1, -1])
                         }
                     };
 
-                    function ju(t) {
+                    function Ru(t) {
                         c(t, "svelte-2s8sz0", ".pdpilot-plot-container.svelte-2s8sz0{width:100%;height:100%;position:relative}svg.svelte-2s8sz0,canvas.svelte-2s8sz0{position:absolute;top:var(--top);left:0}")
                     }
 
-                    function Eu(t) {
+                    function Vu(t) {
                         let e, n, r, i, o = t[21].left - t[28] + "px",
                             l = `${t[22]}px`;
-                        const a = [Ru, Iu],
+                        const a = [qu, Hu],
                             s = [];
 
                         function c(t, e) {
                             return "interpolator" in t[18] ? 0 : 1
                         }
                         return n = c(t), r = s[n] = a[n](t), {
                             c() {
@@ -9475,23 +9528,23 @@
                             },
                             d(t) {
                                 t && d(e), s[n].d()
                             }
                         }
                     }
 
-                    function Iu(t) {
+                    function Hu(t) {
                         let e, n;
-                        return e = new Yc({
+                        return e = new Zc({
                             props: {
                                 width: t[23] + t[27],
-                                height: Zu,
+                                height: ed,
                                 color: t[18],
-                                marginLeft: Qu,
-                                marginRight: Qu,
+                                marginLeft: nd,
+                                marginRight: nd,
                                 title: t[3]
                             }
                         }), {
                             c() {
                                 vt(e.$$.fragment)
                             },
                             m(t, r) {
@@ -9509,23 +9562,23 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function Ru(t) {
+                    function qu(t) {
                         let e, n;
                         return e = new wc({
                             props: {
                                 width: t[23] + t[27],
-                                height: Zu,
+                                height: ed,
                                 color: t[18],
-                                marginLeft: Qu,
-                                marginRight: Qu,
+                                marginLeft: nd,
+                                marginRight: nd,
                                 title: t[3]
                             }
                         }), {
                             c() {
                                 vt(e.$$.fragment)
                             },
                             m(t, r) {
@@ -9543,31 +9596,31 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function Vu(t) {
-                        let e, n, r, i, o = t[16] && t[24].length > 0 && Hu(t),
-                            l = t[8] && Wu(t),
-                            a = t[9] && Uu(t);
+                    function Fu(t) {
+                        let e, n, r, i, o = t[16] && t[24].length > 0 && Wu(t),
+                            l = t[8] && Uu(t),
+                            a = t[9] && Ju(t);
                         return {
                             c() {
                                 o && o.c(), e = v(), l && l.c(), n = v(), a && a.c(), r = v()
                             },
                             m(t, s) {
                                 o && o.m(t, s), u(t, e, s), l && l.m(t, s), u(t, n, s), a && a.m(t, s), u(t, r, s), i = !0
                             },
                             p(t, i) {
-                                t[16] && t[24].length > 0 ? o ? (o.p(t, i), 16842752 & i[0] && ut(o, 1)) : (o = Hu(t), o.c(), ut(o, 1), o.m(e.parentNode, e)) : o && (st(), dt(o, 1, 1, (() => {
+                                t[16] && t[24].length > 0 ? o ? (o.p(t, i), 16842752 & i[0] && ut(o, 1)) : (o = Wu(t), o.c(), ut(o, 1), o.m(e.parentNode, e)) : o && (st(), dt(o, 1, 1, (() => {
                                     o = null
-                                })), ct()), t[8] ? l ? (l.p(t, i), 256 & i[0] && ut(l, 1)) : (l = Wu(t), l.c(), ut(l, 1), l.m(n.parentNode, n)) : l && (st(), dt(l, 1, 1, (() => {
+                                })), ct()), t[8] ? l ? (l.p(t, i), 256 & i[0] && ut(l, 1)) : (l = Uu(t), l.c(), ut(l, 1), l.m(n.parentNode, n)) : l && (st(), dt(l, 1, 1, (() => {
                                     l = null
-                                })), ct()), t[9] ? a ? (a.p(t, i), 512 & i[0] && ut(a, 1)) : (a = Uu(t), a.c(), ut(a, 1), a.m(r.parentNode, r)) : a && (st(), dt(a, 1, 1, (() => {
+                                })), ct()), t[9] ? a ? (a.p(t, i), 512 & i[0] && ut(a, 1)) : (a = Ju(t), a.c(), ut(a, 1), a.m(r.parentNode, r)) : a && (st(), dt(a, 1, 1, (() => {
                                     a = null
                                 })), ct())
                             },
                             i(t) {
                                 i || (ut(o), ut(l), ut(a), i = !0)
                             },
                             o(t) {
@@ -9575,17 +9628,17 @@
                             },
                             d(t) {
                                 t && (d(e), d(n), d(r)), o && o.d(t), l && l.d(t), a && a.d(t)
                             }
                         }
                     }
 
-                    function Hu(t) {
+                    function Wu(t) {
                         let e, n, r, i;
-                        const o = [Fu, qu],
+                        const o = [Xu, Ku],
                             l = [];
 
                         function a(t, e) {
                             return "bandwidth" in t[20] ? 0 : 1
                         }
                         return e = a(t), n = l[e] = o[e](t), {
                             c() {
@@ -9608,15 +9661,15 @@
                             },
                             d(t) {
                                 t && d(r), l[e].d(t)
                             }
                         }
                     }
 
-                    function qu(t) {
+                    function Ku(t) {
                         let e, n;
                         return e = new Qa({
                             props: {
                                 data: t[16],
                                 fill: Fn,
                                 x: t[20],
                                 height: t[13],
@@ -9644,15 +9697,15 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function Fu(t) {
+                    function Xu(t) {
                         let e, n;
                         return e = new ds({
                             props: {
                                 data: t[16],
                                 fill: Fn,
                                 x: t[20],
                                 height: t[13],
@@ -9680,17 +9733,17 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function Wu(t) {
+                    function Uu(t) {
                         let e, n, r, i;
-                        const o = [Xu, Ku],
+                        const o = [Gu, Yu],
                             l = [];
 
                         function a(t, e) {
                             return "bandwidth" in t[20] ? 0 : 1
                         }
                         return e = a(t), n = l[e] = o[e](t), {
                             c() {
@@ -9713,15 +9766,15 @@
                             },
                             d(t) {
                                 t && d(r), l[e].d(t)
                             }
                         }
                     }
 
-                    function Ku(t) {
+                    function Yu(t) {
                         let e, n;
                         return e = new Qa({
                             props: {
                                 data: t[8],
                                 fill: t[26] ? "none" : "var(--gray-3)",
                                 stroke: t[26] ? "var(--black)" : "none",
                                 x: t[20],
@@ -9750,15 +9803,15 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function Xu(t) {
+                    function Gu(t) {
                         let e, n;
                         return e = new ds({
                             props: {
                                 data: t[8],
                                 fill: t[26] ? "none" : "var(--gray-3)",
                                 stroke: t[26] ? "var(--black)" : "none",
                                 x: t[20],
@@ -9787,17 +9840,17 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function Uu(t) {
+                    function Ju(t) {
                         let e, n, r, i;
-                        const o = [Gu, Yu],
+                        const o = [Qu, Zu],
                             l = [];
 
                         function a(t, e) {
                             return "bandwidth" in t[19] ? 0 : 1
                         }
                         return e = a(t), n = l[e] = o[e](t), {
                             c() {
@@ -9820,15 +9873,15 @@
                             },
                             d(t) {
                                 t && d(r), l[e].d(t)
                             }
                         }
                     }
 
-                    function Yu(t) {
+                    function Zu(t) {
                         let e, n;
                         return e = new Qa({
                             props: {
                                 data: t[9],
                                 x: t[19],
                                 height: t[13],
                                 direction: "vertical",
@@ -9853,15 +9906,15 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function Gu(t) {
+                    function Qu(t) {
                         let e, n;
                         return e = new ds({
                             props: {
                                 data: t[9],
                                 x: t[19],
                                 height: t[13],
                                 direction: "vertical",
@@ -9886,17 +9939,17 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function Ju(t) {
-                        let e, n, r, i, o, l, a, c, f, g = `${Zu+t[22]}px`,
-                            v = "" !== t[3] && Eu(t);
+                    function td(t) {
+                        let e, n, r, i, o, l, a, c, f, g = `${ed+t[22]}px`,
+                            v = "" !== t[3] && Vu(t);
                         l = new Ma({
                             props: {
                                 scale: t[20],
                                 y: t[17] - t[21].bottom,
                                 label: t[1],
                                 integerOnly: t[4],
                                 value_map: t[6]
@@ -9906,48 +9959,48 @@
                                 scale: t[19],
                                 x: t[21].left,
                                 label: t[2],
                                 integerOnly: t[5],
                                 value_map: t[7]
                             }
                         });
-                        let b = t[10] && Vu(t);
+                        let b = t[10] && Fu(t);
                         return {
                             c() {
                                 e = h("div"), v && v.c(), n = m(), r = h("canvas"), i = m(), o = p("svg"), vt(l.$$.fragment), vt(a.$$.fragment), c = p("g"), b && b.c(), y(r, "class", "svelte-2s8sz0"), y(o, "width", t[0]), y(o, "height", t[17]), y(o, "class", "svelte-2s8sz0"), y(e, "class", "pdpilot-plot-container svelte-2s8sz0"), k(e, "--top", g)
                             },
                             m(d, h) {
                                 u(d, e, h), v && v.m(e, null), s(e, n), s(e, r), t[53](r), s(e, i), s(e, o), bt(l, o, null), bt(a, o, null), s(o, c), t[54](c), b && b.m(o, null), f = !0
                             },
                             p(t, r) {
-                                "" !== t[3] ? v ? (v.p(t, r), 8 & r[0] && ut(v, 1)) : (v = Eu(t), v.c(), ut(v, 1), v.m(e, n)) : v && (st(), dt(v, 1, 1, (() => {
+                                "" !== t[3] ? v ? (v.p(t, r), 8 & r[0] && ut(v, 1)) : (v = Vu(t), v.c(), ut(v, 1), v.m(e, n)) : v && (st(), dt(v, 1, 1, (() => {
                                     v = null
                                 })), ct());
                                 const i = {};
                                 1048576 & r[0] && (i.scale = t[20]), 2228224 & r[0] && (i.y = t[17] - t[21].bottom), 2 & r[0] && (i.label = t[1]), 16 & r[0] && (i.integerOnly = t[4]), 64 & r[0] && (i.value_map = t[6]), l.$set(i);
                                 const s = {};
-                                524288 & r[0] && (s.scale = t[19]), 2097152 & r[0] && (s.x = t[21].left), 4 & r[0] && (s.label = t[2]), 32 & r[0] && (s.integerOnly = t[5]), 128 & r[0] && (s.value_map = t[7]), a.$set(s), t[10] ? b ? (b.p(t, r), 1024 & r[0] && ut(b, 1)) : (b = Vu(t), b.c(), ut(b, 1), b.m(o, null)) : b && (st(), dt(b, 1, 1, (() => {
+                                524288 & r[0] && (s.scale = t[19]), 2097152 & r[0] && (s.x = t[21].left), 4 & r[0] && (s.label = t[2]), 32 & r[0] && (s.integerOnly = t[5]), 128 & r[0] && (s.value_map = t[7]), a.$set(s), t[10] ? b ? (b.p(t, r), 1024 & r[0] && ut(b, 1)) : (b = Fu(t), b.c(), ut(b, 1), b.m(o, null)) : b && (st(), dt(b, 1, 1, (() => {
                                     b = null
-                                })), ct()), (!f || 1 & r[0]) && y(o, "width", t[0]), (!f || 131072 & r[0]) && y(o, "height", t[17]), 4194304 & r[0] && g !== (g = `${Zu+t[22]}px`) && k(e, "--top", g)
+                                })), ct()), (!f || 1 & r[0]) && y(o, "width", t[0]), (!f || 131072 & r[0]) && y(o, "height", t[17]), 4194304 & r[0] && g !== (g = `${ed+t[22]}px`) && k(e, "--top", g)
                             },
                             i(t) {
                                 f || (ut(v), ut(l.$$.fragment, t), ut(a.$$.fragment, t), ut(b), f = !0)
                             },
                             o(t) {
                                 dt(v), dt(l.$$.fragment, t), dt(a.$$.fragment, t), dt(b), f = !1
                             },
                             d(n) {
                                 n && d(e), v && v.d(), t[53](null), yt(l), yt(a), t[54](null), b && b.d()
                             }
                         }
                     }
-                    const Zu = 24,
-                        Qu = 10;
+                    const ed = 24,
+                        nd = 10;
 
-                    function td(t, e, n) {
+                    function rd(t, e, n) {
                         let r, i, o, l, a, s, c, u, d, f, h, p, g, m, v, b, y, $, w, x, _;
                         j(t, xr, (t => n(50, y = t))), j(t, ur, (t => n(24, $ = t))), j(t, Lr, (t => n(51, w = t))), j(t, _r, (t => n(52, x = t))), j(t, kr, (t => n(56, _ = t)));
                         let k, M, {
                                 width: L
                             } = e,
                             {
                                 height: A
@@ -10088,36 +10141,36 @@
                             "width" in t && n(0, L = t.width), "height" in t && n(29, A = t.height), "xValues" in t && n(30, P = t.xValues), "yValues" in t && n(31, S = t.yValues), "colorValues" in t && n(32, z = t.colorValues), "xKind" in t && n(33, T = t.xKind), "yKind" in t && n(34, N = t.yKind), "colorKind" in t && n(35, C = t.colorKind), "xDomain" in t && n(36, O = t.xDomain), "yDomain" in t && n(37, D = t.yDomain), "colorDomain" in t && n(38, B = t.colorDomain), "colorScheme" in t && n(39, E = t.colorScheme), "xLabel" in t && n(1, R = t.xLabel), "yLabel" in t && n(2, V = t.yLabel), "colorLabel" in t && n(3, H = t.colorLabel), "xAxisIntegerOnly" in t && n(4, F = t.xAxisIntegerOnly), "yAxisIntegerOnly" in t && n(5, W = t.yAxisIntegerOnly), "xAxisValueMap" in t && n(6, X = t.xAxisValueMap), "yAxisValueMap" in t && n(7, U = t.yAxisValueMap), "xDistribution" in t && n(8, Y = t.xDistribution), "yDistribution" in t && n(9, G = t.yDistribution), "opacity" in t && n(40, J = t.opacity), "allowBrushing" in t && n(41, Z = t.allowBrushing), "showMarginalDistribution" in t && n(10, Q = t.showMarginalDistribution), "marginTop" in t && n(11, tt = t.marginTop), "marginRight" in t && n(12, et = t.marginRight), "marginalPlotHeight" in t && n(13, nt = t.marginalPlotHeight)
                         }, t.$$.update = () => {
                             6144 & t.$$.dirty[0] && n(48, r = {
                                 top: tt,
                                 right: et,
                                 bottom: 35,
                                 left: 50
-                            }), 536870913 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(23, i = Math.min(L - r.left - r.right, A - Zu - r.top - r.bottom)), 8388609 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(47, o = (L - i - r.left - r.right) / 2), 545259520 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(49, l = (A - Zu - i - r.top - r.bottom) / 2), 8 & t.$$.dirty[0] && n(28, a = "" === H ? Qu : 0), 8 & t.$$.dirty[0] && n(27, s = "" === H ? 2 * Qu : Qu), 8 & t.$$.dirty[0] | 262144 & t.$$.dirty[1] && n(22, c = "" !== H ? l : 0), 4194304 & t.$$.dirty[0] | 458752 & t.$$.dirty[1] && n(21, u = {
+                            }), 536870913 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(23, i = Math.min(L - r.left - r.right, A - ed - r.top - r.bottom)), 8388609 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(47, o = (L - i - r.left - r.right) / 2), 545259520 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(49, l = (A - ed - i - r.top - r.bottom) / 2), 8 & t.$$.dirty[0] && n(28, a = "" === H ? nd : 0), 8 & t.$$.dirty[0] && n(27, s = "" === H ? 2 * nd : nd), 8 & t.$$.dirty[0] | 262144 & t.$$.dirty[1] && n(22, c = "" !== H ? l : 0), 4194304 & t.$$.dirty[0] | 458752 & t.$$.dirty[1] && n(21, u = {
                                 top: r.top + l - c,
                                 right: r.right + o,
                                 bottom: r.bottom + l,
                                 left: r.left + o
-                            }), 541065216 & t.$$.dirty[0] && n(17, d = Math.max(A - Zu - c, 0)), 2097153 & t.$$.dirty[0] | 36 & t.$$.dirty[1] && n(20, f = "quantitative" === T ? rn().domain(O).range([u.left, L - u.right]) : Rr().domain(O).paddingInner(.25).range([u.left, L - u.right])), 2228224 & t.$$.dirty[0] | 72 & t.$$.dirty[1] && n(19, h = "quantitative" === N ? rn().domain(D).range([d - u.bottom, u.top]) : Rr().domain(D).paddingInner(.25).range([d - u.bottom, u.top])), 400 & t.$$.dirty[1] && n(18, p = "quantitative" === C ? ln().domain(B).interpolator((t => Rc(rt(t)))) : Ir().domain(B).range("highlight" === E ? ["rgb(145, 145, 145)", Fn] : ["#db5c39", "#5c39db"])), 1073741824 & t.$$.dirty[0] && (g = xn(P.length)), 2228225 & t.$$.dirty[0] && n(46, m = oa().extent([
+                            }), 541065216 & t.$$.dirty[0] && n(17, d = Math.max(A - ed - c, 0)), 2097153 & t.$$.dirty[0] | 36 & t.$$.dirty[1] && n(20, f = "quantitative" === T ? rn().domain(O).range([u.left, L - u.right]) : Rr().domain(O).paddingInner(.25).range([u.left, L - u.right])), 2228224 & t.$$.dirty[0] | 72 & t.$$.dirty[1] && n(19, h = "quantitative" === N ? rn().domain(D).range([d - u.bottom, u.top]) : Rr().domain(D).paddingInner(.25).range([d - u.bottom, u.top])), 400 & t.$$.dirty[1] && n(18, p = "quantitative" === C ? ln().domain(B).interpolator((t => qc(rt(t)))) : Ir().domain(B).range("highlight" === E ? ["rgb(145, 145, 145)", Fn] : ["#db5c39", "#5c39db"])), 1073741824 & t.$$.dirty[0] && (g = xn(P.length)), 2228225 & t.$$.dirty[0] && n(46, m = oa().extent([
                                 [u.left - 2, u.top - 2],
                                 [L - u.right + 2, d - u.bottom + 2]
                             ]).on("start", ct).on("brush", ut).on("end", dt)), 163841 & t.$$.dirty[0] | 50176 & t.$$.dirty[1] && it && Z && L > 0 && d > 0 && (n(45, ot = xo(it)), ot.call(m)), 2158592 & t.$$.dirty[1] && ot && x && at && !st && ot.call(m.clear), 2 & t.$$.dirty[0] | 1049600 & t.$$.dirty[1] && n(16, lt = Z ? w.get(R) : void 0), 16842752 & t.$$.dirty[0] && n(26, v = lt && $.length > 0), 65792 & t.$$.dirty[0] && n(25, b = Y ? Rn(Y, lt) : 0), 147457 & t.$$.dirty[0] | 2048 & t.$$.dirty[1] && k && M && (Bn(k, M, L, d), dc(M, f, h, p, P, S, z, y, L, d, 2, J)), 1075707905 & t.$$.dirty[0] | 526851 & t.$$.dirty[1] && dc(M, f, h, p, P, S, z, y, L, d, 2, J)
                         }, [L, R, V, H, F, W, X, U, Y, G, Q, tt, et, nt, k, it, lt, d, p, h, f, u, c, i, $, b, v, s, a, A, P, S, z, T, N, C, O, D, B, E, J, Z, M, at, st, ot, m, o, r, l, y, w, x, function(t) {
                             K[t ? "unshift" : "push"]((() => {
                                 k = t, n(14, k)
                             }))
                         }, function(t) {
                             K[t ? "unshift" : "push"]((() => {
                                 it = t, n(15, it)
                             }))
                         }]
                     }
-                    const ed = class extends xt {
+                    const id = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, td, Ju, D, {
+                            super(), $t(this, t, rd, td, D, {
                                 width: 0,
                                 height: 29,
                                 xValues: 30,
                                 yValues: 31,
                                 colorValues: 32,
                                 xKind: 33,
                                 yKind: 34,
@@ -10137,28 +10190,28 @@
                                 yDistribution: 9,
                                 opacity: 40,
                                 allowBrushing: 41,
                                 showMarginalDistribution: 10,
                                 marginTop: 11,
                                 marginRight: 12,
                                 marginalPlotHeight: 13
-                            }, ju, [-1, -1])
+                            }, Ru, [-1, -1])
                         }
                     };
 
-                    function nd(t) {
+                    function od(t) {
                         c(t, "svelte-tm4cy6", ".segmented-control-container.svelte-tm4cy6.svelte-tm4cy6{display:flex;gap:0.25em;align-items:center}.segmented-control-buttons-row.svelte-tm4cy6.svelte-tm4cy6{display:inline-grid;grid-auto-columns:1fr;grid-auto-flow:column}.segmented-control-buttons-row.svelte-tm4cy6 button.svelte-tm4cy6{border-radius:0;border-left:none;padding:0.0625em 0.125em}.segmented-control-buttons-row.svelte-tm4cy6 button.svelte-tm4cy6:first-child{border-top-left-radius:0.25em;border-bottom-left-radius:0.25em;border-left:1px solid var(--blue)}.segmented-control-buttons-row.svelte-tm4cy6 button.svelte-tm4cy6:last-child{border-top-right-radius:0.25em;border-bottom-right-radius:0.25em}.segmented-control-buttons-row.svelte-tm4cy6 button.selected-segment.svelte-tm4cy6{color:white;background-color:var(--blue)}.segmented-control-buttons-row.svelte-tm4cy6 button.selected-segment.svelte-tm4cy6:active{color:white;background-color:var(--dark-blue);border-color:var(--dark-blue)}")
                     }
 
-                    function rd(t, e, n) {
+                    function ld(t, e, n) {
                         const r = t.slice();
                         return r[5] = e[n].value, r[6] = e[n].label, r[7] = e[n].enabled, r
                     }
 
-                    function id(t) {
+                    function ad(t) {
                         let e, n;
                         return {
                             c() {
                                 e = h("div"), n = g(t[2]), y(e, "class", "pdpilot-bold")
                             },
                             m(t, r) {
                                 u(t, e, r), s(e, n)
@@ -10168,15 +10221,15 @@
                             },
                             d(t) {
                                 t && d(e)
                             }
                         }
                     }
 
-                    function od(t) {
+                    function sd(t) {
                         let e, n, r, i, o, l = t[6] + "";
 
                         function a() {
                             return t[4](t[5])
                         }
                         return {
                             c() {
@@ -10190,49 +10243,49 @@
                             },
                             d(t) {
                                 t && d(e), i = !1, o()
                             }
                         }
                     }
 
-                    function ld(t) {
-                        let e, n, r, i = t[2] && id(t),
+                    function cd(t) {
+                        let e, n, r, i = t[2] && ad(t),
                             o = ft(t[1]),
                             l = [];
-                        for (let e = 0; e < o.length; e += 1) l[e] = od(rd(t, o, e));
+                        for (let e = 0; e < o.length; e += 1) l[e] = sd(ld(t, o, e));
                         return {
                             c() {
                                 e = h("div"), i && i.c(), n = m(), r = h("div");
                                 for (let t = 0; t < l.length; t += 1) l[t].c();
                                 y(r, "class", "segmented-control-buttons-row svelte-tm4cy6"), y(e, "class", "segmented-control-container svelte-tm4cy6")
                             },
                             m(t, o) {
                                 u(t, e, o), i && i.m(e, null), s(e, n), s(e, r);
                                 for (let t = 0; t < l.length; t += 1) l[t] && l[t].m(r, null)
                             },
                             p(t, [a]) {
-                                if (t[2] ? i ? i.p(t, a) : (i = id(t), i.c(), i.m(e, n)) : i && (i.d(1), i = null), 11 & a) {
+                                if (t[2] ? i ? i.p(t, a) : (i = ad(t), i.c(), i.m(e, n)) : i && (i.d(1), i = null), 11 & a) {
                                     let e;
                                     for (o = ft(t[1]), e = 0; e < o.length; e += 1) {
-                                        const n = rd(t, o, e);
-                                        l[e] ? l[e].p(n, a) : (l[e] = od(n), l[e].c(), l[e].m(r, null))
+                                        const n = ld(t, o, e);
+                                        l[e] ? l[e].p(n, a) : (l[e] = sd(n), l[e].c(), l[e].m(r, null))
                                     }
                                     for (; e < l.length; e += 1) l[e].d(1);
                                     l.length = o.length
                                 }
                             },
                             i: z,
                             o: z,
                             d(t) {
                                 t && d(e), i && i.d(), f(l, t)
                             }
                         }
                     }
 
-                    function ad(t, e, n) {
+                    function ud(t, e, n) {
                         let {
                             segments: r
                         } = e, {
                             selectedValue: i
                         } = e, {
                             title: o = ""
                         } = e;
@@ -10240,46 +10293,46 @@
                         function l(t) {
                             n(0, i = t)
                         }
                         return t.$$set = t => {
                             "segments" in t && n(1, r = t.segments), "selectedValue" in t && n(0, i = t.selectedValue), "title" in t && n(2, o = t.title)
                         }, [i, r, o, l, t => l(t)]
                     }
-                    const sd = class extends xt {
+                    const dd = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, ad, ld, D, {
+                            super(), $t(this, t, ud, cd, D, {
                                 segments: 1,
                                 selectedValue: 0,
                                 title: 2
-                            }, nd)
+                            }, od)
                         }
                     };
 
-                    function cd(t) {
+                    function fd(t) {
                         c(t, "svelte-a1f3se", ".one-way-detailed-pdp-container.svelte-a1f3se{display:flex;width:100%;height:100%}.pdpilot-no-clusters-message.svelte-a1f3se{flex:1;text-align:center;align-self:center}.pdpilot-half.svelte-a1f3se{flex:1;display:flex;flex-direction:column}.pdpilot-half-vis.svelte-a1f3se{flex:1}.pdpilot-vertical-divider.svelte-a1f3se{width:1px;margin:0 1em;background-color:var(--gray-1)}")
                     }
 
-                    function ud(t) {
+                    function hd(t) {
                         let e, n, r, i, o, l, a, c, f, p, g, v, b, $, w, x, _, M, L, P, S, z = ("cluster-lines" === t[5] ? .25 : .5) + "em",
                             T = ("cluster-descriptions" === t[4] ? .25 : .5) + "em";
 
                         function N(e) {
                             t[21](e)
                         }
                         let C = {
                             segments: t[19],
                             title: "ICE Plot"
                         };
 
                         function O(e) {
                             t[23](e)
                         }
-                        void 0 !== t[5] && (C.selectedValue = t[5]), r = new sd({
+                        void 0 !== t[5] && (C.selectedValue = t[5]), r = new dd({
                             props: C
-                        }), K.push((() => mt(r, "selectedValue", N))), a = new hu({
+                        }), K.push((() => mt(r, "selectedValue", N))), a = new mu({
                             props: {
                                 pd: t[0],
                                 width: t[11],
                                 height: t[10],
                                 scaleLocally: t[12],
                                 showMarginalDistribution: !1,
                                 marginTop: "cluster-lines" === t[5] ? 0 : 10,
@@ -10290,18 +10343,18 @@
                                 showColorLegend: !1
                             }
                         });
                         let D = {
                             segments: t[6],
                             title: "Context"
                         };
-                        void 0 !== t[4] && (D.selectedValue = t[4]), $ = new sd({
+                        void 0 !== t[4] && (D.selectedValue = t[4]), $ = new dd({
                             props: D
                         }), K.push((() => mt($, "selectedValue", O)));
-                        const B = [hd, fd],
+                        const B = [md, gd],
                             j = [];
 
                         function E(t, e) {
                             return "cluster-descriptions" === t[4] ? 0 : "scatterplot" === t[4] ? 1 : -1
                         }
                         return ~(M = E(t)) && (L = j[M] = B[M](t)), {
                             c() {
@@ -10330,15 +10383,15 @@
                             },
                             d(t) {
                                 t && (d(e), d(f), d(p), d(g), d(v)), yt(r), yt(a), c(), yt($), ~M && j[M].d(), P()
                             }
                         }
                     }
 
-                    function dd(t) {
+                    function pd(t) {
                         let e;
                         return {
                             c() {
                                 e = h("div"), e.textContent = "This feature does not have enough distinct clusters of ICE lines.", y(e, "class", "pdpilot-no-clusters-message svelte-a1f3se")
                             },
                             m(t, n) {
                                 u(t, e, n)
@@ -10348,17 +10401,17 @@
                             o: z,
                             d(t) {
                                 t && d(e)
                             }
                         }
                     }
 
-                    function fd(t) {
+                    function gd(t) {
                         let e, n;
-                        return e = new ed({
+                        return e = new id({
                             props: {
                                 width: t[9],
                                 height: t[8],
                                 xValues: t[13][t[0].x_feature],
                                 yValues: t[14],
                                 colorValues: Array.from({
                                     length: t[15]
@@ -10367,28 +10420,28 @@
                                 yKind: t[17] ? "categorical" : "quantitative",
                                 colorKind: "categorical",
                                 xDomain: "categorical" === t[1].kind ? t[0].x_values : [t[0].x_values[0], t[0].x_values[t[0].x_values.length - 1]],
                                 yDomain: t[18],
                                 colorDomain: [0, 1],
                                 colorScheme: "highlight",
                                 xLabel: t[0].x_feature,
-                                yLabel: "Ground Truth",
+                                yLabel: "Ground truth",
                                 colorLabel: "",
                                 xAxisIntegerOnly: "discrete" === t[1].subkind,
                                 yAxisIntegerOnly: !1,
                                 xAxisValueMap: "value_map" in t[1] ? t[1].value_map : {},
                                 yAxisValueMap: {},
                                 xDistribution: t[1].distribution,
                                 yDistribution: null,
                                 opacity: .5,
                                 allowBrushing: !0,
                                 showMarginalDistribution: !0,
-                                marginTop: gd + 3,
-                                marginRight: gd + 3,
-                                marginalPlotHeight: gd
+                                marginTop: bd + 3,
+                                marginRight: bd + 3,
+                                marginalPlotHeight: bd
                             }
                         }), {
                             c() {
                                 vt(e.$$.fragment)
                             },
                             m(t, r) {
                                 bt(e, t, r), n = !0
@@ -10407,17 +10460,17 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function hd(t) {
+                    function md(t) {
                         let e, n;
-                        return e = new Bu({
+                        return e = new Iu({
                             props: {
                                 pd: t[0],
                                 features: Sn(t[0]).interacting_features
                             }
                         }), e.$on("filter", t[20]), {
                             c() {
                                 vt(e.$$.fragment)
@@ -10437,17 +10490,17 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function pd(t) {
+                    function vd(t) {
                         let e, n, r, i;
-                        const o = [dd, ud],
+                        const o = [pd, hd],
                             l = [];
 
                         function a(t, e) {
                             return "cluster-lines" === t[5] && 1 === t[0].ice.num_clusters ? 0 : 1
                         }
                         return n = a(t), r = l[n] = o[n](t), {
                             c() {
@@ -10469,17 +10522,17 @@
                                 dt(r), i = !1
                             },
                             d(t) {
                                 t && d(e), l[n].d()
                             }
                         }
                     }
-                    const gd = 50;
+                    const bd = 50;
 
-                    function md(t, e, n) {
+                    function yd(t, e, n) {
                         let r, i, o, a, s, c, u, d, f, h, p, g, m;
                         j(t, $r, (t => n(4, s = t))), j(t, yr, (t => n(5, c = t))), j(t, wr, (t => n(12, u = t))), j(t, Jn, (t => n(13, d = t))), j(t, Zn, (t => n(14, f = t))), j(t, Qn, (t => n(15, h = t))), j(t, Mr, (t => n(16, p = t))), j(t, gr, (t => n(17, g = t))), j(t, mr, (t => n(18, m = t)));
                         let v, b, {
                                 pd: y
                             } = e,
                             {
                                 featureInfo: $
@@ -10518,59 +10571,59 @@
                             v = l.entries.get(this)?.contentRect, n(2, v)
                         }, function(t) {
                             s = t, $r.set(s)
                         }, (t, e) => p.has(e) ? 1 : 0, function() {
                             b = l.entries.get(this)?.contentRect, n(3, b)
                         }]
                     }
-                    const vd = class extends xt {
+                    const $d = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, md, pd, D, {
+                            super(), $t(this, t, yd, vd, D, {
                                 pd: 0,
                                 featureInfo: 1
-                            }, cd)
+                            }, fd)
                         }
                     };
 
-                    function bd(t) {
+                    function wd(t) {
                         c(t, "svelte-jg5wjz", ".two-way-pdp-grid.svelte-jg5wjz{display:grid;width:100%;height:100%;grid-template-columns:1fr 1fr 1fr;grid-template-areas:'two-way-interaction two-way-pdp scatter'}")
                     }
 
-                    function yd(t) {
+                    function xd(t) {
                         let e, n, r, i, o, l, a, c, f, p, g;
-                        return r = new hu({
+                        return r = new mu({
                             props: {
                                 pd: t[0],
                                 width: t[4],
                                 height: t[5],
                                 scaleLocally: t[6],
                                 showMarginalPdp: !0,
-                                marginTop: $d + 1,
-                                marginRight: $d + 1,
-                                marginalPlotHeight: $d,
+                                marginTop: _d + 1,
+                                marginRight: _d + 1,
+                                marginalPlotHeight: _d,
                                 iceLevel: "lines",
                                 colorShows: "interactions",
                                 showColorLegend: !0,
                                 colorLegendTitle: "Interactions"
                             }
-                        }), l = new hu({
+                        }), l = new mu({
                             props: {
                                 pd: t[0],
                                 width: t[4],
                                 height: t[5],
                                 scaleLocally: t[6],
                                 showMarginalPdp: !0,
-                                marginTop: $d + 1,
-                                marginRight: $d + 1,
-                                marginalPlotHeight: $d,
+                                marginTop: _d + 1,
+                                marginRight: _d + 1,
+                                marginalPlotHeight: _d,
                                 iceLevel: "lines",
                                 showColorLegend: !0,
                                 colorLegendTitle: "Predictions"
                             }
-                        }), f = new ed({
+                        }), f = new id({
                             props: {
                                 width: t[4],
                                 height: t[5],
                                 xValues: t[7][t[0].x_feature],
                                 yValues: t[7][t[0].y_feature],
                                 colorValues: t[8],
                                 xKind: t[1].kind,
@@ -10578,27 +10631,27 @@
                                 colorKind: t[9] ? "categorical" : "quantitative",
                                 xDomain: "categorical" === t[1].kind ? t[0].x_axis : [t[0].x_axis[0], t[0].x_axis[t[0].x_axis.length - 1]],
                                 yDomain: "categorical" === t[10][t[0].y_feature].kind ? t[0].y_axis : [t[0].y_axis[0], t[0].y_axis[t[0].y_axis.length - 1]],
                                 colorDomain: t[11],
                                 colorScheme: t[9] ? "classes" : "sequential",
                                 xLabel: t[0].x_feature,
                                 yLabel: t[0].y_feature,
-                                colorLabel: "Ground Truth",
+                                colorLabel: "Ground truth",
                                 xAxisIntegerOnly: "discrete" === t[1].subkind,
                                 yAxisIntegerOnly: "discrete" === t[2].subkind,
                                 xAxisValueMap: "value_map" in t[1] ? t[1].value_map : {},
                                 yAxisValueMap: "value_map" in t[2] ? t[2].value_map : {},
                                 xDistribution: t[1].distribution,
                                 yDistribution: t[2].distribution,
                                 opacity: 1,
                                 allowBrushing: !1,
                                 showMarginalDistribution: !0,
-                                marginTop: $d + 3,
-                                marginRight: $d + 3,
-                                marginalPlotHeight: $d
+                                marginTop: _d + 3,
+                                marginRight: _d + 3,
+                                marginalPlotHeight: _d
                             }
                         }), {
                             c() {
                                 e = h("div"), n = h("div"), vt(r.$$.fragment), i = m(), o = h("div"), vt(l.$$.fragment), a = m(), c = h("div"), vt(f.$$.fragment), k(n, "grid-area", "two-way-interaction"), k(o, "grid-area", "two-way-pdp"), k(c, "grid-area", "scatter"), y(e, "class", "two-way-pdp-grid svelte-jg5wjz")
                             },
                             m(d, h) {
                                 u(d, e, h), s(e, n), bt(r, n, null), s(e, i), s(e, o), bt(l, o, null), s(e, a), s(e, c), bt(f, c, null), p = A.observe(e, t[13].bind(e)), g = !0
@@ -10618,17 +10671,17 @@
                                 dt(r.$$.fragment, t), dt(l.$$.fragment, t), dt(f.$$.fragment, t), g = !1
                             },
                             d(t) {
                                 t && d(e), yt(r), yt(l), yt(f), p()
                             }
                         }
                     }
-                    const $d = 50;
+                    const _d = 50;
 
-                    function wd(t, e, n) {
+                    function kd(t, e, n) {
                         let r, i, o, a, s, c, u, d, f;
                         j(t, wr, (t => n(6, a = t))), j(t, Jn, (t => n(7, s = t))), j(t, Zn, (t => n(8, c = t))), j(t, gr, (t => n(9, u = t))), j(t, Gn, (t => n(10, d = t))), j(t, mr, (t => n(11, f = t)));
                         let h, {
                                 pd: p
                             } = e,
                             {
                                 xFeatureInfo: g
@@ -10640,39 +10693,39 @@
                             "pd" in t && n(0, p = t.pd), "xFeatureInfo" in t && n(1, g = t.xFeatureInfo), "yFeatureInfo" in t && n(2, m = t.yFeatureInfo)
                         }, t.$$.update = () => {
                             8 & t.$$.dirty && n(12, r = h ? h.width : 0), 8 & t.$$.dirty && n(5, i = h ? h.height : 0), 4096 & t.$$.dirty && n(4, o = r / 3)
                         }, [p, g, m, h, o, i, a, s, c, u, d, f, r, function() {
                             h = l.entries.get(this)?.contentRect, n(3, h)
                         }]
                     }
-                    const xd = class extends xt {
+                    const Md = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, wd, yd, D, {
+                            super(), $t(this, t, kd, xd, D, {
                                 pd: 0,
                                 xFeatureInfo: 1,
                                 yFeatureInfo: 2
-                            }, bd)
+                            }, wd)
                         }
                     };
 
-                    function _d(t) {
+                    function Ld(t) {
                         c(t, "svelte-1oprcpz", ".zoomed-pdp-container.svelte-1oprcpz.svelte-1oprcpz{width:100%;height:100%;display:flex;flex-direction:column}.zoomed-pdp-header.svelte-1oprcpz.svelte-1oprcpz{height:2em;display:flex;align-items:center;background-color:white;gap:1.5em;padding-left:0.5em;padding-right:0.5em;border-bottom:1px solid var(--gray-1)}.feature-selects.svelte-1oprcpz.svelte-1oprcpz{flex:0 1 auto;min-width:0;display:flex;align-items:center;gap:0.5em}.feature-selects.svelte-1oprcpz label.svelte-1oprcpz{flex:0 1 auto;display:flex;align-items:center;gap:0.25em;min-width:0}.feature-selects.svelte-1oprcpz label span.svelte-1oprcpz{flex:0 0 auto}.feature-selects.svelte-1oprcpz label select.svelte-1oprcpz{flex:0 1 auto;min-width:0;text-overflow:ellipsis}.zoomed-pdp-content.svelte-1oprcpz.svelte-1oprcpz{flex:1;padding:0.5em;min-height:0px}.label-and-input.svelte-1oprcpz.svelte-1oprcpz{flex:0 0 auto;display:flex;align-items:center;gap:0.25em}.detailed-plot-message-container.svelte-1oprcpz.svelte-1oprcpz{height:100%;width:100%;align-items:center;justify-content:center;display:flex}.detailed-plot-message-content.svelte-1oprcpz.svelte-1oprcpz{width:40em;display:flex;flex-direction:column;justify-content:center;gap:1em}.detailed-plot-message-content.svelte-1oprcpz>button.svelte-1oprcpz{margin:auto}")
                     }
 
-                    function kd(t, e, n) {
+                    function Ad(t, e, n) {
                         const r = t.slice();
                         return r[18] = e[n], r
                     }
 
-                    function Md(t, e, n) {
+                    function Pd(t, e, n) {
                         const r = t.slice();
                         return r[18] = e[n], r
                     }
 
-                    function Ld(t) {
+                    function Sd(t) {
                         let e, n, r, i = t[18] + "";
                         return {
                             c() {
                                 e = h("option"), n = g(i), e.__value = r = t[18], _(e, e.__value)
                             },
                             m(t, r) {
                                 u(t, e, r), s(e, n)
@@ -10682,15 +10735,15 @@
                             },
                             d(t) {
                                 t && d(e)
                             }
                         }
                     }
 
-                    function Ad(t) {
+                    function zd(t) {
                         let e, n, r, i = t[18] + "";
                         return {
                             c() {
                                 e = h("option"), n = g(i), e.__value = r = t[18], _(e, e.__value)
                             },
                             m(t, r) {
                                 u(t, e, r), s(e, n)
@@ -10700,33 +10753,33 @@
                             },
                             d(t) {
                                 t && d(e)
                             }
                         }
                     }
 
-                    function Pd(t) {
-                        let e, n, r, i, o, l, a, c = 2 === t[0].num_features && Sd(t);
+                    function Td(t) {
+                        let e, n, r, i, o, l, a, c = 2 === t[0].num_features && Nd(t);
                         return {
                             c() {
                                 e = h("label"), n = h("input"), r = g("Scale\n        locally"), i = m(), c && c.c(), o = v(), y(n, "type", "checkbox"), y(e, "class", "label-and-input svelte-1oprcpz")
                             },
                             m(d, f) {
                                 u(d, e, f), s(e, n), n.checked = t[7], s(e, r), u(d, i, f), c && c.m(d, f), u(d, o, f), l || (a = b(n, "change", t[15]), l = !0)
                             },
                             p(t, e) {
-                                128 & e && (n.checked = t[7]), 2 === t[0].num_features ? c ? c.p(t, e) : (c = Sd(t), c.c(), c.m(o.parentNode, o)) : c && (c.d(1), c = null)
+                                128 & e && (n.checked = t[7]), 2 === t[0].num_features ? c ? c.p(t, e) : (c = Nd(t), c.c(), c.m(o.parentNode, o)) : c && (c.d(1), c = null)
                             },
                             d(t) {
                                 t && (d(e), d(i), d(o)), c && c.d(t), l = !1, a()
                             }
                         }
                     }
 
-                    function Sd(t) {
+                    function Nd(t) {
                         let e, n, r;
                         return {
                             c() {
                                 e = h("button"), e.textContent = "Swap Axes", y(e, "title", "Swap x and y axes")
                             },
                             m(i, o) {
                                 u(i, e, o), n || (r = b(e, "click", t[9]), n = !0)
@@ -10734,17 +10787,17 @@
                             p: z,
                             d(t) {
                                 t && d(e), n = !1, r()
                             }
                         }
                     }
 
-                    function zd(t) {
+                    function Cd(t) {
                         let e, n;
-                        return e = new xd({
+                        return e = new Md({
                             props: {
                                 pd: t[0],
                                 xFeatureInfo: t[4],
                                 yFeatureInfo: t[3]
                             }
                         }), {
                             c() {
@@ -10765,17 +10818,17 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function Td(t) {
+                    function Od(t) {
                         let e, n;
-                        return e = new vd({
+                        return e = new $d({
                             props: {
                                 pd: t[0],
                                 featureInfo: t[4]
                             }
                         }), {
                             c() {
                                 vt(e.$$.fragment)
@@ -10795,19 +10848,19 @@
                             },
                             d(t) {
                                 yt(e, t)
                             }
                         }
                     }
 
-                    function Nd(t) {
+                    function Dd(t) {
                         let e, n;
 
                         function r(t, e) {
-                            return "" === t[2] && "" === t[1] ? Od : Cd
+                            return "" === t[2] && "" === t[1] ? jd : Bd
                         }
                         let i = r(t),
                             o = i(t);
                         return {
                             c() {
                                 e = h("div"), n = h("div"), o.c(), y(n, "class", "detailed-plot-message-content svelte-1oprcpz"), y(e, "class", "detailed-plot-message-container svelte-1oprcpz")
                             },
@@ -10821,15 +10874,15 @@
                             o: z,
                             d(t) {
                                 t && d(e), o.d()
                             }
                         }
                     }
 
-                    function Cd(t) {
+                    function Bd(t) {
                         let e, n, r, i, o, l, a, c, f, p, v, $, w = 2 === t[5].length ? "Computing..." : "Compute Now";
                         return {
                             c() {
                                 e = h("div"), n = g("The two-way PDP between "), r = g(t[2]), i = g(" and "), o = g(t[1]), l = g("\n              was not pre-computed, since we did not detect a likely interaction\n              between the two features."), a = m(), c = h("button"), f = g(w), c.disabled = p = 2 === t[5].length, y(c, "class", "svelte-1oprcpz")
                             },
                             m(d, h) {
                                 u(d, e, h), s(e, n), s(e, r), s(e, i), s(e, o), s(e, l), u(d, a, h), u(d, c, h), s(c, f), v || ($ = b(c, "click", t[8]), v = !0)
@@ -10839,15 +10892,15 @@
                             },
                             d(t) {
                                 t && (d(e), d(a), d(c)), v = !1, $()
                             }
                         }
                     }
 
-                    function Od(t) {
+                    function jd(t) {
                         let e;
                         return {
                             c() {
                                 e = h("div"), e.textContent = "Select one or two features above.", k(e, "text-align", "center")
                             },
                             m(t, n) {
                                 u(t, e, n)
@@ -10855,23 +10908,23 @@
                             p: z,
                             d(t) {
                                 t && d(e)
                             }
                         }
                     }
 
-                    function Dd(t) {
+                    function Ed(t) {
                         let e, n, r, i, o, l, a, c, p, g, v, $, w, x, k, L, A, P, S, z, T, N, O = ft(t[6]),
                             D = [];
-                        for (let e = 0; e < O.length; e += 1) D[e] = Ld(Md(t, O, e));
+                        for (let e = 0; e < O.length; e += 1) D[e] = Sd(Pd(t, O, e));
                         let B = ft(t[6]),
                             j = [];
-                        for (let e = 0; e < B.length; e += 1) j[e] = Ad(kd(t, B, e));
-                        let E = t[0] && Pd(t);
-                        const I = [Nd, Td, zd],
+                        for (let e = 0; e < B.length; e += 1) j[e] = zd(Ad(t, B, e));
+                        let E = t[0] && Td(t);
+                        const I = [Dd, Od, Cd],
                             R = [];
 
                         function V(t, e) {
                             return null === t[0] ? 0 : 1 === t[0].num_features && t[4] ? 1 : 2 === t[0].num_features && t[4] && t[3] ? 2 : -1
                         }
                         return ~(P = V(t)) && (S = R[P] = I[P](t)), {
                             c() {
@@ -10888,30 +10941,30 @@
                                 for (let t = 0; t < j.length; t += 1) j[t] && j[t].m(w, null);
                                 M(w, t[1], !0), s(n, k), E && E.m(n, null), s(e, L), s(e, A), ~P && R[P].m(A, null), z = !0, T || (N = [b(a, "change", t[13]), b(w, "change", t[14])], T = !0)
                             },
                             p(t, [e]) {
                                 if (64 & e) {
                                     let n;
                                     for (O = ft(t[6]), n = 0; n < O.length; n += 1) {
-                                        const r = Md(t, O, n);
-                                        D[n] ? D[n].p(r, e) : (D[n] = Ld(r), D[n].c(), D[n].m(a, null))
+                                        const r = Pd(t, O, n);
+                                        D[n] ? D[n].p(r, e) : (D[n] = Sd(r), D[n].c(), D[n].m(a, null))
                                     }
                                     for (; n < D.length; n += 1) D[n].d(1);
                                     D.length = O.length
                                 }
                                 if (68 & e && M(a, t[2]), 64 & e) {
                                     let n;
                                     for (B = ft(t[6]), n = 0; n < B.length; n += 1) {
-                                        const r = kd(t, B, n);
-                                        j[n] ? j[n].p(r, e) : (j[n] = Ad(r), j[n].c(), j[n].m(w, null))
+                                        const r = Ad(t, B, n);
+                                        j[n] ? j[n].p(r, e) : (j[n] = zd(r), j[n].c(), j[n].m(w, null))
                                     }
                                     for (; n < j.length; n += 1) j[n].d(1);
                                     j.length = B.length
                                 }
-                                66 & e && M(w, t[1]), t[0] ? E ? E.p(t, e) : (E = Pd(t), E.c(), E.m(n, null)) : E && (E.d(1), E = null);
+                                66 & e && M(w, t[1]), t[0] ? E ? E.p(t, e) : (E = Td(t), E.c(), E.m(n, null)) : E && (E.d(1), E = null);
                                 let r = P;
                                 P = V(t), P === r ? ~P && R[P].p(t, e) : (S && (st(), dt(R[r], 1, 1, (() => {
                                     R[r] = null
                                 })), ct()), ~P ? (S = R[P], S ? S.p(t, e) : (S = R[P] = I[P](t), S.c()), ut(S, 1), S.m(A, null)) : S = null)
                             },
                             i(t) {
                                 z || (ut(S), z = !0)
@@ -10921,15 +10974,15 @@
                             },
                             d(t) {
                                 t && d(e), f(D, t), f(j, t), E && E.d(), ~P && R[P].d(), T = !1, C(N)
                             }
                         }
                     }
 
-                    function Bd(t, e, n) {
+                    function Id(t, e, n) {
                         let r, i, o, l, a, s, c, u, d, f;
                         j(t, nr, (t => n(10, o = t))), j(t, Gn, (t => n(11, l = t))), j(t, pr, (t => n(12, a = t))), j(t, br, (t => n(1, s = t))), j(t, vr, (t => n(2, c = t))), j(t, dr, (t => n(5, u = t))), j(t, Yn, (t => n(6, d = t))), j(t, wr, (t => n(7, f = t)));
                         let h = null;
                         return t.$$.update = () => {
                             var e, d;
                             4102 & t.$$.dirty && (c === s && I(br, s = "", s), "" === c && "" !== s && (I(vr, c = s, c), I(br, s = "", s)), n(0, h = "" === s ? null !== (e = a.get(c)) && void 0 !== e ? e : null : null !== (d = o.find((t => t.x_feature === c && t.y_feature === s || t.x_feature === s && t.y_feature === c))) && void 0 !== d ? d : null)), 1024 & t.$$.dirty && o && function() {
                                 const t = o.find((t => t.x_feature === u[0] && t.y_feature === u[1] || t.x_feature === u[1] && t.y_feature === u[0]));
@@ -10950,30 +11003,30 @@
                             c = L(this), vr.set(c)
                         }, function() {
                             s = L(this), br.set(s)
                         }, function() {
                             f = this.checked, wr.set(f)
                         }]
                     }
-                    const jd = class extends xt {
+                    const Rd = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, Bd, Dd, D, {}, _d)
+                            super(), $t(this, t, Id, Ed, D, {}, Ld)
                         }
                     };
 
-                    function Ed(t) {
+                    function Vd(t) {
                         c(t, "svelte-1ps68ru", ".controls-features.svelte-1ps68ru.svelte-1ps68ru{display:flex;flex-direction:column;max-height:100%;row-gap:0.25em}ul.svelte-1ps68ru.svelte-1ps68ru{list-style:none}.fs-row.svelte-1ps68ru.svelte-1ps68ru{display:flex;align-items:center;column-gap:0.25em}input.svelte-1ps68ru.svelte-1ps68ru{min-width:0}.fs-row.svelte-1ps68ru label.svelte-1ps68ru{flex:1}.individual-features.svelte-1ps68ru.svelte-1ps68ru{flex:0 1 auto;overflow-y:auto;min-height:0}.hidden.svelte-1ps68ru.svelte-1ps68ru{display:none}.disabled-feature-label.svelte-1ps68ru.svelte-1ps68ru{color:var(--gray-5);cursor:not-allowed}")
                     }
 
-                    function Id(t, e, n) {
+                    function Hd(t, e, n) {
                         const r = t.slice();
                         return r[13] = e[n].feature, r[14] = e[n].hidden, r[15] = e[n].disabled, r
                     }
 
-                    function Rd(t, e) {
+                    function qd(t, e) {
                         let n, r, i, o, l, a, c, f, p, v, $, k, M, L, A = !1,
                             P = e[13] + "";
                         return k = w(e[9][0]), {
                             key: t,
                             first: null,
                             c() {
                                 n = h("li"), r = h("input"), a = m(), c = h("label"), f = g(P), $ = m(), y(r, "id", i = e[0] + "-" + e[13] + "-checkbox"), y(r, "type", "checkbox"), y(r, "name", "features"), r.__value = o = e[13], _(r, r.__value), r.disabled = l = e[15], y(r, "class", "svelte-1ps68ru"), y(c, "class", "pdpilot-cutoff svelte-1ps68ru"), y(c, "for", p = e[0] + "-" + e[13] + "-checkbox"), y(c, "title", v = e[13]), S(c, "disabled-feature-label", e[15]), y(n, "class", "fs-row svelte-1ps68ru"), S(n, "hidden", e[14]), k.p(r), this.first = n
@@ -10986,49 +11039,49 @@
                             },
                             d(t) {
                                 t && d(n), k.r(), M = !1, L()
                             }
                         }
                     }
 
-                    function Vd(t) {
+                    function Fd(t) {
                         let e, n, r, i, o, l, a, c, f = [],
                             p = new Map,
                             v = ft(t[3]);
                         const $ = t => t[13];
                         for (let e = 0; e < v.length; e += 1) {
-                            let n = Id(t, v, e),
+                            let n = Hd(t, v, e),
                                 r = $(n);
-                            p.set(r, f[e] = Rd(r, n))
+                            p.set(r, f[e] = qd(r, n))
                         }
                         return {
                             c() {
                                 e = h("div"), n = h("label"), r = g("Search\n    "), i = h("input"), o = m(), l = h("ul");
                                 for (let t = 0; t < f.length; t += 1) f[t].c();
                                 y(i, "class", "svelte-1ps68ru"), y(n, "class", "fs-row svelte-1ps68ru"), y(l, "class", "individual-features svelte-1ps68ru"), y(e, "class", "controls-features svelte-1ps68ru")
                             },
                             m(d, h) {
                                 u(d, e, h), s(e, n), s(n, r), s(n, i), _(i, t[1]), s(e, o), s(e, l);
                                 for (let t = 0; t < f.length; t += 1) f[t] && f[t].m(l, null);
                                 a || (c = b(i, "input", t[7]), a = !0)
                             },
                             p(t, [e]) {
-                                2 & e && i.value !== t[1] && _(i, t[1]), 13 & e && (v = ft(t[3]), f = gt(f, e, $, 1, t, v, p, l, ht, Rd, null, Id))
+                                2 & e && i.value !== t[1] && _(i, t[1]), 13 & e && (v = ft(t[3]), f = gt(f, e, $, 1, t, v, p, l, ht, qd, null, Hd))
                             },
                             i: z,
                             o: z,
                             d(t) {
                                 t && d(e);
                                 for (let t = 0; t < f.length; t += 1) f[t].d();
                                 a = !1, c()
                             }
                         }
                     }
 
-                    function Hd(t, e, n) {
+                    function Wd(t, e, n) {
                         let r, i;
                         j(t, Yn, (t => n(6, i = t)));
                         let {
                             enabledFeatures: o
                         } = e, {
                             idPrefix: l
                         } = e;
@@ -11057,32 +11110,32 @@
                             n(2, c = [])
                         }, i, function() {
                             s = this.value, n(1, s)
                         }, function() {
                             c = $(d[0], this.__value, this.checked), n(2, c), n(6, i)
                         }, d]
                     }
-                    const qd = class extends xt {
+                    const Kd = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, Hd, Vd, D, {
+                            super(), $t(this, t, Wd, Fd, D, {
                                 enabledFeatures: 4,
                                 idPrefix: 0,
                                 clear: 5
-                            }, Ed)
+                            }, Vd)
                         }
                         get clear() {
                             return this.$$.ctx[5]
                         }
                     };
 
-                    function Fd(t) {
+                    function Xd(t) {
                         c(t, "svelte-zyfurg", "ul.svelte-zyfurg.svelte-zyfurg{list-style:none}.label-and-input.svelte-zyfurg.svelte-zyfurg{display:flex;align-items:center;gap:0.25em}ul.svelte-zyfurg ul.svelte-zyfurg{margin-left:1em}")
                     }
 
-                    function Wd(t) {
+                    function Ud(t) {
                         let e, n, r, i, o, l, a, c, f, p, g, v, $, x, k, M, L, A, P, S, T, N, O, D, B, j, E, I, R;
                         return E = w(t[7][0]), {
                             c() {
                                 e = h("div"), n = h("ul"), r = h("li"), i = h("label"), o = h("input"), a = h("span"), a.textContent = "Ordered", c = m(), f = h("ul"), p = h("li"), g = h("label"), v = h("input"), $ = h("span"), $.textContent = "Increasing", x = m(), k = h("label"), M = h("input"), L = h("span"), L.textContent = "Decreasing", A = m(), P = h("label"), S = h("input"), T = h("span"), T.textContent = "Mixed", N = m(), O = h("li"), D = h("label"), B = h("input"), j = h("span"), j.textContent = "Nominal", y(o, "type", "checkbox"), o.indeterminate = l = t[0].ordered.shapes.length > 0 && t[0].ordered.shapes.length < t[1].length, y(i, "class", "label-and-input svelte-zyfurg"), y(v, "type", "checkbox"), v.__value = "increasing", _(v, v.__value), y(g, "class", "label-and-input svelte-zyfurg"), y(M, "type", "checkbox"), M.__value = "decreasing", _(M, M.__value), y(k, "class", "label-and-input svelte-zyfurg"), y(S, "type", "checkbox"), S.__value = "mixed", _(S, S.__value), y(P, "class", "label-and-input svelte-zyfurg"), y(f, "class", "svelte-zyfurg"), y(B, "type", "checkbox"), y(D, "class", "label-and-input svelte-zyfurg"), y(n, "class", "svelte-zyfurg"), E.p(v, M, S)
                             },
                             m(l, d) {
                                 u(l, e, d), s(e, n), s(n, r), s(r, i), s(i, o), o.checked = t[0].ordered.checked, s(i, a), s(r, c), s(r, f), s(f, p), s(p, g), s(g, v), v.checked = ~(t[0].ordered.shapes || []).indexOf(v.__value), s(g, $), s(p, x), s(p, k), s(k, M), M.checked = ~(t[0].ordered.shapes || []).indexOf(M.__value), s(k, L), s(p, A), s(p, P), s(P, S), S.checked = ~(t[0].ordered.shapes || []).indexOf(S.__value), s(P, T), s(n, N), s(n, O), s(O, D), s(D, B), B.checked = t[0].nominal.checked, s(D, j), I || (R = [b(o, "change", t[5]), b(o, "change", t[2]), b(v, "change", t[6]), b(v, "change", t[3]), b(M, "change", t[8]), b(M, "change", t[3]), b(S, "change", t[9]), b(S, "change", t[3]), b(B, "change", t[10])], I = !0)
@@ -11094,15 +11147,15 @@
                             o: z,
                             d(t) {
                                 t && d(e), E.r(), I = !1, C(R)
                             }
                         }
                     }
 
-                    function Kd(t, e, n) {
+                    function Yd(t, e, n) {
                         let r = ["increasing", "decreasing", "mixed"];
                         const i = {
                             ordered: {
                                 checked: !0,
                                 shapes: r
                             },
                             nominal: {
@@ -11161,103 +11214,103 @@
                             o.ordered.shapes = $(s[0], this.__value, this.checked), n(0, o), n(1, r)
                         }, function() {
                             o.ordered.shapes = $(s[0], this.__value, this.checked), n(0, o), n(1, r)
                         }, function() {
                             o.nominal.checked = this.checked, n(0, o), n(1, r)
                         }]
                     }
-                    const Xd = class extends xt {
+                    const Gd = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, Kd, Wd, D, {
+                            super(), $t(this, t, Yd, Ud, D, {
                                 clear: 4
-                            }, Fd)
+                            }, Xd)
                         }
                         get clear() {
                             return this.$$.ctx[4]
                         }
                     };
 
-                    function Ud(t) {
+                    function Jd(t) {
                         c(t, "svelte-2uqume", ".toggle-and-title.svelte-2uqume.svelte-2uqume{display:flex;align-items:center;gap:0.25em}.icon-tabler-chevron-down.svelte-2uqume polyline.svelte-2uqume{transition:transform 150ms}.rotate-polyline.svelte-2uqume.svelte-2uqume{transform-origin:50% 50%;transform:rotate(-90deg)}")
                     }
 
-                    function Yd(t) {
-                        let e, n, r, i, o, l, a, c, f, v, $, w = `${Gd}px`,
-                            _ = `${Gd}px`;
+                    function Zd(t) {
+                        let e, n, r, i, o, l, a, c, f, v, $, w = `${Qd}px`,
+                            _ = `${Qd}px`;
                         return {
                             c() {
-                                e = h("div"), n = h("button"), r = p("svg"), i = p("path"), o = p("polyline"), a = m(), c = h("div"), f = g(t[1]), y(i, "stroke", "none"), y(i, "d", "M0 0h24v24H0z"), y(i, "fill", "none"), y(o, "points", l = "2 12 12 22 22 12"), y(o, "class", "svelte-2uqume"), S(o, "rotate-polyline", !t[0]), y(r, "xmlns", "http://www.w3.org/2000/svg"), y(r, "class", "icon-tabler icon-tabler-chevron-down svelte-2uqume"), y(r, "width", Gd), y(r, "height", Gd), y(r, "viewBox", "0 0 24 24"), y(r, "stroke-width", "4"), y(r, "stroke", "currentColor"), y(r, "fill", "none"), y(r, "stroke-linecap", "round"), y(r, "stroke-linejoin", "round"), k(n, "border", "none"), k(n, "width", w), k(n, "height", _), k(n, "padding", "0"), k(n, "color", "var(--black)"), k(n, "background-color", "white"), y(c, "class", "pdpilot-bold"), y(e, "class", "toggle-and-title svelte-2uqume")
+                                e = h("div"), n = h("button"), r = p("svg"), i = p("path"), o = p("polyline"), a = m(), c = h("div"), f = g(t[1]), y(i, "stroke", "none"), y(i, "d", "M0 0h24v24H0z"), y(i, "fill", "none"), y(o, "points", l = "2 12 12 22 22 12"), y(o, "class", "svelte-2uqume"), S(o, "rotate-polyline", !t[0]), y(r, "xmlns", "http://www.w3.org/2000/svg"), y(r, "class", "icon-tabler icon-tabler-chevron-down svelte-2uqume"), y(r, "width", Qd), y(r, "height", Qd), y(r, "viewBox", "0 0 24 24"), y(r, "stroke-width", "4"), y(r, "stroke", "currentColor"), y(r, "fill", "none"), y(r, "stroke-linecap", "round"), y(r, "stroke-linejoin", "round"), k(n, "border", "none"), k(n, "width", w), k(n, "height", _), k(n, "padding", "0"), k(n, "color", "var(--black)"), k(n, "background-color", "white"), y(c, "class", "pdpilot-bold"), y(e, "class", "toggle-and-title svelte-2uqume")
                             },
                             m(l, d) {
                                 u(l, e, d), s(e, n), s(n, r), s(r, i), s(r, o), s(e, a), s(e, c), s(c, f), v || ($ = b(n, "click", t[2]), v = !0)
                             },
                             p(t, [e]) {
                                 1 & e && S(o, "rotate-polyline", !t[0]), 2 & e && x(f, t[1])
                             },
                             i: z,
                             o: z,
                             d(t) {
                                 t && d(e), v = !1, $()
                             }
                         }
                     }
-                    const Gd = 8;
+                    const Qd = 8;
 
-                    function Jd(t, e, n) {
+                    function tf(t, e, n) {
                         let {
                             expanded: r = !1
                         } = e, {
                             title: i
                         } = e;
                         return t.$$set = t => {
                             "expanded" in t && n(0, r = t.expanded), "title" in t && n(1, i = t.title)
                         }, [r, i, () => n(0, r = !r)]
                     }
-                    const Zd = class extends xt {
+                    const ef = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, Jd, Yd, D, {
+                            super(), $t(this, t, tf, Zd, D, {
                                 expanded: 0,
                                 title: 1
-                            }, Ud)
+                            }, Jd)
                         }
                     };
 
-                    function Qd(t) {
+                    function nf(t) {
                         c(t, "svelte-1mkvanr", ".controls-container.svelte-1mkvanr.svelte-1mkvanr{height:100%;flex:0 0 200px;min-width:200px;max-width:200px;padding:0.25em;border-right:1px solid var(--gray-1);display:flex;flex-direction:column;gap:0.5em}.feature-selector-wrapper-outer.svelte-1mkvanr.svelte-1mkvanr{flex:0 1 auto;min-height:0;display:flex;flex-direction:column}.feature-selector-wrapper-inner.svelte-1mkvanr.svelte-1mkvanr{flex:1;min-height:0}.filter-header.svelte-1mkvanr+.filter-content.svelte-1mkvanr{margin-top:0.25em}.filter-content.svelte-1mkvanr.svelte-1mkvanr{margin-left:0.75em}")
                     }
 
-                    function tf(t) {
+                    function rf(t) {
                         let e, n, r, i, o, l, a, c, f, p, g, v, $, w, x, _, M, L, A, P, z, T, N;
 
                         function C(e) {
                             t[11](e)
                         }
                         let O = {
                             title: "Type"
                         };
 
                         function D(e) {
                             t[13](e)
                         }
-                        void 0 !== t[2] && (O.expanded = t[2]), c = new Zd({
+                        void 0 !== t[2] && (O.expanded = t[2]), c = new ef({
                             props: O
-                        }), K.push((() => mt(c, "expanded", C))), v = new Xd({
+                        }), K.push((() => mt(c, "expanded", C))), v = new Gd({
                             props: {}
                         }), t[12](v), v.$on("changeKindFilters", t[5]);
                         let B = {
                             title: "Name"
                         };
-                        void 0 !== t[3] && (B.expanded = t[3]), _ = new Zd({
+                        void 0 !== t[3] && (B.expanded = t[3]), _ = new ef({
                             props: B
                         }), K.push((() => mt(_, "expanded", D)));
                         let j = {
                             enabledFeatures: t[4],
                             idPrefix: "pdpilot-one"
                         };
-                        return P = new qd({
+                        return P = new Kd({
                             props: j
                         }), t[14](P), P.$on("changeNameFilters", t[6]), {
                             c() {
                                 e = h("div"), n = h("div"), n.textContent = "Feature Filters", r = m(), i = h("button"), i.textContent = "Clear Filters", o = m(), l = h("div"), a = h("div"), vt(c.$$.fragment), p = m(), g = h("div"), vt(v.$$.fragment), $ = m(), w = h("div"), x = h("div"), vt(_.$$.fragment), L = m(), A = h("div"), vt(P.$$.fragment), y(n, "class", "pdpilot-bold"), k(i, "align-self", "start"), y(a, "class", "filter-header svelte-1mkvanr"), y(g, "class", "filter-content svelte-1mkvanr"), S(g, "pdp-hide", !t[2]), y(x, "class", "filter-header svelte-1mkvanr"), y(A, "class", "filter-content feature-selector-wrapper-inner svelte-1mkvanr"), S(A, "pdp-hide", !t[3]), y(w, "class", "filter-container feature-selector-wrapper-outer svelte-1mkvanr"), y(e, "class", "controls-container svelte-1mkvanr")
                             },
                             m(d, f) {
                                 u(d, e, f), s(e, n), s(e, r), s(e, i), s(e, o), s(e, l), s(l, a), bt(c, a, null), s(l, p), s(l, g), bt(v, g, null), s(e, $), s(e, w), s(w, x), bt(_, x, null), s(w, L), s(w, A), bt(P, A, null), z = !0, T || (N = b(i, "click", t[7]), T = !0)
@@ -11278,15 +11331,15 @@
                             },
                             d(n) {
                                 n && d(e), yt(c), t[12](null), yt(v), yt(_), t[14](null), yt(P), T = !1, N()
                             }
                         }
                     }
 
-                    function ef(t, e, n) {
+                    function of(t, e, n) {
                         let r, i, o;
                         j(t, pr, (t => n(9, i = t))), j(t, Yn, (t => n(10, o = t)));
                         const l = F();
                         let a, s, c, u = !0,
                             d = !0;
                         return t.$$.update = () => {
                             1792 & t.$$.dirty && n(4, r = o.filter((t => {
@@ -11309,29 +11362,29 @@
                             d = t, n(3, d)
                         }, function(t) {
                             K[t ? "unshift" : "push"]((() => {
                                 s = t, n(1, s)
                             }))
                         }]
                     }
-                    const nf = class extends xt {
+                    const lf = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, ef, tf, D, {}, Qd)
+                            super(), $t(this, t, of, rf, D, {}, nf)
                         }
                     };
 
-                    function rf(t) {
+                    function af(t) {
                         return 0 === t.length || 1 === t[0].num_features
                     }
 
-                    function of(t) {
+                    function sf(t) {
                         c(t, "svelte-19snser", ".tooltip-container.svelte-19snser{position:relative;display:flex;align-items:center}.tooltip-content.svelte-19snser{position:absolute;padding:5px;border-radius:5px;max-width:30em;border:1px solid black;color:black;background-color:white;z-index:1;pointer-events:none}")
                     }
 
-                    function lf(t) {
+                    function cf(t) {
                         let e, n, r, i, o, l, a;
                         return {
                             c() {
                                 e = p("svg"), n = p("path"), r = p("circle"), i = p("line"), o = p("path"), y(n, "stroke", "none"), y(n, "d", "M0 0h24v24H0z"), y(r, "cx", "12"), y(r, "cy", "12"), y(r, "r", "9"), y(i, "x1", "12"), y(i, "y1", "17"), y(i, "x2", "12"), y(i, "y2", "17.01"), y(o, "d", "M12 13.5a1.5 1.5 0 0 1 1 -1.5a2.6 2.6 0 1 0 -3 -4"), y(e, "xmlns", "http://www.w3.org/2000/svg"), y(e, "class", "pdpilot-icon icon-tabler icon-tabler-help"), y(e, "width", "24"), y(e, "height", "24"), y(e, "viewBox", "0 0 24 24"), y(e, "stroke-width", "2"), y(e, "stroke", "currentColor"), y(e, "fill", "none"), y(e, "stroke-linecap", "round"), y(e, "stroke-linejoin", "round")
                             },
                             m(c, d) {
                                 u(c, e, d), s(e, n), s(e, r), s(e, i), s(e, o), l || (a = [b(e, "mouseenter", t[15]), b(e, "mouseleave", t[16])], l = !0)
@@ -11339,15 +11392,15 @@
                             p: z,
                             d(t) {
                                 t && d(e), l = !1, C(a)
                             }
                         }
                     }
 
-                    function af(t) {
+                    function uf(t) {
                         let e, n, r, i, o, l, a;
                         return {
                             c() {
                                 e = p("svg"), n = p("path"), r = p("circle"), i = p("line"), o = p("line"), y(n, "stroke", "none"), y(n, "d", "M0 0h24v24H0z"), y(n, "fill", "none"), y(r, "cx", "12"), y(r, "cy", "12"), y(r, "r", "9"), y(i, "x1", "12"), y(i, "y1", "8"), y(i, "x2", "12"), y(i, "y2", "12"), y(o, "x1", "12"), y(o, "y1", "16"), y(o, "x2", "12.01"), y(o, "y2", "16"), y(e, "xmlns", "http://www.w3.org/2000/svg"), y(e, "class", "pdpilot-icon icon-tabler icon-tabler-alert-circle"), y(e, "width", "24"), y(e, "height", "24"), y(e, "viewBox", "0 0 24 24"), y(e, "stroke-width", "2"), y(e, "stroke", "currentColor"), y(e, "fill", "none"), y(e, "stroke-linecap", "round"), y(e, "stroke-linejoin", "round")
                             },
                             m(c, d) {
                                 u(c, e, d), s(e, n), s(e, r), s(e, i), s(e, o), l || (a = [b(e, "mouseenter", t[13]), b(e, "mouseleave", t[14])], l = !0)
@@ -11355,15 +11408,15 @@
                             p: z,
                             d(t) {
                                 t && d(e), l = !1, C(a)
                             }
                         }
                     }
 
-                    function sf(t) {
+                    function df(t) {
                         let e, n, r = `${t[5]}\n      ${t[6]}\n      ${t[7]}\n      ${t[8]}`;
                         const i = t[12].default,
                             o = function(t, e, n, r) {
                                 if (t) {
                                     const r = E(t, e, n, null);
                                     return t[0](r)
                                 }
@@ -11401,32 +11454,32 @@
                             },
                             d(t) {
                                 t && d(e), o && o.d(t)
                             }
                         }
                     }
 
-                    function cf(t) {
+                    function ff(t) {
                         let e, n, r;
 
                         function i(t, e) {
-                            return "alert" === t[0] ? af : lf
+                            return "alert" === t[0] ? uf : cf
                         }
                         let o = i(t),
                             l = o(t),
-                            a = t[10] && sf(t);
+                            a = t[10] && df(t);
                         return {
                             c() {
                                 e = h("div"), l.c(), n = m(), a && a.c(), y(e, "class", "tooltip-container svelte-19snser")
                             },
                             m(t, i) {
                                 u(t, e, i), l.m(e, null), s(e, n), a && a.m(e, null), r = !0
                             },
                             p(t, [r]) {
-                                o === (o = i(t)) && l ? l.p(t, r) : (l.d(1), l = o(t), l && (l.c(), l.m(e, n))), t[10] ? a ? (a.p(t, r), 1024 & r && ut(a, 1)) : (a = sf(t), a.c(), ut(a, 1), a.m(e, null)) : a && (st(), dt(a, 1, 1, (() => {
+                                o === (o = i(t)) && l ? l.p(t, r) : (l.d(1), l = o(t), l && (l.c(), l.m(e, n))), t[10] ? a ? (a.p(t, r), 1024 & r && ut(a, 1)) : (a = df(t), a.c(), ut(a, 1), a.m(e, null)) : a && (st(), dt(a, 1, 1, (() => {
                                     a = null
                                 })), ct())
                             },
                             i(t) {
                                 r || (ut(a), r = !0)
                             },
                             o(t) {
@@ -11434,15 +11487,15 @@
                             },
                             d(t) {
                                 t && d(e), l.d(), a && a.d()
                             }
                         }
                     }
 
-                    function uf(t, e, n) {
+                    function hf(t, e, n) {
                         let {
                             $$slots: r = {},
                             $$scope: i
                         } = e, {
                             kind: o = "help"
                         } = e, {
                             top: l = "auto"
@@ -11463,51 +11516,51 @@
                         } = e, {
                             width: p = "30em"
                         } = e, g = !1;
                         return t.$$set = t => {
                             "kind" in t && n(0, o = t.kind), "top" in t && n(1, l = t.top), "left" in t && n(2, a = t.left), "right" in t && n(3, s = t.right), "bottom" in t && n(4, c = t.bottom), "marginTop" in t && n(5, u = t.marginTop), "marginRight" in t && n(6, d = t.marginRight), "marginBottom" in t && n(7, f = t.marginBottom), "marginLeft" in t && n(8, h = t.marginLeft), "width" in t && n(9, p = t.width), "$$scope" in t && n(11, i = t.$$scope)
                         }, [o, l, a, s, c, u, d, f, h, p, g, i, r, () => n(10, g = !0), () => n(10, g = !1), () => n(10, g = !0), () => n(10, g = !1)]
                     }
-                    const df = class extends xt {
+                    const pf = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, uf, cf, D, {
+                            super(), $t(this, t, hf, ff, D, {
                                 kind: 0,
                                 top: 1,
                                 left: 2,
                                 right: 3,
                                 bottom: 4,
                                 marginTop: 5,
                                 marginRight: 6,
                                 marginBottom: 7,
                                 marginLeft: 8,
                                 width: 9
-                            }, of)
+                            }, sf)
                         }
                     };
 
-                    function ff(t) {
+                    function gf(t) {
                         c(t, "svelte-alv95s", ".group-container.svelte-alv95s.svelte-alv95s{height:100%;width:100%;display:flex;flex-direction:column;min-height:2em}.pdp-grid-container.svelte-alv95s.svelte-alv95s{flex:1;min-height:0;padding:1px}.pdpilot-no-plots-container.svelte-alv95s.svelte-alv95s{width:100%;height:100%;display:flex;align-items:center;justify-content:center}.pdpilot-no-plots-message.svelte-alv95s.svelte-alv95s{max-width:28em}.pdp-grid.svelte-alv95s.svelte-alv95s{height:100%;display:grid}.group-header.svelte-alv95s.svelte-alv95s{height:2em;display:flex;align-items:center;gap:1em;border-bottom:1px solid var(--gray-1);padding-left:0.5em;padding-right:0.5em}.two-way-color-container.svelte-alv95s.svelte-alv95s{flex:1;margin-left:auto;display:flex;align-items:center}.two-way-color-legend.svelte-alv95s.svelte-alv95s{flex:1}.page-change.svelte-alv95s.svelte-alv95s{display:flex;align-items:center}.current-page-number.svelte-alv95s.svelte-alv95s{width:2em;text-align:center}.label-and-input.svelte-alv95s.svelte-alv95s{display:flex;align-items:center;gap:0.25em}.pdp-grid-element.svelte-alv95s.svelte-alv95s{position:relative}.pdp-grid-element.svelte-alv95s:hover .expand-pdp-button.svelte-alv95s{display:block}.expand-pdp-button.svelte-alv95s.svelte-alv95s{position:absolute;display:none;bottom:2px;left:2px}.dont-shrink.svelte-alv95s.svelte-alv95s{flex:0 0 auto}.dont-show.svelte-alv95s.svelte-alv95s{display:none}ul.svelte-alv95s.svelte-alv95s{list-style:none}li.svelte-alv95s+li.svelte-alv95s{margin-top:0.5em}")
                     }
 
-                    function hf(t, e, n) {
+                    function mf(t, e, n) {
                         const r = t.slice();
                         return r[51] = e[n], r
                     }
 
-                    function pf(t, e, n) {
+                    function vf(t, e, n) {
                         const r = t.slice();
                         return r[54] = e[n].value, r[55] = e[n].title, r
                     }
 
-                    function gf(t, e, n) {
+                    function bf(t, e, n) {
                         const r = t.slice();
                         return r[58] = e[n], r
                     }
 
-                    function mf(t) {
+                    function yf(t) {
                         let e, n, r, i = t[58].name + "";
                         return {
                             c() {
                                 e = h("option"), n = g(i), e.__value = r = t[58], _(e, e.__value)
                             },
                             m(t, r) {
                                 u(t, e, r), s(e, n)
@@ -11517,49 +11570,49 @@
                             },
                             d(t) {
                                 t && d(e)
                             }
                         }
                     }
 
-                    function vf(t) {
+                    function $f(t) {
                         let e;
                         return {
                             c() {
                                 e = h("ul"), e.innerHTML = '<li class="svelte-alv95s"><span class="pdpilot-bold">Interaction:</span> Plots for feature\n                pairs with more interaction are ranked higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Variance:</span> Plots that have more\n                variation in their average predictions are ranked higher.</li>', y(e, "class", "svelte-alv95s")
                             },
                             m(t, n) {
                                 u(t, e, n)
                             },
                             d(t) {
                                 t && d(e)
                             }
                         }
                     }
 
-                    function bf(t) {
+                    function wf(t) {
                         let e;
                         return {
                             c() {
-                                e = h("ul"), e.innerHTML = '<li class="svelte-alv95s"><span class="pdpilot-bold">Variance:</span> Plots that have more\n                variance in their ICE lines are ranked higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Cluster difference:</span> Plots that\n                have ICE clusters farther from the partial dependence line are ranked\n                higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Highlighted similarity:</span> Plots where\n                the highlighted lines are closer together and farther from the partial\n                dependence line are ranked higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Highlighted distribution:</span> Plots\n                for features whose distributions of highlighted instances are more\n                different from the overall distributions are ranked higher.</li>', y(e, "class", "svelte-alv95s")
+                                e = h("ul"), e.innerHTML = '<li class="svelte-alv95s"><span class="pdpilot-bold">Importance:</span> Plots that have more\n                variance in their ICE lines are ranked higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Cluster difference:</span> Plots that\n                have ICE clusters farther from the partial dependence line are ranked\n                higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Highlighted line similarity:</span> Plots\n                where the highlighted lines are closer together and farther from\n                the partial dependence line are ranked higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Highlighted histogram difference:</span> Plots for features whose distributions of highlighted instances\n                are more different from the overall distributions are ranked higher.</li>', y(e, "class", "svelte-alv95s")
                             },
                             m(t, n) {
                                 u(t, e, n)
                             },
                             d(t) {
                                 t && d(e)
                             }
                         }
                     }
 
-                    function yf(t) {
+                    function xf(t) {
                         let e;
 
                         function n(t, e) {
-                            return 1 === t[17] ? bf : vf
+                            return 1 === t[17] ? wf : $f
                         }
                         let r = n(t),
                             i = r(t);
                         return {
                             c() {
                                 e = h("div"), i.c()
                             },
@@ -11571,15 +11624,15 @@
                             },
                             d(t) {
                                 t && d(e), i.d()
                             }
                         }
                     }
 
-                    function $f(t) {
+                    function _f(t) {
                         let e, n, r, i, o, l, a, c;
                         return {
                             c() {
                                 e = h("button"), n = p("svg"), r = p("path"), i = p("path"), o = p("path"), y(r, "stroke", "none"), y(r, "d", "M0 0h24v24H0z"), y(r, "fill", "none"), y(i, "d", "M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4"), y(o, "d", "M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4"), y(n, "xmlns", "http://www.w3.org/2000/svg"), y(n, "class", "pdpilot-icon icon-tabler icon-tabler-refresh"), y(n, "width", "24"), y(n, "height", "24"), y(n, "viewBox", "0 0 24 24"), y(n, "stroke-width", "2"), y(n, "stroke", "currentColor"), y(n, "fill", "none"), y(n, "stroke-linecap", "round"), y(n, "stroke-linejoin", "round"), y(e, "title", "Update sorting"), e.disabled = l = !t[13]
                             },
                             m(l, d) {
                                 u(l, e, d), s(e, n), s(n, r), s(n, i), s(n, o), a || (c = b(e, "click", t[33]), a = !0)
@@ -11589,18 +11642,18 @@
                             },
                             d(t) {
                                 t && d(e), a = !1, c()
                             }
                         }
                     }
 
-                    function wf(t) {
+                    function kf(t) {
                         let e, n, r, i, o, l = ft(t[21]),
                             a = [];
-                        for (let e = 0; e < l.length; e += 1) a[e] = xf(pf(t, l, e));
+                        for (let e = 0; e < l.length; e += 1) a[e] = Mf(vf(t, l, e));
                         return {
                             c() {
                                 e = h("label"), n = g("Plot\n        "), r = h("select");
                                 for (let t = 0; t < a.length; t += 1) a[t].c();
                                 void 0 === t[9] && Q((() => t[34].call(r))), y(e, "class", "label-and-input dont-shrink svelte-alv95s")
                             },
                             m(l, c) {
@@ -11608,29 +11661,29 @@
                                 for (let t = 0; t < a.length; t += 1) a[t] && a[t].m(r, null);
                                 M(r, t[9], !0), i || (o = b(r, "change", t[34]), i = !0)
                             },
                             p(t, e) {
                                 if (2097152 & e[0]) {
                                     let n;
                                     for (l = ft(t[21]), n = 0; n < l.length; n += 1) {
-                                        const i = pf(t, l, n);
-                                        a[n] ? a[n].p(i, e) : (a[n] = xf(i), a[n].c(), a[n].m(r, null))
+                                        const i = vf(t, l, n);
+                                        a[n] ? a[n].p(i, e) : (a[n] = Mf(i), a[n].c(), a[n].m(r, null))
                                     }
                                     for (; n < a.length; n += 1) a[n].d(1);
                                     a.length = l.length
                                 }
                                 2097664 & e[0] && M(r, t[9])
                             },
                             d(t) {
                                 t && d(e), f(a, t), i = !1, o()
                             }
                         }
                     }
 
-                    function xf(t) {
+                    function Mf(t) {
                         let e, n, r, i = t[55] + "";
                         return {
                             c() {
                                 e = h("option"), n = g(i), e.__value = r = t[54], _(e, e.__value)
                             },
                             m(t, r) {
                                 u(t, e, r), s(e, n)
@@ -11638,34 +11691,34 @@
                             p: z,
                             d(t) {
                                 t && d(e)
                             }
                         }
                     }
 
-                    function _f(t) {
+                    function Lf(t) {
                         let e, n, r, i, o, l, a, c, f, p, v;
-                        return c = new df({
+                        return c = new pf({
                             props: {
                                 kind: "help",
                                 right: "0",
                                 top: "0",
                                 marginRight: "1em",
                                 marginTop: "1.5em",
                                 width: "30em",
                                 $$slots: {
-                                    default: [Lf]
+                                    default: [Sf]
                                 },
                                 $$scope: {
                                     ctx: t
                                 }
                             }
                         }), {
                             c() {
-                                e = h("div"), n = h("label"), r = g("Color\n            "), i = h("select"), o = h("option"), o.textContent = "interactions", l = h("option"), l.textContent = "predictions", a = m(), vt(c.$$.fragment), o.__value = "interactions", _(o, o.__value), l.__value = "predictions", _(l, l.__value), void 0 === t[10] && Q((() => t[36].call(i))), y(n, "class", "label-and-input svelte-alv95s"), y(e, "class", "label-and-input dont-shrink svelte-alv95s")
+                                e = h("div"), n = h("label"), r = g("Color\n            "), i = h("select"), o = h("option"), o.textContent = "Predictions", l = h("option"), l.textContent = "Interactions", a = m(), vt(c.$$.fragment), o.__value = "predictions", _(o, o.__value), l.__value = "interactions", _(l, l.__value), void 0 === t[10] && Q((() => t[36].call(i))), y(n, "class", "label-and-input svelte-alv95s"), y(e, "class", "label-and-input dont-shrink svelte-alv95s")
                             },
                             m(d, h) {
                                 u(d, e, h), s(e, n), s(n, r), s(n, i), s(i, o), s(i, l), M(i, t[10], !0), s(e, a), bt(c, e, null), f = !0, p || (v = b(i, "change", t[36]), p = !0)
                             },
                             p(t, e) {
                                 1024 & e[0] && M(i, t[10]);
                                 const n = {};
@@ -11682,15 +11735,15 @@
                             },
                             d(t) {
                                 t && d(e), yt(c), p = !1, v()
                             }
                         }
                     }
 
-                    function kf(t) {
+                    function Af(t) {
                         let e;
                         return {
                             c() {
                                 e = g("This color scale is for a standard two-way PDP. The color of a\n                cell represents the model's average prediction when setting the\n                instances to have the given values for pair of features.")
                             },
                             m(t, n) {
                                 u(t, e, n)
@@ -11698,15 +11751,15 @@
                             p: z,
                             d(t) {
                                 t && d(e)
                             }
                         }
                     }
 
-                    function Mf(t) {
+                    function Pf(t) {
                         let e, n, r, i, o;
                         return {
                             c() {
                                 e = g("This color scale shows the difference between the value in a\n                two-way PDP and the expected value if there was no interaction\n                between the pair of features. It indicates whether the\n                interaction between the two features makes the model's average\n                prediction for the given values "), n = h("span"), n.textContent = "lower", r = g("\n                or\n                "), i = h("span"), i.textContent = "higher", o = g(". The units are the same as your target variable."), k(n, "background", t[19].interpolator()(.1)), k(n, "border-radius", "4px"), k(n, "padding", "0.125em 0.25em"), k(n, "color", "white"), k(i, "background", t[19].interpolator()(.9)), k(i, "border-radius", "4px"), k(i, "padding", "0.125em 0.25em"), k(i, "color", "white")
                             },
                             m(t, l) {
                                 u(t, e, l), u(t, n, l), u(t, r, l), u(t, i, l), u(t, o, l)
@@ -11716,19 +11769,19 @@
                             },
                             d(t) {
                                 t && (d(e), d(n), d(r), d(i), d(o))
                             }
                         }
                     }
 
-                    function Lf(t) {
+                    function Sf(t) {
                         let e;
 
                         function n(t, e) {
-                            return "interactions" === t[10] ? Mf : kf
+                            return "interactions" === t[10] ? Pf : Af
                         }
                         let r = n(t),
                             i = r(t);
                         return {
                             c() {
                                 e = h("div"), i.c()
                             },
@@ -11740,39 +11793,39 @@
                             },
                             d(t) {
                                 t && d(e), i.d()
                             }
                         }
                     }
 
-                    function Af(t) {
+                    function zf(t) {
                         let e, n, r = [],
                             i = new Map,
                             o = `repeat(${t[8]}, minmax(0,${t[11]}px))`,
                             l = `repeat(${t[7]}, minmax(0,${t[12]}px))`,
                             a = ft(t[16]);
                         const s = t => t[51].id;
                         for (let e = 0; e < a.length; e += 1) {
-                            let n = hf(t, a, e),
+                            let n = mf(t, a, e),
                                 o = s(n);
-                            i.set(o, r[e] = Sf(o, n))
+                            i.set(o, r[e] = Nf(o, n))
                         }
                         return {
                             c() {
                                 e = h("div");
                                 for (let t = 0; t < r.length; t += 1) r[t].c();
                                 y(e, "class", "pdp-grid svelte-alv95s"), k(e, "grid-template-columns", o), k(e, "grid-template-rows", l)
                             },
                             m(t, i) {
                                 u(t, e, i);
                                 for (let t = 0; t < r.length; t += 1) r[t] && r[t].m(e, null);
                                 n = !0
                             },
                             p(t, n) {
-                                16997888 & n[0] && (a = ft(t[16]), st(), r = gt(r, n, s, 1, t, a, i, e, pt, Sf, null, hf), ct()), 2304 & n[0] && o !== (o = `repeat(${t[8]}, minmax(0,${t[11]}px))`) && k(e, "grid-template-columns", o), 4224 & n[0] && l !== (l = `repeat(${t[7]}, minmax(0,${t[12]}px))`) && k(e, "grid-template-rows", l)
+                                16997888 & n[0] && (a = ft(t[16]), st(), r = gt(r, n, s, 1, t, a, i, e, pt, Nf, null, mf), ct()), 2304 & n[0] && o !== (o = `repeat(${t[8]}, minmax(0,${t[11]}px))`) && k(e, "grid-template-columns", o), 4224 & n[0] && l !== (l = `repeat(${t[7]}, minmax(0,${t[12]}px))`) && k(e, "grid-template-rows", l)
                             },
                             i(t) {
                                 if (!n) {
                                     for (let t = 0; t < a.length; t += 1) ut(r[t]);
                                     n = !0
                                 }
                             },
@@ -11783,15 +11836,15 @@
                             d(t) {
                                 t && d(e);
                                 for (let t = 0; t < r.length; t += 1) r[t].d()
                             }
                         }
                     }
 
-                    function Pf(t) {
+                    function Tf(t) {
                         let e, n, r;
                         return {
                             c() {
                                 e = h("div"), n = h("div"), r = g(t[2]), y(n, "class", "pdpilot-no-plots-message svelte-alv95s"), y(e, "class", "pdpilot-no-plots-container svelte-alv95s")
                             },
                             m(t, i) {
                                 u(t, e, i), s(e, n), s(n, r)
@@ -11803,22 +11856,22 @@
                             o: z,
                             d(t) {
                                 t && d(e)
                             }
                         }
                     }
 
-                    function Sf(t, e) {
+                    function Nf(t, e) {
                         let n, r, i, o, l, a, c, f, p = `${e[11]}px`,
                             g = `${e[12]}px`;
 
                         function v() {
                             return e[38](e[51])
                         }
-                        return r = new hu({
+                        return r = new mu({
                             props: {
                                 pd: e[51],
                                 width: e[11],
                                 height: e[12],
                                 scaleLocally: e[14],
                                 colorShows: e[10],
                                 showMarginalDistribution: !0,
@@ -11853,47 +11906,47 @@
                             },
                             d(t) {
                                 t && d(n), yt(r), c = !1, f()
                             }
                         }
                     }
 
-                    function zf(t) {
+                    function Cf(t) {
                         let e, n, r, i, o, l, a, c, v, $, w, _, k, L, P, z, T, N, O, D, B, j, E, I, R, V, H, q, F, W, K, X, U, Y, G, J, Z, tt, et, nt, rt, it, ot, lt, at, ht, pt, gt, mt = ft(t[1]),
                             $t = [];
-                        for (let e = 0; e < mt.length; e += 1) $t[e] = mf(gf(t, mt, e));
-                        q = new df({
+                        for (let e = 0; e < mt.length; e += 1) $t[e] = yf(bf(t, mt, e));
+                        q = new pf({
                             props: {
                                 kind: "help",
                                 left: "0",
                                 top: "0",
                                 marginRight: "1em",
                                 marginTop: "1.5em",
-                                width: "30em",
+                                width: "25em",
                                 $$slots: {
-                                    default: [yf]
+                                    default: [xf]
                                 },
                                 $$scope: {
                                     ctx: t
                                 }
                             }
                         });
-                        let wt = 1 === t[17] && t[5].forBrushing && $f(t),
-                            xt = 1 === t[17] && wf(t),
-                            _t = 2 === t[17] && _f(t);
+                        let wt = 1 === t[17] && t[5].forBrushing && _f(t),
+                            xt = 1 === t[17] && kf(t),
+                            _t = 2 === t[17] && Lf(t);
                         et = new wc({
                             props: {
                                 width: t[18],
-                                height: Tf,
+                                height: Of,
                                 color: "interactions" === t[10] ? t[19] : t[20],
                                 marginLeft: 15,
                                 marginRight: 15
                             }
                         });
-                        const kt = [Pf, Af],
+                        const kt = [Tf, zf],
                             Mt = [];
 
                         function Lt(t, e) {
                             return 0 === t[16].length ? 0 : 1
                         }
                         return ot = Lt(t), lt = Mt[ot] = kt[ot](t), {
                             c() {
@@ -11906,26 +11959,26 @@
                                 for (let t = 0; t < $t.length; t += 1) $t[t] && $t[t].m(V, null);
                                 M(V, t[5], !0), s(E, H), bt(q, E, null), s(n, F), wt && wt.m(n, null), s(n, W), xt && xt.m(n, null), s(n, K), s(n, X), s(X, U), U.checked = t[14], s(X, Y), s(n, G), s(n, J), _t && _t.m(J, null), s(J, Z), s(J, tt), bt(et, tt, null), nt = A.observe(tt, t[37].bind(tt)), s(e, rt), s(e, it), Mt[ot].m(it, null), at = A.observe(it, t[39].bind(it)), ht = !0, pt || (gt = [b(i, "click", t[30]), b(P, "click", t[31]), b(V, "change", t[32]), b(U, "change", t[35])], pt = !0)
                             },
                             p(t, e) {
                                 if ((!ht || 64 & e[0] && $ !== ($ = t[6] <= 1)) && (i.disabled = $), (!ht || 64 & e[0]) && x(k, t[6]), (!ht || 32832 & e[0] && B !== (B = t[6] >= t[15])) && (P.disabled = B), 2 & e[0]) {
                                     let n;
                                     for (mt = ft(t[1]), n = 0; n < mt.length; n += 1) {
-                                        const r = gf(t, mt, n);
-                                        $t[n] ? $t[n].p(r, e) : ($t[n] = mf(r), $t[n].c(), $t[n].m(V, null))
+                                        const r = bf(t, mt, n);
+                                        $t[n] ? $t[n].p(r, e) : ($t[n] = yf(r), $t[n].c(), $t[n].m(V, null))
                                     }
                                     for (; n < $t.length; n += 1) $t[n].d(1);
                                     $t.length = mt.length
                                 }
                                 34 & e[0] && M(V, t[5]);
                                 const r = {};
                                 131072 & e[0] | 1073741824 & e[1] && (r.$$scope = {
                                     dirty: e,
                                     ctx: t
-                                }), q.$set(r), 1 === t[17] && t[5].forBrushing ? wt ? wt.p(t, e) : (wt = $f(t), wt.c(), wt.m(n, W)) : wt && (wt.d(1), wt = null), 1 === t[17] ? xt ? xt.p(t, e) : (xt = wf(t), xt.c(), xt.m(n, K)) : xt && (xt.d(1), xt = null), 16384 & e[0] && (U.checked = t[14]), 2 === t[17] ? _t ? (_t.p(t, e), 131072 & e[0] && ut(_t, 1)) : (_t = _f(t), _t.c(), ut(_t, 1), _t.m(J, Z)) : _t && (st(), dt(_t, 1, 1, (() => {
+                                }), q.$set(r), 1 === t[17] && t[5].forBrushing ? wt ? wt.p(t, e) : (wt = _f(t), wt.c(), wt.m(n, W)) : wt && (wt.d(1), wt = null), 1 === t[17] ? xt ? xt.p(t, e) : (xt = kf(t), xt.c(), xt.m(n, K)) : xt && (xt.d(1), xt = null), 16384 & e[0] && (U.checked = t[14]), 2 === t[17] ? _t ? (_t.p(t, e), 131072 & e[0] && ut(_t, 1)) : (_t = Lf(t), _t.c(), ut(_t, 1), _t.m(J, Z)) : _t && (st(), dt(_t, 1, 1, (() => {
                                     _t = null
                                 })), ct());
                                 const o = {};
                                 262144 & e[0] && (o.width = t[18]), 1573888 & e[0] && (o.color = "interactions" === t[10] ? t[19] : t[20]), et.$set(o), (!ht || 147456 & e[0]) && S(tt, "dont-show", 1 === t[17] || t[14]);
                                 let l = ot;
                                 ot = Lt(t), ot === l ? Mt[ot].p(t, e) : (st(), dt(Mt[l], 1, 1, (() => {
                                     Mt[l] = null
@@ -11938,17 +11991,17 @@
                                 dt(q.$$.fragment, t), dt(_t), dt(et.$$.fragment, t), dt(lt), ht = !1
                             },
                             d(t) {
                                 t && d(e), f($t, t), yt(q), wt && wt.d(), xt && xt.d(), _t && _t.d(), yt(et), nt(), Mt[ot].d(), at(), pt = !1, C(gt)
                             }
                         }
                     }
-                    const Tf = 24;
+                    const Of = 24;
 
-                    function Nf(t, e, n) {
+                    function Df(t, e, n) {
                         let r, i, o, a, s, c, u, d, f, h, p, g, m, v, b, y, $, w, x, _, k, M;
                         j(t, hr, (t => n(40, h = t))), j(t, $r, (t => n(41, p = t))), j(t, yr, (t => n(42, g = t))), j(t, wr, (t => n(43, m = t))), j(t, br, (t => n(44, v = t))), j(t, vr, (t => n(45, b = t))), j(t, _r, (t => n(29, y = t))), j(t, er, (t => n(46, $ = t))), j(t, Gn, (t => n(47, w = t))), j(t, Lr, (t => n(48, x = t))), j(t, ur, (t => n(49, _ = t))), j(t, Pr, (t => n(19, k = t))), j(t, Ar, (t => n(20, M = t)));
                         let A, {
                                 data: P
                             } = e,
                             {
                                 sortingOptions: S
@@ -11963,15 +12016,15 @@
                             value: "centered-lines",
                             title: "Centered"
                         }, {
                             value: "cluster-centers",
                             title: "Clusters"
                         }];
                         let N, C, O, D, B = "lines",
-                            E = "interactions",
+                            E = "predictions",
                             R = !1,
                             V = S[0];
 
                         function H(t) {
                             n(13, R = !1), n(25, A = V.sort(t, {
                                 highlightedIndices: _,
                                 highlightedDistributions: x,
@@ -11988,15 +12041,15 @@
 
                         function K(t) {
                             I(vr, b = t.x_feature, b), I(br, v = 2 === t.num_features ? t.y_feature : "", v), I(wr, m = W, m), 1 === t.num_features && (I(yr, g = "cluster-centers" === B ? "cluster-lines" : B, g), I($r, p = "cluster-centers" === B ? "cluster-descriptions" : "scatterplot", p)), I(hr, h = "detailed-plot", h)
                         }
                         return t.$$set = t => {
                             "data" in t && n(0, P = t.data), "sortingOptions" in t && n(1, S = t.sortingOptions), "noPlotsMessage" in t && n(2, z = t.noPlotsMessage)
                         }, t.$$.update = () => {
-                            1 & t.$$.dirty[0] && n(17, r = rf(P) ? 1 : 2), 8 & t.$$.dirty[0] && n(28, i = N ? N.width : 0), 8 & t.$$.dirty[0] && n(27, o = N ? N.height : 0), 16 & t.$$.dirty[0] && n(18, a = C ? C.width : 140), 1 & t.$$.dirty[0] && n(26, s = Math.min(P.length, 12)), 67108864 & t.$$.dirty[0] && n(7, [c, u] = function(t) {
+                            1 & t.$$.dirty[0] && n(17, r = af(P) ? 1 : 2), 8 & t.$$.dirty[0] && n(28, i = N ? N.width : 0), 8 & t.$$.dirty[0] && n(27, o = N ? N.height : 0), 16 & t.$$.dirty[0] && n(18, a = C ? C.width : 140), 1 & t.$$.dirty[0] && n(26, s = Math.min(P.length, 12)), 67108864 & t.$$.dirty[0] && n(7, [c, u] = function(t) {
                                 const e = Math.ceil(Math.sqrt(t)),
                                     n = Math.ceil(t / e);
                                 return 1 === r ? [e, n] : [n, e]
                             }(s), c, (n(8, u), n(26, s), n(0, P))), 268435712 & t.$$.dirty[0] && n(11, O = Math.floor(i / u)), 134217856 & t.$$.dirty[0] && n(12, D = Math.floor(o / c)), 33 & t.$$.dirty[0] && (V.forBrushing || (n(25, A = V.sort(P)), F(1))), 33 & t.$$.dirty[0] && V.forBrushing && H(P), 536870912 & t.$$.dirty[0] && y && n(13, R = !0), 67108865 & t.$$.dirty[0] && n(15, d = Math.ceil(P.length / s)), 100663360 & t.$$.dirty[0] && n(16, f = A.slice((q - 1) * s, q * s))
                         }, [P, S, z, N, C, V, q, c, u, B, E, O, D, R, W, d, f, r, a, k, M, T, H, F, K, A, s, o, i, y, () => F(q - 1), () => F(q + 1), function() {
                             V = L(this), n(5, V), n(1, S)
                         }, () => H(P), function() {
@@ -12007,45 +12060,45 @@
                             E = L(this), n(10, E)
                         }, function() {
                             C = l.entries.get(this)?.contentRect, n(4, C)
                         }, t => K(t), function() {
                             N = l.entries.get(this)?.contentRect, n(3, N)
                         }]
                     }
-                    const Cf = class extends xt {
+                    const Bf = class extends xt {
                             constructor(t) {
-                                super(), $t(this, t, Nf, zf, D, {
+                                super(), $t(this, t, Df, Cf, D, {
                                     data: 0,
                                     sortingOptions: 1,
                                     noPlotsMessage: 2
-                                }, ff, [-1, -1])
+                                }, gf, [-1, -1])
                             }
                         },
-                        Of = [{
-                            name: "Variance",
+                        jf = [{
+                            name: "Importance",
                             forBrushing: !1,
                             sort: function(t) {
-                                return 0 !== t.length && rf(t) ? t.sort(((t, e) => _e(t.deviation, e.deviation))) : t
+                                return 0 !== t.length && af(t) ? t.sort(((t, e) => _e(t.deviation, e.deviation))) : t
                             }
                         }, {
                             name: "Cluster difference",
                             forBrushing: !1,
                             sort: function(t) {
-                                if (0 === t.length || !rf(t)) return t;
+                                if (0 === t.length || !af(t)) return t;
 
                                 function e(t) {
                                     return 1 === t.ice.num_clusters ? -1 / 0 : Sn(t).cluster_distance
                                 }
                                 return t.sort(((t, n) => _e(e(t), e(n))))
                             }
                         }, {
-                            name: "Highlighted similarity",
+                            name: "Highlighted line similarity",
                             forBrushing: !0,
                             sort: function(t, e) {
-                                if (0 === t.length || !rf(t) || !e || !e.highlightedIndices || e.highlightedIndices.length <= 1 || !e.featureToIceLines) return t;
+                                if (0 === t.length || !af(t) || !e || !e.highlightedIndices || e.highlightedIndices.length <= 1 || !e.featureToIceLines) return t;
                                 const n = e.highlightedIndices,
                                     r = e.featureToIceLines,
                                     i = Object.fromEntries(t.map((t => {
                                         var e;
                                         const i = r[t.x_feature],
                                             o = zn(n.map((t => i[t]))),
                                             l = _n(o).map((t => {
@@ -12061,56 +12114,56 @@
                                                 }))
                                             }(o, l, t.ice.centered_pdp);
                                         return [t.x_feature, null !== (e = Ln(a)) && void 0 !== e ? e : 0]
                                     })));
                                 return t.sort(((t, e) => _e(i[t.x_feature], i[e.x_feature])))
                             }
                         }, {
-                            name: "Highlighted distribution",
+                            name: "Highlighted histogram difference",
                             forBrushing: !0,
                             sort: function(t, e) {
-                                if (!(0 !== t.length && rf(t) && e && e.highlightedDistributions && e.featureInfo)) return t;
+                                if (!(0 !== t.length && af(t) && e && e.highlightedDistributions && e.featureInfo)) return t;
                                 const n = e.highlightedDistributions,
                                     r = e.featureInfo,
                                     i = Object.fromEntries(t.map((t => {
                                         const e = n.get(t.x_feature);
                                         if (!e) return [t.x_feature, 0];
                                         const i = r[t.x_feature].distribution.percents,
                                             o = e.percents;
                                         let l = 0;
                                         for (let t = 0; t < i.length; t++) l += Math.abs(o[t] - i[t]);
                                         return [t.x_feature, l]
                                     })));
                                 return t.sort(((t, e) => _e(i[t.x_feature], i[e.x_feature])))
                             }
                         }],
-                        Df = [{
+                        Ef = [{
                             name: "Interaction",
                             forBrushing: !1,
                             sort: function(t) {
-                                return 0 === t.length || rf(t) ? t : t.sort(((t, e) => _e(t.H, e.H)))
+                                return 0 === t.length || af(t) ? t : t.sort(((t, e) => _e(t.H, e.H)))
                             }
                         }, {
                             name: "Variance",
                             forBrushing: !1,
                             sort: function(t) {
-                                return 0 === t.length || rf(t) ? t : t.sort(((t, e) => _e(t.deviation, e.deviation)))
+                                return 0 === t.length || af(t) ? t : t.sort(((t, e) => _e(t.deviation, e.deviation)))
                             }
                         }];
 
-                    function Bf(t) {
+                    function If(t) {
                         c(t, "svelte-cuqal2", ".one-way-grid-container.svelte-cuqal2{height:100%;display:flex}.pdp-grid-wrapper.svelte-cuqal2{flex:1;min-width:0}")
                     }
 
-                    function jf(t) {
+                    function Rf(t) {
                         let e, n, r, i, o, l, a;
-                        return r = new nf({}), r.$on("changeFilters", t[1]), l = new Cf({
+                        return r = new lf({}), r.$on("changeFilters", t[1]), l = new Bf({
                             props: {
                                 data: t[0],
-                                sortingOptions: Of,
+                                sortingOptions: jf,
                                 noPlotsMessage: "No plots to show."
                             }
                         }), {
                             c() {
                                 e = h("div"), n = h("div"), vt(r.$$.fragment), i = m(), o = h("div"), vt(l.$$.fragment), y(o, "class", "pdp-grid-wrapper svelte-cuqal2"), y(e, "class", "one-way-grid-container svelte-cuqal2")
                             },
                             m(t, c) {
@@ -12128,51 +12181,51 @@
                             },
                             d(t) {
                                 t && d(e), yt(r), yt(l)
                             }
                         }
                     }
 
-                    function Ef(t, e, n) {
+                    function Vf(t, e, n) {
                         let r, i, o;
                         j(t, tr, (t => n(3, i = t))), j(t, Yn, (t => n(4, o = t)));
                         let l = o;
                         return t.$$.update = () => {
                             12 & t.$$.dirty && n(0, r = i.filter((t => l.includes(t.x_feature))))
                         }, [r, function(t) {
                             n(2, l = t.detail)
                         }, l, i]
                     }
-                    const If = class extends xt {
+                    const Hf = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, Ef, jf, D, {}, Bf)
+                            super(), $t(this, t, Vf, Rf, D, {}, If)
                         }
                     };
 
-                    function Rf(t) {
+                    function qf(t) {
                         c(t, "svelte-fnunp4", ".controls-container.svelte-fnunp4.svelte-fnunp4{height:100%;flex:0 0 200px;min-width:200px;max-width:200px;padding:0.25em;border-right:1px solid var(--gray-1);display:flex;flex-direction:column;gap:0.5em}.feature-selector-wrapper-outer.svelte-fnunp4.svelte-fnunp4{flex:0 1 auto;min-height:0;display:flex;flex-direction:column}.feature-selector-wrapper-middle.svelte-fnunp4.svelte-fnunp4{flex:1;min-height:0;display:flex;flex-direction:column}.feature-selector-wrapper-inner.svelte-fnunp4.svelte-fnunp4{flex:1;min-height:0}.filter-header.svelte-fnunp4+.filter-content.svelte-fnunp4{margin-top:0.25em}.filter-content.svelte-fnunp4.svelte-fnunp4{margin-left:0.75em}hr.svelte-fnunp4.svelte-fnunp4{margin:0.75em 0;border:0;height:1px;background:var(--gray-2)}.two-way-filter-radio.svelte-fnunp4.svelte-fnunp4{display:flex;flex-direction:column}")
                     }
 
-                    function Vf(t) {
+                    function Ff(t) {
                         let e, n, r, i, o, l, a, c, f, p, v, $, x, M, L, A, P, z, T, N, O, D, B, j, E, I, R, V, H, q;
 
                         function F(e) {
                             t[7](e)
                         }
                         let W = {
                             title: "Name"
                         };
-                        void 0 !== t[1] && (W.expanded = t[1]), c = new Zd({
+                        void 0 !== t[1] && (W.expanded = t[1]), c = new ef({
                             props: W
                         }), K.push((() => mt(c, "expanded", F)));
                         let X = {
                             enabledFeatures: t[3],
                             idPrefix: "pdpilot-two"
                         };
-                        return I = new qd({
+                        return I = new Kd({
                             props: X
                         }), t[11](I), I.$on("changeNameFilters", t[4]), V = w(t[9][0]), {
                             c() {
                                 e = h("div"), n = h("div"), n.textContent = "Feature Filters", r = m(), i = h("button"), i.textContent = "Clear Filters", o = m(), l = h("div"), a = h("div"), vt(c.$$.fragment), p = m(), v = h("div"), $ = h("div"), x = h("div"), x.textContent = "Plots must contain", M = m(), L = h("label"), A = h("input"), P = g("\n          1+ selected feature"), z = m(), T = h("label"), N = h("input"), O = g("\n          2 selected features"), D = m(), B = h("hr"), j = m(), E = h("div"), vt(I.$$.fragment), y(n, "class", "pdpilot-bold"), k(i, "align-self", "start"), y(a, "class", "filter-header svelte-fnunp4"), y(A, "type", "radio"), y(A, "name", "op"), A.__value = "or", _(A, A.__value), y(N, "type", "radio"), y(N, "name", "op"), N.__value = "and", _(N, N.__value), y($, "class", "two-way-filter-radio svelte-fnunp4"), y(B, "class", "svelte-fnunp4"), y(E, "class", "feature-selector-wrapper-inner svelte-fnunp4"), y(v, "class", "filter-content feature-selector-wrapper-middle svelte-fnunp4"), S(v, "pdp-hide", !t[1]), y(l, "class", "filter-container feature-selector-wrapper-outer svelte-fnunp4"), y(e, "class", "controls-container svelte-fnunp4"), V.p(A, N)
                             },
                             m(d, f) {
                                 u(d, e, f), s(e, n), s(e, r), s(e, i), s(e, o), s(e, l), s(l, a), bt(c, a, null), s(l, p), s(l, v), s(v, $), s($, x), s($, M), s($, L), s(L, A), A.checked = A.__value === t[2], s(L, P), s($, z), s($, T), s(T, N), N.checked = N.__value === t[2], s(T, O), s(v, D), s(v, B), s(v, j), s(v, E), bt(I, E, null), R = !0, H || (q = [b(i, "click", t[6]), b(A, "change", t[8]), b(A, "change", t[5]), b(N, "change", t[10]), b(N, "change", t[5])], H = !0)
@@ -12191,15 +12244,15 @@
                             },
                             d(n) {
                                 n && d(e), yt(c), t[11](null), yt(I), V.r(), H = !1, C(q)
                             }
                         }
                     }
 
-                    function Hf(t, e, n) {
+                    function Wf(t, e, n) {
                         let r;
                         j(t, Yn, (t => n(3, r = t)));
                         const i = F();
                         let o, l = !0,
                             a = "and",
                             s = r;
                         return [o, l, a, r, function(t) {
@@ -12228,30 +12281,30 @@
                             function(t) {
                                 K[t ? "unshift" : "push"]((() => {
                                     o = t, n(0, o)
                                 }))
                             }
                         ]
                     }
-                    const qf = class extends xt {
+                    const Kf = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, Hf, Vf, D, {}, Rf)
+                            super(), $t(this, t, Wf, Ff, D, {}, qf)
                         }
                     };
 
-                    function Ff(t) {
+                    function Xf(t) {
                         c(t, "svelte-1akrxps", ".two-way-grid-container.svelte-1akrxps{height:100%;display:flex}.pdp-grid-wrapper.svelte-1akrxps{flex:1;min-width:0}")
                     }
 
-                    function Wf(t) {
+                    function Uf(t) {
                         let e, n, r, i, o, l, a;
-                        return r = new qf({}), r.$on("changeFilters", t[3]), l = new Cf({
+                        return r = new Kf({}), r.$on("changeFilters", t[3]), l = new Bf({
                             props: {
                                 data: t[2],
-                                sortingOptions: Df,
+                                sortingOptions: Ef,
                                 noPlotsMessage: 1 === t[0].length && "and" === t[1] ? "No plots to show." : "No plots to show. PDPilot only pre-computes two-way PDPs when it detects likely interaction between the pair of features."
                             }
                         }), {
                             c() {
                                 e = h("div"), n = h("div"), vt(r.$$.fragment), i = m(), o = h("div"), vt(l.$$.fragment), y(o, "class", "pdp-grid-wrapper svelte-1akrxps"), y(e, "class", "two-way-grid-container svelte-1akrxps")
                             },
                             m(t, c) {
@@ -12269,38 +12322,38 @@
                             },
                             d(t) {
                                 t && d(e), yt(r), yt(l)
                             }
                         }
                     }
 
-                    function Kf(t, e, n) {
+                    function Yf(t, e, n) {
                         let r, i, o;
                         j(t, nr, (t => n(4, i = t))), j(t, Yn, (t => n(5, o = t)));
                         let l = o,
                             a = "and";
                         return t.$$.update = () => {
                             19 & t.$$.dirty && n(2, r = i.filter((t => "and" === a ? l.includes(t.x_feature) && l.includes(t.y_feature) : l.includes(t.x_feature) || l.includes(t.y_feature))))
                         }, [l, a, r, function(t) {
                             n(0, l = t.detail.features), n(1, a = t.detail.op)
                         }, i]
                     }
-                    const Xf = class extends xt {
+                    const Gf = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, Kf, Wf, D, {}, Ff)
+                            super(), $t(this, t, Yf, Uf, D, {}, Xf)
                         }
                     };
 
-                    function Uf(t) {
+                    function Jf(t) {
                         c(t, "svelte-mtrl6h", ".pdpilot-widget-container.svelte-mtrl6h{box-sizing:border-box;width:100%;display:flex;flex-direction:column;font-size:16px;border:1px solid var(--gray-1);background-color:white;color:black;--magenta:rgb(121, 35, 103);--blue:rgb(0, 95, 204);--dark-blue:rgb(1, 51, 104);--gray-0:rgb(247, 247, 247);--gray-1:rgb(226, 226, 226);--gray-2:rgb(198, 198, 198);--gray-3:rgb(171, 171, 171);--gray-4:rgb(145, 145, 145);--gray-5:rgb(119, 119, 119);--gray-6:rgb(94, 94, 94);--gray-7:rgb(71, 71, 71);--gray-8:rgb(48, 48, 48);--gray-9:rgb(27, 27, 27);--black:black;--red:#d62728;--light-red:#fc655a}.pdp-tab-content.svelte-mtrl6h{flex:1;min-height:0}.pdpilot-widget-container.svelte-mtrl6h .pdp-hide{display:none}.pdpilot-widget-container.svelte-mtrl6h canvas,.pdpilot-widget-container.svelte-mtrl6h svg{display:block}.pdpilot-widget-container.svelte-mtrl6h *{box-sizing:border-box;margin:0;padding:0;line-height:1.2}.pdpilot-widget-container.svelte-mtrl6h button{color:var(--blue);background-color:white;border:1px solid var(--blue);border-radius:0.25em;text-align:center;cursor:pointer;font-size:1em;line-height:1em;padding:0.0625em 0.0625em;font-family:inherit}.pdpilot-widget-container.svelte-mtrl6h button:hover:enabled{color:white;background-color:var(--blue)}.pdpilot-widget-container.svelte-mtrl6h button:active:enabled{color:white;background-color:var(--dark-blue);border-color:var(--dark-blue)}.pdpilot-widget-container.svelte-mtrl6h button:disabled{cursor:not-allowed;background-color:transparent;color:var(--gray-4);border-color:var(--gray-4)}.pdpilot-widget-container.svelte-mtrl6h h1{font-size:1.125em;font-weight:500}.pdpilot-widget-container.svelte-mtrl6h h2{font-size:1.0625em;font-weight:500}.pdpilot-widget-container.svelte-mtrl6h .pdpilot-large{font-size:1.125em}.pdpilot-widget-container.svelte-mtrl6h .pdpilot-small{font-size:0.875em}.pdpilot-widget-container.svelte-mtrl6h .pdpilot-bold{font-weight:500}.pdpilot-widget-container.svelte-mtrl6h .pdpilot-icon{width:1em;height:1em}.pdpilot-widget-container.svelte-mtrl6h .pdpilot-cutoff{overflow:hidden;white-space:nowrap;text-overflow:ellipsis}.pdpilot-widget-container.svelte-mtrl6h .icon-tabler{-webkit-transform:translate(0px, 0px);transform:translate(0px, 0px)}")
                     }
 
-                    function Yf(t) {
+                    function Zf(t) {
                         let e, n, r, i, o, l, a, c, f, p, g, v, b = `${t[0]}px`;
-                        return n = new jr({}), o = new If({}), c = new Xf({}), g = new jd({}), {
+                        return n = new jr({}), o = new Hf({}), c = new Gf({}), g = new Rd({}), {
                             c() {
                                 e = h("div"), vt(n.$$.fragment), r = m(), i = h("div"), vt(o.$$.fragment), l = m(), a = h("div"), vt(c.$$.fragment), f = m(), p = h("div"), vt(g.$$.fragment), y(i, "class", "pdp-tab-content svelte-mtrl6h"), S(i, "pdp-hide", "one-way-plots" !== t[1]), y(a, "class", "pdp-tab-content svelte-mtrl6h"), S(a, "pdp-hide", "two-way-plots" !== t[1]), y(p, "class", "pdp-tab-content svelte-mtrl6h"), S(p, "pdp-hide", "detailed-plot" !== t[1]), y(e, "class", "pdpilot-widget-container svelte-mtrl6h"), k(e, "height", b)
                             },
                             m(t, d) {
                                 u(t, e, d), bt(n, e, null), s(e, r), s(e, i), bt(o, i, null), s(e, l), s(e, a), bt(c, a, null), s(e, f), s(e, p), bt(g, p, null), v = !0
                             },
                             p(t, [n]) {
@@ -12314,32 +12367,32 @@
                             },
                             d(t) {
                                 t && d(e), yt(n), yt(o), yt(c), yt(g)
                             }
                         }
                     }
 
-                    function Gf(t, e, n) {
+                    function Qf(t, e, n) {
                         let r, i;
                         return j(t, cr, (t => n(0, r = t))), j(t, hr, (t => n(1, i = t))), [r, i]
                     }
-                    const Jf = class extends xt {
+                    const th = class extends xt {
                         constructor(t) {
-                            super(), $t(this, t, Gf, Yf, D, {}, Uf)
+                            super(), $t(this, t, Qf, Zf, D, {}, Jf)
                         }
                     };
-                    class Zf extends e.DOMWidgetModel {
+                    class eh extends e.DOMWidgetModel {
                         defaults() {
                             return Object.assign(Object.assign({}, super.defaults()), {
-                                _model_name: Zf.model_name,
-                                _model_module: Zf.model_module,
-                                _model_module_version: Zf.model_module_version,
-                                _view_name: Zf.view_name,
-                                _view_module: Zf.view_module,
-                                _view_module_version: Zf.view_module_version,
+                                _model_name: eh.model_name,
+                                _model_module: eh.model_module,
+                                _model_module_version: eh.model_module_version,
+                                _view_name: eh.view_name,
+                                _view_module: eh.view_module,
+                                _view_module_version: eh.view_module_version,
                                 feature_names: [],
                                 feature_info: {},
                                 dataset: {},
                                 labels: [],
                                 num_instances: 0,
                                 one_way_pds: [],
                                 feature_to_ice_lines: {},
@@ -12353,16 +12406,16 @@
                                 height: 600,
                                 highlighted_indices: [],
                                 two_way_to_calculate: [],
                                 cluster_update: {}
                             })
                         }
                     }
-                    Zf.serializers = Object.assign({}, e.DOMWidgetModel.serializers), Zf.model_name = "PDPilotModel", Zf.model_module = Tr, Zf.model_module_version = zr, Zf.view_name = "PDPilotView", Zf.view_module = Tr, Zf.view_module_version = zr;
-                    class Qf extends e.DOMWidgetView {
+                    eh.serializers = Object.assign({}, e.DOMWidgetModel.serializers), eh.model_name = "PDPilotModel", eh.model_module = Tr, eh.model_module_version = zr, eh.view_name = "PDPilotView", eh.view_module = Tr, eh.view_module_version = zr;
+                    class nh extends e.DOMWidgetView {
                         render() {
                             (function(t) {
                                 Yn = Un("feature_names", [], t), Gn = Un("feature_info", {}, t), Jn = Un("dataset", {}, t), Zn = Un("labels", [], t), Qn = Un("num_instances", 0, t), tr = Un("one_way_pds", [], t), er = Un("feature_to_ice_lines", {}, t), nr = Un("two_way_pds", [], t), rr = Un("two_way_pdp_extent", [0, 0], t), ir = Un("two_way_interaction_extent", [0, 0], t), or = Un("one_way_pdp_extent", [0, 0], t), lr = Un("ice_line_extent", [0, 0], t), ar = Un("ice_cluster_center_extent", [0, 0], t), sr = Un("centered_ice_line_extent", [0, 0], t), cr = Un("height", 600, t), ur = Un("highlighted_indices", [], t), dr = Un("two_way_to_calculate", [], t), fr = Un("cluster_update", {}, t), hr = kt("one-way-plots"), pr = Mt(tr, (t => new Map(t.map((t => [t.x_feature, t]))))), gr = Mt(Zn, (t => 2 === new Set(t).size)), mr = Mt([Zn, gr], (([t, e]) => {
                                     const n = [Math.min(...t), Math.max(...t)];
                                     return e ? n : Vn(n)
                                 }));
                                 const e = t.get("one_way_pds"),
@@ -12372,20 +12425,20 @@
                                 }, ((t, e) => ({
                                     x: (.5 + .7548776662466927 * e) % 1,
                                     y: (.5 + .5698402909980532 * e) % 1
                                 }))))), _r = kt(!1), kr = kt(""), Mr = Mt(ur, (t => new Set(t))), Lr = Mt([Gn, Jn, ur], (([t, e, n]) => new Map(Object.entries(t).map((([t, r]) => [t, In(r, e[t], n)]))))), Ar = Mt(rr, (t => ln().domain(Vn(t)).interpolator(un).unknown("black"))), Pr = Mt(ir, (t => {
                                     const e = Vn([0, t[1]])[1];
                                     return an().domain([-e, 0, e]).interpolator(dn).unknown("black")
                                 }))
-                            })(this.model), new Jf({
+                            })(this.model), new th({
                                 target: this.el
                             })
                         }
                     }
-                    const th = {
+                    const rh = {
                         id: "pdpilot:plugin",
                         requires: [e.IJupyterWidgetRegistry],
                         activate: function(e, n) {
                             n.registerWidget({
                                 name: Tr,
                                 version: zr,
                                 exports: t
```

### Comparing `pdpilot-0.5.1/pdpilot/labextension/static/713.5fb1220914a3fc9b6db7.js` & `pdpilot-0.5.2/pdpilot/labextension/static/713.5fb1220914a3fc9b6db7.js`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/pdpilot/labextension/static/remoteEntry.7d03101ac0d410913165.js` & `pdpilot-0.5.2/pdpilot/labextension/static/remoteEntry.93d73cafbbe8e20d7f23.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, u, f, s, d, p, c, h, v, g, m, b, y = {
+    var e, r, t, n, o, i, a, l, u, s, d, f, p, c, h, v, g, b, m, y = {
             4960: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(1568))),
                         "./extension": () => t.e(568).then((() => () => t(1568)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    i = (e, r) => {
                         if (t.S) {
                             var n = "default",
                                 o = t.S[n];
                             if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
                     get: () => o,
-                    init: () => a
+                    init: () => i
                 })
             }
         },
         w = {};
 
     function S(e) {
         var r = w[e];
@@ -43,51 +43,51 @@
         }), r
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        568: "fc735409708fd22de78c",
+        568: "be4561957748b400120d",
         642: "b0459555f41fcaaf7c8d",
         713: "5fb1220914a3fc9b6db7"
     } [e] + ".js?v=" + {
-        568: "fc735409708fd22de78c",
+        568: "be4561957748b400120d",
         642: "b0459555f41fcaaf7c8d",
         713: "5fb1220914a3fc9b6db7"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "pdpilot:", S.l = (t, n, o, a) => {
+    }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "pdpilot:", S.l = (t, n, o, i) => {
         if (e[t]) e[t].push(n);
         else {
-            var i, l;
+            var a, l;
             if (void 0 !== o)
-                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var s = u[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        i = s;
+                for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
+                    var d = u[s];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
+                        a = d;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+            a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, S.nc && a.setAttribute("nonce", S.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
+            var f = (r, n) => {
+                    a.onerror = a.onload = null, clearTimeout(p);
                     var o = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
+                    if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
-                    target: i
+                    target: a
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
+            a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), l && document.head.appendChild(a)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -97,27 +97,27 @@
             r = {};
         S.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
                 S.o(S.S, t) || (S.S[t] = {});
-                var a = S.S[t],
-                    i = "pdpilot",
+                var i = S.S[t],
+                    a = "pdpilot",
                     l = (e, r, t, n) => {
-                        var o = a[e] = a[e] || {},
+                        var o = i[e] = i[e] || {},
                             l = o[r];
-                        (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
+                        (!l || !l.loaded && (!n != !l.eager ? n : a > l.from)) && (o[r] = {
                             get: t,
-                            from: i,
+                            from: a,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyter-widgets/base", "4.1.0", (() => Promise.all([S.e(713), S.e(642)]).then((() => () => S(2713))))), l("pdpilot", "0.5.1", (() => S.e(568).then((() => () => S(1568)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyter-widgets/base", "4.1.0", (() => Promise.all([S.e(713), S.e(642)]).then((() => () => S(2713))))), l("pdpilot", "0.5.2", (() => S.e(568).then((() => () => S(1568)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -133,126 +133,126 @@
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var o = e[n],
-                a = (typeof o)[0];
-            if (n >= r.length) return "u" == a;
-            var i = r[n],
-                l = (typeof i)[0];
-            if (a != l) return "o" == a && "n" == l || "s" == l || "u" == a;
-            if ("o" != a && "u" != a && o != i) return o < i;
+                i = (typeof o)[0];
+            if (n >= r.length) return "u" == i;
+            var a = r[n],
+                l = (typeof a)[0];
+            if (i != l) return "o" == i && "n" == l || "s" == l || "u" == i;
+            if ("o" != i && "u" != i && o != a) return o < a;
             n++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(l = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
+            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(l = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
-        var i = [];
-        for (a = 1; a < e.length; a++) {
-            var l = e[a];
-            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
+        var a = [];
+        for (i = 1; i < e.length; i++) {
+            var l = e[i];
+            a.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? a.pop() + " " + a.pop() : o(l))
         }
         return u();
 
         function u() {
-            return i.pop().replace(/^\((.+)\)$/, "$1")
+            return a.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, a = (e, r) => {
+    }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, s, d = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == d ? l > n && !o : "" == d != o);
-                if ("u" == s) {
-                    if (!u || "u" != d) return !1
+            for (var a = 0, l = 1, u = !0;; l++, a++) {
+                var s, d, f = l < e.length ? (typeof e[l])[0] : "";
+                if (a >= r.length || "o" == (d = (typeof(s = r[a]))[0])) return !u || ("u" == f ? l > n && !o : "" == f != o);
+                if ("u" == d) {
+                    if (!u || "u" != f) return !1
                 } else if (u)
-                    if (d == s)
+                    if (f == d)
                         if (l <= n) {
-                            if (f != e[l]) return !1
+                            if (s != e[l]) return !1
                         } else {
-                            if (o ? f > e[l] : f < e[l]) return !1;
-                            f != e[l] && (u = !1)
+                            if (o ? s > e[l] : s < e[l]) return !1;
+                            s != e[l] && (u = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != f && "n" != f) {
                     if (o || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || s < d != o) return !1;
+                    if (l <= n || d < f != o) return !1;
                     u = !1
-                } else "s" != d && "n" != d && (u = !1, l--)
+                } else "s" != f && "n" != f && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
-        for (i = 1; i < e.length; i++) {
-            var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+        for (a = 1; a < e.length; a++) {
+            var h = e[a];
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
         }
         return !!c()
-    }, i = (e, r) => {
+    }, a = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = l(e, t);
-        return a(n, o) || d(u(e, t, o, n)), p(e[t][o])
-    }, s = (e, r, t) => {
+        return i(n, o) || f(u(e, t, o, n)), p(e[t][o])
+    }, d = (e, r, t) => {
         var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, d = e => {
+        return (r = Object.keys(o).reduce(((e, r) => !i(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
+    }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, o) {
-        var a = S.I(r);
-        return a && a.then ? a.then(e.bind(e, r, S.S[r], t, n, o)) : e(r, S.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), v = c(((e, r, t, n, o) => {
-        var a = r && S.o(r, t) && s(r, t, n);
-        return a ? p(a) : o()
-    })), g = {}, m = {
+        var i = S.I(r);
+        return i && i.then ? i.then(e.bind(e, r, S.S[r], t, n, o)) : e(r, S.S[r], t, n, o)
+    })(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), v = c(((e, r, t, n, o) => {
+        var i = r && S.o(r, t) && d(r, t, n);
+        return i ? p(i) : o()
+    })), g = {}, b = {
         883: () => v("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1, 10], 1, 1, 1, 1, 1
         ], (() => Promise.all([S.e(713), S.e(642)]).then((() => () => S(2713))))),
         5633: () => h("default", "@lumino/messaging", [1, 2, 0, 0]),
         7930: () => h("default", "@lumino/coreutils", [1, 2, 0, 0]),
         8778: () => h("default", "@lumino/widgets", [1, 2, 0, 1])
-    }, b = {
+    }, m = {
         568: [883],
         642: [5633, 7930, 8778]
     }, S.f.consumes = (e, r) => {
-        S.o(b, e) && b[e].forEach((e => {
+        S.o(m, e) && m[e].forEach((e => {
             if (S.o(g, e)) return r.push(g[e]);
             var t = r => {
                     g[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
                 },
                 n = r => {
                     delete g[e], S.m[e] = t => {
                         throw delete S.c[e], r
                     }
                 };
             try {
-                var o = m[e]();
+                var o = b[e]();
                 o.then ? r.push(g[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
@@ -261,33 +261,33 @@
         S.f.j = (r, t) => {
             var n = S.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else if (642 != r) {
                 var o = new Promise(((t, o) => n = e[r] = [t, o]));
                 t.push(n[2] = o);
-                var a = S.p + S.u(r),
-                    i = new Error;
-                S.l(a, (t => {
+                var i = S.p + S.u(r),
+                    a = new Error;
+                S.l(i, (t => {
                     if (S.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                         var o = t && ("load" === t.type ? "missing" : t.type),
-                            a = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
+                            i = t && t.target && t.target.src;
+                        a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
-                var n, o, [a, i, l] = t,
+                var n, o, [i, a, l] = t,
                     u = 0;
-                if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) S.o(i, n) && (S.m[n] = i[n]);
+                if (i.some((r => 0 !== e[r]))) {
+                    for (n in a) S.o(a, n) && (S.m[n] = a[n]);
                     l && l(S)
                 }
-                for (r && r(t); u < a.length; u++) o = a[u], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); u < i.length; u++) o = i[u], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkpdpilot = self.webpackChunkpdpilot || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
     var E = S(4960);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).pdpilot = E
 })();
```

### Comparing `pdpilot-0.5.1/pdpilot/labextension/static/third-party-licenses.json` & `pdpilot-0.5.2/pdpilot/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/pdpilot/metadata.py` & `pdpilot-0.5.2/pdpilot/metadata.py`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/pdpilot/nbextension/index.js` & `pdpilot-0.5.2/pdpilot/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -453,15 +453,15 @@
             },
             146: e => {
                 "use strict";
                 e.exports = t
             },
             147: t => {
                 "use strict";
-                t.exports = JSON.parse('{"name":"pdpilot","version":"0.5.1","description":"A Jupyter widget for exploring PDP and ICE plots.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/DanielKerrigan/PDPilot","bugs":{"url":"https://github.com/DanielKerrigan/PDPilot/issues"},"license":"BSD-3-Clause","author":{"name":"Daniel Kerrigan","email":"kerrigan.d@northeastern.edu"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/DanielKerrigan/PDPilot"},"scripts":{"build":"webpack --mode=development && jupyter labextension build --development=True .","build:prod":"webpack --mode=production && jupyter labextension build .","clean":"npm run clean:lib && npm run clean:nbextension && npm run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf pdpilot/labextension","clean:nbextension":"rimraf pdpilot/nbextension/static/index.js","fix":"prettier --plugin-search-dir . --write src && eslint . --ext .ts,.tsx,.svelte --fix","check":"prettier --plugin-search-dir . --check src && eslint . --ext .ts,.tsx,.svelte && svelte-check","prepack":"npm run build:prod","watch":"npm run watch:nbextension","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch .","test":"uvu -r tsm tests"},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","d3":"^7.8.5","fast-kde":"^0.2.1","lodash.clonedeep":"^4.5.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3 || ^4","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@tsconfig/svelte":"^5.0.0","@types/d3":"^7.4.0","@types/lodash.clonedeep":"^4.5.7","@types/node":"^20.2.5","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.45.0","@typescript-eslint/parser":"^5.45.0","acorn":"^7.2.0","css-loader":"^6.7.0","eslint":"^8.28.0","eslint-config-prettier":"^8.5.0","eslint-plugin-svelte":"^2.30.0","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.8.0","prettier-plugin-svelte":"^2.10.1","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^3.0.0","svelte":"^4.0.0","svelte-check":"^3.4.6","svelte-loader":"^3.1.8","svelte-preprocess":"^5.0.4","ts-loader":"^9.0.0","tslib":"^2.4.1","tsm":"^2.2.1","typescript":"^5.1.6","uvu":"^0.5.3","webpack":">=5.76.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":true,"outputDir":"pdpilot/labextension/"}}')
+                t.exports = JSON.parse('{"name":"pdpilot","version":"0.5.2","description":"A Jupyter widget for exploring PDP and ICE plots.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/DanielKerrigan/PDPilot","bugs":{"url":"https://github.com/DanielKerrigan/PDPilot/issues"},"license":"BSD-3-Clause","author":{"name":"Daniel Kerrigan","email":"kerrigan.d@northeastern.edu"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/DanielKerrigan/PDPilot"},"scripts":{"build":"webpack --mode=development && jupyter labextension build --development=True .","build:prod":"webpack --mode=production && jupyter labextension build .","clean":"npm run clean:lib && npm run clean:nbextension && npm run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf pdpilot/labextension","clean:nbextension":"rimraf pdpilot/nbextension/static/index.js","fix":"prettier --plugin-search-dir . --write src && eslint . --ext .ts,.tsx,.svelte --fix","check":"prettier --plugin-search-dir . --check src && eslint . --ext .ts,.tsx,.svelte && svelte-check","prepack":"npm run build:prod","watch":"npm run watch:nbextension","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch .","test":"uvu -r tsm tests"},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6","d3":"^7.8.5","fast-kde":"^0.2.1","lodash.clonedeep":"^4.5.0"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyterlab/builder":"^3 || ^4","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@tsconfig/svelte":"^5.0.0","@types/d3":"^7.4.0","@types/lodash.clonedeep":"^4.5.7","@types/node":"^20.2.5","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^5.45.0","@typescript-eslint/parser":"^5.45.0","acorn":"^7.2.0","css-loader":"^6.7.0","eslint":"^8.28.0","eslint-config-prettier":"^8.5.0","eslint-plugin-svelte":"^2.30.0","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.8.0","prettier-plugin-svelte":"^2.10.1","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^3.0.0","svelte":"^4.0.0","svelte-check":"^3.4.6","svelte-loader":"^3.1.8","svelte-preprocess":"^5.0.4","ts-loader":"^9.0.0","tslib":"^2.4.1","tsm":"^2.2.1","typescript":"^5.1.6","uvu":"^0.5.3","webpack":">=5.76.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":true,"outputDir":"pdpilot/labextension/"}}')
             }
         },
         n = {};
 
     function r(t) {
         var i = n[t];
         if (void 0 !== i) return i.exports;
@@ -498,16 +498,16 @@
     }, r.nmd = t => (t.paths = [], t.children || (t.children = []), t);
     var i = {};
     return (() => {
         "use strict";
         r.r(i), r.d(i, {
             MODULE_NAME: () => n,
             MODULE_VERSION: () => e,
-            PDPilotModel: () => Zf,
-            PDPilotView: () => Qf
+            PDPilotModel: () => eh,
+            PDPilotView: () => nh
         });
         const t = r(147),
             e = t.version,
             n = t.name;
         var o = r(146);
         new Set;
         const l = "undefined" != typeof window ? window : "undefined" != typeof globalThis ? globalThis : global;
@@ -6259,15 +6259,15 @@
 
         function Ls(t) {
             let e, n, r, i, o, l, a, s, u, h, p, v, b = t[62].filteredIndices.length + "";
             return a = new Va({
                 props: {
                     scale: t[12],
                     x: t[25].left,
-                    label: "centered prediction"
+                    label: "Centered prediction"
                 }
             }), s = new Ma({
                 props: {
                     scale: t[13],
                     y: t[11] - t[25].bottom,
                     showTickLabels: t[62].id === t[16][t[16].length - 1],
                     showAxisLabel: t[62].id === t[16][t[16].length - 1],
@@ -6788,15 +6788,15 @@
                     integerOnly: "discrete" === t[9].subkind,
                     value_map: "value_map" in t[9] ? t[9].value_map : {}
                 }
             }), l = new Va({
                 props: {
                     scale: t[5],
                     x: t[7].left,
-                    label: "centered prediction"
+                    label: "Centered prediction"
                 }
             });
             let h = t[3] && Is(t);
             return {
                 c() {
                     e = g("svg"), s && s.c(), n = g("path"), u && u.c(), i = b(), bt(o.$$.fragment), bt(l.$$.fragment), h && h.c(), $(n, "d", r = t[11](t[0].ice.centered_pdp)), $(n, "stroke", "var(--black)"), $(n, "stroke-width", "2"), $(n, "fill", "none"), $(e, "width", t[1]), $(e, "height", t[2])
                 },
@@ -7117,15 +7117,15 @@
                     integerOnly: "discrete" === t[11].subkind,
                     value_map: "value_map" in t[11] ? t[11].value_map : {}
                 }
             }), a = new Va({
                 props: {
                     scale: t[13],
                     x: t[12].left,
-                    label: t[7] ? "centered prediction" : "prediction"
+                    label: t[7] ? "Centered prediction" : "Prediction"
                 }
             });
             let h = t[3] && Ks(t),
                 m = t[6] && t[18] === t[0].x_feature && Zs(t);
             return {
                 c() {
                     e = p("div"), n = p("canvas"), r = v(), i = g("svg"), o = g("g"), bt(l.$$.fragment), bt(a.$$.fragment), h && h.c(), s = b(), m && m.c(), $(n, "class", "svelte-hmor8t"), $(i, "width", t[1]), $(i, "height", t[2]), $(i, "class", "svelte-hmor8t"), $(e, "class", "pdpilot-plot-container svelte-hmor8t")
@@ -7133,15 +7133,15 @@
                 m(f, p) {
                     d(f, e, p), c(e, n), t[41](n), c(e, r), c(e, i), c(i, o), yt(l, o, null), yt(a, o, null), h && h.m(o, null), c(o, s), m && m.m(o, null), t[42](o), u = !0
                 },
                 p(t, e) {
                     const n = {};
                     16384 & e[0] && (n.scale = t[14]), 4100 & e[0] && (n.y = t[2] - t[12].bottom), 1 & e[0] && (n.label = t[0].x_feature), 2048 & e[0] && (n.integerOnly = "discrete" === t[11].subkind), 2048 & e[0] && (n.value_map = "value_map" in t[11] ? t[11].value_map : {}), l.$set(n);
                     const r = {};
-                    8192 & e[0] && (r.scale = t[13]), 4096 & e[0] && (r.x = t[12].left), 128 & e[0] && (r.label = t[7] ? "centered prediction" : "prediction"), a.$set(r), t[3] ? h ? (h.p(t, e), 8 & e[0] && dt(h, 1)) : (h = Ks(t), h.c(), dt(h, 1), h.m(o, s)) : h && (ct(), ft(h, 1, 1, (() => {
+                    8192 & e[0] && (r.scale = t[13]), 4096 & e[0] && (r.x = t[12].left), 128 & e[0] && (r.label = t[7] ? "Centered prediction" : "Prediction"), a.$set(r), t[3] ? h ? (h.p(t, e), 8 & e[0] && dt(h, 1)) : (h = Ks(t), h.c(), dt(h, 1), h.m(o, s)) : h && (ct(), ft(h, 1, 1, (() => {
                         h = null
                     })), ut()), t[6] && t[18] === t[0].x_feature ? m ? m.p(t, e) : (m = Zs(t), m.c(), m.m(o, null)) : m && (m.d(1), m = null), (!u || 2 & e[0]) && $(i, "width", t[1]), (!u || 4 & e[0]) && $(i, "height", t[2])
                 },
                 i(t) {
                     u || (dt(l.$$.fragment, t), dt(a.$$.fragment, t), dt(h), u = !0)
                 },
                 o(t) {
@@ -7573,15 +7573,15 @@
                         c = on().domain([0, 1]).range([0, n.bandwidth()]);
                     for (let d = 0; d < i.length; d++) {
                         const p = s(a[d].x),
                             g = c(a[d].y);
                         t.strokeStyle = r(l[d]), t.beginPath(), t.arc((null !== (f = e(i[d])) && void 0 !== f ? f : 0) + p, (null !== (h = n(o[d])) && void 0 !== h ? h : 0) + g, u, 0, 2 * Math.PI), t.stroke()
                     }
                 } else if ("bandwidth" in e && !("bandwidth" in n))
-                    if (e.bandwidth() >= 40) $n(Ln(i, o, l), (t => t[0])).forEach((([i, o]) => {
+                    if (e.bandwidth() >= 20) $n(Ln(i, o, l), (t => t[0])).forEach((([i, o]) => {
                         var l, a;
                         t.translate(null !== (l = e(i)) && void 0 !== l ? l : 0, 0),
                             function(t, e, n, r, i, o, l, a, s) {
                                 var c;
                                 if (!e) return;
                                 const u = on().domain([0, null !== (c = sc(t.densities, (t => t.density))) && void 0 !== c ? c : 0]).range([r / 2 - 2, 0]),
                                     d = cc().x0((t => {
@@ -7595,15 +7595,15 @@
                                     e.beginPath(), e.strokeStyle = "function" == typeof s ? s(i) : s, e.moveTo(r / 2 + 2, n(t)), e.lineTo(r, n(t)), e.stroke()
                                 })), e.globalAlpha = 1, e.fillStyle = "black", e.strokeStyle = "white", e.beginPath(), e.arc(r / 2, n(t.mean), 5, 0, 2 * Math.PI), e.fill(), e.stroke(), e.restore()
                             }(Fn(o.map((t => t[1])), o.map((t => t[2]))), t, n, e.bandwidth(), c, d, 0, 0, r), t.translate(-(null !== (a = e(i)) && void 0 !== a ? a : 0), 0)
                     }));
                     else
                         for (let a = 0; a < i.length; a++) t.strokeStyle = r(l[a]), t.beginPath(), t.moveTo(null !== (p = e(i[a])) && void 0 !== p ? p : 0, n(o[a])), t.lineTo((null !== (g = e(i[a])) && void 0 !== g ? g : 0) + e.bandwidth(), n(o[a])), t.stroke();
                 else if (!("bandwidth" in e) && "bandwidth" in n)
-                    if (n.bandwidth() >= 40) $n(Ln(i, o, l), (t => t[1])).forEach((([i, o]) => {
+                    if (n.bandwidth() >= 20) $n(Ln(i, o, l), (t => t[1])).forEach((([i, o]) => {
                         var l, a;
                         t.translate(0, null !== (l = n(i)) && void 0 !== l ? l : 0), fc(Fn(o.map((t => t[0])), o.map((t => t[2]))), t, e, s, n.bandwidth(), d, "rgb(145, 145, 145)", "black", r), t.translate(0, -(null !== (a = n(i)) && void 0 !== a ? a : 0))
                     }));
                     else
                         for (let a = 0; a < i.length; a++) t.strokeStyle = r(l[a]), t.beginPath(), t.moveTo(e(i[a]), null !== (m = n(o[a])) && void 0 !== m ? m : 0), t.lineTo(e(i[a]), (null !== (v = n(o[a])) && void 0 !== v ? v : 0) + n.bandwidth()), t.stroke();
                 else if (!("bandwidth" in e) && !("bandwidth" in n)) {
                     t.globalAlpha = d;
@@ -7760,86 +7760,139 @@
                     marginRight: 10,
                     marginLeft: 11,
                     title: 2
                 }, hc)
             }
         };
 
-        function xc(t) {
-            let e, n, r, i;
+        function xc(t, e, n) {
+            const r = t.slice();
+            return r[13] = e[n], r
+        }
+
+        function _c(t) {
+            let e, n = ht(t[8]),
+                r = [];
+            for (let e = 0; e < n.length; e += 1) r[e] = kc(xc(t, n, e));
             return {
                 c() {
-                    e = g("g"), n = g("path"), $(n, "d", r = t[2](t[3])), $(n, "stroke", t[1]), $(n, "fill", "none"), $(e, "transform", i = "translate(" + t[0] + ")")
+                    for (let t = 0; t < r.length; t += 1) r[t].c();
+                    e = b()
+                },
+                m(t, n) {
+                    for (let e = 0; e < r.length; e += 1) r[e] && r[e].m(t, n);
+                    d(t, e, n)
+                },
+                p(t, i) {
+                    if (377 & i) {
+                        let o;
+                        for (n = ht(t[8]), o = 0; o < n.length; o += 1) {
+                            const l = xc(t, n, o);
+                            r[o] ? r[o].p(l, i) : (r[o] = kc(l), r[o].c(), r[o].m(e.parentNode, e))
+                        }
+                        for (; o < r.length; o += 1) r[o].d(1);
+                        r.length = n.length
+                    }
+                },
+                d(t) {
+                    t && f(e), h(r, t)
+                }
+            }
+        }
+
+        function kc(t) {
+            let e, n, r;
+            return {
+                c() {
+                    e = g("circle"), $(e, "cx", n = "horizontal" === t[0] ? t[4](t[13]) : t[5](t[13])), $(e, "cy", r = "horizontal" === t[0] ? t[5](t[13]) : t[4](t[13])), $(e, "r", t[6]), $(e, "fill", t[3])
+                },
+                m(t, n) {
+                    d(t, e, n)
+                },
+                p(t, i) {
+                    305 & i && n !== (n = "horizontal" === t[0] ? t[4](t[13]) : t[5](t[13])) && $(e, "cx", n), 305 & i && r !== (r = "horizontal" === t[0] ? t[5](t[13]) : t[4](t[13])) && $(e, "cy", r), 64 & i && $(e, "r", t[6]), 8 & i && $(e, "fill", t[3])
+                },
+                d(t) {
+                    t && f(e)
+                }
+            }
+        }
+
+        function Mc(t) {
+            let e, n, r, i, o = "bandwidth" in t[1] && _c(t);
+            return {
+                c() {
+                    e = g("g"), n = g("path"), o && o.c(), $(n, "d", r = t[7](t[8])), $(n, "stroke", t[3]), $(n, "fill", "none"), $(e, "transform", i = "translate(" + t[2] + ")")
                 },
                 m(t, r) {
-                    d(t, e, r), c(e, n)
+                    d(t, e, r), c(e, n), o && o.m(e, null)
                 },
-                p(t, [o]) {
-                    12 & o && r !== (r = t[2](t[3])) && $(n, "d", r), 2 & o && $(n, "stroke", t[1]), 1 & o && i !== (i = "translate(" + t[0] + ")") && $(e, "transform", i)
+                p(t, [l]) {
+                    384 & l && r !== (r = t[7](t[8])) && $(n, "d", r), 8 & l && $(n, "stroke", t[3]), "bandwidth" in t[1] ? o ? o.p(t, l) : (o = _c(t), o.c(), o.m(e, null)) : o && (o.d(1), o = null), 4 & l && i !== (i = "translate(" + t[2] + ")") && $(e, "transform", i)
                 },
                 i: T,
                 o: T,
                 d(t) {
-                    t && f(e)
+                    t && f(e), o && o.d()
                 }
             }
         }
 
-        function _c(t, e, n) {
-            let r, i, o, l, a, s;
-            E(t, ar, (t => n(11, s = t)));
+        function Lc(t, e, n) {
+            let r, i, o, l, a, s, c;
+            E(t, ar, (t => n(12, c = t)));
             let {
-                pd: c
+                pd: u
             } = e, {
-                height: u
+                height: d
             } = e, {
-                direction: d
+                direction: f
             } = e, {
-                x: f
+                x: h
             } = e, {
-                translate: h = [0, 0]
+                translate: p = [0, 0]
             } = e, {
-                stroke: p = "black"
+                stroke: g = "black"
             } = e;
             return t.$$set = t => {
-                "pd" in t && n(4, c = t.pd), "height" in t && n(5, u = t.height), "direction" in t && n(6, d = t.direction), "x" in t && n(7, f = t.x), "translate" in t && n(0, h = t.translate), "stroke" in t && n(1, p = t.stroke)
+                "pd" in t && n(9, u = t.pd), "height" in t && n(10, d = t.height), "direction" in t && n(0, f = t.direction), "x" in t && n(1, h = t.x), "translate" in t && n(2, p = t.translate), "stroke" in t && n(3, g = t.stroke)
             }, t.$$.update = () => {
-                16 & t.$$.dirty && n(3, r = _n(c.x_values.length)), 2144 & t.$$.dirty && n(10, i = on().domain(s).range("horizontal" === d ? [u, 0] : [0, u])), 144 & t.$$.dirty && n(8, o = t => {
+                512 & t.$$.dirty && n(8, r = _n(u.x_values.length)), 5121 & t.$$.dirty && n(11, i = on().domain(c).range("horizontal" === f ? [d, 0] : [0, d])), 514 & t.$$.dirty && n(4, o = t => {
                     var e;
-                    return "bandwidth" in f ? (null !== (e = f(c.x_values[t])) && void 0 !== e ? e : 0) + f.bandwidth() / 2 : f(c.x_values[t])
-                }), 1040 & t.$$.dirty && n(9, l = t => i(c.mean_predictions[t])), 832 & t.$$.dirty && n(2, a = ei().x("horizontal" === d ? o : l).y("horizontal" === d ? l : o))
-            }, [h, p, a, r, c, u, d, f, o, l, i, s]
+                    return "bandwidth" in h ? (null !== (e = h(u.x_values[t])) && void 0 !== e ? e : 0) + h.bandwidth() / 2 : h(u.x_values[t])
+                }), 2560 & t.$$.dirty && n(5, l = t => i(u.mean_predictions[t])), 49 & t.$$.dirty && n(7, a = ei().x("horizontal" === f ? o : l).y("horizontal" === f ? l : o)), 2 & t.$$.dirty && n(6, s = "bandwidth" in h ? Math.min(2, h.bandwidth() / 2) : 0)
+            }, [f, h, p, g, o, l, s, a, r, u, d, i, c]
         }
-        const kc = class extends _t {
+        const Ac = class extends _t {
             constructor(t) {
-                super(), wt(this, t, _c, xc, j, {
-                    pd: 4,
-                    height: 5,
-                    direction: 6,
-                    x: 7,
-                    translate: 0,
-                    stroke: 1
+                super(), wt(this, t, Lc, Mc, j, {
+                    pd: 9,
+                    height: 10,
+                    direction: 0,
+                    x: 1,
+                    translate: 2,
+                    stroke: 3
                 })
             }
         };
 
-        function Mc(t) {
+        function Pc(t) {
             u(t, "svelte-crr1ai", ".two-way-container.svelte-crr1ai{position:relative;width:100%;height:100%}svg.svelte-crr1ai,canvas.svelte-crr1ai{position:absolute;top:var(--top);left:0}")
         }
 
-        function Lc(t) {
+        function Sc(t) {
             let e, n, r, i = t[12].left - t[21] + "px",
                 o = `${t[15]}px`;
             return n = new wc({
                 props: {
                     width: t[17] + t[20],
                     height: t[16],
                     color: t[8],
-                    marginLeft: Oc,
-                    marginRight: Oc,
+                    marginLeft: Bc,
+                    marginRight: Bc,
                     title: t[4]
                 }
             }), {
                 c() {
                     e = p("div"), bt(n.$$.fragment), M(e, "margin-left", i), M(e, "padding-top", o)
                 },
                 m(t, i) {
@@ -7857,25 +7910,25 @@
                 },
                 d(t) {
                     t && f(e), $t(n)
                 }
             }
         }
 
-        function Ac(t) {
+        function zc(t) {
             let e, n, r;
-            return e = new kc({
+            return e = new Ac({
                 props: {
                     pd: t[19],
                     height: t[6],
                     direction: "horizontal",
                     x: t[10],
                     translate: [0, t[12].top - t[6]]
                 }
-            }), n = new kc({
+            }), n = new Ac({
                 props: {
                     pd: t[18],
                     height: t[6],
                     direction: "vertical",
                     x: t[9],
                     translate: [t[1] - t[12].right, 0]
                 }
@@ -7900,24 +7953,24 @@
                 },
                 d(t) {
                     $t(e, t), $t(n, t)
                 }
             }
         }
 
-        function Pc(t) {
+        function Tc(t) {
             let e, n, r, i, o, l, a;
-            const s = [zc, Sc],
+            const s = [Cc, Nc],
                 c = [];
 
             function u(t, e) {
                 return "bandwidth" in t[10] ? 0 : 1
             }
             e = u(t), n = c[e] = s[e](t);
-            const h = [Nc, Tc],
+            const h = [Dc, Oc],
                 p = [];
 
             function g(t, e) {
                 return "bandwidth" in t[9] ? 0 : 1
             }
             return i = g(t), o = p[i] = h[i](t), {
                 c() {
@@ -7944,15 +7997,15 @@
                 },
                 d(t) {
                     t && (f(r), f(l)), c[e].d(t), p[i].d(t)
                 }
             }
         }
 
-        function Sc(t) {
+        function Nc(t) {
             let e, n;
             return e = new Qa({
                 props: {
                     data: t[14].distribution,
                     x: t[10],
                     height: t[6],
                     direction: "horizontal",
@@ -7977,15 +8030,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function zc(t) {
+        function Cc(t) {
             let e, n;
             return e = new ds({
                 props: {
                     data: t[14].distribution,
                     x: t[10],
                     height: t[6],
                     direction: "horizontal",
@@ -8010,15 +8063,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Tc(t) {
+        function Oc(t) {
             let e, n;
             return e = new Qa({
                 props: {
                     data: t[13].distribution,
                     x: t[9],
                     height: t[6],
                     direction: "vertical",
@@ -8043,15 +8096,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Nc(t) {
+        function Dc(t) {
             let e, n;
             return e = new ds({
                 props: {
                     data: t[13].distribution,
                     x: t[9],
                     height: t[6],
                     direction: "vertical",
@@ -8076,17 +8129,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Cc(t) {
+        function jc(t) {
             let e, n, r, i, o, l, a, s, u, h, m = `${t[16]+t[15]}px`,
-                b = t[5] && Lc(t);
+                b = t[5] && Sc(t);
             l = new Ma({
                 props: {
                     scale: t[10],
                     y: t[11] - t[12].bottom,
                     label: t[0].x_feature,
                     integerOnly: "discrete" === t[14].subkind,
                     value_map: "value_map" in t[14] ? t[14].value_map : {}
@@ -8096,29 +8149,29 @@
                     scale: t[9],
                     x: t[12].left,
                     label: t[0].y_feature,
                     integerOnly: "discrete" === t[13].subkind,
                     value_map: "value_map" in t[13] ? t[13].value_map : {}
                 }
             });
-            const y = [Pc, Ac],
+            const y = [Tc, zc],
                 w = [];
 
             function x(t, e) {
                 return t[2] ? 0 : t[3] && t[19] && t[18] ? 1 : -1
             }
             return ~(s = x(t)) && (u = w[s] = y[s](t)), {
                 c() {
                     e = p("div"), b && b.c(), n = v(), r = p("canvas"), i = v(), o = g("svg"), bt(l.$$.fragment), bt(a.$$.fragment), u && u.c(), $(r, "class", "svelte-crr1ai"), $(o, "width", t[1]), $(o, "height", t[11]), $(o, "class", "svelte-crr1ai"), $(e, "class", "two-way-container svelte-crr1ai"), M(e, "--top", m)
                 },
                 m(u, f) {
                     d(u, e, f), b && b.m(e, null), c(e, n), c(e, r), t[51](r), c(e, i), c(e, o), yt(l, o, null), yt(a, o, null), ~s && w[s].m(o, null), h = !0
                 },
                 p(t, r) {
-                    t[5] ? b ? (b.p(t, r), 32 & r[0] && dt(b, 1)) : (b = Lc(t), b.c(), dt(b, 1), b.m(e, n)) : b && (ct(), ft(b, 1, 1, (() => {
+                    t[5] ? b ? (b.p(t, r), 32 & r[0] && dt(b, 1)) : (b = Sc(t), b.c(), dt(b, 1), b.m(e, n)) : b && (ct(), ft(b, 1, 1, (() => {
                         b = null
                     })), ut());
                     const i = {};
                     1024 & r[0] && (i.scale = t[10]), 6144 & r[0] && (i.y = t[11] - t[12].bottom), 1 & r[0] && (i.label = t[0].x_feature), 16384 & r[0] && (i.integerOnly = "discrete" === t[14].subkind), 16384 & r[0] && (i.value_map = "value_map" in t[14] ? t[14].value_map : {}), l.$set(i);
                     const c = {};
                     512 & r[0] && (c.scale = t[9]), 4096 & r[0] && (c.x = t[12].left), 1 & r[0] && (c.label = t[0].y_feature), 8192 & r[0] && (c.integerOnly = "discrete" === t[13].subkind), 8192 & r[0] && (c.value_map = "value_map" in t[13] ? t[13].value_map : {}), a.$set(c);
                     let d = s;
@@ -8133,17 +8186,17 @@
                     ft(b), ft(l.$$.fragment, t), ft(a.$$.fragment, t), ft(u), h = !1
                 },
                 d(n) {
                     n && f(e), b && b.d(), t[51](null), $t(l), $t(a), ~s && w[s].d()
                 }
             }
         }
-        const Oc = 10;
+        const Bc = 10;
 
-        function Dc(t, e, n) {
+        function Ec(t, e, n) {
             let r, i, o, l, a, s, c, u, d, f, h, p, g, m, v, b, y, $, w, x, _, k, M, L, A, P, S, z, T;
             var N, C, O, D, j, B, I, R;
             E(t, mr, (t => n(47, P = t))), E(t, Sr, (t => n(48, S = t))), E(t, zr, (t => n(49, z = t))), E(t, Zn, (t => n(50, T = t)));
             let V, H, {
                     pd: q
                 } = e,
                 {
@@ -8190,66 +8243,66 @@
                     bottom: 35,
                     left: 50
                 }), 4259842 & t.$$.dirty[0] | 16384 & t.$$.dirty[1] && n(17, o = Math.min(W - i.left - i.right, K - r - i.top - i.bottom)), 131074 & t.$$.dirty[0] | 16384 & t.$$.dirty[1] && n(44, l = (W - o - i.left - i.right) / 2), 4390912 & t.$$.dirty[0] | 16384 & t.$$.dirty[1] && n(46, a = (K - r - o - i.top - i.bottom) / 2), 32 & t.$$.dirty[0] | 32768 & t.$$.dirty[1] && n(15, s = Q ? a : 0), 32768 & t.$$.dirty[0] | 57344 & t.$$.dirty[1] && n(12, c = {
                     top: i.top + a - s,
                     right: i.right + l,
                     bottom: i.bottom + a,
                     left: i.left + l
-                }), 4292608 & t.$$.dirty[0] && n(11, u = K - r - s), 1 & t.$$.dirty[0] | 524288 & t.$$.dirty[1] && n(14, d = T[q.x_feature]), 1 & t.$$.dirty[0] | 524288 & t.$$.dirty[1] && n(13, f = T[q.y_feature]), 1 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(42, h = S.copy().domain([q.pdp_min, q.pdp_max])), 1 & t.$$.dirty[0] | 262144 & t.$$.dirty[1] && n(43, p = z.copy().domain([q.interaction_min, 0, q.interaction_max])), 25165824 & t.$$.dirty[0] | 399360 & t.$$.dirty[1] && n(8, g = "interactions" === J ? U ? p : z : U ? h : S), 1 & t.$$.dirty[0] && n(37, m = Wn(q.x_axis)), 1 & t.$$.dirty[0] && n(36, v = Wn(q.y_axis)), 402653185 & t.$$.dirty[0] | 64 & t.$$.dirty[1] && n(41, b = q.x_axis[0] - (null !== n(28, C = null === n(27, N = m.get(q.x_axis[0])) || void 0 === N ? void 0 : N.before) && void 0 !== C ? C : 0)), 1610612737 & t.$$.dirty[0] | 64 & t.$$.dirty[1] && n(40, y = q.x_axis[q.x_axis.length - 1] + (null !== n(30, D = null === n(29, O = m.get(q.x_axis[q.x_axis.length - 1])) || void 0 === O ? void 0 : O.after) && void 0 !== D ? D : 0)), 1 & t.$$.dirty[0] | 35 & t.$$.dirty[1] && n(39, $ = q.y_axis[0] - (null !== n(32, B = null === n(31, j = v.get(q.y_axis[0])) || void 0 === j ? void 0 : j.before) && void 0 !== B ? B : 0)), 1 & t.$$.dirty[0] | 44 & t.$$.dirty[1] && n(38, w = q.y_axis[q.y_axis.length - 1] + (null !== n(34, R = null === n(33, I = v.get(q.y_axis[q.y_axis.length - 1])) || void 0 === I ? void 0 : I.after) && void 0 !== R ? R : 0)), 20483 & t.$$.dirty[0] | 1536 & t.$$.dirty[1] && n(10, x = "quantitative" === d.kind ? on().domain([b, y]).range([c.left, W - c.right]) : Ir().domain(q.x_axis).range([c.left, W - c.right])), 14337 & t.$$.dirty[0] | 384 & t.$$.dirty[1] && n(9, _ = "quantitative" === f.kind ? on().domain([$, w]).range([u - c.bottom, c.top]) : Ir().domain(q.y_axis).range([u - c.bottom, c.top])), 2178 & t.$$.dirty[0] | 16 & t.$$.dirty[1] && H && (En(V, H, W, u), H && null != x && null != _ && uc(q, H, W, u, x, _, g, J, m, v)), 16781059 & t.$$.dirty[0] | 112 & t.$$.dirty[1] && H && null != x && null != _ && uc(q, H, W, u, x, _, g, J, m, v), 16 & t.$$.dirty[0] && n(21, k = "" === Z ? Oc : 0), 16 & t.$$.dirty[0] && n(20, M = "" === Z ? 2 * Oc : Oc), 1 & t.$$.dirty[0] | 65536 & t.$$.dirty[1] && n(19, L = P.get(q.x_feature)), 1 & t.$$.dirty[0] | 65536 & t.$$.dirty[1] && n(18, A = P.get(q.y_feature))
+                }), 4292608 & t.$$.dirty[0] && n(11, u = K - r - s), 1 & t.$$.dirty[0] | 524288 & t.$$.dirty[1] && n(14, d = T[q.x_feature]), 1 & t.$$.dirty[0] | 524288 & t.$$.dirty[1] && n(13, f = T[q.y_feature]), 1 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(42, h = S.copy().domain([q.pdp_min, q.pdp_max])), 1 & t.$$.dirty[0] | 262144 & t.$$.dirty[1] && n(43, p = z.copy().domain([q.interaction_min, 0, q.interaction_max])), 25165824 & t.$$.dirty[0] | 399360 & t.$$.dirty[1] && n(8, g = "interactions" === J ? U ? p : z : U ? h : S), 1 & t.$$.dirty[0] && n(37, m = Wn(q.x_axis)), 1 & t.$$.dirty[0] && n(36, v = Wn(q.y_axis)), 402653185 & t.$$.dirty[0] | 64 & t.$$.dirty[1] && n(41, b = q.x_axis[0] - (null !== n(28, C = null === n(27, N = m.get(q.x_axis[0])) || void 0 === N ? void 0 : N.before) && void 0 !== C ? C : 0)), 1610612737 & t.$$.dirty[0] | 64 & t.$$.dirty[1] && n(40, y = q.x_axis[q.x_axis.length - 1] + (null !== n(30, D = null === n(29, O = m.get(q.x_axis[q.x_axis.length - 1])) || void 0 === O ? void 0 : O.after) && void 0 !== D ? D : 0)), 1 & t.$$.dirty[0] | 35 & t.$$.dirty[1] && n(39, $ = q.y_axis[0] - (null !== n(32, B = null === n(31, j = v.get(q.y_axis[0])) || void 0 === j ? void 0 : j.before) && void 0 !== B ? B : 0)), 1 & t.$$.dirty[0] | 44 & t.$$.dirty[1] && n(38, w = q.y_axis[q.y_axis.length - 1] + (null !== n(34, R = null === n(33, I = v.get(q.y_axis[q.y_axis.length - 1])) || void 0 === I ? void 0 : I.after) && void 0 !== R ? R : 0)), 20483 & t.$$.dirty[0] | 1536 & t.$$.dirty[1] && n(10, x = "quantitative" === d.kind ? on().domain([b, y]).range([c.left, W - c.right]) : Ir().domain(q.x_axis).range([c.left, W - c.right])), 14337 & t.$$.dirty[0] | 384 & t.$$.dirty[1] && n(9, _ = "quantitative" === f.kind ? on().domain([$, w]).range([u - c.bottom, c.top]) : Ir().domain(q.y_axis).range([u - c.bottom, c.top])), 2178 & t.$$.dirty[0] | 16 & t.$$.dirty[1] && H && (En(V, H, W, u), H && null != x && null != _ && uc(q, H, W, u, x, _, g, J, m, v)), 16781059 & t.$$.dirty[0] | 112 & t.$$.dirty[1] && H && null != x && null != _ && uc(q, H, W, u, x, _, g, J, m, v), 16 & t.$$.dirty[0] && n(21, k = "" === Z ? Bc : 0), 16 & t.$$.dirty[0] && n(20, M = "" === Z ? 2 * Bc : Bc), 1 & t.$$.dirty[0] | 65536 & t.$$.dirty[1] && n(19, L = P.get(q.x_feature)), 1 & t.$$.dirty[0] | 65536 & t.$$.dirty[1] && n(18, A = P.get(q.y_feature))
             }, [q, W, Y, G, Z, Q, nt, V, g, _, x, u, c, f, d, s, r, o, A, L, M, k, K, U, J, tt, et, N, C, O, D, j, B, I, R, H, v, m, w, $, y, b, h, p, l, i, a, P, S, z, T, function(t) {
                 X[t ? "unshift" : "push"]((() => {
                     V = t, n(7, V)
                 }))
             }]
         }
-        const jc = class extends _t {
+        const Ic = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Dc, Cc, j, {
+                super(), wt(this, t, Ec, jc, j, {
                     pd: 0,
                     width: 1,
                     height: 22,
                     scaleLocally: 23,
                     showMarginalDistribution: 2,
                     showMarginalPdp: 3,
                     colorShows: 24,
                     colorLegendTitle: 4,
                     showColorLegend: 5,
                     marginTop: 25,
                     marginRight: 26,
                     marginalPlotHeight: 6
-                }, Mc, [-1, -1])
+                }, Pc, [-1, -1])
             }
         };
 
-        function Bc(t, e) {
+        function Rc(t, e) {
             for (var n = new Array(e), r = 0; r < e; ++r) n[r] = t(r / (e - 1));
             return n
         }
 
-        function Ec(t) {
+        function Vc(t) {
             var e = t.length;
             return function(n) {
                 return t[Math.max(0, Math.min(e - 1, Math.floor(n * e)))]
             }
         }
-        const Ic = Ec(cn("44015444025645045745055946075a46085c460a5d460b5e470d60470e6147106347116447136548146748166848176948186a481a6c481b6d481c6e481d6f481f70482071482173482374482475482576482677482878482979472a7a472c7a472d7b472e7c472f7d46307e46327e46337f463480453581453781453882443983443a83443b84433d84433e85423f854240864241864142874144874045884046883f47883f48893e49893e4a893e4c8a3d4d8a3d4e8a3c4f8a3c508b3b518b3b528b3a538b3a548c39558c39568c38588c38598c375a8c375b8d365c8d365d8d355e8d355f8d34608d34618d33628d33638d32648e32658e31668e31678e31688e30698e306a8e2f6b8e2f6c8e2e6d8e2e6e8e2e6f8e2d708e2d718e2c718e2c728e2c738e2b748e2b758e2a768e2a778e2a788e29798e297a8e297b8e287c8e287d8e277e8e277f8e27808e26818e26828e26828e25838e25848e25858e24868e24878e23888e23898e238a8d228b8d228c8d228d8d218e8d218f8d21908d21918c20928c20928c20938c1f948c1f958b1f968b1f978b1f988b1f998a1f9a8a1e9b8a1e9c891e9d891f9e891f9f881fa0881fa1881fa1871fa28720a38620a48621a58521a68522a78522a88423a98324aa8325ab8225ac8226ad8127ad8128ae8029af7f2ab07f2cb17e2db27d2eb37c2fb47c31b57b32b67a34b67935b77937b87838b9773aba763bbb753dbc743fbc7340bd7242be7144bf7046c06f48c16e4ac16d4cc26c4ec36b50c46a52c56954c56856c66758c7655ac8645cc8635ec96260ca6063cb5f65cb5e67cc5c69cd5b6ccd5a6ece5870cf5773d05675d05477d1537ad1517cd2507fd34e81d34d84d44b86d54989d5488bd6468ed64590d74393d74195d84098d83e9bd93c9dd93ba0da39a2da37a5db36a8db34aadc32addc30b0dd2fb2dd2db5de2bb8de29bade28bddf26c0df25c2df23c5e021c8e020cae11fcde11dd0e11cd2e21bd5e21ad8e219dae319dde318dfe318e2e418e5e419e7e419eae51aece51befe51cf1e51df4e61ef6e620f8e621fbe723fde725"));
-        Ec(cn("00000401000501010601010802010902020b02020d03030f03031204041405041606051806051a07061c08071e0907200a08220b09240c09260d0a290e0b2b100b2d110c2f120d31130d34140e36150e38160f3b180f3d19103f1a10421c10441d11471e114920114b21114e22115024125325125527125829115a2a115c2c115f2d11612f116331116533106734106936106b38106c390f6e3b0f703d0f713f0f72400f74420f75440f764510774710784910784a10794c117a4e117b4f127b51127c52137c54137d56147d57157e59157e5a167e5c167f5d177f5f187f601880621980641a80651a80671b80681c816a1c816b1d816d1d816e1e81701f81721f817320817521817621817822817922827b23827c23827e24828025828125818326818426818627818827818928818b29818c29818e2a81902a81912b81932b80942c80962c80982d80992d809b2e7f9c2e7f9e2f7fa02f7fa1307ea3307ea5317ea6317da8327daa337dab337cad347cae347bb0357bb2357bb3367ab5367ab73779b83779ba3878bc3978bd3977bf3a77c03a76c23b75c43c75c53c74c73d73c83e73ca3e72cc3f71cd4071cf4070d0416fd2426fd3436ed5446dd6456cd8456cd9466bdb476adc4869de4968df4a68e04c67e24d66e34e65e44f64e55064e75263e85362e95462ea5661eb5760ec5860ed5a5fee5b5eef5d5ef05f5ef1605df2625df2645cf3655cf4675cf4695cf56b5cf66c5cf66e5cf7705cf7725cf8745cf8765cf9785df9795df97b5dfa7d5efa7f5efa815ffb835ffb8560fb8761fc8961fc8a62fc8c63fc8e64fc9065fd9266fd9467fd9668fd9869fd9a6afd9b6bfe9d6cfe9f6dfea16efea36ffea571fea772fea973feaa74feac76feae77feb078feb27afeb47bfeb67cfeb77efeb97ffebb81febd82febf84fec185fec287fec488fec68afec88cfeca8dfecc8ffecd90fecf92fed194fed395fed597fed799fed89afdda9cfddc9efddea0fde0a1fde2a3fde3a5fde5a7fde7a9fde9aafdebacfcecaefceeb0fcf0b2fcf2b4fcf4b6fcf6b8fcf7b9fcf9bbfcfbbdfcfdbf")), Ec(cn("00000401000501010601010802010a02020c02020e03021004031204031405041706041907051b08051d09061f0a07220b07240c08260d08290e092b10092d110a30120a32140b34150b37160b39180c3c190c3e1b0c411c0c431e0c451f0c48210c4a230c4c240c4f260c51280b53290b552b0b572d0b592f0a5b310a5c320a5e340a5f3609613809623909633b09643d09653e0966400a67420a68440a68450a69470b6a490b6a4a0c6b4c0c6b4d0d6c4f0d6c510e6c520e6d540f6d550f6d57106e59106e5a116e5c126e5d126e5f136e61136e62146e64156e65156e67166e69166e6a176e6c186e6d186e6f196e71196e721a6e741a6e751b6e771c6d781c6d7a1d6d7c1d6d7d1e6d7f1e6c801f6c82206c84206b85216b87216b88226a8a226a8c23698d23698f24699025689225689326679526679727669827669a28659b29649d29649f2a63a02a63a22b62a32c61a52c60a62d60a82e5fa92e5eab2f5ead305dae305cb0315bb1325ab3325ab43359b63458b73557b93556ba3655bc3754bd3853bf3952c03a51c13a50c33b4fc43c4ec63d4dc73e4cc83f4bca404acb4149cc4248ce4347cf4446d04545d24644d34743d44842d54a41d74b3fd84c3ed94d3dda4e3cdb503bdd513ade5238df5337e05536e15635e25734e35933e45a31e55c30e65d2fe75e2ee8602de9612bea632aeb6429eb6628ec6726ed6925ee6a24ef6c23ef6e21f06f20f1711ff1731df2741cf3761bf37819f47918f57b17f57d15f67e14f68013f78212f78410f8850ff8870ef8890cf98b0bf98c0af98e09fa9008fa9207fa9407fb9606fb9706fb9906fb9b06fb9d07fc9f07fca108fca309fca50afca60cfca80dfcaa0ffcac11fcae12fcb014fcb216fcb418fbb61afbb81dfbba1ffbbc21fbbe23fac026fac228fac42afac62df9c72ff9c932f9cb35f8cd37f8cf3af7d13df7d340f6d543f6d746f5d949f5db4cf4dd4ff4df53f4e156f3e35af3e55df2e661f2e865f2ea69f1ec6df1ed71f1ef75f1f179f2f27df2f482f3f586f3f68af4f88ef5f992f6fa96f8fb9af9fc9dfafda1fcffa4"));
-        var Rc = Ec(cn("0d088710078813078916078a19068c1b068d1d068e20068f2206902406912605912805922a05932c05942e05952f059631059733059735049837049938049a3a049a3c049b3e049c3f049c41049d43039e44039e46039f48039f4903a04b03a14c02a14e02a25002a25102a35302a35502a45601a45801a45901a55b01a55c01a65e01a66001a66100a76300a76400a76600a76700a86900a86a00a86c00a86e00a86f00a87100a87201a87401a87501a87701a87801a87a02a87b02a87d03a87e03a88004a88104a78305a78405a78606a68707a68808a68a09a58b0aa58d0ba58e0ca48f0da4910ea3920fa39410a29511a19613a19814a099159f9a169f9c179e9d189d9e199da01a9ca11b9ba21d9aa31e9aa51f99a62098a72197a82296aa2395ab2494ac2694ad2793ae2892b02991b12a90b22b8fb32c8eb42e8db52f8cb6308bb7318ab83289ba3388bb3488bc3587bd3786be3885bf3984c03a83c13b82c23c81c33d80c43e7fc5407ec6417dc7427cc8437bc9447aca457acb4679cc4778cc4977cd4a76ce4b75cf4c74d04d73d14e72d24f71d35171d45270d5536fd5546ed6556dd7566cd8576bd9586ada5a6ada5b69db5c68dc5d67dd5e66de5f65de6164df6263e06363e16462e26561e26660e3685fe4695ee56a5de56b5de66c5ce76e5be76f5ae87059e97158e97257ea7457eb7556eb7655ec7754ed7953ed7a52ee7b51ef7c51ef7e50f07f4ff0804ef1814df1834cf2844bf3854bf3874af48849f48948f58b47f58c46f68d45f68f44f79044f79143f79342f89441f89540f9973ff9983ef99a3efa9b3dfa9c3cfa9e3bfb9f3afba139fba238fca338fca537fca636fca835fca934fdab33fdac33fdae32fdaf31fdb130fdb22ffdb42ffdb52efeb72dfeb82cfeba2cfebb2bfebd2afebe2afec029fdc229fdc328fdc527fdc627fdc827fdca26fdcb26fccd25fcce25fcd025fcd225fbd324fbd524fbd724fad824fada24f9dc24f9dd25f8df25f8e125f7e225f7e425f6e626f6e826f5e926f5eb27f4ed27f3ee27f3f027f2f227f1f426f1f525f0f724f0f921"));
-        const Vc = cn("4e79a7f28e2ce1575976b7b259a14fedc949af7aa1ff9da79c755fbab0ab");
+        const Hc = Vc(cn("44015444025645045745055946075a46085c460a5d460b5e470d60470e6147106347116447136548146748166848176948186a481a6c481b6d481c6e481d6f481f70482071482173482374482475482576482677482878482979472a7a472c7a472d7b472e7c472f7d46307e46327e46337f463480453581453781453882443983443a83443b84433d84433e85423f854240864241864142874144874045884046883f47883f48893e49893e4a893e4c8a3d4d8a3d4e8a3c4f8a3c508b3b518b3b528b3a538b3a548c39558c39568c38588c38598c375a8c375b8d365c8d365d8d355e8d355f8d34608d34618d33628d33638d32648e32658e31668e31678e31688e30698e306a8e2f6b8e2f6c8e2e6d8e2e6e8e2e6f8e2d708e2d718e2c718e2c728e2c738e2b748e2b758e2a768e2a778e2a788e29798e297a8e297b8e287c8e287d8e277e8e277f8e27808e26818e26828e26828e25838e25848e25858e24868e24878e23888e23898e238a8d228b8d228c8d228d8d218e8d218f8d21908d21918c20928c20928c20938c1f948c1f958b1f968b1f978b1f988b1f998a1f9a8a1e9b8a1e9c891e9d891f9e891f9f881fa0881fa1881fa1871fa28720a38620a48621a58521a68522a78522a88423a98324aa8325ab8225ac8226ad8127ad8128ae8029af7f2ab07f2cb17e2db27d2eb37c2fb47c31b57b32b67a34b67935b77937b87838b9773aba763bbb753dbc743fbc7340bd7242be7144bf7046c06f48c16e4ac16d4cc26c4ec36b50c46a52c56954c56856c66758c7655ac8645cc8635ec96260ca6063cb5f65cb5e67cc5c69cd5b6ccd5a6ece5870cf5773d05675d05477d1537ad1517cd2507fd34e81d34d84d44b86d54989d5488bd6468ed64590d74393d74195d84098d83e9bd93c9dd93ba0da39a2da37a5db36a8db34aadc32addc30b0dd2fb2dd2db5de2bb8de29bade28bddf26c0df25c2df23c5e021c8e020cae11fcde11dd0e11cd2e21bd5e21ad8e219dae319dde318dfe318e2e418e5e419e7e419eae51aece51befe51cf1e51df4e61ef6e620f8e621fbe723fde725"));
+        Vc(cn("00000401000501010601010802010902020b02020d03030f03031204041405041606051806051a07061c08071e0907200a08220b09240c09260d0a290e0b2b100b2d110c2f120d31130d34140e36150e38160f3b180f3d19103f1a10421c10441d11471e114920114b21114e22115024125325125527125829115a2a115c2c115f2d11612f116331116533106734106936106b38106c390f6e3b0f703d0f713f0f72400f74420f75440f764510774710784910784a10794c117a4e117b4f127b51127c52137c54137d56147d57157e59157e5a167e5c167f5d177f5f187f601880621980641a80651a80671b80681c816a1c816b1d816d1d816e1e81701f81721f817320817521817621817822817922827b23827c23827e24828025828125818326818426818627818827818928818b29818c29818e2a81902a81912b81932b80942c80962c80982d80992d809b2e7f9c2e7f9e2f7fa02f7fa1307ea3307ea5317ea6317da8327daa337dab337cad347cae347bb0357bb2357bb3367ab5367ab73779b83779ba3878bc3978bd3977bf3a77c03a76c23b75c43c75c53c74c73d73c83e73ca3e72cc3f71cd4071cf4070d0416fd2426fd3436ed5446dd6456cd8456cd9466bdb476adc4869de4968df4a68e04c67e24d66e34e65e44f64e55064e75263e85362e95462ea5661eb5760ec5860ed5a5fee5b5eef5d5ef05f5ef1605df2625df2645cf3655cf4675cf4695cf56b5cf66c5cf66e5cf7705cf7725cf8745cf8765cf9785df9795df97b5dfa7d5efa7f5efa815ffb835ffb8560fb8761fc8961fc8a62fc8c63fc8e64fc9065fd9266fd9467fd9668fd9869fd9a6afd9b6bfe9d6cfe9f6dfea16efea36ffea571fea772fea973feaa74feac76feae77feb078feb27afeb47bfeb67cfeb77efeb97ffebb81febd82febf84fec185fec287fec488fec68afec88cfeca8dfecc8ffecd90fecf92fed194fed395fed597fed799fed89afdda9cfddc9efddea0fde0a1fde2a3fde3a5fde5a7fde7a9fde9aafdebacfcecaefceeb0fcf0b2fcf2b4fcf4b6fcf6b8fcf7b9fcf9bbfcfbbdfcfdbf")), Vc(cn("00000401000501010601010802010a02020c02020e03021004031204031405041706041907051b08051d09061f0a07220b07240c08260d08290e092b10092d110a30120a32140b34150b37160b39180c3c190c3e1b0c411c0c431e0c451f0c48210c4a230c4c240c4f260c51280b53290b552b0b572d0b592f0a5b310a5c320a5e340a5f3609613809623909633b09643d09653e0966400a67420a68440a68450a69470b6a490b6a4a0c6b4c0c6b4d0d6c4f0d6c510e6c520e6d540f6d550f6d57106e59106e5a116e5c126e5d126e5f136e61136e62146e64156e65156e67166e69166e6a176e6c186e6d186e6f196e71196e721a6e741a6e751b6e771c6d781c6d7a1d6d7c1d6d7d1e6d7f1e6c801f6c82206c84206b85216b87216b88226a8a226a8c23698d23698f24699025689225689326679526679727669827669a28659b29649d29649f2a63a02a63a22b62a32c61a52c60a62d60a82e5fa92e5eab2f5ead305dae305cb0315bb1325ab3325ab43359b63458b73557b93556ba3655bc3754bd3853bf3952c03a51c13a50c33b4fc43c4ec63d4dc73e4cc83f4bca404acb4149cc4248ce4347cf4446d04545d24644d34743d44842d54a41d74b3fd84c3ed94d3dda4e3cdb503bdd513ade5238df5337e05536e15635e25734e35933e45a31e55c30e65d2fe75e2ee8602de9612bea632aeb6429eb6628ec6726ed6925ee6a24ef6c23ef6e21f06f20f1711ff1731df2741cf3761bf37819f47918f57b17f57d15f67e14f68013f78212f78410f8850ff8870ef8890cf98b0bf98c0af98e09fa9008fa9207fa9407fb9606fb9706fb9906fb9b06fb9d07fc9f07fca108fca309fca50afca60cfca80dfcaa0ffcac11fcae12fcb014fcb216fcb418fbb61afbb81dfbba1ffbbc21fbbe23fac026fac228fac42afac62df9c72ff9c932f9cb35f8cd37f8cf3af7d13df7d340f6d543f6d746f5d949f5db4cf4dd4ff4df53f4e156f3e35af3e55df2e661f2e865f2ea69f1ec6df1ed71f1ef75f1f179f2f27df2f482f3f586f3f68af4f88ef5f992f6fa96f8fb9af9fc9dfafda1fcffa4"));
+        var qc = Vc(cn("0d088710078813078916078a19068c1b068d1d068e20068f2206902406912605912805922a05932c05942e05952f059631059733059735049837049938049a3a049a3c049b3e049c3f049c41049d43039e44039e46039f48039f4903a04b03a14c02a14e02a25002a25102a35302a35502a45601a45801a45901a55b01a55c01a65e01a66001a66100a76300a76400a76600a76700a86900a86a00a86c00a86e00a86f00a87100a87201a87401a87501a87701a87801a87a02a87b02a87d03a87e03a88004a88104a78305a78405a78606a68707a68808a68a09a58b0aa58d0ba58e0ca48f0da4910ea3920fa39410a29511a19613a19814a099159f9a169f9c179e9d189d9e199da01a9ca11b9ba21d9aa31e9aa51f99a62098a72197a82296aa2395ab2494ac2694ad2793ae2892b02991b12a90b22b8fb32c8eb42e8db52f8cb6308bb7318ab83289ba3388bb3488bc3587bd3786be3885bf3984c03a83c13b82c23c81c33d80c43e7fc5407ec6417dc7427cc8437bc9447aca457acb4679cc4778cc4977cd4a76ce4b75cf4c74d04d73d14e72d24f71d35171d45270d5536fd5546ed6556dd7566cd8576bd9586ada5a6ada5b69db5c68dc5d67dd5e66de5f65de6164df6263e06363e16462e26561e26660e3685fe4695ee56a5de56b5de66c5ce76e5be76f5ae87059e97158e97257ea7457eb7556eb7655ec7754ed7953ed7a52ee7b51ef7c51ef7e50f07f4ff0804ef1814df1834cf2844bf3854bf3874af48849f48948f58b47f58c46f68d45f68f44f79044f79143f79342f89441f89540f9973ff9983ef99a3efa9b3dfa9c3cfa9e3bfb9f3afba139fba238fca338fca537fca636fca835fca934fdab33fdac33fdae32fdaf31fdb130fdb22ffdb42ffdb52efeb72dfeb82cfeba2cfebb2bfebd2afebe2afec029fdc229fdc328fdc527fdc627fdc827fdca26fdcb26fccd25fcce25fcd025fcd225fbd324fbd524fbd724fad824fada24f9dc24f9dd25f8df25f8e125f7e225f7e425f6e626f6e826f5e926f5eb27f4ed27f3ee27f3f027f2f227f1f426f1f525f0f724f0f921"));
+        const Fc = cn("4e79a7f28e2ce1575976b7b259a14fedc949af7aa1ff9da79c755fbab0ab");
 
-        function Hc(t) {
+        function Wc(t) {
             u(t, "svelte-1pgkml6", ".color-container.svelte-1pgkml6{display:flex;align-items:center;gap:1em}.swatches.svelte-1pgkml6{flex:1;display:flex;gap:1em}.swatch-cell.svelte-1pgkml6{display:flex;align-items:center}.swatch-square.svelte-1pgkml6{min-width:var(--size);min-height:var(--size);margin-right:0.25em}")
         }
 
-        function qc(t, e, n) {
+        function Kc(t, e, n) {
             const r = t.slice();
             return r[10] = e[n], r
         }
 
-        function Fc(t) {
+        function Xc(t) {
             let e, n, r;
             return {
                 c() {
                     e = p("div"), n = m(t[5]), r = m(":"), $(e, "class", "pdpilot-small pdpilot-bold")
                 },
                 m(t, i) {
                     d(t, e, i), c(e, n), c(e, r)
@@ -8259,16 +8312,16 @@
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Wc(t) {
-            let e, n, r, i, o, l, a = `${Xc}px`,
+        function Uc(t) {
+            let e, n, r, i, o, l, a = `${Gc}px`,
                 s = (t[6][t[10]] ?? t[10]) + "";
             return {
                 c() {
                     e = p("div"), n = p("div"), r = v(), i = p("div"), o = m(s), l = v(), $(n, "class", "swatch-square svelte-1pgkml6"), M(n, "--size", a), M(n, "background-color", t[2](t[10])), $(i, "class", "swatch-label pdpilot-small"), $(e, "class", "swatch-cell svelte-1pgkml6")
                 },
                 m(t, a) {
                     d(t, e, a), c(e, n), c(e, r), c(e, i), c(i, o), c(e, l)
@@ -8278,57 +8331,57 @@
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Kc(t) {
+        function Yc(t) {
             let e, n, r, i, o = `${t[8]}px`,
                 l = `${t[1]}px`,
                 a = `${t[0]}px`,
                 s = `${t[3]}px`,
                 u = `${t[4]}px`,
-                g = "" !== t[5] && Fc(t),
+                g = "" !== t[5] && Xc(t),
                 m = ht(t[2].domain()),
                 b = [];
-            for (let e = 0; e < m.length; e += 1) b[e] = Wc(qc(t, m, e));
+            for (let e = 0; e < m.length; e += 1) b[e] = Uc(Kc(t, m, e));
             return {
                 c() {
                     e = p("div"), g && g.c(), n = v(), r = p("div");
                     for (let t = 0; t < b.length; t += 1) b[t].c();
                     $(r, "class", "swatches svelte-1pgkml6"), M(r, "max-width", o), $(e, "class", "color-container svelte-1pgkml6"), M(e, "max-height", l), M(e, "max-width", a), M(e, "margin-left", s), M(e, "margin-right", u)
                 },
                 m(o, l) {
                     d(o, e, l), g && g.m(e, null), c(e, n), c(e, r);
                     for (let t = 0; t < b.length; t += 1) b[t] && b[t].m(r, null);
                     i = S.observe(r, t[9].bind(r))
                 },
                 p(t, [i]) {
-                    if ("" !== t[5] ? g ? g.p(t, i) : (g = Fc(t), g.c(), g.m(e, n)) : g && (g.d(1), g = null), 68 & i) {
+                    if ("" !== t[5] ? g ? g.p(t, i) : (g = Xc(t), g.c(), g.m(e, n)) : g && (g.d(1), g = null), 68 & i) {
                         let e;
                         for (m = ht(t[2].domain()), e = 0; e < m.length; e += 1) {
-                            const n = qc(t, m, e);
-                            b[e] ? b[e].p(n, i) : (b[e] = Wc(n), b[e].c(), b[e].m(r, null))
+                            const n = Kc(t, m, e);
+                            b[e] ? b[e].p(n, i) : (b[e] = Uc(n), b[e].c(), b[e].m(r, null))
                         }
                         for (; e < b.length; e += 1) b[e].d(1);
                         b.length = m.length
                     }
                     256 & i && o !== (o = `${t[8]}px`) && M(r, "max-width", o), 2 & i && l !== (l = `${t[1]}px`) && M(e, "max-height", l), 1 & i && a !== (a = `${t[0]}px`) && M(e, "max-width", a), 8 & i && s !== (s = `${t[3]}px`) && M(e, "margin-left", s), 16 & i && u !== (u = `${t[4]}px`) && M(e, "margin-right", u)
                 },
                 i: T,
                 o: T,
                 d(t) {
                     t && f(e), g && g.d(), h(b, t), i()
                 }
             }
         }
-        const Xc = 12;
+        const Gc = 12;
 
-        function Uc(t, e, n) {
+        function Jc(t, e, n) {
             let r, {
                     width: i
                 } = e,
                 {
                     height: o
                 } = e,
                 {
@@ -8351,35 +8404,35 @@
                 "width" in t && n(0, i = t.width), "height" in t && n(1, o = t.height), "color" in t && n(2, l = t.color), "marginLeft" in t && n(3, s = t.marginLeft), "marginRight" in t && n(4, c = t.marginRight), "title" in t && n(5, u = t.title), "value_map" in t && n(6, d = t.value_map)
             }, t.$$.update = () => {
                 128 & t.$$.dirty && n(8, f = r ? r[0].inlineSize : 0)
             }, [i, o, l, s, c, u, d, r, f, function() {
                 r = a.entries.get(this)?.borderBoxSize, n(7, r)
             }]
         }
-        const Yc = class extends _t {
+        const Zc = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Uc, Kc, j, {
+                super(), wt(this, t, Jc, Yc, j, {
                     width: 0,
                     height: 1,
                     color: 2,
                     marginLeft: 3,
                     marginRight: 4,
                     title: 5,
                     value_map: 6
-                }, Hc)
+                }, Wc)
             }
         };
 
-        function Gc(t) {
+        function Qc(t) {
             u(t, "svelte-crr1ai", ".two-way-container.svelte-crr1ai{position:relative;width:100%;height:100%}svg.svelte-crr1ai,canvas.svelte-crr1ai{position:absolute;top:var(--top);left:0}")
         }
 
-        function Jc(t) {
+        function tu(t) {
             let e, n, r, i, o = `${t[9].left}px`;
-            const l = [Qc, Zc],
+            const l = [nu, eu],
                 a = [];
 
             function s(t, e) {
                 return "interpolator" in t[4] ? 0 : 1
             }
             return n = s(t), r = a[n] = l[n](t), {
                 c() {
@@ -8402,17 +8455,17 @@
                 },
                 d(t) {
                     t && f(e), a[n].d()
                 }
             }
         }
 
-        function Zc(t) {
+        function eu(t) {
             let e, n;
-            return e = new Yc({
+            return e = new Zc({
                 props: {
                     width: t[1] - t[9].left - t[9].right,
                     height: t[11],
                     color: t[4],
                     value_map: "value_map" in t[8] ? t[8].value_map : {},
                     title: t[0].y_feature,
                     marginLeft: 10,
@@ -8437,15 +8490,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Qc(t) {
+        function nu(t) {
             let e, n;
             return e = new wc({
                 props: {
                     width: t[1] - t[9].left - t[9].right,
                     height: t[11],
                     color: t[4],
                     title: t[0].y_feature,
@@ -8471,16 +8524,16 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function tu(t) {
-            let e, n, r, i, o, l, a, s, u = t[2] && Jc(t);
+        function ru(t) {
+            let e, n, r, i, o, l, a, s, u = t[2] && tu(t);
             return l = new Ma({
                 props: {
                     scale: t[6],
                     y: t[7] - t[9].bottom,
                     label: t[0].x_feature,
                     integerOnly: "discrete" === t[10].subkind,
                     value_map: "value_map" in t[10] ? t[10].value_map : {}
@@ -8497,15 +8550,15 @@
                 c() {
                     e = p("div"), u && u.c(), n = v(), r = p("canvas"), i = v(), o = g("svg"), bt(l.$$.fragment), bt(a.$$.fragment), $(r, "class", "svelte-crr1ai"), $(o, "width", t[1]), $(o, "height", t[7]), $(o, "class", "svelte-crr1ai"), $(e, "class", "two-way-container svelte-crr1ai"), M(e, "--top", t[11])
                 },
                 m(f, h) {
                     d(f, e, h), u && u.m(e, null), c(e, n), c(e, r), t[23](r), c(e, i), c(e, o), yt(l, o, null), yt(a, o, null), s = !0
                 },
                 p(t, [r]) {
-                    t[2] ? u ? (u.p(t, r), 4 & r && dt(u, 1)) : (u = Jc(t), u.c(), dt(u, 1), u.m(e, n)) : u && (ct(), ft(u, 1, 1, (() => {
+                    t[2] ? u ? (u.p(t, r), 4 & r && dt(u, 1)) : (u = tu(t), u.c(), dt(u, 1), u.m(e, n)) : u && (ct(), ft(u, 1, 1, (() => {
                         u = null
                     })), ut());
                     const i = {};
                     64 & r && (i.scale = t[6]), 640 & r && (i.y = t[7] - t[9].bottom), 1 & r && (i.label = t[0].x_feature), 1024 & r && (i.integerOnly = "discrete" === t[10].subkind), 1024 & r && (i.value_map = "value_map" in t[10] ? t[10].value_map : {}), l.$set(i);
                     const c = {};
                     32 & r && (c.scale = t[5]), 512 & r && (c.x = t[9].left), 256 & r && (c.integerOnly = "discrete" === t[8].subkind), 256 & r && (c.value_map = "value_map" in t[8] ? t[8].value_map : {}), a.$set(c), (!s || 2 & r) && $(o, "width", t[1]), (!s || 128 & r) && $(o, "height", t[7]), 2048 & r && M(e, "--top", t[11])
                 },
@@ -8517,15 +8570,15 @@
                 },
                 d(n) {
                     n && f(e), u && u.d(), t[23](null), $t(l), $t(a)
                 }
             }
         }
 
-        function eu(t, e, n) {
+        function iu(t, e, n) {
             let r, i, o, l, a, s, c, u, d, f, h, p, g, m;
             E(t, or, (t => n(21, g = t))), E(t, Zn, (t => n(22, m = t)));
             let v, b, {
                     pd: y
                 } = e,
                 {
                     width: $
@@ -8561,21 +8614,21 @@
             }, t.$$.update = () => {
                 4 & t.$$.dirty && n(11, r = _ ? 24 : 0), 6144 & t.$$.dirty && n(7, i = w - r), 49152 & t.$$.dirty && n(9, o = {
                     top: k,
                     right: M,
                     bottom: 35,
                     left: 50
                 }), 4194305 & t.$$.dirty && n(10, l = m[y.x_feature]), 4194305 & t.$$.dirty && n(8, a = m[y.y_feature]), 641 & t.$$.dirty && n(20, s = on().domain([y.pdp_min, y.pdp_max]).range([i - o.bottom, o.top])), 2097792 & t.$$.dirty && n(19, c = on().domain(g).range([i - o.bottom, o.top])), 1581056 & t.$$.dirty && n(5, u = x ? s : c), 1539 & t.$$.dirty && n(6, d = "quantitative" === l.kind ? on().domain([y.x_values[0], y.x_values[y.x_values.length - 1]]).range([o.left, $ - o.right]) : Vr().domain(y.x_values).range([o.left, $ - o.right]).padding(.5)), 256 & t.$$.dirty && n(4, f = function(t) {
-                    if ("quantitative" === t.kind) return an().domain([t.values[0], t.values[t.values.length - 1]]).interpolator((t => Ic(1 - t)));
+                    if ("quantitative" === t.kind) return an().domain([t.values[0], t.values[t.values.length - 1]]).interpolator((t => Hc(1 - t)));
                     if ("categorical" !== t.kind || "nominal" !== t.subkind && "one_hot" !== t.subkind) {
                         const e = t.values.length;
-                        return Er().domain(t.values).range(Bc(Ic, e).reverse())
+                        return Er().domain(t.values).range(Rc(Hc, e).reverse())
                     } {
                         const e = t.values.length;
-                        return Er().domain(t.values).range(e <= 10 ? Vc : Bc(Ic, e).reverse())
+                        return Er().domain(t.values).range(e <= 10 ? Fc : Rc(Hc, e).reverse())
                     }
                 }(a)), 65632 & t.$$.dirty && n(17, h = ei().x((t => {
                     var e;
                     return null !== (e = d(t.x)) && void 0 !== e ? e : 0
                 })).y((t => u(t.prediction))).context(b)), 1 & t.$$.dirty && n(18, p = function(t) {
                     var e;
                     const n = new Map;
@@ -8596,31 +8649,31 @@
                 }(y)), 65674 & t.$$.dirty && b && (En(v, b, $, i), b && null != d && null != u && null != h && L(p, b, h, f)), 458864 & t.$$.dirty && b && null != d && null != u && null != h && L(p, b, h, f)
             }, [y, $, _, v, f, u, d, i, a, o, l, r, w, x, k, M, b, h, p, c, s, g, m, function(t) {
                 X[t ? "unshift" : "push"]((() => {
                     v = t, n(3, v)
                 }))
             }]
         }
-        const nu = class extends _t {
+        const ou = class extends _t {
             constructor(t) {
-                super(), wt(this, t, eu, tu, j, {
+                super(), wt(this, t, iu, ru, j, {
                     pd: 0,
                     width: 1,
                     height: 12,
                     scaleLocally: 13,
                     showColorLegend: 2,
                     marginTop: 14,
                     marginRight: 15
-                }, Gc)
+                }, Qc)
             }
         };
 
-        function ru(t) {
+        function lu(t) {
             let e, n;
-            return e = new nu({
+            return e = new ou({
                 props: {
                     pd: t[0],
                     width: t[1],
                     height: t[2],
                     scaleLocally: t[3],
                     showColorLegend: t[7],
                     marginTop: t[9],
@@ -8645,17 +8698,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function iu(t) {
+        function au(t) {
             let e, n;
-            return e = new jc({
+            return e = new Ic({
                 props: {
                     pd: t[0],
                     width: t[1],
                     height: t[2],
                     scaleLocally: t[3],
                     showMarginalDistribution: t[4],
                     showMarginalPdp: t[5],
@@ -8685,17 +8738,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function ou(t) {
+        function su(t) {
             let e, n, r, i;
-            const o = [iu, ru],
+            const o = [au, lu],
                 l = [];
 
             function a(t, e) {
                 return "heatmap" === t[12] ? 0 : 1
             }
             return e = a(t), n = l[e] = o[e](t), {
                 c() {
@@ -8718,15 +8771,15 @@
                 },
                 d(t) {
                     t && f(r), l[e].d(t)
                 }
             }
         }
 
-        function lu(t, e, n) {
+        function cu(t, e, n) {
             let {
                 pd: r
             } = e, {
                 width: i
             } = e, {
                 height: o
             } = e, {
@@ -8750,17 +8803,17 @@
             } = e, {
                 twoWayKind: g = "heatmap"
             } = e;
             return t.$$set = t => {
                 "pd" in t && n(0, r = t.pd), "width" in t && n(1, i = t.width), "height" in t && n(2, o = t.height), "scaleLocally" in t && n(3, l = t.scaleLocally), "showMarginalDistribution" in t && n(4, a = t.showMarginalDistribution), "showMarginalPdp" in t && n(5, s = t.showMarginalPdp), "colorShows" in t && n(6, c = t.colorShows), "showColorLegend" in t && n(7, u = t.showColorLegend), "colorLegendTitle" in t && n(8, d = t.colorLegendTitle), "marginTop" in t && n(9, f = t.marginTop), "marginRight" in t && n(10, h = t.marginRight), "marginalPlotHeight" in t && n(11, p = t.marginalPlotHeight), "twoWayKind" in t && n(12, g = t.twoWayKind)
             }, [r, i, o, l, a, s, c, u, d, f, h, p, g]
         }
-        const au = class extends _t {
+        const uu = class extends _t {
             constructor(t) {
-                super(), wt(this, t, lu, ou, j, {
+                super(), wt(this, t, cu, su, j, {
                     pd: 0,
                     width: 1,
                     height: 2,
                     scaleLocally: 3,
                     showMarginalDistribution: 4,
                     showMarginalPdp: 5,
                     colorShows: 6,
@@ -8770,17 +8823,17 @@
                     marginRight: 10,
                     marginalPlotHeight: 11,
                     twoWayKind: 12
                 })
             }
         };
 
-        function su(t) {
+        function du(t) {
             let e, n, r, i;
-            const o = [uu, cu],
+            const o = [hu, fu],
                 l = [];
 
             function a(t, e) {
                 return 1 === t[0].num_features ? 0 : 2 === t[0].num_features ? 1 : -1
             }
             return ~(e = a(t)) && (n = l[e] = o[e](t)), {
                 c() {
@@ -8803,17 +8856,17 @@
                 },
                 d(t) {
                     t && f(r), ~e && l[e].d(t)
                 }
             }
         }
 
-        function cu(t) {
+        function fu(t) {
             let e, n;
-            return e = new au({
+            return e = new uu({
                 props: {
                     width: t[1],
                     height: t[2],
                     pd: t[0],
                     scaleLocally: t[3],
                     colorShows: t[4],
                     showColorLegend: t[5],
@@ -8844,15 +8897,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function uu(t) {
+        function hu(t) {
             let e, n;
             return e = new ac({
                 props: {
                     width: t[1],
                     height: t[2],
                     pd: t[0],
                     scaleLocally: t[3],
@@ -8884,25 +8937,25 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function du(t) {
-            let e, n, r = t[1] > 0 && t[2] > 0 && su(t);
+        function pu(t) {
+            let e, n, r = t[1] > 0 && t[2] > 0 && du(t);
             return {
                 c() {
                     r && r.c(), e = b()
                 },
                 m(t, i) {
                     r && r.m(t, i), d(t, e, i), n = !0
                 },
                 p(t, [n]) {
-                    t[1] > 0 && t[2] > 0 ? r ? (r.p(t, n), 6 & n && dt(r, 1)) : (r = su(t), r.c(), dt(r, 1), r.m(e.parentNode, e)) : r && (ct(), ft(r, 1, 1, (() => {
+                    t[1] > 0 && t[2] > 0 ? r ? (r.p(t, n), 6 & n && dt(r, 1)) : (r = du(t), r.c(), dt(r, 1), r.m(e.parentNode, e)) : r && (ct(), ft(r, 1, 1, (() => {
                         r = null
                     })), ut())
                 },
                 i(t) {
                     n || (dt(r), n = !0)
                 },
                 o(t) {
@@ -8910,15 +8963,15 @@
                 },
                 d(t) {
                     t && f(e), r && r.d(t)
                 }
             }
         }
 
-        function fu(t, e, n) {
+        function gu(t, e, n) {
             let {
                 pd: r
             } = e, {
                 width: i
             } = e, {
                 height: o
             } = e, {
@@ -8952,17 +9005,17 @@
             } = e, {
                 twoWayKind: $ = "heatmap"
             } = e;
             return t.$$set = t => {
                 "pd" in t && n(0, r = t.pd), "width" in t && n(1, i = t.width), "height" in t && n(2, o = t.height), "scaleLocally" in t && n(3, l = t.scaleLocally), "colorShows" in t && n(4, a = t.colorShows), "showColorLegend" in t && n(5, s = t.showColorLegend), "colorLegendTitle" in t && n(6, c = t.colorLegendTitle), "iceLevel" in t && n(7, u = t.iceLevel), "indices" in t && n(8, d = t.indices), "showMarginalDistribution" in t && n(9, f = t.showMarginalDistribution), "showMarginalPdp" in t && n(10, h = t.showMarginalPdp), "marginTop" in t && n(11, p = t.marginTop), "marginRight" in t && n(12, g = t.marginRight), "marginalPlotHeight" in t && n(13, m = t.marginalPlotHeight), "allowBrushing" in t && n(14, v = t.allowBrushing), "showBrushedBorder" in t && n(15, b = t.showBrushedBorder), "iceLineWidth" in t && n(16, y = t.iceLineWidth), "twoWayKind" in t && n(17, $ = t.twoWayKind)
             }, [r, i, o, l, a, s, c, u, d, f, h, p, g, m, v, b, y, $]
         }
-        const hu = class extends _t {
+        const mu = class extends _t {
             constructor(t) {
-                super(), wt(this, t, fu, du, j, {
+                super(), wt(this, t, gu, pu, j, {
                     pd: 0,
                     width: 1,
                     height: 2,
                     scaleLocally: 3,
                     colorShows: 4,
                     showColorLegend: 5,
                     colorLegendTitle: 6,
@@ -8977,69 +9030,69 @@
                     showBrushedBorder: 15,
                     iceLineWidth: 16,
                     twoWayKind: 17
                 })
             }
         };
 
-        function pu(t, e) {
+        function vu(t, e) {
             if ((i = t.length) > 1)
                 for (var n, r, i, o = 1, l = t[e[0]], a = l.length; o < i; ++o)
                     for (r = l, l = t[e[o]], n = 0; n < a; ++n) l[n][1] += l[n][0] = isNaN(r[n][1]) ? r[n][0] : r[n][1]
         }
 
-        function gu(t) {
+        function bu(t) {
             for (var e = t.length, n = new Array(e); --e >= 0;) n[e] = e;
             return n
         }
 
-        function mu(t, e) {
+        function yu(t, e) {
             return t[e]
         }
 
-        function vu(t) {
+        function $u(t) {
             const e = [];
             return e.key = t, e
         }
 
-        function bu(t, e) {
+        function wu(t, e) {
             if ((r = t.length) > 0) {
                 for (var n, r, i, o = 0, l = t[0].length; o < l; ++o) {
                     for (i = n = 0; n < r; ++n) i += t[n][o][1] || 0;
                     if (i)
                         for (n = 0; n < r; ++n) t[n][o][1] /= i
                 }
-                pu(t, e)
+                vu(t, e)
             }
         }
 
-        function yu(t) {
-            return gu(t).reverse()
+        function xu(t) {
+            return bu(t).reverse()
         }
 
-        function $u(t) {
+        function _u(t) {
             u(t, "svelte-1gasvv0", ".distributions-container.svelte-1gasvv0{width:100%;height:100%;display:flex;flex-direction:column;gap:0.5em}.distributions-settings.svelte-1gasvv0{display:flex;align-items:center;gap:1em}.distribution-plots.svelte-1gasvv0{flex:1;overflow-y:auto;position:relative}.label-and-input.svelte-1gasvv0{display:flex;align-items:center;gap:0.25em}svg.svelte-1gasvv0,canvas.svelte-1gasvv0{position:absolute;left:0}")
         }
 
-        function wu(t, e, n) {
+        function ku(t, e, n) {
             const r = t.slice();
             return r[39] = e[n], r
         }
 
-        function xu(t, e, n) {
+        function Mu(t, e, n) {
             const r = t.slice();
             return r[42] = e[n], r[44] = n, r
         }
 
-        function _u(t, e, n) {
+        function Lu(t, e, n) {
             const r = t.slice();
             return r[45] = e[n], r
         }
 
-        function ku(t) {
+        function Au(t) {
             let e, n, r, i, o;
             return {
                 c() {
                     e = p("label"), n = p("input"), r = m("Normalize bar charts"), $(n, "type", "checkbox"), $(e, "class", "label-and-input svelte-1gasvv0")
                 },
                 m(l, a) {
                     d(l, e, a), c(e, n), n.checked = t[2], c(e, r), i || (o = y(n, "change", t[27]), i = !0)
@@ -9049,18 +9102,18 @@
                 },
                 d(t) {
                     t && f(e), i = !1, o()
                 }
             }
         }
 
-        function Mu(t) {
+        function Pu(t) {
             let e, n, r, i = ht(t[39].data),
                 o = [];
-            for (let e = 0; e < i.length; e += 1) o[e] = Pu(xu(t, i, e));
+            for (let e = 0; e < i.length; e += 1) o[e] = Tu(Mu(t, i, e));
             return n = new Va({
                 props: {
                     scale: t[12],
                     x: t[14].left,
                     label: t[2] ? "percent" : "count",
                     format: t[2] ? Qe("~%") : In
                 }
@@ -9075,16 +9128,16 @@
                     for (let t = 0; t < o.length; t += 1) o[t] && o[t].m(e, null);
                     yt(n, t, i), r = !0
                 },
                 p(t, r) {
                     if (4744 & r[0]) {
                         let n;
                         for (i = ht(t[39].data), n = 0; n < i.length; n += 1) {
-                            const l = xu(t, i, n);
-                            o[n] ? o[n].p(l, r) : (o[n] = Pu(l), o[n].c(), o[n].m(e, null))
+                            const l = Mu(t, i, n);
+                            o[n] ? o[n].p(l, r) : (o[n] = Tu(l), o[n].c(), o[n].m(e, null))
                         }
                         for (; n < o.length; n += 1) o[n].d(1);
                         o.length = i.length
                     }
                     const l = {};
                     4096 & r[0] && (l.scale = t[12]), 4 & r[0] && (l.label = t[2] ? "percent" : "count"), 4 & r[0] && (l.format = t[2] ? Qe("~%") : In), n.$set(l)
                 },
@@ -9096,128 +9149,128 @@
                 },
                 d(t) {
                     t && f(e), h(o, t), $t(n, t)
                 }
             }
         }
 
-        function Lu(t) {
+        function Su(t) {
             let e, n, r, i, o;
             return {
                 c() {
-                    e = g("rect"), $(e, "x", n = Ou(t[45].data[0], t[9][t[39].feature]) + 1), $(e, "width", r = Cu(t[9][t[39].feature]) - 2), $(e, "y", i = t[12](t[45][1])), $(e, "height", o = t[12](t[45][0]) - t[12](t[45][1]))
+                    e = g("rect"), $(e, "x", n = Bu(t[45].data[0], t[9][t[39].feature]) + 1), $(e, "width", r = ju(t[9][t[39].feature]) - 2), $(e, "y", i = t[12](t[45][1])), $(e, "height", o = t[12](t[45][0]) - t[12](t[45][1]))
                 },
                 m(t, n) {
                     d(t, e, n)
                 },
                 p(t, l) {
-                    520 & l[0] && n !== (n = Ou(t[45].data[0], t[9][t[39].feature]) + 1) && $(e, "x", n), 520 & l[0] && r !== (r = Cu(t[9][t[39].feature]) - 2) && $(e, "width", r), 4104 & l[0] && i !== (i = t[12](t[45][1])) && $(e, "y", i), 4104 & l[0] && o !== (o = t[12](t[45][0]) - t[12](t[45][1])) && $(e, "height", o)
+                    520 & l[0] && n !== (n = Bu(t[45].data[0], t[9][t[39].feature]) + 1) && $(e, "x", n), 520 & l[0] && r !== (r = ju(t[9][t[39].feature]) - 2) && $(e, "width", r), 4104 & l[0] && i !== (i = t[12](t[45][1])) && $(e, "y", i), 4104 & l[0] && o !== (o = t[12](t[45][0]) - t[12](t[45][1])) && $(e, "height", o)
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Au(t) {
-            let e, n = t[45][0] !== t[45][1] && Lu(t);
+        function zu(t) {
+            let e, n = t[45][0] !== t[45][1] && Su(t);
             return {
                 c() {
                     n && n.c(), e = b()
                 },
                 m(t, r) {
                     n && n.m(t, r), d(t, e, r)
                 },
                 p(t, r) {
-                    t[45][0] !== t[45][1] ? n ? n.p(t, r) : (n = Lu(t), n.c(), n.m(e.parentNode, e)) : n && (n.d(1), n = null)
+                    t[45][0] !== t[45][1] ? n ? n.p(t, r) : (n = Su(t), n.c(), n.m(e.parentNode, e)) : n && (n.d(1), n = null)
                 },
                 d(t) {
                     t && f(e), n && n.d(t)
                 }
             }
         }
 
-        function Pu(t) {
+        function Tu(t) {
             let e, n, r = ht(t[42]),
                 i = [];
-            for (let e = 0; e < r.length; e += 1) i[e] = Au(_u(t, r, e));
+            for (let e = 0; e < r.length; e += 1) i[e] = zu(Lu(t, r, e));
             return {
                 c() {
                     e = g("g");
                     for (let t = 0; t < i.length; t += 1) i[t].c();
                     $(e, "fill", n = t[7](t[44]))
                 },
                 m(t, n) {
                     d(t, e, n);
                     for (let t = 0; t < i.length; t += 1) i[t] && i[t].m(e, null)
                 },
                 p(t, o) {
                     if (4616 & o[0]) {
                         let n;
                         for (r = ht(t[42]), n = 0; n < r.length; n += 1) {
-                            const l = _u(t, r, n);
-                            i[n] ? i[n].p(l, o) : (i[n] = Au(l), i[n].c(), i[n].m(e, null))
+                            const l = Lu(t, r, n);
+                            i[n] ? i[n].p(l, o) : (i[n] = zu(l), i[n].c(), i[n].m(e, null))
                         }
                         for (; n < i.length; n += 1) i[n].d(1);
                         i.length = r.length
                     }
                     128 & o[0] && n !== (n = t[7](t[44])) && $(e, "fill", n)
                 },
                 d(t) {
                     t && f(e), h(i, t)
                 }
             }
         }
 
-        function Su(t) {
-            let e, n, r, i, o, l, a = "categorical" === t[39].kind && Mu(t);
+        function Nu(t) {
+            let e, n, r, i, o, l, a = "categorical" === t[39].kind && Pu(t);
             return r = new Ma({
                 props: {
                     scale: t[9][t[39].feature],
                     y: t[8].bandwidth() - t[14].bottom,
                     showBaseline: !0,
                     baselineColor: "var(--gray-6)",
                     tickColor: "var(--gray-6)",
                     integerOnly: "discrete" === t[11][t[39].feature].subkind,
-                    value_map: Nu(t[11][t[39].feature]),
+                    value_map: Du(t[11][t[39].feature]),
                     label: t[39].feature
                 }
             }), {
                 c() {
                     e = g("g"), a && a.c(), n = g("g"), bt(r.$$.fragment), $(n, "class", "x-axis"), $(n, "id", i = "axis-" + t[39].feature), $(e, "transform", o = "translate(0," + t[8](t[39].feature) + ")")
                 },
                 m(t, i) {
                     d(t, e, i), a && a.m(e, null), c(e, n), yt(r, n, null), l = !0
                 },
                 p(t, s) {
-                    "categorical" === t[39].kind ? a ? (a.p(t, s), 8 & s[0] && dt(a, 1)) : (a = Mu(t), a.c(), dt(a, 1), a.m(e, n)) : a && (ct(), ft(a, 1, 1, (() => {
+                    "categorical" === t[39].kind ? a ? (a.p(t, s), 8 & s[0] && dt(a, 1)) : (a = Pu(t), a.c(), dt(a, 1), a.m(e, n)) : a && (ct(), ft(a, 1, 1, (() => {
                         a = null
                     })), ut());
                     const c = {};
-                    520 & s[0] && (c.scale = t[9][t[39].feature]), 256 & s[0] && (c.y = t[8].bandwidth() - t[14].bottom), 2056 & s[0] && (c.integerOnly = "discrete" === t[11][t[39].feature].subkind), 2056 & s[0] && (c.value_map = Nu(t[11][t[39].feature])), 8 & s[0] && (c.label = t[39].feature), r.$set(c), (!l || 8 & s[0] && i !== (i = "axis-" + t[39].feature)) && $(n, "id", i), (!l || 264 & s[0] && o !== (o = "translate(0," + t[8](t[39].feature) + ")")) && $(e, "transform", o)
+                    520 & s[0] && (c.scale = t[9][t[39].feature]), 256 & s[0] && (c.y = t[8].bandwidth() - t[14].bottom), 2056 & s[0] && (c.integerOnly = "discrete" === t[11][t[39].feature].subkind), 2056 & s[0] && (c.value_map = Du(t[11][t[39].feature])), 8 & s[0] && (c.label = t[39].feature), r.$set(c), (!l || 8 & s[0] && i !== (i = "axis-" + t[39].feature)) && $(n, "id", i), (!l || 264 & s[0] && o !== (o = "translate(0," + t[8](t[39].feature) + ")")) && $(e, "transform", o)
                 },
                 i(t) {
                     l || (dt(a), dt(r.$$.fragment, t), l = !0)
                 },
                 o(t) {
                     ft(a), ft(r.$$.fragment, t), l = !1
                 },
                 d(t) {
                     t && f(e), a && a.d(), $t(r)
                 }
             }
         }
 
-        function zu(t) {
+        function Cu(t) {
             let e, n, r, i, o, l, a, s, u, b, y, w, x, k, M, L, A = t[10].length + "",
                 S = 1 === t[10].length ? "instance" : "instances",
-                z = t[13].length > 0 && ku(t),
+                z = t[13].length > 0 && Au(t),
                 T = ht(t[3]),
                 N = [];
-            for (let e = 0; e < T.length; e += 1) N[e] = Su(wu(t, T, e));
+            for (let e = 0; e < T.length; e += 1) N[e] = Nu(ku(t, T, e));
             const C = t => ft(N[t], 1, 1, (() => {
                 N[t] = null
             }));
             return {
                 c() {
                     e = p("div"), n = p("div"), z && z.c(), r = v(), i = p("div"), o = m(A), l = v(), a = m(S), s = m(" selected"), u = v(), b = p("div"), y = p("canvas"), w = v(), x = g("svg"), k = g("g");
                     for (let t = 0; t < N.length; t += 1) N[t].c();
@@ -9225,19 +9278,19 @@
                 },
                 m(f, h) {
                     d(f, e, h), c(e, n), z && z.m(n, null), c(n, r), c(n, i), c(i, o), c(i, l), c(i, a), c(i, s), c(e, u), c(e, b), c(b, y), t[28](y), c(b, w), c(b, x), c(x, k);
                     for (let t = 0; t < N.length; t += 1) N[t] && N[t].m(k, null);
                     t[29](k), M = P.observe(b, t[30].bind(b)), L = !0
                 },
                 p(t, e) {
-                    if (t[13].length > 0 ? z ? z.p(t, e) : (z = ku(t), z.c(), z.m(n, r)) : z && (z.d(1), z = null), (!L || 1024 & e[0]) && A !== (A = t[10].length + "") && _(o, A), (!L || 1024 & e[0]) && S !== (S = 1 === t[10].length ? "instance" : "instances") && _(a, S), 23436 & e[0]) {
+                    if (t[13].length > 0 ? z ? z.p(t, e) : (z = Au(t), z.c(), z.m(n, r)) : z && (z.d(1), z = null), (!L || 1024 & e[0]) && A !== (A = t[10].length + "") && _(o, A), (!L || 1024 & e[0]) && S !== (S = 1 === t[10].length ? "instance" : "instances") && _(a, S), 23436 & e[0]) {
                         let n;
                         for (T = ht(t[3]), n = 0; n < T.length; n += 1) {
-                            const r = wu(t, T, n);
-                            N[n] ? (N[n].p(r, e), dt(N[n], 1)) : (N[n] = Su(r), N[n].c(), dt(N[n], 1), N[n].m(k, null))
+                            const r = ku(t, T, n);
+                            N[n] ? (N[n].p(r, e), dt(N[n], 1)) : (N[n] = Nu(r), N[n].c(), dt(N[n], 1), N[n].m(k, null))
                         }
                         for (ct(), n = T.length; n < N.length; n += 1) C(n);
                         ut()
                     }(!L || 1 & e[0]) && $(x, "width", t[0]), (!L || 64 & e[0]) && $(x, "height", t[6])
                 },
                 i(t) {
                     if (!L) {
@@ -9252,32 +9305,32 @@
                 },
                 d(n) {
                     n && f(e), z && z.d(), t[28](null), h(N, n), t[29](null), M()
                 }
             }
         }
 
-        function Tu(t) {
+        function Ou(t) {
             return "categorical" === t.kind
         }
 
-        function Nu(t) {
+        function Du(t) {
             return "value_map" in t ? t.value_map : {}
         }
 
-        function Cu(t) {
+        function ju(t) {
             return t && "bandwidth" in t ? t.bandwidth() : 0
         }
 
-        function Ou(t, e) {
+        function Bu(t, e) {
             var n;
             return e && null !== (n = e(t)) && void 0 !== n ? n : 0
         }
 
-        function Du(t, e, n) {
+        function Eu(t, e, n) {
             let r, i, o, l, s, c, u, d, f, h, p, g, m, v, b, y, $;
             E(t, Qn, (t => n(25, b = t))), E(t, Zn, (t => n(11, y = t))), E(t, er, (t => n(26, $ = t)));
             let {
                 pd: w
             } = e, {
                 features: x
             } = e;
@@ -9361,40 +9414,40 @@
             return F((() => {
                 O && n(18, D = O.getContext("2d"))
             })), t.$$set = t => {
                 "pd" in t && n(15, w = t.pd), "features" in t && n(16, x = t.features)
             }, t.$$.update = () => {
                 2 & t.$$.dirty[0] && n(0, M = k ? k.width : 0), 2 & t.$$.dirty[0] && n(17, L = k ? k.height : 0), 229376 & t.$$.dirty[0] && n(6, r = Math.max(L, x.length * (30 * w.ice.num_clusters + _.top + _.bottom))), 32768 & t.$$.dirty[0] && n(23, i = zn(w).cluster_labels), 32768 & t.$$.dirty[0] && n(21, o = _n(w.ice.num_clusters)), 67584 & t.$$.dirty[0] && n(13, l = x.filter((t => "categorical" === y[t].kind))), 2097152 & t.$$.dirty[0] && n(7, s = Er().domain(o).range(Un)), 65600 & t.$$.dirty[0] && n(8, c = Ir().domain(x).range([0, r])), 67108864 & t.$$.dirty[0] && (u = _n($)), 67108864 & t.$$.dirty[0] && n(10, d = _n($)), 2097156 & t.$$.dirty[0] && n(24, f = function() {
                     var t = Gr([]),
-                        e = gu,
-                        n = pu,
-                        r = mu;
+                        e = bu,
+                        n = vu,
+                        r = yu;
 
                     function i(i) {
-                        var o, l, a = Array.from(t.apply(this, arguments), vu),
+                        var o, l, a = Array.from(t.apply(this, arguments), $u),
                             s = a.length,
                             c = -1;
                         for (const t of i)
                             for (o = 0, ++c; o < s; ++o)(a[o][c] = [0, +r(t, a[o].key, c, i)]).data = t;
                         for (o = 0, l = Yr(e(a)); o < s; ++o) a[l[o]].index = o;
                         return n(a, l), a
                     }
                     return i.keys = function(e) {
                         return arguments.length ? (t = "function" == typeof e ? e : Gr(Array.from(e)), i) : t
                     }, i.value = function(t) {
                         return arguments.length ? (r = "function" == typeof t ? t : Gr(+t), i) : r
                     }, i.order = function(t) {
-                        return arguments.length ? (e = null == t ? gu : "function" == typeof t ? t : Gr(Array.from(t)), i) : e
+                        return arguments.length ? (e = null == t ? bu : "function" == typeof t ? t : Gr(Array.from(t)), i) : e
                     }, i.offset = function(t) {
-                        return arguments.length ? (n = null == t ? pu : t, i) : n
+                        return arguments.length ? (n = null == t ? vu : t, i) : n
                     }, i
                 }().keys(o).value(((t, e) => {
                     var n;
                     return null !== (n = t[1].get(e)) && void 0 !== n ? n : 0
-                })).offset(A ? bu : pu).order(yu)), 67585 & t.$$.dirty[0] && n(9, h = Object.fromEntries(x.map((t => {
+                })).offset(A ? wu : vu).order(xu)), 67585 & t.$$.dirty[0] && n(9, h = Object.fromEntries(x.map((t => {
                     const e = y[t];
                     return [t, "quantitative" === e.kind ? on().domain([e.values[0], e.values[e.values.length - 1]]).range([_.left, M - _.right]) : Ir().domain(e.values).range([_.left, M - _.right])]
                 })))), 58788864 & t.$$.dirty[0] && n(3, P = x.map((t => {
                     if ("categorical" === y[t].kind) {
                         const e = wn(d, (t => t.length), (e => b[t][e]), (t => i[t]));
                         return {
                             feature: t,
@@ -9408,15 +9461,15 @@
                             kind: "quantitative",
                             data: Array.from(e, (([t, e]) => ({
                                 cluster: t,
                                 raincloud: e
                             })))
                         }
                     }
-                }))), 8 & t.$$.dirty[0] && n(22, p = Math.max(...P.filter(Tu).map((t => t.data)).flat(3))), 4194564 & t.$$.dirty[0] && n(12, g = on().domain([0, A ? 1 : p]).range([c.bandwidth() - _.bottom, _.top])), 2097408 & t.$$.dirty[0] && n(19, m = Ir().domain(o).range([_.top, c.bandwidth() - _.bottom]).paddingInner(.2).paddingOuter(.1)), 257 & t.$$.dirty[0] && n(20, v = ia().extent([
+                }))), 8 & t.$$.dirty[0] && n(22, p = Math.max(...P.filter(Ou).map((t => t.data)).flat(3))), 4194564 & t.$$.dirty[0] && n(12, g = on().domain([0, A ? 1 : p]).range([c.bandwidth() - _.bottom, _.top])), 2097408 & t.$$.dirty[0] && n(19, m = Ir().domain(o).range([_.top, c.bandwidth() - _.bottom]).paddingInner(.2).paddingOuter(.1)), 257 & t.$$.dirty[0] && n(20, v = ia().extent([
                     [_.left, -4 + c.bandwidth() - _.bottom],
                     [M - _.right, 4 + c.bandwidth() - _.bottom]
                 ]).on("start brush end", T)), 1114129 & t.$$.dirty[0] && N && x && M > 0 && async function(t) {
                     N && (await Q(), C = wo(N).selectAll(".x-axis"), C.call(t), C.call(t.clear))
                 }(v), 262241 & t.$$.dirty[0] && O && D && (En(O, D, M, r), j(D, h, c, m, s, P, M, r)), 787401 & t.$$.dirty[0] && j(D, h, c, m, s, P, M, r)
             }, [M, k, A, P, N, O, r, s, c, h, d, y, g, l, _, w, x, L, D, m, v, o, p, i, f, b, $, function() {
                 A = this.checked, n(2, A)
@@ -9428,31 +9481,31 @@
                 X[t ? "unshift" : "push"]((() => {
                     N = t, n(4, N)
                 }))
             }, function() {
                 k = a.entries.get(this)?.contentRect, n(1, k)
             }]
         }
-        const ju = class extends _t {
+        const Iu = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Du, zu, j, {
+                super(), wt(this, t, Eu, Cu, j, {
                     pd: 15,
                     features: 16
-                }, $u, [-1, -1])
+                }, _u, [-1, -1])
             }
         };
 
-        function Bu(t) {
+        function Ru(t) {
             u(t, "svelte-2s8sz0", ".pdpilot-plot-container.svelte-2s8sz0{width:100%;height:100%;position:relative}svg.svelte-2s8sz0,canvas.svelte-2s8sz0{position:absolute;top:var(--top);left:0}")
         }
 
-        function Eu(t) {
+        function Vu(t) {
             let e, n, r, i, o = t[21].left - t[28] + "px",
                 l = `${t[22]}px`;
-            const a = [Ru, Iu],
+            const a = [qu, Hu],
                 s = [];
 
             function c(t, e) {
                 return "interpolator" in t[18] ? 0 : 1
             }
             return n = c(t), r = s[n] = a[n](t), {
                 c() {
@@ -9475,23 +9528,23 @@
                 },
                 d(t) {
                     t && f(e), s[n].d()
                 }
             }
         }
 
-        function Iu(t) {
+        function Hu(t) {
             let e, n;
-            return e = new Yc({
+            return e = new Zc({
                 props: {
                     width: t[23] + t[27],
-                    height: Zu,
+                    height: ed,
                     color: t[18],
-                    marginLeft: Qu,
-                    marginRight: Qu,
+                    marginLeft: nd,
+                    marginRight: nd,
                     title: t[3]
                 }
             }), {
                 c() {
                     bt(e.$$.fragment)
                 },
                 m(t, r) {
@@ -9509,23 +9562,23 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Ru(t) {
+        function qu(t) {
             let e, n;
             return e = new wc({
                 props: {
                     width: t[23] + t[27],
-                    height: Zu,
+                    height: ed,
                     color: t[18],
-                    marginLeft: Qu,
-                    marginRight: Qu,
+                    marginLeft: nd,
+                    marginRight: nd,
                     title: t[3]
                 }
             }), {
                 c() {
                     bt(e.$$.fragment)
                 },
                 m(t, r) {
@@ -9543,31 +9596,31 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Vu(t) {
-            let e, n, r, i, o = t[16] && t[24].length > 0 && Hu(t),
-                l = t[8] && Wu(t),
-                a = t[9] && Uu(t);
+        function Fu(t) {
+            let e, n, r, i, o = t[16] && t[24].length > 0 && Wu(t),
+                l = t[8] && Uu(t),
+                a = t[9] && Ju(t);
             return {
                 c() {
                     o && o.c(), e = b(), l && l.c(), n = b(), a && a.c(), r = b()
                 },
                 m(t, s) {
                     o && o.m(t, s), d(t, e, s), l && l.m(t, s), d(t, n, s), a && a.m(t, s), d(t, r, s), i = !0
                 },
                 p(t, i) {
-                    t[16] && t[24].length > 0 ? o ? (o.p(t, i), 16842752 & i[0] && dt(o, 1)) : (o = Hu(t), o.c(), dt(o, 1), o.m(e.parentNode, e)) : o && (ct(), ft(o, 1, 1, (() => {
+                    t[16] && t[24].length > 0 ? o ? (o.p(t, i), 16842752 & i[0] && dt(o, 1)) : (o = Wu(t), o.c(), dt(o, 1), o.m(e.parentNode, e)) : o && (ct(), ft(o, 1, 1, (() => {
                         o = null
-                    })), ut()), t[8] ? l ? (l.p(t, i), 256 & i[0] && dt(l, 1)) : (l = Wu(t), l.c(), dt(l, 1), l.m(n.parentNode, n)) : l && (ct(), ft(l, 1, 1, (() => {
+                    })), ut()), t[8] ? l ? (l.p(t, i), 256 & i[0] && dt(l, 1)) : (l = Uu(t), l.c(), dt(l, 1), l.m(n.parentNode, n)) : l && (ct(), ft(l, 1, 1, (() => {
                         l = null
-                    })), ut()), t[9] ? a ? (a.p(t, i), 512 & i[0] && dt(a, 1)) : (a = Uu(t), a.c(), dt(a, 1), a.m(r.parentNode, r)) : a && (ct(), ft(a, 1, 1, (() => {
+                    })), ut()), t[9] ? a ? (a.p(t, i), 512 & i[0] && dt(a, 1)) : (a = Ju(t), a.c(), dt(a, 1), a.m(r.parentNode, r)) : a && (ct(), ft(a, 1, 1, (() => {
                         a = null
                     })), ut())
                 },
                 i(t) {
                     i || (dt(o), dt(l), dt(a), i = !0)
                 },
                 o(t) {
@@ -9575,17 +9628,17 @@
                 },
                 d(t) {
                     t && (f(e), f(n), f(r)), o && o.d(t), l && l.d(t), a && a.d(t)
                 }
             }
         }
 
-        function Hu(t) {
+        function Wu(t) {
             let e, n, r, i;
-            const o = [Fu, qu],
+            const o = [Xu, Ku],
                 l = [];
 
             function a(t, e) {
                 return "bandwidth" in t[20] ? 0 : 1
             }
             return e = a(t), n = l[e] = o[e](t), {
                 c() {
@@ -9608,15 +9661,15 @@
                 },
                 d(t) {
                     t && f(r), l[e].d(t)
                 }
             }
         }
 
-        function qu(t) {
+        function Ku(t) {
             let e, n;
             return e = new Qa({
                 props: {
                     data: t[16],
                     fill: Kn,
                     x: t[20],
                     height: t[13],
@@ -9644,15 +9697,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Fu(t) {
+        function Xu(t) {
             let e, n;
             return e = new ds({
                 props: {
                     data: t[16],
                     fill: Kn,
                     x: t[20],
                     height: t[13],
@@ -9680,17 +9733,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Wu(t) {
+        function Uu(t) {
             let e, n, r, i;
-            const o = [Xu, Ku],
+            const o = [Gu, Yu],
                 l = [];
 
             function a(t, e) {
                 return "bandwidth" in t[20] ? 0 : 1
             }
             return e = a(t), n = l[e] = o[e](t), {
                 c() {
@@ -9713,15 +9766,15 @@
                 },
                 d(t) {
                     t && f(r), l[e].d(t)
                 }
             }
         }
 
-        function Ku(t) {
+        function Yu(t) {
             let e, n;
             return e = new Qa({
                 props: {
                     data: t[8],
                     fill: t[26] ? "none" : "var(--gray-3)",
                     stroke: t[26] ? "var(--black)" : "none",
                     x: t[20],
@@ -9750,15 +9803,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Xu(t) {
+        function Gu(t) {
             let e, n;
             return e = new ds({
                 props: {
                     data: t[8],
                     fill: t[26] ? "none" : "var(--gray-3)",
                     stroke: t[26] ? "var(--black)" : "none",
                     x: t[20],
@@ -9787,17 +9840,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Uu(t) {
+        function Ju(t) {
             let e, n, r, i;
-            const o = [Gu, Yu],
+            const o = [Qu, Zu],
                 l = [];
 
             function a(t, e) {
                 return "bandwidth" in t[19] ? 0 : 1
             }
             return e = a(t), n = l[e] = o[e](t), {
                 c() {
@@ -9820,15 +9873,15 @@
                 },
                 d(t) {
                     t && f(r), l[e].d(t)
                 }
             }
         }
 
-        function Yu(t) {
+        function Zu(t) {
             let e, n;
             return e = new Qa({
                 props: {
                     data: t[9],
                     x: t[19],
                     height: t[13],
                     direction: "vertical",
@@ -9853,15 +9906,15 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Gu(t) {
+        function Qu(t) {
             let e, n;
             return e = new ds({
                 props: {
                     data: t[9],
                     x: t[19],
                     height: t[13],
                     direction: "vertical",
@@ -9886,17 +9939,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Ju(t) {
-            let e, n, r, i, o, l, a, s, u, h = `${Zu+t[22]}px`,
-                m = "" !== t[3] && Eu(t);
+        function td(t) {
+            let e, n, r, i, o, l, a, s, u, h = `${ed+t[22]}px`,
+                m = "" !== t[3] && Vu(t);
             l = new Ma({
                 props: {
                     scale: t[20],
                     y: t[17] - t[21].bottom,
                     label: t[1],
                     integerOnly: t[4],
                     value_map: t[6]
@@ -9906,48 +9959,48 @@
                     scale: t[19],
                     x: t[21].left,
                     label: t[2],
                     integerOnly: t[5],
                     value_map: t[7]
                 }
             });
-            let b = t[10] && Vu(t);
+            let b = t[10] && Fu(t);
             return {
                 c() {
                     e = p("div"), m && m.c(), n = v(), r = p("canvas"), i = v(), o = g("svg"), bt(l.$$.fragment), bt(a.$$.fragment), s = g("g"), b && b.c(), $(r, "class", "svelte-2s8sz0"), $(o, "width", t[0]), $(o, "height", t[17]), $(o, "class", "svelte-2s8sz0"), $(e, "class", "pdpilot-plot-container svelte-2s8sz0"), M(e, "--top", h)
                 },
                 m(f, h) {
                     d(f, e, h), m && m.m(e, null), c(e, n), c(e, r), t[53](r), c(e, i), c(e, o), yt(l, o, null), yt(a, o, null), c(o, s), t[54](s), b && b.m(o, null), u = !0
                 },
                 p(t, r) {
-                    "" !== t[3] ? m ? (m.p(t, r), 8 & r[0] && dt(m, 1)) : (m = Eu(t), m.c(), dt(m, 1), m.m(e, n)) : m && (ct(), ft(m, 1, 1, (() => {
+                    "" !== t[3] ? m ? (m.p(t, r), 8 & r[0] && dt(m, 1)) : (m = Vu(t), m.c(), dt(m, 1), m.m(e, n)) : m && (ct(), ft(m, 1, 1, (() => {
                         m = null
                     })), ut());
                     const i = {};
                     1048576 & r[0] && (i.scale = t[20]), 2228224 & r[0] && (i.y = t[17] - t[21].bottom), 2 & r[0] && (i.label = t[1]), 16 & r[0] && (i.integerOnly = t[4]), 64 & r[0] && (i.value_map = t[6]), l.$set(i);
                     const s = {};
-                    524288 & r[0] && (s.scale = t[19]), 2097152 & r[0] && (s.x = t[21].left), 4 & r[0] && (s.label = t[2]), 32 & r[0] && (s.integerOnly = t[5]), 128 & r[0] && (s.value_map = t[7]), a.$set(s), t[10] ? b ? (b.p(t, r), 1024 & r[0] && dt(b, 1)) : (b = Vu(t), b.c(), dt(b, 1), b.m(o, null)) : b && (ct(), ft(b, 1, 1, (() => {
+                    524288 & r[0] && (s.scale = t[19]), 2097152 & r[0] && (s.x = t[21].left), 4 & r[0] && (s.label = t[2]), 32 & r[0] && (s.integerOnly = t[5]), 128 & r[0] && (s.value_map = t[7]), a.$set(s), t[10] ? b ? (b.p(t, r), 1024 & r[0] && dt(b, 1)) : (b = Fu(t), b.c(), dt(b, 1), b.m(o, null)) : b && (ct(), ft(b, 1, 1, (() => {
                         b = null
-                    })), ut()), (!u || 1 & r[0]) && $(o, "width", t[0]), (!u || 131072 & r[0]) && $(o, "height", t[17]), 4194304 & r[0] && h !== (h = `${Zu+t[22]}px`) && M(e, "--top", h)
+                    })), ut()), (!u || 1 & r[0]) && $(o, "width", t[0]), (!u || 131072 & r[0]) && $(o, "height", t[17]), 4194304 & r[0] && h !== (h = `${ed+t[22]}px`) && M(e, "--top", h)
                 },
                 i(t) {
                     u || (dt(m), dt(l.$$.fragment, t), dt(a.$$.fragment, t), dt(b), u = !0)
                 },
                 o(t) {
                     ft(m), ft(l.$$.fragment, t), ft(a.$$.fragment, t), ft(b), u = !1
                 },
                 d(n) {
                     n && f(e), m && m.d(), t[53](null), $t(l), $t(a), t[54](null), b && b.d()
                 }
             }
         }
-        const Zu = 24,
-            Qu = 10;
+        const ed = 24,
+            nd = 10;
 
-        function td(t, e, n) {
+        function rd(t, e, n) {
             let r, i, o, l, a, s, c, u, d, f, h, p, g, m, v, b, y, $, w, x, _;
             E(t, kr, (t => n(50, y = t))), E(t, fr, (t => n(24, $ = t))), E(t, Pr, (t => n(51, w = t))), E(t, Mr, (t => n(52, x = t))), E(t, Lr, (t => n(56, _ = t)));
             let k, M, {
                     width: L
                 } = e,
                 {
                     height: A
@@ -10088,36 +10141,36 @@
                 "width" in t && n(0, L = t.width), "height" in t && n(29, A = t.height), "xValues" in t && n(30, P = t.xValues), "yValues" in t && n(31, S = t.yValues), "colorValues" in t && n(32, z = t.colorValues), "xKind" in t && n(33, T = t.xKind), "yKind" in t && n(34, N = t.yKind), "colorKind" in t && n(35, C = t.colorKind), "xDomain" in t && n(36, O = t.xDomain), "yDomain" in t && n(37, D = t.yDomain), "colorDomain" in t && n(38, j = t.colorDomain), "colorScheme" in t && n(39, B = t.colorScheme), "xLabel" in t && n(1, I = t.xLabel), "yLabel" in t && n(2, V = t.yLabel), "colorLabel" in t && n(3, H = t.colorLabel), "xAxisIntegerOnly" in t && n(4, q = t.xAxisIntegerOnly), "yAxisIntegerOnly" in t && n(5, W = t.yAxisIntegerOnly), "xAxisValueMap" in t && n(6, K = t.xAxisValueMap), "yAxisValueMap" in t && n(7, U = t.yAxisValueMap), "xDistribution" in t && n(8, Y = t.xDistribution), "yDistribution" in t && n(9, G = t.yDistribution), "opacity" in t && n(40, J = t.opacity), "allowBrushing" in t && n(41, Z = t.allowBrushing), "showMarginalDistribution" in t && n(10, Q = t.showMarginalDistribution), "marginTop" in t && n(11, tt = t.marginTop), "marginRight" in t && n(12, et = t.marginRight), "marginalPlotHeight" in t && n(13, nt = t.marginalPlotHeight)
             }, t.$$.update = () => {
                 6144 & t.$$.dirty[0] && n(48, r = {
                     top: tt,
                     right: et,
                     bottom: 35,
                     left: 50
-                }), 536870913 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(23, i = Math.min(L - r.left - r.right, A - Zu - r.top - r.bottom)), 8388609 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(47, o = (L - i - r.left - r.right) / 2), 545259520 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(49, l = (A - Zu - i - r.top - r.bottom) / 2), 8 & t.$$.dirty[0] && n(28, a = "" === H ? Qu : 0), 8 & t.$$.dirty[0] && n(27, s = "" === H ? 2 * Qu : Qu), 8 & t.$$.dirty[0] | 262144 & t.$$.dirty[1] && n(22, c = "" !== H ? l : 0), 4194304 & t.$$.dirty[0] | 458752 & t.$$.dirty[1] && n(21, u = {
+                }), 536870913 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(23, i = Math.min(L - r.left - r.right, A - ed - r.top - r.bottom)), 8388609 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(47, o = (L - i - r.left - r.right) / 2), 545259520 & t.$$.dirty[0] | 131072 & t.$$.dirty[1] && n(49, l = (A - ed - i - r.top - r.bottom) / 2), 8 & t.$$.dirty[0] && n(28, a = "" === H ? nd : 0), 8 & t.$$.dirty[0] && n(27, s = "" === H ? 2 * nd : nd), 8 & t.$$.dirty[0] | 262144 & t.$$.dirty[1] && n(22, c = "" !== H ? l : 0), 4194304 & t.$$.dirty[0] | 458752 & t.$$.dirty[1] && n(21, u = {
                     top: r.top + l - c,
                     right: r.right + o,
                     bottom: r.bottom + l,
                     left: r.left + o
-                }), 541065216 & t.$$.dirty[0] && n(17, d = Math.max(A - Zu - c, 0)), 2097153 & t.$$.dirty[0] | 36 & t.$$.dirty[1] && n(20, f = "quantitative" === T ? on().domain(O).range([u.left, L - u.right]) : Ir().domain(O).paddingInner(.25).range([u.left, L - u.right])), 2228224 & t.$$.dirty[0] | 72 & t.$$.dirty[1] && n(19, h = "quantitative" === N ? on().domain(D).range([d - u.bottom, u.top]) : Ir().domain(D).paddingInner(.25).range([d - u.bottom, u.top])), 400 & t.$$.dirty[1] && n(18, p = "quantitative" === C ? an().domain(j).interpolator((t => Rc(rt(t)))) : Er().domain(j).range("highlight" === B ? ["rgb(145, 145, 145)", Kn] : ["#db5c39", "#5c39db"])), 1073741824 & t.$$.dirty[0] && (g = _n(P.length)), 2228225 & t.$$.dirty[0] && n(46, m = oa().extent([
+                }), 541065216 & t.$$.dirty[0] && n(17, d = Math.max(A - ed - c, 0)), 2097153 & t.$$.dirty[0] | 36 & t.$$.dirty[1] && n(20, f = "quantitative" === T ? on().domain(O).range([u.left, L - u.right]) : Ir().domain(O).paddingInner(.25).range([u.left, L - u.right])), 2228224 & t.$$.dirty[0] | 72 & t.$$.dirty[1] && n(19, h = "quantitative" === N ? on().domain(D).range([d - u.bottom, u.top]) : Ir().domain(D).paddingInner(.25).range([d - u.bottom, u.top])), 400 & t.$$.dirty[1] && n(18, p = "quantitative" === C ? an().domain(j).interpolator((t => qc(rt(t)))) : Er().domain(j).range("highlight" === B ? ["rgb(145, 145, 145)", Kn] : ["#db5c39", "#5c39db"])), 1073741824 & t.$$.dirty[0] && (g = _n(P.length)), 2228225 & t.$$.dirty[0] && n(46, m = oa().extent([
                     [u.left - 2, u.top - 2],
                     [L - u.right + 2, d - u.bottom + 2]
                 ]).on("start", ct).on("brush", ut).on("end", dt)), 163841 & t.$$.dirty[0] | 50176 & t.$$.dirty[1] && it && Z && L > 0 && d > 0 && (n(45, ot = wo(it)), ot.call(m)), 2158592 & t.$$.dirty[1] && ot && x && at && !st && ot.call(m.clear), 2 & t.$$.dirty[0] | 1049600 & t.$$.dirty[1] && n(16, lt = Z ? w.get(I) : void 0), 16842752 & t.$$.dirty[0] && n(26, v = lt && $.length > 0), 65792 & t.$$.dirty[0] && n(25, b = Y ? Hn(Y, lt) : 0), 147457 & t.$$.dirty[0] | 2048 & t.$$.dirty[1] && k && M && (En(k, M, L, d), dc(M, f, h, p, P, S, z, y, L, d, 2, J)), 1075707905 & t.$$.dirty[0] | 526851 & t.$$.dirty[1] && dc(M, f, h, p, P, S, z, y, L, d, 2, J)
             }, [L, I, V, H, q, W, K, U, Y, G, Q, tt, et, nt, k, it, lt, d, p, h, f, u, c, i, $, b, v, s, a, A, P, S, z, T, N, C, O, D, j, B, J, Z, M, at, st, ot, m, o, r, l, y, w, x, function(t) {
                 X[t ? "unshift" : "push"]((() => {
                     k = t, n(14, k)
                 }))
             }, function(t) {
                 X[t ? "unshift" : "push"]((() => {
                     it = t, n(15, it)
                 }))
             }]
         }
-        const ed = class extends _t {
+        const id = class extends _t {
             constructor(t) {
-                super(), wt(this, t, td, Ju, j, {
+                super(), wt(this, t, rd, td, j, {
                     width: 0,
                     height: 29,
                     xValues: 30,
                     yValues: 31,
                     colorValues: 32,
                     xKind: 33,
                     yKind: 34,
@@ -10137,28 +10190,28 @@
                     yDistribution: 9,
                     opacity: 40,
                     allowBrushing: 41,
                     showMarginalDistribution: 10,
                     marginTop: 11,
                     marginRight: 12,
                     marginalPlotHeight: 13
-                }, Bu, [-1, -1])
+                }, Ru, [-1, -1])
             }
         };
 
-        function nd(t) {
+        function od(t) {
             u(t, "svelte-tm4cy6", ".segmented-control-container.svelte-tm4cy6.svelte-tm4cy6{display:flex;gap:0.25em;align-items:center}.segmented-control-buttons-row.svelte-tm4cy6.svelte-tm4cy6{display:inline-grid;grid-auto-columns:1fr;grid-auto-flow:column}.segmented-control-buttons-row.svelte-tm4cy6 button.svelte-tm4cy6{border-radius:0;border-left:none;padding:0.0625em 0.125em}.segmented-control-buttons-row.svelte-tm4cy6 button.svelte-tm4cy6:first-child{border-top-left-radius:0.25em;border-bottom-left-radius:0.25em;border-left:1px solid var(--blue)}.segmented-control-buttons-row.svelte-tm4cy6 button.svelte-tm4cy6:last-child{border-top-right-radius:0.25em;border-bottom-right-radius:0.25em}.segmented-control-buttons-row.svelte-tm4cy6 button.selected-segment.svelte-tm4cy6{color:white;background-color:var(--blue)}.segmented-control-buttons-row.svelte-tm4cy6 button.selected-segment.svelte-tm4cy6:active{color:white;background-color:var(--dark-blue);border-color:var(--dark-blue)}")
         }
 
-        function rd(t, e, n) {
+        function ld(t, e, n) {
             const r = t.slice();
             return r[5] = e[n].value, r[6] = e[n].label, r[7] = e[n].enabled, r
         }
 
-        function id(t) {
+        function ad(t) {
             let e, n;
             return {
                 c() {
                     e = p("div"), n = m(t[2]), $(e, "class", "pdpilot-bold")
                 },
                 m(t, r) {
                     d(t, e, r), c(e, n)
@@ -10168,15 +10221,15 @@
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function od(t) {
+        function sd(t) {
             let e, n, r, i, o, l = t[6] + "";
 
             function a() {
                 return t[4](t[5])
             }
             return {
                 c() {
@@ -10190,49 +10243,49 @@
                 },
                 d(t) {
                     t && f(e), i = !1, o()
                 }
             }
         }
 
-        function ld(t) {
-            let e, n, r, i = t[2] && id(t),
+        function cd(t) {
+            let e, n, r, i = t[2] && ad(t),
                 o = ht(t[1]),
                 l = [];
-            for (let e = 0; e < o.length; e += 1) l[e] = od(rd(t, o, e));
+            for (let e = 0; e < o.length; e += 1) l[e] = sd(ld(t, o, e));
             return {
                 c() {
                     e = p("div"), i && i.c(), n = v(), r = p("div");
                     for (let t = 0; t < l.length; t += 1) l[t].c();
                     $(r, "class", "segmented-control-buttons-row svelte-tm4cy6"), $(e, "class", "segmented-control-container svelte-tm4cy6")
                 },
                 m(t, o) {
                     d(t, e, o), i && i.m(e, null), c(e, n), c(e, r);
                     for (let t = 0; t < l.length; t += 1) l[t] && l[t].m(r, null)
                 },
                 p(t, [a]) {
-                    if (t[2] ? i ? i.p(t, a) : (i = id(t), i.c(), i.m(e, n)) : i && (i.d(1), i = null), 11 & a) {
+                    if (t[2] ? i ? i.p(t, a) : (i = ad(t), i.c(), i.m(e, n)) : i && (i.d(1), i = null), 11 & a) {
                         let e;
                         for (o = ht(t[1]), e = 0; e < o.length; e += 1) {
-                            const n = rd(t, o, e);
-                            l[e] ? l[e].p(n, a) : (l[e] = od(n), l[e].c(), l[e].m(r, null))
+                            const n = ld(t, o, e);
+                            l[e] ? l[e].p(n, a) : (l[e] = sd(n), l[e].c(), l[e].m(r, null))
                         }
                         for (; e < l.length; e += 1) l[e].d(1);
                         l.length = o.length
                     }
                 },
                 i: T,
                 o: T,
                 d(t) {
                     t && f(e), i && i.d(), h(l, t)
                 }
             }
         }
 
-        function ad(t, e, n) {
+        function ud(t, e, n) {
             let {
                 segments: r
             } = e, {
                 selectedValue: i
             } = e, {
                 title: o = ""
             } = e;
@@ -10240,46 +10293,46 @@
             function l(t) {
                 n(0, i = t)
             }
             return t.$$set = t => {
                 "segments" in t && n(1, r = t.segments), "selectedValue" in t && n(0, i = t.selectedValue), "title" in t && n(2, o = t.title)
             }, [i, r, o, l, t => l(t)]
         }
-        const sd = class extends _t {
+        const dd = class extends _t {
             constructor(t) {
-                super(), wt(this, t, ad, ld, j, {
+                super(), wt(this, t, ud, cd, j, {
                     segments: 1,
                     selectedValue: 0,
                     title: 2
-                }, nd)
+                }, od)
             }
         };
 
-        function cd(t) {
+        function fd(t) {
             u(t, "svelte-a1f3se", ".one-way-detailed-pdp-container.svelte-a1f3se{display:flex;width:100%;height:100%}.pdpilot-no-clusters-message.svelte-a1f3se{flex:1;text-align:center;align-self:center}.pdpilot-half.svelte-a1f3se{flex:1;display:flex;flex-direction:column}.pdpilot-half-vis.svelte-a1f3se{flex:1}.pdpilot-vertical-divider.svelte-a1f3se{width:1px;margin:0 1em;background-color:var(--gray-1)}")
         }
 
-        function ud(t) {
+        function hd(t) {
             let e, n, r, i, o, l, a, s, u, h, g, m, b, y, w, x, _, k, L, A, S, z = ("cluster-lines" === t[5] ? .25 : .5) + "em",
                 T = ("cluster-descriptions" === t[4] ? .25 : .5) + "em";
 
             function N(e) {
                 t[21](e)
             }
             let C = {
                 segments: t[19],
                 title: "ICE Plot"
             };
 
             function O(e) {
                 t[23](e)
             }
-            void 0 !== t[5] && (C.selectedValue = t[5]), r = new sd({
+            void 0 !== t[5] && (C.selectedValue = t[5]), r = new dd({
                 props: C
-            }), X.push((() => vt(r, "selectedValue", N))), a = new hu({
+            }), X.push((() => vt(r, "selectedValue", N))), a = new mu({
                 props: {
                     pd: t[0],
                     width: t[11],
                     height: t[10],
                     scaleLocally: t[12],
                     showMarginalDistribution: !1,
                     marginTop: "cluster-lines" === t[5] ? 0 : 10,
@@ -10290,18 +10343,18 @@
                     showColorLegend: !1
                 }
             });
             let D = {
                 segments: t[6],
                 title: "Context"
             };
-            void 0 !== t[4] && (D.selectedValue = t[4]), y = new sd({
+            void 0 !== t[4] && (D.selectedValue = t[4]), y = new dd({
                 props: D
             }), X.push((() => vt(y, "selectedValue", O)));
-            const j = [hd, fd],
+            const j = [md, gd],
                 B = [];
 
             function E(t, e) {
                 return "cluster-descriptions" === t[4] ? 0 : "scatterplot" === t[4] ? 1 : -1
             }
             return ~(k = E(t)) && (L = B[k] = j[k](t)), {
                 c() {
@@ -10330,15 +10383,15 @@
                 },
                 d(t) {
                     t && (f(e), f(u), f(h), f(g), f(m)), $t(r), $t(a), s(), $t(y), ~k && B[k].d(), A()
                 }
             }
         }
 
-        function dd(t) {
+        function pd(t) {
             let e;
             return {
                 c() {
                     e = p("div"), e.textContent = "This feature does not have enough distinct clusters of ICE lines.", $(e, "class", "pdpilot-no-clusters-message svelte-a1f3se")
                 },
                 m(t, n) {
                     d(t, e, n)
@@ -10348,17 +10401,17 @@
                 o: T,
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function fd(t) {
+        function gd(t) {
             let e, n;
-            return e = new ed({
+            return e = new id({
                 props: {
                     width: t[9],
                     height: t[8],
                     xValues: t[13][t[0].x_feature],
                     yValues: t[14],
                     colorValues: Array.from({
                         length: t[15]
@@ -10367,28 +10420,28 @@
                     yKind: t[17] ? "categorical" : "quantitative",
                     colorKind: "categorical",
                     xDomain: "categorical" === t[1].kind ? t[0].x_values : [t[0].x_values[0], t[0].x_values[t[0].x_values.length - 1]],
                     yDomain: t[18],
                     colorDomain: [0, 1],
                     colorScheme: "highlight",
                     xLabel: t[0].x_feature,
-                    yLabel: "Ground Truth",
+                    yLabel: "Ground truth",
                     colorLabel: "",
                     xAxisIntegerOnly: "discrete" === t[1].subkind,
                     yAxisIntegerOnly: !1,
                     xAxisValueMap: "value_map" in t[1] ? t[1].value_map : {},
                     yAxisValueMap: {},
                     xDistribution: t[1].distribution,
                     yDistribution: null,
                     opacity: .5,
                     allowBrushing: !0,
                     showMarginalDistribution: !0,
-                    marginTop: gd + 3,
-                    marginRight: gd + 3,
-                    marginalPlotHeight: gd
+                    marginTop: bd + 3,
+                    marginRight: bd + 3,
+                    marginalPlotHeight: bd
                 }
             }), {
                 c() {
                     bt(e.$$.fragment)
                 },
                 m(t, r) {
                     yt(e, t, r), n = !0
@@ -10407,17 +10460,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function hd(t) {
+        function md(t) {
             let e, n;
-            return e = new ju({
+            return e = new Iu({
                 props: {
                     pd: t[0],
                     features: zn(t[0]).interacting_features
                 }
             }), e.$on("filter", t[20]), {
                 c() {
                     bt(e.$$.fragment)
@@ -10437,17 +10490,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function pd(t) {
+        function vd(t) {
             let e, n, r, i;
-            const o = [dd, ud],
+            const o = [pd, hd],
                 l = [];
 
             function a(t, e) {
                 return "cluster-lines" === t[5] && 1 === t[0].ice.num_clusters ? 0 : 1
             }
             return n = a(t), r = l[n] = o[n](t), {
                 c() {
@@ -10469,17 +10522,17 @@
                     ft(r), i = !1
                 },
                 d(t) {
                     t && f(e), l[n].d()
                 }
             }
         }
-        const gd = 50;
+        const bd = 50;
 
-        function md(t, e, n) {
+        function yd(t, e, n) {
             let r, i, o, l, s, c, u, d, f, h, p, g, m;
             E(t, xr, (t => n(4, s = t))), E(t, wr, (t => n(5, c = t))), E(t, _r, (t => n(12, u = t))), E(t, Qn, (t => n(13, d = t))), E(t, tr, (t => n(14, f = t))), E(t, er, (t => n(15, h = t))), E(t, Ar, (t => n(16, p = t))), E(t, vr, (t => n(17, g = t))), E(t, br, (t => n(18, m = t)));
             let v, b, {
                     pd: y
                 } = e,
                 {
                     featureInfo: $
@@ -10518,59 +10571,59 @@
                 v = a.entries.get(this)?.contentRect, n(2, v)
             }, function(t) {
                 s = t, xr.set(s)
             }, (t, e) => p.has(e) ? 1 : 0, function() {
                 b = a.entries.get(this)?.contentRect, n(3, b)
             }]
         }
-        const vd = class extends _t {
+        const $d = class extends _t {
             constructor(t) {
-                super(), wt(this, t, md, pd, j, {
+                super(), wt(this, t, yd, vd, j, {
                     pd: 0,
                     featureInfo: 1
-                }, cd)
+                }, fd)
             }
         };
 
-        function bd(t) {
+        function wd(t) {
             u(t, "svelte-jg5wjz", ".two-way-pdp-grid.svelte-jg5wjz{display:grid;width:100%;height:100%;grid-template-columns:1fr 1fr 1fr;grid-template-areas:'two-way-interaction two-way-pdp scatter'}")
         }
 
-        function yd(t) {
+        function xd(t) {
             let e, n, r, i, o, l, a, s, u, h, g;
-            return r = new hu({
+            return r = new mu({
                 props: {
                     pd: t[0],
                     width: t[4],
                     height: t[5],
                     scaleLocally: t[6],
                     showMarginalPdp: !0,
-                    marginTop: $d + 1,
-                    marginRight: $d + 1,
-                    marginalPlotHeight: $d,
+                    marginTop: _d + 1,
+                    marginRight: _d + 1,
+                    marginalPlotHeight: _d,
                     iceLevel: "lines",
                     colorShows: "interactions",
                     showColorLegend: !0,
                     colorLegendTitle: "Interactions"
                 }
-            }), l = new hu({
+            }), l = new mu({
                 props: {
                     pd: t[0],
                     width: t[4],
                     height: t[5],
                     scaleLocally: t[6],
                     showMarginalPdp: !0,
-                    marginTop: $d + 1,
-                    marginRight: $d + 1,
-                    marginalPlotHeight: $d,
+                    marginTop: _d + 1,
+                    marginRight: _d + 1,
+                    marginalPlotHeight: _d,
                     iceLevel: "lines",
                     showColorLegend: !0,
                     colorLegendTitle: "Predictions"
                 }
-            }), u = new ed({
+            }), u = new id({
                 props: {
                     width: t[4],
                     height: t[5],
                     xValues: t[7][t[0].x_feature],
                     yValues: t[7][t[0].y_feature],
                     colorValues: t[8],
                     xKind: t[1].kind,
@@ -10578,27 +10631,27 @@
                     colorKind: t[9] ? "categorical" : "quantitative",
                     xDomain: "categorical" === t[1].kind ? t[0].x_axis : [t[0].x_axis[0], t[0].x_axis[t[0].x_axis.length - 1]],
                     yDomain: "categorical" === t[10][t[0].y_feature].kind ? t[0].y_axis : [t[0].y_axis[0], t[0].y_axis[t[0].y_axis.length - 1]],
                     colorDomain: t[11],
                     colorScheme: t[9] ? "classes" : "sequential",
                     xLabel: t[0].x_feature,
                     yLabel: t[0].y_feature,
-                    colorLabel: "Ground Truth",
+                    colorLabel: "Ground truth",
                     xAxisIntegerOnly: "discrete" === t[1].subkind,
                     yAxisIntegerOnly: "discrete" === t[2].subkind,
                     xAxisValueMap: "value_map" in t[1] ? t[1].value_map : {},
                     yAxisValueMap: "value_map" in t[2] ? t[2].value_map : {},
                     xDistribution: t[1].distribution,
                     yDistribution: t[2].distribution,
                     opacity: 1,
                     allowBrushing: !1,
                     showMarginalDistribution: !0,
-                    marginTop: $d + 3,
-                    marginRight: $d + 3,
-                    marginalPlotHeight: $d
+                    marginTop: _d + 3,
+                    marginRight: _d + 3,
+                    marginalPlotHeight: _d
                 }
             }), {
                 c() {
                     e = p("div"), n = p("div"), bt(r.$$.fragment), i = v(), o = p("div"), bt(l.$$.fragment), a = v(), s = p("div"), bt(u.$$.fragment), M(n, "grid-area", "two-way-interaction"), M(o, "grid-area", "two-way-pdp"), M(s, "grid-area", "scatter"), $(e, "class", "two-way-pdp-grid svelte-jg5wjz")
                 },
                 m(f, p) {
                     d(f, e, p), c(e, n), yt(r, n, null), c(e, i), c(e, o), yt(l, o, null), c(e, a), c(e, s), yt(u, s, null), h = P.observe(e, t[13].bind(e)), g = !0
@@ -10618,17 +10671,17 @@
                     ft(r.$$.fragment, t), ft(l.$$.fragment, t), ft(u.$$.fragment, t), g = !1
                 },
                 d(t) {
                     t && f(e), $t(r), $t(l), $t(u), h()
                 }
             }
         }
-        const $d = 50;
+        const _d = 50;
 
-        function wd(t, e, n) {
+        function kd(t, e, n) {
             let r, i, o, l, s, c, u, d, f;
             E(t, _r, (t => n(6, l = t))), E(t, Qn, (t => n(7, s = t))), E(t, tr, (t => n(8, c = t))), E(t, vr, (t => n(9, u = t))), E(t, Zn, (t => n(10, d = t))), E(t, br, (t => n(11, f = t)));
             let h, {
                     pd: p
                 } = e,
                 {
                     xFeatureInfo: g
@@ -10640,39 +10693,39 @@
                 "pd" in t && n(0, p = t.pd), "xFeatureInfo" in t && n(1, g = t.xFeatureInfo), "yFeatureInfo" in t && n(2, m = t.yFeatureInfo)
             }, t.$$.update = () => {
                 8 & t.$$.dirty && n(12, r = h ? h.width : 0), 8 & t.$$.dirty && n(5, i = h ? h.height : 0), 4096 & t.$$.dirty && n(4, o = r / 3)
             }, [p, g, m, h, o, i, l, s, c, u, d, f, r, function() {
                 h = a.entries.get(this)?.contentRect, n(3, h)
             }]
         }
-        const xd = class extends _t {
+        const Md = class extends _t {
             constructor(t) {
-                super(), wt(this, t, wd, yd, j, {
+                super(), wt(this, t, kd, xd, j, {
                     pd: 0,
                     xFeatureInfo: 1,
                     yFeatureInfo: 2
-                }, bd)
+                }, wd)
             }
         };
 
-        function _d(t) {
+        function Ld(t) {
             u(t, "svelte-1oprcpz", ".zoomed-pdp-container.svelte-1oprcpz.svelte-1oprcpz{width:100%;height:100%;display:flex;flex-direction:column}.zoomed-pdp-header.svelte-1oprcpz.svelte-1oprcpz{height:2em;display:flex;align-items:center;background-color:white;gap:1.5em;padding-left:0.5em;padding-right:0.5em;border-bottom:1px solid var(--gray-1)}.feature-selects.svelte-1oprcpz.svelte-1oprcpz{flex:0 1 auto;min-width:0;display:flex;align-items:center;gap:0.5em}.feature-selects.svelte-1oprcpz label.svelte-1oprcpz{flex:0 1 auto;display:flex;align-items:center;gap:0.25em;min-width:0}.feature-selects.svelte-1oprcpz label span.svelte-1oprcpz{flex:0 0 auto}.feature-selects.svelte-1oprcpz label select.svelte-1oprcpz{flex:0 1 auto;min-width:0;text-overflow:ellipsis}.zoomed-pdp-content.svelte-1oprcpz.svelte-1oprcpz{flex:1;padding:0.5em;min-height:0px}.label-and-input.svelte-1oprcpz.svelte-1oprcpz{flex:0 0 auto;display:flex;align-items:center;gap:0.25em}.detailed-plot-message-container.svelte-1oprcpz.svelte-1oprcpz{height:100%;width:100%;align-items:center;justify-content:center;display:flex}.detailed-plot-message-content.svelte-1oprcpz.svelte-1oprcpz{width:40em;display:flex;flex-direction:column;justify-content:center;gap:1em}.detailed-plot-message-content.svelte-1oprcpz>button.svelte-1oprcpz{margin:auto}")
         }
 
-        function kd(t, e, n) {
+        function Ad(t, e, n) {
             const r = t.slice();
             return r[18] = e[n], r
         }
 
-        function Md(t, e, n) {
+        function Pd(t, e, n) {
             const r = t.slice();
             return r[18] = e[n], r
         }
 
-        function Ld(t) {
+        function Sd(t) {
             let e, n, r, i = t[18] + "";
             return {
                 c() {
                     e = p("option"), n = m(i), e.__value = r = t[18], k(e, e.__value)
                 },
                 m(t, r) {
                     d(t, e, r), c(e, n)
@@ -10682,15 +10735,15 @@
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Ad(t) {
+        function zd(t) {
             let e, n, r, i = t[18] + "";
             return {
                 c() {
                     e = p("option"), n = m(i), e.__value = r = t[18], k(e, e.__value)
                 },
                 m(t, r) {
                     d(t, e, r), c(e, n)
@@ -10700,33 +10753,33 @@
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Pd(t) {
-            let e, n, r, i, o, l, a, s = 2 === t[0].num_features && Sd(t);
+        function Td(t) {
+            let e, n, r, i, o, l, a, s = 2 === t[0].num_features && Nd(t);
             return {
                 c() {
                     e = p("label"), n = p("input"), r = m("Scale\n        locally"), i = v(), s && s.c(), o = b(), $(n, "type", "checkbox"), $(e, "class", "label-and-input svelte-1oprcpz")
                 },
                 m(u, f) {
                     d(u, e, f), c(e, n), n.checked = t[7], c(e, r), d(u, i, f), s && s.m(u, f), d(u, o, f), l || (a = y(n, "change", t[15]), l = !0)
                 },
                 p(t, e) {
-                    128 & e && (n.checked = t[7]), 2 === t[0].num_features ? s ? s.p(t, e) : (s = Sd(t), s.c(), s.m(o.parentNode, o)) : s && (s.d(1), s = null)
+                    128 & e && (n.checked = t[7]), 2 === t[0].num_features ? s ? s.p(t, e) : (s = Nd(t), s.c(), s.m(o.parentNode, o)) : s && (s.d(1), s = null)
                 },
                 d(t) {
                     t && (f(e), f(i), f(o)), s && s.d(t), l = !1, a()
                 }
             }
         }
 
-        function Sd(t) {
+        function Nd(t) {
             let e, n, r;
             return {
                 c() {
                     e = p("button"), e.textContent = "Swap Axes", $(e, "title", "Swap x and y axes")
                 },
                 m(i, o) {
                     d(i, e, o), n || (r = y(e, "click", t[9]), n = !0)
@@ -10734,17 +10787,17 @@
                 p: T,
                 d(t) {
                     t && f(e), n = !1, r()
                 }
             }
         }
 
-        function zd(t) {
+        function Cd(t) {
             let e, n;
-            return e = new xd({
+            return e = new Md({
                 props: {
                     pd: t[0],
                     xFeatureInfo: t[4],
                     yFeatureInfo: t[3]
                 }
             }), {
                 c() {
@@ -10765,17 +10818,17 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Td(t) {
+        function Od(t) {
             let e, n;
-            return e = new vd({
+            return e = new $d({
                 props: {
                     pd: t[0],
                     featureInfo: t[4]
                 }
             }), {
                 c() {
                     bt(e.$$.fragment)
@@ -10795,19 +10848,19 @@
                 },
                 d(t) {
                     $t(e, t)
                 }
             }
         }
 
-        function Nd(t) {
+        function Dd(t) {
             let e, n;
 
             function r(t, e) {
-                return "" === t[2] && "" === t[1] ? Od : Cd
+                return "" === t[2] && "" === t[1] ? Bd : jd
             }
             let i = r(t),
                 o = i(t);
             return {
                 c() {
                     e = p("div"), n = p("div"), o.c(), $(n, "class", "detailed-plot-message-content svelte-1oprcpz"), $(e, "class", "detailed-plot-message-container svelte-1oprcpz")
                 },
@@ -10821,15 +10874,15 @@
                 o: T,
                 d(t) {
                     t && f(e), o.d()
                 }
             }
         }
 
-        function Cd(t) {
+        function jd(t) {
             let e, n, r, i, o, l, a, s, u, h, g, b, w = 2 === t[5].length ? "Computing..." : "Compute Now";
             return {
                 c() {
                     e = p("div"), n = m("The two-way PDP between "), r = m(t[2]), i = m(" and "), o = m(t[1]), l = m("\n              was not pre-computed, since we did not detect a likely interaction\n              between the two features."), a = v(), s = p("button"), u = m(w), s.disabled = h = 2 === t[5].length, $(s, "class", "svelte-1oprcpz")
                 },
                 m(f, h) {
                     d(f, e, h), c(e, n), c(e, r), c(e, i), c(e, o), c(e, l), d(f, a, h), d(f, s, h), c(s, u), g || (b = y(s, "click", t[8]), g = !0)
@@ -10839,15 +10892,15 @@
                 },
                 d(t) {
                     t && (f(e), f(a), f(s)), g = !1, b()
                 }
             }
         }
 
-        function Od(t) {
+        function Bd(t) {
             let e;
             return {
                 c() {
                     e = p("div"), e.textContent = "Select one or two features above.", M(e, "text-align", "center")
                 },
                 m(t, n) {
                     d(t, e, n)
@@ -10855,23 +10908,23 @@
                 p: T,
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Dd(t) {
+        function Ed(t) {
             let e, n, r, i, o, l, a, s, u, g, m, b, w, x, _, M, A, P, S, z, T, N, C = ht(t[6]),
                 D = [];
-            for (let e = 0; e < C.length; e += 1) D[e] = Ld(Md(t, C, e));
+            for (let e = 0; e < C.length; e += 1) D[e] = Sd(Pd(t, C, e));
             let j = ht(t[6]),
                 B = [];
-            for (let e = 0; e < j.length; e += 1) B[e] = Ad(kd(t, j, e));
-            let E = t[0] && Pd(t);
-            const I = [Nd, Td, zd],
+            for (let e = 0; e < j.length; e += 1) B[e] = zd(Ad(t, j, e));
+            let E = t[0] && Td(t);
+            const I = [Dd, Od, Cd],
                 R = [];
 
             function V(t, e) {
                 return null === t[0] ? 0 : 1 === t[0].num_features && t[4] ? 1 : 2 === t[0].num_features && t[4] && t[3] ? 2 : -1
             }
             return ~(P = V(t)) && (S = R[P] = I[P](t)), {
                 c() {
@@ -10888,30 +10941,30 @@
                     for (let t = 0; t < B.length; t += 1) B[t] && B[t].m(w, null);
                     L(w, t[1], !0), c(n, _), E && E.m(n, null), c(e, M), c(e, A), ~P && R[P].m(A, null), z = !0, T || (N = [y(a, "change", t[13]), y(w, "change", t[14])], T = !0)
                 },
                 p(t, [e]) {
                     if (64 & e) {
                         let n;
                         for (C = ht(t[6]), n = 0; n < C.length; n += 1) {
-                            const r = Md(t, C, n);
-                            D[n] ? D[n].p(r, e) : (D[n] = Ld(r), D[n].c(), D[n].m(a, null))
+                            const r = Pd(t, C, n);
+                            D[n] ? D[n].p(r, e) : (D[n] = Sd(r), D[n].c(), D[n].m(a, null))
                         }
                         for (; n < D.length; n += 1) D[n].d(1);
                         D.length = C.length
                     }
                     if (68 & e && L(a, t[2]), 64 & e) {
                         let n;
                         for (j = ht(t[6]), n = 0; n < j.length; n += 1) {
-                            const r = kd(t, j, n);
-                            B[n] ? B[n].p(r, e) : (B[n] = Ad(r), B[n].c(), B[n].m(w, null))
+                            const r = Ad(t, j, n);
+                            B[n] ? B[n].p(r, e) : (B[n] = zd(r), B[n].c(), B[n].m(w, null))
                         }
                         for (; n < B.length; n += 1) B[n].d(1);
                         B.length = j.length
                     }
-                    66 & e && L(w, t[1]), t[0] ? E ? E.p(t, e) : (E = Pd(t), E.c(), E.m(n, null)) : E && (E.d(1), E = null);
+                    66 & e && L(w, t[1]), t[0] ? E ? E.p(t, e) : (E = Td(t), E.c(), E.m(n, null)) : E && (E.d(1), E = null);
                     let r = P;
                     P = V(t), P === r ? ~P && R[P].p(t, e) : (S && (ct(), ft(R[r], 1, 1, (() => {
                         R[r] = null
                     })), ut()), ~P ? (S = R[P], S ? S.p(t, e) : (S = R[P] = I[P](t), S.c()), dt(S, 1), S.m(A, null)) : S = null)
                 },
                 i(t) {
                     z || (dt(S), z = !0)
@@ -10921,15 +10974,15 @@
                 },
                 d(t) {
                     t && f(e), h(D, t), h(B, t), E && E.d(), ~P && R[P].d(), T = !1, O(N)
                 }
             }
         }
 
-        function jd(t, e, n) {
+        function Id(t, e, n) {
             let r, i, o, l, a, s, c, u, d, f;
             E(t, ir, (t => n(10, o = t))), E(t, Zn, (t => n(11, l = t))), E(t, mr, (t => n(12, a = t))), E(t, $r, (t => n(1, s = t))), E(t, yr, (t => n(2, c = t))), E(t, hr, (t => n(5, u = t))), E(t, Jn, (t => n(6, d = t))), E(t, _r, (t => n(7, f = t)));
             let h = null;
             return t.$$.update = () => {
                 var e, d;
                 4102 & t.$$.dirty && (c === s && R($r, s = "", s), "" === c && "" !== s && (R(yr, c = s, c), R($r, s = "", s)), n(0, h = "" === s ? null !== (e = a.get(c)) && void 0 !== e ? e : null : null !== (d = o.find((t => t.x_feature === c && t.y_feature === s || t.x_feature === s && t.y_feature === c))) && void 0 !== d ? d : null)), 1024 & t.$$.dirty && o && function() {
                     const t = o.find((t => t.x_feature === u[0] && t.y_feature === u[1] || t.x_feature === u[1] && t.y_feature === u[0]));
@@ -10950,30 +11003,30 @@
                 c = A(this), yr.set(c)
             }, function() {
                 s = A(this), $r.set(s)
             }, function() {
                 f = this.checked, _r.set(f)
             }]
         }
-        const Bd = class extends _t {
+        const Rd = class extends _t {
             constructor(t) {
-                super(), wt(this, t, jd, Dd, j, {}, _d)
+                super(), wt(this, t, Id, Ed, j, {}, Ld)
             }
         };
 
-        function Ed(t) {
+        function Vd(t) {
             u(t, "svelte-1ps68ru", ".controls-features.svelte-1ps68ru.svelte-1ps68ru{display:flex;flex-direction:column;max-height:100%;row-gap:0.25em}ul.svelte-1ps68ru.svelte-1ps68ru{list-style:none}.fs-row.svelte-1ps68ru.svelte-1ps68ru{display:flex;align-items:center;column-gap:0.25em}input.svelte-1ps68ru.svelte-1ps68ru{min-width:0}.fs-row.svelte-1ps68ru label.svelte-1ps68ru{flex:1}.individual-features.svelte-1ps68ru.svelte-1ps68ru{flex:0 1 auto;overflow-y:auto;min-height:0}.hidden.svelte-1ps68ru.svelte-1ps68ru{display:none}.disabled-feature-label.svelte-1ps68ru.svelte-1ps68ru{color:var(--gray-5);cursor:not-allowed}")
         }
 
-        function Id(t, e, n) {
+        function Hd(t, e, n) {
             const r = t.slice();
             return r[13] = e[n].feature, r[14] = e[n].hidden, r[15] = e[n].disabled, r
         }
 
-        function Rd(t, e) {
+        function qd(t, e) {
             let n, r, i, o, l, a, s, u, h, g, b, w, M, L, A = !1,
                 P = e[13] + "";
             return w = x(e[9][0]), {
                 key: t,
                 first: null,
                 c() {
                     n = p("li"), r = p("input"), a = v(), s = p("label"), u = m(P), b = v(), $(r, "id", i = e[0] + "-" + e[13] + "-checkbox"), $(r, "type", "checkbox"), $(r, "name", "features"), r.__value = o = e[13], k(r, r.__value), r.disabled = l = e[15], $(r, "class", "svelte-1ps68ru"), $(s, "class", "pdpilot-cutoff svelte-1ps68ru"), $(s, "for", h = e[0] + "-" + e[13] + "-checkbox"), $(s, "title", g = e[13]), z(s, "disabled-feature-label", e[15]), $(n, "class", "fs-row svelte-1ps68ru"), z(n, "hidden", e[14]), w.p(r), this.first = n
@@ -10986,49 +11039,49 @@
                 },
                 d(t) {
                     t && f(n), w.r(), M = !1, L()
                 }
             }
         }
 
-        function Vd(t) {
+        function Fd(t) {
             let e, n, r, i, o, l, a, s, u = [],
                 h = new Map,
                 g = ht(t[3]);
             const b = t => t[13];
             for (let e = 0; e < g.length; e += 1) {
-                let n = Id(t, g, e),
+                let n = Hd(t, g, e),
                     r = b(n);
-                h.set(r, u[e] = Rd(r, n))
+                h.set(r, u[e] = qd(r, n))
             }
             return {
                 c() {
                     e = p("div"), n = p("label"), r = m("Search\n    "), i = p("input"), o = v(), l = p("ul");
                     for (let t = 0; t < u.length; t += 1) u[t].c();
                     $(i, "class", "svelte-1ps68ru"), $(n, "class", "fs-row svelte-1ps68ru"), $(l, "class", "individual-features svelte-1ps68ru"), $(e, "class", "controls-features svelte-1ps68ru")
                 },
                 m(f, h) {
                     d(f, e, h), c(e, n), c(n, r), c(n, i), k(i, t[1]), c(e, o), c(e, l);
                     for (let t = 0; t < u.length; t += 1) u[t] && u[t].m(l, null);
                     a || (s = y(i, "input", t[7]), a = !0)
                 },
                 p(t, [e]) {
-                    2 & e && i.value !== t[1] && k(i, t[1]), 13 & e && (g = ht(t[3]), u = mt(u, e, b, 1, t, g, h, l, pt, Rd, null, Id))
+                    2 & e && i.value !== t[1] && k(i, t[1]), 13 & e && (g = ht(t[3]), u = mt(u, e, b, 1, t, g, h, l, pt, qd, null, Hd))
                 },
                 i: T,
                 o: T,
                 d(t) {
                     t && f(e);
                     for (let t = 0; t < u.length; t += 1) u[t].d();
                     a = !1, s()
                 }
             }
         }
 
-        function Hd(t, e, n) {
+        function Wd(t, e, n) {
             let r, i;
             E(t, Jn, (t => n(6, i = t)));
             let {
                 enabledFeatures: o
             } = e, {
                 idPrefix: l
             } = e;
@@ -11057,32 +11110,32 @@
                 n(2, c = [])
             }, i, function() {
                 s = this.value, n(1, s)
             }, function() {
                 c = w(d[0], this.__value, this.checked), n(2, c), n(6, i)
             }, d]
         }
-        const qd = class extends _t {
+        const Kd = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Hd, Vd, j, {
+                super(), wt(this, t, Wd, Fd, j, {
                     enabledFeatures: 4,
                     idPrefix: 0,
                     clear: 5
-                }, Ed)
+                }, Vd)
             }
             get clear() {
                 return this.$$.ctx[5]
             }
         };
 
-        function Fd(t) {
+        function Xd(t) {
             u(t, "svelte-zyfurg", "ul.svelte-zyfurg.svelte-zyfurg{list-style:none}.label-and-input.svelte-zyfurg.svelte-zyfurg{display:flex;align-items:center;gap:0.25em}ul.svelte-zyfurg ul.svelte-zyfurg{margin-left:1em}")
         }
 
-        function Wd(t) {
+        function Ud(t) {
             let e, n, r, i, o, l, a, s, u, h, g, m, b, w, _, M, L, A, P, S, z, N, C, D, j, B, E, I, R;
             return E = x(t[7][0]), {
                 c() {
                     e = p("div"), n = p("ul"), r = p("li"), i = p("label"), o = p("input"), a = p("span"), a.textContent = "Ordered", s = v(), u = p("ul"), h = p("li"), g = p("label"), m = p("input"), b = p("span"), b.textContent = "Increasing", w = v(), _ = p("label"), M = p("input"), L = p("span"), L.textContent = "Decreasing", A = v(), P = p("label"), S = p("input"), z = p("span"), z.textContent = "Mixed", N = v(), C = p("li"), D = p("label"), j = p("input"), B = p("span"), B.textContent = "Nominal", $(o, "type", "checkbox"), o.indeterminate = l = t[0].ordered.shapes.length > 0 && t[0].ordered.shapes.length < t[1].length, $(i, "class", "label-and-input svelte-zyfurg"), $(m, "type", "checkbox"), m.__value = "increasing", k(m, m.__value), $(g, "class", "label-and-input svelte-zyfurg"), $(M, "type", "checkbox"), M.__value = "decreasing", k(M, M.__value), $(_, "class", "label-and-input svelte-zyfurg"), $(S, "type", "checkbox"), S.__value = "mixed", k(S, S.__value), $(P, "class", "label-and-input svelte-zyfurg"), $(u, "class", "svelte-zyfurg"), $(j, "type", "checkbox"), $(D, "class", "label-and-input svelte-zyfurg"), $(n, "class", "svelte-zyfurg"), E.p(m, M, S)
                 },
                 m(l, f) {
                     d(l, e, f), c(e, n), c(n, r), c(r, i), c(i, o), o.checked = t[0].ordered.checked, c(i, a), c(r, s), c(r, u), c(u, h), c(h, g), c(g, m), m.checked = ~(t[0].ordered.shapes || []).indexOf(m.__value), c(g, b), c(h, w), c(h, _), c(_, M), M.checked = ~(t[0].ordered.shapes || []).indexOf(M.__value), c(_, L), c(h, A), c(h, P), c(P, S), S.checked = ~(t[0].ordered.shapes || []).indexOf(S.__value), c(P, z), c(n, N), c(n, C), c(C, D), c(D, j), j.checked = t[0].nominal.checked, c(D, B), I || (R = [y(o, "change", t[5]), y(o, "change", t[2]), y(m, "change", t[6]), y(m, "change", t[3]), y(M, "change", t[8]), y(M, "change", t[3]), y(S, "change", t[9]), y(S, "change", t[3]), y(j, "change", t[10])], I = !0)
@@ -11094,15 +11147,15 @@
                 o: T,
                 d(t) {
                     t && f(e), E.r(), I = !1, O(R)
                 }
             }
         }
 
-        function Kd(t, e, n) {
+        function Yd(t, e, n) {
             let r = ["increasing", "decreasing", "mixed"];
             const i = {
                 ordered: {
                     checked: !0,
                     shapes: r
                 },
                 nominal: {
@@ -11161,103 +11214,103 @@
                 o.ordered.shapes = w(s[0], this.__value, this.checked), n(0, o), n(1, r)
             }, function() {
                 o.ordered.shapes = w(s[0], this.__value, this.checked), n(0, o), n(1, r)
             }, function() {
                 o.nominal.checked = this.checked, n(0, o), n(1, r)
             }]
         }
-        const Xd = class extends _t {
+        const Gd = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Kd, Wd, j, {
+                super(), wt(this, t, Yd, Ud, j, {
                     clear: 4
-                }, Fd)
+                }, Xd)
             }
             get clear() {
                 return this.$$.ctx[4]
             }
         };
 
-        function Ud(t) {
+        function Jd(t) {
             u(t, "svelte-2uqume", ".toggle-and-title.svelte-2uqume.svelte-2uqume{display:flex;align-items:center;gap:0.25em}.icon-tabler-chevron-down.svelte-2uqume polyline.svelte-2uqume{transition:transform 150ms}.rotate-polyline.svelte-2uqume.svelte-2uqume{transform-origin:50% 50%;transform:rotate(-90deg)}")
         }
 
-        function Yd(t) {
-            let e, n, r, i, o, l, a, s, u, h, b, w = `${Gd}px`,
-                x = `${Gd}px`;
+        function Zd(t) {
+            let e, n, r, i, o, l, a, s, u, h, b, w = `${Qd}px`,
+                x = `${Qd}px`;
             return {
                 c() {
-                    e = p("div"), n = p("button"), r = g("svg"), i = g("path"), o = g("polyline"), a = v(), s = p("div"), u = m(t[1]), $(i, "stroke", "none"), $(i, "d", "M0 0h24v24H0z"), $(i, "fill", "none"), $(o, "points", l = "2 12 12 22 22 12"), $(o, "class", "svelte-2uqume"), z(o, "rotate-polyline", !t[0]), $(r, "xmlns", "http://www.w3.org/2000/svg"), $(r, "class", "icon-tabler icon-tabler-chevron-down svelte-2uqume"), $(r, "width", Gd), $(r, "height", Gd), $(r, "viewBox", "0 0 24 24"), $(r, "stroke-width", "4"), $(r, "stroke", "currentColor"), $(r, "fill", "none"), $(r, "stroke-linecap", "round"), $(r, "stroke-linejoin", "round"), M(n, "border", "none"), M(n, "width", w), M(n, "height", x), M(n, "padding", "0"), M(n, "color", "var(--black)"), M(n, "background-color", "white"), $(s, "class", "pdpilot-bold"), $(e, "class", "toggle-and-title svelte-2uqume")
+                    e = p("div"), n = p("button"), r = g("svg"), i = g("path"), o = g("polyline"), a = v(), s = p("div"), u = m(t[1]), $(i, "stroke", "none"), $(i, "d", "M0 0h24v24H0z"), $(i, "fill", "none"), $(o, "points", l = "2 12 12 22 22 12"), $(o, "class", "svelte-2uqume"), z(o, "rotate-polyline", !t[0]), $(r, "xmlns", "http://www.w3.org/2000/svg"), $(r, "class", "icon-tabler icon-tabler-chevron-down svelte-2uqume"), $(r, "width", Qd), $(r, "height", Qd), $(r, "viewBox", "0 0 24 24"), $(r, "stroke-width", "4"), $(r, "stroke", "currentColor"), $(r, "fill", "none"), $(r, "stroke-linecap", "round"), $(r, "stroke-linejoin", "round"), M(n, "border", "none"), M(n, "width", w), M(n, "height", x), M(n, "padding", "0"), M(n, "color", "var(--black)"), M(n, "background-color", "white"), $(s, "class", "pdpilot-bold"), $(e, "class", "toggle-and-title svelte-2uqume")
                 },
                 m(l, f) {
                     d(l, e, f), c(e, n), c(n, r), c(r, i), c(r, o), c(e, a), c(e, s), c(s, u), h || (b = y(n, "click", t[2]), h = !0)
                 },
                 p(t, [e]) {
                     1 & e && z(o, "rotate-polyline", !t[0]), 2 & e && _(u, t[1])
                 },
                 i: T,
                 o: T,
                 d(t) {
                     t && f(e), h = !1, b()
                 }
             }
         }
-        const Gd = 8;
+        const Qd = 8;
 
-        function Jd(t, e, n) {
+        function tf(t, e, n) {
             let {
                 expanded: r = !1
             } = e, {
                 title: i
             } = e;
             return t.$$set = t => {
                 "expanded" in t && n(0, r = t.expanded), "title" in t && n(1, i = t.title)
             }, [r, i, () => n(0, r = !r)]
         }
-        const Zd = class extends _t {
+        const ef = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Jd, Yd, j, {
+                super(), wt(this, t, tf, Zd, j, {
                     expanded: 0,
                     title: 1
-                }, Ud)
+                }, Jd)
             }
         };
 
-        function Qd(t) {
+        function nf(t) {
             u(t, "svelte-1mkvanr", ".controls-container.svelte-1mkvanr.svelte-1mkvanr{height:100%;flex:0 0 200px;min-width:200px;max-width:200px;padding:0.25em;border-right:1px solid var(--gray-1);display:flex;flex-direction:column;gap:0.5em}.feature-selector-wrapper-outer.svelte-1mkvanr.svelte-1mkvanr{flex:0 1 auto;min-height:0;display:flex;flex-direction:column}.feature-selector-wrapper-inner.svelte-1mkvanr.svelte-1mkvanr{flex:1;min-height:0}.filter-header.svelte-1mkvanr+.filter-content.svelte-1mkvanr{margin-top:0.25em}.filter-content.svelte-1mkvanr.svelte-1mkvanr{margin-left:0.75em}")
         }
 
-        function tf(t) {
+        function rf(t) {
             let e, n, r, i, o, l, a, s, u, h, g, m, b, w, x, _, k, L, A, P, S, T, N;
 
             function C(e) {
                 t[11](e)
             }
             let O = {
                 title: "Type"
             };
 
             function D(e) {
                 t[13](e)
             }
-            void 0 !== t[2] && (O.expanded = t[2]), s = new Zd({
+            void 0 !== t[2] && (O.expanded = t[2]), s = new ef({
                 props: O
-            }), X.push((() => vt(s, "expanded", C))), m = new Xd({
+            }), X.push((() => vt(s, "expanded", C))), m = new Gd({
                 props: {}
             }), t[12](m), m.$on("changeKindFilters", t[5]);
             let j = {
                 title: "Name"
             };
-            void 0 !== t[3] && (j.expanded = t[3]), _ = new Zd({
+            void 0 !== t[3] && (j.expanded = t[3]), _ = new ef({
                 props: j
             }), X.push((() => vt(_, "expanded", D)));
             let B = {
                 enabledFeatures: t[4],
                 idPrefix: "pdpilot-one"
             };
-            return P = new qd({
+            return P = new Kd({
                 props: B
             }), t[14](P), P.$on("changeNameFilters", t[6]), {
                 c() {
                     e = p("div"), n = p("div"), n.textContent = "Feature Filters", r = v(), i = p("button"), i.textContent = "Clear Filters", o = v(), l = p("div"), a = p("div"), bt(s.$$.fragment), h = v(), g = p("div"), bt(m.$$.fragment), b = v(), w = p("div"), x = p("div"), bt(_.$$.fragment), L = v(), A = p("div"), bt(P.$$.fragment), $(n, "class", "pdpilot-bold"), M(i, "align-self", "start"), $(a, "class", "filter-header svelte-1mkvanr"), $(g, "class", "filter-content svelte-1mkvanr"), z(g, "pdp-hide", !t[2]), $(x, "class", "filter-header svelte-1mkvanr"), $(A, "class", "filter-content feature-selector-wrapper-inner svelte-1mkvanr"), z(A, "pdp-hide", !t[3]), $(w, "class", "filter-container feature-selector-wrapper-outer svelte-1mkvanr"), $(e, "class", "controls-container svelte-1mkvanr")
                 },
                 m(u, f) {
                     d(u, e, f), c(e, n), c(e, r), c(e, i), c(e, o), c(e, l), c(l, a), yt(s, a, null), c(l, h), c(l, g), yt(m, g, null), c(e, b), c(e, w), c(w, x), yt(_, x, null), c(w, L), c(w, A), yt(P, A, null), S = !0, T || (N = y(i, "click", t[7]), T = !0)
@@ -11278,15 +11331,15 @@
                 },
                 d(n) {
                     n && f(e), $t(s), t[12](null), $t(m), $t(_), t[14](null), $t(P), T = !1, N()
                 }
             }
         }
 
-        function ef(t, e, n) {
+        function of(t, e, n) {
             let r, i, o;
             E(t, mr, (t => n(9, i = t))), E(t, Jn, (t => n(10, o = t)));
             const l = W();
             let a, s, c, u = !0,
                 d = !0;
             return t.$$.update = () => {
                 1792 & t.$$.dirty && n(4, r = o.filter((t => {
@@ -11309,29 +11362,29 @@
                 d = t, n(3, d)
             }, function(t) {
                 X[t ? "unshift" : "push"]((() => {
                     s = t, n(1, s)
                 }))
             }]
         }
-        const nf = class extends _t {
+        const lf = class extends _t {
             constructor(t) {
-                super(), wt(this, t, ef, tf, j, {}, Qd)
+                super(), wt(this, t, of, rf, j, {}, nf)
             }
         };
 
-        function rf(t) {
+        function af(t) {
             return 0 === t.length || 1 === t[0].num_features
         }
 
-        function of(t) {
+        function sf(t) {
             u(t, "svelte-19snser", ".tooltip-container.svelte-19snser{position:relative;display:flex;align-items:center}.tooltip-content.svelte-19snser{position:absolute;padding:5px;border-radius:5px;max-width:30em;border:1px solid black;color:black;background-color:white;z-index:1;pointer-events:none}")
         }
 
-        function lf(t) {
+        function cf(t) {
             let e, n, r, i, o, l, a;
             return {
                 c() {
                     e = g("svg"), n = g("path"), r = g("circle"), i = g("line"), o = g("path"), $(n, "stroke", "none"), $(n, "d", "M0 0h24v24H0z"), $(r, "cx", "12"), $(r, "cy", "12"), $(r, "r", "9"), $(i, "x1", "12"), $(i, "y1", "17"), $(i, "x2", "12"), $(i, "y2", "17.01"), $(o, "d", "M12 13.5a1.5 1.5 0 0 1 1 -1.5a2.6 2.6 0 1 0 -3 -4"), $(e, "xmlns", "http://www.w3.org/2000/svg"), $(e, "class", "pdpilot-icon icon-tabler icon-tabler-help"), $(e, "width", "24"), $(e, "height", "24"), $(e, "viewBox", "0 0 24 24"), $(e, "stroke-width", "2"), $(e, "stroke", "currentColor"), $(e, "fill", "none"), $(e, "stroke-linecap", "round"), $(e, "stroke-linejoin", "round")
                 },
                 m(s, u) {
                     d(s, e, u), c(e, n), c(e, r), c(e, i), c(e, o), l || (a = [y(e, "mouseenter", t[15]), y(e, "mouseleave", t[16])], l = !0)
@@ -11339,15 +11392,15 @@
                 p: T,
                 d(t) {
                     t && f(e), l = !1, O(a)
                 }
             }
         }
 
-        function af(t) {
+        function uf(t) {
             let e, n, r, i, o, l, a;
             return {
                 c() {
                     e = g("svg"), n = g("path"), r = g("circle"), i = g("line"), o = g("line"), $(n, "stroke", "none"), $(n, "d", "M0 0h24v24H0z"), $(n, "fill", "none"), $(r, "cx", "12"), $(r, "cy", "12"), $(r, "r", "9"), $(i, "x1", "12"), $(i, "y1", "8"), $(i, "x2", "12"), $(i, "y2", "12"), $(o, "x1", "12"), $(o, "y1", "16"), $(o, "x2", "12.01"), $(o, "y2", "16"), $(e, "xmlns", "http://www.w3.org/2000/svg"), $(e, "class", "pdpilot-icon icon-tabler icon-tabler-alert-circle"), $(e, "width", "24"), $(e, "height", "24"), $(e, "viewBox", "0 0 24 24"), $(e, "stroke-width", "2"), $(e, "stroke", "currentColor"), $(e, "fill", "none"), $(e, "stroke-linecap", "round"), $(e, "stroke-linejoin", "round")
                 },
                 m(s, u) {
                     d(s, e, u), c(e, n), c(e, r), c(e, i), c(e, o), l || (a = [y(e, "mouseenter", t[13]), y(e, "mouseleave", t[14])], l = !0)
@@ -11355,15 +11408,15 @@
                 p: T,
                 d(t) {
                     t && f(e), l = !1, O(a)
                 }
             }
         }
 
-        function sf(t) {
+        function df(t) {
             let e, n, r = `${t[5]}\n      ${t[6]}\n      ${t[7]}\n      ${t[8]}`;
             const i = t[12].default,
                 o = function(t, e, n, r) {
                     if (t) {
                         const r = I(t, e, n, null);
                         return t[0](r)
                     }
@@ -11412,32 +11465,32 @@
                 },
                 d(t) {
                     t && f(e), o && o.d(t)
                 }
             }
         }
 
-        function cf(t) {
+        function ff(t) {
             let e, n, r;
 
             function i(t, e) {
-                return "alert" === t[0] ? af : lf
+                return "alert" === t[0] ? uf : cf
             }
             let o = i(t),
                 l = o(t),
-                a = t[10] && sf(t);
+                a = t[10] && df(t);
             return {
                 c() {
                     e = p("div"), l.c(), n = v(), a && a.c(), $(e, "class", "tooltip-container svelte-19snser")
                 },
                 m(t, i) {
                     d(t, e, i), l.m(e, null), c(e, n), a && a.m(e, null), r = !0
                 },
                 p(t, [r]) {
-                    o === (o = i(t)) && l ? l.p(t, r) : (l.d(1), l = o(t), l && (l.c(), l.m(e, n))), t[10] ? a ? (a.p(t, r), 1024 & r && dt(a, 1)) : (a = sf(t), a.c(), dt(a, 1), a.m(e, null)) : a && (ct(), ft(a, 1, 1, (() => {
+                    o === (o = i(t)) && l ? l.p(t, r) : (l.d(1), l = o(t), l && (l.c(), l.m(e, n))), t[10] ? a ? (a.p(t, r), 1024 & r && dt(a, 1)) : (a = df(t), a.c(), dt(a, 1), a.m(e, null)) : a && (ct(), ft(a, 1, 1, (() => {
                         a = null
                     })), ut())
                 },
                 i(t) {
                     r || (dt(a), r = !0)
                 },
                 o(t) {
@@ -11445,15 +11498,15 @@
                 },
                 d(t) {
                     t && f(e), l.d(), a && a.d()
                 }
             }
         }
 
-        function uf(t, e, n) {
+        function hf(t, e, n) {
             let {
                 $$slots: r = {},
                 $$scope: i
             } = e, {
                 kind: o = "help"
             } = e, {
                 top: l = "auto"
@@ -11474,51 +11527,51 @@
             } = e, {
                 width: p = "30em"
             } = e, g = !1;
             return t.$$set = t => {
                 "kind" in t && n(0, o = t.kind), "top" in t && n(1, l = t.top), "left" in t && n(2, a = t.left), "right" in t && n(3, s = t.right), "bottom" in t && n(4, c = t.bottom), "marginTop" in t && n(5, u = t.marginTop), "marginRight" in t && n(6, d = t.marginRight), "marginBottom" in t && n(7, f = t.marginBottom), "marginLeft" in t && n(8, h = t.marginLeft), "width" in t && n(9, p = t.width), "$$scope" in t && n(11, i = t.$$scope)
             }, [o, l, a, s, c, u, d, f, h, p, g, i, r, () => n(10, g = !0), () => n(10, g = !1), () => n(10, g = !0), () => n(10, g = !1)]
         }
-        const df = class extends _t {
+        const pf = class extends _t {
             constructor(t) {
-                super(), wt(this, t, uf, cf, j, {
+                super(), wt(this, t, hf, ff, j, {
                     kind: 0,
                     top: 1,
                     left: 2,
                     right: 3,
                     bottom: 4,
                     marginTop: 5,
                     marginRight: 6,
                     marginBottom: 7,
                     marginLeft: 8,
                     width: 9
-                }, of)
+                }, sf)
             }
         };
 
-        function ff(t) {
+        function gf(t) {
             u(t, "svelte-alv95s", ".group-container.svelte-alv95s.svelte-alv95s{height:100%;width:100%;display:flex;flex-direction:column;min-height:2em}.pdp-grid-container.svelte-alv95s.svelte-alv95s{flex:1;min-height:0;padding:1px}.pdpilot-no-plots-container.svelte-alv95s.svelte-alv95s{width:100%;height:100%;display:flex;align-items:center;justify-content:center}.pdpilot-no-plots-message.svelte-alv95s.svelte-alv95s{max-width:28em}.pdp-grid.svelte-alv95s.svelte-alv95s{height:100%;display:grid}.group-header.svelte-alv95s.svelte-alv95s{height:2em;display:flex;align-items:center;gap:1em;border-bottom:1px solid var(--gray-1);padding-left:0.5em;padding-right:0.5em}.two-way-color-container.svelte-alv95s.svelte-alv95s{flex:1;margin-left:auto;display:flex;align-items:center}.two-way-color-legend.svelte-alv95s.svelte-alv95s{flex:1}.page-change.svelte-alv95s.svelte-alv95s{display:flex;align-items:center}.current-page-number.svelte-alv95s.svelte-alv95s{width:2em;text-align:center}.label-and-input.svelte-alv95s.svelte-alv95s{display:flex;align-items:center;gap:0.25em}.pdp-grid-element.svelte-alv95s.svelte-alv95s{position:relative}.pdp-grid-element.svelte-alv95s:hover .expand-pdp-button.svelte-alv95s{display:block}.expand-pdp-button.svelte-alv95s.svelte-alv95s{position:absolute;display:none;bottom:2px;left:2px}.dont-shrink.svelte-alv95s.svelte-alv95s{flex:0 0 auto}.dont-show.svelte-alv95s.svelte-alv95s{display:none}ul.svelte-alv95s.svelte-alv95s{list-style:none}li.svelte-alv95s+li.svelte-alv95s{margin-top:0.5em}")
         }
 
-        function hf(t, e, n) {
+        function mf(t, e, n) {
             const r = t.slice();
             return r[51] = e[n], r
         }
 
-        function pf(t, e, n) {
+        function vf(t, e, n) {
             const r = t.slice();
             return r[54] = e[n].value, r[55] = e[n].title, r
         }
 
-        function gf(t, e, n) {
+        function bf(t, e, n) {
             const r = t.slice();
             return r[58] = e[n], r
         }
 
-        function mf(t) {
+        function yf(t) {
             let e, n, r, i = t[58].name + "";
             return {
                 c() {
                     e = p("option"), n = m(i), e.__value = r = t[58], k(e, e.__value)
                 },
                 m(t, r) {
                     d(t, e, r), c(e, n)
@@ -11528,49 +11581,49 @@
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function vf(t) {
+        function $f(t) {
             let e;
             return {
                 c() {
                     e = p("ul"), e.innerHTML = '<li class="svelte-alv95s"><span class="pdpilot-bold">Interaction:</span> Plots for feature\n                pairs with more interaction are ranked higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Variance:</span> Plots that have more\n                variation in their average predictions are ranked higher.</li>', $(e, "class", "svelte-alv95s")
                 },
                 m(t, n) {
                     d(t, e, n)
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function bf(t) {
+        function wf(t) {
             let e;
             return {
                 c() {
-                    e = p("ul"), e.innerHTML = '<li class="svelte-alv95s"><span class="pdpilot-bold">Variance:</span> Plots that have more\n                variance in their ICE lines are ranked higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Cluster difference:</span> Plots that\n                have ICE clusters farther from the partial dependence line are ranked\n                higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Highlighted similarity:</span> Plots where\n                the highlighted lines are closer together and farther from the partial\n                dependence line are ranked higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Highlighted distribution:</span> Plots\n                for features whose distributions of highlighted instances are more\n                different from the overall distributions are ranked higher.</li>', $(e, "class", "svelte-alv95s")
+                    e = p("ul"), e.innerHTML = '<li class="svelte-alv95s"><span class="pdpilot-bold">Importance:</span> Plots that have more\n                variance in their ICE lines are ranked higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Cluster difference:</span> Plots that\n                have ICE clusters farther from the partial dependence line are ranked\n                higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Highlighted line similarity:</span> Plots\n                where the highlighted lines are closer together and farther from\n                the partial dependence line are ranked higher.</li> <li class="svelte-alv95s"><span class="pdpilot-bold">Highlighted histogram difference:</span> Plots for features whose distributions of highlighted instances\n                are more different from the overall distributions are ranked higher.</li>', $(e, "class", "svelte-alv95s")
                 },
                 m(t, n) {
                     d(t, e, n)
                 },
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function yf(t) {
+        function xf(t) {
             let e;
 
             function n(t, e) {
-                return 1 === t[17] ? bf : vf
+                return 1 === t[17] ? wf : $f
             }
             let r = n(t),
                 i = r(t);
             return {
                 c() {
                     e = p("div"), i.c()
                 },
@@ -11582,15 +11635,15 @@
                 },
                 d(t) {
                     t && f(e), i.d()
                 }
             }
         }
 
-        function $f(t) {
+        function _f(t) {
             let e, n, r, i, o, l, a, s;
             return {
                 c() {
                     e = p("button"), n = g("svg"), r = g("path"), i = g("path"), o = g("path"), $(r, "stroke", "none"), $(r, "d", "M0 0h24v24H0z"), $(r, "fill", "none"), $(i, "d", "M20 11a8.1 8.1 0 0 0 -15.5 -2m-.5 -4v4h4"), $(o, "d", "M4 13a8.1 8.1 0 0 0 15.5 2m.5 4v-4h-4"), $(n, "xmlns", "http://www.w3.org/2000/svg"), $(n, "class", "pdpilot-icon icon-tabler icon-tabler-refresh"), $(n, "width", "24"), $(n, "height", "24"), $(n, "viewBox", "0 0 24 24"), $(n, "stroke-width", "2"), $(n, "stroke", "currentColor"), $(n, "fill", "none"), $(n, "stroke-linecap", "round"), $(n, "stroke-linejoin", "round"), $(e, "title", "Update sorting"), e.disabled = l = !t[13]
                 },
                 m(l, u) {
                     d(l, e, u), c(e, n), c(n, r), c(n, i), c(n, o), a || (s = y(e, "click", t[33]), a = !0)
@@ -11600,18 +11653,18 @@
                 },
                 d(t) {
                     t && f(e), a = !1, s()
                 }
             }
         }
 
-        function wf(t) {
+        function kf(t) {
             let e, n, r, i, o, l = ht(t[21]),
                 a = [];
-            for (let e = 0; e < l.length; e += 1) a[e] = xf(pf(t, l, e));
+            for (let e = 0; e < l.length; e += 1) a[e] = Mf(vf(t, l, e));
             return {
                 c() {
                     e = p("label"), n = m("Plot\n        "), r = p("select");
                     for (let t = 0; t < a.length; t += 1) a[t].c();
                     void 0 === t[9] && tt((() => t[34].call(r))), $(e, "class", "label-and-input dont-shrink svelte-alv95s")
                 },
                 m(l, s) {
@@ -11619,29 +11672,29 @@
                     for (let t = 0; t < a.length; t += 1) a[t] && a[t].m(r, null);
                     L(r, t[9], !0), i || (o = y(r, "change", t[34]), i = !0)
                 },
                 p(t, e) {
                     if (2097152 & e[0]) {
                         let n;
                         for (l = ht(t[21]), n = 0; n < l.length; n += 1) {
-                            const i = pf(t, l, n);
-                            a[n] ? a[n].p(i, e) : (a[n] = xf(i), a[n].c(), a[n].m(r, null))
+                            const i = vf(t, l, n);
+                            a[n] ? a[n].p(i, e) : (a[n] = Mf(i), a[n].c(), a[n].m(r, null))
                         }
                         for (; n < a.length; n += 1) a[n].d(1);
                         a.length = l.length
                     }
                     2097664 & e[0] && L(r, t[9])
                 },
                 d(t) {
                     t && f(e), h(a, t), i = !1, o()
                 }
             }
         }
 
-        function xf(t) {
+        function Mf(t) {
             let e, n, r, i = t[55] + "";
             return {
                 c() {
                     e = p("option"), n = m(i), e.__value = r = t[54], k(e, e.__value)
                 },
                 m(t, r) {
                     d(t, e, r), c(e, n)
@@ -11649,34 +11702,34 @@
                 p: T,
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function _f(t) {
+        function Lf(t) {
             let e, n, r, i, o, l, a, s, u, h, g;
-            return s = new df({
+            return s = new pf({
                 props: {
                     kind: "help",
                     right: "0",
                     top: "0",
                     marginRight: "1em",
                     marginTop: "1.5em",
                     width: "30em",
                     $$slots: {
-                        default: [Lf]
+                        default: [Sf]
                     },
                     $$scope: {
                         ctx: t
                     }
                 }
             }), {
                 c() {
-                    e = p("div"), n = p("label"), r = m("Color\n            "), i = p("select"), o = p("option"), o.textContent = "interactions", l = p("option"), l.textContent = "predictions", a = v(), bt(s.$$.fragment), o.__value = "interactions", k(o, o.__value), l.__value = "predictions", k(l, l.__value), void 0 === t[10] && tt((() => t[36].call(i))), $(n, "class", "label-and-input svelte-alv95s"), $(e, "class", "label-and-input dont-shrink svelte-alv95s")
+                    e = p("div"), n = p("label"), r = m("Color\n            "), i = p("select"), o = p("option"), o.textContent = "Predictions", l = p("option"), l.textContent = "Interactions", a = v(), bt(s.$$.fragment), o.__value = "predictions", k(o, o.__value), l.__value = "interactions", k(l, l.__value), void 0 === t[10] && tt((() => t[36].call(i))), $(n, "class", "label-and-input svelte-alv95s"), $(e, "class", "label-and-input dont-shrink svelte-alv95s")
                 },
                 m(f, p) {
                     d(f, e, p), c(e, n), c(n, r), c(n, i), c(i, o), c(i, l), L(i, t[10], !0), c(e, a), yt(s, e, null), u = !0, h || (g = y(i, "change", t[36]), h = !0)
                 },
                 p(t, e) {
                     1024 & e[0] && L(i, t[10]);
                     const n = {};
@@ -11693,15 +11746,15 @@
                 },
                 d(t) {
                     t && f(e), $t(s), h = !1, g()
                 }
             }
         }
 
-        function kf(t) {
+        function Af(t) {
             let e;
             return {
                 c() {
                     e = m("This color scale is for a standard two-way PDP. The color of a\n                cell represents the model's average prediction when setting the\n                instances to have the given values for pair of features.")
                 },
                 m(t, n) {
                     d(t, e, n)
@@ -11709,15 +11762,15 @@
                 p: T,
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Mf(t) {
+        function Pf(t) {
             let e, n, r, i, o;
             return {
                 c() {
                     e = m("This color scale shows the difference between the value in a\n                two-way PDP and the expected value if there was no interaction\n                between the pair of features. It indicates whether the\n                interaction between the two features makes the model's average\n                prediction for the given values "), n = p("span"), n.textContent = "lower", r = m("\n                or\n                "), i = p("span"), i.textContent = "higher", o = m(". The units are the same as your target variable."), M(n, "background", t[19].interpolator()(.1)), M(n, "border-radius", "4px"), M(n, "padding", "0.125em 0.25em"), M(n, "color", "white"), M(i, "background", t[19].interpolator()(.9)), M(i, "border-radius", "4px"), M(i, "padding", "0.125em 0.25em"), M(i, "color", "white")
                 },
                 m(t, l) {
                     d(t, e, l), d(t, n, l), d(t, r, l), d(t, i, l), d(t, o, l)
@@ -11727,19 +11780,19 @@
                 },
                 d(t) {
                     t && (f(e), f(n), f(r), f(i), f(o))
                 }
             }
         }
 
-        function Lf(t) {
+        function Sf(t) {
             let e;
 
             function n(t, e) {
-                return "interactions" === t[10] ? Mf : kf
+                return "interactions" === t[10] ? Pf : Af
             }
             let r = n(t),
                 i = r(t);
             return {
                 c() {
                     e = p("div"), i.c()
                 },
@@ -11751,39 +11804,39 @@
                 },
                 d(t) {
                     t && f(e), i.d()
                 }
             }
         }
 
-        function Af(t) {
+        function zf(t) {
             let e, n, r = [],
                 i = new Map,
                 o = `repeat(${t[8]}, minmax(0,${t[11]}px))`,
                 l = `repeat(${t[7]}, minmax(0,${t[12]}px))`,
                 a = ht(t[16]);
             const s = t => t[51].id;
             for (let e = 0; e < a.length; e += 1) {
-                let n = hf(t, a, e),
+                let n = mf(t, a, e),
                     o = s(n);
-                i.set(o, r[e] = Sf(o, n))
+                i.set(o, r[e] = Nf(o, n))
             }
             return {
                 c() {
                     e = p("div");
                     for (let t = 0; t < r.length; t += 1) r[t].c();
                     $(e, "class", "pdp-grid svelte-alv95s"), M(e, "grid-template-columns", o), M(e, "grid-template-rows", l)
                 },
                 m(t, i) {
                     d(t, e, i);
                     for (let t = 0; t < r.length; t += 1) r[t] && r[t].m(e, null);
                     n = !0
                 },
                 p(t, n) {
-                    16997888 & n[0] && (a = ht(t[16]), ct(), r = mt(r, n, s, 1, t, a, i, e, gt, Sf, null, hf), ut()), 2304 & n[0] && o !== (o = `repeat(${t[8]}, minmax(0,${t[11]}px))`) && M(e, "grid-template-columns", o), 4224 & n[0] && l !== (l = `repeat(${t[7]}, minmax(0,${t[12]}px))`) && M(e, "grid-template-rows", l)
+                    16997888 & n[0] && (a = ht(t[16]), ct(), r = mt(r, n, s, 1, t, a, i, e, gt, Nf, null, mf), ut()), 2304 & n[0] && o !== (o = `repeat(${t[8]}, minmax(0,${t[11]}px))`) && M(e, "grid-template-columns", o), 4224 & n[0] && l !== (l = `repeat(${t[7]}, minmax(0,${t[12]}px))`) && M(e, "grid-template-rows", l)
                 },
                 i(t) {
                     if (!n) {
                         for (let t = 0; t < a.length; t += 1) dt(r[t]);
                         n = !0
                     }
                 },
@@ -11794,15 +11847,15 @@
                 d(t) {
                     t && f(e);
                     for (let t = 0; t < r.length; t += 1) r[t].d()
                 }
             }
         }
 
-        function Pf(t) {
+        function Tf(t) {
             let e, n, r;
             return {
                 c() {
                     e = p("div"), n = p("div"), r = m(t[2]), $(n, "class", "pdpilot-no-plots-message svelte-alv95s"), $(e, "class", "pdpilot-no-plots-container svelte-alv95s")
                 },
                 m(t, i) {
                     d(t, e, i), c(e, n), c(n, r)
@@ -11814,22 +11867,22 @@
                 o: T,
                 d(t) {
                     t && f(e)
                 }
             }
         }
 
-        function Sf(t, e) {
+        function Nf(t, e) {
             let n, r, i, o, l, a, s, u, h = `${e[11]}px`,
                 g = `${e[12]}px`;
 
             function m() {
                 return e[38](e[51])
             }
-            return r = new hu({
+            return r = new mu({
                 props: {
                     pd: e[51],
                     width: e[11],
                     height: e[12],
                     scaleLocally: e[14],
                     colorShows: e[10],
                     showMarginalDistribution: !0,
@@ -11864,47 +11917,47 @@
                 },
                 d(t) {
                     t && f(n), $t(r), s = !1, u()
                 }
             }
         }
 
-        function zf(t) {
+        function Cf(t) {
             let e, n, r, i, o, l, a, s, u, b, w, x, k, M, A, S, T, N, C, D, j, B, E, I, R, V, H, q, F, W, K, X, U, Y, G, J, Z, Q, et, nt, rt, it, ot, lt, at, st, pt, gt, mt = ht(t[1]),
                 vt = [];
-            for (let e = 0; e < mt.length; e += 1) vt[e] = mf(gf(t, mt, e));
-            q = new df({
+            for (let e = 0; e < mt.length; e += 1) vt[e] = yf(bf(t, mt, e));
+            q = new pf({
                 props: {
                     kind: "help",
                     left: "0",
                     top: "0",
                     marginRight: "1em",
                     marginTop: "1.5em",
-                    width: "30em",
+                    width: "25em",
                     $$slots: {
-                        default: [yf]
+                        default: [xf]
                     },
                     $$scope: {
                         ctx: t
                     }
                 }
             });
-            let wt = 1 === t[17] && t[5].forBrushing && $f(t),
-                xt = 1 === t[17] && wf(t),
-                _t = 2 === t[17] && _f(t);
+            let wt = 1 === t[17] && t[5].forBrushing && _f(t),
+                xt = 1 === t[17] && kf(t),
+                _t = 2 === t[17] && Lf(t);
             et = new wc({
                 props: {
                     width: t[18],
-                    height: Tf,
+                    height: Of,
                     color: "interactions" === t[10] ? t[19] : t[20],
                     marginLeft: 15,
                     marginRight: 15
                 }
             });
-            const kt = [Pf, Af],
+            const kt = [Tf, zf],
                 Mt = [];
 
             function Lt(t, e) {
                 return 0 === t[16].length ? 0 : 1
             }
             return ot = Lt(t), lt = Mt[ot] = kt[ot](t), {
                 c() {
@@ -11917,26 +11970,26 @@
                     for (let t = 0; t < vt.length; t += 1) vt[t] && vt[t].m(V, null);
                     L(V, t[5], !0), c(E, H), yt(q, E, null), c(n, F), wt && wt.m(n, null), c(n, W), xt && xt.m(n, null), c(n, K), c(n, X), c(X, U), U.checked = t[14], c(X, Y), c(n, G), c(n, J), _t && _t.m(J, null), c(J, Z), c(J, Q), yt(et, Q, null), nt = P.observe(Q, t[37].bind(Q)), c(e, rt), c(e, it), Mt[ot].m(it, null), at = P.observe(it, t[39].bind(it)), st = !0, pt || (gt = [y(i, "click", t[30]), y(A, "click", t[31]), y(V, "change", t[32]), y(U, "change", t[35])], pt = !0)
                 },
                 p(t, e) {
                     if ((!st || 64 & e[0] && b !== (b = t[6] <= 1)) && (i.disabled = b), (!st || 64 & e[0]) && _(k, t[6]), (!st || 32832 & e[0] && j !== (j = t[6] >= t[15])) && (A.disabled = j), 2 & e[0]) {
                         let n;
                         for (mt = ht(t[1]), n = 0; n < mt.length; n += 1) {
-                            const r = gf(t, mt, n);
-                            vt[n] ? vt[n].p(r, e) : (vt[n] = mf(r), vt[n].c(), vt[n].m(V, null))
+                            const r = bf(t, mt, n);
+                            vt[n] ? vt[n].p(r, e) : (vt[n] = yf(r), vt[n].c(), vt[n].m(V, null))
                         }
                         for (; n < vt.length; n += 1) vt[n].d(1);
                         vt.length = mt.length
                     }
                     34 & e[0] && L(V, t[5]);
                     const r = {};
                     131072 & e[0] | 1073741824 & e[1] && (r.$$scope = {
                         dirty: e,
                         ctx: t
-                    }), q.$set(r), 1 === t[17] && t[5].forBrushing ? wt ? wt.p(t, e) : (wt = $f(t), wt.c(), wt.m(n, W)) : wt && (wt.d(1), wt = null), 1 === t[17] ? xt ? xt.p(t, e) : (xt = wf(t), xt.c(), xt.m(n, K)) : xt && (xt.d(1), xt = null), 16384 & e[0] && (U.checked = t[14]), 2 === t[17] ? _t ? (_t.p(t, e), 131072 & e[0] && dt(_t, 1)) : (_t = _f(t), _t.c(), dt(_t, 1), _t.m(J, Z)) : _t && (ct(), ft(_t, 1, 1, (() => {
+                    }), q.$set(r), 1 === t[17] && t[5].forBrushing ? wt ? wt.p(t, e) : (wt = _f(t), wt.c(), wt.m(n, W)) : wt && (wt.d(1), wt = null), 1 === t[17] ? xt ? xt.p(t, e) : (xt = kf(t), xt.c(), xt.m(n, K)) : xt && (xt.d(1), xt = null), 16384 & e[0] && (U.checked = t[14]), 2 === t[17] ? _t ? (_t.p(t, e), 131072 & e[0] && dt(_t, 1)) : (_t = Lf(t), _t.c(), dt(_t, 1), _t.m(J, Z)) : _t && (ct(), ft(_t, 1, 1, (() => {
                         _t = null
                     })), ut());
                     const o = {};
                     262144 & e[0] && (o.width = t[18]), 1573888 & e[0] && (o.color = "interactions" === t[10] ? t[19] : t[20]), et.$set(o), (!st || 147456 & e[0]) && z(Q, "dont-show", 1 === t[17] || t[14]);
                     let l = ot;
                     ot = Lt(t), ot === l ? Mt[ot].p(t, e) : (ct(), ft(Mt[l], 1, 1, (() => {
                         Mt[l] = null
@@ -11949,17 +12002,17 @@
                     ft(q.$$.fragment, t), ft(_t), ft(et.$$.fragment, t), ft(lt), st = !1
                 },
                 d(t) {
                     t && f(e), h(vt, t), $t(q), wt && wt.d(), xt && xt.d(), _t && _t.d(), $t(et), nt(), Mt[ot].d(), at(), pt = !1, O(gt)
                 }
             }
         }
-        const Tf = 24;
+        const Of = 24;
 
-        function Nf(t, e, n) {
+        function Df(t, e, n) {
             let r, i, o, l, s, c, u, d, f, h, p, g, m, v, b, y, $, w, x, _, k, M;
             E(t, gr, (t => n(40, h = t))), E(t, xr, (t => n(41, p = t))), E(t, wr, (t => n(42, g = t))), E(t, _r, (t => n(43, m = t))), E(t, $r, (t => n(44, v = t))), E(t, yr, (t => n(45, b = t))), E(t, Mr, (t => n(29, y = t))), E(t, rr, (t => n(46, $ = t))), E(t, Zn, (t => n(47, w = t))), E(t, Pr, (t => n(48, x = t))), E(t, fr, (t => n(49, _ = t))), E(t, zr, (t => n(19, k = t))), E(t, Sr, (t => n(20, M = t)));
             let L, {
                     data: P
                 } = e,
                 {
                     sortingOptions: S
@@ -11974,15 +12027,15 @@
                 value: "centered-lines",
                 title: "Centered"
             }, {
                 value: "cluster-centers",
                 title: "Clusters"
             }];
             let N, C, O, D, j = "lines",
-                B = "interactions",
+                B = "predictions",
                 I = !1,
                 V = S[0];
 
             function H(t) {
                 n(13, I = !1), n(25, L = V.sort(t, {
                     highlightedIndices: _,
                     highlightedDistributions: x,
@@ -11999,15 +12052,15 @@
 
             function K(t) {
                 R(yr, b = t.x_feature, b), R($r, v = 2 === t.num_features ? t.y_feature : "", v), R(_r, m = W, m), 1 === t.num_features && (R(wr, g = "cluster-centers" === j ? "cluster-lines" : j, g), R(xr, p = "cluster-centers" === j ? "cluster-descriptions" : "scatterplot", p)), R(gr, h = "detailed-plot", h)
             }
             return t.$$set = t => {
                 "data" in t && n(0, P = t.data), "sortingOptions" in t && n(1, S = t.sortingOptions), "noPlotsMessage" in t && n(2, z = t.noPlotsMessage)
             }, t.$$.update = () => {
-                1 & t.$$.dirty[0] && n(17, r = rf(P) ? 1 : 2), 8 & t.$$.dirty[0] && n(28, i = N ? N.width : 0), 8 & t.$$.dirty[0] && n(27, o = N ? N.height : 0), 16 & t.$$.dirty[0] && n(18, l = C ? C.width : 140), 1 & t.$$.dirty[0] && n(26, s = Math.min(P.length, 12)), 67108864 & t.$$.dirty[0] && n(7, [c, u] = function(t) {
+                1 & t.$$.dirty[0] && n(17, r = af(P) ? 1 : 2), 8 & t.$$.dirty[0] && n(28, i = N ? N.width : 0), 8 & t.$$.dirty[0] && n(27, o = N ? N.height : 0), 16 & t.$$.dirty[0] && n(18, l = C ? C.width : 140), 1 & t.$$.dirty[0] && n(26, s = Math.min(P.length, 12)), 67108864 & t.$$.dirty[0] && n(7, [c, u] = function(t) {
                     const e = Math.ceil(Math.sqrt(t)),
                         n = Math.ceil(t / e);
                     return 1 === r ? [e, n] : [n, e]
                 }(s), c, (n(8, u), n(26, s), n(0, P))), 268435712 & t.$$.dirty[0] && n(11, O = Math.floor(i / u)), 134217856 & t.$$.dirty[0] && n(12, D = Math.floor(o / c)), 33 & t.$$.dirty[0] && (V.forBrushing || (n(25, L = V.sort(P)), F(1))), 33 & t.$$.dirty[0] && V.forBrushing && H(P), 536870912 & t.$$.dirty[0] && y && n(13, I = !0), 67108865 & t.$$.dirty[0] && n(15, d = Math.ceil(P.length / s)), 100663360 & t.$$.dirty[0] && n(16, f = L.slice((q - 1) * s, q * s))
             }, [P, S, z, N, C, V, q, c, u, j, B, O, D, I, W, d, f, r, l, k, M, T, H, F, K, L, s, o, i, y, () => F(q - 1), () => F(q + 1), function() {
                 V = A(this), n(5, V), n(1, S)
             }, () => H(P), function() {
@@ -12018,45 +12071,45 @@
                 B = A(this), n(10, B)
             }, function() {
                 C = a.entries.get(this)?.contentRect, n(4, C)
             }, t => K(t), function() {
                 N = a.entries.get(this)?.contentRect, n(3, N)
             }]
         }
-        const Cf = class extends _t {
+        const jf = class extends _t {
                 constructor(t) {
-                    super(), wt(this, t, Nf, zf, j, {
+                    super(), wt(this, t, Df, Cf, j, {
                         data: 0,
                         sortingOptions: 1,
                         noPlotsMessage: 2
-                    }, ff, [-1, -1])
+                    }, gf, [-1, -1])
                 }
             },
-            Of = [{
-                name: "Variance",
+            Bf = [{
+                name: "Importance",
                 forBrushing: !1,
                 sort: function(t) {
-                    return 0 !== t.length && rf(t) ? t.sort(((t, e) => ke(t.deviation, e.deviation))) : t
+                    return 0 !== t.length && af(t) ? t.sort(((t, e) => ke(t.deviation, e.deviation))) : t
                 }
             }, {
                 name: "Cluster difference",
                 forBrushing: !1,
                 sort: function(t) {
-                    if (0 === t.length || !rf(t)) return t;
+                    if (0 === t.length || !af(t)) return t;
 
                     function e(t) {
                         return 1 === t.ice.num_clusters ? -1 / 0 : zn(t).cluster_distance
                     }
                     return t.sort(((t, n) => ke(e(t), e(n))))
                 }
             }, {
-                name: "Highlighted similarity",
+                name: "Highlighted line similarity",
                 forBrushing: !0,
                 sort: function(t, e) {
-                    if (0 === t.length || !rf(t) || !e || !e.highlightedIndices || e.highlightedIndices.length <= 1 || !e.featureToIceLines) return t;
+                    if (0 === t.length || !af(t) || !e || !e.highlightedIndices || e.highlightedIndices.length <= 1 || !e.featureToIceLines) return t;
                     const n = e.highlightedIndices,
                         r = e.featureToIceLines,
                         i = Object.fromEntries(t.map((t => {
                             var e;
                             const i = r[t.x_feature],
                                 o = Tn(n.map((t => i[t]))),
                                 l = kn(o).map((t => {
@@ -12072,56 +12125,56 @@
                                     }))
                                 }(o, l, t.ice.centered_pdp);
                             return [t.x_feature, null !== (e = An(a)) && void 0 !== e ? e : 0]
                         })));
                     return t.sort(((t, e) => ke(i[t.x_feature], i[e.x_feature])))
                 }
             }, {
-                name: "Highlighted distribution",
+                name: "Highlighted histogram difference",
                 forBrushing: !0,
                 sort: function(t, e) {
-                    if (!(0 !== t.length && rf(t) && e && e.highlightedDistributions && e.featureInfo)) return t;
+                    if (!(0 !== t.length && af(t) && e && e.highlightedDistributions && e.featureInfo)) return t;
                     const n = e.highlightedDistributions,
                         r = e.featureInfo,
                         i = Object.fromEntries(t.map((t => {
                             const e = n.get(t.x_feature);
                             if (!e) return [t.x_feature, 0];
                             const i = r[t.x_feature].distribution.percents,
                                 o = e.percents;
                             let l = 0;
                             for (let t = 0; t < i.length; t++) l += Math.abs(o[t] - i[t]);
                             return [t.x_feature, l]
                         })));
                     return t.sort(((t, e) => ke(i[t.x_feature], i[e.x_feature])))
                 }
             }],
-            Df = [{
+            Ef = [{
                 name: "Interaction",
                 forBrushing: !1,
                 sort: function(t) {
-                    return 0 === t.length || rf(t) ? t : t.sort(((t, e) => ke(t.H, e.H)))
+                    return 0 === t.length || af(t) ? t : t.sort(((t, e) => ke(t.H, e.H)))
                 }
             }, {
                 name: "Variance",
                 forBrushing: !1,
                 sort: function(t) {
-                    return 0 === t.length || rf(t) ? t : t.sort(((t, e) => ke(t.deviation, e.deviation)))
+                    return 0 === t.length || af(t) ? t : t.sort(((t, e) => ke(t.deviation, e.deviation)))
                 }
             }];
 
-        function jf(t) {
+        function If(t) {
             u(t, "svelte-cuqal2", ".one-way-grid-container.svelte-cuqal2{height:100%;display:flex}.pdp-grid-wrapper.svelte-cuqal2{flex:1;min-width:0}")
         }
 
-        function Bf(t) {
+        function Rf(t) {
             let e, n, r, i, o, l, a;
-            return r = new nf({}), r.$on("changeFilters", t[1]), l = new Cf({
+            return r = new lf({}), r.$on("changeFilters", t[1]), l = new jf({
                 props: {
                     data: t[0],
-                    sortingOptions: Of,
+                    sortingOptions: Bf,
                     noPlotsMessage: "No plots to show."
                 }
             }), {
                 c() {
                     e = p("div"), n = p("div"), bt(r.$$.fragment), i = v(), o = p("div"), bt(l.$$.fragment), $(o, "class", "pdp-grid-wrapper svelte-cuqal2"), $(e, "class", "one-way-grid-container svelte-cuqal2")
                 },
                 m(t, s) {
@@ -12139,51 +12192,51 @@
                 },
                 d(t) {
                     t && f(e), $t(r), $t(l)
                 }
             }
         }
 
-        function Ef(t, e, n) {
+        function Vf(t, e, n) {
             let r, i, o;
             E(t, nr, (t => n(3, i = t))), E(t, Jn, (t => n(4, o = t)));
             let l = o;
             return t.$$.update = () => {
                 12 & t.$$.dirty && n(0, r = i.filter((t => l.includes(t.x_feature))))
             }, [r, function(t) {
                 n(2, l = t.detail)
             }, l, i]
         }
-        const If = class extends _t {
+        const Hf = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Ef, Bf, j, {}, jf)
+                super(), wt(this, t, Vf, Rf, j, {}, If)
             }
         };
 
-        function Rf(t) {
+        function qf(t) {
             u(t, "svelte-fnunp4", ".controls-container.svelte-fnunp4.svelte-fnunp4{height:100%;flex:0 0 200px;min-width:200px;max-width:200px;padding:0.25em;border-right:1px solid var(--gray-1);display:flex;flex-direction:column;gap:0.5em}.feature-selector-wrapper-outer.svelte-fnunp4.svelte-fnunp4{flex:0 1 auto;min-height:0;display:flex;flex-direction:column}.feature-selector-wrapper-middle.svelte-fnunp4.svelte-fnunp4{flex:1;min-height:0;display:flex;flex-direction:column}.feature-selector-wrapper-inner.svelte-fnunp4.svelte-fnunp4{flex:1;min-height:0}.filter-header.svelte-fnunp4+.filter-content.svelte-fnunp4{margin-top:0.25em}.filter-content.svelte-fnunp4.svelte-fnunp4{margin-left:0.75em}hr.svelte-fnunp4.svelte-fnunp4{margin:0.75em 0;border:0;height:1px;background:var(--gray-2)}.two-way-filter-radio.svelte-fnunp4.svelte-fnunp4{display:flex;flex-direction:column}")
         }
 
-        function Vf(t) {
+        function Ff(t) {
             let e, n, r, i, o, l, a, s, u, h, g, b, w, _, L, A, P, S, T, N, C, D, j, B, E, I, R, V, H, q;
 
             function F(e) {
                 t[7](e)
             }
             let W = {
                 title: "Name"
             };
-            void 0 !== t[1] && (W.expanded = t[1]), s = new Zd({
+            void 0 !== t[1] && (W.expanded = t[1]), s = new ef({
                 props: W
             }), X.push((() => vt(s, "expanded", F)));
             let K = {
                 enabledFeatures: t[3],
                 idPrefix: "pdpilot-two"
             };
-            return I = new qd({
+            return I = new Kd({
                 props: K
             }), t[11](I), I.$on("changeNameFilters", t[4]), V = x(t[9][0]), {
                 c() {
                     e = p("div"), n = p("div"), n.textContent = "Feature Filters", r = v(), i = p("button"), i.textContent = "Clear Filters", o = v(), l = p("div"), a = p("div"), bt(s.$$.fragment), h = v(), g = p("div"), b = p("div"), w = p("div"), w.textContent = "Plots must contain", _ = v(), L = p("label"), A = p("input"), P = m("\n          1+ selected feature"), S = v(), T = p("label"), N = p("input"), C = m("\n          2 selected features"), D = v(), j = p("hr"), B = v(), E = p("div"), bt(I.$$.fragment), $(n, "class", "pdpilot-bold"), M(i, "align-self", "start"), $(a, "class", "filter-header svelte-fnunp4"), $(A, "type", "radio"), $(A, "name", "op"), A.__value = "or", k(A, A.__value), $(N, "type", "radio"), $(N, "name", "op"), N.__value = "and", k(N, N.__value), $(b, "class", "two-way-filter-radio svelte-fnunp4"), $(j, "class", "svelte-fnunp4"), $(E, "class", "feature-selector-wrapper-inner svelte-fnunp4"), $(g, "class", "filter-content feature-selector-wrapper-middle svelte-fnunp4"), z(g, "pdp-hide", !t[1]), $(l, "class", "filter-container feature-selector-wrapper-outer svelte-fnunp4"), $(e, "class", "controls-container svelte-fnunp4"), V.p(A, N)
                 },
                 m(u, f) {
                     d(u, e, f), c(e, n), c(e, r), c(e, i), c(e, o), c(e, l), c(l, a), yt(s, a, null), c(l, h), c(l, g), c(g, b), c(b, w), c(b, _), c(b, L), c(L, A), A.checked = A.__value === t[2], c(L, P), c(b, S), c(b, T), c(T, N), N.checked = N.__value === t[2], c(T, C), c(g, D), c(g, j), c(g, B), c(g, E), yt(I, E, null), R = !0, H || (q = [y(i, "click", t[6]), y(A, "change", t[8]), y(A, "change", t[5]), y(N, "change", t[10]), y(N, "change", t[5])], H = !0)
@@ -12202,15 +12255,15 @@
                 },
                 d(n) {
                     n && f(e), $t(s), t[11](null), $t(I), V.r(), H = !1, O(q)
                 }
             }
         }
 
-        function Hf(t, e, n) {
+        function Wf(t, e, n) {
             let r;
             E(t, Jn, (t => n(3, r = t)));
             const i = W();
             let o, l = !0,
                 a = "and",
                 s = r;
             return [o, l, a, r, function(t) {
@@ -12239,30 +12292,30 @@
                 function(t) {
                     X[t ? "unshift" : "push"]((() => {
                         o = t, n(0, o)
                     }))
                 }
             ]
         }
-        const qf = class extends _t {
+        const Kf = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Hf, Vf, j, {}, Rf)
+                super(), wt(this, t, Wf, Ff, j, {}, qf)
             }
         };
 
-        function Ff(t) {
+        function Xf(t) {
             u(t, "svelte-1akrxps", ".two-way-grid-container.svelte-1akrxps{height:100%;display:flex}.pdp-grid-wrapper.svelte-1akrxps{flex:1;min-width:0}")
         }
 
-        function Wf(t) {
+        function Uf(t) {
             let e, n, r, i, o, l, a;
-            return r = new qf({}), r.$on("changeFilters", t[3]), l = new Cf({
+            return r = new Kf({}), r.$on("changeFilters", t[3]), l = new jf({
                 props: {
                     data: t[2],
-                    sortingOptions: Df,
+                    sortingOptions: Ef,
                     noPlotsMessage: 1 === t[0].length && "and" === t[1] ? "No plots to show." : "No plots to show. PDPilot only pre-computes two-way PDPs when it detects likely interaction between the pair of features."
                 }
             }), {
                 c() {
                     e = p("div"), n = p("div"), bt(r.$$.fragment), i = v(), o = p("div"), bt(l.$$.fragment), $(o, "class", "pdp-grid-wrapper svelte-1akrxps"), $(e, "class", "two-way-grid-container svelte-1akrxps")
                 },
                 m(t, s) {
@@ -12280,38 +12333,38 @@
                 },
                 d(t) {
                     t && f(e), $t(r), $t(l)
                 }
             }
         }
 
-        function Kf(t, e, n) {
+        function Yf(t, e, n) {
             let r, i, o;
             E(t, ir, (t => n(4, i = t))), E(t, Jn, (t => n(5, o = t)));
             let l = o,
                 a = "and";
             return t.$$.update = () => {
                 19 & t.$$.dirty && n(2, r = i.filter((t => "and" === a ? l.includes(t.x_feature) && l.includes(t.y_feature) : l.includes(t.x_feature) || l.includes(t.y_feature))))
             }, [l, a, r, function(t) {
                 n(0, l = t.detail.features), n(1, a = t.detail.op)
             }, i]
         }
-        const Xf = class extends _t {
+        const Gf = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Kf, Wf, j, {}, Ff)
+                super(), wt(this, t, Yf, Uf, j, {}, Xf)
             }
         };
 
-        function Uf(t) {
+        function Jf(t) {
             u(t, "svelte-mtrl6h", ".pdpilot-widget-container.svelte-mtrl6h{box-sizing:border-box;width:100%;display:flex;flex-direction:column;font-size:16px;border:1px solid var(--gray-1);background-color:white;color:black;--magenta:rgb(121, 35, 103);--blue:rgb(0, 95, 204);--dark-blue:rgb(1, 51, 104);--gray-0:rgb(247, 247, 247);--gray-1:rgb(226, 226, 226);--gray-2:rgb(198, 198, 198);--gray-3:rgb(171, 171, 171);--gray-4:rgb(145, 145, 145);--gray-5:rgb(119, 119, 119);--gray-6:rgb(94, 94, 94);--gray-7:rgb(71, 71, 71);--gray-8:rgb(48, 48, 48);--gray-9:rgb(27, 27, 27);--black:black;--red:#d62728;--light-red:#fc655a}.pdp-tab-content.svelte-mtrl6h{flex:1;min-height:0}.pdpilot-widget-container.svelte-mtrl6h .pdp-hide{display:none}.pdpilot-widget-container.svelte-mtrl6h canvas,.pdpilot-widget-container.svelte-mtrl6h svg{display:block}.pdpilot-widget-container.svelte-mtrl6h *{box-sizing:border-box;margin:0;padding:0;line-height:1.2}.pdpilot-widget-container.svelte-mtrl6h button{color:var(--blue);background-color:white;border:1px solid var(--blue);border-radius:0.25em;text-align:center;cursor:pointer;font-size:1em;line-height:1em;padding:0.0625em 0.0625em;font-family:inherit}.pdpilot-widget-container.svelte-mtrl6h button:hover:enabled{color:white;background-color:var(--blue)}.pdpilot-widget-container.svelte-mtrl6h button:active:enabled{color:white;background-color:var(--dark-blue);border-color:var(--dark-blue)}.pdpilot-widget-container.svelte-mtrl6h button:disabled{cursor:not-allowed;background-color:transparent;color:var(--gray-4);border-color:var(--gray-4)}.pdpilot-widget-container.svelte-mtrl6h h1{font-size:1.125em;font-weight:500}.pdpilot-widget-container.svelte-mtrl6h h2{font-size:1.0625em;font-weight:500}.pdpilot-widget-container.svelte-mtrl6h .pdpilot-large{font-size:1.125em}.pdpilot-widget-container.svelte-mtrl6h .pdpilot-small{font-size:0.875em}.pdpilot-widget-container.svelte-mtrl6h .pdpilot-bold{font-weight:500}.pdpilot-widget-container.svelte-mtrl6h .pdpilot-icon{width:1em;height:1em}.pdpilot-widget-container.svelte-mtrl6h .pdpilot-cutoff{overflow:hidden;white-space:nowrap;text-overflow:ellipsis}.pdpilot-widget-container.svelte-mtrl6h .icon-tabler{-webkit-transform:translate(0px, 0px);transform:translate(0px, 0px)}")
         }
 
-        function Yf(t) {
+        function Zf(t) {
             let e, n, r, i, o, l, a, s, u, h, g, m, b = `${t[0]}px`;
-            return n = new jr({}), o = new If({}), s = new Xf({}), g = new Bd({}), {
+            return n = new jr({}), o = new Hf({}), s = new Gf({}), g = new Rd({}), {
                 c() {
                     e = p("div"), bt(n.$$.fragment), r = v(), i = p("div"), bt(o.$$.fragment), l = v(), a = p("div"), bt(s.$$.fragment), u = v(), h = p("div"), bt(g.$$.fragment), $(i, "class", "pdp-tab-content svelte-mtrl6h"), z(i, "pdp-hide", "one-way-plots" !== t[1]), $(a, "class", "pdp-tab-content svelte-mtrl6h"), z(a, "pdp-hide", "two-way-plots" !== t[1]), $(h, "class", "pdp-tab-content svelte-mtrl6h"), z(h, "pdp-hide", "detailed-plot" !== t[1]), $(e, "class", "pdpilot-widget-container svelte-mtrl6h"), M(e, "height", b)
                 },
                 m(t, f) {
                     d(t, e, f), yt(n, e, null), c(e, r), c(e, i), yt(o, i, null), c(e, l), c(e, a), yt(s, a, null), c(e, u), c(e, h), yt(g, h, null), m = !0
                 },
                 p(t, [n]) {
@@ -12325,32 +12378,32 @@
                 },
                 d(t) {
                     t && f(e), $t(n), $t(o), $t(s), $t(g)
                 }
             }
         }
 
-        function Gf(t, e, n) {
+        function Qf(t, e, n) {
             let r, i;
             return E(t, dr, (t => n(0, r = t))), E(t, gr, (t => n(1, i = t))), [r, i]
         }
-        const Jf = class extends _t {
+        const th = class extends _t {
             constructor(t) {
-                super(), wt(this, t, Gf, Yf, j, {}, Uf)
+                super(), wt(this, t, Qf, Zf, j, {}, Jf)
             }
         };
-        class Zf extends o.DOMWidgetModel {
+        class eh extends o.DOMWidgetModel {
             defaults() {
                 return Object.assign(Object.assign({}, super.defaults()), {
-                    _model_name: Zf.model_name,
-                    _model_module: Zf.model_module,
-                    _model_module_version: Zf.model_module_version,
-                    _view_name: Zf.view_name,
-                    _view_module: Zf.view_module,
-                    _view_module_version: Zf.view_module_version,
+                    _model_name: eh.model_name,
+                    _model_module: eh.model_module,
+                    _model_module_version: eh.model_module_version,
+                    _view_name: eh.view_name,
+                    _view_module: eh.view_module,
+                    _view_module_version: eh.view_module_version,
                     feature_names: [],
                     feature_info: {},
                     dataset: {},
                     labels: [],
                     num_instances: 0,
                     one_way_pds: [],
                     feature_to_ice_lines: {},
@@ -12364,16 +12417,16 @@
                     height: 600,
                     highlighted_indices: [],
                     two_way_to_calculate: [],
                     cluster_update: {}
                 })
             }
         }
-        Zf.serializers = Object.assign({}, o.DOMWidgetModel.serializers), Zf.model_name = "PDPilotModel", Zf.model_module = n, Zf.model_module_version = e, Zf.view_name = "PDPilotView", Zf.view_module = n, Zf.view_module_version = e;
-        class Qf extends o.DOMWidgetView {
+        eh.serializers = Object.assign({}, o.DOMWidgetModel.serializers), eh.model_name = "PDPilotModel", eh.model_module = n, eh.model_module_version = e, eh.view_name = "PDPilotView", eh.view_module = n, eh.view_module_version = e;
+        class nh extends o.DOMWidgetView {
             render() {
                 (function(t) {
                     Jn = Gn("feature_names", [], t), Zn = Gn("feature_info", {}, t), Qn = Gn("dataset", {}, t), tr = Gn("labels", [], t), er = Gn("num_instances", 0, t), nr = Gn("one_way_pds", [], t), rr = Gn("feature_to_ice_lines", {}, t), ir = Gn("two_way_pds", [], t), or = Gn("two_way_pdp_extent", [0, 0], t), lr = Gn("two_way_interaction_extent", [0, 0], t), ar = Gn("one_way_pdp_extent", [0, 0], t), sr = Gn("ice_line_extent", [0, 0], t), cr = Gn("ice_cluster_center_extent", [0, 0], t), ur = Gn("centered_ice_line_extent", [0, 0], t), dr = Gn("height", 600, t), fr = Gn("highlighted_indices", [], t), hr = Gn("two_way_to_calculate", [], t), pr = Gn("cluster_update", {}, t), gr = Mt("one-way-plots"), mr = Lt(nr, (t => new Map(t.map((t => [t.x_feature, t]))))), vr = Lt(tr, (t => 2 === new Set(t).size)), br = Lt([tr, vr], (([t, e]) => {
                         const n = [Math.min(...t), Math.max(...t)];
                         return e ? n : qn(n)
                     }));
                     const e = t.get("one_way_pds"),
@@ -12383,15 +12436,15 @@
                     }, ((t, e) => ({
                         x: (.5 + .7548776662466927 * e) % 1,
                         y: (.5 + .5698402909980532 * e) % 1
                     }))))), Mr = Mt(!1), Lr = Mt(""), Ar = Lt(fr, (t => new Set(t))), Pr = Lt([Zn, Qn, fr], (([t, e, n]) => new Map(Object.entries(t).map((([t, r]) => [t, Vn(r, e[t], n)]))))), Sr = Lt(or, (t => an().domain(qn(t)).interpolator(dn).unknown("black"))), zr = Lt(lr, (t => {
                         const e = qn([0, t[1]])[1];
                         return sn().domain([-e, 0, e]).interpolator(fn).unknown("black")
                     }))
-                })(this.model), new Jf({
+                })(this.model), new th({
                     target: this.el
                 })
             }
         }
         window.__webpack_public_path__ = document.querySelector("body").getAttribute("data-base-url") + "nbextensions/pdpilot"
     })(), i
 })()));
```

### Comparing `pdpilot-0.5.1/pdpilot/pdp.py` & `pdpilot-0.5.2/pdpilot/pdp.py`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/pdpilot/tqdm_joblib.py` & `pdpilot-0.5.2/pdpilot/tqdm_joblib.py`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/pdpilot/widget.py` & `pdpilot-0.5.2/pdpilot/widget.py`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/pdpilot.egg-info/PKG-INFO` & `pdpilot-0.5.2/pdpilot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdpilot
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Jupyter widget for exploring PDP and ICE plots.
 Home-page: https://github.com/DanielKerrigan/PDPilot
 Author: Daniel Kerrigan
 Author-email: kerrigan.d@northeastern.edu
 License: BSD
 Keywords: Jupyter,Widgets,IPython,PDP,ICE
 Platform: Linux
```

### Comparing `pdpilot-0.5.1/pdpilot.egg-info/SOURCES.txt` & `pdpilot-0.5.2/pdpilot.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -39,18 +39,18 @@
 pdpilot/widget.py
 pdpilot.egg-info/PKG-INFO
 pdpilot.egg-info/SOURCES.txt
 pdpilot.egg-info/dependency_links.txt
 pdpilot.egg-info/requires.txt
 pdpilot.egg-info/top_level.txt
 pdpilot/labextension/package.json
-pdpilot/labextension/static/568.fc735409708fd22de78c.js
+pdpilot/labextension/static/568.be4561957748b400120d.js
 pdpilot/labextension/static/713.5fb1220914a3fc9b6db7.js
 pdpilot/labextension/static/713.5fb1220914a3fc9b6db7.js.LICENSE.txt
-pdpilot/labextension/static/remoteEntry.7d03101ac0d410913165.js
+pdpilot/labextension/static/remoteEntry.93d73cafbbe8e20d7f23.js
 pdpilot/labextension/static/style.js
 pdpilot/labextension/static/third-party-licenses.json
 pdpilot/nbextension/extension.js
 pdpilot/nbextension/index.js
 src/drawing.ts
 src/extension.ts
 src/fast-kde.d.ts
```

### Comparing `pdpilot-0.5.1/setup.py` & `pdpilot-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/DetailedPlot.svelte` & `pdpilot-0.5.2/src/components/DetailedPlot.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/FeatureKindFilter.svelte` & `pdpilot-0.5.2/src/components/FeatureKindFilter.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/FeatureNameFilter.svelte` & `pdpilot-0.5.2/src/components/FeatureNameFilter.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/InfoTooltip.svelte` & `pdpilot-0.5.2/src/components/InfoTooltip.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/OneWayDetailedPlot.svelte` & `pdpilot-0.5.2/src/components/OneWayDetailedPlot.svelte`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             xDomain={featureInfo.kind === 'categorical'
               ? pd.x_values
               : [pd.x_values[0], pd.x_values[pd.x_values.length - 1]]}
             yDomain={$labelExtent}
             colorDomain={[0, 1]}
             colorScheme={'highlight'}
             xLabel={pd.x_feature}
-            yLabel={'Ground Truth'}
+            yLabel={'Ground truth'}
             colorLabel=""
             xAxisIntegerOnly={featureInfo.subkind === 'discrete'}
             yAxisIntegerOnly={false}
             xAxisValueMap={'value_map' in featureInfo
               ? featureInfo.value_map
               : {}}
             yAxisValueMap={{}}
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 pd} features={getClustering(pd).interacting_features} /> {:else if
 $detailedContextKind === 'scatterplot'}
 num_instances }, (_, i) => $highlightedIndicesSet.has(i) ? 1 : 0 )} xKind=
 {featureInfo.kind} yKind={$isClassification ? 'categorical' : 'quantitative'}
 colorKind={'categorical'} xDomain={featureInfo.kind === 'categorical' ?
 pd.x_values : [pd.x_values[0], pd.x_values[pd.x_values.length - 1]]} yDomain=
 {$labelExtent} colorDomain={[0, 1]} colorScheme={'highlight'} xLabel=
-{pd.x_feature} yLabel={'Ground Truth'} colorLabel="" xAxisIntegerOnly=
+{pd.x_feature} yLabel={'Ground truth'} colorLabel="" xAxisIntegerOnly=
 {featureInfo.subkind === 'discrete'} yAxisIntegerOnly={false} xAxisValueMap=
 {'value_map' in featureInfo ? featureInfo.value_map : {}} yAxisValueMap={{}}
 xDistribution={featureInfo.distribution} yDistribution={null} opacity={0.5}
 allowBrushing={true} showMarginalDistribution={true} marginTop=
 {marginalPlotHeight + 3} marginRight={marginalPlotHeight + 3}
 {marginalPlotHeight} /> {/if}
 {/if}
```

### Comparing `pdpilot-0.5.1/src/components/OneWayGridContainer.svelte` & `pdpilot-0.5.2/src/components/OneWayGridContainer.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/OneWayGridFilters.svelte` & `pdpilot-0.5.2/src/components/OneWayGridFilters.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/PDP.svelte` & `pdpilot-0.5.2/src/components/PDP.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/PDPGrid.svelte` & `pdpilot-0.5.2/src/components/PDPGrid.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     { value: 'lines', title: 'Standard' },
     { value: 'centered-lines', title: 'Centered' },
     { value: 'cluster-centers', title: 'Clusters' },
   ];
 
   let iceLevel: ICELevel = 'lines';
 
-  let colorShows: 'predictions' | 'interactions' = 'interactions';
+  let colorShows: 'predictions' | 'interactions' = 'predictions';
 
   let gridContentRect: DOMRectReadOnly | undefined | null;
   let legendContentRect: DOMRectReadOnly | undefined | null;
 
   $: gridWidth = gridContentRect ? gridContentRect.width : 0;
   $: gridHeight = gridContentRect ? gridContentRect.height : 0;
 
@@ -215,37 +215,38 @@
 
       <InfoTooltip
         kind="help"
         left="0"
         top="0"
         marginRight="1em"
         marginTop="1.5em"
-        width="30em"
+        width="25em"
       >
         <div>
           {#if ways === 1}
             <ul>
               <li>
-                <span class="pdpilot-bold">Variance:</span> Plots that have more
+                <span class="pdpilot-bold">Importance:</span> Plots that have more
                 variance in their ICE lines are ranked higher.
               </li>
               <li>
                 <span class="pdpilot-bold">Cluster difference:</span> Plots that
                 have ICE clusters farther from the partial dependence line are ranked
                 higher.
               </li>
               <li>
-                <span class="pdpilot-bold">Highlighted similarity:</span> Plots where
-                the highlighted lines are closer together and farther from the partial
-                dependence line are ranked higher.
+                <span class="pdpilot-bold">Highlighted line similarity:</span> Plots
+                where the highlighted lines are closer together and farther from
+                the partial dependence line are ranked higher.
               </li>
               <li>
-                <span class="pdpilot-bold">Highlighted distribution:</span> Plots
-                for features whose distributions of highlighted instances are more
-                different from the overall distributions are ranked higher.
+                <span class="pdpilot-bold"
+                  >Highlighted histogram difference:</span
+                > Plots for features whose distributions of highlighted instances
+                are more different from the overall distributions are ranked higher.
               </li>
             </ul>
           {:else}
             <ul>
               <li>
                 <span class="pdpilot-bold">Interaction:</span> Plots for feature
                 pairs with more interaction are ranked higher.
@@ -304,16 +305,16 @@
 
     <div class="two-way-color-container">
       {#if ways === 2}
         <div class="label-and-input dont-shrink">
           <label class="label-and-input">
             Color
             <select bind:value={colorShows}>
-              <option value="interactions">interactions</option>
-              <option value="predictions">predictions</option>
+              <option value="predictions">Predictions</option>
+              <option value="interactions">Interactions</option>
             </select>
           </label>
 
           <InfoTooltip
             kind="help"
             right="0"
             top="0"
```

#### html2text {}

```diff
@@ -2,36 +2,36 @@
 {currentPage}
 = numPages} on:click={() => setPage(currentPage + 1)} title="Next page" >
 {#each sortingOptions as option}
 {option.name}
 {/each}
 
 {#if ways === 1}
-    * Variance: Plots that have more variance in their ICE lines are ranked
+    * Importance: Plots that have more variance in their ICE lines are ranked
       higher.
     * Cluster difference: Plots that have ICE clusters farther from the partial
       dependence line are ranked higher.
-    * Highlighted similarity: Plots where the highlighted lines are closer
+    * Highlighted line similarity: Plots where the highlighted lines are closer
       together and farther from the partial dependence line are ranked higher.
-    * Highlighted distribution: Plots for features whose distributions of
-      highlighted instances are more different from the overall distributions
-      are ranked higher.
+    * Highlighted histogram difference: Plots for features whose distributions
+      of highlighted instances are more different from the overall
+      distributions are ranked higher.
 {:else}
     * Interaction: Plots for feature pairs with more interaction are ranked
       higher.
     * Variance: Plots that have more variation in their average predictions are
       ranked higher.
 {/if}
 {#if ways === 1 && sortingOption.forBrushing}
 {#each iceLevels as { value, title }}
 value}>{title}
 {/each}
   {/if}  ⁰Scale locally
 {#if ways === 2}
- Color [One of: interactions/predictions]
+ Color [One of: Predictions/Interactions]
 {#if colorShows === 'interactions'} This color scale shows the difference
 between the value in a two-way PDP and the expected value if there was no
 interaction between the pair of features. It indicates whether the interaction
 between the two features makes the model's average prediction for the given
 values
 .1 )} style:border-radius="4px" style:padding="0.125em 0.25em" style:
 color="white">lower or
```

### Comparing `pdpilot-0.5.1/src/components/SegmentedButton.svelte` & `pdpilot-0.5.2/src/components/SegmentedButton.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/Tabs.svelte` & `pdpilot-0.5.2/src/components/Tabs.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/ToggleHeader.svelte` & `pdpilot-0.5.2/src/components/ToggleHeader.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/TwoWayDetailedPlot.svelte` & `pdpilot-0.5.2/src/components/TwoWayDetailedPlot.svelte`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
       yDomain={$feature_info[pd.y_feature].kind === 'categorical'
         ? pd.y_axis
         : [pd.y_axis[0], pd.y_axis[pd.y_axis.length - 1]]}
       colorDomain={$labelExtent}
       colorScheme={$isClassification ? 'classes' : 'sequential'}
       xLabel={pd.x_feature}
       yLabel={pd.y_feature}
-      colorLabel="Ground Truth"
+      colorLabel="Ground truth"
       xAxisIntegerOnly={xFeatureInfo.subkind === 'discrete'}
       yAxisIntegerOnly={yFeatureInfo.subkind === 'discrete'}
       xAxisValueMap={'value_map' in xFeatureInfo ? xFeatureInfo.value_map : {}}
       yAxisValueMap={'value_map' in yFeatureInfo ? yFeatureInfo.value_map : {}}
       xDistribution={xFeatureInfo.distribution}
       yDistribution={yFeatureInfo.distribution}
       opacity={1}
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 colorValues={$labels} xKind={xFeatureInfo.kind} yKind={yFeatureInfo.kind}
 colorKind={$isClassification ? 'categorical' : 'quantitative'} xDomain=
 {xFeatureInfo.kind === 'categorical' ? pd.x_axis : [pd.x_axis[0], pd.x_axis
 [pd.x_axis.length - 1]]} yDomain={$feature_info[pd.y_feature].kind ===
 'categorical' ? pd.y_axis : [pd.y_axis[0], pd.y_axis[pd.y_axis.length - 1]]}
 colorDomain={$labelExtent} colorScheme={$isClassification ? 'classes' :
 'sequential'} xLabel={pd.x_feature} yLabel={pd.y_feature} colorLabel="Ground
-Truth" xAxisIntegerOnly={xFeatureInfo.subkind === 'discrete'} yAxisIntegerOnly=
+truth" xAxisIntegerOnly={xFeatureInfo.subkind === 'discrete'} yAxisIntegerOnly=
 {yFeatureInfo.subkind === 'discrete'} xAxisValueMap={'value_map' in
 xFeatureInfo ? xFeatureInfo.value_map : {}} yAxisValueMap={'value_map' in
 yFeatureInfo ? yFeatureInfo.value_map : {}} xDistribution=
 {xFeatureInfo.distribution} yDistribution={yFeatureInfo.distribution} opacity=
 {1} allowBrushing={false} showMarginalDistribution={true} marginTop=
 {marginalPlotHeight + 3} marginRight={marginalPlotHeight + 3}
 {marginalPlotHeight} />
```

### Comparing `pdpilot-0.5.1/src/components/TwoWayGridContainer.svelte` & `pdpilot-0.5.2/src/components/TwoWayGridContainer.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/TwoWayGridFilters.svelte` & `pdpilot-0.5.2/src/components/TwoWayGridFilters.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/Widget.svelte` & `pdpilot-0.5.2/src/components/Widget.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/vis/axis/Label.svelte` & `pdpilot-0.5.2/src/components/vis/axis/Label.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/vis/axis/XAxis.svelte` & `pdpilot-0.5.2/src/components/vis/axis/XAxis.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/vis/axis/YAxis.svelte` & `pdpilot-0.5.2/src/components/vis/axis/YAxis.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/vis/distribution/Scatterplot.svelte` & `pdpilot-0.5.2/src/components/vis/distribution/Scatterplot.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/vis/ice-clusters/ClusterDescriptions.svelte` & `pdpilot-0.5.2/src/components/vis/ice-clusters/ClusterDescriptions.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/vis/legends/CategoricalColorLegend.svelte` & `pdpilot-0.5.2/src/components/vis/legends/CategoricalColorLegend.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/vis/legends/QuantitativeColorLegend.svelte` & `pdpilot-0.5.2/src/components/vis/legends/QuantitativeColorLegend.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/vis/marginal/MarginalBarChart.svelte` & `pdpilot-0.5.2/src/components/vis/marginal/MarginalBarChart.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/vis/marginal/MarginalHistogram.svelte` & `pdpilot-0.5.2/src/components/vis/marginal/MarginalHistogram.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/vis/marginal/MarginalPDP.svelte` & `pdpilot-0.5.2/src/components/vis/marginal/MarginalPDP.svelte`

 * *Files 26% similar despite different names*

```diff
@@ -27,15 +27,27 @@
       : x(pd.x_values[i]);
 
   $: yAccessor = (i: number) => y(pd.mean_predictions[i]);
 
   $: line = d3line<number>()
     .x(direction === 'horizontal' ? xAccessor : yAccessor)
     .y(direction === 'horizontal' ? yAccessor : xAccessor);
+
+  $: radius = 'bandwidth' in x ? Math.min(2, x.bandwidth() / 2) : 0;
 </script>
 
 <g transform="translate({translate})">
   <path d={line(I)} {stroke} fill="none" />
+  {#if 'bandwidth' in x}
+    {#each I as i}
+      <circle
+        cx={direction === 'horizontal' ? xAccessor(i) : yAccessor(i)}
+        cy={direction === 'horizontal' ? yAccessor(i) : xAccessor(i)}
+        r={radius}
+        fill={stroke}
+      />
+    {/each}
+  {/if}
 </g>
 
 <style>
 </style>
```

#### html2text {}

```diff
@@ -1,3 +1,5 @@
 
-stroke} fill="none" />
+stroke} fill="none" /> {#if 'bandwidth' in x} {#each I as i}
+== 'horizontal' ? xAccessor(i) : yAccessor(i)} cy={direction === 'horizontal' ?
+yAccessor(i) : xAccessor(i)} r={radius} fill={stroke} /> {/each} {/if}
```

### Comparing `pdpilot-0.5.1/src/components/vis/one-way/ClusterCenters.svelte` & `pdpilot-0.5.2/src/components/vis/one-way/ClusterCenters.svelte`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     scale={x}
     y={chartHeight - margin.bottom}
     label={pd.x_feature}
     integerOnly={feature.subkind === 'discrete'}
     value_map={'value_map' in feature ? feature.value_map : {}}
   />
 
-  <YAxis scale={y} x={margin.left} label={'centered prediction'} />
+  <YAxis scale={y} x={margin.left} label={'Centered prediction'} />
 
   {#if showMarginalDistribution}
     {#if 'bandwidth' in x}
       <MarginalBarChart
         data={$feature_info[pd.x_feature].distribution}
         {x}
         height={marginalPlotHeight}
```

### Comparing `pdpilot-0.5.1/src/components/vis/one-way/ClusterLines.svelte` & `pdpilot-0.5.2/src/components/vis/one-way/ClusterLines.svelte`

 * *Files 0% similar despite different names*

```diff
@@ -537,15 +537,15 @@
           <text
             dominant-baseline="middle"
             text-anchor="end"
             font-size="10"
             x={width - margin.right}
             y={margin.top / 2}>{cluster.filteredIndices.length} instances</text
           >
-          <YAxis scale={y} x={margin.left} label={'centered prediction'} />
+          <YAxis scale={y} x={margin.left} label={'Centered prediction'} />
           <XAxis
             scale={x}
             y={facetHeight - margin.bottom}
             showTickLabels={cluster.id === clusterIds[clusterIds.length - 1]}
             showAxisLabel={cluster.id === clusterIds[clusterIds.length - 1]}
             label={copyPd.x_feature}
             integerOnly={feature.subkind === 'discrete'}
```

### Comparing `pdpilot-0.5.1/src/components/vis/one-way/FeatureVsLabels.svelte` & `pdpilot-0.5.2/src/components/vis/one-way/FeatureVsLabels.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -302,15 +302,15 @@
       integerOnly={feature.subkind === 'discrete'}
       value_map={'value_map' in feature ? feature.value_map : {}}
     />
 
     <YAxis
       scale={y}
       x={margin.left}
-      label="Ground Truth"
+      label="Ground truth"
       integerOnly={false}
       value_map={{}}
     />
 
     <g bind:this={group} />
 
     {#if showMarginalDistribution}
```

### Comparing `pdpilot-0.5.1/src/components/vis/one-way/Lines.svelte` & `pdpilot-0.5.2/src/components/vis/one-way/Lines.svelte`

 * *Files 1% similar despite different names*

```diff
@@ -335,15 +335,15 @@
         integerOnly={feature.subkind === 'discrete'}
         value_map={'value_map' in feature ? feature.value_map : {}}
       />
 
       <YAxis
         scale={y}
         x={margin.left}
-        label={center ? 'centered prediction' : 'prediction'}
+        label={center ? 'Centered prediction' : 'Prediction'}
       />
 
       {#if showMarginalDistribution}
         {#if allowBrushing && highlightedDistribution && $highlighted_indices.length > 0}
           {#if 'bandwidth' in x}
             <MarginalBarChart
               data={highlightedDistribution}
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 
 width} {height}>
  margin.bottom} label={pd.x_feature} integerOnly={feature.subkind ===
 'discrete'} value_map={'value_map' in feature ? feature.value_map : {}} />
- 'centered prediction' : 'prediction'} /> {#if showMarginalDistribution} {#if
+ 'Centered prediction' : 'Prediction'} /> {#if showMarginalDistribution} {#if
 allowBrushing && highlightedDistribution && $highlighted_indices.length > 0}
 {#if 'bandwidth' in x}
 x} height={marginalPlotHeight} direction="horizontal" translate={[0, margin.top
 - marginalPlotHeight]} unit="percent" maxValue={maxPercent} /> {:else}
 x} height={marginalPlotHeight} direction="horizontal" translate={[0, margin.top
 - marginalPlotHeight]} unit="percent" maxValue={maxPercent} /> {/if} {/if} {#if
 'bandwidth' in x}
```

### Comparing `pdpilot-0.5.1/src/components/vis/one-way/OneWayChart.svelte` & `pdpilot-0.5.2/src/components/vis/one-way/OneWayChart.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/vis/two-way/FeatureVsFeature.svelte` & `pdpilot-0.5.2/src/components/vis/two-way/FeatureVsFeature.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/vis/two-way/TwoWayChart.svelte` & `pdpilot-0.5.2/src/components/vis/two-way/TwoWayChart.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/vis/two-way/TwoWayHeatmap.svelte` & `pdpilot-0.5.2/src/components/vis/two-way/TwoWayHeatmap.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/components/vis/two-way/TwoWayLines.svelte` & `pdpilot-0.5.2/src/components/vis/two-way/TwoWayLines.svelte`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/drawing.ts` & `pdpilot-0.5.2/src/drawing.ts`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
   radius: number,
   alpha: number
 ) {
   if (!ctx) {
     return;
   }
 
-  const minRainCloudSize = 40;
+  const minRainCloudSize = 20;
 
   ctx.save();
 
   ctx.clearRect(0, 0, width, height);
 
   if ('bandwidth' in x && 'bandwidth' in y) {
     // categorical scatterplot
```

### Comparing `pdpilot-0.5.1/src/extension.ts` & `pdpilot-0.5.2/src/extension.ts`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/plugin.ts` & `pdpilot-0.5.2/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/sorting.ts` & `pdpilot-0.5.2/src/sorting.ts`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     }
     return Math.sqrt(distanceToPd) / Math.sqrt(distanceToHighltedCenter);
   });
 }
 
 const singlePDPSortingOptions: PDSortingOption[] = [
   {
-    name: 'Variance',
+    name: 'Importance',
     forBrushing: false,
     sort: function (data: OneWayPD[] | TwoWayPD[]): OneWayPD[] | TwoWayPD[] {
       if (data.length === 0 || !isOneWayPdArray(data)) {
         return data;
       }
 
       return data.sort((a, b) => descending(a.deviation, b.deviation));
@@ -52,15 +52,15 @@
         return getClustering(pd).cluster_distance;
       }
 
       return data.sort((a, b) => descending(getDistance(a), getDistance(b)));
     },
   },
   {
-    name: 'Highlighted similarity',
+    name: 'Highlighted line similarity',
     forBrushing: true,
     sort: function (
       data: OneWayPD[] | TwoWayPD[],
       extra
     ): OneWayPD[] | TwoWayPD[] {
       if (
         data.length === 0 ||
@@ -97,15 +97,15 @@
 
       return data.sort((a, b) =>
         descending(scores[a.x_feature], scores[b.x_feature])
       );
     },
   },
   {
-    name: 'Highlighted distribution',
+    name: 'Highlighted histogram difference',
     forBrushing: true,
     sort: function (
       data: OneWayPD[] | TwoWayPD[],
       extra
     ): OneWayPD[] | TwoWayPD[] {
       if (
         data.length === 0 ||
```

### Comparing `pdpilot-0.5.1/src/stores.ts` & `pdpilot-0.5.2/src/stores.ts`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/types.ts` & `pdpilot-0.5.2/src/types.ts`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/utils.ts` & `pdpilot-0.5.2/src/utils.ts`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/vis-utils.ts` & `pdpilot-0.5.2/src/vis-utils.ts`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/src/widget.ts` & `pdpilot-0.5.2/src/widget.ts`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/tsconfig.json` & `pdpilot-0.5.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `pdpilot-0.5.1/webpack.config.js` & `pdpilot-0.5.2/webpack.config.js`

 * *Files identical despite different names*

