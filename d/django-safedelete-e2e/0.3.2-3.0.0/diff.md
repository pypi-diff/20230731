# Comparing `tmp/django-safedelete-e2e-0.3.2.tar.gz` & `tmp/django-safedelete-e2e-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-safedelete-e2e-0.3.2.tar", last modified: Fri Jul 28 10:12:48 2023, max compression
+gzip compressed data, was "django-safedelete-e2e-3.0.0.tar", last modified: Mon Jul 31 07:04:52 2023, max compression
```

## Comparing `django-safedelete-e2e-0.3.2.tar` & `django-safedelete-e2e-3.0.0.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-28 10:12:48.186564 django-safedelete-e2e-0.3.2/
--rw-r--r--   0 roniee007   (501) staff       (20)       59 2023-07-28 09:39:02.000000 django-safedelete-e2e-0.3.2/AUTHORS
--rw-r--r--   0 roniee007   (501) staff       (20)     1430 2023-07-28 09:39:04.000000 django-safedelete-e2e-0.3.2/CHANGES
--rw-r--r--   0 roniee007   (501) staff       (20)     1479 2023-07-28 09:39:18.000000 django-safedelete-e2e-0.3.2/LICENSE
--rw-r--r--   0 roniee007   (501) staff       (20)       92 2023-07-28 09:39:21.000000 django-safedelete-e2e-0.3.2/MANIFEST.in
--rw-r--r--   0 roniee007   (501) staff       (20)     5281 2023-07-28 10:12:48.186624 django-safedelete-e2e-0.3.2/PKG-INFO
--rw-r--r--   0 roniee007   (501) staff       (20)     2923 2023-07-28 09:39:26.000000 django-safedelete-e2e-0.3.2/README.rst
-drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-28 10:12:48.184576 django-safedelete-e2e-0.3.2/django_safedelete_e2e.egg-info/
--rw-r--r--   0 roniee007   (501) staff       (20)     5281 2023-07-28 10:12:48.000000 django-safedelete-e2e-0.3.2/django_safedelete_e2e.egg-info/PKG-INFO
--rw-r--r--   0 roniee007   (501) staff       (20)      531 2023-07-28 10:12:48.000000 django-safedelete-e2e-0.3.2/django_safedelete_e2e.egg-info/SOURCES.txt
--rw-r--r--   0 roniee007   (501) staff       (20)        1 2023-07-28 10:12:48.000000 django-safedelete-e2e-0.3.2/django_safedelete_e2e.egg-info/dependency_links.txt
--rw-r--r--   0 roniee007   (501) staff       (20)        7 2023-07-28 10:12:48.000000 django-safedelete-e2e-0.3.2/django_safedelete_e2e.egg-info/requires.txt
--rw-r--r--   0 roniee007   (501) staff       (20)       11 2023-07-28 10:12:48.000000 django-safedelete-e2e-0.3.2/django_safedelete_e2e.egg-info/top_level.txt
-drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-28 10:12:48.186206 django-safedelete-e2e-0.3.2/safedelete/
--rw-r--r--   0 roniee007   (501) staff       (20)      630 2023-07-28 09:41:34.000000 django-safedelete-e2e-0.3.2/safedelete/__init__.py
--rw-r--r--   0 roniee007   (501) staff       (20)     5111 2023-07-28 10:10:40.000000 django-safedelete-e2e-0.3.2/safedelete/admin.py
--rw-r--r--   0 roniee007   (501) staff       (20)     3240 2023-07-28 09:41:34.000000 django-safedelete-e2e-0.3.2/safedelete/managers.py
--rw-r--r--   0 roniee007   (501) staff       (20)     6871 2023-07-28 09:41:34.000000 django-safedelete-e2e-0.3.2/safedelete/models.py
--rw-r--r--   0 roniee007   (501) staff       (20)      840 2023-07-28 09:41:34.000000 django-safedelete-e2e-0.3.2/safedelete/settings.py
--rw-r--r--   0 roniee007   (501) staff       (20)      226 2023-07-28 09:41:34.000000 django-safedelete-e2e-0.3.2/safedelete/shortcuts.py
-drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-28 10:12:48.182849 django-safedelete-e2e-0.3.2/safedelete/templates/
-drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-28 10:12:48.186396 django-safedelete-e2e-0.3.2/safedelete/templates/safedelete/
--rw-r--r--   0 roniee007   (501) staff       (20)      658 2023-07-28 09:41:34.000000 django-safedelete-e2e-0.3.2/safedelete/templates/safedelete/undelete_selected_confirmation.html
--rw-r--r--   0 roniee007   (501) staff       (20)    16838 2023-07-28 09:41:34.000000 django-safedelete-e2e-0.3.2/safedelete/tests.py
--rw-r--r--   0 roniee007   (501) staff       (20)     1070 2023-07-28 09:41:34.000000 django-safedelete-e2e-0.3.2/safedelete/utils.py
--rw-r--r--   0 roniee007   (501) staff       (20)       80 2023-07-28 10:12:48.186810 django-safedelete-e2e-0.3.2/setup.cfg
--rw-r--r--   0 roniee007   (501) staff       (20)     1985 2023-07-28 10:11:44.000000 django-safedelete-e2e-0.3.2/setup.py
+drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-31 07:04:52.589856 django-safedelete-e2e-3.0.0/
+-rw-r--r--   0 roniee007   (501) staff       (20)       91 2023-07-31 06:53:40.000000 django-safedelete-e2e-3.0.0/AUTHORS
+-rw-r--r--   0 roniee007   (501) staff       (20)     5633 2023-07-31 06:53:44.000000 django-safedelete-e2e-3.0.0/CHANGES
+-rw-r--r--   0 roniee007   (501) staff       (20)     1479 2023-07-31 06:53:46.000000 django-safedelete-e2e-3.0.0/LICENSE
+-rw-r--r--   0 roniee007   (501) staff       (20)      227 2023-07-31 06:53:54.000000 django-safedelete-e2e-3.0.0/MANIFEST.in
+-rw-r--r--   0 roniee007   (501) staff       (20)    10816 2023-07-31 07:04:52.589929 django-safedelete-e2e-3.0.0/PKG-INFO
+-rw-r--r--   0 roniee007   (501) staff       (20)     4156 2023-07-31 06:53:59.000000 django-safedelete-e2e-3.0.0/README.rst
+drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-31 07:04:52.587215 django-safedelete-e2e-3.0.0/django_safedelete_e2e.egg-info/
+-rw-r--r--   0 roniee007   (501) staff       (20)    10816 2023-07-31 07:04:52.000000 django-safedelete-e2e-3.0.0/django_safedelete_e2e.egg-info/PKG-INFO
+-rw-r--r--   0 roniee007   (501) staff       (20)      613 2023-07-31 07:04:52.000000 django-safedelete-e2e-3.0.0/django_safedelete_e2e.egg-info/SOURCES.txt
+-rw-r--r--   0 roniee007   (501) staff       (20)        1 2023-07-31 07:04:52.000000 django-safedelete-e2e-3.0.0/django_safedelete_e2e.egg-info/dependency_links.txt
+-rw-r--r--   0 roniee007   (501) staff       (20)        7 2023-07-31 07:04:52.000000 django-safedelete-e2e-3.0.0/django_safedelete_e2e.egg-info/requires.txt
+-rw-r--r--   0 roniee007   (501) staff       (20)       11 2023-07-31 07:04:52.000000 django-safedelete-e2e-3.0.0/django_safedelete_e2e.egg-info/top_level.txt
+drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-31 07:04:52.589133 django-safedelete-e2e-3.0.0/safedelete/
+-rw-r--r--   0 roniee007   (501) staff       (20)      630 2023-07-28 09:41:34.000000 django-safedelete-e2e-3.0.0/safedelete/__init__.py
+-rw-r--r--   0 roniee007   (501) staff       (20)     5111 2023-07-28 10:10:40.000000 django-safedelete-e2e-3.0.0/safedelete/admin.py
+drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-31 07:04:52.583189 django-safedelete-e2e-3.0.0/safedelete/locale/
+drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-31 07:04:52.583238 django-safedelete-e2e-3.0.0/safedelete/locale/fr/
+drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-31 07:04:52.589331 django-safedelete-e2e-3.0.0/safedelete/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 roniee007   (501) staff       (20)     1438 2023-07-28 09:41:34.000000 django-safedelete-e2e-3.0.0/safedelete/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 roniee007   (501) staff       (20)     3240 2023-07-28 09:41:34.000000 django-safedelete-e2e-3.0.0/safedelete/managers.py
+-rw-r--r--   0 roniee007   (501) staff       (20)     6871 2023-07-28 09:41:34.000000 django-safedelete-e2e-3.0.0/safedelete/models.py
+-rw-r--r--   0 roniee007   (501) staff       (20)      840 2023-07-28 09:41:34.000000 django-safedelete-e2e-3.0.0/safedelete/settings.py
+-rw-r--r--   0 roniee007   (501) staff       (20)      226 2023-07-28 09:41:34.000000 django-safedelete-e2e-3.0.0/safedelete/shortcuts.py
+drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-31 07:04:52.583361 django-safedelete-e2e-3.0.0/safedelete/static/
+drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-31 07:04:52.589522 django-safedelete-e2e-3.0.0/safedelete/static/safedelete/
+-rw-r--r--   0 roniee007   (501) staff       (20)       90 2023-07-28 09:41:34.000000 django-safedelete-e2e-3.0.0/safedelete/static/safedelete/admin.css
+drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-31 07:04:52.583500 django-safedelete-e2e-3.0.0/safedelete/templates/
+drwxr-xr-x   0 roniee007   (501) staff       (20)        0 2023-07-31 07:04:52.589700 django-safedelete-e2e-3.0.0/safedelete/templates/safedelete/
+-rw-r--r--   0 roniee007   (501) staff       (20)      658 2023-07-28 09:41:34.000000 django-safedelete-e2e-3.0.0/safedelete/templates/safedelete/undelete_selected_confirmation.html
+-rw-r--r--   0 roniee007   (501) staff       (20)    16838 2023-07-28 09:41:34.000000 django-safedelete-e2e-3.0.0/safedelete/tests.py
+-rw-r--r--   0 roniee007   (501) staff       (20)     1070 2023-07-28 09:41:34.000000 django-safedelete-e2e-3.0.0/safedelete/utils.py
+-rw-r--r--   0 roniee007   (501) staff       (20)       80 2023-07-31 07:04:52.590162 django-safedelete-e2e-3.0.0/setup.cfg
+-rw-r--r--   0 roniee007   (501) staff       (20)     2083 2023-07-31 07:02:17.000000 django-safedelete-e2e-3.0.0/setup.py
```

### Comparing `django-safedelete-e2e-0.3.2/LICENSE` & `django-safedelete-e2e-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.2/README.rst` & `django-safedelete-e2e-3.0.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 Django safedelete
 =================
 
