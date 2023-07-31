# Comparing `tmp/scranpy-0.0.2.tar.gz` & `tmp/scranpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scranpy-0.0.2.tar", last modified: Sun Jul 30 03:20:37 2023, max compression
+gzip compressed data, was "scranpy-0.0.3.tar", last modified: Mon Jul 31 05:40:06 2023, max compression
```

## Comparing `scranpy-0.0.2.tar` & `scranpy-0.0.3.tar`

### file list

```diff
@@ -1,236 +1,2554 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.311781 scranpy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-30 03:20:16.000000 scranpy-0.0.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.247779 scranpy-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.263780 scranpy-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-30 03:20:16.000000 scranpy-0.0.2/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-30 03:20:16.000000 scranpy-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-30 03:20:16.000000 scranpy-0.0.2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-30 03:20:16.000000 scranpy-0.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-30 03:20:16.000000 scranpy-0.0.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-30 03:20:16.000000 scranpy-0.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-07-30 03:20:16.000000 scranpy-0.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-30 03:20:16.000000 scranpy-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-30 03:20:16.000000 scranpy-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-30 03:20:37.311781 scranpy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-30 03:20:16.000000 scranpy-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-30 03:20:16.000000 scranpy-0.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.255780 scranpy-0.0.2/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/extern/libscran/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-30 03:20:16.000000 scranpy-0.0.2/extern/libscran/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.251779 scranpy-0.0.2/extern/libscran/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/extern/libscran/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/.github/workflows/doxygenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/.github/workflows/run-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/extern/libscran/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   109654 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/docs/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/extern/libscran/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/extern/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/extern/libscran/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/gallery/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/gallery/minimal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/gallery/pca_test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.251779 scranpy-0.0.2/extern/libscran/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.267780 scranpy-0.0.2/extern/libscran/include/scran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.271780 scranpy-0.0.2/extern/libscran/include/scran/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)    17638 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/aggregation/AggregateAcrossCells.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/aggregation/DownsampleByNeighbors.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.271780 scranpy-0.0.2/extern/libscran/include/scran/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)    13936 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/clustering/BuildSnnGraph.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16608 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/clustering/ClusterSnnGraph.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/clustering/igraph_utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.271780 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/MatrixCalculator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    29152 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/PairwiseEffects.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    48761 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/ScoreMarkers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/SummarizeEffects.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/auc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/cohens_d.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/simple_diff.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/summarize_comparisons.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.275780 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/
--rw-r--r--   0 runner    (1001) docker     (123)    27251 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/MultiBatchPca.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    18792 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/ResidualPca.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/ScaleByNeighbors.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/SimplePca.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/blocking.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/convert.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/wrappers.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.275780 scranpy-0.0.2/extern/libscran/include/scran/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/feature_selection/ChooseHvgs.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/feature_selection/FitVarianceTrend.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27677 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/feature_selection/ModelGeneVariances.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/feature_selection/blocked_variances.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.275780 scranpy-0.0.2/extern/libscran/include/scran/feature_set_enrichment/
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/feature_set_enrichment/HypergeometricTail.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/feature_set_enrichment/ScoreFeatureSet.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.279780 scranpy-0.0.2/extern/libscran/include/scran/normalization/
--rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/normalization/CenterSizeFactors.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/normalization/ChoosePseudoCount.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/normalization/GroupedSizeFactors.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/normalization/LogNormCounts.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/normalization/MedianSizeFactors.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/normalization/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.283780 scranpy-0.0.2/extern/libscran/include/scran/quality_control/
--rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/ChooseOutlierFilters.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/ComputeMedianMad.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/FilterCells.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/PerCellAdtQcMetrics.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/PerCellCrisprQcMetrics.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30743 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/PerCellQcMetrics.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/PerCellRnaQcMetrics.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/SuggestAdtQcFilters.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/SuggestCrisprQcFilters.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/SuggestRnaQcFilters.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/quality_control/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/scran.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.283780 scranpy-0.0.2/extern/libscran/include/scran/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/utils/average_vectors.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/utils/blocking.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/utils/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/utils/subset_vector.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/include/scran/utils/vector_to_pointers.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.283780 scranpy-0.0.2/extern/libscran/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.255780 scranpy-0.0.2/extern/libscran/tests/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.283780 scranpy-0.0.2/extern/libscran/tests/src/aggregation/
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/aggregation/AggregateAcrossCells.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/aggregation/DownsampleByNeighbors.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.283780 scranpy-0.0.2/extern/libscran/tests/src/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/clustering/BuildSnnGraph.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/clustering/ClusterSnnGraph.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.287780 scranpy-0.0.2/extern/libscran/tests/src/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/data/Simulator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/data/data.h
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/data/data_sparse.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.287780 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)    22508 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/MatrixCalculator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/PairwiseEffects.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17375 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/ScoreMarkers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/auc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/cohens_d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/simple_diff.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/summarize_comparisons.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.291780 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/MultiBatchPca.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20523 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/ResidualPca.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/ScaleByNeighbors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/SimplePca.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/compare_pcs.h
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/convert.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/utils.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.291780 scranpy-0.0.2/extern/libscran/tests/src/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/feature_selection/ChooseHvgs.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/feature_selection/FitVarianceTrend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/feature_selection/ModelGeneVariances.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.291780 scranpy-0.0.2/extern/libscran/tests/src/feature_set_enrichment/
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/feature_set_enrichment/HypergeometricTail.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/feature_set_enrichment/ScoreFeatureSet.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.291780 scranpy-0.0.2/extern/libscran/tests/src/normalization/
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/normalization/CenterSizeFactors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/normalization/ChoosePseudoCount.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/normalization/GroupedSizeFactors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/normalization/LogNormCounts.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/normalization/MedianSizeFactors.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.295780 scranpy-0.0.2/extern/libscran/tests/src/quality_control/
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/ChooseOutlierFilters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/ComputeMedianMad.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/FilterCells.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/PerCellAdtQcMetrics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/PerCellCrisprQcMetrics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15529 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/PerCellQcMetrics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/PerCellRnaQcMetrics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/SuggestAdtQcFilters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/SuggestCrisprQcFilters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/SuggestRnaQcFilters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/quality_control/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.299780 scranpy-0.0.2/extern/libscran/tests/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/utils/average_vectors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/utils/blocking.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/utils/compare_almost_equal.h
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/utils/compare_vectors.h
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/utils/custom_parallel.h
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/utils/macros.h
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/libscran/tests/src/utils/subset_vector.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.299780 scranpy-0.0.2/extern/weightedlowess/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.255780 scranpy-0.0.2/extern/weightedlowess/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.299780 scranpy-0.0.2/extern/weightedlowess/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/.github/workflows/compare-limma.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/.github/workflows/doxygenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/.github/workflows/run-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.299780 scranpy-0.0.2/extern/weightedlowess/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   108663 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/docs/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.259780 scranpy-0.0.2/extern/weightedlowess/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.299780 scranpy-0.0.2/extern/weightedlowess/include/WeightedLowess/
--rw-r--r--   0 runner    (1001) docker     (123)    31431 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/include/WeightedLowess/WeightedLowess.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.299780 scranpy-0.0.2/extern/weightedlowess/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.303780 scranpy-0.0.2/extern/weightedlowess/tests/R/
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/R/run.R
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/R/test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.303780 scranpy-0.0.2/extern/weightedlowess/tests/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/src/basic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/src/divzero.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/src/options.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/src/runners.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/src/ties.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/src/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-30 03:20:17.000000 scranpy-0.0.2/extern/weightedlowess/tests/src/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-30 03:20:16.000000 scranpy-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-30 03:20:37.311781 scranpy-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-30 03:20:16.000000 scranpy-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.259780 scranpy-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.303780 scranpy-0.0.2/src/scranpy/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/cpphelpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.307780 scranpy-0.0.2/src/scranpy/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/feature_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/feature_selection/model_gene_variances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.307780 scranpy-0.0.2/src/scranpy/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/lib/log_norm_counts.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/lib/model_gene_variances.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/lib/per_cell_rna_qc_metrics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/lib/suggest_rna_qc_filters.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.307780 scranpy-0.0.2/src/scranpy/normalization/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/normalization/log_norm_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.307780 scranpy-0.0.2/src/scranpy/quality_control/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/quality_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/quality_control/rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-30 03:20:16.000000 scranpy-0.0.2/src/scranpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.307780 scranpy-0.0.2/src/scranpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-30 03:20:37.000000 scranpy-0.0.2/src/scranpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-07-30 03:20:37.000000 scranpy-0.0.2/src/scranpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 03:20:37.000000 scranpy-0.0.2/src/scranpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 03:20:36.000000 scranpy-0.0.2/src/scranpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-30 03:20:37.000000 scranpy-0.0.2/src/scranpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 03:20:37.000000 scranpy-0.0.2/src/scranpy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:20:37.311781 scranpy-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-30 03:20:16.000000 scranpy-0.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-30 03:20:16.000000 scranpy-0.0.2/tests/test_log_norm_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-30 03:20:16.000000 scranpy-0.0.2/tests/test_model_gene_variances.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-30 03:20:16.000000 scranpy-0.0.2/tests/test_quality_control_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-30 03:20:16.000000 scranpy-0.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.445441 scranpy-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-31 05:39:28.000000 scranpy-0.0.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.681439 scranpy-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.745439 scranpy-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-31 05:39:28.000000 scranpy-0.0.3/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-31 05:39:28.000000 scranpy-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-31 05:39:28.000000 scranpy-0.0.3/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-31 05:39:28.000000 scranpy-0.0.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-31 05:39:28.000000 scranpy-0.0.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-31 05:39:28.000000 scranpy-0.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-07-31 05:39:28.000000 scranpy-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-31 05:39:28.000000 scranpy-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-31 05:39:28.000000 scranpy-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-31 05:40:06.445441 scranpy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-31 05:39:28.000000 scranpy-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.745439 scranpy-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-31 05:39:28.000000 scranpy-0.0.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.745439 scranpy-0.0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 05:39:28.000000 scranpy-0.0.3/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-31 05:39:28.000000 scranpy-0.0.3/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-31 05:39:28.000000 scranpy-0.0.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-07-31 05:39:28.000000 scranpy-0.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-31 05:39:28.000000 scranpy-0.0.3/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-31 05:39:28.000000 scranpy-0.0.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-31 05:39:28.000000 scranpy-0.0.3/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 05:39:28.000000 scranpy-0.0.3/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-31 05:39:28.000000 scranpy-0.0.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.737439 scranpy-0.0.3/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.745439 scranpy-0.0.3/extern/aarand/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-31 05:39:29.000000 scranpy-0.0.3/extern/aarand/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.685439 scranpy-0.0.3/extern/aarand/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.749439 scranpy-0.0.3/extern/aarand/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/aarand/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/aarand/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/aarand/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/aarand/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/aarand/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/aarand/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.749439 scranpy-0.0.3/extern/aarand/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108628 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/aarand/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.685439 scranpy-0.0.3/extern/aarand/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.749439 scranpy-0.0.3/extern/aarand/include/aarand/
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/aarand/include/aarand/aarand.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.749439 scranpy-0.0.3/extern/aarand/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/aarand/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.749439 scranpy-0.0.3/extern/aarand/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/aarand/tests/src/exponential.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/aarand/tests/src/normal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/aarand/tests/src/sample.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/aarand/tests/src/shuffle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/aarand/tests/src/uniform.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.753439 scranpy-0.0.3/extern/annoy/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-31 05:39:29.000000 scranpy-0.0.3/extern/annoy/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.685439 scranpy-0.0.3/extern/annoy/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.753439 scranpy-0.0.3/extern/annoy/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/README_GO.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/README_Lua.md
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)   609008 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/ann.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.753439 scranpy-0.0.3/extern/annoy/annoy/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/annoy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/annoy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/annoy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/annoy-dev-1.rockspec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.753439 scranpy-0.0.3/extern/annoy/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/debian/control
+-rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.753439 scranpy-0.0.3/extern/annoy/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/examples/mmap_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/examples/precision_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/examples/precision_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      172 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/examples/s_compile_cpp.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/examples/simple_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.757439 scranpy-0.0.3/extern/annoy/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/src/annoygomodule.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/src/annoygomodule.i
+-rw-r--r--   0 runner    (1001) docker     (123)    45690 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/src/annoylib.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/src/annoyluamodule.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/src/annoymodule.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/src/kissrandom.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/src/mman.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.761439 scranpy-0.0.3/extern/annoy/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/accuracy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/angular_index_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/annoy_test.go
+-rw-r--r--   0 runner    (1001) docker     (123)    16466 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/annoy_test.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/dot_index_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/euclidean_index_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/examples_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/hamming_index_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/holes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/index_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/manhattan_index_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/memory_leak_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/multithreaded_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/on_disk_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/seed_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/test.tree
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/threading_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/test/types_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-31 05:39:37.000000 scranpy-0.0.3/extern/annoy/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.765439 scranpy-0.0.3/extern/eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-31 05:39:31.000000 scranpy-0.0.3/extern/eigen/.git
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.689439 scranpy-0.0.3/extern/eigen/.gitlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.765439 scranpy-0.0.3/extern/eigen/.gitlab/issue_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/.gitlab/issue_templates/Bug Report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/.gitlab/issue_templates/Feature Request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.765439 scranpy-0.0.3/extern/eigen/.gitlab/merge_request_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/.gitlab/merge_request_templates/Merge Request Template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/.hgeol
+-rw-r--r--   0 runner    (1001) docker     (123)    24767 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/COPYING.APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/COPYING.BSD
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/COPYING.GPL
+-rw-r--r--   0 runner    (1001) docker     (123)    26530 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/COPYING.LGPL
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/COPYING.MINPACK
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/COPYING.MPL2
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/COPYING.README
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/CTestConfig.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/CTestCustom.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.769439 scranpy-0.0.3/extern/eigen/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/Cholesky
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/CholmodSupport
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/Core
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/Dense
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/Eigen
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/Eigenvalues
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/Geometry
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/Householder
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/Jacobi
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/KLUSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/LU
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/MetisSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/OrderingMethods
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/PaStiXSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/PardisoSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/QR
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/QtAlignedMalloc
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/SPQRSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/SVD
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/Sparse
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/SparseCholesky
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/SparseCore
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/SparseLU
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/SparseQR
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/StdDeque
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/StdList
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/StdVector
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/SuperLUSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/UmfPackSupport
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.709439 scranpy-0.0.3/extern/eigen/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.773439 scranpy-0.0.3/extern/eigen/Eigen/src/Cholesky/
+-rw-r--r--   0 runner    (1001) docker     (123)    24934 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.773439 scranpy-0.0.3/extern/eigen/Eigen/src/CholmodSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    25441 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.797439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)    19214 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16782 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41673 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/AssignEvaluator.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12488 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    63841 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36282 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31529 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24484 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21679 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38812 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    60784 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24343 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23856 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    49193 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner    (1001) docker     (123)    53832 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19195 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17606 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38277 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35168 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.697439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.797439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64608 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.801439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    87891 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.801439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)   119355 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24820 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)   102394 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.801439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 runner    (1001) docker     (123)    17317 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/CUDA/Complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.805439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner    (1001) docker     (123)    26903 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)    67696 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35534 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/Default/Settings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.805439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57047 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.693439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/HIP/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.805439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.805439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 runner    (1001) docker     (123)    17541 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16159 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33615 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.805439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (123)    22503 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)   189525 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51286 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.805439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    64465 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.809439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/SVE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21200 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.809439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27786 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21856 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.809439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36894 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.809439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/functors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20921 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40146 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.817439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/
+-rw-r--r--   0 runner    (1001) docker     (123)   108448 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20104 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21724 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21354 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14678 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.821439 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23156 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19876 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21931 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4892 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15555 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/IntegralConstant.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4268 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52909 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)    46661 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/Memory.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29336 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.821439 scranpy-0.0.3/extern/eigen/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23640 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35182 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.825439 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)    18939 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20726 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34367 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 runner    (1001) docker     (123)    61930 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.825439 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.825439 scranpy-0.0.3/extern/eigen/Eigen/src/Householder/
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23611 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.829439 scranpy-0.0.3/extern/eigen/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.829439 scranpy-0.0.3/extern/eigen/Eigen/src/Jacobi/
+-rw-r--r--   0 runner    (1001) docker     (123)    16383 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.829439 scranpy-0.0.3/extern/eigen/Eigen/src/KLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/KLUSupport/KLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.829439 scranpy-0.0.3/extern/eigen/Eigen/src/LU/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32383 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15727 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.829439 scranpy-0.0.3/extern/eigen/Eigen/src/LU/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/LU/arch/InverseSize4.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.829439 scranpy-0.0.3/extern/eigen/Eigen/src/MetisSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.833439 scranpy-0.0.3/extern/eigen/Eigen/src/OrderingMethods/
+-rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    61681 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.833439 scranpy-0.0.3/extern/eigen/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    22249 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.833439 scranpy-0.0.3/extern/eigen/Eigen/src/PardisoSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.833439 scranpy-0.0.3/extern/eigen/Eigen/src/QR/
+-rw-r--r--   0 runner    (1001) docker     (123)    25498 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26768 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14641 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.833439 scranpy-0.0.3/extern/eigen/Eigen/src/SPQRSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.833439 scranpy-0.0.3/extern/eigen/Eigen/src/SVD/
+-rw-r--r--   0 runner    (1001) docker     (123)    54214 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32988 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14743 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.837439 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCholesky/
+-rw-r--r--   0 runner    (1001) docker     (123)    24216 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.845440 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24360 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25524 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13256 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57475 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17451 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15600 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25889 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.849439 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/
+-rw-r--r--   0 runner    (1001) docker     (123)    33316 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.849439 scranpy-0.0.3/extern/eigen/Eigen/src/SparseQR/
+-rw-r--r--   0 runner    (1001) docker     (123)    29167 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.853439 scranpy-0.0.3/extern/eigen/Eigen/src/StlSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.853439 scranpy-0.0.3/extern/eigen/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    34324 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.853439 scranpy-0.0.3/extern/eigen/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    24456 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.853439 scranpy-0.0.3/extern/eigen/Eigen/src/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/misc/Image.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30560 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/misc/blas.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/misc/lapack.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1058369 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.857439 scranpy-0.0.3/extern/eigen/Eigen/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21431 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    59020 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/Eigen/src/plugins/ReshapedMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.865440 scranpy-0.0.3/extern/eigen/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/BenchSparseUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/BenchTimer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/BenchUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    28983 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/analyze-blocking-sizes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/basicbench.cxxlist
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/basicbenchmark.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/basicbenchmark.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/benchBlasGemm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/benchCholesky.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/benchEigenSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/benchFFT.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/benchGeometry.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/benchVecAdd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/bench_gemm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/bench_move_semantics.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/bench_multi_compilers.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/bench_norm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/bench_reverse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/bench_sum.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/bench_unrolling
+-rw-r--r--   0 runner    (1001) docker     (123)    22259 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/benchmark-blocking-sizes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/benchmark.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/benchmarkSlice.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/benchmarkX.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/benchmarkXcwise.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1209 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/benchmark_suite
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.865440 scranpy-0.0.3/extern/eigen/bench/btl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.873439 scranpy-0.0.3/extern/eigen/bench/btl/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_aat_product.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_ata_product.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_atv_product.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_axpby.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_axpy.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_cholesky.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_ger.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_hessenberg.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_lu_decomp.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_lu_solve.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_matrix_matrix_product.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_matrix_matrix_product_bis.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_matrix_vector_product.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_partial_lu.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_rot.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_symv.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_syr2.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_trisolve.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_trisolve_matrix.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/action_trmm.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/actions/basic_actions.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.873439 scranpy-0.0.3/extern/eigen/bench/btl/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/cmake/FindACML.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/cmake/FindATLAS.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/cmake/FindBLAZE.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/cmake/FindBlitz.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/cmake/FindCBLAS.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/cmake/FindGMM.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/cmake/FindMKL.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/cmake/FindMTL4.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/cmake/FindOPENBLAS.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/cmake/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/cmake/FindTvmet.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/cmake/MacroOptionalAddSubdirectory.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.877440 scranpy-0.0.3/extern/eigen/bench/btl/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/data/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/data/action_settings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/data/gnuplot_common_settings.hh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2092 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/data/go_mean
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/data/mean.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/data/mk_gnuplot_script.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/data/mk_mean_script.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1742 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/data/mk_new_gnuplot.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/data/perlib_plot_settings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/data/regularize.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/data/smooth.cxx
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1687 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/data/smooth_all.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.877440 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/bench.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/bench_parameter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/btl.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.877440 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/init/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/init/init_function.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/init/init_matrix.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/init/init_vector.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.877440 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/static/bench_static.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/static/intel_bench_fixed_size.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/static/static_size_generator.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.881440 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/timers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/timers/STL_perf_analyzer.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/timers/STL_timer.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/timers/mixed_perf_analyzer.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/timers/portable_perf_analyzer.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/timers/portable_perf_analyzer_old.hh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3534 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/timers/portable_timer.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/timers/x86_perf_analyzer.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/timers/x86_timer.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.881440 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/utils/size_lin_log.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/utils/size_log.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/utils/utilities.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/generic_bench/utils/xy_file.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.713439 scranpy-0.0.3/extern/eigen/bench/btl/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.881440 scranpy-0.0.3/extern/eigen/bench/btl/libs/BLAS/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/BLAS/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35158 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/BLAS/blas.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/BLAS/blas_interface.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/BLAS/blas_interface_impl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/BLAS/c_interface_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/BLAS/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.885439 scranpy-0.0.3/extern/eigen/bench/btl/libs/STL/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/STL/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/STL/STL_interface.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/STL/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.885439 scranpy-0.0.3/extern/eigen/bench/btl/libs/blaze/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/blaze/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/blaze/blaze_interface.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/blaze/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.885439 scranpy-0.0.3/extern/eigen/bench/btl/libs/blitz/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/blitz/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/blitz/blitz_LU_solve_interface.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/blitz/blitz_interface.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/blitz/btl_blitz.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/blitz/btl_tiny_blitz.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/blitz/tiny_blitz_interface.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.885439 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen2/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen2/btl_tiny_eigen2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen2/eigen2_interface.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen2/main_adv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen2/main_linear.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen2/main_matmat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen2/main_vecmat.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.889439 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen3/btl_tiny_eigen3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen3/eigen3_interface.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen3/main_adv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen3/main_linear.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen3/main_matmat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/eigen3/main_vecmat.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.893440 scranpy-0.0.3/extern/eigen/bench/btl/libs/gmm/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/gmm/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/gmm/gmm_LU_solve_interface.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/gmm/gmm_interface.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/gmm/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.893440 scranpy-0.0.3/extern/eigen/bench/btl/libs/mtl4/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/mtl4/.kdbgrc.main
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/mtl4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/mtl4/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/mtl4/mtl4_LU_solve_interface.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/mtl4/mtl4_interface.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.897440 scranpy-0.0.3/extern/eigen/bench/btl/libs/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/tensors/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/tensors/main_linear.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/tensors/main_matmat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/tensors/main_vecmat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/tensors/tensor_interface.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.897440 scranpy-0.0.3/extern/eigen/bench/btl/libs/tvmet/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/tvmet/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/tvmet/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/tvmet/tvmet_interface.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.897440 scranpy-0.0.3/extern/eigen/bench/btl/libs/ublas/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/ublas/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/ublas/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/btl/libs/ublas/ublas_interface.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/check_cache_queries.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/dense_solvers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/eig33.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/geometry.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.901440 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/changesets.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/gemm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/gemm_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/gemm_settings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/gemm_square_settings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/gemv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/gemv_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/gemv_settings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/gemv_square_settings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/gemvt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/lazy_gemm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/lazy_gemm_settings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/llt.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2693 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/make_plot.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.905439 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/resources/chart_footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/resources/chart_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/resources/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/resources/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)   151723 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/resources/s1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   241320 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/resources/s2.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4090 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2031 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/runall.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/trmv_lo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/trmv_lot.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/trmv_up.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/perf_monitoring/trmv_upt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/product_threshold.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/quat_slerp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/quatmul.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/sparse_cholesky.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/sparse_dense_product.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/sparse_lu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/sparse_product.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/sparse_randomsetter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/sparse_setter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/sparse_transpose.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/sparse_trisolver.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.905439 scranpy-0.0.3/extern/eigen/bench/spbench/
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/spbench/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/spbench/sp_solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/spbench/spbench.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/spbench/spbenchsolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18167 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/spbench/spbenchsolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/spbench/spbenchstyle.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/spbench/test_sparseLU.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/spmv.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.909440 scranpy-0.0.3/extern/eigen/bench/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/tensors/README
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/tensors/benchmark.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/tensors/benchmark_main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/tensors/contraction_benchmarks_cpu.cc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      729 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/tensors/eigen_sycl_bench.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/tensors/eigen_sycl_bench_contract.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    20459 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/tensors/tensor_benchmarks.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/tensors/tensor_benchmarks_cpu.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/tensors/tensor_benchmarks_fp16_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/tensors/tensor_benchmarks_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/tensors/tensor_benchmarks_sycl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/tensors/tensor_contract_sycl_bench.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/bench/vdw_new.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.917440 scranpy-0.0.3/extern/eigen/blas/
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/BandTriangularSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/GeneralRank1Update.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/PackedSelfadjointProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/PackedTriangularMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/PackedTriangularSolverVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/Rank2Update.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/complex_double.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/complex_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/double.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.921440 scranpy-0.0.3/extern/eigen/blas/f2c/
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/chbmv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/chpmv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/complexdots.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/ctbmv.c
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/d_cnjg.c
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/datatypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/drotm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/drotmg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/dsbmv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/dspmv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/dtbmv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/lsame.c
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/r_cnjg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/srotm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/srotmg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/ssbmv.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8051 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/sspmv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/stbmv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/zhbmv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/zhpmv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18973 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/f2c/ztbmv.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.925440 scranpy-0.0.3/extern/eigen/blas/fortran/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/fortran/complexdots.f
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/level1_cplx_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/level1_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/level1_real_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/level2_cplx_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/level2_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/level2_real_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38043 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/level3_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/single.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.929440 scranpy-0.0.3/extern/eigen/blas/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    32110 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/cblat1.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/cblat2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   116657 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/cblat2.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/cblat3.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   131550 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/cblat3.f
+-rw-r--r--   0 runner    (1001) docker     (123)    44820 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/dblat1.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/dblat2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   112335 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/dblat2.f
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/dblat3.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   104262 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/dblat3.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/runblastest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    43389 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/sblat1.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/sblat2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   112251 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/sblat2.f
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/sblat3.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   104172 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/sblat3.f
+-rw-r--r--   0 runner    (1001) docker     (123)    32115 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/zblat1.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/zblat2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   117003 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/zblat2.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/zblat3.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   131995 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/testing/zblat3.f
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/blas/xerbla.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.933440 scranpy-0.0.3/extern/eigen/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/ci/CTest2JUnit.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/ci/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/ci/build.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/ci/smoketests.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/ci/test.gitlab-ci.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.945440 scranpy-0.0.3/extern/eigen/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/ComputeCppCompilerChecks.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/ComputeCppIRMap.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/Eigen3Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/Eigen3ConfigLegacy.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/EigenConfigureTesting.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/EigenDetermineOSVersion.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/EigenDetermineVSServicePack.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/EigenSmokeTestList.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    29205 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/EigenTesting.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/EigenUninstall.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindAdolc.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    42828 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindBLAS.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindBLASEXT.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindCHOLMOD.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindComputeCpp.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindEigen2.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindFFTW.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindGLEW.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindGMP.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindGSL.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindGoogleHash.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindHWLOC.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindKLU.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindLAPACK.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindMPFR.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindMPREAL.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindMetis.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindPASTIX.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindPTSCOTCH.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindSCOTCH.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindSPQR.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindStandardMathLibrary.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindSuperLU.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindTriSYCL.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/FindUMFPACK.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/RegexUtils.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/cmake/UseEigen3.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.717439 scranpy-0.0.3/extern/eigen/debug/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.945440 scranpy-0.0.3/extern/eigen/debug/gdb/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/debug/gdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/debug/gdb/printers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.945440 scranpy-0.0.3/extern/eigen/debug/msvc/
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/debug/msvc/eigen.natvis
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/debug/msvc/eigen_autoexp_part.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.945440 scranpy-0.0.3/extern/eigen/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.945440 scranpy-0.0.3/extern/eigen/demos/mandelbrot/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/mandelbrot/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/mandelbrot/README
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/mandelbrot/mandelbrot.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/mandelbrot/mandelbrot.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.949440 scranpy-0.0.3/extern/eigen/demos/mix_eigen_and_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/mix_eigen_and_c/README
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/mix_eigen_and_c/binary_library.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/mix_eigen_and_c/binary_library.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/mix_eigen_and_c/example.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.953440 scranpy-0.0.3/extern/eigen/demos/opengl/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/opengl/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/opengl/README
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/opengl/camera.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/opengl/camera.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/opengl/gpuhelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/opengl/gpuhelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/opengl/icosphere.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/opengl/icosphere.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19192 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/opengl/quaternion_demo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/opengl/quaternion_demo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/opengl/trackball.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/demos/opengl/trackball.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.977440 scranpy-0.0.3/extern/eigen/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/AsciiQuickReference.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/B01_Experimental.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/ClassHierarchy.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/CoeffwiseMathFunctionsTable.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/CustomizingEigen_CustomScalar.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/CustomizingEigen_InheritingMatrix.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/CustomizingEigen_NullaryExpr.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/CustomizingEigen_Plugins.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/DenseDecompositionBenchmark.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    86035 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/Doxyfile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/Eigen_Silly_Professor_64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/FixedSizeVectorizable.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/FunctionsTakingEigenTypes.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/HiPerformance.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/InplaceDecomposition.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    30585 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/InsideEigenExample.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/LeastSquares.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/Manual.dox
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/MatrixfreeSolverExample.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/NewExpressionType.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/Overview.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/PassingByValue.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/Pitfalls.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    14277 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/PreprocessorDirectives.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    29844 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/QuickReference.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/QuickStartGuide.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    19902 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/SparseLinearSystems.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/SparseQuickReference.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/StlContainers.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/StorageOrders.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/StructHavingEigenMembers.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TemplateKeyword.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TopicAliasing.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TopicAssertions.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TopicCMakeGuide.dox
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TopicEigenExpressionTemplates.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TopicLazyEvaluation.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TopicLinearAlgebraDecompositions.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TopicMultithreading.dox
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TopicResizing.dox
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TopicScalarTypes.dox
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TopicVectorization.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TutorialAdvancedInitialization.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TutorialArrayClass.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TutorialBlockOperations.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TutorialGeometry.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TutorialLinearAlgebra.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TutorialMapClass.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TutorialMatrixArithmetic.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    13680 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TutorialMatrixClass.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TutorialReductionsVisitorsBroadcasting.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TutorialReshape.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TutorialSTL.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TutorialSlicingIndexing.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    20483 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TutorialSparse.dox
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/TutorialSparse_example_details.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/UnalignedArrayAssert.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/UsingBlasLapackBackends.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/UsingIntelMKL.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/UsingNVCC.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/WrongStackAlignment.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/eigen_navtree_hacks.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/eigendoxy.css
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/eigendoxy_footer.html.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/eigendoxy_header.html.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/eigendoxy_layout.xml.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/eigendoxy_tabs.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.001440 scranpy-0.0.3/extern/eigen/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/.krazy
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/CustomizingEigen_Inheritance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Cwise_erf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Cwise_erfc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Cwise_lgamma.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/DenseBase_middleCols_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/DenseBase_middleRows_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/DenseBase_template_int_middleCols.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/DenseBase_template_int_middleRows.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/QuickStart_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/QuickStart_example2_dynamic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/QuickStart_example2_fixed.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/TemplateKeyword_flexible.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/TemplateKeyword_simple.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/TutorialInplaceLU.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/TutorialLinAlgComputeTwice.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/TutorialLinAlgExComputeSolveError.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/TutorialLinAlgExSolveColPivHouseholderQR.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/TutorialLinAlgExSolveLDLT.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/TutorialLinAlgInverseDeterminant.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/TutorialLinAlgRankRevealing.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/TutorialLinAlgSVDSolve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/TutorialLinAlgSelfAdjointEigenSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/TutorialLinAlgSetThreshold.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ArrayClass_accessors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ArrayClass_addition.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ArrayClass_cwise_other.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ArrayClass_interop.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ArrayClass_interop_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ArrayClass_mult.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_BlockOperations_block_assignment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_BlockOperations_colrow.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_BlockOperations_corner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_BlockOperations_print_block.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_BlockOperations_vector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_PartialLU_solve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_1nn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_broadcast_simple_rowwise.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_colwise.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_maxnorm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_bool.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_norm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_reductions_operatornorm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_rowwise.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_ReductionsVisitorsBroadcasting_visitors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_simple_example_dynamic_size.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/Tutorial_simple_example_fixed_size.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/class_Block.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/class_CwiseBinaryOp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/class_CwiseUnaryOp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/class_CwiseUnaryOp_ptrfun.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/class_FixedBlock.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/class_FixedReshaped.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/class_FixedVectorBlock.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/class_Reshaped.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/class_VectorBlock.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/function_taking_eigenbase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/function_taking_ref.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/make_circulant.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/make_circulant.cpp.entry
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/make_circulant.cpp.evaluator
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/make_circulant.cpp.expression
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/make_circulant.cpp.main
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/make_circulant.cpp.preamble
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/make_circulant.cpp.traits
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/make_circulant2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/matrixfree_cg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/nullary_indexing.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/tut_arithmetic_add_sub.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/tut_arithmetic_dot_cross.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/tut_arithmetic_matrix_mul.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/tut_arithmetic_redux_basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/tut_arithmetic_scalar_mul_div.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/tut_matrix_coefficient_accessors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/tut_matrix_resize.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/examples/tut_matrix_resize_fixed_size.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/ftv2node.png
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/ftv2pnode.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.097440 scranpy-0.0.3/extern/eigen/doc/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/.krazy
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/AngleAxis_mimic_euler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Array_initializer_list_23_cxx11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Array_initializer_list_vector_cxx11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Array_variadic_ctor_cxx11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/BiCGSTAB_simple.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/BiCGSTAB_step_by_step.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/ColPivHouseholderQR_solve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/ComplexEigenSolver_compute.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/ComplexEigenSolver_eigenvalues.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/ComplexEigenSolver_eigenvectors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/ComplexSchur_compute.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/ComplexSchur_matrixT.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/ComplexSchur_matrixU.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_abs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_abs2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_acos.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_arg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_array_power_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_asin.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_atan.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_boolean_and.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_boolean_not.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_boolean_or.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_boolean_xor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_ceil.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_cos.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_cosh.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_cube.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_equal_equal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_exp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_floor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_greater.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_greater_equal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_inverse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_isFinite.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_isInf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_isNaN.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_less.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_less_equal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_log.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_log10.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_max.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_min.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_minus.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_minus_equal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_not_equal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_plus.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_plus_equal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_pow.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_product.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_quotient.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_rint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_round.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_scalar_power_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_sign.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_sin.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_sinh.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_slash_equal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_sqrt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_square.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_tan.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_tanh.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Cwise_times_equal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/DenseBase_LinSpaced.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/DenseBase_LinSpacedInt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/DenseBase_LinSpaced_seq_deprecated.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/DenseBase_setLinSpaced.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/DirectionWise_hnormalized.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/DirectionWise_replicate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/DirectionWise_replicate_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/EigenSolver_EigenSolver_MatrixType.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/EigenSolver_compute.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/EigenSolver_eigenvalues.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/EigenSolver_eigenvectors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/EigenSolver_pseudoEigenvectors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/FullPivHouseholderQR_solve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/FullPivLU_image.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/FullPivLU_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/FullPivLU_solve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/GeneralizedEigenSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/HessenbergDecomposition_compute.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/HessenbergDecomposition_matrixH.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/HessenbergDecomposition_packedMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/HouseholderQR_householderQ.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/HouseholderQR_solve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/HouseholderSequence_HouseholderSequence.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/IOFormat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/JacobiSVD_basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Jacobi_makeGivens.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Jacobi_makeJacobi.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/LLT_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/LLT_solve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/LeastSquaresNormalEquations.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/LeastSquaresQR.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Map_general_stride.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Map_inner_stride.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Map_outer_stride.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Map_placement_new.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Map_simple.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_adjoint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_all.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_applyOnTheLeft.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_applyOnTheRight.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_array_const.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_asDiagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_block_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_block_int_int_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_bottomLeftCorner_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_bottomRightCorner_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_bottomRows_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_cast.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_col.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_colwise.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_colwise_iterator_cxx11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_computeInverseAndDetWithCheck.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_computeInverseWithCheck.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_cwiseAbs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_cwiseAbs2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_cwiseArg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_cwiseEqual.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_cwiseInverse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_cwiseMax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_cwiseMin.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_cwiseNotEqual.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_cwiseProduct.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_cwiseQuotient.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_cwiseSign.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_cwiseSqrt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_diagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_diagonal_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_diagonal_template_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_eigenvalues.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_end_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_eval.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_fixedBlock_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_hnormalized.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_homogeneous.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_identity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_identity_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_inverse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_isDiagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_isIdentity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_isOnes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_isOrthogonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_isUnitary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_isZero.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_leftCols_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_noalias.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_ones.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_ones_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_ones_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_operatorNorm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_prod.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_random.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_random_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_random_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_replicate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_replicate_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_reshaped_auto.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_reshaped_fixed.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_reshaped_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_reshaped_to_vector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_reverse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_rightCols_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_row.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_rowwise.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_segment_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_select.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_selfadjointView.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_set.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_setIdentity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_setOnes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_setRandom.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_setZero.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_start_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_bottomRows.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_end.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_int_block_int_int_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_int_bottomLeftCorner_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_int_bottomRightCorner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_int_bottomRightCorner_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_int_topLeftCorner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_int_topLeftCorner_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_int_topRightCorner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_int_topRightCorner_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_leftCols.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_rightCols.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_segment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_start.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_template_int_topRows.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_topLeftCorner_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_topRightCorner_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_topRows_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_transpose.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_triangularView.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_zero.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_zero_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/MatrixBase_zero_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_Map_stride.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_initializer_list_23_cxx11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_initializer_list_vector_cxx11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_resize_NoChange_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_resize_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_resize_int_NoChange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_resize_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_setConstant_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_setConstant_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_setIdentity_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_setOnes_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_setOnes_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_setRandom_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_setRandom_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_setZero_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_setZero_int_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Matrix_variadic_ctor_cxx11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/PartialPivLU_solve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/PartialRedux_count.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/PartialRedux_maxCoeff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/PartialRedux_minCoeff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/PartialRedux_norm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/PartialRedux_prod.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/PartialRedux_squaredNorm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/PartialRedux_sum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/RealQZ_compute.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/RealSchur_RealSchur_MatrixType.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/RealSchur_compute.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/SelfAdjointEigenSolver_SelfAdjointEigenSolver_MatrixType2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/SelfAdjointEigenSolver_compute_MatrixType2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/SelfAdjointEigenSolver_eigenvalues.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/SelfAdjointEigenSolver_eigenvectors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/SelfAdjointEigenSolver_operatorInverseSqrt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/SelfAdjointEigenSolver_operatorSqrt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/SelfAdjointView_eigenvalues.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/SelfAdjointView_operatorNorm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Slicing_arrayexpr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Slicing_custom_padding_cxx11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Slicing_rawarray_cxx11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Slicing_stdvector_cxx11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/SparseMatrix_coeffs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/TopicAliasing_block.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/TopicAliasing_block_correct.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/TopicAliasing_cwise.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/TopicAliasing_mult1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/TopicAliasing_mult2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/TopicAliasing_mult3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/TopicAliasing_mult4.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/TopicAliasing_mult5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/TopicStorageOrders_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Triangular_solve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tridiagonalization_Tridiagonalization_MatrixType.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tridiagonalization_compute.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tridiagonalization_decomposeInPlace.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tridiagonalization_diagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tridiagonalization_householderCoefficients.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tridiagonalization_packedMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_AdvancedInitialization_Block.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_AdvancedInitialization_CommaTemporary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_AdvancedInitialization_Join.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_AdvancedInitialization_LinSpaced.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_AdvancedInitialization_ThreeWays.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_AdvancedInitialization_Zero.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_Map_rowmajor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_Map_using.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_ReshapeMat2Mat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_ReshapeMat2Vec.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_SlicingCol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_SlicingVec.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_commainit_01.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_commainit_01b.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_commainit_02.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_range_for_loop_1d_cxx11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_range_for_loop_2d_cxx11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_reshaped_vs_resize_1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_reshaped_vs_resize_2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_solve_matrix_inverse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_solve_multiple_rhs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_solve_reuse_decomposition.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_solve_singular.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_solve_triangular.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_solve_triangular_inplace.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_std_sort.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Tutorial_std_sort_rows_cxx11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/VectorwiseOp_homogeneous.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/Vectorwise_reverse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/class_FullPivLU.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/compile_snippet.cpp.in
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/tut_arithmetic_redux_minmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/tut_arithmetic_transpose_aliasing.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/tut_arithmetic_transpose_conjugate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/tut_arithmetic_transpose_inplace.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/snippets/tut_matrix_assignment_resizing.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.097440 scranpy-0.0.3/extern/eigen/doc/special_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/special_examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/special_examples/Tutorial_sparse_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/special_examples/Tutorial_sparse_example_details.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/special_examples/random_cpp11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/doc/tutorial.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/eigen3.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.121440 scranpy-0.0.3/extern/eigen/failtest/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/bdcsvd_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/block_nonconst_ctor_on_const_xpr_0.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/block_nonconst_ctor_on_const_xpr_1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/block_nonconst_ctor_on_const_xpr_2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/block_on_const_type_actually_const_0.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/block_on_const_type_actually_const_1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/colpivqr_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/const_qualified_block_method_retval_0.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/const_qualified_block_method_retval_1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/const_qualified_diagonal_method_retval.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/const_qualified_transpose_method_retval.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/cwiseunaryview_nonconst_ctor_on_const_xpr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/cwiseunaryview_on_const_type_actually_const.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/diagonal_nonconst_ctor_on_const_xpr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/diagonal_on_const_type_actually_const.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/eigensolver_cplx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/eigensolver_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/failtest_sanity_check.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/fullpivlu_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/fullpivqr_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/initializer_list_1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/initializer_list_2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/jacobisvd_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/ldlt_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/llt_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/map_nonconst_ctor_on_const_ptr_0.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/map_nonconst_ctor_on_const_ptr_1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/map_nonconst_ctor_on_const_ptr_2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/map_nonconst_ctor_on_const_ptr_3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/map_nonconst_ctor_on_const_ptr_4.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/map_on_const_type_actually_const_0.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/map_on_const_type_actually_const_1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/partialpivlu_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/qr_int.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/ref_1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/ref_2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/ref_3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/ref_4.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/ref_5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/selfadjointview_nonconst_ctor_on_const_xpr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/selfadjointview_on_const_type_actually_const.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/sparse_ref_1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/sparse_ref_2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/sparse_ref_3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/sparse_ref_4.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/sparse_ref_5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/sparse_storage_mismatch.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/swap_1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/swap_2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/ternary_1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/ternary_2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/transpose_nonconst_ctor_on_const_xpr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/transpose_on_const_type_actually_const.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/triangularview_nonconst_ctor_on_const_xpr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/failtest/triangularview_on_const_type_actually_const.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.137440 scranpy-0.0.3/extern/eigen/lapack/
+-rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/cholesky.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/clacgv.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/cladiv.f
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/clarf.f
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/clarfb.f
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/clarfg.f
+-rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/clarft.f
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/complex_double.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/complex_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/dladiv.f
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/dlamch.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/dlapy2.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/dlapy3.f
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/dlarf.f
+-rw-r--r--   0 runner    (1001) docker     (123)    22749 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/dlarfb.f
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/dlarfg.f
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/dlarft.f
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/double.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/dsecnd_NONE.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/eigenvalues.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/ilaclc.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/ilaclr.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/iladlc.f
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/iladlr.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/ilaslc.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/ilaslr.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/ilazlc.f
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/ilazlr.f
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/lapack_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/lu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/second_NONE.f
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/single.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/sladiv.f
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/slamch.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/slapy2.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/slapy3.f
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/slarf.f
+-rw-r--r--   0 runner    (1001) docker     (123)    22727 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/slarfb.f
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/slarfg.f
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/slarft.f
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/svd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/zlacgv.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/zladiv.f
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/zlarf.f
+-rw-r--r--   0 runner    (1001) docker     (123)    23498 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/zlarfb.f
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/zlarfg.f
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/lapack/zlarft.f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.141440 scranpy-0.0.3/extern/eigen/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/scripts/CMakeLists.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      577 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/scripts/buildtests.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/scripts/cdashtesting.cmake.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)      670 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/scripts/check.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/scripts/debug.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/scripts/eigen_gen_credits.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/scripts/eigen_gen_docs
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/scripts/eigen_gen_split_test_help.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1009 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/scripts/eigen_monitor_perf.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/scripts/release.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/scripts/relicense.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/signature_of_eigen3_matrix_library
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.205440 scranpy-0.0.3/extern/eigen/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/AnnoyingScalar.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14452 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/MovableScalar.h
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/SafeScalar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/adjoint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27758 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/array_cwise.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/array_for_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/array_of_string.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/array_replicate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/array_reverse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/bandmatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/basicstuff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/bdcsvd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/bfloat16_float.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/bicgstab.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/blasutil.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/block.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/boostmultiprec.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/bug1213.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/bug1213.h
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/bug1213_main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18340 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/cholesky.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/cholmod_support.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/commainitializer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/conjugate_gradient.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/conservative_resize.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/constructor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/corners.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/ctorleak.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/denseLM.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/dense_storage.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/determinant.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/diagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/diagonal_matrix_variadic_ctor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/diagonalmatrices.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/dontalign.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/dynalloc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/eigen2support.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/eigensolver_complex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/eigensolver_generalized_real.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/eigensolver_generic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/eigensolver_selfadjoint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/evaluator_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/evaluators.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/exceptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/fastmath.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/first_aligned.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18093 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/geo_alignedbox.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/geo_eulerangles.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/geo_homogeneous.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/geo_hyperplane.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/geo_orthomethods.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/geo_parametrizedline.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/geo_quaternion.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26366 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/geo_transformations.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/gpu_basic.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/gpu_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/half_float.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/hessenberg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/householder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/incomplete_cholesky.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19424 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/indexed_view.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12744 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/initializer_list_construction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/inplace_decomposition.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/integer_types.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/inverse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/io.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/is_same_dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/jacobi.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/jacobisvd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/klu_support.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/linearstructure.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/lscg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/lu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    33109 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/main.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/mapped_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/mapstaticmethods.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/mapstride.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/meta.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/metis_support.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/miscmatrices.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17824 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/mixingtypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/mpl2only.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/nestbyvalue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/nesting_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/nomalloc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/nullary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/num_dimensions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/numext.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    55436 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/packetmath.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/packetmath_test_shared.h
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/pardiso_support.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/pastix_support.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/permutationmatrices.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/prec_inverse_4x4.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/product.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/product_extra.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/product_large.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/product_mmtr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/product_notemporary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/product_selfadjoint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12656 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/product_small.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/product_symm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/product_syrk.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/product_trmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/product_trmv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/product_trsolve.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/qr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/qr_colpivoting.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/qr_fullpivoting.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/qtvector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/rand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/random_without_cast_overflow.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/real_qz.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/redux.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14363 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/ref.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/reshape.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/resize.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/rvalue_types.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/schur_complex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/schur_real.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/selfadjoint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/simplicial_cholesky.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/sizeof.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/sizeoverflow.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/smallvectors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/solverbase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/sparse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/sparseLM.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    29343 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/sparse_basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/sparse_block.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/sparse_permutations.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25557 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/sparse_product.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/sparse_ref.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24396 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/sparse_solver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/sparse_solvers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/sparse_vector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/sparselu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/sparseqr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/special_numbers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   159516 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/split_test_helper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/spqr_support.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/stable_norm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/stddeque.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/stddeque_overload.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/stdlist.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/stdlist_overload.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/stdvector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/stdvector_overload.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19411 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/stl_iterators.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/superlu_support.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19317 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/svd_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/svd_fill.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/swap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/symbolic_index.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/triangular.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/type_alias.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/umeyama.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/umfpack_support.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/unalignedcount.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/upperbidiagonalization.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20351 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/vectorization_logic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11489 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/vectorwiseop.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/visitor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/test/zerosized.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.205440 scranpy-0.0.3/extern/eigen/unsupported/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.213441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/AdolcForward
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/AlignedVector3
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/ArpackSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/AutoDiff
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/BVH
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.213441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/Tensor
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/TensorSymmetry
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/ThreadPool
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.721439 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.241441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)    62365 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21269 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57932 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    60851 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42150 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15665 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45320 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
+-rw-r--r--   0 runner    (1001) docker     (123)    63402 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    89042 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    70687 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48686 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27527 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12837 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40367 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40005 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26655 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24345 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28066 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25692 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
+-rw-r--r--   0 runner    (1001) docker     (123)    43284 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28764 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44395 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30074 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14793 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16938 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20091 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25279 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30089 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.241441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/TensorSymmetry/
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.241441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/TensorSymmetry/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.245441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/ThreadPool/
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11482 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.245441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    22752 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/util/EmulateArray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/EulerAngles
+-rw-r--r--   0 runner    (1001) docker     (123)    13948 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/FFT
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/IterativeSolvers
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/KroneckerProduct
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/LevenbergMarquardt
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/MPRealSupport
+-rw-r--r--   0 runner    (1001) docker     (123)    17919 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/MatrixFunctions
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/MoreVectorization
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/NonLinearOptimization
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/NumericalDiff
+-rw-r--r--   0 runner    (1001) docker     (123)    19072 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/OpenGLSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/Polynomials
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/Skyline
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/SparseExtra
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/SpecialFunctions
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/Splines
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.725439 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.249441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/AutoDiff/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29107 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.249441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/BVH/
+-rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/BVH/BVAlgorithms.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/BVH/KdBVH.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.249441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner    (1001) docker     (123)    29075 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.253440 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/EulerAngles/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/EulerAngles/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/EulerAngles/EulerAngles.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/EulerAngles/EulerSystem.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.253440 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/FFT/
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/FFT/ei_fftw_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13231 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.253440 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/IterativeSolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17769 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/IterativeSolvers/GMRES.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14794 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/IterativeSolvers/IDRS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/IterativeSolvers/IterationController.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/IterativeSolvers/MINRES.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/IterativeSolvers/Scaling.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.257441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/KroneckerProduct/
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.257441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/LevenbergMarquardt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/LevenbergMarquardt/CopyrightMINPACK.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.257441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/MatrixFunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)    16624 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22671 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17557 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23422 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14212 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.257441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/MoreVectorization/
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.261441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/NonLinearOptimization/
+-rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22135 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/NonLinearOptimization/chkder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/NonLinearOptimization/covar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.261441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/NumericalDiff/
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.265441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Polynomials/
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Polynomials/Companion.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.265441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Skyline/
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Skyline/SkylineMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Skyline/SkylineProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Skyline/SkylineStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Skyline/SkylineUtil.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.269441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SparseExtra/
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40316 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SparseExtra/MarketIO.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SparseExtra/RandomSetter.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.273441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)    10015 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69632 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    58539 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.725439 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/arch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.273441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/arch/AVX/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.273441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.273441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/arch/GPU/
+-rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.273441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.273441 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Splines/
+-rw-r--r--   0 runner    (1001) docker     (123)    18307 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Splines/Spline.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Splines/SplineFitting.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/Eigen/src/Splines/SplineFwd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.273441 scranpy-0.0.3/extern/eigen/unsupported/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/bench/bench_svd.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.277441 scranpy-0.0.3/extern/eigen/unsupported/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/Overview.dox
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/SYCL.dox
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/eigendoxy_layout.xml.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.281441 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/BVH_Example.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/EulerAngles.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/FFT.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/MatrixExponential.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/MatrixFunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/MatrixLogarithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/MatrixPower.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/MatrixPower_optimal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/MatrixSine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/MatrixSinh.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/MatrixSquareRoot.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/PolynomialSolver1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/PolynomialUtils1.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.281441 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/SYCL/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/SYCL/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/examples/SYCL/CwiseMul.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.281441 scranpy-0.0.3/extern/eigen/unsupported/doc/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/doc/snippets/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.329441 scranpy-0.0.3/extern/eigen/unsupported/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/BVH.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/EulerAngles.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/FFT.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/FFTW.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    64597 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/NonLinearOptimization.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/NumericalDiff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/alignedvector3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/autodiff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/autodiff_scalar.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16409 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/bessel_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_eventcount.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_maxsizevector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18740 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_meta.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_non_blocking_thread_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_runqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_argmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_argmax_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_argmax_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_assign.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22378 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_block_access.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31888 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_block_eval.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15858 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_block_io.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_broadcast_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_broadcasting.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15767 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_builtins_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_cast_float16_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_casts.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_chipping.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26158 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_chipping_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_comparisons.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_complex_cwise_ops_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_complex_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_concatenation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_concatenation_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_const.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_contract_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    47521 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_contract_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23176 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_contraction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_convolution.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_convolution_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_custom_index.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_custom_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_custom_op_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_device.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_device_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_dimension.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_empty.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30675 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_executor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14224 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_expr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13705 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_fft.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_fixed_size.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_forced_eval.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_forced_eval_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_generator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_generator_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    58446 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_ifft.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_image_op_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    36037 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_image_patch.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    62111 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_image_patch_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18652 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_index_list.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_inflation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_inflation_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_intdiv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_io.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_layout_swap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_layout_swap_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_lvalue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_map.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_math.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_math_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_mixed_indices.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_morphing.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17549 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_morphing_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_move.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_notification.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_of_complex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_of_const_values.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21223 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_of_float16_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_of_strings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_padding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_padding_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_patch.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_patch_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_random.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_random_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_random_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15346 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_reduction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_reduction_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    42176 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_reduction_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_ref.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_reverse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_reverse_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_roundings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_scan.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_scan_gpu.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_scan_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_shuffling.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_shuffling_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_simple.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_striding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_striding_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_sugar.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14828 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    59079 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_symmetry.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_thread_local.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25491 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_thread_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_trace.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_uint128.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_volume_patch.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/cxx11_tensor_volume_patch_sycl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/dgmres.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/forward_adolc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/gmres.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/idrs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/kronecker_product.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    55504 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/levenberg_marquardt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/matrix_exponential.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/matrix_function.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/matrix_functions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/matrix_power.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/matrix_square_root.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/minres.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/mpreal_support.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18637 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/openglsupport.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/polynomialsolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/polynomialutils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/sparse_extra.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22854 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/special_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/special_packetmath.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-07-31 05:39:39.000000 scranpy-0.0.3/extern/eigen/unsupported/test/splines.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.333441 scranpy-0.0.3/extern/hnswlib/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 05:39:31.000000 scranpy-0.0.3/extern/hnswlib/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.725439 scranpy-0.0.3/extern/hnswlib/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.333441 scranpy-0.0.3/extern/hnswlib/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/ALGO_PARAMS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/TESTING_RECALL.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.725439 scranpy-0.0.3/extern/hnswlib/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.337441 scranpy-0.0.3/extern/hnswlib/examples/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/examples/cpp/EXAMPLES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/examples/cpp/example_filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/examples/cpp/example_mt_filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/examples/cpp/example_mt_replace_deleted.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/examples/cpp/example_mt_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/examples/cpp/example_replace_deleted.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/examples/cpp/example_search.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.337441 scranpy-0.0.3/extern/hnswlib/examples/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/examples/python/EXAMPLES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/examples/python/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/examples/python/example_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/examples/python/example_replace_deleted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/examples/python/example_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/examples/python/example_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/examples/python/pyw_hnswlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.341441 scranpy-0.0.3/extern/hnswlib/hnswlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/hnswlib/bruteforce.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51105 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/hnswlib/hnswalg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/hnswlib/hnswlib.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/hnswlib/space_ip.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/hnswlib/space_l2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/hnswlib/visited_list_pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.341441 scranpy-0.0.3/extern/hnswlib/python_bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/python_bindings/LazyIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/python_bindings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38350 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/python_bindings/bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/python_bindings/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.725439 scranpy-0.0.3/extern/hnswlib/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.345441 scranpy-0.0.3/extern/hnswlib/tests/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/cpp/download_bigann.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/cpp/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/cpp/multiThreadLoad_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/cpp/multiThread_replace_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/cpp/searchKnnCloserFirst_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/cpp/searchKnnWithFilter_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/cpp/sift_1b.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/cpp/sift_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/cpp/update_gen_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/cpp/updates_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.349441 scranpy-0.0.3/extern/hnswlib/tests/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/python/bindings_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/python/bindings_test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/python/bindings_test_getdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/python/bindings_test_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/python/bindings_test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/python/bindings_test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/python/bindings_test_recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/python/bindings_test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/python/bindings_test_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/python/bindings_test_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/python/bindings_test_stress_mt_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/python/git_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/hnswlib/tests/python/speedtest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.353441 scranpy-0.0.3/extern/irlba/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-31 05:39:32.000000 scranpy-0.0.3/extern/irlba/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.725439 scranpy-0.0.3/extern/irlba/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.353441 scranpy-0.0.3/extern/irlba/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/.github/workflows/compare-irlba.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.353441 scranpy-0.0.3/extern/irlba/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/cmake/Config.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.353441 scranpy-0.0.3/extern/irlba/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)   108613 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.357441 scranpy-0.0.3/extern/irlba/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/extern/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.729439 scranpy-0.0.3/extern/irlba/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.357441 scranpy-0.0.3/extern/irlba/include/irlba/
+-rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/include/irlba/irlba.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/include/irlba/lanczos.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16424 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/include/irlba/parallel.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/include/irlba/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15647 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/include/irlba/wrappers.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.357441 scranpy-0.0.3/extern/irlba/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.361441 scranpy-0.0.3/extern/irlba/tests/R/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/tests/R/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/tests/R/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/tests/R/run.R
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/tests/R/test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.361441 scranpy-0.0.3/extern/irlba/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/tests/src/NormalSampler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/tests/src/compare.h
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/tests/src/custom_parallel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/tests/src/invariant.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/tests/src/irlba.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/tests/src/lanczos.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/tests/src/parallel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/tests/src/sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/tests/src/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-31 05:39:40.000000 scranpy-0.0.3/extern/irlba/tests/src/wrappers.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.365441 scranpy-0.0.3/extern/kmeans/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-31 05:39:32.000000 scranpy-0.0.3/extern/kmeans/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.729439 scranpy-0.0.3/extern/kmeans/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.365441 scranpy-0.0.3/extern/kmeans/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/.github/workflows/compare-kmeans.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.365441 scranpy-0.0.3/extern/kmeans/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/cmake/Config.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.365441 scranpy-0.0.3/extern/kmeans/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108617 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.365441 scranpy-0.0.3/extern/kmeans/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/extern/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.729439 scranpy-0.0.3/extern/kmeans/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.369441 scranpy-0.0.3/extern/kmeans/include/kmeans/
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/include/kmeans/Base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/include/kmeans/Details.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/include/kmeans/HartiganWong.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/include/kmeans/InitializeKmeansPP.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/include/kmeans/InitializeNone.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/include/kmeans/InitializePCAPartition.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/include/kmeans/InitializeRandom.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/include/kmeans/Kmeans.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/include/kmeans/Lloyd.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/include/kmeans/MiniBatch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/include/kmeans/QuickSearch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/include/kmeans/compute_centroids.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/include/kmeans/compute_wcss.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/include/kmeans/is_edge_case.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/include/kmeans/random.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.369441 scranpy-0.0.3/extern/kmeans/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.373441 scranpy-0.0.3/extern/kmeans/tests/R/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/tests/R/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/tests/R/run.R
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/tests/R/test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.373441 scranpy-0.0.3/extern/kmeans/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/tests/src/HartiganWong.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/tests/src/InitializeKmeansPP.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/tests/src/InitializePCAPartition.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/tests/src/InitializeRandom.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/tests/src/Kmeans.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/tests/src/Lloyd.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/tests/src/MiniBatch.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/tests/src/TestCore.h
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/kmeans/tests/src/custom_parallel.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.377441 scranpy-0.0.3/extern/knncolle/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 05:39:33.000000 scranpy-0.0.3/extern/knncolle/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.729439 scranpy-0.0.3/extern/knncolle/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.377441 scranpy-0.0.3/extern/knncolle/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.377441 scranpy-0.0.3/extern/knncolle/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/cmake/Config.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.377441 scranpy-0.0.3/extern/knncolle/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108628 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.377441 scranpy-0.0.3/extern/knncolle/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/extern/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.729439 scranpy-0.0.3/extern/knncolle/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.377441 scranpy-0.0.3/extern/knncolle/include/knncolle/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.377441 scranpy-0.0.3/extern/knncolle/include/knncolle/Annoy/
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/include/knncolle/Annoy/Annoy.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.377441 scranpy-0.0.3/extern/knncolle/include/knncolle/BruteForce/
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/include/knncolle/BruteForce/BruteForce.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.377441 scranpy-0.0.3/extern/knncolle/include/knncolle/Hnsw/
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/include/knncolle/Hnsw/Hnsw.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.377441 scranpy-0.0.3/extern/knncolle/include/knncolle/Kmknn/
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/include/knncolle/Kmknn/Kmknn.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.377441 scranpy-0.0.3/extern/knncolle/include/knncolle/VpTree/
+-rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/include/knncolle/VpTree/VpTree.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/include/knncolle/knncolle.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.381441 scranpy-0.0.3/extern/knncolle/include/knncolle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/include/knncolle/utils/Base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/include/knncolle/utils/NeighborQueue.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/include/knncolle/utils/distances.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/include/knncolle/utils/find_nearest_neighbors.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.381441 scranpy-0.0.3/extern/knncolle/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.381441 scranpy-0.0.3/extern/knncolle/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/tests/src/Annoy.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/tests/src/BruteForce.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/tests/src/Hnsw.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/tests/src/Kmknn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/tests/src/TestCore.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/tests/src/VpTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/knncolle/tests/src/find_nearest_neighbors.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.385441 scranpy-0.0.3/extern/libscran/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 05:39:34.000000 scranpy-0.0.3/extern/libscran/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.733439 scranpy-0.0.3/extern/libscran/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.385441 scranpy-0.0.3/extern/libscran/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.385441 scranpy-0.0.3/extern/libscran/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   109654 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.385441 scranpy-0.0.3/extern/libscran/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/extern/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.385441 scranpy-0.0.3/extern/libscran/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/gallery/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/gallery/minimal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/gallery/pca_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.733439 scranpy-0.0.3/extern/libscran/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.385441 scranpy-0.0.3/extern/libscran/include/scran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.385441 scranpy-0.0.3/extern/libscran/include/scran/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)    17638 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/aggregation/AggregateAcrossCells.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/aggregation/DownsampleByNeighbors.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.389441 scranpy-0.0.3/extern/libscran/include/scran/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)    15133 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/clustering/BuildSnnGraph.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16608 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/clustering/ClusterSnnGraph.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/clustering/igraph_utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.389441 scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/MatrixCalculator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    29152 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/PairwiseEffects.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    48761 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/ScoreMarkers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/SummarizeEffects.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/auc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/cohens_d.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/simple_diff.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7366 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/summarize_comparisons.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.393441 scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/
+-rw-r--r--   0 runner    (1001) docker     (123)    27251 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/MultiBatchPca.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18792 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/ResidualPca.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/ScaleByNeighbors.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/SimplePca.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/blocking.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/convert.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/wrappers.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.393441 scranpy-0.0.3/extern/libscran/include/scran/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/feature_selection/ChooseHvgs.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/feature_selection/FitVarianceTrend.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27677 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/feature_selection/ModelGeneVariances.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/feature_selection/blocked_variances.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.393441 scranpy-0.0.3/extern/libscran/include/scran/feature_set_enrichment/
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/feature_set_enrichment/HypergeometricTail.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/feature_set_enrichment/ScoreFeatureSet.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.397441 scranpy-0.0.3/extern/libscran/include/scran/normalization/
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/normalization/CenterSizeFactors.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/normalization/ChoosePseudoCount.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/normalization/GroupedSizeFactors.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/normalization/LogNormCounts.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/normalization/MedianSizeFactors.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/normalization/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.397441 scranpy-0.0.3/extern/libscran/include/scran/quality_control/
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/quality_control/ChooseOutlierFilters.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/quality_control/ComputeMedianMad.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/quality_control/FilterCells.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/quality_control/PerCellAdtQcMetrics.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/quality_control/PerCellCrisprQcMetrics.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30743 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/quality_control/PerCellQcMetrics.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/quality_control/PerCellRnaQcMetrics.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/quality_control/SuggestAdtQcFilters.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/quality_control/SuggestCrisprQcFilters.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/quality_control/SuggestRnaQcFilters.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/quality_control/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/scran.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.401441 scranpy-0.0.3/extern/libscran/include/scran/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/utils/average_vectors.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/utils/blocking.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/utils/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/utils/subset_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/include/scran/utils/vector_to_pointers.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.401441 scranpy-0.0.3/extern/libscran/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.733439 scranpy-0.0.3/extern/libscran/tests/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.401441 scranpy-0.0.3/extern/libscran/tests/src/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/aggregation/AggregateAcrossCells.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/aggregation/DownsampleByNeighbors.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.401441 scranpy-0.0.3/extern/libscran/tests/src/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/clustering/BuildSnnGraph.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/clustering/ClusterSnnGraph.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.401441 scranpy-0.0.3/extern/libscran/tests/src/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/data/Simulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/data/data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/data/data_sparse.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.405441 scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)    22508 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/MatrixCalculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/PairwiseEffects.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17375 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/ScoreMarkers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/auc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/cohens_d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/simple_diff.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/summarize_comparisons.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.405441 scranpy-0.0.3/extern/libscran/tests/src/dimensionality_reduction/
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/dimensionality_reduction/MultiBatchPca.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20523 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/dimensionality_reduction/ResidualPca.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/dimensionality_reduction/ScaleByNeighbors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/dimensionality_reduction/SimplePca.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/dimensionality_reduction/compare_pcs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/dimensionality_reduction/convert.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/dimensionality_reduction/utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.409441 scranpy-0.0.3/extern/libscran/tests/src/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/feature_selection/ChooseHvgs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/feature_selection/FitVarianceTrend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/feature_selection/ModelGeneVariances.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.409441 scranpy-0.0.3/extern/libscran/tests/src/feature_set_enrichment/
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/feature_set_enrichment/HypergeometricTail.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/feature_set_enrichment/ScoreFeatureSet.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.409441 scranpy-0.0.3/extern/libscran/tests/src/normalization/
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/normalization/CenterSizeFactors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/normalization/ChoosePseudoCount.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/normalization/GroupedSizeFactors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/normalization/LogNormCounts.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/normalization/MedianSizeFactors.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.409441 scranpy-0.0.3/extern/libscran/tests/src/quality_control/
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/quality_control/ChooseOutlierFilters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/quality_control/ComputeMedianMad.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/quality_control/FilterCells.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/quality_control/PerCellAdtQcMetrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/quality_control/PerCellCrisprQcMetrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15529 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/quality_control/PerCellQcMetrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/quality_control/PerCellRnaQcMetrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/quality_control/SuggestAdtQcFilters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/quality_control/SuggestCrisprQcFilters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/quality_control/SuggestRnaQcFilters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/quality_control/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.413441 scranpy-0.0.3/extern/libscran/tests/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/utils/average_vectors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/utils/blocking.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/utils/compare_almost_equal.h
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/utils/compare_vectors.h
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/utils/custom_parallel.h
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/utils/macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/libscran/tests/src/utils/subset_vector.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.413441 scranpy-0.0.3/extern/qdtsne/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-31 05:39:34.000000 scranpy-0.0.3/extern/qdtsne/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.737439 scranpy-0.0.3/extern/qdtsne/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.413441 scranpy-0.0.3/extern/qdtsne/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/.github/workflows/compare-Rtsne.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.413441 scranpy-0.0.3/extern/qdtsne/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108627 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.413441 scranpy-0.0.3/extern/qdtsne/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/extern/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.413441 scranpy-0.0.3/extern/qdtsne/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/gallery/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/gallery/speedtest.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.737439 scranpy-0.0.3/extern/qdtsne/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.417441 scranpy-0.0.3/extern/qdtsne/include/qdtsne/
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/include/qdtsne/gaussian.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12402 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/include/qdtsne/interpolate.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/include/qdtsne/qdtsne.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/include/qdtsne/sptree.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/include/qdtsne/symmetrize.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30222 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/include/qdtsne/tsne.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/include/qdtsne/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.417441 scranpy-0.0.3/extern/qdtsne/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.417441 scranpy-0.0.3/extern/qdtsne/tests/R/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/tests/R/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/tests/R/run.R
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/tests/R/test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.417441 scranpy-0.0.3/extern/qdtsne/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/tests/src/custom_parallel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/tests/src/gaussian.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/tests/src/interpolate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/tests/src/sptree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/tests/src/symmetrize.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/tests/src/tsne.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/qdtsne/tests/src/utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.421441 scranpy-0.0.3/extern/umappp/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/umappp/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.737439 scranpy-0.0.3/extern/umappp/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.421441 scranpy-0.0.3/extern/umappp/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/.github/workflows/compare-uwot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.421441 scranpy-0.0.3/extern/umappp/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/cmake/Config.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.421441 scranpy-0.0.3/extern/umappp/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108614 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.421441 scranpy-0.0.3/extern/umappp/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/extern/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.737439 scranpy-0.0.3/extern/umappp/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.421441 scranpy-0.0.3/extern/umappp/include/umappp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/include/umappp/NeighborList.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/include/umappp/Umap.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/include/umappp/combine_neighbor_sets.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/include/umappp/find_ab.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/include/umappp/neighbor_similarities.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19087 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/include/umappp/optimize_layout.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/include/umappp/spectral_init.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/include/umappp/umappp.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.421441 scranpy-0.0.3/extern/umappp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.425441 scranpy-0.0.3/extern/umappp/tests/R/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/tests/R/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/tests/R/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/tests/R/run.R
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/tests/R/test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.425441 scranpy-0.0.3/extern/umappp/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/tests/src/Umap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/tests/src/combine_neighbor_sets.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/tests/src/custom_parallel.h
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/tests/src/find_ab.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/tests/src/neighbor_similarities.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/tests/src/optimize_layout.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/umappp/tests/src/spectral_init.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.429441 scranpy-0.0.3/extern/weightedlowess/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-31 05:39:35.000000 scranpy-0.0.3/extern/weightedlowess/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.737439 scranpy-0.0.3/extern/weightedlowess/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.429441 scranpy-0.0.3/extern/weightedlowess/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/.github/workflows/compare-limma.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.429441 scranpy-0.0.3/extern/weightedlowess/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108663 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.737439 scranpy-0.0.3/extern/weightedlowess/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.429441 scranpy-0.0.3/extern/weightedlowess/include/WeightedLowess/
+-rw-r--r--   0 runner    (1001) docker     (123)    31431 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/include/WeightedLowess/WeightedLowess.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.429441 scranpy-0.0.3/extern/weightedlowess/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.429441 scranpy-0.0.3/extern/weightedlowess/tests/R/
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/tests/R/run.R
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/tests/R/test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.433441 scranpy-0.0.3/extern/weightedlowess/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/tests/src/basic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/tests/src/divzero.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/tests/src/options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/tests/src/runners.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/tests/src/ties.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/tests/src/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-31 05:39:41.000000 scranpy-0.0.3/extern/weightedlowess/tests/src/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-31 05:39:28.000000 scranpy-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-31 05:40:06.445441 scranpy-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-31 05:39:28.000000 scranpy-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:05.741439 scranpy-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.433441 scranpy-0.0.3/src/scranpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.437441 scranpy-0.0.3/src/scranpy/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/clustering/build_snn_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/cpphelpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.437441 scranpy-0.0.3/src/scranpy/dimensionality_reduction/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/dimensionality_reduction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/dimensionality_reduction/run_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/dimensionality_reduction/run_tsne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/dimensionality_reduction/run_umap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.437441 scranpy-0.0.3/src/scranpy/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/feature_selection/model_gene_variances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.441441 scranpy-0.0.3/src/scranpy/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/lib/build_snn_graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/lib/find_nearest_neighbors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/lib/log_norm_counts.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/lib/model_gene_variances.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/lib/parallel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/lib/per_cell_rna_qc_metrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/lib/run_pca.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/lib/run_tsne.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/lib/run_umap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/lib/suggest_rna_qc_filters.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.441441 scranpy-0.0.3/src/scranpy/nearest_neighbors/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/nearest_neighbors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/nearest_neighbors/build_neighbor_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/nearest_neighbors/find_nearest_neighbors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.441441 scranpy-0.0.3/src/scranpy/normalization/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/normalization/log_norm_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.441441 scranpy-0.0.3/src/scranpy/quality_control/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/quality_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/quality_control/rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-31 05:39:28.000000 scranpy-0.0.3/src/scranpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.433441 scranpy-0.0.3/src/scranpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-31 05:40:05.000000 scranpy-0.0.3/src/scranpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   107396 2023-07-31 05:40:05.000000 scranpy-0.0.3/src/scranpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 05:40:05.000000 scranpy-0.0.3/src/scranpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 05:40:04.000000 scranpy-0.0.3/src/scranpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 05:40:05.000000 scranpy-0.0.3/src/scranpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 05:40:05.000000 scranpy-0.0.3/src/scranpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.445441 scranpy-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-31 05:39:28.000000 scranpy-0.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:40:06.445441 scranpy-0.0.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-31 05:39:28.000000 scranpy-0.0.3/tests/data/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-31 05:39:28.000000 scranpy-0.0.3/tests/test_dimreds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-31 05:39:28.000000 scranpy-0.0.3/tests/test_log_norm_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-31 05:39:28.000000 scranpy-0.0.3/tests/test_model_gene_variances.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-31 05:39:28.000000 scranpy-0.0.3/tests/test_nearest_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-31 05:39:28.000000 scranpy-0.0.3/tests/test_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-31 05:39:28.000000 scranpy-0.0.3/tests/test_quality_control_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-31 05:39:28.000000 scranpy-0.0.3/tests/test_snn_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-31 05:39:28.000000 scranpy-0.0.3/tox.ini
```

### Comparing `scranpy-0.0.2/.coveragerc` & `scranpy-0.0.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/.github/workflows/pypi-test.yml` & `scranpy-0.0.3/.github/workflows/pypi-test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,19 @@
         uses: actions/setup-python@v2
         with:
           python-version: 3.9
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install flake8 pytest tox numpy mattress
+      - name: Download knncolle deps
+        run: |
+          cd extern/knncolle
+          cmake .
+          cd ../..
       - name: Test with tox
         run: |
           python setup.py build_ext --inplace
           tox
       - name: Build docs
         run: |
           tox -e docs
