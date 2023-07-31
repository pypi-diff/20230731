# Comparing `tmp/invenio-accounts-3.0.3.tar.gz` & `tmp/invenio-accounts-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-accounts-3.0.3.tar", last modified: Thu Jun 15 12:34:10 2023, max compression
+gzip compressed data, was "dist/invenio-accounts-3.1.0.tar", last modified: Mon Jul 31 08:14:30 2023, max compression
```

## Comparing `invenio-accounts-3.0.3.tar` & `invenio-accounts-3.1.0.tar`

### file list

```diff
@@ -1,274 +1,330 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1912 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2006 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6023 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      878 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10506 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7449 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)    55769 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/docs/admin.png
--rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10254 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     5874 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      829 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7001 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7385 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/alembic/
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/alembic/62efc52773d4_create_useridentity_table.py
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/alembic/843bc79c426f_create_accounts_branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     3842 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/alembic/9848d0149abd_create_accounts_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     2247 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/alembic/999dcbd19ace_users_versioning.py
--rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/alembic/dfbdf43a3e96_separate_login_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/alembic/e12419831262_add_new_columns_on_sessionactivity.py
--rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/alembic/eb9743315a9d_add_userprofile.py
--rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/alembic/f2522cdd5fcd_change_accountsrole_primary_key_to_string.py
--rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4525 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    10959 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/context_processors/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/context_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/context_processors/jwt.py
--rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/datastore.py
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    11798 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/forms.py
--rw-r--r--   0 runner    (1001) docker     (122)     4071 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/hash.py
--rw-r--r--   0 runner    (1001) docker     (122)    13869 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/profiles/
--rw-r--r--   0 runner    (1001) docker     (122)      570 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3359 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/profiles/dicts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/profiles/schemas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     5526 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/sessions.py
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/base_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/change_password.html
--rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/forgot_password.html
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/jwt.html
--rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/login_user.html
--rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/register_user.html
--rw-r--r--   0 runner    (1001) docker     (122)     1818 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/send_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/send_login.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/settings/security.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/templates/security/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/templates/security/email/
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/security/email/change_notice_rest.html
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/security/email/change_notice_rest.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/
--rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/base_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html
--rw-r--r--   0 runner    (1001) docker     (122)     1726 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/jwt.html
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/send_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/send_login.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html
--rw-r--r--   0 runner    (1001) docker     (122)     4809 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9446 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4843 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11937 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      727 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9640 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10653 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3467 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10896 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      936 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9800 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4106 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11345 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11153 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4031 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11067 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3995 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11017 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      533 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9461 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      718 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9631 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10991 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9445 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      769 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4127 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11093 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10687 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      715 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9628 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      874 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9761 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     9380 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9606 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9751 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      673 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9653 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      704 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9641 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      974 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9861 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9448 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3202 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10747 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3944 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10951 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11117 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9668 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10604 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      692 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9605 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     7420 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts/views/
--rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19229 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/views/rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/views/security.py
--rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/invenio_accounts/views/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10506 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/invenio_accounts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)     1546 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     8833 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 12:34:10.000000 invenio-accounts-3.0.3/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (122)     3598 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/e2e/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3709 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/e2e/e2e_basic_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5430 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (122)     7501 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/test_invenio_accounts.py
--rw-r--r--   0 runner    (1001) docker     (122)     4766 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (122)    11240 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/test_template_context_processors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/test_token_duration.py
--rw-r--r--   0 runner    (1001) docker     (122)     6706 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3239 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/test_validated_dicts.py
--rw-r--r--   0 runner    (1001) docker     (122)     6325 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    18215 2023-06-15 12:33:57.000000 invenio-accounts-3.0.3/tests/test_views_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1142 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6129 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10652 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7449 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)    55769 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/docs/admin.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10254 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5874 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7001 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7385 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/alembic/62efc52773d4_create_useridentity_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/alembic/843bc79c426f_create_accounts_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3842 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/alembic/9848d0149abd_create_accounts_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2247 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/alembic/999dcbd19ace_users_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/alembic/dfbdf43a3e96_separate_login_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/alembic/e12419831262_add_new_columns_on_sessionactivity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/alembic/eb9743315a9d_add_userprofile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/alembic/f2522cdd5fcd_change_accountsrole_primary_key_to_string.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4525 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10959 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/context_processors/
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/context_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/context_processors/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11798 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/forms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4071 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/hash.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13869 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/profiles/
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3359 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/profiles/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/profiles/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5526 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/base_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/forgot_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/jwt.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/register_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1818 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/send_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/send_login.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/settings/security.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/templates/security/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/templates/security/email/
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/security/email/change_notice_rest.html
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/security/email/change_notice_rest.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/base_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1437 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/jwt.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2274 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/send_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/send_login.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2950 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4809 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9446 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11939 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9640 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10653 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3467 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10896 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      936 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9800 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4106 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11345 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9459 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9459 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11153 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9460 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9460 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4031 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11067 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9496 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9498 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3995 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11017 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9461 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      718 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9631 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9456 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10991 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9517 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9509 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9445 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9456 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      769 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4127 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11093 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9462 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10687 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      715 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9628 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      874 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9761 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     9380 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9443 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9606 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9751 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      673 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9653 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3971 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10988 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      974 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9861 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9448 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3202 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10747 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3941 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10982 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9459 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11117 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2811 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10944 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9684 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10604 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      692 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9605 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     7420 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts/views/
+-rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19229 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/views/rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/views/security.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/invenio_accounts/views/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10652 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9889 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/invenio_accounts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1556 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     8833 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 08:14:30.000000 invenio-accounts-3.1.0/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (122)     3598 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/e2e/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3709 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/e2e/e2e_basic_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5430 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7501 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/test_invenio_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4766 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11240 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/test_template_context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/test_token_duration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6706 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3239 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/test_validated_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6325 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18215 2023-07-31 08:14:17.000000 invenio-accounts-3.1.0/tests/test_views_rest.py
```

### Comparing `invenio-accounts-3.0.3/.editorconfig` & `invenio-accounts-3.1.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/.github/workflows/pypi-publish.yml` & `invenio-accounts-3.1.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/.github/workflows/tests.yml` & `invenio-accounts-3.1.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/.tx/config` & `invenio-accounts-3.1.0/.tx/config`

 * *Files 8% similar despite different names*

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
 # 1) Create message catalog:
@@ -20,14 +21,14 @@
 #    $ tx push -s -t
 # 5) Pull translations for a single language from Transifex
 #    $ tx pull -l <lang>
 # 6) Pull translations for all languages from Transifex
 #    $ tx pull -a
 
 [main]
-host = https://www.transifex.com
+host = https://app.transifex.com
 
-[invenio.invenio-accounts-messages]
+[o:inveniosoftware:p:invenio:r:invenio-accounts-messages]
 file_filter = invenio_accounts/translations/<lang>/LC_MESSAGES/messages.po
 source_file = invenio_accounts/translations/messages.pot
 source_lang = en
 type = PO
```

### Comparing `invenio-accounts-3.0.3/AUTHORS.rst` & `invenio-accounts-3.1.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/CHANGES.rst` & `invenio-accounts-3.1.0/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 3.1.0 (released 2023-07-31)
+
+- templates: Improve accessibility and layout
+- pulled translations
+
 Version 3.0.3 (released 2023-06-15)
 
 - models: fix autogeneration of role id
 
 Version 3.0.2 (released 2023-06-14)
 
 - alembic: adapt recipe to mysql
```

### Comparing `invenio-accounts-3.0.3/CONTRIBUTING.rst` & `invenio-accounts-3.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/LICENSE` & `invenio-accounts-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/MANIFEST.in` & `invenio-accounts-3.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/PKG-INFO` & `invenio-accounts-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-accounts
-Version: 3.0.3
+Version: 3.1.0
 Summary: Invenio user management and authentication.
 Home-page: https://github.com/inveniosoftware/invenio-accounts
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -62,14 +62,19 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 3.1.0 (released 2023-07-31)
+        
+        - templates: Improve accessibility and layout
+        - pulled translations
+        
         Version 3.0.3 (released 2023-06-15)
         
         - models: fix autogeneration of role id
         
         Version 3.0.2 (released 2023-06-14)
         
         - alembic: adapt recipe to mysql
```

### Comparing `invenio-accounts-3.0.3/README.rst` & `invenio-accounts-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/docs/Makefile` & `invenio-accounts-3.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/docs/admin.png` & `invenio-accounts-3.1.0/docs/admin.png`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/docs/api.rst` & `invenio-accounts-3.1.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/docs/conf.py` & `invenio-accounts-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/docs/configuration.rst` & `invenio-accounts-3.1.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/docs/index.rst` & `invenio-accounts-3.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/docs/make.bat` & `invenio-accounts-3.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/__init__.py` & `invenio-accounts-3.1.0/invenio_accounts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     from werkzeug import security
 
     security.safe_str_cmp = hmac.compare_digest
 
 from .ext import InvenioAccounts, InvenioAccountsREST, InvenioAccountsUI
 from .proxies import current_accounts
 
-__version__ = "3.0.3"
+__version__ = "3.1.0"
 
 __all__ = (
     "__version__",
     "current_accounts",
     "InvenioAccounts",
     "InvenioAccountsUI",
     "InvenioAccountsREST",
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/admin.py` & `invenio-accounts-3.1.0/invenio_accounts/admin.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/alembic/62efc52773d4_create_useridentity_table.py` & `invenio-accounts-3.1.0/invenio_accounts/alembic/62efc52773d4_create_useridentity_table.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/alembic/843bc79c426f_create_accounts_branch.py` & `invenio-accounts-3.1.0/invenio_accounts/alembic/843bc79c426f_create_accounts_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/alembic/9848d0149abd_create_accounts_tables.py` & `invenio-accounts-3.1.0/invenio_accounts/alembic/9848d0149abd_create_accounts_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/alembic/999dcbd19ace_users_versioning.py` & `invenio-accounts-3.1.0/invenio_accounts/alembic/999dcbd19ace_users_versioning.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/alembic/dfbdf43a3e96_separate_login_info.py` & `invenio-accounts-3.1.0/invenio_accounts/alembic/dfbdf43a3e96_separate_login_info.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/alembic/e12419831262_add_new_columns_on_sessionactivity.py` & `invenio-accounts-3.1.0/invenio_accounts/alembic/e12419831262_add_new_columns_on_sessionactivity.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/alembic/eb9743315a9d_add_userprofile.py` & `invenio-accounts-3.1.0/invenio_accounts/alembic/eb9743315a9d_add_userprofile.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/alembic/f2522cdd5fcd_change_accountsrole_primary_key_to_string.py` & `invenio-accounts-3.1.0/invenio_accounts/alembic/f2522cdd5fcd_change_accountsrole_primary_key_to_string.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/api.py` & `invenio-accounts-3.1.0/invenio_accounts/api.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/cli.py` & `invenio-accounts-3.1.0/invenio_accounts/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/config.py` & `invenio-accounts-3.1.0/invenio_accounts/config.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/context_processors/jwt.py` & `invenio-accounts-3.1.0/invenio_accounts/context_processors/jwt.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/datastore.py` & `invenio-accounts-3.1.0/invenio_accounts/datastore.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/errors.py` & `invenio-accounts-3.1.0/invenio_accounts/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/ext.py` & `invenio-accounts-3.1.0/invenio_accounts/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/forms.py` & `invenio-accounts-3.1.0/invenio_accounts/forms.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/hash.py` & `invenio-accounts-3.1.0/invenio_accounts/hash.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/models.py` & `invenio-accounts-3.1.0/invenio_accounts/models.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/profiles/__init__.py` & `invenio-accounts-3.1.0/invenio_accounts/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/profiles/dicts.py` & `invenio-accounts-3.1.0/invenio_accounts/profiles/dicts.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/profiles/schemas.py` & `invenio-accounts-3.1.0/invenio_accounts/profiles/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/proxies.py` & `invenio-accounts-3.1.0/invenio_accounts/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/sessions.py` & `invenio-accounts-3.1.0/invenio_accounts/sessions.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/signals.py` & `invenio-accounts-3.1.0/invenio_accounts/signals.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/tasks.py` & `invenio-accounts-3.1.0/invenio_accounts/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/_macros.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/change_password.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/change_password.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/forgot_password.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/forgot_password.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/login_user.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/register_user.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/register_user.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/reset_password.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/reset_password.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/send_confirmation.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/send_confirmation.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/invenio_accounts/settings/security.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/invenio_accounts/settings/security.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/_macros.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,14 @@
     <label for="new_password">{{_('New password')}}</label>
     {{ render_field(form.new_password, errormsg='new_password' in form.errors) }}
   </div>
   <div class="field">
     <label for="new_password_confirm">{{_('Confirm new password')}}</label>
     {{ render_field(form.new_password_confirm, errormsg='new_password_confirm' in form.errors) }}
   </div>
-  <button type="submit" class="ui submit primary button">
-    <i class="check icon"></i>
-    {{_('Change Password')}}
+  <button type="submit" class="ui submit primary labeled icon button">
+    <i class="check icon" aria-hidden="true"></i>
+    {{_('Change password')}}
   </button>
 </form>
 {%- endwith %}
 {% endblock settings_form %}
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html`

 * *Files 8% similar despite different names*