-.. image:: https://travis-ci.org/makinacorpus/django-safedelete.png
-    :target: https://travis-ci.org/makinacorpus/django-safedelete
+.. image:: https://github.com/makinacorpus/django-safedelete/workflows/Python%20application/badge.svg
+    :target: https://github.com/makinacorpus/django-safedelete/actions?query=workflow%3A%22Python+application%22
 
 .. image:: https://coveralls.io/repos/makinacorpus/django-safedelete/badge.png
     :target: https://coveralls.io/r/makinacorpus/django-safedelete
 
 
 What is it ?
 ------------
 
 For various reasons, you may want to avoid deleting objects from your database.
 
-This Django application provides a model mixin, that allows you to transparently retrieve or delete your objects,
+This Django application provides an abstract model, that allows you to transparently retrieve or delete your objects,
 without having them deleted from your database.
 
 You can choose what happens when you delete an object :
- - it can be masked from your database (soft delete)
- - it can be normally deleted (hard delete)
- - it can be hard-deleted, but if its deletion would delete other objects, it will only be masked
- - it can be never deleted or masked from your database (no delete, use with caution)
+ - it can be masked from your database (SOFT_DELETE, the default behavior)
+ - it can be masked from your database and mask any dependent models. (SOFT_DELETE_CASCADE)
+ - it can be normally deleted (HARD_DELETE)
+ - it can be hard-deleted, but if its deletion would delete other objects, it will only be masked (HARD_DELETE_NOCASCADE)
+ - it can be never deleted or masked from your database (NO_DELETE, use with caution)
 
 
 Example
 -------
 
 .. code-block:: python
 
