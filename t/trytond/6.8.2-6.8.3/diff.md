# Comparing `tmp/trytond-6.8.2.tar.gz` & `tmp/trytond-6.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond-6.8.2.tar", last modified: Wed Jun 21 17:09:49 2023, max compression
+gzip compressed data, was "trytond-6.8.3.tar", last modified: Mon Jul 31 15:06:30 2023, max compression
```

## Comparing `trytond-6.8.2.tar` & `trytond-6.8.3.tar`

### file list

```diff
@@ -1,597 +1,597 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:49.020156 trytond-6.8.2/
--rw-r--r--   0 ced       (1000) ced       (1000)    38781 2023-06-21 17:09:45.000000 trytond-6.8.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-06-21 17:09:44.000000 trytond-6.8.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:32.000000 trytond-6.8.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      204 2023-05-01 12:17:32.000000 trytond-6.8.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2681 2023-06-21 17:09:49.020156 trytond-6.8.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-05-01 12:17:32.000000 trytond-6.8.2/README.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.473482 trytond-6.8.2/bin/
--rwxr-xr-x   0 ced       (1000) ced       (1000)     2888 2023-05-01 12:17:32.000000 trytond-6.8.2/bin/trytond
--rwxr-xr-x   0 ced       (1000) ced       (1000)      807 2023-05-01 12:17:32.000000 trytond-6.8.2/bin/trytond-admin
--rwxr-xr-x   0 ced       (1000) ced       (1000)      783 2023-05-01 12:17:32.000000 trytond-6.8.2/bin/trytond-console
--rwxr-xr-x   0 ced       (1000) ced       (1000)      889 2023-05-01 12:17:32.000000 trytond-6.8.2/bin/trytond-cron
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4892 2023-05-01 12:17:32.000000 trytond-6.8.2/bin/trytond-stat
--rwxr-xr-x   0 ced       (1000) ced       (1000)      898 2023-05-01 12:17:32.000000 trytond-6.8.2/bin/trytond-worker
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.473482 trytond-6.8.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     1677 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1280 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.480149 trytond-6.8.2/doc/ref/
--rw-r--r--   0 ced       (1000) ced       (1000)    10247 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/backend.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3269 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/bus.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2656 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/cache.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2632 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/exceptions.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    31979 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/fields.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1171 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/filestore.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      664 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/i18n.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    31703 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/models.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/pool.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8787 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/pyson.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1461 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/rpc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2109 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/sendmail.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3139 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/tests.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.483482 trytond-6.8.2/doc/ref/tools/
--rw-r--r--   0 ced       (1000) ced       (1000)      565 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/tools/barcode.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      183 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/tools/email.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/tools/immutabledict.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      173 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/tools/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1313 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/tools/misc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/tools/qrcode.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/tools/singleton.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      608 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/tools/timezone.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5510 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/transaction.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6056 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/ref/wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/releases.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.493482 trytond-6.8.2/doc/topics/
--rw-r--r--   0 ced       (1000) ced       (1000)     3717 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/access_rights.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      992 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/actions.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4014 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/backend_types.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/bus.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    14772 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1431 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/cron.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7848 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/domain.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      536 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      983 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/install.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1108 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/logs.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.493482 trytond-6.8.2/doc/topics/models/
--rw-r--r--   0 ced       (1000) ced       (1000)      840 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/models/fields_default_value.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1197 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/models/fields_on_change.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1376 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/models/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.493482 trytond-6.8.2/doc/topics/modules/
--rw-r--r--   0 ced       (1000) ced       (1000)     6022 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/modules/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3887 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/pyson.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.496816 trytond-6.8.2/doc/topics/reports/
--rw-r--r--   0 ced       (1000) ced       (1000)     8742 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/reports/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1381 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/rpc.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/setup_database.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2912 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/start_server.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2229 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/task_queue.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2880 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/testing.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2191 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/translation.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      922 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/triggers.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2596 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/user_application.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2034 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/user_errors_warnings.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.496816 trytond-6.8.2/doc/topics/views/
--rw-r--r--   0 ced       (1000) ced       (1000)     1130 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/views/extension.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    25050 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/views/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1669 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/topics/wizard.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.496816 trytond-6.8.2/doc/tutorial/
--rw-r--r--   0 ced       (1000) ced       (1000)       98 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/index.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.506816 trytond-6.8.2/doc/tutorial/module/
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/anatomy.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1843 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/default_values.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3334 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/domains.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2917 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/extend.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3524 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/function_fields.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      768 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3935 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/model.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2662 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/on_change.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3727 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/report.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1712 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/setup.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/setup_database.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3097 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/states.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4746 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/table_query.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     6258 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/view.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5047 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/wizard.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4773 2023-05-01 12:17:32.000000 trytond-6.8.2/doc/tutorial/module/workflow.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-06-21 17:09:49.020156 trytond-6.8.2/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     5418 2023-05-01 12:17:32.000000 trytond-6.8.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      597 2023-05-01 12:17:32.000000 trytond-6.8.2/tox.ini
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.530149 trytond-6.8.2/trytond/
--rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-05-17 20:29:33.000000 trytond-6.8.2/trytond/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6930 2023-06-10 09:41:09.000000 trytond-6.8.2/trytond/admin.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1370 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/application.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.533483 trytond-6.8.2/trytond/backend/
--rw-r--r--   0 ced       (1000) ced       (1000)     1093 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/backend/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4390 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/backend/database.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.540150 trytond-6.8.2/trytond/backend/postgresql/
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/backend/postgresql/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26462 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/backend/postgresql/database.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3631 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/backend/postgresql/init.sql
--rw-r--r--   0 ced       (1000) ced       (1000)    26820 2023-06-10 09:39:42.000000 trytond-6.8.2/trytond/backend/postgresql/table.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.543483 trytond-6.8.2/trytond/backend/sqlite/
--rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/backend/sqlite/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20773 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/backend/sqlite/database.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2209 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/backend/sqlite/init.sql
--rw-r--r--   0 ced       (1000) ced       (1000)    16323 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/backend/sqlite/table.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4129 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/backend/table.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9431 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/bus.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16982 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7095 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/commandline.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6437 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/config.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2280 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/console.py
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/const.py
--rw-r--r--   0 ced       (1000) ced       (1000)    31266 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/convert.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1490 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/cron.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2055 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2122 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/filestore.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1022 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/i18n.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.593484 trytond-6.8.2/trytond/ir/
--rw-r--r--   0 ced       (1000) ced       (1000)     3329 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    41248 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/action.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9920 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/action.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4059 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/attachment.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1960 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/attachment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6355 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/avatar.py
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2089 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/calendar_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4282 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/calendar_.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1459 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7820 2023-05-04 17:44:31.000000 trytond-6.8.2/trytond/ir/cron.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1954 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/cron.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      596 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/date.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4525 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/email.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    20472 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/email_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5684 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/error.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3592 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/error.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      947 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1858 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/export.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2070 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/export.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.596817 trytond-6.8.2/trytond/ir/fonts/
--rw-r--r--   0 ced       (1000) ced       (1000)     4384 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/fonts/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)    58284 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/fonts/karla.ttf
--rw-r--r--   0 ced       (1000) ced       (1000)     1323 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ir.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    21357 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/lang.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27227 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/lang.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.643484 trytond-6.8.2/trytond/ir/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)   100724 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    99739 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    87078 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)   101295 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)   100595 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    81805 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    93862 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)   102927 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    86753 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)   101311 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    96718 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    86440 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    96368 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    92224 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    92210 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    99075 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    99407 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    97205 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    92005 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)   103100 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    95508 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    86889 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)   111911 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    96295 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1490 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/message.py
--rw-r--r--   0 ced       (1000) ced       (1000)    21762 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    61326 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16085 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/model.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    20966 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/module.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8376 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/module.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     4199 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/note.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1562 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/note.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/queue.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9445 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/queue_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6477 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/resource.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10150 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11734 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2035 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/rule.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    13807 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/sequence.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4927 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     5562 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/session.py
--rw-r--r--   0 ced       (1000) ced       (1000)    67166 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/translation.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7726 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/translation.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    12236 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/trigger.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1529 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/trigger.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.663484 trytond-6.8.2/trytond/ir/ui/
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5531 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/board.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)    18063 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/board.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     1033 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/calendar.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)     3508 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/calendar.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     9858 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/form.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)    33494 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/form.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/graph.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)     5214 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/graph.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     2520 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/icon.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1521 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/icon.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.670151 trytond-6.8.2/trytond/ir/ui/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/icons/tryton-board.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/icons/tryton-calendar.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/icons/tryton-folder.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/icons/tryton-form.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/icons/tryton-graph.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/icons/tryton-list.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/icons/tryton-settings.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/icons/tryton-tree.svg
--rw-r--r--   0 ced       (1000) ced       (1000)     9173 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/menu.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2962 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/menu.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3818 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/tree.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)    13292 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/tree.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/ui.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    22402 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/view.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7956 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/ui/view.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.773486 trytond-6.8.2/trytond/ir/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      566 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_act_window_domain_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_act_window_domain_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_act_window_domain_list2.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1698 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_act_window_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_act_window_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_act_window_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      271 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_act_window_view_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_act_window_view_list2.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      878 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_keyword_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      289 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_keyword_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1752 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_report_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_report_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      736 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_url_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_url_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_wizard_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/action_wizard_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1132 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/attachment_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/attachment_form_preview.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      768 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/attachment_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/cron_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      523 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/cron_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/email_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/email_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1204 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/email_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/email_template_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      699 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/error_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/error_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/export_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/export_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/export_line_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/export_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/icon_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/icon_view_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/lang_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/lang_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/lang_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      219 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/message_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/message_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      779 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_access_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_access_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_button_click_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_button_click_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      676 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_button_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_button_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      534 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_button_rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_button_rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      870 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_data_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      427 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_data_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      779 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_field_access_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_field_access_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      679 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_field_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_field_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      552 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      496 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_log_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_log_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/model_print_model_graph_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/module_activate_upgrade_done_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      657 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/module_activate_upgrade_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/module_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/module_config_wizard_done_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      432 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/module_config_wizard_first_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/module_config_wizard_item_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/module_config_wizard_other_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/module_dependency_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/module_dependency_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      880 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/module_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/module_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/note_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/note_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/rule_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1064 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/rule_group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      443 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/rule_group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      255 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/rule_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1620 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/sequence_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/sequence_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/sequence_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/sequence_type_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/translation_clean_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/translation_clean_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/translation_export_result_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/translation_export_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/translation_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      517 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/translation_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/translation_set_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/translation_set_succeed_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/translation_update_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1035 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/trigger_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/trigger_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/ui_menu_favorite_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      279 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/ui_menu_favorite_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      625 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/ui_menu_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/ui_menu_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/ui_menu_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/ui_view_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      439 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/ui_view_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/ui_view_search_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/ui_view_search_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/ui_view_tree_optional_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/ui_view_tree_optional_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      582 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/ui_view_tree_state_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/ui_view_tree_state_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/ui_view_tree_width_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/ir/view/ui_view_tree_width_list.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.793486 trytond-6.8.2/trytond/model/
--rw-r--r--   0 ced       (1000) ced       (1000)     1177 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1365 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/active.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3105 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/avatar.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1050 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/descriptors.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9337 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/dictschema.py
--rw-r--r--   0 ced       (1000) ced       (1000)      927 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/digits.py
--rw-r--r--   0 ced       (1000) ced       (1000)      962 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.813486 trytond-6.8.2/trytond/model/fields/
--rw-r--r--   0 ced       (1000) ced       (1000)     1216 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4592 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1395 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/boolean.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9577 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/char.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7104 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/date.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8280 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/dict.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27311 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/field.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2603 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7529 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/function.py
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)    18790 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14292 2023-06-10 09:48:56.000000 trytond-6.8.2/trytond/model/fields/many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4401 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1508 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/numeric.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16083 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2116 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8320 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7639 2023-06-10 09:41:31.000000 trytond-6.8.2/trytond/model/fields/selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3517 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/fields/text.py
--rw-r--r--   0 ced       (1000) ced       (1000)      727 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/match.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17168 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4605 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/modelsingleton.py
--rw-r--r--   0 ced       (1000) ced       (1000)    86283 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/modelsql.py
--rw-r--r--   0 ced       (1000) ced       (1000)    82807 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/modelstorage.py
--rw-r--r--   0 ced       (1000) ced       (1000)    36331 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/modelview.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3773 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2712 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/order.py
--rw-r--r--   0 ced       (1000) ced       (1000)      630 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/symbol.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6355 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/tree.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2198 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/union.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2234 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/model/workflow.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.813486 trytond-6.8.2/trytond/modules/
--rw-r--r--   0 ced       (1000) ced       (1000)    16166 2023-05-13 22:24:55.000000 trytond-6.8.2/trytond/modules/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9456 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/pool.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.820153 trytond-6.8.2/trytond/protocols/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/protocols/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8468 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/protocols/dispatcher.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5759 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/protocols/jsonrpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9405 2023-06-10 09:50:52.000000 trytond-6.8.2/trytond/protocols/wrappers.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5602 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/protocols/xmlrpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22275 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/pyson.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.820153 trytond-6.8.2/trytond/report/
--rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/report/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19856 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/report/report.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.836820 trytond-6.8.2/trytond/res/
--rw-r--r--   0 ced       (1000) ced       (1000)     1218 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1301 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/email_reset_password.html
--rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/exceptions.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3732 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/group.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2674 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/group.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     9576 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)    39551 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/ir.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.863487 trytond-6.8.2/trytond/res/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    14621 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15011 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12816 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15227 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15182 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12426 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14090 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14966 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12777 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    15436 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14355 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13372 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13807 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16364 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14553 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14944 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14961 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13981 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14922 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14815 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    13921 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    12777 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    16986 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    14333 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)     1395 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/res.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2454 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)       96 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/tryton.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)    43825 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/user.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8284 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/user.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.876820 trytond-6.8.2/trytond/res/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/view/export_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/view/export_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1153 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/view/group_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/view/group_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/view/sequence_type_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/view/user_application_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/view/user_application_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      578 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/view/user_config_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1527 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1386 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/view/user_form_preferences.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/view/user_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/view/user_warning_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/res/view/user_warning_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     3644 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/rpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4804 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/security.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4965 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/sendmail.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3205 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/status.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:49.003489 trytond-6.8.2/trytond/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)     2462 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1202 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/access.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3885 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/copy_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1989 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/export_data.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1061 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)      707 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_boolean.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2372 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_char.py
--rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_context.py
--rw-r--r--   0 ced       (1000) ced       (1000)      943 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_date.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_datetime.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1820 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_dict.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1248 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2676 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_function.py
--rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_function.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1162 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7491 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2845 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1398 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1354 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_numeric.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5212 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3123 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3071 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1981 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1489 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_text.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1224 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_time.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1063 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/field_timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)        9 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/forbidden.txt
--rw-r--r--   0 ced       (1000) ced       (1000)      917 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/history.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5599 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/import_data.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/import_data.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1083 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/mixin.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4126 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1493 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/model_log.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7377 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/modelsql.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7720 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/modelstorage.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8349 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/modelview.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3695 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/modelview.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1116 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/mptt.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)      632 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/path.py
--rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/resource.py
--rw-r--r--   0 ced       (1000) ced       (1000)      971 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)      584 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/sequence.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    34615 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_access.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6538 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_backend.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4725 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_bus.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9968 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_cache.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11841 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_copy.py
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_descriptors.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14582 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_exportdata.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6048 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_binary.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7503 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_boolean.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22837 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_char.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1021 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_context.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13633 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_date.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15520 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_datetime.py
--rw-r--r--   0 ced       (1000) ced       (1000)     7608 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_depends.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27461 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_dict.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13029 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_float.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3626 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_function.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10440 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_integer.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25082 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_many2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15081 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_many2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12677 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_multiselection.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16606 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_numeric.py
--rw-r--r--   0 ced       (1000) ced       (1000)    23584 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_one2many.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9821 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_one2one.py
--rw-r--r--   0 ced       (1000) ced       (1000)    20600 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_reference.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9360 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_selection.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19472 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_text.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13981 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_time.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15036 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_field_timedelta.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3019 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_filestore.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15175 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_history.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3648 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_i18n.py
--rw-r--r--   0 ced       (1000) ced       (1000)    19311 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_importdata.py
--rw-r--r--   0 ced       (1000) ced       (1000)    16316 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_ir.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4610 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_mixins.py
--rw-r--r--   0 ced       (1000) ced       (1000)    13792 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_model.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4393 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_model_index.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8288 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_model_log.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4825 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_modelsingleton.py
--rw-r--r--   0 ced       (1000) ced       (1000)    51742 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_modelsql.py
--rw-r--r--   0 ced       (1000) ced       (1000)    31235 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_modelstorage.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24647 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_modelview.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3450 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_mptt.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8733 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3073 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_order.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1045 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_path.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3726 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_protocols.py
--rw-r--r--   0 ced       (1000) ced       (1000)    33898 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_pyson.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2340 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_report.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2413 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_res.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2416 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_resource.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6365 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_routes.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4377 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_rpc.py
--rw-r--r--   0 ced       (1000) ced       (1000)    26679 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_rule.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4323 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_sendmail.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5020 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_sequence.py
--rw-r--r--   0 ced       (1000) ced       (1000)    39952 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4759 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_transaction.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11788 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_tree.py
--rw-r--r--   0 ced       (1000) ced       (1000)    15386 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_trigger.py
--rw-r--r--   0 ced       (1000) ced       (1000)    42503 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_tryton.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3353 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_union.py
--rw-r--r--   0 ced       (1000) ced       (1000)    11988 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_user.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5501 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)      819 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_workflow.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3171 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/test_wsgi.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1187 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/tools.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1180 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/tree.py
--rw-r--r--   0 ced       (1000) ced       (1000)      984 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/trigger.py
--rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/tryton.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)      887 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/wizard.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      928 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/workflow.py
--rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tests/workflow.xml
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:49.013489 trytond-6.8.2/trytond/tools/
--rw-r--r--   0 ced       (1000) ced       (1000)     1618 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tools/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1902 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tools/barcode.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1621 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tools/decimal_.py
--rw-r--r--   0 ced       (1000) ced       (1000)    17206 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tools/domain_inversion.py
--rw-r--r--   0 ced       (1000) ced       (1000)      764 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tools/email_.py
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tools/gevent.py
--rw-r--r--   0 ced       (1000) ced       (1000)      545 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tools/immutabledict.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9313 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tools/misc.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3893 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tools/multivalue.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1595 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tools/qrcode.py
--rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tools/singleton.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3864 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tools/string_.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1144 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tools/timezone.py
--rw-r--r--   0 ced       (1000) ced       (1000)    12661 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/transaction.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1445 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tryton.rnc
--rw-r--r--   0 ced       (1000) ced       (1000)     5501 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/tryton.rng
--rw-r--r--   0 ced       (1000) ced       (1000)     2754 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/url.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:49.016822 trytond-6.8.2/trytond/wizard/
--rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/wizard/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    14525 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/wizard/wizard.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6882 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/worker.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9486 2023-05-01 12:17:32.000000 trytond-6.8.2/trytond/wsgi.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-06-21 17:09:48.533483 trytond-6.8.2/trytond.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2681 2023-06-21 17:09:47.000000 trytond-6.8.2/trytond.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)    16279 2023-06-21 17:09:48.000000 trytond-6.8.2/trytond.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-06-21 17:09:47.000000 trytond-6.8.2/trytond.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:29:16.000000 trytond-6.8.2/trytond.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-06-21 17:09:47.000000 trytond-6.8.2/trytond.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-06-21 17:09:47.000000 trytond-6.8.2/trytond.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:30.316774 trytond-6.8.3/
+-rw-r--r--   0 ced       (1000) ced       (1000)    38946 2023-07-31 15:06:26.000000 trytond-6.8.3/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      938 2023-07-31 15:06:25.000000 trytond-6.8.3/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-05-01 12:17:32.000000 trytond-6.8.3/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      204 2023-05-01 12:17:32.000000 trytond-6.8.3/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2681 2023-07-31 15:06:30.316774 trytond-6.8.3/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      195 2023-05-01 12:17:32.000000 trytond-6.8.3/README.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.690099 trytond-6.8.3/bin/
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     2888 2023-05-01 12:17:32.000000 trytond-6.8.3/bin/trytond
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      807 2023-05-01 12:17:32.000000 trytond-6.8.3/bin/trytond-admin
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      783 2023-05-01 12:17:32.000000 trytond-6.8.3/bin/trytond-console
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      889 2023-05-01 12:17:32.000000 trytond-6.8.3/bin/trytond-cron
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4892 2023-05-01 12:17:32.000000 trytond-6.8.3/bin/trytond-stat
+-rwxr-xr-x   0 ced       (1000) ced       (1000)      898 2023-05-01 12:17:32.000000 trytond-6.8.3/bin/trytond-worker
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.693433 trytond-6.8.3/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1677 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1280 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.700100 trytond-6.8.3/doc/ref/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10247 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/backend.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3269 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/bus.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2656 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/cache.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2632 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/exceptions.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    31979 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/fields.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1171 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/filestore.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      664 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/i18n.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    31734 2023-07-22 21:21:59.000000 trytond-6.8.3/doc/ref/models.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2041 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/pool.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8787 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/pyson.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1461 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/rpc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2109 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/sendmail.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3139 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/tests.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.703433 trytond-6.8.3/doc/ref/tools/
+-rw-r--r--   0 ced       (1000) ced       (1000)      565 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/tools/barcode.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      183 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/tools/email.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/tools/immutabledict.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      173 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/tools/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1313 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/tools/misc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      434 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/tools/qrcode.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/tools/singleton.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      608 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/tools/timezone.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5510 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/ref/transaction.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6064 2023-07-22 21:21:59.000000 trytond-6.8.3/doc/ref/wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/releases.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.716766 trytond-6.8.3/doc/topics/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3717 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/access_rights.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      992 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/actions.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4014 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/backend_types.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      788 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/bus.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    14772 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1431 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/cron.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7848 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/domain.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      536 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      983 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/install.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1108 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/logs.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.720100 trytond-6.8.3/doc/topics/models/
+-rw-r--r--   0 ced       (1000) ced       (1000)      840 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/models/fields_default_value.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1197 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/models/fields_on_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1376 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/models/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.720100 trytond-6.8.3/doc/topics/modules/
+-rw-r--r--   0 ced       (1000) ced       (1000)     6022 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/modules/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3887 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/pyson.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.723433 trytond-6.8.3/doc/topics/reports/
+-rw-r--r--   0 ced       (1000) ced       (1000)     8742 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/reports/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1381 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/rpc.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1783 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/setup_database.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2912 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/start_server.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2229 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/task_queue.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2880 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/testing.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2191 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/translation.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      922 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/triggers.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2596 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/user_application.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2034 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/user_errors_warnings.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.723433 trytond-6.8.3/doc/topics/views/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1130 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/views/extension.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    25050 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/views/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1669 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/topics/wizard.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.726766 trytond-6.8.3/doc/tutorial/
+-rw-r--r--   0 ced       (1000) ced       (1000)       98 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/index.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.740100 trytond-6.8.3/doc/tutorial/module/
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/anatomy.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1843 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/default_values.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3334 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/domains.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2917 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/extend.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3524 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/function_fields.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      768 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3935 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/model.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2662 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/on_change.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3727 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/report.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1712 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/setup.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/setup_database.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3097 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/states.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4746 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/table_query.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     6258 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/view.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5047 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/wizard.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4773 2023-05-01 12:17:32.000000 trytond-6.8.3/doc/tutorial/module/workflow.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-07-31 15:06:30.316774 trytond-6.8.3/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     5418 2023-05-01 12:17:32.000000 trytond-6.8.3/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      597 2023-05-01 12:17:32.000000 trytond-6.8.3/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.770100 trytond-6.8.3/trytond/
+-rw-r--r--   0 ced       (1000) ced       (1000)      926 2023-06-21 17:10:04.000000 trytond-6.8.3/trytond/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6930 2023-06-10 09:41:09.000000 trytond-6.8.3/trytond/admin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1370 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/application.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.776767 trytond-6.8.3/trytond/backend/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1093 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/backend/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4390 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/backend/database.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.783434 trytond-6.8.3/trytond/backend/postgresql/
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/backend/postgresql/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    26462 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/backend/postgresql/database.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3631 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/backend/postgresql/init.sql
+-rw-r--r--   0 ced       (1000) ced       (1000)    26820 2023-06-10 09:39:42.000000 trytond-6.8.3/trytond/backend/postgresql/table.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.786767 trytond-6.8.3/trytond/backend/sqlite/
+-rw-r--r--   0 ced       (1000) ced       (1000)      402 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/backend/sqlite/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20773 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/backend/sqlite/database.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2209 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/backend/sqlite/init.sql
+-rw-r--r--   0 ced       (1000) ced       (1000)    16323 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/backend/sqlite/table.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4129 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/backend/table.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9431 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/bus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16982 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7095 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/commandline.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6437 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/config.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2280 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/console.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/const.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31266 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/convert.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1490 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/cron.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2055 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2122 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/filestore.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1036 2023-07-22 21:33:11.000000 trytond-6.8.3/trytond/i18n.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.846768 trytond-6.8.3/trytond/ir/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3329 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    41248 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/action.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9920 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/action.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4059 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/attachment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1960 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/attachment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6355 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/avatar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2089 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/calendar_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4282 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/calendar_.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1459 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7820 2023-05-04 17:44:31.000000 trytond-6.8.3/trytond/ir/cron.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1954 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/cron.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      596 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4525 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/email.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    20472 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/email_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5928 2023-07-03 20:58:53.000000 trytond-6.8.3/trytond/ir/error.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3592 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/error.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      947 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1858 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/export.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2070 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/export.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.850101 trytond-6.8.3/trytond/ir/fonts/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4384 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/fonts/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)    58284 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/fonts/karla.ttf
+-rw-r--r--   0 ced       (1000) ced       (1000)     1323 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ir.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    21357 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/lang.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27227 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/lang.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.903435 trytond-6.8.3/trytond/ir/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)   100724 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    99739 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    87078 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   101295 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   100595 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    81805 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    93862 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   102927 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    86753 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   101311 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    96718 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    86440 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    96368 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    92224 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    92210 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    99075 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    99407 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    97205 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    92005 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   103100 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    95508 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    86889 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   111911 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    96295 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1490 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/message.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    21762 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    61326 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16085 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/model.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    20966 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8376 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/module.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     4199 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/note.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1562 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/note.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/queue.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9445 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/queue_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6477 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/resource.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10150 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11734 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2035 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/rule.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    13807 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/sequence.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4927 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     5562 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/session.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    67166 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/translation.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7726 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/translation.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    12236 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/trigger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1529 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/trigger.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      346 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.930102 trytond-6.8.3/trytond/ir/ui/
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5531 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/board.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)    18063 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/board.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     1033 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/calendar.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)     3508 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/calendar.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     9858 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/form.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)    33494 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/form.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     1400 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/graph.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)     5214 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/graph.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     2520 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/icon.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1521 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/icon.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.940102 trytond-6.8.3/trytond/ir/ui/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/icons/tryton-board.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      313 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/icons/tryton-calendar.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/icons/tryton-folder.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      299 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/icons/tryton-form.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/icons/tryton-graph.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      211 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/icons/tryton-list.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/icons/tryton-settings.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/icons/tryton-tree.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)     9173 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/menu.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2962 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/menu.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3818 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/tree.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)    13292 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/tree.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     2022 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/ui.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    22402 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/view.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7956 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/ui/view.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:30.053437 trytond-6.8.3/trytond/ir/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      566 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_act_window_domain_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      295 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_act_window_domain_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      316 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_act_window_domain_list2.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1698 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_act_window_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_act_window_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      422 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_act_window_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      271 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_act_window_view_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      290 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_act_window_view_list2.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      878 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_keyword_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      289 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_keyword_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1752 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_report_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_report_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      736 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_url_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_url_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      907 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_wizard_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/action_wizard_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1132 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/attachment_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/attachment_form_preview.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      768 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/attachment_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1052 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/cron_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      523 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/cron_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      714 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/email_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      507 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/email_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1204 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/email_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/email_template_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      699 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/error_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      389 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/error_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      406 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/export_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/export_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/export_line_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/export_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/icon_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      343 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/icon_view_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/lang_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2076 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/lang_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      375 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/lang_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      219 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/message_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/message_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      779 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_access_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_access_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      404 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_button_click_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      301 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_button_click_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      676 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_button_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      259 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_button_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      534 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_button_rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_button_rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      870 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_data_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      427 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_data_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      779 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_field_access_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_field_access_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      679 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_field_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      493 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_field_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      552 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      384 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      496 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_log_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      446 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_log_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/model_print_model_graph_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      381 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/module_activate_upgrade_done_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      657 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/module_activate_upgrade_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      449 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/module_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      353 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/module_config_wizard_done_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      432 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/module_config_wizard_first_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/module_config_wizard_item_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      300 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/module_config_wizard_other_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      357 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/module_dependency_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      275 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/module_dependency_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      880 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/module_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      547 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/module_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/note_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/note_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/rule_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1064 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/rule_group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      443 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/rule_group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      255 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/rule_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1620 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/sequence_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      407 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/sequence_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      236 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/sequence_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      222 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/sequence_type_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/translation_clean_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/translation_clean_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/translation_export_result_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      336 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/translation_export_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      786 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/translation_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      517 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/translation_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      363 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/translation_set_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      352 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/translation_set_succeed_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/translation_update_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1035 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/trigger_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      403 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/trigger_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      344 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/ui_menu_favorite_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      279 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/ui_menu_favorite_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      625 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/ui_menu_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/ui_menu_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/ui_menu_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      757 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/ui_view_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      439 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/ui_view_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      436 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/ui_view_search_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      258 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/ui_view_search_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      397 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/ui_view_tree_optional_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      324 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/ui_view_tree_optional_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      582 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/ui_view_tree_state_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/ui_view_tree_state_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      392 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/ui_view_tree_width_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      322 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/ir/view/ui_view_tree_width_list.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:30.076771 trytond-6.8.3/trytond/model/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1177 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1365 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/active.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3105 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/avatar.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1050 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/descriptors.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9337 2023-07-03 21:06:02.000000 trytond-6.8.3/trytond/model/dictschema.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      927 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/digits.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      962 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:30.096771 trytond-6.8.3/trytond/model/fields/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1216 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4592 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1395 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/boolean.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9577 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7104 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8280 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/dict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27311 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/field.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2603 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7529 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/function.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    18790 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14292 2023-06-10 09:48:56.000000 trytond-6.8.3/trytond/model/fields/many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4401 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1508 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/numeric.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16083 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2116 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8320 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7639 2023-06-10 09:41:31.000000 trytond-6.8.3/trytond/model/fields/selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3517 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/fields/text.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      727 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/match.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17168 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4605 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/modelsingleton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    86512 2023-07-31 13:24:22.000000 trytond-6.8.3/trytond/model/modelsql.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    82856 2023-07-22 21:16:13.000000 trytond-6.8.3/trytond/model/modelstorage.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    36331 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/modelview.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3773 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2712 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/order.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      630 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/symbol.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6355 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/tree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2198 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/union.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2234 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/model/workflow.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:30.096771 trytond-6.8.3/trytond/modules/
+-rw-r--r--   0 ced       (1000) ced       (1000)    16338 2023-07-22 21:28:23.000000 trytond-6.8.3/trytond/modules/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9456 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/pool.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:30.103438 trytond-6.8.3/trytond/protocols/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/protocols/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8468 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/protocols/dispatcher.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5759 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/protocols/jsonrpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9405 2023-06-10 09:50:52.000000 trytond-6.8.3/trytond/protocols/wrappers.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5602 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/protocols/xmlrpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22275 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/pyson.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:30.106771 trytond-6.8.3/trytond/report/
+-rw-r--r--   0 ced       (1000) ced       (1000)      213 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/report/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19856 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/report/report.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:30.123438 trytond-6.8.3/trytond/res/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1218 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1301 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/email_reset_password.html
+-rw-r--r--   0 ced       (1000) ced       (1000)      245 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/exceptions.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3732 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/group.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2674 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/group.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     9576 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    39551 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/ir.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:30.153438 trytond-6.8.3/trytond/res/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    14621 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15011 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12816 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15227 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15182 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12426 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14090 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14966 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12777 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    15436 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14355 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13372 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13807 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16364 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14553 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14944 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14961 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13981 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14922 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14815 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    13921 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    12777 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    16986 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    14333 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     1395 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/res.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2454 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)       96 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/tryton.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)    43825 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/user.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8284 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/user.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:30.166772 trytond-6.8.3/trytond/res/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      358 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/view/export_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/view/export_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1153 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/view/group_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      260 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/view/group_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      283 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/view/sequence_type_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      579 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/view/user_application_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/view/user_application_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      578 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/view/user_config_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1527 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1386 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/view/user_form_preferences.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      393 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/view/user_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      355 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/view/user_warning_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      263 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/res/view/user_warning_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     3644 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/rpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4804 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/security.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4965 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/sendmail.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3205 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/status.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:30.300107 trytond-6.8.3/trytond/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2462 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1202 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/access.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3885 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/copy_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2023 2023-07-22 21:16:13.000000 trytond-6.8.3/trytond/tests/export_data.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1061 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      707 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_boolean.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2372 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      829 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_context.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      943 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1244 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_datetime.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1820 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_dict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1248 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2676 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_function.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      320 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_function.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1162 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7491 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2845 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1398 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1354 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_numeric.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5212 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3123 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1981 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1489 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_text.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1224 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_time.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1063 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/field_timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)        9 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/forbidden.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)      917 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/history.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5599 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/import_data.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2214 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/import_data.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1083 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/mixin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4126 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1493 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/model_log.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7377 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/modelsql.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7720 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/modelstorage.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8349 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/modelview.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3695 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/modelview.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1116 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/mptt.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2819 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      632 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/path.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      678 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/resource.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      971 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      584 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/sequence.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    34615 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_access.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6538 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_backend.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4725 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_bus.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9968 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_cache.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11841 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_copy.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_descriptors.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15266 2023-07-22 21:16:13.000000 trytond-6.8.3/trytond/tests/test_exportdata.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6048 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_binary.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7503 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_boolean.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22837 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_char.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1021 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_context.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13633 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_date.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15520 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_datetime.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     7608 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_depends.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27461 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_dict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13029 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_float.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3626 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_function.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10440 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_integer.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25082 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_many2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15081 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_many2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12677 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_multiselection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16606 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_numeric.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    23584 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_one2many.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9821 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_one2one.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    20600 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_reference.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9360 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_selection.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19472 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_text.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13981 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_time.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15036 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_field_timedelta.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3019 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_filestore.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15175 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_history.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3648 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_i18n.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    19311 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_importdata.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    16316 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_ir.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4610 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_mixins.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    13792 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_model.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4396 2023-07-03 20:56:59.000000 trytond-6.8.3/trytond/tests/test_model_index.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8288 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_model_log.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4825 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_modelsingleton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    51742 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_modelsql.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    31235 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_modelstorage.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24647 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_modelview.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3450 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_mptt.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8733 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3073 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_order.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1045 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_path.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3726 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_protocols.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    33898 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_pyson.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2340 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_report.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2413 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2416 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_resource.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6365 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_routes.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4377 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_rpc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27797 2023-07-31 13:24:22.000000 trytond-6.8.3/trytond/tests/test_rule.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4323 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_sendmail.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5020 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_sequence.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    39952 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4759 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_transaction.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11788 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_tree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    15386 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_trigger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    42637 2023-07-10 21:28:50.000000 trytond-6.8.3/trytond/tests/test_tryton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3353 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_union.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    11988 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_user.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5501 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      819 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_workflow.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3171 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/test_wsgi.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1187 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/tools.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1180 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/tree.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      984 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/trigger.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      164 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/tryton.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1586 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      887 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/wizard.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      928 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/workflow.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      218 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tests/workflow.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:30.313440 trytond-6.8.3/trytond/tools/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1618 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tools/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1902 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tools/barcode.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1621 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tools/decimal_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    17206 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tools/domain_inversion.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      764 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tools/email_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tools/gevent.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      545 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tools/immutabledict.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9313 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tools/misc.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3893 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tools/multivalue.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1595 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tools/qrcode.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      526 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tools/singleton.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3864 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tools/string_.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1144 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tools/timezone.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    12661 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/transaction.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1445 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tryton.rnc
+-rw-r--r--   0 ced       (1000) ced       (1000)     5501 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/tryton.rng
+-rw-r--r--   0 ced       (1000) ced       (1000)     2754 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/url.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:30.316774 trytond-6.8.3/trytond/wizard/
+-rw-r--r--   0 ced       (1000) ced       (1000)      342 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/wizard/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    14525 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/wizard/wizard.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6882 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/worker.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9486 2023-05-01 12:17:32.000000 trytond-6.8.3/trytond/wsgi.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-07-31 15:06:29.773434 trytond-6.8.3/trytond.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2681 2023-07-31 15:06:28.000000 trytond-6.8.3/trytond.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)    16279 2023-07-31 15:06:29.000000 trytond-6.8.3/trytond.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-07-31 15:06:28.000000 trytond-6.8.3/trytond.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-17 20:29:16.000000 trytond-6.8.3/trytond.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      481 2023-07-31 15:06:28.000000 trytond-6.8.3/trytond.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-07-31 15:06:28.000000 trytond-6.8.3/trytond.egg-info/top_level.txt
```

### Comparing `trytond-6.8.2/CHANGELOG` & `trytond-6.8.3/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+Version 6.8.3 - 2023-07-31
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Enforce record rules when reading only non SQL fields (#12428)
+
 Version 6.8.2 - 2023-06-21
 --------------------------
 * Bug fixes (see mercurial logs for details)
 
 
 Version 6.8.1 - 2023-05-17
 --------------------------
```

### Comparing `trytond-6.8.2/COPYRIGHT` & `trytond-6.8.3/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/LICENSE` & `trytond-6.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/PKG-INFO` & `trytond-6.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond
-Version: 6.8.2
+Version: 6.8.3
 Summary: Tryton server
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond-6.8.2/bin/trytond` & `trytond-6.8.3/bin/trytond`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/bin/trytond-admin` & `trytond-6.8.3/bin/trytond-admin`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/bin/trytond-console` & `trytond-6.8.3/bin/trytond-console`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/bin/trytond-cron` & `trytond-6.8.3/bin/trytond-cron`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/bin/trytond-stat` & `trytond-6.8.3/bin/trytond-stat`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/bin/trytond-worker` & `trytond-6.8.3/bin/trytond-worker`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/conf.py` & `trytond-6.8.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/index.rst` & `trytond-6.8.3/doc/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/backend.rst` & `trytond-6.8.3/doc/ref/backend.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/bus.rst` & `trytond-6.8.3/doc/ref/bus.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/cache.rst` & `trytond-6.8.3/doc/ref/cache.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/exceptions.rst` & `trytond-6.8.3/doc/ref/exceptions.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/fields.rst` & `trytond-6.8.3/doc/ref/fields.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/filestore.rst` & `trytond-6.8.3/doc/ref/filestore.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/i18n.rst` & `trytond-6.8.3/doc/ref/i18n.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/models.rst` & `trytond-6.8.3/doc/ref/models.rst`

 * *Files 0% similar despite different names*

```diff
@@ -102,32 +102,14 @@
    Return a dictionary with the name of the ``model``, the ``field`` and the
    ``record`` and the ``value`` of the field.
    It is a convenience-method used to format messages which should include
    those names.
 
 Instance methods:
 
-.. method:: Model.on_change(fieldnames)
-
-   Return the list of changes by calling ``on_change`` method of each field.
-
-.. method:: Model.on_change_with(fieldnames)
-
-   Return the new values of all fields by calling ``on_change_with`` method of
-   each field.
-
-.. method:: Model.on_change_notify(fieldnames)
-
-    Returns a list of type and message couple to display on the client side.
-    Available types are ``info``, ``warning`` and ``error``.
-
-    .. note::
-      To be called by the client, this method must be decorated
-      by :meth:`~trytond.model.fields.depends` with the fields needed.
-
 .. method:: Model.pre_validate()
 
    Validate the instance before being stored.
    This method is called by the client to validate the instance.
 
 ModelView
 =========
@@ -224,14 +206,34 @@
    Return the sanitized XML and the corresponding fields definition.
 
    .. note::
 
       This method is public mainly to allow modification the existing XML of
       the view by code.
 
+Instance methods:
+
+.. method:: ModelView.on_change(fieldnames)
+
+   Return the list of changes by calling ``on_change`` method of each field.
+
+.. method:: ModelView.on_change_with(fieldnames)
+
+   Return the new values of all fields by calling ``on_change_with`` method of
+   each field.
+
+.. method:: ModelView.on_change_notify(fieldnames)
+
+    Returns a list of type and message couple to display on the client side.
+    Available types are ``info``, ``warning`` and ``error``.
+
+    .. note::
+      To be called by the client, this method must be decorated
+      by :meth:`~trytond.model.fields.depends` with the fields needed.
+
 ModelStorage
 ============
 
 .. class:: ModelStorage
 
 Add storage capability of record.
```

### Comparing `trytond-6.8.2/doc/ref/pool.rst` & `trytond-6.8.3/doc/ref/pool.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/pyson.rst` & `trytond-6.8.3/doc/ref/pyson.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/rpc.rst` & `trytond-6.8.3/doc/ref/rpc.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/sendmail.rst` & `trytond-6.8.3/doc/ref/sendmail.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/tests.rst` & `trytond-6.8.3/doc/ref/tests.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/tools/barcode.rst` & `trytond-6.8.3/doc/ref/tools/barcode.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/tools/misc.rst` & `trytond-6.8.3/doc/ref/tools/misc.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/tools/timezone.rst` & `trytond-6.8.3/doc/ref/tools/timezone.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/transaction.rst` & `trytond-6.8.3/doc/ref/transaction.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/ref/wizard.rst` & `trytond-6.8.3/doc/ref/wizard.rst`

 * *Files 1% similar despite different names*

```diff
@@ -119,16 +119,16 @@
    The default values of the view can be set with a method on wizard having the
    same name as the state but starting with ``default_``.
    The values of the view can be also set with a method on wizard having the
    same name as the state but starting with ``value_``.
 
    .. note::
       The difference between default values and values is that the client calls
-      :meth:`~trytond.model.Model.on_change` and
-      :meth:`~trytond.model.Model.on_change_with` for the default values.
+      :meth:`~trytond.model.ModelView.on_change` and
+      :meth:`~trytond.model.ModelView.on_change_with` for the default values.
 
 Instance attributes are:
 
 .. attribute:: StateView.model_name
 
    The name of the :class:`~trytond.model.ModelView`.
```

### Comparing `trytond-6.8.2/doc/topics/access_rights.rst` & `trytond-6.8.3/doc/topics/access_rights.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/actions.rst` & `trytond-6.8.3/doc/topics/actions.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/backend_types.rst` & `trytond-6.8.3/doc/topics/backend_types.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/bus.rst` & `trytond-6.8.3/doc/topics/bus.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/configuration.rst` & `trytond-6.8.3/doc/topics/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/cron.rst` & `trytond-6.8.3/doc/topics/cron.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/domain.rst` & `trytond-6.8.3/doc/topics/domain.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/index.rst` & `trytond-6.8.3/doc/topics/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/install.rst` & `trytond-6.8.3/doc/topics/install.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/logs.rst` & `trytond-6.8.3/doc/topics/logs.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/models/fields_default_value.rst` & `trytond-6.8.3/doc/topics/models/fields_default_value.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/models/fields_on_change.rst` & `trytond-6.8.3/doc/topics/models/fields_on_change.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/models/index.rst` & `trytond-6.8.3/doc/topics/models/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/modules/index.rst` & `trytond-6.8.3/doc/topics/modules/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/pyson.rst` & `trytond-6.8.3/doc/topics/pyson.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/reports/index.rst` & `trytond-6.8.3/doc/topics/reports/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/rpc.rst` & `trytond-6.8.3/doc/topics/rpc.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/setup_database.rst` & `trytond-6.8.3/doc/topics/setup_database.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/start_server.rst` & `trytond-6.8.3/doc/topics/start_server.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/task_queue.rst` & `trytond-6.8.3/doc/topics/task_queue.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/testing.rst` & `trytond-6.8.3/doc/topics/testing.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/translation.rst` & `trytond-6.8.3/doc/topics/translation.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/triggers.rst` & `trytond-6.8.3/doc/topics/triggers.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/user_application.rst` & `trytond-6.8.3/doc/topics/user_application.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/user_errors_warnings.rst` & `trytond-6.8.3/doc/topics/user_errors_warnings.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/views/extension.rst` & `trytond-6.8.3/doc/topics/views/extension.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/views/index.rst` & `trytond-6.8.3/doc/topics/views/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/topics/wizard.rst` & `trytond-6.8.3/doc/topics/wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/anatomy.rst` & `trytond-6.8.3/doc/tutorial/module/anatomy.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/default_values.rst` & `trytond-6.8.3/doc/tutorial/module/default_values.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/domains.rst` & `trytond-6.8.3/doc/tutorial/module/domains.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/extend.rst` & `trytond-6.8.3/doc/tutorial/module/extend.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/function_fields.rst` & `trytond-6.8.3/doc/tutorial/module/function_fields.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/index.rst` & `trytond-6.8.3/doc/tutorial/module/index.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/model.rst` & `trytond-6.8.3/doc/tutorial/module/model.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/on_change.rst` & `trytond-6.8.3/doc/tutorial/module/on_change.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/report.rst` & `trytond-6.8.3/doc/tutorial/module/report.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/setup.rst` & `trytond-6.8.3/doc/tutorial/module/setup.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/setup_database.rst` & `trytond-6.8.3/doc/tutorial/module/setup_database.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/states.rst` & `trytond-6.8.3/doc/tutorial/module/states.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/table_query.rst` & `trytond-6.8.3/doc/tutorial/module/table_query.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/view.rst` & `trytond-6.8.3/doc/tutorial/module/view.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/wizard.rst` & `trytond-6.8.3/doc/tutorial/module/wizard.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/doc/tutorial/module/workflow.rst` & `trytond-6.8.3/doc/tutorial/module/workflow.rst`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/setup.py` & `trytond-6.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/tox.ini` & `trytond-6.8.3/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/__init__.py` & `trytond-6.8.3/trytond/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import time
 import warnings
 from email import charset
 
 import __main__
 from lxml import etree, objectify
 
-__version__ = "6.8.2"
+__version__ = "6.8.3"
 
 os.environ.setdefault(
     'TRYTOND_APPNAME',
     os.path.basename(getattr(__main__, '__file__', 'trytond')))
 os.environ.setdefault('TRYTOND_TZ', os.environ.get('TZ', 'UTC'))
 os.environ['TZ'] = 'UTC'
 if hasattr(time, 'tzset'):
```

### Comparing `trytond-6.8.2/trytond/admin.py` & `trytond-6.8.3/trytond/admin.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/application.py` & `trytond-6.8.3/trytond/application.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/backend/__init__.py` & `trytond-6.8.3/trytond/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/backend/database.py` & `trytond-6.8.3/trytond/backend/database.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/backend/postgresql/database.py` & `trytond-6.8.3/trytond/backend/postgresql/database.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/backend/postgresql/init.sql` & `trytond-6.8.3/trytond/backend/postgresql/init.sql`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/backend/postgresql/table.py` & `trytond-6.8.3/trytond/backend/postgresql/table.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/backend/sqlite/database.py` & `trytond-6.8.3/trytond/backend/sqlite/database.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/backend/sqlite/init.sql` & `trytond-6.8.3/trytond/backend/sqlite/init.sql`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/backend/sqlite/table.py` & `trytond-6.8.3/trytond/backend/sqlite/table.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/backend/table.py` & `trytond-6.8.3/trytond/backend/table.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/bus.py` & `trytond-6.8.3/trytond/bus.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/cache.py` & `trytond-6.8.3/trytond/cache.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/commandline.py` & `trytond-6.8.3/trytond/commandline.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/config.py` & `trytond-6.8.3/trytond/config.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/console.py` & `trytond-6.8.3/trytond/console.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/convert.py` & `trytond-6.8.3/trytond/convert.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/cron.py` & `trytond-6.8.3/trytond/cron.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/exceptions.py` & `trytond-6.8.3/trytond/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/filestore.py` & `trytond-6.8.3/trytond/filestore.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/i18n.py` & `trytond-6.8.3/trytond/i18n.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,14 @@
         language, = args
     try:
         module, id_ = message_id.split('.')
     except ValueError:
         return message_id
     try:
         return Message.gettext(module, id_, language, **variables)
-    except KeyError:
+    except (KeyError, ValueError):
         return message_id
 
 
 def lazy_gettext(message_id, *args, **variables):
     "Like gettext but the string returned is lazy"
     return LazyString(gettext, message_id, *args, **variables)
```

### Comparing `trytond-6.8.2/trytond/ir/__init__.py` & `trytond-6.8.3/trytond/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/action.py` & `trytond-6.8.3/trytond/ir/action.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/action.xml` & `trytond-6.8.3/trytond/ir/action.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/attachment.py` & `trytond-6.8.3/trytond/ir/attachment.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/attachment.xml` & `trytond-6.8.3/trytond/ir/attachment.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/avatar.py` & `trytond-6.8.3/trytond/ir/avatar.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/calendar_.py` & `trytond-6.8.3/trytond/ir/calendar_.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/calendar_.xml` & `trytond-6.8.3/trytond/ir/calendar_.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/configuration.py` & `trytond-6.8.3/trytond/ir/configuration.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/cron.py` & `trytond-6.8.3/trytond/ir/cron.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/cron.xml` & `trytond-6.8.3/trytond/ir/cron.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/date.py` & `trytond-6.8.3/trytond/ir/date.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/email.xml` & `trytond-6.8.3/trytond/ir/email.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/email_.py` & `trytond-6.8.3/trytond/ir/email_.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/error.py` & `trytond-6.8.3/trytond/ir/error.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # this repository contains the full copyright notices and license terms.
 import datetime as dt
 import functools
 import logging
 
 from trytond.config import config
 from trytond.exceptions import UserError, UserWarning
-from trytond.model import Index, ModelSQL, ModelView, Workflow, fields
+from trytond.model import (
+    Index, ModelSQL, ModelView, Workflow, dualmethod, fields)
 from trytond.pool import Pool
 from trytond.pyson import Eval
 from trytond.tools import firstline
 from trytond.transaction import Transaction
 
 logger = logging.getLogger(__name__)
 clean_days = config.getint('error', 'clean_days', default=90)
@@ -113,17 +114,22 @@
         return firstline(self.message or '')
 
     def get_rec_name(self, name):
         if self.origin:
             return "%s - %s" % (self.origin_string, self.origin.rec_name)
         return super().get_rec_name(name)
 
-    @classmethod
-    def log(cls, origin, exception):
+    @dualmethod
+    def log(cls, *args, **kwargs):
+        # Test if it is a ModelStorage.log call
+        if len(args) <= 1 or not isinstance(args[1], Exception):
+            return super().log(*args, **kwargs)
         try:
+            origin, exception = args
+            assert not kwargs
             assert isinstance(exception, (UserError, UserWarning))
             with Transaction().new_transaction(autocommit=True):
                 if not cls.search([
                             ('origin', '=', str(origin)),
                             ('message', '=', exception.message),
                             ('description', '=', exception.description),
                             ('state', '!=', 'solved'),
```

### Comparing `trytond-6.8.2/trytond/ir/error.xml` & `trytond-6.8.3/trytond/ir/error.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/exceptions.py` & `trytond-6.8.3/trytond/ir/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/export.py` & `trytond-6.8.3/trytond/ir/export.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/export.xml` & `trytond-6.8.3/trytond/ir/export.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/fonts/LICENSE` & `trytond-6.8.3/trytond/ir/fonts/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/fonts/karla.ttf` & `trytond-6.8.3/trytond/ir/fonts/karla.ttf`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ir.xml` & `trytond-6.8.3/trytond/ir/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/lang.py` & `trytond-6.8.3/trytond/ir/lang.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/lang.xml` & `trytond-6.8.3/trytond/ir/lang.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/bg.po` & `trytond-6.8.3/trytond/ir/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/ca.po` & `trytond-6.8.3/trytond/ir/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/cs.po` & `trytond-6.8.3/trytond/ir/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/de.po` & `trytond-6.8.3/trytond/ir/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/es.po` & `trytond-6.8.3/trytond/ir/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/es_419.po` & `trytond-6.8.3/trytond/ir/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/et.po` & `trytond-6.8.3/trytond/ir/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/fa.po` & `trytond-6.8.3/trytond/ir/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/fi.po` & `trytond-6.8.3/trytond/ir/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/fr.po` & `trytond-6.8.3/trytond/ir/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/hu.po` & `trytond-6.8.3/trytond/ir/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/id.po` & `trytond-6.8.3/trytond/ir/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/it.po` & `trytond-6.8.3/trytond/ir/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/lo.po` & `trytond-6.8.3/trytond/ir/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/lt.po` & `trytond-6.8.3/trytond/ir/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/nl.po` & `trytond-6.8.3/trytond/ir/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/pl.po` & `trytond-6.8.3/trytond/ir/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/pt.po` & `trytond-6.8.3/trytond/ir/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/ro.po` & `trytond-6.8.3/trytond/ir/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/ru.po` & `trytond-6.8.3/trytond/ir/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/sl.po` & `trytond-6.8.3/trytond/ir/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/tr.po` & `trytond-6.8.3/trytond/ir/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/uk.po` & `trytond-6.8.3/trytond/ir/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/locale/zh_CN.po` & `trytond-6.8.3/trytond/ir/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/message.py` & `trytond-6.8.3/trytond/ir/message.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/message.xml` & `trytond-6.8.3/trytond/ir/message.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/model.py` & `trytond-6.8.3/trytond/ir/model.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/model.xml` & `trytond-6.8.3/trytond/ir/model.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/module.py` & `trytond-6.8.3/trytond/ir/module.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/module.xml` & `trytond-6.8.3/trytond/ir/module.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/note.py` & `trytond-6.8.3/trytond/ir/note.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/note.xml` & `trytond-6.8.3/trytond/ir/note.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/queue_.py` & `trytond-6.8.3/trytond/ir/queue_.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/resource.py` & `trytond-6.8.3/trytond/ir/resource.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/routes.py` & `trytond-6.8.3/trytond/ir/routes.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/rule.py` & `trytond-6.8.3/trytond/ir/rule.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/rule.xml` & `trytond-6.8.3/trytond/ir/rule.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/sequence.py` & `trytond-6.8.3/trytond/ir/sequence.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/sequence.xml` & `trytond-6.8.3/trytond/ir/sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/session.py` & `trytond-6.8.3/trytond/ir/session.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/translation.py` & `trytond-6.8.3/trytond/ir/translation.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/translation.xml` & `trytond-6.8.3/trytond/ir/translation.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/trigger.py` & `trytond-6.8.3/trytond/ir/trigger.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/trigger.xml` & `trytond-6.8.3/trytond/ir/trigger.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/board.rnc` & `trytond-6.8.3/trytond/ir/ui/board.rnc`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/board.rng` & `trytond-6.8.3/trytond/ir/ui/board.rng`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/calendar.rnc` & `trytond-6.8.3/trytond/ir/ui/calendar.rnc`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/calendar.rng` & `trytond-6.8.3/trytond/ir/ui/calendar.rng`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/form.rnc` & `trytond-6.8.3/trytond/ir/ui/form.rnc`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/form.rng` & `trytond-6.8.3/trytond/ir/ui/form.rng`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/graph.rnc` & `trytond-6.8.3/trytond/ir/ui/graph.rnc`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/graph.rng` & `trytond-6.8.3/trytond/ir/ui/graph.rng`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/icon.py` & `trytond-6.8.3/trytond/ir/ui/icon.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/icon.xml` & `trytond-6.8.3/trytond/ir/ui/icon.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/icons/LICENSE` & `trytond-6.8.3/trytond/ir/ui/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/icons/tryton-settings.svg` & `trytond-6.8.3/trytond/ir/ui/icons/tryton-settings.svg`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/menu.py` & `trytond-6.8.3/trytond/ir/ui/menu.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/menu.xml` & `trytond-6.8.3/trytond/ir/ui/menu.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/tree.rnc` & `trytond-6.8.3/trytond/ir/ui/tree.rnc`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/tree.rng` & `trytond-6.8.3/trytond/ir/ui/tree.rng`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/ui.xml` & `trytond-6.8.3/trytond/ir/ui/ui.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/view.py` & `trytond-6.8.3/trytond/ir/ui/view.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/ui/view.xml` & `trytond-6.8.3/trytond/ir/ui/view.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/action_act_window_domain_form.xml` & `trytond-6.8.3/trytond/ir/view/action_act_window_domain_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/action_act_window_form.xml` & `trytond-6.8.3/trytond/ir/view/action_act_window_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/action_form.xml` & `trytond-6.8.3/trytond/ir/view/action_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/action_report_form.xml` & `trytond-6.8.3/trytond/ir/view/action_report_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/action_url_form.xml` & `trytond-6.8.3/trytond/ir/view/action_url_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/action_wizard_form.xml` & `trytond-6.8.3/trytond/ir/view/action_wizard_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/attachment_form.xml` & `trytond-6.8.3/trytond/ir/view/attachment_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/attachment_list.xml` & `trytond-6.8.3/trytond/ir/view/attachment_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/cron_form.xml` & `trytond-6.8.3/trytond/ir/view/cron_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/cron_list.xml` & `trytond-6.8.3/trytond/ir/view/cron_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/email_form.xml` & `trytond-6.8.3/trytond/ir/view/email_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/email_template_form.xml` & `trytond-6.8.3/trytond/ir/view/email_template_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/error_form.xml` & `trytond-6.8.3/trytond/ir/view/error_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/lang_form.xml` & `trytond-6.8.3/trytond/ir/view/lang_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/model_access_form.xml` & `trytond-6.8.3/trytond/ir/view/model_access_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/model_button_form.xml` & `trytond-6.8.3/trytond/ir/view/model_button_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/model_button_rule_form.xml` & `trytond-6.8.3/trytond/ir/view/model_button_rule_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/model_data_form.xml` & `trytond-6.8.3/trytond/ir/view/model_data_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/model_field_access_form.xml` & `trytond-6.8.3/trytond/ir/view/model_field_access_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/model_field_form.xml` & `trytond-6.8.3/trytond/ir/view/model_field_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/model_form.xml` & `trytond-6.8.3/trytond/ir/view/model_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/module_activate_upgrade_start_form.xml` & `trytond-6.8.3/trytond/ir/view/module_activate_upgrade_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/module_form.xml` & `trytond-6.8.3/trytond/ir/view/module_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/module_list.xml` & `trytond-6.8.3/trytond/ir/view/module_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/note_form.xml` & `trytond-6.8.3/trytond/ir/view/note_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/note_list.xml` & `trytond-6.8.3/trytond/ir/view/note_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/rule_group_form.xml` & `trytond-6.8.3/trytond/ir/view/rule_group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/sequence_form.xml` & `trytond-6.8.3/trytond/ir/view/sequence_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/translation_form.xml` & `trytond-6.8.3/trytond/ir/view/translation_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/translation_list.xml` & `trytond-6.8.3/trytond/ir/view/translation_list.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/trigger_form.xml` & `trytond-6.8.3/trytond/ir/view/trigger_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/ui_menu_form.xml` & `trytond-6.8.3/trytond/ir/view/ui_menu_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/ui_view_form.xml` & `trytond-6.8.3/trytond/ir/view/ui_view_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/ir/view/ui_view_tree_state_form.xml` & `trytond-6.8.3/trytond/ir/view/ui_view_tree_state_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/__init__.py` & `trytond-6.8.3/trytond/model/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/active.py` & `trytond-6.8.3/trytond/model/active.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/avatar.py` & `trytond-6.8.3/trytond/model/avatar.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/descriptors.py` & `trytond-6.8.3/trytond/model/descriptors.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/dictschema.py` & `trytond-6.8.3/trytond/model/dictschema.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         help=lazy_gettext('ir.msg_dict_schema_selection_sorted_help'))
     help_selection = fields.Text(
         lazy_gettext('ir.msg_dict_schema_help_selection'), translate=True,
         states={
             'invisible': ~Eval('type_').in_(['selection', 'multiselection']),
             },
         depends=['type_'],
-        help=lazy_gettext('is.msg_dict_schema_help_selection_help'))
+        help=lazy_gettext('ir.msg_dict_schema_help_selection_help'))
     selection_json = fields.Function(fields.Char(
             lazy_gettext('ir.msg_dict_schema_selection_json'),
             states={
                 'invisible': ~Eval('type_').in_(
                     ['selection', 'multiselection']),
                 },
             depends=['type_']), 'get_selection_json')
```

### Comparing `trytond-6.8.2/trytond/model/digits.py` & `trytond-6.8.3/trytond/model/digits.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/exceptions.py` & `trytond-6.8.3/trytond/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/__init__.py` & `trytond-6.8.3/trytond/model/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/binary.py` & `trytond-6.8.3/trytond/model/fields/binary.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/boolean.py` & `trytond-6.8.3/trytond/model/fields/boolean.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/char.py` & `trytond-6.8.3/trytond/model/fields/char.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/date.py` & `trytond-6.8.3/trytond/model/fields/date.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/dict.py` & `trytond-6.8.3/trytond/model/fields/dict.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/field.py` & `trytond-6.8.3/trytond/model/fields/field.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/float.py` & `trytond-6.8.3/trytond/model/fields/float.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/function.py` & `trytond-6.8.3/trytond/model/fields/function.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/many2many.py` & `trytond-6.8.3/trytond/model/fields/many2many.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/many2one.py` & `trytond-6.8.3/trytond/model/fields/many2one.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/multiselection.py` & `trytond-6.8.3/trytond/model/fields/multiselection.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/numeric.py` & `trytond-6.8.3/trytond/model/fields/numeric.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/one2many.py` & `trytond-6.8.3/trytond/model/fields/one2many.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/one2one.py` & `trytond-6.8.3/trytond/model/fields/one2one.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/reference.py` & `trytond-6.8.3/trytond/model/fields/reference.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/selection.py` & `trytond-6.8.3/trytond/model/fields/selection.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/fields/text.py` & `trytond-6.8.3/trytond/model/fields/text.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/match.py` & `trytond-6.8.3/trytond/model/match.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/model.py` & `trytond-6.8.3/trytond/model/model.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/modelsingleton.py` & `trytond-6.8.3/trytond/model/modelsingleton.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/modelsql.py` & `trytond-6.8.3/trytond/model/modelsql.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,21 @@
     def __eq__(self, other):
         return (
             str(self.table) == str(other.table)
             and len(self.expressions) == len(other.expressions)
             and all((str(c), u) == (str(oc), ou)
                 for (c, u), (oc, ou) in zip(
                     self.expressions, other.expressions))
-            and self.options == other.options)
+            and self._options_cmp == other._options_cmp)
+
+    @property
+    def _options_cmp(self):
+        def _format(value):
+            return str(value) if isinstance(value, Expression) else value
+        return {k: _format(v) for k, v in self.options.items()}
 
     class Unaccent(Expression):
         "Unaccent function if database support for index"
         __slots__ = ('_expression',)
 
         def __init__(self, expression):
             self._expression = expression
