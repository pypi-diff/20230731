# Comparing `tmp/gurobi_optimods-1.0.1.tar.gz` & `tmp/gurobi_optimods-1.1.0.tar.gz`

## Comparing `gurobi_optimods-1.0.1.tar` & `gurobi_optimods-1.1.0.tar`

### file list

```diff
@@ -1,90 +1,135 @@
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/Makefile
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tox.ini
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/pull_request_template.md
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/ISSUE_TEMPLATE/new_mod.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/code-quality.yml
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/doc-build.yml
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/doc-tests.yml
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/python-tests.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.github/workflows/wheel-tests.yml
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/make.bat
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/requirements.txt
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/adding.rst
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/api.rst
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/conf.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/contact.rst
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/contributing.rst
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/dev-reference.rst
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/gallery.rst
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/index.rst
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/installation.rst
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/license.rst
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/usage.rst
--rw-r--r--   0        0        0     8805 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/bipartite-matching.rst
--rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/lad-regression.rst
--rw-r--r--   0        0        0     9930 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/min-cost-flow.rst
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/mwis.rst
--rw-r--r--   0        0        0    27741 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/portfolio.rst
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/qubo.rst
--rw-r--r--   0        0        0    15439 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/workforce.rst
--rw-r--r--   0        0        0    34323 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-example.png
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-figs.py
--rw-r--r--   0        0        0    34001 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-flow.png
--rw-r--r--   0        0        0    33714 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-result.png
--rw-r--r--   0        0        0    21501 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/lad-outlier-coeffs.png
--rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/lad-outlier-errors.png
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/lad-regression-coeffs.png
--rw-r--r--   0        0        0   540595 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/min-cost-flow-result.png
--rw-r--r--   0        0        0    26538 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/mvp.png
--rw-r--r--   0        0        0    38322 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/mwis.png
--rw-r--r--   0        0        0    16645 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/pie.png
--rw-r--r--   0        0        0    16684 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/qubo.png
--rw-r--r--   0        0        0   367978 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/figures/shortest-path-result.png
--rw-r--r--   0        0        0    14540 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/mods/icons/lad-regression.png
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/refs/graphs.bib
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/refs/portfolio.bib
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/refs/qubo.bib
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/refs/regression.bib
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/docs/source/refs/workforce.bib
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/__init__.py
--rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/bipartite_matching.py
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/datasets.py
--rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/min_cost_flow.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/mwis.py
--rw-r--r--   0        0        0    15040 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/portfolio.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/qubo.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/regression.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/utils.py
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/workforce.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/data/graphs/simple_graph_edges.csv
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/data/graphs/simple_graph_nodes.csv
--rwxr-xr-x   0        0        0    41668 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/data/portfolio/portfolio.csv
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/data/workforce/preferences.csv
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/data/workforce/shift_requirements.csv
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/src/gurobi_optimods/data/workforce/worker_limits.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0    11740 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_bipartite_matching.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_graph_utils.py
--rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_min_cost_flow.py
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_mwis.py
--rw-r--r--   0        0        0    32785 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_portfolio.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_qubo.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_regression.py
--rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_utils.py
--rw-r--r--   0        0        0    10454 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/test_workforce.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/tests/utils.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/LICENSE
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/NOTICE
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/README.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 gurobi_optimods-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/Makefile
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tox.ini
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/.github/ISSUE_TEMPLATE/new_mod.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/.github/workflows/code-quality.yml
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/.github/workflows/doc-build.yml
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/.github/workflows/doc-tests.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/.github/workflows/python-tests.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/.github/workflows/wheel-tests.yml
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/make.bat
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/adding.rst
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/api.rst
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/conf.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/contact.rst
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/contributing.rst
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/dev-reference.rst
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/gallery.rst
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/index.rst
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/installation.rst
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/license.rst
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/usage.rst
+-rw-r--r--   0        0        0     8805 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/bipartite-matching.rst
+-rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/lad-regression.rst
+-rw-r--r--   0        0        0     9930 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/min-cost-flow.rst
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/mwis.rst
+-rw-r--r--   0        0        0    27741 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/portfolio.rst
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/qubo.rst
+-rw-r--r--   0        0        0    12068 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/sharpe-ratio.rst
+-rw-r--r--   0        0        0    15439 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/workforce.rst
+-rw-r--r--   0        0        0    34323 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/bipartite-matching-example.png
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/bipartite-matching-figs.py
+-rw-r--r--   0        0        0    34001 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/bipartite-matching-flow.png
+-rw-r--r--   0        0        0    33714 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/bipartite-matching-result.png
+-rw-r--r--   0        0        0    21501 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/lad-outlier-coeffs.png
+-rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/lad-outlier-errors.png
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/lad-regression-coeffs.png
+-rw-r--r--   0        0        0   540595 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/min-cost-flow-result.png
+-rw-r--r--   0        0        0    26538 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/mvp.png
+-rw-r--r--   0        0        0    38322 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/mwis.png
+-rw-r--r--   0        0        0   113240 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/opf.png
+-rw-r--r--   0        0        0    16645 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/pie.png
+-rw-r--r--   0        0        0    16684 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/qubo.png
+-rw-r--r--   0        0        0   113619 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/sharpe-ratio.png
+-rw-r--r--   0        0        0   367978 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/shortest-path-result.png
+-rw-r--r--   0        0        0    80259 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/switching_opf.png
+-rw-r--r--   0        0        0    37883 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/figures/violations_opf.png
+-rw-r--r--   0        0        0    14540 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/icons/lad-regression.png
+-rw-r--r--   0        0        0    20726 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/opf/opf.rst
+-rw-r--r--   0        0        0    11969 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/mods/opf/opf_specification.rst
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/refs/graphs.bib
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/refs/opf.bib
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/refs/portfolio.bib
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/refs/qubo.bib
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/refs/regression.bib
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/docs/source/refs/workforce.bib
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/__init__.py
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/bipartite_matching.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/datasets.py
+-rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/min_cost_flow.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/mwis.py
+-rw-r--r--   0        0        0    15040 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/portfolio.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/qubo.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/regression.py
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/sharpe_ratio.py
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/utils.py
+-rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/workforce.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/graphs/simple_graph_edges.csv
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/graphs/simple_graph_nodes.csv
+-rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/opf/case118.mat
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/opf/case14.mat
+-rw-r--r--   0        0        0    12853 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/opf/case300.mat
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/opf/case57.mat
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/opf/case9-switching.mat
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/opf/case9.mat
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/opf/case9coords.csv
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/opf/case9volts.csv
+-rw-r--r--   0        0        0   502584 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/opf/caseNY.mat
+-rw-r--r--   0        0        0    68955 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/opf/nybuses.csv
+-rwxr-xr-x   0        0        0    41668 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/portfolio/portfolio.csv
+-rw-r--r--   0        0        0    33126 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/sharpe-ratio/log-returns.csv
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/workforce/preferences.csv
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/workforce/shift_requirements.csv
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/data/workforce/worker_limits.csv
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/opf/__init__.py
+-rw-r--r--   0        0        0     7568 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/opf/api.py
+-rw-r--r--   0        0        0    13476 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/opf/converters.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/opf/graphics.py
+-rw-r--r--   0        0        0    20867 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/opf/grbformulator.py
+-rw-r--r--   0        0        0    35662 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/opf/grbformulator_ac.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/opf/grbformulator_common.py
+-rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/opf/grbformulator_dc.py
+-rw-r--r--   0        0        0    21382 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/opf/grbformulator_iv.py
+-rw-r--r--   0        0        0    22494 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/opf/grbgraphical.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/opf/io.py
+-rw-r--r--   0        0        0     9899 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/opf/plotlyhandler.py
+-rw-r--r--   0        0        0    12472 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/opf/structs.py
+-rw-r--r--   0        0        0    21333 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/src/gurobi_optimods/opf/violations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    11740 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/test_bipartite_matching.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/test_graph_utils.py
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/test_min_cost_flow.py
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/test_mwis.py
+-rw-r--r--   0        0        0    32785 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/test_portfolio.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/test_qubo.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/test_regression.py
+-rw-r--r--   0        0        0     8032 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/test_sharpe_ratio.py
+-rw-r--r--   0        0        0     5567 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/test_utils.py
+-rw-r--r--   0        0        0    10454 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/test_workforce.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/opf/__init__.py
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/opf/test_graphics.py
+-rw-r--r--   0        0        0    19306 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/opf/test_internal.py
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/opf/test_io.py
+-rw-r--r--   0        0        0    23119 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/opf/test_solver.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/opf/test_violations.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/opf/data/bus1-branch1-gen1.json
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/opf/data/bus2-branch2-gen2.json
+-rw-r--r--   0        0        0    12257 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/opf/data/case9_switching_solution.json
+-rw-r--r--   0        0        0   124189 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/tests/opf/data/ny_dc_switching_solution.json.gz
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/LICENSE
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/NOTICE
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/README.md
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 gurobi_optimods-1.1.0/PKG-INFO
```

