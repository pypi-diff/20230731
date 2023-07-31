# Comparing `tmp/django-camomilla-cms-5.8.5.tar.gz` & `tmp/django-camomilla-cms-6.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-camomilla-cms-5.8.5.tar", last modified: Tue Mar  7 17:22:08 2023, max compression
+gzip compressed data, was "django-camomilla-cms-6.0.0b1.tar", last modified: Mon Jul 31 09:05:06 2023, max compression
```

## Comparing `django-camomilla-cms-5.8.5.tar` & `django-camomilla-cms-6.0.0b1.tar`

### file list

```diff
@@ -1,109 +1,136 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.304860 django-camomilla-cms-5.8.5/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      224 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1699 2023-03-07 17:22:08.304860 django-camomilla-cms-5.8.5/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     1163 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.292860 django-camomilla-cms-5.8.5/camomilla/
--rwxr-xr-x   0 root         (0) root         (0)      111 2023-03-07 17:22:06.000000 django-camomilla-cms-5.8.5/camomilla/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2362 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/admin.py
--rwxr-xr-x   0 root         (0) root         (0)      188 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/apps.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/authentication.py
--rw-r--r--   0 root         (0) root         (0)     1220 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/defaults.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.292860 django-camomilla-cms-5.8.5/camomilla/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.292860 django-camomilla-cms-5.8.5/camomilla/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/management/commands/regenerate_thumbnails.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.296860 django-camomilla-cms-5.8.5/camomilla/migrations/
--rw-r--r--   0 root         (0) root         (0)    21066 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/migrations/0002_auto_20200214_1127.py
--rw-r--r--   0 root         (0) root         (0)      795 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/migrations/0003_auto_20210130_1610.py
--rw-r--r--   0 root         (0) root         (0)      616 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/migrations/0004_auto_20210511_0937.py
--rw-r--r--   0 root         (0) root         (0)      418 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/migrations/0005_media_image_props.py
--rw-r--r--   0 root         (0) root         (0)      896 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/migrations/0006_auto_20220103_1845.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/migrations/0007_auto_20220211_1622.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/migrations/0008_auto_20220309_1616.py
--rw-r--r--   0 root         (0) root         (0)     7230 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/migrations/0009_article__hvad_query_category__hvad_query_and_more.py
--rw-r--r--   0 root         (0) root         (0)     3245 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/migrations/0010_auto_20220802_1406.py
--rw-r--r--   0 root         (0) root         (0)      316 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/migrations/0011_auto_20220902_1000.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.296860 django-camomilla-cms-5.8.5/camomilla/models/
--rw-r--r--   0 root         (0) root         (0)      130 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1765 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/models/article.py
--rw-r--r--   0 root         (0) root         (0)      738 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/models/category.py
--rw-r--r--   0 root         (0) root         (0)     1229 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/models/content.py
--rw-r--r--   0 root         (0) root         (0)     7378 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/models/media.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.296860 django-camomilla-cms-5.8.5/camomilla/models/mixins/
--rw-r--r--   0 root         (0) root         (0)     2273 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/models/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/models/page.py
--rw-r--r--   0 root         (0) root         (0)      422 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/models/tag.py
--rw-r--r--   0 root         (0) root         (0)     1976 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/parsers.py
--rwxr-xr-x   0 root         (0) root         (0)     1813 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.296860 django-camomilla-cms-5.8.5/camomilla/serializers/
--rw-r--r--   0 root         (0) root         (0)      128 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/serializers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      469 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/serializers/article.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.296860 django-camomilla-cms-5.8.5/camomilla/serializers/base/
--rw-r--r--   0 root         (0) root         (0)      749 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/serializers/base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.296860 django-camomilla-cms-5.8.5/camomilla/serializers/fields/
--rw-r--r--   0 root         (0) root         (0)      703 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/serializers/fields/__init__.py
--rw-r--r--   0 root         (0) root         (0)      648 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/serializers/fields/file.py
--rw-r--r--   0 root         (0) root         (0)     4402 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/serializers/fields/related.py
--rw-r--r--   0 root         (0) root         (0)     2041 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/serializers/media.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.296860 django-camomilla-cms-5.8.5/camomilla/serializers/mixins/
--rw-r--r--   0 root         (0) root         (0)     6905 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/serializers/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      333 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/serializers/page.py
--rw-r--r--   0 root         (0) root         (0)     3608 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/serializers/user.py
--rw-r--r--   0 root         (0) root         (0)      341 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/storages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.292860 django-camomilla-cms-5.8.5/camomilla/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.292860 django-camomilla-cms-5.8.5/camomilla/templates/camomilla/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.296860 django-camomilla-cms-5.8.5/camomilla/templates/camomilla/widgets/
--rw-r--r--   0 root         (0) root         (0)     3727 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/templates/camomilla/widgets/media_select_multiple.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.296860 django-camomilla-cms-5.8.5/camomilla/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/templatetags/camomilla_filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.300860 django-camomilla-cms-5.8.5/camomilla/theme/
--rwxr-xr-x   0 root         (0) root         (0)       22 2023-03-07 17:22:06.000000 django-camomilla-cms-5.8.5/camomilla/theme/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.292860 django-camomilla-cms-5.8.5/camomilla/theme/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.292860 django-camomilla-cms-5.8.5/camomilla/theme/static/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.300860 django-camomilla-cms-5.8.5/camomilla/theme/static/admin/css/
--rwxr-xr-x   0 root         (0) root         (0)    16681 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/theme/static/admin/css/responsive.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.300860 django-camomilla-cms-5.8.5/camomilla/theme/static/admin/img/
--rw-r--r--   0 root         (0) root         (0)    18821 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/theme/static/admin/img/logo.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.292860 django-camomilla-cms-5.8.5/camomilla/theme/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.300860 django-camomilla-cms-5.8.5/camomilla/theme/templates/admin/
--rwxr-xr-x   0 root         (0) root         (0)      585 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/theme/templates/admin/base_site.html
--rwxr-xr-x   0 root         (0) root         (0)     1562 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/urls.py
--rw-r--r--   0 root         (0) root         (0)     3434 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.300860 django-camomilla-cms-5.8.5/camomilla/views/
--rw-r--r--   0 root         (0) root         (0)      183 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/views/articles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.300860 django-camomilla-cms-5.8.5/camomilla/views/base/
--rw-r--r--   0 root         (0) root         (0)      222 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/views/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      456 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/views/categories.py
--rw-r--r--   0 root         (0) root         (0)     1377 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/views/contents.py
--rw-r--r--   0 root         (0) root         (0)      441 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/views/languages.py
--rw-r--r--   0 root         (0) root         (0)     2871 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/views/medias.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.300860 django-camomilla-cms-5.8.5/camomilla/views/mixins/
--rw-r--r--   0 root         (0) root         (0)     2617 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/views/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4765 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/views/mixins/ordering.py
--rw-r--r--   0 root         (0) root         (0)     5956 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/views/mixins/pagination.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/views/pages.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/views/tags.py
--rw-r--r--   0 root         (0) root         (0)     3134 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/camomilla/views/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.300860 django-camomilla-cms-5.8.5/django_camomilla_cms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1699 2023-03-07 17:22:08.000000 django-camomilla-cms-5.8.5/django_camomilla_cms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2631 2023-03-07 17:22:08.000000 django-camomilla-cms-5.8.5/django_camomilla_cms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-07 17:22:08.000000 django-camomilla-cms-5.8.5/django_camomilla_cms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      193 2023-03-07 17:22:08.000000 django-camomilla-cms-5.8.5/django_camomilla_cms.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-03-07 17:22:08.000000 django-camomilla-cms-5.8.5/django_camomilla_cms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      979 2023-03-07 17:22:08.304860 django-camomilla-cms-5.8.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       80 2023-03-07 17:22:06.000000 django-camomilla-cms-5.8.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-07 17:22:08.304860 django-camomilla-cms-5.8.5/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2358 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     1848 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/tests/test_camomilla_filters.py
--rw-r--r--   0 root         (0) root         (0)      684 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/tests/test_models.py
--rw-r--r--   0 root         (0) root         (0)     3613 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)      562 2023-03-07 17:22:05.000000 django-camomilla-cms-5.8.5/tests/urls.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.926345 django-camomilla-cms-6.0.0b1/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1063 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/LICENSE
+-rw-r--r--   0 bnznamco   (502) staff       (20)      224 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/MANIFEST.in
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1795 2023-07-31 09:05:06.926421 django-camomilla-cms-6.0.0b1/PKG-INFO
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)     1259 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/README.md
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.912175 django-camomilla-cms-6.0.0b1/camomilla/
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)      110 2023-07-31 09:03:58.000000 django-camomilla-cms-6.0.0b1/camomilla/__init__.py
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)     2557 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/admin.py
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)      497 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/apps.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      855 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/authentication.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      165 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/context_processors.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.912317 django-camomilla-cms-6.0.0b1/camomilla/contrib/
+-rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/contrib/__init__.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.912546 django-camomilla-cms-6.0.0b1/camomilla/contrib/modeltranslation/
+-rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/contrib/modeltranslation/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     4883 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/contrib/modeltranslation/hvad_migration.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.912836 django-camomilla-cms-6.0.0b1/camomilla/contrib/rest_framework/
+-rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/contrib/rest_framework/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2621 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/contrib/rest_framework/serializer.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1220 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/defaults.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      502 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/dynamic_pages_urls.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      111 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/camomilla/exceptions.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.913092 django-camomilla-cms-6.0.0b1/camomilla/fields/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      400 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/fields/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1867 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/fields/json.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.913216 django-camomilla-cms-6.0.0b1/camomilla/management/
+-rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/camomilla/management/__init__.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.913470 django-camomilla-cms-6.0.0b1/camomilla/management/commands/
+-rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/camomilla/management/commands/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      497 2023-07-18 12:13:50.000000 django-camomilla-cms-6.0.0b1/camomilla/management/commands/regenerate_thumbnails.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2222 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/model_api.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.914375 django-camomilla-cms-6.0.0b1/camomilla/models/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      151 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/models/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1194 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/models/article.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      956 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/models/content.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     6844 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/models/media.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2901 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/models/menu.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.914525 django-camomilla-cms-6.0.0b1/camomilla/models/mixins/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1225 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/models/mixins/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)    11975 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/models/page.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1976 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/parsers.py
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)     1813 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/permissions.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.915799 django-camomilla-cms-6.0.0b1/camomilla/serializers/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      176 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      401 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/article.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.915926 django-camomilla-cms-6.0.0b1/camomilla/serializers/base/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      488 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/base/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      557 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/content_type.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.916461 django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      528 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      648 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/file.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3474 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/json.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     4402 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/related.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1940 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/media.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      552 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/menu.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.916614 django-camomilla-cms-6.0.0b1/camomilla/serializers/mixins/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     5555 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/mixins/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      405 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/page.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3707 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/user.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      875 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/utils.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1765 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/validators.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2565 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/settings.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.917052 django-camomilla-cms-6.0.0b1/camomilla/storages/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      131 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/storages/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1997 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/storages/optimize.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      343 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/storages/overwrite.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.917544 django-camomilla-cms-6.0.0b1/camomilla/structured/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3957 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/structured/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     8475 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/structured/fields.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     4759 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/structured/models.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.906836 django-camomilla-cms-6.0.0b1/camomilla/templates/
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.917708 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.917890 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/articles/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      239 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/articles/default.html
+-rw-r--r--   0 bnznamco   (502) staff       (20)     6638 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/base.html
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.918058 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/pages/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      144 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/pages/default.html
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.918518 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/parts/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2970 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/parts/langswitch.html
+-rw-r--r--   0 bnznamco   (502) staff       (20)      338 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/parts/menu.html
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.918832 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/widgets/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3727 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/widgets/media_select_multiple.html
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.919334 django-camomilla-cms-6.0.0b1/camomilla/templatetags/
+-rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/camomilla/templatetags/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      563 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templatetags/camomilla_filters.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      862 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templatetags/menus.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.919474 django-camomilla-cms-6.0.0b1/camomilla/theme/
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)       29 2023-07-31 09:03:58.000000 django-camomilla-cms-6.0.0b1/camomilla/theme/__init__.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.907704 django-camomilla-cms-6.0.0b1/camomilla/theme/static/
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.907873 django-camomilla-cms-6.0.0b1/camomilla/theme/static/admin/
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.919632 django-camomilla-cms-6.0.0b1/camomilla/theme/static/admin/css/
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)    16681 2023-07-20 08:16:23.000000 django-camomilla-cms-6.0.0b1/camomilla/theme/static/admin/css/responsive.css
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.920109 django-camomilla-cms-6.0.0b1/camomilla/theme/static/admin/img/
+-rw-r--r--   0 bnznamco   (502) staff       (20)    18821 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/camomilla/theme/static/admin/img/logo.png
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.908058 django-camomilla-cms-6.0.0b1/camomilla/theme/templates/
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.920855 django-camomilla-cms-6.0.0b1/camomilla/theme/templates/admin/
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)      585 2023-07-20 08:16:25.000000 django-camomilla-cms-6.0.0b1/camomilla/theme/templates/admin/base_site.html
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1261 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/translation.py
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)     1716 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/urls.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.921934 django-camomilla-cms-6.0.0b1/camomilla/utils/
+-rw-r--r--   0 bnznamco   (502) staff       (20)       74 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/utils/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      520 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/utils/getters.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      255 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/utils/normalization.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3324 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/utils/seo.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2273 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/utils/translation.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.923313 django-camomilla-cms-6.0.0b1/camomilla/views/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      177 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      572 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/articles.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.923473 django-camomilla-cms-6.0.0b1/camomilla/views/base/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      222 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/views/base/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1206 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/contents.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      441 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/camomilla/views/languages.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3002 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/medias.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1686 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/menus.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.923892 django-camomilla-cms-6.0.0b1/camomilla/views/mixins/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2438 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/mixins/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     4779 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/mixins/ordering.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     5956 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/views/mixins/pagination.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      486 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/pages.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      480 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/tags.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3132 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/users.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.924633 django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1795 2023-07-31 09:05:06.000000 django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/PKG-INFO
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3135 2023-07-31 09:05:06.000000 django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/SOURCES.txt
+-rw-r--r--   0 bnznamco   (502) staff       (20)        1 2023-07-31 09:05:06.000000 django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/dependency_links.txt
+-rw-r--r--   0 bnznamco   (502) staff       (20)      219 2023-07-31 09:05:06.000000 django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/requires.txt
+-rw-r--r--   0 bnznamco   (502) staff       (20)       16 2023-07-31 09:05:06.000000 django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/top_level.txt
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1018 2023-07-31 09:05:06.926745 django-camomilla-cms-6.0.0b1/setup.cfg
+-rw-r--r--   0 bnznamco   (502) staff       (20)       87 2023-07-31 09:03:58.000000 django-camomilla-cms-6.0.0b1/setup.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.926200 django-camomilla-cms-6.0.0b1/tests/
+-rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/tests/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2347 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/tests/test_api.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1848 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/tests/test_camomilla_filters.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      684 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/tests/test_models.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3613 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/tests/test_utils.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      562 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/tests/urls.py
```

### Comparing `django-camomilla-cms-5.8.5/LICENSE` & `django-camomilla-cms-6.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-5.8.5/PKG-INFO` & `django-camomilla-cms-6.0.0b1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 Metadata-Version: 2.1
 Name: django-camomilla-cms
