# Comparing `tmp/maxware_tsp_cli-0.1.0.tar.gz` & `tmp/maxware_tsp_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxware_tsp_cli-0.1.0.tar", max compression
+gzip compressed data, was "maxware_tsp_cli-0.2.0.tar", max compression
```

## Comparing `maxware_tsp_cli-0.1.0.tar` & `maxware_tsp_cli-0.2.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     7633 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-07-30 03:49:14.289866 maxware_tsp_cli-0.1.0/README.md
--rw-r--r--   0        0        0     4084 2023-07-31 00:45:23.157276 maxware_tsp_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       61 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/__init__.py
--rw-r--r--   0        0        0       88 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/__main__.py
--rw-r--r--   0        0        0     1981 2023-07-30 06:29:50.459866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/cli.py
--rw-r--r--   0        0        0     5602 2023-07-30 06:31:16.199866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/cli_common.py
--rw-r--r--   0        0        0      293 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/__init__.py
--rw-r--r--   0        0        0      613 2023-07-30 06:47:49.139866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5137 2023-07-30 06:47:49.139866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/__pycache__/bootstrap.cpython-38.pyc
--rw-r--r--   0        0        0     1353 2023-07-30 06:47:49.429866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/__pycache__/config.cpython-38.pyc
--rw-r--r--   0        0        0     7024 2023-07-30 06:47:49.499866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/__pycache__/launch.cpython-38.pyc
--rw-r--r--   0        0        0     1751 2023-07-30 06:47:51.159866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/__pycache__/shell.cpython-38.pyc
--rw-r--r--   0        0        0     7358 2023-07-30 06:47:51.159866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/__pycache__/source_get.cpython-38.pyc
--rw-r--r--   0        0        0     4131 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/__pycache__/test.cpython-38.pyc
--rw-r--r--   0        0        0     5929 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/bootstrap.py
--rw-r--r--   0        0        0     1173 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/config.py
--rw-r--r--   0        0        0       28 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/db/__init__.py
--rw-r--r--   0        0        0      263 2023-07-30 06:47:49.429866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/db/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      600 2023-07-30 06:47:49.429866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/db/__pycache__/cli.cpython-38.pyc
--rw-r--r--   0        0        0     2070 2023-07-30 06:47:49.429866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/db/__pycache__/connection.cpython-38.pyc
--rw-r--r--   0        0        0     1563 2023-07-30 06:47:49.449866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/db/__pycache__/passwords.cpython-38.pyc
--rw-r--r--   0        0        0      311 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/db/cli.py
--rw-r--r--   0        0        0     1801 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/db/connection.py
--rw-r--r--   0        0        0     1325 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/db/passwords.py
--rw-r--r--   0        0        0    10763 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/launch.py
--rw-r--r--   0        0        0      177 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/__init__.py
--rw-r--r--   0        0        0      423 2023-07-30 06:47:49.499866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1002 2023-07-30 06:47:49.499866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/__pycache__/cli.cpython-38.pyc
--rw-r--r--   0        0        0     2382 2023-07-30 06:47:49.499866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/__pycache__/importer.cpython-38.pyc
--rw-r--r--   0        0        0     3659 2023-07-30 06:47:51.149866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/__pycache__/modules.cpython-38.pyc
--rw-r--r--   0        0        0     4043 2023-07-30 06:47:51.159866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/__pycache__/translations.cpython-38.pyc
--rw-r--r--   0        0        0      710 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/cli.py
--rw-r--r--   0        0        0     2301 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/importer.py
--rw-r--r--   0        0        0     3623 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/modules.py
--rw-r--r--   0        0        0     4000 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/translations.py
--rw-r--r--   0        0        0     1619 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/shell.py
--rw-r--r--   0        0        0     8544 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/source_get.py
--rw-r--r--   0        0        0     4562 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/test.py
--rw-r--r--   0        0        0      161 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/__init__.py
--rw-r--r--   0        0        0      418 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1289 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/__pycache__/git_odoo.cpython-38.pyc
--rw-r--r--   0        0        0     3368 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/__pycache__/git_odoo_addons.cpython-38.pyc
--rw-r--r--   0        0        0     5459 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/__pycache__/git_repo.cpython-38.pyc
--rw-r--r--   0        0        0     4591 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/__pycache__/git_url.cpython-38.pyc
--rw-r--r--   0        0        0     1709 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/__pycache__/zip_download.cpython-38.pyc
--rw-r--r--   0        0        0     1299 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/git_odoo.py
--rw-r--r--   0        0        0     3296 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/git_odoo_addons.py
--rw-r--r--   0        0        0     6460 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/git_repo.py
--rw-r--r--   0        0        0     4585 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/git_url.py
--rw-r--r--   0        0        0     1575 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/zip_download.py
--rw-r--r--   0        0        0       49 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/__init__.py
--rw-r--r--   0        0        0      275 2023-07-30 06:47:49.139866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2570 2023-07-30 06:47:49.139866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/__pycache__/bootstrap.cpython-38.pyc
--rw-r--r--   0        0        0      677 2023-07-30 06:47:49.429866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/__pycache__/cli.cpython-38.pyc
--rw-r--r--   0        0        0     8278 2023-07-30 06:47:49.139866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/__pycache__/odoo_files.cpython-38.pyc
--rw-r--r--   0        0        0     3473 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/__pycache__/odoo_manifest.cpython-38.pyc
--rw-r--r--   0        0        0     2860 2023-07-30 06:47:49.269866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/__pycache__/system.cpython-38.pyc
--rw-r--r--   0        0        0     2225 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/bootstrap.py
--rw-r--r--   0        0        0      386 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/cli.py
--rw-r--r--   0        0        0     8895 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/odoo_files.py
--rw-r--r--   0        0        0     3277 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/odoo_manifest.py
--rw-r--r--   0        0        0     2778 2023-07-30 06:33:46.569866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/system.py
--rw-r--r--   0        0        0       22 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/version.py
--rw-r--r--   0        0        0      847 1970-01-01 00:00:00.000000 maxware_tsp_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7633 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-30 03:49:14.289866 maxware_tsp_cli-0.2.0/README.md
+-rw-r--r--   0        0        0     4093 2023-07-31 06:28:02.951526 maxware_tsp_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/__init__.py
+-rw-r--r--   0        0        0       88 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/__main__.py
+-rw-r--r--   0        0        0     1981 2023-07-30 06:29:50.459866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/cli.py
+-rw-r--r--   0        0        0     5602 2023-07-30 06:31:16.199866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/cli_common.py
+-rw-r--r--   0        0        0      293 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/__init__.py
+-rw-r--r--   0        0        0      613 2023-07-30 06:47:49.139866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5137 2023-07-30 06:47:49.139866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/__pycache__/bootstrap.cpython-38.pyc
+-rw-r--r--   0        0        0     1353 2023-07-30 06:47:49.429866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0        0        0     7024 2023-07-30 06:47:49.499866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/__pycache__/launch.cpython-38.pyc
+-rw-r--r--   0        0        0     1751 2023-07-30 06:47:51.159866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/__pycache__/shell.cpython-38.pyc
+-rw-r--r--   0        0        0     7358 2023-07-30 06:47:51.159866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/__pycache__/source_get.cpython-38.pyc
+-rw-r--r--   0        0        0     4131 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/__pycache__/test.cpython-38.pyc
+-rw-r--r--   0        0        0     5929 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/bootstrap.py
+-rw-r--r--   0        0        0     1173 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/config.py
+-rw-r--r--   0        0        0       28 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/db/__init__.py
+-rw-r--r--   0        0        0      263 2023-07-30 06:47:49.429866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/db/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      600 2023-07-30 06:47:49.429866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/db/__pycache__/cli.cpython-38.pyc
+-rw-r--r--   0        0        0     2070 2023-07-30 06:47:49.429866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/db/__pycache__/connection.cpython-38.pyc
+-rw-r--r--   0        0        0     1563 2023-07-30 06:47:49.449866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/db/__pycache__/passwords.cpython-38.pyc
+-rw-r--r--   0        0        0      311 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/db/cli.py
+-rw-r--r--   0        0        0     1801 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/db/connection.py
+-rw-r--r--   0        0        0     1325 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/db/passwords.py
+-rw-r--r--   0        0        0    10763 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/launch.py
+-rw-r--r--   0        0        0      177 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/__init__.py
+-rw-r--r--   0        0        0      423 2023-07-30 06:47:49.499866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1002 2023-07-30 06:47:49.499866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/__pycache__/cli.cpython-38.pyc
+-rw-r--r--   0        0        0     2382 2023-07-30 06:47:49.499866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/__pycache__/importer.cpython-38.pyc
+-rw-r--r--   0        0        0     3659 2023-07-30 06:47:51.149866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/__pycache__/modules.cpython-38.pyc
+-rw-r--r--   0        0        0     4043 2023-07-30 06:47:51.159866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/__pycache__/translations.cpython-38.pyc
+-rw-r--r--   0        0        0      710 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/cli.py
+-rw-r--r--   0        0        0     2301 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/importer.py
+-rw-r--r--   0        0        0     3623 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/modules.py
+-rw-r--r--   0        0        0     4000 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/translations.py
+-rw-r--r--   0        0        0     1619 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/shell.py
+-rw-r--r--   0        0        0     8544 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/source_get.py
+-rw-r--r--   0        0        0     4562 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/test.py
+-rw-r--r--   0        0        0      161 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1289 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/__pycache__/git_odoo.cpython-38.pyc
+-rw-r--r--   0        0        0     3368 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/__pycache__/git_odoo_addons.cpython-38.pyc
+-rw-r--r--   0        0        0     5459 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/__pycache__/git_repo.cpython-38.pyc
+-rw-r--r--   0        0        0     4591 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/__pycache__/git_url.cpython-38.pyc
+-rw-r--r--   0        0        0     1709 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/__pycache__/zip_download.cpython-38.pyc
+-rw-r--r--   0        0        0     1299 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/git_odoo.py
+-rw-r--r--   0        0        0     3296 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/git_odoo_addons.py
+-rw-r--r--   0        0        0     6460 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/git_repo.py
+-rw-r--r--   0        0        0     4585 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/git_url.py
+-rw-r--r--   0        0        0     1575 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/zip_download.py
+-rw-r--r--   0        0        0       49 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-30 06:47:49.139866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2570 2023-07-30 06:47:49.139866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/__pycache__/bootstrap.cpython-38.pyc
+-rw-r--r--   0        0        0      677 2023-07-30 06:47:49.429866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/__pycache__/cli.cpython-38.pyc
+-rw-r--r--   0        0        0     8278 2023-07-30 06:47:49.139866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/__pycache__/odoo_files.cpython-38.pyc
+-rw-r--r--   0        0        0     3473 2023-07-30 06:47:51.289866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/__pycache__/odoo_manifest.cpython-38.pyc
+-rw-r--r--   0        0        0     2860 2023-07-30 06:47:49.269866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/__pycache__/system.cpython-38.pyc
+-rw-r--r--   0        0        0     2225 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/bootstrap.py
+-rw-r--r--   0        0        0      386 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/cli.py
+-rw-r--r--   0        0        0     8895 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/odoo_files.py
+-rw-r--r--   0        0        0     3277 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/odoo_manifest.py
+-rw-r--r--   0        0        0     2778 2023-07-30 06:33:46.569866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/system.py
+-rw-r--r--   0        0        0       22 2023-07-30 05:08:46.259866 maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/version.py
+-rw-r--r--   0        0        0      847 1970-01-01 00:00:00.000000 maxware_tsp_cli-0.2.0/PKG-INFO
```

### Comparing `maxware_tsp_cli-0.1.0/LICENSE` & `maxware_tsp_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/pyproject.toml` & `maxware_tsp_cli-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maxware-tsp-cli"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Abderrahim Guennoune <aguennoune@outlook.com>"]
 readme = "README.md"
 packages = [{include = "maxware_tsp_cli", from = "src"}]
 keywords = ["odoo", "cli", "maxware", "tsp", "godoo"]
 
 [tool.poetry_bumpversion.file."src/maxware_tsp_cli/version.py"]
