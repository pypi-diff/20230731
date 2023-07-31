# Comparing `tmp/femto-admin-0.1.2.tar.gz` & `tmp/femto-admin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femto-admin-0.1.2.tar", last modified: Fri Jul 28 08:07:03 2023, max compression
+gzip compressed data, was "femto-admin-0.2.0.tar", last modified: Mon Jul 31 08:45:14 2023, max compression
```

## Comparing `femto-admin-0.1.2.tar` & `femto-admin-0.2.0.tar`

### file list

```diff
@@ -1,79 +1,84 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.126054 femto-admin-0.1.2/
--rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 femto-admin-0.1.2/LICENSE
--rw-r--r--   0 sol        (501) staff       (20)       17 2023-07-20 14:49:50.000000 femto-admin-0.1.2/MANIFEST.in
--rw-r--r--   0 sol        (501) staff       (20)     2062 2023-07-28 08:07:03.125804 femto-admin-0.1.2/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1499 2023-07-20 23:49:02.000000 femto-admin-0.1.2/README.md
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.097149 femto-admin-0.1.2/femto_admin/
--rw-r--r--   0 sol        (501) staff       (20)       58 2023-07-28 08:06:43.000000 femto-admin-0.1.2/femto_admin/__init__.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.101303 femto-admin-0.1.2/femto_admin/__pycache__/
--rw-r--r--   0 sol        (501) staff       (20)      247 2023-07-27 11:07:52.000000 femto-admin-0.1.2/femto_admin/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 sol        (501) staff       (20)     7386 2023-07-27 11:12:47.000000 femto-admin-0.1.2/femto_admin/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 sol        (501) staff       (20)      695 2023-07-27 11:45:41.000000 femto-admin-0.1.2/femto_admin/__pycache__/consts.cpython-311.pyc
--rw-r--r--   0 sol        (501) staff       (20)     4441 2023-07-27 21:02:06.000000 femto-admin-0.1.2/femto_admin/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 sol        (501) staff       (20)     3691 2023-07-27 11:12:33.000000 femto-admin-0.1.2/femto_admin/admin.py
--rw-r--r--   0 sol        (501) staff       (20)      225 2023-07-27 11:38:27.000000 femto-admin-0.1.2/femto_admin/consts.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.092930 femto-admin-0.1.2/femto_admin/statics/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.101953 femto-admin-0.1.2/femto_admin/statics/js/
--rw-r--r--   0 sol        (501) staff       (20)     1251 2023-07-27 20:59:11.000000 femto-admin-0.1.2/femto_admin/statics/js/polygon.js
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.102194 femto-admin-0.1.2/femto_admin/statics/placeholders/
--rw-r--r--   0 sol        (501) staff       (20)    16958 2023-06-23 13:05:44.000000 femto-admin-0.1.2/femto_admin/statics/placeholders/favicon.ico
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.102461 femto-admin-0.1.2/femto_admin/statics/placeholders/logo/
--rw-r--r--   0 sol        (501) staff       (20)      418 2023-06-23 17:08:58.000000 femto-admin-0.1.2/femto_admin/statics/placeholders/logo/logo-white.svg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.102691 femto-admin-0.1.2/femto_admin/statics/placeholders/users/
--rw-r--r--   0 sol        (501) staff       (20)     2094 2023-05-04 14:33:48.000000 femto-admin-0.1.2/femto_admin/statics/placeholders/users/admin.jpg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.093441 femto-admin-0.1.2/femto_admin/statics/vendor/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.093208 femto-admin-0.1.2/femto_admin/statics/vendor/DataTables/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.103162 femto-admin-0.1.2/femto_admin/statics/vendor/DataTables/css/
--rw-r--r--   0 sol        (501) staff       (20)    13550 2023-07-04 13:18:30.000000 femto-admin-0.1.2/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css
--rw-r--r--   0 sol        (501) staff       (20)    11981 2023-07-04 13:18:30.000000 femto-admin-0.1.2/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.105386 femto-admin-0.1.2/femto_admin/statics/vendor/DataTables/js/
--rw-r--r--   0 sol        (501) staff       (20)     5265 2023-07-04 13:18:32.000000 femto-admin-0.1.2/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js
--rw-r--r--   0 sol        (501) staff       (20)     2353 2023-07-04 13:18:32.000000 femto-admin-0.1.2/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js
--rw-r--r--   0 sol        (501) staff       (20)   457166 2023-07-04 13:18:32.000000 femto-admin-0.1.2/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js
--rw-r--r--   0 sol        (501) staff       (20)    87093 2023-07-04 13:18:32.000000 femto-admin-0.1.2/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.107080 femto-admin-0.1.2/femto_admin/statics/vendor/jQuery/
--rw-r--r--   0 sol        (501) staff       (20)   284996 2023-07-04 13:23:04.000000 femto-admin-0.1.2/femto_admin/statics/vendor/jQuery/jquery.js
--rw-r--r--   0 sol        (501) staff       (20)    87462 2023-07-04 13:23:04.000000 femto-admin-0.1.2/femto_admin/statics/vendor/jQuery/jquery.min.js
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.093635 femto-admin-0.1.2/femto_admin/statics/vendor/tabler/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.109113 femto-admin-0.1.2/femto_admin/statics/vendor/tabler/css/
--rw-r--r--   0 sol        (501) staff       (20)   642443 2023-05-16 21:47:00.000000 femto-admin-0.1.2/femto_admin/statics/vendor/tabler/css/tabler.css
--rw-r--r--   0 sol        (501) staff       (20)   542559 2023-05-16 21:47:00.000000 femto-admin-0.1.2/femto_admin/statics/vendor/tabler/css/tabler.min.css
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.112762 femto-admin-0.1.2/femto_admin/statics/vendor/tabler/js/
--rw-r--r--   0 sol        (501) staff       (20)     1053 2023-07-19 10:42:04.000000 femto-admin-0.1.2/femto_admin/statics/vendor/tabler/js/dark-theme.js
--rw-r--r--   0 sol        (501) staff       (20)      679 2023-05-16 21:47:00.000000 femto-admin-0.1.2/femto_admin/statics/vendor/tabler/js/dark-theme.min.js
--rw-r--r--   0 sol        (501) staff       (20)   265501 2023-05-16 21:47:00.000000 femto-admin-0.1.2/femto_admin/statics/vendor/tabler/js/tabler.js
--rw-r--r--   0 sol        (501) staff       (20)   136567 2023-05-16 21:47:00.000000 femto-admin-0.1.2/femto_admin/statics/vendor/tabler/js/tabler.min.js
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.115175 femto-admin-0.1.2/femto_admin/templates/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.117586 femto-admin-0.1.2/femto_admin/templates/components/
--rw-r--r--   0 sol        (501) staff       (20)      940 2023-07-27 11:12:41.000000 femto-admin-0.1.2/femto_admin/templates/components/footer.html
--rw-r--r--   0 sol        (501) staff       (20)     1421 2023-07-24 10:32:54.000000 femto-admin-0.1.2/femto_admin/templates/components/global_actions.html
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.125236 femto-admin-0.1.2/femto_admin/templates/components/inputs/
--rw-r--r--   0 sol        (501) staff       (20)       83 2023-07-23 20:17:52.000000 femto-admin-0.1.2/femto_admin/templates/components/inputs/_help.html
--rw-r--r--   0 sol        (501) staff       (20)      424 2023-07-03 09:15:48.000000 femto-admin-0.1.2/femto_admin/templates/components/inputs/color.html
--rw-r--r--   0 sol        (501) staff       (20)      380 2023-07-03 09:15:48.000000 femto-admin-0.1.2/femto_admin/templates/components/inputs/date.html
--rw-r--r--   0 sol        (501) staff       (20)     1019 2023-07-03 09:15:48.000000 femto-admin-0.1.2/femto_admin/templates/components/inputs/datetime.html
--rw-r--r--   0 sol        (501) staff       (20)     1794 2023-07-03 09:15:48.000000 femto-admin-0.1.2/femto_admin/templates/components/inputs/editor.html
--rw-r--r--   0 sol        (501) staff       (20)      489 2023-07-03 09:15:48.000000 femto-admin-0.1.2/femto_admin/templates/components/inputs/image.html
--rw-r--r--   0 sol        (501) staff       (20)      253 2023-07-23 20:19:51.000000 femto-admin-0.1.2/femto_admin/templates/components/inputs/input.html
--rw-r--r--   0 sol        (501) staff       (20)     1333 2023-07-03 09:15:48.000000 femto-admin-0.1.2/femto_admin/templates/components/inputs/json.html
--rw-r--r--   0 sol        (501) staff       (20)      857 2023-07-03 09:15:48.000000 femto-admin-0.1.2/femto_admin/templates/components/inputs/many_to_many.html
--rw-r--r--   0 sol        (501) staff       (20)      812 2023-07-27 13:16:40.000000 femto-admin-0.1.2/femto_admin/templates/components/inputs/point.html
--rw-r--r--   0 sol        (501) staff       (20)     1995 2023-07-27 21:21:38.000000 femto-admin-0.1.2/femto_admin/templates/components/inputs/polygon.html
--rw-r--r--   0 sol        (501) staff       (20)      607 2023-07-03 09:15:48.000000 femto-admin-0.1.2/femto_admin/templates/components/inputs/radio.html
--rw-r--r--   0 sol        (501) staff       (20)      459 2023-07-23 20:17:52.000000 femto-admin-0.1.2/femto_admin/templates/components/inputs/select.html
--rw-r--r--   0 sol        (501) staff       (20)      473 2023-07-03 09:15:48.000000 femto-admin-0.1.2/femto_admin/templates/components/inputs/switch.html
--rw-r--r--   0 sol        (501) staff       (20)      415 2023-07-03 09:15:48.000000 femto-admin-0.1.2/femto_admin/templates/components/inputs/textarea.html
--rw-r--r--   0 sol        (501) staff       (20)     2340 2023-07-27 16:29:04.000000 femto-admin-0.1.2/femto_admin/templates/components/modal.html
--rw-r--r--   0 sol        (501) staff       (20)     7353 2023-07-23 19:34:25.000000 femto-admin-0.1.2/femto_admin/templates/components/notofications.html
--rw-r--r--   0 sol        (501) staff       (20)       27 2023-07-20 15:06:51.000000 femto-admin-0.1.2/femto_admin/templates/dashboard.html
--rw-r--r--   0 sol        (501) staff       (20)    11468 2023-07-24 10:30:44.000000 femto-admin-0.1.2/femto_admin/templates/layout.html
--rw-r--r--   0 sol        (501) staff       (20)      899 2023-07-23 20:48:59.000000 femto-admin-0.1.2/femto_admin/templates/table.html
--rw-r--r--   0 sol        (501) staff       (20)     3935 2023-07-27 21:00:52.000000 femto-admin-0.1.2/femto_admin/utils.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-28 08:07:03.098918 femto-admin-0.1.2/femto_admin.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)     2062 2023-07-28 08:07:03.000000 femto-admin-0.1.2/femto_admin.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     2556 2023-07-28 08:07:03.000000 femto-admin-0.1.2/femto_admin.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-28 08:07:03.000000 femto-admin-0.1.2/femto_admin.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       27 2023-07-28 08:07:03.000000 femto-admin-0.1.2/femto_admin.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       12 2023-07-28 08:07:03.000000 femto-admin-0.1.2/femto_admin.egg-info/top_level.txt
--rw-r--r--   0 sol        (501) staff       (20)      766 2023-07-28 08:06:43.000000 femto-admin-0.1.2/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-28 08:07:03.126117 femto-admin-0.1.2/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.955955 femto-admin-0.2.0/
+-rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 femto-admin-0.2.0/LICENSE
+-rw-r--r--   0 sol        (501) staff       (20)       17 2023-07-20 14:49:50.000000 femto-admin-0.2.0/MANIFEST.in
+-rw-r--r--   0 sol        (501) staff       (20)     2062 2023-07-31 08:45:14.955703 femto-admin-0.2.0/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1499 2023-07-20 23:49:02.000000 femto-admin-0.2.0/README.md
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.937372 femto-admin-0.2.0/femto_admin/
+-rw-r--r--   0 sol        (501) staff       (20)       58 2023-07-31 08:44:53.000000 femto-admin-0.2.0/femto_admin/__init__.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.939503 femto-admin-0.2.0/femto_admin/__pycache__/
+-rw-r--r--   0 sol        (501) staff       (20)      247 2023-07-28 12:51:42.000000 femto-admin-0.2.0/femto_admin/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 sol        (501) staff       (20)     7442 2023-07-30 21:44:10.000000 femto-admin-0.2.0/femto_admin/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 sol        (501) staff       (20)      577 2023-07-30 18:31:17.000000 femto-admin-0.2.0/femto_admin/__pycache__/consts.cpython-311.pyc
+-rw-r--r--   0 sol        (501) staff       (20)     7513 2023-07-31 07:02:33.000000 femto-admin-0.2.0/femto_admin/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 sol        (501) staff       (20)     3729 2023-07-30 21:43:45.000000 femto-admin-0.2.0/femto_admin/admin.py
+-rw-r--r--   0 sol        (501) staff       (20)      280 2023-07-30 18:24:21.000000 femto-admin-0.2.0/femto_admin/consts.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.933180 femto-admin-0.2.0/femto_admin/statics/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.939740 femto-admin-0.2.0/femto_admin/statics/js/
+-rw-r--r--   0 sol        (501) staff       (20)     1251 2023-07-27 20:59:11.000000 femto-admin-0.2.0/femto_admin/statics/js/polygon.js
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.939989 femto-admin-0.2.0/femto_admin/statics/placeholders/
+-rw-r--r--   0 sol        (501) staff       (20)    16958 2023-06-23 13:05:44.000000 femto-admin-0.2.0/femto_admin/statics/placeholders/favicon.ico
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.940266 femto-admin-0.2.0/femto_admin/statics/placeholders/logo/
+-rw-r--r--   0 sol        (501) staff       (20)      418 2023-06-23 17:08:58.000000 femto-admin-0.2.0/femto_admin/statics/placeholders/logo/logo-white.svg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.940498 femto-admin-0.2.0/femto_admin/statics/placeholders/users/
+-rw-r--r--   0 sol        (501) staff       (20)     2094 2023-05-04 14:33:48.000000 femto-admin-0.2.0/femto_admin/statics/placeholders/users/admin.jpg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.933717 femto-admin-0.2.0/femto_admin/statics/vendor/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.933469 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.940978 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/css/
+-rw-r--r--   0 sol        (501) staff       (20)    13550 2023-07-04 13:18:30.000000 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css
+-rw-r--r--   0 sol        (501) staff       (20)    11981 2023-07-04 13:18:30.000000 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.942350 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/
+-rw-r--r--   0 sol        (501) staff       (20)     5265 2023-07-04 13:18:32.000000 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js
+-rw-r--r--   0 sol        (501) staff       (20)     2353 2023-07-04 13:18:32.000000 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js
+-rw-r--r--   0 sol        (501) staff       (20)   457166 2023-07-04 13:18:32.000000 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js
+-rw-r--r--   0 sol        (501) staff       (20)    87093 2023-07-04 13:18:32.000000 femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.943234 femto-admin-0.2.0/femto_admin/statics/vendor/jQuery/
+-rw-r--r--   0 sol        (501) staff       (20)   284996 2023-07-04 13:23:04.000000 femto-admin-0.2.0/femto_admin/statics/vendor/jQuery/jquery.js
+-rw-r--r--   0 sol        (501) staff       (20)    87462 2023-07-04 13:23:04.000000 femto-admin-0.2.0/femto_admin/statics/vendor/jQuery/jquery.min.js
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.933917 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.944521 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/css/
+-rw-r--r--   0 sol        (501) staff       (20)   642443 2023-05-16 21:47:00.000000 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/css/tabler.css
+-rw-r--r--   0 sol        (501) staff       (20)   542559 2023-05-16 21:47:00.000000 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/css/tabler.min.css
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.946358 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/
+-rw-r--r--   0 sol        (501) staff       (20)     1053 2023-07-19 10:42:04.000000 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/dark-theme.js
+-rw-r--r--   0 sol        (501) staff       (20)      679 2023-05-16 21:47:00.000000 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/dark-theme.min.js
+-rw-r--r--   0 sol        (501) staff       (20)   265501 2023-05-16 21:47:00.000000 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/tabler.js
+-rw-r--r--   0 sol        (501) staff       (20)   136567 2023-05-16 21:47:00.000000 femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/tabler.min.js
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.947625 femto-admin-0.2.0/femto_admin/templates/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.949047 femto-admin-0.2.0/femto_admin/templates/components/
+-rw-r--r--   0 sol        (501) staff       (20)     4635 2023-07-28 11:21:54.000000 femto-admin-0.2.0/femto_admin/templates/components/aside.html
+-rw-r--r--   0 sol        (501) staff       (20)     1021 2023-07-28 12:11:41.000000 femto-admin-0.2.0/femto_admin/templates/components/footer.html
+-rw-r--r--   0 sol        (501) staff       (20)     1464 2023-07-28 11:25:51.000000 femto-admin-0.2.0/femto_admin/templates/components/global_actions.html
+-rw-r--r--   0 sol        (501) staff       (20)     4458 2023-07-28 11:52:48.000000 femto-admin-0.2.0/femto_admin/templates/components/header.html
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.954979 femto-admin-0.2.0/femto_admin/templates/components/inputs/
+-rw-r--r--   0 sol        (501) staff       (20)       83 2023-07-23 20:17:52.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/_help.html
+-rw-r--r--   0 sol        (501) staff       (20)      472 2023-07-31 08:22:43.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/checkbox.html
+-rw-r--r--   0 sol        (501) staff       (20)      579 2023-07-30 20:21:41.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/collection.html
+-rw-r--r--   0 sol        (501) staff       (20)      424 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/color.html
+-rw-r--r--   0 sol        (501) staff       (20)      380 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/date.html
+-rw-r--r--   0 sol        (501) staff       (20)     1019 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/datetime.html
+-rw-r--r--   0 sol        (501) staff       (20)     1794 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/editor.html
+-rw-r--r--   0 sol        (501) staff       (20)      489 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/image.html
+-rw-r--r--   0 sol        (501) staff       (20)      359 2023-07-30 20:17:37.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/input.html
+-rw-r--r--   0 sol        (501) staff       (20)     1333 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/json.html
+-rw-r--r--   0 sol        (501) staff       (20)     1968 2023-07-30 19:53:21.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/list.html
+-rw-r--r--   0 sol        (501) staff       (20)      857 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/many_to_many.html
+-rw-r--r--   0 sol        (501) staff       (20)      607 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/radio.html
+-rw-r--r--   0 sol        (501) staff       (20)      781 2023-07-28 14:45:42.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/range.html
+-rw-r--r--   0 sol        (501) staff       (20)      404 2023-07-28 15:47:47.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/select.html
+-rw-r--r--   0 sol        (501) staff       (20)      415 2023-07-03 09:15:48.000000 femto-admin-0.2.0/femto_admin/templates/components/inputs/textarea.html
+-rw-r--r--   0 sol        (501) staff       (20)     2379 2023-07-31 08:19:31.000000 femto-admin-0.2.0/femto_admin/templates/components/modal.html
+-rw-r--r--   0 sol        (501) staff       (20)     7353 2023-07-23 19:34:25.000000 femto-admin-0.2.0/femto_admin/templates/components/notofications.html
+-rw-r--r--   0 sol        (501) staff       (20)       27 2023-07-20 15:06:51.000000 femto-admin-0.2.0/femto_admin/templates/dashboard.html
+-rw-r--r--   0 sol        (501) staff       (20)      132 2023-07-28 11:13:54.000000 femto-admin-0.2.0/femto_admin/templates/index.html
+-rw-r--r--   0 sol        (501) staff       (20)     2073 2023-07-28 11:32:50.000000 femto-admin-0.2.0/femto_admin/templates/layout.html
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.955429 femto-admin-0.2.0/femto_admin/templates/views/
+-rw-r--r--   0 sol        (501) staff       (20)      918 2023-07-28 11:12:19.000000 femto-admin-0.2.0/femto_admin/templates/views/table.html
+-rw-r--r--   0 sol        (501) staff       (20)     5395 2023-07-31 07:02:16.000000 femto-admin-0.2.0/femto_admin/utils.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:45:14.938549 femto-admin-0.2.0/femto_admin.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)     2062 2023-07-31 08:45:14.000000 femto-admin-0.2.0/femto_admin.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     2739 2023-07-31 08:45:14.000000 femto-admin-0.2.0/femto_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-31 08:45:14.000000 femto-admin-0.2.0/femto_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       27 2023-07-31 08:45:14.000000 femto-admin-0.2.0/femto_admin.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       12 2023-07-31 08:45:14.000000 femto-admin-0.2.0/femto_admin.egg-info/top_level.txt
+-rw-r--r--   0 sol        (501) staff       (20)      766 2023-07-28 08:06:43.000000 femto-admin-0.2.0/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-31 08:45:14.956017 femto-admin-0.2.0/setup.cfg
```

### Comparing `femto-admin-0.1.2/LICENSE` & `femto-admin-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/PKG-INFO` & `femto-admin-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femto-admin
-Version: 0.1.2
+Version: 0.2.0
 Summary: Simplest fastest minimal ASGI CRUD Admin panel for Tortoise ORM models. It's generating fully native async auto  zero config one line app
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/femto-admin
 Project-URL: Repository, https://github.com/mixartemev/femto-admin
 Keywords: starlette,fastapi,admin,dashboard,datatables,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

