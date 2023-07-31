# Comparing `tmp/invenio-oauth2server-2.0.0.tar.gz` & `tmp/invenio-oauth2server-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-oauth2server-2.0.0.tar", last modified: Thu Mar  2 15:29:11 2023, max compression
+gzip compressed data, was "dist/invenio-oauth2server-2.1.0.tar", last modified: Mon Jul 31 08:46:58 2023, max compression
```

## Comparing `invenio-oauth2server-2.0.0.tar` & `invenio-oauth2server-2.1.0.tar`

### file list

```diff
@@ -1,264 +1,320 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2010 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2936 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3291 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3557 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      362 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6428 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10339 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/examplesapp.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/docs/images/
--rwxr-xr-x   0 runner    (1001) docker     (122)    15165 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/images/authorization-code.jpg
--rwxr-xr-x   0 runner    (1001) docker     (122)     8247 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/images/client-credentials.jpg
--rwxr-xr-x   0 runner    (1001) docker     (122)    13811 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/images/implicit-grant.jpg
--rw-r--r--   0 runner    (1001) docker     (122)      860 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7009 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)    10987 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/examples/
--rwxr-xr-x   0 runner    (1001) docker     (122)      666 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/examples/app-fixtures.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      893 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/examples/app-setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      229 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/examples/app-teardown.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3981 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/examples/app.py
--rw-r--r--   0 runner    (1001) docker     (122)    14540 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/examples/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/examples/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/examples/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/examples/templates/jwt.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/
--rw-r--r--   0 runner    (1001) docker     (122)     4185 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/_compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/alembic/
--rw-r--r--   0 runner    (1001) docker     (122)     3417 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/alembic/12a88921ada2_create_oauth2server_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     3409 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/alembic/4e57407b8e4a_add_on_delete_cascade.py
--rw-r--r--   0 runner    (1001) docker     (122)      602 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/alembic/aa546f2a8d2f_create_oauth2server_branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2664 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    10561 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     5576 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/forms.py
--rw-r--r--   0 runner    (1001) docker     (122)    12379 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     4916 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/provider.py
--rw-r--r--   0 runner    (1001) docker     (122)      500 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/
--rw-r--r--   0 runner    (1001) docker     (122)     2513 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/authorize.html
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/errors.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/
--rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html
--rw-r--r--   0 runner    (1001) docker     (122)     4174 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html
--rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/helpers.html
--rw-r--r--   0 runner    (1001) docker     (122)     3322 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_new.html
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_permission_view.html
--rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/
--rw-r--r--   0 runner    (1001) docker     (122)     2794 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/
--rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html
--rw-r--r--   0 runner    (1001) docker     (122)     4259 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html
--rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/helpers.html
--rw-r--r--   0 runner    (1001) docker     (122)     3462 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_new.html
--rw-r--r--   0 runner    (1001) docker     (122)     1980 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_permission_view.html
--rw-r--r--   0 runner    (1001) docker     (122)     2074 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/theme/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/theme/semantic/
--rw-r--r--   0 runner    (1001) docker     (122)     1449 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/theme/semantic/form_styling.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18246 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9232 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22974 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      877 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18495 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18587 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     6406 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21060 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18508 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     8305 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22175 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      961 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18558 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     8152 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21903 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     7918 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21572 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18261 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18427 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     6491 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21116 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18245 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      845 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18487 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     7345 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21485 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     6281 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    20976 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18413 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      986 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18583 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      987 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18584 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)    18180 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18418 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      926 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18569 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18451 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18448 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18669 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      524 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18248 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     6452 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21107 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     7862 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21534 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     8189 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21910 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18468 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     7495 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21080 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      748 2023-03-02 15:29:10.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18412 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1981 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/views/
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4413 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/views/server.py
--rw-r--r--   0 runner    (1001) docker     (122)     8238 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/invenio_oauth2server/views/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6428 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8197 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/invenio_oauth2server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      842 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3202 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-02 15:29:11.000000 invenio-oauth2server-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    16943 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4205 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3285 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (122)      882 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/tests/test_alembic.py
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     7981 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/tests/test_invenio_oauth2server.py
--rw-r--r--   0 runner    (1001) docker     (122)     9363 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    37079 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)      949 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     8469 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-03-02 15:29:02.000000 invenio-oauth2server-2.0.0/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2936 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3410 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3557 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      362 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6587 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/examplesapp.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/docs/images/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    15165 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/images/authorization-code.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8247 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/images/client-credentials.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13811 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/images/implicit-grant.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)      860 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7009 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)    10987 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      666 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/examples/app-fixtures.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      893 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/examples/app-setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      229 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/examples/app-teardown.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3981 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/examples/app.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14540 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/examples/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/examples/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/examples/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     2011 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/examples/templates/jwt.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/
+-rw-r--r--   0 runner    (1001) docker     (122)     4185 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)     3417 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/alembic/12a88921ada2_create_oauth2server_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3409 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/alembic/4e57407b8e4a_add_on_delete_cascade.py
+-rw-r--r--   0 runner    (1001) docker     (122)      602 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/alembic/aa546f2a8d2f_create_oauth2server_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2664 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10561 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5581 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/forms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12379 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4916 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)      500 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/
+-rw-r--r--   0 runner    (1001) docker     (122)     2513 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/authorize.html
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/errors.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4174 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/helpers.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3322 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_new.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_permission_view.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/
+-rw-r--r--   0 runner    (1001) docker     (122)     2794 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)     2448 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1109 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4979 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/helpers.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3961 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_new.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1980 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_permission_view.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2310 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/theme/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/theme/semantic/
+-rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/theme/semantic/form_styling.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18246 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9269 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23011 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      877 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18495 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18587 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     6406 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21060 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18508 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     8305 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22175 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18259 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18259 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      961 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18558 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18260 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18260 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     8152 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21903 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18296 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18298 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     7918 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21572 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18261 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18427 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18256 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     6491 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21116 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      593 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18317 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18309 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18245 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18256 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      845 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18487 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     8351 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22013 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      538 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18262 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     6281 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    20976 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18413 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      986 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18583 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      987 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18584 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)    18180 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18243 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18418 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18569 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18451 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18498 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18669 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18248 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     6452 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21107 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     7895 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21601 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18259 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     8189 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21910 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18709 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      760 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18484 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     7495 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21080 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      748 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18412 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1981 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4413 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/views/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8238 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/invenio_oauth2server/views/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6587 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9983 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/invenio_oauth2server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      842 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3202 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:46:58.000000 invenio-oauth2server-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    16955 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4205 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3285 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      882 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/tests/test_alembic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7981 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2138 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/tests/test_invenio_oauth2server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9363 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37079 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8469 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-07-31 08:46:50.000000 invenio-oauth2server-2.1.0/tests/test_validators.py
```

### Comparing `invenio-oauth2server-2.0.0/.editorconfig` & `invenio-oauth2server-2.1.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/.github/workflows/pypi-publish.yml` & `invenio-oauth2server-2.1.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/.github/workflows/tests.yml` & `invenio-oauth2server-2.1.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/.tx/config` & `invenio-oauth2server-2.1.0/.tx/config`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2018 CERN.
+# Copyright (C)      2023 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 
-# TODO: Transifex integration
 #
 # 1) Create message catalog:
 #    $ python setup.py extract_messages
 #    $ python setup.py init_catalog -l <lang>
 #    $ python setup.py compile_catalog
 # 2) Ensure project has been created on Transifex under the inveniosoftware
 #    organisation.
@@ -21,14 +21,14 @@
 #    $ tx push -s -t
 # 5) Pull translations for a single language from Transifex
 #    $ tx pull -l <lang>
 # 6) Pull translations for all languages from Transifex
 #    $ tx pull -a
 
 [main]
-host = https://www.transifex.com
+host = https://app.transifex.com
 
-[invenio.invenio-oauth2server-messages]
+[o:inveniosoftware:p:invenio:r:invenio-oauth2server-messages]
 file_filter = invenio_oauth2server/translations/<lang>/LC_MESSAGES/messages.po
 source_file = invenio_oauth2server/translations/messages.pot
 source_lang = en
 type = PO
```

### Comparing `invenio-oauth2server-2.0.0/AUTHORS.rst` & `invenio-oauth2server-2.1.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/CHANGES.rst` & `invenio-oauth2server-2.1.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.1.0 (released 2023-07-31)
+
+- applications: Improve templates for UI and accessibility
+- pulled translations
+
 Version 2.0.0 (released 2023-03-02)
 
 - drop python2.7 support
 - remove deprecated flask-babelex dependency and imports
 - upgrade invenio-i18n
 - upgrade invenio-admin
```

### Comparing `invenio-oauth2server-2.0.0/CONTRIBUTING.rst` & `invenio-oauth2server-2.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/LICENSE` & `invenio-oauth2server-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/MANIFEST.in` & `invenio-oauth2server-2.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/PKG-INFO` & `invenio-oauth2server-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-oauth2server
-Version: 2.0.0
+Version: 2.1.0
 Summary: "Invenio module that implements OAuth 2 server."
 Home-page: https://github.com/inveniosoftware/invenio-oauth2server
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -50,14 +50,19 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.1.0 (released 2023-07-31)
+        
+        - applications: Improve templates for UI and accessibility
+        - pulled translations
+        
         Version 2.0.0 (released 2023-03-02)
         
         - drop python2.7 support
         - remove deprecated flask-babelex dependency and imports
         - upgrade invenio-i18n
         - upgrade invenio-admin
```

### Comparing `invenio-oauth2server-2.0.0/README.rst` & `invenio-oauth2server-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/docs/Makefile` & `invenio-oauth2server-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/docs/api.rst` & `invenio-oauth2server-2.1.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/docs/conf.py` & `invenio-oauth2server-2.1.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,13 +323,13 @@
 # texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 # texinfo_no_detailmenu = False
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    "https://docs.python.org/": None,
+    "python": ("https://docs.python.org/", None),
     "flask": ("https://flask.palletsprojects.com", None),
 }
 
 # Autodoc configuraton.
 autoclass_content = "both"
```

### Comparing `invenio-oauth2server-2.0.0/docs/examplesapp.rst` & `invenio-oauth2server-2.1.0/docs/examplesapp.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/docs/images/authorization-code.jpg` & `invenio-oauth2server-2.1.0/docs/images/authorization-code.jpg`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/docs/images/client-credentials.jpg` & `invenio-oauth2server-2.1.0/docs/images/client-credentials.jpg`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/docs/images/implicit-grant.jpg` & `invenio-oauth2server-2.1.0/docs/images/implicit-grant.jpg`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/docs/index.rst` & `invenio-oauth2server-2.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/docs/make.bat` & `invenio-oauth2server-2.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/docs/overview.rst` & `invenio-oauth2server-2.1.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/examples/app-fixtures.sh` & `invenio-oauth2server-2.1.0/examples/app-fixtures.sh`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/examples/app-setup.sh` & `invenio-oauth2server-2.1.0/examples/app-setup.sh`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/examples/app.py` & `invenio-oauth2server-2.1.0/examples/app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/examples/consumer.py` & `invenio-oauth2server-2.1.0/examples/consumer.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/examples/templates/jwt.html` & `invenio-oauth2server-2.1.0/examples/templates/jwt.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/__init__.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
 monkey_patch_werkzeug()  # noqa isort:skip
 
 from .decorators import require_api_auth, require_oauth_scopes  # noqa isort:skip
 from .ext import InvenioOAuth2Server, InvenioOAuth2ServerREST  # noqa isort:skip
 from .proxies import current_oauth2server  # noqa isort:skip
 
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 
 __all__ = (
     "__version__",
     "InvenioOAuth2Server",
     "InvenioOAuth2ServerREST",
     "require_api_auth",
     "require_oauth_scopes",
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/_compat.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/_compat.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/admin.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/admin.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/alembic/12a88921ada2_create_oauth2server_tables.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/alembic/12a88921ada2_create_oauth2server_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/alembic/4e57407b8e4a_add_on_delete_cascade.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/alembic/4e57407b8e4a_add_on_delete_cascade.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/alembic/aa546f2a8d2f_create_oauth2server_branch.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/alembic/aa546f2a8d2f_create_oauth2server_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/cli.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/config.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/config.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/decorators.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/errors.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/ext.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/forms.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             except InsecureTransportError:
                 errors.append(v)
             except InvalidRedirectURIError:
                 errors.append(v)
 
         if errors:
             raise validators.ValidationError(
-                _("Invalid redirect URIs: %(urls)s", urls=", ".join(errors))
+                _("Invalid redirect URIs: {urls}").format(urls=", ".join(errors))
             )
 
 
 #
 # Forms
 #
 class ClientFormBase(model_form_factory(Form)):
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/models.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/models.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/provider.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/provider.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/scopes.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/scopes.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/authorize.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/authorize.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/errors.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/errors.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/_macros.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/helpers.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/helpers.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/index.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/index.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_new.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_new.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_permission_view.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_permission_view.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/_macros.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/_macros.html`

 * *Files 23% similar despite different names*

```diff
@@ -4,62 +4,77 @@
   Copyright (C) 2015-2020 CERN.
 
   Invenio is free software; you can redistribute it and/or modify it
   under the terms of the MIT License; see LICENSE file for more details.
 #}
 
 {% macro render_field(field, icon='', placeholder='', errormsg=True, autofocus=False) %}
-{%- if field.widget.input_type == 'hidden' %}
-  {{ field() }}
-{%- else %}
-  <div class="field">
-    <label>{{ field.label }}</label>
-    <div class="ui right icon input">
-      {%- if icon %}
-        <i class="{{icon}}" aria-hidden="true" ></i>
+  {%- if field.widget.input_type == 'hidden' %}
+    {{ field() }}
+  {%- else %}
+    <div class="field">
+      <label>{{ field.label }}</label>
+      <div class="ui right icon input">
+        {%- if icon %}
+          <i class="{{icon}}" aria-hidden="true" ></i>
+        {%- endif %}
+
+        {%- set extras = dict(autofocus='') if autofocus else dict() %}
+        {{ field(placeholder=_(field.label.text | string), **extras) }}
+      </div>
+
+      {%- if field.description %}
+        <small>{{ field.description }}</small>
+      {%- endif %}
+
+      {%- if field.errors and errormsg %} -->
+        <div class="ui pointing red basic label">
+          {%- for error in field.errors %}
+          <p>{{error}}</p>
+          {%- endfor %}
+        </div>
       {%- endif %}
-      {%- set extras = dict(autofocus='') if autofocus else dict() %}
-      {{ field(placeholder=_(field.label.text | string), **extras) }}
     </div>
-    {%- if field.description %}
-    <small>{{ field.description }}</small>
-    {%- endif %}
-    {%- if field.errors and errormsg %} -->
-      <div class="ui pointing red basic label">
-        {%- for error in field.errors %}
-         <p>{{error}}</p>
-        {%- endfor %}
-      </div>
-    {%- endif %}
-  </div>
-{%- endif %}
+  {%- endif %}
 {% endmacro %}
 
 {% macro render_scopes_field(field) %}
 <div class="field">
   <label>{{ field.label }}</label>
   <div class="ui grid">
-    {% for value, label, checked in field.iter_choices() %}
-      {%- set choice_id = field.id ~ "-" ~ value %}
-      <div class="four wide column">
-        <div class="inline field">
-          <div class="ui checkbox">
-            <input id="{{ choice_id }}" {% if checked %} checked {% endif %} value="{{ value }}" name="{{ field.name }}" type="checkbox">
-            <label for="{{ choice_id }}">
-              {{ value }}<br/>
-              <small>{{ label.help_text }}</small>
-            </label>
+    <div class="four column stackable tablet-mobile row">
+      {% for value, label, checked in field.iter_choices() %}
+        {%- set choice_id = field.id ~ "-" ~ value %}
+        <div class="column">
+          <div class="inline field">
+            <div class="ui checkbox">
+              <input
+                id="{{ choice_id }}"
+                aria-describedby="scopes-field-help-text"
+                {% if checked %} checked {% endif %}
+                value="{{ value }}"
+                name="{{ field.name }}"
+                type="checkbox"
+              >
+              <label for="{{ choice_id }}">
+                {{ value }}
+                <small class="block">{{ label.help_text }}</small>
+              </label>
+            </div>
           </div>
         </div>
-      </div>
-    {% endfor %}
+      {% endfor %}
+    </div>
   </div>
   {%- if field.description %}
-  <small>{{ field.description }}</small>
+    <p id="scopes-field-help-text" class="rel-mt-1">
+      <small>{{ field.description }}</small>
+    </p>
   {%- endif %}
+
   {%- if field.errors and errormsg %} -->
     <div class="ui pointing red basic label">
       {%- for error in field.errors %}
         <p>{{error}}</p>
       {%- endfor %}
     </div>
   {%- endif %}
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html`

 * *Files 8% similar despite different names*