@@ -56,14 +61,20 @@
         os: [ubuntu-20.04, macos-11] # at some point get this to work on windows-2019
 
     steps:
       - uses: actions/checkout@v3
         with:
           submodules: true
 
+      - name: Download dependencies
+        run: |
+          cd extern/knncolle
+          cmake .
+          cd ../..
+
       - name: Build wheels
         uses: pypa/cibuildwheel@v2.12.1
         env:
           CIBW_ARCHS_MACOS: x86_64 arm64
           CIBW_ARCHS_LINUX: x86_64 # remove this later so we build for all linux archs
           CIBW_PROJECT_REQUIRES_PYTHON: ">=3.9"
           CIBW_SKIP: pp*
```

### Comparing `scranpy-0.0.2/.gitignore` & `scranpy-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/.readthedocs.yml` & `scranpy-0.0.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/CONTRIBUTING.md` & `scranpy-0.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/LICENSE.txt` & `scranpy-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/PKG-INFO` & `scranpy-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scranpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Analyze multi-modal single-cell data!
 Home-page: https://github.com/biocpy/scranpy
 Author: "Jayaram Kancherla, Aaron Lun"
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/biocpy/scranpy
 Platform: any
@@ -35,14 +35,16 @@
 ## Developer Notes
 
 
 Steps to setup dependencies - 
 
 - initialize git submodules in `extern/libscran`.
 
