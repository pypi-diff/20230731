# Comparing `tmp/scrilla-1.5.7.tar.gz` & `tmp/scrilla-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrilla-1.5.7.tar", last modified: Wed Jun 29 16:29:03 2022, max compression
+gzip compressed data, was "scrilla-1.6.0.tar", last modified: Mon Jul 31 13:40:43 2023, max compression
```

## Comparing `scrilla-1.5.7.tar` & `scrilla-1.6.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.476354 scrilla-1.5.7/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35821 2022-06-29 16:28:02.000000 scrilla-1.5.7/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      353 2022-06-29 16:28:02.000000 scrilla-1.5.7/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6798 2022-06-29 16:29:03.476354 scrilla-1.5.7/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6444 2022-06-29 16:28:02.000000 scrilla-1.5.7/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       74 2022-06-29 16:28:02.000000 scrilla-1.5.7/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1243 2022-06-29 16:29:03.476354 scrilla-1.5.7/setup.cfg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.460353 scrilla-1.5.7/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.464353 scrilla-1.5.7/src/scrilla/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4699 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.468353 scrilla-1.5.7/src/scrilla/analysis/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1880 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15723 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/estimators.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4557 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/integration.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16836 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/markets.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.468353 scrilla-1.5.7/src/scrilla/analysis/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/models/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.468353 scrilla-1.5.7/src/scrilla/analysis/models/geometric/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/models/geometric/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9339 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/models/geometric/probability.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    94742 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/models/geometric/statistics.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.468353 scrilla-1.5.7/src/scrilla/analysis/models/reversion/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/models/reversion/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/models/reversion/probability.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/models/reversion/statistics.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.468353 scrilla-1.5.7/src/scrilla/analysis/objects/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/objects/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15424 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/objects/cashflow.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19346 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/objects/portfolio.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18290 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/optimizer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10330 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/analysis/plotter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    45220 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/cache.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.468353 scrilla-1.5.7/src/scrilla/cloud/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/cloud/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6962 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/cloud/aws.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.464353 scrilla-1.5.7/src/scrilla/data/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.472353 scrilla-1.5.7/src/scrilla/data/assets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      431 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/arrow-back-circle-outline.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      298 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/arrow-back-circle-sharp.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      709 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/calculator-outline.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      368 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/calculator-sharp.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      683 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/calendar-number-outline.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      956 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/calendar-number-sharp.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      773 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/calendar-outline.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      877 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/calendar-sharp.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      382 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/card-outline.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      289 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/card-sharp.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      746 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/cash-outline.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      556 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/cash-sharp.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      415 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/close-circle-outline.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      310 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/close-circle-sharp.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      501 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/document-text-outline.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      348 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/document-text-sharp.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      452 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/download-outline.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      295 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/download-sharp.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      561 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/help-circle-outline.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1339 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/help-circle-sharp.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      593 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/information-circle-outline.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      297 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/information-circle-sharp.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      902 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/logo-github.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      993 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/logo-python.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2464 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/okay-sharp.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2810 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/okay.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      617 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/trash-outline.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      515 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/assets/trash-sharp.svg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.472353 scrilla-1.5.7/src/scrilla/data/cache/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/cache/.gitkeep
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:28:55.000000 scrilla-1.5.7/src/scrilla/data/cache/scrilla.db
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.472353 scrilla-1.5.7/src/scrilla/data/meta/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      179 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/meta/data.json
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.472353 scrilla-1.5.7/src/scrilla/data/static/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/static/.gitkeep
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.472353 scrilla-1.5.7/src/scrilla/data/tmp/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/data/tmp/.gitkeep
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19628 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/files.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.472353 scrilla-1.5.7/src/scrilla/gui/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/gui/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2103 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/gui/definitions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2706 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/gui/formats.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2260 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/gui/main.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.476354 scrilla-1.5.7/src/scrilla/gui/styles/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6585 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/gui/styles/app.qss
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1005 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/gui/styles/icons.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1147 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/gui/styles/themes.json
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.476354 scrilla-1.5.7/src/scrilla/gui/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2391 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/gui/templates/splash.html
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1799 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/gui/utilities.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.476354 scrilla-1.5.7/src/scrilla/gui/widgets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/gui/widgets/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    27927 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/gui/widgets/components.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11738 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/gui/widgets/factories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26374 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/gui/widgets/functions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9162 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/gui/widgets/menu.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    55567 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/main.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    44329 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/services.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14288 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/settings.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.476354 scrilla-1.5.7/src/scrilla/static/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/static/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4998 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/static/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      548 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/static/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    28367 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/static/definitions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5674 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/static/formats.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      623 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/static/functions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7437 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/static/keys.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.476354 scrilla-1.5.7/src/scrilla/util/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/util/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16235 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/util/dater.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3624 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/util/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2563 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/util/helper.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14322 2022-06-29 16:28:02.000000 scrilla-1.5.7/src/scrilla/util/outputter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-06-29 16:28:30.000000 scrilla-1.5.7/src/scrilla/version.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-29 16:29:03.464353 scrilla-1.5.7/src/scrilla.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6798 2022-06-29 16:29:02.000000 scrilla-1.5.7/src/scrilla.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3393 2022-06-29 16:29:03.000000 scrilla-1.5.7/src/scrilla.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-29 16:29:02.000000 scrilla-1.5.7/src/scrilla.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2022-06-29 16:29:03.000000 scrilla-1.5.7/src/scrilla.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      197 2022-06-29 16:29:03.000000 scrilla-1.5.7/src/scrilla.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2022-06-29 16:29:03.000000 scrilla-1.5.7/src/scrilla.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.703401 scrilla-1.6.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35821 2023-07-31 13:38:06.000000 scrilla-1.6.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      353 2023-07-31 13:38:06.000000 scrilla-1.6.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7173 2023-07-31 13:40:43.703401 scrilla-1.6.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6821 2023-07-31 13:38:06.000000 scrilla-1.6.0/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       74 2023-07-31 13:38:06.000000 scrilla-1.6.0/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1243 2023-07-31 13:40:43.703401 scrilla-1.6.0/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.679401 scrilla-1.6.0/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.683401 scrilla-1.6.0/src/scrilla/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4699 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.687401 scrilla-1.6.0/src/scrilla/analysis/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1880 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16929 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/estimators.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4557 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/integration.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16836 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/markets.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.687401 scrilla-1.6.0/src/scrilla/analysis/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/models/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.687401 scrilla-1.6.0/src/scrilla/analysis/models/geometric/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/models/geometric/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9339 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/models/geometric/probability.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    94984 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/models/geometric/statistics.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.687401 scrilla-1.6.0/src/scrilla/analysis/models/reversion/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/models/reversion/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/models/reversion/probability.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/models/reversion/statistics.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.687401 scrilla-1.6.0/src/scrilla/analysis/objects/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/objects/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15424 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/objects/cashflow.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19346 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/objects/portfolio.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18288 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/optimizer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10330 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/analysis/plotter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    47911 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/cache.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.687401 scrilla-1.6.0/src/scrilla/cloud/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/cloud/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6962 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/cloud/aws.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.679401 scrilla-1.6.0/src/scrilla/data/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.695402 scrilla-1.6.0/src/scrilla/data/assets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      431 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/arrow-back-circle-outline.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      298 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/arrow-back-circle-sharp.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      709 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/calculator-outline.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      368 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/calculator-sharp.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      683 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/calendar-number-outline.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      956 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/calendar-number-sharp.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      773 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/calendar-outline.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      877 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/calendar-sharp.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      382 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/card-outline.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      289 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/card-sharp.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      746 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/cash-outline.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      556 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/cash-sharp.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      415 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/close-circle-outline.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      310 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/close-circle-sharp.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      501 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/document-text-outline.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      348 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/document-text-sharp.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      452 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/download-outline.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      295 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/download-sharp.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      561 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/help-circle-outline.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1339 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/help-circle-sharp.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      593 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/information-circle-outline.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      297 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/information-circle-sharp.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      902 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/logo-github.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      993 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/logo-python.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2464 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/okay-sharp.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2810 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/okay.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      617 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/trash-outline.svg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      515 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/assets/trash-sharp.svg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.695402 scrilla-1.6.0/src/scrilla/data/cache/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/cache/.gitkeep
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:35.000000 scrilla-1.6.0/src/scrilla/data/cache/scrilla.db
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.695402 scrilla-1.6.0/src/scrilla/data/meta/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      179 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/meta/data.json
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.695402 scrilla-1.6.0/src/scrilla/data/static/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/static/.gitkeep
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.695402 scrilla-1.6.0/src/scrilla/data/tmp/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/data/tmp/.gitkeep
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19685 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/files.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.695402 scrilla-1.6.0/src/scrilla/gui/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/gui/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3845 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/gui/definitions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2706 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/gui/formats.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2282 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/gui/main.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.695402 scrilla-1.6.0/src/scrilla/gui/styles/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6585 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/gui/styles/app.qss
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1004 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/gui/styles/icons.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1147 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/gui/styles/themes.json
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.695402 scrilla-1.6.0/src/scrilla/gui/templates/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2391 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/gui/templates/splash.html
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1799 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/gui/utilities.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.699401 scrilla-1.6.0/src/scrilla/gui/widgets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/gui/widgets/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    31369 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/gui/widgets/components.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12439 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/gui/widgets/factories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26439 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/gui/widgets/functions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9822 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/gui/widgets/menu.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    55158 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/main.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    45025 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/services.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14306 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.699401 scrilla-1.6.0/src/scrilla/static/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/static/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4998 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/static/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      548 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/static/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    28781 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/static/definitions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5704 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/static/formats.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      623 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/static/functions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7437 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/static/keys.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.699401 scrilla-1.6.0/src/scrilla/util/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/util/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16193 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/util/dater.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3624 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/util/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2563 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/util/helper.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14623 2023-07-31 13:38:06.000000 scrilla-1.6.0/src/scrilla/util/outputter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2023-07-31 13:40:07.000000 scrilla-1.6.0/src/scrilla/version.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-31 13:40:43.683401 scrilla-1.6.0/src/scrilla.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7173 2023-07-31 13:40:43.000000 scrilla-1.6.0/src/scrilla.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3393 2023-07-31 13:40:43.000000 scrilla-1.6.0/src/scrilla.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-31 13:40:43.000000 scrilla-1.6.0/src/scrilla.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       93 2023-07-31 13:40:43.000000 scrilla-1.6.0/src/scrilla.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      197 2023-07-31 13:40:43.000000 scrilla-1.6.0/src/scrilla.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-07-31 13:40:43.000000 scrilla-1.6.0/src/scrilla.egg-info/top_level.txt
```

### Comparing `scrilla-1.5.7/LICENSE` & `scrilla-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/PKG-INFO` & `scrilla-1.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrilla
-Version: 1.5.7
+Version: 1.6.0
 Summary: a financial optimization program
 Author: Grant Moore
 Author-email: chinchalinchin@gmail.com
 License: GNU GPL v3
 Project-URL: Documentation, https://chinchalinchin.github.io/scrilla/
 Project-URL: Source, https://github.com/chinchalinchin/scrilla
 Keywords: finance,statistics,stock market,equities,cryptocurrencies,optimization
