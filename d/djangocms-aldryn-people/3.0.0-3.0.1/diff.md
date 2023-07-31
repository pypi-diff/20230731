# Comparing `tmp/djangocms-aldryn-people-3.0.0.tar.gz` & `tmp/djangocms-aldryn-people-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-aldryn-people-3.0.0.tar", last modified: Mon Jul 24 12:00:17 2023, max compression
+gzip compressed data, was "djangocms-aldryn-people-3.0.1.tar", last modified: Mon Jul 31 14:28:49 2023, max compression
```

## Comparing `djangocms-aldryn-people-3.0.0.tar` & `djangocms-aldryn-people-3.0.1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.515645 djangocms-aldryn-people-3.0.0/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1475 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/LICENSE.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      223 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/MANIFEST.in
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3409 2023-07-24 12:00:17.515645 djangocms-aldryn-people-3.0.0/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2129 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/README.rst
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.503646 djangocms-aldryn-people-3.0.0/aldryn_people/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       63 2023-07-24 12:00:05.000000 djangocms-aldryn-people-3.0.0/aldryn_people/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3304 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/admin.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      129 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/apps.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.499645 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.499645 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.499645 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.507645 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       70 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/base.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      504 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/fullwidth.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      480 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/group_detail.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      743 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/group_list.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.507645 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/includes/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1401 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/includes/group.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2324 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/includes/person.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      357 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/person_detail.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.499645 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/plugins/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.507645 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/plugins/feature/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       64 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/plugins/feature/people_list.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.507645 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/plugins/standard/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1493 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/plugins/standard/people_list.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.499645 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.499645 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.507645 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      436 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/group_detail.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      835 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/group_list.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.507645 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/includes/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1302 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/includes/people_item.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      185 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/includes/people_items.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      312 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/person_detail.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.507645 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.507645 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/feature/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      830 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/feature/people_list.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      829 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/people_list.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.507645 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/standard/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1335 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/standard/people_list.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      408 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/cms_apps.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2705 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/cms_plugins.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5341 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/cms_toolbars.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2864 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/cms_wizards.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.503646 djangocms-aldryn-people-3.0.0/aldryn_people/locale/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.503646 djangocms-aldryn-people-3.0.0/aldryn_people/locale/de/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.511645 djangocms-aldryn-people-3.0.0/aldryn_people/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4384 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8301 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.503646 djangocms-aldryn-people-3.0.0/aldryn_people/locale/en/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.511645 djangocms-aldryn-people-3.0.0/aldryn_people/locale/en/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      378 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6872 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.503646 djangocms-aldryn-people-3.0.0/aldryn_people/locale/es/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.511645 djangocms-aldryn-people-3.0.0/aldryn_people/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      481 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6948 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.503646 djangocms-aldryn-people-3.0.0/aldryn_people/locale/fr/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.511645 djangocms-aldryn-people-3.0.0/aldryn_people/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4681 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8639 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.503646 djangocms-aldryn-people-3.0.0/aldryn_people/locale/it/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.511645 djangocms-aldryn-people-3.0.0/aldryn_people/locale/it/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      481 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6948 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.503646 djangocms-aldryn-people-3.0.0/aldryn_people/locale/nl/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.511645 djangocms-aldryn-people-3.0.0/aldryn_people/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4331 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8251 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/locale/nl/LC_MESSAGES/django.po
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2184 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/menu.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.511645 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6480 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0001_initial.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1078 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0002_auto_20150128_1411.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      511 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0003_auto_20150425_2103.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1061 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0004_auto_20150622_1606.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1103 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0005_auto_20150723_1508.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      571 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0006_person_groups.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      860 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0007_copy_group.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      276 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0008_remove_person_group.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      926 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0009_auto_20150724_1654.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1900 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0010_auto_20150724_1654.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1413 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0011_auto_20150724_1900.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      619 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0012_auto_20150728_1114.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      493 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0013_peopleplugin_show_ungrouped.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1724 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0014_auto_20150807_0033.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      603 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0015_m2m_remove_null.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      570 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0016_person_fk_to_one_to_one.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      594 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0017_auto_20160109_1951.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      539 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0018_auto_20160802_1852.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2523 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0019_alter_group_id_alter_grouptranslation_id_and_more.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/migrations/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    10891 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/models.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      815 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/search_indexes.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.503646 djangocms-aldryn-people-3.0.0/aldryn_people/templates/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.515645 djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      361 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/group_detail.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      594 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/group_list.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.515645 djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/includes/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      922 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/includes/group.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2198 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/includes/person.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      249 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/person_detail.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.503646 djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/plugins/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.515645 djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/plugins/feature/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       64 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/plugins/feature/people_list.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.515645 djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/plugins/standard/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1270 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/plugins/standard/people_list.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.515645 djangocms-aldryn-people-3.0.0/aldryn_people/templatetags/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/templatetags/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      512 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/templatetags/aldryn_people_tags.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.515645 djangocms-aldryn-people-3.0.0/aldryn_people/tests/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    10177 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/tests/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      763 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/tests/test_admin.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      926 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/tests/test_app_hook.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8748 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/tests/test_models.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     7674 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/tests/test_plugins.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1626 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/tests/test_search_indexes.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1780 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/tests/test_toolbar.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2974 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/tests/test_views.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      793 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/urls.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1508 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/utils.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1044 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/vcard.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3561 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/aldryn_people/views.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 12:00:17.515645 djangocms-aldryn-people-3.0.0/djangocms_aldryn_people.egg-info/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3409 2023-07-24 12:00:17.000000 djangocms-aldryn-people-3.0.0/djangocms_aldryn_people.egg-info/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4491 2023-07-24 12:00:17.000000 djangocms-aldryn-people-3.0.0/djangocms_aldryn_people.egg-info/SOURCES.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-24 12:00:17.000000 djangocms-aldryn-people-3.0.0/djangocms_aldryn_people.egg-info/dependency_links.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-19 08:14:30.000000 djangocms-aldryn-people-3.0.0/djangocms_aldryn_people.egg-info/not-zip-safe
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      101 2023-07-24 12:00:17.000000 djangocms-aldryn-people-3.0.0/djangocms_aldryn_people.egg-info/requires.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       14 2023-07-24 12:00:17.000000 djangocms-aldryn-people-3.0.0/djangocms_aldryn_people.egg-info/top_level.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      572 2023-07-24 12:00:17.515645 djangocms-aldryn-people-3.0.0/setup.cfg
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1834 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.0/setup.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.306902 djangocms-aldryn-people-3.0.1/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1475 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/LICENSE.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      223 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/MANIFEST.in
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3421 2023-07-31 14:28:49.306902 djangocms-aldryn-people-3.0.1/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2149 2023-07-31 14:24:44.000000 djangocms-aldryn-people-3.0.1/README.rst
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.290902 djangocms-aldryn-people-3.0.1/aldryn_people/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       63 2023-07-31 14:28:28.000000 djangocms-aldryn-people-3.0.1/aldryn_people/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3304 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/admin.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      129 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/apps.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.286902 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.286902 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.286902 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.294902 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       70 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/base.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      504 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/fullwidth.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      480 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/group_detail.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      743 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/group_list.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.294902 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/includes/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1401 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/includes/group.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2324 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/includes/person.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      357 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/person_detail.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.286902 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/plugins/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.294902 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/plugins/feature/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       64 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/plugins/feature/people_list.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.294902 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/plugins/standard/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1493 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/plugins/standard/people_list.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.286902 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.286902 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.294902 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      436 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/group_detail.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      835 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/group_list.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.294902 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/includes/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1302 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/includes/people_item.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      185 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/includes/people_items.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      312 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/person_detail.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.294902 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.294902 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/feature/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      830 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/feature/people_list.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      829 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/people_list.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.294902 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/standard/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1335 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/standard/people_list.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      408 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/cms_apps.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2705 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/cms_plugins.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5341 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/cms_toolbars.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2864 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/cms_wizards.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.286902 djangocms-aldryn-people-3.0.1/aldryn_people/locale/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.286902 djangocms-aldryn-people-3.0.1/aldryn_people/locale/de/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.298902 djangocms-aldryn-people-3.0.1/aldryn_people/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4384 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8301 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.286902 djangocms-aldryn-people-3.0.1/aldryn_people/locale/en/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.298902 djangocms-aldryn-people-3.0.1/aldryn_people/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      378 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6872 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.286902 djangocms-aldryn-people-3.0.1/aldryn_people/locale/es/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.298902 djangocms-aldryn-people-3.0.1/aldryn_people/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      481 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6948 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.286902 djangocms-aldryn-people-3.0.1/aldryn_people/locale/fr/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.298902 djangocms-aldryn-people-3.0.1/aldryn_people/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4681 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8639 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.286902 djangocms-aldryn-people-3.0.1/aldryn_people/locale/it/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.298902 djangocms-aldryn-people-3.0.1/aldryn_people/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      481 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6948 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.286902 djangocms-aldryn-people-3.0.1/aldryn_people/locale/nl/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.298902 djangocms-aldryn-people-3.0.1/aldryn_people/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4331 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8251 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/locale/nl/LC_MESSAGES/django.po
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2184 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/menu.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.302902 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     6480 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0001_initial.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1078 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0002_auto_20150128_1411.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      511 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0003_auto_20150425_2103.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1061 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0004_auto_20150622_1606.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1103 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0005_auto_20150723_1508.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      571 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0006_person_groups.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      860 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0007_copy_group.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      276 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0008_remove_person_group.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      926 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0009_auto_20150724_1654.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1900 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0010_auto_20150724_1654.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1413 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0011_auto_20150724_1900.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      619 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0012_auto_20150728_1114.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      493 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0013_peopleplugin_show_ungrouped.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1724 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0014_auto_20150807_0033.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      603 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0015_m2m_remove_null.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      570 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0016_person_fk_to_one_to_one.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      594 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0017_auto_20160109_1951.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      539 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0018_auto_20160802_1852.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2523 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0019_alter_group_id_alter_grouptranslation_id_and_more.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/migrations/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    10891 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/models.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      815 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/search_indexes.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.286902 djangocms-aldryn-people-3.0.1/aldryn_people/templates/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.302902 djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      361 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/group_detail.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      594 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/group_list.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.302902 djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/includes/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      922 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/includes/group.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2198 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/includes/person.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      249 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/person_detail.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.286902 djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/plugins/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.302902 djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/plugins/feature/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       64 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/plugins/feature/people_list.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.302902 djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/plugins/standard/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1270 2023-06-19 07:27:43.000000 djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/plugins/standard/people_list.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.302902 djangocms-aldryn-people-3.0.1/aldryn_people/templatetags/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/templatetags/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      512 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/templatetags/aldryn_people_tags.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.306902 djangocms-aldryn-people-3.0.1/aldryn_people/tests/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    10177 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/tests/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      763 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/tests/test_admin.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      926 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/tests/test_app_hook.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     8748 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/tests/test_models.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     7674 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/tests/test_plugins.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1626 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/tests/test_search_indexes.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1780 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/tests/test_toolbar.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2974 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/tests/test_views.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      793 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/urls.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1508 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/utils.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1044 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/vcard.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3561 2023-07-24 11:57:12.000000 djangocms-aldryn-people-3.0.1/aldryn_people/views.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-31 14:28:49.306902 djangocms-aldryn-people-3.0.1/djangocms_aldryn_people.egg-info/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     3421 2023-07-31 14:28:49.000000 djangocms-aldryn-people-3.0.1/djangocms_aldryn_people.egg-info/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4491 2023-07-31 14:28:49.000000 djangocms-aldryn-people-3.0.1/djangocms_aldryn_people.egg-info/SOURCES.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-31 14:28:49.000000 djangocms-aldryn-people-3.0.1/djangocms_aldryn_people.egg-info/dependency_links.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-19 08:14:30.000000 djangocms-aldryn-people-3.0.1/djangocms_aldryn_people.egg-info/not-zip-safe
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      106 2023-07-31 14:28:49.000000 djangocms-aldryn-people-3.0.1/djangocms_aldryn_people.egg-info/requires.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       14 2023-07-31 14:28:49.000000 djangocms-aldryn-people-3.0.1/djangocms_aldryn_people.egg-info/top_level.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      572 2023-07-31 14:28:49.306902 djangocms-aldryn-people-3.0.1/setup.cfg
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1831 2023-07-31 14:20:46.000000 djangocms-aldryn-people-3.0.1/setup.py
```

### Comparing `djangocms-aldryn-people-3.0.0/LICENSE.txt` & `djangocms-aldryn-people-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/PKG-INFO` & `djangocms-aldryn-people-3.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: djangocms-aldryn-people
-Version: 3.0.0
+Version: 3.0.1
 Summary: Aldryn People publishes profile pages for people in your organisation including team members, collaborators, partners, clients, and so on, including photographs and address information.
 Home-page: https://github.com/CZ-NIC/djangocms-aldryn-people
 Author: Divio AG
 Author-email: info@divio.ch
