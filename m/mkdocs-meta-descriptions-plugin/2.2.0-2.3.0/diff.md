# Comparing `tmp/mkdocs-meta-descriptions-plugin-2.2.0.tar.gz` & `tmp/mkdocs-meta-descriptions-plugin-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-meta-descriptions-plugin-2.2.0.tar", last modified: Thu Dec 15 10:06:07 2022, max compression
+gzip compressed data, was "mkdocs-meta-descriptions-plugin-2.3.0.tar", last modified: Mon Jul 31 16:11:02 2023, max compression
```

## Comparing `mkdocs-meta-descriptions-plugin-2.2.0.tar` & `mkdocs-meta-descriptions-plugin-2.3.0.tar`

### file list

```diff
@@ -1,70 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 10:06:07.034244 mkdocs-meta-descriptions-plugin-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 10:06:07.018243 mkdocs-meta-descriptions-plugin-2.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 10:06:07.018243 mkdocs-meta-descriptions-plugin-2.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      558 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 10:06:07.018243 mkdocs-meta-descriptions-plugin-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/.github/workflows/test-build-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      463 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2022-12-15 10:06:07.034244 mkdocs-meta-descriptions-plugin-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 10:06:07.018243 mkdocs-meta-descriptions-plugin-2.2.0/images/
--rw-r--r--   0 runner    (1001) docker     (123)   121881 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/images/readme-example.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 10:06:07.022244 mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 10:06:07.022244 mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2022-12-15 10:06:06.000000 mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2022-12-15 10:06:07.000000 mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 10:06:06.000000 mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-15 10:06:06.000000 mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-15 10:06:06.000000 mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2022-12-15 10:06:06.000000 mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-15 10:06:07.034244 mkdocs-meta-descriptions-plugin-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 10:06:07.030244 mkdocs-meta-descriptions-plugin-2.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 10:06:07.034244 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/admonition-before-first-paragraph.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/escape-html-entities.md
--rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/filename with spaces.md
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/first-paragraph-no-heading.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/first-paragraph-no-intro.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/first-paragraph-no-paragraph.md
--rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/first-paragraph.md
--rw-r--r--   0 runner    (1001) docker     (123)      206 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/front-matter-description.md
--rw-r--r--   0 runner    (1001) docker     (123)      591 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/image.png
--rw-r--r--   0 runner    (1001) docker     (123)      491 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 10:06:07.034244 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/subdirectory/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/subdirectory/first-paragraph.md
--rw-r--r--   0 runner    (1001) docker     (123)      491 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/subdirectory/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/warning-long.md
--rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/warning-not-found.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/warning-short.md
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/meta-descriptions-no-directory-urls.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/meta-descriptions-no-site-description-no-directory-urls.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/meta-descriptions-no-site-description.csv
--rw-r--r--   0 runner    (1001) docker     (123)      929 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/meta-descriptions-no-site-url-no-directory-urls.csv
--rw-r--r--   0 runner    (1001) docker     (123)      861 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/meta-descriptions-no-site-url.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/meta-descriptions.csv
--rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/mkdocs-enable-checks-no-site-description.yml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/mkdocs-enable-checks.yml
--rw-r--r--   0 runner    (1001) docker     (123)      255 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/mkdocs-export-csv-no-site-description.yml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/mkdocs-export-csv-no-site-url.yml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/mkdocs-export-csv.yml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/mkdocs-no-site-description.yml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/mkdocs-quiet.yml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2022-12-15 10:05:45.000000 mkdocs-meta-descriptions-plugin-2.2.0/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:11:02.133383 mkdocs-meta-descriptions-plugin-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:11:02.117383 mkdocs-meta-descriptions-plugin-2.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:11:02.121384 mkdocs-meta-descriptions-plugin-2.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:11:02.121384 mkdocs-meta-descriptions-plugin-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/.github/workflows/test-build-deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-07-31 16:11:02.129383 mkdocs-meta-descriptions-plugin-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:11:02.121384 mkdocs-meta-descriptions-plugin-2.3.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   121881 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/images/readme-example.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:11:02.121384 mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:11:02.121384 mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-07-31 16:11:02.000000 mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-31 16:11:02.000000 mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:11:02.000000 mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-31 16:11:02.000000 mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-31 16:11:02.000000 mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 16:11:02.000000 mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 16:11:02.133383 mkdocs-meta-descriptions-plugin-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:11:02.129383 mkdocs-meta-descriptions-plugin-2.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:11:02.129383 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/admonition-before-first-paragraph.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/escape-html-entities.md
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/filename with spaces.md
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/first-paragraph-no-heading.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/first-paragraph-no-intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/first-paragraph-no-paragraph.md
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/first-paragraph.md
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/front-matter-description.md
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/image.png
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:11:02.129383 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/subdirectory/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/subdirectory/first-paragraph.md
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/subdirectory/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/trim-long-description.md
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/trim-long-first-paragraph.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/warning-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/warning-not-found.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/warning-short.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/meta-descriptions-no-directory-urls.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/meta-descriptions-no-site-description-no-directory-urls.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/meta-descriptions-no-site-description.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/meta-descriptions-no-site-url-no-directory-urls.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/meta-descriptions-no-site-url.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/meta-descriptions-trim-no-directory-urls.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/meta-descriptions-trim.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/meta-descriptions.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/mkdocs-enable-checks-no-site-description.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/mkdocs-enable-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/mkdocs-export-csv-no-site-description.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/mkdocs-export-csv-no-site-url.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/mkdocs-export-csv-trim.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/mkdocs-export-csv.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/mkdocs-no-site-description.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/mkdocs-quiet.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/mkdocs-trim-default.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/mkdocs-trim-max-length.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-07-31 16:10:31.000000 mkdocs-meta-descriptions-plugin-2.3.0/tests/test_plugin.py
```

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `mkdocs-meta-descriptions-plugin-2.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/.github/workflows/test-build-deploy.yml` & `mkdocs-meta-descriptions-plugin-2.3.0/.github/workflows/test-build-deploy.yml`

 * *Files 6% similar despite different names*

```diff
@@ -67,25 +67,32 @@
         with:
           name: coverage
 
       - name: Combine coverage data
         run:
           coverage combine
 