@@ -93,15 +93,15 @@
 
 ```
 pip install scrilla-<major>.<minor>.<micro>-py3-none-any.whl
 ```
 
 ## Configuration
 
-In order to use this application, you will need to register for API keys with [AlphaVantage](https://www.alphavantage.co), [IEX](https://iexcloud.io/) and [Quandl](https://www.quandl.com/). The program will need to be made aware of these keys somehow. The best option is storing these credentials in environment variables. You can add the following lines to your <i>.bashrc</i> profile or corresponding configuration file for whatever shell you are using,
+In order to use this application, you will need to register for API keys with [AlphaVantage](https://www.alphavantage.co), [IEX](https://iexcloud.io/) and [Quandl/Nasdaq](https://www.quandl.com/). The program will need to be made aware of these keys somehow. The best option is storing these credentials in environment variables. You can add the following lines to your <i>.bashrc</i> profile or corresponding configuration file for whatever shell you are using,
 
 ```shell
 export ALPHA_VANTAGE_KEY=<key goes here>
 export QUANDL_KEY=<key goes here>
 export IEX_KEY=<key goes here>
 ```
 
@@ -113,14 +113,16 @@
 
 where `<key>` is one of the values: **ALPHA_VANTAGE_KEY**, **QUANDL_KEY** or **IEX_KEY**. `<value>` is the corresponding key itself given to you after registration. Obviously, `<value>` is case-sensitive
 
 Keep in mind if using this method to store the API keys, the keys will be stored unencrypted in the local installation's <i>/data/common/</i> directory. The recommended method is storing the credentials in the environment. 
 
 If no API keys are found through either of these methods, the application will raise an exception.
 
+**NOTE**: The **Quandl**/**Nasdaq** key is technically no required for the majority of the application to function, as interest rates are now retrieved directly from the **US Treasury** RSS feed. However, it is still recommended that you register for an API key, as **Quandl**/**Nasdaq** is still the only source of economic statistics, like GDP or inflation rates. 
+
 ### Environment File
 
 A sample environment file has been included in _/env/.sample.env_. To configure the application environment, copy this file into a new environment, adjust the values and load it into your session,
 
 ```shell
 cp ./env/.sample.env ./env/.env
 # adjust .env values
```

### Comparing `scrilla-1.5.7/README.md` & `scrilla-1.6.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 ```
 pip install scrilla-<major>.<minor>.<micro>-py3-none-any.whl
 ```
 
 ## Configuration
 
-In order to use this application, you will need to register for API keys with [AlphaVantage](https://www.alphavantage.co), [IEX](https://iexcloud.io/) and [Quandl](https://www.quandl.com/). The program will need to be made aware of these keys somehow. The best option is storing these credentials in environment variables. You can add the following lines to your <i>.bashrc</i> profile or corresponding configuration file for whatever shell you are using,
+In order to use this application, you will need to register for API keys with [AlphaVantage](https://www.alphavantage.co), [IEX](https://iexcloud.io/) and [Quandl/Nasdaq](https://www.quandl.com/). The program will need to be made aware of these keys somehow. The best option is storing these credentials in environment variables. You can add the following lines to your <i>.bashrc</i> profile or corresponding configuration file for whatever shell you are using,
 
 ```shell
 export ALPHA_VANTAGE_KEY=<key goes here>
 export QUANDL_KEY=<key goes here>
 export IEX_KEY=<key goes here>
 ```
 
@@ -97,14 +97,16 @@
 
 where `<key>` is one of the values: **ALPHA_VANTAGE_KEY**, **QUANDL_KEY** or **IEX_KEY**. `<value>` is the corresponding key itself given to you after registration. Obviously, `<value>` is case-sensitive
 
 Keep in mind if using this method to store the API keys, the keys will be stored unencrypted in the local installation's <i>/data/common/</i> directory. The recommended method is storing the credentials in the environment. 
 
 If no API keys are found through either of these methods, the application will raise an exception.
 
+**NOTE**: The **Quandl**/**Nasdaq** key is technically no required for the majority of the application to function, as interest rates are now retrieved directly from the **US Treasury** RSS feed. However, it is still recommended that you register for an API key, as **Quandl**/**Nasdaq** is still the only source of economic statistics, like GDP or inflation rates. 
+
 ### Environment File
 
 A sample environment file has been included in _/env/.sample.env_. To configure the application environment, copy this file into a new environment, adjust the values and load it into your session,
 
 ```shell
 cp ./env/.sample.env ./env/.env
 # adjust .env values
```

### Comparing `scrilla-1.5.7/setup.cfg` & `scrilla-1.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/__init__.py` & `scrilla-1.6.0/src/scrilla/__init__.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/analysis/__init__.py` & `scrilla-1.6.0/src/scrilla/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/analysis/estimators.py` & `scrilla-1.6.0/src/scrilla/analysis/estimators.py`

 * *Files 5% similar despite different names*

```diff
@@ -234,14 +234,15 @@
 
     for i in x:
         xbar += i/n
     return xbar
 
 
 def recursive_rolling_mean(xbar_previous, new_obs, lost_obs, n=settings.DEFAULT_ANALYSIS_PERIOD):
+    # this should be done in terms of the sample arrays, not the observations themselves, i think.
     xbar_next = xbar_previous + (new_obs - lost_obs)/n
     return xbar_next
 
 
 def sample_variance(x: List[float]):
     r"""
     Returns the sample variance from a sample of data \\(\{x_1 , x_2, ... , x_n \}\\),
@@ -252,26 +253,33 @@
     ----------
     1. **x**: ``list``
         List containing a sample of numerical data.
 
     Raises 
     ------
     1. `scrilla.errors.SampleSizeError`
+
+    .. notes::
+        * This a naive two-pass implementation of sample variance. The function does not shift data around the mean, resulting in skewed calculations if the variance is numerically small and the sample is large; if you are concerned about the accuracy of your variance calculation in these instances, a better method is to use `scrilla.analysis.estimators.recursive_sum_of_squares` and then compute the variance by dividing by _(n-1)_, where _n_ is the number of samples.
     """
     # TODO: this is a 'naive' estimation of variance: https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance
 
     mu, sigma, n = sample_mean(x=x), 0, len(x)
 
     if not all(this_x is not None and isinstance(this_x, (float, int)) for this_x in x):
         raise ValueError(
             'Sample contains null values')
 
-    if n in [0, 1]:
+    if n == 0:
         raise errors.SampleSizeError(
-            'Sample variance cannot be computed for a sample size less than or equal to 1.')
+            'Sample variance cannot be computed for a sample size of 0.')
+
+    if n == 1:
+        # no variance for a sample of 1.
+        return 0
 
     for i in x:
         sigma += ((i-mu)**2)/(n-1)
     return sigma
 
 
 def recursive_rolling_variance(var_previous, xbar_previous, new_obs, lost_obs, n=settings.DEFAULT_ANALYSIS_PERIOD):
@@ -279,14 +287,33 @@
     xbar_new = recursive_rolling_mean(xbar_previous=xbar_previous, new_obs=new_obs,
                                       lost_obs=lost_obs, n=n)
     var_new = var_previous + \
         (n/(n-1))*((new_obs**2 - lost_obs**2)/n + (xbar_previous**2-xbar_new**2))
     return var_new
 
 
+def recursive_sum_of_squares(x: List[float], checked: bool = False):
+    n = len(x)
+
+    if not checked:
+        if not all(this_x is not None and isinstance(this_x, (float, int)) for this_x in x):
+            raise ValueError(
+                'Sample contains null values')
+
+        if n == 0:
+            raise errors.SampleSizeError(
+                'Sample variance cannot be computed for a sample size of 0.')
+
+    if n == 1:
+        return 0
+
+    term_variance = (n*x[-1] - sum(x))**2/(n*(n-1))
+    return recursive_sum_of_squares(x[:-1], True) + term_variance
+
+
 def sample_covariance(x: list, y: list):
     """
     Parameters
     ----------
     1. **x**: ``list``
         The *x* sample of paired data (*x*, *y*). Must preserve order with **y**.
     2. **y**: ``list``
```

### Comparing `scrilla-1.5.7/src/scrilla/analysis/integration.py` & `scrilla-1.6.0/src/scrilla/analysis/integration.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/analysis/markets.py` & `scrilla-1.6.0/src/scrilla/analysis/markets.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/analysis/models/geometric/probability.py` & `scrilla-1.6.0/src/scrilla/analysis/models/geometric/probability.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/analysis/models/geometric/statistics.py` & `scrilla-1.6.0/src/scrilla/analysis/models/geometric/statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -813,14 +813,16 @@
     last_price = prices[last_date][keys.keys['PRICES']['CLOSE']]
     first_price = prices[first_date][keys.keys['PRICES']['CLOSE']]
     mean_return = log(float(last_price)/float(first_price)) / \
         (trading_period*sample)
 
     # VOLATILITY CALCULATION
     # NOTE / TODO : this is a 'naive' variance algorithm: https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance
+    # although technically, this is only one pass, since the mean telescopes and doesn't require a full traversal of the
+    # the sample. I should see how this implementation compares to a Young and Cramer Updating algorithm implementation.
     today, variance, tomorrows_price, tomorrows_date = False, 0, 0, None
     # adjust the random variable being measured so expectation is easier to calculate.
     mean_mod_return = mean_return*sqrt(trading_period)
     logger.debug(
         f'Calculating mean annual volatility over last {sample} days for {ticker}', '_calculate_moment_risk_return')
 
     for this_date in prices:
```

### Comparing `scrilla-1.5.7/src/scrilla/analysis/objects/cashflow.py` & `scrilla-1.6.0/src/scrilla/analysis/objects/cashflow.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/analysis/objects/portfolio.py` & `scrilla-1.6.0/src/scrilla/analysis/objects/portfolio.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/analysis/optimizer.py` & `scrilla-1.6.0/src/scrilla/analysis/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,14 +313,14 @@
     maximum_allocation = maximize_portfolio_return(portfolio=portfolio)
 
     minimum_return = portfolio.return_function(minimum_allocation)
     maximum_return = portfolio.return_function(maximum_allocation)
     return_width = (maximum_return - minimum_return)/steps
 
     frontier = []
-    for i in range(steps+1):
+    for i in range(steps):
         target_return = minimum_return + return_width*i
         allocation = optimize_portfolio_variance(
             portfolio=portfolio, target_return=target_return)
         frontier.append(allocation)
 
     return frontier
```

### Comparing `scrilla-1.5.7/src/scrilla/analysis/plotter.py` & `scrilla-1.6.0/src/scrilla/analysis/plotter.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/cache.py` & `scrilla-1.6.0/src/scrilla/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,26 +72,32 @@
         if mode == 'sqlite':
             con = sqlite3.connect(settings.CACHE_SQLITE_FILE)
             executor = con.cursor()
             if formatter is not None:
                 if isinstance(formatter, list):
                     response = executor.executemany(
                         query, formatter).fetchall()
-                else:
-                    response = executor.execute(query, formatter).fetchall()
-            else:
-                response = executor.execute(query).fetchall()
+                    con.commit(), con.close()
+                    return response
+                
+                response = executor.execute(query, formatter)
+                response = response.fetchall()
+                con.commit(), con.close()
+                return response
+
+            response = executor.execute(query).fetchall()
             con.commit(), con.close()
+            return response
+
         elif mode == 'dynamodb':
             response = aws.dynamo_statement(query, formatter)
-        else:
-            raise errors.ConfigurationError(
-                'CACHE_MODE has not been set in "settings.py"')
-        return response
+            return response
 
+        raise errors.ConfigurationError(
+            'CACHE_MODE has not been set in "settings.py"')
 
 class PriceCache(metaclass=Singleton):
     """
     `scrilla.cache.PriceCache` statically accesses *SQLite* functionality from `scrilla.cache.Cache`. It extends basic functionality to cache interest rate data in a table with columns ``(ticker, date, open, close)``. `scrilla.cache.PriceCache` has a `scrilla.cache.Singleton` for its `metaclass`, meaning `PriceCache` is a singleton; it can only be created once; any subsequent instantiations will return the same instance of `PriceCache`. This is done so that all instances of `PriceCache` share the same `self.internal_cache`, allowing frequently accessed data to be stored in memory.
 
     Attributes
     ----------
@@ -238,27 +244,35 @@
             if prices is not None:
                 logger.debug(f'{ticker} prices found in memory',
                              'ProfileCachce.filter')
                 return prices
 
         logger.debug(
             f'Querying {self.mode} cache \n\t{self._query()}\n\t\t with :ticker={ticker}, :start_date={start_date}, :end_date={end_date}', 'ProfileCache.filter')
-        formatter = {'ticker': ticker,
-                     'start_date': start_date, 'end_date': end_date}
+
+        if isinstance(start_date, datetime.date):
+            start_date = dater.to_string(start_date)
+
+        if isinstance(end_date, datetime.date):
+            end_date = dater.to_string(end_date)
+
+        formatter = {'ticker': ticker, 'end_date': end_date, 'start_date': start_date}
+
         results = Cache.execute(
             query=self._query(),
             formatter=formatter,
             mode=self.mode)
 
         if len(results) > 0:
             logger.debug(
                 f'Found {ticker} prices in the cache', 'ProfileCache.filter')
             prices = self.to_dict(results)
             self._update_internal_cache(ticker, prices)
             return prices
+
         logger.debug(
             f'No results found for {ticker} prices in the cache', 'ProfileCache.filter')
         return None
 
 
 class InterestCache(metaclass=Singleton):
     """
@@ -335,14 +349,15 @@
         Parameters
         ----------
         1. **mode**: ``str``
             Determines the data source that acts as the cache. Defaults to `scrilla.settings.CACHE_MODE`. Can be set to either `sqlite` or `dynamodb`. 
         """
         if not self.inited:
             self.uuid = uuid.uuid4()
+            self._init_internal_cache()
             self.inited = True
 
         self.mode = mode
 
         if not files.get_memory_json()['cache'][self.mode]['interest']:
             self._table()
 
@@ -351,86 +366,137 @@
             Cache.execute(query=self.sqlite_create_table_transaction,
                           mode=self.mode)
         elif self.mode == 'dynamodb':
             self.dynamodb_table_configuration = aws.dynamo_table_conf(
                 self.dynamodb_table_configuration)
             Cache.provision(self.dynamodb_table_configuration, self.mode)
 
+    def _init_internal_cache(self):
+        for maturity in keys.keys['YIELD_CURVE']:
+            self.internal_cache[maturity] = {}
+
     def _insert(self):
         if self.mode == 'sqlite':
             return self.sqlite_insert_row_transaction
         elif self.mode == 'dynamodb':
             return self.dynamodb_insert_transaction
 
     def _query(self):
         if self.mode == 'sqlite':
             return self.sqlite_interest_query
         elif self.mode == 'dynamodb':
             return self.dynamodb_query
 
     def _save_internal_cache(self, rates):
-        self.internal_cache.update(rates)
+        """
+        Stores interest rate data in an internal cache, to minimize direct queries to the cache.
+
+        Parameters
+        ----------
+        1. **rates**: ``dict``
+            Dictionary containing interest rate data that needs persisted in-memory.
+
+        .. notes::
+            - The internal cache data structure is as follows,
+                ```json
+                {
+                    "maturity": {
+                        "date": "value"
+                        "date": "value"
+                    },
+
+                }
+                ```
+        """
+        for date in rates:
+            for index, maturity in enumerate(keys.keys['YIELD_CURVE']):
+                self.internal_cache[maturity][date] = rates[date][index]
 
     def _update_internal_cache(self, values, maturity):
-        for date in values.keys():
-            if self.internal_cache.get(date) is None:
-                self.internal_cache[date] = [
-                    None for _ in keys.keys['YIELD_CURVE']]
-            self.internal_cache[date][keys.keys['YIELD_CURVE'].index(
-                maturity)] = values[date]
+        self.internal_cache[maturity].update(values)
 
     def _retrieve_from_internal_cache(self, maturity, start_date, end_date):
-        dates = list(self.internal_cache.keys())
-        start_string = dater.to_string(start_date)
-        end_string = dater.to_string(end_date)
+        dates = list(self.internal_cache[maturity].keys())
+        start_string, end_string = dater.to_string(
+            start_date), dater.to_string(end_date)
+
         if start_string in dates and end_string in dates:
             start_index = dates.index(start_string)
             end_index = dates.index(end_string)
+
             if start_index > end_index:
                 # NOTE: DynamoDB respones are not necessarily ordered
                 # `to_dict` will take care of ordering
                 start_index, end_index = end_index, start_index
+
             rates = dict(itertools.islice(
-                self.internal_cache.items(), start_index, end_index+1))
-            rates = {key: rates[key][keys.keys['YIELD_CURVE'].index(
-                maturity)] for key in rates}
-            logger.debug('Found interest in memory',
-                         'InterestCache._retrieve_from_internal_cache')
-            return rates
+                self.internal_cache[maturity].items(), start_index, end_index+1))
+
+            if dater.business_days_between(start_date, end_date) == len(rates):
+                logger.debug('Found interest in memory',
+                             'InterestCache._retrieve_from_internal_cache')
+                return rates
+        return None
 
     def save_rows(self, rates):