+- run `cmake .` inside the `extern/knncolle` to download the annoy library. a future version of this will use a cmake to setup the extern directory.
+
 First one needs to build the extern library, this would generate a shared object file to `src/scranpy/core-[*].so`
 
 ```shell
 python setup.py build_ext --inplace
 ```
 
 For typical development workflows, run this for tests
```

### Comparing `scranpy-0.0.2/README.md` & `scranpy-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 ## Developer Notes
 
 
 Steps to setup dependencies - 
 
 - initialize git submodules in `extern/libscran`.
 
+- run `cmake .` inside the `extern/knncolle` to download the annoy library. a future version of this will use a cmake to setup the extern directory.
+
 First one needs to build the extern library, this would generate a shared object file to `src/scranpy/core-[*].so`
 
 ```shell
 python setup.py build_ext --inplace
 ```
 
 For typical development workflows, run this for tests
```

### Comparing `scranpy-0.0.2/docs/Makefile` & `scranpy-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/docs/conf.py` & `scranpy-0.0.3/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 todo_emit_warnings = True
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = "alabaster"
+html_theme = "furo"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
     "sidebar_width": "300px",
     "page_width": "1200px"
```

### Comparing `scranpy-0.0.2/docs/index.md` & `scranpy-0.0.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/.github/workflows/doxygenate.yaml` & `scranpy-0.0.3/extern/aarand/.github/workflows/doxygenate.yaml`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/.github/workflows/run-tests.yaml` & `scranpy-0.0.3/extern/libscran/.github/workflows/run-tests.yaml`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/CMakeLists.txt` & `scranpy-0.0.3/extern/libscran/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/LICENSE` & `scranpy-0.0.3/extern/aarand/LICENSE`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/README.md` & `scranpy-0.0.3/extern/libscran/README.md`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/docs/Doxyfile` & `scranpy-0.0.3/extern/libscran/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/extern/CMakeLists.txt` & `scranpy-0.0.3/extern/libscran/extern/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/gallery/CMakeLists.txt` & `scranpy-0.0.3/extern/libscran/gallery/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/gallery/minimal.cpp` & `scranpy-0.0.3/extern/libscran/gallery/minimal.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/gallery/pca_test.cpp` & `scranpy-0.0.3/extern/libscran/gallery/pca_test.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/aggregation/AggregateAcrossCells.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/aggregation/AggregateAcrossCells.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/aggregation/DownsampleByNeighbors.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/aggregation/DownsampleByNeighbors.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/clustering/BuildSnnGraph.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/clustering/BuildSnnGraph.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -173,85 +173,27 @@
             igraph_vector_int_t edge_view;
             igraph_vector_int_view(&edge_view, edges.data(), edges.size());
             return igraph::Graph(&edge_view, ncells, /* directed = */ false);
         }
 #endif
     };
 
