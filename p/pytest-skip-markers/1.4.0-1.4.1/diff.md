# Comparing `tmp/pytest-skip-markers-1.4.0.tar.gz` & `tmp/pytest-skip-markers-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Dec 20 11:47:09 2022, max compression
+gzip compressed data, last modified: Mon Jul 31 14:03:05 2023, max compression
```

## Comparing `pytest-skip-markers-1.4.0.tar` & `pytest-skip-markers-1.4.1.tar`

### file list

```diff
@@ -1,133 +1,143 @@
--rw-r--r--   0 root         (0) root         (0)     4115 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/.codecov.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/.github/
--rw-r--r--   0 root         (0) root         (0)      427 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/.github/CODEOWNERS
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      638 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)    20439 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/.github/workflows/testing.yml
--rw-r--r--   0 root         (0) root         (0)     1922 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     4797 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/.pre-commit-config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/.pre-commit-hooks/
--rw-r--r--   0 root         (0) root         (0)     4547 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/.pre-commit-hooks/check-changelog-entries.py
--rw-r--r--   0 root         (0) root         (0)     3549 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/.pre-commit-hooks/copyright-headers.py
--rw-r--r--   0 root         (0) root         (0)      581 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/.pre-commit-hooks/sort-pylint-spelling-words.py
--rw-r--r--   0 root         (0) root         (0)      503 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/.pylint-spelling-words
--rw-r--r--   0 root         (0) root         (0)    13551 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      735 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)     2991 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)     5256 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     2467 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     9283 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      412 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3826 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2332 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/changelog/
--rw-r--r--   0 root         (0) root         (0)       12 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/changelog/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/_static/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/_static/css/
--rw-r--r--   0 root         (0) root         (0)      425 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/_static/css/inline-include.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/_static/img/
--rw-r--r--   0 root         (0) root         (0)    10359 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/_static/img/SaltProject_Logomark_teal.png
--rw-r--r--   0 root         (0) root         (0)     9591 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/_static/img/SaltProject_altlogo_teal.png
--rw-r--r--   0 root         (0) root         (0)       30 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)     7696 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      258 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/contents.rst
--rw-r--r--   0 root         (0) root         (0)      561 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      760 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/ref/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/ref/pytestskipmarkers/
--rw-r--r--   0 root         (0) root         (0)      137 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/ref/pytestskipmarkers/index.rst
--rw-r--r--   0 root         (0) root         (0)    15427 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/ref/pytestskipmarkers/plugin.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/ref/pytestskipmarkers/utils/
--rw-r--r--   0 root         (0) root         (0)      169 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/ref/pytestskipmarkers/utils/index.rst
--rw-r--r--   0 root         (0) root         (0)      195 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/ref/pytestskipmarkers/utils/markers.rst
--rw-r--r--   0 root         (0) root         (0)      184 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/ref/pytestskipmarkers/utils/platform.rst
--rw-r--r--   0 root         (0) root         (0)      191 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/ref/pytestskipmarkers/utils/ports.rst
--rw-r--r--   0 root         (0) root         (0)      273 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/docs/sitevars.rst
--rw-r--r--   0 root         (0) root         (0)    18994 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/noxfile.py
--rw-r--r--   0 root         (0) root         (0)     1235 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      348 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/requirements/
--rw-r--r--   0 root         (0) root         (0)       68 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/requirements/build.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/requirements/changelog.txt
--rw-r--r--   0 root         (0) root         (0)      144 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      202 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/requirements/lint.txt
--rw-r--r--   0 root         (0) root         (0)       97 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/requirements/tests.txt
--rw-r--r--   0 root         (0) root         (0)     2713 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      186 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytest_skip_markers.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3826 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytest_skip_markers.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3765 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytest_skip_markers.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytest_skip_markers.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytest_skip_markers.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytest_skip_markers.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      536 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytest_skip_markers.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytest_skip_markers.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytestskipmarkers/
--rw-r--r--   0 root         (0) root         (0)     1883 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytestskipmarkers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6567 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytestskipmarkers/plugin.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytestskipmarkers/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytestskipmarkers/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytestskipmarkers/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33348 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytestskipmarkers/utils/markers.py
--rw-r--r--   0 root         (0) root         (0)     5727 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytestskipmarkers/utils/platform.py
--rw-r--r--   0 root         (0) root         (0)     2136 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytestskipmarkers/utils/ports.py
--rw-r--r--   0 root         (0) root         (0)      481 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytestskipmarkers/utils/socket.py
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytestskipmarkers/utils/socket.pyi
--rw-r--r--   0 root         (0) root         (0)     4628 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytestskipmarkers/utils/win_functions.py
--rw-r--r--   0 root         (0) root         (0)       43 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/src/pytestskipmarkers/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      825 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/markers/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/markers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1457 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_destructive_test.py
--rw-r--r--   0 root         (0) root         (0)     1437 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_expensive_test.py
--rw-r--r--   0 root         (0) root         (0)     1867 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_requires_network.py
--rw-r--r--   0 root         (0) root         (0)     1850 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_if_binaries_missing.py
--rw-r--r--   0 root         (0) root         (0)     2317 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_if_not_root.py
--rw-r--r--   0 root         (0) root         (0)     1798 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_on_aarch64.py
--rw-r--r--   0 root         (0) root         (0)     1867 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_on_aix.py
--rw-r--r--   0 root         (0) root         (0)     1887 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_on_darwin.py
--rw-r--r--   0 root         (0) root         (0)     1268 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_on_env.py
--rw-r--r--   0 root         (0) root         (0)     1894 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_on_freebsd.py
--rw-r--r--   0 root         (0) root         (0)     1880 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_on_linux.py
--rw-r--r--   0 root         (0) root         (0)     1887 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_on_netbsd.py
--rw-r--r--   0 root         (0) root         (0)     1894 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_on_openbsd.py
--rw-r--r--   0 root         (0) root         (0)     1805 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_on_photonos.py
--rw-r--r--   0 root         (0) root         (0)     3793 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_on_platforms.py
--rw-r--r--   0 root         (0) root         (0)     1894 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_on_smartos.py
--rw-r--r--   0 root         (0) root         (0)     1868 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_on_spawning_platform.py
--rw-r--r--   0 root         (0) root         (0)     1880 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_on_sunos.py
--rw-r--r--   0 root         (0) root         (0)     1894 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_on_windows.py
--rw-r--r--   0 root         (0) root         (0)     1827 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_aarch64.py
--rw-r--r--   0 root         (0) root         (0)     1895 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_aix.py
--rw-r--r--   0 root         (0) root         (0)     1916 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_darwin.py
--rw-r--r--   0 root         (0) root         (0)     1923 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_freebsd.py
--rw-r--r--   0 root         (0) root         (0)     1909 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_linux.py
--rw-r--r--   0 root         (0) root         (0)     1916 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_netbsd.py
--rw-r--r--   0 root         (0) root         (0)     1923 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_openbsd.py
--rw-r--r--   0 root         (0) root         (0)     1834 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_photonos.py
--rw-r--r--   0 root         (0) root         (0)     4257 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_platforms.py
--rw-r--r--   0 root         (0) root         (0)     1923 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_smartos.py
--rw-r--r--   0 root         (0) root         (0)     1897 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_spawning_platform.py
--rw-r--r--   0 root         (0) root         (0)     1909 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_sunos.py
--rw-r--r--   0 root         (0) root         (0)     1923 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_windows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/unit/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/unit/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/unit/utils/markers/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/unit/utils/markers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2300 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/unit/utils/markers/test_skip_if_binaries_missing.py
--rw-r--r--   0 root         (0) root         (0)      953 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/unit/utils/markers/test_skip_if_no_local_network.py
--rw-r--r--   0 root         (0) root         (0)     1118 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/unit/utils/markers/test_skip_if_no_remote_network.py
--rw-r--r--   0 root         (0) root         (0)      970 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/unit/utils/markers/test_skip_if_not_root.py
--rw-r--r--   0 root         (0) root         (0)     1314 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/unit/utils/markers/test_skip_on_env.py
--rw-r--r--   0 root         (0) root         (0)     7958 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/unit/utils/test_platform.py
--rw-r--r--   0 root         (0) root         (0)     2816 2022-12-20 11:47:09.000000 pytest-skip-markers-1.4.0/tests/unit/utils/test_ports.py
+-rw-r--r--   0 root         (0) root         (0)     4115 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.codecov.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.github/
+-rw-r--r--   0 root         (0) root         (0)      427 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.github/CODEOWNERS
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.github/actions/setup-actionlint/
+-rw-r--r--   0 root         (0) root         (0)      769 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.github/actions/setup-actionlint/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.github/actions/setup-shellcheck/
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.github/actions/setup-shellcheck/action.yml
+-rw-r--r--   0 root         (0) root         (0)      174 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      758 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)    11029 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.github/workflows/testing.yml
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     5104 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.pre-commit-hooks/
+-rw-r--r--   0 root         (0) root         (0)     4546 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.pre-commit-hooks/check-changelog-entries.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.pre-commit-hooks/copyright-headers.py
+-rw-r--r--   0 root         (0) root         (0)      581 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.pre-commit-hooks/sort-pylint-spelling-words.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.pylint-spelling-words
+-rw-r--r--   0 root         (0) root         (0)    13551 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      646 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)     5256 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2467 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     9283 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      412 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3826 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/changelog/
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/changelog/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/_static/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/_static/css/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/_static/css/inline-include.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/_static/img/
+-rw-r--r--   0 root         (0) root         (0)    10359 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/_static/img/SaltProject_Logomark_teal.png
+-rw-r--r--   0 root         (0) root         (0)     9591 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/_static/img/SaltProject_altlogo_teal.png
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/changelog.rst
+-rw-r--r--   0 root         (0) root         (0)     7696 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/contents.rst
+-rw-r--r--   0 root         (0) root         (0)      561 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      760 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/ref/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/ref/pytestskipmarkers/
+-rw-r--r--   0 root         (0) root         (0)      137 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/ref/pytestskipmarkers/index.rst
+-rw-r--r--   0 root         (0) root         (0)    15427 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/ref/pytestskipmarkers/plugin.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/ref/pytestskipmarkers/utils/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/ref/pytestskipmarkers/utils/index.rst
+-rw-r--r--   0 root         (0) root         (0)      195 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/ref/pytestskipmarkers/utils/markers.rst
+-rw-r--r--   0 root         (0) root         (0)      184 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/ref/pytestskipmarkers/utils/platform.rst
+-rw-r--r--   0 root         (0) root         (0)      191 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/ref/pytestskipmarkers/utils/ports.rst
+-rw-r--r--   0 root         (0) root         (0)      273 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/docs/sitevars.rst
+-rw-r--r--   0 root         (0) root         (0)    19003 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/noxfile.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/requirements/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/requirements/build.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/requirements/changelog.txt
+-rw-r--r--   0 root         (0) root         (0)      144 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      202 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/requirements/lint.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/requirements/tests.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/requirements/tools.txt
+-rw-r--r--   0 root         (0) root         (0)     2713 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      186 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytest_skip_markers.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3826 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytest_skip_markers.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3937 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytest_skip_markers.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytest_skip_markers.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytest_skip_markers.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytest_skip_markers.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      536 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytest_skip_markers.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytest_skip_markers.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytestskipmarkers/
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytestskipmarkers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6577 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytestskipmarkers/plugin.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytestskipmarkers/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytestskipmarkers/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytestskipmarkers/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33348 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytestskipmarkers/utils/markers.py
+-rw-r--r--   0 root         (0) root         (0)     5727 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytestskipmarkers/utils/platform.py
+-rw-r--r--   0 root         (0) root         (0)     2136 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytestskipmarkers/utils/ports.py
+-rw-r--r--   0 root         (0) root         (0)      481 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytestskipmarkers/utils/socket.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytestskipmarkers/utils/socket.pyi
+-rw-r--r--   0 root         (0) root         (0)     4628 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytestskipmarkers/utils/win_functions.py
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/src/pytestskipmarkers/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      825 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/markers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/markers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_destructive_test.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_expensive_test.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_requires_network.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_if_binaries_missing.py
+-rw-r--r--   0 root         (0) root         (0)     2317 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_if_not_root.py
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_on_aarch64.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_on_aix.py
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_on_darwin.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_on_env.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_on_freebsd.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_on_linux.py
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_on_netbsd.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_on_openbsd.py
+-rw-r--r--   0 root         (0) root         (0)     1805 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_on_photonos.py
+-rw-r--r--   0 root         (0) root         (0)     3793 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_on_platforms.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_on_smartos.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_on_spawning_platform.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_on_sunos.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_on_windows.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_aarch64.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_aix.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_darwin.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_freebsd.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_linux.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_netbsd.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_openbsd.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_photonos.py
+-rw-r--r--   0 root         (0) root         (0)     4257 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_platforms.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_smartos.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_spawning_platform.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_sunos.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_windows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/unit/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/unit/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/unit/utils/markers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/unit/utils/markers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/unit/utils/markers/test_skip_if_binaries_missing.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/unit/utils/markers/test_skip_if_no_local_network.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/unit/utils/markers/test_skip_if_no_remote_network.py
+-rw-r--r--   0 root         (0) root         (0)      970 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/unit/utils/markers/test_skip_if_not_root.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/unit/utils/markers/test_skip_on_env.py
+-rw-r--r--   0 root         (0) root         (0)     7958 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/unit/utils/test_platform.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tests/unit/utils/test_ports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tools/
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-07-31 14:03:05.000000 pytest-skip-markers-1.4.1/tools/pre_commit.py
```

### Comparing `pytest-skip-markers-1.4.0/.codecov.yml` & `pytest-skip-markers-1.4.1/.codecov.yml`

 * *Files identical despite different names*

### Comparing `pytest-skip-markers-1.4.0/.gitignore` & `pytest-skip-markers-1.4.1/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -129,7 +129,10 @@
 .pyre/
 
 # Ignore the auto generated version.py
 src/pytestskipmarkers/version.py
 
 # Ignore the test generated artifacts
 artifacts/