-        # NOTE: at this point, rates should look like { 'date': [rates], 'date': [rates], ...}
+        """
+
+        .. notes::
+            - this is called with the response from `scrilla.services.StatManaget.get_interest_rates()`. At this point, the data should be formatted as folows,
+                ```json
+                {
+                    "date" : [ "value", "value", ... , "value" ],
+                    "date" : [ "value", "value", ... , "value" ]
+                }
+                ```
+        """
+
         self._save_internal_cache(rates)
         logger.verbose(
             'Attempting to insert interest rates into cache', 'InterestCache.save_rows')
         Cache.execute(
             query=self._insert(),
             formatter=self._to_params(rates)
         )
 
     def filter(self, maturity, start_date, end_date):
+        """
+
+        .. notes::
+            - `scrilla.cache.InterestCache.filter()` is called in `scrilla.services.get_daily_interest_history()` _before_ the API response from the Treasury is saved, i.e. before `scrilla.cache.InterestCache.save_rows()` and thus `scrilla.cache.InterestCache._save_internal_cache()` are called. If the application has just been installed and the cache is empty, then nothing unusual happens. If the application has just been installed and the cache is not empty (perhaps the application was re-installed or data has been inserted manually into the cache), then calling `filter` will return results and those results will populate the internal_cache with a `scrilla.InterestCache._update_internal_cache()` call, meaning in this case the internal cache is hydrated by the `update` method instead of the `save` method. In other words, the internal cache has two different entrypoints and care must be taken so both are taken into account when initializing the internal cache.
+
+        """
         rates = self._retrieve_from_internal_cache(
             maturity, start_date, end_date)
         if rates is not None:
             logger.debug(f'{maturity} interet found in memory',
                          'InterestCache.filter')
             return rates
 
         logger.debug(
             f'Querying {self.mode} cache \n\t{self._query()}\n\t\t with :maturity={maturity}, :start_date={start_date}, :end_date={end_date}',
             'InterestCache.filter')
+
+        if isinstance(start_date, datetime.date):
+            start_date = dater.to_string(start_date)
+
+        if isinstance(end_date, datetime.date):
+            end_date = dater.to_string(end_date)
+            
         formatter = {'maturity': maturity,
                      'start_date': start_date, 'end_date': end_date}
         results = Cache.execute(
             query=self._query(), formatter=formatter, mode=self.mode)
+        # NOTE: [ [ 'date', 'value ] ] at this point
 
         if len(results) > 0:
             logger.debug(
                 f'Found {maturity} yield on in the cache', 'InterestCache.filter')
             rates = self.to_dict(results)
+            # NOTE: { 'date': 'value' } at this point
             self._update_internal_cache(rates, maturity)
             return rates
 
         logger.debug(
             f'No results found for {maturity} yield in cache', 'InterestCache.filter')
         return None
 
@@ -535,17 +601,17 @@
         self.internal_cache[correl_id] = {'correlation': correlation}
         self.internal_cache[permuted_id] = {'correlation': correlation}
         pass
 
     def _retrieve_from_internal_cache(self, params, permuted_params):
         first_id = self.generate_id(params)
         second_id = self.generate_id(permuted_params)
-        if first_id in list(self.internal_cache.keys()):
+        if first_id in list(self.internal_cache):
             return self.internal_cache[first_id]
