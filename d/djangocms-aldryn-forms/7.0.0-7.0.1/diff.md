# Comparing `tmp/djangocms-aldryn-forms-7.0.0.tar.gz` & `tmp/djangocms-aldryn-forms-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-aldryn-forms-7.0.0.tar", last modified: Wed Jul 26 09:24:11 2023, max compression
+gzip compressed data, was "djangocms-aldryn-forms-7.0.1.tar", last modified: Mon Jul 31 13:29:06 2023, max compression
```

## Comparing `djangocms-aldryn-forms-7.0.0.tar` & `djangocms-aldryn-forms-7.0.1.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.736616 djangocms-aldryn-forms-7.0.0/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1474 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/LICENSE.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      265 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.0/MANIFEST.in
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5405 2023-07-26 09:24:11.736616 djangocms-aldryn-forms-7.0.0/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4239 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.0/README.rst
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.724616 djangocms-aldryn-forms-7.0.0/aldryn_forms/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       22 2023-07-26 09:23:55.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1119 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/action_backends.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      262 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/action_backends_base.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.724616 djangocms-aldryn-forms-7.0.0/aldryn_forms/admin/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      798 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/admin/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     7639 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/admin/base.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1844 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/admin/exporter.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4129 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/admin/forms.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3242 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/admin/views.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      126 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/apps.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      291 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/cms_apps.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    34277 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/cms_plugins.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      475 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/compat.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      265 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/constants.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.724616 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       24 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/__init__.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.724616 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       24 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6296 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/cms_plugins.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      897 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/helpers.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.728616 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/migrations/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2355 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/migrations/0001_initial.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1510 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/migrations/0002_form_plugin_add_missing_permission.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      487 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/migrations/0003_auto_20180206_1733.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      618 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/migrations/0004_auto_20190104_1242.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      460 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/migrations/0005_add_field_reply_to_email.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      502 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/migrations/0006_alter_emailnotification_id.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/migrations/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     7082 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/models.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2248 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/notification.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.720616 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/static/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.720616 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/static/email_notifications/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.728616 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/static/email_notifications/admin/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       75 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/static/email_notifications/admin/email-notifications.css
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15451 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/forms.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      749 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/helpers.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.720616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.720616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/cs/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.728616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15913 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/cs/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    16251 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/cs/LC_MESSAGES/django.po
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1124 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/cs/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1342 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/cs/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.720616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/de/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.728616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    11507 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    24568 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.720616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/en/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.728616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/en/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    11067 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    19715 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.720616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/fa/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.728616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/fa/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      369 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/fa/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15633 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/fa/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.720616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/fr/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.728616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    12258 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    20995 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.720616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/it/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.728616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/it/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      376 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15669 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.720616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/lt/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.728616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/lt/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      442 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/lt/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15764 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/lt/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.720616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/nl/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.728616 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    10146 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    19704 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/nl/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.732616 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15017 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0001_initial.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2076 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0002_auto_20151014_1631.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1867 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0003_auto_20151207_1038.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1518 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0004_auto_20151207_1825.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1612 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0005_auto_20160821_1026.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2897 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0006_auto_20160821_1039.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6228 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0007_auto_20170315_1421.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1294 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0008_auto_20170316_0845.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      719 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0009_auto_20171218_1049.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8860 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0010_auto_20171220_1733.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1020 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0011_auto_20180110_1300.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      588 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0012_auto_20190104_1242.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      699 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0013_add_field_is_enable_autofill_from_url_params.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4737 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0014_multiple_files_pload.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1349 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0015_fileupload_name_help_text.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8297 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0016_date_time_fields.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     7455 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0017_alter_datefieldplugin_cmsplugin_ptr_and_more.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       24 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    24229 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/models.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      555 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/signals.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.732616 djangocms-aldryn-forms-7.0.0/aldryn_forms/sizefield/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/sizefield/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      764 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/sizefield/models.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1999 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/sizefield/utils.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      904 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/sizefield/widgets.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.720616 djangocms-aldryn-forms-7.0.0/aldryn_forms/static/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.720616 djangocms-aldryn-forms-7.0.0/aldryn_forms/static/aldryn_forms/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.732616 djangocms-aldryn-forms-7.0.0/aldryn_forms/static/aldryn_forms/js/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4409 2023-07-26 07:42:08.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/static/aldryn_forms/js/main.js
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15270 2023-07-26 07:42:08.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/static/aldryn_forms/js/main.js.map
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.732616 djangocms-aldryn-forms-7.0.0/aldryn_forms/static/aldryn_forms/js/src/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8233 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/static/aldryn_forms/js/src/form.js
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1394 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/static/aldryn_forms/js/src/main.js
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.724616 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.720616 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/admin/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.732616 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/admin/aldryn_forms/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.732616 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/admin/aldryn_forms/display/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      207 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/admin/aldryn_forms/display/recipients.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      243 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/admin/aldryn_forms/display/submission_data.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1278 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/admin/aldryn_forms/export.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      465 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/admin/aldryn_forms/export_wizard.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.732616 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/admin/aldryn_forms/formsubmission/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      507 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/admin/aldryn_forms/formsubmission/change_list.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.732616 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      105 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/base.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.724616 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/email_notifications/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.732616 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/email_notifications/emails/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      409 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/email_notifications/emails/notification.body.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      387 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/email_notifications/emails/notification.body.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      222 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/email_notifications/emails/notification.subject.txt
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.732616 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/email_notifications/emails/themes/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       54 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/email_notifications/emails/themes/default.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       54 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/email_notifications/emails/themes/default.txt
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.732616 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/emails/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.732616 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/emails/includes/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      105 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/emails/includes/form_data.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       93 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/emails/includes/form_data.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      146 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/emails/notification.body.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      137 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/emails/notification.body.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       84 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/emails/notification.subject.txt
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.732616 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/emails/user/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      236 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/emails/user/notification.body.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      134 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/emails/user/notification.subject.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      799 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/field.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.736616 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fields/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fields/booleanfield.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fields/emailfield.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fields/filefield.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fields/hiddenfield.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fields/imagefield.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1521 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fields/multiplecheckboxselectfield.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fields/multipleselectfield.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fields/numberfield.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fields/phonefield.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fields/radioselectfield.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fields/selectfield.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fields/textareafield.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fields/textfield.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      326 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fieldset.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2780 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/form.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      131 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/send.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      139 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/submit_button.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.736616 djangocms-aldryn-forms-7.0.0/aldryn_forms/templatetags/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       24 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templatetags/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1104 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/templatetags/aldryn_forms_tags.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      151 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/urls.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3846 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/utils.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      985 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/validators.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1683 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/aldryn_forms/views.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.736616 djangocms-aldryn-forms-7.0.0/djangocms_aldryn_forms.egg-info/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5405 2023-07-26 09:24:11.000000 djangocms-aldryn-forms-7.0.0/djangocms_aldryn_forms.egg-info/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6410 2023-07-26 09:24:11.000000 djangocms-aldryn-forms-7.0.0/djangocms_aldryn_forms.egg-info/SOURCES.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-26 09:24:11.000000 djangocms-aldryn-forms-7.0.0/djangocms_aldryn_forms.egg-info/dependency_links.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-26 08:05:58.000000 djangocms-aldryn-forms-7.0.0/djangocms_aldryn_forms.egg-info/not-zip-safe
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      190 2023-07-26 09:24:11.000000 djangocms-aldryn-forms-7.0.0/djangocms_aldryn_forms.egg-info/requires.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       13 2023-07-26 09:24:11.000000 djangocms-aldryn-forms-7.0.0/djangocms_aldryn_forms.egg-info/top_level.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      632 2023-07-26 09:24:11.736616 djangocms-aldryn-forms-7.0.0/setup.cfg
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1740 2023-07-26 09:17:43.000000 djangocms-aldryn-forms-7.0.0/setup.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 09:24:11.736616 djangocms-aldryn-forms-7.0.0/tests/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4506 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/tests/test_cms_plugins.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6708 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/tests/test_models.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4212 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.0/tests/test_utils.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     7063 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.0/tests/test_views.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.929060 djangocms-aldryn-forms-7.0.1/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1474 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/LICENSE.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      265 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.1/MANIFEST.in
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5405 2023-07-31 13:29:06.929060 djangocms-aldryn-forms-7.0.1/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4239 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.1/README.rst
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.909060 djangocms-aldryn-forms-7.0.1/aldryn_forms/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       22 2023-07-31 13:28:41.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1119 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/action_backends.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      262 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/action_backends_base.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.909060 djangocms-aldryn-forms-7.0.1/aldryn_forms/admin/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      798 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/admin/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     7639 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/admin/base.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1844 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/admin/exporter.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4129 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/admin/forms.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3242 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/admin/views.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      126 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/apps.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      291 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/cms_apps.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    34444 2023-07-31 13:28:41.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/cms_plugins.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      475 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/compat.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      265 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/constants.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.909060 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       24 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/__init__.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.913060 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       24 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6296 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/cms_plugins.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      897 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/helpers.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.913060 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/migrations/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2355 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/migrations/0001_initial.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1510 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/migrations/0002_form_plugin_add_missing_permission.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      487 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/migrations/0003_auto_20180206_1733.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      618 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/migrations/0004_auto_20190104_1242.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      460 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/migrations/0005_add_field_reply_to_email.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      502 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/migrations/0006_alter_emailnotification_id.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/migrations/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     7082 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/models.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2248 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/notification.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.901060 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/static/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.901060 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/static/email_notifications/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.913060 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/static/email_notifications/admin/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       75 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/static/email_notifications/admin/email-notifications.css
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15451 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/forms.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      749 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/helpers.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.905060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.901060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/cs/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.913060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15913 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/cs/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    16251 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/cs/LC_MESSAGES/django.po
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1124 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/cs/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1342 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/cs/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.901060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/de/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.913060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    11507 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    24568 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.901060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/en/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.913060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    11067 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    19715 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.901060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/fa/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.917060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/fa/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      369 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/fa/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15633 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/fa/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.905060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/fr/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.917060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    12258 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    20995 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.905060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/it/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.917060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      376 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15669 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.905060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/lt/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.917060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/lt/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      442 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/lt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15764 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/lt/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.905060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/nl/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.917060 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    10146 2023-07-26 07:50:59.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    19704 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/nl/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.921060 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15017 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0001_initial.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2076 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0002_auto_20151014_1631.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1867 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0003_auto_20151207_1038.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1518 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0004_auto_20151207_1825.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1612 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0005_auto_20160821_1026.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2897 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0006_auto_20160821_1039.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6228 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0007_auto_20170315_1421.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1294 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0008_auto_20170316_0845.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      719 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0009_auto_20171218_1049.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8860 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0010_auto_20171220_1733.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1020 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0011_auto_20180110_1300.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      588 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0012_auto_20190104_1242.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      699 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0013_add_field_is_enable_autofill_from_url_params.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4737 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0014_multiple_files_pload.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1349 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0015_fileupload_name_help_text.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8297 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0016_date_time_fields.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     7455 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0017_alter_datefieldplugin_cmsplugin_ptr_and_more.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       24 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    24229 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/models.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      555 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/signals.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.921060 djangocms-aldryn-forms-7.0.1/aldryn_forms/sizefield/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/sizefield/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      764 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/sizefield/models.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1999 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/sizefield/utils.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      904 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/sizefield/widgets.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.905060 djangocms-aldryn-forms-7.0.1/aldryn_forms/static/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.905060 djangocms-aldryn-forms-7.0.1/aldryn_forms/static/aldryn_forms/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.921060 djangocms-aldryn-forms-7.0.1/aldryn_forms/static/aldryn_forms/js/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4409 2023-07-26 07:42:08.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/static/aldryn_forms/js/main.js
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    15270 2023-07-26 07:42:08.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/static/aldryn_forms/js/main.js.map
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.921060 djangocms-aldryn-forms-7.0.1/aldryn_forms/static/aldryn_forms/js/src/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8233 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/static/aldryn_forms/js/src/form.js
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1394 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/static/aldryn_forms/js/src/main.js
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.905060 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.905060 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/admin/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.921060 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/admin/aldryn_forms/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.921060 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/admin/aldryn_forms/display/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      207 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/admin/aldryn_forms/display/recipients.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      243 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/admin/aldryn_forms/display/submission_data.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1278 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/admin/aldryn_forms/export.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      465 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/admin/aldryn_forms/export_wizard.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.921060 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/admin/aldryn_forms/formsubmission/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      507 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/admin/aldryn_forms/formsubmission/change_list.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.921060 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      105 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/base.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.905060 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/email_notifications/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.925060 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/email_notifications/emails/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      409 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/email_notifications/emails/notification.body.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      387 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/email_notifications/emails/notification.body.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      222 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/email_notifications/emails/notification.subject.txt
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.925060 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/email_notifications/emails/themes/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       54 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/email_notifications/emails/themes/default.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       54 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/email_notifications/emails/themes/default.txt
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.925060 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/emails/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.925060 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/emails/includes/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      105 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/emails/includes/form_data.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       93 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/emails/includes/form_data.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      146 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/emails/notification.body.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      137 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/emails/notification.body.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       84 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/emails/notification.subject.txt
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.925060 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/emails/user/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      236 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/emails/user/notification.body.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      134 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/emails/user/notification.subject.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      799 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/field.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.925060 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fields/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fields/booleanfield.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fields/emailfield.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fields/filefield.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fields/hiddenfield.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fields/imagefield.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1521 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fields/multiplecheckboxselectfield.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fields/multipleselectfield.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fields/numberfield.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fields/phonefield.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fields/radioselectfield.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fields/selectfield.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fields/textareafield.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       40 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fields/textfield.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      326 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fieldset.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2780 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/form.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      131 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/send.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      139 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/submit_button.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.925060 djangocms-aldryn-forms-7.0.1/aldryn_forms/templatetags/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       24 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templatetags/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1104 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/templatetags/aldryn_forms_tags.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      151 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/urls.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3846 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/utils.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      985 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/validators.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1683 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/aldryn_forms/views.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.925060 djangocms-aldryn-forms-7.0.1/djangocms_aldryn_forms.egg-info/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5405 2023-07-31 13:29:06.000000 djangocms-aldryn-forms-7.0.1/djangocms_aldryn_forms.egg-info/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6410 2023-07-31 13:29:06.000000 djangocms-aldryn-forms-7.0.1/djangocms_aldryn_forms.egg-info/SOURCES.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-31 13:29:06.000000 djangocms-aldryn-forms-7.0.1/djangocms_aldryn_forms.egg-info/dependency_links.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-26 08:05:58.000000 djangocms-aldryn-forms-7.0.1/djangocms_aldryn_forms.egg-info/not-zip-safe
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      190 2023-07-31 13:29:06.000000 djangocms-aldryn-forms-7.0.1/djangocms_aldryn_forms.egg-info/requires.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       13 2023-07-31 13:29:06.000000 djangocms-aldryn-forms-7.0.1/djangocms_aldryn_forms.egg-info/top_level.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      632 2023-07-31 13:29:06.929060 djangocms-aldryn-forms-7.0.1/setup.cfg
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1740 2023-07-26 09:17:43.000000 djangocms-aldryn-forms-7.0.1/setup.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 13:29:06.929060 djangocms-aldryn-forms-7.0.1/tests/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4506 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/tests/test_cms_plugins.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6708 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/tests/test_models.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4212 2023-07-26 09:18:22.000000 djangocms-aldryn-forms-7.0.1/tests/test_utils.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     7063 2023-07-26 07:35:03.000000 djangocms-aldryn-forms-7.0.1/tests/test_views.py
```

### Comparing `djangocms-aldryn-forms-7.0.0/LICENSE.txt` & `djangocms-aldryn-forms-7.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/PKG-INFO` & `djangocms-aldryn-forms-7.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-aldryn-forms
-Version: 7.0.0
+Version: 7.0.1
 Summary: Create forms and embed them on CMS pages.
 Home-page: https://github.com/CZ-NIC/djangocms-aldryn-forms
 Author: Divio AG
 Author-email: info@divio.ch
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `djangocms-aldryn-forms-7.0.0/README.rst` & `djangocms-aldryn-forms-7.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/action_backends.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/action_backends.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/admin/__init__.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/admin/base.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/admin/base.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/admin/exporter.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/admin/exporter.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/admin/forms.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/admin/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/admin/views.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/admin/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/cms_plugins.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/cms_plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 from typing import Dict
 
 from django import forms
+from django.apps import apps
 from django.conf import settings
 from django.contrib import messages
 from django.contrib.admin import TabularInline
 from django.core.validators import MinLengthValidator
 from django.db.models import query
 from django.template.loader import select_template
 from django.utils.safestring import mark_safe
@@ -992,14 +993,16 @@
             if opt.default_value:
                 kwargs['initial'] = opt.pk
                 break
         return kwargs
 
 
 try:
+    if not apps.is_installed("captcha"):  # django-simple-captcha
+        raise ImportError('Module "captcha" is not in INSTALLED_APPS.')
     from captcha.fields import CaptchaField, CaptchaTextInput
 except ImportError:
     pass
 else:
     # Don't like doing this. But we shouldn't force captcha.
     class CaptchaField(Field):
         name = _('Captcha Field')
```

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/cms_plugins.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/helpers.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/migrations/0001_initial.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/migrations/0002_form_plugin_add_missing_permission.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/migrations/0002_form_plugin_add_missing_permission.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/migrations/0004_auto_20190104_1242.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/migrations/0004_auto_20190104_1242.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/models.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/contrib/email_notifications/notification.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/contrib/email_notifications/notification.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/forms.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/helpers.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/cs/LC_MESSAGES/django.mo` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/cs/LC_MESSAGES/django.po` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/cs/LC_MESSAGES/djangojs.mo` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/cs/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/cs/LC_MESSAGES/djangojs.po` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/cs/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/de/LC_MESSAGES/django.mo` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/de/LC_MESSAGES/django.po` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/en/LC_MESSAGES/django.mo` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/en/LC_MESSAGES/django.po` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/fa/LC_MESSAGES/django.po` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/fr/LC_MESSAGES/django.mo` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/fr/LC_MESSAGES/django.po` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/it/LC_MESSAGES/django.po` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/lt/LC_MESSAGES/django.po` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/nl/LC_MESSAGES/django.mo` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/locale/nl/LC_MESSAGES/django.po` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0001_initial.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0002_auto_20151014_1631.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0002_auto_20151014_1631.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0003_auto_20151207_1038.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0003_auto_20151207_1038.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0004_auto_20151207_1825.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0004_auto_20151207_1825.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0005_auto_20160821_1026.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0005_auto_20160821_1026.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0006_auto_20160821_1039.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0006_auto_20160821_1039.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0007_auto_20170315_1421.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0007_auto_20170315_1421.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0008_auto_20170316_0845.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0008_auto_20170316_0845.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0009_auto_20171218_1049.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0009_auto_20171218_1049.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0010_auto_20171220_1733.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0010_auto_20171220_1733.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0011_auto_20180110_1300.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0011_auto_20180110_1300.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0012_auto_20190104_1242.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0012_auto_20190104_1242.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0013_add_field_is_enable_autofill_from_url_params.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0013_add_field_is_enable_autofill_from_url_params.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0014_multiple_files_pload.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0014_multiple_files_pload.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0015_fileupload_name_help_text.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0015_fileupload_name_help_text.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0016_date_time_fields.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0016_date_time_fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/migrations/0017_alter_datefieldplugin_cmsplugin_ptr_and_more.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/migrations/0017_alter_datefieldplugin_cmsplugin_ptr_and_more.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/models.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/signals.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/signals.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/sizefield/models.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/sizefield/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/sizefield/utils.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/sizefield/utils.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/sizefield/widgets.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/sizefield/widgets.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/static/aldryn_forms/js/main.js` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/static/aldryn_forms/js/main.js`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/static/aldryn_forms/js/main.js.map` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/static/aldryn_forms/js/main.js.map`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/static/aldryn_forms/js/src/form.js` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/static/aldryn_forms/js/src/form.js`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/static/aldryn_forms/js/src/main.js` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/static/aldryn_forms/js/src/main.js`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/admin/aldryn_forms/export.html` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/admin/aldryn_forms/export.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/field.html` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/field.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/fields/multiplecheckboxselectfield.html` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/fields/multiplecheckboxselectfield.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/templates/aldryn_forms/form.html` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/templates/aldryn_forms/form.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/templatetags/aldryn_forms_tags.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/templatetags/aldryn_forms_tags.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/utils.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/utils.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/validators.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/validators.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/aldryn_forms/views.py` & `djangocms-aldryn-forms-7.0.1/aldryn_forms/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/djangocms_aldryn_forms.egg-info/PKG-INFO` & `djangocms-aldryn-forms-7.0.1/djangocms_aldryn_forms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-aldryn-forms
-Version: 7.0.0
+Version: 7.0.1
 Summary: Create forms and embed them on CMS pages.
 Home-page: https://github.com/CZ-NIC/djangocms-aldryn-forms
 Author: Divio AG
 Author-email: info@divio.ch
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `djangocms-aldryn-forms-7.0.0/djangocms_aldryn_forms.egg-info/SOURCES.txt` & `djangocms-aldryn-forms-7.0.1/djangocms_aldryn_forms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/setup.cfg` & `djangocms-aldryn-forms-7.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/setup.py` & `djangocms-aldryn-forms-7.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/tests/test_cms_plugins.py` & `djangocms-aldryn-forms-7.0.1/tests/test_cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/tests/test_models.py` & `djangocms-aldryn-forms-7.0.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/tests/test_utils.py` & `djangocms-aldryn-forms-7.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-forms-7.0.0/tests/test_views.py` & `djangocms-aldryn-forms-7.0.1/tests/test_views.py`

 * *Files identical despite different names*