+
+# nvim backup files
+*~
```

### Comparing `pytest-skip-markers-1.4.0/.pre-commit-config.yaml` & `pytest-skip-markers-1.4.1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -32,97 +32,110 @@
       - id: check-copyright-headers
         name: Check python modules for appropriate copyright headers
         files: ^.*\.py$
         entry: python .pre-commit-hooks/copyright-headers.py
         language: system
   # <---- Local Hooks ------------------------------------------------------------------------------------------------
 
+  - repo: https://github.com/s0undt3ch/python-tools-scripts
+    rev: "0.17.0"
+    hooks:
+      - id: tools
+        alias: actionlint
+        name: Lint GitHub Actions Workflows
+        files: "^.github/workflows/"
+        types:
+          - yaml
+        args:
+          - pre-commit
+          - actionlint
+
   # ----- Formatting ------------------------------------------------------------------------------------------------>
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.10.1
     hooks:
       - id: pyupgrade
         name: Rewrite Code to be Py3.7+
         args: [--py37-plus]
 
   - repo: https://github.com/asottile/reorder_python_imports
-    rev: v3.9.0
+    rev: v3.10.0
     hooks:
       - id: reorder-python-imports
         args: [
           --py3-plus,
           --application-directories=.:src:examples/echo-extension/src
         ]
         exclude: ^src/pytestskipmarkers/(version.py|downgraded/.*)$
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.7.0
     hooks:
       - id: black
         args: [-l 100]
         exclude: ^src/pytestskipmarkers/(version.py|downgraded/.*)$
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
+    rev: 1.15.0
     hooks:
       - id: blacken-docs
         args: [--skip-errors]
         files: ^(.*\.rst|docs/.*\.rst|src/pytestskipmarkers/.*\.py)$
         additional_dependencies:
-          - black==22.3.0
+          - black==23.7.0
   # <---- Formatting -------------------------------------------------------------------------------------------------
 
   # ----- Security -------------------------------------------------------------------------------------------------->
   - repo: https://github.com/PyCQA/bandit
-    rev: "1.7.4"
+    rev: "1.7.5"
     hooks:
       - id: bandit
         alias: bandit-salt
         name: Run bandit against Salt
         args: [--silent, -lll, --skip, B701]
         exclude: >
             (?x)^(
                 tests/.*
             )$
   - repo: https://github.com/PyCQA/bandit
-    rev: "1.7.4"
+    rev: "1.7.5"
     hooks:
       - id: bandit
         alias: bandit-tests
         name: Run bandit against the test suite
         args: [--silent, -lll, --skip, B701]
         files: ^tests/.*
   # <---- Security ---------------------------------------------------------------------------------------------------
 
   # ----- Code Analysis --------------------------------------------------------------------------------------------->
   - repo: https://github.com/pycqa/flake8
-    rev: '6.0.0'
+    rev: '6.1.0'
     hooks:
       - id: flake8
         exclude: ^(src/pytestskipmarkers/(downgraded/.*|version\.py)|\.pre-commit-hooks/.*\.py)$
         additional_dependencies:
         - flake8-mypy-fork
         - flake8-docstrings
         - flake8-typing-imports
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.4.1
     hooks:
       - id: mypy
         name: Run mypy against source
         files: ^src/.*\.py$
         exclude: ^src/pytestskipmarkers/(downgraded/.*|utils/(socket|time)\.py)$
         args: [--strict]
         additional_dependencies:
           - attrs
           - types-attrs
           - types-setuptools
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.4.1
     hooks:
       - id: mypy
         name: Run mypy against tests
         files: ^tests/.*\.py$
         exclude: ^src/pytestskipmarkers/(downgraded/.*|utils/(socket|time)\.py)$
         args: []
         additional_dependencies:
```

### Comparing `pytest-skip-markers-1.4.0/.pre-commit-hooks/check-changelog-entries.py` & `pytest-skip-markers-1.4.1/.pre-commit-hooks/check-changelog-entries.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 # pylint: skip-file
 import argparse
 import pathlib
 import re
 import sys
@@ -21,15 +21,14 @@
     "trivial",
 )
 CHANGELOG_ENTRY_REREX = r"^[\d]+\.({})\.rst$".format("|".join(CHANGELOG_EXTENSIONS))
 CHANGELOG_ENTRY_RE = re.compile(CHANGELOG_ENTRY_REREX)
 
 
 def check_changelog_entries(files):
-
     exitcode = 0
     for entry in files:
         path = pathlib.Path(entry).resolve()
         # Is it under changelog/
         try:
             path.relative_to(CHANGELOG_ENTRIES_PATH)
             if path.name in (".gitignore", "_template.rst", __name__):
```

### Comparing `pytest-skip-markers-1.4.0/.pre-commit-hooks/copyright-headers.py` & `pytest-skip-markers-1.4.1/.pre-commit-hooks/copyright-headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 # pylint: disable=invalid-name,missing-module-docstring,missing-function-docstring
 import argparse
 import pathlib
 import re
 import sys
```

### Comparing `pytest-skip-markers-1.4.0/.pre-commit-hooks/sort-pylint-spelling-words.py` & `pytest-skip-markers-1.4.1/.pre-commit-hooks/sort-pylint-spelling-words.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 # pylint: skip-file
 import pathlib
 
 REPO_ROOT = pathlib.Path(__name__).resolve().parent
 PYLINT_SPELLING_WORDS = REPO_ROOT / ".pylint-spelling-words"
```

### Comparing `pytest-skip-markers-1.4.0/.pylintrc` & `pytest-skip-markers-1.4.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `pytest-skip-markers-1.4.0/CHANGELOG.rst` & `pytest-skip-markers-1.4.1/CHANGELOG.rst`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,34 @@
 Backward incompatible (breaking) changes will only be introduced in major versions with advance notice in the
 **Deprecations** section of releases.
 
 .. towncrier-draft-entries::
 
 .. towncrier release notes start
 