-        if second_id in list(self.internal_cache.keys()):
+        if second_id in list(self.internal_cache):
             return self.internal_cache[second_id]
         return None
 
     def save_row(self, ticker_1: str, ticker_2: str, start_date: datetime.date, end_date: datetime.date, correlation: float, weekends: bool, method: str = settings.ESTIMATION_METHOD):
         """
         Uses `self.insert_row_transaction` to save the passed-in information to the SQLite cache.
 
@@ -785,20 +851,20 @@
 
     def _identity(self):
         if self.mode == 'sqlite':
             return self.sqlite_identity_query
         elif self.mode == 'dynamodb':
             return self.dynamodb_identity_query
 
-    def _update_internal_cache(self, profile, keys):
-        key = self._create_cache_key(keys)
+    def _update_internal_cache(self, profile, profile_keys):
+        key = self._create_cache_key(profile_keys)
         self.internal_cache[key] = profile
 
-    def _retrieve_from_internal_cache(self, keys):
-        key = self._create_cache_key(keys)
+    def _retrieve_from_internal_cache(self, profile_keys):
+        key = self._create_cache_key(profile_keys)
         if key in list(self.internal_cache):
             return self.internal_cache[key]
         return None
 
     def save_or_update_row(self, ticker: str, start_date: datetime.date, end_date: datetime.date, annual_return: Union[float, None] = None, annual_volatility: Union[float, None] = None, sharpe_ratio: Union[float, None] = None, asset_beta: Union[float, None] = None, equity_cost: Union[float, None] = None, weekends: int = 0, method: str = settings.ESTIMATION_METHOD):
         filters = {'ticker': ticker, 'start_date': start_date,
                    'end_date': end_date, 'method': method, 'weekends': weekends}
```

### Comparing `scrilla-1.5.7/src/scrilla/cloud/aws.py` & `scrilla-1.6.0/src/scrilla/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/calculator-outline.svg` & `scrilla-1.6.0/src/scrilla/data/assets/calculator-outline.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/calendar-number-outline.svg` & `scrilla-1.6.0/src/scrilla/data/assets/calendar-number-outline.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/calendar-number-sharp.svg` & `scrilla-1.6.0/src/scrilla/data/assets/calendar-number-sharp.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/calendar-outline.svg` & `scrilla-1.6.0/src/scrilla/data/assets/calendar-outline.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/calendar-sharp.svg` & `scrilla-1.6.0/src/scrilla/data/assets/calendar-sharp.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/cash-outline.svg` & `scrilla-1.6.0/src/scrilla/data/assets/cash-outline.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/cash-sharp.svg` & `scrilla-1.6.0/src/scrilla/data/assets/cash-sharp.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/help-circle-outline.svg` & `scrilla-1.6.0/src/scrilla/data/assets/help-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/help-circle-sharp.svg` & `scrilla-1.6.0/src/scrilla/data/assets/help-circle-sharp.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/information-circle-outline.svg` & `scrilla-1.6.0/src/scrilla/data/assets/information-circle-outline.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/logo-github.svg` & `scrilla-1.6.0/src/scrilla/data/assets/logo-github.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/logo-python.svg` & `scrilla-1.6.0/src/scrilla/data/assets/logo-python.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/okay-sharp.svg` & `scrilla-1.6.0/src/scrilla/data/assets/okay-sharp.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/okay.svg` & `scrilla-1.6.0/src/scrilla/data/assets/okay.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/trash-outline.svg` & `scrilla-1.6.0/src/scrilla/data/assets/trash-outline.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/data/assets/trash-sharp.svg` & `scrilla-1.6.0/src/scrilla/data/assets/trash-sharp.svg`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/files.py` & `scrilla-1.6.0/src/scrilla/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,16 @@
                 'profile': False
             }
         }
     }
 
 
 def save_memory_json(persist: Union[dict, None] = None):
-    if persist is None:
-        persist = get_memory_json()
+    if persist is None or not isinstance(persist, dict):
+        return
     save_file(persist, settings.MEMORY_FILE)
 
 
 def get_memory_json():
     if os.path.isfile(settings.MEMORY_FILE):
         memory_json = load_file(settings.MEMORY_FILE)
         return memory_json
@@ -89,15 +89,15 @@
                 json.dump(file_to_save, outfile)
             elif ext == "csv":
                 # TODO: assume input is dict since ll functions in library return dict.
                 writer = csv.DictWriter(outfile, file_to_save.keys())
                 writer.writeheader()
             # TODO: implement other file saving extensions.
         return True
-    except Exception as e:
+    except OSError as e:
         logger.error(e, 'save_file')
         return False
 
 
 def set_credentials(value: str, which_key: str) -> bool:
     file_name = os.path.join(
         settings.COMMON_DIR, f'{which_key}.{settings.FILE_EXT}')
@@ -434,15 +434,15 @@
         filelist = list(os.listdir(directory))
         for f in filelist:
             filename = os.path.basename(f)
             if retain and filename == constants.constants['KEEP_FILE']:
                 continue
             os.remove(os.path.join(directory, f))
         return True
-    except Exception as e:
+    except OSError as e:
         logger.error(e, 'clear_directory')
         return False
 
 
 def is_non_zero_file(fpath: str) -> bool:
     return os.path.isfile(fpath) and os.path.getsize(fpath) > 0
 
@@ -456,13 +456,14 @@
 
     save_memory_json(memory)
 
     if mode == 'sqlite':
         try:
             os.remove(settings.CACHE_SQLITE_FILE)
             return True
-        except OSError:
+        except OSError as e:
+            logger.error(e, 'clear_cache')
             return False
     elif mode == 'dynamodb':
         return aws.dynamo_drop_table(tables)
 
     raise errors.ConfigurationError('`CACHE_MODE` not set!')
```

### Comparing `scrilla-1.5.7/src/scrilla/gui/formats.py` & `scrilla-1.6.0/src/scrilla/gui/formats.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/gui/main.py` & `scrilla-1.6.0/src/scrilla/gui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
     app = QtWidgets.QApplication([])
 
     widget = menu.MenuWidget()
 
     with open(settings.GUI_STYLESHEET_FILE, "r") as f:
         _style = formats.format_stylesheet(f.read())
+        print(_style)
         app.setStyleSheet(_style)
 
     logger.verbose(f'Initializing GUI with style sheet: {_style}', 'do_gui')
 
     if not dimensions['full_screen']:
         widget.resize(dimensions['width'], dimensions['height'])
         center = QtGui.QScreen.availableGeometry(
```

### Comparing `scrilla-1.5.7/src/scrilla/gui/styles/app.qss` & `scrilla-1.6.0/src/scrilla/gui/styles/app.qss`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/gui/styles/icons.json` & `scrilla-1.6.0/src/scrilla/gui/styles/icons.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9629629629629629%*

 * *Differences: {"'$okay'": "{'unpressed': 'okay.svg', delete: ['unpresssed']}"}*

```diff
@@ -21,15 +21,15 @@
     },
     "$hide": {
         "pressed": "arrow-back-circle-sharp.svg",
         "unpressed": "arrow-back-circle-outline.svg"
     },
     "$okay": {
         "pressed": "okay-sharp.svg",
-        "unpresssed": "okay.svg"
+        "unpressed": "okay.svg"
     },
     "$package": {
         "pressed": "logo-python.svg",
         "unpressed": "logo-python.svg"
     },
     "$source": {
         "pressed": "logo-github.svg",
```

### Comparing `scrilla-1.5.7/src/scrilla/gui/styles/themes.json` & `scrilla-1.6.0/src/scrilla/gui/styles/themes.json`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/gui/templates/splash.html` & `scrilla-1.6.0/src/scrilla/gui/templates/splash.html`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/gui/utilities.py` & `scrilla-1.6.0/src/scrilla/gui/utilities.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/gui/widgets/components.py` & `scrilla-1.6.0/src/scrilla/gui/widgets/components.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,19 +42,48 @@
 SYMBOLS_SINGLE = "single"
 """Constant passed into `scrilla.gui.widgets.components.ArgumentWidget` to initialize an input control allowing user to input  single ticker symbol"""
 SYMBOLS_NONE = "none"
 """Constant passed into `scrilla.gui.widgets.components.ArgumentWidget` to initialize an input control without ticker symbols"""
 
 
 class SkeletonWidget(QtWidgets.QWidget):
+    """
+    Base classfor other more complex widgets to inherit. An instance of `scrilla.gui.widgets.SkeletonWidget` generates an empty configuration attribute, i.e. a dictionary of booleans all set to their appropriate values for the given type of Widget and keyed to the available types of arguments for each function in `scrilla`, e.g., each instance of `scrilla.gui.widgets.SkeletonWidget` has the following attribute by default,
+
+    ```python
+    self.controls = {
+        'start_date': True,
+        'end_date': True,
+        'target': False,
+        # ...
+    }
+    ```
+
+    Where the value of the boolean is determined by the type of widget being constructed. The keys and values of the `self.controls` dictionary are generated from `scrilla.static.definitions.FUNC_DICT` and `scrilla.static.definitions.ARG_DICT`, filtering on the `cli_only` configuration option. In other words, the 'control skeleton' is generated by passing in a type of function and checking which types of arguments are restricted to the command line interface only.
+
+    Constructor
+    -----------
+    1. **function**: ``str``
+        Name of the function whose control skeleton is being constructed. Function names are accessible through the `scrilla.static.definitions.FUNC_DICT` dictionary keys. 
+    2. **parent**: ``PySide6.QtWidgets.QWidget``
+        Parent of the widget.
+    """
     def __init__(self, function: str, parent: QtWidgets.QWidget):
         super(SkeletonWidget, self).__init__(parent)
         self._configure_control_skeleton(function)
 
     def _configure_control_skeleton(self, function: str):
+        """
+        Generates the control skeleton and stores it in `self.controls`.
+
+        Parameters
+        ----------
+        1. **function**: ``str``
+            Name of the function whose control is being constructed.
+        """
         self.controls = factories.generate_control_skeleton()
 
         for arg in definitions.FUNC_DICT[function]['args']:
             if not definitions.ARG_DICT[arg]['cli_only']:
                 self.controls[arg] = True
 
 
@@ -146,49 +175,95 @@
             self.required_pane.setObjectName(self.layer)
             self.symbol_widget = factories.argument_widget_factory(
                 component='symbol', title="Symbol: ", optional=False)
         else:
             self.symbol_widget = None
 
         self.group_definitions = None
+
+        # TODO: yes, yes, very clever...i think. still needs re-factored for clarity.
+        # what exactly is going on here?
+
+
         for control in self.controls:
             if self.controls[control]:
-                if self.controls[control]:
-                    if definitions.ARG_DICT[control]["widget_type"] != "group":
-                        self.control_widgets[control] = factories.argument_widget_factory(definitions.ARG_DICT[control]['widget_type'],
-                                                                                          f'{definitions.ARG_DICT[control]["name"]} :',
-                                                                                          optional=True)
-                    else:
-                        if self.group_definitions is None:
-                            self.group_definitions = {}
-                        self.group_definitions[definitions.ARG_DICT[control]
-                                               ['name']] = definitions.ARG_DICT[control]
+                if definitions.ARG_DICT[control]["widget_type"] != "group":
+                    self.control_widgets[control] = factories.argument_widget_factory(definitions.ARG_DICT[control]['widget_type'],
+                                                                                        f'{definitions.ARG_DICT[control]["name"]} :',
+                                                                                        optional=True)
+                else:
+                    if self.group_definitions is None:
+                        self.group_definitions = {}
+                    self.group_definitions[control] = definitions.ARG_DICT[control]
+                                            
+                    # NOTE: at this point, the following should hold:
+                    #   ```python
+                    #   assert isinstance(self.group_definitions, dict[str, any]) 
+                    #   assert isinstance(defintions.ARG_DICT[control]['name'], str)
+                    #   assert isinstance(definitions.ARG_DICT[control], dict[str, any])
+                    #   ```
+                    #
+                    # i.e., `self.group_defintions` should look like,
+                    #   ```python`
+                    #    self.group_defintions = {
+                    #       'moments' : {
+                    #           'name': 'Moment Matching'
+                    #           'values': ['-moments', '--moments', ...],
+                    #           'description': '...',
+                    #           ...
+                    #       }
+                    #   }
+                    #   ```
+
             else:
                 self.control_widgets[control] = None
 
         self.optional_pane = factories.layout_factory(layout='vertical-box')
         self.optional_pane.setObjectName(self.layer)
         self.setLayout(QtWidgets.QVBoxLayout())
 
     def _generate_group_widgets(self):
+        """
+        
+        .. notes::
+            - `groups` is an intermediate dictionary used to group the definitions of each group into an array keyed to the group name, e.g.,
+                ```python
+                groups = {
+                    'Estimation Method': [
+                        {
+                            'name': 'Moment Matching',
+                            # ...
+                        },
+                        {
+                            'name': 'Percentile Matching`,
+                            # ...
+                        },
+                        # ...
+                    ]
+                }
+                ```
+        """
         if self.group_definitions is not None:
             self.group_control_widgets = {}
             groups = {}
-            for definition in self.group_definitions:
-                group_key = self.group_definitions[definition]['group']
+            for definition in self.group_definitions.values():
+
+                group_key = definition['group']
                 group_name = definitions.GROUP_DICT[group_key]
 
                 if group_name not in groups:
                     groups[group_name] = [definition]
                 else:
                     groups[group_name].append(definition)
 
-            for group_name, group in groups.items():
+            # str, dict from `scrilla.static.definitions.ARG_DICT`
+            for group_name, group_def in groups.items():
+                control_names = [ single_def['name'] for single_def in group_def ] 
                 self.group_control_widgets[group_name] = factories.group_widget_factory(
-                    group, group_name)
+                    control_names, group_name)
 
     def _arrange_widgets(self):
         """
         Arrange child widgets in their layouts and provides rendering hints. The `self.symbol_widget` is set into a ``PySide6.QtWidgets.QVBoxLayout`` named `self.required_pane`. The optional input widgets are set into a separate ``PySide6.QtWidgets.QVBoxLayout`` named `self.optional_pane`. `self.required_pane` and `self.optional_pane` are in turn set into a parent `PySide6.QtWidgets.QVBoxLayout``, along with `self.calculate_button` and `self.clear_button`. A strecth widget is inserted between the input widgets and the button widgets. 
 
         """
         factories.set_policy_on_widget_list([self.title, self.optional_title, self.optional_pane],
```

### Comparing `scrilla-1.5.7/src/scrilla/gui/widgets/functions.py` & `scrilla-1.6.0/src/scrilla/gui/widgets/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from typing import Union
 from PySide6 import QtGui, QtCore, QtWidgets
 
 
 from scrilla import settings, services
 from scrilla.static import keys
+from scrilla.static import formats as app_formats
 # TODO: conditional import based on ANALYSIS_MODE
 from scrilla.analysis import estimators, markets, optimizer, plotter
 from scrilla.analysis.models.geometric import statistics
 from scrilla.analysis.objects.portfolio import Portfolio
 from scrilla.analysis.objects.cashflow import Cashflow
 
 from scrilla.util import dater, outputter, helper
@@ -355,17 +356,17 @@
             matrix = statistics.correlation_matrix(tickers=symbols,
                                                    start_date=self.arg_widget.get_control_input(
                                                        'start_date'),
                                                    end_date=self.arg_widget.get_control_input('end_date'))
             for i in range(0, len(symbols)):
                 for j in range(i, len(symbols)):
                     item_upper = factories.atomic_widget_factory(
-                        component='table-item', title=helper.format_float_percent(matrix[i][j]))
+                        component='table-item', title=app_formats.format_float_percent(matrix[i][j]))
                     item_lower = factories.atomic_widget_factory(
-                        component='table-item', title=helper.format_float_percent(matrix[j][i]))
+                        component='table-item', title=app_formats.format_float_percent(matrix[j][i]))
                     self.table_widget.table.setItem(j, i, item_upper)
                     self.table_widget.table.setItem(i, j, item_lower)
         else:
             print('error handling goes here')
 
         self.table_widget.show_table()
         self.arg_widget.fire()
@@ -433,15 +434,15 @@
                 self.table_widget.init_table(rows=symbols, columns=[
                                              'Allocation', 'Shares'])
                 shares = this_portfolio.calculate_approximate_shares(
                     allocation, float(investment), prices)
 
             for i in range(len(symbols)):
                 item = factories.atomic_widget_factory(
-                    component='table-item', title=helper.format_float_percent(allocation[i]))
+                    component='table-item', title=app_formats.format_float_percent(allocation[i]))
                 self.table_widget.table.setItem(i, 0, item)
 
                 if investment is not None:
                     share_item = factories.atomic_widget_factory(
                         component='table-item', title=str(shares[i]))
                     self.table_widget.table.setItem(i, 1, share_item)
```

### Comparing `scrilla-1.5.7/src/scrilla/gui/widgets/menu.py` & `scrilla-1.6.0/src/scrilla/gui/widgets/menu.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,35 @@
 import sys
 
 from PySide6 import QtCore, QtWidgets, QtGui
 
 from scrilla import settings
 
 from scrilla.gui import utilities, definitions
-from scrilla.gui.widgets import factories
+from scrilla.gui.widgets import factories, functions
 
 # NOTE: widget_buttons and function_widgets must preserve order.
 
+def _to_class(name: str):
+    if name == 'correlation':
+        return functions.CorrelationWidget
+    if name == 'plot_return_dist':
+        return functions.DistributionWidget
+    if name == 'yield_curve':
+        return functions.YieldCurveWidget
+    if name == 'discount_dividend':
+        return functions.DiscountDividendWidget
+    if name == 'risk_profile':
+        return functions.RiskProfileWidget
+    if name == 'optimize_portfolio':
+        return functions.OptimizerWidget
+    if name == 'efficient_frontier':
+        return functions.EfficientFrontierWidget
+    if name == 'moving_averages':
+        return functions.MovingAverageWidget
 
 class MenuWidget(QtWidgets.QWidget):
     """
 
     .. notes::
         * Widget Hierarchy: 
 
