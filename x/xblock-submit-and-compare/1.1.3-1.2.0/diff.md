# Comparing `tmp/xblock-submit-and-compare-1.1.3.tar.gz` & `tmp/xblock-submit-and-compare-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xblock-submit-and-compare-1.1.3.tar", last modified: Thu Dec 15 12:02:29 2022, max compression
+gzip compressed data, was "xblock-submit-and-compare-1.2.0.tar", last modified: Mon Jul 31 07:43:11 2023, max compression
```

## Comparing `xblock-submit-and-compare-1.1.3.tar` & `xblock-submit-and-compare-1.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:02:29.488238 xblock-submit-and-compare-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       85 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4928 2022-12-15 12:02:29.488238 xblock-submit-and-compare-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3937 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:02:29.488238 xblock-submit-and-compare-1.1.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       94 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      584 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-15 12:02:29.488238 xblock-submit-and-compare-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5229 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:02:29.488238 xblock-submit-and-compare-1.1.3/submit_and_compare/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:02:29.488238 xblock-submit-and-compare-1.1.3/submit_and_compare/mixins/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/mixins/dates.py
--rw-r--r--   0 runner    (1001) docker     (122)     1590 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/mixins/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     2600 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/mixins/fragment.py
--rw-r--r--   0 runner    (1001) docker     (122)     1570 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/mixins/scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     3692 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:02:29.488238 xblock-submit-and-compare-1.1.3/submit_and_compare/public/
--rw-r--r--   0 runner    (1001) docker     (122)     1537 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/public/edit.js
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/public/view.css
--rw-r--r--   0 runner    (1001) docker     (122)     5156 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/public/view.js
--rw-r--r--   0 runner    (1001) docker     (122)     1354 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/public/view.less
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:02:29.488238 xblock-submit-and-compare-1.1.3/submit_and_compare/scenarios/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/scenarios/submit-and-compare-single.xml
--rw-r--r--   0 runner    (1001) docker     (122)      333 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:02:29.488238 xblock-submit-and-compare-1.1.3/submit_and_compare/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     4020 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/templates/edit.html
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/templates/view.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:02:29.488238 xblock-submit-and-compare-1.1.3/submit_and_compare/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7153 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/tests/test_all.py
--rw-r--r--   0 runner    (1001) docker     (122)     9359 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/views.py
--rw-r--r--   0 runner    (1001) docker     (122)      575 2022-12-15 12:02:18.000000 xblock-submit-and-compare-1.1.3/submit_and_compare/xblocks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-15 12:02:29.488238 xblock-submit-and-compare-1.1.3/xblock_submit_and_compare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4928 2022-12-15 12:02:29.000000 xblock-submit-and-compare-1.1.3/xblock_submit_and_compare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2022-12-15 12:02:29.000000 xblock-submit-and-compare-1.1.3/xblock_submit_and_compare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-15 12:02:29.000000 xblock-submit-and-compare-1.1.3/xblock_submit_and_compare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2022-12-15 12:02:29.000000 xblock-submit-and-compare-1.1.3/xblock_submit_and_compare.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       31 2022-12-15 12:02:29.000000 xblock-submit-and-compare-1.1.3/xblock_submit_and_compare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2022-12-15 12:02:29.000000 xblock-submit-and-compare-1.1.3/xblock_submit_and_compare.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 07:43:11.045557 xblock-submit-and-compare-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4830 2023-07-31 07:43:11.045557 xblock-submit-and-compare-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 07:43:11.041557 xblock-submit-and-compare-1.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-31 07:43:11.045557 xblock-submit-and-compare-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5153 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 07:43:11.041557 xblock-submit-and-compare-1.2.0/submit_and_compare/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 07:43:11.041557 xblock-submit-and-compare-1.2.0/submit_and_compare/mixins/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/mixins/dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1590 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/mixins/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/mixins/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1570 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/mixins/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 07:43:11.041557 xblock-submit-and-compare-1.2.0/submit_and_compare/public/
+-rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/public/edit.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/public/view.css
+-rw-r--r--   0 runner    (1001) docker     (122)     5156 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/public/view.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/public/view.less
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 07:43:11.041557 xblock-submit-and-compare-1.2.0/submit_and_compare/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/scenarios/submit-and-compare-single.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      333 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 07:43:11.045557 xblock-submit-and-compare-1.2.0/submit_and_compare/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     4244 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/templates/edit.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/templates/view.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 07:43:11.045557 xblock-submit-and-compare-1.2.0/submit_and_compare/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7251 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9354 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-31 07:43:02.000000 xblock-submit-and-compare-1.2.0/submit_and_compare/xblocks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 07:43:11.045557 xblock-submit-and-compare-1.2.0/xblock_submit_and_compare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4830 2023-07-31 07:43:11.000000 xblock-submit-and-compare-1.2.0/xblock_submit_and_compare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-31 07:43:11.000000 xblock-submit-and-compare-1.2.0/xblock_submit_and_compare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 07:43:11.000000 xblock-submit-and-compare-1.2.0/xblock_submit_and_compare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-07-31 07:43:11.000000 xblock-submit-and-compare-1.2.0/xblock_submit_and_compare.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-31 07:43:11.000000 xblock-submit-and-compare-1.2.0/xblock_submit_and_compare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-31 07:43:11.000000 xblock-submit-and-compare-1.2.0/xblock_submit_and_compare.egg-info/top_level.txt
```

### Comparing `xblock-submit-and-compare-1.1.3/LICENSE` & `xblock-submit-and-compare-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xblock-submit-and-compare-1.1.3/PKG-INFO` & `xblock-submit-and-compare-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: xblock-submit-and-compare
-Version: 1.1.3
+Version: 1.2.0
 Summary: A submit-and-compare XBlock
 Home-page: https://github.com/Stanford-Online/xblock-submit-and-compare
 Author: stv
 Author-email: stv@stanford.edu
 License: AGPL-3.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Education
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
 
 Submit and Compare XBlock
 =========================
 
