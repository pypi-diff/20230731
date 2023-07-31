# Comparing `tmp/omic-django-herald-0.2.1.20.tar.gz` & `tmp/omic-django-herald-0.2.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\omic-django-herald-0.2.1.20.tar", last modified: Fri Apr  2 11:47:10 2021, max compression
+gzip compressed data, was "omic-django-herald-0.2.1.21.tar", last modified: Mon Jul 31 02:43:06 2023, max compression
```

## Comparing `omic-django-herald-0.2.1.20.tar` & `omic-django-herald-0.2.1.21.tar`

### file list

```diff
@@ -1,60 +1,70 @@
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:10.000000 omic-django-herald-0.2.1.20/
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:09.000000 omic-django-herald-0.2.1.20/herald/
--rw-rw-rw-   0        0        0     2911 2021-03-09 06:38:50.000000 omic-django-herald-0.2.1.20/herald/admin.py
--rw-rw-rw-   0        0        0     1419 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/apps.py
--rw-rw-rw-   0        0        0    14608 2021-04-02 10:39:28.000000 omic-django-herald-0.2.1.20/herald/base.py
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:09.000000 omic-django-herald-0.2.1.20/herald/clients/
--rw-rw-rw-   0        0        0     1817 2021-04-02 10:39:28.000000 omic-django-herald-0.2.1.20/herald/clients/msg91.py
--rw-rw-rw-   0        0        0        0 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/clients/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:09.000000 omic-django-herald-0.2.1.20/herald/contrib/
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:10.000000 omic-django-herald-0.2.1.20/herald/contrib/auth/
--rw-rw-rw-   0        0        0      144 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/contrib/auth/apps.py
--rw-rw-rw-   0        0        0     1751 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/contrib/auth/forms.py
--rw-rw-rw-   0        0        0     3395 2021-03-09 06:38:50.000000 omic-django-herald-0.2.1.20/herald/contrib/auth/notifications.py
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:09.000000 omic-django-herald-0.2.1.20/herald/contrib/auth/templates/
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:09.000000 omic-django-herald-0.2.1.20/herald/contrib/auth/templates/herald/
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:10.000000 omic-django-herald-0.2.1.20/herald/contrib/auth/templates/herald/html/
--rw-rw-rw-   0        0        0      260 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/contrib/auth/templates/herald/html/password_reset.html
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:10.000000 omic-django-herald-0.2.1.20/herald/contrib/auth/templates/herald/text/
--rw-rw-rw-   0        0        0      151 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/contrib/auth/templates/herald/text/password_reset.txt
--rw-rw-rw-   0        0        0       66 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/contrib/auth/__init__.py
--rw-rw-rw-   0        0        0        0 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:10.000000 omic-django-herald-0.2.1.20/herald/management/
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:10.000000 omic-django-herald-0.2.1.20/herald/management/commands/
--rw-rw-rw-   0        0        0     1246 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/management/commands/delnotifs.py
--rw-rw-rw-   0        0        0        0 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/management/commands/__init__.py
--rw-rw-rw-   0        0        0        0 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/management/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:10.000000 omic-django-herald-0.2.1.20/herald/migrations/
--rw-rw-rw-   0        0        0     1276 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      478 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/migrations/0002_sentnotification_attachments.py
--rw-rw-rw-   0        0        0     1876 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/migrations/0003_auto_20170830_1617.py
--rw-rw-rw-   0        0        0      493 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/migrations/0004_auto_20171009_0906.py
--rw-rw-rw-   0        0        0      629 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/migrations/0005_auto_20180516_1755.py
--rw-rw-rw-   0        0        0      635 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/migrations/0006_auto_20190503_0625.py
--rw-rw-rw-   0        0        0      793 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/migrations/0007_auto_20190503_0832.py
--rw-rw-rw-   0        0        0      424 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/migrations/0008_auto_20190503_1320.py
--rw-rw-rw-   0        0        0      442 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/migrations/0009_sentnotification_receiver_doctor_profile_id.py
--rw-rw-rw-   0        0        0      670 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/migrations/0010_auto_20190904_0315.py
--rw-rw-rw-   0        0        0      525 2021-04-02 11:20:16.000000 omic-django-herald-0.2.1.20/herald/migrations/0011_sentnotification_dlt_template_id.py
--rw-rw-rw-   0        0        0        0 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/migrations/__init__.py
--rw-rw-rw-   0        0        0     3837 2021-04-02 10:39:28.000000 omic-django-herald-0.2.1.20/herald/models.py
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:09.000000 omic-django-herald-0.2.1.20/herald/templates/
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:09.000000 omic-django-herald-0.2.1.20/herald/templates/herald/
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:10.000000 omic-django-herald-0.2.1.20/herald/templates/herald/test/
--rw-rw-rw-   0        0        0      575 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/herald/templates/herald/test/notification_list.html
--rw-rw-rw-   0        0        0     2220 2021-04-02 10:39:28.000000 omic-django-herald-0.2.1.20/herald/text_notification.py
--rw-rw-rw-   0        0        0      328 2021-03-09 06:38:50.000000 omic-django-herald-0.2.1.20/herald/urls.py
--rw-rw-rw-   0        0        0     1536 2021-03-09 06:38:50.000000 omic-django-herald-0.2.1.20/herald/views.py
--rw-rw-rw-   0        0        0     1366 2021-03-09 06:38:50.000000 omic-django-herald-0.2.1.20/herald/__init__.py
--rw-rw-rw-   0        0        0     1098 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/LICENSE
--rw-rw-rw-   0        0        0      132 2021-03-09 06:30:22.000000 omic-django-herald-0.2.1.20/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2021-04-02 11:47:10.000000 omic-django-herald-0.2.1.20/omic_django_herald.egg-info/
--rw-rw-rw-   0        0        0        1 2021-04-02 11:47:09.000000 omic-django-herald-0.2.1.20/omic_django_herald.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    18100 2021-04-02 11:47:09.000000 omic-django-herald-0.2.1.20/omic_django_herald.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      106 2021-04-02 11:47:09.000000 omic-django-herald-0.2.1.20/omic_django_herald.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1449 2021-04-02 11:47:09.000000 omic-django-herald-0.2.1.20/omic_django_herald.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2021-04-02 11:47:09.000000 omic-django-herald-0.2.1.20/omic_django_herald.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18100 2021-04-02 11:47:10.000000 omic-django-herald-0.2.1.20/PKG-INFO
--rw-rw-rw-   0        0        0    14066 2021-04-02 11:44:46.000000 omic-django-herald-0.2.1.20/README.md
--rw-rw-rw-   0        0        0      138 2021-04-02 11:47:10.000000 omic-django-herald-0.2.1.20/setup.cfg
--rw-rw-rw-   0        0        0     1927 2021-04-02 11:46:38.000000 omic-django-herald-0.2.1.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.730261 omic-django-herald-0.2.1.21/
+-rw-rw-rw-   0        0        0     1098 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/LICENSE
+-rw-rw-rw-   0        0        0      132 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/MANIFEST.in
+-rw-rw-rw-   0        0        0    15101 2023-07-31 02:43:06.731707 omic-django-herald-0.2.1.21/PKG-INFO
+-rw-rw-rw-   0        0        0    14084 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.530662 omic-django-herald-0.2.1.21/herald/
+-rw-rw-rw-   0        0        0     1317 2023-07-31 02:41:29.000000 omic-django-herald-0.2.1.21/herald/__init__.py
+-rw-rw-rw-   0        0        0     2914 2023-07-31 02:41:29.000000 omic-django-herald-0.2.1.21/herald/admin.py
+-rw-rw-rw-   0        0        0     1419 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/apps.py
+-rw-rw-rw-   0        0        0    14608 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/base.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.539342 omic-django-herald-0.2.1.21/herald/clients/
+-rw-rw-rw-   0        0        0        0 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/clients/__init__.py
+-rw-rw-rw-   0        0        0     1817 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/clients/msg91.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.543718 omic-django-herald-0.2.1.21/herald/contrib/
+-rw-rw-rw-   0        0        0        0 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.573164 omic-django-herald-0.2.1.21/herald/contrib/auth/
+-rw-rw-rw-   0        0        0        0 2023-07-31 02:41:29.000000 omic-django-herald-0.2.1.21/herald/contrib/auth/__init__.py
+-rw-rw-rw-   0        0        0      144 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/contrib/auth/apps.py
+-rw-rw-rw-   0        0        0     1751 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/contrib/auth/forms.py
+-rw-rw-rw-   0        0        0     3393 2023-07-31 02:41:29.000000 omic-django-herald-0.2.1.21/herald/contrib/auth/notifications.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.415156 omic-django-herald-0.2.1.21/herald/contrib/auth/templates/
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.416207 omic-django-herald-0.2.1.21/herald/contrib/auth/templates/herald/
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.617388 omic-django-herald-0.2.1.21/herald/contrib/auth/templates/herald/html/
+-rw-rw-rw-   0        0        0      260 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/contrib/auth/templates/herald/html/password_reset.html
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.620635 omic-django-herald-0.2.1.21/herald/contrib/auth/templates/herald/text/
+-rw-rw-rw-   0        0        0      151 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/contrib/auth/templates/herald/text/password_reset.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.621637 omic-django-herald-0.2.1.21/herald/management/
+-rw-rw-rw-   0        0        0        0 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.625635 omic-django-herald-0.2.1.21/herald/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1246 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/management/commands/delnotifs.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.694764 omic-django-herald-0.2.1.21/herald/migrations/
+-rw-rw-rw-   0        0        0     1276 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      478 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/migrations/0002_sentnotification_attachments.py
+-rw-rw-rw-   0        0        0     1876 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/migrations/0003_auto_20170830_1617.py
+-rw-rw-rw-   0        0        0      493 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/migrations/0004_auto_20171009_0906.py
+-rw-rw-rw-   0        0        0      629 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/migrations/0005_auto_20180516_1755.py
+-rw-rw-rw-   0        0        0      635 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/migrations/0006_auto_20190503_0625.py
+-rw-rw-rw-   0        0        0      793 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/migrations/0007_auto_20190503_0832.py
+-rw-rw-rw-   0        0        0      424 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/migrations/0008_auto_20190503_1320.py
+-rw-rw-rw-   0        0        0      442 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/migrations/0009_sentnotification_receiver_doctor_profile_id.py
+-rw-rw-rw-   0        0        0      670 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/migrations/0010_auto_20190904_0315.py
+-rw-rw-rw-   0        0        0      525 2023-07-31 02:41:17.000000 omic-django-herald-0.2.1.21/herald/migrations/0011_sentnotification_dlt_template_id.py
+-rw-rw-rw-   0        0        0        0 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3837 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/models.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.419358 omic-django-herald-0.2.1.21/herald/templates/
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.419358 omic-django-herald-0.2.1.21/herald/templates/herald/
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.696763 omic-django-herald-0.2.1.21/herald/templates/herald/test/
+-rw-rw-rw-   0        0        0      575 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/templates/herald/test/notification_list.html
+-rw-rw-rw-   0        0        0     2220 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/text_notification.py
+-rw-rw-rw-   0        0        0      335 2023-07-31 02:41:29.000000 omic-django-herald-0.2.1.21/herald/urls.py
+-rw-rw-rw-   0        0        0     1536 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/herald/views.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.704764 omic-django-herald-0.2.1.21/omic_django_herald.egg-info/
+-rw-rw-rw-   0        0        0    15101 2023-07-31 02:43:06.000000 omic-django-herald-0.2.1.21/omic_django_herald.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1664 2023-07-31 02:43:06.000000 omic-django-herald-0.2.1.21/omic_django_herald.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 02:43:06.000000 omic-django-herald-0.2.1.21/omic_django_herald.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-07-31 02:43:06.000000 omic-django-herald-0.2.1.21/omic_django_herald.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-31 02:43:06.000000 omic-django-herald-0.2.1.21/omic_django_herald.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      138 2023-07-31 02:43:06.732760 omic-django-herald-0.2.1.21/setup.cfg
+-rw-rw-rw-   0        0        0     1927 2023-07-31 02:42:18.000000 omic-django-herald-0.2.1.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:43:06.728981 omic-django-herald-0.2.1.21/tests/
+-rw-rw-rw-   0        0        0     2268 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/tests/test_admin.py
+-rw-rw-rw-   0        0        0     3360 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/tests/test_commands.py
+-rw-rw-rw-   0        0        0     1065 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/tests/test_contrib_auth.py
+-rw-rw-rw-   0        0        0     1012 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/tests/test_init.py
+-rw-rw-rw-   0        0        0      375 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/tests/test_migrations.py
+-rw-rw-rw-   0        0        0     1584 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/tests/test_models.py
+-rw-rw-rw-   0        0        0    13933 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/tests/test_notifications.py
+-rw-rw-rw-   0        0        0     2094 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/tests/test_usernotifications.py
+-rw-rw-rw-   0        0        0      750 2023-07-31 02:23:47.000000 omic-django-herald-0.2.1.21/tests/test_views.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `omic-django-herald-0.2.1.20/herald/admin.py` & `omic-django-herald-0.2.1.21/herald/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Admin for notifications
 """
 
 from functools import update_wrapper
 
-from django.conf.urls import url
+from django.urls import re_path
 from django.contrib import admin, messages
 from django.contrib.admin.options import csrf_protect_m
 from django.contrib.admin.utils import unquote
 from django.utils.safestring import mark_safe
 from django.urls import reverse
 
 from .models import SentNotification, Notification
@@ -55,15 +55,15 @@
                 """
                 return self.admin_site.admin_view(view)(*args, **kwargs)
             return update_wrapper(wrapper, view)
 
         info = opts.app_label, opts.model_name
 
         return [
-            url(r'^(.+)/resend/$', wrap(self.resend_view), name='%s_%s_resend' % info),
+            re_path(r'^(.+)/resend/$', wrap(self.resend_view), name='%s_%s_resend' % info),
         ] + urls
 
     @csrf_protect_m
     def resend_view(self, request, object_id, extra_context=None):  # pylint: disable=W0613
         """
         View that re-sends the notification
         """
```