@@ -1022,15 +1028,15 @@
                     'EPOCH', Coalesce(table.write_date, table.create_date)
                     ).cast(sql_type).as_('_timestamp')
 
         if ('write_date' not in fields_names
                 and columns.keys() == {'write_date'}):
             columns.pop('write_date')
             extra_fields.discard('write_date')
-        if columns:
+        if columns or domain:
             if 'id' not in fields_names:
                 columns['id'] = table.id.as_('id')
 
             tables = {None: (table, None)}
             if domain:
                 tables, dom_exp = cls.search_domain(
                     domain, active_test=False, tables=tables)
```

### Comparing `trytond-6.8.2/trytond/model/modelstorage.py` & `trytond-6.8.3/trytond/model/modelstorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -733,18 +733,19 @@
                     if child_fields_names in done:
                         break
                     done.append(child_fields_names)
                     for child_record in value:
                         child_lines = ModelStorage.__export_row(child_record,
                                 child_fields_names)
                         if first:
-                            for child_fpos in range(len(fields_names)):
-                                if child_lines and child_lines[0][child_fpos]:
-                                    data[child_fpos] = \
-                                        child_lines[0][child_fpos]
+                            if child_lines:
+                                for child_fpos in range(len(fields_names)):
+                                    if child_fields_names[child_fpos]:
+                                        data[child_fpos] = (
+                                            child_lines[0][child_fpos])
                             lines += child_lines[1:]
                             first = False
                         else:
                             lines += child_lines
                     break
                 i += 1
             if i == len(fields_tree):