+1.4.1 (2023-07-31)
+==================
+
+Improvements
+------------
+
+- Stop using deprecated `@pytest.mark.trylast` (`#24 <https://github.com/saltstack/pytest-skip-markers/issues/24>`_)
+
+
+Trivial/Internal Changes
+------------------------
+
+- Several minor fixes & improvements:
+
+  * Update pre-commit hooks versions
+  * Update copyright headers
+  * Update workflows
+  * Add dependabot config to update GH Actions workflow versions (`#25 <https://github.com/saltstack/pytest-skip-markers/issues/25>`_)
+
+
 1.4.0 (2022-12-20)
 ==================
 
 Breaking Changes
 ----------------
 
 - Drop support for python versions older than 3.7 (`#22 <https://github.com/saltstack/pytest-skip-markers/issues/22>`_)
```

### Comparing `pytest-skip-markers-1.4.0/CODE_OF_CONDUCT.md` & `pytest-skip-markers-1.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pytest-skip-markers-1.4.0/CONTRIBUTING.md` & `pytest-skip-markers-1.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytest-skip-markers-1.4.0/LICENSE` & `pytest-skip-markers-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-skip-markers-1.4.0/PKG-INFO` & `pytest-skip-markers-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-skip-markers
-Version: 1.4.0
+Version: 1.4.1
 Summary: Pytest Salt Plugin
 Home-page: https://github.com/saltstack/pytest-skip-markers
 Author: Pedro Algarvio
 Author-email: pedro@algarvio.me
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/saltstack/pytest-skip-markers
 Project-URL: Tracker, https://github.com/saltstack/pytest-skip-markers/issues
```

### Comparing `pytest-skip-markers-1.4.0/README.rst` & `pytest-skip-markers-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-skip-markers-1.4.0/docs/Makefile` & `pytest-skip-markers-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-skip-markers-1.4.0/docs/_static/img/SaltProject_Logomark_teal.png` & `pytest-skip-markers-1.4.1/docs/_static/img/SaltProject_Logomark_teal.png`

 * *Files identical despite different names*

### Comparing `pytest-skip-markers-1.4.0/docs/_static/img/SaltProject_altlogo_teal.png` & `pytest-skip-markers-1.4.1/docs/_static/img/SaltProject_altlogo_teal.png`

 * *Files identical despite different names*

### Comparing `pytest-skip-markers-1.4.0/docs/conf.py` & `pytest-skip-markers-1.4.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 # Configuration file for the Sphinx documentation builder.
 #
 # This file only contains a selection of the most common options. For a full
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
```

### Comparing `pytest-skip-markers-1.4.0/docs/index.rst` & `pytest-skip-markers-1.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-skip-markers-1.4.0/docs/make.bat` & `pytest-skip-markers-1.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytest-skip-markers-1.4.0/docs/ref/pytestskipmarkers/plugin.rst` & `pytest-skip-markers-1.4.1/docs/ref/pytestskipmarkers/plugin.rst`

 * *Files identical despite different names*

### Comparing `pytest-skip-markers-1.4.0/noxfile.py` & `pytest-skip-markers-1.4.1/noxfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 import datetime
 import gzip
 import json
 import os
 import pathlib
@@ -500,15 +500,15 @@
         tempd = pathlib.Path(tempfile.mkdtemp()).resolve()
         d_src = tempd.joinpath("src")
         d_src.mkdir()
         d_tar = tempd.joinpath(targz.stem)
         d_targz = tempd.joinpath(targz.name)
         with tarfile.open(d_tar, "w|") as wfile:
             with tarfile.open(targz, "r:gz") as rfile:
-                rfile.extractall(d_src)
+                rfile.extractall(d_src)  # nosec
                 extracted_dir = next(pathlib.Path(d_src).iterdir())
                 for name in sorted(extracted_dir.rglob("*")):
                     wfile.add(
                         str(name),
                         filter=self.tar_reset,
                         recursive=False,
                         arcname=str(name.relative_to(d_src)),
```

### Comparing `pytest-skip-markers-1.4.0/pyproject.toml` & `pytest-skip-markers-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-skip-markers-1.4.0/setup.cfg` & `pytest-skip-markers-1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-skip-markers-1.4.0/src/pytest_skip_markers.egg-info/PKG-INFO` & `pytest-skip-markers-1.4.1/src/pytest_skip_markers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-skip-markers
-Version: 1.4.0
+Version: 1.4.1
 Summary: Pytest Salt Plugin
 Home-page: https://github.com/saltstack/pytest-skip-markers
 Author: Pedro Algarvio
 Author-email: pedro@algarvio.me
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/saltstack/pytest-skip-markers
 Project-URL: Tracker, https://github.com/saltstack/pytest-skip-markers/issues
```

### Comparing `pytest-skip-markers-1.4.0/src/pytest_skip_markers.egg-info/SOURCES.txt` & `pytest-skip-markers-1.4.1/src/pytest_skip_markers.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 README.rst
 noxfile.py
 pyproject.toml
 pytest.ini
 setup.cfg
 setup.py
 .github/CODEOWNERS
+.github/dependabot.yml
+.github/actions/setup-actionlint/action.yml
+.github/actions/setup-shellcheck/action.yml
 .github/workflows/release.yml
 .github/workflows/testing.yml
 .pre-commit-hooks/check-changelog-entries.py
 .pre-commit-hooks/copyright-headers.py
 .pre-commit-hooks/sort-pylint-spelling-words.py
 changelog/.gitignore
 docs/Makefile
@@ -41,14 +44,15 @@
 docs/ref/pytestskipmarkers/utils/ports.rst
 requirements/base.txt
 requirements/build.txt
 requirements/changelog.txt
 requirements/docs.txt
 requirements/lint.txt
 requirements/tests.txt
+requirements/tools.txt
 src/pytest_skip_markers.egg-info/PKG-INFO
 src/pytest_skip_markers.egg-info/SOURCES.txt
 src/pytest_skip_markers.egg-info/dependency_links.txt
 src/pytest_skip_markers.egg-info/entry_points.txt
 src/pytest_skip_markers.egg-info/not-zip-safe
 src/pytest_skip_markers.egg-info/requires.txt
 src/pytest_skip_markers.egg-info/top_level.txt
@@ -103,8 +107,10 @@
 tests/unit/utils/test_platform.py
 tests/unit/utils/test_ports.py
 tests/unit/utils/markers/__init__.py
 tests/unit/utils/markers/test_skip_if_binaries_missing.py
 tests/unit/utils/markers/test_skip_if_no_local_network.py
 tests/unit/utils/markers/test_skip_if_no_remote_network.py
 tests/unit/utils/markers/test_skip_if_not_root.py
-tests/unit/utils/markers/test_skip_on_env.py
+tests/unit/utils/markers/test_skip_on_env.py
+tools/__init__.py
+tools/pre_commit.py
```

### Comparing `pytest-skip-markers-1.4.0/src/pytest_skip_markers.egg-info/requires.txt` & `pytest-skip-markers-1.4.1/src/pytest_skip_markers.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pytest-skip-markers-1.4.0/src/pytestskipmarkers/__init__.py` & `pytest-skip-markers-1.4.1/src/pytestskipmarkers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 # type: ignore
 import pathlib
 import re
 import sys
```

### Comparing `pytest-skip-markers-1.4.0/src/pytestskipmarkers/plugin.py` & `pytest-skip-markers-1.4.1/src/pytestskipmarkers/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Pytest plugin hooks.
 """
 from typing import TYPE_CHECKING
 
@@ -44,15 +44,15 @@
     """
     Fixtures injection based on markers or test skips based on CLI arguments.
     """
     __tracebackhide__ = True
     pytestskipmarkers.utils.markers.evaluate_markers(item)
 
 
-@pytest.mark.trylast  # type: ignore[misc]
+@pytest.hookimpl(trylast=True)  # type: ignore[misc]
 def pytest_configure(config: "Config") -> None:
     """
     Configure the plugin.
 
     called after command line options have been parsed
     and all plugins and initial conftest files been loaded.
     """
```

### Comparing `pytest-skip-markers-1.4.0/src/pytestskipmarkers/utils/markers.py` & `pytest-skip-markers-1.4.1/src/pytestskipmarkers/utils/markers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 PyTest Markers related utilities.
 
 ..
     PYTEST_DONT_REWRITE
```

### Comparing `pytest-skip-markers-1.4.0/src/pytestskipmarkers/utils/platform.py` & `pytest-skip-markers-1.4.1/src/pytestskipmarkers/utils/platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Platform related utilities.
 
 ..
     PYTEST_DONT_REWRITE
```

### Comparing `pytest-skip-markers-1.4.0/src/pytestskipmarkers/utils/ports.py` & `pytest-skip-markers-1.4.1/src/pytestskipmarkers/utils/ports.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Ports related utility functions.
 """
 import contextlib
 import logging
```

### Comparing `pytest-skip-markers-1.4.0/src/pytestskipmarkers/utils/win_functions.py` & `pytest-skip-markers-1.4.1/src/pytestskipmarkers/utils/win_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Windows specific functions.
 
 ..
     PYTEST_DONT_REWRITE
```

### Comparing `pytest-skip-markers-1.4.0/tests/conftest.py` & `pytest-skip-markers-1.4.1/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 import pytest
 
 try:  # pragma: no cover
     import importlib.metadata
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_destructive_test.py` & `pytest-skip-markers-1.4.1/tests/functional/test_destructive_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.destructive_test`` marker.
 """
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_expensive_test.py` & `pytest-skip-markers-1.4.1/tests/functional/test_expensive_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.expensive_test`` marker.
 """
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_requires_network.py` & `pytest-skip-markers-1.4.1/tests/functional/test_requires_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.requires_network`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_if_binaries_missing.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_if_binaries_missing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_if_binaries_missing`` marker.
 """
 import os
 import sys
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_if_not_root.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_if_not_root.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_if_not_root`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_on_aarch64.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_on_aarch64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_on_aarch64`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_on_aix.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_on_aix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_on_aix`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_on_darwin.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_on_darwin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_on_darwin`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_on_env.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_on_env.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_on_env`` marker.
 """
 import os
 import sys
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_on_freebsd.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_smartos.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
-Test the ``@pytest.mark.skip_on_freebsd`` marker.
+Test the ``@pytest.mark.skip_unless_on_smartos`` marker.
 """
 import sys
 from unittest import mock
 
 import pytest
 
 pytestmark = [
@@ -20,51 +20,51 @@
 
 
 def test_skipped(pytester):
     pytester.makepyfile(
         """
         import pytest
 
-        @pytest.mark.skip_on_freebsd
+        @pytest.mark.skip_unless_on_smartos
         def test_one():
             assert True
         """
     )
-    return_value = True
-    with mock.patch("pytestskipmarkers.utils.platform.is_freebsd", return_value=return_value):
+    return_value = False
+    with mock.patch("pytestskipmarkers.utils.platform.is_smartos", return_value=return_value):
         res = pytester.runpytest_inprocess()
         res.assert_outcomes(skipped=1)
     res.stdout.no_fnmatch_line("*PytestUnknownMarkWarning*")
 
 
 def test_not_skipped(pytester):
     pytester.makepyfile(
         """
         import pytest
 
-        @pytest.mark.skip_on_freebsd
+        @pytest.mark.skip_unless_on_smartos
         def test_one():
             assert True
         """
     )
-    return_value = False
-    with mock.patch("pytestskipmarkers.utils.platform.is_freebsd", return_value=return_value):
+    return_value = True
+    with mock.patch("pytestskipmarkers.utils.platform.is_smartos", return_value=return_value):
         res = pytester.runpytest_inprocess()
         res.assert_outcomes(passed=1)
     res.stdout.no_fnmatch_line("*PytestUnknownMarkWarning*")
 
 
 def test_skip_reason(pytester):
     pytester.makepyfile(
         """
         import pytest
 
-        @pytest.mark.skip_on_freebsd(reason='Because!')
+        @pytest.mark.skip_unless_on_smartos(reason='Because!')
         def test_one():
             assert True
         """
     )
-    return_value = True
-    with mock.patch("pytestskipmarkers.utils.platform.is_freebsd", return_value=return_value):
+    return_value = False
+    with mock.patch("pytestskipmarkers.utils.platform.is_smartos", return_value=return_value):
         res = pytester.runpytest_inprocess("-ra", "-s", "-vv")
         res.assert_outcomes(skipped=1)
     res.stdout.fnmatch_lines(["SKIPPED * test_skip_reason.py:*: Because!"])
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_on_linux.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_on_linux.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_on_linux`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_on_netbsd.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_on_netbsd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_on_netbsd`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_on_openbsd.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_on_openbsd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_on_openbsd`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_on_photonos.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_on_photonos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_on_photonos`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_on_platforms.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_on_platforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_on_platforms`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_on_smartos.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_on_smartos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_on_smartos`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_on_spawning_platform.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_on_spawning_platform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_on_spawning_platform`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_on_sunos.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_on_sunos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_on_sunos`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_on_windows.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_on_windows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_on_windows`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_aarch64.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_aarch64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_unless_on_aarch64`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_aix.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_aix.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_unless_on_aix`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_darwin.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_darwin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_unless_on_darwin`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_freebsd.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_freebsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_unless_on_freebsd`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_linux.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_linux.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_unless_on_linux`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_netbsd.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_netbsd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_unless_on_netbsd`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_openbsd.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_openbsd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_unless_on_openbsd`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_photonos.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_photonos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_unless_on_photonos`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_platforms.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_platforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_unless_on_platforms`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_smartos.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_spawning_platform.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
-Test the ``@pytest.mark.skip_unless_on_smartos`` marker.
+Test the ``@pytest.mark.skip_unless_on_spawning_platform`` marker.
 """
 import sys
 from unittest import mock
 
 import pytest
 
 pytestmark = [
@@ -20,51 +20,48 @@
 
 
 def test_skipped(pytester):
     pytester.makepyfile(
         """
         import pytest
 
-        @pytest.mark.skip_unless_on_smartos
+        @pytest.mark.skip_unless_on_spawning_platform
         def test_one():
             assert True
         """
     )
-    return_value = False
-    with mock.patch("pytestskipmarkers.utils.platform.is_smartos", return_value=return_value):
+    with mock.patch("pytestskipmarkers.utils.platform.is_spawning_platform", return_value=False):
         res = pytester.runpytest_inprocess()
         res.assert_outcomes(skipped=1)
     res.stdout.no_fnmatch_line("*PytestUnknownMarkWarning*")
 
 
 def test_not_skipped(pytester):
     pytester.makepyfile(
         """
         import pytest
 
-        @pytest.mark.skip_unless_on_smartos
+        @pytest.mark.skip_unless_on_spawning_platform
         def test_one():
             assert True
         """
     )
-    return_value = True
-    with mock.patch("pytestskipmarkers.utils.platform.is_smartos", return_value=return_value):
+    with mock.patch("pytestskipmarkers.utils.platform.is_spawning_platform", return_value=True):
         res = pytester.runpytest_inprocess()
         res.assert_outcomes(passed=1)
     res.stdout.no_fnmatch_line("*PytestUnknownMarkWarning*")
 
 
 def test_skip_reason(pytester):
     pytester.makepyfile(
         """
         import pytest
 
-        @pytest.mark.skip_unless_on_smartos(reason='Because!')
+        @pytest.mark.skip_unless_on_spawning_platform(reason='Because!')
         def test_one():
             assert True
         """
     )
-    return_value = False
-    with mock.patch("pytestskipmarkers.utils.platform.is_smartos", return_value=return_value):
+    with mock.patch("pytestskipmarkers.utils.platform.is_spawning_platform", return_value=False):
         res = pytester.runpytest_inprocess("-ra", "-s", "-vv")
         res.assert_outcomes(skipped=1)
     res.stdout.fnmatch_lines(["SKIPPED * test_skip_reason.py:*: Because!"])
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_spawning_platform.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_on_freebsd.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
-Test the ``@pytest.mark.skip_unless_on_spawning_platform`` marker.
+Test the ``@pytest.mark.skip_on_freebsd`` marker.
 """
 import sys
 from unittest import mock
 
 import pytest
 
 pytestmark = [
@@ -20,48 +20,51 @@
 
 
 def test_skipped(pytester):
     pytester.makepyfile(
         """
         import pytest
 
-        @pytest.mark.skip_unless_on_spawning_platform
+        @pytest.mark.skip_on_freebsd
         def test_one():
             assert True
         """
     )
-    with mock.patch("pytestskipmarkers.utils.platform.is_spawning_platform", return_value=False):
+    return_value = True
+    with mock.patch("pytestskipmarkers.utils.platform.is_freebsd", return_value=return_value):
         res = pytester.runpytest_inprocess()
         res.assert_outcomes(skipped=1)
     res.stdout.no_fnmatch_line("*PytestUnknownMarkWarning*")
 
 
 def test_not_skipped(pytester):
     pytester.makepyfile(
         """
         import pytest
 
-        @pytest.mark.skip_unless_on_spawning_platform
+        @pytest.mark.skip_on_freebsd
         def test_one():
             assert True
         """
     )
-    with mock.patch("pytestskipmarkers.utils.platform.is_spawning_platform", return_value=True):
+    return_value = False
+    with mock.patch("pytestskipmarkers.utils.platform.is_freebsd", return_value=return_value):
         res = pytester.runpytest_inprocess()
         res.assert_outcomes(passed=1)
     res.stdout.no_fnmatch_line("*PytestUnknownMarkWarning*")
 
 
 def test_skip_reason(pytester):
     pytester.makepyfile(
         """
         import pytest
 
-        @pytest.mark.skip_unless_on_spawning_platform(reason='Because!')
+        @pytest.mark.skip_on_freebsd(reason='Because!')
         def test_one():
             assert True
         """
     )
-    with mock.patch("pytestskipmarkers.utils.platform.is_spawning_platform", return_value=False):
+    return_value = True
+    with mock.patch("pytestskipmarkers.utils.platform.is_freebsd", return_value=return_value):
         res = pytester.runpytest_inprocess("-ra", "-s", "-vv")
         res.assert_outcomes(skipped=1)
     res.stdout.fnmatch_lines(["SKIPPED * test_skip_reason.py:*: Because!"])
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_sunos.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_sunos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_unless_on_sunos`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/functional/test_skip_unless_on_windows.py` & `pytest-skip-markers-1.4.1/tests/functional/test_skip_unless_on_windows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the ``@pytest.mark.skip_unless_on_windows`` marker.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/unit/utils/markers/test_skip_if_binaries_missing.py` & `pytest-skip-markers-1.4.1/tests/unit/utils/markers/test_skip_if_binaries_missing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the "skip_if_binaries_missing" marker helper.
 """
 import os
 import sys
```

### Comparing `pytest-skip-markers-1.4.0/tests/unit/utils/markers/test_skip_if_no_local_network.py` & `pytest-skip-markers-1.4.1/tests/unit/utils/markers/test_skip_if_no_local_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the "skip_if_no_local_network" marker helper.
 """
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/unit/utils/markers/test_skip_if_no_remote_network.py` & `pytest-skip-markers-1.4.1/tests/unit/utils/markers/test_skip_if_no_remote_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the "skip_if_no_remote_network" marker helper.
 """
 import os
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/unit/utils/markers/test_skip_if_not_root.py` & `pytest-skip-markers-1.4.1/tests/unit/utils/markers/test_skip_if_not_root.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the "skip_if_not_root" marker helper.
 """
 import sys
 from unittest import mock
```

### Comparing `pytest-skip-markers-1.4.0/tests/unit/utils/markers/test_skip_on_env.py` & `pytest-skip-markers-1.4.1/tests/unit/utils/markers/test_skip_on_env.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the "skip_on_env" marker helper.
 """
 import logging
 import os
```

### Comparing `pytest-skip-markers-1.4.0/tests/unit/utils/test_platform.py` & `pytest-skip-markers-1.4.1/tests/unit/utils/test_platform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Tests for pytestskipmarkers.utils.platform.
 """
 import logging
 import subprocess
```

### Comparing `pytest-skip-markers-1.4.0/tests/unit/utils/test_ports.py` & `pytest-skip-markers-1.4.1/tests/unit/utils/test_ports.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2022 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 #
 """
 Test the port related utilities.
 """
 import functools
 from unittest import mock
```