### Comparing `omic-django-herald-0.2.1.20/herald/apps.py` & `omic-django-herald-0.2.1.21/herald/apps.py`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/base.py` & `omic-django-herald-0.2.1.21/herald/base.py`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/clients/msg91.py` & `omic-django-herald-0.2.1.21/herald/clients/msg91.py`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/contrib/auth/forms.py` & `omic-django-herald-0.2.1.21/herald/contrib/auth/forms.py`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/contrib/auth/notifications.py` & `omic-django-herald-0.2.1.21/herald/contrib/auth/notifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Herald notifications for working with django.contrib.auth
 """
 
 from django.contrib.auth import get_user_model
 from django.contrib.auth.tokens import default_token_generator
 from django.contrib.sites.models import Site
 from django.template import loader
-from django.utils.encoding import force_bytes, force_text
+from django.utils.encoding import force_bytes, force_str
 from django.utils.http import urlsafe_base64_encode
 from django.urls import reverse
 
 from ... import registry
 from ...base import EmailNotification
 
 
@@ -41,15 +41,15 @@
 
         if not self.site_name or self.domain:
             current_site = Site.objects.get_current()
             self.site_name = current_site.name
             self.domain = current_site.domain
 
         protocol = 'https' if self.use_https else 'http'
-        uid = force_text(urlsafe_base64_encode(force_bytes(self.user.pk)))
+        uid = force_str(urlsafe_base64_encode(force_bytes(self.user.pk)))
         token = self.token_generator.make_token(self.user)
 
         context.update({
             'full_reset_url': '{}://{}{}'.format(
                 protocol,
                 self.domain,
                 reverse('password_reset_confirm', kwargs={'uidb64': uid, 'token': token})
```

### Comparing `omic-django-herald-0.2.1.20/herald/management/commands/delnotifs.py` & `omic-django-herald-0.2.1.21/herald/management/commands/delnotifs.py`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/migrations/0001_initial.py` & `omic-django-herald-0.2.1.21/herald/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/migrations/0003_auto_20170830_1617.py` & `omic-django-herald-0.2.1.21/herald/migrations/0003_auto_20170830_1617.py`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/migrations/0005_auto_20180516_1755.py` & `omic-django-herald-0.2.1.21/herald/migrations/0005_auto_20180516_1755.py`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/migrations/0006_auto_20190503_0625.py` & `omic-django-herald-0.2.1.21/herald/migrations/0006_auto_20190503_0625.py`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/migrations/0007_auto_20190503_0832.py` & `omic-django-herald-0.2.1.21/herald/migrations/0007_auto_20190503_0832.py`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/migrations/0010_auto_20190904_0315.py` & `omic-django-herald-0.2.1.21/herald/migrations/0010_auto_20190904_0315.py`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/migrations/0011_sentnotification_dlt_template_id.py` & `omic-django-herald-0.2.1.21/herald/migrations/0011_sentnotification_dlt_template_id.py`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/models.py` & `omic-django-herald-0.2.1.21/herald/models.py`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/templates/herald/test/notification_list.html` & `omic-django-herald-0.2.1.21/herald/templates/herald/test/notification_list.html`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/text_notification.py` & `omic-django-herald-0.2.1.21/herald/text_notification.py`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/views.py` & `omic-django-herald-0.2.1.21/herald/views.py`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/herald/__init__.py` & `omic-django-herald-0.2.1.21/herald/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Notification classes. Used for sending texts and emails
 """
 __version__ = '0.2.1'
 
-default_app_config = 'herald.apps.HeraldConfig'
 
 
 class NotificationRegistry(object):
     """
     Stores the notification classes that get registered.
     """