```

### Comparing `trytond-6.8.2/trytond/model/modelview.py` & `trytond-6.8.3/trytond/model/modelview.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/multivalue.py` & `trytond-6.8.3/trytond/model/multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/order.py` & `trytond-6.8.3/trytond/model/order.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/symbol.py` & `trytond-6.8.3/trytond/model/symbol.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/tree.py` & `trytond-6.8.3/trytond/model/tree.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/union.py` & `trytond-6.8.3/trytond/model/union.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/model/workflow.py` & `trytond-6.8.3/trytond/model/workflow.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/modules/__init__.py` & `trytond-6.8.3/trytond/modules/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,19 +270,22 @@
                     cursor.execute(*ir_module.insert(
                             [ir_module.create_uid, ir_module.create_date,
                                 ir_module.name, ir_module.state],
                             [[0, CurrentTimestamp(), module, 'activated'],
                                 ]))
                 module2state[module] = 'activated'
 
-            # Clear cache from old data cached before transaction started
-            Cache.clear_all()
-            # Avoid clearing cache to prevent dead lock on ir.cache table
+            # Rollback cache changes to prevent dead lock on ir.cache table
             Cache.rollback(transaction)
             transaction.commit()
+            # Clear the cache so that the transaction has an empty cache
+            # from now on. The cache is not empty because the rollback might
+            # have filled it with old data from before the transaction
+            # started.
+            Cache.clear_all()
             # Clear transaction cache to update default_factory
             transaction.cache.clear()
 
         if not update:
             pool.setup()
         else:
             # Remove unknown models and fields
