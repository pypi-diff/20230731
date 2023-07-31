# Comparing `tmp/calendra-7.7.0.tar.gz` & `tmp/calendra-7.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendra-7.7.0.tar", last modified: Sun Jul 30 23:47:52 2023, max compression
+gzip compressed data, was "calendra-7.7.1.tar", last modified: Mon Jul 31 00:12:58 2023, max compression
```

## Comparing `calendra-7.7.0.tar` & `calendra-7.7.1.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.995426 calendra-7.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-30 23:47:30.000000 calendra-7.7.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-30 23:47:30.000000 calendra-7.7.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.911426 calendra-7.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-30 23:47:30.000000 calendra-7.7.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-30 23:47:30.000000 calendra-7.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.911426 calendra-7.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-30 23:47:30.000000 calendra-7.7.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-30 23:47:30.000000 calendra-7.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-30 23:47:30.000000 calendra-7.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-30 23:47:30.000000 calendra-7.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37920 2023-07-30 23:47:30.000000 calendra-7.7.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-30 23:47:52.995426 calendra-7.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-07-30 23:47:30.000000 calendra-7.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.915426 calendra-7.7.0/calendra/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.923426 calendra-7.7.0/calendra/africa/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/algeria.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/angola.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/benin.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/ivory_coast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/kenya.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/madagascar.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/mozambique.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/nigeria.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/sao_tome.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/south_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/africa/tunisia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.927426 calendra-7.7.0/calendra/america/
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/argentina.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/barbados.py
--rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/brazil.py
--rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/canada.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/chile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/colombia.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/el_salvador.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/mexico.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/panama.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/america/paraguay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.935426 calendra-7.7.0/calendra/asia/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/china.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/hong_kong.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/israel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/japan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/kazakhstan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/malaysia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/philippines.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/qatar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/singapore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/south_korea.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/asia/taiwan.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/astronomy.py
--rw-r--r--   0 runner    (1001) docker     (123)    36986 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/core.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      146 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/create-astronomical-data.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/equinoxes.json.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.951426 calendra-7.7.0/calendra/europe/
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/austria.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/belarus.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/belgium.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/bulgaria.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/cayman_islands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/croatia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/cyprus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/czech_republic.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/denmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/estonia.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/european_central_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/finland.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/france.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/georgia.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/germany.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/greece.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/guernsey.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/hungary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/iceland.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/ireland.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/italy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/latvia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/lithuania.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/luxembourg.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/malta.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/monaco.py
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/netherlands.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/norway.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/poland.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/portugal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/romania.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/russia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.951426 calendra-7.7.0/calendra/europe/scotland/
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/scotland/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.955426 calendra-7.7.0/calendra/europe/scotland/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/scotland/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/scotland/mixins/autumn_holiday.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/scotland/mixins/fair_holiday.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/scotland/mixins/spring_holiday.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/scotland/mixins/victoria_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/serbia.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/slovakia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/slovenia.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/spain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/sweden.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/switzerland.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/turkey.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/ukraine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/europe/united_kingdom.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/holiday.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.955426 calendra-7.7.0/calendra/oceania/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/oceania/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10933 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/oceania/australia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/oceania/marshall_islands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/oceania/new_zealand.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/precomputed_astronomy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/registry_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/skyfield_astronomy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/solar_terms.json.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.967426 calendra-7.7.0/calendra/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30521 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)    31913 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_america.py
--rw-r--r--   0 runner    (1001) docker     (123)    49921 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_asia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_astronomy.py
--rw-r--r--   0 runner    (1001) docker     (123)    34341 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_brazil.py
--rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_canada.py
--rw-r--r--   0 runner    (1001) docker     (123)    31483 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)   107597 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_europe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_germany.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_global_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_ical_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_mozambique.py
--rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_oceania.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_precomputed_astronomy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_registry_africa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_registry_america.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_registry_asia.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_registry_europe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_registry_oceania.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_registry_usa.py
--rw-r--r--   0 runner    (1001) docker     (123)    18902 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_scotland.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_skyfield_astronomy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_spain.py
--rw-r--r--   0 runner    (1001) docker     (123)    47309 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_switzerland.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_turkey.py
--rw-r--r--   0 runner    (1001) docker     (123)    79160 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/tests/test_usa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.991426 calendra-7.7.0/calendra/usa/
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/alabama.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/alaska.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/american_samoa.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/arizona.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/arkansas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/california.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/colorado.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/connecticut.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/delaware.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/district_columbia.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/florida.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/georgia.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/guam.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/hawaii.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/idaho.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/illinois.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/indiana.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/iowa.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/kansas.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/kentucky.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/louisiana.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/maine.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/maryland.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/massachusetts.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/michigan.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/minnesota.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/mississippi.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/missouri.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/montana.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/nebraska.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/nevada.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/new_hampshire.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/new_jersey.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/new_mexico.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/new_york.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/north_carolina.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/north_dakota.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/ohio.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/oklahoma.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/oregon.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/pennsylvania.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/rhode_island.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/south_carolina.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/south_dakota.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/tennessee.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/texas.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/utah.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/vermont.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/virginia.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/washington.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/west_virginia.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/wisconsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-30 23:47:30.000000 calendra-7.7.0/calendra/usa/wyoming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.919426 calendra-7.7.0/calendra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-30 23:47:52.000000 calendra-7.7.0/calendra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-30 23:47:52.000000 calendra-7.7.0/calendra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 23:47:52.000000 calendra-7.7.0/calendra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-30 23:47:52.000000 calendra-7.7.0/calendra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-30 23:47:52.000000 calendra-7.7.0/calendra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 23:47:52.991426 calendra-7.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/advanced.md
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/basic.md
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/class-options.md
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/ical.md
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-30 23:47:30.000000 calendra-7.7.0/docs/iso-registry.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-30 23:47:30.000000 calendra-7.7.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-30 23:47:30.000000 calendra-7.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-30 23:47:30.000000 calendra-7.7.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-30 23:47:52.995426 calendra-7.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-30 23:47:30.000000 calendra-7.7.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-30 23:47:30.000000 calendra-7.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:12:58.636558 calendra-7.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-31 00:12:37.000000 calendra-7.7.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-31 00:12:37.000000 calendra-7.7.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:12:58.608558 calendra-7.7.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-31 00:12:37.000000 calendra-7.7.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-31 00:12:37.000000 calendra-7.7.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:12:58.608558 calendra-7.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-31 00:12:37.000000 calendra-7.7.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-31 00:12:37.000000 calendra-7.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 00:12:37.000000 calendra-7.7.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-31 00:12:37.000000 calendra-7.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37961 2023-07-31 00:12:37.000000 calendra-7.7.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-31 00:12:58.636558 calendra-7.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-07-31 00:12:37.000000 calendra-7.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:12:58.612558 calendra-7.7.1/calendra/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:12:58.620558 calendra-7.7.1/calendra/africa/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/africa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/africa/algeria.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/africa/angola.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/africa/benin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/africa/ivory_coast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/africa/kenya.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/africa/madagascar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/africa/mozambique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/africa/nigeria.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/africa/sao_tome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/africa/south_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/africa/tunisia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:12:58.620558 calendra-7.7.1/calendra/america/
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/america/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/america/argentina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/america/barbados.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/america/brazil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/america/canada.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/america/chile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/america/colombia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/america/el_salvador.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/america/mexico.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/america/panama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/america/paraguay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:12:58.620558 calendra-7.7.1/calendra/asia/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/asia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/asia/china.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/asia/hong_kong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/asia/israel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/asia/japan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/asia/kazakhstan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/asia/malaysia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/asia/philippines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/asia/qatar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/asia/singapore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/asia/south_korea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/asia/taiwan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/astronomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36986 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/core.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      146 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/create-astronomical-data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/equinoxes.json.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:12:58.624558 calendra-7.7.1/calendra/europe/
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/austria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/belarus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/belgium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/bulgaria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/cayman_islands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/croatia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/cyprus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/czech_republic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/denmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/estonia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/european_central_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/finland.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/france.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/georgia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/germany.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/greece.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/guernsey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/hungary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/iceland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/ireland.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/italy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/latvia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/lithuania.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/luxembourg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/malta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/monaco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/netherlands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/norway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/poland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/portugal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/romania.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/russia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:12:58.624558 calendra-7.7.1/calendra/europe/scotland/
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/scotland/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:12:58.628558 calendra-7.7.1/calendra/europe/scotland/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/scotland/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/scotland/mixins/autumn_holiday.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/scotland/mixins/fair_holiday.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/scotland/mixins/spring_holiday.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/scotland/mixins/victoria_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/serbia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/slovakia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/slovenia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/spain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/sweden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/switzerland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/turkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/ukraine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/europe/united_kingdom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/holiday.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:12:58.628558 calendra-7.7.1/calendra/oceania/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/oceania/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10933 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/oceania/australia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/oceania/marshall_islands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/oceania/new_zealand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/precomputed_astronomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/registry_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/skyfield_astronomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/solar_terms.json.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:12:58.628558 calendra-7.7.1/calendra/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30521 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31913 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49921 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_asia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_astronomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34341 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_brazil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_canada.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31483 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107597 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_europe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_germany.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_global_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_ical_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_mozambique.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13673 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_oceania.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_precomputed_astronomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_registry_africa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_registry_america.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_registry_asia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_registry_europe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_registry_oceania.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_registry_usa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18902 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_scotland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_skyfield_astronomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_spain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47309 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_switzerland.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_turkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79160 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/tests/test_usa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:12:58.636558 calendra-7.7.1/calendra/usa/
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/alabama.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/alaska.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/american_samoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/arizona.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/arkansas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/california.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/colorado.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/connecticut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/delaware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/district_columbia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/florida.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/georgia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/guam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/hawaii.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/idaho.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/illinois.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/indiana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/iowa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/kansas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/kentucky.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/louisiana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/maine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/maryland.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/massachusetts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/michigan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/minnesota.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/mississippi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/missouri.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/montana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/nebraska.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/nevada.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/new_hampshire.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/new_jersey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/new_mexico.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/new_york.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/north_carolina.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/north_dakota.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/ohio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/oklahoma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/oregon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/pennsylvania.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/rhode_island.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/south_carolina.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/south_dakota.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/tennessee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/texas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/utah.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/vermont.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/virginia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/washington.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/west_virginia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/wisconsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-31 00:12:37.000000 calendra-7.7.1/calendra/usa/wyoming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:12:58.616558 calendra-7.7.1/calendra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-31 00:12:58.000000 calendra-7.7.1/calendra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-31 00:12:58.000000 calendra-7.7.1/calendra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:12:58.000000 calendra-7.7.1/calendra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-31 00:12:58.000000 calendra-7.7.1/calendra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 00:12:58.000000 calendra-7.7.1/calendra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:12:58.636558 calendra-7.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-31 00:12:37.000000 calendra-7.7.1/docs/advanced.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-31 00:12:37.000000 calendra-7.7.1/docs/basic.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-31 00:12:37.000000 calendra-7.7.1/docs/class-options.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-31 00:12:37.000000 calendra-7.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-31 00:12:37.000000 calendra-7.7.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-31 00:12:37.000000 calendra-7.7.1/docs/ical.md
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-31 00:12:37.000000 calendra-7.7.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-31 00:12:37.000000 calendra-7.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-31 00:12:37.000000 calendra-7.7.1/docs/iso-registry.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-31 00:12:37.000000 calendra-7.7.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-31 00:12:37.000000 calendra-7.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-31 00:12:37.000000 calendra-7.7.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-31 00:12:58.636558 calendra-7.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-31 00:12:37.000000 calendra-7.7.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-31 00:12:37.000000 calendra-7.7.1/tox.ini
```

### Comparing `calendra-7.7.0/.github/PULL_REQUEST_TEMPLATE.md` & `calendra-7.7.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/.github/workflows/main.yml` & `calendra-7.7.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/LICENSE` & `calendra-7.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/NEWS.rst` & `calendra-7.7.1/NEWS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v7.7.1
+======
+
+No significant changes.
+
+
 v7.7.0
 ======
 
 Features
 --------
 
 - Incorporate changes from workalendar v17.0.0 (2023-01-01)