```

### Comparing `omic-django-herald-0.2.1.20/LICENSE` & `omic-django-herald-0.2.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `omic-django-herald-0.2.1.20/omic_django_herald.egg-info/PKG-INFO` & `omic-django-herald-0.2.1.21/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,402 +1,402 @@
 Metadata-Version: 2.1
 Name: omic-django-herald
-Version: 0.2.1.20
+Version: 0.2.1.21
 Summary: Django library for separating the message content from transmission method
 Home-page: https://github.com/vvkvivekl/omic-django-herald/
-Author: Omic Health
-Author-email: info@omic.health
+Download-URL: https://github.com/vvkvivekl/omic-django-herald/tarball/0.2.1.21
+Author: Pred Health
+Author-email: info@pred.health
 License: MIT
-Download-URL: https://github.com/vvkvivekl/omic-django-herald/tarball/0.2.1.20
-Description: # django-herald-msg91
-        
-        [![Latest PyPI version](https://badge.fury.io/py/omic-django-herald.svg)](https://pypi.python.org/pypi/omic-django-herald)
-        
-        Forked from: [django-herald](https://github.com/worthwhile/django-herald/tree/a0da436e003829b72b87b2bcfdc4d0e5e4449adb)
-        
-        I've added support for sending messages using the [msg91](https://msg91.com/) platform backend for sending text messages (SMS) in India.
-        
-        Please go over the installation steps mentioned in the [original ReadMe](https://github.com/worthwhile/django-herald/tree/a0da436e003829b72b87b2bcfdc4d0e5e4449adb)
-        
-        # Differences in setup:
-        
-        ### Installation
-        `pip install omic-django-herald`
-        
-        ### Settings
-        In your Django settings file, add the following settings:
-        ```
-        MSG91_TRANSACTIONAL_SENDER_ID = 'SOCKET'
-        MSG91_AUTHKEY = '228352HGNg5dF65b57672G'
-        ```
-        Replace 'SOCKET' with any 6 alphebet series that you want in the user's text message inbox.
-        Replace '228352HGNg5dF65b57672G' with your authkey from your [msg91](https://msg91.com/) account
-        
-        **Note:** it'll show up as BT-SOCKET or similar...the first two alphabets indicate the text message provider and the region and is not controllable.
-        
-        ### Usage
-        ```python
-        from herald import registry
-        from herald.text_notification import Msg91TextNotification
-        
-        @registry.register_decorator()
-        class InvitationMessage(Msg91TextNotification):
-            template_name = 'invitation_message'  # name of template, without extension
-        
-            def __init__(self, to_number, invited_by_user, user_full_name, invitation_url):
-                # set context for the template rendering
-                self.context = {
-                    'invited_by_user': invited_by_user,
-                    'user_full_name': user_full_name,
-                    'invitation_url': invitation_url
-                }
-        
-                self.to_number = to_number
-        ```
-        
-        # Original ReadMe
-        [![Logo](https://github.com/worthwhile/django-herald/raw/master/logo.png)](https://github.com/worthwhile/django-herald)
-        
-        A Django messaging library that features:
-        
-        - Class-based declaration and registry approach, like Django Admin
-        - Supports multiple transmission methods (Email, SMS, Slack, etc) per message
-        - Browser-based previewing of messages
-        - Maintains a history of messaging sending attempts and can view these messages
-        - Disabling notifications per user
-        
-        # Python/Django Support
-        
-        We try to make herald support all versions of django that django supports + all versions in between.
-        
-        For python, herald supports all versions of python that the above versions of django support.
-        
-        So as of herald v0.2 we support django 1.11, 2.0, 2.1, and 2.2, and python 2.7, 3.4, 3.5, 3.6, and 3.7.
-        
-        ## What version of herald do I need if I have django x and python x?
-        
-        If the django/python version combination has a `---` in the table, it is not guaranteed to be supported.
-        
-        |                   | py 2.7   | py 3.3   | py 3.4   | py 3.5   | py 3.6   | py 3.7   |
-        |:-----------------:|:--------:|:--------:|:--------:|:--------:|:--------:|:--------:|
-        | **dj 1.8**        | <0.2     | <0.2     | <0.2     | <0.2     | ---      | ---      |
-        | **dj 1.9 - 1.10** | <0.2     | ---      | <0.2     | <0.2     | ---      | ---      |
-        | **dj 1.11**       | \>=0.1.5 | ---      | \>=0.1.5 | \>=0.1.5 | \>=0.1.5 | ---      |
-        | **dj 2.0**        | ---      | ---      | \>=0.1.5 | \>=0.1.5 | \>=0.1.5 | \>=0.2   |
-        | **dj 2.1**        | ---      | ---      | ---      | \>=0.2   | \>=0.2   | \>=0.2   |
-        | **dj 2.2**        | ---      | ---      | ---      | \>=0.2   | \>=0.2   | \>=0.2   |
-        
-        
-        # Installation
-        
-        1. `pip install django-herald`
-        2. Add `herald` and `django.contrib.sites` to `INSTALLED_APPS`.
-        3. Add herald's URLS:
-        
-            ```python
-            if settings.DEBUG:
-                urlpatterns = [
-                    url(r'^herald/', include('herald.urls')),
-                ] + urlpatterns
-            ```
-        
-        # Usage
-        
-        1. Create a `notifications.py` file in any django app. This is where your notification classes will live. Add a class like this:
-        
-        ```python
-        from herald import registry
-        from herald.base import EmailNotification
-        
-        
-        class WelcomeEmail(EmailNotification):  # extend from EmailNotification for emails
-            template_name = 'welcome_email'  # name of template, without extension
-            subject = 'Welcome'  # subject of email
-        
-            def __init__(self, user):  # optionally customize the initialization
-                self.context = {'user': user}  # set context for the template rendering
-                self.to_emails = [user.email]  # set list of emails to send to
-        
-            @staticmethod
-            def get_demo_args():  # define a static method to return list of args needed to initialize class for testing
-                from users.models import User
-                return [User.objects.order_by('?')[0]]
-        
-        registry.register(WelcomeEmail)  # finally, register your notification class
-        
-        # Alternatively, a class decorator can be used to register the notification:
-        
-        @registry.register_decorator()
-        class WelcomeEmail(EmailNotification):
-            ...
-        ```
-        
-        
-        2. Create templates for rendering the email using this file structure:
-        
-                templates/
-                    herald/
-                        text/
-                            welcome_email.txt
-                        html/
-                            welcome_email.html
-        
-        3. Test how your email looks by navigating to `/herald/`.
-        
-        4. Send your email wherever you need in your code:
-        
-                WelcomeEmail(user).send()
-        
-        5. View the sent emails in django admin and even be able to resend it.
-        
-        ## Email options
-        
-        The following options can be set on the email notification class. For Example:
-        
-        ```
-        class WelcomeEmail(EmailNotification):
-            cc = ['test@example.com']
-        ```
-        
-        - `from_email`: (`str`, default: `settings.DEFAULT_FROM_EMAIL`) email address of sender
-        - `subject`: (`str`, default: ) email subject
-        - `to_emails`: (`List[str]`, default: `None`) list of email strings to send to
-        - `bcc`: (`List[str]`, default: `None`) list of email strings to send as bcc
-        - `cc`: (`List[str]`, default: `None`) list of email strings to send as cc
-        - `headers`: (`dict`, default: `None`) extra headers to be passed along to the `EmailMultiAlternatives` object
-        - `reply_to`: (`List[str]`, default: `None`) list of email strings to send as the Reply-To emails
-        - `attachments`: (`list`) list of attachments. See "Email Attachments" below for more info
-            
-            
-        ## Automatically Deleting Old Notifications
-        
-        Herald can automatically delete old notifications whenever a new notification is sent.
-        
-        To enable this, set the `HERALD_NOTIFICATION_RETENTION_TIME` setting to a timedelta instance.
-        
-        For example:
-        
-        ```
-        HERALD_NOTIFICATION_RETENTION_TIME = timedelta(weeks=8)
-        ```
-        
-        Will delete all notifications older than 8 weeks every time a new notification is sent.
-        
-        ## Manually Deleting Old Notifications
-        
-        The `delnotifs` command is useful for purging the notification history.
-        
-        The default usage will delete everything from sent during today:
-        
-        ```bash
-        python manage.py delnotifs
-        ```
-        
-        However, you can also pass arguments for `start` or `end` dates. `end` is up to, but not including that date.
-        
-        ```bash
-        python manage.py delnotifs --start='2016-01-01' --end='2016-01-10'
-        ```
-        
-        
-        ## Asynchronous Email Sending
-        
-        If you are sending slightly different emails to a large number of people, it might take quite a while to process. By default, Django will process this all synchronously. For asynchronous support, we recommend django-celery-email. It is very straightfoward to setup and integrate: https://github.com/pmclanahan/django-celery-email
-        
-        
-        ## herald.contrib.auth
-        
-        Django has built-in support for sending password reset emails. If you would like to send those emails using herald, you can use the notification class in herald.contrib.auth.
-        
-        First, add `herald.contrib.auth` to `INSTALLED_APPS` (in addition to `herald`).
-        
-        Second, use the `HeraldPasswordResetForm` in place of django's built in `PasswordResetForm`. This step is entirely dependant on your project structure, but it essentially just involves changing the form class on the password reset view in some way:
-        
-        ```python
-        # you may simply just need to override the password reset url like so:
-        url(r'^password_reset/$', password_reset, name='password_reset', {'password_reset_form': HeraldPasswordResetForm}),
-        
-        # of if you are using something like django-authtools:
-        url(r'^password_reset/$', PasswordResetView.as_view(form_class=HeraldPasswordResetForm), name='password_reset'),
-        
-        # or you may have a customized version of the password reset view:
-        class MyPasswordResetView(FormView):
-            form_class = HeraldPasswordResetForm  # change the form class here
-        
-        # or, you may have a custom password reset form already. In that case, you will want to extend from the HeraldPasswordResetForm:
-        class MyPasswordResetForm(HeraldPasswordResetForm):
-            ...
-        
-        # alternatively, you could even just send the notification wherever you wish, seperate from the form:
-        PasswordResetEmail(some_user).send()
-        ```
-        
-        Third, you may want to customize the templates for the email. By default, herald will use the `registration/password_reset_email.html` that is provided by django for both the html and text versions of the email. But you can simply override `herald/html/password_reset.html` and/or `herald/text/password_reset.txt` to suit your needs.
-        
-        ## User Disabled Notifications
-        
-        If you want to disable certain notifications per user, add a record to the UserNotification table and
-        add notifications to the disabled_notifications many to many table.
-        
-        For example:
-        
-        ```python
-        user = User.objects.get(id=user.id)
-        
-        notification = Notification.objects.get(notification_class=MyNotification.get_class_path())
-        
-        # disable the notification
-        user.usernotification.disabled_notifications.add(notification)
-        ```
-        
-        By default, notifications can be disabled.  You can put can_disable = False in your notification class and the system will
-        populate the database with this default.  Your Notification class can also override the verbose_name by setting it in your
-        inherited Notification class.  Like this:
-        
-        ```python
-        class MyNotification(EmailNotification):
-            can_disable = False
-            verbose_name = "My Required Notification"
-        ```
-        
-        ## Email Attachments
-        
-        To send attachments, assign a list of attachments to the attachments attribute of your EmailNotification instance, or override the get_attachments() method.
-        
-        Each attachment in the list can be one of the following:
-        
-        1. A tuple which consists of the filename, the raw attachment data, and the mimetype. It is up to you to get the attachment data. Like this:
-        
-        ```python
-        raw_data = get_pdf_data()
-        
-        email.attachments = [
-            ('Report.pdf', raw_data, 'application/pdf'),
-            ('report.txt', 'text version of report', 'text/plain')
-        ]
-        email.send()
-        ```
-        
-        2. A MIMEBase object. See the documentation for attachments under EmailMessage Objects/attachments in the Django documentation.
-        
-        3. A django `File` object.
-        
-        ### Inline Attachments
-        
-        Sometimes you want to embed an image directly into the email content.  Do that by using a MIMEImage assigning a content id header to a MIMEImage, like this:
-        
-        ```python
-        email = WelcomeEmail(user)
-        im = get_thumbnail(image_file.name, '600x600', quality=95)
-        my_image = MIMEImage(im.read()) # MIMEImage inherits from MIMEBase
-        my_image.add_header('Content-ID', '<{}>'.format(image_file.name))
-        ```
-        
-        You can refer to these images in your html email templates using the Content ID (cid) like this:
-        
-        ```html
-        <img src="cid:{{image_file.name}}" />
-        ```
-        
-        You would of course need to add the "image_file" to your template context in the example above.  You can also accomplish this using file operations.  In this example we overrode the get_attachments method of an EmailNotification.
-        
-        ```python
-        class MyNotification(EmailNotification):
-            context = {'hello': 'world'}
-            template_name = 'welcome_email'
-            to_emails = ['somebody@example.com']
-            subject = "My email test"
-        
-            def get_attachments(self):
-                fp = open('python.jpeg', 'rb')
-                img = MIMEImage(fp.read())
-                img.add_header('Content-ID', '<{}>'.format('python.jpeg'))
-                return [
-                    img,
-                ]
-        ```
-        
-        And in your template you would refer to it like this, and you would not need to add anything to the context:
-        
-        ```html
-            <img src="cid:python.jpeg" />
-        ```
-        
-        ### HTML2Text Support
-        
-        Django Herald can auto convert your HTML emails to plain text.  Any email without a plain text version
-        will be auto converted if you enable this feature.
-        
-        ```
-        # Install html2text
-        pip install django-herald[html2text]
-        ```
-        
-        In your settings.py file:
-        
-        ```
-        HERALD_HTML2TEXT_ENABLED = True
-        ```
-        
-        You can customize the output of HTML2Text by setting a configuration dictionary. See 
-        [HTML2Text Configuration](https://github.com/Alir3z4/html2text/blob/master/docs/usage.md) for options
-        
-        ```
-        HERALD_HTML2TEXT_CONFIG = {
-            # Key / value configuration of html2text 
-            'ignore_images': True  # Ignores images in conversion
-        }
-        ```
-        
-        ### Twilio
-        
-        ```
-        # Install twilio
-        pip install django-herald[twilio]
-        ```
-        
-        You can retrieve these values on [Twilio Console](https://twilio.com/console). Once you have retrieve the necessary ids, you can place those to your `settings.py`.
-        
-        For reference, Twilio has some great tutorials for python.
-        [Twilio Python Tutorial](https://www.twilio.com/docs/sms/quickstart/python)
-        
-        ```
-        # Twilio configurations
-        # values taken from `twilio console`
-        TWILIO_ACCOUNT_SID = "your_account_sid"
-        TWILIO_AUTH_TOKEN = "your_auth_token"
-        TWILIO_DEFAULT_FROM_NUMBER = "+1234567890"
-        
-        ```
-        
-        ### Other MIME attachments
-        
-        You can also attach any MIMEBase objects as regular attachments, but you must add a content-disposition header, or they will be inaccessible:
-        
-        ```python
-        my_image.add_header('Content-Disposition', 'attachment; filename="python.jpg"')
-        ```
-        
-        Attachments can cause your database to become quite large, so you should be sure to run the management commands to purge the database of old messages.
-        
-        # Running Tests
-        
-        ```bash
-        python runtests.py
-        ```
-        
 Keywords: django,notifications,messaging
-Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: twilio
 Provides-Extra: html2text
+License-File: LICENSE
+
+# django-herald-msg91
+
+[![Latest PyPI version](https://badge.fury.io/py/mindbogglr-django-herald.svg)](https://pypi.python.org/pypi/mindbogglr-django-herald)
+
+Forked from: [django-herald](https://github.com/worthwhile/django-herald/tree/a0da436e003829b72b87b2bcfdc4d0e5e4449adb)
+
+I've added support for sending messages using the [msg91](https://msg91.com/) platform backend for sending text messages (SMS) in India.
+
+Please go over the installation steps mentioned in the [original ReadMe](https://github.com/worthwhile/django-herald/tree/a0da436e003829b72b87b2bcfdc4d0e5e4449adb)
+
+# Differences in setup:
+
+### Installation
+`pip install mindbogglr-django-herald`
+
+### Settings
+In your Django settings file, add the following settings:
+```
+MSG91_TRANSACTIONAL_SENDER_ID = 'SOCKET'
+MSG91_AUTHKEY = '228352HGNg5dF65b57672G'
+```
+Replace 'SOCKET' with any 6 alphebet series that you want in the user's text message inbox.
+Replace '228352HGNg5dF65b57672G' with your authkey from your [msg91](https://msg91.com/) account
+
+**Note:** it'll show up as BT-SOCKET or similar...the first two alphabets indicate the text message provider and the region and is not controllable.
+
+### Usage
+```python
+from herald import registry
+from herald.text_notification import Msg91TextNotification
+
+@registry.register_decorator()
+class InvitationMessage(Msg91TextNotification):
+    template_name = 'invitation_message'  # name of template, without extension
+
+    def __init__(self, to_number, invited_by_user, user_full_name, invitation_url):
+        # set context for the template rendering
+        self.context = {
+            'invited_by_user': invited_by_user,
+            'user_full_name': user_full_name,
+            'invitation_url': invitation_url
+        }
+
+        self.to_number = to_number
+```
+
+# Original ReadMe
+[![Logo](https://github.com/worthwhile/django-herald/raw/master/logo.png)](https://github.com/worthwhile/django-herald)
+
+A Django messaging library that features:
+
+- Class-based declaration and registry approach, like Django Admin
+- Supports multiple transmission methods (Email, SMS, Slack, etc) per message
+- Browser-based previewing of messages
+- Maintains a history of messaging sending attempts and can view these messages
+- Disabling notifications per user
+
+# Python/Django Support
+
+We try to make herald support all versions of django that django supports + all versions in between.
+
+For python, herald supports all versions of python that the above versions of django support.
+
+So as of herald v0.2 we support django 1.11, 2.0, 2.1, and 2.2, and python 2.7, 3.4, 3.5, 3.6, and 3.7.
+
+## What version of herald do I need if I have django x and python x?
+
+If the django/python version combination has a `---` in the table, it is not guaranteed to be supported.
+
+|                   | py 2.7   | py 3.3   | py 3.4   | py 3.5   | py 3.6   | py 3.7   |
+|:-----------------:|:--------:|:--------:|:--------:|:--------:|:--------:|:--------:|
+| **dj 1.8**        | <0.2     | <0.2     | <0.2     | <0.2     | ---      | ---      |
+| **dj 1.9 - 1.10** | <0.2     | ---      | <0.2     | <0.2     | ---      | ---      |
+| **dj 1.11**       | \>=0.1.5 | ---      | \>=0.1.5 | \>=0.1.5 | \>=0.1.5 | ---      |
+| **dj 2.0**        | ---      | ---      | \>=0.1.5 | \>=0.1.5 | \>=0.1.5 | \>=0.2   |
+| **dj 2.1**        | ---      | ---      | ---      | \>=0.2   | \>=0.2   | \>=0.2   |
+| **dj 2.2**        | ---      | ---      | ---      | \>=0.2   | \>=0.2   | \>=0.2   |
+
+
+# Installation
+
+1. `pip install django-herald`
+2. Add `herald` and `django.contrib.sites` to `INSTALLED_APPS`.
+3. Add herald's URLS:
+
+    ```python
+    if settings.DEBUG:
+        urlpatterns = [
+            url(r'^herald/', include('herald.urls')),
+        ] + urlpatterns
+    ```
+
+# Usage
+
+1. Create a `notifications.py` file in any django app. This is where your notification classes will live. Add a class like this:
+
+```python
+from herald import registry
+from herald.base import EmailNotification
+
+
+class WelcomeEmail(EmailNotification):  # extend from EmailNotification for emails
+    template_name = 'welcome_email'  # name of template, without extension
+    subject = 'Welcome'  # subject of email
+
+    def __init__(self, user):  # optionally customize the initialization
+        self.context = {'user': user}  # set context for the template rendering
+        self.to_emails = [user.email]  # set list of emails to send to
+
+    @staticmethod
+    def get_demo_args():  # define a static method to return list of args needed to initialize class for testing
+        from users.models import User
+        return [User.objects.order_by('?')[0]]
+
+registry.register(WelcomeEmail)  # finally, register your notification class
+
+# Alternatively, a class decorator can be used to register the notification:
+
+@registry.register_decorator()
+class WelcomeEmail(EmailNotification):
+    ...
+```
+
+
+2. Create templates for rendering the email using this file structure:
+
+        templates/
+            herald/
+                text/
+                    welcome_email.txt
+                html/
+                    welcome_email.html
+
+3. Test how your email looks by navigating to `/herald/`.
+
+4. Send your email wherever you need in your code:
+
+        WelcomeEmail(user).send()
+
+5. View the sent emails in django admin and even be able to resend it.
+
+## Email options
+
+The following options can be set on the email notification class. For Example:
+
+```
+class WelcomeEmail(EmailNotification):
+    cc = ['test@example.com']
+```
+
+- `from_email`: (`str`, default: `settings.DEFAULT_FROM_EMAIL`) email address of sender
+- `subject`: (`str`, default: ) email subject
+- `to_emails`: (`List[str]`, default: `None`) list of email strings to send to
+- `bcc`: (`List[str]`, default: `None`) list of email strings to send as bcc
+- `cc`: (`List[str]`, default: `None`) list of email strings to send as cc
+- `headers`: (`dict`, default: `None`) extra headers to be passed along to the `EmailMultiAlternatives` object
+- `reply_to`: (`List[str]`, default: `None`) list of email strings to send as the Reply-To emails
+- `attachments`: (`list`) list of attachments. See "Email Attachments" below for more info
+    
+    
+## Automatically Deleting Old Notifications
+
+Herald can automatically delete old notifications whenever a new notification is sent.
+
+To enable this, set the `HERALD_NOTIFICATION_RETENTION_TIME` setting to a timedelta instance.
+
+For example:
+
+```
+HERALD_NOTIFICATION_RETENTION_TIME = timedelta(weeks=8)
+```
+
+Will delete all notifications older than 8 weeks every time a new notification is sent.
+
+## Manually Deleting Old Notifications
+
+The `delnotifs` command is useful for purging the notification history.
+
+The default usage will delete everything from sent during today:
+
+```bash
+python manage.py delnotifs
+```
+
+However, you can also pass arguments for `start` or `end` dates. `end` is up to, but not including that date.
+
+```bash
+python manage.py delnotifs --start='2016-01-01' --end='2016-01-10'
+```
+
+
+## Asynchronous Email Sending
+
+If you are sending slightly different emails to a large number of people, it might take quite a while to process. By default, Django will process this all synchronously. For asynchronous support, we recommend django-celery-email. It is very straightfoward to setup and integrate: https://github.com/pmclanahan/django-celery-email
+
+
+## herald.contrib.auth
+
+Django has built-in support for sending password reset emails. If you would like to send those emails using herald, you can use the notification class in herald.contrib.auth.
+
+First, add `herald.contrib.auth` to `INSTALLED_APPS` (in addition to `herald`).
+
+Second, use the `HeraldPasswordResetForm` in place of django's built in `PasswordResetForm`. This step is entirely dependant on your project structure, but it essentially just involves changing the form class on the password reset view in some way:
+
+```python
+# you may simply just need to override the password reset url like so:
+url(r'^password_reset/$', password_reset, name='password_reset', {'password_reset_form': HeraldPasswordResetForm}),
+
+# of if you are using something like django-authtools:
+url(r'^password_reset/$', PasswordResetView.as_view(form_class=HeraldPasswordResetForm), name='password_reset'),
+
+# or you may have a customized version of the password reset view:
+class MyPasswordResetView(FormView):
+    form_class = HeraldPasswordResetForm  # change the form class here
+
+# or, you may have a custom password reset form already. In that case, you will want to extend from the HeraldPasswordResetForm:
+class MyPasswordResetForm(HeraldPasswordResetForm):
+    ...
+
+# alternatively, you could even just send the notification wherever you wish, seperate from the form:
+PasswordResetEmail(some_user).send()
+```
+
+Third, you may want to customize the templates for the email. By default, herald will use the `registration/password_reset_email.html` that is provided by django for both the html and text versions of the email. But you can simply override `herald/html/password_reset.html` and/or `herald/text/password_reset.txt` to suit your needs.
+
+## User Disabled Notifications
+
+If you want to disable certain notifications per user, add a record to the UserNotification table and
+add notifications to the disabled_notifications many to many table.
+
+For example:
+
+```python
+user = User.objects.get(id=user.id)
+
+notification = Notification.objects.get(notification_class=MyNotification.get_class_path())
+
+# disable the notification
+user.usernotification.disabled_notifications.add(notification)
+```
+
+By default, notifications can be disabled.  You can put can_disable = False in your notification class and the system will
+populate the database with this default.  Your Notification class can also override the verbose_name by setting it in your
+inherited Notification class.  Like this:
+
+```python
+class MyNotification(EmailNotification):
+    can_disable = False
+    verbose_name = "My Required Notification"
+```
+
+## Email Attachments
+
+To send attachments, assign a list of attachments to the attachments attribute of your EmailNotification instance, or override the get_attachments() method.
+
+Each attachment in the list can be one of the following:
+
+1. A tuple which consists of the filename, the raw attachment data, and the mimetype. It is up to you to get the attachment data. Like this:
+
+```python
+raw_data = get_pdf_data()
+
+email.attachments = [
+    ('Report.pdf', raw_data, 'application/pdf'),
+    ('report.txt', 'text version of report', 'text/plain')
+]
+email.send()
+```
+
+2. A MIMEBase object. See the documentation for attachments under EmailMessage Objects/attachments in the Django documentation.
+
+3. A django `File` object.
+
+### Inline Attachments
+
+Sometimes you want to embed an image directly into the email content.  Do that by using a MIMEImage assigning a content id header to a MIMEImage, like this:
+
+```python
+email = WelcomeEmail(user)
+im = get_thumbnail(image_file.name, '600x600', quality=95)
+my_image = MIMEImage(im.read()) # MIMEImage inherits from MIMEBase
+my_image.add_header('Content-ID', '<{}>'.format(image_file.name))
+```
+
+You can refer to these images in your html email templates using the Content ID (cid) like this:
+
+```html
+<img src="cid:{{image_file.name}}" />
+```
+
+You would of course need to add the "image_file" to your template context in the example above.  You can also accomplish this using file operations.  In this example we overrode the get_attachments method of an EmailNotification.
+
+```python
+class MyNotification(EmailNotification):
+    context = {'hello': 'world'}
+    template_name = 'welcome_email'
+    to_emails = ['somebody@example.com']
+    subject = "My email test"
+
+    def get_attachments(self):
+        fp = open('python.jpeg', 'rb')
+        img = MIMEImage(fp.read())
+        img.add_header('Content-ID', '<{}>'.format('python.jpeg'))
+        return [
+            img,
+        ]
+```
+
+And in your template you would refer to it like this, and you would not need to add anything to the context:
+
+```html
+    <img src="cid:python.jpeg" />
+```
+
+### HTML2Text Support
+
+Django Herald can auto convert your HTML emails to plain text.  Any email without a plain text version
+will be auto converted if you enable this feature.
+
+```
+# Install html2text
+pip install django-herald[html2text]
+```
+
+In your settings.py file:
+
+```
+HERALD_HTML2TEXT_ENABLED = True
+```
+
+You can customize the output of HTML2Text by setting a configuration dictionary. See 
+[HTML2Text Configuration](https://github.com/Alir3z4/html2text/blob/master/docs/usage.md) for options
+
+```
+HERALD_HTML2TEXT_CONFIG = {
+    # Key / value configuration of html2text 
+    'ignore_images': True  # Ignores images in conversion
+}
+```
+
+### Twilio
+
+```
+# Install twilio
+pip install django-herald[twilio]
+```
+
+You can retrieve these values on [Twilio Console](https://twilio.com/console). Once you have retrieve the necessary ids, you can place those to your `settings.py`.
+
+For reference, Twilio has some great tutorials for python.
+[Twilio Python Tutorial](https://www.twilio.com/docs/sms/quickstart/python)
+
+```
+# Twilio configurations
+# values taken from `twilio console`
+TWILIO_ACCOUNT_SID = "your_account_sid"
+TWILIO_AUTH_TOKEN = "your_auth_token"
+TWILIO_DEFAULT_FROM_NUMBER = "+1234567890"
+
+```
+
+### Other MIME attachments
+
+You can also attach any MIMEBase objects as regular attachments, but you must add a content-disposition header, or they will be inaccessible:
+
+```python
+my_image.add_header('Content-Disposition', 'attachment; filename="python.jpg"')
+```
+
+Attachments can cause your database to become quite large, so you should be sure to run the management commands to purge the database of old messages.
+
+# Running Tests
+
+```bash
+python runtests.py
+```
```

