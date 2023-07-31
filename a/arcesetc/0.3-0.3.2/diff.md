# Comparing `tmp/arcesetc-0.3.tar.gz` & `tmp/arcesetc-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcesetc-0.3.tar", last modified: Fri Jul 28 18:57:25 2023, max compression
+gzip compressed data, was "arcesetc-0.3.2.tar", last modified: Mon Jul 31 15:56:54 2023, max compression
```

## Comparing `arcesetc-0.3.tar` & `arcesetc-0.3.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.926827 arcesetc-0.3/
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.902302 arcesetc-0.3/.github/
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.906566 arcesetc-0.3/.github/workflows/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      412 2023-07-28 18:34:36.000000 arcesetc-0.3/.github/workflows/ci.yml
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1902 2023-07-28 15:20:05.000000 arcesetc-0.3/.gitignore
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      606 2023-07-28 18:38:07.000000 arcesetc-0.3/.readthedocs.yml
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1072 2023-07-28 15:20:05.000000 arcesetc-0.3/LICENSE
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4759 2023-07-28 18:57:25.926637 arcesetc-0.3/PKG-INFO
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3140 2023-07-28 18:56:40.000000 arcesetc-0.3/README.rst
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.907978 arcesetc-0.3/arcesetc/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      453 2023-07-28 18:34:36.000000 arcesetc-0.3/arcesetc/__init__.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      878 2023-07-28 18:34:36.000000 arcesetc-0.3/arcesetc/conftest.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.917116 arcesetc-0.3/arcesetc/data/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   737280 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/data/BD28_4211.0026.wfrmcpc.fits
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   737280 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/data/HIP107864.0003.wfrmcpc.fits
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   737280 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/data/HR5191.0002.wfrmcpc.fits
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      246 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/data/README.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   987636 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/data/archive.hdf5
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2025 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/data/sptype_dict.json
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1152 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/data/sptype_to_temp.json
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     6732 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/plots.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.917594 arcesetc-0.3/arcesetc/tests/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      108 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/tests/__init__.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4099 2023-07-28 18:34:36.000000 arcesetc-0.3/arcesetc/tests/test_utils.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     9169 2023-07-28 15:20:05.000000 arcesetc-0.3/arcesetc/util.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      155 2023-07-28 18:57:25.000000 arcesetc-0.3/arcesetc/version.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.909116 arcesetc-0.3/arcesetc.egg-info/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4759 2023-07-28 18:57:25.000000 arcesetc-0.3/arcesetc.egg-info/PKG-INFO
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2112 2023-07-28 18:57:25.000000 arcesetc-0.3/arcesetc.egg-info/SOURCES.txt
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2023-07-28 18:57:25.000000 arcesetc-0.3/arcesetc.egg-info/dependency_links.txt
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2023-07-28 15:33:13.000000 arcesetc-0.3/arcesetc.egg-info/not-zip-safe
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      248 2023-07-28 18:57:25.000000 arcesetc-0.3/arcesetc.egg-info/requires.txt
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       44 2023-07-28 18:57:25.000000 arcesetc-0.3/arcesetc.egg-info/top_level.txt
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1853 2023-07-28 15:20:05.000000 arcesetc-0.3/contributing.rst
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.919161 arcesetc-0.3/docs/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       98 2023-07-28 18:37:19.000000 arcesetc-0.3/docs/.rtd_environment.yaml
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2719 2023-07-28 18:34:36.000000 arcesetc-0.3/docs/Makefile
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.902947 arcesetc-0.3/docs/_build/
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.903823 arcesetc-0.3/docs/_build/html/
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.903732 arcesetc-0.3/docs/_build/html/_downloads/
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.919363 arcesetc-0.3/docs/_build/html/_downloads/1285442fc69ec296739193a5bb01cfd3/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      271 2023-07-28 18:25:45.000000 arcesetc-0.3/docs/_build/html/_downloads/1285442fc69ec296739193a5bb01cfd3/gettingstarted-4.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.919628 arcesetc-0.3/docs/_build/html/_downloads/134ab96a9d43a359afd7287f2aa43fe5/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      271 2023-07-28 18:32:03.000000 arcesetc-0.3/docs/_build/html/_downloads/134ab96a9d43a359afd7287f2aa43fe5/gettingstarted-4.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.919888 arcesetc-0.3/docs/_build/html/_downloads/841caadd042d58ca8a1c4363a8e368a7/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      276 2023-07-28 18:25:45.000000 arcesetc-0.3/docs/_build/html/_downloads/841caadd042d58ca8a1c4363a8e368a7/gettingstarted-2.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.920165 arcesetc-0.3/docs/_build/html/_downloads/b66b1a2ed9b3ca7d529871c1355618c7/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      280 2023-07-28 18:25:45.000000 arcesetc-0.3/docs/_build/html/_downloads/b66b1a2ed9b3ca7d529871c1355618c7/gettingstarted-1.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.920460 arcesetc-0.3/docs/_build/html/_downloads/c5ac9a86f2a29263110f45bf565f7bd4/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      270 2023-07-28 18:25:45.000000 arcesetc-0.3/docs/_build/html/_downloads/c5ac9a86f2a29263110f45bf565f7bd4/gettingstarted-3.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.920739 arcesetc-0.3/docs/_build/html/_downloads/d90ff9160e5ef651bae7944605ca23d4/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      280 2023-07-28 18:32:02.000000 arcesetc-0.3/docs/_build/html/_downloads/d90ff9160e5ef651bae7944605ca23d4/gettingstarted-1.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.921011 arcesetc-0.3/docs/_build/html/_downloads/d97ef3d967eb2cc595a6a4c3ad1454e7/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      276 2023-07-28 18:32:02.000000 arcesetc-0.3/docs/_build/html/_downloads/d97ef3d967eb2cc595a6a4c3ad1454e7/gettingstarted-2.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.921305 arcesetc-0.3/docs/_build/html/_downloads/da6f961d2f854338ba956b87cf0e425a/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      270 2023-07-28 18:32:03.000000 arcesetc-0.3/docs/_build/html/_downloads/da6f961d2f854338ba956b87cf0e425a/gettingstarted-3.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.903886 arcesetc-0.3/docs/_build/html/plot_directive/
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.922361 arcesetc-0.3/docs/_build/html/plot_directive/arcesetc/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      280 2023-07-28 18:32:02.000000 arcesetc-0.3/docs/_build/html/plot_directive/arcesetc/gettingstarted-1.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      276 2023-07-28 18:32:02.000000 arcesetc-0.3/docs/_build/html/plot_directive/arcesetc/gettingstarted-2.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      270 2023-07-28 18:32:03.000000 arcesetc-0.3/docs/_build/html/plot_directive/arcesetc/gettingstarted-3.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      271 2023-07-28 18:32:03.000000 arcesetc-0.3/docs/_build/html/plot_directive/arcesetc/gettingstarted-4.py
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.904040 arcesetc-0.3/docs/_templates/
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.923092 arcesetc-0.3/docs/_templates/autosummary/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      250 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/_templates/autosummary/base.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      251 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      252 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.924119 arcesetc-0.3/docs/arcesetc/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    59283 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/arcesetc/cmd.png
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3768 2023-07-28 18:34:36.000000 arcesetc-0.3/docs/arcesetc/gettingstarted.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      165 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/arcesetc/index.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      485 2023-07-28 18:34:36.000000 arcesetc-0.3/docs/arcesetc/installation.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2003 2023-07-28 18:34:36.000000 arcesetc-0.3/docs/arcesetc/nextsteps.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     5913 2023-07-28 18:34:36.000000 arcesetc-0.3/docs/conf.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      780 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/index.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3426 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/paper.bib
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3131 2023-07-28 15:20:05.000000 arcesetc-0.3/docs/paper.md
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.925734 arcesetc-0.3/licenses/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     9745 2023-07-28 15:20:05.000000 arcesetc-0.3/licenses/APACHE2.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1305 2023-07-28 15:20:05.000000 arcesetc-0.3/licenses/BSD2.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1510 2023-07-28 15:20:05.000000 arcesetc-0.3/licenses/BSD3.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    37593 2023-07-28 15:20:05.000000 arcesetc-0.3/licenses/GPLv3.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1054 2023-07-28 15:20:05.000000 arcesetc-0.3/licenses/MIT.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      372 2023-07-28 15:20:05.000000 arcesetc-0.3/licenses/README.rst
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1659 2023-07-28 15:20:05.000000 arcesetc-0.3/licenses/TEMPLATE_LICENCE.rst
-drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-28 18:57:25.925909 arcesetc-0.3/notebooks/
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   241099 2023-07-28 15:20:05.000000 arcesetc-0.3/notebooks/example.ipynb
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2128 2023-07-28 18:34:36.000000 arcesetc-0.3/pyproject.toml
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       38 2023-07-28 18:57:25.926878 arcesetc-0.3/setup.cfg
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       61 2023-07-28 18:34:36.000000 arcesetc-0.3/setup.py
--rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1763 2023-07-28 18:34:36.000000 arcesetc-0.3/tox.ini
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.556864 arcesetc-0.3.2/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.533062 arcesetc-0.3.2/.github/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.537033 arcesetc-0.3.2/.github/workflows/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      412 2023-07-29 00:22:36.000000 arcesetc-0.3.2/.github/workflows/ci.yml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1902 2023-07-28 15:20:05.000000 arcesetc-0.3.2/.gitignore
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      606 2023-07-28 18:38:07.000000 arcesetc-0.3.2/.readthedocs.yml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1072 2023-07-28 15:20:05.000000 arcesetc-0.3.2/LICENSE
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4761 2023-07-31 15:56:54.556673 arcesetc-0.3.2/PKG-INFO
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3140 2023-07-28 18:56:40.000000 arcesetc-0.3.2/README.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.538657 arcesetc-0.3.2/arcesetc/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      266 2023-07-31 14:40:48.000000 arcesetc-0.3.2/arcesetc/__init__.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      878 2023-07-28 18:34:36.000000 arcesetc-0.3.2/arcesetc/conftest.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.546887 arcesetc-0.3.2/arcesetc/data/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   737280 2023-07-28 15:20:05.000000 arcesetc-0.3.2/arcesetc/data/BD28_4211.0026.wfrmcpc.fits
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   737280 2023-07-28 15:20:05.000000 arcesetc-0.3.2/arcesetc/data/HIP107864.0003.wfrmcpc.fits
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   737280 2023-07-28 15:20:05.000000 arcesetc-0.3.2/arcesetc/data/HR5191.0002.wfrmcpc.fits
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      246 2023-07-28 15:20:05.000000 arcesetc-0.3.2/arcesetc/data/README.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   987636 2023-07-28 15:20:05.000000 arcesetc-0.3.2/arcesetc/data/archive.hdf5
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2025 2023-07-28 15:20:05.000000 arcesetc-0.3.2/arcesetc/data/sptype_dict.json
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1152 2023-07-28 15:20:05.000000 arcesetc-0.3.2/arcesetc/data/sptype_to_temp.json
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     6732 2023-07-28 15:20:05.000000 arcesetc-0.3.2/arcesetc/plots.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.547291 arcesetc-0.3.2/arcesetc/tests/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      108 2023-07-28 15:20:05.000000 arcesetc-0.3.2/arcesetc/tests/__init__.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4099 2023-07-28 18:34:36.000000 arcesetc-0.3.2/arcesetc/tests/test_utils.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     9169 2023-07-28 15:20:05.000000 arcesetc-0.3.2/arcesetc/util.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      160 2023-07-31 15:56:54.000000 arcesetc-0.3.2/arcesetc/version.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.539816 arcesetc-0.3.2/arcesetc.egg-info/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     4761 2023-07-31 15:56:54.000000 arcesetc-0.3.2/arcesetc.egg-info/PKG-INFO
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2112 2023-07-31 15:56:54.000000 arcesetc-0.3.2/arcesetc.egg-info/SOURCES.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2023-07-31 15:56:54.000000 arcesetc-0.3.2/arcesetc.egg-info/dependency_links.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)        1 2023-07-28 15:33:13.000000 arcesetc-0.3.2/arcesetc.egg-info/not-zip-safe
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      248 2023-07-31 15:56:54.000000 arcesetc-0.3.2/arcesetc.egg-info/requires.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       44 2023-07-31 15:56:54.000000 arcesetc-0.3.2/arcesetc.egg-info/top_level.txt
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1853 2023-07-28 15:20:05.000000 arcesetc-0.3.2/contributing.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.548691 arcesetc-0.3.2/docs/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       98 2023-07-28 18:37:19.000000 arcesetc-0.3.2/docs/.rtd_environment.yaml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2719 2023-07-28 18:34:36.000000 arcesetc-0.3.2/docs/Makefile
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.533703 arcesetc-0.3.2/docs/_build/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.534571 arcesetc-0.3.2/docs/_build/html/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.534467 arcesetc-0.3.2/docs/_build/html/_downloads/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.548877 arcesetc-0.3.2/docs/_build/html/_downloads/1285442fc69ec296739193a5bb01cfd3/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      271 2023-07-28 18:25:45.000000 arcesetc-0.3.2/docs/_build/html/_downloads/1285442fc69ec296739193a5bb01cfd3/gettingstarted-4.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.549142 arcesetc-0.3.2/docs/_build/html/_downloads/134ab96a9d43a359afd7287f2aa43fe5/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      271 2023-07-28 18:32:03.000000 arcesetc-0.3.2/docs/_build/html/_downloads/134ab96a9d43a359afd7287f2aa43fe5/gettingstarted-4.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.549391 arcesetc-0.3.2/docs/_build/html/_downloads/841caadd042d58ca8a1c4363a8e368a7/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      276 2023-07-28 18:25:45.000000 arcesetc-0.3.2/docs/_build/html/_downloads/841caadd042d58ca8a1c4363a8e368a7/gettingstarted-2.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.549660 arcesetc-0.3.2/docs/_build/html/_downloads/b66b1a2ed9b3ca7d529871c1355618c7/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      280 2023-07-28 18:25:45.000000 arcesetc-0.3.2/docs/_build/html/_downloads/b66b1a2ed9b3ca7d529871c1355618c7/gettingstarted-1.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.549945 arcesetc-0.3.2/docs/_build/html/_downloads/c5ac9a86f2a29263110f45bf565f7bd4/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      270 2023-07-28 18:25:45.000000 arcesetc-0.3.2/docs/_build/html/_downloads/c5ac9a86f2a29263110f45bf565f7bd4/gettingstarted-3.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.550233 arcesetc-0.3.2/docs/_build/html/_downloads/d90ff9160e5ef651bae7944605ca23d4/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      280 2023-07-28 18:32:02.000000 arcesetc-0.3.2/docs/_build/html/_downloads/d90ff9160e5ef651bae7944605ca23d4/gettingstarted-1.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.550508 arcesetc-0.3.2/docs/_build/html/_downloads/d97ef3d967eb2cc595a6a4c3ad1454e7/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      276 2023-07-28 18:32:02.000000 arcesetc-0.3.2/docs/_build/html/_downloads/d97ef3d967eb2cc595a6a4c3ad1454e7/gettingstarted-2.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.550784 arcesetc-0.3.2/docs/_build/html/_downloads/da6f961d2f854338ba956b87cf0e425a/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      270 2023-07-28 18:32:03.000000 arcesetc-0.3.2/docs/_build/html/_downloads/da6f961d2f854338ba956b87cf0e425a/gettingstarted-3.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.534639 arcesetc-0.3.2/docs/_build/html/plot_directive/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.551768 arcesetc-0.3.2/docs/_build/html/plot_directive/arcesetc/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      280 2023-07-28 18:32:02.000000 arcesetc-0.3.2/docs/_build/html/plot_directive/arcesetc/gettingstarted-1.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      276 2023-07-28 18:32:02.000000 arcesetc-0.3.2/docs/_build/html/plot_directive/arcesetc/gettingstarted-2.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      270 2023-07-28 18:32:03.000000 arcesetc-0.3.2/docs/_build/html/plot_directive/arcesetc/gettingstarted-3.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      271 2023-07-28 18:32:03.000000 arcesetc-0.3.2/docs/_build/html/plot_directive/arcesetc/gettingstarted-4.py
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.534798 arcesetc-0.3.2/docs/_templates/
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.552602 arcesetc-0.3.2/docs/_templates/autosummary/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      250 2023-07-28 15:20:05.000000 arcesetc-0.3.2/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      251 2023-07-28 15:20:05.000000 arcesetc-0.3.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      252 2023-07-28 15:20:05.000000 arcesetc-0.3.2/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.553972 arcesetc-0.3.2/docs/arcesetc/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    59283 2023-07-28 15:20:05.000000 arcesetc-0.3.2/docs/arcesetc/cmd.png
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3768 2023-07-28 18:34:36.000000 arcesetc-0.3.2/docs/arcesetc/gettingstarted.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      165 2023-07-28 15:20:05.000000 arcesetc-0.3.2/docs/arcesetc/index.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      485 2023-07-28 18:34:36.000000 arcesetc-0.3.2/docs/arcesetc/installation.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2003 2023-07-28 18:34:36.000000 arcesetc-0.3.2/docs/arcesetc/nextsteps.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     5910 2023-07-31 15:48:56.000000 arcesetc-0.3.2/docs/conf.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      780 2023-07-28 15:20:05.000000 arcesetc-0.3.2/docs/index.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3426 2023-07-28 15:20:05.000000 arcesetc-0.3.2/docs/paper.bib
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     3131 2023-07-28 15:20:05.000000 arcesetc-0.3.2/docs/paper.md
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.555750 arcesetc-0.3.2/licenses/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     9745 2023-07-28 15:20:05.000000 arcesetc-0.3.2/licenses/APACHE2.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1305 2023-07-28 15:20:05.000000 arcesetc-0.3.2/licenses/BSD2.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1510 2023-07-28 15:20:05.000000 arcesetc-0.3.2/licenses/BSD3.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)    37593 2023-07-28 15:20:05.000000 arcesetc-0.3.2/licenses/GPLv3.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1054 2023-07-28 15:20:05.000000 arcesetc-0.3.2/licenses/MIT.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      372 2023-07-28 15:20:05.000000 arcesetc-0.3.2/licenses/README.rst
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1659 2023-07-28 15:20:05.000000 arcesetc-0.3.2/licenses/TEMPLATE_LICENCE.rst
+drwxr-xr-x   0 bmmorris  (5602) STSCI\science  (1031)        0 2023-07-31 15:56:54.555932 arcesetc-0.3.2/notebooks/
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)   241099 2023-07-28 15:20:05.000000 arcesetc-0.3.2/notebooks/example.ipynb
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     2128 2023-07-28 18:34:36.000000 arcesetc-0.3.2/pyproject.toml
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)       38 2023-07-31 15:56:54.556917 arcesetc-0.3.2/setup.cfg
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)      578 2023-07-31 15:49:07.000000 arcesetc-0.3.2/setup.py
+-rw-r--r--   0 bmmorris  (5602) STSCI\science  (1031)     1763 2023-07-28 18:34:36.000000 arcesetc-0.3.2/tox.ini
```

### Comparing `arcesetc-0.3/.gitignore` & `arcesetc-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/.readthedocs.yml` & `arcesetc-0.3.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/LICENSE` & `arcesetc-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/PKG-INFO` & `arcesetc-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcesetc
-Version: 0.3
+Version: 0.3.2
 Summary: Exposure time calculator for APO/ARCES
 Author: Trevor Dorn-Wallenstein
 Author-email: Brett Morris <morrisbrettm@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Brett M. Morris