```diff
@@ -28,33 +28,43 @@
 000001b0: 2069 6d70 6f72 7420 7265 6e64 6572 5f66   import render_f
 000001c0: 6965 6c64 2077 6974 6820 636f 6e74 6578  ield with contex
 000001d0: 7420 257d 0a0a 7b25 2062 6c6f 636b 2073  t %}..{% block s
 000001e0: 6574 7469 6e67 735f 636f 6e74 656e 7420  ettings_content 
 000001f0: 257d 0a7b 7b20 6865 6c70 6572 732e 7061  %}.{{ helpers.pa
 00000200: 6e65 6c5f 7374 6172 7428 0a20 2020 205f  nel_start(.    _
 00000210: 2827 4e65 7720 4f41 7574 6820 4170 706c  ('New OAuth Appl
-00000220: 6963 6174 696f 6e27 292c 0a29 207d 7d0a  ication'),.) }}.
-00000230: 3c66 6f72 6d20 636c 6173 733d 2275 6920  <form class="ui 
-00000240: 666f 726d 2220 726f 6c65 3d22 666f 726d  form" role="form
-00000250: 2220 6d65 7468 6f64 3d22 504f 5354 223e  " method="POST">
-00000260: 0a20 207b 252d 2066 6f72 2066 6965 6c64  .  {%- for field
-00000270: 2069 6e20 666f 726d 2025 7d0a 2020 2020   in form %}.    
-00000280: 7b7b 2072 656e 6465 725f 6669 656c 6428  {{ render_field(
-00000290: 6669 656c 6429 207d 7d0a 2020 7b25 2d20  field) }}.  {%- 
-000002a0: 656e 6466 6f72 2025 7d0a 2020 3c61 2068  endfor %}.  <a h
-000002b0: 7265 663d 227b 7b20 7572 6c5f 666f 7228  ref="{{ url_for(
-000002c0: 272e 696e 6465 7827 2920 7d7d 2220 636c  '.index') }}" cl
-000002d0: 6173 733d 2275 6920 6275 7474 6f6e 223e  ass="ui button">
-000002e0: 0a20 2020 203c 6920 636c 6173 733d 2269  .    <i class="i
-000002f0: 636f 6e20 7822 3e3c 2f69 3e20 7b7b 205f  con x"></i> {{ _
-00000300: 2827 4361 6e63 656c 2729 207d 7d0a 2020  ('Cancel') }}.  
-00000310: 3c2f 613e 0a20 203c 6275 7474 6f6e 2074  </a>.  <button t
-00000320: 7970 653d 2273 7562 6d69 7422 2063 6c61  ype="submit" cla
-00000330: 7373 3d22 7569 2062 7574 746f 6e20 7072  ss="ui button pr
-00000340: 696d 6172 7922 3e0a 2020 2020 3c69 2063  imary">.    <i c
-00000350: 6c61 7373 3d22 6963 6f6e 2063 6865 636b  lass="icon check
-00000360: 223e 3c2f 693e 207b 7b20 5f28 2752 6567  "></i> {{ _('Reg
-00000370: 6973 7465 7227 2920 7d7d 0a20 203c 2f62  ister') }}.  </b
-00000380: 7574 746f 6e3e 0a3c 2f66 6f72 6d3e 0a7b  utton>.</form>.{
-00000390: 7b20 6865 6c70 6572 732e 7061 6e65 6c5f  { helpers.panel_
-000003a0: 656e 6428 2920 7d7d 0a7b 2520 656e 6462  end() }}.{% endb
-000003b0: 6c6f 636b 2025 7d0a                      lock %}.
+00000220: 6963 6174 696f 6e27 292c 0a20 2020 2062  ication'),.    b
+00000230: 7265 6164 6372 756d 625f 7061 7468 3d75  readcrumb_path=u
+00000240: 726c 5f66 6f72 2827 2e69 6e64 6578 2729  rl_for('.index')
+00000250: 2c0a 2020 2020 6272 6561 6463 7275 6d62  ,.    breadcrumb
+00000260: 5f74 6974 6c65 3d5f 2827 4170 706c 6963  _title=_('Applic
+00000270: 6174 696f 6e73 2729 2c0a 2920 7d7d 0a3c  ations'),.) }}.<
+00000280: 666f 726d 2063 6c61 7373 3d22 7569 2066  form class="ui f
+00000290: 6f72 6d22 2072 6f6c 653d 2266 6f72 6d22  orm" role="form"
+000002a0: 206d 6574 686f 643d 2250 4f53 5422 3e0a   method="POST">.
+000002b0: 2020 7b25 2d20 666f 7220 6669 656c 6420    {%- for field 
+000002c0: 696e 2066 6f72 6d20 257d 0a20 2020 207b  in form %}.    {
+000002d0: 7b20 7265 6e64 6572 5f66 6965 6c64 2866  { render_field(f
+000002e0: 6965 6c64 2920 7d7d 0a20 207b 252d 2065  ield) }}.  {%- e
+000002f0: 6e64 666f 7220 257d 0a20 203c 6120 726f  ndfor %}.  <a ro
+00000300: 6c65 3d22 6275 7474 6f6e 2220 6872 6566  le="button" href
+00000310: 3d22 7b7b 2075 726c 5f66 6f72 2827 2e69  ="{{ url_for('.i
+00000320: 6e64 6578 2729 207d 7d22 2063 6c61 7373  ndex') }}" class
+00000330: 3d22 7569 206c 6162 656c 6564 2069 636f  ="ui labeled ico
+00000340: 6e20 6275 7474 6f6e 223e 0a20 2020 203c  n button">.    <
+00000350: 6920 636c 6173 733d 2269 636f 6e20 7822  i class="icon x"
+00000360: 2061 7269 612d 6869 6464 656e 3d22 7472   aria-hidden="tr
+00000370: 7565 223e 3c2f 693e 207b 7b20 5f28 2743  ue"></i> {{ _('C
+00000380: 616e 6365 6c27 2920 7d7d 0a20 203c 2f61  ancel') }}.  </a
+00000390: 3e0a 2020 3c62 7574 746f 6e20 7479 7065  >.  <button type
+000003a0: 3d22 7375 626d 6974 2220 636c 6173 733d  ="submit" class=
+000003b0: 2275 6920 6c61 6265 6c65 6420 6963 6f6e  "ui labeled icon
+000003c0: 2062 7574 746f 6e20 7072 696d 6172 7922   button primary"
+000003d0: 3e0a 2020 2020 3c69 2063 6c61 7373 3d22  >.    <i class="
+000003e0: 6963 6f6e 2063 6865 636b 2220 6172 6961  icon check" aria
+000003f0: 2d68 6964 6465 6e3d 2274 7275 6522 3e3c  -hidden="true"><
+00000400: 2f69 3e20 7b7b 205f 2827 5265 6769 7374  /i> {{ _('Regist
+00000410: 6572 2729 207d 7d0a 2020 3c2f 6275 7474  er') }}.  </butt
+00000420: 6f6e 3e0a 3c2f 666f 726d 3e0a 7b7b 2068  on>.</form>.{{ h
+00000430: 656c 7065 7273 2e70 616e 656c 5f65 6e64  elpers.panel_end
+00000440: 2829 207d 7d0a 7b25 2065 6e64 626c 6f63  () }}.{% endbloc
+00000450: 6b20 257d 0a                             k %}.
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html`

 * *Files 9% similar despite different names*

```diff
@@ -11,102 +11,114 @@
 {%- extends "invenio_oauth2server/settings/index.html" %}
 
 {%- import "invenio_oauth2server/settings/helpers.html" as helpers with context %}
 {%- from "invenio_oauth2server/settings/_macros.html" import render_field with context %}
 
 {% block settings_content %}
   {{ helpers.panel_start(
-      _('Application / %(client_name)s', client_name=client.name),
+      _('%(client_name)s', client_name=client.name),
+      breadcrumb_path=url_for('.index'),
+      breadcrumb_title=_('Applications'),
       with_body=False,
   ) }}
 
   <div class="ui segment">
-    <form class="ui form" method="POST" action="{{ url_for('.client_reset', client_id=client.client_id) }}">
-      <input type="hidden" name="reset" value="yes">
-      <button type="submit" class="ui right floated negative button">
-        <i class="icon ban"></i> {{ _('Reset client secret') }}
-      </button>
-    </form>
-    <h4 class="ui header">
-      {{ _('Client ID') }}
-      <div class="sub header">
-        <code>{{ client.client_id }}</code>
-      </div>
-    </h4>
-    <h4 class="ui header">
-      {{ _('Client Secret') }}
-      <div class="sub header">
-        <code>{{ client.client_secret }}</code>
-        <br><small>{{ _('Do not share the client secret with anyone!') }}</small></p>
+    <div class="ui grid">
+      <div class="two column stackable tablet-mobile row">
+        <div class="column">
+          <h3 class="ui small header">{{ _('Client ID') }}</h3>
+          <code class="word-break-all">{{ client.client_id }}</code>
+
+          <h3 class="ui small header">{{ _('Client Secret') }}</h3>
+          <code class="word-break-all">{{ client.client_secret }}</code>
+          <p><small>{{ _('Do not share the client secret with anyone!') }}</small></p>
+        </div>
+
+        <div class="bottom aligned column">
+          <form class="ui form text-align-right" method="POST" action="{{ url_for('.client_reset', client_id=client.client_id) }}">
+            <input type="hidden" name="reset" value="yes">
+            <button type="submit" class="ui negative labeled icon button">
+              <i class="icon ban" aria-hidden="true"></i> {{ _('Reset client secret') }}
+            </button>
+          </form>
+        </div>
       </div>
-    </h4>
+    </div>
+
   </div>
-  {%- block client_footer_text %}{%- endblock client_footer_text %}
+
+  {%- block client_footer_text %}
+  {%- endblock client_footer_text %}
+
   <div class="ui segment">
-    <form class="ui form" method="POST" role="form" action="">
-      {%- for field in form %}
-      {{ render_field(field) }}
-      {%- endfor %}
-
-      <button type="submit" name="delete" class="ui button negative">
-        <i class="icon trash"></i> {{ _('Delete') }}
-      </button>
-      <button type="submit" name="save" class="ui button primary">
-        <i class="icon check"></i> {{ _('Save') }}
-      </button>
-    </form>
+    <div class="ui grid">
+      <div class="one column stackable tablet-mobile row">
+        <div class="column">
+          <h3 class="ui small header">{{ _("Application settings") }}</h3>
+          <form class="ui form" method="POST" role="form" action="">
+            {%- for field in form %}
+              {{ render_field(field) }}
+            {%- endfor %}
+            <button type="submit" name="delete" class="ui button labeled icon negative">
+              <i class="icon trash" aria-hidden="true"></i> {{ _('Delete') }}
+            </button>
+            <button type="submit" name="save" class="ui button labeled icon primary">
+              <i class="icon check" aria-hidden="true"></i> {{ _('Save') }}
+            </button>
+          </form>
+        </div>
+      </div>
+    </div>
   </div>
   {{helpers.panel_end(with_body=False)}}
 
   {{helpers.panel_start(_('OAuth 2.0 Endpoints'))}}
-  <div class="ui equal width grid">
-    <div class="column">
-      <p>
-        <h3 class="ui header">
+  <div class="ui grid">
+    <div class="two column stackable tablet-mobile row">
+      <div class="column">
+        <h3 class="ui small header">
           {{ _('Authorize URL (GET)') }}
           <div class="sub header">
             {{ url_for('invenio_oauth2server.authorize', _external=True, _scheme='https')}}
           </div>
         </h3>
-        <small>
+
+        <p>
           {{ _('Query parameters') }} (<a href="{{ url_for(
               'invenio_oauth2server.authorize', response_type='code',
               client_id=client.client_id,
               scope='deposit:write deposit:actions',
               state='CHANGEME',
               redirect_uri=client.default_redirect_uri,
-              _external=False) }}">
-            {{_('example request')}}
-          </a>):
+              _external=False) }}">{{_('example request')}}</a>):
           <ul>
             <li>response_type ({{ _("required, use") }} <code>code</code> {{ _("or") }} <code>token</code>)</li>
             <li>client_id ({{ _("required") }})</li>
             <li>scope ({{ _("required, space separate list of scopes") }})</li>
             <li>redirect_uri ({{ _("required, URL encoded") }})</li>
             <li>state ({{ _("recommended, for CSRF protection") }})</li>
           </ul>
-        </small>
-      </p>
-    </div>
-    <div class="column">
-      <p>
-      <h3 class="ui header">
-        {{ _('Access token URL (POST)') }}
-        <div class="sub header">
-          {{ url_for('invenio_oauth2server.access_token', _external=True, _scheme='https')}}
-        </div>
-      </h3>
-      <small>{{ _('Request body parameters:') }}
-        <ul>
-          <li>client_id ({{ _("required") }}).</li>
-          <li>client_secret ({{ _("required") }}).</li>
-          <li>grant_type ({{ _("required, use") }} {% for c in config.OAUTH2SERVER_ALLOWED_GRANT_TYPES %}<code>{{c}}</code>{% if not loop.last %}, {% endif %}{% endfor %}).</li>
-          <li>code ({{ _("required for grant_type") }} <code>authorization code</code>).</li>
-          <li>scope ({{ _("required for grant_type") }} <code>client_credentials</code>).</li>
-          <li>refresh_token ({{ _("required for grant_type") }} <code>refresh_token</code>).</li>
-        </ul>
-      </small>
-      </p>
+        </p>
+      </div>
+      <div class="column">
+        <h3 class="ui small header">
+          {{ _('Access token URL (POST)') }}
+          <div class="sub header">
+            {{ url_for('invenio_oauth2server.access_token', _external=True, _scheme='https')}}
+          </div>
+        </h3>
+        <p>
+          {{ _('Request body parameters:') }}
+          <ul>
+            <li>client_id ({{ _("required") }}).</li>
+            <li>client_secret ({{ _("required") }}).</li>
+            <li>grant_type ({{ _("required, use") }} {% for c in config.OAUTH2SERVER_ALLOWED_GRANT_TYPES %}<code>{{c}}</code>{% if not loop.last %}, {% endif %}{% endfor %}).</li>
+            <li>code ({{ _("required for grant_type") }} <code>authorization code</code>).</li>
+            <li>scope ({{ _("required for grant_type") }} <code>client_credentials</code>).</li>
+            <li>refresh_token ({{ _("required for grant_type") }} <code>refresh_token</code>).</li>
+          </ul>
+        </p>
+      </div>
     </div>
   </div>
   {{helpers.panel_end()}}
 {% endblock settings_content %}
```

#### html2text {}

```diff
@@ -1,23 +1,25 @@
 {# -*- coding: utf-8 -*- This file is part of Invenio. Copyright (C) 2015-2020
 CERN. Copyright (C) 2021 Graz University of Technology. Invenio is free
 software; you can redistribute it and/or modify it under the terms of the MIT
 License; see LICENSE file for more details. #} {%- extends
 "invenio_oauth2server/settings/index.html" %} {%- import "invenio_oauth2server/
 settings/helpers.html" as helpers with context %} {%- from
 "invenio_oauth2server/settings/_macros.html" import render_field with context
-%} {% block settings_content %} {{ helpers.panel_start( _('Application / %
-(client_name)s', client_name=client.name), with_body=False, ) }}
-   {{ _('Reset client secret') }}
-{{ _('Client ID') }}
+%} {% block settings_content %} {{ helpers.panel_start( _('%(client_name)s',
+client_name=client.name), breadcrumb_path=url_for('.index'), breadcrumb_title=_
+('Applications'), with_body=False, ) }}
+**** {{ _('Client ID') }} ****
 {{ client.client_id }}
-{{ _('Client Secret') }}
+**** {{ _('Client Secret') }} ****
 {{ client.client_secret }}
 {{ _('Do not share the client secret with anyone!') }}
-{%- block client_footer_text %}{%- endblock client_footer_text %}
+   {{ _('Reset client secret') }}
+{%- block client_footer_text %} {%- endblock client_footer_text %}
+**** {{ _("Application settings") }} ****
 {%- for field in form %} {{ render_field(field) }} {%- endfor %}   {{ _
 ('Delete') }}    {{ _('Save') }}
 {{helpers.panel_end(with_body=False)}} {{helpers.panel_start(_('OAuth 2.0
 Endpoints'))}}
 {{ _('Authorize URL (GET)') }}
 {{ url_for('invenio_oauth2server.authorize', _external=True, _scheme='https')}}
 {{ _('Query parameters') }} ({{_('example_request')}}):
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/helpers.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/helpers.html`

 * *Files 22% similar despite different names*

