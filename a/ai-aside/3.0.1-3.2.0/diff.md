# Comparing `tmp/ai-aside-3.0.1.tar.gz` & `tmp/ai-aside-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-aside-3.0.1.tar", last modified: Thu Jul 20 14:10:32 2023, max compression
+gzip compressed data, was "ai-aside-3.2.0.tar", last modified: Mon Jul 31 14:26:27 2023, max compression
```

## Comparing `ai-aside-3.0.1.tar` & `ai-aside-3.2.0.tar`

### file list

```diff
@@ -1,40 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:32.349169 ai-aside-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1732 2023-07-20 14:10:26.000000 ai-aside-3.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-20 14:10:26.000000 ai-aside-3.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-07-20 14:10:26.000000 ai-aside-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8514 2023-07-20 14:10:32.349169 ai-aside-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-07-20 14:10:26.000000 ai-aside-3.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:32.345168 ai-aside-3.0.1/ai_aside/
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     8561 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/block.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:32.349169 ai-aside-3.0.1/ai_aside/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1627 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/platform_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:32.349169 ai-aside-3.0.1/ai_aside/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      655 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      317 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1838 2023-07-20 14:10:26.000000 ai-aside-3.0.1/ai_aside/waffle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:32.345168 ai-aside-3.0.1/ai_aside.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8514 2023-07-20 14:10:32.000000 ai-aside-3.0.1/ai_aside.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-20 14:10:32.000000 ai-aside-3.0.1/ai_aside.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 14:10:32.000000 ai-aside-3.0.1/ai_aside.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-07-20 14:10:32.000000 ai-aside-3.0.1/ai_aside.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 14:10:32.000000 ai-aside-3.0.1/ai_aside.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-20 14:10:32.000000 ai-aside-3.0.1/ai_aside.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-20 14:10:32.000000 ai-aside-3.0.1/ai_aside.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:32.349169 ai-aside-3.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-20 14:10:26.000000 ai-aside-3.0.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-20 14:10:26.000000 ai-aside-3.0.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-07-20 14:10:32.349169 ai-aside-3.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5302 2023-07-20 14:10:26.000000 ai-aside-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:10:32.349169 ai-aside-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     9822 2023-07-20 14:10:26.000000 ai-aside-3.0.1/tests/test_block.py
--rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-07-20 14:10:26.000000 ai-aside-3.0.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2360 2023-07-20 14:10:26.000000 ai-aside-3.0.1/tests/test_text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 14:26:27.489581 ai-aside-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     2291 2023-07-31 14:26:22.000000 ai-aside-3.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-31 14:26:22.000000 ai-aside-3.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-07-31 14:26:22.000000 ai-aside-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    12822 2023-07-31 14:26:27.489581 ai-aside-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9820 2023-07-31 14:26:22.000000 ai-aside-3.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 14:26:27.485580 ai-aside-3.2.0/ai_aside/
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9174 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/block.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 14:26:27.485580 ai-aside-3.2.0/ai_aside/config_api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/config_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3231 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/config_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/config_api/internal.py
+-rw-r--r--   0 runner    (1001) docker     (122)      814 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/config_api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6269 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/config_api/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      362 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 14:26:27.485580 ai-aside-3.2.0/ai_aside/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1627 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/migrations/0002_auto_20230720_1544.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1855 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      968 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/platform_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 14:26:27.485580 ai-aside-3.2.0/ai_aside/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2611 2023-07-31 14:26:22.000000 ai-aside-3.2.0/ai_aside/waffle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 14:26:27.485580 ai-aside-3.2.0/ai_aside.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    12822 2023-07-31 14:26:27.000000 ai-aside-3.2.0/ai_aside.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      976 2023-07-31 14:26:27.000000 ai-aside-3.2.0/ai_aside.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 14:26:27.000000 ai-aside-3.2.0/ai_aside.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-07-31 14:26:27.000000 ai-aside-3.2.0/ai_aside.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 14:26:27.000000 ai-aside-3.2.0/ai_aside.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-07-31 14:26:27.000000 ai-aside-3.2.0/ai_aside.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-31 14:26:27.000000 ai-aside-3.2.0/ai_aside.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 14:26:27.485580 ai-aside-3.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-07-31 14:26:22.000000 ai-aside-3.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-31 14:26:22.000000 ai-aside-3.2.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-07-31 14:26:27.489581 ai-aside-3.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5394 2023-07-31 14:26:22.000000 ai-aside-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 14:26:27.489581 ai-aside-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    13106 2023-07-31 14:26:22.000000 ai-aside-3.2.0/tests/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-07-31 14:26:22.000000 ai-aside-3.2.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2360 2023-07-31 14:26:22.000000 ai-aside-3.2.0/tests/test_text_utils.py
```

### Comparing `ai-aside-3.0.1/CHANGELOG.rst` & `ai-aside-3.2.0/CHANGELOG.rst`

 * *Files 25% similar despite different names*

```diff
@@ -10,14 +10,32 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+3.2.0 – 2023-07-26
+**********************************************
+
+Features
+=========
+* Added the checks for the module settings behind the waffle flag `summaryhook.summaryhook_summaries_configuration`.
+* Added is this course configurable endpoint
+* Error suppression logs now include block ID
+* Missing video transcript is caught earlier in content fetch
+
+3.1.0 – 2023-07-20
+**********************************************
+
+Features
+=========
+
+* Added API endpoints for updating settings for courses and modules (enable/disable for now) (Has migrations)
+
 3.0.1 – 2023-07-20
 **********************************************
 
 * Add positive log when summary fragement decides to inject
 
 3.0.0 – 2023-07-16
 **********************************************
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_wkmd5tit_/tmphcvlb4y__TarContainer/0/1.rst", line 74, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_wkmd5tit_/tmphcvlb4y__TarContainer/0/1.rst", line 74, column 0: CDATA terminal not found*