### Comparing `omic-django-herald-0.2.1.20/omic_django_herald.egg-info/SOURCES.txt` & `omic-django-herald-0.2.1.21/omic_django_herald.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -36,8 +36,17 @@
 herald/migrations/0011_sentnotification_dlt_template_id.py
 herald/migrations/__init__.py
 herald/templates/herald/test/notification_list.html
 omic_django_herald.egg-info/PKG-INFO
 omic_django_herald.egg-info/SOURCES.txt
 omic_django_herald.egg-info/dependency_links.txt
 omic_django_herald.egg-info/requires.txt
-omic_django_herald.egg-info/top_level.txt
+omic_django_herald.egg-info/top_level.txt
+tests/test_admin.py
+tests/test_commands.py
+tests/test_contrib_auth.py
+tests/test_init.py
+tests/test_migrations.py
+tests/test_models.py
+tests/test_notifications.py
+tests/test_usernotifications.py
+tests/test_views.py
```

### Comparing `omic-django-herald-0.2.1.20/PKG-INFO` & `omic-django-herald-0.2.1.21/omic_django_herald.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,402 +1,402 @@
 Metadata-Version: 2.1
 Name: omic-django-herald
-Version: 0.2.1.20
+Version: 0.2.1.21
 Summary: Django library for separating the message content from transmission method
 Home-page: https://github.com/vvkvivekl/omic-django-herald/