### Comparing `gurobi_optimods-1.0.1/CODE_OF_CONDUCT.md` & `gurobi_optimods-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/CONTRIBUTING.md` & `gurobi_optimods-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/.github/pull_request_template.md` & `gurobi_optimods-1.1.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/.github/ISSUE_TEMPLATE/new_mod.md` & `gurobi_optimods-1.1.0/.github/ISSUE_TEMPLATE/new_mod.md`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/.github/workflows/code-quality.yml` & `gurobi_optimods-1.1.0/.github/workflows/code-quality.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/.github/workflows/doc-build.yml` & `gurobi_optimods-1.1.0/.github/workflows/doc-build.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/.github/workflows/doc-tests.yml` & `gurobi_optimods-1.1.0/.github/workflows/doc-tests.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/.github/workflows/publish-pypi.yml` & `gurobi_optimods-1.1.0/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/.github/workflows/python-tests.yml` & `gurobi_optimods-1.1.0/.github/workflows/python-tests.yml`

 * *Files 18% similar despite different names*

```diff
@@ -26,11 +26,11 @@
         run: |
           python -m pip install --upgrade pip
       - name: Install dependencies
         run: |
           python -m pip install .
       - name: Run unittest
         run: python -m unittest discover -b
-      - name: Install networkx (optional dependency)
-        run: python -m pip install networkx
+      - name: Install example dependencies
+        run: python -m pip install .[examples]
       - name: Run additional tests
         run: python -m unittest discover -b
```