```

### Comparing `arcesetc-0.3/README.rst` & `arcesetc-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/arcesetc/conftest.py` & `arcesetc-0.3.2/arcesetc/conftest.py`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/arcesetc/data/BD28_4211.0026.wfrmcpc.fits` & `arcesetc-0.3.2/arcesetc/data/BD28_4211.0026.wfrmcpc.fits`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/arcesetc/data/HIP107864.0003.wfrmcpc.fits` & `arcesetc-0.3.2/arcesetc/data/HIP107864.0003.wfrmcpc.fits`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/arcesetc/data/HR5191.0002.wfrmcpc.fits` & `arcesetc-0.3.2/arcesetc/data/HR5191.0002.wfrmcpc.fits`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/arcesetc/data/archive.hdf5` & `arcesetc-0.3.2/arcesetc/data/archive.hdf5`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/arcesetc/data/sptype_dict.json` & `arcesetc-0.3.2/arcesetc/data/sptype_dict.json`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/arcesetc/data/sptype_to_temp.json` & `arcesetc-0.3.2/arcesetc/data/sptype_to_temp.json`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/arcesetc/plots.py` & `arcesetc-0.3.2/arcesetc/plots.py`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/arcesetc/tests/test_utils.py` & `arcesetc-0.3.2/arcesetc/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/arcesetc/util.py` & `arcesetc-0.3.2/arcesetc/util.py`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/arcesetc.egg-info/PKG-INFO` & `arcesetc-0.3.2/arcesetc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcesetc
-Version: 0.3
+Version: 0.3.2
 Summary: Exposure time calculator for APO/ARCES
 Author: Trevor Dorn-Wallenstein
 Author-email: Brett Morris <morrisbrettm@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Brett M. Morris
```