-License: BSD License
+License: BSD
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
@@ -58,22 +58,22 @@
 
 We're grateful to all contributors who have helped create and maintain this package.
 
 Contributors are listed at `contributions page
 <https://github.com/aldryn/aldryn-translation-tools/graphs/contributors>`_.
 
 
-.. |Project continuation| image:: https://img.shields.io/badge/Continuation-Divio_Aldryn_Search-blue
+.. |Project continuation| image:: https://img.shields.io/badge/Continuation-Divio_Aldryn_People-blue
     :target: https://github.com/CZ-NIC/djangocms-aldryn-people
     :alt: Continuation of the deprecated project "Divio Aldryn People"
 .. |Pypi package| image:: https://img.shields.io/pypi/v/djangocms-aldryn-people.svg
     :target: https://pypi.python.org/pypi/djangocms-aldryn-people/
     :alt: Pypi package
 .. |Pypi status| image:: https://img.shields.io/pypi/status/djangocms-aldryn-people.svg
    :target: https://pypi.python.org/pypi/djangocms-aldryn-people
    :alt: status
 .. |Python versions| image:: https://img.shields.io/pypi/pyversions/djangocms-aldryn-people.svg
    :target: https://pypi.python.org/pypi/djangocms-aldryn-people
    :alt: Python versions
 .. |License| image:: https://img.shields.io/pypi/l/djangocms-aldryn-people.svg