```

### Comparing `trytond-6.8.2/trytond/pool.py` & `trytond-6.8.3/trytond/pool.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/protocols/dispatcher.py` & `trytond-6.8.3/trytond/protocols/dispatcher.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/protocols/jsonrpc.py` & `trytond-6.8.3/trytond/protocols/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/protocols/wrappers.py` & `trytond-6.8.3/trytond/protocols/wrappers.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/protocols/xmlrpc.py` & `trytond-6.8.3/trytond/protocols/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/pyson.py` & `trytond-6.8.3/trytond/pyson.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/report/report.py` & `trytond-6.8.3/trytond/report/report.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/__init__.py` & `trytond-6.8.3/trytond/res/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/email_reset_password.html` & `trytond-6.8.3/trytond/res/email_reset_password.html`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/group.py` & `trytond-6.8.3/trytond/res/group.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/group.xml` & `trytond-6.8.3/trytond/res/group.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/ir.py` & `trytond-6.8.3/trytond/res/ir.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/ir.xml` & `trytond-6.8.3/trytond/res/ir.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/bg.po` & `trytond-6.8.3/trytond/res/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/ca.po` & `trytond-6.8.3/trytond/res/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/cs.po` & `trytond-6.8.3/trytond/res/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/de.po` & `trytond-6.8.3/trytond/res/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/es.po` & `trytond-6.8.3/trytond/res/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/es_419.po` & `trytond-6.8.3/trytond/res/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/et.po` & `trytond-6.8.3/trytond/res/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/fa.po` & `trytond-6.8.3/trytond/res/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/fi.po` & `trytond-6.8.3/trytond/res/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/fr.po` & `trytond-6.8.3/trytond/res/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/hu.po` & `trytond-6.8.3/trytond/res/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/id.po` & `trytond-6.8.3/trytond/res/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/it.po` & `trytond-6.8.3/trytond/res/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/lo.po` & `trytond-6.8.3/trytond/res/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/lt.po` & `trytond-6.8.3/trytond/res/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/nl.po` & `trytond-6.8.3/trytond/res/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/pl.po` & `trytond-6.8.3/trytond/res/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/pt.po` & `trytond-6.8.3/trytond/res/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/ro.po` & `trytond-6.8.3/trytond/res/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/ru.po` & `trytond-6.8.3/trytond/res/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/sl.po` & `trytond-6.8.3/trytond/res/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/tr.po` & `trytond-6.8.3/trytond/res/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/uk.po` & `trytond-6.8.3/trytond/res/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/locale/zh_CN.po` & `trytond-6.8.3/trytond/res/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/message.xml` & `trytond-6.8.3/trytond/res/message.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/routes.py` & `trytond-6.8.3/trytond/res/routes.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/user.py` & `trytond-6.8.3/trytond/res/user.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/user.xml` & `trytond-6.8.3/trytond/res/user.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/view/group_form.xml` & `trytond-6.8.3/trytond/res/view/group_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/view/user_application_form.xml` & `trytond-6.8.3/trytond/res/view/user_application_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/view/user_config_start_form.xml` & `trytond-6.8.3/trytond/res/view/user_config_start_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/view/user_form.xml` & `trytond-6.8.3/trytond/res/view/user_form.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/res/view/user_form_preferences.xml` & `trytond-6.8.3/trytond/res/view/user_form_preferences.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/rpc.py` & `trytond-6.8.3/trytond/rpc.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/security.py` & `trytond-6.8.3/trytond/security.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/sendmail.py` & `trytond-6.8.3/trytond/sendmail.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/status.py` & `trytond-6.8.3/trytond/status.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/__init__.py` & `trytond-6.8.3/trytond/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/access.py` & `trytond-6.8.3/trytond/tests/access.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/copy_.py` & `trytond-6.8.3/trytond/tests/copy_.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/export_data.py` & `trytond-6.8.3/trytond/tests/export_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from trytond.pool import Pool, PoolMeta
 
 
 class ExportDataTarget(ModelSQL):
     "Export Data Target"
     __name__ = 'test.export_data.target'
     name = fields.Char('Name')
+    value = fields.Float("Value")
 
 
 class ExportData(ModelSQL):
     "Export Data"
     __name__ = 'test.export_data'
     boolean = fields.Boolean('Boolean')
     integer = fields.Integer('Integer')
```