```diff
@@ -10,138 +10,214 @@
 00000090: 6e64 2f6f 7220 6d6f 6469 6679 2069 740a  nd/or modify it.
 000000a0: 2020 756e 6465 7220 7468 6520 7465 726d    under the term
 000000b0: 7320 6f66 2074 6865 204d 4954 204c 6963  s of the MIT Lic
 000000c0: 656e 7365 3b20 7365 6520 4c49 4345 4e53  ense; see LICENS
 000000d0: 4520 6669 6c65 2066 6f72 206d 6f72 6520  E file for more 
 000000e0: 6465 7461 696c 732e 0a23 7d0a 0a7b 252d  details..#}..{%-
 000000f0: 206d 6163 726f 2070 616e 656c 5f73 7461   macro panel_sta
-00000100: 7274 2874 6974 6c65 2c20 6963 6f6e 3d27  rt(title, icon='
-00000110: 272c 2062 746e 5f74 6578 743d 2727 2c20  ', btn_text='', 
-00000120: 6274 6e3d 2727 2c20 6274 6e5f 6963 6f6e  btn='', btn_icon
-00000130: 3d27 272c 0a20 2020 2020 2020 2020 2020  ='',.           
-00000140: 2020 2020 2020 2020 2020 2062 746e 5f68             btn_h
-00000150: 7265 663d 2727 2c20 6274 6e5f 636c 6173  ref='', btn_clas
-00000160: 733d 2762 6173 6963 2073 6563 6f6e 6461  s='basic seconda
-00000170: 7279 272c 2062 746e 5f6e 616d 653d 2727  ry', btn_name=''
-00000180: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000190: 2020 2020 2020 2020 6274 6e32 3d27 272c          btn2='',
-000001a0: 2062 746e 5f69 636f 6e32 3d27 272c 2062   btn_icon2='', b
-000001b0: 746e 5f68 7265 6632 3d27 272c 2062 746e  tn_href2='', btn
-000001c0: 5f63 6c61 7373 323d 2762 6173 6963 2073  _class2='basic s
-000001d0: 6563 6f6e 6461 7279 272c 0a20 2020 2020  econdary',.     
-000001e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001f0: 2062 746e 5f6e 616d 6532 3d27 272c 2069   btn_name2='', i
-00000200: 643d 2222 2c20 7769 7468 5f62 6f64 793d  d="", with_body=
-00000210: 5472 7565 2c20 7061 6e65 6c5f 6578 7472  True, panel_extr
-00000220: 615f 636c 6173 733d 2273 6563 6f6e 6461  a_class="seconda
-00000230: 7279 2229 2025 7d0a 7b25 2d20 626c 6f63  ry") %}.{%- bloc
-00000240: 6b20 7061 6e65 6c5f 7374 6172 7420 7363  k panel_start sc
-00000250: 6f70 6564 2025 7d0a 3c64 6976 2063 6c61  oped %}.<div cla
-00000260: 7373 3d22 7569 2073 6567 6d65 6e74 7322  ss="ui segments"
-00000270: 207b 2520 6966 2069 6420 257d 2069 643d   {% if id %} id=
-00000280: 227b 7b20 6964 207d 7d22 207b 2520 656e  "{{ id }}" {% en
-00000290: 6469 6620 257d 3e0a 0a20 207b 252d 2062  dif %}>..  {%- b
-000002a0: 6c6f 636b 2070 616e 656c 5f68 6561 6469  lock panel_headi
-000002b0: 6e67 2073 636f 7065 6420 257d 0a0a 2020  ng scoped %}..  
-000002c0: 2020 3c64 6976 2063 6c61 7373 3d22 7569    <div class="ui
-000002d0: 2073 6567 6d65 6e74 207b 7b70 616e 656c   segment {{panel
-000002e0: 5f65 7874 7261 5f63 6c61 7373 7d7d 223e  _extra_class}}">
-000002f0: 0a20 2020 2020 203c 6469 7620 636c 6173  .      <div clas
-00000300: 733d 2275 6920 6571 7561 6c20 7769 6474  s="ui equal widt
-00000310: 6820 6772 6964 223e 0a20 2020 2020 2020  h grid">.       
-00000320: 203c 6469 7620 636c 6173 733d 2263 6f6c   <div class="col
-00000330: 756d 6e22 3e0a 2020 2020 2020 2020 2020  umn">.          
-00000340: 3c73 7472 6f6e 6720 636c 6173 733d 2268  <strong class="h
-00000350: 6561 6465 7220 6974 656d 223e 7b25 6966  eader item">{%if
-00000360: 2069 636f 6e20 257d 3c69 2063 6c61 7373   icon %}<i class
-00000370: 3d22 7b7b 2069 636f 6e20 7d7d 223e 3c2f  ="{{ icon }}"></
-00000380: 693e 7b25 2065 6e64 6966 2025 7d20 7b7b  i>{% endif %} {{
-00000390: 2074 6974 6c65 207d 7d3c 2f73 7472 6f6e   title }}</stron
-000003a0: 673e 0a20 2020 2020 2020 203c 2f64 6976  g>.        </div
-000003b0: 3e0a 2020 2020 2020 2020 3c64 6976 2063  >.        <div c
-000003c0: 6c61 7373 3d22 7269 6768 7420 666c 6f61  lass="right floa
-000003d0: 7465 6420 7269 6768 7420 616c 6967 6e65  ted right aligne
-000003e0: 6420 636f 6c75 6d6e 223e 0a20 2020 2020  d column">.     
-000003f0: 2020 2020 207b 252d 2069 6620 6274 6e20       {%- if btn 
-00000400: 616e 6420 2862 746e 5f68 7265 6620 6f72  and (btn_href or
-00000410: 2062 746e 5f74 6578 7429 202d 257d 0a20   btn_text) -%}. 
-00000420: 2020 2020 2020 2020 2020 207b 252d 2069             {%- i
-00000430: 6620 6274 6e5f 6872 6566 2025 7d0a 2020  f btn_href %}.  
-00000440: 2020 2020 2020 2020 2020 2020 3c61 2063              <a c
-00000450: 6c61 7373 3d22 7569 2063 6f6d 7061 6374  lass="ui compact
-00000460: 2074 696e 7920 6275 7474 6f6e 207b 7b20   tiny button {{ 
-00000470: 6274 6e5f 636c 6173 7320 7d7d 2220 6872  btn_class }}" hr
-00000480: 6566 3d22 7b7b 2062 746e 5f68 7265 6620  ef="{{ btn_href 
-00000490: 7d7d 223e 0a20 2020 2020 2020 2020 2020  }}">.           
-000004a0: 2020 2020 207b 2520 6966 2062 746e 5f69       {% if btn_i
-000004b0: 636f 6e20 257d 3c69 2063 6c61 7373 3d22  con %}<i class="
-000004c0: 7b7b 2062 746e 5f69 636f 6e20 7d7d 223e  {{ btn_icon }}">
-000004d0: 3c2f 693e 207b 2520 656e 6469 6620 257d  </i> {% endif %}
-000004e0: 7b7b 2062 746e 207d 7d0a 2020 2020 2020  {{ btn }}.      
-000004f0: 2020 2020 2020 2020 3c2f 613e 0a20 2020          </a>.   
-00000500: 2020 2020 2020 2020 207b 252d 2065 6c69           {%- eli
-00000510: 6620 6274 6e5f 6e61 6d65 2025 7d0a 2020  f btn_name %}.  
-00000520: 2020 2020 2020 2020 2020 2020 3c62 7574              <but
-00000530: 746f 6e20 6e61 6d65 3d22 7b7b 2062 746e  ton name="{{ btn
-00000540: 5f6e 616d 6520 7d7d 2220 636c 6173 733d  _name }}" class=
-00000550: 2275 6920 636f 6d70 6163 7420 7469 6e79  "ui compact tiny
-00000560: 2062 7574 746f 6e20 7b7b 2062 746e 5f63   button {{ btn_c
-00000570: 6c61 7373 207d 7d22 3e7b 2520 6966 2062  lass }}">{% if b
-00000580: 746e 5f69 636f 6e20 257d 3c69 2063 6c61  tn_icon %}<i cla
-00000590: 7373 3d22 7b7b 2062 746e 5f69 636f 6e20  ss="{{ btn_icon 
-000005a0: 7d7d 223e 3c2f 693e 207b 2520 656e 6469  }}"></i> {% endi
-000005b0: 6620 257d 7b7b 2062 746e 207d 7d3c 2f62  f %}{{ btn }}</b
-000005c0: 7574 746f 6e3e 0a20 2020 2020 2020 2020  utton>.         
-000005d0: 2020 207b 252d 2065 6e64 6966 2025 7d0a     {%- endif %}.
-000005e0: 2020 2020 2020 2020 2020 7b25 2d20 656e            {%- en
-000005f0: 6469 6620 2d25 7d0a 0a20 2020 2020 2020  dif -%}..       
-00000600: 2020 207b 252d 2069 6620 6274 6e32 2061     {%- if btn2 a
-00000610: 6e64 2062 746e 5f68 7265 6632 202d 257d  nd btn_href2 -%}
-00000620: 0a20 2020 2020 2020 2020 2020 207b 252d  .            {%-
-00000630: 2069 6620 6274 6e5f 6872 6566 3220 257d   if btn_href2 %}
-00000640: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00000650: 6120 636c 6173 733d 2275 6920 636f 6d70  a class="ui comp
-00000660: 6163 7420 7469 6e79 2062 7574 746f 6e20  act tiny button 
-00000670: 7b7b 2062 746e 5f63 6c61 7373 3220 7d7d  {{ btn_class2 }}
-00000680: 2220 6872 6566 3d22 7b7b 2062 746e 5f68  " href="{{ btn_h
-00000690: 7265 6632 207d 7d22 3e7b 2520 6966 2062  ref2 }}">{% if b
-000006a0: 746e 5f69 636f 6e32 2025 7d3c 6920 636c  tn_icon2 %}<i cl
-000006b0: 6173 733d 227b 7b20 6274 6e5f 6963 6f6e  ass="{{ btn_icon
-000006c0: 3220 7d7d 223e 3c2f 693e 207b 2520 656e  2 }}"></i> {% en
-000006d0: 6469 6620 257d 7b7b 2062 746e 3220 7d7d  dif %}{{ btn2 }}
-000006e0: 3c2f 613e 0a20 2020 2020 2020 2020 2020  </a>.           
-000006f0: 207b 252d 2065 6c69 6620 6274 6e5f 6e61   {%- elif btn_na
-00000700: 6d65 3220 257d 0a20 2020 2020 2020 2020  me2 %}.         
-00000710: 2020 2020 203c 6275 7474 6f6e 206e 616d       <button nam
-00000720: 653d 227b 7b20 6274 6e5f 6e61 6d65 3220  e="{{ btn_name2 
-00000730: 7d7d 2220 636c 6173 733d 2275 6920 636f  }}" class="ui co
-00000740: 6d70 6163 7420 7469 6e79 2062 7574 746f  mpact tiny butto
-00000750: 6e20 7b7b 2062 746e 5f63 6c61 7373 3220  n {{ btn_class2 
-00000760: 7d7d 223e 7b25 2069 6620 6274 6e5f 6963  }}">{% if btn_ic
-00000770: 6f6e 3220 257d 3c69 2063 6c61 7373 3d22  on2 %}<i class="
-00000780: 7b7b 2062 746e 5f69 636f 6e32 207d 7d22  {{ btn_icon2 }}"
-00000790: 3e3c 2f69 3e20 7b25 2065 6e64 6966 2025  ></i> {% endif %
-000007a0: 7d7b 7b20 6274 6e32 207d 7d3c 2f62 7574  }{{ btn2 }}</but
-000007b0: 746f 6e3e 0a20 2020 2020 2020 2020 2020  ton>.           
-000007c0: 207b 252d 2065 6e64 6966 2025 7d0a 2020   {%- endif %}.  
-000007d0: 2020 2020 2020 2020 7b25 2d20 656e 6469          {%- endi
-000007e0: 6620 2d25 7d0a 2020 2020 2020 2020 3c2f  f -%}.        </
-000007f0: 6469 763e 0a20 2020 2020 203c 2f64 6976  div>.      </div
-00000800: 3e0a 2020 2020 3c2f 6469 763e 0a20 207b  >.    </div>.  {
-00000810: 252d 2065 6e64 626c 6f63 6b20 257d 0a0a  %- endblock %}..
-00000820: 2020 7b25 2d20 6966 2077 6974 685f 626f    {%- if with_bo
-00000830: 6479 2025 7d0a 2020 2020 3c64 6976 2063  dy %}.    <div c
-00000840: 6c61 7373 3d22 7569 2073 6567 6d65 6e74  lass="ui segment
-00000850: 223e 0a20 207b 252d 2065 6e64 6966 2025  ">.  {%- endif %
-00000860: 7d0a 0a7b 252d 2065 6e64 626c 6f63 6b20  }..{%- endblock 
-00000870: 257d 0a7b 252d 2065 6e64 6d61 6372 6f20  %}.{%- endmacro 
-00000880: 257d 0a0a 0a7b 252d 206d 6163 726f 2070  %}...{%- macro p
-00000890: 616e 656c 5f65 6e64 2877 6974 685f 626f  anel_end(with_bo
-000008a0: 6479 3d54 7275 6529 2025 7d0a 7b25 2d20  dy=True) %}.{%- 
-000008b0: 626c 6f63 6b20 7061 6e65 6c5f 656e 6420  block panel_end 
-000008c0: 7363 6f70 6564 2025 7d0a 2020 7b25 2d20  scoped %}.  {%- 
-000008d0: 6966 2077 6974 685f 626f 6479 2025 7d0a  if with_body %}.
-000008e0: 2020 2020 3c2f 6469 763e 0a20 207b 252d      </div>.  {%-
-000008f0: 2065 6e64 6966 2025 7d0a 3c2f 6469 763e   endif %}.</div>
-00000900: 0a7b 252d 2065 6e64 626c 6f63 6b20 257d  .{%- endblock %}
-00000910: 0a7b 252d 2065 6e64 6d61 6372 6f20 257d  .{%- endmacro %}
-00000920: 0a                                       .
+00000100: 7274 280a 2020 2020 7469 746c 652c 0a20  rt(.    title,. 
+00000110: 2020 2062 7265 6164 6372 756d 625f 7061     breadcrumb_pa
+00000120: 7468 3d27 272c 0a20 2020 2062 7265 6164  th='',.    bread
+00000130: 6372 756d 625f 7469 746c 653d 2727 2c0a  crumb_title='',.
+00000140: 2020 2020 6963 6f6e 3d27 272c 0a20 2020      icon='',.   
+00000150: 2062 746e 5f74 6578 743d 2727 2c0a 2020   btn_text='',.  
+00000160: 2020 6274 6e3d 2727 2c0a 2020 2020 6274    btn='',.    bt
+00000170: 6e5f 6963 6f6e 3d27 272c 0a20 2020 2062  n_icon='',.    b
+00000180: 746e 5f68 7265 663d 2727 2c0a 2020 2020  tn_href='',.    
+00000190: 6274 6e5f 636c 6173 733d 2762 6173 6963  btn_class='basic
+000001a0: 2073 6563 6f6e 6461 7279 272c 0a20 2020   secondary',.   
+000001b0: 2062 746e 5f6e 616d 653d 2727 2c0a 2020   btn_name='',.  
+000001c0: 2020 6274 6e32 3d27 272c 0a20 2020 2062    btn2='',.    b
+000001d0: 746e 5f69 636f 6e32 3d27 272c 0a20 2020  tn_icon2='',.   
+000001e0: 2062 746e 5f68 7265 6632 3d27 272c 0a20   btn_href2='',. 
+000001f0: 2020 2062 746e 5f63 6c61 7373 323d 2762     btn_class2='b
+00000200: 6173 6963 2073 6563 6f6e 6461 7279 272c  asic secondary',
+00000210: 0a20 2020 2062 746e 5f6e 616d 6532 3d27  .    btn_name2='
+00000220: 272c 0a20 2020 2069 643d 2222 2c0a 2020  ',.    id="",.  
+00000230: 2020 7769 7468 5f62 6f64 793d 5472 7565    with_body=True
+00000240: 2c0a 2020 2020 7061 6e65 6c5f 6578 7472  ,.    panel_extr
+00000250: 615f 636c 6173 733d 2273 6563 6f6e 6461  a_class="seconda
+00000260: 7279 220a 2020 290a 257d 0a0a 2020 7b25  ry".  ).%}..  {%
+00000270: 2d20 626c 6f63 6b20 7061 6e65 6c5f 7374  - block panel_st
+00000280: 6172 7420 7363 6f70 6564 2025 7d0a 2020  art scoped %}.  
+00000290: 3c73 6563 7469 6f6e 2061 7269 612d 6c61  <section aria-la
+000002a0: 6265 6c3d 227b 7b20 5f28 7469 746c 6529  bel="{{ _(title)
+000002b0: 207d 7d22 2063 6c61 7373 3d22 7569 2073   }}" class="ui s
+000002c0: 6567 6d65 6e74 7322 207b 2520 6966 2069  egments" {% if i
+000002d0: 6420 257d 2069 643d 227b 7b20 6964 207d  d %} id="{{ id }
+000002e0: 7d22 207b 2520 656e 6469 6620 257d 3e0a  }" {% endif %}>.
+000002f0: 0a20 2020 207b 252d 2062 6c6f 636b 2070  .    {%- block p
+00000300: 616e 656c 5f68 6561 6469 6e67 2073 636f  anel_heading sco
+00000310: 7065 6420 257d 0a20 2020 2020 203c 6469  ped %}.      <di
+00000320: 7620 636c 6173 733d 2275 6920 7365 676d  v class="ui segm
+00000330: 656e 7420 7b7b 7061 6e65 6c5f 6578 7472  ent {{panel_extr
+00000340: 615f 636c 6173 737d 7d22 3e0a 0a20 2020  a_class}}">..   
+00000350: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00000360: 2275 6920 7477 6f20 636f 6c75 6d6e 2067  "ui two column g
+00000370: 7269 6422 3e0a 2020 2020 2020 2020 2020  rid">.          
+00000380: 3c64 6976 2063 6c61 7373 3d22 6d69 6464  <div class="midd
+00000390: 6c65 2061 6c69 676e 6564 2063 6f6c 756d  le aligned colum
+000003a0: 6e22 3e0a 2020 2020 2020 2020 2020 2020  n">.            
+000003b0: 7b25 2069 6620 6272 6561 6463 7275 6d62  {% if breadcrumb
+000003c0: 5f70 6174 6820 616e 6420 6272 6561 6463  _path and breadc
+000003d0: 7275 6d62 5f74 6974 6c65 2025 7d0a 2020  rumb_title %}.  
+000003e0: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
+000003f0: 6e20 636c 6173 733d 2275 6920 7469 6e79  n class="ui tiny
+00000400: 2068 6561 6465 7222 3e0a 2020 2020 2020   header">.      
+00000410: 2020 2020 2020 2020 2020 3c61 0a20 2020            <a.   
+00000420: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00000430: 7265 663d 227b 7b20 6272 6561 6463 7275  ref="{{ breadcru
+00000440: 6d62 5f70 6174 6820 7d7d 220a 2020 2020  mb_path }}".    
+00000450: 2020 2020 2020 2020 2020 2020 2020 6172                ar
+00000460: 6961 2d6c 6162 656c 3d22 4261 636b 2074  ia-label="Back t
+00000470: 6f20 7b7b 2062 7265 6164 6372 756d 625f  o {{ breadcrumb_
+00000480: 7469 746c 6520 7d7d 220a 2020 2020 2020  title }}".      
+00000490: 2020 2020 2020 2020 2020 3e0a 2020 2020            >.    
+000004a0: 2020 2020 2020 2020 2020 2020 2020 7b7b                {{
+000004b0: 2062 7265 6164 6372 756d 625f 7469 746c   breadcrumb_titl
+000004c0: 6520 7d7d 0a20 2020 2020 2020 2020 2020  e }}.           
+000004d0: 2020 2020 203c 2f61 3e0a 2020 2020 2020       </a>.      
+000004e0: 2020 2020 2020 2020 2020 3c73 7061 6e20            <span 
+000004f0: 6172 6961 2d68 6964 6465 6e3d 2274 7275  aria-hidden="tru
+00000500: 6522 3e2f 3c2f 7370 616e 3e0a 2020 2020  e">/</span>.    
+00000510: 2020 2020 2020 2020 2020 3c2f 7370 616e            </span
+00000520: 3e0a 2020 2020 2020 2020 2020 2020 7b25  >.            {%
+00000530: 2065 6e64 6966 2025 7d0a 0a20 2020 2020   endif %}..     
+00000540: 2020 2020 2020 207b 2569 6620 6963 6f6e         {%if icon
+00000550: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00000560: 2020 3c69 2063 6c61 7373 3d22 7b7b 2069    <i class="{{ i
+00000570: 636f 6e20 7d7d 2220 6172 6961 2d68 6964  con }}" aria-hid
+00000580: 6465 6e3d 2274 7275 6522 3e3c 2f69 3e0a  den="true"></i>.
+00000590: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+000005a0: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+000005b0: 2020 2020 3c68 3220 636c 6173 733d 2275      <h2 class="u
+000005c0: 6920 7469 6e79 2068 6561 6465 7220 696e  i tiny header in
+000005d0: 6c69 6e65 2d62 6c6f 636b 206d 2d30 223e  line-block m-0">
+000005e0: 7b7b 2074 6974 6c65 207d 7d3c 2f68 323e  {{ title }}</h2>
+000005f0: 0a20 2020 2020 2020 2020 203c 2f64 6976  .          </div
+00000600: 3e0a 0a20 2020 2020 2020 2020 203c 6469  >..          <di
+00000610: 7620 636c 6173 733d 2272 6967 6874 2061  v class="right a
+00000620: 6c69 676e 6564 2063 6f6c 756d 6e22 3e0a  ligned column">.
+00000630: 2020 2020 2020 2020 2020 2020 7b25 2d20              {%- 
+00000640: 6966 2062 746e 2061 6e64 2028 6274 6e5f  if btn and (btn_
+00000650: 6872 6566 206f 7220 6274 6e5f 7465 7874  href or btn_text
+00000660: 2920 2d25 7d0a 2020 2020 2020 2020 2020  ) -%}.          
+00000670: 2020 2020 7b25 2d20 6966 2062 746e 5f68      {%- if btn_h
+00000680: 7265 6620 257d 0a20 2020 2020 2020 2020  ref %}.         
+00000690: 2020 2020 2020 203c 6120 636c 6173 733d         <a class=
+000006a0: 2275 6920 636f 6d70 6163 7420 7469 6e79  "ui compact tiny
+000006b0: 2062 7574 746f 6e20 7b7b 2027 6963 6f6e   button {{ 'icon
+000006c0: 2720 6966 2062 746e 5f69 636f 6e20 7d7d  ' if btn_icon }}
+000006d0: 207b 7b20 6274 6e5f 636c 6173 7320 7d7d   {{ btn_class }}
+000006e0: 2220 6872 6566 3d22 7b7b 2062 746e 5f68  " href="{{ btn_h
+000006f0: 7265 6620 7d7d 223e 0a20 2020 2020 2020  ref }}">.       
+00000700: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
+00000710: 2062 746e 5f69 636f 6e20 257d 0a20 2020   btn_icon %}.   
+00000720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000730: 203c 6920 636c 6173 733d 227b 7b20 6274   <i class="{{ bt
+00000740: 6e5f 6963 6f6e 207d 7d22 2061 7269 612d  n_icon }}" aria-
+00000750: 6869 6464 656e 3d22 7472 7565 223e 3c2f  hidden="true"></
+00000760: 693e 0a20 2020 2020 2020 2020 2020 2020  i>.             
+00000770: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
+00000780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000790: 2020 207b 7b20 6274 6e20 7d7d 0a20 2020     {{ btn }}.   
+000007a0: 2020 2020 2020 2020 2020 2020 203c 2f61               </a
+000007b0: 3e0a 0a20 2020 2020 2020 2020 2020 2020  >..             
+000007c0: 207b 252d 2065 6c69 6620 6274 6e5f 6e61   {%- elif btn_na
+000007d0: 6d65 2025 7d0a 2020 2020 2020 2020 2020  me %}.          
+000007e0: 2020 2020 2020 3c62 7574 746f 6e20 6e61        <button na
+000007f0: 6d65 3d22 7b7b 2062 746e 5f6e 616d 6520  me="{{ btn_name 
+00000800: 7d7d 2220 636c 6173 733d 2275 6920 636f  }}" class="ui co
+00000810: 6d70 6163 7420 7469 6e79 2062 7574 746f  mpact tiny butto
+00000820: 6e20 7b7b 2027 6963 6f6e 2720 6966 2062  n {{ 'icon' if b
+00000830: 746e 5f69 636f 6e20 7d7d 207b 7b20 6274  tn_icon }} {{ bt
+00000840: 6e5f 636c 6173 7320 7d7d 223e 0a20 2020  n_class }}">.   
+00000850: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00000860: 2520 6966 2062 746e 5f69 636f 6e20 257d  % if btn_icon %}
+00000870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000880: 2020 2020 203c 6920 636c 6173 733d 227b       <i class="{
+00000890: 7b20 6274 6e5f 6963 6f6e 207d 7d22 3e3c  { btn_icon }}"><
+000008a0: 2f69 3e0a 2020 2020 2020 2020 2020 2020  /i>.            
+000008b0: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+000008c0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000008d0: 2020 2020 7b7b 2062 746e 207d 7d0a 2020      {{ btn }}.  
+000008e0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000008f0: 6275 7474 6f6e 3e0a 2020 2020 2020 2020  button>.        
+00000900: 2020 2020 2020 7b25 2d20 656e 6469 6620        {%- endif 
+00000910: 257d 0a20 2020 2020 2020 2020 2020 207b  %}.            {
+00000920: 252d 2065 6e64 6966 202d 257d 0a0a 2020  %- endif -%}..  
+00000930: 2020 2020 2020 2020 2020 7b25 2d20 6966            {%- if
+00000940: 2062 746e 3220 616e 6420 6274 6e5f 6872   btn2 and btn_hr
+00000950: 6566 3220 2d25 7d0a 2020 2020 2020 2020  ef2 -%}.        
+00000960: 2020 2020 2020 7b25 2d20 6966 2062 746e        {%- if btn
+00000970: 5f68 7265 6632 2025 7d0a 2020 2020 2020  _href2 %}.      
+00000980: 2020 2020 2020 2020 2020 3c61 0a20 2020            <a.   
+00000990: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000009a0: 6c61 7373 3d22 7569 2063 6f6d 7061 6374  lass="ui compact
+000009b0: 2074 696e 7920 6275 7474 6f6e 207b 7b20   tiny button {{ 
+000009c0: 2769 636f 6e27 2069 6620 6274 6e5f 6963  'icon' if btn_ic
+000009d0: 6f6e 3220 7d7d 207b 7b20 6274 6e5f 636c  on2 }} {{ btn_cl
+000009e0: 6173 7332 207d 7d22 0a20 2020 2020 2020  ass2 }}".       
+000009f0: 2020 2020 2020 2020 2020 2068 7265 663d             href=
+00000a00: 227b 7b20 6274 6e5f 6872 6566 3220 7d7d  "{{ btn_href2 }}
+00000a10: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00000a20: 2020 3e0a 2020 2020 2020 2020 2020 2020    >.            
+00000a30: 2020 2020 2020 7b25 2069 6620 6274 6e5f        {% if btn_
+00000a40: 6963 6f6e 3220 257d 0a20 2020 2020 2020  icon2 %}.       
+00000a50: 2020 2020 2020 2020 2020 2020 203c 6920               <i 
+00000a60: 636c 6173 733d 227b 7b20 6274 6e5f 6963  class="{{ btn_ic
+00000a70: 6f6e 3220 7d7d 223e 3c2f 693e 0a20 2020  on2 }}"></i>.   
+00000a80: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00000a90: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+00000aa0: 2020 2020 2020 2020 2020 2020 207b 7b20               {{ 
+00000ab0: 6274 6e32 207d 7d0a 2020 2020 2020 2020  btn2 }}.        
+00000ac0: 2020 2020 2020 2020 3c2f 613e 0a0a 2020          </a>..  
+00000ad0: 2020 2020 2020 2020 2020 2020 7b25 2d20              {%- 
+00000ae0: 656c 6966 2062 746e 5f6e 616d 6532 2025  elif btn_name2 %
+00000af0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00000b00: 2020 3c62 7574 746f 6e0a 2020 2020 2020    <button.      
+00000b10: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00000b20: 3d22 7b7b 2062 746e 5f6e 616d 6532 207d  ="{{ btn_name2 }
+00000b30: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+00000b40: 2020 2020 2063 6c61 7373 3d22 7569 2063       class="ui c
+00000b50: 6f6d 7061 6374 2074 696e 7920 6275 7474  ompact tiny butt
+00000b60: 6f6e 207b 7b20 6274 6e5f 636c 6173 7332  on {{ btn_class2
+00000b70: 207d 7d20 7b7b 2027 6963 6f6e 2720 6966   }} {{ 'icon' if
+00000b80: 2062 746e 5f69 636f 6e32 207d 7d22 0a20   btn_icon2 }}". 
+00000b90: 2020 2020 2020 2020 2020 2020 2020 203e                 >
+00000ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000bb0: 2020 207b 2520 6966 2062 746e 5f69 636f     {% if btn_ico
+00000bc0: 6e32 2025 7d0a 2020 2020 2020 2020 2020  n2 %}.          
+00000bd0: 2020 2020 2020 2020 2020 3c69 2063 6c61            <i cla
+00000be0: 7373 3d22 7b7b 2062 746e 5f69 636f 6e32  ss="{{ btn_icon2
+00000bf0: 207d 7d22 3e3c 2f69 3e0a 2020 2020 2020   }}"></i>.      
+00000c00: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
+00000c10: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+00000c20: 2020 2020 2020 2020 2020 7b7b 2062 746e            {{ btn
+00000c30: 3220 7d7d 0a20 2020 2020 2020 2020 2020  2 }}.           
+00000c40: 2020 2020 203c 2f62 7574 746f 6e3e 0a20       </button>. 
+00000c50: 2020 2020 2020 2020 2020 2020 207b 252d               {%-
+00000c60: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
+00000c70: 2020 2020 2020 7b25 2d20 656e 6469 6620        {%- endif 
+00000c80: 2d25 7d0a 2020 2020 2020 2020 2020 3c2f  -%}.          </
+00000c90: 6469 763e 0a20 2020 2020 2020 203c 2f64  div>.        </d
+00000ca0: 6976 3e0a 2020 2020 2020 3c2f 6469 763e  iv>.      </div>
+00000cb0: 0a20 2020 207b 252d 2065 6e64 626c 6f63  .    {%- endbloc
+00000cc0: 6b20 257d 0a0a 2020 2020 7b25 2d20 6966  k %}..    {%- if
+00000cd0: 2077 6974 685f 626f 6479 2025 7d0a 2020   with_body %}.  
+00000ce0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00000cf0: 7569 2073 6567 6d65 6e74 223e 0a20 2020  ui segment">.   
+00000d00: 207b 252d 2065 6e64 6966 2025 7d0a 0a20   {%- endif %}.. 
+00000d10: 207b 252d 2065 6e64 626c 6f63 6b20 257d   {%- endblock %}
+00000d20: 0a7b 252d 2065 6e64 6d61 6372 6f20 257d  .{%- endmacro %}
+00000d30: 0a0a 0a7b 252d 206d 6163 726f 2070 616e  ...{%- macro pan
+00000d40: 656c 5f65 6e64 2877 6974 685f 626f 6479  el_end(with_body
+00000d50: 3d54 7275 6529 2025 7d0a 2020 7b25 2d20  =True) %}.  {%- 
+00000d60: 626c 6f63 6b20 7061 6e65 6c5f 656e 6420  block panel_end 
+00000d70: 7363 6f70 6564 2025 7d0a 2020 2020 7b25  scoped %}.    {%
+00000d80: 2d20 6966 2077 6974 685f 626f 6479 2025  - if with_body %
+00000d90: 7d0a 2020 2020 2020 3c2f 6469 763e 0a20  }.      </div>. 
+00000da0: 2020 207b 252d 2065 6e64 6966 2025 7d0a     {%- endif %}.
+00000db0: 2020 2020 3c2f 7365 6374 696f 6e3e 0a20      </section>. 
+00000dc0: 207b 252d 2065 6e64 626c 6f63 6b20 257d   {%- endblock %}
+00000dd0: 0a7b 252d 2065 6e64 6d61 6372 6f20 257d  .{%- endmacro %}
+00000de0: 0a                                       .
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html`

 * *Files 23% similar despite different names*