@@ -147,9 +144,7 @@
 .. |image-lms-view-normal| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/lms-view-normal.png
    :width: 100%
 .. |image-lms-view-zoom| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/lms-view-zoom.png
    :width: 100%
 .. _View a demo of the CMS: https://youtu.be/IcbGYfbav2w
 .. _View a demo of the LMS: https://youtu.be/0mpjuThDoyE
 .. https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/xblock-image-modal-demo-lms.mov
-
-
```

### Comparing `xblock-submit-and-compare-1.1.3/README.rst` & `xblock-submit-and-compare-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `xblock-submit-and-compare-1.1.3/requirements/constraints.txt` & `xblock-submit-and-compare-1.2.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `xblock-submit-and-compare-1.1.3/setup.py` & `xblock-submit-and-compare-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import os
 import re
 from os import path
 
 from setuptools import find_packages, setup
 
-version = '1.1.3'
+version = '1.2.0'
 description = __doc__.strip().split('\n')[0]
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.rst')) as file_in:
     long_description = file_in.read()
 
 
 def load_requirements(*requirements_paths):
@@ -117,16 +117,14 @@
         'Operating System :: OS Independent',
         'Programming Language :: JavaScript',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.8',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
-        'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.2',
         'Topic :: Education',
         'Topic :: Internet :: WWW/HTTP',
     ],
     test_suite='submit_and_compare.tests',
 )
```

### Comparing `xblock-submit-and-compare-1.1.3/submit_and_compare/mixins/dates.py` & `xblock-submit-and-compare-1.2.0/submit_and_compare/mixins/dates.py`

 * *Files identical despite different names*

### Comparing `xblock-submit-and-compare-1.1.3/submit_and_compare/mixins/events.py` & `xblock-submit-and-compare-1.2.0/submit_and_compare/mixins/events.py`

 * *Files identical despite different names*

### Comparing `xblock-submit-and-compare-1.1.3/submit_and_compare/mixins/fragment.py` & `xblock-submit-and-compare-1.2.0/submit_and_compare/mixins/fragment.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,20 @@
     ]
     static_js = [
         'view.js',
     ]
     static_js_init = None
     template = 'view.html'
 