-      - name: Generate XML report of coverage results
+      - name: Generate XML coverage report
         run:
           coverage xml
 
       - name: Run codacy-coverage-reporter
         uses: codacy/codacy-coverage-reporter-action@v1.3
         if: always()
         with:
           project-token: ${{ secrets.CODACY_PROJECT_TOKEN }}
           coverage-reports: coverage.xml
 
+      - name: Upload XML coverage report artifact
+        uses: actions/upload-artifact@v3
+        with:
+          name: coverage.xml
+          path: coverage.xml
+          retention-days: 3
+
   build:
     name: Build
     needs: test
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
@@ -124,18 +131,18 @@
       - name: Download binaries artifact
         uses: actions/download-artifact@v3
         with:
           name: dist
           path: dist/
 
       - name: Deploy to Test PyPI
-        uses: pypa/gh-action-pypi-publish@v1.6.4
+        uses: pypa/gh-action-pypi-publish@v1.8.8
         with:
           password: ${{ secrets.PYPI_API_TOKEN_TEST }}
-          repository_url: https://test.pypi.org/legacy/
+          repository-url: https://test.pypi.org/legacy/
 
   deploy:
     name: Deploy to PyPI
     needs: build
     runs-on: ubuntu-latest
     if: startsWith(github.ref, 'refs/tags')
     steps:
@@ -144,15 +151,15 @@
       - name: Download binaries artifact
         uses: actions/download-artifact@v3
         with:
           name: dist
           path: dist/
 
       - name: Deploy to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.6.4
