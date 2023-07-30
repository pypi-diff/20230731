# Comparing `tmp/calendra-7.6.1.tar.gz` & `tmp/calendra-7.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendra-7.6.1.tar", last modified: Sun Sep  4 00:25:58 2022, max compression
+gzip compressed data, was "calendra-7.7.0.tar", last modified: Sun Jul 30 23:47:52 2023, max compression
```

## Comparing `calendra-7.6.1.tar` & `calendra-7.7.0.tar`

### file list

```diff
@@ -1,226 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 00:25:58.004720 calendra-7.6.1/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-04 00:25:15.000000 calendra-7.6.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-09-04 00:25:15.000000 calendra-7.6.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-09-04 00:25:15.000000 calendra-7.6.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 00:25:57.976719 calendra-7.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2022-09-04 00:25:15.000000 calendra-7.6.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-04 00:25:15.000000 calendra-7.6.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 00:25:57.976719 calendra-7.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-09-04 00:25:15.000000 calendra-7.6.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-04 00:25:15.000000 calendra-7.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-04 00:25:15.000000 calendra-7.6.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    37035 2022-09-04 00:25:15.000000 calendra-7.6.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-09-04 00:25:15.000000 calendra-7.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7442 2022-09-04 00:25:58.004720 calendra-7.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6811 2022-09-04 00:25:15.000000 calendra-7.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 00:25:57.976719 calendra-7.6.1/calendra/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 00:25:57.980719 calendra-7.6.1/calendra/africa/
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/africa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/africa/algeria.py
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/africa/angola.py
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/africa/benin.py
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/africa/ivory_coast.py
--rw-r--r--   0 runner    (1001) docker     (121)     2399 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/africa/kenya.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/africa/madagascar.py
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/africa/mozambique.py
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/africa/nigeria.py
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/africa/sao_tome.py
--rw-r--r--   0 runner    (1001) docker     (121)     5504 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/africa/south_africa.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 00:25:57.980719 calendra-7.6.1/calendra/america/
--rw-r--r--   0 runner    (1001) docker     (121)     3528 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/america/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4700 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/america/argentina.py
--rw-r--r--   0 runner    (1001) docker     (121)     2536 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/america/barbados.py
--rw-r--r--   0 runner    (1001) docker     (121)    20368 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/america/brazil.py
--rw-r--r--   0 runner    (1001) docker     (121)    10180 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/america/canada.py
--rw-r--r--   0 runner    (1001) docker     (121)     3750 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/america/chile.py
--rw-r--r--   0 runner    (1001) docker     (121)     4169 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/america/colombia.py
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/america/mexico.py
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/america/panama.py
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/america/paraguay.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 00:25:57.980719 calendra-7.6.1/calendra/asia/
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/asia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5592 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/asia/china.py
--rw-r--r--   0 runner    (1001) docker     (121)     3278 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/asia/hong_kong.py
--rw-r--r--   0 runner    (1001) docker     (121)     2649 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/asia/israel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4376 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/asia/japan.py
--rw-r--r--   0 runner    (1001) docker     (121)     2525 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/asia/kazakhstan.py
--rw-r--r--   0 runner    (1001) docker     (121)     3215 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/asia/malaysia.py
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/asia/philippines.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/asia/qatar.py
--rw-r--r--   0 runner    (1001) docker     (121)     2808 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/asia/singapore.py
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/asia/south_korea.py
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/asia/taiwan.py
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/astronomy.py
--rw-r--r--   0 runner    (1001) docker     (121)    36986 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/core.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      146 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/create-astronomical-data.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/equinoxes.json.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 00:25:57.988720 calendra-7.6.1/calendra/europe/
--rw-r--r--   0 runner    (1001) docker     (121)     4658 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/austria.py
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/belarus.py
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/belgium.py
--rw-r--r--   0 runner    (1001) docker     (121)     2574 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/bulgaria.py
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/cayman_islands.py
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/croatia.py
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/cyprus.py
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/czech_republic.py
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/denmark.py
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/estonia.py
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/european_central_bank.py
--rw-r--r--   0 runner    (1001) docker     (121)     1612 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/finland.py
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/france.py
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/georgia.py
--rw-r--r--   0 runner    (1001) docker     (121)     4589 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/germany.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/greece.py
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/guernsey.py
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/hungary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/iceland.py
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/ireland.py
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/italy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1801 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/latvia.py
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/lithuania.py
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/luxembourg.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/malta.py
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/monaco.py
--rw-r--r--   0 runner    (1001) docker     (121)     9078 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/netherlands.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/norway.py
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/poland.py
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/portugal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/romania.py
--rw-r--r--   0 runner    (1001) docker     (121)     3547 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/russia.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 00:25:57.988720 calendra-7.6.1/calendra/europe/scotland/
--rw-r--r--   0 runner    (1001) docker     (121)    14009 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/scotland/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 00:25:57.988720 calendra-7.6.1/calendra/europe/scotland/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/scotland/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/scotland/mixins/autumn_holiday.py
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/scotland/mixins/fair_holiday.py
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/scotland/mixins/spring_holiday.py
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/scotland/mixins/victoria_day.py
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/serbia.py
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/slovakia.py
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/slovenia.py
--rw-r--r--   0 runner    (1001) docker     (121)     5138 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/spain.py
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/sweden.py
--rw-r--r--   0 runner    (1001) docker     (121)     8725 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/switzerland.py
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/turkey.py
--rw-r--r--   0 runner    (1001) docker     (121)     2812 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/ukraine.py
--rw-r--r--   0 runner    (1001) docker     (121)     3585 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/europe/united_kingdom.py
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4925 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/holiday.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 00:25:57.988720 calendra-7.6.1/calendra/oceania/
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/oceania/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10933 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/oceania/australia.py
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/oceania/marshall_islands.py
--rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/oceania/new_zealand.py
--rw-r--r--   0 runner    (1001) docker     (121)     3954 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/precomputed_astronomy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4417 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/registry_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     4525 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/skyfield_astronomy.py
--rw-r--r--   0 runner    (1001) docker     (121)     7314 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/solar_terms.json.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 00:25:57.992720 calendra-7.6.1/calendra/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4642 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28848 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_africa.py
--rw-r--r--   0 runner    (1001) docker     (121)    28414 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_america.py
--rw-r--r--   0 runner    (1001) docker     (121)    48553 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_asia.py
--rw-r--r--   0 runner    (1001) docker     (121)     3496 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_astronomy.py
--rw-r--r--   0 runner    (1001) docker     (121)    34341 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_brazil.py
--rw-r--r--   0 runner    (1001) docker     (121)    17100 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_canada.py
--rw-r--r--   0 runner    (1001) docker     (121)    31483 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)   107365 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_europe.py
--rw-r--r--   0 runner    (1001) docker     (121)    11052 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_germany.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_global_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     5186 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_ical_export.py
--rw-r--r--   0 runner    (1001) docker     (121)     5577 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_mozambique.py
--rw-r--r--   0 runner    (1001) docker     (121)    13673 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_oceania.py
--rw-r--r--   0 runner    (1001) docker     (121)     6904 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_precomputed_astronomy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5157 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_registry_africa.py
--rw-r--r--   0 runner    (1001) docker     (121)     3636 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_registry_america.py
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_registry_asia.py
--rw-r--r--   0 runner    (1001) docker     (121)     4943 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_registry_europe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_registry_oceania.py
--rw-r--r--   0 runner    (1001) docker     (121)     3407 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_registry_usa.py
--rw-r--r--   0 runner    (1001) docker     (121)    18902 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_scotland.py
--rw-r--r--   0 runner    (1001) docker     (121)     3496 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_skyfield_astronomy.py
--rw-r--r--   0 runner    (1001) docker     (121)    14036 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_spain.py
--rw-r--r--   0 runner    (1001) docker     (121)    47309 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_switzerland.py
--rw-r--r--   0 runner    (1001) docker     (121)     3369 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_turkey.py
--rw-r--r--   0 runner    (1001) docker     (121)    79160 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/tests/test_usa.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 00:25:58.000720 calendra-7.6.1/calendra/usa/
--rw-r--r--   0 runner    (1001) docker     (121)     3374 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/alabama.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/alaska.py
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/american_samoa.py
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/arizona.py
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/arkansas.py
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/california.py
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/colorado.py
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/connecticut.py
--rw-r--r--   0 runner    (1001) docker     (121)    10359 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/delaware.py
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/district_columbia.py
--rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/florida.py
--rw-r--r--   0 runner    (1001) docker     (121)     2930 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/georgia.py
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/guam.py
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/hawaii.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/idaho.py
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/illinois.py
--rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/indiana.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/iowa.py
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/kansas.py
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/kentucky.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/louisiana.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/maine.py
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/maryland.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/massachusetts.py
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/michigan.py
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/minnesota.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/mississippi.py
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/missouri.py
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/montana.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/nebraska.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/nevada.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/new_hampshire.py
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/new_jersey.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/new_mexico.py
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/new_york.py
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/north_carolina.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/north_dakota.py
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/ohio.py
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/oklahoma.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/oregon.py
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/pennsylvania.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/rhode_island.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/south_carolina.py
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/south_dakota.py
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/tennessee.py
--rw-r--r--   0 runner    (1001) docker     (121)     3138 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/texas.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/utah.py
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/vermont.py
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/virginia.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/washington.py
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/west_virginia.py
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/wisconsin.py
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-09-04 00:25:15.000000 calendra-7.6.1/calendra/usa/wyoming.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 00:25:57.976719 calendra-7.6.1/calendra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7442 2022-09-04 00:25:57.000000 calendra-7.6.1/calendra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5672 2022-09-04 00:25:57.000000 calendra-7.6.1/calendra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-04 00:25:57.000000 calendra-7.6.1/calendra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-09-04 00:25:57.000000 calendra-7.6.1/calendra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-04 00:25:57.000000 calendra-7.6.1/calendra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 00:25:58.004720 calendra-7.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     3664 2022-09-04 00:25:15.000000 calendra-7.6.1/docs/advanced.md
--rw-r--r--   0 runner    (1001) docker     (121)     4471 2022-09-04 00:25:15.000000 calendra-7.6.1/docs/basic.md
--rw-r--r--   0 runner    (1001) docker     (121)     4592 2022-09-04 00:25:15.000000 calendra-7.6.1/docs/class-options.md
--rw-r--r--   0 runner    (1001) docker     (121)     1406 2022-09-04 00:25:15.000000 calendra-7.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-09-04 00:25:15.000000 calendra-7.6.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2593 2022-09-04 00:25:15.000000 calendra-7.6.1/docs/ical.md
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-09-04 00:25:15.000000 calendra-7.6.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-09-04 00:25:15.000000 calendra-7.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7196 2022-09-04 00:25:15.000000 calendra-7.6.1/docs/iso-registry.md
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-04 00:25:15.000000 calendra-7.6.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-09-04 00:25:15.000000 calendra-7.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-09-04 00:25:15.000000 calendra-7.6.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-09-04 00:25:58.008720 calendra-7.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-09-04 00:25:15.000000 calendra-7.6.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.995426 calendra-7.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-30 23:47:30.000000 calendra-7.7.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-30 23:47:30.000000 calendra-7.7.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.911426 calendra-7.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-30 23:47:30.000000 calendra-7.7.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-30 23:47:30.000000 calendra-7.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.911426 calendra-7.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-30 23:47:30.000000 calendra-7.7.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 23:47:30.000000 calendra-7.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-30 23:47:30.000000 calendra-7.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-30 23:47:30.000000 calendra-7.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37920 2023-07-30 23:47:30.000000 calendra-7.7.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-30 23:47:52.995426 calendra-7.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-07-30 23:47:30.000000 calendra-7.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.915426 calendra-7.7.0/calendra/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.923426 calendra-7.7.0/calendra/africa/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/algeria.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/angola.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/benin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/ivory_coast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/kenya.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/madagascar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/mozambique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/nigeria.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/sao_tome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/south_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/tunisia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.927426 calendra-7.7.0/calendra/america/
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/argentina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/barbados.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/brazil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/canada.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/chile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/colombia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/el_salvador.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/mexico.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/panama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/paraguay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.935426 calendra-7.7.0/calendra/asia/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/china.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/hong_kong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/israel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/japan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/kazakhstan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/malaysia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/philippines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/qatar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/singapore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/south_korea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/taiwan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/astronomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36986 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/core.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      146 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/create-astronomical-data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/equinoxes.json.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.951426 calendra-7.7.0/calendra/europe/
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/austria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/belarus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/belgium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/bulgaria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/cayman_islands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/croatia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/cyprus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/czech_republic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/denmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/estonia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/european_central_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/finland.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/france.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/georgia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/germany.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/greece.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/guernsey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/hungary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/iceland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/ireland.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/italy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/latvia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/lithuania.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/luxembourg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/malta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/monaco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/netherlands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/norway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/poland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/portugal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/romania.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/russia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.951426 calendra-7.7.0/calendra/europe/scotland/
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/scotland/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.955426 calendra-7.7.0/calendra/europe/scotland/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/scotland/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/scotland/mixins/autumn_holiday.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/scotland/mixins/fair_holiday.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/scotland/mixins/spring_holiday.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/scotland/mixins/victoria_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/serbia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/slovakia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/slovenia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/spain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/sweden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/switzerland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/turkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/ukraine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/united_kingdom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/holiday.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.955426 calendra-7.7.0/calendra/oceania/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/oceania/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10933 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/oceania/australia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/oceania/marshall_islands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/oceania/new_zealand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/precomputed_astronomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/registry_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/skyfield_astronomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/solar_terms.json.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.967426 calendra-7.7.0/calendra/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30521 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31913 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49921 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_asia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_astronomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34341 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_brazil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_canada.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31483 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107597 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_europe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_germany.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_global_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_ical_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_mozambique.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_oceania.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_precomputed_astronomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_registry_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_registry_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_registry_asia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_registry_europe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_registry_oceania.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_registry_usa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18902 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_scotland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_skyfield_astronomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_spain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47309 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_switzerland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_turkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79160 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_usa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.991426 calendra-7.7.0/calendra/usa/
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/alabama.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/alaska.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/american_samoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/arizona.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/arkansas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/california.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/colorado.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/connecticut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/delaware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/district_columbia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/florida.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/georgia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/guam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/hawaii.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/idaho.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/illinois.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/indiana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/iowa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/kansas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/kentucky.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/louisiana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/maine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/maryland.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/massachusetts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/michigan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/minnesota.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/mississippi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/missouri.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/montana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/nebraska.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/nevada.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/new_hampshire.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/new_jersey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/new_mexico.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/new_york.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/north_carolina.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/north_dakota.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/ohio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/oklahoma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/oregon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/pennsylvania.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/rhode_island.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/south_carolina.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/south_dakota.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/tennessee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/texas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/utah.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/vermont.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/virginia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/washington.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/west_virginia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/wisconsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/wyoming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.919426 calendra-7.7.0/calendra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-30 23:47:52.000000 calendra-7.7.0/calendra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-30 23:47:52.000000 calendra-7.7.0/calendra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 23:47:52.000000 calendra-7.7.0/calendra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-30 23:47:52.000000 calendra-7.7.0/calendra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-30 23:47:52.000000 calendra-7.7.0/calendra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.991426 calendra-7.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/advanced.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/basic.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/class-options.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/ical.md
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/iso-registry.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-30 23:47:30.000000 calendra-7.7.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-30 23:47:30.000000 calendra-7.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-30 23:47:30.000000 calendra-7.7.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-30 23:47:52.995426 calendra-7.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-30 23:47:30.000000 calendra-7.7.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-30 23:47:30.000000 calendra-7.7.0/tox.ini
```

### Comparing `calendra-7.6.1/.github/PULL_REQUEST_TEMPLATE.md` & `calendra-7.7.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/CHANGES.rst` & `calendra-7.7.0/NEWS.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,49 @@
+v7.7.0
+======
+
+Features
+--------
+
+- Incorporate changes from workalendar v17.0.0 (2023-01-01)
+
+  New calendars
+
+  - New calendar: Added Tunisia calendar by @macharmi (#702)
+  - New calendar: Added El Salvador calendar by @hersoncruz (#708).
+
+  Other changes
+
+  - Update China's public holidays for 2023 (#728).
+  - Removed compatibility with Python 3.6, also, removed tests & amended documentation (#705).
+  - Upgraded `tox` usage, now compatble with tox 4+ (added `allowlist_externals`).
+  - Added support for Python 3.10 (#706).
+  - Added support for Python 3.11 (#732).
+  - Refactor ``NetherlandsWithSchoolHolidays.get_christmas_holidays`` for simplicity and readability.
+
+- Incorporate changes from workalendar v16.4.0 (2022-09-16)
+
+  - Fixed United Kingdom's 2022 holidays ; Added Bank Holiday for the State Funeral of Queen Elizabeth II (#719).
+
+- Require Python 3.8 or later.
+
+
 v7.6.1
-------
+======
 
 Updated some latent references to peopledoc.
 
 v7.6.0
-------
+======
 
 Internal refactoring and simplification. Removed redundant "shift" holidays
 from european countries.
 
 v7.5.0
-------
+======
 
 Incorporate changes from workalendar v16.3.0 (2022-02-22)
 
 Calendars
 
 - New calendar: Added Georgia (country) calendar by @atj01 (#687).
 - New calendar: Added Kazakhstan calendar by @atj01 (#688).
@@ -33,15 +62,15 @@
 
 Incorporate changes from workalendar v16.1.0 (2021-10-01)
 
 - Fixed United Kingdom's 2022 holidays ; Spring Bank Holiday has been moved to the 3rd of June and Queen's Platinum Jubilee added to 2nd of June.
 - New calendar: Added Guernsey calendar by @ludsoft (#681)
 
 v7.4.0
-------
+======
 
 Incorporate changes from workalendar v16.0.0 (2021-09-16)
 
 Calendars
 
 - New calendar: Added Philippines calendar by @micodls (#396)
 
@@ -52,15 +81,15 @@
 - Remove unused `JalaliMixin`
 - Replace `pkg_resources` with `importlib_metadata` to fetch the version number in `__init__.py` (#657)
 - Added new badges (pypi, conda, license) and installation instructions (pip, conda) to readme file @sugatoray (#673).
 - Added the "Workalendar maintainers" in the LICENSE file.
 - Changed the maintainer email.
 
 v7.3.0
-------
+======
 
 Incorporate changes from workalendar v15.4.0 (2021-07-12)
 
 - New calendar: Added Nigeria calendar by @taiyeoguns (#656)
 - Fix: Chilean calendar floating dates, add Indigenous Peoples Day using solar term, thx @ajcobo.
 
 Incorporate changes from workalendar v15.3.1 (2021-07-02)
@@ -95,15 +124,15 @@
 
 Incorporate changes from workalendar v15.0.1 (2021-02-26)
 
 - Hotfix: Taiwan exceptional working day on February, 20th 2021 (#628).
 - Hotfix: September 11th is a working day in Taiwan (#628).
 
 v7.2.0
-------
+======
 
 Incorporate changes from workalendar v15.0.0 (2021-02-19)
 
 Major changes
 
 - API: New method available in `core` module: `Calendar.get_iso_week_date()` to find the weekday X of the week number Y (#619).
 - Requirements: Replace pytz with `(backports.)zoneinfo`, thx to @eumiro (#614)
@@ -119,15 +148,15 @@
 - Improve Netherlands coverage (#546, #619).
 - Improve Russia coverage (#546).
 - Improve USA calendar coverage by removing a method that wasn't used anyways (`get_washington_birthday_december()`). The method is implemented in both Indiana and Georgia State calendars, and is specific for each state, even if they look very similar (#546).
 - Improve the `astronomy.py` module coverage (#546).
 - Improve coverage for the `tests/__init__.py` module (#546). *Note:* system-dependant test branch (if Windows) won't be counted for coverage.
 
 v7.1.0
-------
+======
 
 Incorporate changes from workalendar v14.3.0 (2021-01-15)
 
 Calendars
 
 - Update Malaysia 2022-2024 (Deepavali + Thaipusam) by @jack-pace
 
@@ -143,15 +172,15 @@
 - Use f-string for string formatting, thx to @eumiro (#605)
 - Simplify collections handling, thx to @eumiro (#606)
 - Use integers for time units divisions, thx to @eumiro
 - Adding Mac OS & Windows tests to the test matrix (related to #607).
 - Fix tests when running them on Windows (#607).
 
 v7.0.0
-------
+======
 
 New feature
 
 - Enhanced support for multi-day "series" holidays such as Chinese Spring
   Festival and Islamic Eid. Previously, if one day of the series was shifted
   as per the observance shift rules, it would "merge" into the next day of the
   series, effectively shortening the observed series. Now, all the following
@@ -347,26 +376,26 @@
 - Fix several miscalculations in Georgia (USA) calendar (#451).
 
 Incorporate changes from workalendar v8.0.1 (2020-01-24)
 
 - Fix Family Day for British Columbia (Canada) which was switched from 2nd to 3rd Monday of February in 2019 - thx @jbroudou for the bug report (#454).
 
 v6.1.2
-------
+======
 
 #14: Replaced implicit dependency on setuptools with explicit
 dependency on importlib.metadata.
 
 v6.1.1
-------
+======
 
 Fix version inference when installed from sdist.
 
 v6.1.0
-------
+======
 
 Incorporate changes from workalendar v8.0.0 (2020-01-10)
 
 - **BREAKING CHANGE** Drop Support for Python 2 - EOL January 1st 2020 (#442).
 - Added Ukraine calendar, by @apelloni.
 - Small cleanup in the ``.travis.yml`` file, thx to @Natim.
 
@@ -409,20 +438,20 @@
 
 - Fixes and additions to some Brazil calendars ; again, thanks to @luismalta & @mileo, (#409 & #415)
 - Fix Denmark, re-add Christmas Eve, which is widely treated as public holiday ; thx to @KidkArolis, (#414).
 - Increase Malaysia coverage by adding tests for missing Deepavali & Thaipusam.
 - Increase China coverage by adding tests for special extra-holidays & extra-working days cases.
 
 v6.0.0
-------
+======
 
 Require Python 3.6 or later.
 
 v5.0.0
-------
+======
 
 #11: Add support for ``__add__`` and ``__sub__`` for
 ``Holiday`` instances on Python 3.8 and later. Now adding
 a timedelta to a ``Holiday`` returns another ``Holiday``.
 
 Incorporate changes from workalendar v7.0.0 (2019-09-20)
 
@@ -440,15 +469,15 @@
 - Added first day counting when computing working_days delta (#393), thx @Querdos.
 
 Incorporate changes from workalendar v5.2.3 (2019-07-11)
 - Fix Romania, make sure Easter and related holidays are calculated using the Orthodox calendar, thx to @KidkArolis (#389).
 
 
 v4.0.0
-------
+======
 
 Incorporate changes from workalendar v5.2.2. (2019-07-07)
 
 - **Deprecation Warning:** *Currently the registry returns `OrderedDict` objects when you're querying for regions or subregions. Expect that the next major release will preferrably return plain'ol' `dict` objects. If your scripts rely on the order of the objects returned, you'll have to sort them yourself.*
 - Fix Denmark, remove observances (remove Palm Sunday, Constitution Day, Christmas Eve and New Year's Eve) (#387, #386)
 
 Incorporate changes from workalendar v5.2.1 (2019-07-05)
@@ -579,15 +608,15 @@
 
     - Added New Zealand, by @johnguant (#306).
     - Added Paraguay calendar, following the work of @reichert (#268).
     - Added China calendar, by @iamsk (#304).
     - Added Israel, by @armona, @tsehori (#281).
 
 3.0
----
+===
 
 Incorporate changes from workalendar 3.2.1:
 
 - Added DEEPAVALI days for 2019 and 2020, thx @pvalenti (#282).
 - Fixed Germany Reformation Day miscalculation. Some German states include Reformation Day since the "beginning" ; in 2017, all states included Reformation Day as a holiday (500th anniversary of the Reformation) ; starting of 2018, 4 states added Reformation Day (#295).
 
 Incorporate changes from workalendar 3.2.0:
@@ -646,15 +675,15 @@
 - Fixing Federal Christmas Shift ; added a `include_veterans_day` flag to enable/disable Veteran's day on specific calendar - e.g. Mozilla's dedicated calendar (#242).
 - **Deprecation:** Dropped support for Python 3.3 (#245).
 - Fixed Travis-ci configuration for Python 3.5 and al (#252).
 - First step iteration on the "global registry" feature. European countries are now part of a registry loaded in the ``workalendar.registry`` module. Please use with care at the moment (#248).
 - Refactored Australia family and community day calculation (#244).
 
 2.0
----
+===
 
 Incorporate changes from workalendar 2.1.0:
 
 - Added Hong Kong, by @nedlowe (#235).
 - Splitted `africa.py` file into an `africa/` module (#236).
 - Added Alabama Counties - Baldwin County, Mobile County, Perry County. Refactored UnitedStates classes to have a parameter to include the "Mardi Gras" day (#214).
 - Added brazilian calendar to consider working days for bank transactions, by @fvlima (#238).
@@ -706,15 +735,15 @@
 - Add Croatia. thx @gregn610 (#157)
 
 Incorporate changes from workalendar 0.8.1:
 
 - Reformation Day is a national holiday in Germany, but only in 2017 (#150).
 
 1.8
----
+===
 
 Now tests are run using tox and releases are made automatically
 using Travis-CI deployment framework.
 
 Incorporate changes from workalendar 0.8.0:
 
 - Fix Czech Republic calendar - as of 2016, Good Friday has become a holiday (#148).
@@ -732,40 +761,40 @@
 - Added Estonia, thx to @landler (#134),
 - Europe-related modules being reorganized, thx to @Natim (#135),
 - Fixed King / Queen's day in Netherlands, thx to @PeterJacob (#138),
 - Added a pull-request template (#125),
 - Added a Makefile for various dev-related tasks -- installs, running tests, uploading to PyPI... (#133).
 
 1.7.1
------
+=====
 
 - #7: Avoid crashing on import when installed as zip package.
 
 1.7
----
+===
 
 Incorporate changes from workalendar 0.5.0:
 
 - A new holiday has appeared in Japan as of 2016 (#131), thx @suhara for the report.
 
 Incorporate changes from workalendar 0.4.5:
 
 - Added Slovenia, thx to @ratek1 (#124).
 - Added Switzerland, thx to @sykaeh (#127).
 
 1.6
----
+===
 
 - #6: Remove observance shift for Sweden.
 - Use `jaraco skeleton <https://github.com/jaraco/skeleton>`_ to
   maintain the project structure, adding automatic releases
   from continuous integration and bundled documentation.
 
 1.5
----
+===
 
 Incorporate changes from workalendar 0.4.3:
 
 - Added Denmark (#117).
 - Tiny fixes in the ``usa.py`` module (flake8 + typo) (#122)
 - Added datetime to date conversion in is_holiday() (#118)
 - Added function to get the holiday label by date (#120)
@@ -786,71 +815,71 @@
 Incorporate changes from workalendar 0.4.0:
 
 - Added Colombia calendar, thx to @spalac24
 - Added Slovakia calendar, thx to @Adman
 - Fixed the Boxing day & boxing day shift for Australia
 
 1.4
----
+===
 
 ``Calendar.get_observed_date`` now allows ``observance_shift`` to be
 a callable accepting the holiday and calendar and returning the observed
 date. ``Holiday`` supplies a ``get_nearest_weekday`` method suitable for
 locating the nearest weekday.
 
 - #5: USA Independence Day now honors the nearest weekday model.
 
 1.3
----
+===
 
 Incorporate these fixes from Workalendar 0.3:
 
 - ``delta`` argument for ``add_working_days()`` can be negative. added a
   ``sub_working_days()`` method that computes working days backwards.
 - BUGFIX: Renaming Showa Day. "ō is not romji" (#100) (thx @shinriyo)
 - BUGFIX: Belgian National Day title (#99) (thx @laulaz)
 
 1.2.1
------
+=====
 
 Correct usage in example.
 
 1.2
----
+===
 
 Fixed issue #4 where Finland holidays were shifted but shouldn't have been.
 Calendars and Holidays may now specify observance_shift=None to signal no
 shift.
 
 Package can now be tested with pytest-runner by invoking ``python setup.py
 pytest``.
 
 1.1.3
------
+=====
 
 Fix name of Finnish Independence Day.
 
 1.1.2
------
+=====
 
 Fixed issues with packaging (disabled installation an zip egg and now use
 setuptools always).
 
 1.1
----
+===
 
 UnitedKingdom Calendar now uses indicated/observed Holidays.
 
 Includes these changes slated for workalendar 0.3:
 
 - BUGFIX: shifting UK boxing day if Christmas day falls on a Friday (shift to
   next Monday) (#95)
 
 1.0
----
+===
 
 Initial release of Calendra based on Workalendar 0.2.
 
 - Adds Holiday class per (#79). Adds support for giving
   holidays a more rich description and better resolution of observed versus
   indicated holidays. See the pull request for detail on the motivation and
   implementation. See the usa.UnitedStates calendar for example usage.
```

### Comparing `calendra-7.6.1/LICENSE` & `calendra-7.7.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `calendra-7.6.1/PKG-INFO` & `calendra-7.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: calendra
-Version: 7.6.1
+Version: 7.7.0
 Summary: Worldwide holidays and working days helper and toolkit.
 Home-page: https://github.com/jaraco/calendra
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: docs
 Provides-Extra: astronomy
 License-File: LICENSE
 
-[![](https://img.shields.io/pypi/v/calendra.svg)][1]
+[![](https://img.shields.io/pypi/v/calendra.svg)][https://pypi.org/project/calendra]
 
-[![](https://img.shields.io/pypi/pyversions/calendra.svg)][1]
+![](https://img.shields.io/pypi/pyversions/calendra.svg)
 
-  [1]: https://pypi.org/project/calendra
+[![tests](https://github.com/jaraco/calendra/workflows/Automated%20Tests/badge.svg)](https://github.com/jaraco/calendra/actions?query=workflow%3A%22Automated+Tests%22)
 
-[![Automated Tests](https://github.com/jaraco/calendra/workflows/Automated%20Tests/badge.svg)](https://github.com/jaraco/calendra/actions?query=workflow%3A%22Automated+Tests%22)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+
+[![Code style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![](https://readthedocs.org/projects/calendra/badge/?version=latest)](https://calendra.readthedocs.io/en/latest/?badge=latest)
 
-[![license](http://img.shields.io/pypi/l/workalendar.svg)](https://github.com/workalendar/workalendar/blob/master/LICENSE)
-[![pypi](http://img.shields.io/pypi/v/workalendar.svg)](https://pypi.python.org/pypi/workalendar)
-[![conda](https://img.shields.io/conda/v/conda-forge/workalendar?color=blue&logo=anaconda)](https://anaconda.org/conda-forge/workalendar)
+[![](https://img.shields.io/badge/skeleton-2023-informational)][https://blog.jaraco.com/skeleton]
+
 
 ## Overview
 
 Calendra is a Python module that offers classes able to handle calendars, list legal / religious holidays and gives working-day-related computation functions.
 
 ## History
 
@@ -148,14 +149,15 @@
 
 - Argentina
 - Barbados
 - Brazil (all states, cities and for bank transactions, except the city of Viana)
 - Canada (including provincial and territory holidays)
 - Chile
 - Colombia
+- El Salvador
 - Mexico
 - Panama
 - Paraguay
 - United States of America
   - State holidays for all the 50 States
   - American Samoa
   - Chicago, Illinois
@@ -194,14 +196,15 @@
 - Ivory Coast
 - Kenya
 - Madagascar
 - Mozambique
 - Nigeria
 - São Tomé
 - South Africa
+- Tunisia
 
 And more to come (I hope!)
 
 ## Caveats
 
 Please take note that some calendars are not 100% accurate. The most common example is the Islamic calendar, where some computed holidays are not exactly on the same official day decided by religious authorities, and this may vary country by country. Whenever it's possible, try to adjust your results with the official data provided by the adequate authorities.
```

### Comparing `calendra-7.6.1/README.md` & `calendra-7.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-[![](https://img.shields.io/pypi/v/calendra.svg)][1]
+[![](https://img.shields.io/pypi/v/calendra.svg)][https://pypi.org/project/calendra]
 
-[![](https://img.shields.io/pypi/pyversions/calendra.svg)][1]
+![](https://img.shields.io/pypi/pyversions/calendra.svg)
 
-  [1]: https://pypi.org/project/calendra
+[![tests](https://github.com/jaraco/calendra/workflows/Automated%20Tests/badge.svg)](https://github.com/jaraco/calendra/actions?query=workflow%3A%22Automated+Tests%22)
 
-[![Automated Tests](https://github.com/jaraco/calendra/workflows/Automated%20Tests/badge.svg)](https://github.com/jaraco/calendra/actions?query=workflow%3A%22Automated+Tests%22)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+
+[![Code style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![](https://readthedocs.org/projects/calendra/badge/?version=latest)](https://calendra.readthedocs.io/en/latest/?badge=latest)
 
-[![license](http://img.shields.io/pypi/l/workalendar.svg)](https://github.com/workalendar/workalendar/blob/master/LICENSE)
-[![pypi](http://img.shields.io/pypi/v/workalendar.svg)](https://pypi.python.org/pypi/workalendar)
-[![conda](https://img.shields.io/conda/v/conda-forge/workalendar?color=blue&logo=anaconda)](https://anaconda.org/conda-forge/workalendar)
+[![](https://img.shields.io/badge/skeleton-2023-informational)][https://blog.jaraco.com/skeleton]
+
 
 ## Overview
 
 Calendra is a Python module that offers classes able to handle calendars, list legal / religious holidays and gives working-day-related computation functions.
 
 ## History
 
@@ -129,14 +130,15 @@
 
 - Argentina
 - Barbados
 - Brazil (all states, cities and for bank transactions, except the city of Viana)
 - Canada (including provincial and territory holidays)
 - Chile
 - Colombia
+- El Salvador
 - Mexico
 - Panama
 - Paraguay
 - United States of America
   - State holidays for all the 50 States
   - American Samoa
   - Chicago, Illinois
@@ -175,14 +177,15 @@
 - Ivory Coast
 - Kenya
 - Madagascar
 - Mozambique
 - Nigeria
 - São Tomé
 - South Africa
+- Tunisia
 
 And more to come (I hope!)
 
 ## Caveats
 
 Please take note that some calendars are not 100% accurate. The most common example is the Islamic calendar, where some computed holidays are not exactly on the same official day decided by religious authorities, and this may vary country by country. Whenever it's possible, try to adjust your results with the official data provided by the adequate authorities.
```

### Comparing `calendra-7.6.1/calendra/africa/algeria.py` & `calendra-7.7.0/calendra/africa/algeria.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/africa/angola.py` & `calendra-7.7.0/calendra/africa/angola.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/africa/benin.py` & `calendra-7.7.0/calendra/africa/benin.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/africa/ivory_coast.py` & `calendra-7.7.0/calendra/africa/ivory_coast.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/africa/kenya.py` & `calendra-7.7.0/calendra/africa/kenya.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/africa/madagascar.py` & `calendra-7.7.0/calendra/africa/madagascar.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/africa/mozambique.py` & `calendra-7.7.0/calendra/africa/mozambique.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/africa/nigeria.py` & `calendra-7.7.0/calendra/africa/nigeria.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/africa/sao_tome.py` & `calendra-7.7.0/calendra/africa/sao_tome.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/africa/south_africa.py` & `calendra-7.7.0/calendra/africa/south_africa.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/america/__init__.py` & `calendra-7.7.0/calendra/america/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 )
 from .chile import Chile
 from .colombia import Colombia
 from .mexico import Mexico
 from .panama import Panama
 from .paraguay import Paraguay
 from .argentina import Argentina
+from .el_salvador import ElSalvador
 
 
 __all__ = (
     # Brazil & its states.
     'Brazil',
     'BrazilAcre',
     'BrazilAlagoas',
@@ -112,8 +113,9 @@
     'Barbados',
     'Chile',
     'Colombia',
     'Mexico',
     'Panama',
     'Paraguay',
     'Argentina',
+    'ElSalvador',
 )
```

### Comparing `calendra-7.6.1/calendra/america/argentina.py` & `calendra-7.7.0/calendra/america/argentina.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/america/barbados.py` & `calendra-7.7.0/calendra/america/barbados.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/america/brazil.py` & `calendra-7.7.0/calendra/america/brazil.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/america/canada.py` & `calendra-7.7.0/calendra/america/canada.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/america/chile.py` & `calendra-7.7.0/calendra/america/chile.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/america/colombia.py` & `calendra-7.7.0/calendra/america/colombia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/america/mexico.py` & `calendra-7.7.0/calendra/america/mexico.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/america/panama.py` & `calendra-7.7.0/calendra/america/panama.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/america/paraguay.py` & `calendra-7.7.0/calendra/america/paraguay.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/asia/__init__.py` & `calendra-7.7.0/calendra/asia/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/asia/china.py` & `calendra-7.7.0/calendra/asia/china.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,14 +38,22 @@
     2022:
         {
             'Ching Ming Festival': [(4, 3), (4, 4), (4, 5)],
             'Labour Day Holiday': [(4, 30), (5, 1), (5, 2), (5, 3), (5, 4)],
             'Dragon Boat Festival': [(6, 3), (6, 4), (6, 5)],
             'Mid-Autumn Festival': [(9, 10), (9, 11), (9, 12)]
         },
+    2023:
+        {
+            'Ching Ming Festival': [(4, 5)],
+            'Labour Day Holiday': [(4, 29), (4, 30), (5, 1), (5, 2), (5, 3)],
+            'Dragon Boat Festival': [(6, 22), (6, 23), (6, 24)],
+            'Mid-Autumn Festival': [(9, 29)],
+            'National Day': [(9, 30)]
+        },
 }
 
 workdays = {
     2018:
         {
             'Spring Festival Shift': [(2, 11), (2, 24)],
             'Ching Ming Festival Shift': [(4, 8)],
@@ -76,26 +84,29 @@
     2022:
         {
             'Spring Festival Shift': [(1, 29), (1, 30)],
             'Ching Ming Festival Shift': [(4, 2)],
             'Labour Day Holiday Shift': [(4, 24), (5, 7)],
             'National Day Shift': [(10, 8), (10, 9)]
         },
+    2023:
+        {
+            'Spring Festival Shift': [(1, 28), (1, 29)],
+            'Labour Day Holiday Shift': [(4, 23), (5, 6)],
+            'Dragon Boat Festival Shift': [(6, 25)],
+            'National Day Shift': [(10, 7), (10, 8)]
+        },
 }
 
 
 @iso_register('CN')
 class China(ChineseNewYearCalendar):
     "China"
-    # WARNING: Support 2018-2022 currently, need update every year.
+    # WARNING: Support 2018-2023 currently, need update every year.
     shift_new_years_day = True
-    # National Days, 10.1 - 10.7
-    national_days = [(10, i, "National Day") for i in range(1, 8)]
-    FIXED_HOLIDAYS = tuple(national_days)
-
     include_chinese_new_year_eve = True
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.extra_working_days = []
         for year, data in workdays.items():
             for holiday_name, day_list in data.items():
@@ -115,14 +126,19 @@
 
     def get_variable_days(self, year):
         days = super().get_variable_days(year)
         # Spring Festival, eve, 1.1, and 1.2 - 1.6 in lunar day
         for i in range(2, 7):
             days.append((ChineseNewYearCalendar.lunar(year, 1, i),
                          "Spring Festival"))
+        # National Days, 10.1 - 10.7 in general
+        for i in range(1, 8):
+            if date(year, 10, i) not in self.extra_working_days:
+                days.append((date(year, 10, i), "National Day"))
+
         # other holidays
         for holiday_name, day_list in holidays[year].items():
             for v in day_list:
                 days.append((date(year, v[0], v[1]), holiday_name))
         return days
 
     def is_working_day(self, day,
```

### Comparing `calendra-7.6.1/calendra/asia/hong_kong.py` & `calendra-7.7.0/calendra/asia/hong_kong.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/asia/israel.py` & `calendra-7.7.0/calendra/asia/israel.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/asia/japan.py` & `calendra-7.7.0/calendra/asia/japan.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/asia/kazakhstan.py` & `calendra-7.7.0/calendra/asia/kazakhstan.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/asia/malaysia.py` & `calendra-7.7.0/calendra/asia/malaysia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/asia/philippines.py` & `calendra-7.7.0/calendra/asia/philippines.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/asia/singapore.py` & `calendra-7.7.0/calendra/asia/singapore.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/asia/south_korea.py` & `calendra-7.7.0/calendra/asia/south_korea.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/asia/taiwan.py` & `calendra-7.7.0/calendra/asia/taiwan.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/core.py` & `calendra-7.7.0/calendra/core.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/equinoxes.json.gz` & `calendra-7.7.0/calendra/equinoxes.json.gz`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/__init__.py` & `calendra-7.7.0/calendra/europe/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/austria.py` & `calendra-7.7.0/calendra/europe/austria.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/belarus.py` & `calendra-7.7.0/calendra/europe/belarus.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/bulgaria.py` & `calendra-7.7.0/calendra/europe/bulgaria.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/cayman_islands.py` & `calendra-7.7.0/calendra/europe/cayman_islands.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/croatia.py` & `calendra-7.7.0/calendra/europe/croatia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/cyprus.py` & `calendra-7.7.0/calendra/europe/cyprus.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/czech_republic.py` & `calendra-7.7.0/calendra/europe/czech_republic.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/denmark.py` & `calendra-7.7.0/calendra/europe/denmark.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/estonia.py` & `calendra-7.7.0/calendra/europe/estonia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/finland.py` & `calendra-7.7.0/calendra/europe/finland.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/france.py` & `calendra-7.7.0/calendra/europe/france.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/georgia.py` & `calendra-7.7.0/calendra/europe/georgia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/germany.py` & `calendra-7.7.0/calendra/europe/germany.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/greece.py` & `calendra-7.7.0/calendra/europe/greece.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/guernsey.py` & `calendra-7.7.0/calendra/europe/guernsey.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/hungary.py` & `calendra-7.7.0/calendra/europe/hungary.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/iceland.py` & `calendra-7.7.0/calendra/europe/iceland.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/ireland.py` & `calendra-7.7.0/calendra/europe/ireland.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/italy.py` & `calendra-7.7.0/calendra/europe/italy.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/latvia.py` & `calendra-7.7.0/calendra/europe/latvia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/lithuania.py` & `calendra-7.7.0/calendra/europe/lithuania.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/luxembourg.py` & `calendra-7.7.0/calendra/europe/luxembourg.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/malta.py` & `calendra-7.7.0/calendra/europe/malta.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/monaco.py` & `calendra-7.7.0/calendra/europe/monaco.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/netherlands.py` & `calendra-7.7.0/calendra/europe/netherlands.py`

 * *Files 4% similar despite different names*

```diff
@@ -157,40 +157,38 @@
         if self.region in FALL_HOLIDAYS_EARLY_REGIONS[year]:
             start = start - timedelta(weeks=1)
 
         return [
             (start + timedelta(days=i), "Fall holiday") for i in range(n_days)
         ]
 
-    def get_christmas_holidays(self, year, in_december=True, in_january=True):
+    def get_christmas_holidays(self, year):
         """
         Return Christmas holidays
 
         Christmas holidays run partially in December and partially in January
         (spillover from previous year).
         """
+        return (
+            self._get_christmas_holidays_december(year) +
+            self._get_christmas_holidays_january(year)
+        )
 
-        if in_december:
-
-            # 27 December is always in a full week of holidays
-            week = date(year, 12, 27).isocalendar()[1]
+    def _get_christmas_holidays_december(self, year):
+        # 27 December is always in a full week of holidays
+        week = date(year, 12, 27).isocalendar()[1]
 
-            # Holiday starts on the preceding Saturday
-            start = self.get_iso_week_date(year, week - 1, ISO_SAT)
-            dates = [
-                (start + timedelta(days=i), "Christmas holiday")
-                for i in range((date(year, 12, 31) - start).days + 1)
-            ]
-
-            if in_january:
-                dates.extend(
-                    self.get_christmas_holidays(year, in_december=False)
-                )
-            return dates
+        # Holiday starts on the preceding Saturday
+        start = self.get_iso_week_date(year, week - 1, ISO_SAT)
+        return [
+            (start + timedelta(days=i), "Christmas holiday")
+            for i in range((date(year, 12, 31) - start).days + 1)
+        ]
 
+    def _get_christmas_holidays_january(self, year):
         # 27 December is always in a full week of holidays
         week = date(year - 1, 12, 27).isocalendar()[1]
 
         # Holiday ends 15 days after the preceding Saturday
         # Saturday of the previous week (previous year!)
         start = self.get_iso_week_date(year - 1, week - 1, ISO_SAT)
         end = start + timedelta(days=15)
```

### Comparing `calendra-7.6.1/calendra/europe/norway.py` & `calendra-7.7.0/calendra/europe/norway.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/poland.py` & `calendra-7.7.0/calendra/europe/poland.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/portugal.py` & `calendra-7.7.0/calendra/europe/portugal.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/romania.py` & `calendra-7.7.0/calendra/europe/romania.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/russia.py` & `calendra-7.7.0/calendra/europe/russia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/scotland/__init__.py` & `calendra-7.7.0/calendra/europe/scotland/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/scotland/mixins/__init__.py` & `calendra-7.7.0/calendra/europe/scotland/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/scotland/mixins/autumn_holiday.py` & `calendra-7.7.0/calendra/europe/scotland/mixins/autumn_holiday.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/scotland/mixins/fair_holiday.py` & `calendra-7.7.0/calendra/europe/scotland/mixins/fair_holiday.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/scotland/mixins/spring_holiday.py` & `calendra-7.7.0/calendra/europe/scotland/mixins/spring_holiday.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/scotland/mixins/victoria_day.py` & `calendra-7.7.0/calendra/europe/scotland/mixins/victoria_day.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/serbia.py` & `calendra-7.7.0/calendra/europe/serbia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/slovakia.py` & `calendra-7.7.0/calendra/europe/slovakia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/slovenia.py` & `calendra-7.7.0/calendra/europe/slovenia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/spain.py` & `calendra-7.7.0/calendra/europe/spain.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/sweden.py` & `calendra-7.7.0/calendra/europe/sweden.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/switzerland.py` & `calendra-7.7.0/calendra/europe/switzerland.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/turkey.py` & `calendra-7.7.0/calendra/europe/turkey.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/ukraine.py` & `calendra-7.7.0/calendra/europe/ukraine.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/europe/united_kingdom.py` & `calendra-7.7.0/calendra/europe/united_kingdom.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
         1973: [(date(1973, 11, 14), "Royal wedding"), ],
         1977: [(date(1977, 6, 7), "Queen’s Silver Jubilee"), ],
         1981: [(date(1981, 7, 29), "Royal wedding"), ],
         1999: [(date(1999, 12, 31), "New Year's Eve"), ],
         2002: [(date(2002, 6, 3), "Queen’s Golden Jubilee"), ],
         2011: [(date(2011, 4, 29), "Royal Wedding"), ],
         2012: [(date(2012, 6, 5), "Queen’s Diamond Jubilee"), ],
-        2022: [(date(2022, 6, 3), "Queen’s Platinum Jubilee bank holiday"), ],
+        2022: [(date(2022, 6, 3), "Queen’s Platinum Jubilee bank holiday"),
+               (date(2022, 9, 19), "State Funeral of Queen Elizabeth II"), ],
     }
 
     def get_early_may_bank_holiday(self, year):
         """
         Return Early May bank holiday
         """
         day = date(year, 5, 1) + rd.relativedelta(weekday=rd.MO(1))
```

### Comparing `calendra-7.6.1/calendra/exceptions.py` & `calendra-7.7.0/calendra/exceptions.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/holiday.py` & `calendra-7.7.0/calendra/holiday.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/oceania/__init__.py` & `calendra-7.7.0/calendra/oceania/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/oceania/australia.py` & `calendra-7.7.0/calendra/oceania/australia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/oceania/marshall_islands.py` & `calendra-7.7.0/calendra/oceania/marshall_islands.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/oceania/new_zealand.py` & `calendra-7.7.0/calendra/oceania/new_zealand.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/precomputed_astronomy.py` & `calendra-7.7.0/calendra/precomputed_astronomy.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/registry.py` & `calendra-7.7.0/calendra/registry.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/registry_tools.py` & `calendra-7.7.0/calendra/registry_tools.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/skyfield_astronomy.py` & `calendra-7.7.0/calendra/skyfield_astronomy.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/solar_terms.json.gz` & `calendra-7.7.0/calendra/solar_terms.json.gz`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/__init__.py` & `calendra-7.7.0/calendra/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_africa.py` & `calendra-7.7.0/calendra/tests/test_africa.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,53 @@
     Benin,
     IvoryCoast,
     Kenya,
     Madagascar,
     Nigeria,
     SaoTomeAndPrincipe,
     SouthAfrica,
+    Tunisia,
 )
 from ..core import MON, FRI
 from ..exceptions import CalendarError
 
 
+class TunisiaTest(GenericCalendarTest):
+    cal_class = Tunisia
+
+    def test_year_2013(self):
+        holidays = self.cal.holidays_set(2013)
+        self.assertIn(date(2013, 3, 20), holidays)  # Independance Day
+        self.assertIn(date(2013, 7, 25), holidays)  # Republic Day
+        self.assertIn(date(2013, 1, 24), holidays)   # Milad un Nabi
+        self.assertIn(date(2013, 8, 8), holidays)  # Eid ul-fitr
+        self.assertIn(date(2013, 8, 9), holidays)  # Eid ul-fitr next day
+        self.assertIn(date(2013, 10, 15), holidays)  # Evacuation Day
+
+    def test_year_2022(self):
+        holidays = self.cal.holidays_set(2022)
+        self.assertIn(date(2022, 3, 20), holidays)  # Independance Day
+        self.assertIn(date(2022, 7, 25), holidays)  # Republic Day
+        self.assertIn(date(2022, 10, 8), holidays)   # Milad un Nabi
+        self.assertIn(date(2022, 5, 3), holidays)  # Eid ul-fitr
+        self.assertIn(date(2022, 5, 4), holidays)  # Eid ul-fitr next day
+        self.assertIn(date(2022, 10, 15), holidays)  # Evacuation Day
+
+    def test_revolution_day(self):
+        holidays = self.cal.holidays_set(2013)
+        self.assertNotIn(date(2013, 12, 17), holidays)  # Revolution Day
+        self.assertIn(date(2013, 1, 14), holidays)  # Revolution Day
+        holidays = self.cal.holidays_set(2022)
+        self.assertIn(date(2022, 12, 17), holidays)  # Revolution Day
+        self.assertNotIn(date(2022, 1, 14), holidays)  # Revolution Day
+        holidays = self.cal.holidays_set(2010)
+        self.assertNotIn(date(2010, 12, 17), holidays)  # Revolution Day
+        self.assertNotIn(date(2010, 1, 14), holidays)  # Revolution Day
+
+
 class AlgeriaTest(GenericCalendarTest):
     cal_class = Algeria
 
     def test_year_2013(self):
         holidays = self.cal.holidays_set(2013)
         self.assertIn(date(2013, 1, 1), holidays)  # New year
         self.assertIn(date(2013, 1, 24), holidays)   # Milad un Nabi
```

### Comparing `calendra-7.6.1/calendra/tests/test_america.py` & `calendra-7.7.0/calendra/tests/test_america.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 from datetime import date
 
-from ..america import (Argentina, Barbados, Chile, Colombia, Mexico, Panama,
-                       Paraguay)
+from ..america import (
+        Argentina,
+        Barbados,
+        Chile,
+        Colombia,
+        ElSalvador,
+        Mexico,
+        Panama,
+        Paraguay
+    )
 from . import GenericCalendarTest
 
 
 class ArgentinaTest(GenericCalendarTest):
     cal_class = Argentina
 
     def test_holidays_2018(self):
@@ -612,7 +620,71 @@
         self.assertIn(date(2021, 5, 1), holidays)  # Labour Day
         self.assertIn(date(2021, 5, 24), holidays)  # Whit Monday
         self.assertIn(date(2021, 8, 2), holidays)  # Kabooment Day
         self.assertIn(date(2021, 8, 3), holidays)  # Emancipation Day
         self.assertIn(date(2021, 11, 30), holidays)  # Independant Day
         self.assertIn(date(2021, 12, 25), holidays)  # Christmas Day
         self.assertIn(date(2021, 12, 27), holidays)  # Boxing Day
+
+
+class ElSalvadorTest(GenericCalendarTest):
+    cal_class = ElSalvador
+
+    def test_holidays_2018(self):
+        holidays = self.cal.holidays_set(2018)
+        self.assertIn(date(2018, 1, 1), holidays)   # New Year's Day
+        self.assertIn(date(2018, 3, 29), holidays)  # Maundy Thursday
+        self.assertIn(date(2018, 3, 30), holidays)  # Good Friday
+        self.assertIn(date(2018, 3, 31), holidays)  # Holy Saturday
+        self.assertIn(date(2018, 5, 1), holidays)   # Labor Day
+        self.assertIn(date(2018, 5, 10), holidays)  # Mothers' Day
+        self.assertIn(date(2018, 6, 17), holidays)  # Fathers' Day
+        # Celebrations of San Salvador
+        self.assertIn(date(2018, 8, 6), holidays)
+        self.assertIn(date(2018, 9, 15), holidays)  # Independence Day
+        self.assertIn(date(2018, 11, 2), holidays)  # All Saints Day
+        self.assertIn(date(2018, 12, 25), holidays)  # XMas
+
+    def test_holidays_2019(self):
+        holidays = self.cal.holidays_set(2019)
+        self.assertIn(date(2019, 1, 1), holidays)   # New Year's Day
+        self.assertIn(date(2019, 4, 18), holidays)  # Maundy Thursday
+        self.assertIn(date(2019, 4, 19), holidays)  # Good Friday
+        self.assertIn(date(2019, 4, 20), holidays)  # Holy Saturday
+        self.assertIn(date(2019, 5, 1), holidays)   # Labor Day
+        self.assertIn(date(2019, 5, 10), holidays)  # Mothers' Day
+        self.assertIn(date(2019, 6, 17), holidays)  # Fathers' Day
+        # Celebrations of San Salvador
+        self.assertIn(date(2019, 8, 6), holidays)
+        self.assertIn(date(2019, 9, 15), holidays)  # Independence Day
+        self.assertIn(date(2019, 11, 2), holidays)  # All Saints Day
+        self.assertIn(date(2019, 12, 25), holidays)  # XMas
+
+    def test_holidays_2020(self):
+        holidays = self.cal.holidays_set(2020)
+        self.assertIn(date(2020, 1, 1), holidays)   # New Year's Day
+        self.assertIn(date(2020, 4, 9), holidays)   # Maundy Thursday
+        self.assertIn(date(2020, 4, 10), holidays)  # Good Friday
+        self.assertIn(date(2020, 4, 11), holidays)  # Holy Saturday
+        self.assertIn(date(2020, 5, 1), holidays)   # Labor Day
+        self.assertIn(date(2020, 5, 10), holidays)  # Mothers' Day
+        self.assertIn(date(2020, 6, 17), holidays)  # Fathers' Day
+        # Celebrations of San Salvador
+        self.assertIn(date(2020, 8, 6), holidays)
+        self.assertIn(date(2020, 9, 15), holidays)  # Independence Day
+        self.assertIn(date(2020, 11, 2), holidays)  # All Saints Day
+        self.assertIn(date(2020, 12, 25), holidays)  # XMas
+
+    def test_holidays_2021(self):
+        holidays = self.cal.holidays_set(2021)
+        self.assertIn(date(2021, 1, 1), holidays)   # New Year's Day
+        self.assertIn(date(2021, 4, 2), holidays)   # Maundy Thursday
+        self.assertIn(date(2021, 4, 2), holidays)   # Good Friday
+        self.assertIn(date(2021, 4, 3), holidays)   # Holy Saturday
+        self.assertIn(date(2021, 5, 1), holidays)   # Labor Day
+        self.assertIn(date(2021, 5, 10), holidays)  # Mothers' Day
+        self.assertIn(date(2021, 6, 17), holidays)  # Fathers' Day
+        # Celebrations of San Salvador
+        self.assertIn(date(2021, 8, 6), holidays)
+        self.assertIn(date(2021, 9, 15), holidays)  # Independence Day
+        self.assertIn(date(2021, 11, 2), holidays)  # All Saints Day
+        self.assertIn(date(2021, 12, 25), holidays)  # XMas
```

### Comparing `calendra-7.6.1/calendra/tests/test_asia.py` & `calendra-7.7.0/calendra/tests/test_asia.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,27 +109,48 @@
         # Ching Ming Festival Shift
         self.assertNotIn(date(2022, 4, 2), holidays)
         self.assertNotIn(date(2022, 4, 24), holidays)  # Labour Day Shift
         self.assertNotIn(date(2022, 5, 7), holidays)  # Labour Day Shift
         self.assertNotIn(date(2022, 10, 8), holidays)  # National Day Shift
         self.assertNotIn(date(2022, 10, 9), holidays)  # National Day Shift
 
+    def test_year_2023(self):
+        holidays = self.cal.holidays_set(2023)
+        self.assertIn(date(2023, 1, 2), holidays)       # New Year
+        self.assertIn(date(2023, 1, 21), holidays)      # Spring Festival
+        self.assertIn(date(2023, 1, 27), holidays)      # Spring Festival
+        self.assertIn(date(2023, 4, 5), holidays)       # Ching Ming Festival
+        self.assertIn(date(2023, 4, 29), holidays)      # Labour Day Holiday
+        self.assertIn(date(2023, 5, 3), holidays)       # Labour Day Holiday
+        self.assertIn(date(2023, 6, 22), holidays)      # Dragon Boat Festival
+        self.assertIn(date(2023, 6, 24), holidays)      # Dragon Boat Festival
+        self.assertIn(date(2023, 9, 29), holidays)      # Mid-Autumn Festival
+        self.assertIn(date(2023, 9, 30), holidays)      # National Day
+        self.assertIn(date(2023, 10, 6), holidays)      # National Day
+
+        self.assertNotIn(date(2023, 1, 28), holidays)   # Spring Festival Shift
+        self.assertNotIn(date(2023, 1, 29), holidays)   # Spring Festival Shift
+        self.assertNotIn(date(2023, 4, 23), holidays)   # Labour Day Shift
+        self.assertNotIn(date(2023, 5, 6), holidays)    # Labour Day Shift
+        self.assertNotIn(date(2023, 10, 7), holidays)   # National Day Shift
+        self.assertNotIn(date(2023, 10, 8), holidays)   # National Day Shift
+
     def test_missing_holiday_year(self):
         save_2018 = china_holidays[2018]
         del china_holidays[2018]
         with self.assertRaises(CalendarError):
             self.cal.holidays_set(2018)
         china_holidays[2018] = save_2018
 
     def test_warning(self):
         year = date.today().year
         with patch('warnings.warn') as patched:
             self.cal.get_calendar_holidays(year)
         patched.assert_called_with(
-            'Support years 2018-2022 currently, need update every year.'
+            'Support years 2018-2023 currently, need update every year.'
         )
 
     def test_is_working_day(self):
         # It's a SAT, but it's a working day this year
         self.assertTrue(self.cal.is_working_day(date(2019, 2, 2)))
         # It's a SUN, but it's a working day this year
         self.assertTrue(self.cal.is_working_day(date(2019, 2, 3)))
```

### Comparing `calendra-7.6.1/calendra/tests/test_astronomy.py` & `calendra-7.7.0/calendra/tests/test_astronomy.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_brazil.py` & `calendra-7.7.0/calendra/tests/test_brazil.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_canada.py` & `calendra-7.7.0/calendra/tests/test_canada.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_core.py` & `calendra-7.7.0/calendra/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_europe.py` & `calendra-7.7.0/calendra/tests/test_europe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1976,14 +1976,18 @@
         self.assertNotIn(date(2022, 5, 30), holidays)  # Spring Bank Holiday
         self.assertIn(date(2022, 6, 2), holidays)  # Spring Bank Holiday
         # Platinum Jubilee Bank Holiday
         self.assertIn(date(2022, 6, 3), holidays)
         self.assertIn(date(2022, 8, 29), holidays)  # Summer bank holiday
         self.assertIn(date(2022, 12, 26), observed)  # Boxing Day
         self.assertIn(date(2022, 12, 27), observed)  # Christmas Day
+        # State Funeral of Queen Elizabeth II
+        self.assertIn(date(2022, 9, 19), holidays)
+        self.assertIn(date(2022, 12, 26), observed)  # Boxing Day
+        self.assertIn(date(2022, 12, 27), observed)  # Christmas Day
 
 
 class UnitedKingdomNorthernIrelandTest(UnitedKingdomTest):
     cal_class = UnitedKingdomNorthernIreland
 
     def test_regional_2013(self):
         holidays = self.cal.holidays_set(2013)
```

### Comparing `calendra-7.6.1/calendra/tests/test_germany.py` & `calendra-7.7.0/calendra/tests/test_germany.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_ical_export.py` & `calendra-7.7.0/calendra/tests/test_ical_export.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_mozambique.py` & `calendra-7.7.0/calendra/tests/test_mozambique.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_oceania.py` & `calendra-7.7.0/calendra/tests/test_oceania.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_precomputed_astronomy.py` & `calendra-7.7.0/calendra/tests/test_precomputed_astronomy.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_registry.py` & `calendra-7.7.0/calendra/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_registry_africa.py` & `calendra-7.7.0/calendra/tests/test_registry_africa.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_registry_america.py` & `calendra-7.7.0/calendra/tests/test_registry_america.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_registry_asia.py` & `calendra-7.7.0/calendra/tests/test_registry_asia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_registry_europe.py` & `calendra-7.7.0/calendra/tests/test_registry_europe.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_registry_oceania.py` & `calendra-7.7.0/calendra/tests/test_registry_oceania.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_registry_usa.py` & `calendra-7.7.0/calendra/tests/test_registry_usa.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_scotland.py` & `calendra-7.7.0/calendra/tests/test_scotland.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_skyfield_astronomy.py` & `calendra-7.7.0/calendra/tests/test_skyfield_astronomy.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_spain.py` & `calendra-7.7.0/calendra/tests/test_spain.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_switzerland.py` & `calendra-7.7.0/calendra/tests/test_switzerland.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_turkey.py` & `calendra-7.7.0/calendra/tests/test_turkey.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/tests/test_usa.py` & `calendra-7.7.0/calendra/tests/test_usa.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/__init__.py` & `calendra-7.7.0/calendra/usa/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/alabama.py` & `calendra-7.7.0/calendra/usa/alabama.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/alaska.py` & `calendra-7.7.0/calendra/usa/alaska.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/american_samoa.py` & `calendra-7.7.0/calendra/usa/american_samoa.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/california.py` & `calendra-7.7.0/calendra/usa/california.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/core.py` & `calendra-7.7.0/calendra/usa/core.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/florida.py` & `calendra-7.7.0/calendra/usa/florida.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/georgia.py` & `calendra-7.7.0/calendra/usa/georgia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/hawaii.py` & `calendra-7.7.0/calendra/usa/hawaii.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/illinois.py` & `calendra-7.7.0/calendra/usa/illinois.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/indiana.py` & `calendra-7.7.0/calendra/usa/indiana.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/kansas.py` & `calendra-7.7.0/calendra/usa/kansas.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/michigan.py` & `calendra-7.7.0/calendra/usa/michigan.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/mississippi.py` & `calendra-7.7.0/calendra/usa/mississippi.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/montana.py` & `calendra-7.7.0/calendra/usa/montana.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/north_carolina.py` & `calendra-7.7.0/calendra/usa/north_carolina.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/texas.py` & `calendra-7.7.0/calendra/usa/texas.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/vermont.py` & `calendra-7.7.0/calendra/usa/vermont.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/virginia.py` & `calendra-7.7.0/calendra/usa/virginia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra/usa/west_virginia.py` & `calendra-7.7.0/calendra/usa/west_virginia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/calendra.egg-info/PKG-INFO` & `calendra-7.7.0/calendra.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: calendra
-Version: 7.6.1
+Version: 7.7.0
 Summary: Worldwide holidays and working days helper and toolkit.
 Home-page: https://github.com/jaraco/calendra
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: docs
 Provides-Extra: astronomy
 License-File: LICENSE
 
-[![](https://img.shields.io/pypi/v/calendra.svg)][1]
+[![](https://img.shields.io/pypi/v/calendra.svg)][https://pypi.org/project/calendra]
 
-[![](https://img.shields.io/pypi/pyversions/calendra.svg)][1]
+![](https://img.shields.io/pypi/pyversions/calendra.svg)
 
-  [1]: https://pypi.org/project/calendra
+[![tests](https://github.com/jaraco/calendra/workflows/Automated%20Tests/badge.svg)](https://github.com/jaraco/calendra/actions?query=workflow%3A%22Automated+Tests%22)
 
-[![Automated Tests](https://github.com/jaraco/calendra/workflows/Automated%20Tests/badge.svg)](https://github.com/jaraco/calendra/actions?query=workflow%3A%22Automated+Tests%22)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+
+[![Code style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![](https://readthedocs.org/projects/calendra/badge/?version=latest)](https://calendra.readthedocs.io/en/latest/?badge=latest)
 
-[![license](http://img.shields.io/pypi/l/workalendar.svg)](https://github.com/workalendar/workalendar/blob/master/LICENSE)
-[![pypi](http://img.shields.io/pypi/v/workalendar.svg)](https://pypi.python.org/pypi/workalendar)
-[![conda](https://img.shields.io/conda/v/conda-forge/workalendar?color=blue&logo=anaconda)](https://anaconda.org/conda-forge/workalendar)
+[![](https://img.shields.io/badge/skeleton-2023-informational)][https://blog.jaraco.com/skeleton]
+
 
 ## Overview
 
 Calendra is a Python module that offers classes able to handle calendars, list legal / religious holidays and gives working-day-related computation functions.
 
 ## History
 
@@ -148,14 +149,15 @@
 
 - Argentina
 - Barbados
 - Brazil (all states, cities and for bank transactions, except the city of Viana)
 - Canada (including provincial and territory holidays)
 - Chile
 - Colombia
+- El Salvador
 - Mexico
 - Panama
 - Paraguay
 - United States of America
   - State holidays for all the 50 States
   - American Samoa
   - Chicago, Illinois
@@ -194,14 +196,15 @@
 - Ivory Coast
 - Kenya
 - Madagascar
 - Mozambique
 - Nigeria
 - São Tomé
 - South Africa
+- Tunisia
 
 And more to come (I hope!)
 
 ## Caveats
 
 Please take note that some calendars are not 100% accurate. The most common example is the Islamic calendar, where some computed holidays are not exactly on the same official day decided by religious authorities, and this may vary country by country. Whenever it's possible, try to adjust your results with the official data provided by the adequate authorities.
```

### Comparing `calendra-7.6.1/calendra.egg-info/SOURCES.txt` & `calendra-7.7.0/calendra.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 .coveragerc
 .editorconfig
-.flake8
 .pre-commit-config.yaml
-.readthedocs.yml
-CHANGES.rst
+.readthedocs.yaml
 LICENSE
+NEWS.rst
 README.md
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
+towncrier.toml
 tox.ini
 .github/PULL_REQUEST_TEMPLATE.md
 .github/dependabot.yml
 .github/workflows/main.yml
 calendra/__init__.py
 calendra/astronomy.py
 calendra/core.py
@@ -38,21 +38,23 @@
 calendra/africa/ivory_coast.py
 calendra/africa/kenya.py
 calendra/africa/madagascar.py
 calendra/africa/mozambique.py
 calendra/africa/nigeria.py
 calendra/africa/sao_tome.py
 calendra/africa/south_africa.py
+calendra/africa/tunisia.py
 calendra/america/__init__.py
 calendra/america/argentina.py
 calendra/america/barbados.py
 calendra/america/brazil.py
 calendra/america/canada.py
 calendra/america/chile.py
 calendra/america/colombia.py
+calendra/america/el_salvador.py
 calendra/america/mexico.py
 calendra/america/panama.py
 calendra/america/paraguay.py
 calendra/asia/__init__.py
 calendra/asia/china.py
 calendra/asia/hong_kong.py
 calendra/asia/israel.py
```

### Comparing `calendra-7.6.1/docs/advanced.md` & `calendra-7.7.0/docs/advanced.md`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/docs/basic.md` & `calendra-7.7.0/docs/basic.md`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/docs/class-options.md` & `calendra-7.7.0/docs/class-options.md`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/docs/conf.py` & `calendra-7.7.0/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ['sphinx.ext.autodoc', 'jaraco.packaging.sphinx', 'rst.linker']
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(
             GH='https://github.com',
             workalendar='https://github.com/workalendar/workalendar/',
         ),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
@@ -32,16 +35,19 @@
                 pattern=r'(?P<wk_ver>[Ww]orkalendar \d+\.\d+(\.\d+)?)',
                 url='{workalendar}blob/master/Changelog.md',
             ),
         ],
     )
 }
 
-# Be strict about any broken references:
+# Be strict about any broken references
 nitpicky = True
 
 # Include Python intersphinx mapping to prevent failures
 # jaraco/skeleton#51
 extensions += ['sphinx.ext.intersphinx']
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
 }
+
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
```

### Comparing `calendra-7.6.1/docs/ical.md` & `calendra-7.7.0/docs/ical.md`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/docs/index.md` & `calendra-7.7.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/docs/iso-registry.md` & `calendra-7.7.0/docs/iso-registry.md`

 * *Files identical despite different names*

### Comparing `calendra-7.6.1/setup.cfg` & `calendra-7.7.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -12,44 +12,45 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	python-dateutil
 	lunardate
 	backports.zoneinfo;python_version<"3.9"
 	tzdata;platform_system=="Windows"
 	convertdate
 	pyluach
 	importlib_metadata; python_version < "3.8"
 	more_itertools
 
 [options.extras_require]
 testing = 
 	pytest >= 3.5, !=3.7.3
 	pytest-checkdocs >= 2.4
-	pytest-flake8
-	flake8 < 5
 	pytest-cov
-	pytest-enabler >= 1.3
+	pytest-enabler >= 2.2
+	pytest-ruff
 	
 	pygments
 	pytest-cov
 	pytest-pep8
 	pandas
 	jaraco.test >= 3.2.0
 	freezegun
 docs = 
-	sphinx
-	jaraco.packaging >= 9
+	sphinx >= 3.5
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 astronomy = 
 	skyfield
 	skyfield-data
 	tqdm
 
 [options.entry_points]
```