+    def get_i18n_service(self):
+        """
+        Get the i18n service from the runtime
+        """
+        return self.runtime.service(self, 'i18n')
+
     def provide_context(self, context):  # pragma: no cover
         """
         Build a context dictionary to render the student view
 
         This should generally be overriden by child classes.
         """
         context = context or {}
@@ -67,15 +73,15 @@
         js = js or []
         rendered_template = ''
         if template:  # pragma: no cover
             template = 'templates/' + template
             rendered_template = self.loader.render_django_template(
                 template,
                 context=Context(context),
-                i18n_service=self.runtime.service(self, 'i18n'),
+                i18n_service=self.get_i18n_service(),
             )
         fragment = Fragment(rendered_template)
         for item in css:
             if item.startswith('/'):
                 url = item
             else:
                 item = 'public/' + item
```

### Comparing `xblock-submit-and-compare-1.1.3/submit_and_compare/mixins/scenario.py` & `xblock-submit-and-compare-1.2.0/submit_and_compare/mixins/scenario.py`

 * *Files identical despite different names*

### Comparing `xblock-submit-and-compare-1.1.3/submit_and_compare/models.py` & `xblock-submit-and-compare-1.2.0/submit_and_compare/models.py`

 * *Files identical despite different names*

### Comparing `xblock-submit-and-compare-1.1.3/submit_and_compare/public/edit.js` & `xblock-submit-and-compare-1.2.0/submit_and_compare/public/edit.js`

 * *Files identical despite different names*

### Comparing `xblock-submit-and-compare-1.1.3/submit_and_compare/public/view.css` & `xblock-submit-and-compare-1.2.0/submit_and_compare/public/view.css`

 * *Files identical despite different names*

### Comparing `xblock-submit-and-compare-1.1.3/submit_and_compare/public/view.js` & `xblock-submit-and-compare-1.2.0/submit_and_compare/public/view.js`

 * *Files identical despite different names*

### Comparing `xblock-submit-and-compare-1.1.3/submit_and_compare/public/view.less` & `xblock-submit-and-compare-1.2.0/submit_and_compare/public/view.less`

 * *Files identical despite different names*

### Comparing `xblock-submit-and-compare-1.1.3/submit_and_compare/templates/edit.html` & `xblock-submit-and-compare-1.2.0/submit_and_compare/templates/edit.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 {% load i18n %}
 
 <div class="wrapper-comp-settings editor-with-buttons is-active" id="settings-tab">
     <ul class="list-input settings-list">
         
          <li class="field comp-setting-entry is-set">
             <div class="wrapper-comp-setting">
-                <label class="label setting-label" for="submit_and_compare_edit_display_name">Display Name</label>
+                <label class="label setting-label" for="submit_and_compare_edit_display_name">{% trans "Display Name" %}</label>
                 <input class="input setting-input" id="submit_and_compare_edit_display_name" value="{{ display_name }}" type="text">
             </div>
-            <span class="tip setting-help">This name appears in the horizontal navigation at the top of the page</span>
+            <span class="tip setting-help">{% trans "This name appears in the horizontal navigation at the top of the page" %}</span>
         </li>
 
         <li class="field comp-setting-entry is-set">
           <div class="wrapper-comp-setting">
-                <label class="label setting-label" for="submit_and_compare_edit_weight">Weight</label>
+                <label class="label setting-label" for="submit_and_compare_edit_weight">{% trans "Weight" %}</label>
                 <input class="input setting-input" id="submit_and_compare_edit_weight" step="1" min="0" value="{{ weight }}" type="number">
           </div>
-          <span class="tip setting-help">This assigns an integer value representing the weight of this problem</span>
+          <span class="tip setting-help">{% trans "This assigns an integer value representing the weight of this problem" %}</span>
         </li>
 
         <li class="field comp-setting-entry is-set">
           <div class="wrapper-comp-setting">
-                <label class="label setting-label" for="submit_and_compare_edit_max_attempts">Max Attempts</label>
+                <label class="label setting-label" for="submit_and_compare_edit_max_attempts">{% trans "Max Attempts" %}</label>
                 <input class="input setting-input" id="submit_and_compare_edit_max_attempts" step="1" min="0" value="{{ max_attempts }}" type="number">
           </div>