```diff
@@ -9,90 +9,99 @@
 {%- extends config.OAUTH2SERVER_SETTINGS_TEMPLATE %}
 
 {# FIXME Import from future formatter. #}
 {%- from "invenio_oauth2server/settings/_macros.html" import render_field with context%}
 {%- import "invenio_oauth2server/settings/helpers.html" as helpers with context %}
 
 {% block settings_content %}
-{{helpers.panel_start(
-    _('Developer Applications'),
-    btn=_('New application'),
-    btn_icon='plus icon',
-    btn_href=url_for('.client_new'),
-    with_body=False,
-)}}
-<div class="ui segment">
-{% if clients %}
-  <p>{{ _('You have registered these applications to use the %(site_name)s API:', site_name=config.THEME_SITENAME) }}</p>
-  <div class="ui divided list">
-    {%- for c in clients %}
-      <div class="item">
-        <a class="header" href="{{url_for('.client_view', client_id=c.client_id)}}">{{c.name}}</a>
-        <div class="description">
-          <small>{{ c.description }}</small>
-        </div>
-      </div>
-    {%- endfor %}
-  </div>
-{% else %}
-  <p>{{ _("You have not yet registered any applications. Click the 'New application' button to create an application to access the %(site_name)s API.", site_name=config['THEME_SITENAME']) }}</p>
-{% endif %}
-</div>
-
-{{helpers.panel_end(with_body=False)}}
-{{helpers.panel_start(
-    _('Personal access tokens'),
-    btn=_('New token'),
-    btn_icon='plus icon',
-    btn_href=url_for('.token_new'),
-    with_body=False,
-)}}
-{% if tokens %}
-  <div class="ui segment">
-    <p>{{ _('Following are personal tokens used to access the %(site_name)s API:', site_name=config.THEME_SITENAME) }}</p>
-    <div class="ui divided list">
+  {{helpers.panel_start(
+      _('Developer applications'),
+      btn=_('New application'),
+      btn_icon='plus icon',
+      btn_href=url_for('.client_new'),
+      with_body=False,
+  )}}
+  {% if clients %}
+    <p class="ui segment">{{ _('You have registered these applications to use the %(site_name)s API:', site_name=config.THEME_SITENAME) }}</p>
+    <ul class="ui segments no-style-list no-border no-border-radius-top m-0 p-0">
+      {%- for c in clients %}
+        <li class="ui segment">
+          <a href="{{url_for('.client_view', client_id=c.client_id)}}">{{c.name}}</a>
+          <div class="description">
+            <small>{{ c.description }}</small>
+          </div>
+        </li>
+      {%- endfor %}
+      </ul>
+  {% else %}
+    <p class="ui segment">{{ _("You have not yet registered any applications. Click the 'New application' button to create an application to access the %(site_name)s API.", site_name=config['THEME_SITENAME']) }}</p>
+  {% endif %}
+  {{helpers.panel_end(with_body=False)}}
+
+
+  {{helpers.panel_start(
+      _('Personal access tokens'),
+      btn=_('New token'),
+      btn_icon='plus icon',
+      btn_href=url_for('.token_new'),
+      with_body=False,
+  )}}
+  {% if tokens %}
+    <p class="ui segment">
+      {{ _('Following are personal tokens used to access the %(site_name)s API:', site_name=config.THEME_SITENAME) }}
+    </p>
+
+    <ul class="ui segments no-style-list no-border no-border-radius-top m-0 p-0">
       {%- for t in tokens %}
-        <div class="item">
+        <li class="ui segment">
           <a class="header" href="{{url_for('.token_view', token_id=t.id)}}">{{ t.client.name }}</a>
-          <div class="description">
+          <ul class="ui horizontal bulleted link list block">
             {% if t.scopes %}
-              {% for s in t.get_visible_scopes() %}{{ s }}{% if not loop.last%}, {% endif%}{% endfor %}
+              {% for s in t.get_visible_scopes() %}
+                <li class="item ml-0">{{ s }}{% if not loop.last%}, {% endif%}</li>
+              {% endfor %}
             {% endif %}
-            <br/><small>{{ t.client.description }}</small>
-          </div>
-        </div>
+          </ul>
+          <small>{{ t.client.description }}</small>
+        </li>
       {%- endfor %}
-    </div>
-  </div>
+    </ul>
+
+  {% else %}
+    <p class="ui segment">
+      {{ _("You have not yet created any personal access tokens. Click the 'New token' button to create a personal access token.") }}
+    </p>
+  {% endif %}
+  {{helpers.panel_end(with_body=False)}}
+
+
+  {{helpers.panel_start(
+      _('Authorized applications'),
+      with_body=False,
+  )}}
 
-{% else %}
-  <div class="ui segment">
-    <p>{{ _("You have not yet created any personal access tokens. Click the 'New token' button to create a personal access token.") }}</p>
-  </div>
-{% endif %}
-{{helpers.panel_end(with_body=False)}}
-{{helpers.panel_start(
-    _('Authorized applications'),
-    with_body=False,
-)}}
-<div class="ui segment">
-{% if authorized_apps %}
-  <p>{{ _('You have granted the following application access to your account:') }}</p>
-  <div class="ui divided list">
-    {%- for a in authorized_apps %}
-      <div class="item">
-        <div class="right floated content">
-          <a href="{{url_for('.token_revoke', token_id=a.id)}}" class="ui tiny button primary"><i class="icon x"></i> {{ _('Revoke') }}</a>
-        </div>
-        <a class="header" href="{{url_for('.token_permission_view', token_id=a.id)}}">{{a.client.name}}</a>
-        <div class="description">
-          {{a.client.description}}
-        </div>
-      </div>
-    {%- endfor %}
-</div>
-{% else %}
-  <p>{{ _('You have not yet granted any external applications access to your account.') }}</p>
-{% endif %}
-</div>
-{{helpers.panel_end(with_body=False)}}
+    {% if authorized_apps %}
+      <p class="ui segment">{{ _('You have granted the following application access to your account:') }}</p>
+      <ul class="ui segments no-style-list no-border no-border-radius-top m-0 p-0">
+        {%- for a in authorized_apps %}
+          <li class="ui segment flex justify-space-between">
+            <div>
+              <a class="header" href="{{url_for('.token_permission_view', token_id=a.id)}}">
+                {{a.client.name}}
+              </a>
+              <p>
+                <small>{{a.client.description}}</small>
+              </p>
+            </div>
+            <div>
+              <a href="{{url_for('.token_revoke', token_id=a.id)}}" class="ui tiny labeled icon button">
+                <i class="icon x" aria-hidden="true"></i> {{ _('Revoke') }}
+              </a>
+            </div>
+          </li>
+        {%- endfor %}
+        </ul>
+    {% else %}
+      <p class="ui segment">{{ _('You have not yet granted any external applications access to your account.') }}</p>
+    {% endif %}
+  {{helpers.panel_end(with_body=False)}}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,49 +1,46 @@
 {# -*- coding: utf-8 -*- This file is part of Invenio. Copyright (C) 2015-2020
 CERN. Invenio is free software; you can redistribute it and/or modify it under
 the terms of the MIT License; see LICENSE file for more details. #} {%- extends
 config.OAUTH2SERVER_SETTINGS_TEMPLATE %} {# FIXME Import from future formatter.
 #} {%- from "invenio_oauth2server/settings/_macros.html" import render_field
 with context%} {%- import "invenio_oauth2server/settings/helpers.html" as
 helpers with context %} {% block settings_content %} {{helpers.panel_start( _
-('Developer Applications'), btn=_('New application'), btn_icon='plus icon',
-btn_href=url_for('.client_new'), with_body=False, )}}
-{% if clients %}
+('Developer applications'), btn=_('New application'), btn_icon='plus icon',
+btn_href=url_for('.client_new'), with_body=False, )}} {% if clients %}
 {{ _('You have registered these applications to use the %(site_name)s API:',
 site_name=config.THEME_SITENAME) }}
-{%- for c in clients %}
-{{c.name}}
-{{ c.description }}
-{%- endfor %}
+    * {%- for c in clients %}
+    * {{c.name}}
+      {{ c.description }}
+    * {%- endfor %}
 {% else %}
 {{ _("You have not yet registered any applications. Click the 'New application'
 button to create an application to access the %(site_name)s API.",
 site_name=config['THEME_SITENAME']) }}
-{% endif %}
-{{helpers.panel_end(with_body=False)}} {{helpers.panel_start( _('Personal
-access tokens'), btn=_('New token'), btn_icon='plus icon', btn_href=url_for
-('.token_new'), with_body=False, )}} {% if tokens %}
+{% endif %} {{helpers.panel_end(with_body=False)}} {{helpers.panel_start( _
+('Personal access tokens'), btn=_('New token'), btn_icon='plus icon',
+btn_href=url_for('.token_new'), with_body=False, )}} {% if tokens %}
 {{ _('Following are personal tokens used to access the %(site_name)s API:',
 site_name=config.THEME_SITENAME) }}
-{%- for t in tokens %}
-{{_t.client.name_}}
-{% if t.scopes %} {% for s in t.get_visible_scopes() %}{{ s }}{% if not
-loop.last%}, {% endif%}{% endfor %} {% endif %}
-{{ t.client.description }}
-{%- endfor %}
+    * {%- for t in tokens %}
+    * {{_t.client.name_}}
+          o {% if t.scopes %} {% for s in t.get_visible_scopes() %}
+          o {{ s }}{% if not loop.last%}, {% endif%}
+          o {% endfor %} {% endif %}
+      {{ t.client.description }}
+    * {%- endfor %}
 {% else %}
 {{ _("You have not yet created any personal access tokens. Click the 'New
 token' button to create a personal access token.") }}
 {% endif %} {{helpers.panel_end(with_body=False)}} {{helpers.panel_start( _
-('Authorized applications'), with_body=False, )}}
-{% if authorized_apps %}
+('Authorized applications'), with_body=False, )}} {% if authorized_apps %}
 {{ _('You have granted the following application access to your account:') }}
-{%- for a in authorized_apps %}
- {{__('Revoke')_}}
-{{a.client.name}}
-{{a.client.description}}
-{%- endfor %}
+    * {%- for a in authorized_apps %}
+    * {{a.client.name}}
+      {{a.client.description}}
+       {{__('Revoke')_}}
+    * {%- endfor %}
 {% else %}
 {{ _('You have not yet granted any external applications access to your
 account.') }}
-{% endif %}
-{{helpers.panel_end(with_body=False)}} {% endblock %}
+{% endif %} {{helpers.panel_end(with_body=False)}} {% endblock %}
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_new.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_new.html`

 * *Files 13% similar despite different names*

```diff
@@ -12,21 +12,23 @@
 
 {%- import "invenio_oauth2server/settings/helpers.html" as helpers with context %}
 {%- from "invenio_oauth2server/settings/_macros.html" import render_field, render_scopes_field with context %}
 
 {% block settings_content %}
 {{ helpers.panel_start(
     _('New personal access token'),
+    breadcrumb_path=url_for('.index'),
+    breadcrumb_title=_('Applications'),
 ) }}
 <form class="ui form" role="form" method="POST">
   {{ render_field(form.name, autofocus=True) }}
   {{ render_scopes_field(form.scopes) }}
   {{ form.csrf_token }}
-  <a href="{{ url_for('.index') }}" class="ui button">
-    <i class="icon x"></i> {{ _('Cancel') }}
+  <a href="{{ url_for('.index') }}" class="ui labeled icon button">
+    <i class="icon x" aria-hidden="true"></i> {{ _('Cancel') }}
   </a>
-  <button type="submit" class="ui button primary">
-    <i class="icon check"></i> {{ _('Create') }}
+  <button type="submit" class="ui labeled icon button primary">
+    <i class="icon check" aria-hidden="true"></i> {{ _('Create') }}
   </button>
 </form>
 {{helpers.panel_end()}}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {# -*- coding: utf-8 -*- This file is part of Invenio. Copyright (C) 2015-2020
 CERN. Invenio is free software; you can redistribute it and/or modify it under
 the terms of the MIT License; see LICENSE file for more details. #} {%- extends
 "invenio_oauth2server/settings/index.html" %} {%- import "invenio_oauth2server/
 settings/helpers.html" as helpers with context %} {%- from
 "invenio_oauth2server/settings/_macros.html" import render_field,
 render_scopes_field with context %} {% block settings_content %} {
-{ helpers.panel_start( _('New personal access token'), ) }}
+{ helpers.panel_start( _('New personal access token'), breadcrumb_path=url_for
+('.index'), breadcrumb_title=_('Applications'), ) }}
 {{ render_field(form.name, autofocus=True) }} {{ render_scopes_field
 (form.scopes) }} {{ form.csrf_token }}
  {{__('Cancel')_}}
    {{ _('Create') }}
 {{helpers.panel_end()}} {% endblock %}
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_permission_view.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_permission_view.html`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html` & `invenio-oauth2server-2.1.0/invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html`

 * *Files 16% similar despite different names*

```diff
@@ -9,49 +9,56 @@
 
 {%- extends "invenio_oauth2server/settings/index.html" %}
 
 {%- import "invenio_oauth2server/settings/helpers.html" as helpers with context %}
 {%- from "invenio_oauth2server/settings/_macros.html" import render_field, render_scopes_field with context %}
 
 {% block settings_content %}