### Comparing `gurobi_optimods-1.0.1/.github/workflows/release.yml` & `gurobi_optimods-1.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/.github/workflows/wheel-tests.yml` & `gurobi_optimods-1.1.0/.github/workflows/wheel-tests.yml`

 * *Files 25% similar despite different names*

```diff
@@ -34,19 +34,19 @@
           python -m build
       - name: Fetch dependencies for offline install
         run: |
           pip wheel --wheel-dir=dist gurobipy pandas numpy scipy gurobipy-pandas
       - name: Install from built wheel
         run: |
           python -m pip install --find-links dist --no-index --only-binary=:all: gurobi-optimods
-      - name: Test import
-        run: |
-          python -c "import gurobi_optimods"
       - name: Run unit tests
         run: |
           python -m unittest discover -b
-      - name: Install networkx (optional dependency)
+      - name: Fetch dependencies for offline install
+        run: |
+          pip wheel --wheel-dir=dist matplotlib networkx plotly scikit-learn
+      - name: Install example dependencies
         run: |
-          python -m pip install networkx
+          python -m pip install --find-links dist --no-index --only-binary=:all: gurobi-optimods[examples]
       - name: Run additional tests
         run: |
           python -m unittest discover -b
```

### Comparing `gurobi_optimods-1.0.1/docs/Makefile` & `gurobi_optimods-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/make.bat` & `gurobi_optimods-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/adding.rst` & `gurobi_optimods-1.1.0/docs/source/adding.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/conf.py` & `gurobi_optimods-1.1.0/docs/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3/", None),
     "sphinx": ("https://www.sphinx-doc.org/en/master/", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable/", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/", None),
     "networkx": ("https://networkx.org/documentation/stable", None),
+    "plotly": ("https://plotly.com/python-api-reference", None),
 }
 
 templates_path = ["_templates"]
 
 html_theme = "sphinx_rtd_theme"
 
 autosectionlabel_prefix_document = True
@@ -56,28 +57,29 @@
 extlinks_detect_hardcoded_links = True
 extlinks = {
     "pypi": ("https://pypi.org/project/%s/", "%s"),
     "ghsrc": ("https://github.com/Gurobi/gurobi-optimods/tree/main/%s", "%s"),
 }
 
 # -- Bibfiles
