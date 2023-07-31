# Comparing `tmp/staff_graded-xblock-2.0.1.tar.gz` & `tmp/staff_graded-xblock-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staff_graded-xblock-2.0.1.tar", last modified: Thu Apr  7 17:37:04 2022, max compression
+gzip compressed data, was "staff_graded-xblock-2.1.1.tar", last modified: Mon Jul 31 11:20:08 2023, max compression
```

## Comparing `staff_graded-xblock-2.0.1.tar` & `staff_graded-xblock-2.1.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 17:37:04.249620 staff_graded-xblock-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-04-07 17:36:58.000000 staff_graded-xblock-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-04-07 17:37:04.249620 staff_graded-xblock-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6093 2022-04-07 17:36:58.000000 staff_graded-xblock-2.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 17:37:04.249620 staff_graded-xblock-2.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-04-07 17:36:58.000000 staff_graded-xblock-2.0.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-07 17:37:04.249620 staff_graded-xblock-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-04-07 17:36:58.000000 staff_graded-xblock-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 17:37:04.249620 staff_graded-xblock-2.0.1/staff_graded/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-07 17:36:58.000000 staff_graded-xblock-2.0.1/staff_graded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10984 2022-04-07 17:36:58.000000 staff_graded-xblock-2.0.1/staff_graded/staff_graded.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 17:37:04.249620 staff_graded-xblock-2.0.1/staff_graded/static/
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-04-07 17:36:58.000000 staff_graded-xblock-2.0.1/staff_graded/static/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 17:37:04.249620 staff_graded-xblock-2.0.1/staff_graded/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-04-07 17:36:58.000000 staff_graded-xblock-2.0.1/staff_graded/static/css/staff_graded.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 17:37:04.249620 staff_graded-xblock-2.0.1/staff_graded/static/html/
--rw-r--r--   0 runner    (1001) docker     (121)     3390 2022-04-07 17:36:58.000000 staff_graded-xblock-2.0.1/staff_graded/static/html/staff_graded.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 17:37:04.249620 staff_graded-xblock-2.0.1/staff_graded/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 17:37:04.249620 staff_graded-xblock-2.0.1/staff_graded/static/js/src/
--rw-r--r--   0 runner    (1001) docker     (121)     3485 2022-04-07 17:36:58.000000 staff_graded-xblock-2.0.1/staff_graded/static/js/src/staff_graded.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 17:37:04.249620 staff_graded-xblock-2.0.1/staff_graded_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-04-07 17:37:04.000000 staff_graded-xblock-2.0.1/staff_graded_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-04-07 17:37:04.000000 staff_graded-xblock-2.0.1/staff_graded_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-07 17:37:04.000000 staff_graded-xblock-2.0.1/staff_graded_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-04-07 17:37:04.000000 staff_graded-xblock-2.0.1/staff_graded_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-04-07 17:37:04.000000 staff_graded-xblock-2.0.1/staff_graded_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-04-07 17:37:04.000000 staff_graded-xblock-2.0.1/staff_graded_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 11:20:08.711184 staff_graded-xblock-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-31 11:20:04.000000 staff_graded-xblock-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-31 11:20:04.000000 staff_graded-xblock-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-07-31 11:20:08.711184 staff_graded-xblock-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6105 2023-07-31 11:20:04.000000 staff_graded-xblock-2.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 11:20:08.707184 staff_graded-xblock-2.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-07-31 11:20:04.000000 staff_graded-xblock-2.1.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-31 11:20:08.711184 staff_graded-xblock-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2831 2023-07-31 11:20:04.000000 staff_graded-xblock-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 11:20:08.707184 staff_graded-xblock-2.1.1/staff_graded/
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-07-31 11:20:04.000000 staff_graded-xblock-2.1.1/staff_graded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11681 2023-07-31 11:20:04.000000 staff_graded-xblock-2.1.1/staff_graded/staff_graded.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 11:20:08.707184 staff_graded-xblock-2.1.1/staff_graded/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-07-31 11:20:04.000000 staff_graded-xblock-2.1.1/staff_graded/static/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 11:20:08.707184 staff_graded-xblock-2.1.1/staff_graded/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-31 11:20:04.000000 staff_graded-xblock-2.1.1/staff_graded/static/css/staff_graded.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 11:20:08.707184 staff_graded-xblock-2.1.1/staff_graded/static/html/
+-rw-r--r--   0 runner    (1001) docker     (122)     3390 2023-07-31 11:20:04.000000 staff_graded-xblock-2.1.1/staff_graded/static/html/staff_graded.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 11:20:08.707184 staff_graded-xblock-2.1.1/staff_graded/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 11:20:08.707184 staff_graded-xblock-2.1.1/staff_graded/static/js/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     3485 2023-07-31 11:20:04.000000 staff_graded-xblock-2.1.1/staff_graded/static/js/src/staff_graded.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 11:20:08.711184 staff_graded-xblock-2.1.1/staff_graded_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-07-31 11:20:08.000000 staff_graded-xblock-2.1.1/staff_graded_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-31 11:20:08.000000 staff_graded-xblock-2.1.1/staff_graded_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 11:20:08.000000 staff_graded-xblock-2.1.1/staff_graded_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-31 11:20:08.000000 staff_graded-xblock-2.1.1/staff_graded_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-07-31 11:20:08.000000 staff_graded-xblock-2.1.1/staff_graded_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-31 11:20:08.000000 staff_graded-xblock-2.1.1/staff_graded_xblock.egg-info/top_level.txt
```

### Comparing `staff_graded-xblock-2.0.1/README.rst` & `staff_graded-xblock-2.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 See `edx-developer-guide <https://edx.readthedocs.io/projects/edx-developer-guide/en/latest/internationalization/i18n.html#javascript-files>`_
 for more information.
 
 2. Run i18n tools to create Raw message catalogs
 -------------------------------------------------
 
 This cookiecutter template offers multiple make targets which are shortcuts to