-          <span class="tip setting-help">This assigns an integer value representing the maximum number of times a student can attempt the problem</span>
+          <span class="tip setting-help">{% trans "This assigns an integer value representing the maximum number of times a student can attempt the problem" %}</span>
         </li>
 
          <li class="field comp-setting-entry is-set">
             <div class="wrapper-comp-setting">
-                <label class="label setting-label" for="submit_and_compare_edit_your_answer_label">Label for Student Answer</label>
+                <label class="label setting-label" for="submit_and_compare_edit_your_answer_label">{% trans "Label for Student Answer" %}</label>
                 <input class="input setting-input" id="submit_and_compare_edit_your_answer_label" value="{{ your_answer_label }}" type="text">
             </div>
-            <span class="tip setting-help">Label for the text area containing the student's answer</span>
+            <span class="tip setting-help">{% trans "Label for the text area containing the student's answer" %}</span>
         </li>
 
          <li class="field comp-setting-entry is-set">
             <div class="wrapper-comp-setting">
-                <label class="label setting-label" for="submit_and_compare_edit_our_answer_label">Label for Expert Answer</label>
+                <label class="label setting-label" for="submit_and_compare_edit_our_answer_label">{% trans "Label for Expert Answer" %}</label>
                 <input class="input setting-input" id="submit_and_compare_edit_our_answer_label" value="{{ our_answer_label }}" type="text">
             </div>
-            <span class="tip setting-help">Label for the 'expert' answer</span>
+            <span class="tip setting-help">{% trans "Label for the 'expert' answer" %}</span>
         </li>
 
         <li class="field comp-setting-entry is-set">
             <div class="wrapper-comp-setting">
-                <label class="label setting-label" for="submit_and_compare_edit_submit_button_label">Label for Submit Button</label>
+                <label class="label setting-label" for="submit_and_compare_edit_submit_button_label">{% trans "Label for Submit Button" %}</label>
                 <input class="input setting-input" id="submit_and_compare_edit_submit_button_label" value="{{ submit_button_label }}" type="text">
             </div>
-            <span class="tip setting-help">Label for the submit button</span>
+            <span class="tip setting-help">{% trans "Label for the submit button" %}</span>
         </li>
         
         <li class="field comp-setting-entry is-set">
           <div class="wrapper-comp-setting">
-            <label class="label setting-label" for="edit_data">Definition</label>
-            <span class="tip setting-help">The XML definition for the question and expert answer</span>
+            <label class="label setting-label" for="edit_data">{% trans "Definition" %}</label>
+            <span class="tip setting-help">{% trans "The XML definition for the question and expert answer" %}</span>
             <div class='codemirror-editor-wrapper'>
               <textarea class="block-xml-editor edit-data">{{ xml_data }}</textarea>
             </div>
           </div>
       </li>
 
     </ul>
     
     <div class="xblock-actions">
         <ul>
             <li class="action-item">
-                <a href="#" class="button action-primary action-save">Save</a>
+                <a href="#" class="button action-primary action-save">{% trans "Save" %}</a>
             </li>
             <li class="action-item">
-                <a href="#" class="button action-cancel">Cancel</a>
+                <a href="#" class="button action-cancel">{% trans "Cancel" %}</a>
             </li>
         </ul>
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,18 +1,21 @@
 {% load i18n %}