### Comparing `femto-admin-0.1.2/README.md` & `femto-admin-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/__pycache__/admin.cpython-311.pyc` & `femto-admin-0.2.0/femto_admin/__pycache__/admin.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,23 +1,23 @@
 magic:    0xa70d0d0a
-moddate:  0x2151c264 (Thu Jul 27 11:12:33 2023 UTC)
-files sz: 3691
+moddate:  0x91d9c664 (Sun Jul 30 21:43:45 2023 UTC)
+files sz: 3729
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d005a000100640064026c016d025a026d035a036d
       045a040100640064036c056d065a060100640064046c076d085a086d095a
       090100640064056c0a6d0b5a0b6d0c5a0c0100640064066c0d6d0e5a0e01
-      00640064076c0f6d105a100100640064086c116d125a126d135a13010064
-      0064096c146d155a1501006400640a6c165a166400640b6c176d185a1801
-      0002004700640c8400640d6512a6030000ab0300000000000000005a1964
-      0a5300
+      00640064076c0f6d105a100100640064086c116d125a120100640064096c
+      136d145a1401006400640a6c156d165a1601006400640b6c175a17640064
+      0c6c186d195a19010002004700640d8400640e6512a6030000ab03000000
+      00000000005a1a640b5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('datetime',))
                  6 IMPORT_NAME              0 (datetime)
                  8 IMPORT_FROM              0 (datetime)
                 10 STORE_NAME               0 (datetime)