```diff
@@ -12,38 +12,40 @@
 {%- set messages = get_flashed_messages(with_categories=true) -%}
 
 {% block page_body %}
 <div class="ui padded segments big form">
   <div class="ui segment padded">
 
     {%- block form_header %}
-      <h3 class="ui reset-password header">{{_('Reset Password')}}</h3>
+      <h1 class="ui small reset-password header">{{_('Reset password')}}</h1>
     {%- endblock form_header %}
 
     {%- if messages %}
       {%- for category, message in messages %}
       <p>{{ message }}</p>
       {%- endfor %}
     {%- else %}
-      <p class="">
+      <p>
         {{_('Enter your email address below and we will send you a link to reset your password.')}}
       </p>
       {%- with form = forgot_password_form %}
       <form action="{{ url_for_security('forgot_password') }}" method="POST" name="forgot_password_form">
         {{ form.hidden_tag() }}
         {{ render_field(form.email, icon="user icon", autofocus=True, errormsg='email' in form.errors) }}
-        <button type="submit" class="ui fluid large submit primary button">{{_('Reset Password')}}</button>
+        <button type="submit" class="ui fluid large submit primary button">{{_('Reset password')}}</button>
       </form>
       {%- endwith %}
     {%- endif %}
 
   </div>
 
   {%- if current_user.is_anonymous %}
-    <div class="ui primary segment padded text-muted">
-      <a href="{{url_for('security.login')}}">{{_('Log in')}}</a>{% if security.registerable %}
-        {{_('or')}} <a href="{{url_for('security.register')}}">{{_('Sign up')}}</a>{% endif %}
-    </div>
+    <p class="ui primary segment padded text-muted">
+      <a href="{{url_for('security.login')}}">{{_('Log in')}}</a>
+      {% if security.registerable %}
+        {{_('or')}} <a href="{{url_for('security.register')}}">{{_('Sign up')}}</a>
+      {% endif %}
+    </p>
   {%- endif %}
 
 </div>
 {% endblock page_body %}
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
 {# -*- coding: utf-8 -*- This file is part of Invenio. Copyright (C) 2015-2020
 CERN. Invenio is free software; you can redistribute it and/or modify it under
 the terms of the MIT License; see LICENSE file for more details. #} {%- extends
 config.ACCOUNTS_COVER_TEMPLATE %} {% from "invenio_accounts/_macros.html"
 import render_field, form_errors %} {%- set messages = get_flashed_messages
 (with_categories=true) -%} {% block page_body %}
 {%- block form_header %}
-**** {{_('Reset Password')}} ****
+****** {{_('Reset password')}} ******
 {%- endblock form_header %} {%- if messages %} {%- for category, message in
 messages %}
 {{ message }}
 {%- endfor %} {%- else %}
 {{_('Enter your email address below and we will send you a link to reset your
 password.')}}
 {%- with form = forgot_password_form %}
 {{ form.hidden_tag() }} {{ render_field(form.email, icon="user icon",
-autofocus=True, errormsg='email' in form.errors) }} {{_('Reset Password')}}
+autofocus=True, errormsg='email' in form.errors) }} {{_('Reset password')}}
 {%- endwith %} {%- endif %}
 {%- if current_user.is_anonymous %}
-{{_('Log_in')}}{% if security.registerable %} {{_('or')}} {{_('Sign_up')}}{%
+{{_('Log_in')}} {% if security.registerable %} {{_('or')}} {{_('Sign_up')}} {%
 endif %}
 {%- endif %}
 {% endblock page_body %}
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html`

 * *Files 6% similar despite different names*

```diff
@@ -11,42 +11,41 @@
 {% from "invenio_accounts/_macros.html" import render_field, form_errors %}
 
 {% block page_body %}
   <div class="ui padded segments big form">
     <div class="ui login segment padded">
       <div class="divider hidden"></div>
       {%- block form_header %}
-        <h3 class="ui login header">{{ _('Log in to account') }}</h3>
+        <h1 class="ui small login header">{{ _('Log in to account') }}</h1>
       {%- endblock form_header %}
 
       {%- block form_outer %}
         {%- if config.ACCOUNTS_LOCAL_LOGIN_ENABLED %}
           {%- with form = login_user_form %}
             <form action="{{ url_for_security('login') }}" method="POST"
                   name="login_user_form" class="ui big form">
               {{ form.hidden_tag() }}
               {{ render_field(form.email, icon="user icon", autofocus=True, errormsg='email' in form.errors) }}
               {{ render_field(form.password, icon="lock icon", errormsg='password' in form.errors) }}
               <button type="submit" class="ui fluid large submit primary button">
-                <i class="ui sign-in icon"></i>{{ _('Log in') }}
+                <i class="ui sign-in icon" aria-hidden="true"></i>{{ _('Log in') }}
               </button>
             </form>
           {%- endwith %}
         {%- endif %}
       {%- endblock form_outer %}
       <div class="divider hidden"></div>
-
     </div>
 
     {%- block registerable %}
       {%- if security.registerable %}
-        <div class="ui primary segment padded text-muted">
+        <p class="ui primary segment padded text-muted">
             {% trans sitename=config.ACCOUNTS_SITENAME %}New to {{ sitename }}?{% endtrans %}
             <a href="{{ url_for_security('register', next=request.args.get('next')) }}">{{ _('Sign up') }}</a>
-        </div>
+        </p>
       {%- endif %}
     {%- endblock registerable %}
   </div>
 
   {%- block recoverable %}
     {%- if security.recoverable %}
       <div class="ui basic segment padded">
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 {# -*- coding: utf-8 -*- This file is part of Invenio. Copyright (C) 2015-2020
 CERN. Copyright (C) 2021 TU Wien. Invenio is free software; you can
 redistribute it and/or modify it under the terms of the MIT License; see
 LICENSE file for more details. #} {%- extends config.ACCOUNTS_COVER_TEMPLATE %}
 {% from "invenio_accounts/_macros.html" import render_field, form_errors %} {%
 block page_body %}
 {%- block form_header %}
-**** {{ _('Log in to account') }} ****
+****** {{ _('Log in to account') }} ******
 {%- endblock form_header %} {%- block form_outer %} {%- if
 config.ACCOUNTS_LOCAL_LOGIN_ENABLED %} {%- with form = login_user_form %}
 {{ form.hidden_tag() }} {{ render_field(form.email, icon="user icon",
 autofocus=True, errormsg='email' in form.errors) }} {{ render_field
 (form.password, icon="lock icon", errormsg='password' in form.errors) }}  {{ _
 ('Log in') }}
 {%- endwith %} {%- endif %} {%- endblock form_outer %}
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 {% block page_body %}
 
   <div class="ui padded segments big form">
     <div class="ui segment padded relaxed">
       <div class="divider hidden"></div>
 
       {%- block form_header %}
-        <h3 class="ui login header">
+        <h1 class="ui small login header">
           {% trans sitename=config.ACCOUNTS_SITENAME %}Sign up for an {{ sitename }} account!{% endtrans %}
-        </h3>
+        </h1>
       {%- endblock form_header %}
 
       {%- with form = register_user_form %}
         <form action="{{ url_for_security('register') }}" method="POST"
               name="register_user_form">
           {{ form.hidden_tag() }}
           {%- block registration_form_fields scoped %}
@@ -41,14 +41,14 @@
             <i class="ui edit outline icon"></i>{{ _('Sign up') }}
           </button>
         </form>
       {%- endwith %}
       <div class="divider hidden"></div>
     </div>
 
-    <div class="ui primary segment padded text-muted">
+    <p class="ui primary segment padded text-muted">
       {{ _('Already have an account?') }}
       <a href="{{ url_for_security('login', next=request.args.get('next')) }}">{{ _('Log in') }}</a>
-    </div>
+    </p>
   </div>
 
 {% endblock page_body %}
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 {# -*- coding: utf-8 -*- This file is part of Invenio. Copyright (C) 2015-2020
 CERN. Invenio is free software; you can redistribute it and/or modify it under
 the terms of the MIT License; see LICENSE file for more details. #} {%- extends
 config.ACCOUNTS_COVER_TEMPLATE %} {% from "invenio_accounts/_macros.html"
 import render_field, form_errors %} {% block page_body %}
 {%- block form_header %}
-**** {% trans sitename=config.ACCOUNTS_SITENAME %}Sign up for an {{ sitename }}
-account!{% endtrans %} ****
+****** {% trans sitename=config.ACCOUNTS_SITENAME %}Sign up for an {{ sitename
+}} account!{% endtrans %} ******
 {%- endblock form_header %} {%- with form = register_user_form %}
 {{ form.hidden_tag() }} {%- block registration_form_fields scoped %} {
 { render_field(form.email, icon="user icon", autofocus=True, errormsg='email'
 in form.errors) }} {{ render_field(form.password, icon="lock icon",
 errormsg='password' in form.errors) }} {%- if form.password_confirm %} {
 { render_field(form.password_confirm, icon="lock icon", errormsg=False) }} {%-
 endif %} {%- endblock registration_form_fields %} {%- if form.recaptcha %}
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html`

 * *Files 4% similar despite different names*