-use `edx-i18n-tools <https://github.com/edx/i18n-tools>`_.
+use `edx-i18n-tools <https://github.com/openedx/i18n-tools>`_.
 
 After marking strings as translatable we have to create the raw message catalogs.
 These catalogs are created in ``.po`` files. For more information see
 `GNU PO file documentation <https://www.gnu.org/software/gettext/manual/html_node/PO-Files.html>`_.
 These catalogs can be created by running::
 
 
@@ -95,15 +95,15 @@
 For more information see
 `GNU PO file documentation <https://www.gnu.org/software/gettext/manual/html_node/PO-Files.html>`_.
 
 To use translations from transifex use the follow Make target to pull translations::
 
     $ make pull_translations
 
-See `config instructions <https://github.com/edx/i18n-tools#transifex-commands>`_ for information on how to set up your
+See `config instructions <https://github.com/openedx/i18n-tools#transifex-commands>`_ for information on how to set up your
 transifex credentials.
 
 See `transifex documentation <https://docs.transifex.com/integrations/django>`_ for more details about integrating
 django with transiflex.
 
 3.2 Compile translations
 *************************
@@ -118,15 +118,15 @@
 After compiling the ``.po`` file(s), ``django-statici18n`` is used to create language specific catalogs. See
 ``django-statici18n`` `documentation <https://django-statici18n.readthedocs.io/en/latest/>`_ for more information.
 
 To upload translations to transiflex use the follow Make target::
 
     $ make push_translations
 
-See `config instructions <https://github.com/edx/i18n-tools#transifex-commands>`_ for information on how to set up your
+See `config instructions <https://github.com/openedx/i18n-tools#transifex-commands>`_ for information on how to set up your
 transifex credentials.
 
 See `transifex documentation <https://docs.transifex.com/integrations/django>`_ for more details about integrating
 django with transiflex.
 
  **Note:** The ``dev.run`` make target will automatically compile any translations.