-Version: 5.8.5
+Version: 6.0.0b1
 Summary: Django powered cms
 Home-page: https://github.com/lotrekagency/camomilla
 Author: Lotrèk
 Author-email: dimmitutto@lotrek.it
 License: MIT
 Keywords: cms,django,api cms
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.0.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# camomilla cms [![PyPI](https://img.shields.io/pypi/v/django-camomilla-cms?style=flat-square)](https://pypi.org/project/django-camomilla-cms) ![Codecov](https://img.shields.io/codecov/c/github/lotrekagency/camomilla?style=flat-square) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/lotrekagency/camomilla/Test,%20Coverage%20and%20Release?style=flat-square) [![GitHub](https://img.shields.io/github/license/lotrekagency/camomilla?style=flat-square)](./LICENSE)
+# camomilla django cms [![PyPI](https://img.shields.io/pypi/v/django-camomilla-cms?style=flat-square)](https://pypi.org/project/django-camomilla-cms) ![Codecov](https://img.shields.io/codecov/c/github/lotrekagency/camomilla?style=flat-square) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/lotrekagency/camomilla/Test,%20Coverage%20and%20Release?style=flat-square) [![GitHub](https://img.shields.io/github/license/lotrekagency/camomilla?style=flat-square)](./LICENSE)
 