```diff
@@ -11,34 +11,37 @@
 {% from "invenio_accounts/_macros.html" import render_field, form_errors %}
 {%- set messages = get_flashed_messages(with_categories=true) -%}
 
 {% block page_body %}
 <div class="ui padded segments big form">
   <div class="ui segment">
     {%- block form_header %}
-      <h3 class="ui reset-password header">{{_('Reset Password')}}</h3>
+      <h1 class="ui small reset-password header">{{_('Reset password')}}</h1>
     {%- endblock form_header %}
 
     {%- if messages %}
       {%- for category, message in messages %}
         <p>{{ message }}</p>
       {%- endfor %}
     {%- else %}
       {%- with form = reset_password_form %}
       <form action="{{ url_for_security('reset_password', token=reset_password_token) }}" method="POST" name="reset_password_form">
         {{ form.hidden_tag() }}
         {{ render_field(form.password, icon="lock icon", autofocus=True, errormsg='password' in form.errors) }}
         {{ render_field(form.password_confirm, icon="lock icon", autofocus=False,  errormsg='password_confirm' in form.errors) }}
-        <button type="submit" class="ui fluid large submit primary button">{{_('Reset Password')}}</button>
+        <button type="submit" class="ui fluid large submit primary button">{{_('Reset password')}}</button>
       </form>
       {%- endwith %}
     {%- endif %}
   </div>
 
   {%- if current_user.is_anonymous %}
     <div class="ui secondary segment">
-      <h4><a href="{{url_for('security.login')}}">{{_('Log in')}}</a>{% if security.registerable %}
-        {{_('or')}} <a href="{{url_for('security.register')}}">{{_('Sign up')}}</a>{% endif %}</h4>
-    </div>
+      <p class="ui small header"><a href="{{url_for('security.login')}}">{{_('Log in')}}</a>
+        {% if security.registerable %}
+          {{_('or')}} <a href="{{url_for('security.register')}}">{{_('Sign up')}}</a>
+        {% endif %}
+      </p>
+    </p>
   {%- endif %}
 </div>
 {% endblock page_body %}
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 {# -*- coding: utf-8 -*- This file is part of Invenio. Copyright (C) 2015-2020
 CERN. Invenio is free software; you can redistribute it and/or modify it under
 the terms of the MIT License; see LICENSE file for more details. #} {%- extends
 config.ACCOUNTS_COVER_TEMPLATE %} {% from "invenio_accounts/_macros.html"
 import render_field, form_errors %} {%- set messages = get_flashed_messages
 (with_categories=true) -%} {% block page_body %}
 {%- block form_header %}
-**** {{_('Reset Password')}} ****
+****** {{_('Reset password')}} ******
 {%- endblock form_header %} {%- if messages %} {%- for category, message in
 messages %}
 {{ message }}
 {%- endfor %} {%- else %} {%- with form = reset_password_form %}
 {{ form.hidden_tag() }} {{ render_field(form.password, icon="lock icon",
 autofocus=True, errormsg='password' in form.errors) }} {{ render_field
 (form.password_confirm, icon="lock icon", autofocus=False,
-errormsg='password_confirm' in form.errors) }} {{_('Reset Password')}}
+errormsg='password_confirm' in form.errors) }} {{_('Reset password')}}
 {%- endwith %} {%- endif %}
 {%- if current_user.is_anonymous %}
-*** {{_('Log_in')}}{% if security.registerable %} {{_('or')}} {{_('Sign_up')}}
-{% endif %} ***
+{{_('Log_in')}} {% if security.registerable %} {{_('or')}} {{_('Sign_up')}} {%
+endif %}
 {%- endif %}
 {% endblock page_body %}
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/send_confirmation.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/send_confirmation.html`

 * *Files 4% similar despite different names*

```diff
@@ -10,50 +10,54 @@
 
 {% from "invenio_accounts/_macros.html" import render_field, form_errors %}
 {% block page_header %}
 <div class="ui two column centered grid">
   <div class="row"></div>
   <div class="row"></div>
   <div class="column">
-    {%- block brand %} {%- if config.THEME_LOGO %}
-    <a href="/">
-      <img
-        class="ui centered image masthead-brand"
-        src="{{ url_for('static', filename=config.THEME_LOGO)}}"
-        alt="{{ _(config.THEME_SITENAME) }}"
-        width="250px"
-      />
-    </a>
-    {%- elif config.THEME_SITENAME %}
-    <a href="/" class="text-center masthead-brand">
-      {{ _(config.THEME_SITENAME) }}
-    </a>
-    {% endif %} {%- endblock %}
+    {%- block brand %}
+      {%- if config.THEME_LOGO %}
+        <a href="/">
+          <img
+            class="ui centered image masthead-brand"
+            src="{{ url_for('static', filename=config.THEME_LOGO)}}"
+            alt="{{ _(config.THEME_SITENAME) }}"
+            width="250px"
+          />
+        </a>
+        {%- elif config.THEME_SITENAME %}
+        <a href="/" class="text-center masthead-brand">
+          {{ _(config.THEME_SITENAME) }}
+        </a>
+      {% endif %}
+    {%- endblock %}
   </div>
 </div>
 {% endblock page_header%}
 
 {% block page_body %}
-{%- with form = send_confirmation_form %}
-<div class="ui doubling three column centered grid">
-  <div class="row"></div>
-  <div class="row">
-    <div class="column ui middle">
-      <h1 class="ui header aligned center">{{config.ACCOUNTS_SITENAME}}</h1>
-      <div class="ui segment">
-        <h3 class="ui header aligned center">{{_('Resend Confirmation Email')}}</h3>
-        <div class="column ui middle">
-          <p class="left floated">{{_('Enter your email address below and we will send you an email confirmation link.')}}</p>
+  {%- with form = send_confirmation_form %}
+  <div class="ui doubling three column centered grid">
+    <div class="row"></div>
+    <div class="row">
+      <div class="column ui middle">
+        <h1 class="ui header aligned center">{{config.ACCOUNTS_SITENAME}}</h1>
+        <div class="ui segment">
+          <h2 class="ui header aligned center">{{_('Resend confirmation email')}}</h2>
+          <div class="column ui middle">
+            <p class="left floated">
+              {{_('Enter your email address below and we will send you an email confirmation link.')}}
+            </p>
+          </div>
+          <form class="ui large form" action="{{ url_for_security('login') }}" method="POST" name="login_user_form">
+            {{form.hidden_tag()}}
+            {{ render_field(form.email, icon="icon user", autofocus=True, errormsg='email' in form.errors) }}
+            <button type="submit" class="ui fluid large submit primary button">
+              <i class="ui sign-in icon" aria-hidden="true"></i>{{_('Send confirmation')}}
+            </button>
+          </form>
         </div>
-        <form class="ui large form" action="{{ url_for_security('login') }}" method="POST" name="login_user_form">
-        {{form.hidden_tag()}}
-        {{ render_field(form.email, icon="icon user", autofocus=True, errormsg='email' in form.errors) }}
-        <button type="submit" class="ui fluid large submit primary button">
-          <i class="ui sign-in icon"></i>{{_('Send Confirmation')}}
-        </button>
-        </form>
       </div>
     </div>
   </div>
-</div>
-{%- endwith %}
+  {%- endwith %}
 {% endblock page_body %}
```

#### html2text {}

```diff
@@ -5,13 +5,13 @@
 import render_field, form_errors %} {% block page_header %}
 {%- block brand %} {%- if config.THEME_LOGO %} [{{__(config.THEME_SITENAME)_}}]
 {%- elif config.THEME_SITENAME %} {{__(config.THEME_SITENAME)_}} {% endif %}
 {%- endblock %}
 {% endblock page_header%} {% block page_body %} {%- with form =
 send_confirmation_form %}
 ****** {{config.ACCOUNTS_SITENAME}} ******
-**** {{_('Resend Confirmation Email')}} ****
+***** {{_('Resend confirmation email')}} *****
 {{_('Enter your email address below and we will send you an email confirmation
 link.')}}
 {{form.hidden_tag()}} {{ render_field(form.email, icon="icon user",
-autofocus=True, errormsg='email' in form.errors) }}  {{_('Send Confirmation')}}
+autofocus=True, errormsg='email' in form.errors) }}  {{_('Send confirmation')}}
 {%- endwith %} {% endblock page_body %}
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html` & `invenio-accounts-3.1.0/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html`

 * *Files 12% similar despite different names*