-
 bibtex_bibfiles = [
     "refs/graphs.bib",
+    "refs/opf.bib",
     "refs/portfolio.bib",
     "refs/qubo.bib",
     "refs/regression.bib",
     "refs/workforce.bib",
 ]
 
 # -- numpydoc magic linking
 
 numpydoc_xref_param_type = True
 numpydoc_xref_aliases = {
     "DataFrame": "pandas.DataFrame",
+    "Series": "pandas.Series",
     "DiGraph": "networkx.DiGraph",
     "Graph": "networkx.Graph",
     "LinAlgError": "numpy.linalg.LinAlgError",
     "spmatrix": "scipy.sparse.spmatrix",
 }
 numpydoc_xref_ignore = {"optional", "or", "of"}
 
@@ -93,29 +95,33 @@
     """Replace the create_env keyword argument accepted by decorated mods with
     the parameters added by the decorator"""
 
     if what in ["function", "method"] and hasattr(obj, "_decorated_mod"):
         if "create_env" not in signature:
             raise ValueError(f"Decorated mod {name} does not accept create_env")
         new_signature = signature.replace(
-            "create_env", "verbose=True, logfile=None, solver_params=None"
+            "create_env",
+            "verbose=True, logfile=None, time_limit=None, solver_params=None",
         )
         print(f"Modified signature of {name}")
         return new_signature, return_annotation
 
     return signature, return_annotation
 
 
 boilerplate = """
     **verbose** : :ref:`bool <python:bltin-boolean-values>`, optional
         ``verbose=False`` suppresses all console output
 
     **logfile** : :class:`python:str`, optional
         Write all mod output to the given file path
 
+    **time_limit** : :class:`python:float`
+        Solver time limit in seconds (default no limit)
+
     **solver_params** : :class:`python:dict`, optional
         Gurobi parameters to be passed to the solver
 """
 boilerplate = boilerplate.split("\n")
 
 
 def process_docstring(app, what, name, obj, options, lines):
```

### Comparing `gurobi_optimods-1.0.1/docs/source/contributing.rst` & `gurobi_optimods-1.1.0/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/dev-reference.rst` & `gurobi_optimods-1.1.0/docs/source/dev-reference.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/gallery.rst` & `gurobi_optimods-1.1.0/docs/source/gallery.rst`

 * *Files 18% similar despite different names*

```diff
@@ -26,26 +26,38 @@
 
     .. grid-item-card:: Maximum Weighted Independent Set
         :link: mods/mwis
         :link-type: doc
         :text-align: center
         :img-top: mods/figures/mwis.png
 
+    .. grid-item-card:: Optimal Power Flow
+        :link: mods/opf/opf
+        :link-type: doc
+        :text-align: center
+        :img-top: mods/figures/opf.png
+
     .. grid-item-card:: Mean-Variance Portfolio
         :link: mods/portfolio
         :link-type: doc
         :text-align: center
         :img-top: mods/figures/mvp.png
 
     .. grid-item-card:: Quadratic Unconstrained Binary Optimization (QUBO)
         :link: mods/qubo
         :link-type: doc
         :text-align: center
         :img-top: mods/figures/qubo.png
 
+    .. grid-item-card:: Maximum Sharpe Ratio
+        :link: mods/sharpe-ratio
+        :link-type: doc
+        :text-align: center
+        :img-top: mods/figures/sharpe-ratio.png
+
     .. grid-item-card:: Workforce Scheduling
         :link: mods/workforce
         :link-type: doc
         :text-align: center
         :img-top: mods/figures/bipartite-matching-flow.png
 
 
@@ -53,10 +65,12 @@
    :maxdepth: 1
    :hidden:
 
    mods/bipartite-matching
    mods/lad-regression
    mods/min-cost-flow
    mods/mwis
+   mods/opf/opf
    mods/portfolio
    mods/qubo
+   mods/sharpe-ratio
    mods/workforce
```

### Comparing `gurobi_optimods-1.0.1/docs/source/index.rst` & `gurobi_optimods-1.1.0/docs/source/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Welcome to Gurobi OptiMods's documentation!
 ===========================================
 