+    # imports
+    from safedelete.models import SafeDeleteModel
+    from safedelete.models import HARD_DELETE_NOCASCADE
+
     # Models
 
-    # We create a new mixin, with the given policy : Objects will be hard-deleted, or soft deleted if other objects would have been deleted too.
-    SafeDeleteMixin = safedelete_mixin_factory(HARD_DELETE_NOCASCADE)
+    # We create a new model, with the given policy : Objects will be hard-deleted, or soft deleted if other objects would have been deleted too.
+    class Article(SafeDeleteModel):
+        _safedelete_policy = HARD_DELETE_NOCASCADE
 
-    class Article(SafeDeleteMixin):
         name = models.CharField(max_length=100)
 
-    class Order(SafeDeleteMixin):
+    class Order(SafeDeleteModel):
+        _safedelete_policy = HARD_DELETE_NOCASCADE
+
         name = models.CharField(max_length=100)
         articles = models.ManyToManyField(Article)
 
 
     # Example of use
 
     >>> article1 = Article(name='article1')
@@ -61,53 +68,75 @@
 
 
 Compatibilities
 ---------------
 
 * Branch 0.2.x is compatible with django >= 1.2
 * Branch 0.3.x is compatible with django >= 1.4
-
-Current branch (0.3.x) has been tested with :
-
-*  Django 1.4, using python 2.6 and 2.7.
-*  Django 1.5 and 1.6, using python 2.6, 2.7 and 3.x.
-*  Django 1.7 using python 2.7 and python 3.x.
-*  Django 1.8 using python 2.7 and python 3.x.
-*  Django 1.9 using python 2.7 and python 3.x.
-
+* Branch 0.4.x is compatible with django >= 1.8
+* Branch 0.5.x is compatible with django >= 1.11
+* Branch 1.0.x, 1.1.x and 1.2.x are compatible with django >= 2.2
+* Branch 1.3.x is compatible with django >= 3.2 and Python >= 3.7
+
+Current branch (1.3.x) is tested with :
+
+*  Django 3.2 using python 3.7 to 3.10.
+*  Django 4.0 using python 3.8 to 3.10.
+*  Django 4.1 using python 3.8 to 3.10.
+*  Django 4.2 using python 3.8 to 3.11.
 
 
 Installation
 ------------
 
 Installing from pypi (using pip). ::
 
     pip install django-safedelete
 
 
 Installing from github. ::
 
     pip install -e git://github.com/makinacorpus/django-safedelete.git#egg=django-safedelete
 