-{{ helpers.panel_start(
-    _('Personal access token / %(name)s',
-    name=token.client.name),
-    with_body=False,
-) }}
-{% if show_token %}
-<div class="ui segment">
-  <p>
-    <strong>{{ _('Access token') }}</strong><br>
-    <div class="ui small label">
-      <code>{{ token.access_token }}</code>
-    </div>
-  </p>
-  <div class="ui info message">
-    <p><i class="bullhorn icon"></i> {{ _("Please copy the personal access token now. You won't see it again!") }}</p>
-  </div>
-  <div class="ui negative message">
-    <p><i class="exclamation triangle icon"></i> {{ _('Do not share this personal access token. It gives full access to your account.') }}</p>
+  {{ helpers.panel_start(
+      _('%(name)s', name=token.client.name),
+      breadcrumb_path=url_for('.index'),
+      breadcrumb_title=_('Applications'),
+      with_body=False,
+  ) }}
+  {% if show_token %}
+  <div class="ui segment">
+    <h3 class="ui small header">{{ _('Access token') }}</h3>
+    <code class="word-break-all">{{ token.access_token }}</code>
+
+    <p class="ui icon info message">
+      <i class="bullhorn large icon" aria-hidden="true"></i>
+      {{ _("Please copy the personal access token now. You won't see it again!") }}
+    </p>
+
+    <p class="ui icon negative message">
+      <i class="exclamation triangle large icon" aria-hidden="true"></i>
+      {{ _('Do not share this personal access token. It gives full access to your account.') }}
+    </p>
+
+    {%- block token_footer_text %}{%- endblock %}
   </div>
-  {%- block token_footer_text %}{%- endblock %}
-</div>
-{% endif %}
-<div class="ui segment">
+
+  {% endif %}
+  <div class="ui segment">
     {% if not show_token %}
-    <div class="ui warning message">
-      <p>{{ _("If you've lost or forgotten this token please create a new one. Be aware that any scripts or applications using this token will need to be updated.") }}</p>
-    </div>
+      <p class="ui warning message">
+        {{ _("If you've lost or forgotten this token please create a new one. Be aware that any scripts or applications using this token will need to be updated.") }}
+      </p>
     {% endif %}
+
     <form class="ui form" method="POST" role="form" action="">
       {{ render_field(form.name, autofocus=True) }}
       {{ render_scopes_field(form.scopes) }}
       {{ form.csrf_token }}
-      <button type="submit" name="delete" class="ui button negative">
-        <i class="icon trash"></i> {{ _('Delete') }}
-      </button>
-      <button type="submit" name="save" class="ui button primary">
-        <i class="icon check"></i> {{ _('Save') }}
-      </button>
+
+      <div class="rel-mt-2">
+        <button type="submit" name="delete" class="ui labeled icon button negative">
+          <i class="icon trash" aria-hidden="true"></i> {{ _('Delete') }}
+        </button>
+        <button type="submit" name="save" class="ui labeled icon button primary">
+          <i class="icon check" aria-hidden="true"></i> {{ _('Save') }}
+        </button>
+      </div>
     </form>
-</div>
-{{helpers.panel_end(with_body=False)}}
+  </div>
+  {{helpers.panel_end(with_body=False)}}
 {% endblock %}
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/theme/semantic/form_styling.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/theme/semantic/form_styling.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,28 +14,34 @@
 
     def __init__(self, multiple=False):
         """Init."""
         self.multiple = multiple
 
     def __call__(self, field, **kwargs):
         """Render select field."""
-        html = ['<div class="ui fluid selection dropdown">']
+        html = [
+            '<div role="listbox" aria-expanded="false" class="ui fluid selection dropdown">'
+        ]
         html.append('<input type="hidden" name="{0}">'.format(field.name))
-        html.append('<i class="dropdown icon"></i>')
+        html.append('<i class="dropdown icon" aria-hidden="true"></i>')
         items_html = []
         default_text_html = []
         for val, label, selected in field.iter_choices():
             if selected:
                 default_text_html = [
-                    '<div class="text">{0}</div><div class="menu">'.format(label)
+                    '<div aria-atomic="true" aria-live="polite" class="text">{0}</div><div class="menu">'.format(
+                        label
+                    )
                 ]
             items_html.append(self.render_option(val, label, selected))
         items_html.append("</div></div>")
         html = html + default_text_html + items_html
         return HTMLString("".join(html))
 
     @classmethod
     def render_option(cls, value, label, selected, **kwargs):
         """Render option."""
         return HTMLString(
-            '<div class="item" data-value="{0}">{1}</div>'.format(value, label)
+            (
+                '<div role="option" aria-selected="{2}" class="item" data-value="{0}">{1}</div>'
+            ).format(value, label, selected)
         )
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/af/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/af/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 4461 7465 3a20 3230 3136 2d30 382d 3138  Date: 2016-08-18
 000000d0: 2030 383a 3033 2b30 3030 300a 4c61 7374   08:03+0000.Last
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/af/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/af/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
-"Language-Team: Afrikaans (https://www.transifex.com/inveniosoftware/teams/23537/af/)\n"
+"Language-Team: Afrikaans (https://app.transifex.com/inveniosoftware/teams/23537/af/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: af\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
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
@@ -21,37 +21,37 @@
 msgid "Access token"
 msgstr "رمز ولوج"
 
 msgid "Access token URL (POST)"
 msgstr "عنوان ويب URL لرمز الولوج ( طلب POST)"
 
 msgid "Allow access to email address (read-only)."
-msgstr "تمكين الولوج لعنوان البريد (للقراءة فقط)."
+msgstr "السّماح بالولوج لعنوان البريد (للقراءة فقط)."
 
 msgid "Application"
 msgstr "تطبيق"
 
 msgid ""
 "Application '%(client_name)s' by '%(client_user)s' wants permission to "
 "access your '%(current_user)s' account."
 msgstr ""
-"تطبيق '%(client_name)s' لـ '%(client_user)s' يريد إذنًا للولوج إلى حساب "
+"تطبيق '%(client_name)s' من طرف  '%(client_user)s' يريد إذنًا للولوج إلى حسابك "
 "'%(current_user)s' ."
 
 msgid "Application / %(client_name)s"
 msgstr "تطبيق / %(client_name)s"
 
 msgid "Applications"
 msgstr "تطبيقات"
 
 msgid "Authorize URL (GET)"
 msgstr "ترخيص URL  (طلب GET)"
 
 msgid "Authorize application"
-msgstr "التطبيق المخول"
+msgstr "الإذن بالتّطبيق"
 
 msgid "Authorized application: %(client_name)s"
 msgstr "تطبيق مخول :%(client_name)s"
 
 msgid "Authorized applications"
 msgstr "التطبيقات المخولة"
 
@@ -168,15 +168,15 @@
 msgid "Personal access tokens"
 msgstr "رموز الولوج الشخصي. "
 
 msgid "Please copy the personal access token now. You won't see it again!"
 msgstr "يرجى نسخ رمز الولوج الشخصي الآن. لن يمكنك رأيته مرة أخرى!"
 
 msgid "Public"
-msgstr "عام"
+msgstr "مشاع"
 
 msgid "Query parameters"
 msgstr "معلمات الاستعلام"
 
 msgid "Redirect URIs (one per line)"
 msgstr "إعادة توجيه عناوين ويب URIs (واحد لكل سطر)  "
 
@@ -213,17 +213,17 @@
 msgid ""
 "Select confidential if your application is capable of keeping the issued "
 "client secret confidential (e.g. a web application), select public if your "
 "application cannot (e.g. a browser-based JavaScript application). If you "
 "select public, your application MUST validate the redirect URI."
 msgstr ""
 " اختر \"سري\" إذا كان التطبيق الخاص بك قادرًا على الحفاظ على سرية الحريف (على "
-"سبيل المثال ، تطبيق ويب) ، حدد \"عام\" إذا كان التطبيق الخاص بك لا يمكنه ذلك "
-"(على سبيل المثال ، تطبيق تعتمد على متصفح  JavaScript ). إذا قمت بتحديد "
-"\"عام\" ، يجب أن يتحقق التطبيق الخاص بك من صحة عنوان URI لإعادة التوجيه."
+"سبيل المثال ، تطبيق ويب) ، حدد \"مشاع\" إذا كان التطبيق الخاص بك لا يمكنه "
+"ذلك (على سبيل المثال ، تطبيق تعتمد على متصفح  JavaScript ). إذا قمت بتحديد "
+"\"مشاع\" ، يجب أن يتحقق التطبيق الخاص بك من صحة عنوان URI لإعادة التوجيه."
 
 msgid "The name must be less than 40 characters long."
 msgstr "يجب أن يكون طول الاسم أقل من 40 حرفا."
 
 msgid ""
 "The service that redirected your here made an invalid authorization request "
 "(error code: %(x_error)s)."
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ar/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-oauth2server project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2021
-# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022
 # Bessem Aamira <bessemamira@gmail.com>, 2022
+# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
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
 
@@ -64,26 +64,26 @@
 msgid ""
 "Select confidential if your application is capable of keeping the issued "
 "client secret confidential (e.g. a web application), select public if your "
 "application cannot (e.g. a browser-based JavaScript application). If you "
 "select public, your application MUST validate the redirect URI."
 msgstr ""
 " اختر \"سري\" إذا كان التطبيق الخاص بك قادرًا على الحفاظ على سرية الحريف "
-"(على سبيل المثال ، تطبيق ويب) ، حدد \"عام\" إذا كان التطبيق الخاص بك لا "
+"(على سبيل المثال ، تطبيق ويب) ، حدد \"مشاع\" إذا كان التطبيق الخاص بك لا "
 "يمكنه ذلك (على سبيل المثال ، تطبيق تعتمد على متصفح  JavaScript ). إذا قمت "
-"بتحديد \"عام\" ، يجب أن يتحقق التطبيق الخاص بك من صحة عنوان URI لإعادة "
+"بتحديد \"مشاع\" ، يجب أن يتحقق التطبيق الخاص بك من صحة عنوان URI لإعادة "
 "التوجيه."
 
 #: invenio_oauth2server/forms.py:164
 msgid "Confidential"
 msgstr "سري"
 
 #: invenio_oauth2server/forms.py:164
 msgid "Public"
-msgstr "عام"
+msgstr "مشاع"
 
 #: invenio_oauth2server/forms.py:174
 msgid "Name of personal access token."
 msgstr "إسم الرمز للولوج الشخصي. "
 
 #: invenio_oauth2server/forms.py:178
 msgid "The name must be less than 40 characters long."
@@ -121,35 +121,35 @@
 
 #: invenio_oauth2server/models.py:145
 msgid "URL of your application (displayed to users)."
 msgstr "URL تطبيقك  (المعروض للمستخدمين)."
 
 #: invenio_oauth2server/scopes.py:20
 msgid "Allow access to email address (read-only)."
-msgstr "تمكين الولوج لعنوان البريد (للقراءة فقط)."
+msgstr "السّماح بالولوج لعنوان البريد (للقراءة فقط)."
 
 #: invenio_oauth2server/templates/invenio_oauth2server/authorize.html:19
 #: invenio_oauth2server/templates/invenio_oauth2server/authorize.html:20
 #: invenio_oauth2server/templates/invenio_oauth2server/authorize.html:59
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html:18
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html:21
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html:66
 #: invenio_oauth2server/views/server.py:67
 msgid "Authorize application"
-msgstr "التطبيق المخول"
+msgstr "الإذن بالتّطبيق"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/authorize.html:21
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html:23
 #, python-format
 msgid ""
 "Application '%(client_name)s' by '%(client_user)s' wants permission to "
 "access your '%(current_user)s' account."
 msgstr ""
-"تطبيق '%(client_name)s' لـ '%(client_user)s' يريد إذنًا للولوج إلى حساب "
-"'%(current_user)s' ."
+"تطبيق '%(client_name)s' من طرف  '%(client_user)s' يريد إذنًا للولوج إلى "
+"حسابك '%(current_user)s' ."
 
 #: invenio_oauth2server/templates/invenio_oauth2server/authorize.html:28
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_permission_view.html:30
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html:34
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_permission_view.html:26
 msgid "Review permissions"
 msgstr "مراجعة الأذون"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/bg/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/teams/23537/bg/)\n"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/teams/23537/bg/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Ferran Jorba <Ferran.Jorba@uab.cat>, 2021\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ca/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Ferran Jorba <Ferran.Jorba@uab.cat>, 2021\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/teams/23537/ca/)\n"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/teams/23537/ca/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Jiří Kunčar <jiri.kuncar@gmail.com>, 2021\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/cs/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Jiří Kunčar <jiri.kuncar@gmail.com>, 2021\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/cs/)\n"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/cs/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/da/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/da/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Lars Holm Nielsen <lars.holm.nielsen@cern.ch>, 2022\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/da/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/da/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Lars Holm Nielsen <lars.holm.nielsen@cern.ch>, 2022\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/da/)\n"
+"Language-Team: Danish (https://app.transifex.com/inveniosoftware/teams/23537/da/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: da\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/de/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/de/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/de/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/de/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/el/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/el/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Theodoros Theodoropoulos, 2021\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/el/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/el/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Theodoros Theodoropoulos, 2021\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/el/)\n"
+"Language-Team: Greek (https://app.transifex.com/inveniosoftware/teams/23537/el/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/es/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/es/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2021\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/es/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/es/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Jesús Martín <jesusmartin@sallep.net>, 2021\n"
-"Language-Team: Spanish (https://www.transifex.com/inveniosoftware/teams/23537/es/)\n"
+"Language-Team: Spanish (https://app.transifex.com/inveniosoftware/teams/23537/es/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: es\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/et/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/et/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/et/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/et/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 eb01 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 ec01 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d6f 6175 7468 3273   invenio-oauth2s
 00000050: 6572 7665 7220 312e 332e 370a 5265 706f  erver 1.3.7.Repo
 00000060: 7274 2d4d 7367 6964 2d42 7567 732d 546f  rt-Msgid-Bugs-To
 00000070: 3a20 696e 666f 4069 6e76 656e 696f 736f  : info@invenioso
 00000080: 6674 7761 7265 2e6f 7267 0a50 4f54 2d43  ftware.org.POT-C
 00000090: 7265 6174 696f 6e2d 4461 7465 3a20 3230  reation-Date: 20
 000000a0: 3232 2d31 302d 3132 2030 393a 3236 2b30  22-10-12 09:26+0
 000000b0: 3030 300a 504f 2d52 6576 6973 696f 6e2d  000.PO-Revision-
 000000c0: 4461 7465 3a20 3230 3136 2d30 382d 3138  Date: 2016-08-18
 000000d0: 2030 383a 3033 2b30 3030 300a 4c61 7374   08:03+0000.Last
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
+00000110: 2068 755f 4855 0a4c 616e 6775 6167 652d   hu_HU.Language-
+00000120: 5465 616d 3a20 4875 6e67 6172 6961 6e20  Team: Hungarian 
+00000130: 2848 756e 6761 7279 2920 2868 7474 7073  (Hungary) (https
+00000140: 3a2f 2f61 7070 2e74 7261 6e73 6966 6578  ://app.transifex
+00000150: 2e63 6f6d 2f69 6e76 656e 696f 736f 6674  .com/inveniosoft
+00000160: 7761 7265 2f74 6561 6d73 2f32 3335 3337  ware/teams/23537
+00000170: 2f68 755f 4855 2f29 0a50 6c75 7261 6c2d  /hu_HU/).Plural-
+00000180: 466f 726d 733a 206e 706c 7572 616c 733d  Forms: nplurals=
+00000190: 323b 2070 6c75 7261 6c3d 286e 2021 3d20  2; plural=(n != 
+000001a0: 3129 3b0a 4d49 4d45 2d56 6572 7369 6f6e  1);.MIME-Version
+000001b0: 3a20 312e 300a 436f 6e74 656e 742d 5479  : 1.0.Content-Ty
+000001c0: 7065 3a20 7465 7874 2f70 6c61 696e 3b20  pe: text/plain; 
+000001d0: 6368 6172 7365 743d 7574 662d 380a 436f  charset=utf-8.Co
+000001e0: 6e74 656e 742d 5472 616e 7366 6572 2d45  ntent-Transfer-E
+000001f0: 6e63 6f64 696e 673a 2038 6269 740a 4765  ncoding: 8bit.Ge
+00000200: 6e65 7261 7465 642d 4279 3a20 4261 6265  nerated-By: Babe
+00000210: 6c20 322e 3132 2e31 0a00                 l 2.12.1..
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
-"Language-Team: Estonian (Estonia) (https://www.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
+"Language-Team: English (Hungary) (https://app.transifex.com/inveniosoftware/teams/23537/en_HU/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: et_EE\n"
+"Language: en_HU\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_oauth2server/admin.py:68
 msgid "OAuth Applications"
 msgstr ""
 
 #: invenio_oauth2server/admin.py:69 invenio_oauth2server/admin.py:78
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fa/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
-"Language-Team: Persian (https://www.transifex.com/inveniosoftware/teams/23537/fa/)\n"
+"Language-Team: Persian (https://app.transifex.com/inveniosoftware/teams/23537/fa/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fa\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2021\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/fr/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2021\n"
-"Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/fr/)\n"
+"Language-Team: French (https://app.transifex.com/inveniosoftware/teams/23537/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 4461 7465 3a20 3230 3136 2d30 382d 3138  Date: 2016-08-18
 000000d0: 2030 383a 3033 2b30 3030 300a 4c61 7374   08:03+0000.Last
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/gl/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
-"Language-Team: Galician (https://www.transifex.com/inveniosoftware/teams/23537/gl/)\n"
+"Language-Team: Galician (https://app.transifex.com/inveniosoftware/teams/23537/gl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: gl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/no/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/teams/23537/hr/)\n"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/teams/23537/no/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: hr\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"Language: no\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_oauth2server/admin.py:68
 msgid "OAuth Applications"
 msgstr ""
 
 #: invenio_oauth2server/admin.py:69 invenio_oauth2server/admin.py:78
 msgid "User Management"
@@ -84,23 +84,23 @@
 "Scopes assign permissions to your personal access token. A personal access "
 "token works just like a normal OAuth  access token for authentication "
 "against the API."
 msgstr ""
 
 #: invenio_oauth2server/models.py:122
 msgid "Name"
-msgstr "Ime"
+msgstr "Navn"
 
 #: invenio_oauth2server/models.py:123
 msgid "Name of application (displayed to users)."
 msgstr ""
 
 #: invenio_oauth2server/models.py:133
 msgid "Description"
-msgstr "Opis"
+msgstr "Beskrivelse"
 
 #: invenio_oauth2server/models.py:134
 msgid "Optional. Description of the application (displayed to users)."
 msgstr ""
 
 #: invenio_oauth2server/models.py:144
 msgid "Website URL"
@@ -159,15 +159,15 @@
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_permission_view.html:47
 msgid "Visit application website"
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/authorize.html:60
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html:67
 msgid "Reject"
-msgstr ""
+msgstr "Avslå"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/errors.html:18
 #: invenio_oauth2server/templates/invenio_oauth2server/errors.html:22
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html:17
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html:20
 msgid "Invalid authorization request"
 msgstr ""
@@ -191,20 +191,20 @@
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html:25
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_new.html:26
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html:24
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_new.html:25
 msgid "Cancel"
-msgstr "Odustani"
+msgstr "Avbryt"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html:26
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html:27
 msgid "Register"
-msgstr "Registriraj se"
+msgstr "Registrer"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:17
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:18
 #, python-format
 msgid "Application / %(client_name)s"
 msgstr ""
 
@@ -229,22 +229,22 @@
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:47
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html:48
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:51
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html:49
 msgid "Delete"
-msgstr "Briši"
+msgstr "Slett"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:48
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html:49
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:54
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html:52
 msgid "Save"
-msgstr "Spremi"
+msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:55
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:60
 msgid "OAuth 2.0 Endpoints"
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:59
@@ -424,15 +424,15 @@
 msgid ""
 "If you've lost or forgotten this token please create a new one. Be aware "
 "that any scripts or applications using this token will need to be updated."
 msgstr ""
 
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:81
 msgid "or"
-msgstr "ili"
+msgstr "eller"
 
 #: invenio_oauth2server/views/settings.py:105
 #, python-format
 msgid "%(icon)s Applications"
 msgstr ""
 
 #: invenio_oauth2server/views/settings.py:110