@@ -41,15 +58,15 @@
         self._generate_menu_bar()
         self._generate_splash()
         self._arrange_menu_widgets()
         self._stage_menu_widgets()
 
     def _generate_menu_bar(self):
         self.menu_bar = factories.atomic_widget_factory(
-            component='menu-bar', title=None)
+            component='menu-bar')
         self.menus = []
 
         for j, menu in enumerate(definitions.MENUBAR_WIDGET):
             self.menus.append(self.menu_bar.addMenu(menu))
             for i, action in enumerate(definitions.MENUBAR_WIDGET[menu]):
                 q_action = QtGui.QAction(action['name'], self)
                 q_action.setShortcut(action['shortcut'])
@@ -107,16 +124,16 @@
             component='hide-button', title=None)
 
         self.widget_buttons = [factories.atomic_widget_factory(
             component='button', title=function['name']) for function in definitions.FUNC_WIDGETS.values()]
         self.exit_button = factories.atomic_widget_factory(
             component='button', title="Exit")
 
-        self.function_widgets = [function['class'](
-            'great-grand-child', self) for function in definitions.FUNC_WIDGETS.values()]
+        self.function_widgets = [_to_class(function)(
+            'great-grand-child', self) for function in definitions.FUNC_WIDGETS]
 
         self.display_pane = factories.layout_factory(layout='vertical-box')
         self.display_pane.setObjectName('grand-child')
 
         self.container_pane = factories.layout_factory(layout='horizontal-box')
         self.container_pane.setObjectName('child')
```

### Comparing `scrilla-1.5.7/src/scrilla/main.py` & `scrilla-1.6.0/src/scrilla/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,23 @@
 The arguments are parsed in such a way that arguments which are not supplied are set to None. All application functions are set up to accept None as a value for their optional arguments. This makes passing arguments to application functions easier as the `main.py` script doesn't have to worry about their values. In other words, `main.py` always passes all arguments to application functions, even if they aren't supplied through the command line; it just sets the ones which aren't supplied to None.
 """
 
 import time
 from datetime import date
 from typing import Callable, Dict, List, Union
 
-from scrilla.settings import LOG_LEVEL, ESTIMATION_METHOD
+from scrilla import settings, files, cache
 from scrilla.static import definitions
 from scrilla.util.errors import InputValidationError
-from scrilla.files import init_static_data
-from scrilla.cache import init_cache
-from scrilla.static.formats import format_args
+from scrilla.static import formats
 from scrilla.util.outputter import Logger
 
 # TODO: conditional imports based on value of ANALYSIS_MODE
 
-logger = Logger('main', LOG_LEVEL)
+logger = Logger('main', settings.LOG_LEVEL)
 
 
 def validate_function_usage(selection: str, args: List[str], wrapper_function: Callable, required_length: int = 1, exact: bool = False) -> None:
     """
     Parameters
     ----------
     1. **selection** : ``str``
@@ -97,76 +95,72 @@
     return args['json'] and not args['suppress_output']
 
 
 def do_program(cli_args: List[str]) -> None:
     """
     Parses command line arguments and passes the formatted arguments to appropriate function from the library.
     """
-    init_static_data()
-    init_cache()
+    files.init_static_data()
+    cache.init_cache()
 
-    args = format_args(cli_args, ESTIMATION_METHOD)
+    args = formats.format_args(cli_args, settings.ESTIMATION_METHOD)
     exact, selected_function = False, None
 
     # START CLI FUNCTION DEFINITIONS
 
     # NO ARGUMENT FUNCTIONS
     # FUNCTION: Help Message
     if args['function_arg'] in definitions.FUNC_DICT["help"]['values']:
         def cli_help():
             from scrilla.util.outputter import help_msg
-            help_msg()
+            # NOTE: in this case, the arguments are function names, not tickers.
+            #       it may be behoove the application to rejigger the argparse
+            #       just so names are consistent with what is represented.
+            help_msg(function_filter=args['tickers'])
         selected_function, required_length = cli_help, 0
 
     # FUNCTION: Clear Cache
     elif args['function_arg'] in definitions.FUNC_DICT["clear_cache"]['values']:
         def cli_clear_cache():