-    * Display Name [{{ display_name }}  ]
-      This name appears in the horizontal navigation at the top of the page
-    * Weight [Unknown INPUT type]
-      This assigns an integer value representing the weight of this problem
-    * Max Attempts [Unknown INPUT type]
-      This assigns an integer value representing the maximum number of times a
-      student can attempt the problem
-    * Label for Student Answer [{{ your_answer_label }}]
-      Label for the text area containing the student's answer
-    * Label for Expert Answer [{{ our_answer_label }}]
-      Label for the 'expert' answer
-    * Label for Submit Button [{{ submit_button_label }}]
-      Label for the submit button
-    * Definition The XML definition for the question and expert answer
+    * {% trans "Display Name" %} [{{ display_name }}  ]
+      {% trans "This name appears in the horizontal navigation at the top of
+      the page" %}
+    * {% trans "Weight" %} [Unknown INPUT type]
+      {% trans "This assigns an integer value representing the weight of this
+      problem" %}
+    * {% trans "Max Attempts" %} [Unknown INPUT type]
+      {% trans "This assigns an integer value representing the maximum number
+      of times a student can attempt the problem" %}
+    * {% trans "Label for Student Answer" %} [{{ your_answer_label }}]
+      {% trans "Label for the text area containing the student's answer" %}
+    * {% trans "Label for Expert Answer" %} [{{ our_answer_label }}]
+      {% trans "Label for the 'expert' answer" %}
+    * {% trans "Label for Submit Button" %} [{{ submit_button_label }}]
+      {% trans "Label for the submit button" %}
+    * {% trans "Definition" %} {% trans "The XML definition for the question
+      and expert answer" %}
       {{ xml_data }}
-    * Save
-    * Cancel
+    * {%_trans_"Save"_%}
+    * {%_trans_"Cancel"_%}
```

### Comparing `xblock-submit-and-compare-1.1.3/submit_and_compare/templates/view.html` & `xblock-submit-and-compare-1.2.0/submit_and_compare/templates/view.html`

 * *Files identical despite different names*

### Comparing `xblock-submit-and-compare-1.1.3/submit_and_compare/tests/test_all.py` & `xblock-submit-and-compare-1.2.0/submit_and_compare/tests/test_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 import re
 import unittest
 from xml.sax.saxutils import escape
 
 from unittest import mock
 from django.test.client import Client
-from django.utils.translation import ugettext as _
 from opaque_keys.edx.locations import SlashSeparatedCourseKey
 from xblock.field_data import DictFieldData
 
 from ..xblocks import SubmitAndCompareXBlock
 from ..views import get_body
 
 
@@ -50,15 +49,19 @@
         )
         self.assertIn(self.xblock._get_problem_progress(), student_view_html)
 
     def test_studio_view(self):
         """
         Checks studio view for instance variables specified by the instructor.
         """
-        studio_view_html = self.studio_view_html()
+        with mock.patch(
+            "submit_and_compare.mixins.fragment.XBlockFragmentBuilderMixin.get_i18n_service",
+            return_value=None
+        ):
+            studio_view_html = self.studio_view_html()
         self.assertIn(self.xblock.display_name, studio_view_html)
         xblock_body = get_body(
             self.xblock.question_string
         )
         studio_view_html = re.sub(r'\W+', ' ', studio_view_html.strip())
         xblock_body = re.sub(r'\W+', ' ', xblock_body.strip())
         self.assertIn(
@@ -108,54 +111,54 @@
         """
         Tests that the the string returned by get_problem_progress
         when the weight of the problem is singular, and the score is zero
         """
         self.xblock.score = 0
         self.xblock.weight = 1
         self.assertEqual(
-            _('(1 point possible)'),
+            '(1 point possible)',
             self.xblock._get_problem_progress(),
         )
 
     def test_problem_progress_score_zero_weight_plural(self):
         # pylint: disable=invalid-name, protected-access
         """
         Tests that the the string returned by get_problem_progress
         when the weight of the problem is plural, and the score is zero
         """
         self.xblock.score = 0
         self.xblock.weight = 3
         self.assertEqual(
-            _('(3 points possible)'),
+            '(3 points possible)',
             self.xblock._get_problem_progress(),
         )
 
     def test_problem_progress_score_positive_weight_singular(self):
         # pylint: disable=invalid-name, protected-access
         """
         Tests that the the string returned by get_problem_progress
         when the weight of the problem is singular, and the score is positive
         """
         self.xblock.score = 1
         self.xblock.weight = 1
         self.assertEqual(
-            _('(1/1 point)'),
+            '(1/1 point)',
             self.xblock._get_problem_progress(),
         )
 
     def test_problem_progress_score_positive_weight_plural(self):
         # pylint: disable=invalid-name, protected-access
         """
         Tests that the the string returned by get_problem_progress
         when the weight of the problem is plural, and the score is positive
         """
         self.xblock.score = 1
         self.xblock.weight = 3
         self.assertEqual(
-            _('(3/3 points)'),
+            '(3/3 points)',
             self.xblock._get_problem_progress(),
         )
 
     def test_used_attempts_feedback_blank(self):
         # pylint: disable=invalid-name, protected-access
         """
         Tests that get_used_attempts_feedback returns no feedback when
@@ -168,15 +171,15 @@
         # pylint: disable=invalid-name, protected-access
         """
         Tests that get_used_attempts_feedback returns the expected feedback
         """
         self.xblock.max_attempts = 5
         self.xblock.count_attempts = 3
         self.assertEqual(
-            _('You have used 3 of 5 submissions'),
+            'You have used 3 of 5 submissions',
             self.xblock._get_used_attempts_feedback(),
         )
 
     def test_submit_class_blank(self):
         # pylint: disable=protected-access
         """
         Tests that get_submit_class returns a blank value when appropriate
```

### Comparing `xblock-submit-and-compare-1.1.3/submit_and_compare/views.py` & `xblock-submit-and-compare-1.2.0/submit_and_compare/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Handle view logic for the XBlock
 """
 import logging
 
-from django.utils.translation import ungettext
-from django.utils.translation import ugettext as _
+from django.utils.translation import ngettext
+from django.utils.translation import gettext as _
 from lxml import etree
 from six import StringIO
 from xblock.core import XBlock
 from xblockutils.resources import ResourceLoader
 
 from .mixins.fragment import XBlockFragmentBuilderMixin
 
@@ -233,15 +233,15 @@
         """
         Returns the text with feedback to the user about the number of attempts
         they have used if applicable
         """
         result = ''
         if self.max_attempts > 0:
             # pylint: disable=no-member
-            result = ungettext(
+            result = ngettext(
                 'You have used {count_attempts} of {max_attempts} submission',
                 'You have used {count_attempts} of {max_attempts} submissions',
                 self.max_attempts,
             ).format(
                 count_attempts=self.count_attempts,
                 max_attempts=self.max_attempts,
             )
@@ -276,27 +276,27 @@
         Returns a statement of progress for the XBlock, which depends
         on the user's current score
         """
         if self.weight == 0:
             result = ''
         elif self.score == 0.0:
             result = "({})".format(
-                ungettext(
+                ngettext(
                     '{weight} point possible',
                     '{weight} points possible',
                     self.weight,
                 ).format(
                     weight=self.weight,
                 )
             )
         else:
             scaled_score = self.score * self.weight
             score_string = f'{scaled_score:g}'
             result = "({})".format(
-                ungettext(
+                ngettext(
                     score_string + '/' + "{weight} point",
                     score_string + '/' + "{weight} points",
                     self.weight,
                 ).format(
                     weight=self.weight,
                 )
             )
```

### Comparing `xblock-submit-and-compare-1.1.3/submit_and_compare/xblocks.py` & `xblock-submit-and-compare-1.2.0/submit_and_compare/xblocks.py`

 * *Files identical despite different names*

### Comparing `xblock-submit-and-compare-1.1.3/xblock_submit_and_compare.egg-info/PKG-INFO` & `xblock-submit-and-compare-1.2.0/xblock_submit_and_compare.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: xblock-submit-and-compare
-Version: 1.1.3
+Version: 1.2.0
 Summary: A submit-and-compare XBlock
 Home-page: https://github.com/Stanford-Online/xblock-submit-and-compare
 Author: stv
 Author-email: stv@stanford.edu
 License: AGPL-3.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Education
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
 
 Submit and Compare XBlock
 =========================
 
@@ -147,9 +144,7 @@
 .. |image-lms-view-normal| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/lms-view-normal.png
    :width: 100%
 .. |image-lms-view-zoom| image:: https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/lms-view-zoom.png
    :width: 100%
 .. _View a demo of the CMS: https://youtu.be/IcbGYfbav2w
 .. _View a demo of the LMS: https://youtu.be/0mpjuThDoyE
 .. https://s3-us-west-1.amazonaws.com/stanford-openedx-docs/xblocks/image-modal/static/images/xblock-image-modal-demo-lms.mov
-
-
```

### Comparing `xblock-submit-and-compare-1.1.3/xblock_submit_and_compare.egg-info/SOURCES.txt` & `xblock-submit-and-compare-1.2.0/xblock_submit_and_compare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