+Add ``safedelete`` in your ``INSTALLED_APPS``:
+
+.. code-block:: python
+
+    INSTALLED_APPS = [
+        'safedelete',
+        [...]
+    ]
+
 
 The application doesn't have any special requirement.
 
 
+Configuration
+-------------
+
+In the main django settings you can activate the boolean variable ``SAFE_DELETE_INTERPRET_UNDELETED_OBJECTS_AS_CREATED``.
+If you do this the ``update_or_create()`` function from django's standard manager class will return ``True`` for
+the ``created`` variable if the object was soft-deleted and is now "revived".
+
+By default, the field that indicates a database entry is soft-deleted is ``deleted``, however, you can override the field name
+using the ``SAFE_DELETE_FIELD_NAME`` setting.
+
 Documentation
 -------------
 
-The documentation is available `here <https://django-safedelete.readthedocs.io>`_.
+The documentation is available `here <http://django-safedelete.readthedocs.org>`_. Generate your own documentation using:
+
+    tox -e docs
 
 
 Licensing
 ---------
 
 Please see the LICENSE file.
 
 Contacts
 --------
 
 Please see the AUTHORS file.
 
 .. image:: https://drupal.org/files/imagecache/grid-3/Logo_slogan_300dpi.png
     :target: http://www.makina-corpus.com
-
```

### Comparing `django-safedelete-e2e-0.3.2/safedelete/__init__.py` & `django-safedelete-e2e-3.0.0/safedelete/__init__.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.2/safedelete/admin.py` & `django-safedelete-e2e-3.0.0/safedelete/admin.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.2/safedelete/managers.py` & `django-safedelete-e2e-3.0.0/safedelete/managers.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.2/safedelete/models.py` & `django-safedelete-e2e-3.0.0/safedelete/models.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.2/safedelete/settings.py` & `django-safedelete-e2e-3.0.0/safedelete/settings.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.2/safedelete/templates/safedelete/undelete_selected_confirmation.html` & `django-safedelete-e2e-3.0.0/safedelete/templates/safedelete/undelete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.2/safedelete/tests.py` & `django-safedelete-e2e-3.0.0/safedelete/tests.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.2/safedelete/utils.py` & `django-safedelete-e2e-3.0.0/safedelete/utils.py`

 * *Files identical despite different names*

### Comparing `django-safedelete-e2e-0.3.2/setup.py` & `django-safedelete-e2e-3.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import codecs
 import os
 import re
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open('README.rst', 'r') as f_readme:
     with open('CHANGES', 'r') as f_changes:
         long_description = f_readme.read() + '\n\n' + f_changes.read()
 
@@ -18,38 +18,41 @@
 #     with codecs.open(init_path, 'r', 'utf-8') as f:
 #         for line in f:
 #             match = version_re.match(line.strip())
 #             if match:
 #                 return match.groups()[0]
 #     raise RuntimeError("Unable to find version string.")
 
+
 # version = get_version('safedelete')
 
 setup(
     name='django-safedelete-e2e',
     packages=find_packages(),
-    version='0.3.2',
+    version="3.0.0",
     description='Mask your objects instead of deleting them from your database.',
     long_description=long_description,
-    author='rounak kabra',
-    author_email='rounak.kabra@e2enetworks.com',
-    url='https://github.com/Roniee007/django-safedelete-e2e',
+    author='Rounak Kabra',
+    author_email='rounak.kabra@e2enetowrks.com',
+    url='https://github.com/makinacorpus/django-safedelete',
     # download_url='https://github.com/makinacorpus/django-safedelete/tarball/%s' % version,
     keywords=['django', 'delete', 'safedelete', 'softdelete'],
     classifiers=[
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.6',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.2',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'Development Status :: 4 - Beta',
     ],
     license='BSD',
     install_requires=['Django'],
     include_package_data=True,
 )
```