-            from scrilla.files import clear_directory
-            from scrilla.settings import CACHE_DIR
-            logger.info(f'Clearing {CACHE_DIR}', 'do_program')
-            clear_directory(directory=CACHE_DIR, retain=True)
+            logger.info(f'Clearing {settings.CACHE_DIR}', 'do_program')
+            files.clear_cache()
         selected_function, required_length = cli_clear_cache, 0
 
     # FUNCTION: Clear Static
     elif args['function_arg'] in definitions.FUNC_DICT["clear_static"]['values']:
         def cli_clear_static():
-            from scrilla.files import clear_directory
-            from scrilla.settings import STATIC_DIR
-            logger.info(f'Clearing {STATIC_DIR}', 'do_program')
-            clear_directory(directory=STATIC_DIR, retain=True)
+            logger.info(f'Clearing {settings.STATIC_DIR}', 'do_program')
+            files.clear_directory(directory=settings.STATIC_DIR, retain=True)
         selected_function, required_length = cli_clear_static, 0
 
     # FUNCTION: Clear Common
     elif args['function_arg'] in definitions.FUNC_DICT["clear_common"]['values']:
         def cli_clear_common():
-            from scrilla.files import clear_directory
-            from scrilla.settings import COMMON_DIR
-            logger.info(f'Clearing {COMMON_DIR}', 'do_program')
-            clear_directory(directory=COMMON_DIR, retain=True)
+            logger.info(f'Clearing {settings.COMMON_DIR}', 'do_program')
+            files.clear_directory(directory=settings.COMMON_DIR, retain=True)
         selected_function, required_length = cli_clear_common, 0
 
     # FUNCTION: Print Stock Watchlist
     elif args['function_arg'] in definitions.FUNC_DICT['list_watchlist']['values']:
         def cli_watchlist():
-            from scrilla.files import get_watchlist
             from scrilla.util.outputter import title_line, print_list
-            tickers = get_watchlist()
-            title_line("Stock Watchlist")
+            tickers = files.get_watchlist()
+            title_line("Watchlist")
             print_list(tickers)
         selected_function, required_length = cli_watchlist, 0
+
     # FUNCTION: Purge Data Directories
     elif args['function_arg'] in definitions.FUNC_DICT["purge"]['values']:
         def cli_purge():
-            from scrilla.files import clear_directory
-            from scrilla.settings import CACHE_DIR, STATIC_DIR, COMMON_DIR
+            from scrilla.files import clear_directory, clear_cache
             logger.info(
-                f'Clearing {STATIC_DIR}, {CACHE_DIR} and {COMMON_DIR}', 'do_program')
-            clear_directory(directory=STATIC_DIR, retain=True)
-            clear_directory(directory=CACHE_DIR, retain=True)
-            clear_directory(directory=COMMON_DIR, retain=True)
+                f'Clearing {settings.STATIC_DIR}, {settings.CACHE_DIR} and {settings.COMMON_DIR}', 'do_program')
+            files.clear_directory(directory=settings.STATIC_DIR, retain=True)
+            files.clear_directory(directory=settings.COMMON_DIR, retain=True)
+            files.clear_cache()
         selected_function, required_length = cli_purge, 0
 
     # FUNCTION: Display Version
     elif args['function_arg'] in definitions.FUNC_DICT["version"]['values']:
         def cli_version():
             from scrilla.settings import APP_DIR
             from os.path import join
@@ -184,14 +178,15 @@
             # TODO: this is inefficient. get_daily_interest_history should be modified
             # to return all maturities if no maturity is specified. otherwise, this is
             # duplicating a ton of operations
             for maturity in keys['YIELD_CURVE']:
                 curve_rate = get_daily_interest_history(maturity=maturity,
                                                         start_date=args['start_date'],
                                                         end_date=args['start_date'])
+
                 yield_curve[maturity] = curve_rate[list(
                     curve_rate.keys())[0]]/100
 
                 if print_format_to_screen(args):
                     from scrilla.util.outputter import scalar_result
                     scalar_result(calculation=maturity,
                                   result=yield_curve[maturity], currency=False)
@@ -440,30 +435,33 @@
         selected_function, required_length, exact = cli_correlation_series, 2, True
 
     # FUNCTION: Discount Dividend Model
     elif args['function_arg'] in definitions.FUNC_DICT["discount_dividend"]['values']:
         def cli_discount_dividend():
             from scrilla.services import get_dividend_history
             from scrilla.analysis.objects.cashflow import Cashflow
+            from scrilla.static.keys import keys
             model_results = {}
 
             for arg in args['tickers']:
                 dividends = get_dividend_history(arg)
                 if args['discount'] is None:
                     from scrilla.analysis.markets import cost_of_equity
                     discount = cost_of_equity(
                         ticker=arg, method=args['estimation_method'])
                 else:
                     discount = args['discount']
-                model_results[f'{arg}_discount_dividend'] = Cashflow(sample=dividends,
-                                                                     discount_rate=discount).calculate_net_present_value()
+                result = Cashflow(sample=dividends,
+                                  discount_rate=discount).calculate_net_present_value()
+                model_results[arg] = {keys['MODELS']['DDM']: result}
+
                 if print_format_to_screen(args):
                     from scrilla.util.outputter import scalar_result
                     scalar_result(f'Net Present Value ({arg} dividends)',
-                                  model_results[f'{arg}_discount_dividend'])
+                                  model_results[arg][keys['MODELS']['DDM']])
 
             if print_json_to_screen(args):
                 from json import dumps
                 print(dumps(model_results))
 
             if args['save_file'] is not None:
                 from scrilla.files import save_file
@@ -509,29 +507,26 @@
             if args['investment'] is not None:
                 from scrilla.services import get_daily_prices_latest
                 prices = get_daily_prices_latest(
                     tickers=args['tickers'])
             else:
                 prices = None
 
-            print(prices)
-
             if print_format_to_screen(args):
                 from scrilla.util.outputter import efficient_frontier as frontier_output
                 frontier_output(portfolio=portfolio,
                                 frontier=frontier,
                                 investment=args['investment'],
                                 latest_prices=prices)
             if print_json_to_screen(args):
                 from json import dumps
