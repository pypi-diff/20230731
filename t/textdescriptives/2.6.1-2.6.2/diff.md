# Comparing `tmp/textdescriptives-2.6.1.tar.gz` & `tmp/textdescriptives-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textdescriptives-2.6.1.tar", last modified: Wed May  3 07:18:23 2023, max compression
+gzip compressed data, was "textdescriptives-2.6.2.tar", last modified: Mon Jul 31 11:05:34 2023, max compression
```

## Comparing `textdescriptives-2.6.1.tar` & `textdescriptives-2.6.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.876781 textdescriptives-2.6.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.860781 textdescriptives-2.6.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.864781 textdescriptives-2.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      632 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.864781 textdescriptives-2.6.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/workflows/draft-pdf.yml
--rw-r--r--   0 root         (0) root         (0)     1673 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)      867 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/workflows/stale.yml
--rw-r--r--   0 root         (0) root         (0)     2254 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)     2140 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1388 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      907 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)     8642 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1361 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/CITATION.cff
--rw-r--r--   0 root         (0) root         (0)     5242 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4473 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    23729 2023-05-03 07:18:23.876781 textdescriptives-2.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9398 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.864781 textdescriptives-2.6.1/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.868781 textdescriptives-2.6.1/docs/_static/
--rw-r--r--   0 root         (0) root         (0)   642030 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   139565 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/_static/icon_dark_old.png
--rw-r--r--   0 root         (0) root         (0)   125611 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/_static/icon_old.png
--rw-r--r--   0 root         (0) root         (0)     3540 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/coherence.rst
--rw-r--r--   0 root         (0) root         (0)     3547 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     3189 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/dependencydistance.rst
--rw-r--r--   0 root         (0) root         (0)     3198 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/descriptivestats.rst
--rw-r--r--   0 root         (0) root         (0)      477 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/extractors.rst
--rw-r--r--   0 root         (0) root         (0)     1909 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2752 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     2140 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/information_theory.rst
--rw-r--r--   0 root         (0) root         (0)      859 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      795 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      987 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)     2784 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/posstats.rst
--rw-r--r--   0 root         (0) root         (0)     8242 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/quality.rst
--rw-r--r--   0 root         (0) root         (0)     4669 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/readability.md
--rw-r--r--   0 root         (0) root         (0)      388 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/tutorial.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.868781 textdescriptives-2.6.1/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    96689 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/tutorials/filter_corpus_using_quality.ipynb
--rw-r--r--   0 root         (0) root         (0)   115780 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/tutorials/introductory_tutorial.ipynb
--rw-r--r--   0 root         (0) root         (0)      273 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/tutorials/requirements.txt
--rw-r--r--   0 root         (0) root         (0)    13090 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/tutorials/sklearn_integration.ipynb
--rw-r--r--   0 root         (0) root         (0)     7465 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/docs/usingthepackage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.868781 textdescriptives-2.6.1/paper/
--rw-r--r--   0 root         (0) root         (0)    23688 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9237 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)    42220 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/paper/paper_quarto.pdf
--rw-r--r--   0 root         (0) root         (0)     9724 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/paper/paper_quarto.qmd
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/paper/readme.md
--rw-r--r--   0 root         (0) root         (0)     3038 2023-05-03 07:18:13.000000 textdescriptives-2.6.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 07:18:23.876781 textdescriptives-2.6.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.860781 textdescriptives-2.6.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.868781 textdescriptives-2.6.1/src/textdescriptives/
--rw-r--r--   0 root         (0) root         (0)      328 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/__init__.py
--rw-r--r--   0 root         (0) root         (0)      492 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/about.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.872781 textdescriptives-2.6.1/src/textdescriptives/components/
--rw-r--r--   0 root         (0) root         (0)      396 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5353 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/coherence.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     7504 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     5515 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/information_theory.py
--rw-r--r--   0 root         (0) root         (0)     4087 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)    22254 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/quality.py
--rw-r--r--   0 root         (0) root         (0)    10426 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/quality_data_classes.py
--rw-r--r--   0 root         (0) root         (0)     7713 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/readability.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/components/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.872781 textdescriptives-2.6.1/src/textdescriptives/data/
--rw-r--r--   0 root         (0) root         (0)   503663 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/data/spam.csv
--rw-r--r--   0 root         (0) root         (0)     6126 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/extractors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.872781 textdescriptives-2.6.1/src/textdescriptives/integrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/integrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4355 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/integrations/sklearn_featurizer.py
--rw-r--r--   0 root         (0) root         (0)     1330 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/load_components.py
--rw-r--r--   0 root         (0) root         (0)     6203 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/src/textdescriptives/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.872781 textdescriptives-2.6.1/src/textdescriptives.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23729 2023-05-03 07:18:23.000000 textdescriptives-2.6.1/src/textdescriptives.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2507 2023-05-03 07:18:23.000000 textdescriptives-2.6.1/src/textdescriptives.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 07:18:23.000000 textdescriptives-2.6.1/src/textdescriptives.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      493 2023-05-03 07:18:23.000000 textdescriptives-2.6.1/src/textdescriptives.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-03 07:18:23.000000 textdescriptives-2.6.1/src/textdescriptives.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 07:18:23.876781 textdescriptives-2.6.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28399 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/books.py
--rw-r--r--   0 root         (0) root         (0)      382 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2821 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_coherence.py
--rw-r--r--   0 root         (0) root         (0)     2930 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     3505 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     5331 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_extractors.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_information.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_load_components.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)     9305 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_quality.py
--rw-r--r--   0 root         (0) root         (0)     4827 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_readability.py
--rw-r--r--   0 root         (0) root         (0)      572 2023-05-03 07:18:12.000000 textdescriptives-2.6.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:05:34.029662 textdescriptives-2.6.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:05:34.013662 textdescriptives-2.6.2/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:05:34.013662 textdescriptives-2.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      776 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:05:34.013662 textdescriptives-2.6.2/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      669 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)      867 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/.github/workflows/stale.yml
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1384 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      907 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)     8642 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/CITATION.cff
+-rw-r--r--   0 root         (0) root         (0)     5242 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    23729 2023-07-31 11:05:34.029662 textdescriptives-2.6.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9398 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:05:34.017662 textdescriptives-2.6.2/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:05:34.021662 textdescriptives-2.6.2/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)   642030 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   139565 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/_static/icon_dark_old.png
+-rw-r--r--   0 root         (0) root         (0)   125611 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/_static/icon_old.png
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/coherence.rst
+-rw-r--r--   0 root         (0) root         (0)     3547 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     3189 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/dependencydistance.rst
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/descriptivestats.rst
+-rw-r--r--   0 root         (0) root         (0)      477 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/extractors.rst
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/information_theory.rst
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      795 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      987 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)     2784 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/posstats.rst
+-rw-r--r--   0 root         (0) root         (0)     8242 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/quality.rst
+-rw-r--r--   0 root         (0) root         (0)     4669 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/readability.md
+-rw-r--r--   0 root         (0) root         (0)      388 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/tutorial.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:05:34.021662 textdescriptives-2.6.2/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    96689 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/tutorials/filter_corpus_using_quality.ipynb
+-rw-r--r--   0 root         (0) root         (0)   115780 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/tutorials/introductory_tutorial.ipynb
+-rw-r--r--   0 root         (0) root         (0)      273 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/tutorials/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)    13090 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/tutorials/sklearn_integration.ipynb
+-rw-r--r--   0 root         (0) root         (0)     7465 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/docs/usingthepackage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:05:34.021662 textdescriptives-2.6.2/paper/
+-rw-r--r--   0 root         (0) root         (0)    23688 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9237 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)    42220 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/paper/paper_quarto.pdf
+-rw-r--r--   0 root         (0) root         (0)     9724 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/paper/paper_quarto.qmd
+-rw-r--r--   0 root         (0) root         (0)      473 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/paper/readme.md
+-rw-r--r--   0 root         (0) root         (0)     3022 2023-07-31 11:05:26.000000 textdescriptives-2.6.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 11:05:34.029662 textdescriptives-2.6.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:05:34.009662 textdescriptives-2.6.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:05:34.021662 textdescriptives-2.6.2/src/textdescriptives/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      492 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/about.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:05:34.025662 textdescriptives-2.6.2/src/textdescriptives/components/
+-rw-r--r--   0 root         (0) root         (0)      396 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5353 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/components/coherence.py
+-rw-r--r--   0 root         (0) root         (0)     5705 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/components/dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     7504 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/components/descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     5515 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/components/information_theory.py
+-rw-r--r--   0 root         (0) root         (0)     4087 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/components/pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)    22254 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/components/quality.py
+-rw-r--r--   0 root         (0) root         (0)    10426 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/components/quality_data_classes.py
+-rw-r--r--   0 root         (0) root         (0)     7713 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/components/readability.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/components/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:05:34.025662 textdescriptives-2.6.2/src/textdescriptives/data/
+-rw-r--r--   0 root         (0) root         (0)   503663 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/data/spam.csv
+-rw-r--r--   0 root         (0) root         (0)     6126 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/extractors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:05:34.025662 textdescriptives-2.6.2/src/textdescriptives/integrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/integrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/integrations/sklearn_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/load_components.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/src/textdescriptives/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:05:34.025662 textdescriptives-2.6.2/src/textdescriptives.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23729 2023-07-31 11:05:33.000000 textdescriptives-2.6.2/src/textdescriptives.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2507 2023-07-31 11:05:34.000000 textdescriptives-2.6.2/src/textdescriptives.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 11:05:33.000000 textdescriptives-2.6.2/src/textdescriptives.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      473 2023-07-31 11:05:33.000000 textdescriptives-2.6.2/src/textdescriptives.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-31 11:05:33.000000 textdescriptives-2.6.2/src/textdescriptives.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 11:05:34.029662 textdescriptives-2.6.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28399 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/tests/books.py
+-rw-r--r--   0 root         (0) root         (0)      382 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/tests/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2821 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/tests/test_coherence.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/tests/test_dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/tests/test_descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/tests/test_extractors.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/tests/test_information.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/tests/test_load_components.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/tests/test_pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)     9305 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/tests/test_quality.py
+-rw-r--r--   0 root         (0) root         (0)     4827 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/tests/test_readability.py
+-rw-r--r--   0 root         (0) root         (0)      572 2023-07-31 11:05:22.000000 textdescriptives-2.6.2/tests/test_utils.py
```

### Comparing `textdescriptives-2.6.1/.github/ISSUE_TEMPLATE/01_bugs.md` & `textdescriptives-2.6.2/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/.github/ISSUE_TEMPLATE/config.yml` & `textdescriptives-2.6.2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/.github/dependabot.yml` & `textdescriptives-2.6.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/.github/workflows/dependabot_automerge.yml` & `textdescriptives-2.6.2/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/.github/workflows/documentation.yml` & `textdescriptives-2.6.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/.github/workflows/draft-pdf.yml` & `textdescriptives-2.6.2/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/.github/workflows/stale.yml` & `textdescriptives-2.6.2/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/.github/workflows/tests.yml` & `textdescriptives-2.6.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/.gitignore` & `textdescriptives-2.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/.pre-commit-config.yaml` & `textdescriptives-2.6.2/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 default_stages: [commit, push]
 
 ci:
   autofix_prs: false
 
 repos:
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
+    rev: v2.2.5
     hooks:
       - id: codespell
         args: [
             "-w", # Write changes to files
             "--skip",
             "*.csv,*.bib,tests/books.py,*.ipynb",
             # don't code output from notebooks
             "-L",
             "vise", # Ignore the Danish word 'vise'
           ]
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.2
+    rev: v3.9.0
     hooks:
       - id: pyupgrade
 
   - repo: https://github.com/bwhmather/ssort
     rev: v0.11.6
     hooks:
       - id: ssort
 
   - repo: https://github.com/asottile/add-trailing-comma