```

### Comparing `calendra-7.7.0/PKG-INFO` & `calendra-7.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendra
-Version: 7.7.0
+Version: 7.7.1
 Summary: Worldwide holidays and working days helper and toolkit.
 Home-page: https://github.com/jaraco/calendra
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,27 +13,27 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: docs
 Provides-Extra: astronomy
 License-File: LICENSE
 
-[![](https://img.shields.io/pypi/v/calendra.svg)][https://pypi.org/project/calendra]
+[![](https://img.shields.io/pypi/v/calendra.svg)](https://pypi.org/project/calendra)
 
 ![](https://img.shields.io/pypi/pyversions/calendra.svg)
 
-[![tests](https://github.com/jaraco/calendra/workflows/Automated%20Tests/badge.svg)](https://github.com/jaraco/calendra/actions?query=workflow%3A%22Automated+Tests%22)
+[![tests](https://github.com/jaraco/calendra/workflows/tests/badge.svg)](https://github.com/jaraco/calendra/actions?query=workflow%3A%22tests%22)
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 [![Code style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![](https://readthedocs.org/projects/calendra/badge/?version=latest)](https://calendra.readthedocs.io/en/latest/?badge=latest)
 
-[![](https://img.shields.io/badge/skeleton-2023-informational)][https://blog.jaraco.com/skeleton]
+[![](https://img.shields.io/badge/skeleton-2023-informational)](https://blog.jaraco.com/skeleton)
 
 
 ## Overview
 
 Calendra is a Python module that offers classes able to handle calendars, list legal / religious holidays and gives working-day-related computation functions.
 
 ## History
```

### Comparing `calendra-7.7.0/README.md` & `calendra-7.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-[![](https://img.shields.io/pypi/v/calendra.svg)][https://pypi.org/project/calendra]
+[![](https://img.shields.io/pypi/v/calendra.svg)](https://pypi.org/project/calendra)
 
 ![](https://img.shields.io/pypi/pyversions/calendra.svg)
 
-[![tests](https://github.com/jaraco/calendra/workflows/Automated%20Tests/badge.svg)](https://github.com/jaraco/calendra/actions?query=workflow%3A%22Automated+Tests%22)
+[![tests](https://github.com/jaraco/calendra/workflows/tests/badge.svg)](https://github.com/jaraco/calendra/actions?query=workflow%3A%22tests%22)
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 [![Code style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![](https://readthedocs.org/projects/calendra/badge/?version=latest)](https://calendra.readthedocs.io/en/latest/?badge=latest)
 
-[![](https://img.shields.io/badge/skeleton-2023-informational)][https://blog.jaraco.com/skeleton]
+[![](https://img.shields.io/badge/skeleton-2023-informational)](https://blog.jaraco.com/skeleton)
 
 
 ## Overview
 
 Calendra is a Python module that offers classes able to handle calendars, list legal / religious holidays and gives working-day-related computation functions.
 
 ## History
```

### Comparing `calendra-7.7.0/calendra/africa/__init__.py` & `calendra-7.7.1/calendra/africa/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/africa/algeria.py` & `calendra-7.7.1/calendra/africa/algeria.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/africa/angola.py` & `calendra-7.7.1/calendra/africa/angola.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/africa/benin.py` & `calendra-7.7.1/calendra/africa/benin.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/africa/ivory_coast.py` & `calendra-7.7.1/calendra/africa/ivory_coast.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/africa/kenya.py` & `calendra-7.7.1/calendra/africa/kenya.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/africa/madagascar.py` & `calendra-7.7.1/calendra/africa/madagascar.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/africa/mozambique.py` & `calendra-7.7.1/calendra/africa/mozambique.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/africa/nigeria.py` & `calendra-7.7.1/calendra/africa/nigeria.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/africa/sao_tome.py` & `calendra-7.7.1/calendra/africa/sao_tome.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/africa/south_africa.py` & `calendra-7.7.1/calendra/africa/south_africa.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/africa/tunisia.py` & `calendra-7.7.1/calendra/africa/tunisia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/america/__init__.py` & `calendra-7.7.1/calendra/america/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/america/argentina.py` & `calendra-7.7.1/calendra/america/argentina.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/america/barbados.py` & `calendra-7.7.1/calendra/america/barbados.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/america/brazil.py` & `calendra-7.7.1/calendra/america/brazil.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/america/canada.py` & `calendra-7.7.1/calendra/america/canada.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/america/chile.py` & `calendra-7.7.1/calendra/america/chile.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/america/colombia.py` & `calendra-7.7.1/calendra/america/colombia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/america/el_salvador.py` & `calendra-7.7.1/calendra/america/el_salvador.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/america/mexico.py` & `calendra-7.7.1/calendra/america/mexico.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/america/panama.py` & `calendra-7.7.1/calendra/america/panama.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/america/paraguay.py` & `calendra-7.7.1/calendra/america/paraguay.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/asia/__init__.py` & `calendra-7.7.1/calendra/asia/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/asia/china.py` & `calendra-7.7.1/calendra/asia/china.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/asia/hong_kong.py` & `calendra-7.7.1/calendra/asia/hong_kong.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/asia/israel.py` & `calendra-7.7.1/calendra/asia/israel.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/asia/japan.py` & `calendra-7.7.1/calendra/asia/japan.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/asia/kazakhstan.py` & `calendra-7.7.1/calendra/asia/kazakhstan.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/asia/malaysia.py` & `calendra-7.7.1/calendra/asia/malaysia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/asia/philippines.py` & `calendra-7.7.1/calendra/asia/philippines.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/asia/singapore.py` & `calendra-7.7.1/calendra/asia/singapore.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/asia/south_korea.py` & `calendra-7.7.1/calendra/asia/south_korea.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/asia/taiwan.py` & `calendra-7.7.1/calendra/asia/taiwan.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/core.py` & `calendra-7.7.1/calendra/core.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/equinoxes.json.gz` & `calendra-7.7.1/calendra/equinoxes.json.gz`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/__init__.py` & `calendra-7.7.1/calendra/europe/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/austria.py` & `calendra-7.7.1/calendra/europe/austria.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/belarus.py` & `calendra-7.7.1/calendra/europe/belarus.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/bulgaria.py` & `calendra-7.7.1/calendra/europe/bulgaria.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/cayman_islands.py` & `calendra-7.7.1/calendra/europe/cayman_islands.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/croatia.py` & `calendra-7.7.1/calendra/europe/croatia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/cyprus.py` & `calendra-7.7.1/calendra/europe/cyprus.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/czech_republic.py` & `calendra-7.7.1/calendra/europe/czech_republic.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/denmark.py` & `calendra-7.7.1/calendra/europe/denmark.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/estonia.py` & `calendra-7.7.1/calendra/europe/estonia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/finland.py` & `calendra-7.7.1/calendra/europe/finland.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/france.py` & `calendra-7.7.1/calendra/europe/france.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/georgia.py` & `calendra-7.7.1/calendra/europe/georgia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/germany.py` & `calendra-7.7.1/calendra/europe/germany.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/greece.py` & `calendra-7.7.1/calendra/europe/greece.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/guernsey.py` & `calendra-7.7.1/calendra/europe/guernsey.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/hungary.py` & `calendra-7.7.1/calendra/europe/hungary.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/iceland.py` & `calendra-7.7.1/calendra/europe/iceland.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/ireland.py` & `calendra-7.7.1/calendra/europe/ireland.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/italy.py` & `calendra-7.7.1/calendra/europe/italy.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/latvia.py` & `calendra-7.7.1/calendra/europe/latvia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/lithuania.py` & `calendra-7.7.1/calendra/europe/lithuania.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/luxembourg.py` & `calendra-7.7.1/calendra/europe/luxembourg.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/malta.py` & `calendra-7.7.1/calendra/europe/malta.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/monaco.py` & `calendra-7.7.1/calendra/europe/monaco.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/netherlands.py` & `calendra-7.7.1/calendra/europe/netherlands.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/norway.py` & `calendra-7.7.1/calendra/europe/norway.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/poland.py` & `calendra-7.7.1/calendra/europe/poland.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/portugal.py` & `calendra-7.7.1/calendra/europe/portugal.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/romania.py` & `calendra-7.7.1/calendra/europe/romania.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/russia.py` & `calendra-7.7.1/calendra/europe/russia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/scotland/__init__.py` & `calendra-7.7.1/calendra/europe/scotland/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/scotland/mixins/__init__.py` & `calendra-7.7.1/calendra/europe/scotland/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/scotland/mixins/autumn_holiday.py` & `calendra-7.7.1/calendra/europe/scotland/mixins/autumn_holiday.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/scotland/mixins/fair_holiday.py` & `calendra-7.7.1/calendra/europe/scotland/mixins/fair_holiday.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/scotland/mixins/spring_holiday.py` & `calendra-7.7.1/calendra/europe/scotland/mixins/spring_holiday.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/scotland/mixins/victoria_day.py` & `calendra-7.7.1/calendra/europe/scotland/mixins/victoria_day.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/serbia.py` & `calendra-7.7.1/calendra/europe/serbia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/slovakia.py` & `calendra-7.7.1/calendra/europe/slovakia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/slovenia.py` & `calendra-7.7.1/calendra/europe/slovenia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/spain.py` & `calendra-7.7.1/calendra/europe/spain.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/sweden.py` & `calendra-7.7.1/calendra/europe/sweden.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/switzerland.py` & `calendra-7.7.1/calendra/europe/switzerland.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/turkey.py` & `calendra-7.7.1/calendra/europe/turkey.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/ukraine.py` & `calendra-7.7.1/calendra/europe/ukraine.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/europe/united_kingdom.py` & `calendra-7.7.1/calendra/europe/united_kingdom.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/exceptions.py` & `calendra-7.7.1/calendra/exceptions.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/holiday.py` & `calendra-7.7.1/calendra/holiday.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/oceania/__init__.py` & `calendra-7.7.1/calendra/oceania/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/oceania/australia.py` & `calendra-7.7.1/calendra/oceania/australia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/oceania/marshall_islands.py` & `calendra-7.7.1/calendra/oceania/marshall_islands.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/oceania/new_zealand.py` & `calendra-7.7.1/calendra/oceania/new_zealand.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/precomputed_astronomy.py` & `calendra-7.7.1/calendra/precomputed_astronomy.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/registry.py` & `calendra-7.7.1/calendra/registry.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/registry_tools.py` & `calendra-7.7.1/calendra/registry_tools.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/skyfield_astronomy.py` & `calendra-7.7.1/calendra/skyfield_astronomy.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/solar_terms.json.gz` & `calendra-7.7.1/calendra/solar_terms.json.gz`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/__init__.py` & `calendra-7.7.1/calendra/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_africa.py` & `calendra-7.7.1/calendra/tests/test_africa.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_america.py` & `calendra-7.7.1/calendra/tests/test_america.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_asia.py` & `calendra-7.7.1/calendra/tests/test_asia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_astronomy.py` & `calendra-7.7.1/calendra/tests/test_astronomy.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_brazil.py` & `calendra-7.7.1/calendra/tests/test_brazil.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_canada.py` & `calendra-7.7.1/calendra/tests/test_canada.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_core.py` & `calendra-7.7.1/calendra/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_europe.py` & `calendra-7.7.1/calendra/tests/test_europe.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_germany.py` & `calendra-7.7.1/calendra/tests/test_germany.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_ical_export.py` & `calendra-7.7.1/calendra/tests/test_ical_export.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_mozambique.py` & `calendra-7.7.1/calendra/tests/test_mozambique.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_oceania.py` & `calendra-7.7.1/calendra/tests/test_oceania.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_precomputed_astronomy.py` & `calendra-7.7.1/calendra/tests/test_precomputed_astronomy.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_registry.py` & `calendra-7.7.1/calendra/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_registry_africa.py` & `calendra-7.7.1/calendra/tests/test_registry_africa.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_registry_america.py` & `calendra-7.7.1/calendra/tests/test_registry_america.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_registry_asia.py` & `calendra-7.7.1/calendra/tests/test_registry_asia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_registry_europe.py` & `calendra-7.7.1/calendra/tests/test_registry_europe.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_registry_oceania.py` & `calendra-7.7.1/calendra/tests/test_registry_oceania.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_registry_usa.py` & `calendra-7.7.1/calendra/tests/test_registry_usa.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_scotland.py` & `calendra-7.7.1/calendra/tests/test_scotland.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_skyfield_astronomy.py` & `calendra-7.7.1/calendra/tests/test_skyfield_astronomy.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_spain.py` & `calendra-7.7.1/calendra/tests/test_spain.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_switzerland.py` & `calendra-7.7.1/calendra/tests/test_switzerland.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_turkey.py` & `calendra-7.7.1/calendra/tests/test_turkey.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/tests/test_usa.py` & `calendra-7.7.1/calendra/tests/test_usa.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/__init__.py` & `calendra-7.7.1/calendra/usa/__init__.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/alabama.py` & `calendra-7.7.1/calendra/usa/alabama.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/alaska.py` & `calendra-7.7.1/calendra/usa/alaska.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/american_samoa.py` & `calendra-7.7.1/calendra/usa/american_samoa.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/california.py` & `calendra-7.7.1/calendra/usa/california.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/core.py` & `calendra-7.7.1/calendra/usa/core.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/florida.py` & `calendra-7.7.1/calendra/usa/florida.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/georgia.py` & `calendra-7.7.1/calendra/usa/georgia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/hawaii.py` & `calendra-7.7.1/calendra/usa/hawaii.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/illinois.py` & `calendra-7.7.1/calendra/usa/illinois.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/indiana.py` & `calendra-7.7.1/calendra/usa/indiana.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/kansas.py` & `calendra-7.7.1/calendra/usa/kansas.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/michigan.py` & `calendra-7.7.1/calendra/usa/michigan.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/mississippi.py` & `calendra-7.7.1/calendra/usa/mississippi.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/montana.py` & `calendra-7.7.1/calendra/usa/montana.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/north_carolina.py` & `calendra-7.7.1/calendra/usa/north_carolina.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/texas.py` & `calendra-7.7.1/calendra/usa/texas.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/vermont.py` & `calendra-7.7.1/calendra/usa/vermont.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/virginia.py` & `calendra-7.7.1/calendra/usa/virginia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra/usa/west_virginia.py` & `calendra-7.7.1/calendra/usa/west_virginia.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/calendra.egg-info/PKG-INFO` & `calendra-7.7.1/calendra.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendra
-Version: 7.7.0
+Version: 7.7.1
 Summary: Worldwide holidays and working days helper and toolkit.
 Home-page: https://github.com/jaraco/calendra
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,27 +13,27 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: docs
 Provides-Extra: astronomy
 License-File: LICENSE
 
-[![](https://img.shields.io/pypi/v/calendra.svg)][https://pypi.org/project/calendra]
+[![](https://img.shields.io/pypi/v/calendra.svg)](https://pypi.org/project/calendra)
 
 ![](https://img.shields.io/pypi/pyversions/calendra.svg)
 
-[![tests](https://github.com/jaraco/calendra/workflows/Automated%20Tests/badge.svg)](https://github.com/jaraco/calendra/actions?query=workflow%3A%22Automated+Tests%22)
+[![tests](https://github.com/jaraco/calendra/workflows/tests/badge.svg)](https://github.com/jaraco/calendra/actions?query=workflow%3A%22tests%22)
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 [![Code style: Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![](https://readthedocs.org/projects/calendra/badge/?version=latest)](https://calendra.readthedocs.io/en/latest/?badge=latest)
 
-[![](https://img.shields.io/badge/skeleton-2023-informational)][https://blog.jaraco.com/skeleton]
+[![](https://img.shields.io/badge/skeleton-2023-informational)](https://blog.jaraco.com/skeleton)
 
 
 ## Overview
 
 Calendra is a Python module that offers classes able to handle calendars, list legal / religious holidays and gives working-day-related computation functions.
 
 ## History
```

### Comparing `calendra-7.7.0/calendra.egg-info/SOURCES.txt` & `calendra-7.7.1/calendra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/docs/advanced.md` & `calendra-7.7.1/docs/advanced.md`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/docs/basic.md` & `calendra-7.7.1/docs/basic.md`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/docs/class-options.md` & `calendra-7.7.1/docs/class-options.md`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/docs/conf.py` & `calendra-7.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/docs/ical.md` & `calendra-7.7.1/docs/ical.md`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/docs/index.md` & `calendra-7.7.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/docs/iso-registry.md` & `calendra-7.7.1/docs/iso-registry.md`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/pytest.ini` & `calendra-7.7.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/setup.cfg` & `calendra-7.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `calendra-7.7.0/tox.ini` & `calendra-7.7.1/tox.ini`

 * *Files identical despite different names*