@@ -443,8 +443,8 @@
 #: invenio_oauth2server/views/settings.py:212
 msgid "New"
 msgstr ""
 
 #: invenio_oauth2server/views/settings.py:174
 #: invenio_oauth2server/views/settings.py:238
 msgid "Edit"
-msgstr "Uredi"
+msgstr "Endre"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
-"Last-Translator: Andrea Dömötör, 2022\n"
+"Last-Translator: Andrea Dömötör, 2023\n"
 "Language: hu\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/hu/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
@@ -20,24 +20,24 @@
 msgid "Access token"
 msgstr "Hozzáférési token"
 
 msgid "Access token URL (POST)"
 msgstr "Hozzáférési token URL (POST)"
 
 msgid "Allow access to email address (read-only)."
-msgstr "Hozzáférés engedélyezése az email címnek (csak olvasás)"
+msgstr "Hozzáférés engedélyezése az email címnek (csak olvasás)."
 
 msgid "Application"
 msgstr "Alkalmazás"
 
 msgid ""
 "Application '%(client_name)s' by '%(client_user)s' wants permission to "
 "access your '%(current_user)s' account."
 msgstr ""
-"'%(client_user)s' '%(client_name)s' alkalmazása szeretne hozzáférni az ön "
+"'%(client_user)s' '%(client_name)s' alkalmazása szeretne hozzáférni az Ön "
 "'%(current_user)s' fiókjához."
 
 msgid "Application / %(client_name)s"
 msgstr "Alkalmazás / %(client_name)s"
 
 msgid "Applications"
 msgstr "Alkalmazások"
@@ -57,15 +57,15 @@
 msgid "Cancel"
 msgstr "Mégsem"
 
 msgid "Client ID"
 msgstr "Kliens ID"
 
 msgid "Client Secret"
-msgstr "Ügyfél titok"
+msgstr "Ügyféltitok"
 
 msgid "Client type"
 msgstr "Ügyfél típus"
 
 msgid "Confidential"
 msgstr "Titkos"
 
@@ -78,15 +78,15 @@
 msgid "Description"
 msgstr "Leírás"
 
 msgid "Developer Applications"
 msgstr "Fejlesztői alkalmazások"
 
 msgid "Do not share the client secret with anyone!"
-msgstr "Az ügyfél titok megosztása másokkal nem ajánlatos!"
+msgstr "Az ügyféltitok megosztása másokkal nem ajánlatos!"
 
 msgid ""
 "Do not share this personal access token. It gives full access to your "
 "account."
 msgstr ""
 "Ne ossza meg ezt a személyes hozzáférési tokent! Ez teljes hozzáférést ad a "
 "felhasználói fiókjához."
@@ -188,15 +188,15 @@
 msgid "Reject"
 msgstr "Elutasítás"
 
 msgid "Request body parameters:"
 msgstr "Szövegtörzs paraméterek kérése:"
 
 msgid "Reset client secret"
-msgstr "Ügyfél titok visszaállítása"
+msgstr "Ügyféltitok visszaállítása"
 
 msgid "Review permissions"
 msgstr "Jogosultságok áttekintése"
 
 msgid "Revoke"
 msgstr "Visszavonás"
 
@@ -208,14 +208,26 @@
 "token works just like a normal OAuth  access token for authentication "
 "against the API."
 msgstr ""
 "A hatókörök engedélyeket rendelnek hozzá az ön személyes hozzáférési "
 "tokenjéhez. A személyes hozzáférési token ugyanúgy működik API-"
 "hitelesítésre, mint egy normál OAuth hozzáférési token."
 
+msgid ""
+"Select confidential if your application is capable of keeping the issued "
+"client secret confidential (e.g. a web application), select public if your "
+"application cannot (e.g. a browser-based JavaScript application). If you "
+"select public, your application MUST validate the redirect URI."
+msgstr ""
+"Válassza a Bizalmas lehetőséget, ha az Ön alkalmazása képes a kiadott kliens "
+"titkosítására (pl. webes alkalmazás), egyébként (pl. böngésző alapú "
+"JavaScript alkalmazás) válassza a Nyilvános lehetőséget. Ha a Nyilvános "
+"lehetőséget választja, az alkalmazásnak érvényesíteni KELL az átirányítási "
+"URI-t."
+
 msgid "The name must be less than 40 characters long."
 msgstr "A névnek kevesebb, mint 40 karakterből kell állnia."
 
 msgid ""
 "The service that redirected your here made an invalid authorization request "
 "(error code: %(x_error)s)."
 msgstr ""
@@ -263,9 +275,24 @@
 
 msgid "example request"
 msgstr "példa kérés"
 
 msgid "or"
 msgstr "vagy"
 
+msgid "recommended, for CSRF protection"
+msgstr "CSRF védelemhez ajánlott"
+
 msgid "required"
 msgstr "kötelező"
+
+msgid "required for grant_type"
+msgstr "szükséges ehhez: grant_type"
+
+msgid "required, URL encoded"
+msgstr "kötelező, URL-kódolt"
+
+msgid "required, space separate list of scopes"
+msgstr "kötelező, hatókörök listája space-szel elválasztva"
+
+msgid "required, use"
+msgstr "kötelező, használja"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hu/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Translations template for invenio-oauth2server.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-oauth2server project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
-# Andrea Dömötör, 2022
+# Dorottya Szemigán, 2023
+# Andrea Dömötör, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
-"Last-Translator: Andrea Dömötör, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/teams/23537/hu/)\n"
+"Last-Translator: Andrea Dömötör, 2023\n"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/teams/23537/hu/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
@@ -61,14 +62,19 @@
 #: invenio_oauth2server/forms.py:156
 msgid ""
 "Select confidential if your application is capable of keeping the issued "
 "client secret confidential (e.g. a web application), select public if your "
 "application cannot (e.g. a browser-based JavaScript application). If you "
 "select public, your application MUST validate the redirect URI."
 msgstr ""
+"Válassza a Bizalmas lehetőséget, ha az Ön alkalmazása képes a kiadott kliens"
+" titkosítására (pl. webes alkalmazás), egyébként (pl. böngésző alapú "
+"JavaScript alkalmazás) válassza a Nyilvános lehetőséget. Ha a Nyilvános "
+"lehetőséget választja, az alkalmazásnak érvényesíteni KELL az átirányítási "
+"URI-t."
 
 #: invenio_oauth2server/forms.py:164
 msgid "Confidential"
 msgstr "Titkos"
 
 #: invenio_oauth2server/forms.py:164
 msgid "Public"
@@ -114,15 +120,15 @@
 
 #: invenio_oauth2server/models.py:145
 msgid "URL of your application (displayed to users)."
 msgstr "Az ön alkalmazásának URL-je (a felhasználók számára megjelenítve)"
 
 #: invenio_oauth2server/scopes.py:20
 msgid "Allow access to email address (read-only)."
-msgstr "Hozzáférés engedélyezése az email címnek (csak olvasás)"
+msgstr "Hozzáférés engedélyezése az email címnek (csak olvasás)."
 
 #: invenio_oauth2server/templates/invenio_oauth2server/authorize.html:19
 #: invenio_oauth2server/templates/invenio_oauth2server/authorize.html:20
 #: invenio_oauth2server/templates/invenio_oauth2server/authorize.html:59
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html:18
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html:21
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html:66
@@ -133,15 +139,15 @@
 #: invenio_oauth2server/templates/invenio_oauth2server/authorize.html:21
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html:23
 #, python-format
 msgid ""
 "Application '%(client_name)s' by '%(client_user)s' wants permission to "
 "access your '%(current_user)s' account."
 msgstr ""
-"'%(client_user)s' '%(client_name)s' alkalmazása szeretne hozzáférni az ön "
+"'%(client_user)s' '%(client_name)s' alkalmazása szeretne hozzáférni az Ön "
 "'%(current_user)s' fiókjához."
 
 #: invenio_oauth2server/templates/invenio_oauth2server/authorize.html:28
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_permission_view.html:30
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html:34
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_permission_view.html:26
 msgid "Review permissions"
@@ -222,25 +228,25 @@
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:30
 msgid "Client ID"
 msgstr "Kliens ID"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:23
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:36
 msgid "Client Secret"
-msgstr "Ügyfél titok"
+msgstr "Ügyféltitok"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:24
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:39
 msgid "Do not share the client secret with anyone!"
-msgstr "Az ügyfél titok megosztása másokkal nem ajánlatos!"
+msgstr "Az ügyféltitok megosztása másokkal nem ajánlatos!"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:30
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:26
 msgid "Reset client secret"
-msgstr "Ügyfél titok visszaállítása"
+msgstr "Ügyféltitok visszaállítása"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:47
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html:48
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:51
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html:49
 msgid "Delete"
 msgstr "Törlés"
@@ -273,39 +279,39 @@
 msgstr "példa kérés"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:72
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:89
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:81
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:102
 msgid "required, use"
-msgstr ""
+msgstr "kötelező, használja"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:73
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:87
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:88
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:82
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:100
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:101
 msgid "required"
 msgstr "kötelező"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:74
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:83
 msgid "required, space separate list of scopes"
-msgstr ""
+msgstr "kötelező, hatókörök listája space-szel elválasztva"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:75
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:84
 msgid "required, URL encoded"
-msgstr ""
+msgstr "kötelező, URL-kódolt"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:76
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:85
 msgid "recommended, for CSRF protection"
-msgstr ""
+msgstr "CSRF védelemhez ajánlott"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:83
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:93
 msgid "Access token URL (POST)"
 msgstr "Hozzáférési token URL (POST)"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:85
@@ -316,15 +322,15 @@
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:90
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:91
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:92
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:103
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:104
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:105
 msgid "required for grant_type"
-msgstr ""
+msgstr "szükséges ehhez: grant_type"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/index.html:17
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html:17
 msgid "Developer Applications"
 msgstr "Fejlesztői alkalmazások"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/index.html:18
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/it/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/it/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2021\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/it/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/it/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2021\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/teams/23537/it/)\n"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/teams/23537/it/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: it\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ja/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files 25% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,36 +1,36 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
-"Language: ja\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/"
-"teams/23537/ja/)\n"
+"Language: zh_TW\n"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/"
+"teams/23537/zh_TW/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
 msgid "Cancel"
-msgstr "キャンセル"
+msgstr "取消"
 
 msgid "Delete"
-msgstr "削除"
+msgstr "刪除"
 
 msgid "Description"
-msgstr "説明"
+msgstr "描述"
 
 msgid "Edit"
-msgstr "編集"
+msgstr "編輯"
 
 msgid "Name"
-msgstr "名前"
+msgstr "名稱"
 
 msgid "Register"
-msgstr "登録"
+msgstr "註冊"
 
 msgid "or"
-msgstr "または"
+msgstr "或"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ja/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ja/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/teams/23537/ja/)\n"
+"Language-Team: Japanese (https://app.transifex.com/inveniosoftware/teams/23537/ja/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ja\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ka/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/teams/23537/ka/)\n"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/teams/23537/ka/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/lt/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/lt/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/lt/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/hr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/teams/23537/lt/)\n"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/teams/23537/hr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: lt\n"
-"Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Language: hr\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 
 #: invenio_oauth2server/admin.py:68
 msgid "OAuth Applications"
 msgstr ""
 
 #: invenio_oauth2server/admin.py:69 invenio_oauth2server/admin.py:78
 msgid "User Management"
@@ -84,23 +84,23 @@
 "Scopes assign permissions to your personal access token. A personal access "
 "token works just like a normal OAuth  access token for authentication "
 "against the API."
 msgstr ""
 
 #: invenio_oauth2server/models.py:122
 msgid "Name"
-msgstr "Pavadinimas"
+msgstr "Ime"
 
 #: invenio_oauth2server/models.py:123
 msgid "Name of application (displayed to users)."
 msgstr ""
 
 #: invenio_oauth2server/models.py:133
 msgid "Description"
-msgstr "Aprašymas"
+msgstr "Opis"
 
 #: invenio_oauth2server/models.py:134
 msgid "Optional. Description of the application (displayed to users)."
 msgstr ""
 
 #: invenio_oauth2server/models.py:144
 msgid "Website URL"
@@ -159,15 +159,15 @@
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_permission_view.html:47
 msgid "Visit application website"
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/authorize.html:60
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html:67
 msgid "Reject"
-msgstr "Atmesti"
+msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/errors.html:18
 #: invenio_oauth2server/templates/invenio_oauth2server/errors.html:22
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html:17
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html:20
 msgid "Invalid authorization request"
 msgstr ""
@@ -191,20 +191,20 @@
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html:25
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_new.html:26
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html:24
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_new.html:25
 msgid "Cancel"
-msgstr "Atšaukti"
+msgstr "Odustani"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html:26
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html:27
 msgid "Register"
-msgstr "Registruotis"
+msgstr "Registriraj se"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:17
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:18
 #, python-format
 msgid "Application / %(client_name)s"
 msgstr ""
 
@@ -229,22 +229,22 @@
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:47
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html:48
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:51
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html:49
 msgid "Delete"
-msgstr "Ištrinti"
+msgstr "Briši"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:48
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html:49
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:54
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html:52
 msgid "Save"
-msgstr "Išsaugoti"
+msgstr "Spremi"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:55
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:60
 msgid "OAuth 2.0 Endpoints"
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:59
@@ -424,27 +424,27 @@
 msgid ""
 "If you've lost or forgotten this token please create a new one. Be aware "
 "that any scripts or applications using this token will need to be updated."
 msgstr ""
 
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:81
 msgid "or"
-msgstr "ar"
+msgstr "ili"
 
 #: invenio_oauth2server/views/settings.py:105
 #, python-format
 msgid "%(icon)s Applications"
 msgstr ""
 
 #: invenio_oauth2server/views/settings.py:110
 msgid "Applications"
 msgstr ""
 
 #: invenio_oauth2server/views/settings.py:151
 #: invenio_oauth2server/views/settings.py:212
 msgid "New"
-msgstr "Naujas"
+msgstr ""
 
 #: invenio_oauth2server/views/settings.py:174
 #: invenio_oauth2server/views/settings.py:238
 msgid "Edit"
