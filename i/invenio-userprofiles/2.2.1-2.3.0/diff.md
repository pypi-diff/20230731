# Comparing `tmp/invenio-userprofiles-2.2.1.tar.gz` & `tmp/invenio-userprofiles-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-userprofiles-2.2.1.tar", last modified: Fri May 26 08:06:16 2023, max compression
+gzip compressed data, was "dist/invenio-userprofiles-2.3.0.tar", last modified: Mon Jul 31 12:55:35 2023, max compression
```

## Comparing `invenio-userprofiles-2.2.1.tar` & `invenio-userprofiles-2.3.0.tar`

### file list

```diff
@@ -1,215 +1,271 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3785 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      362 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      857 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4887 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/babel.ini
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/constraints-pypi.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10438 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7009 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/alembic/
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/alembic/41157f1933d6_remove_table.py
--rw-r--r--   0 runner    (1001) docker     (122)      570 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/alembic/71634726ec7e_create_userprofiles_branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/alembic/c25ef2c50ffa_create_userprofiles_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     9949 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/forms.py
--rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/invenio_userprofiles/
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/invenio_userprofiles/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/invenio_userprofiles/register_user.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/invenio_userprofiles/settings/
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/invenio_userprofiles/settings/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/invenio_userprofiles/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/invenio_userprofiles/settings/profile.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/register_user.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      976 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4713 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3880 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     6885 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4881 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4947 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2164 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5630 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5345 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     6290 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4890 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2981 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     6184 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5883 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4728 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      726 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4913 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2263 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4712 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4940 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3097 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5984 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5678 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4880 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      745 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4962 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5001 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4863 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5012 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4912 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      650 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4898 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5028 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      524 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4715 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-05-26 08:06:15.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5660 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5872 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5626 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2873 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     5768 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4858 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/validators.py
--rw-r--r--   0 runner    (1001) docker     (122)     6051 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/invenio_userprofiles/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4887 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6258 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/invenio_userprofiles.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      463 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      347 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/run-i18n-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      754 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2281 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:06:16.000000 invenio-userprofiles-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3794 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1232 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3936 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (122)     1947 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/tests/test_invenio_userprofile.py
--rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (122)    11946 2023-05-26 08:06:04.000000 invenio-userprofiles-2.2.1/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2295 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3785 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      362 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      857 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5123 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/babel.ini
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10438 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7009 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)     2615 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/alembic/41157f1933d6_remove_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/alembic/71634726ec7e_create_userprofiles_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/alembic/c25ef2c50ffa_create_userprofiles_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9949 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/forms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/invenio_userprofiles/
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/invenio_userprofiles/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/invenio_userprofiles/register_user.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/invenio_userprofiles/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/invenio_userprofiles/settings/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/invenio_userprofiles/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/invenio_userprofiles/settings/profile.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/register_user.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      976 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4713 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3854 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     6859 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4881 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4947 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2164 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5630 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5345 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     6290 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4726 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4726 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4890 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2981 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4727 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4727 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     6184 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4763 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4765 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5883 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4728 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4913 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2263 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      593 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4776 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4712 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4940 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3096 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     6010 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      538 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4729 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5678 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4880 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      745 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4962 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5001 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4710 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4863 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5012 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4912 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5084 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5028 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4715 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5660 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5872 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4726 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5626 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4285 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     7192 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      760 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4951 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2873 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     5768 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4858 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/validators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6051 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/invenio_userprofiles/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5123 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8044 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/invenio_userprofiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-31 12:55:34.000000 invenio-userprofiles-2.3.0/invenio_userprofiles.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      347 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/run-i18n-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1504 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2281 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:55:35.000000 invenio-userprofiles-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3794 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1232 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1459 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3936 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1947 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/tests/test_invenio_userprofile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11946 2023-07-31 12:55:24.000000 invenio-userprofiles-2.3.0/tests/test_views.py
```

### Comparing `invenio-userprofiles-2.2.1/.editorconfig` & `invenio-userprofiles-2.3.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/.tx/config` & `invenio-userprofiles-2.3.0/.tx/config`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2018 CERN.
+# Copyright (C)      2023 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 
 # TODO: Transifex integration
 #
@@ -21,14 +22,14 @@
 #    $ tx push -s -t
 # 5) Pull translations for a single language from Transifex
 #    $ tx pull -l <lang>
 # 6) Pull translations for all languages from Transifex
 #    $ tx pull -a
 
 [main]
-host = https://www.transifex.com
+host = https://app.transifex.com
 
-[invenio.invenio-userprofiles-messages]
+[o:inveniosoftware:p:invenio:r:invenio-userprofiles-messages]
 file_filter = invenio_userprofiles/translations/<lang>/LC_MESSAGES/messages.po
 source_file = invenio_userprofiles/translations/messages.pot
 source_lang = en
 type = PO
```

### Comparing `invenio-userprofiles-2.2.1/AUTHORS.rst` & `invenio-userprofiles-2.3.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/CHANGES.rst` & `invenio-userprofiles-2.3.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.3.0 (released 2023-07-31)
+
+- settings profile: Update buttons with labeled styling and a11y fixes
+- alembic: fix recipe based on latest sqlalchemy-continuum
+- pull translations
+
 Version 2.2.1 (released 2023-05-26)
 
 - fix styling for locale preferences field
 
 Version 2.2.0 (released 2023-04-25)
 
 - add locale to user profile preferences
```

### Comparing `invenio-userprofiles-2.2.1/CONTRIBUTING.rst` & `invenio-userprofiles-2.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/LICENSE` & `invenio-userprofiles-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/MANIFEST.in` & `invenio-userprofiles-2.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/PKG-INFO` & `invenio-userprofiles-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-userprofiles
-Version: 2.2.1
+Version: 2.3.0
 Summary: User profiles module for Invenio.
 Home-page: https://github.com/inveniosoftware/invenio-userprofiles
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -46,14 +46,20 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.3.0 (released 2023-07-31)
+        
+        - settings profile: Update buttons with labeled styling and a11y fixes
+        - alembic: fix recipe based on latest sqlalchemy-continuum
+        - pull translations
+        
         Version 2.2.1 (released 2023-05-26)
         
         - fix styling for locale preferences field
         
         Version 2.2.0 (released 2023-04-25)
         
         - add locale to user profile preferences
```

### Comparing `invenio-userprofiles-2.2.1/README.rst` & `invenio-userprofiles-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/docs/Makefile` & `invenio-userprofiles-2.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/docs/api.rst` & `invenio-userprofiles-2.3.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/docs/conf.py` & `invenio-userprofiles-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/docs/index.rst` & `invenio-userprofiles-2.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/docs/make.bat` & `invenio-userprofiles-2.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/__init__.py` & `invenio-userprofiles-2.3.0/invenio_userprofiles/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     security.safe_str_cmp = hmac.compare_digest
 
 from .api import current_userprofile
 from .ext import InvenioUserProfiles
 from .models import UserProfile, UserProfileProxy
 