### Comparing `trytond-6.8.2/trytond/tests/field_binary.py` & `trytond-6.8.3/trytond/tests/field_binary.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_boolean.py` & `trytond-6.8.3/trytond/tests/field_boolean.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_char.py` & `trytond-6.8.3/trytond/tests/field_char.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_context.py` & `trytond-6.8.3/trytond/tests/field_context.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_date.py` & `trytond-6.8.3/trytond/tests/field_date.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_datetime.py` & `trytond-6.8.3/trytond/tests/field_datetime.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_dict.py` & `trytond-6.8.3/trytond/tests/field_dict.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_float.py` & `trytond-6.8.3/trytond/tests/field_float.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_function.py` & `trytond-6.8.3/trytond/tests/field_function.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_integer.py` & `trytond-6.8.3/trytond/tests/field_integer.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_many2many.py` & `trytond-6.8.3/trytond/tests/field_many2many.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_many2one.py` & `trytond-6.8.3/trytond/tests/field_many2one.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_multiselection.py` & `trytond-6.8.3/trytond/tests/field_multiselection.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_numeric.py` & `trytond-6.8.3/trytond/tests/field_numeric.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_one2many.py` & `trytond-6.8.3/trytond/tests/field_one2many.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_one2one.py` & `trytond-6.8.3/trytond/tests/field_one2one.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_reference.py` & `trytond-6.8.3/trytond/tests/field_reference.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_selection.py` & `trytond-6.8.3/trytond/tests/field_selection.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_text.py` & `trytond-6.8.3/trytond/tests/field_text.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_time.py` & `trytond-6.8.3/trytond/tests/field_time.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/field_timedelta.py` & `trytond-6.8.3/trytond/tests/field_timedelta.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/history.py` & `trytond-6.8.3/trytond/tests/history.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/import_data.py` & `trytond-6.8.3/trytond/tests/import_data.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/import_data.xml` & `trytond-6.8.3/trytond/tests/import_data.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/mixin.py` & `trytond-6.8.3/trytond/tests/mixin.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/model.py` & `trytond-6.8.3/trytond/tests/model.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/model_log.py` & `trytond-6.8.3/trytond/tests/model_log.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/modelsql.py` & `trytond-6.8.3/trytond/tests/modelsql.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/modelstorage.py` & `trytond-6.8.3/trytond/tests/modelstorage.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/modelview.py` & `trytond-6.8.3/trytond/tests/modelview.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/modelview.xml` & `trytond-6.8.3/trytond/tests/modelview.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/mptt.py` & `trytond-6.8.3/trytond/tests/mptt.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/multivalue.py` & `trytond-6.8.3/trytond/tests/multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/path.py` & `trytond-6.8.3/trytond/tests/path.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/resource.py` & `trytond-6.8.3/trytond/tests/resource.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/rule.py` & `trytond-6.8.3/trytond/tests/rule.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/sequence.xml` & `trytond-6.8.3/trytond/tests/sequence.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_access.py` & `trytond-6.8.3/trytond/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_backend.py` & `trytond-6.8.3/trytond/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_bus.py` & `trytond-6.8.3/trytond/tests/test_bus.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_cache.py` & `trytond-6.8.3/trytond/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_copy.py` & `trytond-6.8.3/trytond/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_exportdata.py` & `trytond-6.8.3/trytond/tests/test_exportdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,14 +351,34 @@
 
         self.assertEqual(
             ExportData.export_data([export1, export2], ['id',
                     'one2many/name']),
             [[export1.id, 'Target 1'], ['', 'Target 2'], [export2.id, '']])
 
     @with_transaction()