```diff
@@ -8,55 +8,71 @@
 #}
 {%- extends config.ACCOUNTS_SETTINGS_TEMPLATE %}
 
 {% set panel_title = _('Sessions') %}
 {% set panel_icon = current_theme_icons.shield %}
 {% from "invenio_accounts/_macros.html" import render_field, form_errors %}
 
-{% block settings_form %}
-  <p>{{_('This is a list of devices that have logged into your account.')}}</p>
-  <div class="ui divider"></div>
-  <div class="ui items">
-    {%- for session in sessions %}
-    {%- set is_current_sid = is_current(session.sid_s) %}
-    {%- set form = formclass(sid_s=session.sid_s) %}
-    <div class="item">
-      <div>
-        {%- if is_current_sid %}
-          <i class="circle icon green" aria-hidden="true"></i>
-        {%- else %}
-          <i class="circle icon grey" aria-hidden="true"></i>
-        {%- endif %}
-      </div>
-      <div class="content">
-        <h5 class="ui header">{{ session.ip }}</h5>
-        <br>
-        <small>
-          {{_("Signed in")}}:
-          {{ session.created | tousertimezone | dateformat }}
-          {% if is_current_sid %}({{ _("current session") }}){% endif %}
-          {%- if session.browser %}
-            <br>
-            {{ session.browser }} {{ session.browser_version }} on {{ session.os }} ({{ session.device }})
-          {%- endif %}
-          {%- if session.country %}
-            <br>{{_('Location')}}: {{session.country}}
-          {%- endif %}
-        </small>
-      </div>
-      <div>
-        <form
-          action="{{url_for('invenio_accounts.revoke_session') if not is_current_sid else url_for_security('logout')}}"
-          method="{{'POST' if not is_current_sid else 'GET'}}"
-        >
-          {{ form.csrf_token }}
-          {{ form.sid_s }}
-          <button type="submit" class="ui right floated button" title="{{remove_action}}">
-            <i class="{{'times' if not is_current_sid else 'sign-out'}} icon"></i> {{_("Revoke") if not is_current_sid else _('Logout')}}
-          </button>
-        </form>
-      </div>
-    </div>
-    {% endfor %}
-   </div>
+{%- block settings_body %}
+
+  {% block settings_form %}
+    <p class="ui segment">{{_('This is a list of devices that have logged into your account.')}}</p>
+
+    <ul class="ui segments no-border no-border-radius-top no-style-list m-0 p-0">
+      {%- for session in sessions %}
+        {%- set is_current_sid = is_current(session.sid_s) %}
+        {%- set form = formclass(sid_s=session.sid_s) %}
+        <li class="ui segment grid">
+          <div class="two column stackable row">
+            <div class="column">
+              <div class="header mb-10 flex">
+                {%- if is_current_sid %}
+                  <i class="circle icon green" aria-hidden="true"></i>
+                {%- else %}
+                  <i class="circle icon grey" aria-hidden="true"></i>
+                {%- endif %}
+                <h2 class="ui tiny header m-0">{{ session.ip }}</h2>
+              </div>
+
+              <p>
+                <small>
+                  {{_("Signed in")}}:
+                  {{ session.created | tousertimezone | dateformat }}
+                  {% if is_current_sid %}({{ _("current session") }}){% endif %}
+                  {%- if session.browser %}
+                    <br>
+                    {{ session.browser }} {{ session.browser_version }} on {{ session.os }} ({{ session.device }})
+                  {%- endif %}
+                  {%- if session.country %}
+                    <br>{{_('Location')}}: {{session.country}}
+                  {%- endif %}
+                </small>
+              </p>
+            </div>
+
+            <div class="middle aligned column">
+              <form
+                action="{{url_for('invenio_accounts.revoke_session') if not is_current_sid else url_for_security('logout')}}"
+                method="{{'POST' if not is_current_sid else 'GET'}}"
+              >
+                {{ form.csrf_token }}
+                {{ form.sid_s }}
+                <button
+                  type="submit"
+                  class="ui right floated labeled icon button"
+                  title="{{remove_action}}"
+                >
+                  <i
+                    class="{{'times' if not is_current_sid else 'sign-out'}} icon"
+                    aria-hidden="true"
+                  ></i>
+                  {{_("Revoke") if not is_current_sid else _('Logout')}}
+                </button>
+              </form>
+            </div>
+          </div>
+        </li>
+      {% endfor %}
+    </ul>
+  {% endblock settings_form %}
+{%- endblock settings_body %}
 
-{% endblock settings_form %}
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/testutils.py` & `invenio-accounts-3.1.0/invenio_accounts/testutils.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/af/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/af/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-accounts 2.0.0*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 3a20 3230 3136 2d30 382d 3138 2030 383a  : 2016-08-18 08:
 000000d0: 3239 2b30 3030 300a 4c61 7374 2d54 7261  29+0000.Last-Tra
 000000e0: 6e73 6c61 746f 723a 2046 554c 4c20 4e41  nslator: FULL NA
 000000f0: 4d45 203c 454d 4149 4c40 4144 4452 4553  ME <EMAIL@ADDRES
 00000100: 533e 0a4c 616e 6775 6167 653a 2061 660a  S>.Language: af.
 00000110: 4c61 6e67 7561 6765 2d54 6561 6d3a 2041  Language-Team: A
 00000120: 6672 696b 6161 6e73 2028 6874 7470 733a  frikaans (https:
-00000130: 2f2f 7777 772e 7472 616e 7369 6665 782e  //www.transifex.
+00000130: 2f2f 6170 702e 7472 616e 7369 6665 782e  //app.transifex.
 00000140: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
 00000150: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
 00000160: 6166 2f29 0a50 6c75 7261 6c2d 466f 726d  af/).Plural-Form
 00000170: 733a 206e 706c 7572 616c 733d 323b 2070  s: nplurals=2; p
 00000180: 6c75 7261 6c3d 286e 2021 3d20 3129 3b0a  lural=(n != 1);.
 00000190: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
 000001a0: 300a 436f 6e74 656e 742d 5479 7065 3a20  0.Content-Type:
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/af/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/af/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
-"Language-Team: Afrikaans (https://www.transifex.com/inveniosoftware/teams/23537/af/)\n"
+"Language-Team: Afrikaans (https://app.transifex.com/inveniosoftware/teams/23537/af/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: af\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/ar/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/ar/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,16 +1,16 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
-"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022\n"
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
@@ -153,15 +153,15 @@
 "Username must start with a letter, be at least three characters long and "
 "only contain alphanumeric characters, dashes and underscores."
 msgstr ""
 "إسم المستخدم يتكون من ثلاثة حروف على الأقل. يجب ان يبدأ بحرف هجائي. و تستعمل "
 "فيه الحروف الهجائية، الأرقم و الشّرطات القصيرة و الطويلة."
 
 msgid "Value must be either 'public' or 'restricted'."
-msgstr "يجب أن تكون القيمة إما \"عام\" أو \"مقيّد\"."
+msgstr "يجب أن تكون القيمة إما \"مشاع\" أو \"مقيّد\"."
 
 msgid "Your password has been changed."
 msgstr "تم تغيير كلمة العبور الخاصة بك."
 
 msgid "click here to reset it."
 msgstr "انقر هنا لإعادة ضبطه"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/ar/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/ar/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # This file is distributed under the same license as the invenio-accounts
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2017
 # Bessem Aamira <bessemamira@gmail.com>, 2022
-# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022
+# Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
-"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2022\n"
-"Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/ar/)\n"
+"Last-Translator: Salaheddine Ben Ali <salaheddine.benali@cnudst.tn>, 2023\n"
+"Language-Team: Arabic (https://app.transifex.com/inveniosoftware/teams/23537/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
@@ -84,15 +84,15 @@
 
 #: invenio_accounts/forms.py:24
 msgid "Please complete the reCAPTCHA."
 msgstr "يرجى إكمال اختبار reCAPTCHA."
 
 #: invenio_accounts/profiles/schemas.py:20
 msgid "Value must be either 'public' or 'restricted'."
-msgstr "يجب أن تكون القيمة إما \"عام\" أو \"مقيّد\"."
+msgstr "يجب أن تكون القيمة إما \"مشاع\" أو \"مقيّد\"."
 
 #: invenio_accounts/templates/invenio_accounts/change_password.html:13
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html:13
 #: invenio_accounts/views/settings.py:80
 msgid "Change password"
 msgstr "غير كلمة المرور"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/bg/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/bg/LC_MESSAGES/messages.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/bg/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/bg/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/teams/23537/bg/)\n"
+"Language-Team: Bulgarian (https://app.transifex.com/inveniosoftware/teams/23537/bg/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: bg\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/ca/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/ca/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/ca/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/ca/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Catalan (https://www.transifex.com/inveniosoftware/teams/23537/ca/)\n"
+"Language-Team: Catalan (https://app.transifex.com/inveniosoftware/teams/23537/ca/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ca\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/cs/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/cs/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Jiří Kunčar <jiri.kuncar@gmail.com>, 2022\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/cs/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/cs/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Jiří Kunčar <jiri.kuncar@gmail.com>, 2022\n"
-"Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/cs/)\n"
+"Language-Team: Czech (https://app.transifex.com/inveniosoftware/teams/23537/cs/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: cs\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/da/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/da/LC_MESSAGES/messages.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/da/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/da/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/da/)\n"
+"Language-Team: Danish (https://app.transifex.com/inveniosoftware/teams/23537/da/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: da\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/de/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/de/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/de/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/de/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/el/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/el/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/el/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/el/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/es/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/es/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/es/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/es/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/et/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/et/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Mart Jantson, 2022\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/et/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/et/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Mart Jantson, 2022\n"
-"Language-Team: Estonian (https://www.transifex.com/inveniosoftware/teams/23537/et/)\n"
+"Language-Team: Estonian (https://app.transifex.com/inveniosoftware/teams/23537/et/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: et\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-accounts 2.0.0*

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 e701 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 e201 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d61 6363 6f75 6e74   invenio-account
 00000050: 7320 322e 302e 300a 5265 706f 7274 2d4d  s 2.0.0.Report-M
 00000060: 7367 6964 2d42 7567 732d 546f 3a20 696e  sgid-Bugs-To: in
 00000070: 666f 4069 6e76 656e 696f 736f 6674 7761  fo@inveniosoftwa
 00000080: 7265 2e6f 7267 0a50 4f54 2d43 7265 6174  re.org.POT-Creat
 00000090: 696f 6e2d 4461 7465 3a20 3230 3232 2d31  ion-Date: 2022-1
 000000a0: 302d 3132 2030 393a 3035 2b30 3030 300a  0-12 09:05+0000.
 000000b0: 504f 2d52 6576 6973 696f 6e2d 4461 7465  PO-Revision-Date
 000000c0: 3a20 3230 3136 2d30 382d 3138 2030 383a  : 2016-08-18 08:
 000000d0: 3239 2b30 3030 300a 4c61 7374 2d54 7261  29+0000.Last-Tra
 000000e0: 6e73 6c61 746f 723a 2046 554c 4c20 4e41  nslator: FULL NA
 000000f0: 4d45 203c 454d 4149 4c40 4144 4452 4553  ME <EMAIL@ADDRES
-00000100: 533e 0a4c 616e 6775 6167 653a 2065 745f  S>.Language: et_
-00000110: 4545 0a4c 616e 6775 6167 652d 5465 616d  EE.Language-Team
-00000120: 3a20 4573 746f 6e69 616e 2028 4573 746f  : Estonian (Esto
-00000130: 6e69 6129 2028 6874 7470 733a 2f2f 7777  nia) (https://ww
-00000140: 772e 7472 616e 7369 6665 782e 636f 6d2f  w.transifex.com/
-00000150: 696e 7665 6e69 6f73 6f66 7477 6172 652f  inveniosoftware/
-00000160: 7465 616d 732f 3233 3533 372f 6574 5f45  teams/23537/et_E
-00000170: 452f 290a 506c 7572 616c 2d46 6f72 6d73  E/).Plural-Forms
-00000180: 3a20 6e70 6c75 7261 6c73 3d32 3b20 706c  : nplurals=2; pl
-00000190: 7572 616c 3d28 6e20 213d 2031 293b 0a4d  ural=(n != 1);.M
-000001a0: 494d 452d 5665 7273 696f 6e3a 2031 2e30  IME-Version: 1.0
-000001b0: 0a43 6f6e 7465 6e74 2d54 7970 653a 2074  .Content-Type: t
-000001c0: 6578 742f 706c 6169 6e3b 2063 6861 7273  ext/plain; chars
-000001d0: 6574 3d75 7466 2d38 0a43 6f6e 7465 6e74  et=utf-8.Content
-000001e0: 2d54 7261 6e73 6665 722d 456e 636f 6469  -Transfer-Encodi
-000001f0: 6e67 3a20 3862 6974 0a47 656e 6572 6174  ng: 8bit.Generat
-00000200: 6564 2d42 793a 2042 6162 656c 2032 2e31  ed-By: Babel 2.1
-00000210: 322e 310a 00                             2.1..
+00000100: 533e 0a4c 616e 6775 6167 653a 2066 615f  S>.Language: fa_
+00000110: 4952 0a4c 616e 6775 6167 652d 5465 616d  IR.Language-Team
+00000120: 3a20 5065 7273 6961 6e20 2849 7261 6e29  : Persian (Iran)
+00000130: 2028 6874 7470 733a 2f2f 6170 702e 7472   (https://app.tr
+00000140: 616e 7369 6665 782e 636f 6d2f 696e 7665  ansifex.com/inve
+00000150: 6e69 6f73 6f66 7477 6172 652f 7465 616d  niosoftware/team
+00000160: 732f 3233 3533 372f 6661 5f49 522f 290a  s/23537/fa_IR/).
+00000170: 506c 7572 616c 2d46 6f72 6d73 3a20 6e70  Plural-Forms: np
+00000180: 6c75 7261 6c73 3d32 3b20 706c 7572 616c  lurals=2; plural
+00000190: 3d28 6e20 3e20 3129 3b0a 4d49 4d45 2d56  =(n > 1);.MIME-V
+000001a0: 6572 7369 6f6e 3a20 312e 300a 436f 6e74  ersion: 1.0.Cont
+000001b0: 656e 742d 5479 7065 3a20 7465 7874 2f70  ent-Type: text/p
+000001c0: 6c61 696e 3b20 6368 6172 7365 743d 7574  lain; charset=ut
+000001d0: 662d 380a 436f 6e74 656e 742d 5472 616e  f-8.Content-Tran
+000001e0: 7366 6572 2d45 6e63 6f64 696e 673a 2038  sfer-Encoding: 8
+000001f0: 6269 740a 4765 6e65 7261 7465 642d 4279  bit.Generated-By
+00000200: 3a20 4261 6265 6c20 322e 3132 2e31 0a00  : Babel 2.12.1..
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
-"Language-Team: Estonian (Estonia) (https://www.transifex.com/inveniosoftware/teams/23537/et_EE/)\n"
+"Language-Team: German (Austria) (https://app.transifex.com/inveniosoftware/teams/23537/de_AT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: et_EE\n"
+"Language: de_AT\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_accounts/admin.py:78
 msgid "Inactivate"
 msgstr ""
 
 #: invenio_accounts/admin.py:79
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/fa/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/fa/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/fa/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/fa/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/fr/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/fr/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/fr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/gl/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/gl/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-accounts 2.0.0*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 3a20 3230 3136 2d30 382d 3138 2030 383a  : 2016-08-18 08:
 000000d0: 3239 2b30 3030 300a 4c61 7374 2d54 7261  29+0000.Last-Tra
 000000e0: 6e73 6c61 746f 723a 2046 554c 4c20 4e41  nslator: FULL NA
 000000f0: 4d45 203c 454d 4149 4c40 4144 4452 4553  ME <EMAIL@ADDRES
 00000100: 533e 0a4c 616e 6775 6167 653a 2067 6c0a  S>.Language: gl.
 00000110: 4c61 6e67 7561 6765 2d54 6561 6d3a 2047  Language-Team: G
 00000120: 616c 6963 6961 6e20 2868 7474 7073 3a2f  alician (https:/
-00000130: 2f77 7777 2e74 7261 6e73 6966 6578 2e63  /www.transifex.c
+00000130: 2f61 7070 2e74 7261 6e73 6966 6578 2e63  /app.transifex.c
 00000140: 6f6d 2f69 6e76 656e 696f 736f 6674 7761  om/inveniosoftwa
 00000150: 7265 2f74 6561 6d73 2f32 3335 3337 2f67  re/teams/23537/g
 00000160: 6c2f 290a 506c 7572 616c 2d46 6f72 6d73  l/).Plural-Forms
 00000170: 3a20 6e70 6c75 7261 6c73 3d32 3b20 706c  : nplurals=2; pl
 00000180: 7572 616c 3d28 6e20 213d 2031 293b 0a4d  ural=(n != 1);.M
 00000190: 494d 452d 5665 7273 696f 6e3a 2031 2e30  IME-Version: 1.0
 000001a0: 0a43 6f6e 7465 6e74 2d54 7970 653a 2074  .Content-Type: t
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/gl/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
-"Language-Team: Galician (https://www.transifex.com/inveniosoftware/teams/23537/gl/)\n"
+"Language-Team: German (Germany) (https://app.transifex.com/inveniosoftware/teams/23537/de_DE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: gl\n"
+"Language: de_DE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_accounts/admin.py:78
 msgid "Inactivate"
 msgstr ""
 
 #: invenio_accounts/admin.py:79
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/hr/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/hr/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/hr/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/hr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Croatian (https://www.transifex.com/inveniosoftware/teams/23537/hr/)\n"
+"Language-Team: Croatian (https://app.transifex.com/inveniosoftware/teams/23537/hr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: hr\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/hu/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/hu/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Andrea Dömötör, 2022\n"
 "Language: hu\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/"
 "teams/23537/hu/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/hu/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/hu/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Andrea Dömötör, 2022\n"
-"Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/teams/23537/hu/)\n"
+"Language-Team: Hungarian (https://app.transifex.com/inveniosoftware/teams/23537/hu/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: hu\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/it/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/it/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/it/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/it/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Alizee Pace <alizee.pace@gmail.com>, 2022\n"
-"Language-Team: Italian (https://www.transifex.com/inveniosoftware/teams/23537/it/)\n"
+"Language-Team: Italian (https://app.transifex.com/inveniosoftware/teams/23537/it/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: it\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/ja/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/ja/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/ja/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/ja/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Japanese (https://www.transifex.com/inveniosoftware/teams/23537/ja/)\n"
+"Language-Team: Japanese (https://app.transifex.com/inveniosoftware/teams/23537/ja/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ja\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/ka/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/ka/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/ka/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/ka/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Georgian (https://www.transifex.com/inveniosoftware/teams/23537/ka/)\n"
+"Language-Team: Georgian (https://app.transifex.com/inveniosoftware/teams/23537/ka/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/lt/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/lt/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/lt/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/lt/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Lithuanian (https://www.transifex.com/inveniosoftware/teams/23537/lt/)\n"
+"Language-Team: Lithuanian (https://app.transifex.com/inveniosoftware/teams/23537/lt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: lt\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/messages.pot` & `invenio-accounts-3.1.0/invenio_accounts/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/no/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/no/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/no/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/no/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/teams/23537/no/)\n"
+"Language-Team: Norwegian (https://app.transifex.com/inveniosoftware/teams/23537/no/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: no\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/pl/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/pl/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/pl/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/pl/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Polish (https://www.transifex.com/inveniosoftware/teams/23537/pl/)\n"
+"Language-Team: Polish (https://app.transifex.com/inveniosoftware/teams/23537/pl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/pt/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/pt/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/pt/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/pt/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/teams/23537/pt/)\n"
+"Language-Team: Portuguese (https://app.transifex.com/inveniosoftware/teams/23537/pt/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: pt\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/ro/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
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
 
 #: invenio_accounts/admin.py:78
 msgid "Inactivate"
 msgstr ""
 
 #: invenio_accounts/admin.py:79
 msgid "Are you sure you want to inactivate selected users?"
@@ -53,19 +53,19 @@
 
 #: invenio_accounts/admin.py:124
 msgid "Failed to activate users."
 msgstr ""
 
 #: invenio_accounts/admin.py:222
 msgid "Email"
-msgstr "E-mail"
+msgstr "電郵"
 
 #: invenio_accounts/admin.py:223
 msgid "User ID"
-msgstr "ID Utilizator"
+msgstr "用戶ID"
 
 #: invenio_accounts/admin.py:230 invenio_accounts/admin.py:236
 #: invenio_accounts/admin.py:242 invenio_accounts/admin.py:248
 msgid "User Management"
 msgstr ""
 
 #: invenio_accounts/admin.py:249
@@ -96,15 +96,15 @@
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html:21
 msgid "Current password"
 msgstr ""
 
 #: invenio_accounts/templates/invenio_accounts/change_password.html:26
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html:25
 msgid "New password"
-msgstr "Parola nouă"
+msgstr "新密碼"
 
 #: invenio_accounts/templates/invenio_accounts/change_password.html:30
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html:29
 msgid "Confirm new password"
 msgstr ""
 
 #: invenio_accounts/templates/invenio_accounts/change_password.html:34
@@ -142,15 +142,15 @@
 msgstr ""
 
 #: invenio_accounts/templates/invenio_accounts/forgot_password.html:37
 #: invenio_accounts/templates/invenio_accounts/reset_password.html:38
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html:44
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html:40
 msgid "or"
-msgstr "sau"
+msgstr "或"
 
 #: invenio_accounts/templates/invenio_accounts/forgot_password.html:37
 #: invenio_accounts/templates/invenio_accounts/login_user.html:38
 #: invenio_accounts/templates/invenio_accounts/register_user.html:32
 #: invenio_accounts/templates/invenio_accounts/reset_password.html:38
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html:44
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html:44
@@ -231,15 +231,15 @@
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html:42
 msgid "Location"
 msgstr ""
 
 #: invenio_accounts/templates/invenio_accounts/settings/security.html:55
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html:54
 msgid "Logout"
-msgstr ""
+msgstr "登出"
 
 #: invenio_accounts/templates/security/email/change_notice_rest.html:1
 msgid "Your password has been changed."
 msgstr ""
 
 #: invenio_accounts/templates/security/email/change_notice_rest.html:3
 msgid "If you did not change your password,"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/ru/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/ru/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/ru/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/ru/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Russian (https://www.transifex.com/inveniosoftware/teams/23537/ru/)\n"
+"Language-Team: Russian (https://app.transifex.com/inveniosoftware/teams/23537/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/rw/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/rw/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-accounts 2.0.0*

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: 3a20 3230 3136 2d30 382d 3138 2030 383a  : 2016-08-18 08:
 000000d0: 3239 2b30 3030 300a 4c61 7374 2d54 7261  29+0000.Last-Tra
 000000e0: 6e73 6c61 746f 723a 2046 554c 4c20 4e41  nslator: FULL NA
 000000f0: 4d45 203c 454d 4149 4c40 4144 4452 4553  ME <EMAIL@ADDRES
 00000100: 533e 0a4c 616e 6775 6167 653a 2072 770a  S>.Language: rw.
 00000110: 4c61 6e67 7561 6765 2d54 6561 6d3a 204b  Language-Team: K
 00000120: 696e 7961 7277 616e 6461 2028 6874 7470  inyarwanda (http
-00000130: 733a 2f2f 7777 772e 7472 616e 7369 6665  s://www.transife
+00000130: 733a 2f2f 6170 702e 7472 616e 7369 6665  s://app.transife
 00000140: 782e 636f 6d2f 696e 7665 6e69 6f73 6f66  x.com/inveniosof
 00000150: 7477 6172 652f 7465 616d 732f 3233 3533  tware/teams/2353
 00000160: 372f 7277 2f29 0a50 6c75 7261 6c2d 466f  7/rw/).Plural-Fo
 00000170: 726d 733a 206e 706c 7572 616c 733d 323b  rms: nplurals=2;
 00000180: 2070 6c75 7261 6c3d 286e 2021 3d20 3129   plural=(n != 1)
 00000190: 3b0a 4d49 4d45 2d56 6572 7369 6f6e 3a20  ;.MIME-Version: 
 000001a0: 312e 300a 436f 6e74 656e 742d 5479 7065  1.0.Content-Type
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/rw/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
-"Language-Team: Kinyarwanda (https://www.transifex.com/inveniosoftware/teams/23537/rw/)\n"
+"Language-Team: English (Austria) (https://app.transifex.com/inveniosoftware/teams/23537/en_AT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: rw\n"
+"Language: en_AT\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: invenio_accounts/admin.py:78
 msgid "Inactivate"
 msgstr ""
 
 #: invenio_accounts/admin.py:79
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/sk/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/sk/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/sk/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/sk/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/sv/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/sv/LC_MESSAGES/messages.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,34 +1,34 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
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
 
 msgid "%(icon)s Change password"
 msgstr "%(icon)s Ändra lösenord"
 
 msgid "%(icon)s Security"
 msgstr "%(icon)s Säkerhet"
 
 msgid "Account"
-msgstr "konto"
+msgstr "Konto"
 
 msgid "Activate"
-msgstr "Active"
+msgstr "Aktivera"
 
 msgid "Already have an account?"
 msgstr "Har du redan ett konto?"
 
 msgid "Are you sure you want to activate selected users?"
 msgstr "Är du säker på att du vill aktivera valda användare?"
 
@@ -38,15 +38,15 @@
 msgid "Cannot find user."
 msgstr "Kan inte hitta användare."
 
 msgid "Change Password"
 msgstr "Ändra Lösenord"
 
 msgid "Change password"
-msgstr "ändra lösenord"
+msgstr "Ändra lösenord"
 
 msgid "Confirm new password"
 msgstr "Bekräfta nytt lösenord"
 
 msgid "Current password"
 msgstr "Nuvarande lösenord"
 
@@ -82,15 +82,15 @@
 msgid "Inactivate"
 msgstr "Inaktivera"
 
 msgid "Linked account identities"
 msgstr "Länkade kontoidentiteter"
 
 msgid "Location"
-msgstr "Lokalisering"
+msgstr "Plats"
 
 msgid "Log in"
 msgstr "Logga in"
 
 msgid "Log in to account"
 msgstr "Logga in på kontot"
 
@@ -103,15 +103,15 @@
 msgid "New to %(sitename)s?"
 msgstr "Ny på %(sitename)s?"
 
 msgid "Please complete the reCAPTCHA."
 msgstr "Vänligen slutför reCAPTCHA."
 
 msgid "Resend Confirmation Email"
-msgstr "Skicka om e-postbekräftelse"
+msgstr "Skicka om bekräftelsemejl"
 
 msgid "Reset Password"
 msgstr "Återställ lösenord"
 
 msgid "Revoke"
 msgstr "Återkalla"
 
@@ -121,36 +121,36 @@
 msgid "Send Confirmation"
 msgstr "Skicka bekräftelse"
 
 msgid "Sessions"
 msgstr "Sessioner"
 
 msgid "Sign up"
-msgstr "Skriva upp"
+msgstr "Registrera konto"
 
 msgid "Sign up for a %(sitename)s account!"
 msgstr "Registrera dig för ett %(sitename)s konto!"
 
 msgid "Sign up for an %(sitename)s account!"
 msgstr "Registrera dig för ett %(sitename)s konto!"
 
 msgid "Signed in"
 msgstr "Inloggad"
 
 msgid "This is a list of devices that have logged into your account."
 msgstr "Detta är en lista över enheter som har loggat in på ditt konto."
 
 msgid "User ID"
-msgstr "Användarid"
+msgstr "AnvändarId"
 
 msgid "User Management"
-msgstr "Användarhantering"
+msgstr "Hantera användare"
 
 msgid "User(s) were successfully inactivated."
-msgstr "Användare(s) har inaktiverats."
+msgstr "Användare har inaktiverats."
 
 msgid ""
 "Username must start with a letter, be at least three characters long and "
 "only contain alphanumeric characters, dashes and underscores."
 msgstr ""
 "Användarnamn måste börja med en bokstav, vara minst tre tecken långt och "
 "endast innehålla alfanumeriska tecken, bindestreck och understreck."
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/sv/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/ro/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -2,280 +2,280 @@
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-accounts
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
 # Translators:
 # Tibor Simko <tibor.simko@cern.ch>, 2022
-# Sam Arbid, 2022
+# Nicolaie Constantinescu, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
-"Last-Translator: Sam Arbid, 2022\n"
-"Language-Team: Swedish (https://www.transifex.com/inveniosoftware/teams/23537/sv/)\n"
+"Last-Translator: Nicolaie Constantinescu, 2023\n"
+"Language-Team: Romanian (https://app.transifex.com/inveniosoftware/teams/23537/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: sv\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: ro\n"
+"Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
 
 #: invenio_accounts/admin.py:78
 msgid "Inactivate"
-msgstr "Inaktivera"
+msgstr "Inactivează"
 
 #: invenio_accounts/admin.py:79
 msgid "Are you sure you want to inactivate selected users?"
-msgstr "Är du säker på att du vill inaktivera valda användare?"
+msgstr "Ești sigur că dorești inactivarea utilizatorilor selectați?"
 
 #: invenio_accounts/admin.py:89 invenio_accounts/admin.py:114
 msgid "Cannot find user."
-msgstr "Kan inte hitta användare."
+msgstr "Nu găsesc utilizatorul."
 
 #: invenio_accounts/admin.py:93 invenio_accounts/admin.py:118
 msgid "User(s) were successfully inactivated."
-msgstr "Användare(s) har inaktiverats."
+msgstr "Utilizatorul(ii) inactiv(i)."
 
 #: invenio_accounts/admin.py:99
 msgid "Failed to inactivate users."
-msgstr "Det gick inte att inaktivera användare."
+msgstr "Nu pot inactiva utilizatorii."
 
 #: invenio_accounts/admin.py:103
 msgid "Activate"
-msgstr "Active"
+msgstr "Activează"
 
 #: invenio_accounts/admin.py:104
 msgid "Are you sure you want to activate selected users?"
-msgstr "Är du säker på att du vill aktivera valda användare?"
+msgstr "Ești sigur că dorești activarea utilizatorilor selectați?"
 
 #: invenio_accounts/admin.py:124
 msgid "Failed to activate users."
-msgstr "Det gick inte att aktivera användare."
+msgstr "Nu pot activa utilizatorii."
 
 #: invenio_accounts/admin.py:222
 msgid "Email"
-msgstr "Epost"
+msgstr "E-mail"
 
 #: invenio_accounts/admin.py:223
 msgid "User ID"
-msgstr "Användarid"
+msgstr "ID Utilizator"
 
 #: invenio_accounts/admin.py:230 invenio_accounts/admin.py:236
 #: invenio_accounts/admin.py:242 invenio_accounts/admin.py:248
 msgid "User Management"
-msgstr "Användarhantering"
+msgstr "Management utilizatori"
 
 #: invenio_accounts/admin.py:249
 msgid "Linked account identities"
-msgstr "Länkade kontoidentiteter"
+msgstr "Identități conectate a unor conturi diferite"
 
 #: invenio_accounts/config.py:322
 msgid ""
 "Username must start with a letter, be at least three characters long and "
 "only contain alphanumeric characters, dashes and underscores."
 msgstr ""
-"Användarnamn måste börja med en bokstav, vara minst tre tecken långt och "
-"endast innehålla alfanumeriska tecken, bindestreck och understreck."
+"Numele utilizatorului trebuie să înceapă cu o literă, să fie cel puțin de "
+"trei caractere și să conțină caractere alfanumerice, linii sau underscore."
 
 #: invenio_accounts/forms.py:24
 msgid "Please complete the reCAPTCHA."
-msgstr "Vänligen slutför reCAPTCHA."
+msgstr "Rezolvă reCAPTCHA."
 
 #: invenio_accounts/profiles/schemas.py:20
 msgid "Value must be either 'public' or 'restricted'."
-msgstr "Värdet måste vara antingen \"offentligt\" eller \"begränsat\"."
+msgstr "Valoare trebui să fie ori „public”, ori „restricționat”."
 
 #: invenio_accounts/templates/invenio_accounts/change_password.html:13
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html:13
 #: invenio_accounts/views/settings.py:80
 msgid "Change password"
-msgstr "ändra lösenord"
+msgstr "Modifică parola"
 
 #: invenio_accounts/templates/invenio_accounts/change_password.html:22
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html:21
 msgid "Current password"
-msgstr "Nuvarande lösenord"
+msgstr "Parolă curentă"
 
 #: invenio_accounts/templates/invenio_accounts/change_password.html:26
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html:25
 msgid "New password"
-msgstr "Nytt lösenord"
+msgstr "Parola nouă"
 
 #: invenio_accounts/templates/invenio_accounts/change_password.html:30
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html:29
 msgid "Confirm new password"
-msgstr "Bekräfta nytt lösenord"
+msgstr "Confirmă parola nouă"
 
 #: invenio_accounts/templates/invenio_accounts/change_password.html:34
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html:34
 msgid "Change Password"
-msgstr "Ändra Lösenord"
+msgstr "Modifică parola"
 
 #: invenio_accounts/templates/invenio_accounts/forgot_password.html:19
 #: invenio_accounts/templates/invenio_accounts/forgot_password.html:29
 #: invenio_accounts/templates/invenio_accounts/reset_password.html:20
 #: invenio_accounts/templates/invenio_accounts/reset_password.html:30
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html:19
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html:34
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html:18
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html:31
 msgid "Reset Password"
-msgstr "Återställ lösenord"
+msgstr "Resetează parola"
 
 #: invenio_accounts/templates/invenio_accounts/forgot_password.html:25
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html:28
 msgid ""
 "Enter your email address below and we will send you a link to reset your "
 "password."
 msgstr ""
-"Ange din e-postadress nedan så skickar vi en länk för att återställa ditt "
-"lösenord."
+"Introdu mai jos adresa de email și îți vom trimite un link pentru a reseta "
+"parola."
 
 #: invenio_accounts/templates/invenio_accounts/forgot_password.html:37
 #: invenio_accounts/templates/invenio_accounts/login_user.html:29
 #: invenio_accounts/templates/invenio_accounts/register_user.html:38
 #: invenio_accounts/templates/invenio_accounts/reset_password.html:38
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html:43
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html:30
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html:50
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html:39
 msgid "Log in"
-msgstr "Logga in"
+msgstr "Log in"
 
 #: invenio_accounts/templates/invenio_accounts/forgot_password.html:37
 #: invenio_accounts/templates/invenio_accounts/reset_password.html:38
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html:44
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html:40
 msgid "or"
-msgstr "eller"
+msgstr "sau"
 
 #: invenio_accounts/templates/invenio_accounts/forgot_password.html:37
 #: invenio_accounts/templates/invenio_accounts/login_user.html:38
 #: invenio_accounts/templates/invenio_accounts/register_user.html:32
 #: invenio_accounts/templates/invenio_accounts/reset_password.html:38
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html:44
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html:44
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html:41
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html:40
 msgid "Sign up"
-msgstr "Skriva upp"
+msgstr "Sign up"
 
 #: invenio_accounts/templates/invenio_accounts/login_user.html:19
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html:18
 msgid "Log in to account"
-msgstr "Logga in på kontot"
+msgstr "Loghează-te în cont"
 
 #: invenio_accounts/templates/invenio_accounts/login_user.html:38
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html:43
 #, python-format
 msgid "New to %(sitename)s?"
-msgstr "Ny på %(sitename)s?"
+msgstr "Ești nou pe %(sitename)s?"
 
 #: invenio_accounts/templates/invenio_accounts/login_user.html:45
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html:54
 msgid "Forgot password?"
-msgstr "Glömt ditt lösenord?"
+msgstr "Ai uitat parola?"
 
 #: invenio_accounts/templates/invenio_accounts/register_user.html:18
 #, python-format
 msgid "Sign up for a %(sitename)s account!"
-msgstr "Registrera dig för ett %(sitename)s konto!"
+msgstr "Sign up pentru un cont la %(sitename)s!"
 
 #: invenio_accounts/templates/invenio_accounts/register_user.html:37
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html:49
 msgid "Already have an account?"
-msgstr "Har du redan ett konto?"
+msgstr "Ai deja cont?"
 
 #: invenio_accounts/templates/invenio_accounts/send_confirmation.html:19
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/send_confirmation.html:43
 msgid "Resend Confirmation Email"
-msgstr "Skicka om e-postbekräftelse"
+msgstr "Retrimite email de confirmare"
 
 #: invenio_accounts/templates/invenio_accounts/send_confirmation.html:20
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/send_confirmation.html:45
 msgid ""
 "Enter your email address below and we will send you an email confirmation "
 "link."
 msgstr ""
-"Ange din e-postadress nedan så skickar vi en bekräftelselänk till dig via "
-"e-post."
+"Introdu adresa de email mai jos și îți vom trimite un link în email-ul de "
+"confirmare."
 
 #: invenio_accounts/templates/invenio_accounts/send_confirmation.html:25
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/send_confirmation.html:51
 msgid "Send Confirmation"
-msgstr "Skicka bekräftelse"
+msgstr "Trimite confirmare"
 
 #: invenio_accounts/templates/invenio_accounts/settings/security.html:11
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html:11
 msgid "Sessions"
-msgstr "Sessioner"
+msgstr "Sesiuni"
 
 #: invenio_accounts/templates/invenio_accounts/settings/security.html:16
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html:54
 msgid "Revoke"
-msgstr "Återkalla"
+msgstr "Revocă"
 
 #: invenio_accounts/templates/invenio_accounts/settings/security.html:20
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html:16
 msgid "This is a list of devices that have logged into your account."
-msgstr "Detta är en lista över enheter som har loggat in på ditt konto."
+msgstr "Aceasta este o listă cu dispozitive care s-au logat la contul tău."
 
 #: invenio_accounts/templates/invenio_accounts/settings/security.html:36
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html:34
 msgid "Signed in"
-msgstr "Inloggad"
+msgstr "Signed in"
 
 #: invenio_accounts/templates/invenio_accounts/settings/security.html:38
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html:36
 msgid "current session"
-msgstr "nuvarande session"
+msgstr "sesiunea curentă"
 
 #: invenio_accounts/templates/invenio_accounts/settings/security.html:46
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html:42
 msgid "Location"
-msgstr "Lokalisering"
+msgstr "Locație"
 
 #: invenio_accounts/templates/invenio_accounts/settings/security.html:55
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html:54
 msgid "Logout"
-msgstr "Logga ut"
+msgstr "Logout"
 
 #: invenio_accounts/templates/security/email/change_notice_rest.html:1
 msgid "Your password has been changed."
-msgstr "Ditt lösenord har ändrats."
+msgstr "Parola ta a fost modificată."
 
 #: invenio_accounts/templates/security/email/change_notice_rest.html:3
 msgid "If you did not change your password,"
-msgstr "Om du inte ändrade ditt lösenord,"
+msgstr "Dacă nu ai schimbat parola,"
 
 #: invenio_accounts/templates/security/email/change_notice_rest.html:3
 msgid "click here to reset it."
-msgstr "klicka här för att återställa den."
+msgstr "apasă aici pentru a o reseta."
 
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html:20
 #, python-format
 msgid "Sign up for an %(sitename)s account!"
-msgstr "Registrera dig för ett %(sitename)s konto!"
+msgstr "Sign up pentru un cont la %(sitename)s!"
 
 #: invenio_accounts/views/security.py:35
 #, python-format
 msgid "%(icon)s Security"
-msgstr "%(icon)s Säkerhet"
+msgstr "%(icon)s Securitate"
 
 #: invenio_accounts/views/security.py:40
 msgid "Security"
-msgstr "Säkerhet"
+msgstr "Securitate"
 
 #: invenio_accounts/views/settings.py:53
 msgid "Account"
-msgstr "konto"
+msgstr "Cont"
 
 #. NOTE: Menu item text (icon replaced by a key icon).
 #: invenio_accounts/views/settings.py:68
 #, python-format
 msgid "%(icon)s Change password"
-msgstr "%(icon)s Ändra lösenord"
+msgstr "%(icon)s Modifică parola"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/tr/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Berat Aldemir <berataldemir@gmail.com>, 2022\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/tr/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/tr/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Berat Aldemir <berataldemir@gmail.com>, 2022\n"
-"Language-Team: Turkish (https://www.transifex.com/inveniosoftware/teams/23537/tr/)\n"
+"Language-Team: Turkish (https://app.transifex.com/inveniosoftware/teams/23537/tr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
 "Language: tr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/uk/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-accounts 2.0.0*

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,34 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 b602 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 e701 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d61 6363 6f75 6e74   invenio-account
 00000050: 7320 322e 302e 300a 5265 706f 7274 2d4d  s 2.0.0.Report-M
 00000060: 7367 6964 2d42 7567 732d 546f 3a20 696e  sgid-Bugs-To: in
 00000070: 666f 4069 6e76 656e 696f 736f 6674 7761  fo@inveniosoftwa
 00000080: 7265 2e6f 7267 0a50 4f54 2d43 7265 6174  re.org.POT-Creat
 00000090: 696f 6e2d 4461 7465 3a20 3230 3232 2d31  ion-Date: 2022-1
 000000a0: 302d 3132 2030 393a 3035 2b30 3030 300a  0-12 09:05+0000.
 000000b0: 504f 2d52 6576 6973 696f 6e2d 4461 7465  PO-Revision-Date
 000000c0: 3a20 3230 3136 2d30 382d 3138 2030 383a  : 2016-08-18 08:
 000000d0: 3239 2b30 3030 300a 4c61 7374 2d54 7261  29+0000.Last-Tra
 000000e0: 6e73 6c61 746f 723a 2046 554c 4c20 4e41  nslator: FULL NA
 000000f0: 4d45 203c 454d 4149 4c40 4144 4452 4553  ME <EMAIL@ADDRES
-00000100: 533e 0a4c 616e 6775 6167 653a 2075 6b0a  S>.Language: uk.
-00000110: 4c61 6e67 7561 6765 2d54 6561 6d3a 2055  Language-Team: U
-00000120: 6b72 6169 6e69 616e 2028 6874 7470 733a  krainian (https:
-00000130: 2f2f 7777 772e 7472 616e 7369 6665 782e  //www.transifex.
-00000140: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
-00000150: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
-00000160: 756b 2f29 0a50 6c75 7261 6c2d 466f 726d  uk/).Plural-Form
-00000170: 733a 206e 706c 7572 616c 733d 343b 2070  s: nplurals=4; p
-00000180: 6c75 7261 6c3d 286e 2025 2031 203d 3d20  lural=(n % 1 == 
-00000190: 3020 2626 206e 2025 2031 3020 3d3d 2031  0 && n % 10 == 1
-000001a0: 2026 2620 6e20 2520 3130 3020 213d 2031   && n % 100 != 1
-000001b0: 3120 3f20 3020 3a20 6e20 2520 3120 3d3d  1 ? 0 : n % 1 ==
-000001c0: 2030 2026 2620 6e20 2520 3130 203e 3d20   0 && n % 10 >= 
-000001d0: 3220 2626 206e 2025 2031 3020 3c3d 2034  2 && n % 10 <= 4
-000001e0: 2026 2620 286e 2025 2031 3030 203c 2031   && (n % 100 < 1
-000001f0: 3220 7c7c 206e 2025 2031 3030 203e 2031  2 || n % 100 > 1
-00000200: 3429 203f 2031 203a 206e 2025 2031 203d  4) ? 1 : n % 1 =
-00000210: 3d20 3020 2626 2028 6e20 2520 3130 203d  = 0 && (n % 10 =
-00000220: 3d30 207c 7c20 286e 2025 2031 3020 3e3d  =0 || (n % 10 >=
-00000230: 3520 2626 206e 2025 2031 3020 3c3d 3929  5 && n % 10 <=9)
-00000240: 207c 7c20 286e 2025 2031 3030 203e 3d31   || (n % 100 >=1
-00000250: 3120 2626 206e 2025 2031 3030 203c 3d31  1 && n % 100 <=1
-00000260: 3420 2929 203f 2032 3a20 3329 3b0a 4d49  4 )) ? 2: 3);.MI
-00000270: 4d45 2d56 6572 7369 6f6e 3a20 312e 300a  ME-Version: 1.0.
-00000280: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
-00000290: 7874 2f70 6c61 696e 3b20 6368 6172 7365  xt/plain; charse
-000002a0: 743d 7574 662d 380a 436f 6e74 656e 742d  t=utf-8.Content-
-000002b0: 5472 616e 7366 6572 2d45 6e63 6f64 696e  Transfer-Encodin
-000002c0: 673a 2038 6269 740a 4765 6e65 7261 7465  g: 8bit.Generate
-000002d0: 642d 4279 3a20 4261 6265 6c20 322e 3132  d-By: Babel 2.12
-000002e0: 2e31 0a00                                .1..
+00000100: 533e 0a4c 616e 6775 6167 653a 2065 745f  S>.Language: et_
+00000110: 4545 0a4c 616e 6775 6167 652d 5465 616d  EE.Language-Team
+00000120: 3a20 4573 746f 6e69 616e 2028 4573 746f  : Estonian (Esto
+00000130: 6e69 6129 2028 6874 7470 733a 2f2f 6170  nia) (https://ap
+00000140: 702e 7472 616e 7369 6665 782e 636f 6d2f  p.transifex.com/
+00000150: 696e 7665 6e69 6f73 6f66 7477 6172 652f  inveniosoftware/
+00000160: 7465 616d 732f 3233 3533 372f 6574 5f45  teams/23537/et_E
+00000170: 452f 290a 506c 7572 616c 2d46 6f72 6d73  E/).Plural-Forms
+00000180: 3a20 6e70 6c75 7261 6c73 3d32 3b20 706c  : nplurals=2; pl
+00000190: 7572 616c 3d28 6e20 213d 2031 293b 0a4d  ural=(n != 1);.M
+000001a0: 494d 452d 5665 7273 696f 6e3a 2031 2e30  IME-Version: 1.0
+000001b0: 0a43 6f6e 7465 6e74 2d54 7970 653a 2074  .Content-Type: t
+000001c0: 6578 742f 706c 6169 6e3b 2063 6861 7273  ext/plain; chars
+000001d0: 6574 3d75 7466 2d38 0a43 6f6e 7465 6e74  et=utf-8.Content
+000001e0: 2d54 7261 6e73 6665 722d 456e 636f 6469  -Transfer-Encodi
+000001f0: 6e67 3a20 3862 6974 0a47 656e 6572 6174  ng: 8bit.Generat
+00000200: 6564 2d42 793a 2042 6162 656c 2032 2e31  ed-By: Babel 2.1
+00000210: 322e 310a 00                             2.1..
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/uk/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
-"Language-Team: Ukrainian (https://www.transifex.com/inveniosoftware/teams/23537/uk/)\n"
+"Language-Team: Ukrainian (Ukraine) (https://app.transifex.com/inveniosoftware/teams/23537/uk_UA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: uk\n"
+"Language: uk_UA\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #: invenio_accounts/admin.py:78
 msgid "Inactivate"
 msgstr ""
 
 #: invenio_accounts/admin.py:79
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
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

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-accounts-3.1.0/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,15 +2,15 @@
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
 "Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
 "Language: zh_TW\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/"
+"Language-Team: Chinese (Taiwan) (https://app.transifex.com/inveniosoftware/"
 "teams/23537/zh_TW/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-accounts-3.1.0/invenio_accounts/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # Translations template for invenio-accounts.
 # Copyright (C) 2022 CERN
 # This file is distributed under the same license as the invenio-accounts
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 # 
-# Translators:
-# Tibor Simko <tibor.simko@cern.ch>, 2022
-# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio-accounts 2.0.0\n"
 "Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
 "POT-Creation-Date: 2022-10-12 09:05+0000\n"
 "PO-Revision-Date: 2016-08-18 08:29+0000\n"
-"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2022\n"
-"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/teams/23537/zh_TW/)\n"
+"Language-Team: Persian (Iran) (https://app.transifex.com/inveniosoftware/teams/23537/fa_IR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.10.3\n"
-"Language: zh_TW\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Language: fa_IR\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: invenio_accounts/admin.py:78
 msgid "Inactivate"
 msgstr ""
 
 #: invenio_accounts/admin.py:79
 msgid "Are you sure you want to inactivate selected users?"
@@ -53,19 +49,19 @@
 
 #: invenio_accounts/admin.py:124
 msgid "Failed to activate users."
 msgstr ""
 
 #: invenio_accounts/admin.py:222
 msgid "Email"
-msgstr "電郵"
+msgstr ""
 
 #: invenio_accounts/admin.py:223
 msgid "User ID"
-msgstr "用戶ID"
+msgstr ""
 
 #: invenio_accounts/admin.py:230 invenio_accounts/admin.py:236
 #: invenio_accounts/admin.py:242 invenio_accounts/admin.py:248
 msgid "User Management"
 msgstr ""
 
 #: invenio_accounts/admin.py:249
@@ -96,15 +92,15 @@
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html:21
 msgid "Current password"
 msgstr ""
 
 #: invenio_accounts/templates/invenio_accounts/change_password.html:26
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html:25
 msgid "New password"
-msgstr "新密碼"
+msgstr ""
 
 #: invenio_accounts/templates/invenio_accounts/change_password.html:30
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html:29
 msgid "Confirm new password"
 msgstr ""
 
 #: invenio_accounts/templates/invenio_accounts/change_password.html:34
@@ -142,15 +138,15 @@
 msgstr ""
 
 #: invenio_accounts/templates/invenio_accounts/forgot_password.html:37
 #: invenio_accounts/templates/invenio_accounts/reset_password.html:38
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html:44
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html:40
 msgid "or"
-msgstr "或"
+msgstr ""
 
 #: invenio_accounts/templates/invenio_accounts/forgot_password.html:37
 #: invenio_accounts/templates/invenio_accounts/login_user.html:38
 #: invenio_accounts/templates/invenio_accounts/register_user.html:32
 #: invenio_accounts/templates/invenio_accounts/reset_password.html:38
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html:44
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html:44
@@ -231,15 +227,15 @@
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html:42
 msgid "Location"
 msgstr ""
 
 #: invenio_accounts/templates/invenio_accounts/settings/security.html:55
 #: invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html:54
 msgid "Logout"
-msgstr "登出"
+msgstr ""
 
 #: invenio_accounts/templates/security/email/change_notice_rest.html:1
 msgid "Your password has been changed."
 msgstr ""
 
 #: invenio_accounts/templates/security/email/change_notice_rest.html:3
 msgid "If you did not change your password,"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts/utils.py` & `invenio-accounts-3.1.0/invenio_accounts/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/views/__init__.py` & `invenio-accounts-3.1.0/invenio_accounts/views/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/views/rest.py` & `invenio-accounts-3.1.0/invenio_accounts/views/rest.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/views/security.py` & `invenio-accounts-3.1.0/invenio_accounts/views/security.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts/views/settings.py` & `invenio-accounts-3.1.0/invenio_accounts/views/settings.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/invenio_accounts.egg-info/PKG-INFO` & `invenio-accounts-3.1.0/invenio_accounts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-accounts
-Version: 3.0.3
+Version: 3.1.0
 Summary: Invenio user management and authentication.
 Home-page: https://github.com/inveniosoftware/invenio-accounts
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -62,14 +62,19 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 3.1.0 (released 2023-07-31)
+        
+        - templates: Improve accessibility and layout
+        - pulled translations
+        
         Version 3.0.3 (released 2023-06-15)
         
         - models: fix autogeneration of role id
         
         Version 3.0.2 (released 2023-06-14)
         
         - alembic: adapt recipe to mysql
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts.egg-info/SOURCES.txt` & `invenio-accounts-3.1.0/invenio_accounts.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -109,40 +109,64 @@
 invenio_accounts/translations/ca/LC_MESSAGES/messages.po
 invenio_accounts/translations/cs/LC_MESSAGES/messages.mo
 invenio_accounts/translations/cs/LC_MESSAGES/messages.po
 invenio_accounts/translations/da/LC_MESSAGES/messages.mo
 invenio_accounts/translations/da/LC_MESSAGES/messages.po
 invenio_accounts/translations/de/LC_MESSAGES/messages.mo
 invenio_accounts/translations/de/LC_MESSAGES/messages.po
+invenio_accounts/translations/de_AT/LC_MESSAGES/messages.mo
+invenio_accounts/translations/de_AT/LC_MESSAGES/messages.po
+invenio_accounts/translations/de_DE/LC_MESSAGES/messages.mo
+invenio_accounts/translations/de_DE/LC_MESSAGES/messages.po
 invenio_accounts/translations/el/LC_MESSAGES/messages.mo
 invenio_accounts/translations/el/LC_MESSAGES/messages.po
+invenio_accounts/translations/en_AT/LC_MESSAGES/messages.mo
+invenio_accounts/translations/en_AT/LC_MESSAGES/messages.po
+invenio_accounts/translations/en_HU/LC_MESSAGES/messages.mo
+invenio_accounts/translations/en_HU/LC_MESSAGES/messages.po
 invenio_accounts/translations/es/LC_MESSAGES/messages.mo
 invenio_accounts/translations/es/LC_MESSAGES/messages.po
+invenio_accounts/translations/es_CU/LC_MESSAGES/messages.mo
+invenio_accounts/translations/es_CU/LC_MESSAGES/messages.po
+invenio_accounts/translations/es_MX/LC_MESSAGES/messages.mo
+invenio_accounts/translations/es_MX/LC_MESSAGES/messages.po
 invenio_accounts/translations/et/LC_MESSAGES/messages.mo
 invenio_accounts/translations/et/LC_MESSAGES/messages.po
 invenio_accounts/translations/et_EE/LC_MESSAGES/messages.mo
 invenio_accounts/translations/et_EE/LC_MESSAGES/messages.po
 invenio_accounts/translations/fa/LC_MESSAGES/messages.mo
 invenio_accounts/translations/fa/LC_MESSAGES/messages.po
+invenio_accounts/translations/fa_IR/LC_MESSAGES/messages.mo
+invenio_accounts/translations/fa_IR/LC_MESSAGES/messages.po
 invenio_accounts/translations/fr/LC_MESSAGES/messages.mo
 invenio_accounts/translations/fr/LC_MESSAGES/messages.po
+invenio_accounts/translations/fr_CI/LC_MESSAGES/messages.mo
+invenio_accounts/translations/fr_CI/LC_MESSAGES/messages.po
+invenio_accounts/translations/fr_FR/LC_MESSAGES/messages.mo
+invenio_accounts/translations/fr_FR/LC_MESSAGES/messages.po
 invenio_accounts/translations/gl/LC_MESSAGES/messages.mo
 invenio_accounts/translations/gl/LC_MESSAGES/messages.po
+invenio_accounts/translations/hi_IN/LC_MESSAGES/messages.mo
+invenio_accounts/translations/hi_IN/LC_MESSAGES/messages.po
 invenio_accounts/translations/hr/LC_MESSAGES/messages.mo
 invenio_accounts/translations/hr/LC_MESSAGES/messages.po
 invenio_accounts/translations/hu/LC_MESSAGES/messages.mo
 invenio_accounts/translations/hu/LC_MESSAGES/messages.po
+invenio_accounts/translations/hu_HU/LC_MESSAGES/messages.mo
+invenio_accounts/translations/hu_HU/LC_MESSAGES/messages.po
 invenio_accounts/translations/it/LC_MESSAGES/messages.mo
 invenio_accounts/translations/it/LC_MESSAGES/messages.po
 invenio_accounts/translations/ja/LC_MESSAGES/messages.mo
 invenio_accounts/translations/ja/LC_MESSAGES/messages.po
 invenio_accounts/translations/ka/LC_MESSAGES/messages.mo
 invenio_accounts/translations/ka/LC_MESSAGES/messages.po
 invenio_accounts/translations/lt/LC_MESSAGES/messages.mo
 invenio_accounts/translations/lt/LC_MESSAGES/messages.po
+invenio_accounts/translations/ne/LC_MESSAGES/messages.mo
+invenio_accounts/translations/ne/LC_MESSAGES/messages.po
 invenio_accounts/translations/no/LC_MESSAGES/messages.mo
 invenio_accounts/translations/no/LC_MESSAGES/messages.po
 invenio_accounts/translations/pl/LC_MESSAGES/messages.mo
 invenio_accounts/translations/pl/LC_MESSAGES/messages.po
 invenio_accounts/translations/pt/LC_MESSAGES/messages.mo
 invenio_accounts/translations/pt/LC_MESSAGES/messages.po
 invenio_accounts/translations/ro/LC_MESSAGES/messages.mo
@@ -151,18 +175,22 @@
 invenio_accounts/translations/ru/LC_MESSAGES/messages.po
 invenio_accounts/translations/rw/LC_MESSAGES/messages.mo
 invenio_accounts/translations/rw/LC_MESSAGES/messages.po
 invenio_accounts/translations/sk/LC_MESSAGES/messages.mo
 invenio_accounts/translations/sk/LC_MESSAGES/messages.po
 invenio_accounts/translations/sv/LC_MESSAGES/messages.mo
 invenio_accounts/translations/sv/LC_MESSAGES/messages.po
+invenio_accounts/translations/sv_SE/LC_MESSAGES/messages.mo
+invenio_accounts/translations/sv_SE/LC_MESSAGES/messages.po
 invenio_accounts/translations/tr/LC_MESSAGES/messages.mo
 invenio_accounts/translations/tr/LC_MESSAGES/messages.po
 invenio_accounts/translations/uk/LC_MESSAGES/messages.mo
 invenio_accounts/translations/uk/LC_MESSAGES/messages.po
+invenio_accounts/translations/uk_UA/LC_MESSAGES/messages.mo
+invenio_accounts/translations/uk_UA/LC_MESSAGES/messages.po
 invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.mo
 invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.po
 invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.mo
 invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.po
 invenio_accounts/views/__init__.py
 invenio_accounts/views/rest.py
 invenio_accounts/views/security.py
```