-Author: Omic Health
-Author-email: info@omic.health
+Download-URL: https://github.com/vvkvivekl/omic-django-herald/tarball/0.2.1.21
+Author: Pred Health
+Author-email: info@pred.health
 License: MIT
-Download-URL: https://github.com/vvkvivekl/omic-django-herald/tarball/0.2.1.20
-Description: # django-herald-msg91
-        
-        [![Latest PyPI version](https://badge.fury.io/py/omic-django-herald.svg)](https://pypi.python.org/pypi/omic-django-herald)
-        
-        Forked from: [django-herald](https://github.com/worthwhile/django-herald/tree/a0da436e003829b72b87b2bcfdc4d0e5e4449adb)
-        
-        I've added support for sending messages using the [msg91](https://msg91.com/) platform backend for sending text messages (SMS) in India.
-        
-        Please go over the installation steps mentioned in the [original ReadMe](https://github.com/worthwhile/django-herald/tree/a0da436e003829b72b87b2bcfdc4d0e5e4449adb)
-        
-        # Differences in setup:
-        
-        ### Installation
-        `pip install omic-django-herald`
-        
-        ### Settings
-        In your Django settings file, add the following settings:
-        ```
-        MSG91_TRANSACTIONAL_SENDER_ID = 'SOCKET'
-        MSG91_AUTHKEY = '228352HGNg5dF65b57672G'
-        ```
-        Replace 'SOCKET' with any 6 alphebet series that you want in the user's text message inbox.
-        Replace '228352HGNg5dF65b57672G' with your authkey from your [msg91](https://msg91.com/) account
-        
-        **Note:** it'll show up as BT-SOCKET or similar...the first two alphabets indicate the text message provider and the region and is not controllable.
-        
-        ### Usage
-        ```python
-        from herald import registry
-        from herald.text_notification import Msg91TextNotification
-        
-        @registry.register_decorator()
-        class InvitationMessage(Msg91TextNotification):
-            template_name = 'invitation_message'  # name of template, without extension
-        
-            def __init__(self, to_number, invited_by_user, user_full_name, invitation_url):
-                # set context for the template rendering
-                self.context = {
-                    'invited_by_user': invited_by_user,
-                    'user_full_name': user_full_name,
-                    'invitation_url': invitation_url
-                }
-        
-                self.to_number = to_number
-        ```
-        
-        # Original ReadMe
-        [![Logo](https://github.com/worthwhile/django-herald/raw/master/logo.png)](https://github.com/worthwhile/django-herald)
-        
-        A Django messaging library that features:
-        
-        - Class-based declaration and registry approach, like Django Admin
-        - Supports multiple transmission methods (Email, SMS, Slack, etc) per message
-        - Browser-based previewing of messages
-        - Maintains a history of messaging sending attempts and can view these messages
-        - Disabling notifications per user
-        
-        # Python/Django Support
-        
-        We try to make herald support all versions of django that django supports + all versions in between.
-        
-        For python, herald supports all versions of python that the above versions of django support.
-        
-        So as of herald v0.2 we support django 1.11, 2.0, 2.1, and 2.2, and python 2.7, 3.4, 3.5, 3.6, and 3.7.
-        
-        ## What version of herald do I need if I have django x and python x?
-        
-        If the django/python version combination has a `---` in the table, it is not guaranteed to be supported.
-        
-        |                   | py 2.7   | py 3.3   | py 3.4   | py 3.5   | py 3.6   | py 3.7   |
-        |:-----------------:|:--------:|:--------:|:--------:|:--------:|:--------:|:--------:|
-        | **dj 1.8**        | <0.2     | <0.2     | <0.2     | <0.2     | ---      | ---      |
-        | **dj 1.9 - 1.10** | <0.2     | ---      | <0.2     | <0.2     | ---      | ---      |
-        | **dj 1.11**       | \>=0.1.5 | ---      | \>=0.1.5 | \>=0.1.5 | \>=0.1.5 | ---      |
-        | **dj 2.0**        | ---      | ---      | \>=0.1.5 | \>=0.1.5 | \>=0.1.5 | \>=0.2   |
-        | **dj 2.1**        | ---      | ---      | ---      | \>=0.2   | \>=0.2   | \>=0.2   |
-        | **dj 2.2**        | ---      | ---      | ---      | \>=0.2   | \>=0.2   | \>=0.2   |
-        
-        
-        # Installation
-        
-        1. `pip install django-herald`
-        2. Add `herald` and `django.contrib.sites` to `INSTALLED_APPS`.
-        3. Add herald's URLS:
-        
-            ```python
-            if settings.DEBUG:
-                urlpatterns = [
-                    url(r'^herald/', include('herald.urls')),
-                ] + urlpatterns
-            ```
-        
-        # Usage
-        
-        1. Create a `notifications.py` file in any django app. This is where your notification classes will live. Add a class like this:
-        
-        ```python
-        from herald import registry
-        from herald.base import EmailNotification
-        
-        
-        class WelcomeEmail(EmailNotification):  # extend from EmailNotification for emails
-            template_name = 'welcome_email'  # name of template, without extension
-            subject = 'Welcome'  # subject of email
-        
-            def __init__(self, user):  # optionally customize the initialization
-                self.context = {'user': user}  # set context for the template rendering
-                self.to_emails = [user.email]  # set list of emails to send to
-        
-            @staticmethod
-            def get_demo_args():  # define a static method to return list of args needed to initialize class for testing
-                from users.models import User
-                return [User.objects.order_by('?')[0]]
-        
-        registry.register(WelcomeEmail)  # finally, register your notification class
-        
-        # Alternatively, a class decorator can be used to register the notification:
-        
-        @registry.register_decorator()
-        class WelcomeEmail(EmailNotification):
-            ...
-        ```
-        
-        
-        2. Create templates for rendering the email using this file structure:
-        
-                templates/
-                    herald/
-                        text/
-                            welcome_email.txt
-                        html/
-                            welcome_email.html
-        
-        3. Test how your email looks by navigating to `/herald/`.
-        
-        4. Send your email wherever you need in your code:
-        
-                WelcomeEmail(user).send()
-        
-        5. View the sent emails in django admin and even be able to resend it.
-        
-        ## Email options
-        
-        The following options can be set on the email notification class. For Example:
-        
-        ```
-        class WelcomeEmail(EmailNotification):
-            cc = ['test@example.com']
-        ```
-        
-        - `from_email`: (`str`, default: `settings.DEFAULT_FROM_EMAIL`) email address of sender
-        - `subject`: (`str`, default: ) email subject
-        - `to_emails`: (`List[str]`, default: `None`) list of email strings to send to
-        - `bcc`: (`List[str]`, default: `None`) list of email strings to send as bcc
-        - `cc`: (`List[str]`, default: `None`) list of email strings to send as cc
-        - `headers`: (`dict`, default: `None`) extra headers to be passed along to the `EmailMultiAlternatives` object
-        - `reply_to`: (`List[str]`, default: `None`) list of email strings to send as the Reply-To emails
-        - `attachments`: (`list`) list of attachments. See "Email Attachments" below for more info
-            
-            
-        ## Automatically Deleting Old Notifications
-        
-        Herald can automatically delete old notifications whenever a new notification is sent.
-        
-        To enable this, set the `HERALD_NOTIFICATION_RETENTION_TIME` setting to a timedelta instance.
-        
-        For example:
-        
-        ```
-        HERALD_NOTIFICATION_RETENTION_TIME = timedelta(weeks=8)
-        ```
-        
-        Will delete all notifications older than 8 weeks every time a new notification is sent.
-        
-        ## Manually Deleting Old Notifications
-        
-        The `delnotifs` command is useful for purging the notification history.
-        
-        The default usage will delete everything from sent during today:
-        
-        ```bash
-        python manage.py delnotifs
-        ```
-        
-        However, you can also pass arguments for `start` or `end` dates. `end` is up to, but not including that date.
-        
-        ```bash
-        python manage.py delnotifs --start='2016-01-01' --end='2016-01-10'
-        ```
-        
-        
-        ## Asynchronous Email Sending
-        
-        If you are sending slightly different emails to a large number of people, it might take quite a while to process. By default, Django will process this all synchronously. For asynchronous support, we recommend django-celery-email. It is very straightfoward to setup and integrate: https://github.com/pmclanahan/django-celery-email
-        
-        
-        ## herald.contrib.auth
-        
-        Django has built-in support for sending password reset emails. If you would like to send those emails using herald, you can use the notification class in herald.contrib.auth.
-        
-        First, add `herald.contrib.auth` to `INSTALLED_APPS` (in addition to `herald`).
-        
-        Second, use the `HeraldPasswordResetForm` in place of django's built in `PasswordResetForm`. This step is entirely dependant on your project structure, but it essentially just involves changing the form class on the password reset view in some way:
-        
-        ```python
-        # you may simply just need to override the password reset url like so:
-        url(r'^password_reset/$', password_reset, name='password_reset', {'password_reset_form': HeraldPasswordResetForm}),
-        
-        # of if you are using something like django-authtools:
-        url(r'^password_reset/$', PasswordResetView.as_view(form_class=HeraldPasswordResetForm), name='password_reset'),
-        
-        # or you may have a customized version of the password reset view:
-        class MyPasswordResetView(FormView):
-            form_class = HeraldPasswordResetForm  # change the form class here
-        
-        # or, you may have a custom password reset form already. In that case, you will want to extend from the HeraldPasswordResetForm:
-        class MyPasswordResetForm(HeraldPasswordResetForm):
-            ...
-        
-        # alternatively, you could even just send the notification wherever you wish, seperate from the form:
-        PasswordResetEmail(some_user).send()
-        ```
-        
-        Third, you may want to customize the templates for the email. By default, herald will use the `registration/password_reset_email.html` that is provided by django for both the html and text versions of the email. But you can simply override `herald/html/password_reset.html` and/or `herald/text/password_reset.txt` to suit your needs.
-        
-        ## User Disabled Notifications
-        
-        If you want to disable certain notifications per user, add a record to the UserNotification table and
-        add notifications to the disabled_notifications many to many table.
-        
-        For example:
-        
-        ```python
-        user = User.objects.get(id=user.id)
-        
-        notification = Notification.objects.get(notification_class=MyNotification.get_class_path())
-        
-        # disable the notification
-        user.usernotification.disabled_notifications.add(notification)
-        ```
-        
-        By default, notifications can be disabled.  You can put can_disable = False in your notification class and the system will
-        populate the database with this default.  Your Notification class can also override the verbose_name by setting it in your
-        inherited Notification class.  Like this:
-        
-        ```python
-        class MyNotification(EmailNotification):
-            can_disable = False
-            verbose_name = "My Required Notification"
-        ```
-        
-        ## Email Attachments
-        
-        To send attachments, assign a list of attachments to the attachments attribute of your EmailNotification instance, or override the get_attachments() method.
-        
-        Each attachment in the list can be one of the following:
-        
-        1. A tuple which consists of the filename, the raw attachment data, and the mimetype. It is up to you to get the attachment data. Like this:
-        
-        ```python
-        raw_data = get_pdf_data()
-        
-        email.attachments = [
-            ('Report.pdf', raw_data, 'application/pdf'),
-            ('report.txt', 'text version of report', 'text/plain')
-        ]
-        email.send()
-        ```
-        
-        2. A MIMEBase object. See the documentation for attachments under EmailMessage Objects/attachments in the Django documentation.
-        
-        3. A django `File` object.
-        
-        ### Inline Attachments
-        
-        Sometimes you want to embed an image directly into the email content.  Do that by using a MIMEImage assigning a content id header to a MIMEImage, like this:
-        
-        ```python
-        email = WelcomeEmail(user)
-        im = get_thumbnail(image_file.name, '600x600', quality=95)
-        my_image = MIMEImage(im.read()) # MIMEImage inherits from MIMEBase
-        my_image.add_header('Content-ID', '<{}>'.format(image_file.name))
-        ```
-        
-        You can refer to these images in your html email templates using the Content ID (cid) like this:
-        
-        ```html
-        <img src="cid:{{image_file.name}}" />
-        ```
-        
-        You would of course need to add the "image_file" to your template context in the example above.  You can also accomplish this using file operations.  In this example we overrode the get_attachments method of an EmailNotification.
-        
-        ```python
-        class MyNotification(EmailNotification):
-            context = {'hello': 'world'}
-            template_name = 'welcome_email'
-            to_emails = ['somebody@example.com']
-            subject = "My email test"
-        
-            def get_attachments(self):
-                fp = open('python.jpeg', 'rb')
-                img = MIMEImage(fp.read())
-                img.add_header('Content-ID', '<{}>'.format('python.jpeg'))
-                return [
-                    img,
-                ]
-        ```
-        
-        And in your template you would refer to it like this, and you would not need to add anything to the context:
-        
-        ```html
-            <img src="cid:python.jpeg" />
-        ```
-        
-        ### HTML2Text Support
-        
-        Django Herald can auto convert your HTML emails to plain text.  Any email without a plain text version
-        will be auto converted if you enable this feature.
-        
-        ```
-        # Install html2text
-        pip install django-herald[html2text]
-        ```
-        
-        In your settings.py file:
-        
-        ```
-        HERALD_HTML2TEXT_ENABLED = True
-        ```
-        
-        You can customize the output of HTML2Text by setting a configuration dictionary. See 
-        [HTML2Text Configuration](https://github.com/Alir3z4/html2text/blob/master/docs/usage.md) for options
-        
-        ```
-        HERALD_HTML2TEXT_CONFIG = {
-            # Key / value configuration of html2text 
-            'ignore_images': True  # Ignores images in conversion
-        }
-        ```
-        
-        ### Twilio
-        
-        ```
-        # Install twilio
-        pip install django-herald[twilio]
-        ```
-        
-        You can retrieve these values on [Twilio Console](https://twilio.com/console). Once you have retrieve the necessary ids, you can place those to your `settings.py`.
-        
-        For reference, Twilio has some great tutorials for python.
-        [Twilio Python Tutorial](https://www.twilio.com/docs/sms/quickstart/python)
-        
-        ```
-        # Twilio configurations
-        # values taken from `twilio console`
-        TWILIO_ACCOUNT_SID = "your_account_sid"
-        TWILIO_AUTH_TOKEN = "your_auth_token"
-        TWILIO_DEFAULT_FROM_NUMBER = "+1234567890"
-        
-        ```
-        
-        ### Other MIME attachments
-        
-        You can also attach any MIMEBase objects as regular attachments, but you must add a content-disposition header, or they will be inaccessible:
-        
-        ```python
-        my_image.add_header('Content-Disposition', 'attachment; filename="python.jpg"')
-        ```
-        
-        Attachments can cause your database to become quite large, so you should be sure to run the management commands to purge the database of old messages.
-        
-        # Running Tests
-        
-        ```bash
-        python runtests.py
-        ```
-        
 Keywords: django,notifications,messaging
-Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: twilio
 Provides-Extra: html2text
+License-File: LICENSE
+
+# django-herald-msg91
+
+[![Latest PyPI version](https://badge.fury.io/py/mindbogglr-django-herald.svg)](https://pypi.python.org/pypi/mindbogglr-django-herald)
+
+Forked from: [django-herald](https://github.com/worthwhile/django-herald/tree/a0da436e003829b72b87b2bcfdc4d0e5e4449adb)
+
+I've added support for sending messages using the [msg91](https://msg91.com/) platform backend for sending text messages (SMS) in India.
+
+Please go over the installation steps mentioned in the [original ReadMe](https://github.com/worthwhile/django-herald/tree/a0da436e003829b72b87b2bcfdc4d0e5e4449adb)
+
+# Differences in setup:
+
+### Installation
+`pip install mindbogglr-django-herald`
+
+### Settings
+In your Django settings file, add the following settings:
+```
+MSG91_TRANSACTIONAL_SENDER_ID = 'SOCKET'
+MSG91_AUTHKEY = '228352HGNg5dF65b57672G'
+```
+Replace 'SOCKET' with any 6 alphebet series that you want in the user's text message inbox.
+Replace '228352HGNg5dF65b57672G' with your authkey from your [msg91](https://msg91.com/) account
+
+**Note:** it'll show up as BT-SOCKET or similar...the first two alphabets indicate the text message provider and the region and is not controllable.
+
+### Usage
+```python
+from herald import registry
+from herald.text_notification import Msg91TextNotification
+
+@registry.register_decorator()
+class InvitationMessage(Msg91TextNotification):
+    template_name = 'invitation_message'  # name of template, without extension
+
+    def __init__(self, to_number, invited_by_user, user_full_name, invitation_url):
+        # set context for the template rendering
+        self.context = {
+            'invited_by_user': invited_by_user,
+            'user_full_name': user_full_name,
+            'invitation_url': invitation_url
+        }
+
+        self.to_number = to_number
+```
+
+# Original ReadMe
+[![Logo](https://github.com/worthwhile/django-herald/raw/master/logo.png)](https://github.com/worthwhile/django-herald)
+
+A Django messaging library that features:
+
+- Class-based declaration and registry approach, like Django Admin
+- Supports multiple transmission methods (Email, SMS, Slack, etc) per message
+- Browser-based previewing of messages
+- Maintains a history of messaging sending attempts and can view these messages
+- Disabling notifications per user
+
+# Python/Django Support
+
+We try to make herald support all versions of django that django supports + all versions in between.
+
+For python, herald supports all versions of python that the above versions of django support.
+
+So as of herald v0.2 we support django 1.11, 2.0, 2.1, and 2.2, and python 2.7, 3.4, 3.5, 3.6, and 3.7.
+
+## What version of herald do I need if I have django x and python x?
+
+If the django/python version combination has a `---` in the table, it is not guaranteed to be supported.
+
+|                   | py 2.7   | py 3.3   | py 3.4   | py 3.5   | py 3.6   | py 3.7   |
+|:-----------------:|:--------:|:--------:|:--------:|:--------:|:--------:|:--------:|
+| **dj 1.8**        | <0.2     | <0.2     | <0.2     | <0.2     | ---      | ---      |
+| **dj 1.9 - 1.10** | <0.2     | ---      | <0.2     | <0.2     | ---      | ---      |
+| **dj 1.11**       | \>=0.1.5 | ---      | \>=0.1.5 | \>=0.1.5 | \>=0.1.5 | ---      |
+| **dj 2.0**        | ---      | ---      | \>=0.1.5 | \>=0.1.5 | \>=0.1.5 | \>=0.2   |
+| **dj 2.1**        | ---      | ---      | ---      | \>=0.2   | \>=0.2   | \>=0.2   |
+| **dj 2.2**        | ---      | ---      | ---      | \>=0.2   | \>=0.2   | \>=0.2   |
+
+
+# Installation
+
+1. `pip install django-herald`
+2. Add `herald` and `django.contrib.sites` to `INSTALLED_APPS`.
+3. Add herald's URLS:
+
+    ```python
+    if settings.DEBUG:
+        urlpatterns = [
+            url(r'^herald/', include('herald.urls')),
+        ] + urlpatterns
+    ```
+
+# Usage
+
+1. Create a `notifications.py` file in any django app. This is where your notification classes will live. Add a class like this:
+
+```python
+from herald import registry
+from herald.base import EmailNotification
+
+
+class WelcomeEmail(EmailNotification):  # extend from EmailNotification for emails
+    template_name = 'welcome_email'  # name of template, without extension
+    subject = 'Welcome'  # subject of email
+
+    def __init__(self, user):  # optionally customize the initialization
+        self.context = {'user': user}  # set context for the template rendering
+        self.to_emails = [user.email]  # set list of emails to send to
+
+    @staticmethod
+    def get_demo_args():  # define a static method to return list of args needed to initialize class for testing
+        from users.models import User
+        return [User.objects.order_by('?')[0]]
+
+registry.register(WelcomeEmail)  # finally, register your notification class
+
+# Alternatively, a class decorator can be used to register the notification:
+
+@registry.register_decorator()
+class WelcomeEmail(EmailNotification):
+    ...
+```
+
+
+2. Create templates for rendering the email using this file structure:
+
+        templates/
+            herald/
+                text/
+                    welcome_email.txt
+                html/
+                    welcome_email.html
+
+3. Test how your email looks by navigating to `/herald/`.
+
+4. Send your email wherever you need in your code:
+
+        WelcomeEmail(user).send()
+
+5. View the sent emails in django admin and even be able to resend it.
+
+## Email options
+
+The following options can be set on the email notification class. For Example:
+
+```
+class WelcomeEmail(EmailNotification):
+    cc = ['test@example.com']
+```
+
+- `from_email`: (`str`, default: `settings.DEFAULT_FROM_EMAIL`) email address of sender
+- `subject`: (`str`, default: ) email subject
+- `to_emails`: (`List[str]`, default: `None`) list of email strings to send to
+- `bcc`: (`List[str]`, default: `None`) list of email strings to send as bcc
+- `cc`: (`List[str]`, default: `None`) list of email strings to send as cc
+- `headers`: (`dict`, default: `None`) extra headers to be passed along to the `EmailMultiAlternatives` object
+- `reply_to`: (`List[str]`, default: `None`) list of email strings to send as the Reply-To emails
+- `attachments`: (`list`) list of attachments. See "Email Attachments" below for more info
+    
+    
+## Automatically Deleting Old Notifications
+
+Herald can automatically delete old notifications whenever a new notification is sent.
+
+To enable this, set the `HERALD_NOTIFICATION_RETENTION_TIME` setting to a timedelta instance.
+
+For example:
+
+```
+HERALD_NOTIFICATION_RETENTION_TIME = timedelta(weeks=8)
+```
+
+Will delete all notifications older than 8 weeks every time a new notification is sent.
+
+## Manually Deleting Old Notifications
+
+The `delnotifs` command is useful for purging the notification history.
+
+The default usage will delete everything from sent during today:
+
+```bash
+python manage.py delnotifs
+```
+
+However, you can also pass arguments for `start` or `end` dates. `end` is up to, but not including that date.
+
+```bash
+python manage.py delnotifs --start='2016-01-01' --end='2016-01-10'
+```
+
+
+## Asynchronous Email Sending
+
+If you are sending slightly different emails to a large number of people, it might take quite a while to process. By default, Django will process this all synchronously. For asynchronous support, we recommend django-celery-email. It is very straightfoward to setup and integrate: https://github.com/pmclanahan/django-celery-email
+
+
+## herald.contrib.auth
+
+Django has built-in support for sending password reset emails. If you would like to send those emails using herald, you can use the notification class in herald.contrib.auth.
+
+First, add `herald.contrib.auth` to `INSTALLED_APPS` (in addition to `herald`).
+
+Second, use the `HeraldPasswordResetForm` in place of django's built in `PasswordResetForm`. This step is entirely dependant on your project structure, but it essentially just involves changing the form class on the password reset view in some way:
+
+```python
+# you may simply just need to override the password reset url like so:
+url(r'^password_reset/$', password_reset, name='password_reset', {'password_reset_form': HeraldPasswordResetForm}),
+
+# of if you are using something like django-authtools:
+url(r'^password_reset/$', PasswordResetView.as_view(form_class=HeraldPasswordResetForm), name='password_reset'),
+
+# or you may have a customized version of the password reset view:
+class MyPasswordResetView(FormView):
+    form_class = HeraldPasswordResetForm  # change the form class here
+
+# or, you may have a custom password reset form already. In that case, you will want to extend from the HeraldPasswordResetForm:
+class MyPasswordResetForm(HeraldPasswordResetForm):
+    ...
+
+# alternatively, you could even just send the notification wherever you wish, seperate from the form:
+PasswordResetEmail(some_user).send()
+```
+
+Third, you may want to customize the templates for the email. By default, herald will use the `registration/password_reset_email.html` that is provided by django for both the html and text versions of the email. But you can simply override `herald/html/password_reset.html` and/or `herald/text/password_reset.txt` to suit your needs.
+
+## User Disabled Notifications
+
+If you want to disable certain notifications per user, add a record to the UserNotification table and
+add notifications to the disabled_notifications many to many table.
+
+For example:
+
+```python
+user = User.objects.get(id=user.id)
+
+notification = Notification.objects.get(notification_class=MyNotification.get_class_path())
+
+# disable the notification
+user.usernotification.disabled_notifications.add(notification)
+```
+
+By default, notifications can be disabled.  You can put can_disable = False in your notification class and the system will
+populate the database with this default.  Your Notification class can also override the verbose_name by setting it in your
+inherited Notification class.  Like this:
+
+```python
+class MyNotification(EmailNotification):
+    can_disable = False
+    verbose_name = "My Required Notification"
+```
+
+## Email Attachments
+
+To send attachments, assign a list of attachments to the attachments attribute of your EmailNotification instance, or override the get_attachments() method.
+
+Each attachment in the list can be one of the following:
+
+1. A tuple which consists of the filename, the raw attachment data, and the mimetype. It is up to you to get the attachment data. Like this:
+
+```python
+raw_data = get_pdf_data()
+
+email.attachments = [
+    ('Report.pdf', raw_data, 'application/pdf'),
+    ('report.txt', 'text version of report', 'text/plain')
+]
+email.send()
+```
+
+2. A MIMEBase object. See the documentation for attachments under EmailMessage Objects/attachments in the Django documentation.
+
+3. A django `File` object.
+
+### Inline Attachments
+
+Sometimes you want to embed an image directly into the email content.  Do that by using a MIMEImage assigning a content id header to a MIMEImage, like this:
+
+```python
+email = WelcomeEmail(user)
+im = get_thumbnail(image_file.name, '600x600', quality=95)
+my_image = MIMEImage(im.read()) # MIMEImage inherits from MIMEBase
+my_image.add_header('Content-ID', '<{}>'.format(image_file.name))
+```
+
+You can refer to these images in your html email templates using the Content ID (cid) like this:
+
+```html
+<img src="cid:{{image_file.name}}" />
+```
+
+You would of course need to add the "image_file" to your template context in the example above.  You can also accomplish this using file operations.  In this example we overrode the get_attachments method of an EmailNotification.
+
+```python
+class MyNotification(EmailNotification):
+    context = {'hello': 'world'}
+    template_name = 'welcome_email'
+    to_emails = ['somebody@example.com']
+    subject = "My email test"
+
+    def get_attachments(self):
+        fp = open('python.jpeg', 'rb')
+        img = MIMEImage(fp.read())
+        img.add_header('Content-ID', '<{}>'.format('python.jpeg'))
+        return [
+            img,
+        ]
+```
+
+And in your template you would refer to it like this, and you would not need to add anything to the context:
+
+```html
+    <img src="cid:python.jpeg" />
+```
+
+### HTML2Text Support
+
+Django Herald can auto convert your HTML emails to plain text.  Any email without a plain text version
+will be auto converted if you enable this feature.
+
+```
+# Install html2text
+pip install django-herald[html2text]
+```
+
+In your settings.py file:
+
+```
+HERALD_HTML2TEXT_ENABLED = True
+```
+
+You can customize the output of HTML2Text by setting a configuration dictionary. See 
+[HTML2Text Configuration](https://github.com/Alir3z4/html2text/blob/master/docs/usage.md) for options
+
+```
+HERALD_HTML2TEXT_CONFIG = {
+    # Key / value configuration of html2text 
+    'ignore_images': True  # Ignores images in conversion
+}
+```
+
+### Twilio
+
+```
+# Install twilio
+pip install django-herald[twilio]
+```
+
+You can retrieve these values on [Twilio Console](https://twilio.com/console). Once you have retrieve the necessary ids, you can place those to your `settings.py`.
+
+For reference, Twilio has some great tutorials for python.
+[Twilio Python Tutorial](https://www.twilio.com/docs/sms/quickstart/python)
+
+```
+# Twilio configurations
+# values taken from `twilio console`
+TWILIO_ACCOUNT_SID = "your_account_sid"
+TWILIO_AUTH_TOKEN = "your_auth_token"
+TWILIO_DEFAULT_FROM_NUMBER = "+1234567890"
+
+```
+
+### Other MIME attachments
+
+You can also attach any MIMEBase objects as regular attachments, but you must add a content-disposition header, or they will be inaccessible:
+
+```python
+my_image.add_header('Content-Disposition', 'attachment; filename="python.jpg"')
+```
+
+Attachments can cause your database to become quite large, so you should be sure to run the management commands to purge the database of old messages.
+
+# Running Tests
+
+```bash
+python runtests.py
+```
```

### Comparing `omic-django-herald-0.2.1.20/README.md` & `omic-django-herald-0.2.1.21/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # django-herald-msg91
 
-[![Latest PyPI version](https://badge.fury.io/py/omic-django-herald.svg)](https://pypi.python.org/pypi/omic-django-herald)
+[![Latest PyPI version](https://badge.fury.io/py/mindbogglr-django-herald.svg)](https://pypi.python.org/pypi/mindbogglr-django-herald)
 
 Forked from: [django-herald](https://github.com/worthwhile/django-herald/tree/a0da436e003829b72b87b2bcfdc4d0e5e4449adb)
 
 I've added support for sending messages using the [msg91](https://msg91.com/) platform backend for sending text messages (SMS) in India.
 
 Please go over the installation steps mentioned in the [original ReadMe](https://github.com/worthwhile/django-herald/tree/a0da436e003829b72b87b2bcfdc4d0e5e4449adb)
 
 # Differences in setup:
 
 ### Installation
-`pip install omic-django-herald`
+`pip install mindbogglr-django-herald`
 
 ### Settings
 In your Django settings file, add the following settings:
 ```
 MSG91_TRANSACTIONAL_SENDER_ID = 'SOCKET'
 MSG91_AUTHKEY = '228352HGNg5dF65b57672G'
 ```
```

### Comparing `omic-django-herald-0.2.1.20/setup.py` & `omic-django-herald-0.2.1.21/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import find_packages, setup
 
-VERSION = __import__('herald').__version__ + '.20'
+VERSION = __import__('herald').__version__ + '.21'
 
 
 def read_file(filename):
     """Read a file into a string"""
     path = os.path.abspath(os.path.dirname(__file__))
     filepath = os.path.join(path, filename)
     try:
@@ -29,16 +29,16 @@
 html2text_requires = [
     'html2text',
 ]
 
 setup(
     name='omic-django-herald',
     version=VERSION,
-    author='Omic Health',
-    author_email='info@omic.health',
+    author='Pred Health',
+    author_email='info@pred.health',
     install_requires=install_requires,
     extras_require={
         'dev': install_requires + dev_requires,
         'twilio': twilio_requires,
         'html2text': html2text_requires,
     },
     packages=find_packages(include=('herald', 'herald.*')),
```