-    :target: https://pypi.python.org/pypi/djangocms-aldryn-people/
+    :target: https://github.com/CZ-NIC/djangocms-aldryn-people/blob/master/LICENSE.txt
     :alt: license
```

### Comparing `djangocms-aldryn-people-3.0.0/README.rst` & `djangocms-aldryn-people-3.0.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -29,22 +29,22 @@
 
 We're grateful to all contributors who have helped create and maintain this package.
 
 Contributors are listed at `contributions page
 <https://github.com/aldryn/aldryn-translation-tools/graphs/contributors>`_.
 
 
-.. |Project continuation| image:: https://img.shields.io/badge/Continuation-Divio_Aldryn_Search-blue
+.. |Project continuation| image:: https://img.shields.io/badge/Continuation-Divio_Aldryn_People-blue
     :target: https://github.com/CZ-NIC/djangocms-aldryn-people
     :alt: Continuation of the deprecated project "Divio Aldryn People"
 .. |Pypi package| image:: https://img.shields.io/pypi/v/djangocms-aldryn-people.svg
     :target: https://pypi.python.org/pypi/djangocms-aldryn-people/
     :alt: Pypi package
 .. |Pypi status| image:: https://img.shields.io/pypi/status/djangocms-aldryn-people.svg
    :target: https://pypi.python.org/pypi/djangocms-aldryn-people
    :alt: status
 .. |Python versions| image:: https://img.shields.io/pypi/pyversions/djangocms-aldryn-people.svg
    :target: https://pypi.python.org/pypi/djangocms-aldryn-people
    :alt: Python versions
 .. |License| image:: https://img.shields.io/pypi/l/djangocms-aldryn-people.svg
