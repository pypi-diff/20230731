# Comparing `tmp/edxval-2.3.0.tar.gz` & `tmp/edxval-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edxval-2.3.0.tar", last modified: Mon Jun 12 11:15:24 2023, max compression
+gzip compressed data, was "edxval-2.4.0.tar", last modified: Mon Jul 31 09:46:09 2023, max compression
```

## Comparing `edxval-2.3.0.tar` & `edxval-2.4.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:24.443369 edxval-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)    35135 2023-06-12 11:15:19.000000 edxval-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-12 11:15:19.000000 edxval-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-12 11:15:24.443369 edxval-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-06-12 11:15:19.000000 edxval-2.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:24.439369 edxval-2.3.0/edxval/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4084 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    44550 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:24.443369 edxval-2.3.0/edxval/config/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/config/waffle.py
--rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:24.443369 edxval-2.3.0/edxval/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)    10986 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/migrations/0001_squashed_0016_add_transcript_credentials_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      464 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/migrations/0002_add_error_description_field.py
--rw-r--r--   0 runner    (1001) docker     (122)      447 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/migrations/0003_delete_transcriptcredentials.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22828 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:24.443369 edxval-2.3.0/edxval/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10706 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (122)   129574 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     5488 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3463 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/test_transcript_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    42047 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/transcript_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     8793 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    14390 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/views.py
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-06-12 11:15:19.000000 edxval-2.3.0/edxval/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:24.443369 edxval-2.3.0/edxval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-12 11:15:24.000000 edxval-2.3.0/edxval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-12 11:15:24.000000 edxval-2.3.0/edxval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 11:15:24.000000 edxval-2.3.0/edxval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-06-12 11:15:24.000000 edxval-2.3.0/edxval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-12 11:15:24.000000 edxval-2.3.0/edxval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 11:15:24.443369 edxval-2.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-06-12 11:15:19.000000 edxval-2.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      119 2023-06-12 11:15:19.000000 edxval-2.3.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      789 2023-06-12 11:15:24.443369 edxval-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2716 2023-06-12 11:15:19.000000 edxval-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:46:09.737382 edxval-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    35135 2023-07-31 09:46:04.000000 edxval-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-31 09:46:04.000000 edxval-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-07-31 09:46:09.737382 edxval-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-07-31 09:46:04.000000 edxval-2.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:46:09.733381 edxval-2.4.0/edxval/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3865 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44550 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:46:09.737382 edxval-2.4.0/edxval/config/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/config/waffle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:46:09.737382 edxval-2.4.0/edxval/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)    10986 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/migrations/0001_squashed_0016_add_transcript_credentials_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      464 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/migrations/0002_add_error_description_field.py
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/migrations/0003_delete_transcriptcredentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22828 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:46:09.737382 edxval-2.4.0/edxval/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10706 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)   129574 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5488 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3463 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/tests/test_transcript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42047 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/transcript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8793 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14390 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-07-31 09:46:04.000000 edxval-2.4.0/edxval/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:46:09.733381 edxval-2.4.0/edxval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-07-31 09:46:09.000000 edxval-2.4.0/edxval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-07-31 09:46:09.000000 edxval-2.4.0/edxval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 09:46:09.000000 edxval-2.4.0/edxval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-31 09:46:09.000000 edxval-2.4.0/edxval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-31 09:46:09.000000 edxval-2.4.0/edxval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:46:09.737382 edxval-2.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-07-31 09:46:04.000000 edxval-2.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-07-31 09:46:04.000000 edxval-2.4.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-07-31 09:46:09.737382 edxval-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2716 2023-07-31 09:46:04.000000 edxval-2.4.0/setup.py
```

### Comparing `edxval-2.3.0/LICENSE` & `edxval-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/PKG-INFO` & `edxval-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edxval
-Version: 2.3.0
+Version: 2.4.0
 Summary: edx-val
 Home-page: http://github.com/openedx/edx-val
 Author: edX
 License: AGPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `edxval-2.3.0/README.rst` & `edxval-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/admin.py` & `edxval-2.4.0/edxval/admin.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     TranscriptPreference,
     Video,
     VideoImage,
     VideoTranscript,
 )
 
 
+@admin.register(Profile)
 class ProfileAdmin(admin.ModelAdmin):
     """ Admin for profile """
     list_display = ('id', 'profile_name')
     list_display_links = ('id', 'profile_name')
     admin_order_field = 'profile_name'
 
 
@@ -33,99 +34,95 @@
     """ Admin for CourseVideo """
     model = CourseVideo
     extra = 0
     verbose_name = "Course"
     verbose_name_plural = "Courses"
 
 
+@admin.register(Video)
 class VideoAdmin(admin.ModelAdmin):
     """ Admin for Video """
     list_display = (
         'id', 'edx_video_id', 'client_video_id', 'duration', 'created', 'status'
     )
     list_display_links = ('id', 'edx_video_id')
     search_fields = ('id', 'edx_video_id', 'client_video_id', 'status')
     list_per_page = 50
     admin_order_field = 'edx_video_id'
     inlines = [CourseVideoInline, EncodedVideoInline]
 
 
+@admin.register(VideoImage)
 class VideoImageAdmin(admin.ModelAdmin):
     """ Admin for VideoImage """
     raw_id_fields = ('course_video', )
     list_display = ('get_course_video', 'image', 'generated_images')
     search_fields = ('id', 'course_video__course_id', 'course_video__video__edx_video_id', 'generated_images')
 
+    @admin.display(
+        description='Course Video',
+        ordering='course_video',
+    )
     def get_course_video(self, obj):
         """ get course video """
         return '"{course_id}" -- "{edx_video_id}" '.format(
             course_id=obj.course_video.course_id,
             edx_video_id=obj.course_video.video.edx_video_id
         )
-
-    get_course_video.admin_order_field = 'course_video'
-    get_course_video.short_description = 'Course Video'
-
     model = VideoImage
-
     verbose_name = 'Video Image'
     verbose_name_plural = 'Video Images'
 
 
+@admin.register(CourseVideo)
 class CourseVideoAdmin(admin.ModelAdmin):
     """ Admin for CourseVideo """
     list_display = ('course_id', 'get_video_id', 'is_hidden')
     search_fields = ('id', 'course_id', 'video__status', 'video__edx_video_id')
 
+    @admin.display(
+        description='edX Video Id',
+        ordering='video',
+    )
     def get_video_id(self, obj):
         """ get video id """
         return obj.video.edx_video_id
-
-    get_video_id.admin_order_field = 'video'
-    get_video_id.short_description = 'edX Video Id'
-
     model = CourseVideo
     verbose_name = 'Course Video'
     verbose_name_plural = 'Course Videos'
 
 
+@admin.register(VideoTranscript)
 class VideoTranscriptAdmin(admin.ModelAdmin):
     """ Admin for VideoTranscript """
     raw_id_fields = ('video',)
     list_display = ('get_video', 'language_code', 'provider', 'file_format')
     search_fields = ('id', 'video__edx_video_id', 'language_code')
 
+    @admin.display(
+        description='Video',
+        ordering='video',
+    )
     def get_video(self, transcript):
         """ get video """
         return transcript.video.edx_video_id if getattr(transcript, 'video', False) else ''
-
-    get_video.admin_order_field = 'video'
-    get_video.short_description = 'Video'
-
     model = VideoTranscript
     verbose_name = 'Video Transcript'
     verbose_name_plural = 'Video Transcripts'
 
 
+@admin.register(TranscriptPreference)
 class TranscriptPreferenceAdmin(admin.ModelAdmin):
     """ Admin for TranscriptPreference """
     list_display = ('course_id', 'provider', 'video_source_language', 'preferred_languages')
 
     model = TranscriptPreference
 
 
+@admin.register(ThirdPartyTranscriptCredentialsState)
 class ThirdPartyTranscriptCredentialsStateAdmin(admin.ModelAdmin):
     """ Admin for ThirdPartyTranscriptCredentialsState  """
     list_display = ('org', 'provider', 'has_creds', 'created', 'modified')
 
     model = ThirdPartyTranscriptCredentialsState
     verbose_name = 'Organization Transcript Credential State'
     verbose_name_plural = 'Organization Transcript Credentials State'
-
-
-admin.site.register(Profile, ProfileAdmin)
-admin.site.register(Video, VideoAdmin)
-admin.site.register(VideoTranscript, VideoTranscriptAdmin)
-admin.site.register(TranscriptPreference, TranscriptPreferenceAdmin)
-admin.site.register(VideoImage, VideoImageAdmin)
-admin.site.register(CourseVideo, CourseVideoAdmin)
-admin.site.register(ThirdPartyTranscriptCredentialsState, ThirdPartyTranscriptCredentialsStateAdmin)
```