-                from scrilla.static.formats import format_frontier
-                print(dumps(format_frontier(portfolio=portfolio,
-                                            frontier=frontier,
-                                            investment=args['investment'],
-                                            latest_prices=prices)))
+                print(dumps(formats.format_frontier(portfolio=portfolio,
+                                                    frontier=frontier,
+                                                    investment=args['investment'],
+                                                    latest_prices=prices)))
 
             if args['save_file'] is not None:
                 from scrilla.files import save_frontier
                 save_frontier(portfolio=portfolio,
                               frontier=frontier,
                               investment=args['investment'],
                               file_name=args['save_file'],
@@ -564,19 +559,18 @@
                 optimal_result(portfolio=portfolio,
                                allocation=allocation,
                                investment=args['investment'],
                                latest_prices=prices)
 
             if print_json_to_screen(args):
                 from json import dumps
-                from scrilla.static.formats import format_allocation
-                print(dumps(format_allocation(allocation=allocation,
-                                              portfolio=portfolio,
-                                              investment=args['investment'],
-                                              latest_prices=prices)))
+                print(dumps(formats.format_allocation(allocation=allocation,
+                                                      portfolio=portfolio,
+                                                      investment=args['investment'],
+                                                      latest_prices=prices)))
 
             if args['save_file'] is not None:
                 from scrilla.files import save_allocation
                 save_allocation(allocation=allocation,
                                 portfolio=portfolio,
                                 file_name=args['save_file'],
                                 investment=args['investment'],
@@ -641,20 +635,19 @@
                 optimal_result(
                     portfolio=portfolio,
                     allocation=allocation,
                     investment=args['investment'],
                     latest_prices=prices)
 
             if print_json_to_screen(args):
-                from scrilla.static.formats import format_allocation
                 from json import dumps
-                print(dumps(format_allocation(allocation=allocation,
-                                              portfolio=portfolio,
-                                              investment=args['investment'],
-                                              latest_prices=prices)))
+                print(dumps(formats.format_allocation(allocation=allocation,
+                                                      portfolio=portfolio,
+                                                      investment=args['investment'],
+                                                      latest_prices=prices)))
 
             if args['save_file'] is not None:
                 from scrilla.files import save_allocation
                 save_allocation(allocation=allocation,
                                 portfolio=portfolio,
                                 file_name=args['save_file'],
                                 investment=args['investment'],
@@ -687,20 +680,19 @@
                 from scrilla.util.outputter import optimal_result
                 optimal_result(portfolio=portfolio,
                                allocation=allocation,
                                investment=args['investment'],
                                latest_prices=prices)
 
             if print_json_to_screen(args):
-                from scrilla.static.formats import format_allocation
                 from json import dumps
-                print(dumps(format_allocation(allocation=allocation,
-                                              portfolio=portfolio,
-                                              investment=args['investment'],
-                                              latest_prices=prices)))
+                print(dumps(formats.format_allocation(allocation=allocation,
+                                                      portfolio=portfolio,
+                                                      investment=args['investment'],
+                                                      latest_prices=prices)))
 
             if args['save_file'] is not None:
                 from scrilla.files import save_allocation
                 save_allocation(allocation=allocation,
                                 portfolio=portfolio,
                                 file_name=args['save_file'],
                                 investment=args['investment'],
@@ -930,17 +922,16 @@
             from scrilla.services import get_risk_free_rate
             from scrilla.settings import RISK_FREE_RATE
             rate = {}
             rate[RISK_FREE_RATE] = get_risk_free_rate()
 
             if print_format_to_screen(args):
                 from scrilla.util.outputter import title_line, scalar_result
-                from scrilla.static.formats import formats
                 title_line("Risk Free Rate")
-                scalar_result(calculation=formats['RISK_FREE_TITLE'].format(RISK_FREE_RATE),
+                scalar_result(calculation=formats.formats['RISK_FREE_TITLE'].format(RISK_FREE_RATE),
                               result=rate[RISK_FREE_RATE], currency=False)
             if print_json_to_screen(args):
                 from json import dumps
                 print(dumps(rate))
 
             if args['save_file'] is not None:
                 from scrilla.files import save_file
@@ -1086,16 +1077,15 @@
                 from scrilla.files import save_file
                 save_file(file_to_save=all_stats, file_name=args['save_file'])
         selected_function, required_length = cli_statistic_history, 1
 
     # FUNCTION: Set Watchlist
     elif args['function_arg'] in definitions.FUNC_DICT["watchlist"]['values']:
         def cli_watchlist():
-            from scrilla.files import add_watchlist
-            add_watchlist(new_tickers=args['tickers'])
+            files.add_watchlist(new_tickers=args['tickers'])
             logger.info(
                 "Watchlist saved. Use -ls option to print watchlist.", 'do_program')
         selected_function, required_length = cli_watchlist, 1
 
     else:
         def cli_help():
             from scrilla.util.outputter import help_msg
```

### Comparing `scrilla-1.5.7/src/scrilla/services.py` & `scrilla-1.6.0/src/scrilla/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,17 +132,14 @@
                 end_string = dater.to_string(end_date)
             query += f'&{self.service_map["PARAMS"]["END"]}={end_string}'
 
         if start_date is not None and not self._is_treasury():
             start_string = dater.to_string(start_date)
             query += f'&{self.service_map["PARAMS"]["START"]}={start_string}'
 
-        logger.debug(
-            f'StatManager Query (w/o key) = {query}', 'StatManager._construct_query')
-
         if self.service_map["PARAMS"].get("KEY", None) is not None:
             if query:
                 return f'{query}&{self.service_map["PARAMS"]["KEY"]}={self.key}'
             return f'{self.service_map["PARAMS"]["KEY"]}={self.key}'
         return query
 
     def _construct_stat_url(self, symbol: str, start_date: date, end_date: date):
@@ -186,15 +183,20 @@
 
         .. notes::
             * The URL returned by this method will always contain a query for a historical range of US Treasury Yields, i.e. this method is specifically for queries involving the "Risk-Free" (right? right? *crickets*) Yield Curve. 
         """
         url = f'{self.url}/{self.service_map["PATHS"]["YIELD"]}?'
         if self._is_treasury():
             url += f'{self.service_map["PARAMS"]["DATA"]}={self.service_map["ARGUMENTS"]["DAILY"]}'
-        url += self._construct_query(start_date=start_date, end_date=end_date)
+        query = self._construct_query(start_date=start_date, end_date=end_date)
+        
+        logger.debug(
+            f'StatManager Query (w/o key) = {url}?{query}', 'StatManager._construct_query')
+
+        url += query
         return url
 
     def get_stats(self, symbol, start_date, end_date):
         url = self._construct_stat_url(symbol, start_date, end_date)
         response = requests.get(url).json()
 
         raw_stat = response[self.service_map["KEYS"]["FIRST_LAYER"]
@@ -202,41 +204,52 @@
         formatted_stat = {}
 
         for stat in raw_stat:
             formatted_stat[stat[0]] = stat[1]
         return formatted_stat
 
     def get_interest_rates(self, start_date, end_date):
+        """
+
+        .. notes::
+            - Regardless of the `scrilla.settings.STAT_MANAGER`, the return format for this method is as follows: 
+                ```json
+                {
+                    "date": [ "value", "value", ... , "value" ],
+                    "date": [ "value", "value", ... , "value" ]
+                }
+                ```
+        """
         url = self._construct_interest_url(
             start_date=start_date, end_date=end_date)
         formatted_interest = {}
 
         if self._is_quandl():
             response = requests.get(url)
 
             response = response.json()
             raw_interest = response[self.service_map["KEYS"]
                                     ["FIRST_LAYER"]][self.service_map["KEYS"]["SECOND_LAYER"]]
             for rate in raw_interest:
                 formatted_interest[rate[0]] = rate[1:]
 
         elif self._is_treasury():
-            # this is ugly, but it's the government's fault for not supporting an API
+            # NOTE: this is ugly, but it's the government's fault for not supporting an API
             # from this century.
 
             def __paginate(page_no, page_url):
                 page_url = f'{page_url}&{self.service_map["PARAMS"]["PAGE"]}={page_no}'
                 logger.verbose(
                     f'Paginating: {page_url}', 'StatManager.get_interest_rates.__paginate')
                 page_response = ET.fromstring(requests.get(page_url).text)
                 return page_no - 1, page_response
 
             record_time = dater.business_days_between(
                 constants.constants['YIELD_START_DATE'], end_date, True)
-            # subtract to reindex to 0
+            # NOTE: subtract to reindex to 0
             pages = record_time // self.service_map["KEYS"]["PAGE_LENGTH"] - 1
             pages += 1 if record_time % self.service_map["KEYS"]["PAGE_LENGTH"] > 0 else 0
             page = pages
 
             logger.debug(
                 f'Sorting through {pages} pages of Treasury data', 'StatManager.get_interest_rates')
             logger.debug(
@@ -382,15 +395,15 @@
         elif asset_type == keys.keys['ASSETS']['CRYPTO']:
             query += f'&{self.service_map["PARAMS"]["FUNCTION"]}={self.service_map["ARGUMENTS"]["CRYPTO_DAILY"]}'
             query += f'&{self.service_map["PARAMS"]["DENOMINATION"]}={constants.constants["DENOMINATION"]}'
 
         auth_query = query + f'&{self.service_map["PARAMS"]["KEY"]}={self.key}'
         url = f'{self.url}?{auth_query}'
         logger.debug(
-            f'PriceManager query (w/o key) = {query}', 'PriceManager._construct_url')
+            f'PriceManager query (w/o key) = {self.url}?{query}', 'PriceManager._construct_url')
         return url
 
     def get_prices(self, ticker: str, start_date: date, end_date: date, asset_type: str):
         """
         Retrieve prices from external service.
 
         Parameters
@@ -765,17 +778,18 @@
         maturity, start_date=start_date, end_date=end_date)
 
     if rates is not None:
         logger.debug(
             f'Comparing cache-size({len(rates)}) = date-size({dater.business_days_between(start_date, end_date, True)})', 'get_daily_interest_history')
 
     # TODO: this only works when stats are reported daily and that the latest date in the dataset is actually end_date.
+            # bond prices aren't published until the end of the day...
     if rates is not None and \
-            dater.to_string(end_date) in rates.keys() and \
-            dater.business_days_between(start_date, end_date) == len(rates):
+            dater.to_string(dater.get_previous_business_date(end_date)) in rates.keys() and \
+            dater.business_days_between(start_date, end_date, True) == len(rates):
         return rates
 
     logger.debug(
         f'Cached {maturity} data is out of date, passing request to external service', 'get_daily_interest_history')
     rates = stat_manager.get_interest_rates(
         start_date=start_date, end_date=end_date)
 
@@ -791,15 +805,16 @@
     Returns the latest interest rate for the inputted US Treasury maturity.
 
     Parameters
     ----------
     1. **maturity**: ``str``
         Maturity of the US Treasury security whose interest rate is to be retrieved. Allowable values accessible through `keys.keys['YIELD_CURVE']
     """
-    end_date = dater.get_last_trading_date(True)
+        # the government is lazy and doesn't publish data on time, so subtract a business day
+    end_date = dater.decrement_date_by_business_days(dater.get_last_trading_date(True), 1, True)
     start_date = dater.decrement_date_by_business_days(end_date, 1, True)
     interest_history = get_daily_interest_history(
         maturity, start_date, end_date)
     first_element = helper.get_first_json_key(interest_history)
     return interest_history[first_element]
```

### Comparing `scrilla-1.5.7/src/scrilla/settings.py` & `scrilla-1.6.0/src/scrilla/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,7 +333,9 @@
     ------
     1. **scrilla.settings.APIKeyError**
     """
     if not AV_KEY:
         raise APIKeyError(
             'Alpha Vantage API Key not found. Either set ALPHA_VANTAGE_KEY environment variable or use "-store" CLI function to save key.')
     return AV_KEY
+
+print(CACHE_DIR)
```

### Comparing `scrilla-1.5.7/src/scrilla/static/config.py` & `scrilla-1.6.0/src/scrilla/static/config.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/static/constants.py` & `scrilla-1.6.0/src/scrilla/static/constants.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/static/definitions.py` & `scrilla-1.6.0/src/scrilla/static/definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         'description': "Generate a sample of the portfolio's efficient frontier for the supplied list of tickers. The efficient frontier algorithm will minimize a portfolio's volality for a given rate of return and then maximize its return, and then use these points to generate the rest of the frontier by taking increments along the line connecting the (risk,return) profile of the minimum volatility portfolio to the (risk, return) profile of the maximum return portfolio. The number of points calculated in the efficient frontier can be specifed as an integer with the -steps flag. If no -steps is provided, the value of the environment variable FRONTIER_STEPS will be used.",
         'tickers': True,
     },
     "help": {
         'name': 'Help Message',
         'values': ["help", "h"],
         'args': None,
-        'description': "Print this help message.",
+        'description': "Print this help message. Provide a function name(s) to only display the help message for a specific function(s)",
         'tickers': False,
     },
     "interest_history": {
         'name': 'Interest Rate History',
         'values': ["interest", "int"],
         'args': ['start_date', 'end_date', 'save_file', 'suppress_output', 'json'],
         'description': "Prints the interest histories for each inputted maturity over the specified date range. If no date range is given, price histories will default to the last 100 days. See `scrilla -yield` for list of maturities.",
@@ -128,15 +128,15 @@
         'args': None,
         'description': "Lists the equity symbols currently saved to your watchlist.",
         'tickers': False,
     },
     "maximize_return": {
         'name': 'Maximize Portfolio Return',
         'values': ["max-return", "max"],
-        'args': ['start_date', 'end_date', 'investment', 'target', 'save_file', 'suppress_output', 'json', keys.keys['ESTIMATION']['MOMENT'], keys.keys['ESTIMATION']['PERCENT'], keys.keys['ESTIMATION']['LIKE']],
+        'args': ['start_date', 'end_date', 'investment', 'save_file', 'suppress_output', 'json', keys.keys['ESTIMATION']['MOMENT'], keys.keys['ESTIMATION']['PERCENT'], keys.keys['ESTIMATION']['LIKE']],
         'description': "Maximize the return of the portfolio defined by the supplied list of ticker symbols. Returns an array representing the allocations to be made for each asset in a portfolio. If no start or end dates are specified, calculations default to the last 100 days of prices. You can specify an investment with the '-invest' flag, otherwise the result will be output in percentage terms. Note: This function will always allocate 100% to the asset with the highest return. It's a good way to check and see if there are bugs in the algorithm after changes.",
         'tickers': True,
     },
     "moving_averages": {
         'name': 'Moving Averages Series',
         'values': ["mov-averages", "mas"],
         'args': ['start_date', 'end_date', keys.keys['ESTIMATION']['MOMENT'], keys.keys['ESTIMATION']['PERCENT'], keys.keys['ESTIMATION']['LIKE']],
@@ -290,15 +290,15 @@
         'description': "Saves the supplist list of tickers to your watchlist. These equity symbol are used by the screening algorithms when searching for stocks that trade at a discount.",
         'tickers': False,
     },
     "yield_curve": {
         'name': 'Latest Yield Curve',
         'values': ["yield-curve", "yc"],
         'args': ['start_date'],
-        'description': "Displays the current United States Treasury Yield Curve.",
+        'description': "Displays the United States Treasury Yield Curve for a given day.",
         'tickers': False,
     }
 }
 """
 A dictionary containing configuration information for function arguments. This dictionary is used at various points in the library, such as `scrilla.gui.widgets.functions` and `scrilla.static.formats.format_args`, to generate function interfaces. 
 """
 
@@ -515,25 +515,26 @@
         'group': 'estimation_method',
         'required': False,
         'syntax': None,
         'cli_only': False
     }
 }
 """
-A dictionary containing configuration information for application arguments. This dictionary is used at various points in the library, such as `scrilla.gui.widgets.functions` and `scrilla.util.helper`, to parse construct and parse input elements.
+A dictionary containing configuration information for application arguments. This dictionary is used at various points in the library, such as `scrilla.gui.widgets.functions` and `scrilla.util.helper`, to construct and parse input elements.
 
 .. notes::
-    * Every argument has four ways of being inputted: short-dash-long, long-dash-long, short-dash-short, long-dash-short, e.g. the following commands are all equivalent,
-    ```
+    - Every argument has four ways of being inputted into the CLI: short-dash-long, long-dash-long, short-dash-short, long-dash-short, e.g. the following commands are all equivalent,
+    ```shell
     scrilla risk-profile LMT GD LNT -json
     ```
-    ```
+    ```shell
     scrilla risk-profile LMT GD LNT --json
     ```
-    ```
+    ```shell
     scrilla risk-profile LMT GD LNT -js
     ```
-    ```
+    ```shell
     scrilla risk-profile LMT GD LNT --js
     ```
-    * arguments with a format of `group` are mutually exclusively modes, similar to a radio button.
+    - arguments with a format of `group` are mutually exclusively modes, similar to a radio button. Indeed, group arguments are translated into `PySide6.QtWidgets.QRadioButtons` in `scrilla.gui.widgets.factories.group_widget_factory`.
+    - The attribute `cli_only` determes which arguments are available as GUI widgets and which arguments are only accessible through the command line interface (cli).
 """
```

### Comparing `scrilla-1.5.7/src/scrilla/static/formats.py` & `scrilla-1.6.0/src/scrilla/static/formats.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,17 +53,17 @@
         total = portfolio.calculate_actual_total(
             x=allocation, total=investment, latest_prices=latest_prices)
 
     annual_volatility = portfolio.volatility_function(x=allocation)
     annual_return = portfolio.return_function(x=allocation)
 
     for j, item in enumerate(portfolio.tickers):
-        holding = {'ticker': item, 'allocation': round(allocation[j], constants['ACCURACY']), 'annual_return': round(
-            portfolio.mean_return[j], constants['ACCURACY']), 'annual_volatility': round(
-            portfolio.sample_vol[j], constants['ACCURACY'])}
+        holding = {'ticker': item, 'allocation': round(allocation[j], constants.constants['ACCURACY']), 'annual_return': round(
+            portfolio.mean_return[j], constants.constants['ACCURACY']), 'annual_volatility': round(
+            portfolio.sample_vol[j], constants.constants['ACCURACY'])}
         if investment is not None:
             holding['shares'] = float(shares[j])
         allocation_format.append(holding)
 
     json_format = {'holdings': allocation_format,
                    'portfolio_return': annual_return, 'portfolio_volatility': annual_volatility}
```

### Comparing `scrilla-1.5.7/src/scrilla/static/functions.py` & `scrilla-1.6.0/src/scrilla/static/functions.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/static/keys.py` & `scrilla-1.6.0/src/scrilla/static/keys.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/util/dater.py` & `scrilla-1.6.0/src/scrilla/util/dater.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,16 +299,16 @@
         if is_trading_date(this_date, bond):
             dates.append(this_date)
     return dates
 
 
 def business_days_between(start_date: Union[date, str], end_date: Union[date, str], bond: bool = False) -> List[int]:
     start_date, end_date = validate_date_range(start_date, end_date)
-    dates = dates_between(start_date, end_date)
-    return len([1 for this_date in dates if is_trading_date(this_date, bond)])
+    dates = business_dates_between(start_date, end_date, bond)
+    return len(dates)
 
 
 def weekends_between(start_date: Union[date, str], end_date: Union[date, str]) -> List[int]:
     start_date, end_date = validate_date_range(start_date, end_date)
     dates = dates_between(start_date, end_date)
     return len([1 for day in dates if day.weekday() > 4])
```

### Comparing `scrilla-1.5.7/src/scrilla/util/errors.py` & `scrilla-1.6.0/src/scrilla/util/errors.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/util/helper.py` & `scrilla-1.6.0/src/scrilla/util/helper.py`

 * *Files identical despite different names*

### Comparing `scrilla-1.5.7/src/scrilla/util/outputter.py` & `scrilla-1.6.0/src/scrilla/util/outputter.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     print(' '*indent, calculation, ' = ', round(float(result), 4), '%')
 
 
 def equivalent_result(right_hand, left_hand, value, indent=formats.formats['INDENT']):
     print(' '*indent, f'{right_hand} = {left_hand} = {value}')
 
 
-def help_msg(indent=formats.formats['INDENT']):
+def help_msg(indent: int = formats.formats['INDENT'], function_filter: Union[List[str], None] = None):
     func_dict, arg_dict = definitions.FUNC_DICT, definitions.ARG_DICT
 
     title_line('scrilla')
     space(1)
 
     for paragraph in definitions.HELP_MSG:
         for line in break_lines(paragraph):
@@ -122,42 +122,45 @@
         space(1)
 
     title_line('SYNTAX')
     center(definitions.SYNTAX)
     space(1)
 
     for func_name in func_dict:
-        title_line(func_dict[func_name]['name'])
-        for line in break_lines(func_dict[func_name]['description']):
-            center(line)
-        separator_line()
+        if function_filter is None or len(function_filter) == 0 or \
+                any(filt in func_dict[func_name]['values'] for filt in function_filter):
+
+            title_line(func_dict[func_name]['name'])
+            for line in break_lines(func_dict[func_name]['description']):
+                center(line)
+            separator_line()
 
-        commands = func_dict[func_name]['values']
-        print(' ', f'COMMAND: {commands[0]}, {commands[1]}')
+            commands = func_dict[func_name]['values']
+            print(' ', f'COMMAND: {commands[0]}, {commands[1]}')
 
-        if func_dict[func_name]['args'] is not None:
-            for arg_name in func_dict[func_name]['args']:
-                aliases = arg_dict[arg_name]['values']
+            if func_dict[func_name]['args'] is not None:
+                for arg_name in func_dict[func_name]['args']:
+                    aliases = arg_dict[arg_name]['values']
 
-                print(
-                    ' '*indent, f'OPTION: {aliases[0]}, {aliases[1]}, {aliases[2]}, {aliases[3]}')
+                    print(
+                        ' '*indent, f'OPTION: {aliases[0]}, {aliases[1]}, {aliases[2]}, {aliases[3]}')
 
-                if arg_dict[arg_name]['required']:
-                    print(' '*2*indent, 'REQUIRED')
+                    if arg_dict[arg_name]['required']:
+                        print(' '*2*indent, 'REQUIRED')
 
-                print(' '*2*indent, f'NAME: {arg_dict[arg_name]["name"]}')
+                    print(' '*2*indent, f'NAME: {arg_dict[arg_name]["name"]}')
 
-                if arg_dict[arg_name]['default'] is not None:
-                    print(' '*2*indent,
-                          f'DEFAULT: {arg_dict[arg_name]["default"]}')
+                    if arg_dict[arg_name]['default'] is not None:
+                        print(' '*2*indent,
+                              f'DEFAULT: {arg_dict[arg_name]["default"]}')
 
-                if arg_dict[arg_name]['syntax'] is not None:
-                    print(' '*2*indent,
-                          f'FORMAT: {arg_dict[arg_name]["syntax"]}')
-        separator_line()
+                    if arg_dict[arg_name]['syntax'] is not None:
+                        print(' '*2*indent,
+                              f'FORMAT: {arg_dict[arg_name]["syntax"]}')
+            separator_line()
 
 # ANALYSIS SPECIFIC OUTPUT FUNCTIONS
 
 
 def portfolio_percent_result(result, tickers, indent=formats.formats['INDENT']):
     for i, item in enumerate(tickers):
         print(' '*indent, f'{item} =', round(100*result[i], 2), '%')
```

### Comparing `scrilla-1.5.7/src/scrilla.egg-info/PKG-INFO` & `scrilla-1.6.0/src/scrilla.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrilla
-Version: 1.5.7
+Version: 1.6.0
 Summary: a financial optimization program
 Author: Grant Moore
 Author-email: chinchalinchin@gmail.com
 License: GNU GPL v3
 Project-URL: Documentation, https://chinchalinchin.github.io/scrilla/
 Project-URL: Source, https://github.com/chinchalinchin/scrilla
 Keywords: finance,statistics,stock market,equities,cryptocurrencies,optimization
@@ -93,15 +93,15 @@
 
 ```
 pip install scrilla-<major>.<minor>.<micro>-py3-none-any.whl
 ```
 
 ## Configuration
 
-In order to use this application, you will need to register for API keys with [AlphaVantage](https://www.alphavantage.co), [IEX](https://iexcloud.io/) and [Quandl](https://www.quandl.com/). The program will need to be made aware of these keys somehow. The best option is storing these credentials in environment variables. You can add the following lines to your <i>.bashrc</i> profile or corresponding configuration file for whatever shell you are using,
+In order to use this application, you will need to register for API keys with [AlphaVantage](https://www.alphavantage.co), [IEX](https://iexcloud.io/) and [Quandl/Nasdaq](https://www.quandl.com/). The program will need to be made aware of these keys somehow. The best option is storing these credentials in environment variables. You can add the following lines to your <i>.bashrc</i> profile or corresponding configuration file for whatever shell you are using,
 
 ```shell
 export ALPHA_VANTAGE_KEY=<key goes here>
 export QUANDL_KEY=<key goes here>
 export IEX_KEY=<key goes here>
 ```
 
@@ -113,14 +113,16 @@
 
 where `<key>` is one of the values: **ALPHA_VANTAGE_KEY**, **QUANDL_KEY** or **IEX_KEY**. `<value>` is the corresponding key itself given to you after registration. Obviously, `<value>` is case-sensitive
 
 Keep in mind if using this method to store the API keys, the keys will be stored unencrypted in the local installation's <i>/data/common/</i> directory. The recommended method is storing the credentials in the environment. 
 
 If no API keys are found through either of these methods, the application will raise an exception.
 
+**NOTE**: The **Quandl**/**Nasdaq** key is technically no required for the majority of the application to function, as interest rates are now retrieved directly from the **US Treasury** RSS feed. However, it is still recommended that you register for an API key, as **Quandl**/**Nasdaq** is still the only source of economic statistics, like GDP or inflation rates. 
+
 ### Environment File
 
 A sample environment file has been included in _/env/.sample.env_. To configure the application environment, copy this file into a new environment, adjust the values and load it into your session,
 
 ```shell
 cp ./env/.sample.env ./env/.env
 # adjust .env values
```

### Comparing `scrilla-1.5.7/src/scrilla.egg-info/SOURCES.txt` & `scrilla-1.6.0/src/scrilla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