```diff
@@ -1,14 +1,22 @@
 Change Log ########## .. All enhancements and patches to ai_aside will be
 documented in this file. It adheres to the structure of https://
 keepachangelog.com/ , but in reStructuredText instead of Markdown (for ease of
 incorporation into Sphinx documentation and the PyPI description). This project
 adheres to Semantic Versioning (https://semver.org/). .. There should always be
 an "Unreleased" section for changes pending release. Unreleased **********
-3.0.1 â 2023-07-20 ********************************************** * Add
-positive log when summary fragement decides to inject 3.0.0 â 2023-07-16
+3.2.0 â 2023-07-26 ********************************************** Features
+========= * Added the checks for the module settings behind the waffle flag
+`summaryhook.summaryhook_summaries_configuration`. * Added is this course
+configurable endpoint * Error suppression logs now include block ID * Missing
+video transcript is caught earlier in content fetch 3.1.0 â 2023-07-20
+********************************************** Features ========= * Added API
+endpoints for updating settings for courses and modules (enable/disable for
+now) (Has migrations) 3.0.1 â 2023-07-20
+********************************************** * Add positive log when summary
+fragement decides to inject 3.0.0 â 2023-07-16
 ********************************************** Features ========= * Summary
 content handler now requires a staff user identity, otherwise returns 403. This
 is a breaking change. * Added models to summaryhook_aside (Has migrations) *
 Catch exceptions in a couple of locations so the aside cannot crash content.
 2.0.2 â 2023-07-05 ********************************************** Fix ===== *
 Updated HTML parser to remove tags with their content for specific cases like `
```

### Comparing `ai-aside-3.0.1/LICENSE.txt` & `ai-aside-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.1/ai_aside/block.py` & `ai-aside-3.2.0/ai_aside/block.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 
 from django.conf import settings
 from django.template import Context, Template
 from web_fragments.fragment import Fragment
 from webob import Response
 from xblock.core import XBlock, XBlockAside
 
+from ai_aside.config_api.api import is_summary_enabled
 from ai_aside.platform_imports import get_block, get_text_transcript
 from ai_aside.text_utils import html_to_text