### Comparing `edxval-2.3.0/edxval/api.py` & `edxval-2.4.0/edxval/api.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/config/waffle.py` & `edxval-2.4.0/edxval/config/waffle.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/exceptions.py` & `edxval-2.4.0/edxval/exceptions.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/migrations/0001_squashed_0016_add_transcript_credentials_model.py` & `edxval-2.4.0/edxval/migrations/0001_squashed_0016_add_transcript_credentials_model.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/models.py` & `edxval-2.4.0/edxval/models.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/serializers.py` & `edxval-2.4.0/edxval/serializers.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/tests/__init__.py` & `edxval-2.4.0/edxval/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/tests/constants.py` & `edxval-2.4.0/edxval/tests/constants.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/tests/test_admin.py` & `edxval-2.4.0/edxval/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/tests/test_api.py` & `edxval-2.4.0/edxval/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/tests/test_models.py` & `edxval-2.4.0/edxval/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/tests/test_serializers.py` & `edxval-2.4.0/edxval/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/tests/test_transcript_utils.py` & `edxval-2.4.0/edxval/tests/test_transcript_utils.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/tests/test_utils.py` & `edxval-2.4.0/edxval/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/tests/test_views.py` & `edxval-2.4.0/edxval/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/transcript_utils.py` & `edxval-2.4.0/edxval/transcript_utils.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/urls.py` & `edxval-2.4.0/edxval/urls.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/utils.py` & `edxval-2.4.0/edxval/utils.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/views.py` & `edxval-2.4.0/edxval/views.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval/wsgi.py` & `edxval-2.4.0/edxval/wsgi.py`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/edxval.egg-info/PKG-INFO` & `edxval-2.4.0/edxval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edxval
-Version: 2.3.0
+Version: 2.4.0
 Summary: edx-val
 Home-page: http://github.com/openedx/edx-val
 Author: edX
 License: AGPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `edxval-2.3.0/edxval.egg-info/SOURCES.txt` & `edxval-2.4.0/edxval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/setup.cfg` & `edxval-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `edxval-2.3.0/setup.py` & `edxval-2.4.0/setup.py`

 * *Files identical despite different names*