-    :target: https://pypi.python.org/pypi/djangocms-aldryn-people/
+    :target: https://github.com/CZ-NIC/djangocms-aldryn-people/blob/master/LICENSE.txt
     :alt: license
```

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/admin.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/group_list.html` & `djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/group_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/includes/group.html` & `djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/includes/group.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/includes/person.html` & `djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/includes/person.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/plugins/standard/people_list.html` & `djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/bootstrap3/templates/aldryn_people/plugins/standard/people_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/group_list.html` & `djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/group_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/includes/people_item.html` & `djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/includes/people_item.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/feature/people_list.html` & `djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/feature/people_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/people_list.html` & `djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/people_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/standard/people_list.html` & `djangocms-aldryn-people-3.0.1/aldryn_people/boilerplates/legacy/templates/aldryn_people/plugins/standard/people_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/cms_plugins.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/cms_toolbars.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/cms_wizards.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/cms_wizards.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/locale/de/LC_MESSAGES/django.mo` & `djangocms-aldryn-people-3.0.1/aldryn_people/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/locale/de/LC_MESSAGES/django.po` & `djangocms-aldryn-people-3.0.1/aldryn_people/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/locale/en/LC_MESSAGES/django.po` & `djangocms-aldryn-people-3.0.1/aldryn_people/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/locale/es/LC_MESSAGES/django.po` & `djangocms-aldryn-people-3.0.1/aldryn_people/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/locale/fr/LC_MESSAGES/django.mo` & `djangocms-aldryn-people-3.0.1/aldryn_people/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/locale/fr/LC_MESSAGES/django.po` & `djangocms-aldryn-people-3.0.1/aldryn_people/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/locale/it/LC_MESSAGES/django.po` & `djangocms-aldryn-people-3.0.1/aldryn_people/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/locale/nl/LC_MESSAGES/django.mo` & `djangocms-aldryn-people-3.0.1/aldryn_people/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/locale/nl/LC_MESSAGES/django.po` & `djangocms-aldryn-people-3.0.1/aldryn_people/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/menu.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/menu.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0001_initial.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0002_auto_20150128_1411.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0002_auto_20150128_1411.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0004_auto_20150622_1606.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0004_auto_20150622_1606.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0005_auto_20150723_1508.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0005_auto_20150723_1508.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0006_person_groups.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0006_person_groups.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0007_copy_group.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0007_copy_group.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0009_auto_20150724_1654.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0009_auto_20150724_1654.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0010_auto_20150724_1654.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0010_auto_20150724_1654.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0011_auto_20150724_1900.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0011_auto_20150724_1900.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0012_auto_20150728_1114.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0012_auto_20150728_1114.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0014_auto_20150807_0033.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0014_auto_20150807_0033.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0015_m2m_remove_null.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0015_m2m_remove_null.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0016_person_fk_to_one_to_one.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0016_person_fk_to_one_to_one.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0017_auto_20160109_1951.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0017_auto_20160109_1951.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0018_auto_20160802_1852.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0018_auto_20160802_1852.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/migrations/0019_alter_group_id_alter_grouptranslation_id_and_more.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/migrations/0019_alter_group_id_alter_grouptranslation_id_and_more.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/models.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/search_indexes.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/search_indexes.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/group_list.html` & `djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/group_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/includes/group.html` & `djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/includes/group.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/includes/person.html` & `djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/includes/person.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/templates/aldryn_people/plugins/standard/people_list.html` & `djangocms-aldryn-people-3.0.1/aldryn_people/templates/aldryn_people/plugins/standard/people_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/templatetags/aldryn_people_tags.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/templatetags/aldryn_people_tags.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/tests/__init__.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/tests/test_admin.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/tests/test_app_hook.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/tests/test_app_hook.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/tests/test_models.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/tests/test_plugins.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/tests/test_search_indexes.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/tests/test_search_indexes.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/tests/test_toolbar.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/tests/test_toolbar.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/tests/test_views.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/urls.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/urls.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/utils.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/utils.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/vcard.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/vcard.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/aldryn_people/views.py` & `djangocms-aldryn-people-3.0.1/aldryn_people/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/djangocms_aldryn_people.egg-info/PKG-INFO` & `djangocms-aldryn-people-3.0.1/djangocms_aldryn_people.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: djangocms-aldryn-people
-Version: 3.0.0
+Version: 3.0.1
 Summary: Aldryn People publishes profile pages for people in your organisation including team members, collaborators, partners, clients, and so on, including photographs and address information.
 Home-page: https://github.com/CZ-NIC/djangocms-aldryn-people
 Author: Divio AG
 Author-email: info@divio.ch
-License: BSD License
+License: BSD
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
@@ -58,22 +58,22 @@
 
 We're grateful to all contributors who have helped create and maintain this package.
 
 Contributors are listed at `contributions page
 <https://github.com/aldryn/aldryn-translation-tools/graphs/contributors>`_.
 
 