+    def test_one2many_empty_value(self):
+        "Test export_data one2many with first child with 0 value"
+        pool = Pool()
+        ExportData = pool.get('test.export_data')
+        ExportDataTarget = pool.get('test.export_data.target')
+
+        export, = ExportData.create([{}])
+        ExportDataTarget.create([{
+                    'value': 0,
+                    'one2many': export.id,
+                    }, {
+                    'value': 42,
+                    'one2many': export.id,
+                    }])
+
+        self.assertEqual(
+            ExportData.export_data([export], ['id', 'one2many/value']),
+            [[export.id, 0], ['', 42]])
+
+    @with_transaction()
     def test_reference(self):
         'Test export_data reference'
         pool = Pool()
         ExportData = pool.get('test.export_data')
         ExportDataTarget = pool.get('test.export_data.target')
 
         target1, = ExportDataTarget.create([{'name': "Target test"}])
```

### Comparing `trytond-6.8.2/trytond/tests/test_field_binary.py` & `trytond-6.8.3/trytond/tests/test_field_binary.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_boolean.py` & `trytond-6.8.3/trytond/tests/test_field_boolean.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_char.py` & `trytond-6.8.3/trytond/tests/test_field_char.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_context.py` & `trytond-6.8.3/trytond/tests/test_field_context.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_date.py` & `trytond-6.8.3/trytond/tests/test_field_date.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_datetime.py` & `trytond-6.8.3/trytond/tests/test_field_datetime.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_depends.py` & `trytond-6.8.3/trytond/tests/test_field_depends.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_dict.py` & `trytond-6.8.3/trytond/tests/test_field_dict.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_float.py` & `trytond-6.8.3/trytond/tests/test_field_float.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_function.py` & `trytond-6.8.3/trytond/tests/test_field_function.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_integer.py` & `trytond-6.8.3/trytond/tests/test_field_integer.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_many2many.py` & `trytond-6.8.3/trytond/tests/test_field_many2many.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_many2one.py` & `trytond-6.8.3/trytond/tests/test_field_many2one.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_multiselection.py` & `trytond-6.8.3/trytond/tests/test_field_multiselection.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_numeric.py` & `trytond-6.8.3/trytond/tests/test_field_numeric.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_one2many.py` & `trytond-6.8.3/trytond/tests/test_field_one2many.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_one2one.py` & `trytond-6.8.3/trytond/tests/test_field_one2one.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_reference.py` & `trytond-6.8.3/trytond/tests/test_field_reference.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_selection.py` & `trytond-6.8.3/trytond/tests/test_field_selection.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_text.py` & `trytond-6.8.3/trytond/tests/test_field_text.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_time.py` & `trytond-6.8.3/trytond/tests/test_field_time.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_field_timedelta.py` & `trytond-6.8.3/trytond/tests/test_field_timedelta.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_filestore.py` & `trytond-6.8.3/trytond/tests/test_filestore.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_history.py` & `trytond-6.8.3/trytond/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_i18n.py` & `trytond-6.8.3/trytond/tests/test_i18n.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_importdata.py` & `trytond-6.8.3/trytond/tests/test_importdata.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_ir.py` & `trytond-6.8.3/trytond/tests/test_ir.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_mixins.py` & `trytond-6.8.3/trytond/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_model.py` & `trytond-6.8.3/trytond/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_model_index.py` & `trytond-6.8.3/trytond/tests/test_model_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         table2 = Table('test')
         index2 = Index(
             table2,
             (table2.name, Index.Equality(order='DESC')),
             (table2.amount, Index.Range()),
             where=table2.amount == 'foo')
 