-## Install
+## Install 
+
+```shell
+$ pip install django-camomilla-cms
+```
+
+## Setup 
+```shell
+$ mkdir -p camomilla_migrations
+$ touch camomilla_migrations.__init__.py
+$ python manage.py makemigrations camomilla
+$ python manage.py migrate camomilla
+```
 
-	$ pip install -r requirements.txt
 
 ## Settings
 
 Camomilla brings a lot of default settings you can include in your project's ones
 
     from camomilla.defaults import *
 
 Remember to add all the required applications in your project
 
-    INSTALLED_APPS = [
-        ...
-        'rest_framework',
-        'rest_framework.authtoken',
-        'camomilla',
-        'hvad',
-        ...
-    ]
+```python
+INSTALLED_APPS = [
+    ...
+    'camomilla',
+    'camomilla.theme',
+    'djsuperadmin',
+    'modeltranslation',
+    'djlotrek',
+    'rest_framework',
+    'rest_framework.authtoken',
+    ...
+]
+```
 
 ## Run the server
 
     $ python manage.py runserver
 
 ## Run tests
 
     pip install -r requirements-dev.txt
     make test
-
-## Don't fear the hvader
-
-Feel free to make your models untranslatable, [we have a nice solution for them](https://github.com/lotrekagency/hvad-migration)
-
```

### Comparing `django-camomilla-cms-5.8.5/README.md` & `django-camomilla-cms-6.0.0b1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,47 @@
-# camomilla cms [![PyPI](https://img.shields.io/pypi/v/django-camomilla-cms?style=flat-square)](https://pypi.org/project/django-camomilla-cms) ![Codecov](https://img.shields.io/codecov/c/github/lotrekagency/camomilla?style=flat-square) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/lotrekagency/camomilla/Test,%20Coverage%20and%20Release?style=flat-square) [![GitHub](https://img.shields.io/github/license/lotrekagency/camomilla?style=flat-square)](./LICENSE)
+# camomilla django cms [![PyPI](https://img.shields.io/pypi/v/django-camomilla-cms?style=flat-square)](https://pypi.org/project/django-camomilla-cms) ![Codecov](https://img.shields.io/codecov/c/github/lotrekagency/camomilla?style=flat-square) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/lotrekagency/camomilla/Test,%20Coverage%20and%20Release?style=flat-square) [![GitHub](https://img.shields.io/github/license/lotrekagency/camomilla?style=flat-square)](./LICENSE)
 
-## Install
+## Install 
+
+```shell
+$ pip install django-camomilla-cms
+```
+
+## Setup 
+```shell
+$ mkdir -p camomilla_migrations
+$ touch camomilla_migrations.__init__.py
+$ python manage.py makemigrations camomilla
+$ python manage.py migrate camomilla
+```
 
-	$ pip install -r requirements.txt
 
 ## Settings
 
 Camomilla brings a lot of default settings you can include in your project's ones
 
     from camomilla.defaults import *
 
 Remember to add all the required applications in your project
 
-    INSTALLED_APPS = [
-        ...
-        'rest_framework',
-        'rest_framework.authtoken',
-        'camomilla',
-        'hvad',
-        ...
-    ]
+```python
+INSTALLED_APPS = [
+    ...
+    'camomilla',
+    'camomilla.theme',
+    'djsuperadmin',
+    'modeltranslation',
+    'djlotrek',
+    'rest_framework',
+    'rest_framework.authtoken',
+    ...
+]
+```
 
 ## Run the server
 
     $ python manage.py runserver
 
 ## Run tests
 
     pip install -r requirements-dev.txt
     make test
-
-## Don't fear the hvader
-
-Feel free to make your models untranslatable, [we have a nice solution for them](https://github.com/lotrekagency/hvad-migration)
-
```

### Comparing `django-camomilla-cms-5.8.5/camomilla/authentication.py` & `django-camomilla-cms-6.0.0b1/camomilla/authentication.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-5.8.5/camomilla/defaults.py` & `django-camomilla-cms-6.0.0b1/camomilla/defaults.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-5.8.5/camomilla/fields.py` & `django-camomilla-cms-6.0.0b1/camomilla/fields/json.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 import json
+
 import django
 from django.conf import settings
+
 if django.VERSION >= (4, 0):
     from django.db.models import JSONField as DjangoJSONField
 else:
     from django.contrib.postgres.fields import JSONField as DjangoJSONField
+
 from django.contrib.postgres.fields import ArrayField as DjangoArrayField
 from django.db import models
 
 
-ORDERING_ACCEPTED_FIELDS = (
-    models.BigIntegerField,
-    models.IntegerField,
-    models.PositiveIntegerField,
-    models.PositiveSmallIntegerField,
-    models.SmallIntegerField,
-)
-
-
 class JSONField(DjangoJSONField):
     pass
 
 
 class ArrayField(DjangoArrayField):
     pass
```

### Comparing `django-camomilla-cms-5.8.5/camomilla/models/content.py` & `django-camomilla-cms-6.0.0b1/camomilla/models/content.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,15 @@
 from django.db import models
-
 from django.urls import reverse
-
-from hvad.models import TranslatableModel, TranslatedFields
-
 from djsuperadmin.mixins import DjSuperAdminMixin
 
 
-class BaseContent(DjSuperAdminMixin, TranslatableModel):
-    identifier = models.CharField(max_length=200)
-    translations = TranslatedFields(
-        title=models.CharField(max_length=200),
-        subtitle=models.CharField(max_length=200, blank=True, null=True, default=""),
-        permalink=models.CharField(max_length=200, blank=False, null=True),
-        content=models.TextField(default=""),
-    )
+class AbstractContent(DjSuperAdminMixin, models.Model):
+    identifier = models.TextField()
+    content = models.TextField(default="")
     page = models.ForeignKey(
         "camomilla.Page",
         blank=False,
         null=True,
         on_delete=models.SET_NULL,
         related_name="contents",
     )
@@ -29,15 +20,17 @@
 
     @property
     def superadmin_patch_url(self):
         return reverse("camomilla-content-djsuperadmin", kwargs={"pk": self.pk})
 
     class Meta:
         abstract = True
-        unique_together = [("page", "identifier")]
+        unique_together = ["identifier", "page"]
 
     def __str__(self):
+        if len(self.identifier) > 40:
+            return "%s..." % self.identifier[:40]
         return self.identifier
 
 
-class Content(BaseContent):
-    translations = TranslatedFields()
+class Content(AbstractContent):
+    pass
```

### Comparing `django-camomilla-cms-5.8.5/camomilla/models/media.py` & `django-camomilla-cms-6.0.0b1/camomilla/models/media.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 import json
 import os
-import magic
 from io import BytesIO
 
-from django.conf import settings
+import magic
 from django.core.exceptions import ValidationError
 from django.core.files.base import ContentFile
 from django.core.files.storage import default_storage as storage
 from django.db import models
 from django.db.models.fields.related import ForeignObjectRel
-from ..fields import JSONField
 from django.db.models.signals import post_save, pre_delete
 from django.dispatch import receiver
 from django.utils.safestring import mark_safe
+from django.utils.text import slugify
 from django.utils.translation import gettext_lazy as _
-from hvad.models import TranslatableModel, TranslatedFields
 from PIL import Image
 
+from camomilla.fields import JSONField
+from camomilla.settings import THUMBNAIL_FOLDER, THUMBNAIL_HEIGHT, THUMBNAIL_WIDTH
+from camomilla.storages.optimize import OptimizedStorage
 
-class BaseMediaFolder(TranslatableModel):
-    translations = TranslatedFields(
-        description=models.CharField(max_length=200, blank=True, null=True),
-        title=models.CharField(max_length=200, blank=True, null=True),
-    )
-    slug = models.SlugField()
+
+class AbstractMediaFolder(models.Model):
+    title = models.CharField(max_length=200)
+    slug = models.SlugField(editable=False, max_length=200, blank=True, null=True)
     creation_date = models.DateTimeField(auto_now_add=True)
     last_modified = models.DateTimeField(auto_now=True)
-    icon = models.ForeignKey(
-        "camomilla.Media",
-        on_delete=models.SET_NULL,
-        null=True,
-        blank=True,
-        verbose_name=_("Image cover"),
-    )
     path = models.TextField(blank=True, null=True)
     updir = models.ForeignKey(
         "self",
         on_delete=models.CASCADE,
         related_name="child_folders",
         null=True,
         blank=True,
@@ -46,51 +38,47 @@
         abstract = True
 
     def update_childs(self):
         for folder in self.child_folders.all():
             folder.save()
 
     def save(self, *args, **kwargs):
+        self.slug = slugify(self.title)
         if self.updir:
             if self.updir.id == self.id:
                 raise ValidationError({"updir": "Unvalid parent"})
             self.path = "{0}/{1}".format(self.updir.path, self.slug)
-
         else:
             self.path = "/{0}".format(self.slug)
 
-        super(BaseMediaFolder, self).save(*args, **kwargs)
+        super().save(*args, **kwargs)
         self.update_childs()
 
     def __str__(self):
-        to_string = self.slug
-        if self.title:
-            to_string += " - " + self.title
-        return to_string
+        return "[%s] %s" % (self.__class__.__name__, self.name)
 
 
-class MediaFolder(BaseMediaFolder):
-    translations = TranslatedFields()
+class MediaFolder(AbstractMediaFolder):
+    pass
 
 
-class Media(TranslatableModel):
-    translations = TranslatedFields(
-        alt_text=models.CharField(max_length=200, blank=True, null=True),
-        title=models.CharField(max_length=200, blank=True, null=True),
-        description=models.TextField(blank=True, null=True),
-    )
-    file = models.FileField()
+class Media(models.Model):
+    # Seo Attributes
+    alt_text = models.CharField(max_length=200, blank=True, null=True)
+    title = models.CharField(max_length=200, blank=True, null=True)
+    description = models.TextField(blank=True, null=True)
+
+    file = models.FileField(storage=OptimizedStorage())
     thumbnail = models.ImageField(
-        upload_to=getattr(settings, "THUMB_FOLDER", "thumbnails"),
+        upload_to=THUMBNAIL_FOLDER,
         max_length=500,
         null=True,
         blank=True,
     )
     created = models.DateTimeField(auto_now=True)
-    name = models.CharField(max_length=200, blank=True, null=True)
     size = models.IntegerField(default=0, blank=True, null=True)
     mime_type = models.CharField(max_length=128, blank=True, null=True)
     image_props = JSONField(default=dict, blank=True)
     folder = models.ForeignKey(
         MediaFolder,
         null=True,
         blank=True,
@@ -117,14 +105,15 @@
     image_preview.short_description = _("Preview")
     image_thumb_preview.short_description = _("Thumbnail")
 
     class Meta:
         ordering = ["-pk"]
 
     def regenerate_thumbnail(self):
+        self._remove_thumbnail()
         if self.file:
             self._make_thumbnail()
 
     def get_foreign_fields(self):
         return [
             field.get_accessor_name()
             for field in self._meta.get_fields()
@@ -136,101 +125,86 @@
         json_r = {
             "id": self.pk,
             "thumbnail": "" if not self.is_image else self.thumbnail.url,
             "label": self.__str__(),
         }
         return json.dumps(json_r)
 
-    def _make_thumbnail(self):
-        try:
-            fh = storage.open(self.file.name, "rb")
-            self.mime_type = magic.from_buffer(fh.read(2048), mime=True)
-        except FileNotFoundError as ex:
-            print(ex)
-            self.image_props = {}
-            self.mime_type = ""
-            return False
+    def _update_file_info(self, img_bytes=None):
         try:
-            orig_image = Image.open(fh)
-            image = orig_image.copy()
-            self.image_props = {
-                "width": orig_image.width,
-                "height": orig_image.height,
-                "format": orig_image.format,
-                "mode": orig_image.mode,
-            }
+            if not img_bytes:
+                img_bytes = self.file.storage.open(self.file.name, "rb")
+            self.mime_type = magic.from_buffer(img_bytes.read(2048), mime=True)
+            with Image.open(img_bytes) as image:
+                self.image_props = {
+                    "width": image.width,
+                    "height": image.height,
+                    "format": image.format,
+                    "mode": image.mode,
+                }
         except Exception as ex:
             print(ex)
             return False
 
+    def _make_thumbnail(self, img_bytes=None):
         try:
-            image.thumbnail(
-                (
-                    getattr(settings, "CAMOMILLA_THUMBNAIL_WIDTH", 50),
-                    getattr(settings, "CAMOMILLA_THUMBNAIL_HEIGHT", 50),
-                ),
-                Image.ANTIALIAS,
-            )
-            fh.close()
-
-            # Path to save to, name, and extension
-            thumb_name, thumb_extension = os.path.splitext(self.file.name)
-            thumb_extension = thumb_extension.lower()
-
-            thumb_filename = thumb_name + "_thumb" + thumb_extension
-
-            temp_thumb = BytesIO()
-            image.save(temp_thumb, "PNG", optimize=True)
-            temp_thumb.seek(0)
-
-            # Load a ContentFile into the thumbnail field so it gets saved
-            self.thumbnail.save(
-                thumb_filename, ContentFile(temp_thumb.read()), save=False
-            )
-            temp_thumb.close()
+            if not img_bytes:
+                img_bytes = self.file.storage.open(self.file.name, "rb")
+            with Image.open(img_bytes) as orig_image:
+                image = orig_image.copy()
+                image.thumbnail((THUMBNAIL_WIDTH, THUMBNAIL_HEIGHT), Image.ANTIALIAS)
+
+                # Path to save to, name, and extension
+                thumb_name, thumb_extension = os.path.splitext(self.file.name)
+                thumb_extension = thumb_extension.lower()
+                thumb_filename = thumb_name + "_thumb" + thumb_extension
+                temp_thumb = BytesIO()
+                image.save(temp_thumb, "PNG", optimize=True)
+                temp_thumb.seek(0)
+                # Load a ContentFile into the thumbnail field so it gets saved
+                self.thumbnail.save(
+                    thumb_filename, ContentFile(temp_thumb.read()), save=False
+                )
+                temp_thumb.close()
         except Exception:
             return False
 
         return True
 
     def _remove_file(self):
         if self.file:
-            file_to_remove = os.path.join(settings.MEDIA_ROOT, self.file.name)
-            if os.path.isfile(file_to_remove):
-                os.remove(file_to_remove)
+            self.file.storage.delete(self.file.name)
 
     def _remove_thumbnail(self):
         if self.thumbnail:
-            file_to_remove = os.path.join(settings.MEDIA_ROOT, self.thumbnail.name)
-            if os.path.isfile(file_to_remove):
-                os.remove(file_to_remove)
+            self.thumbnail.storage.delete(self.thumbnail.name)
 
     def _get_file_size(self):
-        if self.file:
-            file_to_calc = os.path.join(settings.MEDIA_ROOT, self.file.name)
-            if os.path.isfile(file_to_calc):
-                return self.file.size
-            else:
-                return 0
+        try:
+            return self.file.storage.size(self.file.name)
+        except:
+            return 0
 
     def __str__(self):
-        if self.name:
-            return self.name
+        if self.title:
+            return self.title
         return self.file.name
 
 
 @receiver(post_save, sender=Media, dispatch_uid="make thumbnails")
-def update_media(sender, instance, **kwargs):
+def update_media(sender, instance: Media, **kwargs):
     instance._remove_thumbnail()
-    instance._make_thumbnail()
+    image_bytes = instance.file.storage.open(instance.file.name, "rb")
+    instance._update_file_info(image_bytes)
+    instance._make_thumbnail(image_bytes)
     Media.objects.filter(pk=instance.pk).update(
         size=instance._get_file_size(),
         thumbnail=instance.thumbnail,
         mime_type=instance.mime_type,
         image_props=instance.image_props,
     )
 
 
 @receiver(pre_delete, sender=Media, dispatch_uid="make thumbnails")
-def delete_media_files(sender, instance, **kwargs):
+def delete_media_files(sender, instance: Media, **kwargs):
     instance._remove_thumbnail()
     instance._remove_file()
```

### Comparing `django-camomilla-cms-5.8.5/camomilla/parsers.py` & `django-camomilla-cms-6.0.0b1/camomilla/parsers.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-5.8.5/camomilla/permissions.py` & `django-camomilla-cms-6.0.0b1/camomilla/permissions.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-5.8.5/camomilla/serializers/base/__init__.py` & `django-camomilla-cms-6.0.0b1/camomilla/serializers/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-from hvad.contrib.restframework import TranslatableModelSerializer
-from rest_framework import serializers
+def build_standard_model_serializer(model, depth, bases=None):
+    if bases is None:
+        from rest_framework.serializers import ModelSerializer
+        from camomilla.serializers.fields import FieldsOverrideMixin
+        from camomilla.serializers.mixins import (
+            JSONFieldPatchMixin,
+            NestMixin,
+            OrderingMixin,
+            SetupEagerLoadingMixin,
+        )
 
-from ..fields import FieldsOverrideMixin, TranslatableFieldsOverrideMixin
-from ..mixins import (
-    JSONFieldPatchMixin,
-    LangInfoMixin,
-    OrderingMixin,
-    SetupEagerLoadingMixin,
-    TranslationSetMixin,
-    NestMixin,
-)
-
-
-class BaseModelSerializer(
-    NestMixin,
-    FieldsOverrideMixin,
-    JSONFieldPatchMixin,
-    OrderingMixin,
-    SetupEagerLoadingMixin,
-    serializers.ModelSerializer,
-):
-    pass
-
-
-class BaseTranslatableModelSerializer(
-    NestMixin,
-    TranslatableFieldsOverrideMixin,
-    JSONFieldPatchMixin,
-    OrderingMixin,
-    LangInfoMixin,
-    TranslationSetMixin,
-    TranslatableModelSerializer,
-):
-    pass
+        bases = (
+            NestMixin,
+            FieldsOverrideMixin,
+            JSONFieldPatchMixin,
+            OrderingMixin,
+            SetupEagerLoadingMixin,
+            ModelSerializer,
+        )
+    return type(
+        f"{model.__name__}StandardSerializer",
+        bases,
+        {
+            "Meta": type(
+                "Meta",
+                (object,),
+                {"model": model, "depth": depth, "fields": "__all__"},
+            )
+        },
+    )
```

### Comparing `django-camomilla-cms-5.8.5/camomilla/serializers/fields/__init__.py` & `django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-from .related import RelatedField
-from .file import ImageField, FileField
-from hvad.contrib.restframework import TranslatableModelSerializer
 from django.db import models
 from rest_framework import serializers
 
+from camomilla import structured
+
+from .json import StructuredJSONField
+from .file import FileField, ImageField
+from .related import RelatedField
+
 
 class FieldsOverrideMixin:
     serializer_field_mapping = {
         **serializers.ModelSerializer.serializer_field_mapping,
         models.FileField: FileField,
         models.ImageField: ImageField,
+        structured.StructuredJSONField: StructuredJSONField,
     }
     serializer_related_field = RelatedField
-
-
-class TranslatableFieldsOverrideMixin(FieldsOverrideMixin):
-
-    serializer_field_mapping = {
-        **TranslatableModelSerializer.serializer_field_mapping,
-        models.FileField: FileField,
-        models.ImageField: ImageField,
-    }
```

### Comparing `django-camomilla-cms-5.8.5/camomilla/serializers/fields/file.py` & `django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/file.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-5.8.5/camomilla/serializers/fields/related.py` & `django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/related.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-5.8.5/camomilla/serializers/media.py` & `django-camomilla-cms-6.0.0b1/camomilla/serializers/media.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 from rest_framework import serializers
 
-from ..models import Media, MediaFolder
-from ..storages import OverwriteStorage
-from .base import BaseTranslatableModelSerializer
+from camomilla.models import Media, MediaFolder
+from camomilla.serializers.base import BaseModelSerializer
+from camomilla.storages import OverwriteStorage
 
 
-class MediaListSerializer(BaseTranslatableModelSerializer):
+class MediaListSerializer(BaseModelSerializer):
     is_image = serializers.SerializerMethodField("get_is_image")
 
     def get_is_image(self, obj):
         return obj.is_image
 
     class Meta:
         model = Media
         fields = "__all__"
 
 
-class MediaSerializer(BaseTranslatableModelSerializer):
+class MediaSerializer(BaseModelSerializer):
     links = serializers.SerializerMethodField("get_linked_instances")
     is_image = serializers.SerializerMethodField("get_is_image")
 
     class Meta:
         model = Media
         fields = "__all__"
 
     def get_linked_instances(self, obj):
         result = []
         links = obj.get_foreign_fields()
         for link in links:
             manager = getattr(obj, link)
-            if hasattr(manager, "language"):
-                manager = manager.language()
             for item in manager.all():
                 if item.__class__.__name__ != "MediaTranslation":
                     result.append(
                         {
                             "model": item.__class__.__name__,
                             "name": item.__str__(),
                             "id": item.pk,
@@ -53,13 +51,13 @@
                 return instance
         return super().update(instance, data)
 
     def get_is_image(self, obj):
         return obj.is_image
 
 
-class MediaFolderSerializer(BaseTranslatableModelSerializer):
+class MediaFolderSerializer(BaseModelSerializer):
     icon = MediaSerializer(read_only=True)
 
     class Meta:
         model = MediaFolder
         fields = "__all__"
```

### Comparing `django-camomilla-cms-5.8.5/camomilla/serializers/user.py` & `django-camomilla-cms-6.0.0b1/camomilla/serializers/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.forms import ValidationError
-from .base import BaseModelSerializer
+from camomilla.serializers.base import BaseModelSerializer
 from django.contrib.auth import get_user_model, password_validation
 from django.contrib.auth.models import Permission
 from rest_framework import serializers
 from django.utils.translation import gettext_lazy as _
+from django.db.models import Q
 
 
 class PermissionSerializer(BaseModelSerializer):
     class Meta:
         model = Permission
         fields = "__all__"
 
@@ -35,16 +36,17 @@
             context=self.context,
             many=True,
         ).data
 
     def get_all_permissions(self, instance):
         return PermissionSerializer(
             Permission.objects.filter(
-                group__pk__in=instance.groups.values_list("pk", flat=True)
-            ).union(instance.user_permissions.all()),
+                Q(group__pk__in=instance.groups.values_list("pk", flat=True)) |
+                Q(pk__in=instance.user_permissions.values_list("pk", flat=True))
+            ),
             context=self.context,
             many=True,
         ).data
 
     def validate_password(self, value):
         password_validation.validate_password(value)
         return value
```

### Comparing `django-camomilla-cms-5.8.5/camomilla/templates/camomilla/widgets/media_select_multiple.html` & `django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/widgets/media_select_multiple.html`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-5.8.5/camomilla/templatetags/camomilla_filters.py` & `django-camomilla-cms-6.0.0b1/camomilla/templatetags/camomilla_filters.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,22 +3,18 @@
 
 
 register = template.Library()
 
 
 @register.filter(name="filter_content")
 def filter_content(page, args):
-    curr_lang = get_language()
     try:
-        content = page.contents.language(curr_lang).get(identifier=args)
+        content = page.contents.get(identifier=args)
     except page.contents.model.DoesNotExist:
         content, _ = page.contents.get_or_create(identifier=args)
-    if curr_lang not in content.translations.all_languages():
-        content.translate(curr_lang)
-        content.save()
     return content
 
 
 @register.filter(name="alternate_urls")
 def alternate_urls(page, request):
     alternates = page.alternate_urls(request)
     return alternates.get("alternate_urls", alternates).items()
```

### Comparing `django-camomilla-cms-5.8.5/camomilla/theme/static/admin/css/responsive.css` & `django-camomilla-cms-6.0.0b1/camomilla/theme/static/admin/css/responsive.css`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-5.8.5/camomilla/theme/static/admin/img/logo.png` & `django-camomilla-cms-6.0.0b1/camomilla/theme/static/admin/img/logo.png`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-5.8.5/camomilla/theme/templates/admin/base_site.html` & `django-camomilla-cms-6.0.0b1/camomilla/theme/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-5.8.5/camomilla/urls.py` & `django-camomilla-cms-6.0.0b1/camomilla/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,49 @@
-from .views import (
+from django.shortcuts import redirect
+from django.urls import include, path
+from rest_framework import routers
+from importlib.util import find_spec
+
+from camomilla.views import (
     ArticleViewSet,
-    CamomillaObtainAuthToken,
-    CamomillaAuthLogout,
     CamomillaAuthLogin,
-    CategoryViewSet,
+    CamomillaAuthLogout,
+    CamomillaObtainAuthToken,
+    ContentViewSet,
+    LanguageViewSet,
     MediaFolderViewSet,
+    MediaViewSet,
+    PageViewSet,
+    PermissionViewSet,
+    TagViewSet,
+    UserViewSet,
+    MenuViewSet,
 )
-from .views import TagViewSet, ContentViewSet, MediaViewSet, PermissionViewSet
-from .views import PageViewSet, LanguageViewSet, UserViewSet
-
-from django.urls import include, path
-from django.shortcuts import redirect
-
-from rest_framework import routers
 
 router = routers.DefaultRouter()
 
 router.register(r"tags", TagViewSet, "camomilla-tags")
-router.register(r"categories", CategoryViewSet, "camomilla-categories")
 router.register(r"articles", ArticleViewSet, "camomilla-articles")
 router.register(r"contents", ContentViewSet, "camomilla-content")
 router.register(r"media", MediaViewSet, "camomilla-media")
 router.register(r"media-folders", MediaFolderViewSet, "camomilla-media_folders")
 router.register(r"pages", PageViewSet, "camomilla-pages")
 router.register(r"sitemap", PageViewSet, "camomilla-sitemap")
 router.register(r"users", UserViewSet, "camomilla-users")
 router.register(r"permissions", PermissionViewSet, "camomilla-permissions")
-
+router.register(r"menus", MenuViewSet, "camomilla-menus")
 
 urlpatterns = [
     path("", include(router.urls)),
     path(
         "profiles/me/", lambda _: redirect("../../users/current/"), name="profiles-me"
     ),
     path("token-auth/", CamomillaObtainAuthToken.as_view(), name="api_token"),
     path("auth/login/", CamomillaAuthLogin.as_view(), name="login"),
     path("auth/logout/", CamomillaAuthLogout.as_view(), name="logout"),
     path("languages/", LanguageViewSet.as_view(), name="get_languages"),
 ]
+
+if find_spec("djsuperadmin.urls") is not None:
+    urlpatterns += [
+        path("djsuperadmin/", include("djsuperadmin.urls")),
+    ]
```

### Comparing `django-camomilla-cms-5.8.5/camomilla/utils.py` & `django-camomilla-cms-6.0.0b1/camomilla/utils/seo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 import urllib.parse
 
 from django.apps import apps
 from django.conf import settings
 from django.http import Http404
-from django.utils.translation import activate, get_language
 from django.urls import resolve, reverse
+from django.utils.translation import activate, get_language
+
+from camomilla.exceptions import NeedARedirect
+
 
-from .exceptions import NeedARedirect
+def is_page(model):
+    from camomilla.models import AbstractPage
+
+    return next(
+        (True for base in model.__bases__ if issubclass(base, AbstractPage)), False
+    )
 
 
 def get_host_url(request):
     if request:
         return "{0}://{1}".format(request.scheme, request.META["HTTP_HOST"])
 
 
@@ -38,15 +46,14 @@
     if not lang:
         lang = get_language()
     kwargs = {attr_page: identifier}
     try:
         page = model_page.objects.prefetch_related("contents").get(**kwargs)
     except model_page.DoesNotExist:
         page, _ = model_page.objects.get_or_create(**kwargs)
-    page.translate(lang)
     page = compile_seo(request, page, lang)
     return page
 
 
 def get_seo_model(request, model, **params):
     seo_obj = find_or_redirect(request, model, **params)
     return compile_seo(request, seo_obj, get_language())
@@ -69,36 +76,27 @@
     else:
         seo_obj.og_url = get_complete_url(request, seo_obj.og_url, lang)
     return seo_obj
 
 
 def find_or_redirect(request, obj_class, **kwargs):
     try:
-        obj = obj_class.objects.language().get(**kwargs)
+        obj = obj_class.objects.get(**kwargs)
         return obj
     except obj_class.DoesNotExist:
         cur_language = get_language()
         for language in settings.LANGUAGES:
             try:
                 activate(language[0])
-                obj = obj_class.objects.language().get(**kwargs)
+                obj = obj_class.objects.get(**kwargs)
                 activate(cur_language)
-                obj = obj_class.objects.language().get(pk=obj.pk)
+                obj = obj_class.objects.get(pk=obj.pk)
                 args = []
                 for kwarg_key, kwarg_val in kwargs.items():
                     args.append(getattr(obj, kwarg_key))
                 url_name = resolve(request.path_info).url_name
                 language_path = reverse(url_name, args=args)
                 raise NeedARedirect(language_path)
             except obj_class.DoesNotExist:
                 pass
         activate(cur_language)
         raise Http404()
-
-
-def dict_merge(dct, merge_dct):
-    for k, v in merge_dct.items():
-        if k in dct and isinstance(dct[k], dict) and isinstance(v, dict):  # noqa
-            dict_merge(dct[k], v)
-        else:
-            dct[k] = v
-    return dct
```

### Comparing `django-camomilla-cms-5.8.5/camomilla/views/articles.py` & `django-camomilla-cms-6.0.0b1/camomilla/views/articles.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from .base import BaseModelViewset
-from .mixins import GetUserLanguageMixin, BulkDeleteMixin
-
-from ..models import Article
-from ..serializers import ArticleSerializer
-from ..permissions import CamomillaBasePermissions
+from camomilla.models import Article
+from camomilla.permissions import CamomillaBasePermissions
+from camomilla.serializers import ArticleSerializer
+from camomilla.views.base import BaseModelViewset
+from camomilla.views.mixins import BulkDeleteMixin, GetUserLanguageMixin
 
 
 class ArticleViewSet(GetUserLanguageMixin, BulkDeleteMixin, BaseModelViewset):
 
     queryset = Article.objects.all()
     serializer_class = ArticleSerializer
     permission_classes = (CamomillaBasePermissions,)
```

### Comparing `django-camomilla-cms-5.8.5/camomilla/views/medias.py` & `django-camomilla-cms-6.0.0b1/camomilla/views/medias.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,24 @@
-from .base import BaseModelViewset
-from .mixins import BulkDeleteMixin, GetUserLanguageMixin, TrigramSearchMixin
-from ..parsers import MultipartJsonParser
-from ..permissions import CamomillaBasePermissions
-
-
-from rest_framework.response import Response
 from rest_framework.parsers import JSONParser
+from rest_framework.response import Response
 
-from ..models import Media, MediaFolder
-from ..serializers import MediaSerializer, MediaFolderSerializer, MediaListSerializer
+from camomilla.models import Media, MediaFolder
+from camomilla.parsers import MultipartJsonParser
+from camomilla.permissions import CamomillaBasePermissions
+from camomilla.serializers import (
+    MediaFolderSerializer,
+    MediaListSerializer,
+    MediaSerializer,
+)
+from camomilla.views.base import BaseModelViewset
+from camomilla.views.mixins import (
+    BulkDeleteMixin,
+    GetUserLanguageMixin,
+    TrigramSearchMixin,
+)
 
 
 class ParseMimeMixin(object):
     def parse_filter(self, filter):
         filter_name, value = filter.split("=")
         if filter_name == "mime_type":
             if value == "*/*":
@@ -25,34 +31,34 @@
 class MediaFolderViewSet(
     GetUserLanguageMixin, ParseMimeMixin, TrigramSearchMixin, BaseModelViewset
 ):
     model = MediaFolder
     serializer_class = MediaFolderSerializer
     permission_classes = (CamomillaBasePermissions,)
     items_per_page = 18
-    search_fields = ["name", "title", "alt_text"]
+    search_fields = ["title", "alt_text", "file"]
 
     def get_queryset(self):
         return self.model.objects.all()
 
     def get_serializer_context(self):
         return {**super().get_serializer_context(), "action": "list"}
 
     def get_mixed_response(self, request, *args, **kwargs):
-        updir = kwargs.get("pk", None)
+        search = self.request.GET.get("search", None)
+        all = self.request.GET.get("all", "false").lower() == 'true'
+        updir = None if all else kwargs.get("pk", None)
+        if not search and all:
+            self.search_fields = []
 
         parent_folder = MediaFolderSerializer(
             self.model.objects.filter(pk=updir).first()
         ).data
-        folder_queryset = self.model.objects.language(self.active_language).fallbacks().filter(updir__pk=updir)
-        media_queryset = (
-            Media.objects.language(self.active_language).fallbacks()
-            if request.GET.get("search", None)
-            else Media.objects.all()
-        ).filter(folder__pk=updir)
+        folder_queryset = self.model.objects.filter(updir__pk=updir)
+        media_queryset = Media.objects.filter(**({} if all else {"folder__pk": updir}))
 
         folder_data = MediaFolderSerializer(
             folder_queryset, many=True, context={"request": request}
         ).data
         media_data = self.format_output(
             *self.handle_pagination_stack(media_queryset),
             SerializerClass=MediaListSerializer
```

### Comparing `django-camomilla-cms-5.8.5/camomilla/views/mixins/__init__.py` & `django-camomilla-cms-6.0.0b1/camomilla/views/mixins/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,15 @@
         return self.active_language
 
     def initialize_request(self, request, *args, **kwargs):
         self._get_user_language(request)
         return super().initialize_request(request, *args, **kwargs)
 
     def get_queryset(self):
-        return (
-            self.model.objects.language(self.active_language).fallbacks().all()
-            if self.language_fallbacks
-            else self.model.objects.language(self.active_language).all()
-        )
+        return self.model.objects.all()
 
 
 class OptimViewMixin:
     def get_serializer_class(self):
         if hasattr(self, "action_serializers"):
             if self.action in self.action_serializers:
                 return self.action_serializers[self.action]
```

### Comparing `django-camomilla-cms-5.8.5/camomilla/views/mixins/ordering.py` & `django-camomilla-cms-6.0.0b1/camomilla/views/mixins/ordering.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from rest_framework.decorators import action
 from rest_framework.response import Response
-from ...permissions import CamomillaBasePermissions
+from camomilla.permissions import CamomillaBasePermissions
 from django.core.exceptions import ImproperlyConfigured
 from django.db import transaction, router
 from django.db.models.signals import post_save, pre_save
 from itertools import chain
 from django.db.models.expressions import F
-from ...fields import ORDERING_ACCEPTED_FIELDS
+from camomilla.fields import ORDERING_ACCEPTED_FIELDS
 
 
 class OrderingMixin:
     @action(
         detail=False, methods=["post"], permission_classes=(CamomillaBasePermissions,)
     )
     def update_order(self, request):
```

### Comparing `django-camomilla-cms-5.8.5/camomilla/views/mixins/pagination.py` & `django-camomilla-cms-6.0.0b1/camomilla/views/mixins/pagination.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-5.8.5/camomilla/views/users.py` & `django-camomilla-cms-6.0.0b1/camomilla/views/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-from .base import BaseModelViewset
-from django.contrib.auth import get_user_model
+from django.contrib.auth import get_user_model, login, logout
 from django.contrib.auth.models import Permission
-
 from django.db.models import Q
-
 from rest_framework.authtoken.models import Token
-from rest_framework.response import Response
 from rest_framework.authtoken.views import ObtainAuthToken
 from rest_framework.decorators import action
 from rest_framework.permissions import IsAuthenticated
+from rest_framework.response import Response
+from rest_framework.views import APIView
 
-from ..serializers import (
+from camomilla.permissions import CamomillaBasePermissions, CamomillaSuperUser, ReadOnly
+from camomilla.serializers import (
+    PermissionSerializer,
     UserProfileSerializer,
     UserSerializer,
-    PermissionSerializer,
 )
-from ..permissions import CamomillaSuperUser, CamomillaBasePermissions, ReadOnly
-from django.contrib.auth import login, logout
-from rest_framework.views import APIView
+from camomilla.views.base import BaseModelViewset
 
 
 class CamomillaObtainAuthToken(ObtainAuthToken):
     def post(self, request, *args, **kwargs):
         serializer = self.serializer_class(data=request.data)
         serializer.is_valid(raise_exception=True)
         user = serializer.validated_data["user"]
```

### Comparing `django-camomilla-cms-5.8.5/django_camomilla_cms.egg-info/PKG-INFO` & `django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 Metadata-Version: 2.1
 Name: django-camomilla-cms
-Version: 5.8.5
+Version: 6.0.0b1
 Summary: Django powered cms
 Home-page: https://github.com/lotrekagency/camomilla
 Author: Lotrèk
 Author-email: dimmitutto@lotrek.it
 License: MIT
 Keywords: cms,django,api cms
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.0.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# camomilla cms [![PyPI](https://img.shields.io/pypi/v/django-camomilla-cms?style=flat-square)](https://pypi.org/project/django-camomilla-cms) ![Codecov](https://img.shields.io/codecov/c/github/lotrekagency/camomilla?style=flat-square) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/lotrekagency/camomilla/Test,%20Coverage%20and%20Release?style=flat-square) [![GitHub](https://img.shields.io/github/license/lotrekagency/camomilla?style=flat-square)](./LICENSE)
+# camomilla django cms [![PyPI](https://img.shields.io/pypi/v/django-camomilla-cms?style=flat-square)](https://pypi.org/project/django-camomilla-cms) ![Codecov](https://img.shields.io/codecov/c/github/lotrekagency/camomilla?style=flat-square) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/lotrekagency/camomilla/Test,%20Coverage%20and%20Release?style=flat-square) [![GitHub](https://img.shields.io/github/license/lotrekagency/camomilla?style=flat-square)](./LICENSE)
 
-## Install
+## Install 
+
+```shell
+$ pip install django-camomilla-cms
+```
+
+## Setup 
+```shell
+$ mkdir -p camomilla_migrations
+$ touch camomilla_migrations.__init__.py
+$ python manage.py makemigrations camomilla
+$ python manage.py migrate camomilla
+```
 
-	$ pip install -r requirements.txt
 
 ## Settings
 
 Camomilla brings a lot of default settings you can include in your project's ones
 
     from camomilla.defaults import *
 
 Remember to add all the required applications in your project
 
-    INSTALLED_APPS = [
-        ...
-        'rest_framework',
-        'rest_framework.authtoken',
-        'camomilla',
-        'hvad',
-        ...
-    ]
+```python
+INSTALLED_APPS = [
+    ...
+    'camomilla',
+    'camomilla.theme',
+    'djsuperadmin',
+    'modeltranslation',
+    'djlotrek',
+    'rest_framework',
+    'rest_framework.authtoken',
+    ...
+]
+```
 
 ## Run the server
 
     $ python manage.py runserver
 
 ## Run tests
 
     pip install -r requirements-dev.txt
     make test
-
-## Don't fear the hvader
-
-Feel free to make your models untranslatable, [we have a nice solution for them](https://github.com/lotrekagency/hvad-migration)
-
```

### Comparing `django-camomilla-cms-5.8.5/django_camomilla_cms.egg-info/SOURCES.txt` & `django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,68 +3,86 @@
 README.md
 setup.cfg
 setup.py
 camomilla/__init__.py
 camomilla/admin.py
 camomilla/apps.py
 camomilla/authentication.py
+camomilla/context_processors.py
 camomilla/defaults.py
+camomilla/dynamic_pages_urls.py
 camomilla/exceptions.py
-camomilla/fields.py
+camomilla/model_api.py
 camomilla/parsers.py
 camomilla/permissions.py
-camomilla/storages.py
+camomilla/settings.py
+camomilla/translation.py
 camomilla/urls.py
-camomilla/utils.py
+camomilla/contrib/__init__.py
+camomilla/contrib/modeltranslation/__init__.py
+camomilla/contrib/modeltranslation/hvad_migration.py
+camomilla/contrib/rest_framework/__init__.py
+camomilla/contrib/rest_framework/serializer.py
+camomilla/fields/__init__.py
+camomilla/fields/json.py
 camomilla/management/__init__.py
 camomilla/management/commands/__init__.py
 camomilla/management/commands/regenerate_thumbnails.py
-camomilla/migrations/0001_initial.py
-camomilla/migrations/0002_auto_20200214_1127.py
-camomilla/migrations/0003_auto_20210130_1610.py
-camomilla/migrations/0004_auto_20210511_0937.py
-camomilla/migrations/0005_media_image_props.py
-camomilla/migrations/0006_auto_20220103_1845.py
-camomilla/migrations/0007_auto_20220211_1622.py
-camomilla/migrations/0008_auto_20220309_1616.py
-camomilla/migrations/0009_article__hvad_query_category__hvad_query_and_more.py
-camomilla/migrations/0010_auto_20220802_1406.py
-camomilla/migrations/0011_auto_20220902_1000.py
-camomilla/migrations/__init__.py
 camomilla/models/__init__.py
 camomilla/models/article.py
-camomilla/models/category.py
 camomilla/models/content.py
 camomilla/models/media.py
+camomilla/models/menu.py
 camomilla/models/page.py
-camomilla/models/tag.py
 camomilla/models/mixins/__init__.py
 camomilla/serializers/__init__.py
 camomilla/serializers/article.py
+camomilla/serializers/content_type.py
 camomilla/serializers/media.py
+camomilla/serializers/menu.py
 camomilla/serializers/page.py
 camomilla/serializers/user.py
+camomilla/serializers/utils.py
+camomilla/serializers/validators.py
 camomilla/serializers/base/__init__.py
 camomilla/serializers/fields/__init__.py
 camomilla/serializers/fields/file.py
+camomilla/serializers/fields/json.py
 camomilla/serializers/fields/related.py
 camomilla/serializers/mixins/__init__.py
-camomilla/templates/camomilla/widgets/media_select_multiple.html
+camomilla/storages/__init__.py
+camomilla/storages/optimize.py
+camomilla/storages/overwrite.py
+camomilla/structured/__init__.py
+camomilla/structured/fields.py
+camomilla/structured/models.py
+camomilla/templates/defaults/base.html
+camomilla/templates/defaults/articles/default.html
+camomilla/templates/defaults/pages/default.html
+camomilla/templates/defaults/parts/langswitch.html
+camomilla/templates/defaults/parts/menu.html
+camomilla/templates/defaults/widgets/media_select_multiple.html
 camomilla/templatetags/__init__.py
 camomilla/templatetags/camomilla_filters.py
+camomilla/templatetags/menus.py
 camomilla/theme/__init__.py
 camomilla/theme/static/admin/css/responsive.css
 camomilla/theme/static/admin/img/logo.png
 camomilla/theme/templates/admin/base_site.html
+camomilla/utils/__init__.py
+camomilla/utils/getters.py
+camomilla/utils/normalization.py
+camomilla/utils/seo.py
+camomilla/utils/translation.py
 camomilla/views/__init__.py
 camomilla/views/articles.py
-camomilla/views/categories.py
 camomilla/views/contents.py
 camomilla/views/languages.py
 camomilla/views/medias.py
+camomilla/views/menus.py
 camomilla/views/pages.py
 camomilla/views/tags.py
 camomilla/views/users.py
 camomilla/views/base/__init__.py
 camomilla/views/mixins/__init__.py
 camomilla/views/mixins/ordering.py
 camomilla/views/mixins/pagination.py
```

### Comparing `django-camomilla-cms-5.8.5/setup.cfg` & `django-camomilla-cms-6.0.0b1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 	Intended Audience :: Developers
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
 include_package_data = True
-python_requires = >= 3.0.*
+python_requires = >= 3.6
 install_requires = 
-	lotrek-django-hvad>=2.0.6
+	django-modeltranslation>=0.18.7
 	djsuperadmin>=0.9,<1.0.0
-	djangorestframework>=3.10.0<4.0.0
+	djangorestframework>=3.10.0,<4.0.0
 	djlotrek>=0.1.6,<1.0.0
 	Pillow>=6.2.0,<7.0.0
 	django-ckeditor>=5.7.1,<7.0.0
-	python-magic>=0.4<0.5
-	Django>=1.8
+	python-magic>=0.4,<0.5
+	jsonmodels==2.6.0
+	Django>=3.2
 
 [bdist_wheel]
 universal = true
 
 [semantic_release]
 version_variable = setup.py:__version__,camomilla/__init__.py:__version__,camomilla/theme/__init__.py:__version__
+branch = next
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django-camomilla-cms-5.8.5/tests/test_api.py` & `django-camomilla-cms-6.0.0b1/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pytest
 from django.contrib.auth.models import User
 from rest_framework.test import APIClient
 
-from camomilla.models import Tag, Category
-
+from camomilla.models import Tag
 client = APIClient()
 
 
 def login_superuser():
     User.objects.create_superuser("admin", "myemail@test.com", "adminadmin")
     response = client.post(
         "/api/camomilla/token-auth/", {"username": "admin", "password": "adminadmin"}
```

### Comparing `django-camomilla-cms-5.8.5/tests/test_camomilla_filters.py` & `django-camomilla-cms-6.0.0b1/tests/test_camomilla_filters.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-5.8.5/tests/test_models.py` & `django-camomilla-cms-6.0.0b1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-5.8.5/tests/test_utils.py` & `django-camomilla-cms-6.0.0b1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-5.8.5/tests/urls.py` & `django-camomilla-cms-6.0.0b1/tests/urls.py`

 * *Files identical despite different names*

