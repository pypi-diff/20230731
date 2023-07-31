# Comparing `tmp/django-silly-stripe-1.0.1.tar.gz` & `tmp/django-silly-stripe-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-silly-stripe-1.0.1.tar", last modified: Thu Jul 27 19:16:04 2023, max compression
+gzip compressed data, was "django-silly-stripe-1.0.2.tar", last modified: Mon Jul 31 14:28:20 2023, max compression
```

## Comparing `django-silly-stripe-1.0.1.tar` & `django-silly-stripe-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,38 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-27 19:16:04.859230 django-silly-stripe-1.0.1/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-stripe-1.0.1/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1727 2023-07-27 19:16:04.859230 django-silly-stripe-1.0.1/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1104 2023-07-27 19:14:42.000000 django-silly-stripe-1.0.1/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-27 19:16:04.855230 django-silly-stripe-1.0.1/django_silly_stripe/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       52 2023-07-27 19:14:42.000000 django-silly-stripe-1.0.1/django_silly_stripe/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1973 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.1/django_silly_stripe/admin.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1406 2023-07-27 19:14:42.000000 django-silly-stripe-1.0.1/django_silly_stripe/conf.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      942 2023-07-27 19:14:42.000000 django-silly-stripe-1.0.1/django_silly_stripe/helpers.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3428 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.1/django_silly_stripe/models.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2203 2023-07-27 16:54:42.000000 django-silly-stripe-1.0.1/django_silly_stripe/urls.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     8757 2023-07-27 19:14:42.000000 django-silly-stripe-1.0.1/django_silly_stripe/views.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-27 19:16:04.855230 django-silly-stripe-1.0.1/django_silly_stripe.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1727 2023-07-27 19:16:04.000000 django-silly-stripe-1.0.1/django_silly_stripe.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      450 2023-07-27 19:16:04.000000 django-silly-stripe-1.0.1/django_silly_stripe.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-07-27 19:16:04.000000 django-silly-stripe-1.0.1/django_silly_stripe.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       14 2023-07-27 19:16:04.000000 django-silly-stripe-1.0.1/django_silly_stripe.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       20 2023-07-27 19:16:04.000000 django-silly-stripe-1.0.1/django_silly_stripe.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-07-27 19:16:04.859230 django-silly-stripe-1.0.1/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1642 2023-07-12 12:08:15.000000 django-silly-stripe-1.0.1/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:28:20.297106 django-silly-stripe-1.0.2/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-stripe-1.0.2/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1727 2023-07-31 14:28:20.297106 django-silly-stripe-1.0.2/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1104 2023-07-27 19:14:42.000000 django-silly-stripe-1.0.2/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:28:20.289106 django-silly-stripe-1.0.2/django_silly_stripe/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       52 2023-07-31 14:25:00.000000 django-silly-stripe-1.0.2/django_silly_stripe/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1973 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.2/django_silly_stripe/admin.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1406 2023-07-27 19:43:59.000000 django-silly-stripe-1.0.2/django_silly_stripe/conf.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      942 2023-07-27 19:14:42.000000 django-silly-stripe-1.0.2/django_silly_stripe/helpers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:28:20.293106 django-silly-stripe-1.0.2/django_silly_stripe/migrations/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      931 2023-07-16 19:12:41.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0001_initial.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      620 2023-07-17 19:35:25.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0002_alter_customer_user.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      552 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0003_remove_customer_stripe_id_alter_customer_id.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      458 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0004_customer_email.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      414 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0005_customer_name.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1889 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0006_product_price.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      398 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0007_price_metadata.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      868 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0008_subscription.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      814 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0009_subscription_end_time_subscription_start_time_and_more.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      603 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0010_alter_subscription_end_time_and_more.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      435 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/0011_subscription_cancel_at_period_end.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-12 12:59:48.000000 django-silly-stripe-1.0.2/django_silly_stripe/migrations/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3428 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.2/django_silly_stripe/models.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:28:20.293106 django-silly-stripe-1.0.2/django_silly_stripe/templates/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:26:16.000000 django-silly-stripe-1.0.2/django_silly_stripe/templates/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:28:20.297106 django-silly-stripe-1.0.2/django_silly_stripe/templates/admin/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:26:01.000000 django-silly-stripe-1.0.2/django_silly_stripe/templates/admin/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6732 2023-07-25 12:20:33.000000 django-silly-stripe-1.0.2/django_silly_stripe/templates/admin/base.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2203 2023-07-27 16:54:42.000000 django-silly-stripe-1.0.2/django_silly_stripe/urls.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     8757 2023-07-27 19:42:29.000000 django-silly-stripe-1.0.2/django_silly_stripe/views.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:28:20.293106 django-silly-stripe-1.0.2/django_silly_stripe.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1727 2023-07-31 14:28:20.000000 django-silly-stripe-1.0.2/django_silly_stripe.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1327 2023-07-31 14:28:20.000000 django-silly-stripe-1.0.2/django_silly_stripe.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-07-31 14:28:20.000000 django-silly-stripe-1.0.2/django_silly_stripe.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       14 2023-07-31 14:28:20.000000 django-silly-stripe-1.0.2/django_silly_stripe.egg-info/requires.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       20 2023-07-31 14:28:20.000000 django-silly-stripe-1.0.2/django_silly_stripe.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-07-31 14:28:20.297106 django-silly-stripe-1.0.2/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1772 2023-07-31 14:28:03.000000 django-silly-stripe-1.0.2/setup.py
```

### Comparing `django-silly-stripe-1.0.1/LICENSE.md` & `django-silly-stripe-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.1/PKG-INFO` & `django-silly-stripe-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-stripe
-Version: 1.0.1
+Version: 1.0.2
 Summary: Wrapper package for python stripe with Django and/or DRF
 Home-page: https://github.com/byoso/django_silly_stripe
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django stripe
 Platform: UNKNOWN
```

### Comparing `django-silly-stripe-1.0.1/README.md` & `django-silly-stripe-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.1/django_silly_stripe/admin.py` & `django-silly-stripe-1.0.2/django_silly_stripe/admin.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.1/django_silly_stripe/conf.py` & `django-silly-stripe-1.0.2/django_silly_stripe/conf.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.1/django_silly_stripe/helpers.py` & `django-silly-stripe-1.0.2/django_silly_stripe/helpers.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.1/django_silly_stripe/models.py` & `django-silly-stripe-1.0.2/django_silly_stripe/models.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.1/django_silly_stripe/urls.py` & `django-silly-stripe-1.0.2/django_silly_stripe/urls.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.1/django_silly_stripe/views.py` & `django-silly-stripe-1.0.2/django_silly_stripe/views.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.1/django_silly_stripe.egg-info/PKG-INFO` & `django-silly-stripe-1.0.2/django_silly_stripe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-stripe
-Version: 1.0.1
+Version: 1.0.2
 Summary: Wrapper package for python stripe with Django and/or DRF
 Home-page: https://github.com/byoso/django_silly_stripe
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django stripe
 Platform: UNKNOWN
```

### Comparing `django-silly-stripe-1.0.1/setup.py` & `django-silly-stripe-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,14 +42,17 @@
         "Programming Language :: Python :: 3",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
     ],
     packages=[
         "django_silly_stripe",
+        "django_silly_stripe.migrations",
+        "django_silly_stripe.templates",
+        "django_silly_stripe.templates.admin",
         ],
     # include_package_data=True,
     package_data={'': ['*.txt', '*.html', '*.po', '*.mo', '*.pot']},
     python_requires='>=3.7',
     install_requires=[
         "stripe>=5.4.0",
     ],
```