-msgstr "Redaguoti"
+msgstr "Uredi"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/messages.pot` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/no/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/no/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/no/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,38 +2,39 @@
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-oauth2server project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2021
+# Nicolaie Constantinescu, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/teams/23537/no/)\n"
+"Last-Translator: Nicolaie Constantinescu, 2023\n"
+"Language-Team: Romanian (https://app.transifex.com/inveniosoftware/teams/23537/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: no\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: ro\n"
+"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
 
 #: invenio_oauth2server/admin.py:68
 msgid "OAuth Applications"
 msgstr ""
 
 #: invenio_oauth2server/admin.py:69 invenio_oauth2server/admin.py:78
 msgid "User Management"
-msgstr ""
+msgstr "Management utilizator"
 
 #: invenio_oauth2server/admin.py:77
 msgid "OAuth Application Tokens"
 msgstr ""
 
 #: invenio_oauth2server/forms.py:103
 #, python-format
@@ -84,23 +85,23 @@
 "Scopes assign permissions to your personal access token. A personal access "
 "token works just like a normal OAuth  access token for authentication "
 "against the API."
 msgstr ""
 
 #: invenio_oauth2server/models.py:122
 msgid "Name"
-msgstr "Navn"
+msgstr "Nume"
 
 #: invenio_oauth2server/models.py:123
 msgid "Name of application (displayed to users)."
 msgstr ""
 
 #: invenio_oauth2server/models.py:133
 msgid "Description"
-msgstr "Beskrivelse"
+msgstr "Descriere"
 
 #: invenio_oauth2server/models.py:134
 msgid "Optional. Description of the application (displayed to users)."
 msgstr ""
 
 #: invenio_oauth2server/models.py:144
 msgid "Website URL"
@@ -159,15 +160,15 @@
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_permission_view.html:47
 msgid "Visit application website"
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/authorize.html:60
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/authorize.html:67
 msgid "Reject"
-msgstr "Avslå"
+msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/errors.html:18
 #: invenio_oauth2server/templates/invenio_oauth2server/errors.html:22
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html:17
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html:20
 msgid "Invalid authorization request"
 msgstr ""
@@ -191,20 +192,20 @@
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html:25
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_new.html:26
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html:24
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_new.html:25
 msgid "Cancel"
-msgstr "Avbryt"
+msgstr "Anulează"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html:26
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html:27
 msgid "Register"
-msgstr "Registrer"
+msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:17
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:18
 #, python-format
 msgid "Application / %(client_name)s"
 msgstr ""
 
@@ -229,15 +230,15 @@
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:47
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html:48
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:51
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html:49
 msgid "Delete"
-msgstr "Slett"
+msgstr "Şterge"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:48
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html:49
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:54
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html:52
 msgid "Save"
 msgstr ""
@@ -368,15 +369,15 @@
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html:79
 msgid "You have granted the following application access to your account:"
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/index.html:76
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html:84
 msgid "Revoke"
-msgstr ""
+msgstr "Revocă"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/index.html:84
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html:94
 msgid ""
 "You have not yet granted any external applications access to your account."
 msgstr ""
 
@@ -424,15 +425,15 @@
 msgid ""
 "If you've lost or forgotten this token please create a new one. Be aware "
 "that any scripts or applications using this token will need to be updated."
 msgstr ""
 
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:81
 msgid "or"
-msgstr "eller"
+msgstr "sau"
 
 #: invenio_oauth2server/views/settings.py:105
 #, python-format
 msgid "%(icon)s Applications"
 msgstr ""
 
 #: invenio_oauth2server/views/settings.py:110
@@ -443,8 +444,8 @@
 #: invenio_oauth2server/views/settings.py:212
 msgid "New"
 msgstr ""
 
 #: invenio_oauth2server/views/settings.py:174
 #: invenio_oauth2server/views/settings.py:238
 msgid "Edit"
-msgstr "Endre"
+msgstr "Editează"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Karolina Przerwa, 2022\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/pl/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Karolina Przerwa, 2022\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/pl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
 "Language: pt\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/"
 "teams/23537/pt/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/pt/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
+"Last-Translator: Nicolaie Constantinescu, 2023\n"
 "Language: ro\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Romanian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/ro/)\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
 "2:1));\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
@@ -26,9 +26,15 @@
 
 msgid "Edit"
 msgstr "Editează"
 
 msgid "Name"
 msgstr "Nume"
 
+msgid "Revoke"
+msgstr "Revocă"
+
+msgid "User Management"
+msgstr "Management utilizator"
+
 msgid "or"
 msgstr "sau"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ro/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
-"Language-Team: Romanian (https://www.transifex.com/inveniosoftware/teams/23537/ro/)\n"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: ro\n"
-"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
+"Language: zh_TW\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: invenio_oauth2server/admin.py:68
 msgid "OAuth Applications"
 msgstr ""
 
 #: invenio_oauth2server/admin.py:69 invenio_oauth2server/admin.py:78
 msgid "User Management"
@@ -84,23 +84,23 @@
 "Scopes assign permissions to your personal access token. A personal access "
 "token works just like a normal OAuth  access token for authentication "
 "against the API."
 msgstr ""
 
 #: invenio_oauth2server/models.py:122
 msgid "Name"
-msgstr "Nume"
+msgstr "名稱"
 
 #: invenio_oauth2server/models.py:123
 msgid "Name of application (displayed to users)."
 msgstr ""
 
 #: invenio_oauth2server/models.py:133
 msgid "Description"
-msgstr "Descriere"
+msgstr "描述"
 
 #: invenio_oauth2server/models.py:134
 msgid "Optional. Description of the application (displayed to users)."
 msgstr ""
 
 #: invenio_oauth2server/models.py:144
 msgid "Website URL"
@@ -191,20 +191,20 @@
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html:25
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_new.html:26
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html:24
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_new.html:25
 msgid "Cancel"
-msgstr "Anulează"
+msgstr "取消"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html:26
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html:27
 msgid "Register"
-msgstr ""
+msgstr "註冊"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:17
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:18
 #, python-format
 msgid "Application / %(client_name)s"
 msgstr ""
 
@@ -229,15 +229,15 @@
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:47
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html:48
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:51
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html:49
 msgid "Delete"
-msgstr "Şterge"
+msgstr "刪除"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:48
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html:49
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:54
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html:52
 msgid "Save"
 msgstr ""
@@ -424,15 +424,15 @@
 msgid ""
 "If you've lost or forgotten this token please create a new one. Be aware "
 "that any scripts or applications using this token will need to be updated."
 msgstr ""
 
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:81
 msgid "or"
-msgstr "sau"
+msgstr "或"
 
 #: invenio_oauth2server/views/settings.py:105
 #, python-format
 msgid "%(icon)s Applications"
 msgstr ""
 
 #: invenio_oauth2server/views/settings.py:110
@@ -443,8 +443,8 @@
 #: invenio_oauth2server/views/settings.py:212
 msgid "New"
 msgstr ""
 
 #: invenio_oauth2server/views/settings.py:174
 #: invenio_oauth2server/views/settings.py:238
 msgid "Edit"
-msgstr "Editează"
+msgstr "編輯"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ru/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/teams/23537/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/teams/23537/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/rw/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 de01 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 eb01 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d6f 6175 7468 3273   invenio-oauth2s
 00000050: 6572 7665 7220 312e 332e 370a 5265 706f  erver 1.3.7.Repo
 00000060: 7274 2d4d 7367 6964 2d42 7567 732d 546f  rt-Msgid-Bugs-To
 00000070: 3a20 696e 666f 4069 6e76 656e 696f 736f  : info@invenioso
 00000080: 6674 7761 7265 2e6f 7267 0a50 4f54 2d43  ftware.org.POT-C
 00000090: 7265 6174 696f 6e2d 4461 7465 3a20 3230  reation-Date: 20
 000000a0: 3232 2d31 302d 3132 2030 393a 3236 2b30  22-10-12 09:26+0
 000000b0: 3030 300a 504f 2d52 6576 6973 696f 6e2d  000.PO-Revision-
 000000c0: 4461 7465 3a20 3230 3136 2d30 382d 3138  Date: 2016-08-18
 000000d0: 2030 383a 3033 2b30 3030 300a 4c61 7374   08:03+0000.Last
 000000e0: 2d54 7261 6e73 6c61 746f 723a 2046 554c  -Translator: FUL
 000000f0: 4c20 4e41 4d45 203c 454d 4149 4c40 4144  L NAME <EMAIL@AD
 00000100: 4452 4553 533e 0a4c 616e 6775 6167 653a  DRESS>.Language:
-00000110: 2072 770a 4c61 6e67 7561 6765 2d54 6561   rw.Language-Tea
-00000120: 6d3a 204b 696e 7961 7277 616e 6461 2028  m: Kinyarwanda (
-00000130: 6874 7470 733a 2f2f 7777 772e 7472 616e  https://www.tran
-00000140: 7369 6665 782e 636f 6d2f 696e 7665 6e69  sifex.com/inveni
-00000150: 6f73 6f66 7477 6172 652f 7465 616d 732f  osoftware/teams/
-00000160: 3233 3533 372f 7277 2f29 0a50 6c75 7261  23537/rw/).Plura
-00000170: 6c2d 466f 726d 733a 206e 706c 7572 616c  l-Forms: nplural
-00000180: 733d 323b 2070 6c75 7261 6c3d 286e 2021  s=2; plural=(n !
-00000190: 3d20 3129 3b0a 4d49 4d45 2d56 6572 7369  = 1);.MIME-Versi
-000001a0: 6f6e 3a20 312e 300a 436f 6e74 656e 742d  on: 1.0.Content-
-000001b0: 5479 7065 3a20 7465 7874 2f70 6c61 696e  Type: text/plain
-000001c0: 3b20 6368 6172 7365 743d 7574 662d 380a  ; charset=utf-8.
-000001d0: 436f 6e74 656e 742d 5472 616e 7366 6572  Content-Transfer
-000001e0: 2d45 6e63 6f64 696e 673a 2038 6269 740a  -Encoding: 8bit.
-000001f0: 4765 6e65 7261 7465 642d 4279 3a20 4261  Generated-By: Ba
-00000200: 6265 6c20 322e 3132 2e31 0a00            bel 2.12.1..
+00000110: 2065 745f 4545 0a4c 616e 6775 6167 652d   et_EE.Language-
+00000120: 5465 616d 3a20 4573 746f 6e69 616e 2028  Team: Estonian (
+00000130: 4573 746f 6e69 6129 2028 6874 7470 733a  Estonia) (https:
+00000140: 2f2f 6170 702e 7472 616e 7369 6665 782e  //app.transifex.
+00000150: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
+00000160: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
+00000170: 6574 5f45 452f 290a 506c 7572 616c 2d46  et_EE/).Plural-F
+00000180: 6f72 6d73 3a20 6e70 6c75 7261 6c73 3d32  orms: nplurals=2
+00000190: 3b20 706c 7572 616c 3d28 6e20 213d 2031  ; plural=(n != 1
+000001a0: 293b 0a4d 494d 452d 5665 7273 696f 6e3a  );.MIME-Version:
+000001b0: 2031 2e30 0a43 6f6e 7465 6e74 2d54 7970   1.0.Content-Typ
+000001c0: 653a 2074 6578 742f 706c 6169 6e3b 2063  e: text/plain; c
+000001d0: 6861 7273 6574 3d75 7466 2d38 0a43 6f6e  harset=utf-8.Con
+000001e0: 7465 6e74 2d54 7261 6e73 6665 722d 456e  tent-Transfer-En
+000001f0: 636f 6469 6e67 3a20 3862 6974 0a47 656e  coding: 8bit.Gen
+00000200: 6572 6174 6564 2d42 793a 2042 6162 656c  erated-By: Babel
+00000210: 2032 2e31 322e 310a 00                    2.12.1..
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/rw/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/ne/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
-"Language-Team: Kinyarwanda (https://www.transifex.com/inveniosoftware/teams/23537/rw/)\n"
+"Language-Team: Nepali (https://app.transifex.com/inveniosoftware/teams/23537/ne/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: rw\n"
+"Language: ne\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_oauth2server/admin.py:68
 msgid "OAuth Applications"
 msgstr ""
 
 #: invenio_oauth2server/admin.py:69 invenio_oauth2server/admin.py:78
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sk/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
-"Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/sk/)\n"
+"Language-Team: Slovak (https://app.transifex.com/inveniosoftware/teams/23537/sk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: sk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
+"Last-Translator: Rim Sharif, 2023\n"
 "Language: sv\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/"
 "teams/23537/sv/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
@@ -33,51 +33,51 @@
 "Application '%(client_name)s' by '%(client_user)s' wants permission to "
 "access your '%(current_user)s' account."
 msgstr ""
 "Applikationen '%(client_name)s' av '%(client_user)s' vill ha åtkomst till "
 "ditt '%(current_user)s' konto."
 
 msgid "Application / %(client_name)s"
-msgstr "Ansökan / %(client_name)s"
+msgstr "Applikation/ %(client_name)s"
 
 msgid "Applications"
 msgstr "Applikationer"
 
 msgid "Authorize URL (GET)"
 msgstr "Auktorisera URL(GET)"
 
 msgid "Authorize application"
 msgstr "Auktoriserad applikation"
 
 msgid "Authorized application: %(client_name)s"
-msgstr "Authorized application: %(client_name)s"
+msgstr "Auktoriserad applikation: %(client_name)s"
 
 msgid "Authorized applications"
-msgstr "Tillåtna applikationer"
+msgstr "Auktoriserade applikationer"
 
 msgid "Cancel"
 msgstr "Avbryt"
 
 msgid "Client ID"
 msgstr "Klient ID"
 
 msgid "Client Secret"
-msgstr "Klienthemlighet"
+msgstr "Klientnyckel"
 
 msgid "Client type"
 msgstr "Klienttyp"
 
 msgid "Confidential"
 msgstr "Konfidentiell"
 
 msgid "Create"
 msgstr "Skapa"
 
 msgid "Delete"
-msgstr "Ta bort"
+msgstr "Radera"
 
 msgid "Description"
 msgstr "Beskrivning"
 
 msgid "Developer Applications"
 msgstr "Utvecklarapplikationer"
 
@@ -92,32 +92,32 @@
 "konto."
 
 msgid "Edit"
 msgstr "Redigera"
 
 msgid "Following are personal tokens used to access the %(site_name)s API:"
 msgstr ""
-"Följande är personliga symboler som används för att komma åt %(site_name)s "
-"API:et:"
+"Följande är personliga tokens som används för att komma åt %(site_name)s API:"
+"et:"
 
 msgid "Get me out of here!"
 msgstr "Få mig härifrån!"
 
 msgid ""
 "If you've lost or forgotten this token please create a new one. Be aware "
 "that any scripts or applications using this token will need to be updated."
 msgstr ""
 "Om du har tappat bort eller glömt denna token, skapa en ny. Tänk på att alla "
 "skript eller applikationer som använder denna token måste uppdateras."
 
 msgid "Invalid authorization request"
-msgstr "Felaktig Behörighetsbegäran"
+msgstr "Felaktig auktoriseringsförfrågan"
 
 msgid "Invalid redirect URIs: %(urls)s"
-msgstr "Ogiltiga omdirigerings-URI:er:%(urls)s"
+msgstr "Ogiltiga omdirigerings-URI:%(urls)s"
 
 msgid "Name"
 msgstr "Namn"
 
 msgid "Name of application (displayed to users)."
 msgstr "Namn på applikation (visas för användare)."
 
@@ -127,45 +127,45 @@
 msgid "New"
 msgstr "Ny"
 
 msgid "New OAuth Application"
 msgstr "Ny OAuth-applikation"
 
 msgid "New application"
-msgstr "Ny ansökan"
+msgstr "Ny applikation"
 
 msgid "New personal access token"
 msgstr "Ny personlig åtkomsttoken"
 
 msgid "New token"
 msgstr "Ny token"
 
 msgid "No permissions granted."
 msgstr "Inga behörigheter har beviljats."
 
 msgid "OAuth 2.0 Endpoints"
-msgstr "OAUTH 2.0 Endpoints"
+msgstr "OAUTH 2.0 Ändpunkter"
 
 msgid "OAuth Application Tokens"
 msgstr "OAuth Application Tokens"
 
 msgid "OAuth Applications"
 msgstr "OAuth-applikationer"
 
 msgid ""
 "One redirect URI per line. This is your application's authorization callback "
 "URLs. HTTPS must be used for all hosts except localhost (for testing "
 "purposes)."
 msgstr ""
-"En omdirigering URI per rad. Det här är din applikations auktoriserings -"
-"återuppringnings -URL: er. HTTPS måste användas för alla värdar utom "
-"localhost (för teständamål)."
+"En URI omdirigering per rad. Det här är din applikations auktoriserings "
+"callback-URL: er. HTTPS måste användas för alla värdar utom lokal värd (för "
+"teständamål)."
 
 msgid "Optional. Description of the application (displayed to users)."
-msgstr "Frivillig. Beskrivning av applikationen (visas för användare)."
+msgstr "Valfri. Beskrivning av applikationen (visas för användare)."
 
 msgid "Personal access token / %(name)s"
 msgstr "Personlig åtkomsttoken / %(name)s"
 
 msgid "Personal access tokens"
 msgstr "Personlig åtkomsttokens"
 
@@ -177,27 +177,27 @@
 msgid "Public"
 msgstr "Offentlig"
 
 msgid "Query parameters"
 msgstr "Query parametrar"
 
 msgid "Redirect URIs (one per line)"
-msgstr "Omdirigera URIS (en per rad)"
+msgstr "Omdirigera URI (en per rad)"
 
 msgid "Register"
 msgstr "Registrera"
 
 msgid "Reject"
 msgstr "Avvisa"
 
 msgid "Request body parameters:"
-msgstr "Begär kroppsparametrar:"
+msgstr "Begär body-parametrar:"
 
 msgid "Reset client secret"
-msgstr "Återställ klienthemlighet"
+msgstr "Återställ klientnyckel"
 
 msgid "Review permissions"
 msgstr "Granska behörigheter"
 
 msgid "Revoke"
 msgstr "Återkalla"
 
@@ -206,52 +206,52 @@
 
 msgid ""
 "Scopes assign permissions to your personal access token. A personal access "
 "token works just like a normal OAuth  access token for authentication "
 "against the API."
 msgstr ""
 "SCOPES Tilldelar behörigheter till ditt personliga åtkomsttoken. En "
-"personlig åtkomsttoken fungerar precis som ett normalt OAUT -åtkomsttoken "
+"personlig åtkomsttoken fungerar precis som ett normalt OAuth -åtkomsttoken "
 "för autentisering mot API."
 
 msgid ""
 "Select confidential if your application is capable of keeping the issued "
 "client secret confidential (e.g. a web application), select public if your "
 "application cannot (e.g. a browser-based JavaScript application). If you "
 "select public, your application MUST validate the redirect URI."
 msgstr ""
-"Välj konfidentiell Om din ansökan kan hålla den utfärdade klienten hemlig "
-"konfidentiell (t.ex. en webbapplikation), välj Public om din applikation "
+"Välj konfidentiell om din ansökan kan hålla den utfärdade klientnyckeln "
+"konfidentiell (t.ex. en webbapplikation), välj offentlig om din applikation "
 "inte kan (t.ex. en webbläsarbaserad JavaScript-applikation). Om du väljer "
-"allmänheten MÅSTE din ansökan validera omdirigering av URI."
+"offentlig MÅSTE din ansökan validera omdirigering av URI."
 
 msgid "The name must be less than 40 characters long."
 msgstr "Namnet måste vara mindre än 40 tecken långt."
 
 msgid ""
 "The service that redirected your here made an invalid authorization request "
 "(error code: %(x_error)s)."
 msgstr ""
-"Tjänsten som omdirigerade din här gjorde en felaktig behörighetsbegäran "
+"Tjänsten som omdirigerade dig här gjorde en felaktig behörighetsförfrågan "
 "(felkod: %(x_error)s)."
 
 msgid "URL of your application (displayed to users)."
 msgstr "URL till din applikation (visas för användare)."
 
 msgid "User Management"
-msgstr "Användarhantering"
+msgstr "Hantera Användare"
 
 msgid "Visit application website"
 msgstr "Besök applikation hemsida"
 
 msgid "Website URL"
-msgstr "Webbadress"
+msgstr "Webbsida URL"
 
 msgid "You have granted the following application access to your account:"
-msgstr "Du har beviljat följande applikation till ditt konto:"
+msgstr "Du har beviljat följande applikation åtkomst till ditt konto:"
 
 msgid ""
 "You have not yet created any personal access tokens. Click the 'New token' "
 "button to create a personal access token."
 msgstr ""
 "Du har ännu inte skapat några personliga åtkomsttokens. Klicka på knappen "
 "\"Ny token\" för att skapa en personlig åtkomsttoken."
@@ -262,38 +262,38 @@
 "Du har ännu inte beviljat några externa applikationer åtkomst till ditt "
 "konto."
 
 msgid ""
 "You have not yet registered any applications. Click the 'New application' "
 "button to create an application to access the %(site_name)s API."
 msgstr ""
-"Du har ännu inte registrerat några ansökningar. Klicka på knappen \"Ny "
+"Du har ännu inte registrerat några applikationer. Klicka på knappen \"Ny "
 "applikation\" för att skapa en applikation för att komma åt %(site_name)s "
 "API."
 
 msgid "You have registered these applications to use the %(site_name)s API:"
 msgstr ""
 "Du har registrerat dessa applikationer för att använda %(site_name)sAPI:"
 
 msgid "example request"
-msgstr "exempel begäran"
+msgstr "exempel förfrågan"
 
 msgid "or"
 msgstr "eller"
 
 msgid "recommended, for CSRF protection"
-msgstr "recommended, for CSRF protection"
+msgstr "rekommenderas, for CSRF skydd"
 
 msgid "required"
 msgstr "nödvändig"
 
 msgid "required for grant_type"
-msgstr "krävs för grant_type"
+msgstr "obligatorisk för grant_type"
 
 msgid "required, URL encoded"
-msgstr "krävs, URL-kodad"
+msgstr "obligatorisk, URL-kodad"
 
 msgid "required, space separate list of scopes"
-msgstr "krävs, utrymme separat lista över omfattningar"
+msgstr "obligatorisk, separera lista över omfattningar med mellanslag"
 
 msgid "required, use"
 msgstr "krävs, använd"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/sv/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,77 +3,79 @@
 # This file is distributed under the same license as the
 # invenio-oauth2server project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2021
 # Sam Arbid, 2022
+# yyones, 2023
+# Rim Sharif, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/teams/23537/sv/)\n"
+"Last-Translator: Rim Sharif, 2023\n"
+"Language-Team: Swedish (https://app.transifex.com/inveniosoftware/teams/23537/sv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: sv\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_oauth2server/admin.py:68
 msgid "OAuth Applications"
 msgstr "OAuth-applikationer"
 
 #: invenio_oauth2server/admin.py:69 invenio_oauth2server/admin.py:78
 msgid "User Management"
-msgstr "Användarhantering"
+msgstr "Hantera Användare"
 
 #: invenio_oauth2server/admin.py:77
 msgid "OAuth Application Tokens"
 msgstr "OAuth Application Tokens"
 
 #: invenio_oauth2server/forms.py:103
 #, python-format
 msgid "Invalid redirect URIs: %(urls)s"
-msgstr "Ogiltiga omdirigerings-URI:er:%(urls)s"
+msgstr "Ogiltiga omdirigerings-URI:%(urls)s"
 
 #: invenio_oauth2server/forms.py:135
 msgid "Redirect URIs (one per line)"
-msgstr "Omdirigera URIS (en per rad)"
+msgstr "Omdirigera URI (en per rad)"
 
 #: invenio_oauth2server/forms.py:136
 msgid ""
 "One redirect URI per line. This is your application's authorization callback"
 " URLs. HTTPS must be used for all hosts except localhost (for testing "
 "purposes)."
 msgstr ""
-"En omdirigering URI per rad. Det här är din applikations auktoriserings "
-"-återuppringnings -URL: er. HTTPS måste användas för alla värdar utom "
-"localhost (för teständamål)."
+"En URI omdirigering per rad. Det här är din applikations auktoriserings "
+"callback-URL: er. HTTPS måste användas för alla värdar utom lokal värd (för "
+"teständamål)."
 
 #: invenio_oauth2server/forms.py:155
 msgid "Client type"
 msgstr "Klienttyp"
 
 #: invenio_oauth2server/forms.py:156
 msgid ""
 "Select confidential if your application is capable of keeping the issued "
 "client secret confidential (e.g. a web application), select public if your "
 "application cannot (e.g. a browser-based JavaScript application). If you "
 "select public, your application MUST validate the redirect URI."
 msgstr ""
-"Välj konfidentiell Om din ansökan kan hålla den utfärdade klienten hemlig "
-"konfidentiell (t.ex. en webbapplikation), välj Public om din applikation "
+"Välj konfidentiell om din ansökan kan hålla den utfärdade klientnyckeln "
+"konfidentiell (t.ex. en webbapplikation), välj offentlig om din applikation "
 "inte kan (t.ex. en webbläsarbaserad JavaScript-applikation). Om du väljer "
-"allmänheten MÅSTE din ansökan validera omdirigering av URI."
+"offentlig MÅSTE din ansökan validera omdirigering av URI."
 
 #: invenio_oauth2server/forms.py:164
 msgid "Confidential"
 msgstr "Konfidentiell"
 
 #: invenio_oauth2server/forms.py:164
 msgid "Public"
@@ -90,15 +92,15 @@
 #: invenio_oauth2server/forms.py:186
 msgid ""
 "Scopes assign permissions to your personal access token. A personal access "
 "token works just like a normal OAuth  access token for authentication "
 "against the API."
 msgstr ""
 "SCOPES Tilldelar behörigheter till ditt personliga åtkomsttoken. En "
-"personlig åtkomsttoken fungerar precis som ett normalt OAUT -åtkomsttoken "
+"personlig åtkomsttoken fungerar precis som ett normalt OAuth -åtkomsttoken "
 "för autentisering mot API."
 
 #: invenio_oauth2server/models.py:122
 msgid "Name"
 msgstr "Namn"
 
 #: invenio_oauth2server/models.py:123
@@ -107,19 +109,19 @@
 
 #: invenio_oauth2server/models.py:133
 msgid "Description"
 msgstr "Beskrivning"
 
 #: invenio_oauth2server/models.py:134
 msgid "Optional. Description of the application (displayed to users)."
-msgstr "Frivillig. Beskrivning av applikationen (visas för användare)."
+msgstr "Valfri. Beskrivning av applikationen (visas för användare)."
 
 #: invenio_oauth2server/models.py:144
 msgid "Website URL"
-msgstr "Webbadress"
+msgstr "Webbsida URL"
 
 #: invenio_oauth2server/models.py:145
 msgid "URL of your application (displayed to users)."
 msgstr "URL till din applikation (visas för användare)."
 
 #: invenio_oauth2server/scopes.py:20
 msgid "Allow access to email address (read-only)."
@@ -179,24 +181,24 @@
 msgstr "Avvisa"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/errors.html:18
 #: invenio_oauth2server/templates/invenio_oauth2server/errors.html:22
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html:17
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html:20
 msgid "Invalid authorization request"
-msgstr "Felaktig Behörighetsbegäran"
+msgstr "Felaktig auktoriseringsförfrågan"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/errors.html:24
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html:22
 #, python-format
 msgid ""
 "The service that redirected your here made an invalid authorization request "
 "(error code: %(x_error)s)."
 msgstr ""
-"Tjänsten som omdirigerade din här gjorde en felaktig behörighetsbegäran "
+"Tjänsten som omdirigerade dig här gjorde en felaktig behörighetsförfrågan "
 "(felkod: %(x_error)s)."
 
 #: invenio_oauth2server/templates/invenio_oauth2server/errors.html:31
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/errors.html:28
 msgid "Get me out of here!"
 msgstr "Få mig härifrån!"
 
@@ -217,69 +219,69 @@
 msgid "Register"
 msgstr "Registrera"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:17
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:18
 #, python-format
 msgid "Application / %(client_name)s"
-msgstr "Ansökan / %(client_name)s"
+msgstr "Applikation/ %(client_name)s"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:22
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:30
 msgid "Client ID"
 msgstr "Klient ID"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:23
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:36
 msgid "Client Secret"
-msgstr "Klienthemlighet"
+msgstr "Klientnyckel"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:24
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:39
 msgid "Do not share the client secret with anyone!"
 msgstr "Dela inte klientens hemlighet med någon!"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:30
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:26
 msgid "Reset client secret"
-msgstr "Återställ klienthemlighet"
+msgstr "Återställ klientnyckel"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:47
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html:48
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:51
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html:49
 msgid "Delete"
-msgstr "Ta bort"
+msgstr "Radera"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:48
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html:49
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:54
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html:52
 msgid "Save"
 msgstr "Spara"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:55
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:60
 msgid "OAuth 2.0 Endpoints"
-msgstr "OAUTH 2.0 Endpoints"
+msgstr "OAUTH 2.0 Ändpunkter"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:59
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:65
 msgid "Authorize URL (GET)"
 msgstr "Auktorisera URL(GET)"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:62
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:71
 msgid "Query parameters"
 msgstr "Query parametrar"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:69
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:78
 msgid "example request"
-msgstr "exempel begäran"
+msgstr "exempel förfrågan"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:72
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:89
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:81
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:102
 msgid "required, use"
 msgstr "krävs, använd"
@@ -292,54 +294,54 @@
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:101
 msgid "required"
 msgstr "nödvändig"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:74
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:83
 msgid "required, space separate list of scopes"
-msgstr "krävs, utrymme separat lista över omfattningar"
+msgstr "obligatorisk, separera lista över omfattningar med mellanslag"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:75
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:84
 msgid "required, URL encoded"
-msgstr "krävs, URL-kodad"
+msgstr "obligatorisk, URL-kodad"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:76
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:85
 msgid "recommended, for CSRF protection"
-msgstr "recommended, for CSRF protection"
+msgstr "rekommenderas, for CSRF skydd"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:83
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:93
 msgid "Access token URL (POST)"
 msgstr "URL för åtkomsttoken (POST)"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:85
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:98
 msgid "Request body parameters:"
-msgstr "Begär kroppsparametrar:"
+msgstr "Begär body-parametrar:"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:90
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:91
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:92
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:103
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:104
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:105
 msgid "required for grant_type"
-msgstr "krävs för grant_type"
+msgstr "obligatorisk för grant_type"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/index.html:17
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html:17
 msgid "Developer Applications"
 msgstr "Utvecklarapplikationer"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/index.html:18
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html:18
 msgid "New application"
-msgstr "Ny ansökan"
+msgstr "Ny applikation"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/index.html:25
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html:25
 #, python-format
 msgid "You have registered these applications to use the %(site_name)s API:"
 msgstr ""
 "Du har registrerat dessa applikationer för att använda %(site_name)sAPI:"
@@ -347,15 +349,15 @@
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/index.html:36
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html:37
 #, python-format
 msgid ""
 "You have not yet registered any applications. Click the 'New application' "
 "button to create an application to access the %(site_name)s API."
 msgstr ""
-"Du har ännu inte registrerat några ansökningar. Klicka på knappen \"Ny "
+"Du har ännu inte registrerat några applikationer. Klicka på knappen \"Ny "
 "applikation\" för att skapa en applikation för att komma åt %(site_name)s "
 "API."
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/index.html:41
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html:43
 msgid "Personal access tokens"
 msgstr "Personlig åtkomsttokens"
@@ -366,35 +368,35 @@
 msgstr "Ny token"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/index.html:49
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html:51
 #, python-format
 msgid "Following are personal tokens used to access the %(site_name)s API:"
 msgstr ""
-"Följande är personliga symboler som används för att komma åt %(site_name)s "
+"Följande är personliga tokens som används för att komma åt %(site_name)s "
 "API:et:"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/index.html:60
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html:69
 msgid ""
 "You have not yet created any personal access tokens. Click the 'New token' "
 "button to create a personal access token."
 msgstr ""
 "Du har ännu inte skapat några personliga åtkomsttokens. Klicka på knappen "
 "\"Ny token\" för att skapa en personlig åtkomsttoken."
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/index.html:65
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html:74
 msgid "Authorized applications"
-msgstr "Tillåtna applikationer"
+msgstr "Auktoriserade applikationer"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/index.html:70
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html:79
 msgid "You have granted the following application access to your account:"
-msgstr "Du har beviljat följande applikation till ditt konto:"
+msgstr "Du har beviljat följande applikation åtkomst till ditt konto:"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/index.html:76
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/index.html:84
 msgid "Revoke"
 msgstr "Återkalla"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/index.html:84
@@ -415,15 +417,15 @@
 msgid "Create"
 msgstr "Skapa"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_permission_view.html:17
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_permission_view.html:17
 #, python-format
 msgid "Authorized application: %(client_name)s"
-msgstr "Authorized application: %(client_name)s"
+msgstr "Auktoriserad applikation: %(client_name)s"
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html:17
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html:17
 #, python-format
 msgid "Personal access token / %(name)s"
 msgstr "Personlig åtkomsttoken / %(name)s"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -3,15 +3,15 @@
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume."
 "com>, 2021\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/tr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
 "Last-Translator: Ben Translation and Interpreting Services <info@bentercume.com>, 2021\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/teams/23537/tr/)\n"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/teams/23537/tr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/uk/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-oauth2server 1.3.7*

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 ba02 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 ca02 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d6f 6175 7468 3273   invenio-oauth2s
 00000050: 6572 7665 7220 312e 332e 370a 5265 706f  erver 1.3.7.Repo
 00000060: 7274 2d4d 7367 6964 2d42 7567 732d 546f  rt-Msgid-Bugs-To
 00000070: 3a20 696e 666f 4069 6e76 656e 696f 736f  : info@invenioso
 00000080: 6674 7761 7265 2e6f 7267 0a50 4f54 2d43  ftware.org.POT-C
 00000090: 7265 6174 696f 6e2d 4461 7465 3a20 3230  reation-Date: 20
 000000a0: 3232 2d31 302d 3132 2030 393a 3236 2b30  22-10-12 09:26+0
 000000b0: 3030 300a 504f 2d52 6576 6973 696f 6e2d  000.PO-Revision-
 000000c0: 4461 7465 3a20 3230 3136 2d30 382d 3138  Date: 2016-08-18
 000000d0: 2030 383a 3033 2b30 3030 300a 4c61 7374   08:03+0000.Last
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/uk/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
-"Language-Team: Ukrainian (https://www.transifex.com/inveniosoftware/teams/23537/uk/)\n"
+"Language-Team: Ukrainian (Ukraine) (https://app.transifex.com/inveniosoftware/teams/23537/uk_UA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: uk\n"
+"Language: uk_UA\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #: invenio_oauth2server/admin.py:68
 msgid "OAuth Applications"
 msgstr ""
 
 #: invenio_oauth2server/admin.py:69 invenio_oauth2server/admin.py:78
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
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

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,36 +0,0 @@
-msgid ""
-msgstr ""
-"Project-Id-Version: invenio-oauth2server 1.3.7\n"
-"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2022-10-12 09:26+0000\n"
-"PO-Revision-Date: 2016-08-18 08:03+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
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
-msgid "Delete"
-msgstr "刪除"
-
-msgid "Description"
-msgstr "描述"
-
-msgid "Edit"
-msgstr "編輯"
-
-msgid "Name"
-msgstr "名稱"
-
-msgid "Register"
-msgstr "註冊"
-
-msgid "or"
-msgstr "或"
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-oauth2server-2.1.0/invenio_oauth2server/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # Translations template for invenio-oauth2server.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the
 # invenio-oauth2server project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
-# Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2021
-# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-oauth2server 1.3.7\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:26+0000\n"
 "PO-Revision-Date: 2016-08-18 08:03+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2021\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
+"Language-Team: German (Austria) (https://app.transifex.com/inveniosoftware/teams/23537/de_AT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: zh_TW\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: de_AT\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_oauth2server/admin.py:68
 msgid "OAuth Applications"
 msgstr ""
 
 #: invenio_oauth2server/admin.py:69 invenio_oauth2server/admin.py:78
 msgid "User Management"
@@ -84,23 +80,23 @@
 "Scopes assign permissions to your personal access token. A personal access "
 "token works just like a normal OAuth  access token for authentication "
 "against the API."
 msgstr ""
 
 #: invenio_oauth2server/models.py:122
 msgid "Name"
-msgstr "名稱"
+msgstr ""
 
 #: invenio_oauth2server/models.py:123
 msgid "Name of application (displayed to users)."
 msgstr ""
 
 #: invenio_oauth2server/models.py:133
 msgid "Description"
-msgstr "描述"
+msgstr ""
 
 #: invenio_oauth2server/models.py:134
 msgid "Optional. Description of the application (displayed to users)."
 msgstr ""
 
 #: invenio_oauth2server/models.py:144
 msgid "Website URL"
@@ -191,20 +187,20 @@
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html:25
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_new.html:26
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html:24
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_new.html:25
 msgid "Cancel"
-msgstr "取消"
+msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_new.html:26
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_new.html:27
 msgid "Register"
-msgstr "註冊"
+msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:17
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:18
 #, python-format
 msgid "Application / %(client_name)s"
 msgstr ""
 
@@ -229,15 +225,15 @@
 msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:47
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html:48
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:51
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html:49
 msgid "Delete"
-msgstr "刪除"
+msgstr ""
 
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/client_view.html:48
 #: invenio_oauth2server/templates/invenio_oauth2server/settings/token_view.html:49
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:54
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/token_view.html:52
 msgid "Save"
 msgstr ""
@@ -424,15 +420,15 @@
 msgid ""
 "If you've lost or forgotten this token please create a new one. Be aware "
 "that any scripts or applications using this token will need to be updated."
 msgstr ""
 
 #: invenio_oauth2server/templates/semantic-ui/invenio_oauth2server/settings/client_view.html:81
 msgid "or"
-msgstr "或"
+msgstr ""
 
 #: invenio_oauth2server/views/settings.py:105
 #, python-format
 msgid "%(icon)s Applications"
 msgstr ""
 
 #: invenio_oauth2server/views/settings.py:110
@@ -443,8 +439,8 @@
 #: invenio_oauth2server/views/settings.py:212
 msgid "New"
 msgstr ""
 
 #: invenio_oauth2server/views/settings.py:174
 #: invenio_oauth2server/views/settings.py:238
 msgid "Edit"
-msgstr "編輯"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/utils.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/validators.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/validators.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/views/server.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/views/server.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server/views/settings.py` & `invenio-oauth2server-2.1.0/invenio_oauth2server/views/settings.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server.egg-info/PKG-INFO` & `invenio-oauth2server-2.1.0/invenio_oauth2server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-oauth2server
-Version: 2.0.0
+Version: 2.1.0
 Summary: "Invenio module that implements OAuth 2 server."
 Home-page: https://github.com/inveniosoftware/invenio-oauth2server
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -50,14 +50,19 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.1.0 (released 2023-07-31)
+        
+        - applications: Improve templates for UI and accessibility
+        - pulled translations
+        
         Version 2.0.0 (released 2023-03-02)
         
         - drop python2.7 support
         - remove deprecated flask-babelex dependency and imports
         - upgrade invenio-i18n
         - upgrade invenio-admin
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server.egg-info/SOURCES.txt` & `invenio-oauth2server-2.1.0/invenio_oauth2server.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -105,40 +105,64 @@
 invenio_oauth2server/translations/ca/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/cs/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/cs/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/da/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/da/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/de/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/de/LC_MESSAGES/messages.po
+invenio_oauth2server/translations/de_AT/LC_MESSAGES/messages.mo
+invenio_oauth2server/translations/de_AT/LC_MESSAGES/messages.po
+invenio_oauth2server/translations/de_DE/LC_MESSAGES/messages.mo
+invenio_oauth2server/translations/de_DE/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/el/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/el/LC_MESSAGES/messages.po
+invenio_oauth2server/translations/en_AT/LC_MESSAGES/messages.mo
+invenio_oauth2server/translations/en_AT/LC_MESSAGES/messages.po
+invenio_oauth2server/translations/en_HU/LC_MESSAGES/messages.mo
+invenio_oauth2server/translations/en_HU/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/es/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/es/LC_MESSAGES/messages.po
+invenio_oauth2server/translations/es_CU/LC_MESSAGES/messages.mo
+invenio_oauth2server/translations/es_CU/LC_MESSAGES/messages.po
+invenio_oauth2server/translations/es_MX/LC_MESSAGES/messages.mo
+invenio_oauth2server/translations/es_MX/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/et/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/et/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/et_EE/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/fa/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/fa/LC_MESSAGES/messages.po
+invenio_oauth2server/translations/fa_IR/LC_MESSAGES/messages.mo
+invenio_oauth2server/translations/fa_IR/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/fr/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/fr/LC_MESSAGES/messages.po
+invenio_oauth2server/translations/fr_CI/LC_MESSAGES/messages.mo
+invenio_oauth2server/translations/fr_CI/LC_MESSAGES/messages.po
+invenio_oauth2server/translations/fr_FR/LC_MESSAGES/messages.mo
+invenio_oauth2server/translations/fr_FR/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/gl/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/gl/LC_MESSAGES/messages.po
+invenio_oauth2server/translations/hi_IN/LC_MESSAGES/messages.mo
+invenio_oauth2server/translations/hi_IN/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/hr/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/hr/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/hu/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/hu/LC_MESSAGES/messages.po
+invenio_oauth2server/translations/hu_HU/LC_MESSAGES/messages.mo
+invenio_oauth2server/translations/hu_HU/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/it/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/it/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/ja/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/ja/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/ka/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/ka/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/lt/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/lt/LC_MESSAGES/messages.po
+invenio_oauth2server/translations/ne/LC_MESSAGES/messages.mo
+invenio_oauth2server/translations/ne/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/no/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/no/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/pl/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/pl/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/pt/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/pt/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/ro/LC_MESSAGES/messages.mo
@@ -147,18 +171,22 @@
 invenio_oauth2server/translations/ru/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/rw/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/rw/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/sk/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/sk/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/sv/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/sv/LC_MESSAGES/messages.po
+invenio_oauth2server/translations/sv_SE/LC_MESSAGES/messages.mo
+invenio_oauth2server/translations/sv_SE/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/tr/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/tr/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/uk/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/uk/LC_MESSAGES/messages.po
+invenio_oauth2server/translations/uk_UA/LC_MESSAGES/messages.mo
+invenio_oauth2server/translations/uk_UA/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/zh_CN/LC_MESSAGES/messages.po
 invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.mo
 invenio_oauth2server/translations/zh_TW/LC_MESSAGES/messages.po
 invenio_oauth2server/views/__init__.py
 invenio_oauth2server/views/server.py
 invenio_oauth2server/views/settings.py
```

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server.egg-info/entry_points.txt` & `invenio-oauth2server-2.1.0/invenio_oauth2server.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/invenio_oauth2server.egg-info/requires.txt` & `invenio-oauth2server-2.1.0/invenio_oauth2server.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/run-tests.sh` & `invenio-oauth2server-2.1.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/setup.cfg` & `invenio-oauth2server-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/tests/conftest.py` & `invenio-oauth2server-2.1.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from flask_mail import Mail
 from flask_menu import Menu
 from helpers import create_oauth_client, patch_request
 from invenio_accounts import InvenioAccountsREST, InvenioAccountsUI
 from invenio_accounts.models import User
 from invenio_accounts.views import blueprint as accounts_blueprint
 from invenio_db import InvenioDB, db