### Comparing `arcesetc-0.3/arcesetc.egg-info/SOURCES.txt` & `arcesetc-0.3.2/arcesetc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/contributing.rst` & `arcesetc-0.3.2/contributing.rst`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/docs/Makefile` & `arcesetc-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/docs/arcesetc/cmd.png` & `arcesetc-0.3.2/docs/arcesetc/cmd.png`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/docs/arcesetc/gettingstarted.rst` & `arcesetc-0.3.2/docs/arcesetc/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/docs/arcesetc/nextsteps.rst` & `arcesetc-0.3.2/docs/arcesetc/nextsteps.rst`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/docs/conf.py` & `arcesetc-0.3.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,19 @@
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 __import__(project)
 package = sys.modules[project]
 
-# The short X.Y version.
-version = package.__version__.split('-', 1)[0]
 # The full version, including alpha/beta/rc tags.
-release = package.__version__
+release = __version__
+dev = "dev" in release
+# The short X.Y version.
+version = '.'.join(release.split('.')[:2])
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # A NOTE ON HTML THEMES
 # The global astropy configuration uses a custom theme, 'bootstrap-astropy',
 # which is installed along with astropy. A different theme can be used or
@@ -86,15 +87,15 @@
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
 #html_last_updated_fmt = ''
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-html_title = '{0} v{1}'.format(project, release)
+html_title = '{0}'.format(project)
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = project + 'doc'
 
 # Prefixes that are ignored for sorting the Python module index
 modindex_common_prefix = ["arcesetc."]
```

### Comparing `arcesetc-0.3/docs/index.rst` & `arcesetc-0.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/docs/paper.bib` & `arcesetc-0.3.2/docs/paper.bib`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/docs/paper.md` & `arcesetc-0.3.2/docs/paper.md`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/licenses/APACHE2.rst` & `arcesetc-0.3.2/licenses/APACHE2.rst`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/licenses/BSD2.rst` & `arcesetc-0.3.2/licenses/BSD2.rst`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/licenses/BSD3.rst` & `arcesetc-0.3.2/licenses/BSD3.rst`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/licenses/GPLv3.rst` & `arcesetc-0.3.2/licenses/GPLv3.rst`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/licenses/MIT.rst` & `arcesetc-0.3.2/licenses/MIT.rst`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/licenses/TEMPLATE_LICENCE.rst` & `arcesetc-0.3.2/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/notebooks/example.ipynb` & `arcesetc-0.3.2/notebooks/example.ipynb`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/pyproject.toml` & `arcesetc-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arcesetc-0.3/tox.ini` & `arcesetc-0.3.2/tox.ini`

 * *Files identical despite different names*