-    rev: v2.4.0
+    rev: v3.0.0
     hooks:
       - id: add-trailing-comma
 
   # - repo: https://github.com/PyCQA/docformatter
   #   rev: v1.6.0.rc1
   #   hooks:
   #     - id: docformatter
@@ -43,21 +43,21 @@
   #           --wrap-descriptions,
   #           "80",
   #           --wrap-summaries,
   #           "80",
   #         ]
 
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
         #args: [--line-length, "88"]
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.263
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.280
     hooks:
       - id: ruff
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
+    rev: v1.4.1
     hooks:
       - id: mypy
```

### Comparing `textdescriptives-2.6.1/.zenodo.json` & `textdescriptives-2.6.2/.zenodo.json`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/CHANGELOG.md` & `textdescriptives-2.6.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/CITATION.cff` & `textdescriptives-2.6.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/CODE_OF_CONDUCT.md` & `textdescriptives-2.6.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/CONTRIBUTING.md` & `textdescriptives-2.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/LICENSE` & `textdescriptives-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/PKG-INFO` & `textdescriptives-2.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.6.1
+Version: 2.6.2
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `textdescriptives-2.6.1/README.md` & `textdescriptives-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/Makefile` & `textdescriptives-2.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/_static/icon.png` & `textdescriptives-2.6.2/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/_static/icon_dark_old.png` & `textdescriptives-2.6.2/docs/_static/icon_dark_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/_static/icon_old.png` & `textdescriptives-2.6.2/docs/_static/icon_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/coherence.rst` & `textdescriptives-2.6.2/docs/coherence.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/conf.py` & `textdescriptives-2.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/dependencydistance.rst` & `textdescriptives-2.6.2/docs/dependencydistance.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/descriptivestats.rst` & `textdescriptives-2.6.2/docs/descriptivestats.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/faq.rst` & `textdescriptives-2.6.2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/index.rst` & `textdescriptives-2.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/information_theory.rst` & `textdescriptives-2.6.2/docs/information_theory.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/installation.rst` & `textdescriptives-2.6.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/make.bat` & `textdescriptives-2.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/news.rst` & `textdescriptives-2.6.2/docs/news.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/posstats.rst` & `textdescriptives-2.6.2/docs/posstats.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/quality.rst` & `textdescriptives-2.6.2/docs/quality.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/readability.md` & `textdescriptives-2.6.2/docs/readability.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/tutorials/filter_corpus_using_quality.ipynb` & `textdescriptives-2.6.2/docs/tutorials/filter_corpus_using_quality.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/tutorials/introductory_tutorial.ipynb` & `textdescriptives-2.6.2/docs/tutorials/introductory_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/tutorials/sklearn_integration.ipynb` & `textdescriptives-2.6.2/docs/tutorials/sklearn_integration.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/docs/usingthepackage.rst` & `textdescriptives-2.6.2/docs/usingthepackage.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/paper/paper.bib` & `textdescriptives-2.6.2/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/paper/paper.md` & `textdescriptives-2.6.2/paper/paper.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/paper/paper_quarto.pdf` & `textdescriptives-2.6.2/paper/paper_quarto.pdf`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/paper/paper_quarto.qmd` & `textdescriptives-2.6.2/paper/paper_quarto.qmd`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/pyproject.toml` & `textdescriptives-2.6.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "textdescriptives"
-version = "2.6.1"
+version = "2.6.2"
 description = "A library for calculating a variety of features from text using spaCy"
 authors = [{name = "Lasse Hansen", email = "lasseh0310@gmail.com"},
              {name = "Kenneth Enevoldsen"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
@@ -28,34 +28,34 @@
     "text statistics",
     "text descriptives",
     "text analytics",
     "text mining",
 ]
 
 dependencies = [
-    "spacy[lookups]>=3.1.0,<3.6.0",
-    "numpy>=1.20.0,<1.25.0",
-    "pandas>=1.0.0,<1.6.0",
+    "spacy[lookups]>=3.1.0",
+    "numpy>=1.20.0",
+    "pandas>=1.0.0",
     "pyphen>=0.11.0,<0.15.0",
     "ftfy>=6.0.3,<6.1.0",
 ]
 
 requires-python = ">=3.8"
 
 [project.urls]
 homepage = "https://hlasse.github.io/TextDescriptives/"
 repository = "https://github.com/HLasse/textdescriptives"
 documentation = "https://hlasse.github.io/TextDescriptives/"
 
 [project.optional-dependencies]
 style = [
     "black==23.3.0",
-    "pre-commit==3.2.2",
-    "ruff==0.0.263",
-    "mypy==1.1.1"
+    "pre-commit==3.3.3",
+    "ruff==0.0.275",
+    "mypy==1.4.1"
 ]
 tests = [
     "pytest>=7.1.3",
     "pytest-cov>=3.0.0",
 ]
 docs = [
     "sphinx>=5.3.0",
@@ -68,15 +68,15 @@
 ]
 tutorials = [
     "jupyter",
     "seaborn",
     "matplotlib",
     "datasets>=2.8.0",
     "scikit-learn>=1.1.1",
-    "ipython<=8.12",
+    "ipython<=8.14.0",
 ]
 sklearn = [
     "scikit-learn>=1.1.1",
 ]
 
 [project.readme]
 file = "README.md"
@@ -116,16 +116,16 @@
     # Don't complain if non-runnable code isn't run:
     "if 0:",
     "if __name__ == .__main__.:",
 ]
 
 [tool.semantic_release]
 branch = "main"