-    /**
-     * @param ndims Number of dimensions.
-     * @param ncells Number of cells.
-     * @param mat Pointer to an array of expression values or a low-dimensional representation thereof.
-     * Rows should be dimensions while columns should be cells.
-     * Data should be stored in column-major format.
-     *
-     * @return The edges and weights of the constructed SNN graph.
-     */
-    Results run(size_t ndims, size_t ncells, const double* mat) const {
-        std::unique_ptr<knncolle::Base<> > ptr;
-        if (!approximate) {
-            ptr.reset(new knncolle::VpTreeEuclidean<>(ndims, ncells, mat));
-        } else {
-            ptr.reset(new knncolle::AnnoyEuclidean<>(ndims, ncells, mat));
-        }
-        return run(ptr.get());
-    }
-
-    /**
-     * @tparam Algorithm Any instance of a `knncolle::Base` subclass.
-     *
-     * @param search Pointer to a `knncolle::Base` instance to use for the nearest-neighbor search.
-     *
-     * @return The edges and weights of the constructed SNN graph.
-     */
-    template<class Algorithm>
-    Results run(const Algorithm* search) const {
-        // Collecting neighbors.
-        size_t ncells = search->nobs();
-        std::vector<std::vector<int> > indices(ncells);
-
-#ifndef SCRAN_CUSTOM_PARALLEL
-        #pragma omp parallel for num_threads(nthreads)
-        for (size_t i = 0; i < ncells; ++i) {
-#else
-        SCRAN_CUSTOM_PARALLEL([&](size_t, size_t start, size_t length) -> void {
-        for (size_t i = start, end = start + length; i < end; ++i) {
-#endif
-            auto neighbors = search->find_nearest_neighbors(i, num_neighbors);
-            auto& current = indices[i];
-            for (auto x : neighbors) {
-                current.push_back(x.first);
-            }
-        }
-#ifdef SCRAN_CUSTOM_PARALLEL
-        }, ncells, nthreads);
-#endif
-
-        return run(indices);
-    }
-
-    /**
-     * @tparam Indices Vector of integer indices.
-     *
-     * @param indices Vector of indices of the neighbors for each cell, sorted by increasing distance.
-     *
-     * @return The edges and weights of the constructed SNN graph.
-     */
-    template<class Indices>
-    Results run(const std::vector<Indices>& indices) const {
+private:
+    template<class Indices_, class Function_>
+    Results run(const std::vector<Indices_>& indices, Function_ get_index) const {
         size_t ncells = indices.size();
 
         // Not parallel-frendly, so we don't construct this with the neighbor search
         std::vector<std::vector<std::pair<int, int> > > hosts(ncells);
         for (size_t i = 0; i < ncells; ++i) {
             hosts[i].push_back(std::make_pair(0, i)); // each point is its own 0-th nearest neighbor
             const auto& current = indices[i];
             int counter = 1;
             for (auto x : current) {
-                hosts[x].push_back(std::make_pair(counter, i));
+                hosts[get_index(x)].push_back(std::make_pair(counter, i));
                 ++counter;
             }
         }
 
         // Constructing the shared neighbor graph.
         std::vector<std::vector<int> > edge_stores(ncells);
         std::vector<std::vector<double> > weight_stores(ncells);
@@ -271,18 +213,20 @@
             #pragma omp for
             for (size_t j = 0; j < ncells; ++j) {
 #else
             for (size_t j = start, end = start + length; j < end; ++j) {
 #endif
 
                 const auto& current_neighbors = indices[j];
-                for (int i = 0; i <= current_neighbors.size(); ++i) {
+                int nneighbors = current_neighbors.size();
+
+                for (int i = 0; i <= nneighbors; ++i) {
                     // First iteration treats 'j' as the zero-th neighbor.
                     // Remaining iterations go through the neighbors of 'j'.
-                    const int cur_neighbor = (i==0 ? j : current_neighbors[i-1]);
+                    const int cur_neighbor = (i==0 ? j : get_index(current_neighbors[i-1]));
 
                     // Going through all observations 'h' for which 'cur_neighbor'
                     // is a nearest neighbor, a.k.a., 'cur_neighbor' is a shared
                     // neighbor of both 'h' and 'j'.
                     for (const auto& h : hosts[cur_neighbor]) {
                         auto othernode = h.second;
 
@@ -314,19 +258,19 @@
                 auto& current_weights = weight_stores[j];
                 current_weights.reserve(current_added.size() * 2);
 
                 for (auto othernode : current_added) {
                     int& otherscore = current_score[othernode];
                     double finalscore;
                     if (weight_scheme == RANKED) {
-                        finalscore = static_cast<double>(current_neighbors.size()) - 0.5 * static_cast<double>(otherscore);
+                        finalscore = static_cast<double>(nneighbors) - 0.5 * static_cast<double>(otherscore);
                     } else {
                         finalscore = otherscore;
                         if (weight_scheme == JACCARD) {
-                            finalscore = finalscore / (2 * (current_neighbors.size() + 1) - finalscore);
+                            finalscore = finalscore / (2 * (nneighbors + 1) - finalscore);
                         }
                     }
 
                     current_edges.push_back(j);
                     current_edges.push_back(othernode);
                     current_weights.push_back(std::max(finalscore, 1e-6)); // Ensuring that an edge with a positive weight is always reported.
 
@@ -362,12 +306,94 @@
         output.edges.reserve(nedges * 2);
         for (const auto& e : edge_stores) {
             output.edges.insert(output.edges.end(), e.begin(), e.end());
         }
 
         return output;
     }
+
+public:
+    /**
+     * @param ndims Number of dimensions.
+     * @param ncells Number of cells.
+     * @param mat Pointer to an array of expression values or a low-dimensional representation thereof.
+     * Rows should be dimensions while columns should be cells.
+     * Data should be stored in column-major format.
+     *
+     * @return The edges and weights of the constructed SNN graph.
+     */
+    Results run(size_t ndims, size_t ncells, const double* mat) const {
+        std::unique_ptr<knncolle::Base<> > ptr;
+        if (!approximate) {
+            ptr.reset(new knncolle::VpTreeEuclidean<>(ndims, ncells, mat));
+        } else {
+            ptr.reset(new knncolle::AnnoyEuclidean<>(ndims, ncells, mat));
+        }
+        return run(ptr.get());
+    }
+
+    /**
+     * @tparam Algorithm Any instance of a `knncolle::Base` subclass.
+     *
+     * @param search Pointer to a `knncolle::Base` instance to use for the nearest-neighbor search.
+     *
+     * @return The edges and weights of the constructed SNN graph.
+     */
+    template<class Algorithm>
+    Results run(const Algorithm* search) const {
+        // Collecting neighbors.
+        size_t ncells = search->nobs();
+        std::vector<std::vector<int> > indices(ncells);
+
+#ifndef SCRAN_CUSTOM_PARALLEL
+        #pragma omp parallel for num_threads(nthreads)
+        for (size_t i = 0; i < ncells; ++i) {
+#else
+        SCRAN_CUSTOM_PARALLEL([&](size_t, size_t start, size_t length) -> void {
+        for (size_t i = start, end = start + length; i < end; ++i) {
+#endif
+            auto neighbors = search->find_nearest_neighbors(i, num_neighbors);
+            auto& current = indices[i];
+            for (auto x : neighbors) {
+                current.push_back(x.first);
+            }
+        }
+#ifdef SCRAN_CUSTOM_PARALLEL
+        }, ncells, nthreads);
+#endif
+
+        return run(indices);
+    }
+
+    /**
+     * @tparam Index_ Integer type for the indices.
+     * @tparam Distance_ Floating-point type for the distances.
+     *
+     * @param neighbors Vector of indices and distances of the neighbors for each cell, sorted by increasing distance.
+     *
+     * @return The edges and weights of the constructed SNN graph.
+     *
+     * Distances are ignored here; this overload is only provided to enable convenient usage with pre-computed neighbors from **knncolle**.
+     */
+    template<typename Index_, typename Distance_>
+    Results run(const knncolle::NeighborList<Index_, Distance_>& neighbors) const {
+        return run(neighbors, [](const std::pair<Index_, Distance_>& x) -> Index_ { return x.first; });
+    }
+
+    /**
+     * @tparam Indices_ Vector-like class containing integer indices.
+     * This should provide the `[` and `size()` methods.
+     *
+     * @param indices Vector of indices of the neighbors for each cell, sorted by increasing distance.
+     *
+     * @return The edges and weights of the constructed SNN graph.
+     */
+    template<class Indices_>
+    Results run(const std::vector<Indices_>& indices) const {
+        typedef typename std::remove_cv<typename std::remove_reference<decltype(std::declval<Indices_>()[0])>::type>::type Element;
+        return run(indices, [](Element i) -> Element { return i; });
+    }
 };
 
 }
 
 #endif
```

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/clustering/ClusterSnnGraph.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/clustering/ClusterSnnGraph.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/clustering/igraph_utils.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/clustering/igraph_utils.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/MatrixCalculator.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/MatrixCalculator.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/PairwiseEffects.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/PairwiseEffects.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/ScoreMarkers.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/ScoreMarkers.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/SummarizeEffects.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/SummarizeEffects.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/auc.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/auc.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/cohens_d.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/cohens_d.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/simple_diff.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/simple_diff.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/differential_analysis/summarize_comparisons.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/differential_analysis/summarize_comparisons.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/MultiBatchPca.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/MultiBatchPca.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/ResidualPca.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/ResidualPca.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/ScaleByNeighbors.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/ScaleByNeighbors.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/SimplePca.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/SimplePca.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/blocking.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/blocking.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/convert.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/convert.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/utils.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/utils.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/dimensionality_reduction/wrappers.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/dimensionality_reduction/wrappers.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/feature_selection/ChooseHvgs.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/feature_selection/ChooseHvgs.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/feature_selection/FitVarianceTrend.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/feature_selection/FitVarianceTrend.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/feature_selection/ModelGeneVariances.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/feature_selection/ModelGeneVariances.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/feature_selection/blocked_variances.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/feature_selection/blocked_variances.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/feature_set_enrichment/HypergeometricTail.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/feature_set_enrichment/HypergeometricTail.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/feature_set_enrichment/ScoreFeatureSet.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/feature_set_enrichment/ScoreFeatureSet.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/normalization/CenterSizeFactors.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/normalization/CenterSizeFactors.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/normalization/ChoosePseudoCount.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/normalization/ChoosePseudoCount.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/normalization/GroupedSizeFactors.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/normalization/GroupedSizeFactors.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/normalization/LogNormCounts.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/normalization/LogNormCounts.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/normalization/MedianSizeFactors.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/normalization/MedianSizeFactors.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/normalization/utils.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/normalization/utils.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/quality_control/ChooseOutlierFilters.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/quality_control/ChooseOutlierFilters.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/quality_control/ComputeMedianMad.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/quality_control/ComputeMedianMad.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/quality_control/FilterCells.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/quality_control/FilterCells.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/quality_control/PerCellAdtQcMetrics.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/quality_control/PerCellAdtQcMetrics.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/quality_control/PerCellCrisprQcMetrics.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/quality_control/PerCellCrisprQcMetrics.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/quality_control/PerCellQcMetrics.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/quality_control/PerCellQcMetrics.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/quality_control/PerCellRnaQcMetrics.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/quality_control/PerCellRnaQcMetrics.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/quality_control/SuggestAdtQcFilters.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/quality_control/SuggestAdtQcFilters.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/quality_control/SuggestCrisprQcFilters.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/quality_control/SuggestCrisprQcFilters.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/quality_control/SuggestRnaQcFilters.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/quality_control/SuggestRnaQcFilters.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/quality_control/utils.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/quality_control/utils.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/scran.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/scran.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/utils/average_vectors.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/utils/average_vectors.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/utils/blocking.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/utils/blocking.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/utils/macros.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/utils/macros.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/utils/subset_vector.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/utils/subset_vector.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/include/scran/utils/vector_to_pointers.hpp` & `scranpy-0.0.3/extern/libscran/include/scran/utils/vector_to_pointers.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/CMakeLists.txt` & `scranpy-0.0.3/extern/libscran/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/aggregation/AggregateAcrossCells.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/aggregation/AggregateAcrossCells.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/aggregation/DownsampleByNeighbors.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/aggregation/DownsampleByNeighbors.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/clustering/BuildSnnGraph.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/clustering/BuildSnnGraph.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,21 @@
 
     scran::BuildSnnGraph builder;
     builder.set_neighbors(k).set_approximate(true);
 
     auto output = builder.run(ndim, nobs, data.data());
     EXPECT_EQ(output.ncells, nobs);
     EXPECT_TRUE(output.weights.size() > 1); // well, it gives _something_, at least.
+
+    // Same results as if we had run it manually.
+    knncolle::AnnoyEuclidean<> idx(ndim, nobs, data.data());
+    auto res = knncolle::find_nearest_neighbors(&idx, k, 1);
+    auto output2 = builder.run(res);
+    EXPECT_EQ(output.edges, output2.edges);
+    EXPECT_EQ(output.weights, output2.weights);
 }
 
 INSTANTIATE_TEST_SUITE_P(
     BuildSnnGraph,
     BuildSnnGraphAnnoyTest,
     ::testing::Combine(
         ::testing::Values(5, 10), // number of dimensions
```

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/clustering/ClusterSnnGraph.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/clustering/ClusterSnnGraph.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/data/Simulator.hpp` & `scranpy-0.0.3/extern/libscran/tests/src/data/Simulator.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/data/data_sparse.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/data/data_sparse.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/MatrixCalculator.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/MatrixCalculator.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/PairwiseEffects.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/PairwiseEffects.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/ScoreMarkers.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/ScoreMarkers.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/auc.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/auc.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/cohens_d.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/cohens_d.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/simple_diff.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/simple_diff.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/summarize_comparisons.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/summarize_comparisons.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/differential_analysis/utils.h` & `scranpy-0.0.3/extern/libscran/tests/src/differential_analysis/utils.h`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/MultiBatchPca.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/dimensionality_reduction/MultiBatchPca.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/ResidualPca.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/dimensionality_reduction/ResidualPca.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/ScaleByNeighbors.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/dimensionality_reduction/ScaleByNeighbors.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/SimplePca.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/dimensionality_reduction/SimplePca.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/compare_pcs.h` & `scranpy-0.0.3/extern/libscran/tests/src/dimensionality_reduction/compare_pcs.h`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/convert.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/dimensionality_reduction/convert.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/dimensionality_reduction/utils.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/dimensionality_reduction/utils.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/feature_selection/ChooseHvgs.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/feature_selection/ChooseHvgs.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/feature_selection/FitVarianceTrend.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/feature_selection/FitVarianceTrend.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/feature_selection/ModelGeneVariances.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/feature_selection/ModelGeneVariances.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/feature_set_enrichment/HypergeometricTail.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/feature_set_enrichment/HypergeometricTail.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/feature_set_enrichment/ScoreFeatureSet.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/feature_set_enrichment/ScoreFeatureSet.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/normalization/CenterSizeFactors.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/normalization/CenterSizeFactors.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/normalization/ChoosePseudoCount.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/normalization/ChoosePseudoCount.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/normalization/GroupedSizeFactors.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/normalization/GroupedSizeFactors.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/normalization/LogNormCounts.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/normalization/LogNormCounts.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/normalization/MedianSizeFactors.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/normalization/MedianSizeFactors.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/quality_control/ChooseOutlierFilters.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/quality_control/ChooseOutlierFilters.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/quality_control/ComputeMedianMad.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/quality_control/ComputeMedianMad.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/quality_control/FilterCells.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/quality_control/FilterCells.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/quality_control/PerCellAdtQcMetrics.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/quality_control/PerCellAdtQcMetrics.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/quality_control/PerCellCrisprQcMetrics.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/quality_control/PerCellCrisprQcMetrics.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/quality_control/PerCellQcMetrics.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/quality_control/PerCellQcMetrics.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/quality_control/PerCellRnaQcMetrics.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/quality_control/PerCellRnaQcMetrics.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/quality_control/SuggestAdtQcFilters.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/quality_control/SuggestAdtQcFilters.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/quality_control/SuggestCrisprQcFilters.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/quality_control/SuggestCrisprQcFilters.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/quality_control/SuggestRnaQcFilters.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/quality_control/SuggestRnaQcFilters.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/quality_control/utils.h` & `scranpy-0.0.3/extern/libscran/tests/src/quality_control/utils.h`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/utils/average_vectors.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/utils/average_vectors.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/utils/blocking.cpp` & `scranpy-0.0.3/extern/libscran/tests/src/utils/blocking.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/utils/compare_almost_equal.h` & `scranpy-0.0.3/extern/libscran/tests/src/utils/compare_almost_equal.h`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/utils/compare_vectors.h` & `scranpy-0.0.3/extern/libscran/tests/src/utils/compare_vectors.h`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/libscran/tests/src/utils/custom_parallel.h` & `scranpy-0.0.3/extern/libscran/tests/src/utils/custom_parallel.h`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/.github/workflows/compare-limma.yaml` & `scranpy-0.0.3/extern/weightedlowess/.github/workflows/compare-limma.yaml`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/.github/workflows/doxygenate.yaml` & `scranpy-0.0.3/extern/irlba/.github/workflows/doxygenate.yaml`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/.github/workflows/run-tests.yaml` & `scranpy-0.0.3/extern/knncolle/.github/workflows/run-tests.yaml`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/LICENSE` & `scranpy-0.0.3/extern/irlba/LICENSE`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/README.md` & `scranpy-0.0.3/extern/weightedlowess/README.md`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/docs/Doxyfile` & `scranpy-0.0.3/extern/weightedlowess/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/include/WeightedLowess/WeightedLowess.hpp` & `scranpy-0.0.3/extern/weightedlowess/include/WeightedLowess/WeightedLowess.hpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/tests/CMakeLists.txt` & `scranpy-0.0.3/extern/weightedlowess/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/tests/R/run.R` & `scranpy-0.0.3/extern/weightedlowess/tests/R/run.R`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/tests/R/test.cpp` & `scranpy-0.0.3/extern/weightedlowess/tests/R/test.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/tests/src/basic.cpp` & `scranpy-0.0.3/extern/weightedlowess/tests/src/basic.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/tests/src/divzero.cpp` & `scranpy-0.0.3/extern/weightedlowess/tests/src/divzero.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/tests/src/options.cpp` & `scranpy-0.0.3/extern/weightedlowess/tests/src/options.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/tests/src/runners.cpp` & `scranpy-0.0.3/extern/weightedlowess/tests/src/runners.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/tests/src/ties.cpp` & `scranpy-0.0.3/extern/weightedlowess/tests/src/ties.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/extern/weightedlowess/tests/src/utils.cpp` & `scranpy-0.0.3/extern/weightedlowess/tests/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/setup.cfg` & `scranpy-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	mattress
 	numpy>=1.22.4
 	BiocFrame
+	igraph
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `scranpy-0.0.2/src/scranpy/__init__.py` & `scranpy-0.0.3/src/scranpy/__init__.py`

 * *Files identical despite different names*

### Comparing `scranpy-0.0.2/src/scranpy/feature_selection/model_gene_variances.py` & `scranpy-0.0.3/src/scranpy/feature_selection/model_gene_variances.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Optional, Sequence
 
 import numpy as np
 from biocframe import BiocFrame
-from mattress import TatamiNumericPointer, tatamize
 
 from ..cpphelpers import lib
-from ..types import MatrixTypes, is_matrix_expected_type
-from ..utils import factorize
+from ..types import MatrixTypes
+from ..utils import factorize, validate_and_tatamize_input
 
 __author__ = "ltla, jkanche"
 __copyright__ = "ltla, jkanche"
 __license__ = "MIT"
 
 
 def model_gene_variances(
@@ -36,21 +35,15 @@
             Defaults to 0.3.
         num_threads (int, optional): number of threads to use. Defaults to 1.
         verbose (bool, optional): display logs?. Defaults to False.
 
     Returns:
         BiocFrame: data frame with various metrics.
     """
-    if not is_matrix_expected_type(x):
-        raise TypeError(
-            f"Input must be a tatami, numpy or sparse matrix, provided {type(x)}."
-        )
-
-    if not isinstance(x, TatamiNumericPointer):
-        x = tatamize(x)
+    x = validate_and_tatamize_input(x)
 
     NR = x.nrow()
     means = np.ndarray((NR,), dtype=np.float64)
     variances = np.ndarray((NR,), dtype=np.float64)
     fitted = np.ndarray((NR,), dtype=np.float64)
     residuals = np.ndarray((NR,), dtype=np.float64)
     extra = None
```

### Comparing `scranpy-0.0.2/src/scranpy/lib/log_norm_counts.cpp` & `scranpy-0.0.3/src/scranpy/lib/log_norm_counts.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#include "parallel.h" // must be first, to set all macros.
+
 #include "scran/normalization/LogNormCounts.hpp"
 #include "Mattress.h"
 
 #include <cstdint>
 #include <memory>
 
 extern "C" {
```

### Comparing `scranpy-0.0.2/src/scranpy/lib/model_gene_variances.cpp` & `scranpy-0.0.3/src/scranpy/lib/model_gene_variances.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#include "parallel.h" // must be first, to set all macros.
+
 #include "Mattress.h"
 #include "scran/feature_selection/ModelGeneVariances.hpp"
 #include <cstdint>
 
 extern "C" {
 
 void model_gene_variances(const Mattress* mat, double* means, double* variances, double* fitted, double* residuals, double span, int num_threads) {
```

### Comparing `scranpy-0.0.2/src/scranpy/lib/per_cell_rna_qc_metrics.cpp` & `scranpy-0.0.3/src/scranpy/lib/per_cell_rna_qc_metrics.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#include "parallel.h" // must be first, to set all macros.
+
 #include "Mattress.h"
 #include "scran/quality_control/PerCellRnaQcMetrics.hpp"
 #include <cstdint>
 
 extern "C" {
 
 void per_cell_rna_qc_metrics(const Mattress* mat, int num_subsets, const uintptr_t* subset_ptrs, double* sum_output, int32_t* detected_output, uintptr_t* subset_output, int num_threads) {
```

### Comparing `scranpy-0.0.2/src/scranpy/lib/suggest_rna_qc_filters.cpp` & `scranpy-0.0.3/src/scranpy/lib/suggest_rna_qc_filters.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#include "parallel.h"
+
 #include "scran/quality_control/SuggestRnaQcFilters.hpp"
 #include <cstdint>
 
 extern "C" {
 
 void suggest_rna_qc_filters(
     int num_cells,
```

### Comparing `scranpy-0.0.2/src/scranpy/normalization/log_norm_counts.py` & `scranpy-0.0.3/src/scranpy/normalization/log_norm_counts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, Sequence
 
 import numpy as np
 from mattress import TatamiNumericPointer, tatamize
 
 from .._logging import logger
 from ..cpphelpers import lib
-from ..types import MatrixTypes, is_matrix_expected_type
+from ..types import MatrixTypes, validate_matrix_types
 from ..utils import factorize
 
 __author__ = "ltla, jkanche"
 __copyright__ = "ltla, jkanche"
 __license__ = "MIT"
 
 
@@ -42,18 +42,15 @@
 
     Raises:
         TypeError, ValueError: if arguments don't meet expectations.
 
     Returns:
         TatamiNumericPointer: log normalized matrix.
     """
-    if not is_matrix_expected_type(x):
-        raise TypeError(
-            f"Input must be a tatami, numpy or sparse matrix, provided {type(x)}."
-        )
+    validate_matrix_types(x)
 
     if not isinstance(x, TatamiNumericPointer):
         raise ValueError("coming soon when DelayedArray support is implemented")
 
     NC = x.ncol()
 
     use_sf = size_factors is not None
```

### Comparing `scranpy-0.0.2/src/scranpy/quality_control/rna.py` & `scranpy-0.0.3/src/scranpy/quality_control/rna.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,53 @@
-from typing import Optional, Sequence
+from typing import Mapping, Optional, Sequence
 
 import numpy as np
 from biocframe import BiocFrame
-from mattress import TatamiNumericPointer, tatamize
 
 from .._logging import logger
 from ..cpphelpers import lib
-from ..types import MatrixTypes, is_matrix_expected_type
-from ..utils import factorize, to_logical
+from ..types import MatrixTypes
+from ..utils import factorize, to_logical, validate_and_tatamize_input
 
 __author__ = "ltla, jkanche"
 __copyright__ = "ltla, jkanche"
 __license__ = "MIT"
 
 
 def per_cell_rna_qc_metrics(
-    x: MatrixTypes, subsets: dict = {}, num_threads: int = 1, verbose: bool = False
+    x: MatrixTypes,
+    subsets: Optional[Mapping] = None,
+    num_threads: int = 1,
+    verbose: bool = False,
 ) -> BiocFrame:
     """Compute qc metrics (RNA).
 
     This function expects the matrix (`x`) to be features (rows) by cells (columns) and
     not the other way around!
 
     Args:
         x (MatrixTypes): input matrix.
-        subsets (dict, optional): named feature subsets.
+        subsets (Mapping, optional): named feature subsets.
             Each key is the name of the subset and each value is an array of
             integer indices, specifying the rows of `x` belonging to the subset.
             Defaults to {}.
         num_threads (int, optional): number of threads to use. Defaults to 1.
         verbose (bool, optional): display logs?. Defaults to False.
 
     Raises:
         TypeError: if x is not an expected matrix type.
 
     Returns:
         BiocFrame: data frame containing per-cell count sums, number of detected
         features and the proportion of counts in each subset.
     """
-    if not is_matrix_expected_type(x):
-        raise TypeError(
-            f"Input must be a tatami, numpy or sparse matrix, provided {type(x)}."
-        )
+    x = validate_and_tatamize_input(x)
 
-    if not isinstance(x, TatamiNumericPointer):
-        x = tatamize(x)
+    if subsets is None:
+        subsets = {}
 
     nc = x.ncol()
     sums = np.ndarray((nc,), dtype=np.float64)
     detected = np.ndarray((nc,), dtype=np.int32)
 
     keys = list(subsets.keys())
     num_subsets = len(keys)
```

### Comparing `scranpy-0.0.2/src/scranpy/types.py` & `scranpy-0.0.3/src/scranpy/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,78 @@
 from collections import namedtuple
 from typing import Any, Callable, Union
 
 import numpy as np
 import scipy.sparse as sp
 from mattress import TatamiNumericPointer
 
+from .nearest_neighbors import NeighborIndex, NeighborResults
+
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 MatrixTypes = Union[TatamiNumericPointer, np.ndarray, sp.spmatrix]
 FactorizedArray = namedtuple("FactorizedArray", ["levels", "indices"])
+NeighborIndexOrResults = Union[NeighborIndex, NeighborResults, np.ndarray]
 
 
 def is_matrix_expected_type(x: Any) -> bool:
-    """Checks if `x` is an expect matrix type.
+    """Checks if `x` is an expected matrix type.
 
     Args:
         x (Any): any object.
 
     Returns:
         bool: True if `x` is supported.
     """
     return (
         isinstance(x, TatamiNumericPointer)
         or isinstance(x, np.ndarray)
         or isinstance(x, sp.spmatrix)
     )
 
 
+def is_neighbor_class(x: Any) -> bool:
+    """Checks if `x` is an expected nearest neighbor input.
+
+    Args:
+        x (Any): any object.
+
+    Returns:
+        bool: True if `x` is supported.
+    """
+    return (
+        isinstance(x, NeighborIndex)
+        or isinstance(x, NeighborResults)
+        or isinstance(x, np.ndarray)
+    )
+
+
 def is_list_of_type(x: Any, target_type: Callable) -> bool:
     """Checks if `x` is a list of `target_type`.
 
     Args:
         x (Any): any object.
         target_type (Callable): Type to check for, e.g. str, int
 
     Returns:
         bool: True if `x` is list and all values are of the same type.
     """
     return (isinstance(x, list) or isinstance(x, tuple)) and all(
         isinstance(item, target_type) for item in x
     )
+
+
+def validate_matrix_types(x: MatrixTypes):
+    """Validate if x is an expected matrix type.
+
+    Args:
+        x (MatrixTypes): Inpute Matrix
+
+    Raises:
+        TypeError: if x is not a tatami, numpy or scipy matrix.
+    """
+    if not is_matrix_expected_type(x):
+        raise TypeError(
+            f"Input must be a tatami, numpy or sparse matrix, provided {type(x)}."
+        )
```

### Comparing `scranpy-0.0.2/src/scranpy.egg-info/PKG-INFO` & `scranpy-0.0.3/src/scranpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scranpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Analyze multi-modal single-cell data!
 Home-page: https://github.com/biocpy/scranpy
 Author: "Jayaram Kancherla, Aaron Lun"
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/biocpy/scranpy
 Platform: any
@@ -35,14 +35,16 @@
 ## Developer Notes
 
 
 Steps to setup dependencies - 
 
 - initialize git submodules in `extern/libscran`.
 
+- run `cmake .` inside the `extern/knncolle` to download the annoy library. a future version of this will use a cmake to setup the extern directory.
+
 First one needs to build the extern library, this would generate a shared object file to `src/scranpy/core-[*].so`
 
 ```shell
 python setup.py build_ext --inplace
 ```
 
 For typical development workflows, run this for tests
```

### Comparing `scranpy-0.0.2/tests/test_quality_control_steps.py` & `scranpy-0.0.3/tests/test_quality_control_steps.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from scranpy.quality_control import per_cell_rna_qc_metrics, suggest_rna_qc_filters
 
 __author__ = "ltla, jkanche"
 __copyright__ = "ltla, jkanche"
 __license__ = "MIT"
 
 
-def test_quality_control_numpy():
-    x = np.random.rand(1000, 100)
+def test_quality_control_numpy(mock_data):
+    x = mock_data.x
     result = per_cell_rna_qc_metrics(x, subsets={"foo": [1, 10, 100]})
 
     assert result is not None
     assert result.dims[0] == 100
     assert result.column("sums") is not None
     assert result.column("detected") is not None
     assert result.column("subset_proportions") is not None
@@ -29,34 +29,28 @@
     assert np.array_equal(result.column("detected"), resultp.column("detected"))
     assert np.array_equal(
         result.column("subset_proportions").column(0),
         resultp.column("subset_proportions").column(0),
     )
 
 
-def test_suggest_rna_qc_filters():
-    x = np.random.rand(1000, 100)
+def test_suggest_rna_qc_filters(mock_data):
+    x = mock_data.x
     result = per_cell_rna_qc_metrics(x, subsets={"foo": [1, 10, 100]})
     filters = suggest_rna_qc_filters(result)
 
     assert filters is not None
     assert filters.dims[0] == 1
     assert filters.column("sums") is not None
     assert filters.column("detected") is not None
     assert filters.column("subset_proportions") is not None
     assert filters.column("subset_proportions").column("foo") is not None
 
-    # Adding blocks
-    # TODO: factor out random block generation into a separate function!)
-    x = np.random.rand(1000, 100) * 20
-    block_levels = ["A", "B", "C"]
-    block = []
-    for i in range(x.shape[1]):
-        block.append(block_levels[i % len(block_levels)])
-
-    filters_blocked = suggest_rna_qc_filters(result, block=block)
+    #  with blocks
+    x = mock_data.x * 20
+    filters_blocked = suggest_rna_qc_filters(result, block=mock_data.block)
 
     assert filters_blocked.shape[0] == 3
     assert len(list(set(filters_blocked.rowNames).difference(["A", "B", "C"]))) == 0
 
     subfilters = filters_blocked.column("subset_proportions")
     assert len(list(set(subfilters.rowNames).difference(["A", "B", "C"]))) == 0
```

### Comparing `scranpy-0.0.2/tox.ini` & `scranpy-0.0.3/tox.ini`

 * *Files identical despite different names*