+        uses: pypa/gh-action-pypi-publish@v1.8.8
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
 
   deploy-gh-pages:
     name: Deploy GitHub Pages
     needs: deploy-test
     runs-on: ubuntu-latest
```

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/.gitignore` & `mkdocs-meta-descriptions-plugin-2.3.0/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -105,16 +105,17 @@
 # Spyder project settings
 .spyderproject
 .spyproject
 
 # Rope project settings
 .ropeproject
 
-# mkdocs documentation
+# MkDocs documentation
 /site
+/tests/site
 
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
```

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/CHANGELOG.md` & `mkdocs-meta-descriptions-plugin-2.3.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 # Change log
 
 This file lists all updates to the [mkdocs-meta-descriptions plugin](https://github.com/prcr/mkdocs-meta-descriptions-plugin).
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [v2.3.0](https://www.github.com/prcr/mkdocs-meta-descriptions-plugin/compare/v2.2.0...v2.3.0) (2023-07-31)
+
+### Added
+
+-   New option [`trim`](https://github.com/prcr/mkdocs-meta-descriptions-plugin#trim) to trim meta descriptions coming from the first paragraph of the pages to include at most `max_length` characters. Fixes [#259](https://github.com/prcr/mkdocs-meta-descriptions-plugin/issues/259). Thanks to [@mur4d1n](https://github.com/mur4d1n) for the contribution! 🎉
+
+### Changed
+
+-   If you're using MkDocs>=1.5.0, the log messages produced by the plugin have the prefix `meta-descriptions:` instead of `[meta-descriptions]` since the plugin [now uses the built-in MkDocs logger](https://www.mkdocs.org/dev-guide/plugins/#logging-in-plugins) to help format log messages consistently across plugins.
+
 ## [v2.2.0](https://www.github.com/prcr/mkdocs-meta-descriptions-plugin/compare/v2.1.0...v2.2.0) (2022-12-15)
 
 ### Added
 
 -   Added support for [Python 3.11](https://www.python.org/downloads/release/python-3111/).
 
 ## [v2.1.0](https://www.github.com/prcr/mkdocs-meta-descriptions-plugin/compare/v2.0.0...v2.1.0) (2022-10-01)
@@ -47,15 +57,15 @@
 
 ## [v1.0.0](https://www.github.com/prcr/mkdocs-meta-descriptions-plugin/compare/v0.0.5...v1.0.0) (2021-05-15)
 
 First stable version.
 
 ### Added
 
--   Support for [exporting meta descriptions](README.md#export_csv) as CSV file.
+-   Support for [exporting meta descriptions](https://github.com/prcr/mkdocs-meta-descriptions-plugin#export_csv) as CSV file.
 
 ## [v0.0.5](https://www.github.com/prcr/mkdocs-meta-descriptions-plugin/compare/v0.0.4...v0.0.5) (2021-05-10)
 
 ### Fixed
 
 -   Slacken minimum requirements for Python packages to make the plugin compatible with a wider range of environments.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/CODE_OF_CONDUCT.md` & `mkdocs-meta-descriptions-plugin-2.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/LICENSE` & `mkdocs-meta-descriptions-plugin-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/PKG-INFO` & `mkdocs-meta-descriptions-plugin-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-meta-descriptions-plugin
-Version: 2.2.0
+Version: 2.3.0
 Summary: Generate meta descriptions from the first paragraphs in your MkDocs pages
 Home-page: https://github.com/prcr/mkdocs-meta-descriptions-plugin
 Author: Paulo Ribeiro
 Author-email: paulo@diffraction.pt
 License: MIT
 Keywords: mkdocs meta description seo paragraph
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,16 +21,16 @@
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mkdocs-meta-descriptions-plugin
 
 [![CI/CD](https://github.com/prcr/mkdocs-meta-descriptions-plugin/actions/workflows/test-build-deploy.yml/badge.svg)](https://github.com/prcr/mkdocs-meta-descriptions-plugin/actions/workflows/test-build-deploy.yml)
-[![Codacy](https://app.codacy.com/project/badge/Grade/08bc759a053f475091318f53ea67bd05)](https://www.codacy.com/gh/prcr/mkdocs-meta-descriptions-plugin/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=prcr/mkdocs-meta-descriptions-plugin&amp;utm_campaign=Badge_Grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/08bc759a053f475091318f53ea67bd05)](https://www.codacy.com/gh/prcr/mkdocs-meta-descriptions-plugin/dashboard?utm_source=github.com&utm_medium=referral&utm_content=prcr/mkdocs-meta-descriptions-plugin&utm_campaign=Badge_Coverage)
+[![Codacy](https://app.codacy.com/project/badge/Grade/08bc759a053f475091318f53ea67bd05)](https://app.codacy.com/gh/prcr/mkdocs-meta-descriptions-plugin/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=prcr/mkdocs-meta-descriptions-plugin&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/08bc759a053f475091318f53ea67bd05)](https://app.codacy.com/gh/prcr/mkdocs-meta-descriptions-plugin/dashboard?utm_source=github.com&utm_medium=referral&utm_content=prcr/mkdocs-meta-descriptions-plugin&utm_campaign=Badge_Coverage)
 [![PyPI](https://img.shields.io/pypi/dm/mkdocs-meta-descriptions-plugin?label=PyPI)](https://pypi.org/project/mkdocs-meta-descriptions-plugin/)
 
 Use this MkDocs plugin to automatically generate meta descriptions for your pages using the first paragraph of each page. This is useful if you start each page with a short introduction or summary that can be reused as the meta description.
 
 ![Meta description obtained from first paragraph of the page](https://raw.githubusercontent.com/prcr/mkdocs-meta-descriptions-plugin/main/images/readme-example.png)
 
 For each page, the plugin:
@@ -79,21 +79,22 @@
 plugins:
   - meta-descriptions:
       export_csv: false
       quiet: false
       enable_checks: false
       min_length: 50
       max_length: 160
+      trim: false
 ```
 
 ### `export_csv`
 
 If `true`, the plugin exports the meta descriptions of all Markdown pages to the CSV file `<site_dir>/meta-descriptions.csv`. The default is `false`.
 
-This is useful to review and keep track of all the meta descriptions in your pages, especially if you're maintaining a big site.
+This is useful to review and keep track of all the meta descriptions for your pages, especially if you're maintaining a big site.
 
 ### `quiet`
 
 If `true`, the plugin logs messages of level `INFO` using the level `DEBUG` instead. The default is `false`.
 
 Enable this option to have a cleaner MkDocs console output. You can still see all logs by running MkDocs with the `--verbose` flag.
 
@@ -109,12 +110,18 @@
 
 Make sure that you set `enable_checks: true` for this option to have an effect.
 
 ### `max_length`
 
 Maximum number of characters that each meta description should have. The default is 160 characters, based on [these general recommendations](https://moz.com/learn/seo/meta-description).
 
-Make sure that you set `enable_checks: true` for this option to have an effect.
+Make sure that you set `enable_checks: true` or `trim: true` for this option to have an effect.
+
+### `trim`
+
+If `true`, the plugin trims meta descriptions coming from the first paragraph of the pages to include at most `max_length` characters.
+
+Note that this option doesn't change any meta descriptions defined explicitly on the [page meta-data](https://www.mkdocs.org/user-guide/writing-your-docs/#meta-data).
 
 ## See also
 
 Read more about [using MkDocs plugins](http://www.mkdocs.org/user-guide/plugins/).
```

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/README.md` & `mkdocs-meta-descriptions-plugin-2.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # mkdocs-meta-descriptions-plugin
 
 [![CI/CD](https://github.com/prcr/mkdocs-meta-descriptions-plugin/actions/workflows/test-build-deploy.yml/badge.svg)](https://github.com/prcr/mkdocs-meta-descriptions-plugin/actions/workflows/test-build-deploy.yml)
-[![Codacy](https://app.codacy.com/project/badge/Grade/08bc759a053f475091318f53ea67bd05)](https://www.codacy.com/gh/prcr/mkdocs-meta-descriptions-plugin/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=prcr/mkdocs-meta-descriptions-plugin&amp;utm_campaign=Badge_Grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/08bc759a053f475091318f53ea67bd05)](https://www.codacy.com/gh/prcr/mkdocs-meta-descriptions-plugin/dashboard?utm_source=github.com&utm_medium=referral&utm_content=prcr/mkdocs-meta-descriptions-plugin&utm_campaign=Badge_Coverage)
+[![Codacy](https://app.codacy.com/project/badge/Grade/08bc759a053f475091318f53ea67bd05)](https://app.codacy.com/gh/prcr/mkdocs-meta-descriptions-plugin/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=prcr/mkdocs-meta-descriptions-plugin&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/08bc759a053f475091318f53ea67bd05)](https://app.codacy.com/gh/prcr/mkdocs-meta-descriptions-plugin/dashboard?utm_source=github.com&utm_medium=referral&utm_content=prcr/mkdocs-meta-descriptions-plugin&utm_campaign=Badge_Coverage)
 [![PyPI](https://img.shields.io/pypi/dm/mkdocs-meta-descriptions-plugin?label=PyPI)](https://pypi.org/project/mkdocs-meta-descriptions-plugin/)
 
 Use this MkDocs plugin to automatically generate meta descriptions for your pages using the first paragraph of each page. This is useful if you start each page with a short introduction or summary that can be reused as the meta description.
 
 ![Meta description obtained from first paragraph of the page](https://raw.githubusercontent.com/prcr/mkdocs-meta-descriptions-plugin/main/images/readme-example.png)
 
 For each page, the plugin:
@@ -55,21 +55,22 @@
 plugins:
   - meta-descriptions:
       export_csv: false
       quiet: false
       enable_checks: false
       min_length: 50
       max_length: 160
+      trim: false
 ```
 
 ### `export_csv`
 
 If `true`, the plugin exports the meta descriptions of all Markdown pages to the CSV file `<site_dir>/meta-descriptions.csv`. The default is `false`.
 
-This is useful to review and keep track of all the meta descriptions in your pages, especially if you're maintaining a big site.
+This is useful to review and keep track of all the meta descriptions for your pages, especially if you're maintaining a big site.
 
 ### `quiet`
 
 If `true`, the plugin logs messages of level `INFO` using the level `DEBUG` instead. The default is `false`.
 
 Enable this option to have a cleaner MkDocs console output. You can still see all logs by running MkDocs with the `--verbose` flag.
 
@@ -85,12 +86,18 @@
 
 Make sure that you set `enable_checks: true` for this option to have an effect.
 
 ### `max_length`
 
 Maximum number of characters that each meta description should have. The default is 160 characters, based on [these general recommendations](https://moz.com/learn/seo/meta-description).
 
-Make sure that you set `enable_checks: true` for this option to have an effect.
+Make sure that you set `enable_checks: true` or `trim: true` for this option to have an effect.
+
+### `trim`
+
+If `true`, the plugin trims meta descriptions coming from the first paragraph of the pages to include at most `max_length` characters.
+
+Note that this option doesn't change any meta descriptions defined explicitly on the [page meta-data](https://www.mkdocs.org/user-guide/writing-your-docs/#meta-data).
 
 ## See also
 
 Read more about [using MkDocs plugins](http://www.mkdocs.org/user-guide/plugins/).
```

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/images/readme-example.png` & `mkdocs-meta-descriptions-plugin-2.3.0/images/readme-example.png`

 * *Files identical despite different names*

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin/checker.py` & `mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin/checker.py`

 * *Files identical despite different names*

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin/common.py` & `mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin/common.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,27 @@
-from logging import getLogger
+import mkdocs
+from packaging import version
+
+MKDOCS_VERSION = version.parse(mkdocs.__version__)
+MKDOCS_1_5_0 = version.parse("1.5.0")
+
+if MKDOCS_VERSION < MKDOCS_1_5_0:
+    from logging import getLogger
+else:
+    from mkdocs.plugins import get_plugin_logger
 
 
 class Logger:
     _initialized = False
-    _tag = "[meta-descriptions] "
-    _logger = getLogger("mkdocs.mkdocs_meta_descriptions_plugin")
+    if MKDOCS_VERSION < MKDOCS_1_5_0:
+        _tag = "[meta-descriptions] "
+        _logger = getLogger("mkdocs.plugins." + __name__)
+    else:
+        _tag = ""
+        _logger = get_plugin_logger("meta-descriptions")
     _quiet = False
 
     Debug, Info, Warning, Error = range(0, 4)
 
     def initialize(self, config):
         self._quiet = config.get("quiet")
         self._initialized = True
```

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin/export.py` & `mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,10 +43,10 @@
             with open(output_file_path, "w") as csv_file:
                 csv_writer = csv.writer(csv_file)
                 csv_writer.writerow(["Page", "Meta description"])
                 for url_path, meta_description in self._meta_descriptions.items():
                     csv_writer.writerow(
                         [urljoin(self._site_url, url_path), meta_description]
                     )
-            logger.write(logger.Info, f"Exported meta descriptions to: {output_file_path}")
+            logger.write(logger.Info, f"Exported meta descriptions to {output_file_path}")
         else:
             logger.write(logger.Warning, "Can't find meta descriptions to write to CSV file")
```

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin/plugin.py` & `mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from textwrap import shorten
 from html import escape
 
 from bs4 import BeautifulSoup
 from mkdocs.config import config_options
 from mkdocs.plugins import BasePlugin
 
 from .common import logger
@@ -14,14 +15,15 @@
 
     config_scheme = (
         ("export_csv", config_options.Type(bool, default=False)),
         ("quiet", config_options.Type(bool, default=False)),
         ("enable_checks", config_options.Type(bool, default=False)),
         ("min_length", config_options.Type(int, default=50)),
         ("max_length", config_options.Type(int, default=160)),
+        ("trim", config_options.Type(bool, default=False)),
     )
 
     def __init__(self):
         self._headings_pattern = re.compile("<h[2-6]", flags=re.IGNORECASE)
         self._pages = []
         self._count_meta = 0             # Pages with meta descriptions defined on the page meta-data
         self._count_first_paragraph = 0  # Pages with meta descriptions from the first paragraph
@@ -49,15 +51,19 @@
             # Skip pages that already have an explicit meta description
             self._count_meta += 1
             logger.write(logger.Debug, f"Adding meta description from front matter: {page.file.src_path}")
         else:
             # Create meta description based on the first paragraph of the page
             first_paragraph_text = self._get_first_paragraph_text(html)
             if len(first_paragraph_text) > 0:
-                page.meta["description"] = first_paragraph_text
+                if self.config.get("trim"):
+                    page.meta["description"] = shorten(first_paragraph_text, self.config.get("max_length"),
+                                                       placeholder="")
+                else:
+                    page.meta["description"] = first_paragraph_text
                 self._count_first_paragraph += 1
                 logger.write(logger.Debug, f"Adding meta description from first paragraph: {page.file.src_path}")
             else:
                 self._count_empty += 1
                 logger.write(logger.Debug, f"Couldn't add meta description: {page.file.src_path}")
         return html
```

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin.egg-info/PKG-INFO` & `mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-meta-descriptions-plugin
-Version: 2.2.0
+Version: 2.3.0
 Summary: Generate meta descriptions from the first paragraphs in your MkDocs pages
 Home-page: https://github.com/prcr/mkdocs-meta-descriptions-plugin
 Author: Paulo Ribeiro
 Author-email: paulo@diffraction.pt
 License: MIT
 Keywords: mkdocs meta description seo paragraph
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,16 +21,16 @@
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mkdocs-meta-descriptions-plugin
 
 [![CI/CD](https://github.com/prcr/mkdocs-meta-descriptions-plugin/actions/workflows/test-build-deploy.yml/badge.svg)](https://github.com/prcr/mkdocs-meta-descriptions-plugin/actions/workflows/test-build-deploy.yml)
-[![Codacy](https://app.codacy.com/project/badge/Grade/08bc759a053f475091318f53ea67bd05)](https://www.codacy.com/gh/prcr/mkdocs-meta-descriptions-plugin/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=prcr/mkdocs-meta-descriptions-plugin&amp;utm_campaign=Badge_Grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/08bc759a053f475091318f53ea67bd05)](https://www.codacy.com/gh/prcr/mkdocs-meta-descriptions-plugin/dashboard?utm_source=github.com&utm_medium=referral&utm_content=prcr/mkdocs-meta-descriptions-plugin&utm_campaign=Badge_Coverage)
+[![Codacy](https://app.codacy.com/project/badge/Grade/08bc759a053f475091318f53ea67bd05)](https://app.codacy.com/gh/prcr/mkdocs-meta-descriptions-plugin/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=prcr/mkdocs-meta-descriptions-plugin&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/08bc759a053f475091318f53ea67bd05)](https://app.codacy.com/gh/prcr/mkdocs-meta-descriptions-plugin/dashboard?utm_source=github.com&utm_medium=referral&utm_content=prcr/mkdocs-meta-descriptions-plugin&utm_campaign=Badge_Coverage)
 [![PyPI](https://img.shields.io/pypi/dm/mkdocs-meta-descriptions-plugin?label=PyPI)](https://pypi.org/project/mkdocs-meta-descriptions-plugin/)
 
 Use this MkDocs plugin to automatically generate meta descriptions for your pages using the first paragraph of each page. This is useful if you start each page with a short introduction or summary that can be reused as the meta description.
 
 ![Meta description obtained from first paragraph of the page](https://raw.githubusercontent.com/prcr/mkdocs-meta-descriptions-plugin/main/images/readme-example.png)
 
 For each page, the plugin:
@@ -79,21 +79,22 @@
 plugins:
   - meta-descriptions:
       export_csv: false
       quiet: false
       enable_checks: false
       min_length: 50
       max_length: 160
+      trim: false
 ```
 
 ### `export_csv`
 
 If `true`, the plugin exports the meta descriptions of all Markdown pages to the CSV file `<site_dir>/meta-descriptions.csv`. The default is `false`.
 
-This is useful to review and keep track of all the meta descriptions in your pages, especially if you're maintaining a big site.
+This is useful to review and keep track of all the meta descriptions for your pages, especially if you're maintaining a big site.
 
 ### `quiet`
 
 If `true`, the plugin logs messages of level `INFO` using the level `DEBUG` instead. The default is `false`.
 
 Enable this option to have a cleaner MkDocs console output. You can still see all logs by running MkDocs with the `--verbose` flag.
 
@@ -109,12 +110,18 @@
 
 Make sure that you set `enable_checks: true` for this option to have an effect.
 
 ### `max_length`
 
 Maximum number of characters that each meta description should have. The default is 160 characters, based on [these general recommendations](https://moz.com/learn/seo/meta-description).
 
-Make sure that you set `enable_checks: true` for this option to have an effect.
+Make sure that you set `enable_checks: true` or `trim: true` for this option to have an effect.
+
+### `trim`
+
+If `true`, the plugin trims meta descriptions coming from the first paragraph of the pages to include at most `max_length` characters.
+
+Note that this option doesn't change any meta descriptions defined explicitly on the [page meta-data](https://www.mkdocs.org/user-guide/writing-your-docs/#meta-data).
 
 ## See also
 
 Read more about [using MkDocs plugins](http://www.mkdocs.org/user-guide/plugins/).
```

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/mkdocs_meta_descriptions_plugin.egg-info/SOURCES.txt` & `mkdocs-meta-descriptions-plugin-2.3.0/mkdocs_meta_descriptions_plugin.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -26,33 +26,40 @@
 mkdocs_meta_descriptions_plugin.egg-info/requires.txt
 mkdocs_meta_descriptions_plugin.egg-info/top_level.txt
 tests/meta-descriptions-no-directory-urls.csv
 tests/meta-descriptions-no-site-description-no-directory-urls.csv
 tests/meta-descriptions-no-site-description.csv
 tests/meta-descriptions-no-site-url-no-directory-urls.csv
 tests/meta-descriptions-no-site-url.csv
+tests/meta-descriptions-trim-no-directory-urls.csv
+tests/meta-descriptions-trim.csv
 tests/meta-descriptions.csv
 tests/mkdocs-enable-checks-no-site-description.yml
 tests/mkdocs-enable-checks.yml
 tests/mkdocs-export-csv-no-site-description.yml
 tests/mkdocs-export-csv-no-site-url.yml
+tests/mkdocs-export-csv-trim.yml
 tests/mkdocs-export-csv.yml
 tests/mkdocs-no-site-description.yml
 tests/mkdocs-quiet.yml
+tests/mkdocs-trim-default.yml
+tests/mkdocs-trim-max-length.yml
 tests/mkdocs.yml
 tests/requirements.txt
 tests/test_plugin.py
 tests/docs/admonition-before-first-paragraph.md
 tests/docs/escape-html-entities.md
 tests/docs/filename with spaces.md
 tests/docs/first-paragraph-no-heading.md
 tests/docs/first-paragraph-no-intro.md
 tests/docs/first-paragraph-no-paragraph.md
 tests/docs/first-paragraph.md
 tests/docs/front-matter-description.md
 tests/docs/image.png
 tests/docs/index.md
+tests/docs/trim-long-description.md
+tests/docs/trim-long-first-paragraph.md
 tests/docs/warning-long.md
 tests/docs/warning-not-found.md
 tests/docs/warning-short.md
 tests/docs/subdirectory/first-paragraph.md
 tests/docs/subdirectory/index.md
```

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/schema.json` & `mkdocs-meta-descriptions-plugin-2.3.0/schema.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998553240740741%*

 * *Differences: {"'oneOf'": "{1: {'properties': {'meta-descriptions': {'properties': {'trim': "*

 * *            "OrderedDict([('title', 'Trim meta descriptions'), ('markdownDescription', "*

 * *            "'https://github.com/prcr/mkdocs-meta-descriptions-plugin#trim'), ('type', 'boolean'), "*

 * *            "('default', 'false')])}}}}}"}*

```diff
@@ -41,14 +41,20 @@
                             "type": "integer"
                         },
                         "quiet": {
                             "default": "false",
                             "markdownDescription": "https://github.com/prcr/mkdocs-meta-descriptions-plugin#quiet",
                             "title": "Quiet output",
                             "type": "boolean"
+                        },
+                        "trim": {
+                            "default": "false",
+                            "markdownDescription": "https://github.com/prcr/mkdocs-meta-descriptions-plugin#trim",
+                            "title": "Trim meta descriptions",
+                            "type": "boolean"
                         }
                     },
                     "type": "object"
                 }
             },
             "type": "object"
         }
```

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/setup.py` & `mkdocs-meta-descriptions-plugin-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `mkdocs-meta-descriptions-plugin-2.2.0/tests/docs/image.png` & `mkdocs-meta-descriptions-plugin-2.3.0/tests/docs/image.png`

 * *Files identical despite different names*