@@ -70,125 +70,131 @@
                 92 LOAD_CONST               7 (('Jinja2Templates',))
                 94 IMPORT_NAME             15 (starlette.templating)
                 96 IMPORT_FROM             16 (Jinja2Templates)
                 98 STORE_NAME              16 (Jinja2Templates)
                100 POP_TOP
    
      9         102 LOAD_CONST               0 (0)
-               104 LOAD_CONST               8 (('Api', 'Model'))
+               104 LOAD_CONST               8 (('Api',))
                106 IMPORT_NAME             17 (tortoise_api.api)
                108 IMPORT_FROM             18 (Api)
                110 STORE_NAME              18 (Api)
-               112 IMPORT_FROM             19 (Model)
-               114 STORE_NAME              19 (Model)
-               116 POP_TOP
+               112 POP_TOP
    
-    10         118 LOAD_CONST               0 (0)
-               120 LOAD_CONST               9 (('jsonify',))
-               122 IMPORT_NAME             20 (tortoise_api.util)
-               124 IMPORT_FROM             21 (jsonify)
-               126 STORE_NAME              21 (jsonify)
-               128 POP_TOP
+    10         114 LOAD_CONST               0 (0)
+               116 LOAD_CONST               9 (('jsonify',))
+               118 IMPORT_NAME             19 (tortoise_api.util)
+               120 IMPORT_FROM             20 (jsonify)
+               122 STORE_NAME              20 (jsonify)
+               124 POP_TOP
    
-    12         130 LOAD_CONST               0 (0)
-               132 LOAD_CONST              10 (None)
-               134 IMPORT_NAME             22 (femto_admin)
-               136 STORE_NAME              22 (femto_admin)
+    11         126 LOAD_CONST               0 (0)
+               128 LOAD_CONST              10 (('Model',))
+               130 IMPORT_NAME             21 (tortoise_api_model)
+               132 IMPORT_FROM             22 (Model)
+               134 STORE_NAME              22 (Model)
+               136 POP_TOP
    
     13         138 LOAD_CONST               0 (0)
-               140 LOAD_CONST              11 (('_fields',))
-               142 IMPORT_NAME             23 (femto_admin.utils)
-               144 IMPORT_FROM             24 (_fields)
-               146 STORE_NAME              24 (_fields)
-               148 POP_TOP
+               140 LOAD_CONST              11 (None)
+               142 IMPORT_NAME             23 (femto_admin)
+               144 STORE_NAME              23 (femto_admin)
    
-    16         150 PUSH_NULL
-               152 LOAD_BUILD_CLASS
-               154 LOAD_CONST              12 (<code object Admin, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 16>)
-               156 MAKE_FUNCTION            0
-               158 LOAD_CONST              13 ('Admin')
-               160 LOAD_NAME               18 (Api)
-               162 PRECALL                  3
-               166 CALL                     3
-               176 STORE_NAME              25 (Admin)
-               178 LOAD_CONST              10 (None)
-               180 RETURN_VALUE
+    14         146 LOAD_CONST               0 (0)
+               148 LOAD_CONST              12 (('_fields',))
+               150 IMPORT_NAME             24 (femto_admin.utils)
+               152 IMPORT_FROM             25 (_fields)
+               154 STORE_NAME              25 (_fields)
+               156 POP_TOP
+   
+    17         158 PUSH_NULL
+               160 LOAD_BUILD_CLASS
+               162 LOAD_CONST              13 (<code object Admin, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 17>)
+               164 MAKE_FUNCTION            0
+               166 LOAD_CONST              14 ('Admin')
+               168 LOAD_NAME               18 (Api)
+               170 PRECALL                  3
+               174 CALL                     3
+               184 STORE_NAME              26 (Admin)
+               186 LOAD_CONST              11 (None)
+               188 RETURN_VALUE
    consts
       0
       ('datetime',)
       ('ChoiceLoader', 'FileSystemLoader', 'PackageLoader')
       ('Request',)
       ('RedirectResponse', 'JSONResponse')
       ('Mount', 'Route')
       ('StaticFiles',)
       ('Jinja2Templates',)
-      ('Api', 'Model')
+      ('Api',)
       ('jsonify',)
