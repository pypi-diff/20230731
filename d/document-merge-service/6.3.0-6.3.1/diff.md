# Comparing `tmp/document_merge_service-6.3.0.tar.gz` & `tmp/document_merge_service-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_merge_service-6.3.0.tar", max compression
+gzip compressed data, was "document_merge_service-6.3.1.tar", max compression
```

## Comparing `document_merge_service-6.3.0.tar` & `document_merge_service-6.3.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0    11947 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/LICENSE
--rw-r--r--   0        0        0     2243 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/README.md
--rw-r--r--   0        0        0        0 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/__init__.py
--rw-r--r--   0        0        0      405 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/apps.py
--rw-r--r--   0        0        0     3159 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/authentication.py
--rw-r--r--   0        0        0      504 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/__init__.py
--rw-r--r--   0        0        0      559 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/black.png
--rw-r--r--   0        0        0     9125 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/docx-mailmerge-syntax.docx
--rw-r--r--   0        0        0    11489 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/docx-mailmerge.docx
--rw-r--r--   0        0        0     5735 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/docx-template-filters.docx
--rw-r--r--   0        0        0     6087 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/docx-template-loopcontrols.docx
--rw-r--r--   0        0        0     5952 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/docx-template-placeholdercheck.docx
--rw-r--r--   0        0        0     5091 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/docx-template-syntax.docx
--rw-r--r--   0        0        0     5490 2023-07-25 08:52:57.511416 document_merge_service-6.3.0/document_merge_service/api/data/docx-template.docx
--rw-r--r--   0        0        0  1127936 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/loadtest/1.doc
--rw-r--r--   0        0        0   175922 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/loadtest/2.docx
--rw-r--r--   0        0        0   163307 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/loadtest/3.docx
--rw-r--r--   0        0        0   141498 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/loadtest/4.docx
--rw-r--r--   0        0        0       22 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/test.txt
--rw-r--r--   0        0        0        5 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/xlsx-not-valid.xlsx
--rw-r--r--   0        0        0     6467 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/xlsx-structure.xlsx
--rw-r--r--   0        0        0     6432 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/xlsx-syntax.xlsx
--rw-r--r--   0        0        0     4750 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/xlsx-template.xlsx
--rw-r--r--   0        0        0     9772 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/engines.py
--rw-r--r--   0        0        0      389 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/factories.py
--rw-r--r--   0        0        0     2841 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/filters.py
--rw-r--r--   0        0        0     2546 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/jinja.py
--rw-r--r--   0        0        0        0 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/management/commands/__init__.py
--rw-r--r--   0        0        0     1628 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/management/commands/clean_dangling_files.py
--rw-r--r--   0        0        0     1354 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/management/commands/upload_local_templates.py
--rw-r--r--   0        0        0     1248 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      488 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/migrations/0002_template_group.py
--rw-r--r--   0        0        0      374 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/migrations/0003_template_meta.py
--rw-r--r--   0        0        0      145 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/migrations/0004_cleanup_files.py
--rw-r--r--   0        0        0     1004 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py
--rw-r--r--   0        0        0      932 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/migrations/0006_remove_template_group.py
--rw-r--r--   0        0        0        0 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/migrations/__init__.py
--rw-r--r--   0        0        0     1845 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/models.py
--rw-r--r--   0        0        0      231 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/pagination.py
--rw-r--r--   0        0        0      289 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/permissions.py
--rw-r--r--   0        0        0     4651 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/serializers.py
--rw-r--r--   0        0        0        0 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/__init__.py
--rw-r--r--   0        0        0    30689 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/__snapshots__/test_template.ambr
--rw-r--r--   0        0        0     2270 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_authentication.py
--rw-r--r--   0        0        0      942 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_clean_dangling_files.py
--rw-r--r--   0        0        0     1963 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_excel.py
--rw-r--r--   0        0        0     1372 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_filters.py
--rw-r--r--   0        0        0     1300 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_jinja.py
--rw-r--r--   0        0        0      749 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_pagination.py
--rw-r--r--   0        0        0    25634 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_template.py
--rw-r--r--   0        0        0     3425 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_unoconv.py
--rw-r--r--   0        0        0      597 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_upload_local_templates.py
--rw-r--r--   0        0        0     6947 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/unoconv.py
--rw-r--r--   0        0        0      356 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/urls.py
--rw-r--r--   0        0        0     3570 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/views.py
--rw-r--r--   0        0        0     2909 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/conftest.py
--rw-r--r--   0        0        0        0 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/extensions/__init__.py
--rw-r--r--   0        0        0       52 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/extensions/permissions.py
--rw-r--r--   0        0        0       52 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/extensions/visibilities.py
--rw-r--r--   0        0        0      789 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/sentry.py
--rw-r--r--   0        0        0     8938 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/settings.py
--rw-r--r--   0        0        0        0 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/tests/__init__.py
--rw-r--r--   0        0        0      434 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/tests/test_sentry.py
--rw-r--r--   0        0        0      615 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/tests/test_settings.py
--rw-r--r--   0        0        0      225 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/urls.py
--rw-r--r--   0        0        0      412 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/wsgi.py
--rw-r--r--   0        0        0     3555 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/pyproject.toml
--rw-r--r--   0        0        0     4191 1970-01-01 00:00:00.000000 document_merge_service-6.3.0/PKG-INFO
+-rw-r--r--   0        0        0    12161 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/LICENSE
+-rw-r--r--   0        0        0     2243 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/__init__.py
+-rw-r--r--   0        0        0      405 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/apps.py
+-rw-r--r--   0        0        0     3232 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/authentication.py
+-rw-r--r--   0        0        0      504 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/__init__.py
+-rw-r--r--   0        0        0      559 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/black.png
+-rw-r--r--   0        0        0     9125 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/docx-mailmerge-syntax.docx
+-rw-r--r--   0        0        0    11489 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/docx-mailmerge.docx
+-rw-r--r--   0        0        0     5735 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/docx-template-filters.docx
+-rw-r--r--   0        0        0     6087 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/docx-template-loopcontrols.docx
+-rw-r--r--   0        0        0     5952 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/docx-template-placeholdercheck.docx
+-rw-r--r--   0        0        0     5091 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/docx-template-syntax.docx
+-rw-r--r--   0        0        0     5490 2023-07-31 12:45:30.722650 document_merge_service-6.3.1/document_merge_service/api/data/docx-template.docx
+-rw-r--r--   0        0        0  1127936 2023-07-31 12:45:30.726650 document_merge_service-6.3.1/document_merge_service/api/data/loadtest/1.doc
+-rw-r--r--   0        0        0   175922 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/loadtest/2.docx
+-rw-r--r--   0        0        0   163307 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/loadtest/3.docx
+-rw-r--r--   0        0        0   141498 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/loadtest/4.docx
+-rw-r--r--   0        0        0       22 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/test.txt
+-rw-r--r--   0        0        0        5 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/xlsx-not-valid.xlsx
+-rw-r--r--   0        0        0     6467 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/xlsx-structure.xlsx
+-rw-r--r--   0        0        0     6432 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/xlsx-syntax.xlsx
+-rw-r--r--   0        0        0     4750 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/data/xlsx-template.xlsx
+-rw-r--r--   0        0        0     9772 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/engines.py
+-rw-r--r--   0        0        0      389 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/factories.py
+-rw-r--r--   0        0        0     2841 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/filters.py
+-rw-r--r--   0        0        0     2546 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/jinja.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/management/commands/__init__.py
+-rw-r--r--   0        0        0     1628 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/management/commands/clean_dangling_files.py
+-rw-r--r--   0        0        0     1354 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/management/commands/upload_local_templates.py
+-rw-r--r--   0        0        0     1248 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      488 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/migrations/0002_template_group.py
+-rw-r--r--   0        0        0      374 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/migrations/0003_template_meta.py
+-rw-r--r--   0        0        0      145 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/migrations/0004_cleanup_files.py
+-rw-r--r--   0        0        0     1004 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/migrations/0005_xlsx_template_engine.py
+-rw-r--r--   0        0        0      932 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/migrations/0006_remove_template_group.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/migrations/__init__.py
+-rw-r--r--   0        0        0     1845 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/models.py
+-rw-r--r--   0        0        0      231 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/pagination.py
+-rw-r--r--   0        0        0      289 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/permissions.py
+-rw-r--r--   0        0        0     4651 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/serializers.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/__init__.py
+-rw-r--r--   0        0        0    30689 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/__snapshots__/test_template.ambr
+-rw-r--r--   0        0        0     2357 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_authentication.py
+-rw-r--r--   0        0        0      942 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_clean_dangling_files.py
+-rw-r--r--   0        0        0     1963 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_excel.py
+-rw-r--r--   0        0        0     1372 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_filters.py
+-rw-r--r--   0        0        0     1300 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_jinja.py
+-rw-r--r--   0        0        0      749 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_pagination.py
+-rw-r--r--   0        0        0    25634 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_template.py
+-rw-r--r--   0        0        0     3425 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_unoconv.py
+-rw-r--r--   0        0        0      597 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/tests/test_upload_local_templates.py
+-rw-r--r--   0        0        0     6947 2023-07-31 12:45:30.730650 document_merge_service-6.3.1/document_merge_service/api/unoconv.py
+-rw-r--r--   0        0        0      356 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/api/urls.py
+-rw-r--r--   0        0        0     3570 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/api/views.py
+-rw-r--r--   0        0        0     2909 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/extensions/__init__.py
+-rw-r--r--   0        0        0       52 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/extensions/permissions.py
+-rw-r--r--   0        0        0       52 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/extensions/visibilities.py
+-rw-r--r--   0        0        0      789 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/sentry.py
+-rw-r--r--   0        0        0     8938 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/settings.py
+-rw-r--r--   0        0        0        0 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/tests/__init__.py
+-rw-r--r--   0        0        0      434 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/tests/test_sentry.py
+-rw-r--r--   0        0        0      615 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/tests/test_settings.py
+-rw-r--r--   0        0        0      225 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/urls.py
+-rw-r--r--   0        0        0      412 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/document_merge_service/wsgi.py
+-rw-r--r--   0        0        0     3555 2023-07-31 12:45:30.734650 document_merge_service-6.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4191 1970-01-01 00:00:00.000000 document_merge_service-6.3.1/PKG-INFO
```

### Comparing `document_merge_service-6.3.0/CHANGELOG.md` & `document_merge_service-6.3.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 6.3.1 (31 July 2023)
+### Fix
+
+* **auth:** Don't run any authentication logic if auth is disabled ([`564b504`](https://github.com/adfinis/document-merge-service/commit/564b504be673f34677eb6736a3b26dbbfdd3d7ec))
+
 ## 6.3.0 (25 July 2023)
 ### Feature
 
 * **extensions:** Add setting for passing custom arguments into extensions ([`b76e293`](https://github.com/adfinis/document-merge-service/commit/b76e2930535f15820e449930e57d004c54e1ba2d))
 
 ## 6.2.2 (24 July 2023)
 ### Fix
```

### Comparing `document_merge_service-6.3.0/LICENSE` & `document_merge_service-6.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/README.md` & `document_merge_service-6.3.1/README.md`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/authentication.py` & `document_merge_service-6.3.1/document_merge_service/api/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,17 @@
                 f"Retrieving userinfo from {settings.OIDC_USERINFO_ENDPOINT} "
                 f"failed with error '{str(e)}'."
             )
 
         return response.json()
 
     def authenticate(self, request):
+        if not settings.REQUIRE_AUTHENTICATION:
+            return None
+
         token = self.get_bearer_token(request)
         if token is None:
             return None
 
         userinfo_method = functools.partial(self.get_userinfo, token=token)
         # token might be too long for key so we use hash sum instead.
         hashsum_token = hashlib.sha256(force_bytes(token)).hexdigest()
```

### Comparing `document_merge_service-6.3.0/document_merge_service/api/data/black.png` & `document_merge_service-6.3.1/document_merge_service/api/data/black.png`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/data/docx-mailmerge-syntax.docx` & `document_merge_service-6.3.1/document_merge_service/api/data/docx-mailmerge-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/data/docx-mailmerge.docx` & `document_merge_service-6.3.1/document_merge_service/api/data/docx-mailmerge.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/data/docx-template-filters.docx` & `document_merge_service-6.3.1/document_merge_service/api/data/docx-template-filters.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/data/docx-template-loopcontrols.docx` & `document_merge_service-6.3.1/document_merge_service/api/data/docx-template-loopcontrols.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/data/docx-template-placeholdercheck.docx` & `document_merge_service-6.3.1/document_merge_service/api/data/docx-template-placeholdercheck.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/data/docx-template-syntax.docx` & `document_merge_service-6.3.1/document_merge_service/api/data/docx-template-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/data/docx-template.docx` & `document_merge_service-6.3.1/document_merge_service/api/data/docx-template.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/data/loadtest/1.doc` & `document_merge_service-6.3.1/document_merge_service/api/data/loadtest/1.doc`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/data/loadtest/2.docx` & `document_merge_service-6.3.1/document_merge_service/api/data/loadtest/2.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/data/loadtest/3.docx` & `document_merge_service-6.3.1/document_merge_service/api/data/loadtest/3.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/data/loadtest/4.docx` & `document_merge_service-6.3.1/document_merge_service/api/data/loadtest/4.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/data/xlsx-structure.xlsx` & `document_merge_service-6.3.1/document_merge_service/api/data/xlsx-structure.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/data/xlsx-syntax.xlsx` & `document_merge_service-6.3.1/document_merge_service/api/data/xlsx-syntax.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/data/xlsx-template.xlsx` & `document_merge_service-6.3.1/document_merge_service/api/data/xlsx-template.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/engines.py` & `document_merge_service-6.3.1/document_merge_service/api/engines.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/filters.py` & `document_merge_service-6.3.1/document_merge_service/api/filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/jinja.py` & `document_merge_service-6.3.1/document_merge_service/api/jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/management/commands/clean_dangling_files.py` & `document_merge_service-6.3.1/document_merge_service/api/management/commands/clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/management/commands/upload_local_templates.py` & `document_merge_service-6.3.1/document_merge_service/api/management/commands/upload_local_templates.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/migrations/0001_initial.py` & `document_merge_service-6.3.1/document_merge_service/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py` & `document_merge_service-6.3.1/document_merge_service/api/migrations/0005_xlsx_template_engine.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/migrations/0006_remove_template_group.py` & `document_merge_service-6.3.1/document_merge_service/api/migrations/0006_remove_template_group.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/models.py` & `document_merge_service-6.3.1/document_merge_service/api/models.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/serializers.py` & `document_merge_service-6.3.1/document_merge_service/api/serializers.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/tests/__snapshots__/test_template.ambr` & `document_merge_service-6.3.1/document_merge_service/api/tests/__snapshots__/test_template.ambr`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/tests/test_authentication.py` & `document_merge_service-6.3.1/document_merge_service/api/tests/test_authentication.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,16 @@
         ("Bearer Token", status.HTTP_200_OK, False),
         ("Bearer Token", status.HTTP_502_BAD_GATEWAY, True),
     ],
 )
 def test_bearer_token_authentication_authenticate(
     rf, authentication_header, error, requests_mock, settings, status_code
 ):