-__version__ = "2.2.1"
+__version__ = "2.3.0"
 
 __all__ = (
     "__version__",
     "current_userprofile",
     "InvenioUserProfiles",
     "UserProfile",
     "UserProfileProxy",
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/alembic/41157f1933d6_remove_table.py` & `invenio-userprofiles-2.3.0/invenio_userprofiles/alembic/41157f1933d6_remove_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,29 +8,32 @@
 
 """Remove table."""
 
 import json
 
 import sqlalchemy as sa
 from alembic import op
+from sqlalchemy.sql import text
 
 # revision identifiers, used by Alembic.
 revision = "41157f1933d6"
 down_revision = "c25ef2c50ffa"
 branch_labels = ()
 depends_on = "eb9743315a9d"  # invenio-accounts: add_userprofile
 
 
 def upgrade():
     """Upgrade database."""
     # Migrate username and full_name to invenio_accounts table.
     connection = op.get_bind()
     results = connection.execute(
-        "SELECT user_id, username, displayname, full_name "
-        "FROM userprofiles_userprofile;"
+        text(
+            "SELECT user_id, username, displayname, full_name "
+            "FROM userprofiles_userprofile;"
+        )
     ).all()
 
     for r in results:
         user_id, username, displayname, full_name = r
         profile_data = {
             "full_name": full_name,
         }
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/alembic/71634726ec7e_create_userprofiles_branch.py` & `invenio-userprofiles-2.3.0/invenio_userprofiles/alembic/71634726ec7e_create_userprofiles_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/alembic/c25ef2c50ffa_create_userprofiles_tables.py` & `invenio-userprofiles-2.3.0/invenio_userprofiles/alembic/c25ef2c50ffa_create_userprofiles_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/api.py` & `invenio-userprofiles-2.3.0/invenio_userprofiles/api.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/config.py` & `invenio-userprofiles-2.3.0/invenio_userprofiles/config.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/ext.py` & `invenio-userprofiles-2.3.0/invenio_userprofiles/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/forms.py` & `invenio-userprofiles-2.3.0/invenio_userprofiles/forms.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/models.py` & `invenio-userprofiles-2.3.0/invenio_userprofiles/models.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/templates/invenio_userprofiles/register_user.html` & `invenio-userprofiles-2.3.0/invenio_userprofiles/templates/invenio_userprofiles/register_user.html`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/templates/invenio_userprofiles/settings/_macros.html` & `invenio-userprofiles-2.3.0/invenio_userprofiles/templates/invenio_userprofiles/settings/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/templates/invenio_userprofiles/settings/profile.html` & `invenio-userprofiles-2.3.0/invenio_userprofiles/templates/invenio_userprofiles/settings/profile.html`

 * *Files 25% similar despite different names*

```diff
@@ -10,34 +10,37 @@
 
 {% from "invenio_userprofiles/settings/_macros.html" import render_field, form_errors %}
 
 {% set panel_title = _("Profile") %}
 {% set panel_icon = "fa fa-user" %}
 
 {%- block settings_form %}
-{%- if security.confirmable and not current_user.confirmed_at %}
-<form method="POST" role="form">
-{{ verification_form.csrf_token }}
-<div class="alert alert-warning">
-  {{ _("You have not yet verified your email address.") }} {{ verification_form.send_verification_email(class_="btn btn-default btn-xs") }}
-</div>
-<input type="hidden" name="submit" value="verification" />
-</form>
-{%- endif %}
-{%- set form = profile_form %}
-{%- set read_only = config.USERPROFILES_READ_ONLY %}
-<form method="POST" name="profile_form">
-{%- for field in form %}
-{%- if field.widget.input_type == 'hidden' %}
-{{ field() }}
-{%- elif not read_only or "repeat" not in field.id %}
-{{ render_field(field, autofocus=True, enabled=not read_only, placeholder=field.label.text) }}
-{%- endif %}
-{%- endfor %}
-{%- if not read_only %}
-<div class="form-actions">
-  <a href="." class="btn btn-default"><i class="fa fa-times"></i> {{ _('Cancel') }}</a>
-  <button type="submit" name="submit" value="profile" class="btn btn-primary"><i class="fa fa-check"></i> {{ _('Update profile') }}</button>
-</div>
-{%- endif %}
-</form>
+  {%- if security.confirmable and not current_user.confirmed_at %}
+    <form method="POST" role="form">
+      {{ verification_form.csrf_token }}
+      <div class="alert alert-warning">
+        {{ _("You have not yet verified your email address.") }} {{ verification_form.send_verification_email(class_="btn btn-default btn-xs") }}
+      </div>
+      <input type="hidden" name="submit" value="verification" />
+    </form>
+  {%- endif %}
+
+  {%- set form = profile_form %}
+  {%- set read_only = config.USERPROFILES_READ_ONLY %}
+
+  <form method="POST" name="profile_form">
+  {%- for field in form %}
+    {%- if field.widget.input_type == 'hidden' %}
+      {{ field() }}
+    {%- elif not read_only or "repeat" not in field.id %}
+      {{ render_field(field, autofocus=True, enabled=not read_only, placeholder=field.label.text) }}
+    {%- endif %}
+  {%- endfor %}
+
+  {%- if not read_only %}
+    <div class="form-actions">
+      <a href="." class="btn btn-default"><i class="fa fa-times"></i> {{ _('Cancel') }}</a>
+      <button type="submit" name="submit" value="profile" class="btn btn-primary"><i class="fa fa-check"></i> {{ _('Update profile') }}</button>
+    </div>
+  {%- endif %}
+  </form>
 {%- endblock settings_form %}
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/register_user.html` & `invenio-userprofiles-2.3.0/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/register_user.html`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/_macros.html` & `invenio-userprofiles-2.3.0/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html` & `invenio-userprofiles-2.3.0/invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html`

 * *Files 12% similar despite different names*

```diff
@@ -24,196 +24,240 @@
 00000170: 5f65 7272 6f72 7320 257d 0a0a 7b25 2073  _errors %}..{% s
 00000180: 6574 2070 616e 656c 5f74 6974 6c65 203d  et panel_title =
 00000190: 205f 2822 5072 6f66 696c 6522 2920 257d   _("Profile") %}
 000001a0: 0a7b 2520 7365 7420 7061 6e65 6c5f 6963  .{% set panel_ic
 000001b0: 6f6e 203d 2022 7573 6572 2069 636f 6e22  on = "user icon"
 000001c0: 2025 7d0a 0a7b 252d 2062 6c6f 636b 2073   %}..{%- block s
 000001d0: 6574 7469 6e67 735f 636f 6e74 656e 7420  ettings_content 
-000001e0: 7363 6f70 6564 2025 7d0a 3c64 6976 2063  scoped %}.<div c
-000001f0: 6c61 7373 3d22 7569 2073 6567 6d65 6e74  lass="ui segment
-00000200: 7322 3e0a 2020 3c64 6976 2063 6c61 7373  s">.  <div class
-00000210: 3d22 7569 2073 6567 6d65 6e74 2073 6563  ="ui segment sec
-00000220: 6f6e 6461 7279 223e 0a0a 2020 2020 7b25  ondary">..    {%
-00000230: 2d20 626c 6f63 6b20 7365 7474 696e 6773  - block settings
-00000240: 5f63 6f6e 7465 6e74 5f74 6974 6c65 2073  _content_title s
-00000250: 636f 7065 6420 257d 0a20 2020 2020 207b  coped %}.      {
-00000260: 252d 2069 6620 7061 6e65 6c5f 6963 6f6e  %- if panel_icon
-00000270: 2025 7d0a 0a20 2020 2020 2020 207b 252d   %}..        {%-
-00000280: 2062 6c6f 636b 2073 6574 7469 6e67 735f   block settings_
-00000290: 636f 6e74 656e 745f 7469 746c 655f 6963  content_title_ic
-000002a0: 6f6e 2073 636f 7065 6420 257d 0a20 2020  on scoped %}.   
-000002b0: 2020 2020 2020 203c 6920 636c 6173 733d         <i class=
-000002c0: 227b 7b20 7061 6e65 6c5f 6963 6f6e 207d  "{{ panel_icon }
-000002d0: 7d22 3e3c 2f69 3e0a 2020 2020 2020 2020  }"></i>.        
-000002e0: 7b25 2d20 656e 6462 6c6f 636b 2025 7d0a  {%- endblock %}.
-000002f0: 0a20 2020 2020 207b 252d 2065 6e64 6966  .      {%- endif
-00000300: 2025 7d0a 2020 2020 2020 3c73 7472 6f6e   %}.      <stron
-00000310: 6720 636c 6173 733d 2268 6561 6465 7220  g class="header 
-00000320: 6974 656d 223e 7b7b 2070 616e 656c 5f74  item">{{ panel_t
-00000330: 6974 6c65 7c64 6566 6175 6c74 2822 2229  itle|default("")
-00000340: 207d 7d3c 2f73 7472 6f6e 673e 0a20 2020   }}</strong>.   
-00000350: 207b 252d 2065 6e64 626c 6f63 6b20 257d   {%- endblock %}
-00000360: 0a0a 2020 3c2f 6469 763e 0a0a 2020 7b25  ..  </div>..  {%
-00000370: 2d20 626c 6f63 6b20 7365 7474 696e 6773  - block settings
-00000380: 5f62 6f64 7920 7363 6f70 6564 2025 7d0a  _body scoped %}.
-00000390: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000003a0: 7569 2073 6567 6d65 6e74 223e 0a20 2020  ui segment">.   
-000003b0: 2020 207b 252d 2062 6c6f 636b 2073 6574     {%- block set
-000003c0: 7469 6e67 735f 666f 726d 2025 7d0a 2020  tings_form %}.  
-000003d0: 2020 2020 7b25 2d20 6966 2073 6563 7572      {%- if secur
-000003e0: 6974 792e 636f 6e66 6972 6d61 626c 6520  ity.confirmable 
-000003f0: 616e 6420 6e6f 7420 6375 7272 656e 745f  and not current_
-00000400: 7573 6572 2e63 6f6e 6669 726d 6564 5f61  user.confirmed_a
-00000410: 7420 257d 0a20 2020 2020 203c 666f 726d  t %}.      <form
-00000420: 206d 6574 686f 643d 2250 4f53 5422 2072   method="POST" r
-00000430: 6f6c 653d 2266 6f72 6d22 3e0a 2020 2020  ole="form">.    
-00000440: 2020 2020 7b7b 2076 6572 6966 6963 6174      {{ verificat
-00000450: 696f 6e5f 666f 726d 2e63 7372 665f 746f  ion_form.csrf_to
-00000460: 6b65 6e20 7d7d 0a20 2020 2020 2020 203c  ken }}.        <
-00000470: 6469 7620 636c 6173 733d 2275 6920 7761  div class="ui wa
-00000480: 726e 696e 6720 6d65 7373 6167 6522 3e0a  rning message">.
-00000490: 2020 2020 2020 2020 2020 7b7b 205f 2822            {{ _("
-000004a0: 596f 7520 6861 7665 206e 6f74 2079 6574  You have not yet
-000004b0: 2076 6572 6966 6965 6420 796f 7572 2065   verified your e
-000004c0: 6d61 696c 2061 6464 7265 7373 2e22 2920  mail address.") 
-000004d0: 7d7d 207b 7b20 7665 7269 6669 6361 7469  }} {{ verificati
-000004e0: 6f6e 5f66 6f72 6d2e 7365 6e64 5f76 6572  on_form.send_ver
-000004f0: 6966 6963 6174 696f 6e5f 656d 6169 6c28  ification_email(
-00000500: 636c 6173 735f 3d22 636f 6d70 6163 7420  class_="compact 
-00000510: 7569 2073 6d61 6c6c 2062 6173 6963 2062  ui small basic b
-00000520: 7574 746f 6e22 2920 7d7d 0a20 2020 2020  utton") }}.     
-00000530: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00000540: 2020 3c69 6e70 7574 2074 7970 653d 2268    <input type="h
-00000550: 6964 6465 6e22 206e 616d 653d 2273 7562  idden" name="sub
-00000560: 6d69 7422 2076 616c 7565 3d22 7665 7269  mit" value="veri
-00000570: 6669 6361 7469 6f6e 2220 2f3e 0a20 2020  fication" />.   
-00000580: 2020 203c 2f66 6f72 6d3e 0a20 2020 2020     </form>.     
-00000590: 207b 252d 2065 6e64 6966 2025 7d0a 2020   {%- endif %}.  
-000005a0: 2020 2020 7b25 2d20 7365 7420 666f 726d      {%- set form
-000005b0: 203d 2070 726f 6669 6c65 5f66 6f72 6d20   = profile_form 
-000005c0: 257d 0a20 2020 2020 207b 252d 2073 6574  %}.      {%- set
-000005d0: 2072 6561 645f 6f6e 6c79 203d 2063 6f6e   read_only = con
-000005e0: 6669 672e 5553 4552 5052 4f46 494c 4553  fig.USERPROFILES
-000005f0: 5f52 4541 445f 4f4e 4c59 2025 7d0a 2020  _READ_ONLY %}.  
-00000600: 2020 2020 3c66 6f72 6d20 7b25 2069 6620      <form {% if 
-00000610: 6e6f 7420 7265 6164 5f6f 6e6c 7920 257d  not read_only %}
-00000620: 6d65 7468 6f64 3d22 504f 5354 227b 2520  method="POST"{% 
-00000630: 656e 6469 6620 257d 206e 616d 653d 2270  endif %} name="p
-00000640: 726f 6669 6c65 5f66 6f72 6d22 2063 6c61  rofile_form" cla
-00000650: 7373 3d22 7569 2066 6f72 6d22 3e0a 2020  ss="ui form">.  
-00000660: 2020 2020 2020 7b25 2d20 666f 7220 6669        {%- for fi
-00000670: 656c 6420 696e 2066 6f72 6d20 257d 0a20  eld in form %}. 
-00000680: 2020 2020 2020 207b 252d 2069 6620 6669         {%- if fi
-00000690: 656c 642e 7769 6467 6574 2e69 6e70 7574  eld.widget.input
-000006a0: 5f74 7970 6520 3d3d 2027 6869 6464 656e  _type == 'hidden
-000006b0: 2720 257d 0a20 2020 2020 2020 207b 7b20  ' %}.        {{ 
-000006c0: 6669 656c 6428 2920 7d7d 0a20 2020 2020  field() }}.     
-000006d0: 2020 207b 252d 2065 6c69 6620 6e6f 7420     {%- elif not 
-000006e0: 7265 6164 5f6f 6e6c 7920 6f72 2022 7265  read_only or "re
-000006f0: 7065 6174 2220 6e6f 7420 696e 2066 6965  peat" not in fie
-00000700: 6c64 2e69 6420 257d 0a20 2020 2020 2020  ld.id %}.       
-00000710: 207b 7b20 7265 6e64 6572 5f66 6965 6c64   {{ render_field
-00000720: 2866 6965 6c64 2c20 6175 746f 666f 6375  (field, autofocu
-00000730: 733d 5472 7565 2c20 656e 6162 6c65 643d  s=True, enabled=
-00000740: 6e6f 7420 7265 6164 5f6f 6e6c 792c 2070  not read_only, p
-00000750: 6c61 6365 686f 6c64 6572 3d66 6965 6c64  laceholder=field
-00000760: 2e6c 6162 656c 2e74 6578 7429 207d 7d0a  .label.text) }}.
-00000770: 2020 2020 2020 2020 7b25 2d20 656e 6469          {%- endi
-00000780: 6620 257d 0a20 2020 2020 2020 207b 252d  f %}.        {%-
-00000790: 2065 6e64 666f 7220 257d 0a20 2020 2020   endfor %}.     
-000007a0: 2020 207b 252d 2069 6620 6e6f 7420 7265     {%- if not re
-000007b0: 6164 5f6f 6e6c 7920 257d 0a20 2020 2020  ad_only %}.     
-000007c0: 2020 203c 6469 7620 636c 6173 733d 2266     <div class="f
-000007d0: 6f72 6d2d 6163 7469 6f6e 7322 3e0a 2020  orm-actions">.  
-000007e0: 2020 2020 2020 2020 3c61 2068 7265 663d          <a href=
-000007f0: 222e 2220 636c 6173 733d 2275 6920 6275  "." class="ui bu
-00000800: 7474 6f6e 223e 3c69 2063 6c61 7373 3d22  tton"><i class="
-00000810: 636c 6f73 6520 6963 6f6e 223e 3c2f 693e  close icon"></i>
-00000820: 207b 7b20 5f28 2743 616e 6365 6c27 2920   {{ _('Cancel') 
-00000830: 7d7d 3c2f 613e 0a20 2020 2020 2020 2020  }}</a>.         
-00000840: 203c 6275 7474 6f6e 2074 7970 653d 2273   <button type="s
-00000850: 7562 6d69 7422 206e 616d 653d 2273 7562  ubmit" name="sub
-00000860: 6d69 7422 2076 616c 7565 3d22 7072 6f66  mit" value="prof
-00000870: 696c 6522 2063 6c61 7373 3d22 7569 2070  ile" class="ui p
-00000880: 7269 6d61 7279 2062 7574 746f 6e22 3e3c  rimary button"><
-00000890: 6920 636c 6173 733d 2263 6865 636b 2069  i class="check i
-000008a0: 636f 6e22 3e3c 2f69 3e20 7b7b 205f 2827  con"></i> {{ _('
-000008b0: 5570 6461 7465 2070 726f 6669 6c65 2729  Update profile')
-000008c0: 207d 7d3c 2f62 7574 746f 6e3e 0a20 2020   }}</button>.   
-000008d0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-000008e0: 2020 2020 7b25 2d20 656e 6469 6620 257d      {%- endif %}
-000008f0: 0a20 2020 2020 203c 2f66 6f72 6d3e 0a20  .      </form>. 
-00000900: 2020 2020 207b 252d 2065 6e64 626c 6f63       {%- endbloc
-00000910: 6b20 7365 7474 696e 6773 5f66 6f72 6d20  k settings_form 
-00000920: 257d 0a20 2020 203c 2f64 6976 3e0a 2020  %}.    </div>.  
-00000930: 7b25 2d20 656e 6462 6c6f 636b 2073 6574  {%- endblock set
-00000940: 7469 6e67 735f 626f 6479 2025 7d0a 0a3c  tings_body %}..<
-00000950: 2f64 6976 3e0a 0a3c 6469 7620 636c 6173  /div>..<div clas
-00000960: 733d 2275 6920 7365 676d 656e 7473 223e  s="ui segments">
-00000970: 0a20 203c 6469 7620 636c 6173 733d 2275  .  <div class="u
-00000980: 6920 7365 676d 656e 7420 7365 636f 6e64  i segment second
-00000990: 6172 7922 3e0a 2020 2020 2020 3c69 2063  ary">.      <i c
-000009a0: 6c61 7373 3d22 736c 6964 6572 7320 686f  lass="sliders ho
-000009b0: 7269 7a6f 6e74 616c 2069 636f 6e22 3e3c  rizontal icon"><
-000009c0: 2f69 3e0a 2020 2020 2020 3c73 7472 6f6e  /i>.      <stron
-000009d0: 6720 636c 6173 733d 2268 6561 6465 7220  g class="header 
-000009e0: 6974 656d 223e 7b7b 205f 2822 5072 6566  item">{{ _("Pref
-000009f0: 6572 656e 6365 7322 2920 7d7d 3c2f 7374  erences") }}</st
-00000a00: 726f 6e67 3e0a 2020 3c2f 6469 763e 0a20  rong>.  </div>. 
-00000a10: 203c 6469 7620 636c 6173 733d 2275 6920   <div class="ui 
-00000a20: 7365 676d 656e 7422 3e0a 2020 2020 2020  segment">.      
-00000a30: 7b25 2d20 7365 7420 666f 726d 203d 2070  {%- set form = p
-00000a40: 7265 6665 7265 6e63 6573 5f66 6f72 6d20  references_form 
-00000a50: 257d 0a20 2020 2020 203c 666f 726d 207b  %}.      <form {
-00000a60: 2520 6966 206e 6f74 2072 6561 645f 6f6e  % if not read_on
-00000a70: 6c79 2025 7d6d 6574 686f 643d 2250 4f53  ly %}method="POS
-00000a80: 5422 7b25 2065 6e64 6966 2025 7d20 6e61  T"{% endif %} na
-00000a90: 6d65 3d22 7072 6566 6572 656e 6365 735f  me="preferences_
-00000aa0: 666f 726d 2220 636c 6173 733d 2275 6920  form" class="ui 
-00000ab0: 666f 726d 223e 0a20 2020 2020 2020 207b  form">.        {
-00000ac0: 252d 2066 6f72 2066 6965 6c64 2069 6e20  %- for field in 
-00000ad0: 666f 726d 2025 7d0a 2020 2020 2020 2020  form %}.        
-00000ae0: 2020 7b25 2d20 6966 2066 6965 6c64 2e77    {%- if field.w
-00000af0: 6964 6765 742e 696e 7075 745f 7479 7065  idget.input_type
-00000b00: 203d 3d20 2768 6964 6465 6e27 2025 7d0a   == 'hidden' %}.
-00000b10: 2020 2020 2020 2020 2020 2020 7b7b 2066              {{ f
-00000b20: 6965 6c64 2829 207d 7d0a 2020 2020 2020  ield() }}.      
-00000b30: 2020 2020 7b25 2d20 656c 6966 2066 6965      {%- elif fie
-00000b40: 6c64 2e74 7970 6520 3d3d 2027 5365 6c65  ld.type == 'Sele
-00000b50: 6374 4669 656c 6427 2025 7d0a 2020 2020  ctField' %}.    
-00000b60: 2020 2020 2020 2020 7b7b 2072 656e 6465          {{ rende
-00000b70: 725f 6669 656c 6428 6669 656c 642c 2066  r_field(field, f
-00000b80: 6965 6c64 5f63 6c61 7373 3d22 7569 2064  ield_class="ui d
-00000b90: 726f 7064 6f77 6e22 2920 7d7d 0a20 2020  ropdown") }}.   
-00000ba0: 2020 2020 2020 207b 252d 2065 6c73 6520         {%- else 
-00000bb0: 257d 0a20 2020 2020 2020 2020 2020 207b  %}.            {
-00000bc0: 7b20 7265 6e64 6572 5f66 6965 6c64 2866  { render_field(f
-00000bd0: 6965 6c64 2c20 706c 6163 6568 6f6c 6465  ield, placeholde
-00000be0: 723d 6669 656c 642e 6c61 6265 6c2e 7465  r=field.label.te
-00000bf0: 7874 2c20 6669 656c 645f 636c 6173 733d  xt, field_class=
-00000c00: 2266 6f72 6d2d 636f 6e74 726f 6c20 6e6f  "form-control no
-00000c10: 2d64 6f74 732d 6c69 7374 2070 6c2d 3022  -dots-list pl-0"
-00000c20: 2920 7d7d 0a20 2020 2020 2020 2020 207b  ) }}.          {
-00000c30: 252d 2065 6e64 6966 2025 7d0a 2020 2020  %- endif %}.    
-00000c40: 2020 2020 7b25 2d20 656e 6466 6f72 2025      {%- endfor %
-00000c50: 7d0a 2020 2020 2020 2020 3c64 6976 2063  }.        <div c
-00000c60: 6c61 7373 3d22 666f 726d 2d61 6374 696f  lass="form-actio
-00000c70: 6e73 223e 0a20 2020 2020 2020 2020 203c  ns">.          <
-00000c80: 6120 6872 6566 3d22 2e22 2063 6c61 7373  a href="." class
-00000c90: 3d22 7569 2062 7574 746f 6e22 3e3c 6920  ="ui button"><i 
-00000ca0: 636c 6173 733d 2263 6c6f 7365 2069 636f  class="close ico
-00000cb0: 6e22 3e3c 2f69 3e20 7b7b 205f 2827 4361  n"></i> {{ _('Ca
-00000cc0: 6e63 656c 2729 207d 7d3c 2f61 3e0a 2020  ncel') }}</a>.  
-00000cd0: 2020 2020 2020 2020 3c62 7574 746f 6e20          <button 
-00000ce0: 7479 7065 3d22 7375 626d 6974 2220 6e61  type="submit" na
-00000cf0: 6d65 3d22 7375 626d 6974 2220 7661 6c75  me="submit" valu
-00000d00: 653d 2270 7265 6665 7265 6e63 6573 2220  e="preferences" 
-00000d10: 636c 6173 733d 2275 6920 7072 696d 6172  class="ui primar
-00000d20: 7920 6275 7474 6f6e 223e 3c69 2063 6c61  y button"><i cla
-00000d30: 7373 3d22 6368 6563 6b20 6963 6f6e 223e  ss="check icon">
-00000d40: 3c2f 693e 207b 7b20 5f28 2755 7064 6174  </i> {{ _('Updat
-00000d50: 6520 7072 6566 6572 656e 6365 7327 2920  e preferences') 
-00000d60: 7d7d 3c2f 6275 7474 6f6e 3e0a 2020 2020  }}</button>.    
-00000d70: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00000d80: 203c 2f66 6f72 6d3e 0a20 203c 2f64 6976   </form>.  </div
-00000d90: 3e0a 7b25 2065 6e64 626c 6f63 6b20 257d  >.{% endblock %}
-00000da0: 0a                                       .
+000001e0: 7363 6f70 6564 2025 7d0a 2020 3c73 6563  scoped %}.  <sec
+000001f0: 7469 6f6e 2061 7269 612d 6c61 6265 6c3d  tion aria-label=
+00000200: 227b 7b20 5f28 7061 6e65 6c5f 7469 746c  "{{ _(panel_titl
+00000210: 657c 6465 6661 756c 7428 2727 2929 207d  e|default('')) }
+00000220: 7d22 2063 6c61 7373 3d22 7569 2073 6567  }" class="ui seg
+00000230: 6d65 6e74 7322 3e0a 2020 2020 3c64 6976  ments">.    <div
+00000240: 2063 6c61 7373 3d22 7569 2073 6567 6d65   class="ui segme
+00000250: 6e74 2073 6563 6f6e 6461 7279 223e 0a0a  nt secondary">..
+00000260: 2020 2020 2020 7b25 2d20 626c 6f63 6b20        {%- block 
+00000270: 7365 7474 696e 6773 5f63 6f6e 7465 6e74  settings_content
+00000280: 5f74 6974 6c65 2073 636f 7065 6420 257d  _title scoped %}
+00000290: 0a20 2020 2020 2020 207b 252d 2069 6620  .        {%- if 
+000002a0: 7061 6e65 6c5f 6963 6f6e 2025 7d0a 0a20  panel_icon %}.. 
+000002b0: 2020 2020 2020 2020 207b 252d 2062 6c6f           {%- blo
+000002c0: 636b 2073 6574 7469 6e67 735f 636f 6e74  ck settings_cont
+000002d0: 656e 745f 7469 746c 655f 6963 6f6e 2073  ent_title_icon s
+000002e0: 636f 7065 6420 257d 0a20 2020 2020 2020  coped %}.       
+000002f0: 2020 2020 203c 6920 636c 6173 733d 227b       <i class="{
+00000300: 7b20 7061 6e65 6c5f 6963 6f6e 207d 7d22  { panel_icon }}"
+00000310: 2061 7269 612d 6869 6464 656e 3d22 7472   aria-hidden="tr
+00000320: 7565 223e 3c2f 693e 0a20 2020 2020 2020  ue"></i>.       
+00000330: 2020 207b 252d 2065 6e64 626c 6f63 6b20     {%- endblock 
+00000340: 257d 0a0a 2020 2020 2020 2020 7b25 2d20  %}..        {%- 
+00000350: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+00000360: 203c 6832 2063 6c61 7373 3d22 7569 2074   <h2 class="ui t
+00000370: 696e 7920 6865 6164 6572 2069 6e6c 696e  iny header inlin
+00000380: 652d 626c 6f63 6b20 6d2d 3022 3e7b 7b20  e-block m-0">{{ 
+00000390: 7061 6e65 6c5f 7469 746c 657c 6465 6661  panel_title|defa
+000003a0: 756c 7428 2222 2920 7d7d 3c2f 6832 3e0a  ult("") }}</h2>.
+000003b0: 2020 2020 2020 7b25 2d20 656e 6462 6c6f        {%- endblo
+000003c0: 636b 2025 7d0a 0a20 2020 203c 2f64 6976  ck %}..    </div
+000003d0: 3e0a 0a20 2020 207b 252d 2062 6c6f 636b  >..    {%- block
+000003e0: 2073 6574 7469 6e67 735f 626f 6479 2073   settings_body s
+000003f0: 636f 7065 6420 257d 0a20 2020 2020 203c  coped %}.      <
+00000400: 6469 7620 636c 6173 733d 2275 6920 7365  div class="ui se
+00000410: 676d 656e 7422 3e0a 0a20 2020 2020 2020  gment">..       
+00000420: 207b 252d 2062 6c6f 636b 2073 6574 7469   {%- block setti
+00000430: 6e67 735f 666f 726d 2025 7d0a 2020 2020  ngs_form %}.    
+00000440: 2020 2020 2020 7b25 2d20 6966 2073 6563        {%- if sec
+00000450: 7572 6974 792e 636f 6e66 6972 6d61 626c  urity.confirmabl
+00000460: 6520 616e 6420 6e6f 7420 6375 7272 656e  e and not curren
+00000470: 745f 7573 6572 2e63 6f6e 6669 726d 6564  t_user.confirmed
+00000480: 5f61 7420 257d 0a20 2020 2020 2020 2020  _at %}.         
+00000490: 2020 203c 666f 726d 206d 6574 686f 643d     <form method=
+000004a0: 2250 4f53 5422 2072 6f6c 653d 2266 6f72  "POST" role="for
+000004b0: 6d22 3e0a 2020 2020 2020 2020 2020 2020  m">.            
+000004c0: 2020 7b7b 2076 6572 6966 6963 6174 696f    {{ verificatio
+000004d0: 6e5f 666f 726d 2e63 7372 665f 746f 6b65  n_form.csrf_toke
+000004e0: 6e20 7d7d 0a20 2020 2020 2020 2020 2020  n }}.           
+000004f0: 2020 203c 6469 7620 636c 6173 733d 2275     <div class="u
+00000500: 6920 7761 726e 696e 6720 6d65 7373 6167  i warning messag
+00000510: 6522 3e0a 2020 2020 2020 2020 2020 2020  e">.            
+00000520: 2020 2020 7b7b 205f 2822 596f 7520 6861      {{ _("You ha
+00000530: 7665 206e 6f74 2079 6574 2076 6572 6966  ve not yet verif
+00000540: 6965 6420 796f 7572 2065 6d61 696c 2061  ied your email a
+00000550: 6464 7265 7373 2e22 2920 7d7d 207b 7b20  ddress.") }} {{ 
+00000560: 7665 7269 6669 6361 7469 6f6e 5f66 6f72  verification_for
+00000570: 6d2e 7365 6e64 5f76 6572 6966 6963 6174  m.send_verificat
+00000580: 696f 6e5f 656d 6169 6c28 636c 6173 735f  ion_email(class_
+00000590: 3d22 636f 6d70 6163 7420 7569 2073 6d61  ="compact ui sma
+000005a0: 6c6c 2062 6173 6963 2062 7574 746f 6e22  ll basic button"
+000005b0: 2920 7d7d 0a20 2020 2020 2020 2020 2020  ) }}.           
+000005c0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+000005d0: 2020 2020 2020 2020 3c69 6e70 7574 2074          <input t
+000005e0: 7970 653d 2268 6964 6465 6e22 206e 616d  ype="hidden" nam
+000005f0: 653d 2273 7562 6d69 7422 2076 616c 7565  e="submit" value
+00000600: 3d22 7665 7269 6669 6361 7469 6f6e 2220  ="verification" 
+00000610: 2f3e 0a20 2020 2020 2020 2020 2020 203c  />.            <
+00000620: 2f66 6f72 6d3e 0a20 2020 2020 2020 2020  /form>.         
+00000630: 207b 252d 2065 6e64 6966 2025 7d0a 0a20   {%- endif %}.. 
+00000640: 2020 2020 2020 2020 207b 252d 2073 6574           {%- set
+00000650: 2066 6f72 6d20 3d20 7072 6f66 696c 655f   form = profile_
+00000660: 666f 726d 2025 7d0a 2020 2020 2020 2020  form %}.        
+00000670: 2020 7b25 2d20 7365 7420 7265 6164 5f6f    {%- set read_o
+00000680: 6e6c 7920 3d20 636f 6e66 6967 2e55 5345  nly = config.USE
+00000690: 5250 524f 4649 4c45 535f 5245 4144 5f4f  RPROFILES_READ_O
+000006a0: 4e4c 5920 257d 0a0a 2020 2020 2020 2020  NLY %}..        
+000006b0: 2020 3c66 6f72 6d20 7b25 2069 6620 6e6f    <form {% if no
+000006c0: 7420 7265 6164 5f6f 6e6c 7920 257d 6d65  t read_only %}me
+000006d0: 7468 6f64 3d22 504f 5354 227b 2520 656e  thod="POST"{% en
+000006e0: 6469 6620 257d 206e 616d 653d 2270 726f  dif %} name="pro
+000006f0: 6669 6c65 5f66 6f72 6d22 2063 6c61 7373  file_form" class
+00000700: 3d22 7569 2066 6f72 6d22 3e0a 2020 2020  ="ui form">.    
+00000710: 2020 2020 2020 2020 7b25 2d20 666f 7220          {%- for 
+00000720: 6669 656c 6420 696e 2066 6f72 6d20 257d  field in form %}
+00000730: 0a20 2020 2020 2020 2020 2020 2020 207b  .              {
+00000740: 252d 2069 6620 6669 656c 642e 7769 6467  %- if field.widg
+00000750: 6574 2e69 6e70 7574 5f74 7970 6520 3d3d  et.input_type ==
+00000760: 2027 6869 6464 656e 2720 257d 0a20 2020   'hidden' %}.   
+00000770: 2020 2020 2020 2020 2020 2020 207b 7b20               {{ 
+00000780: 6669 656c 6428 2920 7d7d 0a20 2020 2020  field() }}.     
+00000790: 2020 2020 2020 2020 207b 252d 2065 6c69           {%- eli
+000007a0: 6620 6e6f 7420 7265 6164 5f6f 6e6c 7920  f not read_only 
+000007b0: 6f72 2022 7265 7065 6174 2220 6e6f 7420  or "repeat" not 
+000007c0: 696e 2066 6965 6c64 2e69 6420 257d 0a20  in field.id %}. 
+000007d0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+000007e0: 7b20 7265 6e64 6572 5f66 6965 6c64 2866  { render_field(f
+000007f0: 6965 6c64 2c20 6175 746f 666f 6375 733d  ield, autofocus=
+00000800: 5472 7565 2c20 656e 6162 6c65 643d 6e6f  True, enabled=no
+00000810: 7420 7265 6164 5f6f 6e6c 792c 2070 6c61  t read_only, pla
+00000820: 6365 686f 6c64 6572 3d66 6965 6c64 2e6c  ceholder=field.l
+00000830: 6162 656c 2e74 6578 7429 207d 7d0a 2020  abel.text) }}.  
+00000840: 2020 2020 2020 2020 2020 2020 7b25 2d20              {%- 
+00000850: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+00000860: 2020 2020 207b 252d 2065 6e64 666f 7220       {%- endfor 
+00000870: 257d 0a0a 2020 2020 2020 2020 2020 2020  %}..            
+00000880: 7b25 2d20 6966 206e 6f74 2072 6561 645f  {%- if not read_
+00000890: 6f6e 6c79 2025 7d0a 2020 2020 2020 2020  only %}.        
+000008a0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+000008b0: 3d22 666f 726d 2d61 6374 696f 6e73 223e  ="form-actions">
+000008c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000008d0: 203c 6120 726f 6c65 3d22 6275 7474 6f6e   <a role="button
+000008e0: 2220 6872 6566 3d22 2e22 2063 6c61 7373  " href="." class
+000008f0: 3d22 7569 206c 6162 656c 6564 2069 636f  ="ui labeled ico
+00000900: 6e20 6275 7474 6f6e 223e 0a20 2020 2020  n button">.     
+00000910: 2020 2020 2020 2020 2020 2020 203c 6920               <i 
+00000920: 636c 6173 733d 2263 6c6f 7365 2069 636f  class="close ico
+00000930: 6e22 2061 7269 612d 6869 6464 656e 3e3c  n" aria-hidden><
+00000940: 2f69 3e0a 2020 2020 2020 2020 2020 2020  /i>.            
+00000950: 2020 2020 2020 7b7b 205f 2827 4361 6e63        {{ _('Canc
+00000960: 656c 2729 207d 7d0a 2020 2020 2020 2020  el') }}.        
+00000970: 2020 2020 2020 2020 3c2f 613e 0a0a 2020          </a>..  
+00000980: 2020 2020 2020 2020 2020 2020 2020 3c62                <b
+00000990: 7574 746f 6e20 7479 7065 3d22 7375 626d  utton type="subm
+000009a0: 6974 2220 6e61 6d65 3d22 7375 626d 6974  it" name="submit
+000009b0: 2220 7661 6c75 653d 2270 726f 6669 6c65  " value="profile
+000009c0: 2220 636c 6173 733d 2275 6920 7072 696d  " class="ui prim
+000009d0: 6172 7920 6c61 6265 6c65 6420 6963 6f6e  ary labeled icon
+000009e0: 2062 7574 746f 6e22 3e0a 2020 2020 2020   button">.      
+000009f0: 2020 2020 2020 2020 2020 2020 3c69 2063              <i c
+00000a00: 6c61 7373 3d22 6368 6563 6b20 6963 6f6e  lass="check icon
+00000a10: 2220 6172 6961 2d68 6964 6465 6e3d 2274  " aria-hidden="t
+00000a20: 7275 6522 3e3c 2f69 3e0a 2020 2020 2020  rue"></i>.      
+00000a30: 2020 2020 2020 2020 2020 2020 7b7b 205f              {{ _
+00000a40: 2827 5570 6461 7465 2070 726f 6669 6c65  ('Update profile
+00000a50: 2729 207d 7d0a 2020 2020 2020 2020 2020  ') }}.          
+00000a60: 2020 2020 2020 3c2f 6275 7474 6f6e 3e0a        </button>.
+00000a70: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00000a80: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00000a90: 207b 252d 2065 6e64 6966 2025 7d0a 2020   {%- endif %}.  
+00000aa0: 2020 2020 2020 2020 3c2f 666f 726d 3e0a          </form>.
+00000ab0: 2020 2020 2020 2020 7b25 2d20 656e 6462          {%- endb
+00000ac0: 6c6f 636b 2073 6574 7469 6e67 735f 666f  lock settings_fo
+00000ad0: 726d 2025 7d0a 2020 2020 2020 3c2f 6469  rm %}.      </di
+00000ae0: 763e 0a20 2020 207b 252d 2065 6e64 626c  v>.    {%- endbl
+00000af0: 6f63 6b20 7365 7474 696e 6773 5f62 6f64  ock settings_bod
+00000b00: 7920 257d 0a20 2020 203c 2f73 6563 7469  y %}.    </secti
+00000b10: 6f6e 3e0a 0a20 203c 7365 6374 696f 6e20  on>..  <section 
+00000b20: 6172 6961 2d6c 6162 656c 3d22 7b7b 205f  aria-label="{{ _
+00000b30: 2827 5072 6566 6572 656e 6365 7327 2920  ('Preferences') 
+00000b40: 7d7d 2220 636c 6173 733d 2275 6920 7365  }}" class="ui se
+00000b50: 676d 656e 7473 223e 0a20 2020 203c 6469  gments">.    <di
+00000b60: 7620 636c 6173 733d 2275 6920 7365 676d  v class="ui segm
+00000b70: 656e 7420 7365 636f 6e64 6172 7922 3e0a  ent secondary">.
+00000b80: 2020 2020 2020 3c69 2063 6c61 7373 3d22        <i class="
+00000b90: 736c 6964 6572 7320 686f 7269 7a6f 6e74  sliders horizont
+00000ba0: 616c 2069 636f 6e22 2061 7269 612d 6869  al icon" aria-hi
+00000bb0: 6464 656e 3d22 7472 7565 223e 3c2f 693e  dden="true"></i>
+00000bc0: 0a20 2020 2020 203c 6832 2063 6c61 7373  .      <h2 class
+00000bd0: 3d22 7569 2074 696e 7920 6865 6164 6572  ="ui tiny header
+00000be0: 2069 6e6c 696e 652d 626c 6f63 6b20 6d2d   inline-block m-
+00000bf0: 3022 3e0a 2020 2020 2020 2020 7b7b 205f  0">.        {{ _
+00000c00: 2822 5072 6566 6572 656e 6365 7322 2920  ("Preferences") 
+00000c10: 7d7d 0a20 2020 2020 203c 2f68 323e 0a20  }}.      </h2>. 
+00000c20: 2020 203c 2f64 6976 3e0a 0a20 2020 203c     </div>..    <
+00000c30: 6469 7620 636c 6173 733d 2275 6920 7365  div class="ui se
+00000c40: 676d 656e 7422 3e0a 2020 2020 2020 7b25  gment">.      {%
+00000c50: 2d20 7365 7420 666f 726d 203d 2070 7265  - set form = pre
+00000c60: 6665 7265 6e63 6573 5f66 6f72 6d20 257d  ferences_form %}
+00000c70: 0a0a 2020 2020 2020 3c66 6f72 6d20 7b25  ..      <form {%
+00000c80: 2069 6620 6e6f 7420 7265 6164 5f6f 6e6c   if not read_onl
+00000c90: 7920 257d 6d65 7468 6f64 3d22 504f 5354  y %}method="POST
+00000ca0: 227b 2520 656e 6469 6620 257d 206e 616d  "{% endif %} nam
+00000cb0: 653d 2270 7265 6665 7265 6e63 6573 5f66  e="preferences_f
+00000cc0: 6f72 6d22 2063 6c61 7373 3d22 7569 2066  orm" class="ui f
+00000cd0: 6f72 6d22 3e0a 2020 2020 2020 2020 7b25  orm">.        {%
+00000ce0: 2d20 666f 7220 6669 656c 6420 696e 2066  - for field in f
+00000cf0: 6f72 6d20 257d 0a20 2020 2020 2020 2020  orm %}.         
+00000d00: 207b 252d 2069 6620 6669 656c 642e 7769   {%- if field.wi
+00000d10: 6467 6574 2e69 6e70 7574 5f74 7970 6520  dget.input_type 
+00000d20: 3d3d 2027 6869 6464 656e 2720 257d 0a20  == 'hidden' %}. 
+00000d30: 2020 2020 2020 2020 2020 207b 7b20 6669             {{ fi
+00000d40: 656c 6428 2920 7d7d 0a20 2020 2020 2020  eld() }}.       
+00000d50: 2020 207b 252d 2065 6c69 6620 6669 656c     {%- elif fiel
+00000d60: 642e 7479 7065 203d 3d20 2753 656c 6563  d.type == 'Selec
+00000d70: 7446 6965 6c64 2720 257d 0a20 2020 2020  tField' %}.     
+00000d80: 2020 2020 2020 207b 7b20 7265 6e64 6572         {{ render
+00000d90: 5f66 6965 6c64 2866 6965 6c64 2c20 6669  _field(field, fi
+00000da0: 656c 645f 636c 6173 733d 2275 6920 6472  eld_class="ui dr
+00000db0: 6f70 646f 776e 2229 207d 7d0a 2020 2020  opdown") }}.    
+00000dc0: 2020 2020 2020 7b25 2d20 656c 7365 2025        {%- else %
+00000dd0: 7d0a 2020 2020 2020 2020 2020 2020 7b7b  }.            {{
+00000de0: 2072 656e 6465 725f 6669 656c 6428 6669   render_field(fi
+00000df0: 656c 642c 2070 6c61 6365 686f 6c64 6572  eld, placeholder
+00000e00: 3d66 6965 6c64 2e6c 6162 656c 2e74 6578  =field.label.tex
+00000e10: 742c 2066 6965 6c64 5f63 6c61 7373 3d22  t, field_class="
+00000e20: 666f 726d 2d63 6f6e 7472 6f6c 206e 6f2d  form-control no-
+00000e30: 646f 7473 2d6c 6973 7420 706c 2d30 2229  dots-list pl-0")
+00000e40: 207d 7d0a 2020 2020 2020 2020 2020 7b25   }}.          {%
+00000e50: 2d20 656e 6469 6620 257d 0a20 2020 2020  - endif %}.     
+00000e60: 2020 207b 252d 2065 6e64 666f 7220 257d     {%- endfor %}
+00000e70: 0a0a 2020 2020 2020 2020 3c64 6976 2063  ..        <div c
+00000e80: 6c61 7373 3d22 666f 726d 2d61 6374 696f  lass="form-actio
+00000e90: 6e73 223e 0a20 2020 2020 2020 2020 203c  ns">.          <
+00000ea0: 6120 726f 6c65 3d22 6275 7474 6f6e 2220  a role="button" 
+00000eb0: 6872 6566 3d22 2e22 2063 6c61 7373 3d22  href="." class="
+00000ec0: 7569 206c 6162 656c 6564 2069 636f 6e20  ui labeled icon 
+00000ed0: 6275 7474 6f6e 223e 0a20 2020 2020 2020  button">.       
+00000ee0: 2020 2020 203c 6920 636c 6173 733d 2263       <i class="c
+00000ef0: 6c6f 7365 2069 636f 6e22 2061 7269 612d  lose icon" aria-
+00000f00: 6869 6464 656e 3d22 7472 7565 223e 3c2f  hidden="true"></
+00000f10: 693e 0a20 2020 2020 2020 2020 2020 207b  i>.            {
+00000f20: 7b20 5f28 2743 616e 6365 6c27 2920 7d7d  { _('Cancel') }}
+00000f30: 0a20 2020 2020 2020 2020 203c 2f61 3e0a  .          </a>.
+00000f40: 2020 2020 2020 2020 2020 3c62 7574 746f            <butto
+00000f50: 6e20 7479 7065 3d22 7375 626d 6974 2220  n type="submit" 
+00000f60: 6e61 6d65 3d22 7375 626d 6974 2220 7661  name="submit" va
+00000f70: 6c75 653d 2270 7265 6665 7265 6e63 6573  lue="preferences
+00000f80: 2220 636c 6173 733d 2275 6920 7072 696d  " class="ui prim
+00000f90: 6172 7920 6c61 6265 6c65 6420 6963 6f6e  ary labeled icon
+00000fa0: 2062 7574 746f 6e22 3e0a 2020 2020 2020   button">.      
+00000fb0: 2020 2020 2020 3c69 2063 6c61 7373 3d22        <i class="
+00000fc0: 6368 6563 6b20 6963 6f6e 2220 6172 6961  check icon" aria
+00000fd0: 2d68 6964 6465 6e3d 2274 7275 6522 3e3c  -hidden="true"><
+00000fe0: 2f69 3e0a 2020 2020 2020 2020 2020 2020  /i>.            
+00000ff0: 7b7b 205f 2827 5570 6461 7465 2070 7265  {{ _('Update pre
+00001000: 6665 7265 6e63 6573 2729 207d 7d0a 2020  ferences') }}.  
+00001010: 2020 2020 2020 2020 3c2f 6275 7474 6f6e          </button
+00001020: 3e0a 2020 2020 2020 2020 3c2f 6469 763e  >.        </div>
+00001030: 0a20 2020 2020 203c 2f66 6f72 6d3e 0a20  .      </form>. 
+00001040: 2020 203c 2f64 6976 3e0a 2020 3c2f 7365     </div>.  </se
+00001050: 6374 696f 6e3e 0a7b 2520 656e 6462 6c6f  ction>.{% endblo
+00001060: 636b 2025 7d0a                           ck %}.
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/af/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/af/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-userprofiles 2.0.3*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 4461 7465 3a20 3230 3136 2d30 382d 3138  Date: 2016-08-18
 000000d0: 2031 343a 3134 2b30 3030 300a 4c61 7374   14:14+0000.Last
 000000e0: 2d54 7261 6e73 6c61 746f 723a 2046 554c  -Translator: FUL
 000000f0: 4c20 4e41 4d45 203c 454d 4149 4c40 4144  L NAME <EMAIL@AD
 00000100: 4452 4553 533e 0a4c 616e 6775 6167 653a  DRESS>.Language:
 00000110: 2061 660a 4c61 6e67 7561 6765 2d54 6561   af.Language-Tea
 00000120: 6d3a 2041 6672 696b 6161 6e73 2028 6874  m: Afrikaans (ht
-00000130: 7470 733a 2f2f 7777 772e 7472 616e 7369  tps://www.transi
+00000130: 7470 733a 2f2f 6170 702e 7472 616e 7369  tps://app.transi
 00000140: 6665 782e 636f 6d2f 696e 7665 6e69 6f73  fex.com/invenios
 00000150: 6f66 7477 6172 652f 7465 616d 732f 3233  oftware/teams/23
 00000160: 3533 372f 6166 2f29 0a50 6c75 7261 6c2d  537/af/).Plural-
 00000170: 466f 726d 733a 206e 706c 7572 616c 733d  Forms: nplurals=
 00000180: 323b 2070 6c75 7261 6c3d 286e 2021 3d20  2; plural=(n != 
 00000190: 3129 3b0a 4d49 4d45 2d56 6572 7369 6f6e  1);.MIME-Version
 000001a0: 3a20 312e 300a 436f 6e74 656e 742d 5479  : 1.0.Content-Ty
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/af/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/af/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
-"Language-Team: Afrikaans (https://www.transifex.com/inveniosoftware/teams/23537/af/)\n"
+"Language-Team: Afrikaans (https://app.transifex.com/inveniosoftware/teams/23537/af/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: af\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ar/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ar/LC_MESSAGES/messages.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
-"Last-Translator: Bessem Aamira <bessemamira@gmail.com>, 2022\n"
+"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023\n"
 "Language: ar\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/"
 "ar/)\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
@@ -27,15 +27,15 @@
 msgid "Email address"
 msgstr "عنوان البريد الإلكتروني"
 
 msgid "Email addresses do not match."
 msgstr "عناوين البريد الإلكتروني غير متطابقة."
 
 msgid "Email visibility"
-msgstr "رؤية عنوان البريد الالكتروني"
+msgstr "مرئيّة عنوان البريد الالكتروني"
 
 msgid "Full name"
 msgstr "الإسم الكامل"
 
 msgid "Hidden"
 msgstr "مخفي"
 
@@ -48,54 +48,54 @@
 msgid "Preferences were updated."
 msgstr "تم تحيين الإعدادات."
 
 msgid "Profile"
 msgstr "الملف الشّخصي"
 
 msgid "Profile visibility"
-msgstr "رؤية الملف الشخصي"
+msgstr "مرئيّة الملف الشخصي"
 
 msgid "Profile was updated."
 msgstr "وقع تحديث الملف الشّخصي"
 
 msgid ""
 "Profile was updated. We have sent a verification email to %(email)s. Please "
 "check it."
 msgstr ""
 "وقع تحديث الملف الشّخصي. أرسلنا بريدا للتّثبّت إلى %(email)s. فالرجاء التّأكّد."
 
 msgid "Public"
-msgstr "عام"
+msgstr "مشاع"
 
 msgid ""
 "Public email visibility enables your profile to be found by your email "
 "address."
 msgstr ""
-"تتيح رؤية عنوان البريد الإلكتروني المضمن بالملف الشخصي للعامة إمكانية البحث "
-"و ايجاد ملف الحساب الشخصي عبر بريده الإلكتروني. "
+"تتيح مرئية عنوان البريد الإلكتروني للعامة إمكانية إيجاد ملف حسابك الشخصي عبر "
+"بريدك الإلكتروني. "
 
 msgid ""
 "Public profiles can be found by other users via searches on username, full "
 "name and affiliation. Hidden profiles cannot be found by other users."
 msgstr ""
 "الملفات الشخصية العامة يمكن البحث عنها من قبل المستخدمين الآخرين عن طريق اسم "
-"المستخدم و الاسم الكامل و الانتماءات. الملفات الخصية الخفية لا يمكن إيجادها "
+"المستخدم و الاسم الكامل و الانتماءات. الملفات الشّخصية الخفية لا يمكن إيجادها "
 "من قبل بقية المستخدمين."
 
 msgid "Re-enter email address"
 msgstr "أعد كتابة عنوان البريد الإلكتروني"
 
 msgid "Required. %(username_rules)s"
 msgstr "ضروري. %(username_rules)s"
 
 msgid "Resend verification email"
 msgstr "أعد إرسال بريد التثبّت"
 
 msgid "Update preferences"
-msgstr "تحيين الأعدادات"
+msgstr "تحيين الإعدادات"
 
 msgid "Update profile"
 msgstr "تحديث الملف الشّخصي"
 
 msgid "Username"
 msgstr "اسم المستخدم"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ar/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ar/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-userprofiles project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2016
-# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022
 # Bessem Aamira <bessemamira@gmail.com>, 2022
+# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
-"Last-Translator: Bessem Aamira <bessemamira@gmail.com>, 2022\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/ar/)\n"
+"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023\n"
+"Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
@@ -78,44 +78,44 @@
 #. NOTE: Form button label
 #: invenio_userprofiles/forms.py:151
 msgid "Resend verification email"
 msgstr "أعد إرسال بريد التثبّت"
 
 #: invenio_userprofiles/forms.py:190
 msgid "Profile visibility"
-msgstr "رؤية الملف الشخصي"
+msgstr "مرئيّة الملف الشخصي"
 
 #: invenio_userprofiles/forms.py:192 invenio_userprofiles/forms.py:205
 msgid "Public"
-msgstr "عام"
+msgstr "مشاع"
 
 #: invenio_userprofiles/forms.py:193 invenio_userprofiles/forms.py:206
 msgid "Hidden"
 msgstr "مخفي"
 
 #: invenio_userprofiles/forms.py:195
 msgid ""
 "Public profiles can be found by other users via searches on username, full "
 "name and affiliation. Hidden profiles cannot be found by other users."
 msgstr ""
 "الملفات الشخصية العامة يمكن البحث عنها من قبل المستخدمين الآخرين عن طريق اسم"
-" المستخدم و الاسم الكامل و الانتماءات. الملفات الخصية الخفية لا يمكن إيجادها"
-" من قبل بقية المستخدمين."
+" المستخدم و الاسم الكامل و الانتماءات. الملفات الشّخصية الخفية لا يمكن "
+"إيجادها من قبل بقية المستخدمين."
 
 #: invenio_userprofiles/forms.py:203
 msgid "Email visibility"
-msgstr "رؤية عنوان البريد الالكتروني"
+msgstr "مرئيّة عنوان البريد الالكتروني"
 
 #: invenio_userprofiles/forms.py:208
 msgid ""
 "Public email visibility enables your profile to be found by your email "
 "address."
 msgstr ""
-"تتيح رؤية عنوان البريد الإلكتروني المضمن بالملف الشخصي للعامة إمكانية البحث "
-"و ايجاد ملف الحساب الشخصي عبر بريده الإلكتروني. "
+"تتيح مرئية عنوان البريد الإلكتروني للعامة إمكانية إيجاد ملف حسابك الشخصي عبر"
+" بريدك الإلكتروني. "
 
 #: invenio_userprofiles/validators.py:18
 msgid ""
 "Username must start with a letter, be at least three characters long and "
 "only contain alphanumeric characters, dashes and underscores."
 msgstr ""
 "إسم المستخدم يتكون من ثلاثة حروف على الأقل. يجب ان يبدأ بحرف هجائي. و تستعمل"
@@ -176,8 +176,8 @@
 
 #: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:71
 msgid "Preferences"
 msgstr "الإعدادات"
 
 #: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:85
 msgid "Update preferences"
-msgstr "تحيين الأعدادات"
+msgstr "تحيين الإعدادات"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/bg/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/bg/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: bg\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/bg/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/bg/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/bg/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/teams/23537/bg/)\n"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/teams/23537/bg/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ca/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ca/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Ferran Jorba <Ferran.Jorba@uab.cat>, 2022\n"
 "Language: ca\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ca/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ca/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ca/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Ferran Jorba <Ferran.Jorba@uab.cat>, 2022\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/teams/23537/ca/)\n"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/teams/23537/ca/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/cs/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/cs/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Ivan Masár <helix84@centrum.sk>, 2022\n"
 "Language: cs\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/"
 "cs/)\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/cs/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/cs/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Ivan Masár <helix84@centrum.sk>, 2022\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/cs/)\n"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/cs/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/da/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/da/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2016\n"
 "Language: da\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Danish (https://app.transifex.com/inveniosoftware/teams/23537/"
 "da/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/da/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/da/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2016\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/da/)\n"
+"Language-Team: Danish (https://app.transifex.com/inveniosoftware/teams/23537/da/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: da\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/de/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/de/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: chriz_uniba <christina.zeller@uni-bamberg.de>, 2022\n"
 "Language: de\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/"
 "de/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/de/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/de/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: chriz_uniba <christina.zeller@uni-bamberg.de>, 2022\n"
-"Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/de/)\n"
+"Language-Team: German (https://app.transifex.com/inveniosoftware/teams/23537/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/el/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/el/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: el\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/"
 "el/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/el/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/el/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/el/)\n"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/el/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/en/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/es/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2022\n"
 "Language: es\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/es/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/es/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2022\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/teams/23537/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/teams/23537/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/et/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/et/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Martin Jantson <martinjantson97@gmail.com>, 2022\n"
 "Language: et\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/et/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/et/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/et/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Martin Jantson <martinjantson97@gmail.com>, 2022\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/teams/23537/et/)\n"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/teams/23537/et/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-userprofiles 2.0.3*

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 eb01 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 1002 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d75 7365 7270 726f   invenio-userpro
 00000050: 6669 6c65 7320 322e 302e 330a 5265 706f  files 2.0.3.Repo
 00000060: 7274 2d4d 7367 6964 2d42 7567 732d 546f  rt-Msgid-Bugs-To
 00000070: 3a20 696e 666f 4069 6e76 656e 696f 736f  : info@invenioso
 00000080: 6674 7761 7265 2e6f 7267 0a50 4f54 2d43  ftware.org.POT-C
 00000090: 7265 6174 696f 6e2d 4461 7465 3a20 3230  reation-Date: 20
 000000a0: 3232 2d31 302d 3132 2030 393a 3535 2b30  22-10-12 09:55+0
 000000b0: 3230 300a 504f 2d52 6576 6973 696f 6e2d  200.PO-Revision-
 000000c0: 4461 7465 3a20 3230 3136 2d30 382d 3138  Date: 2016-08-18
 000000d0: 2031 343a 3134 2b30 3030 300a 4c61 7374   14:14+0000.Last
 000000e0: 2d54 7261 6e73 6c61 746f 723a 2046 554c  -Translator: FUL
 000000f0: 4c20 4e41 4d45 203c 454d 4149 4c40 4144  L NAME <EMAIL@AD
 00000100: 4452 4553 533e 0a4c 616e 6775 6167 653a  DRESS>.Language:
-00000110: 2065 745f 4545 0a4c 616e 6775 6167 652d   et_EE.Language-
-00000120: 5465 616d 3a20 4573 746f 6e69 616e 2028  Team: Estonian (
-00000130: 4573 746f 6e69 6129 2028 6874 7470 733a  Estonia) (https:
-00000140: 2f2f 7777 772e 7472 616e 7369 6665 782e  //www.transifex.
-00000150: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
-00000160: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
-00000170: 6574 5f45 452f 290a 506c 7572 616c 2d46  et_EE/).Plural-F
-00000180: 6f72 6d73 3a20 6e70 6c75 7261 6c73 3d32  orms: nplurals=2
-00000190: 3b20 706c 7572 616c 3d28 6e20 213d 2031  ; plural=(n != 1
-000001a0: 293b 0a4d 494d 452d 5665 7273 696f 6e3a  );.MIME-Version:
-000001b0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
-000001c0: 653a 2074 6578 742f 706c 6169 6e3b 2063  e: text/plain; c
-000001d0: 6861 7273 6574 3d75 7466 2d38 0a43 6f6e  harset=utf-8.Con
-000001e0: 7465 6e74 2d54 7261 6e73 6665 722d 456e  tent-Transfer-En
-000001f0: 636f 6469 6e67 3a20 3862 6974 0a47 656e  coding: 8bit.Gen
-00000200: 6572 6174 6564 2d42 793a 2042 6162 656c  erated-By: Babel
-00000210: 2032 2e31 322e 310a 00                    2.12.1..
+00000110: 2065 735f 4d58 0a4c 616e 6775 6167 652d   es_MX.Language-
+00000120: 5465 616d 3a20 5370 616e 6973 6820 284d  Team: Spanish (M
+00000130: 6578 6963 6f29 2028 6874 7470 733a 2f2f  exico) (https://
+00000140: 6170 702e 7472 616e 7369 6665 782e 636f  app.transifex.co
+00000150: 6d2f 696e 7665 6e69 6f73 6f66 7477 6172  m/inveniosoftwar
+00000160: 652f 7465 616d 732f 3233 3533 372f 6573  e/teams/23537/es
+00000170: 5f4d 582f 290a 506c 7572 616c 2d46 6f72  _MX/).Plural-For
+00000180: 6d73 3a20 6e70 6c75 7261 6c73 3d33 3b20  ms: nplurals=3; 
+00000190: 706c 7572 616c 3d6e 203d 3d20 3120 3f20  plural=n == 1 ? 
+000001a0: 3020 3a20 6e20 213d 2030 2026 2620 6e20  0 : n != 0 && n 
+000001b0: 2520 3130 3030 3030 3020 3d3d 2030 203f  % 1000000 == 0 ?
+000001c0: 2031 203a 2032 3b0a 4d49 4d45 2d56 6572   1 : 2;.MIME-Ver
+000001d0: 7369 6f6e 3a20 312e 300a 436f 6e74 656e  sion: 1.0.Conten
+000001e0: 742d 5479 7065 3a20 7465 7874 2f70 6c61  t-Type: text/pla
+000001f0: 696e 3b20 6368 6172 7365 743d 7574 662d  in; charset=utf-
+00000200: 380a 436f 6e74 656e 742d 5472 616e 7366  8.Content-Transf
+00000210: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
+00000220: 740a 4765 6e65 7261 7465 642d 4279 3a20  t.Generated-By: 
+00000230: 4261 6265 6c20 322e 3132 2e31 0a00       Babel 2.12.1..
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
-"Language-Team: Estonian (Estonia) (https://www.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
+"Language-Team: Estonian (Estonia) (https://app.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: et_EE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/fa/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fa/LC_MESSAGES/messages.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: fa\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Persian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/fa/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/fa/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fa/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/teams/23537/fa/)\n"
+"Language-Team: Persian (https://app.transifex.com/inveniosoftware/teams/23537/fa/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fa\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/fr/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
 "Language: fr\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/"
 "fr/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/fr/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/fr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/fr/)\n"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/gl/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/gl/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-userprofiles 2.0.3*

 * *Files 22% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 4461 7465 3a20 3230 3136 2d30 382d 3138  Date: 2016-08-18
 000000d0: 2031 343a 3134 2b30 3030 300a 4c61 7374   14:14+0000.Last
 000000e0: 2d54 7261 6e73 6c61 746f 723a 2046 554c  -Translator: FUL
 000000f0: 4c20 4e41 4d45 203c 454d 4149 4c40 4144  L NAME <EMAIL@AD
 00000100: 4452 4553 533e 0a4c 616e 6775 6167 653a  DRESS>.Language:
 00000110: 2067 6c0a 4c61 6e67 7561 6765 2d54 6561   gl.Language-Tea
 00000120: 6d3a 2047 616c 6963 6961 6e20 2868 7474  m: Galician (htt
-00000130: 7073 3a2f 2f77 7777 2e74 7261 6e73 6966  ps://www.transif
+00000130: 7073 3a2f 2f61 7070 2e74 7261 6e73 6966  ps://app.transif
 00000140: 6578 2e63 6f6d 2f69 6e76 656e 696f 736f  ex.com/invenioso
 00000150: 6674 7761 7265 2f74 6561 6d73 2f32 3335  ftware/teams/235
 00000160: 3337 2f67 6c2f 290a 506c 7572 616c 2d46  37/gl/).Plural-F
 00000170: 6f72 6d73 3a20 6e70 6c75 7261 6c73 3d32  orms: nplurals=2
 00000180: 3b20 706c 7572 616c 3d28 6e20 213d 2031  ; plural=(n != 1
 00000190: 293b 0a4d 494d 452d 5665 7273 696f 6e3a  );.MIME-Version:
 000001a0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/gl/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
-"Language-Team: Galician (https://www.transifex.com/inveniosoftware/teams/23537/gl/)\n"
+"Language-Team: German (Austria) (https://app.transifex.com/inveniosoftware/teams/23537/de_AT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: gl\n"
+"Language: de_AT\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #. NOTE: Form field label
 #: invenio_userprofiles/forms.py:51
 msgid "Username"
 msgstr ""
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/hr/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hr/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: hr\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/hr/)\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/hr/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hr/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/teams/23537/hr/)\n"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/teams/23537/hr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: hr\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/hu/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hu/LC_MESSAGES/messages.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
-"Last-Translator: Andrea Dömötör, 2022\n"
+"Last-Translator: Dorottya Szemigán, 2023\n"
 "Language: hu\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/hu/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
@@ -38,15 +38,15 @@
 msgid "Hidden"
 msgstr "Elrejtve"
 
 msgid "Please re-enter your email address."
 msgstr "Kérjük, adja meg újra az email címét!"
 
 msgid "Preferences"
-msgstr "Beállítások"
+msgstr "Preferenciák"
 
 msgid "Preferences were updated."
 msgstr "A beállításokat frissítettük."
 
 msgid "Profile"
 msgstr "Profil"
 
@@ -67,15 +67,15 @@
 msgstr "Nyilvános"
 
 msgid ""
 "Public email visibility enables your profile to be found by your email "
 "address."
 msgstr ""
 "A nyilvánosan látható email lehetővé teszi, hogy email cím alapján "
-"megtalálják az ön profilját."
+"megtalálják az Ön profilját."
 
 msgid ""
 "Public profiles can be found by other users via searches on username, full "
 "name and affiliation. Hidden profiles cannot be found by other users."
 msgstr ""
 "A nyilvános profilok megtalálhatók a keresőben felhasználónév, teljes név és "
 "affiliáció alapján. A rejtett profilok nem kereshetők más felhasználók "
@@ -87,15 +87,15 @@
 msgid "Required. %(username_rules)s"
 msgstr "Kötelező. %(username_rules)s"
 
 msgid "Resend verification email"
 msgstr "Visszaigazoló email újraküldése"
 
 msgid "Update preferences"
-msgstr "Frissítési beállítások"
+msgstr "Preferenciák frissítése"
 
 msgid "Update profile"
 msgstr "Profil frissítése"
 
 msgid "Username"
 msgstr "Felhasználónév"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/hu/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hu/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-userprofiles project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Andrea Dömötör, 2022
+# Dorottya Szemigán, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
-"Last-Translator: Andrea Dömötör, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/teams/23537/hu/)\n"
+"Last-Translator: Dorottya Szemigán, 2023\n"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/teams/23537/hu/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
@@ -105,15 +106,15 @@
 
 #: invenio_userprofiles/forms.py:208
 msgid ""
 "Public email visibility enables your profile to be found by your email "
 "address."
 msgstr ""
 "A nyilvánosan látható email lehetővé teszi, hogy email cím alapján "
-"megtalálják az ön profilját."
+"megtalálják az Ön profilját."
 
 #: invenio_userprofiles/validators.py:18
 msgid ""
 "Username must start with a letter, be at least three characters long and "
 "only contain alphanumeric characters, dashes and underscores."
 msgstr ""
 "A felhasználónévnek egy betűvel kell kezdődnie, legalább három karakter "
@@ -171,12 +172,12 @@
 #: invenio_userprofiles/templates/invenio_userprofiles/settings/profile.html:39
 #: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:58
 msgid "Update profile"
 msgstr "Profil frissítése"
 
 #: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:71
 msgid "Preferences"
-msgstr "Beállítások"
+msgstr "Preferenciák"
 
 #: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:85
 msgid "Update preferences"
-msgstr "Frissítési beállítások"
+msgstr "Preferenciák frissítése"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/it/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/it/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -3,15 +3,15 @@
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Zacharias Zacharodimos <zacharias.zacharodimos@cern.ch>, "
 "2022\n"
 "Language: it\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/it/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/it/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/it/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Zacharias Zacharodimos <zacharias.zacharodimos@cern.ch>, 2022\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/teams/23537/it/)\n"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/teams/23537/it/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: it\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ja/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ja/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: ja\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Japanese (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ja/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ja/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ja/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/teams/23537/ja/)\n"
+"Language-Team: Japanese (https://app.transifex.com/inveniosoftware/teams/23537/ja/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ja\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ka/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ka/LC_MESSAGES/messages.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: ka\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ka/)\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ka/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ka/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/teams/23537/ka/)\n"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/teams/23537/ka/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/lt/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/lt/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: lt\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/lt/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
 "11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
 "1 : n % 1 != 0 ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/lt/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/lt/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/teams/23537/lt/)\n"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/teams/23537/lt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/messages.pot` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/no/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/no/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: no\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/no/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/no/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/no/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/teams/23537/no/)\n"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/teams/23537/no/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: no\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/pl/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/pl/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: pl\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/"
 "pl/)\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/pl/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/pl/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/pl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/pt/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,24 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language: pt\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/"
-"teams/23537/pt/)\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
-"1000000 == 0 ? 1 : 2;\n"
+"Language: zh_TW\n"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/"
+"teams/23537/zh_TW/)\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "Cancel"
-msgstr "Cancelar"
+msgstr "取消"
 
 msgid "Email address"
-msgstr "Endereço de email"
+msgstr "電郵"
+
+msgid "Username"
+msgstr "帳號"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/pt/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/pt/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/teams/23537/pt/)\n"
+"Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/teams/23537/pt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pt\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ro/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ne/LC_MESSAGES/messages.mo`

 * *Files 22% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +0,0 @@
-msgid ""
-msgstr ""
-"Project-Id-Version: invenio-userprofiles 2.0.3\n"
-"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2022-10-12 09:55+0200\n"
-"PO-Revision-Date: 2016-08-18 14:14+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language: ro\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/"
-"teams/23537/ro/)\n"
-"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
-"2:1));\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
-
-msgid "Cancel"
-msgstr "Anulează"
-
-msgid "Username"
-msgstr "Nume utilizator"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ro/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/rw/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 # Translations template for invenio-userprofiles.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-userprofiles project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
-# Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2016
-# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/teams/23537/ro/)\n"
+"Language-Team: Kinyarwanda (https://app.transifex.com/inveniosoftware/teams/23537/rw/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ro\n"
-"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
+"Language: rw\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #. NOTE: Form field label
 #: invenio_userprofiles/forms.py:51
 msgid "Username"
-msgstr "Nume utilizator"
+msgstr ""
 
 #. NOTE: Form field help text
 #: invenio_userprofiles/forms.py:53
 #, python-format
 msgid "Required. %(username_rules)s"
 msgstr ""
 
@@ -152,15 +148,15 @@
 msgid "You have not yet verified your email address."
 msgstr ""
 
 #: invenio_userprofiles/templates/invenio_userprofiles/settings/profile.html:38
 #: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:57
 #: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:84
 msgid "Cancel"
-msgstr "Anulează"
+msgstr ""
 
 #: invenio_userprofiles/templates/invenio_userprofiles/settings/profile.html:39
 #: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:58
 msgid "Update profile"
 msgstr ""
 
 #: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:71
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ru/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ru/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: ru\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ru/)\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/ru/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/ru/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/teams/23537/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/teams/23537/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/rw/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/rw/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-userprofiles 2.0.3*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 4461 7465 3a20 3230 3136 2d30 382d 3138  Date: 2016-08-18
 000000d0: 2031 343a 3134 2b30 3030 300a 4c61 7374   14:14+0000.Last
 000000e0: 2d54 7261 6e73 6c61 746f 723a 2046 554c  -Translator: FUL
 000000f0: 4c20 4e41 4d45 203c 454d 4149 4c40 4144  L NAME <EMAIL@AD
 00000100: 4452 4553 533e 0a4c 616e 6775 6167 653a  DRESS>.Language:
 00000110: 2072 770a 4c61 6e67 7561 6765 2d54 6561   rw.Language-Tea
 00000120: 6d3a 204b 696e 7961 7277 616e 6461 2028  m: Kinyarwanda (
-00000130: 6874 7470 733a 2f2f 7777 772e 7472 616e  https://www.tran
+00000130: 6874 7470 733a 2f2f 6170 702e 7472 616e  https://app.tran
 00000140: 7369 6665 782e 636f 6d2f 696e 7665 6e69  sifex.com/inveni
 00000150: 6f73 6f66 7477 6172 652f 7465 616d 732f  osoftware/teams/
 00000160: 3233 3533 372f 7277 2f29 0a50 6c75 7261  23537/rw/).Plura
 00000170: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
 00000180: 733d 323b 2070 6c75 7261 6c3d 286e 2021  s=2; plural=(n !
 00000190: 3d20 3129 3b0a 4d49 4d45 2d56 6572 7369  = 1);.MIME-Versi
 000001a0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/rw/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
-"Language-Team: Kinyarwanda (https://www.transifex.com/inveniosoftware/teams/23537/rw/)\n"
+"Language-Team: Hungarian (Hungary) (https://app.transifex.com/inveniosoftware/teams/23537/hu_HU/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: rw\n"
+"Language: hu_HU\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #. NOTE: Form field label
 #: invenio_userprofiles/forms.py:51
 msgid "Username"
 msgstr ""
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/sk/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sk/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Ivan Masár <helix84@centrum.sk>, 2022\n"
 "Language: sk\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/"
 "sk/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
 ">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/sk/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sk/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Ivan Masár <helix84@centrum.sk>, 2022\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/sk/)\n"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/sk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: sk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/sv/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sv/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Sam Arbid, 2022\n"
 "Language: sv\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/sv/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/sv/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/sv/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Sam Arbid, 2022\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/teams/23537/sv/)\n"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/teams/23537/sv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: sv\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/tr/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -3,15 +3,15 @@
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume."
 "com>, 2022\n"
 "Language: tr\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/tr/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/tr/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/tr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume.com>, 2022\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/teams/23537/tr/)\n"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/teams/23537/tr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/uk/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-userprofiles 2.0.3*

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 ba02 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 ca02 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d75 7365 7270 726f   invenio-userpro
 00000050: 6669 6c65 7320 322e 302e 330a 5265 706f  files 2.0.3.Repo
 00000060: 7274 2d4d 7367 6964 2d42 7567 732d 546f  rt-Msgid-Bugs-To
 00000070: 3a20 696e 666f 4069 6e76 656e 696f 736f  : info@invenioso
 00000080: 6674 7761 7265 2e6f 7267 0a50 4f54 2d43  ftware.org.POT-C
 00000090: 7265 6174 696f 6e2d 4461 7465 3a20 3230  reation-Date: 20
 000000a0: 3232 2d31 302d 3132 2030 393a 3535 2b30  22-10-12 09:55+0
 000000b0: 3230 300a 504f 2d52 6576 6973 696f 6e2d  200.PO-Revision-
 000000c0: 4461 7465 3a20 3230 3136 2d30 382d 3138  Date: 2016-08-18
 000000d0: 2031 343a 3134 2b30 3030 300a 4c61 7374   14:14+0000.Last
 000000e0: 2d54 7261 6e73 6c61 746f 723a 2046 554c  -Translator: FUL
 000000f0: 4c20 4e41 4d45 203c 454d 4149 4c40 4144  L NAME <EMAIL@AD
 00000100: 4452 4553 533e 0a4c 616e 6775 6167 653a  DRESS>.Language:
-00000110: 2075 6b0a 4c61 6e67 7561 6765 2d54 6561   uk.Language-Tea
-00000120: 6d3a 2055 6b72 6169 6e69 616e 2028 6874  m: Ukrainian (ht
-00000130: 7470 733a 2f2f 7777 772e 7472 616e 7369  tps://www.transi
-00000140: 6665 782e 636f 6d2f 696e 7665 6e69 6f73  fex.com/invenios
-00000150: 6f66 7477 6172 652f 7465 616d 732f 3233  oftware/teams/23
-00000160: 3533 372f 756b 2f29 0a50 6c75 7261 6c2d  537/uk/).Plural-
-00000170: 466f 726d 733a 206e 706c 7572 616c 733d  Forms: nplurals=
-00000180: 343b 2070 6c75 7261 6c3d 286e 2025 2031  4; plural=(n % 1
-00000190: 203d 3d20 3020 2626 206e 2025 2031 3020   == 0 && n % 10 
-000001a0: 3d3d 2031 2026 2620 6e20 2520 3130 3020  == 1 && n % 100 
-000001b0: 213d 2031 3120 3f20 3020 3a20 6e20 2520  != 11 ? 0 : n % 
-000001c0: 3120 3d3d 2030 2026 2620 6e20 2520 3130  1 == 0 && n % 10
-000001d0: 203e 3d20 3220 2626 206e 2025 2031 3020   >= 2 && n % 10 
-000001e0: 3c3d 2034 2026 2620 286e 2025 2031 3030  <= 4 && (n % 100
-000001f0: 203c 2031 3220 7c7c 206e 2025 2031 3030   < 12 || n % 100
-00000200: 203e 2031 3429 203f 2031 203a 206e 2025   > 14) ? 1 : n %
-00000210: 2031 203d 3d20 3020 2626 2028 6e20 2520   1 == 0 && (n % 
-00000220: 3130 203d 3d30 207c 7c20 286e 2025 2031  10 ==0 || (n % 1
-00000230: 3020 3e3d 3520 2626 206e 2025 2031 3020  0 >=5 && n % 10 
-00000240: 3c3d 3929 207c 7c20 286e 2025 2031 3030  <=9) || (n % 100
-00000250: 203e 3d31 3120 2626 206e 2025 2031 3030   >=11 && n % 100
-00000260: 203c 3d31 3420 2929 203f 2032 3a20 3329   <=14 )) ? 2: 3)
-00000270: 3b0a 4d49 4d45 2d56 6572 7369 6f6e 3a20  ;.MIME-Version: 
-00000280: 312e 300a 436f 6e74 656e 742d 5479 7065  1.0.Content-Type
-00000290: 3a20 7465 7874 2f70 6c61 696e 3b20 6368  : text/plain; ch
-000002a0: 6172 7365 743d 7574 662d 380a 436f 6e74  arset=utf-8.Cont
-000002b0: 656e 742d 5472 616e 7366 6572 2d45 6e63  ent-Transfer-Enc
-000002c0: 6f64 696e 673a 2038 6269 740a 4765 6e65  oding: 8bit.Gene
-000002d0: 7261 7465 642d 4279 3a20 4261 6265 6c20  rated-By: Babel 
-000002e0: 322e 3132 2e31 0a00                      2.12.1..
+00000110: 2075 6b5f 5541 0a4c 616e 6775 6167 652d   uk_UA.Language-
+00000120: 5465 616d 3a20 556b 7261 696e 6961 6e20  Team: Ukrainian 
+00000130: 2855 6b72 6169 6e65 2920 2868 7474 7073  (Ukraine) (https
+00000140: 3a2f 2f61 7070 2e74 7261 6e73 6966 6578  ://app.transifex
+00000150: 2e63 6f6d 2f69 6e76 656e 696f 736f 6674  .com/inveniosoft
+00000160: 7761 7265 2f74 6561 6d73 2f32 3335 3337  ware/teams/23537
+00000170: 2f75 6b5f 5541 2f29 0a50 6c75 7261 6c2d  /uk_UA/).Plural-
+00000180: 466f 726d 733a 206e 706c 7572 616c 733d  Forms: nplurals=
+00000190: 343b 2070 6c75 7261 6c3d 286e 2025 2031  4; plural=(n % 1
+000001a0: 203d 3d20 3020 2626 206e 2025 2031 3020   == 0 && n % 10 
+000001b0: 3d3d 2031 2026 2620 6e20 2520 3130 3020  == 1 && n % 100 
+000001c0: 213d 2031 3120 3f20 3020 3a20 6e20 2520  != 11 ? 0 : n % 
+000001d0: 3120 3d3d 2030 2026 2620 6e20 2520 3130  1 == 0 && n % 10
+000001e0: 203e 3d20 3220 2626 206e 2025 2031 3020   >= 2 && n % 10 
+000001f0: 3c3d 2034 2026 2620 286e 2025 2031 3030  <= 4 && (n % 100
+00000200: 203c 2031 3220 7c7c 206e 2025 2031 3030   < 12 || n % 100
+00000210: 203e 2031 3429 203f 2031 203a 206e 2025   > 14) ? 1 : n %
+00000220: 2031 203d 3d20 3020 2626 2028 6e20 2520   1 == 0 && (n % 
+00000230: 3130 203d 3d30 207c 7c20 286e 2025 2031  10 ==0 || (n % 1
+00000240: 3020 3e3d 3520 2626 206e 2025 2031 3020  0 >=5 && n % 10 
+00000250: 3c3d 3929 207c 7c20 286e 2025 2031 3030  <=9) || (n % 100
+00000260: 203e 3d31 3120 2626 206e 2025 2031 3030   >=11 && n % 100
+00000270: 203c 3d31 3420 2929 203f 2032 3a20 3329   <=14 )) ? 2: 3)
+00000280: 3b0a 4d49 4d45 2d56 6572 7369 6f6e 3a20  ;.MIME-Version: 
+00000290: 312e 300a 436f 6e74 656e 742d 5479 7065  1.0.Content-Type
+000002a0: 3a20 7465 7874 2f70 6c61 696e 3b20 6368  : text/plain; ch
+000002b0: 6172 7365 743d 7574 662d 380a 436f 6e74  arset=utf-8.Cont
+000002c0: 656e 742d 5472 616e 7366 6572 2d45 6e63  ent-Transfer-Enc
+000002d0: 6f64 696e 673a 2038 6269 740a 4765 6e65  oding: 8bit.Gene
+000002e0: 7261 7465 642d 4279 3a20 4261 6265 6c20  rated-By: Babel 
+000002f0: 322e 3132 2e31 0a00                      2.12.1..
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/uk/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
-"Language-Team: Ukrainian (https://www.transifex.com/inveniosoftware/teams/23537/uk/)\n"
+"Language-Team: Ukrainian (Ukraine) (https://app.transifex.com/inveniosoftware/teams/23537/uk_UA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: uk\n"
+"Language: uk_UA\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #. NOTE: Form field label
 #: invenio_userprofiles/forms.py:51
 msgid "Username"
 msgstr ""
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Kalven Richie, 2022\n"
 "Language: zh_CN\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/"
 "teams/23537/zh_CN/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Kalven Richie, 2022\n"
-"Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
+"Language-Team: Chinese (China) (https://app.transifex.com/inveniosoftware/teams/23537/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,24 +0,0 @@
-msgid ""
-msgstr ""
-"Project-Id-Version: invenio-userprofiles 2.0.3\n"
-"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2022-10-12 09:55+0200\n"
-"PO-Revision-Date: 2016-08-18 14:14+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language: zh_TW\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/"
-"teams/23537/zh_TW/)\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
-
-msgid "Cancel"
-msgstr "取消"
-
-msgid "Email address"
-msgstr "電郵"
-
-msgid "Username"
-msgstr "帳號"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-userprofiles 2.0.3\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:55+0200\n"
 "PO-Revision-Date: 2016-08-18 14:14+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: zh_TW\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/validators.py` & `invenio-userprofiles-2.3.0/invenio_userprofiles/validators.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles/views.py` & `invenio-userprofiles-2.3.0/invenio_userprofiles/views.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles.egg-info/PKG-INFO` & `invenio-userprofiles-2.3.0/invenio_userprofiles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-userprofiles
-Version: 2.2.1
+Version: 2.3.0
 Summary: User profiles module for Invenio.
 Home-page: https://github.com/inveniosoftware/invenio-userprofiles
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -46,14 +46,20 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.3.0 (released 2023-07-31)
+        
+        - settings profile: Update buttons with labeled styling and a11y fixes
+        - alembic: fix recipe based on latest sqlalchemy-continuum
+        - pull translations
+        
         Version 2.2.1 (released 2023-05-26)
         
         - fix styling for locale preferences field
         
         Version 2.2.0 (released 2023-04-25)
         
         - add locale to user profile preferences
```

### Comparing `invenio-userprofiles-2.2.1/invenio_userprofiles.egg-info/SOURCES.txt` & `invenio-userprofiles-2.3.0/invenio_userprofiles/translations/uk/LC_MESSAGES/messages.po`

 * *Files 27% similar despite different names*

```diff
@@ -1,134 +1,182 @@
-.dockerignore
-.editorconfig
-.git-blame-ignore-revs
-AUTHORS.rst
-CHANGES.rst
-CONTRIBUTING.rst
-INSTALL.rst
-LICENSE
-MANIFEST.in
-README.rst
-babel.ini
-constraints-pypi.txt
-pyproject.toml
-requirements-devel.txt
-run-i18n-tests.sh
-run-tests.sh
-setup.cfg
-setup.py
-.tx/config
-docs/Makefile
-docs/api.rst
-docs/authors.rst
-docs/changes.rst
-docs/conf.py
-docs/configuration.rst
-docs/contributing.rst
-docs/index.rst
-docs/installation.rst
-docs/license.rst
-docs/make.bat
-docs/requirements.txt
-invenio_userprofiles/__init__.py
-invenio_userprofiles/api.py
-invenio_userprofiles/config.py
-invenio_userprofiles/ext.py
-invenio_userprofiles/forms.py
-invenio_userprofiles/models.py
-invenio_userprofiles/validators.py
-invenio_userprofiles/views.py
-invenio_userprofiles.egg-info/PKG-INFO
-invenio_userprofiles.egg-info/SOURCES.txt
-invenio_userprofiles.egg-info/dependency_links.txt
-invenio_userprofiles.egg-info/entry_points.txt
-invenio_userprofiles.egg-info/not-zip-safe
-invenio_userprofiles.egg-info/requires.txt
-invenio_userprofiles.egg-info/top_level.txt
-invenio_userprofiles/alembic/41157f1933d6_remove_table.py
-invenio_userprofiles/alembic/71634726ec7e_create_userprofiles_branch.py
-invenio_userprofiles/alembic/c25ef2c50ffa_create_userprofiles_tables.py
-invenio_userprofiles/templates/invenio_userprofiles/base.html
-invenio_userprofiles/templates/invenio_userprofiles/register_user.html
-invenio_userprofiles/templates/invenio_userprofiles/settings/_macros.html
-invenio_userprofiles/templates/invenio_userprofiles/settings/base.html
-invenio_userprofiles/templates/invenio_userprofiles/settings/profile.html
-invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/base.html
-invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/register_user.html
-invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/_macros.html
-invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/base.html
-invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html
-invenio_userprofiles/translations/messages.pot
-invenio_userprofiles/translations/af/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/af/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/ar/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/ar/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/bg/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/bg/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/ca/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/ca/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/cs/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/cs/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/da/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/da/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/de/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/de/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/el/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/el/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/en/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/en/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/es/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/es/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/et/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/et/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/et_EE/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/et_EE/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/fa/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/fa/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/fr/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/fr/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/gl/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/gl/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/hr/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/hr/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/hu/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/hu/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/it/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/it/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/ja/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/ja/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/ka/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/ka/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/lt/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/lt/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/no/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/no/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/pl/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/pl/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/pt/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/pt/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/ro/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/ro/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/ru/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/ru/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/rw/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/rw/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/sk/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/sk/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/sv/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/sv/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/tr/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/tr/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/uk/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/uk/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/zh_CN/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/zh_CN/LC_MESSAGES/messages.po
-invenio_userprofiles/translations/zh_TW/LC_MESSAGES/messages.mo
-invenio_userprofiles/translations/zh_TW/LC_MESSAGES/messages.po
-tests/conftest.py
-tests/helpers.py
-tests/test_api.py
-tests/test_forms.py
-tests/test_invenio_userprofile.py
-tests/test_models.py
-tests/test_validators.py
-tests/test_views.py
+# Translations template for invenio-userprofiles.
+# Copyright (C) 2022 CERN
+# This file is distributed under the same license as the
+# invenio-userprofiles project.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# 
+# Translators:
+# Vasyl Ostrovskyi <vasyusya@yahoo.com>, 2023
+# 
+#, fuzzy
+msgid ""
+msgstr ""
+"Project-Id-Version: invenio-userprofiles 2.0.3\n"
+"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
+"POT-Creation-Date: 2022-10-12 09:55+0200\n"
+"PO-Revision-Date: 2016-08-18 14:14+0000\n"
+"Last-Translator: Vasyl Ostrovskyi <vasyusya@yahoo.com>, 2023\n"
+"Language-Team: Ukrainian (https://app.transifex.com/inveniosoftware/teams/23537/uk/)\n"
+"MIME-Version: 1.0\n"
+"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Transfer-Encoding: 8bit\n"
+"Generated-By: Babel 2.10.3\n"
+"Language: uk\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
+
+#. NOTE: Form field label
+#: invenio_userprofiles/forms.py:51
+msgid "Username"
+msgstr "Назва облікового запису"
+
+#. NOTE: Form field help text
+#: invenio_userprofiles/forms.py:53
+#, python-format
+msgid "Required. %(username_rules)s"
+msgstr "Обов'язкове. %(username_rules)s"
+
+#: invenio_userprofiles/forms.py:54
+msgid "Username not provided."
+msgstr "Не вкзано назву облікового запису"
+
+#. NOTE: Form label
+#: invenio_userprofiles/forms.py:60
+msgid "Full name"
+msgstr "Повне ім'я"
+
+#. NOTE: Form label
+#: invenio_userprofiles/forms.py:67
+msgid "Affiliations"
+msgstr "Приналежності"
+
+#. NOTE: Form validation error.
+#: invenio_userprofiles/forms.py:86
+msgid "Username is not available."
+msgstr "Ця назва облікового запису недоступна."
+
+#. NOTE: Form field label
+#: invenio_userprofiles/forms.py:119
+msgid "Email address"
+msgstr "Електронна пошта"
+
+#. NOTE: Form field label
+#: invenio_userprofiles/forms.py:133
+msgid "Re-enter email address"
+msgstr "Електронна пошта - ще раз."
+
+#. NOTE: Form field help text
+#: invenio_userprofiles/forms.py:135
+msgid "Please re-enter your email address."
+msgstr "Будь ласка, вкажіть ще раз адресу вашої електронної пошти."
+
+#. NOTE: Form validation error.
+#: invenio_userprofiles/forms.py:142
+msgid "Email addresses do not match."
+msgstr "Адреси електронної пошти не співпадають."
+
+#. NOTE: Form button label
+#: invenio_userprofiles/forms.py:151
+msgid "Resend verification email"
+msgstr "Повторно надіслати лист для підтвердження."
+
+#: invenio_userprofiles/forms.py:190
+msgid "Profile visibility"
+msgstr "Видимість профілю"
+
+#: invenio_userprofiles/forms.py:192 invenio_userprofiles/forms.py:205
+msgid "Public"
+msgstr "Публічний"
+
+#: invenio_userprofiles/forms.py:193 invenio_userprofiles/forms.py:206
+msgid "Hidden"
+msgstr "Прихований"
+
+#: invenio_userprofiles/forms.py:195
+msgid ""
+"Public profiles can be found by other users via searches on username, full "
+"name and affiliation. Hidden profiles cannot be found by other users."
+msgstr ""
+"Публічні профілі можуть бути знайдені іншими користувачами пошуком за назвою"
+" олікового запису, повним ім'ям, чи приналежністю. Приховані профілі не бузе"
+" знайдено іншими користувачами."
+
+#: invenio_userprofiles/forms.py:203
+msgid "Email visibility"
+msgstr "Видимість електронної адреси"
+
+#: invenio_userprofiles/forms.py:208
+msgid ""
+"Public email visibility enables your profile to be found by your email "
+"address."
+msgstr ""
+"Публічна видимість електронної адреси дозоляє знайти ваш профіль за адресою "
+"електронної пошти."
+
+#: invenio_userprofiles/validators.py:18
+msgid ""
+"Username must start with a letter, be at least three characters long and "
+"only contain alphanumeric characters, dashes and underscores."
+msgstr ""
+"Назва облікового запису повинна починатись з літери, містити не менше трьох "
+"символів, та містити лише літери латинського алфавіту, цифри, знаки дефісу "
+"та підкреслення."
+
+#. NOTE: Menu item text (icon replaced by a user icon).
+#: invenio_userprofiles/views.py:101
+#, python-format
+msgid "%(icon)s Profile"
+msgstr "%(icon)s Профіль"
+
+#: invenio_userprofiles/templates/invenio_userprofiles/settings/profile.html:13
+#: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:13
+#: invenio_userprofiles/views.py:105
+msgid "Profile"
+msgstr "Профіль"
+
+#. NOTE: Flash message.
+#: invenio_userprofiles/views.py:165
+msgid "Verification email sent."
+msgstr "Листа для підтвердження надіслано."
+
+#. NOTE: Flash message after successful update of profile.
+#: invenio_userprofiles/views.py:187
+#, python-format
+msgid ""
+"Profile was updated. We have sent a verification email to %(email)s. Please "
+"check it."
+msgstr ""
+"Профіль оновлено. Ми надіслали листа для підтвердження до %(email)s. Будь "
+"ласка, перегляньте його."
+
+#. NOTE: Flash message after successful update of profile.
+#: invenio_userprofiles/views.py:196
+msgid "Profile was updated."
+msgstr "Профіль оновлено."
+
+#. NOTE: Flash message after successful update of profile.
+#: invenio_userprofiles/views.py:205
+msgid "Preferences were updated."
+msgstr "Налаштування оновлено."
+
+#: invenio_userprofiles/templates/invenio_userprofiles/settings/profile.html:21
+#: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:40
+msgid "You have not yet verified your email address."
+msgstr "Ви ще не підтвердили адреси вашої електронної пошти."
+
+#: invenio_userprofiles/templates/invenio_userprofiles/settings/profile.html:38
+#: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:57
+#: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:84
+msgid "Cancel"
+msgstr "Скасувати"
+
+#: invenio_userprofiles/templates/invenio_userprofiles/settings/profile.html:39
+#: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:58
+msgid "Update profile"
+msgstr "Оновити профіль"
+
+#: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:71
+msgid "Preferences"
+msgstr "Налаштування"
+
+#: invenio_userprofiles/templates/semantic-ui/invenio_userprofiles/settings/profile.html:85
+msgid "Update preferences"
+msgstr "Оновити налаштування"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `invenio-userprofiles-2.2.1/setup.cfg` & `invenio-userprofiles-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/tests/conftest.py` & `invenio-userprofiles-2.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/tests/helpers.py` & `invenio-userprofiles-2.3.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/tests/test_api.py` & `invenio-userprofiles-2.3.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/tests/test_forms.py` & `invenio-userprofiles-2.3.0/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/tests/test_invenio_userprofile.py` & `invenio-userprofiles-2.3.0/tests/test_invenio_userprofile.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/tests/test_models.py` & `invenio-userprofiles-2.3.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/tests/test_validators.py` & `invenio-userprofiles-2.3.0/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `invenio-userprofiles-2.2.1/tests/test_views.py` & `invenio-userprofiles-2.3.0/tests/test_views.py`

 * *Files identical despite different names*