-        self.assertEqual(index1, index2)
+        self.assertNotEqual(index1, index2)
 
     def test_index_inequality_option_param(self):
         "Test Index inequality on option param"
         table1 = Table('test')
         index1 = Index(
             table1,
             (table1.name, Index.Equality(order='DESC')),
```

### Comparing `trytond-6.8.2/trytond/tests/test_model_log.py` & `trytond-6.8.3/trytond/tests/test_model_log.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_modelsingleton.py` & `trytond-6.8.3/trytond/tests/test_modelsingleton.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_modelsql.py` & `trytond-6.8.3/trytond/tests/test_modelsql.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_modelstorage.py` & `trytond-6.8.3/trytond/tests/test_modelstorage.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_modelview.py` & `trytond-6.8.3/trytond/tests/test_modelview.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_mptt.py` & `trytond-6.8.3/trytond/tests/test_mptt.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_multivalue.py` & `trytond-6.8.3/trytond/tests/test_multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_order.py` & `trytond-6.8.3/trytond/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_path.py` & `trytond-6.8.3/trytond/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_protocols.py` & `trytond-6.8.3/trytond/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_pyson.py` & `trytond-6.8.3/trytond/tests/test_pyson.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_report.py` & `trytond-6.8.3/trytond/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_res.py` & `trytond-6.8.3/trytond/tests/test_res.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_resource.py` & `trytond-6.8.3/trytond/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_routes.py` & `trytond-6.8.3/trytond/tests/test_routes.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_rpc.py` & `trytond-6.8.3/trytond/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_rule.py` & `trytond-6.8.3/trytond/tests/test_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,14 +316,41 @@
                     }])
         test, = TestRule.create([{'field': 'foo'}])
 
         with self.assertRaisesRegex(AccessError, "Field different from foo"):
             TestRule.read([test.id], ['field'])
 
     @with_transaction(context=_context)