-.. |Project continuation| image:: https://img.shields.io/badge/Continuation-Divio_Aldryn_Search-blue
+.. |Project continuation| image:: https://img.shields.io/badge/Continuation-Divio_Aldryn_People-blue
     :target: https://github.com/CZ-NIC/djangocms-aldryn-people
     :alt: Continuation of the deprecated project "Divio Aldryn People"
 .. |Pypi package| image:: https://img.shields.io/pypi/v/djangocms-aldryn-people.svg
     :target: https://pypi.python.org/pypi/djangocms-aldryn-people/
     :alt: Pypi package
 .. |Pypi status| image:: https://img.shields.io/pypi/status/djangocms-aldryn-people.svg
    :target: https://pypi.python.org/pypi/djangocms-aldryn-people
    :alt: status
 .. |Python versions| image:: https://img.shields.io/pypi/pyversions/djangocms-aldryn-people.svg
    :target: https://pypi.python.org/pypi/djangocms-aldryn-people
    :alt: Python versions
 .. |License| image:: https://img.shields.io/pypi/l/djangocms-aldryn-people.svg
-    :target: https://pypi.python.org/pypi/djangocms-aldryn-people/
+    :target: https://github.com/CZ-NIC/djangocms-aldryn-people/blob/master/LICENSE.txt
     :alt: license
```

### Comparing `djangocms-aldryn-people-3.0.0/djangocms_aldryn_people.egg-info/SOURCES.txt` & `djangocms-aldryn-people-3.0.1/djangocms_aldryn_people.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/setup.cfg` & `djangocms-aldryn-people-3.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-people-3.0.0/setup.py` & `djangocms-aldryn-people-3.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from aldryn_people import __version__
 
 
 REQUIREMENTS = [
     'djangocms-aldryn-common',
     'djangocms-aldryn-translation-tools',
     'django-filer',
-    'easy-thumbnails',
+    'easy-thumbnails[svg]',
     'phonenumbers',
 ]
 
 # https://pypi.python.org/pypi?%3Aaction=list_classifiers
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
@@ -38,15 +38,15 @@
                 'organisation including team members, collaborators, '
                 'partners, clients, and so on, including photographs and '
                 'address information.',
     author='Divio AG',
     author_email='info@divio.ch',
     url='https://github.com/CZ-NIC/djangocms-aldryn-people',
     packages=find_packages(),
-    license='BSD License',
+    license='BSD',
     platforms=['OS Independent'],
     install_requires=REQUIREMENTS,
     classifiers=CLASSIFIERS,
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     include_package_data=True,
     zip_safe=False,
```