-**Gurobi OptiMods**: nice APIs for common optimization tasks.
+**Gurobi OptiMods**: data-driven APIs for common optimization tasks.
 
-``gurobi-optimods`` is an open-source Python repository of implemented
+`Gurobi/gurobi-optimods <https://github.com/Gurobi/gurobi-optimods>`_
+is an open-source Python repository of implemented
 optimization use cases using Gurobi, each with clear, informative, and pretty
 documentation that explains how to use it and the mathematical model behind it.
 
 The package is a collection of independent 'Mods'. Each Mod is intended to be
 immediately applicable to real use cases. However, we expect that for many
 practical applications users will need to understand and extend the
 implementation of a Mod to tailor it to their use case. Read the :doc:`usage`
```

### Comparing `gurobi_optimods-1.0.1/docs/source/installation.rst` & `gurobi_optimods-1.1.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/license.rst` & `gurobi_optimods-1.1.0/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/usage.rst` & `gurobi_optimods-1.1.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/bipartite-matching.rst` & `gurobi_optimods-1.1.0/docs/source/mods/bipartite-matching.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/lad-regression.rst` & `gurobi_optimods-1.1.0/docs/source/mods/lad-regression.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/min-cost-flow.rst` & `gurobi_optimods-1.1.0/docs/source/mods/min-cost-flow.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/mwis.rst` & `gurobi_optimods-1.1.0/docs/source/mods/mwis.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/portfolio.rst` & `gurobi_optimods-1.1.0/docs/source/mods/portfolio.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/qubo.rst` & `gurobi_optimods-1.1.0/docs/source/mods/qubo.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/workforce.rst` & `gurobi_optimods-1.1.0/docs/source/mods/workforce.rst`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-example.png` & `gurobi_optimods-1.1.0/docs/source/mods/figures/bipartite-matching-example.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-figs.py` & `gurobi_optimods-1.1.0/docs/source/mods/figures/bipartite-matching-figs.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-flow.png` & `gurobi_optimods-1.1.0/docs/source/mods/figures/bipartite-matching-flow.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/figures/bipartite-matching-result.png` & `gurobi_optimods-1.1.0/docs/source/mods/figures/bipartite-matching-result.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/figures/lad-outlier-coeffs.png` & `gurobi_optimods-1.1.0/docs/source/mods/figures/lad-outlier-coeffs.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/figures/lad-outlier-errors.png` & `gurobi_optimods-1.1.0/docs/source/mods/figures/lad-outlier-errors.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/figures/lad-regression-coeffs.png` & `gurobi_optimods-1.1.0/docs/source/mods/figures/lad-regression-coeffs.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/figures/min-cost-flow-result.png` & `gurobi_optimods-1.1.0/docs/source/mods/figures/min-cost-flow-result.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/figures/mvp.png` & `gurobi_optimods-1.1.0/docs/source/mods/figures/mvp.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/figures/mwis.png` & `gurobi_optimods-1.1.0/docs/source/mods/figures/mwis.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/figures/pie.png` & `gurobi_optimods-1.1.0/docs/source/mods/figures/pie.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/figures/qubo.png` & `gurobi_optimods-1.1.0/docs/source/mods/figures/qubo.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/figures/shortest-path-result.png` & `gurobi_optimods-1.1.0/docs/source/mods/figures/shortest-path-result.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/mods/icons/lad-regression.png` & `gurobi_optimods-1.1.0/docs/source/mods/icons/lad-regression.png`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/refs/graphs.bib` & `gurobi_optimods-1.1.0/docs/source/refs/graphs.bib`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/docs/source/refs/qubo.bib` & `gurobi_optimods-1.1.0/docs/source/refs/qubo.bib`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/src/gurobi_optimods/bipartite_matching.py` & `gurobi_optimods-1.1.0/src/gurobi_optimods/bipartite_matching.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/src/gurobi_optimods/datasets.py` & `gurobi_optimods-1.1.0/src/gurobi_optimods/datasets.py`

 * *Files 23% similar despite different names*

```diff
@@ -129,7 +129,44 @@
         cap = sp.coo_matrix((data, (a0, a1)))
 
     dem = None
     if demand:
         dem = node_data["demand"].values
 
     return G, cap, costs, dem
