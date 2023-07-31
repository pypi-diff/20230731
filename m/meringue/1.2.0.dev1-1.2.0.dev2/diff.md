# Comparing `tmp/meringue-1.2.0.dev1.tar.gz` & `tmp/meringue-1.2.0.dev2.tar.gz`

## Comparing `meringue-1.2.0.dev1.tar` & `meringue-1.2.0.dev2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/apps.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/handlers.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/routers.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/docs/__init__.py
--rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/docs/patchers.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/docs/views.py
--rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/conf/__init__.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/conf/default_settings.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/apps.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/options.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/query.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/translation.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/upload_handlers.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/views.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/templatetags/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/templatetags/meringue_base.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/utils/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/utils/crypt.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/utils/datetime.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/utils/frontend.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/actions.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/apps.py
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/constants.py
--rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/drf_fields.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/exceptions.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/generators.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/images.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/properties.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/shortcuts.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/storage.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/templatetags/__init__.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/templatetags/m_thumbnails.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/AUTHORS
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/LICENSE
--rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/README.md
--rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     7910 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/apps.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/handlers.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/routers.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/docs/__init__.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/docs/patchers.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/api/docs/views.py
+-rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/conf/__init__.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/conf/default_settings.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/apps.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/options.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/query.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/translation.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/upload_handlers.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/views.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/templatetags/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/templatetags/meringue_base.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/utils/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/utils/crypt.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/utils/datetime.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/core/utils/frontend.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/actions.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/apps.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/constants.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/drf_fields.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/exceptions.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/generators.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/images.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/properties.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/shortcuts.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/storage.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/templatetags/__init__.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/meringue/thumbnail/templatetags/m_thumbnails.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/AUTHORS
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/LICENSE
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/README.md
+-rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     7910 2020-02-02 00:00:00.000000 meringue-1.2.0.dev2/PKG-INFO
```

### Comparing `meringue-1.2.0.dev1/meringue/api/handlers.py` & `meringue-1.2.0.dev2/meringue/api/handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/api/routers.py` & `meringue-1.2.0.dev2/meringue/api/routers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/api/utils.py` & `meringue-1.2.0.dev2/meringue/api/utils.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/api/docs/patchers.py` & `meringue-1.2.0.dev2/meringue/api/docs/patchers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/api/docs/views.py` & `meringue-1.2.0.dev2/meringue/api/docs/views.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/conf/__init__.py` & `meringue-1.2.0.dev2/meringue/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/conf/default_settings.py` & `meringue-1.2.0.dev2/meringue/conf/default_settings.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/core/models.py` & `meringue-1.2.0.dev2/meringue/core/models.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/core/query.py` & `meringue-1.2.0.dev2/meringue/core/query.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/core/translation.py` & `meringue-1.2.0.dev2/meringue/core/translation.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/core/upload_handlers.py` & `meringue-1.2.0.dev2/meringue/core/upload_handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/core/locale/en/LC_MESSAGES/django.po` & `meringue-1.2.0.dev2/meringue/core/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/core/locale/ru/LC_MESSAGES/django.po` & `meringue-1.2.0.dev2/meringue/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/core/templatetags/meringue_base.py` & `meringue-1.2.0.dev2/meringue/core/templatetags/meringue_base.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/core/utils/crypt.py` & `meringue-1.2.0.dev2/meringue/core/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/core/utils/datetime.py` & `meringue-1.2.0.dev2/meringue/core/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/core/utils/frontend.py` & `meringue-1.2.0.dev2/meringue/core/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/thumbnail/actions.py` & `meringue-1.2.0.dev2/meringue/thumbnail/actions.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/thumbnail/constants.py` & `meringue-1.2.0.dev2/meringue/thumbnail/constants.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/thumbnail/drf_fields.py` & `meringue-1.2.0.dev2/meringue/thumbnail/drf_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import os
 from pathlib import PurePath
 
 from rest_framework.fields import ImageField
 
 from meringue.thumbnail.constants import FORMATS_BY_EXTENSIONS
