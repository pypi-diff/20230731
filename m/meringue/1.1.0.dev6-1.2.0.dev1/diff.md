# Comparing `tmp/meringue-1.1.0.dev6.tar.gz` & `tmp/meringue-1.2.0.dev1.tar.gz`

## Comparing `meringue-1.1.0.dev6.tar` & `meringue-1.2.0.dev1.tar`

### file list

```diff
@@ -1,33 +1,47 @@
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/apps.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/handlers.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/routers.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/docs/__init__.py
--rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/docs/patchers.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/api/docs/views.py
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/conf/__init__.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/conf/default_settings.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/apps.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/options.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/query.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/translation.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/upload_handlers.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/views.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/templatetags/__init__.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/templatetags/meringue_base.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/utils/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/utils/crypt.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/utils/datetime.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/meringue/core/utils/frontend.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/AUTHORS
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/LICENSE
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/README.md
--rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/pyproject.toml
--rw-r--r--   0        0        0     8924 2020-02-02 00:00:00.000000 meringue-1.1.0.dev6/PKG-INFO
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/apps.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/handlers.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/routers.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/docs/__init__.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/docs/patchers.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/api/docs/views.py
+-rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/conf/__init__.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/conf/default_settings.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/apps.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/options.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/query.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/translation.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/upload_handlers.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/views.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/templatetags/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/templatetags/meringue_base.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/utils/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/utils/crypt.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/utils/datetime.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/core/utils/frontend.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/actions.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/apps.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/constants.py
+-rw-r--r--   0        0        0     5092 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/drf_fields.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/exceptions.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/generators.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/images.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/properties.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/shortcuts.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/storage.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/templatetags/__init__.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/meringue/thumbnail/templatetags/m_thumbnails.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/AUTHORS
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/LICENSE
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/README.md
+-rw-r--r--   0        0        0     8704 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     7910 2020-02-02 00:00:00.000000 meringue-1.2.0.dev1/PKG-INFO
```