-from invenio_i18n import Babel
+from invenio_i18n import InvenioI18N
 from six import get_method_self
 from sqlalchemy_utils.functions import create_database, database_exists, drop_database
 
 from invenio_oauth2server import InvenioOAuth2Server, InvenioOAuth2ServerREST
 from invenio_oauth2server.decorators import require_api_auth, require_oauth_scopes
 from invenio_oauth2server.models import Client, Scope, Token
 from invenio_oauth2server.views import server_blueprint, settings_blueprint
@@ -82,15 +82,15 @@
                     # Special catch all:
                     "*": "{} icon",
                 }
             },
             ACCOUNTS_COVER_TEMPLATE="invenio_accounts/base_cover.html",
             ACCOUNTS_BASE_TEMPLATE="invenio_accounts/base.html",
         )
-        Babel(app)
+        InvenioI18N(app)
         Mail(app)
         Menu(app)
         Breadcrumbs(app)
         InvenioDB(app)
         InvenioOAuth2Server(app)
 
     api_app = Flask("testapiapp", instance_path=instance_path)
```

### Comparing `invenio-oauth2server-2.0.0/tests/helpers.py` & `invenio-oauth2server-2.1.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/tests/test_admin.py` & `invenio-oauth2server-2.1.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/tests/test_alembic.py` & `invenio-oauth2server-2.1.0/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/tests/test_cli.py` & `invenio-oauth2server-2.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/tests/test_decorators.py` & `invenio-oauth2server-2.1.0/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/tests/test_invenio_oauth2server.py` & `invenio-oauth2server-2.1.0/tests/test_invenio_oauth2server.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/tests/test_models.py` & `invenio-oauth2server-2.1.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/tests/test_provider.py` & `invenio-oauth2server-2.1.0/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/tests/test_server.py` & `invenio-oauth2server-2.1.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/tests/test_settings.py` & `invenio-oauth2server-2.1.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/tests/test_utils.py` & `invenio-oauth2server-2.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-oauth2server-2.0.0/tests/test_validators.py` & `invenio-oauth2server-2.1.0/tests/test_validators.py`

 * *Files identical despite different names*