+    settings.REQUIRE_AUTHENTICATION = True
+
     userinfo = {"sub": "1"}
     requests_mock.get(
         settings.OIDC_USERINFO_ENDPOINT,
         status_code=status_code,
         request_headers={"Authorization": authentication_header},
         text=json.dumps(userinfo),
     )
@@ -47,14 +49,15 @@
                 == userinfo
             )
 
 
 def test_bearer_token_authentication_authenticate_groups_claim(
     settings, requests_mock, rf
 ):
+    settings.REQUIRE_AUTHENTICATION = True
     settings.OIDC_GROUPS_CLAIM = "document-merge-service"
 
     userinfo = {"sub": "1", settings.OIDC_GROUPS_CLAIM: ["test"]}
     requests_mock.get(settings.OIDC_USERINFO_ENDPOINT, text=json.dumps(userinfo))
 
     request = rf.get("/openid", HTTP_AUTHORIZATION="Bearer Token")
     user, auth = authentication.BearerTokenAuthentication().authenticate(request)
```

### Comparing `document_merge_service-6.3.0/document_merge_service/api/tests/test_clean_dangling_files.py` & `document_merge_service-6.3.1/document_merge_service/api/tests/test_clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/tests/test_excel.py` & `document_merge_service-6.3.1/document_merge_service/api/tests/test_excel.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/tests/test_filters.py` & `document_merge_service-6.3.1/document_merge_service/api/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/tests/test_jinja.py` & `document_merge_service-6.3.1/document_merge_service/api/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/tests/test_pagination.py` & `document_merge_service-6.3.1/document_merge_service/api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/tests/test_template.py` & `document_merge_service-6.3.1/document_merge_service/api/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/tests/test_unoconv.py` & `document_merge_service-6.3.1/document_merge_service/api/tests/test_unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/tests/test_upload_local_templates.py` & `document_merge_service-6.3.1/document_merge_service/api/tests/test_upload_local_templates.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/unoconv.py` & `document_merge_service-6.3.1/document_merge_service/api/unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/api/views.py` & `document_merge_service-6.3.1/document_merge_service/api/views.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/conftest.py` & `document_merge_service-6.3.1/document_merge_service/conftest.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/sentry.py` & `document_merge_service-6.3.1/document_merge_service/sentry.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/settings.py` & `document_merge_service-6.3.1/document_merge_service/settings.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/document_merge_service/tests/test_settings.py` & `document_merge_service-6.3.1/document_merge_service/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.3.0/pyproject.toml` & `document_merge_service-6.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "document-merge-service"
-version = "6.3.0"
+version = "6.3.1"
 description = "Merge Document Template Service"
 license = "GPL-3.0-or-later"
 authors = ["Adfinis AG <info@adfinis.com>"]
 homepage = "https://github.com/adfinis/document-merge-service"
 repository = "https://github.com/adfinis/document-merge-service"
 documentation = "https://github.com/adfinis/document-merge-service/blob/main/README.md"
 readme = "README.md"
```

### Comparing `document_merge_service-6.3.0/PKG-INFO` & `document_merge_service-6.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: document-merge-service
-Version: 6.3.0
+Version: 6.3.1
 Summary: Merge Document Template Service
 Home-page: https://github.com/adfinis/document-merge-service
 License: GPL-3.0-or-later
 Author: Adfinis AG
 Author-email: info@adfinis.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