+
+
+def load_sharpe_ratio():
+    data = pd.read_csv(DATA_FILE_DIR / "sharpe-ratio/log-returns.csv", index_col=0)
+    # Annualize covariance-variance matrix and expected returns
+    return AttrDict(cov_matrix=data.cov() * len(data.index), mu=data.sum())
+
+
+def load_opf_example(case):
+    from gurobi_optimods.opf.io import read_case_matpower
+
+    file_path = DATA_FILE_DIR / f"opf/{case}.mat"
+    return read_case_matpower(file_path)
+
+
+def load_opf_extra(extra):
+    data_files = {
+        "case9-coordinates": ("case9coords.csv", "coords"),
+        "case9-voltages": ("case9volts.csv", "volts"),
+        "caseNY-coordinates": ("nybuses.csv", "coords"),
+    }
+
+    file_name, file_type = data_files[extra]
+    file_path = DATA_FILE_DIR.joinpath("opf").joinpath(file_name)
+    data = pd.read_csv(file_path)
+
+    if file_type == "coords":
+
+        def mapper(row):
+            return row["bus_i"], (row["lat"], row["lon"])
+
+    elif file_type == "volts":
+
+        def mapper(row):
+            return row["bus_i"], (row["Vm"], row["Va"])
+
+    return dict(mapper(record) for record in data.to_dict("records"))
```

### Comparing `gurobi_optimods-1.0.1/src/gurobi_optimods/min_cost_flow.py` & `gurobi_optimods-1.1.0/src/gurobi_optimods/min_cost_flow.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/src/gurobi_optimods/mwis.py` & `gurobi_optimods-1.1.0/src/gurobi_optimods/mwis.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/src/gurobi_optimods/portfolio.py` & `gurobi_optimods-1.1.0/src/gurobi_optimods/portfolio.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/src/gurobi_optimods/qubo.py` & `gurobi_optimods-1.1.0/src/gurobi_optimods/qubo.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,26 +49,24 @@
 
     elif where == GRB.Callback.MIPSOL:
         obj = model.cbGet(GRB.Callback.MIPSOL_OBJ)
         logger.info(f"New QUBO solution found with objective {obj}")
 
 
 @optimod()
-def solve_qubo(coeff_matrix, time_limit=GRB.INFINITY, *, create_env) -> QuboResult:
+def solve_qubo(coeff_matrix, *, create_env) -> QuboResult:
     """
     Solve a quadratic unconstrained binary optimization (QUBO) problem, i.e.,
     minimize quadratic function :math:`x'Qx` defined by coefficient matrix
     :math:`Q` over a binary decision variable vector :math:`x`
 
     Parameters
     ----------
     coeff_matrix : spmatrix
         Quadratic coefficient matrix
-    time_limit : float
-        Time limit in seconds (optional, default no limit)
 
     Returns
     -------
     QuboResult
         A dataclass containing a 0/1 solution array and its objective value
     """
 
@@ -77,15 +75,15 @@
 
     shape = coeff_matrix.shape
     if shape[0] != shape[1]:
         raise ValueError("Matrix is not quadratic.")
 
     n = shape[0]
 
-    params = {"TimeLimit": time_limit, "LogToConsole": 0}
+    params = {"LogToConsole": 0}
 
     with create_env(params=params) as env, gp.Model(env=env) as model:
         x = model.addMVar(n, vtype=GRB.BINARY)
         model.setObjective(x @ coeff_matrix @ x, GRB.MINIMIZE)
 
         model._next_output_time = 5
         model.optimize(callback)
```

### Comparing `gurobi_optimods-1.0.1/src/gurobi_optimods/regression.py` & `gurobi_optimods-1.1.0/src/gurobi_optimods/regression.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/src/gurobi_optimods/utils.py` & `gurobi_optimods-1.1.0/src/gurobi_optimods/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 @contextmanager
 def _mod_context(
     *,
     mod_logger: logging.Logger,
     log_to_console: bool,
     log_to_file: Optional[str],
+    time_limit: Optional[float],
     user_params: Optional[Dict],
 ):
     if not log_to_console and log_to_file:
         raise ValueError("Cannot disable console output and log to file")
 
     # Base setting: silence
     decorator_params = {"OutputFlag": 0}