### Comparing `meringue-1.1.0.dev6/meringue/api/handlers.py` & `meringue-1.2.0.dev1/meringue/api/handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev6/meringue/api/routers.py` & `meringue-1.2.0.dev1/meringue/api/routers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev6/meringue/api/utils.py` & `meringue-1.2.0.dev1/meringue/api/utils.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev6/meringue/api/docs/patchers.py` & `meringue-1.2.0.dev1/meringue/api/docs/patchers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev6/meringue/api/docs/views.py` & `meringue-1.2.0.dev1/meringue/api/docs/views.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev6/meringue/core/models.py` & `meringue-1.2.0.dev1/meringue/core/models.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev6/meringue/core/query.py` & `meringue-1.2.0.dev1/meringue/core/query.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev6/meringue/core/translation.py` & `meringue-1.2.0.dev1/meringue/core/translation.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev6/meringue/core/upload_handlers.py` & `meringue-1.2.0.dev1/meringue/core/upload_handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev6/meringue/core/locale/en/LC_MESSAGES/django.po` & `meringue-1.2.0.dev1/meringue/core/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev6/meringue/core/locale/ru/LC_MESSAGES/django.po` & `meringue-1.2.0.dev1/meringue/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev6/meringue/core/templatetags/meringue_base.py` & `meringue-1.2.0.dev1/meringue/core/templatetags/meringue_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 
 
 @register.simple_tag
 def cop_year() -> str:
     """
     A tag that displays the year or range of years for the copyright string in `YYYY-YYYY` format.
 
-    For the tag to work, you must fill in the `COP_YEAR` parameter in the settings.
-
     Examples:
         ```jinja
         <p>Copyright © {% cop_year %} My company</p>
         ```
 
     Raises:
         Exception: To use the `cop_year` tag, you must fill in the `COP_YEAR` parameter in the
```

### Comparing `meringue-1.1.0.dev6/meringue/core/utils/crypt.py` & `meringue-1.2.0.dev1/meringue/core/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev6/meringue/core/utils/datetime.py` & `meringue-1.2.0.dev1/meringue/core/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev6/meringue/core/utils/frontend.py` & `meringue-1.2.0.dev1/meringue/core/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev6/LICENSE` & `meringue-1.2.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev6/README.md` & `meringue-1.2.0.dev1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -63,29 +63,24 @@
 However, if someone decides to use this functionality in their project, and even more so to add functionality or change the implementation to a more correct, beautiful or understandable one, I will only be happy, do not worry and feel free to write to me by [mail](mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue).
 
 
 ## Roadmap
 
 Adding new functionality. Can change.
 
-* [x] Universal manager worked with all abstract models.
-* [x] Tests of all functionality.
-* [x] Methods for encrypting and decrypting text content (To create various secrets, such as a link to change your password or activate your profile).
-* [x] Functionality for obtaining absolute links to resources presented on the front, located on another domain (When working through api) (utils methods, template tags and filters).
 * [ ] [drf](https://www.django-rest-framework.org/) serializer serializer for automatic form generation on the front when working through rest api. (An npm package on [vuejs](https://vuejs.org/) will also be developed generating form based on response from api).
-* [x] Extended [drf router](https://www.django-rest-framework.org/api-guide/routers/) that allows you to add resources like `/profile` returning the profile data of an authorized user without his id.
 * [ ] Authorization backend for authorization by a pair of email and password.
-* [x] Helpers to extend documentation generated by [drf-spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to easily add links to different deployed environments (production, test, local, etc.) or let's say for more digestible tags instead of initially generated ones
-* [x] drf-spectacular view with patching documentation.
 * [ ] Functionality for working with images.
-	* [ ] Image editor like easy_thumbnails.
-	* [ ] A field for the drf serializer that returns a set of images (for example, a standard image and a double-sized image for a retina screen), as well as in different formats (for example, in the original format and in webp).
+	* [x] Image editor like easy_thumbnails.
+	* [x] A field for the drf serializer that returns a set of images (for example, a standard image and a double-sized image for a retina screen), as well as in different formats (for example, in the original format and in webp).
+	* [ ] Job chain presets
+	* [ ] Tests
+	* [ ] Docs
 * [ ] Functionality similar to that described in the previous paragraph only for video.
 * [ ] Functionality for loading private files available through [nginx internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal).
-* [x] Exception handler for drf that returns an error code in addition to the error text.
 
 
 ## Contributing
 
 - [x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and [here](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to resolve the versioning
 - [x] Linter with a [Ruff](https://github.com/charliermarsh/ruff)
 - [x] Formatter with a [Black](https://github.com/psf/black)
```

#### html2text {}

```diff
@@ -11,44 +11,31 @@
 also organize the documentation so that colleagues can understand how and what
 works. However, if someone decides to use this functionality in their project,
 and even more so to add functionality or change the implementation to a more
 correct, beautiful or understandable one, I will only be happy, do not worry
 and feel free to write to me by [mail](mailto:dd@manin.space), create an
 [issue](https://github.com/dd/Meringue/issues) or [pull request](https://
 github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue). ##
-Roadmap Adding new functionality. Can change. * [x] Universal manager worked
-with all abstract models. * [x] Tests of all functionality. * [x] Methods for
-encrypting and decrypting text content (To create various secrets, such as a
-link to change your password or activate your profile). * [x] Functionality for
-obtaining absolute links to resources presented on the front, located on
-another domain (When working through api) (utils methods, template tags and
-filters). * [ ] [drf](https://www.django-rest-framework.org/) serializer
-serializer for automatic form generation on the front when working through rest
-api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
-generating form based on response from api). * [x] Extended [drf router](https:
-//www.django-rest-framework.org/api-guide/routers/) that allows you to add
-resources like `/profile` returning the profile data of an authorized user
-without his id. * [ ] Authorization backend for authorization by a pair of
-email and password. * [x] Helpers to extend documentation generated by [drf-
-spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to
-easily add links to different deployed environments (production, test, local,
-etc.) or let's say for more digestible tags instead of initially generated ones
-* [x] drf-spectacular view with patching documentation. * [ ] Functionality for
-working with images. * [ ] Image editor like easy_thumbnails. * [ ] A field for
-the drf serializer that returns a set of images (for example, a standard image
-and a double-sized image for a retina screen), as well as in different formats
-(for example, in the original format and in webp). * [ ] Functionality similar
-to that described in the previous paragraph only for video. * [ ] Functionality
-for loading private files available through [nginx internal](http://nginx.org/
-en/docs/http/ngx_http_core_module.html#internal). * [x] Exception handler for
-drf that returns an error code in addition to the error text. ## Contributing -
-[x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and
-[here](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-
-workflow)) to resolve the versioning - [x] Linter with a [Ruff](https://
-github.com/charliermarsh/ruff) - [x] Formatter with a [Black](https://
+Roadmap Adding new functionality. Can change. * [ ] [drf](https://www.django-
+rest-framework.org/) serializer serializer for automatic form generation on the
+front when working through rest api. (An npm package on [vuejs](https://
+vuejs.org/) will also be developed generating form based on response from api).
+* [ ] Authorization backend for authorization by a pair of email and password.
+* [ ] Functionality for working with images. * [x] Image editor like
+easy_thumbnails. * [x] A field for the drf serializer that returns a set of
+images (for example, a standard image and a double-sized image for a retina
+screen), as well as in different formats (for example, in the original format
+and in webp). * [ ] Job chain presets * [ ] Tests * [ ] Docs * [ ]
+Functionality similar to that described in the previous paragraph only for
+video. * [ ] Functionality for loading private files available through [nginx
+internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal). ##
+Contributing - [x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-
+flow/) and [here](https://www.atlassian.com/git/tutorials/comparing-workflows/
+gitflow-workflow)) to resolve the versioning - [x] Linter with a [Ruff](https:/
+/github.com/charliermarsh/ruff) - [x] Formatter with a [Black](https://
 github.com/psf/black) - [x] Lint commit with [Gitlint](https://
 jorisroovers.com/gitlint/) and [Conventional Commits](https://
 www.conventionalcommits.org/) - [x] Documentation with [mkdocs](https://
 www.mkdocs.org/) and [mkdocs-material](https://squidfunk.github.io/mkdocs-
 material/) - [x] Testing local with [hatch](https://hatch.pypa.io/1.7/meta/faq/
 #environments) - [x] Testing in CI/CD on push - [ ] Add [mypy](https://mypy-
 lang.org/) ???
```

### Comparing `meringue-1.1.0.dev6/pyproject.toml` & `meringue-1.2.0.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,25 @@
 
 [tool.hatch.envs.default]
 description = "Dev environment"
 python = "3.11"
 dependencies = [
 	"pre-commit==3.3.3",
 	"ipython==8.14.0",
+	"django==4.2",
+	"pytz==2023.3",
+	"django-modeltranslation==0.18.11",
 	"pycryptodome==3.18.0",
 	"djangorestframework==3.14.0",
 	"drf-spectacular==0.26.4",
+	"Pillow==10.0.0",
 ]
+[tool.hatch.envs.default.env-vars]
+DJANGO_SETTINGS_MODULE = 'test_project.settings'
+PYTHONPATH  = '.'
 [tool.hatch.envs.default.scripts]
 precommit_install = "pre-commit install {args}"
 precommit_uninstall = "pre-commit uninstall {args}"
 init = [
 	"git config --local gitflow.branch.master \"master\"",
 	"git config --local gitflow.branch.develop \"dev\"",
 	"git config --local gitflow.prefix.feature \"feature/\"",
@@ -190,22 +197,22 @@
 djangorestframework = ["3.14.0"]
 
 [tool.hatch.envs.docs]
 description = "Docs environment"
 detached = true
 python = "3.11"
 dependencies = [
-	"mkdocs[i18n]==1.4.3",
+	"mkdocs[i18n]==1.5.1",
 	"mkdocs-literate-nav==0.6.0",
-	"mkdocs-material==9.1.19",
+	"mkdocs-material==9.1.21",
 	"mkdocs-git-revision-date-localized-plugin==1.2.0",
 	"mkdocs-git-authors-plugin==0.7.2",
 	"mkdocstrings[python]==0.22.0",
 	"black==23.7.0",
-	"mkdocs-minify-plugin==0.6.4",
+	"mkdocs-minify-plugin==0.7.0",
 	"mkdocs-gen-files==0.5.0",
 	"Pygments==2.15.1",
 	"mike==1.1.2",
 	"linkchecker==10.2.1",
 ]
 [tool.hatch.envs.docs.env-vars]
 MERINGUE_MKDOCS_ENABLE_MINIFY = 'false'
```

### Comparing `meringue-1.1.0.dev6/PKG-INFO` & `meringue-1.2.0.dev1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meringue
-Version: 1.1.0.dev6
+Version: 1.2.0.dev1
 Summary: A set of various functionality for a Django based web application.
 Project-URL: Homepage, https://github.com/dd/Meringue
 Project-URL: Documentation, https://dd.github.io/Meringue/
 Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues
 Author-email: Dmitry Dobrynin <dd@manin.space>
@@ -120,29 +120,24 @@
 However, if someone decides to use this functionality in their project, and even more so to add functionality or change the implementation to a more correct, beautiful or understandable one, I will only be happy, do not worry and feel free to write to me by [mail](mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue).
 
 
 ## Roadmap
 
 Adding new functionality. Can change.
 
-* [x] Universal manager worked with all abstract models.
-* [x] Tests of all functionality.
-* [x] Methods for encrypting and decrypting text content (To create various secrets, such as a link to change your password or activate your profile).
-* [x] Functionality for obtaining absolute links to resources presented on the front, located on another domain (When working through api) (utils methods, template tags and filters).
 * [ ] [drf](https://www.django-rest-framework.org/) serializer serializer for automatic form generation on the front when working through rest api. (An npm package on [vuejs](https://vuejs.org/) will also be developed generating form based on response from api).
-* [x] Extended [drf router](https://www.django-rest-framework.org/api-guide/routers/) that allows you to add resources like `/profile` returning the profile data of an authorized user without his id.
 * [ ] Authorization backend for authorization by a pair of email and password.
-* [x] Helpers to extend documentation generated by [drf-spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to easily add links to different deployed environments (production, test, local, etc.) or let's say for more digestible tags instead of initially generated ones
-* [x] drf-spectacular view with patching documentation.
 * [ ] Functionality for working with images.
-	* [ ] Image editor like easy_thumbnails.
-	* [ ] A field for the drf serializer that returns a set of images (for example, a standard image and a double-sized image for a retina screen), as well as in different formats (for example, in the original format and in webp).
+	* [x] Image editor like easy_thumbnails.
+	* [x] A field for the drf serializer that returns a set of images (for example, a standard image and a double-sized image for a retina screen), as well as in different formats (for example, in the original format and in webp).
+	* [ ] Job chain presets
+	* [ ] Tests
+	* [ ] Docs
 * [ ] Functionality similar to that described in the previous paragraph only for video.
 * [ ] Functionality for loading private files available through [nginx internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal).
-* [x] Exception handler for drf that returns an error code in addition to the error text.
 
 
 ## Contributing
 
 - [x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and [here](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to resolve the versioning
 - [x] Linter with a [Ruff](https://github.com/charliermarsh/ruff)
 - [x] Formatter with a [Black](https://github.com/psf/black)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: meringue Version: 1.1.0.dev6 Summary: A set of
+Metadata-Version: 2.1 Name: meringue Version: 1.2.0.dev1 Summary: A set of
 various functionality for a Django based web application. Project-URL:
 Homepage, https://github.com/dd/Meringue Project-URL: Documentation, https://
 dd.github.io/Meringue/ Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues Author-email:
 Dmitry Dobrynin
 manin.space> License-Expression: LGPL-3.0 License-File: AUTHORS License-File:
@@ -45,44 +45,31 @@
 also organize the documentation so that colleagues can understand how and what
 works. However, if someone decides to use this functionality in their project,
 and even more so to add functionality or change the implementation to a more
 correct, beautiful or understandable one, I will only be happy, do not worry
 and feel free to write to me by [mail](mailto:dd@manin.space), create an
 [issue](https://github.com/dd/Meringue/issues) or [pull request](https://
 github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue). ##
-Roadmap Adding new functionality. Can change. * [x] Universal manager worked
-with all abstract models. * [x] Tests of all functionality. * [x] Methods for
-encrypting and decrypting text content (To create various secrets, such as a
-link to change your password or activate your profile). * [x] Functionality for
-obtaining absolute links to resources presented on the front, located on
-another domain (When working through api) (utils methods, template tags and
-filters). * [ ] [drf](https://www.django-rest-framework.org/) serializer
-serializer for automatic form generation on the front when working through rest
-api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
-generating form based on response from api). * [x] Extended [drf router](https:
-//www.django-rest-framework.org/api-guide/routers/) that allows you to add
-resources like `/profile` returning the profile data of an authorized user
-without his id. * [ ] Authorization backend for authorization by a pair of
-email and password. * [x] Helpers to extend documentation generated by [drf-
-spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to
-easily add links to different deployed environments (production, test, local,
-etc.) or let's say for more digestible tags instead of initially generated ones
-* [x] drf-spectacular view with patching documentation. * [ ] Functionality for
-working with images. * [ ] Image editor like easy_thumbnails. * [ ] A field for
-the drf serializer that returns a set of images (for example, a standard image
-and a double-sized image for a retina screen), as well as in different formats
-(for example, in the original format and in webp). * [ ] Functionality similar
-to that described in the previous paragraph only for video. * [ ] Functionality
-for loading private files available through [nginx internal](http://nginx.org/
-en/docs/http/ngx_http_core_module.html#internal). * [x] Exception handler for
-drf that returns an error code in addition to the error text. ## Contributing -
-[x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and
-[here](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-
-workflow)) to resolve the versioning - [x] Linter with a [Ruff](https://
-github.com/charliermarsh/ruff) - [x] Formatter with a [Black](https://
+Roadmap Adding new functionality. Can change. * [ ] [drf](https://www.django-
+rest-framework.org/) serializer serializer for automatic form generation on the
+front when working through rest api. (An npm package on [vuejs](https://
+vuejs.org/) will also be developed generating form based on response from api).
+* [ ] Authorization backend for authorization by a pair of email and password.
+* [ ] Functionality for working with images. * [x] Image editor like
+easy_thumbnails. * [x] A field for the drf serializer that returns a set of
+images (for example, a standard image and a double-sized image for a retina
+screen), as well as in different formats (for example, in the original format
+and in webp). * [ ] Job chain presets * [ ] Tests * [ ] Docs * [ ]
+Functionality similar to that described in the previous paragraph only for
+video. * [ ] Functionality for loading private files available through [nginx
+internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal). ##
+Contributing - [x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-
+flow/) and [here](https://www.atlassian.com/git/tutorials/comparing-workflows/
+gitflow-workflow)) to resolve the versioning - [x] Linter with a [Ruff](https:/
+/github.com/charliermarsh/ruff) - [x] Formatter with a [Black](https://
 github.com/psf/black) - [x] Lint commit with [Gitlint](https://
 jorisroovers.com/gitlint/) and [Conventional Commits](https://
 www.conventionalcommits.org/) - [x] Documentation with [mkdocs](https://
 www.mkdocs.org/) and [mkdocs-material](https://squidfunk.github.io/mkdocs-
 material/) - [x] Testing local with [hatch](https://hatch.pypa.io/1.7/meta/faq/
 #environments) - [x] Testing in CI/CD on push - [ ] Add [mypy](https://mypy-
 lang.org/) ???
```