+      ('Model',)
       None
       ('_fields',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 10
          flags     : 0
          code
             0x8700970065005a0164005a02640d640365036404650464056504640665
             0465037a0700006608880066016407840d5a0588006601640884085a0664
             0965076602640a84045a08640965076602640b84045a0964096507660264
             0c84045a0a880078015a0b5300
                        0 MAKE_CELL                0 (__class__)
          
-          16           2 RESUME                   0
+          17           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Admin')
                       10 STORE_NAME               2 (__qualname__)
          
-          17          12 LOAD_CONST              13 ((False, 'Admin', None, None))
+          18          12 LOAD_CONST              13 ((False, 'Admin', None, None))
                       14 LOAD_CONST               3 ('debug')
                       16 LOAD_NAME                3 (bool)
                       18 LOAD_CONST               4 ('title')
                       20 LOAD_NAME                4 (str)
                       22 LOAD_CONST               5 ('static_dir')
                       24 LOAD_NAME                4 (str)
                       26 LOAD_CONST               6 ('logo')
                       28 LOAD_NAME                4 (str)
                       30 LOAD_NAME                3 (bool)
                       32 BINARY_OP                7 (|)
                       36 BUILD_TUPLE              8
                       38 LOAD_CLOSURE             0 (__class__)
                       40 BUILD_TUPLE              1
-                      42 LOAD_CONST               7 (<code object __init__, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 17>)
+                      42 LOAD_CONST               7 (<code object __init__, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 18>)
                       44 MAKE_FUNCTION           13 (defaults, annotations, closure)
                       46 STORE_NAME               5 (__init__)
          
-          52          48 LOAD_CLOSURE             0 (__class__)
+          53          48 LOAD_CLOSURE             0 (__class__)
                       50 BUILD_TUPLE              1
-                      52 LOAD_CONST               8 (<code object start, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 52>)
+                      52 LOAD_CONST               8 (<code object start, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 53>)
                       54 MAKE_FUNCTION            8 (closure)
                       56 STORE_NAME               6 (start)
          
-          58          58 LOAD_CONST               9 ('request')
+          59          58 LOAD_CONST               9 ('request')
                       60 LOAD_NAME                7 (Request)
                       62 BUILD_TUPLE              2
-                      64 LOAD_CONST              10 (<code object dash, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 58>)
+                      64 LOAD_CONST              10 (<code object dash, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 59>)
                       66 MAKE_FUNCTION            4 (annotations)
                       68 STORE_NAME               8 (dash)
          
-          65          70 LOAD_CONST               9 ('request')
+          66          70 LOAD_CONST               9 ('request')
                       72 LOAD_NAME                7 (Request)
                       74 BUILD_TUPLE              2
-                      76 LOAD_CONST              11 (<code object index, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 65>)
+                      76 LOAD_CONST              11 (<code object index, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 66>)
                       78 MAKE_FUNCTION            4 (annotations)
                       80 STORE_NAME               9 (index)
          
-          74          82 LOAD_CONST               9 ('request')
+          75          82 LOAD_CONST               9 ('request')
                       84 LOAD_NAME                7 (Request)
                       86 BUILD_TUPLE              2
-                      88 LOAD_CONST              12 (<code object dt, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 74>)
+                      88 LOAD_CONST              12 (<code object dt, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 75>)
                       90 MAKE_FUNCTION            4 (annotations)
                       92 STORE_NAME              10 (dt)
                       94 LOAD_CLOSURE             0 (__class__)
                       96 COPY                     1
                       98 STORE_NAME              11 (__classcell__)
                      100 RETURN_VALUE
          consts
@@ -234,106 +240,106 @@
                   0000006a140000000000000000a6000000ab0000000000000000006a1500
                   00000000000000742c000000000000000000006a17000000000000000064
                   169c027c056a0d00000000000000006a0e000000000000000064173c0000
                   007c01720264186e0164197c056a0d00000000000000006a0e0000000000
                   000000641a3c0000007c057c005f18000000000000000064135300
                              0 COPY_FREE_VARS           1
                
-                17           2 RESUME                   0
+                18           2 RESUME                   0
                
-                23           4 LOAD_GLOBAL              1 (NULL + super)
+                24           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (__init__)
                             52 LOAD_FAST                1 (debug)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 POP_TOP
                
-                24          70 LOAD_FAST                2 (title)
+                25          70 LOAD_FAST                2 (title)
                             72 LOAD_FAST                0 (self)
                             74 STORE_ATTR               2 (title)
                
-                27          84 LOAD_GLOBAL              7 (NULL + Mount)
+                28          84 LOAD_GLOBAL              7 (NULL + Mount)
                             96 LOAD_CONST               1 ('/static')
                             98 LOAD_GLOBAL              9 (NULL + StaticFiles)
                            110 LOAD_CONST               2 ('femto_admin')
                            112 BUILD_LIST               1
                            114 KW_NAMES                 3
                            116 PRECALL                  1
                            120 CALL                     1
                            130 LOAD_CONST               4 ('public')
                            132 KW_NAMES                 5
                            134 PRECALL                  3
                            138 CALL                     3
                
-                28         148 LOAD_GLOBAL              7 (NULL + Mount)
+                29         148 LOAD_GLOBAL              7 (NULL + Mount)
                            160 LOAD_CONST               6 ('/api')
                            162 LOAD_FAST                0 (self)
                            164 LOAD_ATTR                5 (routes)
                            174 KW_NAMES                 7
                            176 PRECALL                  2
                            180 CALL                     2
                
-                29         190 LOAD_GLOBAL             13 (NULL + Route)
+                30         190 LOAD_GLOBAL             13 (NULL + Route)
                            202 LOAD_CONST               8 ('/favicon.ico')
-                           204 LOAD_CONST               9 (<code object <lambda>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 29>)
+                           204 LOAD_CONST               9 (<code object <lambda>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 30>)
                            206 MAKE_FUNCTION            0
                            208 LOAD_CONST              10 ('GET')
                            210 BUILD_LIST               1
                            212 KW_NAMES                11
                            214 PRECALL                  3
                            218 CALL                     3
                
-                30         228 LOAD_GLOBAL             13 (NULL + Route)
+                31         228 LOAD_GLOBAL             13 (NULL + Route)
                            240 LOAD_CONST              12 ('/{model}')
                            242 LOAD_FAST                0 (self)
                            244 LOAD_ATTR                7 (index)
                            254 PRECALL                  2
                            258 CALL                     2
                
-                31         268 LOAD_GLOBAL             13 (NULL + Route)
+                32         268 LOAD_GLOBAL             13 (NULL + Route)
                            280 LOAD_CONST              13 ('/dt/{model}')
                            282 LOAD_FAST                0 (self)
                            284 LOAD_ATTR                8 (dt)
                            294 PRECALL                  2
                            298 CALL                     2
                
-                32         308 LOAD_GLOBAL             13 (NULL + Route)
+                33         308 LOAD_GLOBAL             13 (NULL + Route)
                            320 LOAD_CONST              14 ('/')
                            322 LOAD_FAST                0 (self)
                            324 LOAD_ATTR                9 (dash)
                            334 PRECALL                  2
                            338 CALL                     2
                
-                26         348 BUILD_LIST               6
+                27         348 BUILD_LIST               6
                            350 LOAD_FAST                0 (self)
                            352 STORE_ATTR               5 (routes)
                
-                34         362 LOAD_FAST                0 (self)
+                35         362 LOAD_FAST                0 (self)
                            364 LOAD_ATTR                5 (routes)
                            374 LOAD_CONST              15 (1)
                            376 BINARY_SUBSCR
                            386 LOAD_ATTR                5 (routes)
                            396 LOAD_METHOD             10 (pop)
                            418 LOAD_CONST              15 (1)
                            420 PRECALL                  1
                            424 CALL                     1
                            434 POP_TOP
                
-                36         436 LOAD_GLOBAL             23 (NULL + Jinja2Templates)
+                37         436 LOAD_GLOBAL             23 (NULL + Jinja2Templates)
                            448 LOAD_CONST              16 ('templates')
                            450 PRECALL                  1
                            454 CALL                     1
                            464 STORE_FAST               5 (templates)
                
-                37         466 LOAD_FAST                3 (static_dir)
+                38         466 LOAD_FAST                3 (static_dir)
                            468 POP_JUMP_FORWARD_IF_FALSE    76 (to 622)
                
-                38         470 LOAD_FAST                0 (self)
+                39         470 LOAD_FAST                0 (self)
                            472 LOAD_ATTR                5 (routes)
                            482 LOAD_METHOD             12 (append)
                            504 LOAD_GLOBAL              7 (NULL + Mount)
                            516 LOAD_CONST              14 ('/')
                            518 LOAD_FAST                3 (static_dir)
                            520 BINARY_OP                0 (+)
                            524 LOAD_GLOBAL              9 (NULL + StaticFiles)
@@ -345,80 +351,80 @@
                            556 KW_NAMES                 5
                            558 PRECALL                  3
                            562 CALL                     3
                            572 PRECALL                  1
                            576 CALL                     1
                            586 POP_TOP
                
-                39         588 LOAD_FAST                4 (logo)
+                40         588 LOAD_FAST                4 (logo)
                            590 POP_JUMP_FORWARD_IF_NONE    15 (to 622)
                
-                40         592 LOAD_FAST                4 (logo)
+                41         592 LOAD_FAST                4 (logo)
                            594 LOAD_FAST                5 (templates)
                            596 LOAD_ATTR               13 (env)
                            606 LOAD_ATTR               14 (globals)
                            616 LOAD_CONST              20 ('logo')
                            618 STORE_SUBSCR
                
-                41     >>  622 LOAD_GLOBAL             31 (NULL + ChoiceLoader)
+                42     >>  622 LOAD_GLOBAL             31 (NULL + ChoiceLoader)
                
-                43         634 LOAD_GLOBAL             33 (NULL + FileSystemLoader)
+                44         634 LOAD_GLOBAL             33 (NULL + FileSystemLoader)
                            646 LOAD_CONST              16 ('templates')
                            648 PRECALL                  1
                            652 CALL                     1
                
-                44         662 LOAD_GLOBAL             35 (NULL + PackageLoader)
+                45         662 LOAD_GLOBAL             35 (NULL + PackageLoader)
                            674 LOAD_CONST               2 ('femto_admin')
                            676 LOAD_CONST              16 ('templates')
                            678 PRECALL                  2
                            682 CALL                     2
                
-                42         692 BUILD_LIST               2
+                43         692 BUILD_LIST               2
                
-                41         694 PRECALL                  1
+                42         694 PRECALL                  1
                            698 CALL                     1
                            708 LOAD_FAST                5 (templates)
                            710 LOAD_ATTR               13 (env)
                            720 STORE_ATTR              18 (loader)
                
-                47         730 LOAD_FAST                0 (self)
+                48         730 LOAD_FAST                0 (self)
                            732 LOAD_ATTR                2 (title)
                            742 LOAD_FAST                5 (templates)
                            744 LOAD_ATTR               13 (env)
                            754 LOAD_ATTR               14 (globals)
                            764 LOAD_CONST              21 ('title')
                            766 STORE_SUBSCR
                
-                48         770 LOAD_GLOBAL             39 (NULL + datetime)
+                49         770 LOAD_GLOBAL             39 (NULL + datetime)
                            782 LOAD_ATTR               20 (now)
                            792 PRECALL                  0
                            796 CALL                     0
                            806 LOAD_ATTR               21 (year)
                            816 LOAD_GLOBAL             44 (femto_admin)
                            828 LOAD_ATTR               23 (__version__)
                            838 LOAD_CONST              22 (('year', 'ver'))
                            840 BUILD_CONST_KEY_MAP      2
                            842 LOAD_FAST                5 (templates)
                            844 LOAD_ATTR               13 (env)
                            854 LOAD_ATTR               14 (globals)
                            864 LOAD_CONST              23 ('meta')
                            866 STORE_SUBSCR
                
-                49         870 LOAD_FAST                1 (debug)
+                50         870 LOAD_FAST                1 (debug)
                            872 POP_JUMP_FORWARD_IF_FALSE     2 (to 878)
                            874 LOAD_CONST              24 ('')
                            876 JUMP_FORWARD             1 (to 880)
                        >>  878 LOAD_CONST              25 ('min.')
                        >>  880 LOAD_FAST                5 (templates)
                            882 LOAD_ATTR               13 (env)
                            892 LOAD_ATTR               14 (globals)
                            902 LOAD_CONST              26 ('minify')
                            904 STORE_SUBSCR
                
-                50         908 LOAD_FAST                5 (templates)
+                51         908 LOAD_FAST                5 (templates)
                            910 LOAD_FAST                0 (self)
                            912 STORE_ATTR              24 (templates)
                            922 LOAD_CONST              19 (None)
                            924 RETURN_VALUE
                consts
                   '\n        Parameters:\n            title: Admin title.\n            # auth_provider: Authentication Provider\n        '
                   '/static'
@@ -433,15 +439,15 @@
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 4
                      flags     : 19
                      code
                         0x970074010000000000000000000064016402ac03a6020000ab02000000
                         00000000005300
-                      29           0 RESUME                   0
+                      30           0 RESUME                   0
                                    2 LOAD_GLOBAL              1 (NULL + RedirectResponse)
                                   14 LOAD_CONST               1 ('./static/placeholders/favicon.ico')
                                   16 LOAD_CONST               2 (301)
                                   18 KW_NAMES                 3
                                   20 PRECALL                  2
                                   24 CALL                     2
                                   34 RETURN_VALUE
@@ -452,15 +458,15 @@
                         ('status_code',)
                      names      ('RedirectResponse',)
                      varnames   ('r',)
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                      name       '<lambda>'
-                     firstlineno 29
+                     firstlineno 30
                      lnotab 0x
                   'GET'
                   ('methods',)
                   '/{model}'
                   '/dt/{model}'
                   '/'
                   1
@@ -477,15 +483,15 @@
                   'minify'
                names      ('super', '__init__', 'title', 'Mount', 'StaticFiles', 'routes', 'Route', 'index', 'dt', 'dash', 'pop', 'Jinja2Templates', 'append', 'env', 'globals', 'ChoiceLoader', 'FileSystemLoader', 'PackageLoader', 'loader', 'datetime', 'now', 'year', 'femto_admin', '__version__', 'templates')
                varnames   ('self', 'debug', 'title', 'static_dir', 'logo', 'templates')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                name       '__init__'
-               firstlineno 17
+               firstlineno 18
                lnotab
                   0x040642010e0340012a0126012801280128fa0e084a021e010401760104
                   011e010c021c011efe02ff2406280164012601
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 3
@@ -494,150 +500,154 @@
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a00100000000000000000000000000000000000000007c01a6010000ab
                   0100000000000000007d027c006a0200000000000000007c006a03000000
                   00000000006a0400000000000000006a05000000000000000064013c0000
                   007c025300
                              0 COPY_FREE_VARS           1
                
-                52           2 RESUME                   0
+                53           2 RESUME                   0
                
-                53           4 LOAD_GLOBAL              1 (NULL + super)
+                54           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (start)
                             52 LOAD_FAST                1 (models_module)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 STORE_FAST               2 (app)
                
-                54          70 LOAD_FAST                0 (self)
+                55          70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                2 (models)
                             82 LOAD_FAST                0 (self)
                             84 LOAD_ATTR                3 (templates)
                             94 LOAD_ATTR                4 (env)
                            104 LOAD_ATTR                5 (globals)
                            114 LOAD_CONST               1 ('models')
                            116 STORE_SUBSCR
                
-                55         120 LOAD_FAST                2 (app)
+                56         120 LOAD_FAST                2 (app)
                            122 RETURN_VALUE
                consts
                   None
                   'models'
                names      ('super', 'start', 'models', 'templates', 'env', 'globals')
                varnames   ('self', 'models_module', 'app')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                name       'start'
-               firstlineno 52
+               firstlineno 53
                lnotab 0x040142013201
             'request'
             code
                argcount  : 2
                nlocals   : 2
-               stacksize : 7
+               stacksize : 6
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
-                  00000000000000000000006401640264037c0164049c03a6020000ab0200
-                  000000000000005300
-                58           0 RETURN_GENERATOR
+                  0000000000000000000000640164027c0164039c02a6020000ab02000000
+                  00000000005300
+                59           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                59           6 LOAD_FAST                0 (self)
+                60           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (templates)
                             18 LOAD_METHOD              1 (TemplateResponse)
                             40 LOAD_CONST               1 ('dashboard.html')
                
-                60          42 LOAD_CONST               2 ('Home')
-               
-                61          44 LOAD_CONST               3 ('Dashboard')
+                62          42 LOAD_CONST               2 ('Dashboard')
                
-                62          46 LOAD_FAST                1 (request)
+                63          44 LOAD_FAST                1 (request)
                
-                59          48 LOAD_CONST               4 (('model', 'subtitle', 'request'))
-                            50 BUILD_CONST_KEY_MAP      3
-                            52 PRECALL                  2
-                            56 CALL                     2
-                            66 RETURN_VALUE
+                60          46 LOAD_CONST               3 (('subtitle', 'request'))
+                            48 BUILD_CONST_KEY_MAP      2
+                            50 PRECALL                  2
+                            54 CALL                     2
+                            64 RETURN_VALUE
                consts
                   None
                   'dashboard.html'
-                  'Home'
                   'Dashboard'
-                  ('model', 'subtitle', 'request')
+                  ('subtitle', 'request')
                names      ('templates', 'TemplateResponse')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                name       'dash'
-               firstlineno 58
-               lnotab 0x060124010201020102fd
+               firstlineno 59
+               lnotab 0x06012402020102fd
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 9
                flags     : 131
                code
                   0x4b00010097007c00a00000000000000000000000000000000000000000
                   007c01a6010000ab0100000000000000007d027c006a0100000000000000
                   00a002000000000000000000000000000000000000000064017c026a0300
                   000000000000007c026a0400000000000000006a0500000000000000007c
-                  01740d000000000000000000007c02a6010000ab01000000000000000064
-                  029c04a6020000ab0200000000000000005300
-                65           0 RETURN_GENERATOR
+                  01740d000000000000000000007c02a6010000ab01000000000000000083
+                  0064007b0356009703860464029c04a6020000ab02000000000000000053
+                  00
+                66           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                66           6 LOAD_FAST                0 (self)
+                67           6 LOAD_FAST                0 (self)
                              8 LOAD_METHOD              0 (_get_model)
                             30 LOAD_FAST                1 (request)
                             32 PRECALL                  1
                             36 CALL                     1
                             46 STORE_FAST               2 (model)
                
-                67          48 LOAD_FAST                0 (self)
+                68          48 LOAD_FAST                0 (self)
                             50 LOAD_ATTR                1 (templates)
                             60 LOAD_METHOD              2 (TemplateResponse)
-                            82 LOAD_CONST               1 ('table.html')
+                            82 LOAD_CONST               1 ('index.html')
                
-                68          84 LOAD_FAST                2 (model)
+                69          84 LOAD_FAST                2 (model)
                             86 LOAD_ATTR                3 (__name__)
                
-                69          96 LOAD_FAST                2 (model)
+                70          96 LOAD_FAST                2 (model)
                             98 LOAD_ATTR                4 (_meta)
                            108 LOAD_ATTR                5 (table_description)
                
-                70         118 LOAD_FAST                1 (request)
+                71         118 LOAD_FAST                1 (request)
                
-                71         120 LOAD_GLOBAL             13 (NULL + _fields)
+                72         120 LOAD_GLOBAL             13 (NULL + _fields)
                            132 LOAD_FAST                2 (model)
                            134 PRECALL                  1
                            138 CALL                     1
-               
-                67         148 LOAD_CONST               2 (('model', 'subtitle', 'request', 'fields'))
-                           150 BUILD_CONST_KEY_MAP      4
-                           152 PRECALL                  2
-                           156 CALL                     2
-                           166 RETURN_VALUE
+                           148 GET_AWAITABLE            0
+                           150 LOAD_CONST               0 (None)
+                       >>  152 SEND                     3 (to 160)
+                           154 YIELD_VALUE
+                           156 RESUME                   3
+                           158 JUMP_BACKWARD_NO_INTERRUPT     4 (to 152)
+               
+                68     >>  160 LOAD_CONST               2 (('model', 'subtitle', 'request', 'fields'))
+                           162 BUILD_CONST_KEY_MAP      4
+                           164 PRECALL                  2
+                           168 CALL                     2
+                           178 RETURN_VALUE
                consts
                   None
-                  'table.html'
+                  'index.html'
                   ('model', 'subtitle', 'request', 'fields')
                names      ('_get_model', 'templates', 'TemplateResponse', '__name__', '_meta', 'table_description', '_fields')
                varnames   ('self', 'request', 'model')
                freevars   ()
                cellvars   ()
                filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                name       'index'
-               firstlineno 65
-               lnotab 0x06012a0124010c01160102011cfc
+               firstlineno 66
+               lnotab 0x06012a0124010c011601020128fc
             code
                argcount  : 2
                nlocals   : 5
                stacksize : 4
                flags     : 131
                code
                   0x87054b000100970064017400000000000000000000006602640284048a
@@ -646,33 +656,33 @@
                   000000000000000000a6000000ab0000000000000000006a030000000000
                   0000007c026a0400000000000000006a0500000000000000008e00830064
                   007b035600970386047d0388056601640384087c034400a6000000ab0000
                   000000000000007d04740d0000000000000000000064047c046901a60100
                   00ab0100000000000000005300
                              0 MAKE_CELL                5 (render)
                
-                74           2 RETURN_GENERATOR
+                75           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                
-                75           8 LOAD_CONST               1 ('dct')
+                76           8 LOAD_CONST               1 ('dct')
                             10 LOAD_GLOBAL              0 (dict)
                             22 BUILD_TUPLE              2
-                            24 LOAD_CONST               2 (<code object render, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 75>)
+                            24 LOAD_CONST               2 (<code object render, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 76>)
                             26 MAKE_FUNCTION            4 (annotations)
                             28 STORE_DEREF              5 (render)
                
-                87          30 LOAD_FAST                0 (self)
+                88          30 LOAD_FAST                0 (self)
                             32 LOAD_METHOD              1 (_get_model)
                             54 LOAD_FAST                1 (request)
                             56 PRECALL                  1
                             60 CALL                     1
                             70 STORE_FAST               2 (model)
                
-                88          72 PUSH_NULL
+                89          72 PUSH_NULL
                             74 LOAD_FAST                2 (model)
                             76 LOAD_METHOD              2 (all)
                             98 PRECALL                  0
                            102 CALL                     0
                            112 LOAD_ATTR                3 (prefetch_related)
                            122 LOAD_FAST                2 (model)
                            124 LOAD_ATTR                4 (_meta)
@@ -682,25 +692,25 @@
                            148 LOAD_CONST               0 (None)
                        >>  150 SEND                     3 (to 158)
                            152 YIELD_VALUE
                            154 RESUME                   3
                            156 JUMP_BACKWARD_NO_INTERRUPT     4 (to 150)
                        >>  158 STORE_FAST               3 (objects)
                
-                89         160 LOAD_CLOSURE             5 (render)
+                90         160 LOAD_CLOSURE             5 (render)
                            162 BUILD_TUPLE              1
-                           164 LOAD_CONST               3 (<code object <listcomp>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 89>)
+                           164 LOAD_CONST               3 (<code object <listcomp>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 90>)
                            166 MAKE_FUNCTION            8 (closure)
                            168 LOAD_FAST                3 (objects)
                            170 GET_ITER
                            172 PRECALL                  0
                            176 CALL                     0
                            186 STORE_FAST               4 (data)
                
-                90         188 LOAD_GLOBAL             13 (NULL + JSONResponse)
+                91         188 LOAD_GLOBAL             13 (NULL + JSONResponse)
                            200 LOAD_CONST               4 ('data')
                            202 LOAD_FAST                4 (data)
                            204 BUILD_MAP                1
                            206 PRECALL                  1
                            210 CALL                     1
                            220 RETURN_VALUE
                consts
@@ -715,32 +725,32 @@
                         0x87018702970064017400000000000000000000006602640284048a0288
                         026601640384088a0188016601640484087c00a001000000000000000000
                         0000000000000000000000a6000000ab0000000000000000004400a60000
                         00ab0000000000000000005300
                                    0 MAKE_CELL                1 (check)
                                    2 MAKE_CELL                2 (rel)
                      
-                      75           4 RESUME                   0
+                      76           4 RESUME                   0
                      
-                      76           6 LOAD_CONST               1 ('val')
+                      77           6 LOAD_CONST               1 ('val')
                                    8 LOAD_GLOBAL              0 (dict)
                                   20 BUILD_TUPLE              2
-                                  22 LOAD_CONST               2 (<code object rel, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 76>)
+                                  22 LOAD_CONST               2 (<code object rel, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 77>)
                                   24 MAKE_FUNCTION            4 (annotations)
                                   26 STORE_DEREF              2 (rel)
                      
-                      78          28 LOAD_CLOSURE             2 (rel)
+                      79          28 LOAD_CLOSURE             2 (rel)
                                   30 BUILD_TUPLE              1
-                                  32 LOAD_CONST               3 (<code object check, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 78>)
+                                  32 LOAD_CONST               3 (<code object check, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 79>)
                                   34 MAKE_FUNCTION            8 (closure)
                                   36 STORE_DEREF              1 (check)
                      
-                      85          38 LOAD_CLOSURE             1 (check)
+                      86          38 LOAD_CLOSURE             1 (check)
                                   40 BUILD_TUPLE              1
-                                  42 LOAD_CONST               4 (<code object <listcomp>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 85>)
+                                  42 LOAD_CONST               4 (<code object <listcomp>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 86>)
                                   44 MAKE_FUNCTION            8 (closure)
                                   46 LOAD_FAST                0 (dct)
                                   48 LOAD_METHOD              1 (items)
                                   70 PRECALL                  0
                                   74 CALL                     0
                                   84 GET_ITER
                                   86 PRECALL                  0
@@ -754,17 +764,17 @@
                            nlocals   : 1
                            stacksize : 7
                            flags     : 19
                            code
                               0x970064017c006402190000000000000000009b0064037c006404190000
                               000000000000009b0064057c006406190000000000000000009b0064079d
                               075300
-                            76           0 RESUME                   0
+                            77           0 RESUME                   0
                            
-                            77           2 LOAD_CONST               1 ('<a class="m-1 py-1 px-2 badge bg-blue-lt lead" href="/')
+                            78           2 LOAD_CONST               1 ('<a class="m-1 py-1 px-2 badge bg-blue-lt lead" href="/')
                                          4 LOAD_FAST                0 (val)
                                          6 LOAD_CONST               2 ('type')
                                          8 BINARY_SUBSCR
                                         18 FORMAT_VALUE             0
                                         20 LOAD_CONST               3 ('/')
                                         22 LOAD_FAST                0 (val)
                                         24 LOAD_CONST               4 ('id')
@@ -789,15 +799,15 @@
                               '</a>'
                            names      ()
                            varnames   ('val',)
                            freevars   ()
                            cellvars   ()
                            filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                            name       'rel'
-                           firstlineno 76
+                           firstlineno 77
                            lnotab 0x0201
                         code
                            argcount  : 1
                            nlocals   : 1
                            stacksize : 4
                            flags     : 19
                            code
@@ -811,38 +821,38 @@
                               00723d64017c00640219000000000000000000a002000000000000000000
                               0000000000000000000000a6000000ab0000000000000000007600722164
                               03a004000000000000000000000000000000000000000088016601640484
                               087c004400a6000000ab000000000000000000a6010000ab010000000000
                               00000053007c005300
                                          0 COPY_FREE_VARS           1
                            
-                            78           2 RESUME                   0
+                            79           2 RESUME                   0
                            
-                            79           4 LOAD_GLOBAL              1 (NULL + isinstance)
+                            80           4 LOAD_GLOBAL              1 (NULL + isinstance)
                                         16 LOAD_FAST                0 (val)
                                         18 LOAD_GLOBAL              2 (dict)
                                         30 PRECALL                  2
                                         34 CALL                     2
                                         44 POP_JUMP_FORWARD_IF_FALSE    33 (to 112)
                                         46 LOAD_CONST               1 ('repr')
                                         48 LOAD_FAST                0 (val)
                                         50 LOAD_METHOD              2 (keys)
                                         72 PRECALL                  0
                                         76 CALL                     0
                                         86 CONTAINS_OP              0
                                         88 POP_JUMP_FORWARD_IF_FALSE    11 (to 112)
                            
-                            80          90 PUSH_NULL
+                            81          90 PUSH_NULL
                                         92 LOAD_DEREF               1 (rel)
                                         94 LOAD_FAST                0 (val)
                                         96 PRECALL                  1
                                        100 CALL                     1
                                        110 RETURN_VALUE
                            
-                            81     >>  112 LOAD_GLOBAL              1 (NULL + isinstance)
+                            82     >>  112 LOAD_GLOBAL              1 (NULL + isinstance)
                                        124 LOAD_FAST                0 (val)
                                        126 LOAD_GLOBAL              6 (list)
                                        138 PRECALL                  2
                                        142 CALL                     2
                                        152 POP_JUMP_FORWARD_IF_FALSE    90 (to 334)
                                        154 LOAD_FAST                0 (val)
                                        156 POP_JUMP_FORWARD_IF_FALSE    88 (to 334)
@@ -860,29 +870,29 @@
                                        218 BINARY_SUBSCR
                                        228 LOAD_METHOD              2 (keys)
                                        250 PRECALL                  0
                                        254 CALL                     0
                                        264 CONTAINS_OP              0
                                        266 POP_JUMP_FORWARD_IF_FALSE    33 (to 334)
                            
-                            82         268 LOAD_CONST               3 (' ')
+                            83         268 LOAD_CONST               3 (' ')
                                        270 LOAD_METHOD              4 (join)
                                        292 LOAD_CLOSURE             1 (rel)
                                        294 BUILD_TUPLE              1
-                                       296 LOAD_CONST               4 (<code object <genexpr>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 82>)
+                                       296 LOAD_CONST               4 (<code object <genexpr>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 83>)
                                        298 MAKE_FUNCTION            8 (closure)
                                        300 LOAD_FAST                0 (val)
                                        302 GET_ITER
                                        304 PRECALL                  0
                                        308 CALL                     0
                                        318 PRECALL                  1
                                        322 CALL                     1
                                        332 RETURN_VALUE
                            
-                            83     >>  334 LOAD_FAST                0 (val)
+                            84     >>  334 LOAD_FAST                0 (val)
                                        336 RETURN_VALUE
                            consts
                               None
                               'repr'
                               0
                               ' '
                               code
@@ -891,15 +901,15 @@
                                  stacksize : 4
                                  flags     : 51
                                  code
                                     0x95014b00010097007c005d0f7d01020089027c01a6010000ab01000000
                                     00000000005600970101008c1064005300
                                                0 COPY_FREE_VARS           1
                                  
-                                  82           2 RETURN_GENERATOR
+                                  83           2 RETURN_GENERATOR
                                                4 POP_TOP
                                                6 RESUME                   0
                                                8 LOAD_FAST                0 (.0)
                                          >>   10 FOR_ITER                15 (to 42)
                                               12 STORE_FAST               1 (v)
                                               14 PUSH_NULL
                                               16 LOAD_DEREF               2 (rel)
@@ -916,35 +926,35 @@
                                     None
                                  names      ()
                                  varnames   ('.0', 'v')
                                  freevars   ('rel',)
                                  cellvars   ()
                                  filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                                  name       '<genexpr>'
-                                 firstlineno 82
+                                 firstlineno 83
                                  lnotab 0x
                            names      ('isinstance', 'dict', 'keys', 'list', 'join')
                            varnames   ('val',)
                            freevars   ('rel',)
                            cellvars   ()
                            filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                            name       'check'
-                           firstlineno 78
+                           firstlineno 79
                            lnotab 0x0401560116019c014201
                         code
                            argcount  : 1
                            nlocals   : 3
                            stacksize : 5
                            flags     : 19
                            code
                               0x9501970067007c005d105c0200007d017d02020089037c02a6010000ab
                               01000000000000000091028c115300
                                          0 COPY_FREE_VARS           1
                            
-                            85           2 RESUME                   0
+                            86           2 RESUME                   0
                                          4 BUILD_LIST               0
                                          6 LOAD_FAST                0 (.0)
                                    >>    8 FOR_ITER                16 (to 42)
                                         10 UNPACK_SEQUENCE          2
                                         14 STORE_FAST               1 (key)
                                         16 STORE_FAST               2 (val)
                                         18 PUSH_NULL
@@ -958,36 +968,36 @@
                            consts
                            names      ()
                            varnames   ('.0', 'key', 'val')
                            freevars   ('check',)
                            cellvars   ()
                            filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                            name       '<listcomp>'
-                           firstlineno 85
+                           firstlineno 86
                            lnotab 0x
                      names      ('dict', 'items')
                      varnames   ('dct',)
                      freevars   ()
                      cellvars   ('check', 'rel')
                      filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                      name       'render'
-                     firstlineno 75
+                     firstlineno 76
                      lnotab 0x060116020a07
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 7
                      flags     : 19
                      code
                         0x9501970067007c005d1a7d01020089027401000000000000000000007c
                         01a6010000ab010000000000000000a6010000ab01000000000000000091
                         028c1b5300
                                    0 COPY_FREE_VARS           1
                      
-                      89           2 RESUME                   0
+                      90           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                26 (to 62)
                                   10 STORE_FAST               1 (obj)
                                   12 PUSH_NULL
                                   14 LOAD_DEREF               2 (render)
                                   16 LOAD_GLOBAL              1 (NULL + jsonify)
@@ -1002,36 +1012,36 @@
                      consts
                      names      ('jsonify',)
                      varnames   ('.0', 'obj')
                      freevars   ('render',)
                      cellvars   ()
                      filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                      name       '<listcomp>'
-                     firstlineno 89
+                     firstlineno 90
                      lnotab 0x
                   'data'
                names      ('dict', '_get_model', 'all', 'prefetch_related', '_meta', 'fetch_fields', 'JSONResponse')
                varnames   ('self', 'request', 'model', 'objects', 'data')
                freevars   ()
                cellvars   ('render',)
                filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                name       'dt'
-               firstlineno 74
+               firstlineno 75
                lnotab 0x0801160c2a0158011c01
             (False, 'Admin', None, None)
          names      ('__name__', '__module__', '__qualname__', 'bool', 'str', '__init__', 'start', 'Request', 'dash', 'index', 'dt', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
          name       'Admin'
-         firstlineno 16
+         firstlineno 17
          lnotab 0x0c0124230a060c070c09
       'Admin'
-   names      ('datetime', 'jinja2', 'ChoiceLoader', 'FileSystemLoader', 'PackageLoader', 'starlette.requests', 'Request', 'starlette.responses', 'RedirectResponse', 'JSONResponse', 'starlette.routing', 'Mount', 'Route', 'starlette.staticfiles', 'StaticFiles', 'starlette.templating', 'Jinja2Templates', 'tortoise_api.api', 'Api', 'Model', 'tortoise_api.util', 'jsonify', 'femto_admin', 'femto_admin.utils', '_fields', 'Admin')
+   names      ('datetime', 'jinja2', 'ChoiceLoader', 'FileSystemLoader', 'PackageLoader', 'starlette.requests', 'Request', 'starlette.responses', 'RedirectResponse', 'JSONResponse', 'starlette.routing', 'Mount', 'Route', 'starlette.staticfiles', 'StaticFiles', 'starlette.templating', 'Jinja2Templates', 'tortoise_api.api', 'Api', 'tortoise_api.util', 'jsonify', 'tortoise_api_model', 'Model', 'femto_admin', 'femto_admin.utils', '_fields', 'Admin')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c0214010c01100110010c010c0110010c0208010c03
+   lnotab 0x00ff02010c0214010c01100110010c010c010c010c010c0208010c03
```

### Comparing `femto-admin-0.1.2/femto_admin/admin.py` & `femto-admin-0.2.0/femto_admin/admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 from jinja2 import ChoiceLoader, FileSystemLoader, PackageLoader
 from starlette.requests import Request
 from starlette.responses import RedirectResponse, JSONResponse
 from starlette.routing import Mount, Route
 from starlette.staticfiles import StaticFiles
 from starlette.templating import Jinja2Templates
-from tortoise_api.api import Api, Model
+from tortoise_api.api import Api
 from tortoise_api.util import jsonify
+from tortoise_api_model import Model
 
 import femto_admin
 from femto_admin.utils import _fields
 
 
 class Admin(Api):
     def __init__(self, debug: bool = False, title: str = "Admin", static_dir: str = None, logo: str|bool = None):
@@ -53,26 +54,26 @@
         app = super().start(models_module)
         self.templates.env.globals["models"] = self.models
         return app
 
     # INTERFACE
     async def dash(self, request: Request):
         return self.templates.TemplateResponse("dashboard.html", {
-            'model': 'Home',
+            # 'model': 'Home',
             'subtitle': 'Dashboard',
             'request': request,
         })
 
     async def index(self, request: Request):
         model: type[Model] = self._get_model(request)
-        return self.templates.TemplateResponse("table.html", {
+        return self.templates.TemplateResponse("index.html", {
             'model': model.__name__,
             'subtitle': model._meta.table_description,
             'request': request,
-            'fields': _fields(model),
+            'fields': await _fields(model),
         })
 
     async def dt(self, request: Request):
         def render(dct: dict):
             def rel(val: dict):
                 return f'<a class="m-1 py-1 px-2 badge bg-blue-lt lead" href="/{val["type"]}/{val["id"]}">{val["repr"]}</a>'
             def check(val):
```

### Comparing `femto-admin-0.1.2/femto_admin/statics/js/polygon.js` & `femto-admin-0.2.0/femto_admin/statics/js/polygon.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/placeholders/favicon.ico` & `femto-admin-0.2.0/femto_admin/statics/placeholders/favicon.ico`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/placeholders/users/admin.jpg` & `femto-admin-0.2.0/femto_admin/statics/placeholders/users/admin.jpg`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css` & `femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css` & `femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js` & `femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js` & `femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js` & `femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js` & `femto-admin-0.2.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/vendor/jQuery/jquery.js` & `femto-admin-0.2.0/femto_admin/statics/vendor/jQuery/jquery.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/vendor/jQuery/jquery.min.js` & `femto-admin-0.2.0/femto_admin/statics/vendor/jQuery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/vendor/tabler/css/tabler.css` & `femto-admin-0.2.0/femto_admin/statics/vendor/tabler/css/tabler.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/vendor/tabler/css/tabler.min.css` & `femto-admin-0.2.0/femto_admin/statics/vendor/tabler/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/vendor/tabler/js/dark-theme.js` & `femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/dark-theme.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/vendor/tabler/js/dark-theme.min.js` & `femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/dark-theme.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/vendor/tabler/js/tabler.js` & `femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/tabler.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/statics/vendor/tabler/js/tabler.min.js` & `femto-admin-0.2.0/femto_admin/statics/vendor/tabler/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/templates/components/footer.html` & `femto-admin-0.2.0/femto_admin/templates/components/footer.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-<footer class="footer footer-transparent d-print-none">
+<footer class="footer footer-transparent d-print-none py-1">
     <div class="container-fluid">
         <div class="row text-center align-items-center flex-row-reverse">
             <div class="col-lg-auto ms-lg-auto">
                 <ul class="list-inline list-inline-dots mb-0">
                     <li class="list-inline-item">
-                        <a class="link-secondary" rel="noopener">v{{ meta.ver }}</a>
+                        <a class="link-secondary" rel="noopener" target="_blank" href="https://pypi.org/project/femto-admin/{{ meta.ver }}/">v{{ meta.ver }}</a>
                     </li>
                 </ul>
             </div>
             <div class="col-12 col-lg-auto mt-3 mt-lg-0">
                 <ul class="list-inline list-inline-dots mb-0">
                     <li class="list-inline-item">
                         <a href="https://github.com/mixartemev/femto-admin" target="_blank" class="link-secondary" rel="noopener">Femto Admin</a>
```

#### html2text {}

```diff
@@ -1,2 +1,2 @@
-    * v{{ meta.ver }}
+    * v{{_meta.ver_}}
     * Femto_Admin Â© {{ meta.year }}
```

### Comparing `femto-admin-0.1.2/femto_admin/templates/components/global_actions.html` & `femto-admin-0.2.0/femto_admin/templates/components/global_actions.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 <div class="col-auto ms-auto d-print-none">
     <div class="btn-list">
+        {% if model %}
         <a href="#" class="btn btn-primary d-none d-sm-inline-block" data-bs-toggle="modal"
            data-bs-target="#modal-{{ model }}">
             <!-- Download SVG icon from https://tabler-icons.io/i/plus -->
             <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24"
                  viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none"
                  stroke-linecap="round" stroke-linejoin="round">
                 <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
@@ -19,9 +20,10 @@
                  viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none"
                  stroke-linecap="round" stroke-linejoin="round">
                 <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                 <path d="M12 5l0 14"/>
                 <path d="M5 12l14 0"/>
             </svg>
         </a>
+        {% endif %}
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1 +1 @@
-______Create_new_{{_model_}} _____
+{% if model %} ______Create_new_{{_model_}} _____ {% endif %}
```

### Comparing `femto-admin-0.1.2/femto_admin/templates/components/inputs/datetime.html` & `femto-admin-0.2.0/femto_admin/templates/components/inputs/datetime.html`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/templates/components/inputs/editor.html` & `femto-admin-0.2.0/femto_admin/templates/components/inputs/editor.html`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/templates/components/inputs/json.html` & `femto-admin-0.2.0/femto_admin/templates/components/inputs/json.html`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/templates/components/inputs/many_to_many.html` & `femto-admin-0.2.0/femto_admin/templates/components/inputs/many_to_many.html`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/templates/components/inputs/point.html` & `femto-admin-0.2.0/femto_admin/templates/components/inputs/range.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-{% if field.template=='point' %}<fieldset class="form-fieldset">{% endif %}
+{% if field.template=='range' %}<fieldset class="form-fieldset">{% endif %}
     <div class="form-group row">
-        <label class="col-2 col-form-label" for="lat">Lat</label>
+        <label class="col-2 col-form-label" for="lat">From</label>
         <div class="col-4">
-            <input type="number" class="form-control col-4" name="{{ key }}" step="0.0000001" placeholder="Latitude" {% if disabled %}disabled{% endif %} value="{{ value and value.y }}">
+            <input type="number" class="form-control col-4" name="{{ key }}" placeholder="Man value" {% if disabled %}disabled{% endif %} value="{{ value and value[0] }}">
         </div>
-        <label class="col-2 col-form-label" for="lat">Lng</label>
+        <label class="col-2 col-form-label" for="lat">To</label>
         <div class="col-4">
-            <input type="number" class="form-control col-4" name="{{ key }}" step="0.0000001" placeholder="Longitude" {% if disabled %}disabled{% endif %} value="{{ value and value.x }}">
+            <input type="number" class="form-control col-4" name="{{ key }}" placeholder="Max Value" {% if disabled %}disabled{% endif %} value="{{ value and value[1] }}">
         </div>
     </div>
-{% if field.template=='point' %}</fieldset>{% endif %}
+{% if field.template=='range' %}</fieldset>{% endif %}
 {% include "components/inputs/_help.html" %}
```

### Comparing `femto-admin-0.1.2/femto_admin/templates/components/inputs/polygon.html` & `femto-admin-0.2.0/femto_admin/templates/components/inputs/list.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 <div id="{{ key }}" class="field-list {% if error %}is-invalid{% endif %}">
     <input id="{{ key }}-next-index" value="{{ (data or []) | length }}" hidden>
     <div class="template d-none">
         {% filter forceescape %}
             <div class="mb-3 field-list-item">
                 <div class="d-flex">
                     <div class="flex-grow-1">
-{#                        {% with data=None, error=False, field=field._field_at(None) %}#}
-                            {% include "components/inputs/point.html" %}
-{#                        {% endwith %}#}
+                        {% with field=field.base_field %}
+                            {% include "components/inputs/collection.html" %}
+                        {% endwith %}
                     </div>
                     <button type="button" class="field-list-btn-remove btn btn-ghost-danger btn-icon mx-2 py-0">
                         <b class="fa fa-close">x</b>
                     </button>
                 </div>
             </div>
         {% endfilter %}
@@ -19,15 +19,15 @@
     <fieldset class="list-container form-fieldset d-flex flex-column">
         {% if (data or []) | length > 0 %}
             {% for value in data %}
                 <div class="mb-3 field-list-item">
                     <div class="d-flex">
                         <div class="flex-grow-1">
 {#                            {% with data=value, field=field._field_at(loop.index), error=error.get(loop.index0, None) if (error | is_dict) else None %}#}
-                            {% include "components/inputs/point.html" %}
+                            {% include "components/inputs/collection.html" %}
 {#                            {% endwith %}#}
                         </div>
                         <button type="button" class="field-list-btn-remove btn btn-ghost-danger btn-icon mx-2 py-0">
                             <i class="fa fa-close">x</i>
                         </button>
                     </div>
                 </div>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 [{{ (data or []) | length }}]
 {% filter forceescape %}
-{# {% with data=None, error=False, field=field._field_at(None) %}#} {% include
-"components/inputs/point.html" %} {# {% endwith %}#}
+{% with field=field.base_field %} {% include "components/inputs/
+collection.html" %} {% endwith %}
  x
 {% endfilter %}
  {% if (data or []) | length > 0 %} {% for value in data %}
 {# {% with data=value, field=field._field_at(loop.index), error=error.get
 (loop.index0, None) if (error | is_dict) else None %}#} {% include "components/
-inputs/point.html" %} {# {% endwith %}#}
+inputs/collection.html" %} {# {% endwith %}#}
  x
 {% endfor %} {% endif %}
 Add item
 {% block scripts %}
  {% endblock %}
```

### Comparing `femto-admin-0.1.2/femto_admin/templates/components/inputs/radio.html` & `femto-admin-0.2.0/femto_admin/templates/components/inputs/radio.html`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/templates/components/modal.html` & `femto-admin-0.2.0/femto_admin/templates/components/modal.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 <div class="modal modal-blur fade" id="modal-{{ model }}" tabindex="-1" role="dialog" aria-hidden="true">
     <div class="modal-dialog modal-xl" role="document">
         <div class="modal-content">
             <div class="modal-header">
                 <h5 class="modal-title">{{ title }}</h5>
                 <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
             </div>
-            <form action="/api/{{ model }}" method="POST">
+            <form action="/api/{{ model }}" method="POST" enctype="">
                 <div class="modal-body">
                     <div class="row mb-3">
     {#                    {% block modal_content %}#}
     {#                    {% endblock %}#}
                         {% for key, field in fields.items() %}
                             {% if not field.auto %}
                                 <div class="col-lg-12 mb-3">
                                     <label class="form-label">{{ key }}</label>
-                                    {% with value=obj[field.name] if obj else None %}
-                                        {% include "components/inputs/"+field.template+".html" %}
+                                    {% with value=obj[field.name] if obj else None, key=field.source_field or key %}
+                                        {% include "components/inputs/"+field.input+".html" %}
                                     {% endwith %}
                                 </div>
                             {% endif %}
                         {% endfor %}
                     </div>
                 </div>
                 <div class="modal-footer">
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 ** {{ title }} **
 {# {% block modal_content %}#} {# {% endblock %}#} {% for key, field in
 fields.items() %} {% if not field.auto %}
-{{ key }} {% with value=obj[field.name] if obj else None %} {% include
-"components/inputs/"+field.template+".html" %} {% endwith %}
+{{ key }} {% with value=obj[field.name] if obj else None,
+key=field.source_field or key %} {% include "components/inputs/
+"+field.input+".html" %} {% endwith %}
 {% endif %} {% endfor %}
 Cancel        {{ action }} {{ model }}
```

### Comparing `femto-admin-0.1.2/femto_admin/templates/components/notofications.html` & `femto-admin-0.2.0/femto_admin/templates/components/notofications.html`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.2/femto_admin/templates/table.html` & `femto-admin-0.2.0/femto_admin/templates/views/table.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-{% extends "layout.html" %}
+{% macro table() -%}
 
-{% block styles %}
     <link href="{{ url_for('public', path='vendor/DataTables/css/dataTables.bootstrap5.'+minify+'css') }}" rel="stylesheet"/>
-{% endblock %}
 
-{% block body %}
     <table id="dt" class="table table-striped" style="width:100%">
         <thead>
         <tr>
             {% for field in fields %}
                 {% if not field.endswith('_id') %}
                     <th>{{ field }}</th>
                 {% endif %}
             {% endfor %}
         </tr>
         </thead>
     </table>
-{% endblock %}
 
-{% block scripts %}
-    <script src="{{ url_for('public', path='vendor/DataTables/js/jquery.dataTables.'+minify+'js') }}"></script>
-    <script src="{{ url_for('public', path='vendor/DataTables/js/dataTables.bootstrap5.'+minify+'js') }}"></script>
-    <script>new DataTable('#dt', {ajax: 'dt/{{ request.path_params["model"] }}'})</script>
-{% endblock %}
+    <script defer src="{{ url_for('public', path='vendor/DataTables/js/jquery.dataTables.'+minify+'js') }}"></script>
+    <script defer src="{{ url_for('public', path='vendor/DataTables/js/dataTables.bootstrap5.'+minify+'js') }}"></script>
+    <script>
+        document.addEventListener("DOMContentLoaded", function () {
+            new DataTable('#dt', {ajax: 'dt/{{ request.path_params["model"] }}'})
+        });
+    </script>
+
+{% endmacro %}
```

#### html2text {}

```diff
@@ -1,5 +1,3 @@
-{% extends "layout.html" %} {% block styles %}
- {% endblock %} {% block body %}
+{% macro table() -%}
 {{ field }}
-{% endblock %} {% block scripts %}
- {% endblock %}
+ {% endmacro %}
```

### Comparing `femto-admin-0.1.2/femto_admin.egg-info/PKG-INFO` & `femto-admin-0.2.0/femto_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femto-admin
-Version: 0.1.2
+Version: 0.2.0
 Summary: Simplest fastest minimal ASGI CRUD Admin panel for Tortoise ORM models. It's generating fully native async auto  zero config one line app
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/femto-admin
 Project-URL: Repository, https://github.com/mixartemev/femto-admin
 Keywords: starlette,fastapi,admin,dashboard,datatables,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

### Comparing `femto-admin-0.1.2/femto_admin.egg-info/SOURCES.txt` & `femto-admin-0.2.0/femto_admin.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -30,28 +30,32 @@
 femto_admin/statics/vendor/tabler/css/tabler.css
 femto_admin/statics/vendor/tabler/css/tabler.min.css
 femto_admin/statics/vendor/tabler/js/dark-theme.js
 femto_admin/statics/vendor/tabler/js/dark-theme.min.js
 femto_admin/statics/vendor/tabler/js/tabler.js
 femto_admin/statics/vendor/tabler/js/tabler.min.js
 femto_admin/templates/dashboard.html
+femto_admin/templates/index.html
 femto_admin/templates/layout.html
-femto_admin/templates/table.html
+femto_admin/templates/components/aside.html
 femto_admin/templates/components/footer.html
 femto_admin/templates/components/global_actions.html
+femto_admin/templates/components/header.html
 femto_admin/templates/components/modal.html
 femto_admin/templates/components/notofications.html
 femto_admin/templates/components/inputs/_help.html
+femto_admin/templates/components/inputs/checkbox.html
+femto_admin/templates/components/inputs/collection.html
 femto_admin/templates/components/inputs/color.html
 femto_admin/templates/components/inputs/date.html
 femto_admin/templates/components/inputs/datetime.html
 femto_admin/templates/components/inputs/editor.html
 femto_admin/templates/components/inputs/image.html
 femto_admin/templates/components/inputs/input.html
 femto_admin/templates/components/inputs/json.html
+femto_admin/templates/components/inputs/list.html
 femto_admin/templates/components/inputs/many_to_many.html
-femto_admin/templates/components/inputs/point.html
-femto_admin/templates/components/inputs/polygon.html
 femto_admin/templates/components/inputs/radio.html
+femto_admin/templates/components/inputs/range.html
 femto_admin/templates/components/inputs/select.html
-femto_admin/templates/components/inputs/switch.html
-femto_admin/templates/components/inputs/textarea.html
+femto_admin/templates/components/inputs/textarea.html
+femto_admin/templates/views/table.html
```

### Comparing `femto-admin-0.1.2/pyproject.toml` & `femto-admin-0.2.0/pyproject.toml`

 * *Files identical despite different names*