@@ -78,14 +79,20 @@
         fh.setFormatter(ShortFormatter())
 
         # Send both mod logs and gurobi logs to the same file handler
         mod_logger.addHandler(fh)
         grb_logger.setLevel(logging.INFO)
         grb_logger.addHandler(fh)
 
+    if user_params is None:
+        user_params = {}
+
+    if time_limit is not None:
+        user_params["TimeLimit"] = float(time_limit)
+
     # Environment factory for decorated mod to use
     def create_env(params=None):
         final_params = {}
         final_params.update(decorator_params)
         if params:
             final_params.update(params)
         if user_params:
@@ -108,20 +115,26 @@
 def optimod(mod_logger=None):
     if mod_logger is None:
         mod_logger = global_mod_logger
 
     def optimod_decorator(func):
         @functools.wraps(func)
         def optimod_decorated(
-            *args, verbose=True, logfile=None, solver_params=None, **kwargs
+            *args,
+            verbose=True,
+            logfile=None,
+            time_limit=None,
+            solver_params=None,
+            **kwargs,
         ):
             with _mod_context(
                 mod_logger=mod_logger,
                 log_to_console=verbose,
                 log_to_file=logfile,
+                time_limit=time_limit,
                 user_params=solver_params,
             ) as create_env:
                 try:
                     return func(*args, create_env=create_env, **kwargs)
 
                 except gp.GurobiError as ge:
                     if ge.errno == gp.GRB.ERROR_SIZE_LIMIT_EXCEEDED:
```

### Comparing `gurobi_optimods-1.0.1/src/gurobi_optimods/workforce.py` & `gurobi_optimods-1.1.0/src/gurobi_optimods/workforce.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/src/gurobi_optimods/data/portfolio/portfolio.csv` & `gurobi_optimods-1.1.0/src/gurobi_optimods/data/portfolio/portfolio.csv`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/src/gurobi_optimods/data/workforce/preferences.csv` & `gurobi_optimods-1.1.0/src/gurobi_optimods/data/workforce/preferences.csv`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/tests/test_bipartite_matching.py` & `gurobi_optimods-1.1.0/tests/test_bipartite_matching.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/tests/test_graph_utils.py` & `gurobi_optimods-1.1.0/tests/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/tests/test_min_cost_flow.py` & `gurobi_optimods-1.1.0/tests/test_min_cost_flow.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/tests/test_mwis.py` & `gurobi_optimods-1.1.0/tests/test_mwis.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/tests/test_portfolio.py` & `gurobi_optimods-1.1.0/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/tests/test_qubo.py` & `gurobi_optimods-1.1.0/tests/test_qubo.py`

 * *Files 17% similar despite different names*

```diff
@@ -51,7 +51,16 @@
         data = [-1, -2, 3]
         row = [0, 0, 1]
         col = [1, 2, 2]
         Q = sp.coo_matrix((data, (row, col)), shape=(3, 3))
         result = solve_qubo(Q)
         self.assertEqual(result.objective_value, -2)
         assert_array_equal(result.solution, np.array([1, 0, 1]))
+
+    def test_large_matrix_time_limit(self):
+        # Should get a solution quickly, but take forever without a time limit.
+        # Largest model size solvable by the trial license.
+        Q = sp.random(200, 200, 0.5)
+        Q = sp.coo_matrix((Q.data - 0.5, (Q.row, Q.col)))
+        result = solve_qubo(Q, time_limit=0.5)
+        self.assertLess(result.objective_value, 0.0)
+        self.assertEqual(result.solution.shape, (200,))
```

### Comparing `gurobi_optimods-1.0.1/tests/test_regression.py` & `gurobi_optimods-1.1.0/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/tests/test_utils.py` & `gurobi_optimods-1.1.0/tests/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -113,14 +113,25 @@
                     "Model too large for size-limited license", traceback.format_exc()
                 )
                 self.assertNotIn(
                     "https://www.gurobi.com/free-trial", traceback.format_exc()
                 )
                 raise
 
+    def test_time_limit(self):
+        # Make time limit is a first class parameter for all mods
+
+        with redirect_stdout(io.StringIO()) as buffer_stdout, redirect_stderr(
+            io.StringIO()
+        ) as buffer_stderr:
+            self.mod(time_limit=10)
+
+        self.assertIn("Set parameter TimeLimit to value 10", buffer_stdout.getvalue())
+        self.assertEqual(buffer_stderr.getvalue(), "")
+
 
 class TestOverrideParams(unittest.TestCase):
     def test_mod_override_outputflag(self):
         # The mod can pass custom parameters which override those created
         # by verbose/logfile
 
         @optimod()