+    def test_perm_read_with_rule_no_sql_type_fail(self):
+        "Test read with rule fail and without SQL type"
+        pool = Pool()
+        TestRule = pool.get('test.rule')
+        RuleGroup = pool.get('ir.rule.group')
+        Model = pool.get('ir.model')
+
+        model, = Model.search([('model', '=', 'test.rule')])
+        rule_group, = RuleGroup.create([{
+                    'name': "Field different from foo",
+                    'model': model.id,
+                    'global_p': True,
+                    'perm_read': True,
+                    'perm_create': False,
+                    'perm_write': False,
+                    'perm_delete': False,
+                    'rules': [('create', [{
+                                    'domain': json.dumps(
+                                        [('field', '!=', 'foo')]),
+                                    }])],
+                    }])
+        test, = TestRule.create([{'field': 'foo'}])
+
+        with self.assertRaisesRegex(AccessError, "Field different from foo"):
+            TestRule.read([test.id], ['rec_name'])
+
+    @with_transaction(context=_context)
     def test_search_without_rule(self):
         "Test search without rule"
         pool = Pool()
         TestRule = pool.get('test.rule')
 
         test, = TestRule.create([{'field': 'foo'}])
```

### Comparing `trytond-6.8.2/trytond/tests/test_sendmail.py` & `trytond-6.8.3/trytond/tests/test_sendmail.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_sequence.py` & `trytond-6.8.3/trytond/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_tools.py` & `trytond-6.8.3/trytond/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_transaction.py` & `trytond-6.8.3/trytond/tests/test_transaction.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_tree.py` & `trytond-6.8.3/trytond/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_trigger.py` & `trytond-6.8.3/trytond/tests/test_trigger.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_tryton.py` & `trytond-6.8.3/trytond/tests/test_tryton.py`

 * *Files 0% similar despite different names*

```diff
@@ -745,14 +745,16 @@
                     self.assertTrue(all(len(v) == 2 for v in selection_values),
                         msg='Invalid selection values "%(values)s" on field '
                         '"%(field)s" of model "%(model)s"' % {
                             'values': selection_values,
                             'field': field_name,
                             'model': model.__name__,
                             })
+                    if field._type == 'multiselection':
+                        self.assertNotIn(None, dict(selection_values).keys())
 
     @with_transaction()
     def test_function_fields(self):
         "Test function fields methods"
         for mname, model in Pool().iterobject():
             if not isregisteredby(model, self.module):
                 continue
```

### Comparing `trytond-6.8.2/trytond/tests/test_union.py` & `trytond-6.8.3/trytond/tests/test_union.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_user.py` & `trytond-6.8.3/trytond/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_wizard.py` & `trytond-6.8.3/trytond/tests/test_wizard.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_workflow.py` & `trytond-6.8.3/trytond/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/test_wsgi.py` & `trytond-6.8.3/trytond/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/tools.py` & `trytond-6.8.3/trytond/tests/tools.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/tree.py` & `trytond-6.8.3/trytond/tests/tree.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/trigger.py` & `trytond-6.8.3/trytond/tests/trigger.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/wizard.py` & `trytond-6.8.3/trytond/tests/wizard.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/wizard.xml` & `trytond-6.8.3/trytond/tests/wizard.xml`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tests/workflow.py` & `trytond-6.8.3/trytond/tests/workflow.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tools/__init__.py` & `trytond-6.8.3/trytond/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tools/barcode.py` & `trytond-6.8.3/trytond/tools/barcode.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tools/decimal_.py` & `trytond-6.8.3/trytond/tools/decimal_.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tools/domain_inversion.py` & `trytond-6.8.3/trytond/tools/domain_inversion.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tools/email_.py` & `trytond-6.8.3/trytond/tools/email_.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tools/immutabledict.py` & `trytond-6.8.3/trytond/tools/immutabledict.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tools/misc.py` & `trytond-6.8.3/trytond/tools/misc.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tools/multivalue.py` & `trytond-6.8.3/trytond/tools/multivalue.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tools/qrcode.py` & `trytond-6.8.3/trytond/tools/qrcode.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tools/singleton.py` & `trytond-6.8.3/trytond/tools/singleton.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tools/string_.py` & `trytond-6.8.3/trytond/tools/string_.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tools/timezone.py` & `trytond-6.8.3/trytond/tools/timezone.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/transaction.py` & `trytond-6.8.3/trytond/transaction.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tryton.rnc` & `trytond-6.8.3/trytond/tryton.rnc`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/tryton.rng` & `trytond-6.8.3/trytond/tryton.rng`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/url.py` & `trytond-6.8.3/trytond/url.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/wizard/wizard.py` & `trytond-6.8.3/trytond/wizard/wizard.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/worker.py` & `trytond-6.8.3/trytond/worker.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond/wsgi.py` & `trytond-6.8.3/trytond/wsgi.py`

 * *Files identical despite different names*

### Comparing `trytond-6.8.2/trytond.egg-info/PKG-INFO` & `trytond-6.8.3/trytond.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trytond
-Version: 6.8.2
+Version: 6.8.3
 Summary: Tryton server
 Home-page: http://www.tryton.org/
 Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
```

### Comparing `trytond-6.8.2/trytond.egg-info/SOURCES.txt` & `trytond-6.8.3/trytond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