-from ai_aside.waffle import summary_enabled, summary_staff_only
+from ai_aside.waffle import summaries_configuration_enabled as ff_is_summary_config_enabled
+from ai_aside.waffle import summary_enabled as ff_summary_enabled
+from ai_aside.waffle import summary_staff_only as ff_summary_staff_only
 
 log = logging.getLogger(__name__)
 
 # map block types to what ai-spot expects for content types
 CATEGORY_TYPE_MAP = {
     "html": "TEXT",
     "video": "VIDEO",
@@ -52,24 +55,24 @@
     return template.render(Context(context))
 
 
 def _extract_child_contents(child, category):
     """
     Process the child contents based on its category.
 
-    Returns a string.
+    Returns a string or None if there are no contents available.
     """
     if category == 'html':
         content_html = child.get_html()
         text = html_to_text(content_html)
 
         return text
 
     if category == 'video':
-        transcript = get_text_transcript(child)
+        transcript = get_text_transcript(child)  # may be None
         return transcript
 
     return None
 
 
 def _parse_children_contents(block):
     """
@@ -187,15 +190,16 @@
 
         This function absorbs all exceptions to protect the LMS,
         delegating real work to _student_view_can_throw
         """
         try:
             return self._student_view_can_throw(block)
         except Exception as ex:  # pylint: disable=broad-exception-caught
-            log.error(f'Summary hook aside suppressed exception during student_view_aside: {ex}')
+            usage_id = block.scope_ids.usage_id
+            log.error(f'Summary hook aside suppressed exception on {usage_id} during student_view_aside: {ex}')
             return Fragment('')
 
     def _student_view_can_throw(self, block):
         """
         Render the aside contents for the student view.
 
         Returns a Fragment.
@@ -253,23 +257,34 @@
 
         This function absorbs all exceptions to protect the LMS,
         delegating real work to _should_apply_throws.
         """
         try:
             return cls._should_apply_can_throw(block)
         except Exception as ex:  # pylint: disable=broad-exception-caught
-            log.error(f'Summary hook aside suppressed exception during should_apply_to_block: {ex}')
+            usage_id = block.scope_ids.usage_id
+            log.error(f'Summary hook aside suppressed exception on {usage_id} during should_apply_to_block: {ex}')
             return False
 
     @classmethod
     def _should_apply_can_throw(cls, block):
         """
         Determine whether this aside should apply to a given block type, course, and user.
 
         This function can throw exceptions.
         """
         if getattr(block, 'category', None) != 'vertical':
             return False
+
         course_key = block.scope_ids.usage_id.course_key
-        if _staff_user(block) and summary_staff_only(course_key):
+        unit_key = block.scope_ids.usage_id
+
+        if _staff_user(block) and ff_summary_staff_only(course_key):
+            return True
+
+        if ff_is_summary_config_enabled(course_key):
+            return is_summary_enabled(course_key, unit_key)
+
+        if ff_summary_enabled(course_key):
             return True
-        return summary_enabled(course_key)
+
+        return False
```

### Comparing `ai-aside-3.0.1/ai_aside/migrations/0001_initial.py` & `ai-aside-3.2.0/ai_aside/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.1/ai_aside/models.py` & `ai-aside-3.2.0/ai_aside/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,25 +7,20 @@
 
 
 class AIAsideCourseEnabled(models.Model):
     """
     Maps Course Key to enabled boolean.
     """
 
-    course_key = CourseKeyField(db_index=True, max_length=255)
+    course_key = CourseKeyField(db_index=True, max_length=255, unique=True)
     enabled = models.BooleanField(default=False, null=False)
 
     created = models.DateTimeField(auto_now_add=True, db_index=True)
     modified = models.DateTimeField(auto_now=True)
 
-    class Meta:
-        """Default order."""
-
-        ordering = ['-created']
-
     def __str__(self):
         """Query."""
         return (
             "id={id} "
             "created={created} "
             "course_key={course_key} "
             "enabled={enabled}".format(
@@ -46,17 +41,17 @@
     unit_key = UsageKeyField(db_index=True, max_length=255)
     enabled = models.BooleanField(default=False, null=False)
 
     created = models.DateTimeField(auto_now_add=True, db_index=True)
     modified = models.DateTimeField(auto_now=True)
 
     class Meta:
-        """Default order."""
+        """Course and unit are unique together."""
 
-        ordering = ['-created']
+        unique_together = ('course_key', 'unit_key')
 
     def __str__(self):
         """Query."""
         return (
             "id={id} "
             "created={created} "
             "course_key={course_key} "
```

### Comparing `ai-aside-3.0.1/ai_aside/platform_imports.py` & `ai-aside-3.2.0/ai_aside/platform_imports.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,23 @@
 
 We know these functions will be available at run time, but they
 cannot be imported normally.
 """
 
 
 def get_text_transcript(video_block):
-    """Get the transcript for a video block in text format."""
+    """Get the transcript for a video block in text format, or None."""
     # pylint: disable=import-error, import-outside-toplevel
+    from xmodule.exceptions import NotFoundError
     from xmodule.video_block.transcripts_utils import get_transcript
-    transcript, _, _ = get_transcript(video_block, output_format='txt')
+    try:
+        transcript, _, _ = get_transcript(video_block, output_format='txt')
+    except NotFoundError:
+        # some old videos have no transcripts, just accept that reality
+        return None
     return transcript
 
 
 def get_block(usage_key):
     """Get a block from the module store given the usage key."""
     # pylint: disable=import-error, import-outside-toplevel
     from xmodule.modulestore.django import modulestore
```

### Comparing `ai-aside-3.0.1/ai_aside/settings/devstack.py` & `ai-aside-3.2.0/ai_aside/settings/devstack.py`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.1/ai_aside/text_utils.py` & `ai-aside-3.2.0/ai_aside/text_utils.py`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.1/ai_aside/waffle.py` & `ai-aside-3.2.0/ai_aside/waffle.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,43 +15,63 @@
 # .. toggle_use_cases: temporary
 # .. toggle_creation_date: 2023-03-06
 # .. toggle_target_removal_date: 2023-12-06
 # .. toggle_tickets: ACADEMIC-15709 (2U)
 # .. toggle_warning: None.
 SUMMARYHOOK_ENABLED = 'summaryhook_enabled'
 
-# Namespace
-WAFFLE_NAMESPACE = 'summaryhook'
 
 # .. toggle_name: summaryhook.staff_only
 # .. toggle_implementation: CourseWaffleFlag
 # .. toggle_default: False
 # .. toggle_description: Enables OpenAI driven summary xblock aside for staff only
 # .. toggle_use_cases: temporary
 # .. toggle_creation_date: 2023-03-14
 # .. toggle_target_removal_date: 2023-12-06
 # .. toggle_tickets: ACADEMIC-15709 (2U)
 # .. toggle_warning: None.
 SUMMARYHOOK_STAFF_ONLY = 'summaryhook_staff_only'
 
 
-def _get_summaryhook_waffle_flag(flag_name):
+# .. toggle_name: summaryhook.summaries_configuration
+# .. toggle_implementation: CourseWaffleFlag
+# .. toggle_default: False
+# .. toggle_description: Enables summaries configuration for course and/or unit
+# .. toggle_use_cases: temporary
+# .. toggle_creation_date: 2023-07-24
+# .. toggle_target_removal_date: 2024-04-06
+# .. toggle_tickets: ACADEMIC-16209 (2U)
+# .. toggle_warning: None.
+SUMMARYHOOK_SUMMARIES_CONFIGURATION = 'summaryhook_summaries_configuration'
+
+
+def _is_get_summaryhook_waffle_flag_enabled(flag_name, course_key):
     """
     Import and return Waffle flag for enabling the summary hook.
     """
-    # pylint: disable=import-error,import-outside-toplevel
-    from openedx.core.djangoapps.waffle_utils import CourseWaffleFlag
-    return CourseWaffleFlag(f'{WAFFLE_NAMESPACE}.{flag_name}', __name__)
+    # pylint: disable=import-outside-toplevel
+    try:
+        from openedx.core.djangoapps.waffle_utils import CourseWaffleFlag
+        return CourseWaffleFlag(f'{WAFFLE_NAMESPACE}.{flag_name}', __name__).is_enabled(course_key)
+    except ImportError:
+        return False
 
 
 def summary_enabled(course_key):
     """
     Return whether the summaryhook.summaryhook_enabled WaffleFlag is on.
     """
-    return _get_summaryhook_waffle_flag(SUMMARYHOOK_ENABLED).is_enabled(course_key)
+    return _is_get_summaryhook_waffle_flag_enabled(SUMMARYHOOK_ENABLED, course_key)
 
 
 def summary_staff_only(course_key):
     """
     Return whether the summaryhook.summaryhook_staff_only WaffleFlag is on.
     """
-    return _get_summaryhook_waffle_flag(SUMMARYHOOK_STAFF_ONLY).is_enabled(course_key)
+    return _is_get_summaryhook_waffle_flag_enabled(SUMMARYHOOK_STAFF_ONLY, course_key)
+
+
+def summaries_configuration_enabled(course_key):
+    """
+    Return whether the summaryhook.summaryhook_summaries_configuration WaffleFlag is on.
+    """
+    return _is_get_summaryhook_waffle_flag_enabled(SUMMARYHOOK_SUMMARIES_CONFIGURATION, course_key)
```

### Comparing `ai-aside-3.0.1/ai_aside.egg-info/SOURCES.txt` & `ai-aside-3.2.0/ai_aside.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -3,27 +3,34 @@
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 ai_aside/__init__.py
 ai_aside/apps.py
 ai_aside/block.py
+ai_aside/constants.py
 ai_aside/models.py
 ai_aside/platform_imports.py
 ai_aside/text_utils.py
 ai_aside/urls.py
 ai_aside/waffle.py
 ai_aside.egg-info/PKG-INFO
 ai_aside.egg-info/SOURCES.txt
 ai_aside.egg-info/dependency_links.txt
 ai_aside.egg-info/entry_points.txt
 ai_aside.egg-info/not-zip-safe
 ai_aside.egg-info/requires.txt
 ai_aside.egg-info/top_level.txt
+ai_aside/config_api/__init__.py
+ai_aside/config_api/api.py
+ai_aside/config_api/internal.py
+ai_aside/config_api/urls.py
+ai_aside/config_api/views.py
 ai_aside/migrations/0001_initial.py
+ai_aside/migrations/0002_auto_20230720_1544.py
 ai_aside/migrations/__init__.py
 ai_aside/settings/__init__.py
 ai_aside/settings/common.py
 ai_aside/settings/devstack.py
 ai_aside/settings/production.py
 requirements/base.in
 requirements/constraints.txt
```

### Comparing `ai-aside-3.0.1/requirements/constraints.txt` & `ai-aside-3.2.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.1/setup.py` & `ai-aside-3.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,13 +129,16 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
     entry_points={
         "lms.djangoapp": [
             "ai_aside = ai_aside.apps:AiAsideConfig",
         ],
+        "cms.djangoapp": [
+            "ai_aside = ai_aside.apps:AiAsideConfig",
+        ],
         "xblock_asides.v1": [
             "summaryhook_aside = ai_aside.block:SummaryHookAside",
         ],
     },
 
 )
```

### Comparing `ai-aside-3.0.1/tests/test_block.py` & `ai-aside-3.2.0/tests/test_block.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,17 +44,25 @@
         return self.children
 
 
 @override_settings(SUMMARY_HOOK_MIN_SIZE=40, HTML_TAGS_TO_REMOVE=['script', 'style', 'test'])
 class TestSummaryHookAside(TestCase):
     """Summary hook aside tests"""
     def setUp(self):
-        module_mock = MagicMock()
-        module_mock.get_transcript = fake_get_transcript
-        modules = {'xmodule.video_block.transcripts_utils': module_mock}
+        transcript_utils_mock = MagicMock()
+        transcript_utils_mock.get_transcript = fake_get_transcript
+
+        xmodule_exceptions_mock = MagicMock()
+        xmodule_exceptions_mock.NotFoundError = MagicMock()
+
+        modules = {
+            'xmodule.exceptions': xmodule_exceptions_mock,
+            'xmodule.video_block.transcripts_utils': transcript_utils_mock,
+        }
+
         patch.dict('sys.modules', modules).start()
 
     def test_format_date(self):
         date = datetime(2023, 5, 1, 12, 0, 0)
         formatted_date = _format_date(date)
         self.assertEqual(formatted_date, '2023-05-01 12:00:00')
 
@@ -258,9 +266,85 @@
 
         length, items = _parse_children_contents(block)
 
         self.assertEqual(length, 0)
         self.assertEqual(items, [])
 
 
+@override_settings(SUMMARY_HOOK_MIN_SIZE=40, HTML_TAGS_TO_REMOVE=['script', 'style', 'test'])
+class TestSummaryHookAsideMissingTranscript(TestCase):
+    """Summary hook aside tests for the case where a transcript is missing"""
+    def setUp(self):
+        class FakeNotFoundError(BaseException):
+            pass
+
+        xmodule_exceptions_mock = MagicMock()
+        xmodule_exceptions_mock.NotFoundError = FakeNotFoundError
+
+        def error_get_transcript(child, lang=None, output_format='SRT',
+                                 youtube_id=None):
+            raise FakeNotFoundError()
+
+        transcript_utils_mock = MagicMock()
+        transcript_utils_mock.get_transcript = error_get_transcript
+
+        modules = {
+            'xmodule.exceptions': xmodule_exceptions_mock,
+            'xmodule.video_block.transcripts_utils': transcript_utils_mock,
+        }
+
+        patch.dict('sys.modules', modules).start()
+
+    def test_extract_child_contents_with_broken_video(self):
+        category = 'video'
+
+        child = FakeChild(category)
+        content = _extract_child_contents(child, category)
+        self.assertEqual(content, None)
+
+    def test_parse_children_contents_with_partly_valid_children(self):
+        children = [
+            FakeChild('html', '01', '''
+                <p>
+                    Lorem ipsum dolor sit amet, consectetur adipiscing elit.
+                    Vivamus dapibus elit lacus, at vehicula arcu vehicula in.
+                    In id felis arcu. Maecenas elit quam, volutpat cursus pharetra vel, tempor at lorem.
+                    Fusce luctus orci quis tempor aliquet.
+                </p>'''),
+            FakeChild('html', '02', '''
+                <Everything on the content on this child is inside a tag, so parsing it would return almost>
+                    Nothing
+                </The quick brown fox jumps over the lazy dog>'''),
+            FakeChild('video', '03'),
+            FakeChild('unknown', '04'),
+        ]
+        block = FakeBlock(children)
+
+        expected_length, expected_items = (
+            245,
+            [{
+                'definition_id': 'def-id-01',
+                'content_type': 'TEXT',
+                'content_text': dedent('''\
+                    Lorem ipsum dolor sit amet, consectetur adipiscing elit.
+                    Vivamus dapibus elit lacus, at vehicula arcu vehicula in.
+                    In id felis arcu. Maecenas elit quam, volutpat cursus pharetra vel, tempor at lorem.
+                    Fusce luctus orci quis tempor aliquet.'''),
+                'published_on': 'published-on-01',
+                'edited_on': 'edited-on-01',
+            }, {
+                'definition_id': 'def-id-02',
+                'content_type': 'TEXT',
+                'content_text': 'Nothing',
+                'published_on': 'published-on-02',
+                'edited_on': 'edited-on-02',
+            }]
+        )
+
+        length, items = _parse_children_contents(block)
+
+        self.assertEqual(length, expected_length)
+        self.assertEqual(items, expected_items)
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ai-aside-3.0.1/tests/test_models.py` & `ai-aside-3.2.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ai-aside-3.0.1/tests/test_text_utils.py` & `ai-aside-3.2.0/tests/test_text_utils.py`

 * *Files identical despite different names*