@@ -18,15 +18,15 @@
 ruamel-yaml = "^0.17.21"
 gitpython = "^3.1.27"
 godoo-rpc = "^0.1.1"
 openupgradelib = "^3.3.4"
 psycopg2 = "^2.9.6"
 passlib = "^1.7.3"
 typer-common-functions = "^0.0.3"
-odoo = "^16.0.0"
+odoo = ">=16.0.0,<17.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pylint-odoo = "^8.0.16"
 ipdb = "^0.13.9"
 debugpy = "^1.6.0"
 black = "^22.10.0"
```

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/cli.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/cli.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/cli_common.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/cli_common.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/__pycache__/__init__.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/__pycache__/bootstrap.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/__pycache__/bootstrap.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/__pycache__/config.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/__pycache__/config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/__pycache__/launch.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/__pycache__/launch.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/__pycache__/shell.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/__pycache__/shell.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/__pycache__/source_get.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/__pycache__/source_get.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/__pycache__/test.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/__pycache__/test.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/bootstrap.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/bootstrap.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/config.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/db/__pycache__/cli.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/db/__pycache__/cli.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/db/__pycache__/connection.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/db/__pycache__/connection.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/db/__pycache__/passwords.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/db/__pycache__/passwords.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/db/connection.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/db/connection.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/db/passwords.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/db/passwords.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/launch.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/launch.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/__pycache__/cli.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/__pycache__/cli.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/__pycache__/importer.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/__pycache__/importer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/__pycache__/modules.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/__pycache__/modules.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/__pycache__/translations.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/__pycache__/translations.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/cli.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/cli.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/importer.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/importer.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/modules.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/modules.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/rpc/translations.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/rpc/translations.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/shell.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/shell.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/source_get.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/source_get.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/commands/test.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/__pycache__/git_odoo.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/__pycache__/git_odoo.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/__pycache__/git_odoo_addons.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/__pycache__/git_odoo_addons.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/__pycache__/git_repo.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/__pycache__/git_repo.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/__pycache__/git_url.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/__pycache__/git_url.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/__pycache__/zip_download.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/__pycache__/zip_download.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/git_odoo.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/git_odoo.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/git_odoo_addons.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/git_odoo_addons.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/git_repo.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/git_repo.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/git_url.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/git_url.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/git/zip_download.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/git/zip_download.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/__pycache__/bootstrap.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/__pycache__/bootstrap.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/__pycache__/cli.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/__pycache__/cli.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/__pycache__/odoo_files.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/__pycache__/odoo_files.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/__pycache__/odoo_manifest.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/__pycache__/odoo_manifest.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/__pycache__/system.cpython-38.pyc` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/__pycache__/system.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/bootstrap.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/odoo_files.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/odoo_files.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/odoo_manifest.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/odoo_manifest.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/src/maxware_tsp_cli/helpers/system.py` & `maxware_tsp_cli-0.2.0/src/maxware_tsp_cli/helpers/system.py`

 * *Files identical despite different names*

### Comparing `maxware_tsp_cli-0.1.0/PKG-INFO` & `maxware_tsp_cli-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxware-tsp-cli
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Keywords: odoo,cli,maxware,tsp,godoo
 Author: Abderrahim Guennoune
 Author-email: aguennoune@outlook.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