```

### Comparing `staff_graded-xblock-2.0.1/setup.py` & `staff_graded-xblock-2.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,25 +61,26 @@
 VERSION = get_version("staff_graded/__init__.py")
 
 
 setup(
     name='staff_graded-xblock',
     version=VERSION,
     description='Staff Graded XBlock',   # TODO: write a better description.
+    long_description='Staff Graded XBlock',  # TODO: write a better description.
     license='AGPL v3',          # TODO: choose a license: 'AGPL v3' and 'Apache 2.0' are popular.
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
     ],
     packages=[
         'staff_graded',
     ],
     install_requires=load_requirements('requirements/base.in'),
     entry_points={
         'xblock.v1': [
```

### Comparing `staff_graded-xblock-2.0.1/staff_graded/staff_graded.py` & `staff_graded-xblock-2.1.1/staff_graded/staff_graded.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,34 +18,34 @@
 from xblockutils.resources import ResourceLoader
 from xblockutils.studio_editable import StudioEditableXBlockMixin
 
 try:
     from openedx.core.djangoapps.course_groups.cohorts import \
         get_course_cohorts
 except ImportError:
-    get_course_cohorts = lambda course_key: []
+    get_course_cohorts = lambda course_key: []  # pylint: disable=unnecessary-lambda-assignment
 
 try:
     from common.djangoapps.course_modes.models import CourseMode
     modes_for_course = CourseMode.modes_for_course
 except ImportError:
-    modes_for_course = lambda course_key: [('audit', 'Audit Track'), ('masters', "Master's Track"),
+    modes_for_course = lambda course_key: [('audit', 'Audit Track'), ('masters', "Master's Track"), # pylint: disable=unnecessary-lambda-assignment
                                            ('verified', "Verified Track")]
 
 from bulk_grades.api import ScoreCSVProcessor, get_score, set_score
 
-_ = lambda text: text
+_ = lambda text: text   # pylint: disable=unnecessary-lambda-assignment
 
 log = logging.getLogger(__name__)
 
 
 @XBlock.needs('settings')
 @XBlock.needs('i18n')
 @XBlock.needs('user')
-class StaffGradedXBlock(StudioEditableXBlockMixin, ScorableXBlockMixin, XBlock):
+class StaffGradedXBlock(StudioEditableXBlockMixin, ScorableXBlockMixin, XBlock):    # pylint: disable=abstract-method
     """
     Staff Graded Points block
     """
     display_name = String(
         display_name=_("Display Name"),
         help=_("The display name for this component."),
         scope=Scope.settings,
@@ -96,41 +96,41 @@
         statici18n_js_url = self._get_statici18n_js_url()
         if statici18n_js_url:
             frag.add_javascript_url(self.runtime.local_resource_url(self, statici18n_js_url))
 
         frag.add_javascript(self.resource_string("static/js/src/staff_graded.js"))
         frag.initialize_js('StaffGradedXBlock')
 
-        context['id'] = self.location.html_id()
+        context['id'] = self.location.html_id()     # pylint: disable=no-member
         context['instructions'] = markdown.markdown(self.instructions)
         context['display_name'] = self.display_name
         context['is_staff'] = self.runtime.user_is_staff
 
-        course_id = self.location.course_key
+        course_id = self.location.course_key     # pylint: disable=no-member
         context['available_cohorts'] = [cohort.name for cohort in get_course_cohorts(course_id=course_id)]
         context['available_tracks'] = [
-            (mode.slug, mode.name) for mode in
+            (mode.slug, mode.name) for mode in       # pylint: disable=no-member
             modes_for_course(course_id, only_selectable=False)
             ]
 
         if context['is_staff']:
-            from crum import get_current_request
-            from django.middleware.csrf import get_token
+            from crum import get_current_request        # pylint: disable=import-outside-toplevel
+            from django.middleware.csrf import get_token      # pylint: disable=import-outside-toplevel
             context['import_url'] = self.runtime.handler_url(self, "csv_import_handler")
             context['export_url'] = self.runtime.handler_url(self, "csv_export_handler")
             context['poll_url'] = self.runtime.handler_url(self, "get_results_handler")
             context['csrf_token'] = get_token(get_current_request())
             frag.add_javascript(loader.load_unicode('static/js/src/staff_graded.js'))
             frag.initialize_js('StaffGradedProblem',
                                json_args={k: context[k]
                                           for k
                                           in ('csrf_token', 'import_url', 'export_url', 'poll_url', 'id')})
 
         try:
-            score = get_score(self.location, self.runtime.user_id) or {}
+            score = get_score(self.location, self.runtime.user_id) or {}      # pylint: disable=no-member
             context['grades_available'] = True
         except NoSuchServiceError:
             context['grades_available'] = False
         else:
             if score:
                 grade = score['score']
                 context['score_string'] = _('{score} / {total} points').format(score=grade, total=self.weight)
@@ -159,15 +159,15 @@
 
     @staticmethod
     def _get_statici18n_js_url():
         """
         Returns the Javascript translation file for the currently selected language, if any.
         Defaults to English if available.
         """
-        from django.utils import translation
+        from django.utils import translation     # pylint: disable=import-outside-toplevel
         locale_code = translation.get_language()
         if locale_code is None:
             return None
         text_js = 'public/js/translations/{locale_code}/text.js'
         lang_code = locale_code.split('-')[0]
         for code in (locale_code, lang_code, 'en'):
             loader = ResourceLoader(__name__)
@@ -177,15 +177,15 @@
         return None
 
     @staticmethod
     def get_dummy():
         """
         Dummy method to generate initial i18n
         """
-        from django.utils import translation
+        from django.utils import translation      # pylint: disable=import-outside-toplevel
         return translation.gettext_noop('Dummy')
 
     @XBlock.handler
     def csv_import_handler(self, request, suffix=''):  # pylint: disable=unused-argument
         """
         Endpoint that handles CSV uploads.
         """
@@ -195,16 +195,16 @@
         _ = self.runtime.service(self, "i18n").ugettext
 
         try:
             score_file = request.POST['csv'].file
         except KeyError:
             data = {'error_rows': [1], 'error_messages': [_('missing file')]}
         else:
-            log.info('Processing %d byte score file %s for %s', score_file.size, score_file.name, self.location)
-            block_id = self.location
+            log.info('Processing %d byte score file %s for %s', score_file.size, score_file.name, self.location)     # pylint: disable=no-member
+            block_id = self.location     # pylint: disable=no-member
             block_weight = self.weight
             processor = ScoreCSVProcessor(
                 block_id=str(block_id),
                 max_points=block_weight,
                 user_id=self.runtime.user_id)
             processor.process_file(score_file, autocommit=True)
             data = processor.status()
@@ -226,22 +226,22 @@
             return Response('not allowed', status_code=403)
 
         track = request.GET.get('track', None)
         cohort = request.GET.get('cohort', None)
 
         buf = io.StringIO()
         ScoreCSVProcessor(
-            block_id=str(self.location),
+            block_id=str(self.location),      # pylint: disable=no-member
             max_points=self.weight,
             display_name=self.display_name,
             track=track,
             cohort=cohort).write_file(buf)
         resp = Response(buf.getvalue())
         resp.content_type = 'text/csv'
-        resp.content_disposition = f'attachment; filename="{self.location}.csv"'
+        resp.content_disposition = f'attachment; filename="{self.location}.csv"'     # pylint: disable=no-member
         return resp
 
     @XBlock.handler
     def get_results_handler(self, request, suffix=''):  # pylint: disable=unused-argument
         """
         Endpoint to poll for celery results.
         """
@@ -268,15 +268,15 @@
         """
         Return a raw score already persisted on the XBlock.  Should not
         perform new calculations.
 
         Returns:
             Score(raw_earned=float, raw_possible=float)
         """
-        score = get_score(self.runtime.user_id, self.location)
+        score = get_score(self.runtime.user_id, self.location)     # pylint: disable=no-member
         score = score or {'grade': 0, 'max_grade': 1}
         return Score(raw_earned=score['grade'], raw_possible=score['max_grade'])
 
     def set_score(self, score):
         """
         Persist a score to the XBlock.
 
@@ -287,15 +287,15 @@
         Arguments:
             score: Score(raw_earned=float, raw_possible=float)
 
         Returns:
             None
         """
         state = json.dumps({'grader': self._get_current_username()})
-        set_score(self.location,
+        set_score(self.location,     # pylint: disable=no-member
                   self.runtime.user_id,
                   score.raw_earned,
                   score.raw_possible,
                   state=state)
 
     def publish_grade(self):
         pass
```

### Comparing `staff_graded-xblock-2.0.1/staff_graded/static/README.txt` & `staff_graded-xblock-2.1.1/staff_graded/static/README.txt`

 * *Files identical despite different names*

### Comparing `staff_graded-xblock-2.0.1/staff_graded/static/html/staff_graded.html` & `staff_graded-xblock-2.1.1/staff_graded/static/html/staff_graded.html`

 * *Files identical despite different names*

### Comparing `staff_graded-xblock-2.0.1/staff_graded/static/js/src/staff_graded.js` & `staff_graded-xblock-2.1.1/staff_graded/static/js/src/staff_graded.js`

 * *Files identical despite different names*

### Comparing `staff_graded-xblock-2.0.1/staff_graded_xblock.egg-info/PKG-INFO` & `staff_graded-xblock-2.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
-Name: staff-graded-xblock
-Version: 2.0.1
+Name: staff_graded-xblock
+Version: 2.1.1
 Summary: Staff Graded XBlock
 License: AGPL v3
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-
-UNKNOWN
+Classifier: Framework :: Django :: 4.2
+License-File: LICENSE
 
+Staff Graded XBlock
```

### Comparing `staff_graded-xblock-2.0.1/staff_graded_xblock.egg-info/SOURCES.txt` & `staff_graded-xblock-2.1.1/staff_graded_xblock.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.rst
 setup.py
 requirements/base.in
 staff_graded/__init__.py
 staff_graded/staff_graded.py
 staff_graded/static/README.txt
```