```

### Comparing `gurobi_optimods-1.0.1/tests/test_workforce.py` & `gurobi_optimods-1.1.0/tests/test_workforce.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/tests/utils.py` & `gurobi_optimods-1.1.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/.gitignore` & `gurobi_optimods-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/LICENSE` & `gurobi_optimods-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/NOTICE` & `gurobi_optimods-1.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `gurobi_optimods-1.0.1/README.md` & `gurobi_optimods-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/gurobi-optimods.svg)](https://pypi.org/project/gurobi-optimods)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gurobi-optimods.svg)](https://pypi.org/project/gurobi-optimods)
 [![Tests](https://github.com/Gurobi/gurobi-optimods/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/Gurobi/gurobi-optimods/actions/workflows/test.yml?query=branch%3Amain++)
 [![Docs](https://readthedocs.com/projects/gurobi-optimization-gurobi-optimods/badge/?version=stable)](https://gurobi-optimization-gurobi-optimods.readthedocs-hosted.com/en/stable)
 
-# gurobi-optimods: nice APIs for common optimization tasks
+# gurobi-optimods: data-driven APIs for common optimization tasks
 
 ``gurobi-optimods`` is an open-source Python repository of implemented
 optimization use cases, each with clear, informative, and pretty documentation
 that explains how to use it and the mathematical model behind it.
 
 ## Features
```

### Comparing `gurobi_optimods-1.0.1/pyproject.toml` & `gurobi_optimods-1.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gurobi-optimods"
-description = "Nice APIs for common optimization tasks"
+description = "Data-driven APIs for common optimization tasks"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = ["optimization", "gurobipy", "pandas", "scipy"]
 authors = [
     { name = "Simon Bowly", email = "bowly@gurobi.com" },
     { name = "Robert Luce", email = "luce@gurobi.com" },
@@ -29,16 +29,17 @@
     "pandas",
     "scipy>=1.8.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 examples = [
-    "networkx",
     "matplotlib",
+    "networkx",
+    "plotly",
     "scikit-learn"
 ]
 
 [tool.hatch.version]
 path = "src/gurobi_optimods/__init__.py"
 
 [tool.isort]
```

### Comparing `gurobi_optimods-1.0.1/PKG-INFO` & `gurobi_optimods-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gurobi-optimods
-Version: 1.0.1
-Summary: Nice APIs for common optimization tasks
+Version: 1.1.0
+Summary: Data-driven APIs for common optimization tasks
 Author-email: Simon Bowly <bowly@gurobi.com>, Robert Luce <luce@gurobi.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
 Keywords: gurobipy,optimization,pandas,scipy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -19,23 +19,24 @@
 Requires-Dist: gurobipy>=10.0.1
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy>=1.8.0
 Provides-Extra: examples
 Requires-Dist: matplotlib; extra == 'examples'
 Requires-Dist: networkx; extra == 'examples'
+Requires-Dist: plotly; extra == 'examples'
 Requires-Dist: scikit-learn; extra == 'examples'
 Description-Content-Type: text/markdown
 
 [![PyPI - Version](https://img.shields.io/pypi/v/gurobi-optimods.svg)](https://pypi.org/project/gurobi-optimods)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gurobi-optimods.svg)](https://pypi.org/project/gurobi-optimods)
 [![Tests](https://github.com/Gurobi/gurobi-optimods/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/Gurobi/gurobi-optimods/actions/workflows/test.yml?query=branch%3Amain++)
 [![Docs](https://readthedocs.com/projects/gurobi-optimization-gurobi-optimods/badge/?version=stable)](https://gurobi-optimization-gurobi-optimods.readthedocs-hosted.com/en/stable)
 
-# gurobi-optimods: nice APIs for common optimization tasks
+# gurobi-optimods: data-driven APIs for common optimization tasks
 
 ``gurobi-optimods`` is an open-source Python repository of implemented
 optimization use cases, each with clear, informative, and pretty documentation
 that explains how to use it and the mathematical model behind it.
 
 ## Features
```