-from meringue.thumbnail.generator import DefaultThumbnailer
+from meringue.thumbnail.generators import DefaultThumbnailer
 from meringue.thumbnail.shortcuts import _dummyimage
 
 
 logger = logging.getLogger("meringue.thumbnail")
 
 
 def get_format_from_path(path):
@@ -35,15 +35,15 @@
 
         else:
             self.job_chain = []
 
         super().__init__(**kwargs)
 
 
-class ImageOptimizedField(BaseImageField):
+class MImageField(BaseImageField):
     """
     Optimize image to represent them
     """
 
     def to_representation(self, value):
         """
         TODO:
@@ -61,15 +61,15 @@
         else:
             logger.error(f"File `{value.path}` not found")
             result = _dummyimage([])
 
         return result
 
 
-class ImageSetDimensionsField(ImageField):
+class MImageSetField(ImageField):
     """
     Image field - make multiple files in different formats.
 
     Can set size (eg '100x100'), job_chain (arrays of jobs by dimensions) or nothing to optimize
     images only
     """
```

### Comparing `meringue-1.2.0.dev1/meringue/thumbnail/exceptions.py` & `meringue-1.2.0.dev2/meringue/thumbnail/exceptions.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/thumbnail/generators.py` & `meringue-1.2.0.dev2/meringue/thumbnail/generators.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/thumbnail/images.py` & `meringue-1.2.0.dev2/meringue/thumbnail/images.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/thumbnail/properties.py` & `meringue-1.2.0.dev2/meringue/thumbnail/properties.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/thumbnail/shortcuts.py` & `meringue-1.2.0.dev2/meringue/thumbnail/shortcuts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import re
 from pathlib import Path
 
 from django.conf import settings
 
 from meringue.conf import m_settings
-from meringue.thumbnail.generator import DefaultThumbnailer
+from meringue.thumbnail.generators import DefaultThumbnailer
 from meringue.thumbnail.types import JobChainType
 
 
 logger = logging.getLogger("meringue.thumbnail")
 
 
 def _dummyimage(job_chain: str) -> str:
@@ -61,15 +61,15 @@
         format: Output image format.
         **kwargs: Output image save extra params.
 
     Returns:
         Thumbnail url.
     """
 
-    # if not file_path.exists():
-    #     msg = f"File `{file_path}` not found."
-    #     logger.error(msg)
-    #     return _dummyimage(job_chain)
+    if not file_path.exists():
+        msg = f"File `{file_path}` not found."
+        logger.error(msg)
+        return _dummyimage(job_chain)
 
     thumbnailer = DefaultThumbnailer(file_path, job_chain=job_chain)
     thumbnail_image = thumbnailer.get_thumbnail(out_format, **kwargs)
     return thumbnail_image.url
```

### Comparing `meringue-1.2.0.dev1/meringue/thumbnail/storage.py` & `meringue-1.2.0.dev2/meringue/thumbnail/storage.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/meringue/thumbnail/templatetags/m_thumbnails.py` & `meringue-1.2.0.dev2/meringue/thumbnail/templatetags/m_thumbnails.py`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/LICENSE` & `meringue-1.2.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/README.md` & `meringue-1.2.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/pyproject.toml` & `meringue-1.2.0.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meringue-1.2.0.dev1/PKG-INFO` & `meringue-1.2.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meringue
-Version: 1.2.0.dev1
+Version: 1.2.0.dev2
 Summary: A set of various functionality for a Django based web application.
 Project-URL: Homepage, https://github.com/dd/Meringue
 Project-URL: Documentation, https://dd.github.io/Meringue/
 Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues
 Author-email: Dmitry Dobrynin <dd@manin.space>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: meringue Version: 1.2.0.dev1 Summary: A set of
+Metadata-Version: 2.1 Name: meringue Version: 1.2.0.dev2 Summary: A set of
 various functionality for a Django based web application. Project-URL:
 Homepage, https://github.com/dd/Meringue Project-URL: Documentation, https://
 dd.github.io/Meringue/ Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues Author-email:
 Dmitry Dobrynin
 manin.space> License-Expression: LGPL-3.0 License-File: AUTHORS License-File:
```