-version_variable = [
-    "pyproject.toml:version"
+version_toml = [
+    "pyproject.toml:project.version"
 ]
 build_command = "python -m pip install build; python -m build"
 
 [tool.ruff]
 exclude = [
     ".venv",
     ".env",
```

### Comparing `textdescriptives-2.6.1/src/textdescriptives/components/coherence.py` & `textdescriptives-2.6.2/src/textdescriptives/components/coherence.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/src/textdescriptives/components/dependency_distance.py` & `textdescriptives-2.6.2/src/textdescriptives/components/dependency_distance.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
         Returns:
             dict: Dictionary with the following keys: dependency_distance_mean:
                 Mean dependency distance and prop_adjacent_dependency_relation:
                 Proportion of adjacent dependency relations
         """
         dep_dists, adj_deps = zip(
-            *[token._.dependency_distance.values() for token in span]
+            *[token._.dependency_distance.values() for token in span],
         )
         return {
             "dependency_distance_mean": np.mean(dep_dists),
             "prop_adjacent_dependency_relation": np.mean(adj_deps),
         }
 
     def doc_dependency(self, doc: Doc) -> dict:
@@ -81,15 +81,15 @@
             return {
                 "dependency_distance_mean": np.nan,
                 "dependency_distance_std": np.nan,
                 "prop_adjacent_dependency_relation_mean": np.nan,
                 "prop_adjacent_dependency_relation_std": np.nan,
             }
         dep_dists, adj_deps = zip(
-            *[sent._.dependency_distance.values() for sent in doc.sents]
+            *[sent._.dependency_distance.values() for sent in doc.sents],
         )
         return {
             "dependency_distance_mean": np.mean(dep_dists),
             "dependency_distance_std": np.std(dep_dists),
             "prop_adjacent_dependency_relation_mean": np.mean(adj_deps),
             "prop_adjacent_dependency_relation_std": np.std(adj_deps),
         }
```

### Comparing `textdescriptives-2.6.1/src/textdescriptives/components/descriptive_stats.py` & `textdescriptives-2.6.2/src/textdescriptives/components/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/src/textdescriptives/components/information_theory.py` & `textdescriptives-2.6.2/src/textdescriptives/components/information_theory.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/src/textdescriptives/components/pos_proportions.py` & `textdescriptives-2.6.2/src/textdescriptives/components/pos_proportions.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/src/textdescriptives/components/quality.py` & `textdescriptives-2.6.2/src/textdescriptives/components/quality.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/src/textdescriptives/components/quality_data_classes.py` & `textdescriptives-2.6.2/src/textdescriptives/components/quality_data_classes.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/src/textdescriptives/components/readability.py` & `textdescriptives-2.6.2/src/textdescriptives/components/readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/src/textdescriptives/components/utils.py` & `textdescriptives-2.6.2/src/textdescriptives/components/utils.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/src/textdescriptives/data/spam.csv` & `textdescriptives-2.6.2/src/textdescriptives/data/spam.csv`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/src/textdescriptives/extractors.py` & `textdescriptives-2.6.2/src/textdescriptives/extractors.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/src/textdescriptives/integrations/sklearn_featurizer.py` & `textdescriptives-2.6.2/src/textdescriptives/integrations/sklearn_featurizer.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/src/textdescriptives/load_components.py` & `textdescriptives-2.6.2/src/textdescriptives/load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/src/textdescriptives/utils.py` & `textdescriptives-2.6.2/src/textdescriptives/utils.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/src/textdescriptives.egg-info/PKG-INFO` & `textdescriptives-2.6.2/src/textdescriptives.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.6.1
+Version: 2.6.2
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `textdescriptives-2.6.1/src/textdescriptives.egg-info/SOURCES.txt` & `textdescriptives-2.6.2/src/textdescriptives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/tests/books.py` & `textdescriptives-2.6.2/tests/books.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/tests/test_coherence.py` & `textdescriptives-2.6.2/tests/test_coherence.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/tests/test_dependency_distance.py` & `textdescriptives-2.6.2/tests/test_dependency_distance.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/tests/test_descriptive_stats.py` & `textdescriptives-2.6.2/tests/test_descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/tests/test_extractors.py` & `textdescriptives-2.6.2/tests/test_extractors.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/tests/test_information.py` & `textdescriptives-2.6.2/tests/test_information.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/tests/test_load_components.py` & `textdescriptives-2.6.2/tests/test_load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/tests/test_pos_proportions.py` & `textdescriptives-2.6.2/tests/test_pos_proportions.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/tests/test_quality.py` & `textdescriptives-2.6.2/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/tests/test_readability.py` & `textdescriptives-2.6.2/tests/test_readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.6.1/tests/test_utils.py` & `textdescriptives-2.6.2/tests/test_utils.py`

 * *Files identical despite different names*