### Comparing `invenio-accounts-3.0.3/invenio_accounts.egg-info/entry_points.txt` & `invenio-accounts-3.1.0/invenio_accounts.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/requirements-devel.txt` & `invenio-accounts-3.1.0/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/run-tests.sh` & `invenio-accounts-3.1.0/run-tests.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env bash
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2020 CERN.
-# Copyright (C) 2022 Graz University of Technology.
+# Copyright (C)      2020 CERN.
+# Copyright (C) 2022-2023 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 # Quit on errors
 set -o errexit
```

### Comparing `invenio-accounts-3.0.3/setup.cfg` & `invenio-accounts-3.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/conftest.py` & `invenio-accounts-3.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/e2e/conftest.py` & `invenio-accounts-3.1.0/tests/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/e2e/e2e_basic_test.py` & `invenio-accounts-3.1.0/tests/e2e/e2e_basic_test.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/test_admin.py` & `invenio-accounts-3.1.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/test_cli.py` & `invenio-accounts-3.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/test_forms.py` & `invenio-accounts-3.1.0/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/test_hash.py` & `invenio-accounts-3.1.0/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/test_invenio_accounts.py` & `invenio-accounts-3.1.0/tests/test_invenio_accounts.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/test_models.py` & `invenio-accounts-3.1.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/test_schemas.py` & `invenio-accounts-3.1.0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/test_sessions.py` & `invenio-accounts-3.1.0/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/test_tasks.py` & `invenio-accounts-3.1.0/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/test_template_context_processors.py` & `invenio-accounts-3.1.0/tests/test_template_context_processors.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/test_token_duration.py` & `invenio-accounts-3.1.0/tests/test_token_duration.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/test_utils.py` & `invenio-accounts-3.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/test_validated_dicts.py` & `invenio-accounts-3.1.0/tests/test_validated_dicts.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/test_views.py` & `invenio-accounts-3.1.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.3/tests/test_views_rest.py` & `invenio-accounts-3.1.0/tests/test_views_rest.py`

 * *Files identical despite different names*

