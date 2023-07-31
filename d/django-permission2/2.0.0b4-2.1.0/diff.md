# Comparing `tmp/django-permission2-2.0.0b4.tar.gz` & `tmp/django_permission2-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-permission2-2.0.0b4.tar", max compression
+gzip compressed data, was "django_permission2-2.1.0.tar", max compression
```

## Comparing `django-permission2-2.0.0b4.tar` & `django_permission2-2.1.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0     1100 2022-08-12 09:02:31.728382 django-permission2-2.0.0b4/LICENSE
--rw-r--r--   0        0        0      695 2022-08-12 16:25:39.627690 django-permission2-2.0.0b4/pyproject.toml
--rw-r--r--   0        0        0     2576 2022-08-12 09:04:21.978170 django-permission2-2.0.0b4/src/permission/__init__.py
--rw-r--r--   0        0        0      340 2022-08-12 08:41:33.519139 django-permission2-2.0.0b4/src/permission/apps.py
--rw-r--r--   0        0        0     4138 2022-08-12 08:41:33.519211 django-permission2-2.0.0b4/src/permission/backends.py
--rw-r--r--   0        0        0     2055 2022-08-12 09:46:01.282694 django-permission2-2.0.0b4/src/permission/compat.py
--rw-r--r--   0        0        0     1742 2022-08-12 09:02:31.709815 django-permission2-2.0.0b4/src/permission/conf.py
--rw-r--r--   0        0        0       74 2022-08-12 08:41:33.519430 django-permission2-2.0.0b4/src/permission/decorators/__init__.py
--rw-r--r--   0        0        0     3773 2022-08-12 09:34:41.154162 django-permission2-2.0.0b4/src/permission/decorators/classbase.py
--rw-r--r--   0        0        0     5904 2022-08-12 09:31:59.833790 django-permission2-2.0.0b4/src/permission/decorators/functionbase.py
--rw-r--r--   0        0        0     3010 2022-08-12 09:33:41.802239 django-permission2-2.0.0b4/src/permission/decorators/methodbase.py
--rw-r--r--   0        0        0     2598 2022-08-12 08:41:33.519728 django-permission2-2.0.0b4/src/permission/decorators/permission_required.py
--rw-r--r--   0        0        0      990 2022-08-12 08:41:33.519819 django-permission2-2.0.0b4/src/permission/decorators/utils.py
--rw-r--r--   0        0        0     8352 2022-08-12 08:41:33.519906 django-permission2-2.0.0b4/src/permission/handlers.py
--rw-r--r--   0        0        0      409 2022-08-12 08:41:33.519996 django-permission2-2.0.0b4/src/permission/logics/__init__.py
--rw-r--r--   0        0        0     5358 2022-08-12 08:41:33.520084 django-permission2-2.0.0b4/src/permission/logics/author.py
--rw-r--r--   0        0        0     1554 2022-08-12 08:41:33.520151 django-permission2-2.0.0b4/src/permission/logics/base.py
--rw-r--r--   0        0        0     5642 2022-08-12 08:41:33.520238 django-permission2-2.0.0b4/src/permission/logics/collaborators.py
--rw-r--r--   0        0        0     5588 2022-08-12 08:41:33.520318 django-permission2-2.0.0b4/src/permission/logics/groupin.py
--rw-r--r--   0        0        0     4588 2022-08-12 08:41:33.520397 django-permission2-2.0.0b4/src/permission/logics/oneself.py
--rw-r--r--   0        0        0     5221 2022-08-12 08:41:33.520479 django-permission2-2.0.0b4/src/permission/logics/staff.py
--rw-r--r--   0        0        0        0 2022-08-12 08:41:33.520505 django-permission2-2.0.0b4/src/permission/models.py
--rw-r--r--   0        0        0        0 2022-08-12 08:41:33.520576 django-permission2-2.0.0b4/src/permission/templatetags/__init__.py
--rw-r--r--   0        0        0     4183 2022-08-12 08:41:33.520676 django-permission2-2.0.0b4/src/permission/templatetags/permissionif.py
--rw-r--r--   0        0        0        0 2022-08-12 08:41:33.520741 django-permission2-2.0.0b4/src/permission/tests/__init__.py
--rw-r--r--   0        0        0      903 2022-08-12 09:29:42.810235 django-permission2-2.0.0b4/src/permission/tests/compat.py
--rw-r--r--   0        0        0     1535 2022-08-12 09:28:24.057861 django-permission2-2.0.0b4/src/permission/tests/models.py
--rw-r--r--   0        0        0     7651 2022-08-12 08:41:33.520954 django-permission2-2.0.0b4/src/permission/tests/test_backends.py
--rw-r--r--   0        0        0        0 2022-08-12 08:41:33.521014 django-permission2-2.0.0b4/src/permission/tests/test_decorators/__init__.py
--rw-r--r--   0        0        0     7369 2022-08-12 08:41:33.521092 django-permission2-2.0.0b4/src/permission/tests/test_decorators/test_classbase.py
--rw-r--r--   0        0        0     7063 2022-08-12 08:41:33.521178 django-permission2-2.0.0b4/src/permission/tests/test_decorators/test_functionbase.py
--rw-r--r--   0        0        0     7349 2022-08-12 08:41:33.521240 django-permission2-2.0.0b4/src/permission/tests/test_decorators/test_methodbase.py
--rw-r--r--   0        0        0     3567 2022-08-12 08:41:33.521312 django-permission2-2.0.0b4/src/permission/tests/test_decorators/test_permission_required.py
--rw-r--r--   0        0        0     2631 2022-08-12 08:41:33.521387 django-permission2-2.0.0b4/src/permission/tests/test_decorators/utils.py
--rw-r--r--   0        0        0    11108 2022-08-12 09:25:46.204484 django-permission2-2.0.0b4/src/permission/tests/test_handlers.py
--rw-r--r--   0        0        0        0 2022-08-12 08:41:33.521554 django-permission2-2.0.0b4/src/permission/tests/test_logics/__init__.py
--rw-r--r--   0        0        0    11051 2022-08-12 08:41:33.521904 django-permission2-2.0.0b4/src/permission/tests/test_logics/test_author.py
--rw-r--r--   0        0        0     2079 2022-08-12 08:41:33.521977 django-permission2-2.0.0b4/src/permission/tests/test_logics/test_base.py
--rw-r--r--   0        0        0    11426 2022-08-12 08:41:33.522057 django-permission2-2.0.0b4/src/permission/tests/test_logics/test_collaborators.py
--rw-r--r--   0        0        0    13817 2022-08-12 08:41:33.522142 django-permission2-2.0.0b4/src/permission/tests/test_logics/test_groupin.py
--rw-r--r--   0        0        0     9483 2022-08-12 08:41:33.522228 django-permission2-2.0.0b4/src/permission/tests/test_logics/test_oneself.py
--rw-r--r--   0        0        0     8794 2022-08-12 08:41:33.522304 django-permission2-2.0.0b4/src/permission/tests/test_logics/test_staff.py
--rw-r--r--   0        0        0        0 2022-08-12 08:41:33.522361 django-permission2-2.0.0b4/src/permission/tests/test_templatetags/__init__.py
--rw-r--r--   0        0        0    20669 2022-08-12 08:41:33.522479 django-permission2-2.0.0b4/src/permission/tests/test_templatetags/test_permissionif.py
--rw-r--r--   0        0        0        0 2022-08-12 08:41:33.522553 django-permission2-2.0.0b4/src/permission/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     4691 2022-08-12 11:22:31.277382 django-permission2-2.0.0b4/src/permission/tests/test_utils/test_field_lookup.py
--rw-r--r--   0        0        0     2991 2022-08-12 08:41:33.522695 django-permission2-2.0.0b4/src/permission/tests/test_utils/test_handlers.py
--rw-r--r--   0        0        0     4217 2022-08-12 08:41:33.522766 django-permission2-2.0.0b4/src/permission/tests/test_utils/test_logics.py
--rw-r--r--   0        0        0       53 2022-08-12 08:41:33.522817 django-permission2-2.0.0b4/src/permission/tests/test_utils/test_permissions.py
--rw-r--r--   0        0        0     1979 2022-08-12 08:41:33.522893 django-permission2-2.0.0b4/src/permission/tests/utils.py
--rw-r--r--   0        0        0        0 2022-08-12 08:41:33.522952 django-permission2-2.0.0b4/src/permission/utils/__init__.py
--rw-r--r--   0        0        0     2548 2022-08-12 09:46:43.988728 django-permission2-2.0.0b4/src/permission/utils/autodiscover.py
--rw-r--r--   0        0        0     1757 2022-08-12 11:02:23.383470 django-permission2-2.0.0b4/src/permission/utils/field_lookup.py
--rw-r--r--   0        0        0     3041 2022-08-12 08:41:33.523198 django-permission2-2.0.0b4/src/permission/utils/handlers.py
--rw-r--r--   0        0        0     3012 2022-08-12 08:41:33.523264 django-permission2-2.0.0b4/src/permission/utils/logics.py
--rw-r--r--   0        0        0     3903 2022-08-12 09:13:40.635638 django-permission2-2.0.0b4/src/permission/utils/permissions.py
--rw-r--r--   0        0        0     1131 2022-08-12 16:50:17.297871 django-permission2-2.0.0b4/setup.py
--rw-r--r--   0        0        0      765 2022-08-12 16:50:17.298042 django-permission2-2.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1100 2022-08-12 09:02:31.728382 django_permission2-2.1.0/LICENSE
+-rw-r--r--   0        0        0     7011 2023-07-19 21:34:24.847273 django_permission2-2.1.0/README.rst
+-rw-r--r--   0        0        0     2401 2023-07-31 13:51:40.472367 django_permission2-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2501 2023-07-19 21:34:24.831196 django_permission2-2.1.0/src/permission/__init__.py
+-rw-r--r--   0        0        0      342 2022-08-12 18:00:24.100692 django_permission2-2.1.0/src/permission/apps.py
+-rw-r--r--   0        0        0     4211 2022-08-12 18:00:25.556370 django_permission2-2.1.0/src/permission/backends.py
+-rw-r--r--   0        0        0     2019 2022-08-12 18:00:24.503799 django_permission2-2.1.0/src/permission/compat.py
+-rw-r--r--   0        0        0     1742 2022-08-12 18:00:25.560562 django_permission2-2.1.0/src/permission/conf.py
+-rw-r--r--   0        0        0       74 2022-08-12 08:41:33.519430 django_permission2-2.1.0/src/permission/decorators/__init__.py
+-rw-r--r--   0        0        0     3738 2022-11-30 11:48:28.326637 django_permission2-2.1.0/src/permission/decorators/classbase.py
+-rw-r--r--   0        0        0     5846 2022-08-12 18:00:25.560625 django_permission2-2.1.0/src/permission/decorators/functionbase.py
+-rw-r--r--   0        0        0     2977 2022-08-12 18:03:52.413709 django_permission2-2.1.0/src/permission/decorators/methodbase.py
+-rw-r--r--   0        0        0     2567 2022-08-12 18:03:52.075855 django_permission2-2.1.0/src/permission/decorators/permission_required.py
+-rw-r--r--   0        0        0      941 2022-08-12 18:03:52.415655 django_permission2-2.1.0/src/permission/decorators/utils.py
+-rw-r--r--   0        0        0     8270 2022-08-12 21:56:17.551320 django_permission2-2.1.0/src/permission/handlers.py
+-rw-r--r--   0        0        0      409 2022-08-12 18:00:25.573995 django_permission2-2.1.0/src/permission/logics/__init__.py
+-rw-r--r--   0        0        0     5214 2022-08-12 18:00:25.552492 django_permission2-2.1.0/src/permission/logics/author.py
+-rw-r--r--   0        0        0     1548 2022-08-12 18:00:24.326537 django_permission2-2.1.0/src/permission/logics/base.py
+-rw-r--r--   0        0        0     5498 2022-08-12 18:00:25.556300 django_permission2-2.1.0/src/permission/logics/collaborators.py
+-rw-r--r--   0        0        0     5408 2022-08-12 18:00:25.564843 django_permission2-2.1.0/src/permission/logics/groupin.py
+-rw-r--r--   0        0        0     4446 2022-08-12 18:00:25.540449 django_permission2-2.1.0/src/permission/logics/oneself.py
+-rw-r--r--   0        0        0     5051 2022-08-12 18:00:25.539720 django_permission2-2.1.0/src/permission/logics/staff.py
+-rw-r--r--   0        0        0        0 2022-08-12 08:41:33.520505 django_permission2-2.1.0/src/permission/models.py
+-rw-r--r--   0        0        0        0 2022-08-12 08:41:33.520576 django_permission2-2.1.0/src/permission/templatetags/__init__.py
+-rw-r--r--   0        0        0     4114 2022-08-12 18:00:25.562574 django_permission2-2.1.0/src/permission/templatetags/permissionif.py
+-rw-r--r--   0        0        0        0 2022-08-12 08:41:33.520741 django_permission2-2.1.0/src/permission/tests/__init__.py
+-rw-r--r--   0        0        0      909 2022-08-12 18:00:24.332549 django_permission2-2.1.0/src/permission/tests/compat.py
+-rw-r--r--   0        0        0     1642 2022-08-12 18:00:25.554514 django_permission2-2.1.0/src/permission/tests/models.py
+-rw-r--r--   0        0        0     8168 2022-08-12 18:00:25.557871 django_permission2-2.1.0/src/permission/tests/test_backends.py
+-rw-r--r--   0        0        0        0 2022-08-12 08:41:33.521014 django_permission2-2.1.0/src/permission/tests/test_decorators/__init__.py
+-rw-r--r--   0        0        0     6791 2022-08-12 18:03:52.666597 django_permission2-2.1.0/src/permission/tests/test_decorators/test_classbase.py
+-rw-r--r--   0        0        0     6791 2022-08-12 18:03:52.613407 django_permission2-2.1.0/src/permission/tests/test_decorators/test_functionbase.py
+-rw-r--r--   0        0        0     6854 2022-08-12 18:03:52.641671 django_permission2-2.1.0/src/permission/tests/test_decorators/test_methodbase.py
+-rw-r--r--   0        0        0     3531 2023-07-31 12:28:09.624036 django_permission2-2.1.0/src/permission/tests/test_decorators/test_permission_required.py
+-rw-r--r--   0        0        0     2600 2022-08-12 18:00:25.572206 django_permission2-2.1.0/src/permission/tests/test_decorators/utils.py
+-rw-r--r--   0        0        0    12138 2022-08-12 21:54:57.355495 django_permission2-2.1.0/src/permission/tests/test_handlers.py
+-rw-r--r--   0        0        0        0 2022-08-12 08:41:33.521554 django_permission2-2.1.0/src/permission/tests/test_logics/__init__.py
+-rw-r--r--   0        0        0    10853 2022-08-12 18:00:25.563879 django_permission2-2.1.0/src/permission/tests/test_logics/test_author.py
+-rw-r--r--   0        0        0     2046 2022-08-12 18:00:25.567869 django_permission2-2.1.0/src/permission/tests/test_logics/test_base.py
+-rw-r--r--   0        0        0    11228 2022-08-12 18:00:25.542633 django_permission2-2.1.0/src/permission/tests/test_logics/test_collaborators.py
+-rw-r--r--   0        0        0    13715 2022-08-12 18:00:25.568628 django_permission2-2.1.0/src/permission/tests/test_logics/test_groupin.py
+-rw-r--r--   0        0        0     9094 2022-08-12 18:00:25.576169 django_permission2-2.1.0/src/permission/tests/test_logics/test_oneself.py
+-rw-r--r--   0        0        0     8750 2022-08-12 18:00:25.569463 django_permission2-2.1.0/src/permission/tests/test_logics/test_staff.py
+-rw-r--r--   0        0        0        0 2022-08-12 08:41:33.522361 django_permission2-2.1.0/src/permission/tests/test_templatetags/__init__.py
+-rw-r--r--   0        0        0    20727 2023-07-31 12:28:09.624254 django_permission2-2.1.0/src/permission/tests/test_templatetags/test_permissionif.py
+-rw-r--r--   0        0        0        0 2022-08-12 08:41:33.522553 django_permission2-2.1.0/src/permission/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     4374 2022-08-12 18:00:25.553437 django_permission2-2.1.0/src/permission/tests/test_utils/test_field_lookup.py
+-rw-r--r--   0        0        0     2722 2022-08-12 18:00:25.555289 django_permission2-2.1.0/src/permission/tests/test_utils/test_handlers.py
+-rw-r--r--   0        0        0     4143 2022-08-12 18:00:25.563412 django_permission2-2.1.0/src/permission/tests/test_utils/test_logics.py
+-rw-r--r--   0        0        0       53 2022-08-12 08:41:33.522817 django_permission2-2.1.0/src/permission/tests/test_utils/test_permissions.py
+-rw-r--r--   0        0        0      491 2023-07-19 21:34:24.831461 django_permission2-2.1.0/src/permission/tests/test_version.py
+-rw-r--r--   0        0        0     1934 2022-08-12 18:00:25.558129 django_permission2-2.1.0/src/permission/tests/utils.py
+-rw-r--r--   0        0        0        0 2022-08-12 08:41:33.522952 django_permission2-2.1.0/src/permission/utils/__init__.py
+-rw-r--r--   0        0        0     2517 2022-08-12 18:00:25.559249 django_permission2-2.1.0/src/permission/utils/autodiscover.py
+-rw-r--r--   0        0        0     1758 2022-08-12 18:00:25.568930 django_permission2-2.1.0/src/permission/utils/field_lookup.py
+-rw-r--r--   0        0        0     3034 2022-08-12 18:05:47.059700 django_permission2-2.1.0/src/permission/utils/handlers.py
+-rw-r--r--   0        0        0     3026 2022-08-12 18:00:25.571822 django_permission2-2.1.0/src/permission/utils/logics.py
+-rw-r--r--   0        0        0     3873 2022-08-12 18:00:24.545351 django_permission2-2.1.0/src/permission/utils/permissions.py
+-rw-r--r--   0        0        0     8925 1970-01-01 00:00:00.000000 django_permission2-2.1.0/PKG-INFO
```

### Comparing `django-permission2-2.0.0b4/LICENSE` & `django_permission2-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-permission2-2.0.0b4/src/permission/__init__.py` & `django_permission2-2.1.0/src/permission/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,58 @@
-from app_version import get_versions
-__version__, VERSION = get_versions('django-permission2', allow_ambiguous=True)
+import importlib.metadata
 
-# load shortcut functions
-from permission.utils.logics import add_permission_logic
-from permission.utils.logics import remove_permission_logic
+__version__ = importlib.metadata.version("django-permission2")
 
-# autodiscover
-from permission.utils.autodiscover import autodiscover
+from django.core.exceptions import ImproperlyConfigured
 
 from permission.conf import settings
-from django.core.exceptions import ImproperlyConfigured
 
+# autodiscover
+from permission.utils.autodiscover import autodiscover
+
+# load shortcut functions
+from permission.utils.logics import add_permission_logic, remove_permission_logic
 
-if 'permission' in settings.INSTALLED_APPS:
+if "permission" in settings.INSTALLED_APPS:
     if settings.PERMISSION_CHECK_AUTHENTICATION_BACKENDS:
-        if ('permission.backends.PermissionBackend' not in
-                settings.AUTHENTICATION_BACKENDS):
+        if (
+            "permission.backends.PermissionBackend"
+            not in settings.AUTHENTICATION_BACKENDS
+        ):
             raise ImproperlyConfigured(
-                    '"permission.backends.PermissionBackend" is not found in '
-                    '`AUTHENTICATION_BACKENDS`.\n'
-                    'Users require to specify the backend manually to the '
-                    'option.\n'
-                    'Users can ignore this exception via setting `False` to '
-                    '`PERMISSION_CHECK_AUTHENTICATION_BACKENDS`.'
-                )
+                '"permission.backends.PermissionBackend" is not found in '
+                "`AUTHENTICATION_BACKENDS`.\n"
+                "Users require to specify the backend manually to the "
+                "option.\n"
+                "Users can ignore this exception via setting `False` to "
+                "`PERMISSION_CHECK_AUTHENTICATION_BACKENDS`."
+            )
     if settings.PERMISSION_REPLACE_BUILTIN_IF:
         from permission.compat import add_to_builtins
+
         if add_to_builtins:
-            add_to_builtins('permission.templatetags.permissionif')
+            add_to_builtins("permission.templatetags.permissionif")
         elif settings.PERMISSION_CHECK_TEMPLATES_OPTIONS_BUILTINS:
             # Check if settings.TEMPLATES[?]['OPTIONS']['builtins'] has
             # 'permission.templatetags.permissionif'
             def has_permissionif_in_builtins():
                 for template in settings.TEMPLATES:
-                    OPTIONS  = template.get('OPTIONS', {})
-                    builtins = OPTIONS.get('builtins', [])
+                    OPTIONS = template.get("OPTIONS", {})
+                    builtins = OPTIONS.get("builtins", [])
                     for builtin in builtins:
-                        if builtin == 'permission.templatetags.permissionif':
+                        if builtin == "permission.templatetags.permissionif":
                             return True
                 return False
+
             if not has_permissionif_in_builtins():
                 raise ImproperlyConfigured(
                     '"permission.templatetags.permissionif" is not found in '
-                    'none of `TEMPLATES[?][\'OPTIONS\'][\'builtins\']`.\n'
-                    'From Django 1.9, users require to specify the module '
-                    'to the option for loading a templatetag automatically '
-                    'or load the module manually.\n'
-                    'Users can ignore this exception via setting `False` to '
-                    '`PERMISSION_CHECK_TEMPLATES_OPTIONS_BUILTINS`.'
+                    "none of `TEMPLATES[?]['OPTIONS']['builtins']`.\n"
+                    "From Django 1.9, users require to specify the module "
+                    "to the option for loading a templatetag automatically "
+                    "or load the module manually.\n"
+                    "Users can ignore this exception via setting `False` to "
+                    "`PERMISSION_CHECK_TEMPLATES_OPTIONS_BUILTINS`."
                 )
 
 # Django Application
-default_app_config = 'permission.apps.PermissionConfig'
+default_app_config = "permission.apps.PermissionConfig"
```

### Comparing `django-permission2-2.0.0b4/src/permission/backends.py` & `django_permission2-2.1.0/src/permission/backends.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 """
 Logical permission backends module
 """
 from permission.conf import settings
 from permission.utils.handlers import registry
 from permission.utils.permissions import perm_to_permission
 
-
-__all__    = ('PermissionBackend',)
+__all__ = ("PermissionBackend",)
 
 
 class PermissionBackend(object):
     """
     A handler based permission backend
     """
+
     supports_object_permissions = True
     supports_anonymous_user = True
     supports_inactive_user = True
 
     # pylint:disable=unused-argument
     def authenticate(self, username, password):
         """
@@ -62,20 +62,23 @@
             try:
                 perm_to_permission(perm)
             except AttributeError:
                 # Django 1.2 internally use wrong permission string thus ignore
                 pass
 
         # get permission handlers fot this perm
-        cache_name = '_%s_cache' % perm
+        cache_name = "_%s_cache" % perm
         if hasattr(self, cache_name):
             handlers = getattr(self, cache_name)
         else:
-            handlers = [h for h in registry.get_handlers()
-                        if perm in h.get_supported_permissions()]
+            handlers = [
+                h
+                for h in registry.get_handlers()
+                if perm in h.get_supported_permissions()
+            ]
             setattr(self, cache_name, handlers)
         for handler in handlers:
             if handler.has_perm(user_obj, perm, obj=obj):
                 return True
         return False
 
     def has_module_perms(self, user_obj, app_label):
@@ -104,18 +107,21 @@
         ------
         django.core.exceptions.ObjectDoesNotExist
             If the specified string permission does not exist and
             ``PERMISSION_CHECK_PERMISSION_PRESENCE`` is ``True`` in ``settings``
             module.
         """
         # get permission handlers fot this perm
-        cache_name = '_%s_cache' % app_label
+        cache_name = "_%s_cache" % app_label
         if hasattr(self, cache_name):
             handlers = getattr(self, cache_name)
         else:
-            handlers = [h for h in registry.get_handlers()
-                        if app_label in h.get_supported_app_labels()]
+            handlers = [
+                h
+                for h in registry.get_handlers()
+                if app_label in h.get_supported_app_labels()
+            ]
             setattr(self, cache_name, handlers)
         for handler in handlers:
             if handler.has_module_perms(user_obj, app_label):
                 return True
         return False
```

### Comparing `django-permission2-2.0.0b4/src/permission/compat.py` & `django_permission2-2.1.0/src/permission/compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # coding=utf-8
 import django
+
 if django.VERSION >= (1, 9):
     add_to_builtins = None
 else:
     try:
         from django.template.base import add_to_builtins
     except ImportError:
         from django.template.loader import add_to_builtins
@@ -11,62 +12,71 @@
 try:
     # django.utils.importlib is removed from Django 1.9
     from importlib import import_module
 except ImportError:
     from django.utils.importlib import import_module
 
 if django.VERSION < (1, 10):
+
     def is_authenticated(user_obj):
         return user_obj.is_authenticated()
 
     def is_anonyomus(user_obj):
         return user_obj.is_anonymous()
+
 else:
+
     def is_authenticated(user_obj):
         return user_obj.is_authenticated
 
     def is_anonyomus(user_obj):
         return user_obj.is_anonymous
- 
+
+
 try:
     # Django 1.7 or over use the new application loading system
     from django.apps import apps
+
     get_model = apps.get_model
 except ImportError:
     from django.db.models.loading import get_model
 
 try:
     from django.utils.module_loading import import_string
 except ImportError:
     try:
         from django.utils.module_loading import import_by_path as import_string
     except ImportError:
+
         def import_string(dotted_path):
             try:
-                module_path, class_name = dotted_path.rsplit('.', 1)
+                module_path, class_name = dotted_path.rsplit(".", 1)
             except ValueError:
-                raise ImportError(
-                    "%s doesn't look like a module path" % dotted_path
-                )
+                raise ImportError("%s doesn't look like a module path" % dotted_path)
             module = import_module(module_path)
             try:
                 return getattr(module, class_name)
             except AttributeError:
                 raise ImportError(
-                    'Module "%s" does not define a "%s" attribute/class' % (
-                        module_path, class_name
-                    ))
+                    'Module "%s" does not define a "%s" attribute/class'
+                    % (module_path, class_name)
+                )
+
 
 try:
     # Python 3
     from urllib.parse import urlparse
 except ImportError:
     # Python 2
     from urlparse import urlparse
 
 import sys
+
 if sys.version_info >= (3, 0):
+
     def isstr(x):
         return isinstance(x, str)
+
 else:
+
     def isstr(x):
         return isinstance(x, basestring)
```

### Comparing `django-permission2-2.0.0b4/src/permission/conf.py` & `django_permission2-2.1.0/src/permission/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # coding=utf-8
 """
 django-permission2 application configure
 """
+from appconf import AppConf
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
-from appconf import AppConf
-from permission.handlers import LogicalPermissionHandler
 
+from permission.handlers import LogicalPermissionHandler
 
-__all__ = ('settings',)
+__all__ = ("settings",)
 
 
 class PermissionConf(AppConf):
-    DEFAULT_PERMISSION_HANDLER = 'permission.handlers.LogicalPermissionHandler'
+    DEFAULT_PERMISSION_HANDLER = "permission.handlers.LogicalPermissionHandler"
     """Default permission handler class"""
 
     CHECK_PERMISSION_PRESENCE = settings.DEBUG
     """Check if the specified string permission exists"""
 
     REPLACE_BUILTIN_IF = True
     """Whether replace builtin if templatetag"""
 
-    DEFAULT_APL_FIELD_NAME = 'author'
+    DEFAULT_APL_FIELD_NAME = "author"
     DEFAULT_APL_ANY_PERMISSION = False
     DEFAULT_APL_CHANGE_PERMISSION = True
     DEFAULT_APL_DELETE_PERMISSION = True
 
-    DEFAULT_CPL_FIELD_NAME = 'collaborators'
+    DEFAULT_CPL_FIELD_NAME = "collaborators"
     DEFAULT_CPL_ANY_PERMISSION = False
     DEFAULT_CPL_CHANGE_PERMISSION = True
     DEFAULT_CPL_DELETE_PERMISSION = False
 
     DEFAULT_GIPL_ANY_PERMISSION = False
     DEFAULT_GIPL_ADD_PERMISSION = True
     DEFAULT_GIPL_CHANGE_PERMISSION = True
@@ -41,16 +41,16 @@
     DEFAULT_OSPL_DELETE_PERMISSION = True
 
     DEFAULT_SPL_ANY_PERMISSION = False
     DEFAULT_SPL_ADD_PERMISSION = True
     DEFAULT_SPL_CHANGE_PERMISSION = True
     DEFAULT_SPL_DELETE_PERMISSION = False
 
-    AUTODISCOVER_MODULE_NAME = 'perms'
-    AUTODISCOVER_VARIABLE_NAME = 'PERMISSION_LOGICS'
+    AUTODISCOVER_MODULE_NAME = "perms"
+    AUTODISCOVER_VARIABLE_NAME = "PERMISSION_LOGICS"
     AUTODISCOVER_ENABLE = True
 
     CHECK_AUTHENTICATION_BACKENDS = True
     """Check if AUTHENTICATION_BACKENDS is correctly configured"""
 
     CHECK_TEMPLATES_OPTIONS_BUILTINS = True
     """Check if TEMPLATES[?]['OPTIONS']['builtins'] is correctly configured"""
```

### Comparing `django-permission2-2.0.0b4/src/permission/decorators/classbase.py` & `django_permission2-2.1.0/src/permission/decorators/classbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # coding=utf-8
 """
 permission_required decorator for generic classbased view from django 1.3
 """
 from functools import wraps
+
 from django.core.exceptions import PermissionDenied
+
 from permission.decorators.utils import redirect_to_login
 
 
-def permission_required(perm, queryset=None,
-                        login_url=None, raise_exception=False):
+def permission_required(perm, queryset=None, login_url=None, raise_exception=False):
     """
     Permission check decorator for classbased generic view
 
     This decorator works as class decorator
     DO NOT use ``method_decorator`` or whatever while this decorator will use
     ``self`` argument for method of classbased generic view.
 
@@ -32,37 +33,40 @@
 
     Examples
     --------
     >>> @permission_required('auth.change_user')
     >>> class UpdateAuthUserView(UpdateView):
     ...     pass
     """
+
     def wrapper(cls):
         def view_wrapper(view_func):
             @wraps(view_func)
             def inner(self, request, *args, **kwargs):
                 # get object
                 obj = get_object_from_classbased_instance(
-                        self, queryset, request, *args, **kwargs
-                    )
+                    self, queryset, request, *args, **kwargs
+                )
 
                 if not request.user.has_perm(perm, obj=obj):
                     if raise_exception:
                         raise PermissionDenied
                     else:
                         return redirect_to_login(request, login_url)
                 return view_func(self, request, *args, **kwargs)
+
             return inner
+
         cls.dispatch = view_wrapper(cls.dispatch)
         return cls
+
     return wrapper
 
 
-def get_object_from_classbased_instance(
-        instance, queryset, request, *args, **kwargs):
+def get_object_from_classbased_instance(instance, queryset, request, *args, **kwargs):
     """
     Get object from an instance of classbased generic view
 
     Parameters
     ----------
     instance : instance
         An instance of classbased generic view
@@ -73,40 +77,40 @@
 
     Returns
     -------
     instance
         An instance of model object or None
     """
     from django.views.generic.edit import BaseCreateView
+
     # initialize request, args, kwargs of classbased_instance
     # most of methods of classbased view assumed these attributes
     # but these attributes is initialized in ``dispatch`` method.
     instance.request = request
     instance.args = args
     instance.kwargs = kwargs
 
     # get queryset from class if ``queryset_or_model`` is not specified
-    if hasattr(instance, 'get_queryset') and not queryset:
+    if hasattr(instance, "get_queryset") and not queryset:
         queryset = instance.get_queryset()
-    elif hasattr(instance, 'queryset') and not queryset:
+    elif hasattr(instance, "queryset") and not queryset:
         queryset = instance.queryset
-    elif hasattr(instance, 'model') and not queryset:
+    elif hasattr(instance, "model") and not queryset:
         queryset = instance.model._default_manager.all()
 
     # get object
-    if hasattr(instance, 'get_object'):
+    if hasattr(instance, "get_object"):
         try:
             obj = instance.get_object(queryset)
         except AttributeError as e:
             # CreateView has ``get_object`` method but CreateView
             # should not have any object before thus simply set
             # None
             if isinstance(instance, BaseCreateView):
                 obj = None
             else:
                 raise e
-    elif hasattr(instance, 'object'):
+    elif hasattr(instance, "object"):
         obj = instance.object
     else:
         obj = None
     return obj
-
```

### Comparing `django-permission2-2.0.0b4/src/permission/decorators/functionbase.py` & `django_permission2-2.1.0/src/permission/decorators/functionbase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # coding=utf-8
 """
 permission_required decorator for generic function view
 """
 import copy
 from functools import wraps
-from django.shortcuts import get_object_or_404
+
 from django.core.exceptions import PermissionDenied
+from django.shortcuts import get_object_or_404
+
 from permission.decorators.utils import redirect_to_login
 
 
-def permission_required(perm, queryset=None,
-                        login_url=None, raise_exception=False):
+def permission_required(perm, queryset=None, login_url=None, raise_exception=False):
     """
     Permission check decorator for function-base generic view
 
     This decorator works as function decorator
 
     Parameters
     ----------
@@ -32,24 +33,25 @@
 
     Examples
     --------
     >>> @permission_required('auth.change_user')
     >>> def update_auth_user(request, *args, **kwargs):
     ...     pass
     """
+
     def wrapper(view_func):
         @wraps(view_func)
         def inner(request, *args, **kwargs):
             _kwargs = copy.copy(kwargs)
             # overwrite queryset if specified
             if queryset:
-                _kwargs['queryset'] = queryset
+                _kwargs["queryset"] = queryset
 
             # get object from view
-            if 'date_field' in _kwargs:
+            if "date_field" in _kwargs:
                 fn = get_object_from_date_based_view
             else:
                 fn = get_object_from_list_detail_view
             if fn.validate(request, *args, **_kwargs):
                 obj = fn(request, *args, **_kwargs)
             else:
                 # required arguments is not passed
@@ -57,15 +59,17 @@
 
             if not request.user.has_perm(perm, obj=obj):
                 if raise_exception:
                     raise PermissionDenied
                 else:
                     return redirect_to_login(request, login_url)
             return view_func(request, *args, **_kwargs)
+
         return inner
+
     return wrapper
 
 
 def get_object_from_list_detail_view(request, *args, **kwargs):
     """
     Get object from generic list_detail.detail view
 
@@ -75,36 +79,39 @@
         An instance of HttpRequest
 
     Returns
     -------
     instance
         An instance of model object or None
     """
-    queryset = kwargs['queryset']
-    object_id = kwargs.get('object_id', None)
-    slug = kwargs.get('slug', None)
-    slug_field = kwargs.get('slug_field', 'slug')
+    queryset = kwargs["queryset"]
+    object_id = kwargs.get("object_id", None)
+    slug = kwargs.get("slug", None)
+    slug_field = kwargs.get("slug_field", "slug")
     if object_id:
         obj = get_object_or_404(queryset, pk=object_id)
     elif slug and slug_field:
         obj = get_object_or_404(queryset, **{slug_field: slug})
     else:
         raise AttributeError(
-                "Generic detail view must be called with either an "
-                "object_id or a slug/slug_field."
-            )
+            "Generic detail view must be called with either an "
+            "object_id or a slug/slug_field."
+        )
     return obj
+
+
 def _get_object_from_list_detail_view_validation(request, *args, **kwargs):
-    if 'queryset' not in kwargs:
+    if "queryset" not in kwargs:
         return False
-    elif 'object_id' not in kwargs and 'slug' not in kwargs:
+    elif "object_id" not in kwargs and "slug" not in kwargs:
         return False
     return True
-get_object_from_list_detail_view.validate = \
-        _get_object_from_list_detail_view_validation
+
+
+get_object_from_list_detail_view.validate = _get_object_from_list_detail_view_validation
 
 
 def get_object_from_date_based_view(request, *args, **kwargs):  # noqa
     """
     Get object from generic date_based.detail view
 
     Parameters
@@ -113,68 +120,76 @@
         An instance of HttpRequest
 
     Returns
     -------
     instance
         An instance of model object or None
     """
-    import time
     import datetime
-    from django.http import Http404
+    import time
+
     from django.db.models.fields import DateTimeField
+    from django.http import Http404
+
     try:
         from django.utils import timezone
+
         datetime_now = timezone.now
     except ImportError:
         datetime_now = datetime.datetime.now
-    year, month, day = kwargs['year'], kwargs['month'], kwargs['day']
-    month_format = kwargs.get('month_format', '%b')
-    day_format = kwargs.get('day_format', '%d')
-    date_field = kwargs['date_field']
-    queryset = kwargs['queryset']
-    object_id = kwargs.get('object_id', None)
-    slug = kwargs.get('slug', None)
-    slug_field = kwargs.get('slug_field', 'slug')
+    year, month, day = kwargs["year"], kwargs["month"], kwargs["day"]
+    month_format = kwargs.get("month_format", "%b")
+    day_format = kwargs.get("day_format", "%d")
+    date_field = kwargs["date_field"]
+    queryset = kwargs["queryset"]
+    object_id = kwargs.get("object_id", None)
+    slug = kwargs.get("slug", None)
+    slug_field = kwargs.get("slug_field", "slug")
 
     try:
         tt = time.strptime(
-                '%s-%s-%s' % (year, month, day),
-                '%s-%s-%s' % ('%Y', month_format, day_format)
-            )
+            "%s-%s-%s" % (year, month, day),
+            "%s-%s-%s" % ("%Y", month_format, day_format),
+        )
         date = datetime.date(*tt[:3])
     except ValueError:
         raise Http404
 
     model = queryset.model
 
     if isinstance(model._meta.get_field(date_field), DateTimeField):
         lookup_kwargs = {
-                '%s__range' % date_field: (
-                    datetime.datetime.combine(date, datetime.time.min),
-                    datetime.datetime.combine(date, datetime.time.max),
-                )}
+            "%s__range"
+            % date_field: (
+                datetime.datetime.combine(date, datetime.time.min),
+                datetime.datetime.combine(date, datetime.time.max),
+            )
+        }
     else:
         lookup_kwargs = {date_field: date}
 
     now = datetime_now()
-    if date >= now.date() and not kwargs.get('allow_future', False):
-        lookup_kwargs['%s__lte' % date_field] = now
+    if date >= now.date() and not kwargs.get("allow_future", False):
+        lookup_kwargs["%s__lte" % date_field] = now
     if object_id:
-        lookup_kwargs['pk'] = object_id
+        lookup_kwargs["pk"] = object_id
     elif slug and slug_field:
-        lookup_kwargs['%s__exact' % slug_field] = slug
+        lookup_kwargs["%s__exact" % slug_field] = slug
     else:
         raise AttributeError(
-                "Generic detail view must be called with either an "
-                "object_id or a slug/slug_field."
-            )
+            "Generic detail view must be called with either an "
+            "object_id or a slug/slug_field."
+        )
     return get_object_or_404(queryset, **lookup_kwargs)
+
+
 def _get_object_from_date_based_view_validation(request, *args, **kwargs):
-    if 'queryset' not in kwargs:
+    if "queryset" not in kwargs:
         return False
-    elif 'year' not in kwargs or 'month' not in kwargs or 'day' not in kwargs:
+    elif "year" not in kwargs or "month" not in kwargs or "day" not in kwargs:
         return False
-    elif 'object_id' not in kwargs and 'slug' not in kwargs:
+    elif "object_id" not in kwargs and "slug" not in kwargs:
         return False
     return True
-get_object_from_date_based_view.validate = \
-        _get_object_from_date_based_view_validation
+
+
+get_object_from_date_based_view.validate = _get_object_from_date_based_view_validation
```

### Comparing `django-permission2-2.0.0b4/src/permission/decorators/methodbase.py` & `django_permission2-2.1.0/src/permission/decorators/methodbase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # coding=utf-8
 """
 permission_required decorator for generic classbased/functionbased view
 """
 from functools import wraps
-from django.http import HttpRequest
+
 from django.core.exceptions import PermissionDenied
+from django.http import HttpRequest
+
 from permission.decorators.utils import redirect_to_login
 
 
-def permission_required(perm, queryset=None,
-                        login_url=None, raise_exception=False):
+def permission_required(perm, queryset=None, login_url=None, raise_exception=False):
     """
     Permission check decorator for classbased/functionbased generic view
 
     This decorator works as method or function decorator
     DO NOT use ``method_decorator`` or whatever while this decorator will use
     ``self`` argument for method of classbased generic view.
 
@@ -39,38 +40,44 @@
     >>>     def dispatch(self, request, *args, **kwargs):
     ...         pass
     >>> # As function decorator
     >>> @permission_required('auth.change_user')
     >>> def update_auth_user(request, *args, **kwargs):
     ...     pass
     """
+
     def wrapper(view_method):
         @wraps(view_method)
         def inner(self, request=None, *args, **kwargs):
             if isinstance(self, HttpRequest):
-                from permission.decorators.functionbase import \
-                        permission_required as decorator
+                from permission.decorators.functionbase import (
+                    permission_required as decorator,
+                )
+
                 # this is a functional view not classbased view.
-                decorator = decorator(perm, queryset,
-                                      login_url, raise_exception)
+                decorator = decorator(perm, queryset, login_url, raise_exception)
                 decorator = decorator(view_method)
                 if not request:
                     args = list(args)
                     args.insert(0, request)
                 request = self
                 return decorator(request, *args, **kwargs)
             else:
-                from permission.decorators.classbase import \
-                        get_object_from_classbased_instance
+                from permission.decorators.classbase import (
+                    get_object_from_classbased_instance,
+                )
+
                 # get object
                 obj = get_object_from_classbased_instance(
-                        self, queryset, request, *args, **kwargs
-                    )
+                    self, queryset, request, *args, **kwargs
+                )
 
                 if not request.user.has_perm(perm, obj=obj):
                     if raise_exception:
                         raise PermissionDenied
                     else:
                         return redirect_to_login(request, login_url)
                 return view_method(self, request, *args, **kwargs)
+
         return inner
+
     return wrapper
```

### Comparing `django-permission2-2.0.0b4/src/permission/decorators/permission_required.py` & `django_permission2-2.1.0/src/permission/decorators/permission_required.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 Decorator module for permission
 """
 import inspect
-from django.db.models import Model
 
+from django.db.models import Model
 
-__all__ = ['permission_required']
+__all__ = ["permission_required"]
 
 
-def permission_required(perm, queryset_or_model=None,
-                        login_url=None, raise_exception=False):
+def permission_required(
+    perm, queryset_or_model=None, login_url=None, raise_exception=False
+):
     """
     Permission check decorator for classbased/functional generic view
 
     This decorator works as class, method or function decorator without any
     modification.
     DO NOT use ``method_decorator`` or whatever while this decorator will use
     ``self`` argument for method of classbased generic view.
@@ -55,17 +56,19 @@
     """
     # convert model to queryset
     if queryset_or_model and issubclass(queryset_or_model, Model):
         queryset_or_model = queryset_or_model._default_manager.all()
 
     def wrapper(class_or_method):
         if inspect.isclass(class_or_method):
-            from permission.decorators.classbase import \
-                    permission_required as decorator
+            from permission.decorators.classbase import permission_required as decorator
         else:
             # method_permission_required can handle method or function
             # correctly.
-            from permission.decorators.methodbase import \
-                    permission_required as decorator
-        return decorator(perm, queryset_or_model,
-                         login_url, raise_exception)(class_or_method)
+            from permission.decorators.methodbase import (
+                permission_required as decorator,
+            )
+        return decorator(perm, queryset_or_model, login_url, raise_exception)(
+            class_or_method
+        )
+
     return wrapper
```

### Comparing `django-permission2-2.0.0b4/src/permission/decorators/utils.py` & `django_permission2-2.1.0/src/permission/decorators/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # coding=utf-8
 """
 Decorator utility module
 """
 from django.contrib.auth import REDIRECT_FIELD_NAME
-from permission.conf import settings
-from permission.compat import urlparse
 
+from permission.compat import urlparse
+from permission.conf import settings
 
-__all__ = ['redirect_to_login']
+__all__ = ["redirect_to_login"]
 
 
-def redirect_to_login(request, login_url=None,
-                      redirect_field_name=REDIRECT_FIELD_NAME):
+def redirect_to_login(request, login_url=None, redirect_field_name=REDIRECT_FIELD_NAME):
     """redirect to login"""
     path = request.build_absolute_uri()
     # if the login url is the same scheme and net location then just
     # use the path as the "next" url.
-    login_scheme, login_netloc = \
-            urlparse(login_url or settings.LOGIN_URL)[:2]
+    login_scheme, login_netloc = urlparse(login_url or settings.LOGIN_URL)[:2]
     current_scheme, current_netloc = urlparse(path)[:2]
-    if ((not login_scheme or login_scheme == current_scheme) and
-            (not login_netloc or login_netloc == current_netloc)):
+    if (not login_scheme or login_scheme == current_scheme) and (
+        not login_netloc or login_netloc == current_netloc
+    ):
         path = request.get_full_path()
-    from django.contrib.auth.views import \
-            redirect_to_login as auth_redirect_to_login
+    from django.contrib.auth.views import redirect_to_login as auth_redirect_to_login
+
     return auth_redirect_to_login(path, login_url, redirect_field_name)
```

### Comparing `django-permission2-2.0.0b4/src/permission/handlers.py` & `django_permission2-2.1.0/src/permission/handlers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # coding=utf-8
-import collections
-from permission.utils.permissions import get_app_perms
-from permission.utils.permissions import get_model_perms
+from collections.abc import Callable
+
+from permission.utils.permissions import get_app_perms, get_model_perms
 
 
 class PermissionHandler(object):
     """
     Abstract permission handler class
     """
+
     _includes = None
     _excludes = None
 
     @property
     def includes(self):
         return self._includes
 
     @includes.setter
     def includes(self, value):
         # clear cache
-        if hasattr(self, '_perms_cache'):
+        if hasattr(self, "_perms_cache"):
             del self._perms_cache
         self._includes = value
 
     @property
     def excludes(self):
         return self._excludes
 
     @excludes.setter
     def excludes(self, value):
         # clear cache
-        if hasattr(self, '_perms_cache'):
+        if hasattr(self, "_perms_cache"):
             del self._perms_cache
         self._excludes = value
 
     def __init__(self, model_or_app_label):
         """
         Constructor
 
@@ -61,28 +62,28 @@
         Get permissions related to the application specified in constructor
 
         Returns
         -------
         set
             A set instance of `app_label.codename` formatted permission strings
         """
-        if not hasattr(self, '_app_perms_cache'):
+        if not hasattr(self, "_app_perms_cache"):
             self._app_perms_cache = get_app_perms(self.app_label)
         return self._app_perms_cache
 
     def _get_model_perms(self, *args):
         """
         Get permissions related to the model specified in constructor
 
         Returns
         -------
         set
             A set instance of `app_label.codename` formatted permission strings
         """
-        if not hasattr(self, '_model_perms_cache'):
+        if not hasattr(self, "_model_perms_cache"):
             if self.model is None:
                 self._model_perms_cache = set()
             else:
                 self._model_perms_cache = get_model_perms(self.model)
         return self._model_perms_cache
 
     def get_supported_permissions(self):
@@ -91,22 +92,20 @@
         Specified with :attr:`includes` and :attr:`excludes` of this instance.
 
         Returns
         -------
         set
             A set instance of `app_label.codename` formatted permission strings
         """
-        if not hasattr(self, '_perms_cache'):
-            if (self.includes and
-                    isinstance(self.includes, collections.Callable)):
+        if not hasattr(self, "_perms_cache"):
+            if self.includes and isinstance(self.includes, Callable):
                 includes = self.includes(self)
             else:
                 includes = self.includes or []
-            if (self.excludes and
-                    isinstance(self.excludes, collections.Callable)):
+            if self.excludes and isinstance(self.excludes, Callable):
                 excludes = self.excludes(self)
             else:
                 excludes = self.excludes or []
             includes = set(includes)
             excludes = set(excludes)
             includes = includes.difference(excludes)
             self._perms_cache = includes
@@ -119,15 +118,15 @@
 
         Returns
         -------
         set
             A set instance of app_label
         """
         get_app_label = lambda x: x.split(".", 1)[0]
-        if not hasattr(self, '_app_labels_cache'):
+        if not hasattr(self, "_app_labels_cache"):
             perms = self.get_supported_permissions()
             self._app_labels_cache = set([get_app_label(x) for x in perms])
         return self._app_labels_cache
 
     def has_perm(self, user_obj, perm, obj=None):
         """
         Check if user have permission (of object)
@@ -146,18 +145,21 @@
         boolean
             Whether the specified user have specified permission (of specified
             object).
 
         .. note::
             Sub class must override this method.
         """
-        raise NotImplementedError((
-            "'%s' does not override `has_perm(user_obj, perm, obj=None)` "
-            "method. Sub class must override this method."
-        ) % self.__class__)
+        raise NotImplementedError(
+            (
+                "'%s' does not override `has_perm(user_obj, perm, obj=None)` "
+                "method. Sub class must override this method."
+            )
+            % self.__class__
+        )
 
     def has_module_perms(self, user_obj, app_label):
         """
         Check if user have permission of specified app
 
         Parameters
         ----------
@@ -202,17 +204,17 @@
             A django model class.
 
         .. note::
             LogicalPermissionHandler cannot treat application level permission
         """
         # logical permission handler cannot treat application level permission
         if isinstance(model, str):
-            raise AttributeError((
-                "'%s' cannot treat application level permission."
-            ) % self.__class__)
+            raise AttributeError(
+                ("'%s' cannot treat application level permission.") % self.__class__
+            )
         super(LogicalPermissionHandler, self).__init__(model)
 
     def has_perm(self, user_obj, perm, obj=None):
         """
         Check if user have permission (of object) based on
         specified models's ``_permission_logics`` attribute.
 
@@ -232,24 +234,23 @@
         boolean
             Whether the specified user have specified permission (of specified
             object).
         """
         if perm not in self.get_supported_permissions():
             return False
         # use cache to reduce method call
-        CACHE_NAME = '_logical_perms_cache'
+        CACHE_NAME = "_logical_perms_cache"
         if not hasattr(user_obj, CACHE_NAME):
             setattr(user_obj, CACHE_NAME, {})
         cache = getattr(user_obj, CACHE_NAME)
         cachekey = "%s %s" % (perm, hash(obj))
         if cachekey not in cache:
             cache[cachekey] = self._has_perm(user_obj, perm, obj)
         return cache[cachekey]
 
     def _has_perm(self, user_obj, perm, obj=None):
         if perm not in self.get_supported_permissions():
             return False
-        for permission_logic in getattr(self.model,
-                                        '_permission_logics', set()):
+        for permission_logic in getattr(self.model, "_permission_logics", set()):
             if permission_logic.has_perm(user_obj, perm, obj):
                 return True
         return False
```

### Comparing `django-permission2-2.0.0b4/src/permission/logics/author.py` & `django_permission2-2.1.0/src/permission/logics/author.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # coding=utf-8
 """
 Permission logic module for author based permission system
 """
+from permission.compat import is_authenticated
 from permission.conf import settings
 from permission.logics.base import PermissionLogic
 from permission.utils.field_lookup import field_lookup
-from permission.compat import is_authenticated
 
 
 class AuthorPermissionLogic(PermissionLogic):
     """
     Permission logic class for author based permission system
     """
-    def __init__(self,
-                 field_name=None,
-                 any_permission=None,
-                 change_permission=None,
-                 delete_permission=None):
+
+    def __init__(
+        self,
+        field_name=None,
+        any_permission=None,
+        change_permission=None,
+        delete_permission=None,
+    ):
         """
         Constructor
 
         Parameters
         ----------
         field_name : string
             A field name of object which store the author as django user model.
@@ -51,25 +54,21 @@
         """
         self.field_name = field_name
         self.any_permission = any_permission
         self.change_permission = change_permission
         self.delete_permission = delete_permission
 
         if self.field_name is None:
-            self.field_name = \
-                settings.PERMISSION_DEFAULT_APL_FIELD_NAME
+            self.field_name = settings.PERMISSION_DEFAULT_APL_FIELD_NAME
         if self.any_permission is None:
-            self.any_permission = \
-                settings.PERMISSION_DEFAULT_APL_ANY_PERMISSION
+            self.any_permission = settings.PERMISSION_DEFAULT_APL_ANY_PERMISSION
         if self.change_permission is None:
-            self.change_permission = \
-                settings.PERMISSION_DEFAULT_APL_CHANGE_PERMISSION
+            self.change_permission = settings.PERMISSION_DEFAULT_APL_CHANGE_PERMISSION
         if self.delete_permission is None:
-            self.delete_permission = \
-                settings.PERMISSION_DEFAULT_APL_DELETE_PERMISSION
+            self.delete_permission = settings.PERMISSION_DEFAULT_APL_DELETE_PERMISSION
 
     def has_perm(self, user_obj, perm, obj=None):
         """
         Check if user have permission (of object)
 
         If the user_obj is not authenticated, it return ``False``.
 
@@ -100,16 +99,16 @@
         boolean
             Whether the specified user have specified permission (of specified
             object).
         """
         if not is_authenticated(user_obj):
             return False
         # construct the permission full name
-        change_permission = self.get_full_permission_string('change')
-        delete_permission = self.get_full_permission_string('delete')
+        change_permission = self.get_full_permission_string("change")
+        delete_permission = self.get_full_permission_string("delete")
         # check if the user is authenticated
         if obj is None:
             # object permission without obj should return True
             # Ref: https://code.djangoproject.com/wiki/RowLevelPermissions
             if self.any_permission:
                 return True
             if self.change_permission and perm == change_permission:
@@ -120,14 +119,12 @@
         elif user_obj.is_active:
             # get author instance
             author = field_lookup(obj, self.field_name)
             if author == user_obj:
                 if self.any_permission:
                     # have any kind of permissions to the obj
                     return True
-                if (self.change_permission and
-                        perm == change_permission):
+                if self.change_permission and perm == change_permission:
                     return True
-                if (self.delete_permission and
-                        perm == delete_permission):
+                if self.delete_permission and perm == delete_permission:
                     return True
         return False
```

### Comparing `django-permission2-2.0.0b4/src/permission/logics/base.py` & `django_permission2-2.1.0/src/permission/logics/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # coding=utf-8
 
 
 class PermissionLogic(object):
     """
     Abstract permission logic class
     """
+
     def get_full_permission_string(self, perm):
         """
         Return full permission string (app_label.perm_model)
         """
-        if not getattr(self, 'model', None):
-            raise AttributeError("You need to use `add_permission_logic` to "
-                                 "register the instance to the model class "
-                                 "before calling this method.")
+        if not getattr(self, "model", None):
+            raise AttributeError(
+                "You need to use `add_permission_logic` to "
+                "register the instance to the model class "
+                "before calling this method."
+            )
         app_label = self.model._meta.app_label
         model_name = self.model._meta.object_name.lower()
         return "%s.%s_%s" % (app_label, perm, model_name)
 
     def has_perm(self, user_obj, perm, obj=None):
         """
         Check if user have permission (of object)
@@ -36,10 +39,11 @@
             Whether the specified user have specified permission (of specified
             object).
 
         .. note::
             Sub class must override this method.
         """
         raise NotImplementedError(
-                "'%s' does not override `has_perm(user_obj, perm, obj=None)` "
-                "method. Sub class of `PermissionLogic` must override this "
-                "method.")
+            "'%s' does not override `has_perm(user_obj, perm, obj=None)` "
+            "method. Sub class of `PermissionLogic` must override this "
+            "method."
+        )
```

### Comparing `django-permission2-2.0.0b4/src/permission/logics/collaborators.py` & `django_permission2-2.1.0/src/permission/logics/collaborators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # coding=utf-8
 """
 Permission logic module for collaborators based permission system
 """
+from permission.compat import is_authenticated
 from permission.conf import settings
 from permission.logics.base import PermissionLogic
 from permission.utils.field_lookup import field_lookup
-from permission.compat import is_authenticated
 
 
 class CollaboratorsPermissionLogic(PermissionLogic):
     """
     Permission logic class for collaborators based permission system
     """
-    def __init__(self,
-                 field_name=None,
-                 any_permission=None,
-                 change_permission=None,
-                 delete_permission=None):
+
+    def __init__(
+        self,
+        field_name=None,
+        any_permission=None,
+        change_permission=None,
+        delete_permission=None,
+    ):
         """
         Constructor
 
         Parameters
         ----------
         field_name : string
             A field name of object which store the collaborators as django
@@ -53,25 +56,21 @@
         """
         self.field_name = field_name
         self.any_permission = any_permission
         self.change_permission = change_permission
         self.delete_permission = delete_permission
 
         if self.field_name is None:
-            self.field_name = \
-                settings.PERMISSION_DEFAULT_CPL_FIELD_NAME
+            self.field_name = settings.PERMISSION_DEFAULT_CPL_FIELD_NAME
         if self.any_permission is None:
-            self.any_permission = \
-                settings.PERMISSION_DEFAULT_CPL_ANY_PERMISSION
+            self.any_permission = settings.PERMISSION_DEFAULT_CPL_ANY_PERMISSION
         if self.change_permission is None:
-            self.change_permission = \
-                settings.PERMISSION_DEFAULT_CPL_CHANGE_PERMISSION
+            self.change_permission = settings.PERMISSION_DEFAULT_CPL_CHANGE_PERMISSION
         if self.delete_permission is None:
-            self.delete_permission = \
-                settings.PERMISSION_DEFAULT_CPL_DELETE_PERMISSION
+            self.delete_permission = settings.PERMISSION_DEFAULT_CPL_DELETE_PERMISSION
 
     def has_perm(self, user_obj, perm, obj=None):
         """
         Check if user have permission (of object)
 
         If the user_obj is not authenticated, it return ``False``.
 
@@ -103,35 +102,33 @@
         boolean
             Whether the specified user have specified permission (of specified
             object).
         """
         if not is_authenticated(user_obj):
             return False
         # construct the permission full name
-        change_permission = self.get_full_permission_string('change')
-        delete_permission = self.get_full_permission_string('delete')
+        change_permission = self.get_full_permission_string("change")
+        delete_permission = self.get_full_permission_string("delete")
         if obj is None:
             # object permission without obj should return True
             # Ref: https://code.djangoproject.com/wiki/RowLevelPermissions
             if self.any_permission:
                 return True
             if self.change_permission and perm == change_permission:
                 return True
             if self.delete_permission and perm == delete_permission:
                 return True
             return False
         elif user_obj.is_active:
             # get collaborator queryset
             collaborators = field_lookup(obj, self.field_name)
-            if hasattr(collaborators, 'all'):
+            if hasattr(collaborators, "all"):
                 collaborators = collaborators.all()
             if user_obj in collaborators:
                 if self.any_permission:
                     # have any kind of permissions to the obj
                     return True
-                if (self.change_permission and
-                        perm == change_permission):
+                if self.change_permission and perm == change_permission:
                     return True
-                if (self.delete_permission and
-                        perm == delete_permission):
+                if self.delete_permission and perm == delete_permission:
                     return True
         return False
```

### Comparing `django-permission2-2.0.0b4/src/permission/logics/groupin.py` & `django_permission2-2.1.0/src/permission/logics/groupin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # coding=utf-8
 """
 Permission logic module for group based permission system
 """
+from permission.compat import is_authenticated
 from permission.conf import settings
 from permission.logics.base import PermissionLogic
-from permission.compat import is_authenticated
 
 
 class GroupInPermissionLogic(PermissionLogic):
     """
     Permission logic class for group based permission system
     """
-    def __init__(self,
-                 group_names,
-                 any_permission=None,
-                 add_permission=None,
-                 change_permission=None,
-                 delete_permission=None):   # noqa
+
+    def __init__(
+        self,
+        group_names,
+        any_permission=None,
+        add_permission=None,
+        change_permission=None,
+        delete_permission=None,
+    ):  # noqa
         """
         Constructor
 
         Parameters
         ----------
         group_names : string or list
             A group name list of this permission logic treat
@@ -55,25 +58,21 @@
             self.group_names = [self.group_names]
         self.any_permission = any_permission
         self.add_permission = add_permission
         self.change_permission = change_permission
         self.delete_permission = delete_permission
 
         if self.any_permission is None:
-            self.any_permission = \
-                settings.PERMISSION_DEFAULT_GIPL_ANY_PERMISSION
+            self.any_permission = settings.PERMISSION_DEFAULT_GIPL_ANY_PERMISSION
         if self.add_permission is None:
-            self.add_permission = \
-                settings.PERMISSION_DEFAULT_GIPL_ADD_PERMISSION
+            self.add_permission = settings.PERMISSION_DEFAULT_GIPL_ADD_PERMISSION
         if self.change_permission is None:
-            self.change_permission = \
-                settings.PERMISSION_DEFAULT_GIPL_CHANGE_PERMISSION
+            self.change_permission = settings.PERMISSION_DEFAULT_GIPL_CHANGE_PERMISSION
         if self.delete_permission is None:
-            self.delete_permission = \
-                settings.PERMISSION_DEFAULT_GIPL_DELETE_PERMISSION
+            self.delete_permission = settings.PERMISSION_DEFAULT_GIPL_DELETE_PERMISSION
 
     def has_perm(self, user_obj, perm, obj=None):
         """
         Check if user have permission (of object)
 
         If the user_obj is not authenticated, it return ``False``.
 
@@ -104,17 +103,17 @@
         boolean
             Whether the specified user have specified permission (of specified
             object).
         """
         if not is_authenticated(user_obj):
             return False
         # construct the permission full name
-        add_permission = self.get_full_permission_string('add')
-        change_permission = self.get_full_permission_string('change')
-        delete_permission = self.get_full_permission_string('delete')
+        add_permission = self.get_full_permission_string("add")
+        change_permission = self.get_full_permission_string("change")
+        delete_permission = self.get_full_permission_string("delete")
         if obj is None:
             if user_obj.groups.filter(name__in=self.group_names):
                 if self.add_permission and perm == add_permission:
                     return True
                 if self.change_permission and perm == change_permission:
                     return True
                 if self.delete_permission and perm == delete_permission:
@@ -122,17 +121,14 @@
                 return self.any_permission
             return False
         elif user_obj.is_active:
             if user_obj.groups.filter(name__in=self.group_names):
                 if self.any_permission:
                     # have any kind of permissions to the obj
                     return True
-                if (self.add_permission and
-                        perm == add_permission):
+                if self.add_permission and perm == add_permission:
                     return True
-                if (self.change_permission and
-                        perm == change_permission):
+                if self.change_permission and perm == change_permission:
                     return True
-                if (self.delete_permission and
-                        perm == delete_permission):
+                if self.delete_permission and perm == delete_permission:
                     return True
         return False
```

### Comparing `django-permission2-2.0.0b4/src/permission/logics/oneself.py` & `django_permission2-2.1.0/src/permission/logics/oneself.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding=utf-8
 """
 Permission logic module to  manage users' self-modifications
 """
+from permission.compat import is_authenticated
 from permission.conf import settings
 from permission.logics.base import PermissionLogic
-from permission.compat import is_authenticated
 
 
 class OneselfPermissionLogic(PermissionLogic):
     """
     Permission logic class to manage users' self-modifications
 
     Written by quasiyoke.
     https://github.com/lambdalisue/django-permission/pull/27
     """
-    def __init__(self,
-                 any_permission=None,
-                 change_permission=None,
-                 delete_permission=None):
+
+    def __init__(
+        self, any_permission=None, change_permission=None, delete_permission=None
+    ):
         """
         Constructor
 
         Parameters
         ----------
         any_permission : boolean
             True for give any permission of the user to himself.
@@ -42,22 +42,19 @@
             settings.
         """
         self.any_permission = any_permission
         self.change_permission = change_permission
         self.delete_permission = delete_permission
 
         if self.any_permission is None:
-            self.any_permission = \
-                settings.PERMISSION_DEFAULT_OSPL_ANY_PERMISSION
+            self.any_permission = settings.PERMISSION_DEFAULT_OSPL_ANY_PERMISSION
         if self.change_permission is None:
-            self.change_permission = \
-                settings.PERMISSION_DEFAULT_OSPL_CHANGE_PERMISSION
+            self.change_permission = settings.PERMISSION_DEFAULT_OSPL_CHANGE_PERMISSION
         if self.delete_permission is None:
-            self.delete_permission = \
-                settings.PERMISSION_DEFAULT_OSPL_DELETE_PERMISSION
+            self.delete_permission = settings.PERMISSION_DEFAULT_OSPL_DELETE_PERMISSION
 
     def has_perm(self, user_obj, perm, obj=None):
         """
         Check if user have permission of himself
 
         If the user_obj is not authenticated, it return ``False``.
 
@@ -86,16 +83,16 @@
         boolean
             Whether the specified user have specified permission (of specified
             object).
         """
         if not is_authenticated(user_obj):
             return False
         # construct the permission full name
-        change_permission = self.get_full_permission_string('change')
-        delete_permission = self.get_full_permission_string('delete')
+        change_permission = self.get_full_permission_string("change")
+        delete_permission = self.get_full_permission_string("delete")
         # check if the user is authenticated
         if obj is None:
             # object permission without obj should return True
             # Ref: https://code.djangoproject.com/wiki/RowLevelPermissions
             if self.any_permission:
                 return True
             if self.change_permission and perm == change_permission:
@@ -105,14 +102,12 @@
             return False
         elif user_obj.is_active:
             # check if the user trying to interact with himself
             if obj == user_obj:
                 if self.any_permission:
                     # have any kind of permissions to himself
                     return True
-                if (self.change_permission and
-                        perm == change_permission):
+                if self.change_permission and perm == change_permission:
                     return True
-                if (self.delete_permission and
-                        perm == delete_permission):
+                if self.delete_permission and perm == delete_permission:
                     return True
         return False
```

### Comparing `django-permission2-2.0.0b4/src/permission/logics/staff.py` & `django_permission2-2.1.0/src/permission/logics/staff.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # coding=utf-8
 """
 Permission logic module for author based permission system
 """
+from permission.compat import is_authenticated
 from permission.conf import settings
 from permission.logics.base import PermissionLogic
-from permission.compat import is_authenticated
 
 
 class StaffPermissionLogic(PermissionLogic):
     """
     Permission logic class for is_staff authority based permission system
     """
-    def __init__(self,
-                 any_permission=None,
-                 add_permission=None,
-                 change_permission=None,
-                 delete_permission=None):
+
+    def __init__(
+        self,
+        any_permission=None,
+        add_permission=None,
+        change_permission=None,
+        delete_permission=None,
+    ):
         """
         Constructor
 
         Parameters
         ----------
         any_permission : boolean
             True for give any permission of the specified object to the staff
@@ -50,25 +53,21 @@
         """
         self.any_permission = any_permission
         self.add_permission = add_permission
         self.change_permission = change_permission
         self.delete_permission = delete_permission
 
         if self.any_permission is None:
-            self.any_permission = \
-                settings.PERMISSION_DEFAULT_SPL_ANY_PERMISSION
+            self.any_permission = settings.PERMISSION_DEFAULT_SPL_ANY_PERMISSION
         if self.add_permission is None:
-            self.add_permission = \
-                settings.PERMISSION_DEFAULT_SPL_ADD_PERMISSION
+            self.add_permission = settings.PERMISSION_DEFAULT_SPL_ADD_PERMISSION
         if self.change_permission is None:
-            self.change_permission = \
-                settings.PERMISSION_DEFAULT_SPL_CHANGE_PERMISSION
+            self.change_permission = settings.PERMISSION_DEFAULT_SPL_CHANGE_PERMISSION
         if self.delete_permission is None:
-            self.delete_permission = \
-                settings.PERMISSION_DEFAULT_SPL_DELETE_PERMISSION
+            self.delete_permission = settings.PERMISSION_DEFAULT_SPL_DELETE_PERMISSION
 
     def has_perm(self, user_obj, perm, obj=None):
         """
         Check if user have permission (of object)
 
         If the user_obj is not authenticated, it return ``False``.
 
@@ -97,17 +96,17 @@
         boolean
             Weather the specified user have specified permission (of specified
             object).
         """
         if not is_authenticated(user_obj):
             return False
         # construct the permission full name
-        add_permission = self.get_full_permission_string('add')
-        change_permission = self.get_full_permission_string('change')
-        delete_permission = self.get_full_permission_string('delete')
+        add_permission = self.get_full_permission_string("add")
+        change_permission = self.get_full_permission_string("change")
+        delete_permission = self.get_full_permission_string("delete")
         if obj is None:
             if user_obj.is_staff:
                 if self.add_permission and perm == add_permission:
                     return True
                 if self.change_permission and perm == change_permission:
                     return True
                 if self.delete_permission and perm == delete_permission:
@@ -115,17 +114,14 @@
                 return self.any_permission
             return False
         elif user_obj.is_active:
             if user_obj.is_staff:
                 if self.any_permission:
                     # have any kind of permissions to the obj
                     return True
-                if (self.add_permission and
-                        perm == add_permission):
+                if self.add_permission and perm == add_permission:
                     return True
-                if (self.change_permission and
-                        perm == change_permission):
+                if self.change_permission and perm == change_permission:
                     return True
-                if (self.delete_permission and
-                        perm == delete_permission):
+                if self.delete_permission and perm == delete_permission:
                     return True
         return False
```

### Comparing `django-permission2-2.0.0b4/src/permission/templatetags/permissionif.py` & `django_permission2-2.1.0/src/permission/templatetags/permissionif.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # vim: set fileencoding=utf-8 :
 """
 permissionif templatetag
 """
 from django import template
 from django.template import TemplateSyntaxError
-from django.template.smartif import infix
-from django.template.smartif import IfParser
-from django.template.smartif import OPERATORS
-from django.template.defaulttags import IfNode
-from django.template.defaulttags import TemplateLiteral
+from django.template.defaulttags import IfNode, TemplateLiteral
+from django.template.smartif import OPERATORS, IfParser, infix
+
 from permission.conf import settings
 
 register = template.Library()
 
 
 def of_operator(context, x, y):
     """
@@ -33,26 +31,28 @@
     perm = y.eval(context)
     if isinstance(perm, (list, tuple)):
         perm, obj = perm
     else:
         obj = None
     return user.has_perm(perm, obj)
 
+
 # Add 'of' and 'has' operator to existing operators
 EXTRA_OPERATORS = {
-    'of': infix(20, of_operator),
-    'has': infix(10, has_operator),
+    "of": infix(20, of_operator),
+    "has": infix(10, has_operator),
 }
 EXTRA_OPERATORS.update(OPERATORS)
 for key, op in EXTRA_OPERATORS.items():
     op.id = key
 
 
 class PermissionIfParser(IfParser):
     """Permission if parser"""
+
     OPERATORS = EXTRA_OPERATORS
     """use extra operator"""
 
     def translate_token(self, token):
         try:
             # use own operators instead of builtin operators
             op = self.OPERATORS[token]
@@ -69,15 +69,15 @@
         self.template_parser = parser
         super(TemplatePermissionIfParser, self).__init__(*args, **kwargs)
 
     def create_var(self, value):
         return TemplateLiteral(self.template_parser.compile_filter(value), value)
 
 
-@register.tag('permission')
+@register.tag("permission")
 def do_permissionif(parser, token):
     """
     Permission if templatetag
 
     Examples
     --------
     ::
@@ -122,23 +122,28 @@
         conditions_nodelists.append((None, nodelist))
         token = parser.next_token()
 
     # {% endif %}
     assert token.contents == ENDIF
 
     return IfNode(conditions_nodelists)
+
+
 do_permissionif.Parser = TemplatePermissionIfParser
 
 
 # To replace builtin if
 def replace_builtin_if(replace=False):
     if replace:
-        OPERATORS.update({
-            'has': EXTRA_OPERATORS['has'],
-            'of': EXTRA_OPERATORS['of'],
-        })
+        OPERATORS.update(
+            {
+                "has": EXTRA_OPERATORS["has"],
+                "of": EXTRA_OPERATORS["of"],
+            }
+        )
     else:
         # remove of, has from OPERATORS
-        OPERATORS.pop('of', None)
-        OPERATORS.pop('has', None)
+        OPERATORS.pop("of", None)
+        OPERATORS.pop("has", None)
+
 
 replace_builtin_if(settings.PERMISSION_REPLACE_BUILTIN_IF)
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/compat.py` & `django_permission2-2.1.0/src/permission/tests/compat.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,26 +5,32 @@
     from mock import MagicMock
 
 from django.test import override_settings
 
 try:
     from unittest import skipIf
 except ImportError:
+
     def skipIf(condition, message):
         def decorator(f):
             return None if condition else f
+
         return decorator
 
+
 from django.conf import settings
+
 try:
     from django.test.runner import DiscoverRunner as TestRunnerBase
 except ImportError:
     from django.test.simple import DjangoTestSuiteRunner as TestRunnerBase
 
 settings.TESTING = False
+
+
 class TestRunner(TestRunnerBase):
     def setup_test_environment(self, **kwargs):
         super(TestRunner, self).setup_test_environment(**kwargs)
         settings.TESTING = True
 
     def teardown_test_environment(self, **kwargs):
         super(TestRunner, self).teardown_test_environment(**kwargs)
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_backends.py` & `django_permission2-2.1.0/src/permission/tests/test_backends.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,60 @@
-from django.test import TestCase, override_settings
 from django.core.exceptions import ObjectDoesNotExist
+from django.test import TestCase, override_settings
+
 from ..backends import PermissionBackend
 from ..utils.handlers import registry
 from .compat import MagicMock
-from .utils import create_user, create_article
 from .models import Article
+from .utils import create_article, create_user
 
 
 @override_settings(
     AUTHENTICATION_BACKENDS=(
-        'django.contrib.auth.backends.ModelBackend',
-        'permission.backends.PermissionBackend',
+        "django.contrib.auth.backends.ModelBackend",
+        "permission.backends.PermissionBackend",
     ),
 )
 class PermissionPermissionBackendTestCase(TestCase):
     def setUp(self):
-        self.user = create_user('john')
-        self.perm1 = 'permission.add_article'
-        self.perm2 = 'permission.change_article'
-        self.perm3 = 'permission.delete_article'
-        self.article = create_article('test')
+        self.user = create_user("john")
+        self.perm1 = "permission.add_article"
+        self.perm2 = "permission.change_article"
+        self.perm3 = "permission.delete_article"
+        self.article = create_article("test")
         self.original_get_handlers = registry.get_handlers
 
     def tearDown(self):
         registry.get_handlers = self.original_get_handlers
 
     def test_constructor(self):
         backend = PermissionBackend()
 
     def test_authenticate(self):
         backend = PermissionBackend()
         self.assertEqual(backend.authenticate(None, None), None)
 
     def test_has_perm_without_obj(self):
         perms = [
-            'permission.add_article',
-            'permission.change_article',
-            'permission.delete_article',
+            "permission.add_article",
+            "permission.change_article",
+            "permission.delete_article",
         ]
-        registry.get_handlers = MagicMock(return_value=[
-            MagicMock(get_supported_permissions=MagicMock(return_value=perms),
-                      has_perm=MagicMock(return_value=False)),
-            MagicMock(get_supported_permissions=MagicMock(return_value=perms),
-                      has_perm=MagicMock(return_value=True)),
-        ])
+        registry.get_handlers = MagicMock(
+            return_value=[
+                MagicMock(
+                    get_supported_permissions=MagicMock(return_value=perms),
+                    has_perm=MagicMock(return_value=False),
+                ),
+                MagicMock(
+                    get_supported_permissions=MagicMock(return_value=perms),
+                    has_perm=MagicMock(return_value=True),
+                ),
+            ]
+        )
 
         backend = PermissionBackend()
         self.assertFalse(registry.get_handlers.called)
         self.assertFalse(registry.get_handlers()[0].get_supported_permissions.called)
         self.assertFalse(registry.get_handlers()[1].get_supported_permissions.called)
         self.assertFalse(registry.get_handlers()[0].has_perm.called)
         self.assertFalse(registry.get_handlers()[1].has_perm.called)
@@ -58,24 +65,30 @@
         self.assertTrue(registry.get_handlers()[0].get_supported_permissions.called)
         self.assertTrue(registry.get_handlers()[1].get_supported_permissions.called)
         self.assertTrue(registry.get_handlers()[0].has_perm.called)
         self.assertTrue(registry.get_handlers()[1].has_perm.called)
 
     def test_has_perm_with_obj(self):
         perms = [
-            'permission.add_article',
-            'permission.change_article',
-            'permission.delete_article',
+            "permission.add_article",
+            "permission.change_article",
+            "permission.delete_article",
         ]
-        registry.get_handlers = MagicMock(return_value=[
-            MagicMock(get_supported_permissions=MagicMock(return_value=perms),
-                      has_perm=MagicMock(return_value=False)),
-            MagicMock(get_supported_permissions=MagicMock(return_value=perms),
-                      has_perm=MagicMock(return_value=True)),
-        ])
+        registry.get_handlers = MagicMock(
+            return_value=[
+                MagicMock(
+                    get_supported_permissions=MagicMock(return_value=perms),
+                    has_perm=MagicMock(return_value=False),
+                ),
+                MagicMock(
+                    get_supported_permissions=MagicMock(return_value=perms),
+                    has_perm=MagicMock(return_value=True),
+                ),
+            ]
+        )
 
         backend = PermissionBackend()
         self.assertFalse(registry.get_handlers.called)
         self.assertFalse(registry.get_handlers()[0].get_supported_permissions.called)
         self.assertFalse(registry.get_handlers()[1].get_supported_permissions.called)
         self.assertFalse(registry.get_handlers()[0].has_perm.called)
         self.assertFalse(registry.get_handlers()[1].has_perm.called)
@@ -89,92 +102,110 @@
         self.assertTrue(registry.get_handlers()[1].has_perm.called)
 
     @override_settings(
         PERMISSION_CHECK_PERMISSION_PRESENCE=False,
     )
     def test_has_perm_with_nil_permission(self):
         perms = [
-            'permission.add_article',
-            'permission.change_article',
-            'permission.delete_article',
+            "permission.add_article",
+            "permission.change_article",
+            "permission.delete_article",
         ]
-        registry.get_handlers = MagicMock(return_value=[
-            MagicMock(get_permissions=MagicMock(return_value=perms),
-                      has_perm=MagicMock(return_value=False)),
-            MagicMock(get_permissions=MagicMock(return_value=perms),
-                      has_perm=MagicMock(return_value=True)),
-        ])
+        registry.get_handlers = MagicMock(
+            return_value=[
+                MagicMock(
+                    get_permissions=MagicMock(return_value=perms),
+                    has_perm=MagicMock(return_value=False),
+                ),
+                MagicMock(
+                    get_permissions=MagicMock(return_value=perms),
+                    has_perm=MagicMock(return_value=True),
+                ),
+            ]
+        )
 
         backend = PermissionBackend()
-        self.assertFalse(backend.has_perm(None, 'permissions.nil_permission'))
+        self.assertFalse(backend.has_perm(None, "permissions.nil_permission"))
 
     @override_settings(
         PERMISSION_CHECK_PERMISSION_PRESENCE=True,
     )
     def test_has_perm_with_nil_permission_raise(self):
         perms = [
-            'permission.add_article',
-            'permission.change_article',
-            'permission.delete_article',
+            "permission.add_article",
+            "permission.change_article",
+            "permission.delete_article",
         ]
-        registry.get_handlers = MagicMock(return_value=[
-            MagicMock(get_permissions=MagicMock(return_value=perms),
-                      has_perm=MagicMock(return_value=False)),
-            MagicMock(get_permissions=MagicMock(return_value=perms),
-                      has_perm=MagicMock(return_value=True)),
-        ])
-
-        backend = PermissionBackend()
-        self.assertRaises(ObjectDoesNotExist,
-                backend.has_perm,
-                None, 'permissions.nil_permission')
+        registry.get_handlers = MagicMock(
+            return_value=[
+                MagicMock(
+                    get_permissions=MagicMock(return_value=perms),
+                    has_perm=MagicMock(return_value=False),
+                ),
+                MagicMock(
+                    get_permissions=MagicMock(return_value=perms),
+                    has_perm=MagicMock(return_value=True),
+                ),
+            ]
+        )
+
+        backend = PermissionBackend()
+        self.assertRaises(
+            ObjectDoesNotExist, backend.has_perm, None, "permissions.nil_permission"
+        )
 
     @override_settings(
         PERMISSION_CHECK_PERMISSION_PRESENCE=False,
-        AUTHENTICATION_BACKENDS = (
-            'django.contrib.auth.backends.ModelBackend',
-            'permission.backends.PermissionBackend',
+        AUTHENTICATION_BACKENDS=(
+            "django.contrib.auth.backends.ModelBackend",
+            "permission.backends.PermissionBackend",
         ),
     )
     def test_has_perm_with_nil_permission_with_user(self):
-        self.assertFalse(self.user.has_perm('permissions.nil_permission'))
+        self.assertFalse(self.user.has_perm("permissions.nil_permission"))
 
     @override_settings(
         PERMISSION_CHECK_PERMISSION_PRESENCE=True,
-        AUTHENTICATION_BACKENDS = (
-            'django.contrib.auth.backends.ModelBackend',
-            'permission.backends.PermissionBackend',
+        AUTHENTICATION_BACKENDS=(
+            "django.contrib.auth.backends.ModelBackend",
+            "permission.backends.PermissionBackend",
         ),
     )
     def test_has_perm_with_nil_permission_raise_with_user(self):
-        self.assertRaises(ObjectDoesNotExist,
-                self.user.has_perm,
-                'permissions.nil_permission')
+        self.assertRaises(
+            ObjectDoesNotExist, self.user.has_perm, "permissions.nil_permission"
+        )
 
     def test_has_module_perms(self):
         perms = [
-            'permission.add_article',
-            'permission.change_article',
-            'permission.delete_article',
+            "permission.add_article",
+            "permission.change_article",
+            "permission.delete_article",
         ]
-        app_labels = ['permission']
-        registry.get_handlers = MagicMock(return_value=[
-            MagicMock(get_supported_app_labels=MagicMock(return_value=app_labels),
-                      has_module_perms=MagicMock(return_value=False)),
-            MagicMock(get_supported_app_labels=MagicMock(return_value=app_labels),
-                      has_module_perms=MagicMock(return_value=True)),
-        ])
+        app_labels = ["permission"]
+        registry.get_handlers = MagicMock(
+            return_value=[
+                MagicMock(
+                    get_supported_app_labels=MagicMock(return_value=app_labels),
+                    has_module_perms=MagicMock(return_value=False),
+                ),
+                MagicMock(
+                    get_supported_app_labels=MagicMock(return_value=app_labels),
+                    has_module_perms=MagicMock(return_value=True),
+                ),
+            ]
+        )
 
         backend = PermissionBackend()
         self.assertFalse(registry.get_handlers.called)
         self.assertFalse(registry.get_handlers()[0].get_supported_app_labels.called)
         self.assertFalse(registry.get_handlers()[1].get_supported_app_labels.called)
         self.assertFalse(registry.get_handlers()[0].has_module_perms.called)
         self.assertFalse(registry.get_handlers()[1].has_module_perms.called)
 
-        self.assertTrue(backend.has_module_perms(self.user, 'permission'))
+        self.assertTrue(backend.has_module_perms(self.user, "permission"))
 
         self.assertTrue(registry.get_handlers.called)
         self.assertTrue(registry.get_handlers()[0].get_supported_app_labels.called)
         self.assertTrue(registry.get_handlers()[1].get_supported_app_labels.called)
         self.assertTrue(registry.get_handlers()[0].has_module_perms.called)
         self.assertTrue(registry.get_handlers()[1].has_module_perms.called)
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_decorators/test_classbase.py` & `django_permission2-2.1.0/src/permission/tests/test_decorators/test_methodbase.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-from django.test import TestCase
+# coding=utf-8
 from django.core.exceptions import PermissionDenied
+from django.test import TestCase
+
+from ...decorators.methodbase import permission_required
 from ...utils.handlers import registry
-from ...decorators.classbase import permission_required
 from ..compat import MagicMock
 from .utils import (
     create_mock_handler,
-    create_mock_request,
-    create_mock_queryset,
     create_mock_model,
-    create_mock_view_func,
+    create_mock_queryset,
+    create_mock_request,
     create_mock_view_class,
+    create_mock_view_func,
 )
 
 
 class PermissionClassDecoratorsTestCase(TestCase):
     def setUp(self):
         self.handler = create_mock_handler()
         self.request = create_mock_request(self.handler)
         self.model = create_mock_model()
         self.model_instance = self.model()
         self.queryset = create_mock_queryset(self.model_instance)
 
         self.view_func = create_mock_view_func()
-        self.view_class = permission_required(
-                'permission.add_article')(
-                    create_mock_view_class(self.view_func)
-                )
-        self.view_class_exc = permission_required(
-                'permission.add_article',
-                raise_exception=True)(
-                    create_mock_view_class(self.view_func)
-                )
+        self.view_class = create_mock_view_class(
+            permission_required("permission.add_article")(self.view_func)
+        )
+        self.view_class_exc = create_mock_view_class(
+            permission_required(
+                "permission.add_article",
+                raise_exception=True,
+            )(self.view_func)
+        )
 
         # store original registry
         self._original_registry = registry._registry
 
         # clear registry and register mock handler
         registry._registry = {}
         registry.register(
-                self.model,
-                self.handler,
-            )
+            self.model,
+            self.handler,
+        )
 
         # clear call history
         self.handler.has_perm.return_value = False
 
     def tearDown(self):
         # restore original registry
         registry._registry = self._original_registry
@@ -53,153 +55,144 @@
         # set object
         self.view_class.object = self.model_instance
         self.view_class_exc.object = self.model_instance
 
         # has_perm always return False
         self.view_class.as_view()(self.request, pk=1)
         self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertFalse(self.view_func.called)
 
-        self.assertRaises(PermissionDenied,
-                          self.view_class_exc.as_view(),
-                          self.request,
-                          pk=1)
+        self.assertRaises(
+            PermissionDenied, self.view_class_exc.as_view(), self.request, pk=1
+        )
         self.assertFalse(self.view_func.called)
 
         # has_perm always return True
         self.handler.has_perm.return_value = True
         self.view_class.as_view()(self.request, pk=1)
         self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertTrue(self.view_func.called)
 
     def test_with_get_object(self):
         # set object
-        self.view_class.get_object = MagicMock(
-                return_value=self.model_instance)
-        self.view_class_exc.get_object = MagicMock(
-                return_value=self.model_instance)
+        self.view_class.get_object = MagicMock(return_value=self.model_instance)
+        self.view_class_exc.get_object = MagicMock(return_value=self.model_instance)
 
         # has_perm always return False
         self.view_class.as_view()(self.request, pk=1)
         self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertFalse(self.view_func.called)
 
-        self.assertRaises(PermissionDenied,
-                          self.view_class_exc.as_view(),
-                          self.request,
-                          pk=1)
+        self.assertRaises(
+            PermissionDenied, self.view_class_exc.as_view(), self.request, pk=1
+        )
         self.assertFalse(self.view_func.called)
 
         # has_perm always return True
         self.handler.has_perm.return_value = True
         self.view_class.as_view()(self.request, pk=1)
         self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertTrue(self.view_func.called)
 
     def test_with_queryset(self):
         # set object
         get_object = lambda x, y: y.get(*x.args, **x.kwargs)
         self.view_class.get_object = get_object
         self.view_class_exc.get_object = get_object
         self.view_class.queryset = self.queryset
         self.view_class_exc.queryset = self.queryset
 
         # has_perm always return False
         self.view_class.as_view()(self.request, pk=1)
         self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertFalse(self.view_func.called)
 
-        self.assertRaises(PermissionDenied,
-                          self.view_class_exc.as_view(),
-                          self.request,
-                          pk=1)
+        self.assertRaises(
+            PermissionDenied, self.view_class_exc.as_view(), self.request, pk=1
+        )
         self.assertFalse(self.view_func.called)
 
         # has_perm always return True
         self.handler.has_perm.return_value = True
         self.view_class.as_view()(self.request, pk=1)
         self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertTrue(self.view_func.called)
 
     def test_with_get_queryset(self):
         # set object
         get_object = lambda x, y: y.get(*x.args, **x.kwargs)
         self.view_class.get_object = get_object
         self.view_class_exc.get_object = get_object
-        self.view_class.get_queryset = MagicMock(
-                return_value=self.queryset)
-        self.view_class_exc.get_queryset = MagicMock(
-                return_value=self.queryset)
+        self.view_class.get_queryset = MagicMock(return_value=self.queryset)
+        self.view_class_exc.get_queryset = MagicMock(return_value=self.queryset)
 
         # has_perm always return False
         self.view_class.as_view()(self.request, pk=1)
         self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertFalse(self.view_func.called)
 
-        self.assertRaises(PermissionDenied,
-                          self.view_class_exc.as_view(),
-                          self.request,
-                          pk=1)
+        self.assertRaises(
+            PermissionDenied, self.view_class_exc.as_view(), self.request, pk=1
+        )
         self.assertFalse(self.view_func.called)
 
         # has_perm always return True
         self.handler.has_perm.return_value = True
         self.view_class.as_view()(self.request, pk=1)
         self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertTrue(self.view_func.called)
-
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_decorators/test_functionbase.py` & `django_permission2-2.1.0/src/permission/tests/test_decorators/test_classbase.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,194 +1,194 @@
-# coding=utf-8
-from django.test import TestCase
 from django.core.exceptions import PermissionDenied
+from django.test import TestCase
+
+from ...decorators.classbase import permission_required
 from ...utils.handlers import registry
-from ...decorators.functionbase import permission_required
+from ..compat import MagicMock
 from .utils import (
     create_mock_handler,
+    create_mock_model,
+    create_mock_queryset,
     create_mock_request,
+    create_mock_view_class,
     create_mock_view_func,
-    create_mock_queryset,
-    create_mock_model,
 )
 
 
-class PermissionFunctionDecoratorsTestCase(TestCase):
+class PermissionClassDecoratorsTestCase(TestCase):
     def setUp(self):
         self.handler = create_mock_handler()
         self.request = create_mock_request(self.handler)
         self.model = create_mock_model()
         self.model_instance = self.model()
         self.queryset = create_mock_queryset(self.model_instance)
+
         self.view_func = create_mock_view_func()
-        self.decorated = permission_required(
-                'permission.add_article')(self.view_func)
-        self.decorated_exc = permission_required(
-                'permission.add_article', raise_exception=True)(self.view_func)
+        self.view_class = permission_required("permission.add_article")(
+            create_mock_view_class(self.view_func)
+        )
+        self.view_class_exc = permission_required(
+            "permission.add_article", raise_exception=True
+        )(create_mock_view_class(self.view_func))
 
         # store original registry
         self._original_registry = registry._registry
 
         # clear registry and register mock handler
         registry._registry = {}
         registry.register(
-                self.model,
-                self.handler,
-            )
+            self.model,
+            self.handler,
+        )
+
+        # clear call history
+        self.handler.has_perm.return_value = False
 
     def tearDown(self):
         # restore original registry
         registry._registry = self._original_registry
 
-    def test_list_detail_object_id(self):
+    def test_with_object(self):
+        # set object
+        self.view_class.object = self.model_instance
+        self.view_class_exc.object = self.model_instance
+
         # has_perm always return False
-        self.view_func.called = False
-        self.handler.has_perm.return_value = False
-        self.decorated(self.request,
-                       queryset=self.queryset,
-                       object_id=1)
-        self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.assertFalse(self.view_func.called)
-
-        self.assertRaises(PermissionDenied, self.decorated_exc,
-                          self.request, queryset=self.queryset,
-                          object_id=1)
+        self.view_class.as_view()(self.request, pk=1)
+        self.request.user.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.assertFalse(self.view_func.called)
+
+        self.assertRaises(
+            PermissionDenied, self.view_class_exc.as_view(), self.request, pk=1
+        )
         self.assertFalse(self.view_func.called)
 
         # has_perm always return True
         self.handler.has_perm.return_value = True
-        self.decorated(
-                self.request,
-                queryset=self.queryset,
-                object_id=1)
-        self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+        self.view_class.as_view()(self.request, pk=1)
+        self.request.user.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertTrue(self.view_func.called)
 
-    def test_list_detail_slug(self):
-        self.view_func.called = False
-        self.handler.has_perm.return_value = False
+    def test_with_get_object(self):
+        # set object
+        self.view_class.get_object = MagicMock(return_value=self.model_instance)
+        self.view_class_exc.get_object = MagicMock(return_value=self.model_instance)
+
         # has_perm always return False
-        self.decorated(
-                self.request,
-                queryset=self.queryset,
-                slug='permission_test_article1',
-                slug_field='title')
-        self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+        self.view_class.as_view()(self.request, pk=1)
+        self.request.user.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertFalse(self.view_func.called)
+
+        self.assertRaises(
+            PermissionDenied, self.view_class_exc.as_view(), self.request, pk=1
+        )
+        self.assertFalse(self.view_func.called)
+
         # has_perm always return True
         self.handler.has_perm.return_value = True
-        self.decorated(
-                self.request,
-                queryset=self.queryset,
-                slug='permission_test_article1',
-                slug_field='title')
-        self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+        self.view_class.as_view()(self.request, pk=1)
+        self.request.user.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertTrue(self.view_func.called)
 
-    def test_date_based_object_id(self):
-        self.view_func.called = False
-        self.handler.has_perm.return_value = False
+    def test_with_queryset(self):
+        # set object
+        get_object = lambda x, y: y.get(*x.args, **x.kwargs)
+        self.view_class.get_object = get_object
+        self.view_class_exc.get_object = get_object
+        self.view_class.queryset = self.queryset
+        self.view_class_exc.queryset = self.queryset
+
         # has_perm always return False
-        self.decorated(
-                self.request,
-                queryset=self.queryset,
-                year='2000', month='1', day='1',
-                date_field='created_at',
-                month_format='%m',
-                object_id=1)
-        self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+        self.view_class.as_view()(self.request, pk=1)
+        self.request.user.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertFalse(self.view_func.called)
+
+        self.assertRaises(
+            PermissionDenied, self.view_class_exc.as_view(), self.request, pk=1
+        )
+        self.assertFalse(self.view_func.called)
+
         # has_perm always return True
         self.handler.has_perm.return_value = True
-        self.decorated(
-                self.request,
-                queryset=self.queryset,
-                year='2000', month='1', day='1',
-                date_field='created_at',
-                month_format='%m',
-                object_id=1)
-        self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+        self.view_class.as_view()(self.request, pk=1)
+        self.request.user.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertTrue(self.view_func.called)
 
-    def test_date_based_slug(self):
-        self.view_func.called = False
-        self.handler.has_perm.return_value = False
+    def test_with_get_queryset(self):
+        # set object
+        get_object = lambda x, y: y.get(*x.args, **x.kwargs)
+        self.view_class.get_object = get_object
+        self.view_class_exc.get_object = get_object
+        self.view_class.get_queryset = MagicMock(return_value=self.queryset)
+        self.view_class_exc.get_queryset = MagicMock(return_value=self.queryset)
+
         # has_perm always return False
-        self.decorated(
-                self.request,
-                queryset=self.queryset,
-                year='2000', month='1', day='1',
-                date_field='created_at',
-                month_format='%m',
-                slug='permission_test_article1',
-                slug_field='title')
-        self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+        self.view_class.as_view()(self.request, pk=1)
+        self.request.user.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertFalse(self.view_func.called)
+
+        self.assertRaises(
+            PermissionDenied, self.view_class_exc.as_view(), self.request, pk=1
+        )
+        self.assertFalse(self.view_func.called)
+
         # has_perm always return True
         self.handler.has_perm.return_value = True
-        self.decorated(
-                self.request,
-                queryset=self.queryset,
-                year='2000', month='1', day='1',
-                date_field='created_at',
-                month_format='%m',
-                slug='permission_test_article1',
-                slug_field='title')
-        self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+        self.view_class.as_view()(self.request, pk=1)
+        self.request.user.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertTrue(self.view_func.called)
-
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_decorators/test_methodbase.py` & `django_permission2-2.1.0/src/permission/tests/test_decorators/test_functionbase.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,205 +1,207 @@
 # coding=utf-8
-from django.test import TestCase
 from django.core.exceptions import PermissionDenied
+from django.test import TestCase
+
+from ...decorators.functionbase import permission_required
 from ...utils.handlers import registry
-from ...decorators.methodbase import permission_required
-from ..compat import MagicMock
 from .utils import (
     create_mock_handler,
-    create_mock_request,
-    create_mock_queryset,
     create_mock_model,
+    create_mock_queryset,
+    create_mock_request,
     create_mock_view_func,
-    create_mock_view_class,
 )
 
 
-class PermissionClassDecoratorsTestCase(TestCase):
+class PermissionFunctionDecoratorsTestCase(TestCase):
     def setUp(self):
         self.handler = create_mock_handler()
         self.request = create_mock_request(self.handler)
         self.model = create_mock_model()
         self.model_instance = self.model()
         self.queryset = create_mock_queryset(self.model_instance)
-
         self.view_func = create_mock_view_func()
-        self.view_class = create_mock_view_class(
-            permission_required(
-                'permission.add_article')(self.view_func))
-        self.view_class_exc = create_mock_view_class(
-            permission_required(
-                'permission.add_article',
-                raise_exception=True,
-            )(self.view_func))
+        self.decorated = permission_required("permission.add_article")(self.view_func)
+        self.decorated_exc = permission_required(
+            "permission.add_article", raise_exception=True
+        )(self.view_func)
 
         # store original registry
         self._original_registry = registry._registry
 
         # clear registry and register mock handler
         registry._registry = {}
         registry.register(
-                self.model,
-                self.handler,
-            )
-
-        # clear call history
-        self.handler.has_perm.return_value = False
+            self.model,
+            self.handler,
+        )
 
     def tearDown(self):
         # restore original registry
         registry._registry = self._original_registry
 
-    def test_with_object(self):
-        # set object
-        self.view_class.object = self.model_instance
-        self.view_class_exc.object = self.model_instance
-
+    def test_list_detail_object_id(self):
         # has_perm always return False
-        self.view_class.as_view()(self.request, pk=1)
+        self.view_func.called = False
+        self.handler.has_perm.return_value = False
+        self.decorated(self.request, queryset=self.queryset, object_id=1)
         self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.assertFalse(self.view_func.called)
-
-        self.assertRaises(PermissionDenied,
-                          self.view_class_exc.as_view(),
-                          self.request,
-                          pk=1)
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.assertFalse(self.view_func.called)
+
+        self.assertRaises(
+            PermissionDenied,
+            self.decorated_exc,
+            self.request,
+            queryset=self.queryset,
+            object_id=1,
+        )
         self.assertFalse(self.view_func.called)
 
         # has_perm always return True
         self.handler.has_perm.return_value = True
-        self.view_class.as_view()(self.request, pk=1)
+        self.decorated(self.request, queryset=self.queryset, object_id=1)
         self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertTrue(self.view_func.called)
 
-    def test_with_get_object(self):
-        # set object
-        self.view_class.get_object = MagicMock(
-                return_value=self.model_instance)
-        self.view_class_exc.get_object = MagicMock(
-                return_value=self.model_instance)
-
+    def test_list_detail_slug(self):
+        self.view_func.called = False
+        self.handler.has_perm.return_value = False
         # has_perm always return False
-        self.view_class.as_view()(self.request, pk=1)
-        self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.assertFalse(self.view_func.called)
-
-        self.assertRaises(PermissionDenied,
-                          self.view_class_exc.as_view(),
-                          self.request,
-                          pk=1)
+        self.decorated(
+            self.request,
+            queryset=self.queryset,
+            slug="permission_test_article1",
+            slug_field="title",
+        )
+        self.request.user.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertFalse(self.view_func.called)
-
         # has_perm always return True
         self.handler.has_perm.return_value = True
-        self.view_class.as_view()(self.request, pk=1)
-        self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+        self.decorated(
+            self.request,
+            queryset=self.queryset,
+            slug="permission_test_article1",
+            slug_field="title",
+        )
+        self.request.user.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertTrue(self.view_func.called)
 
-    def test_with_queryset(self):
-        # set object
-        get_object = lambda x, y: y.get(*x.args, **x.kwargs)
-        self.view_class.get_object = get_object
-        self.view_class_exc.get_object = get_object
-        self.view_class.queryset = self.queryset
-        self.view_class_exc.queryset = self.queryset
-
+    def test_date_based_object_id(self):
+        self.view_func.called = False
+        self.handler.has_perm.return_value = False
         # has_perm always return False
-        self.view_class.as_view()(self.request, pk=1)
-        self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.assertFalse(self.view_func.called)
-
-        self.assertRaises(PermissionDenied,
-                          self.view_class_exc.as_view(),
-                          self.request,
-                          pk=1)
+        self.decorated(
+            self.request,
+            queryset=self.queryset,
+            year="2000",
+            month="1",
+            day="1",
+            date_field="created_at",
+            month_format="%m",
+            object_id=1,
+        )
+        self.request.user.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertFalse(self.view_func.called)
-
         # has_perm always return True
         self.handler.has_perm.return_value = True
-        self.view_class.as_view()(self.request, pk=1)
-        self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+        self.decorated(
+            self.request,
+            queryset=self.queryset,
+            year="2000",
+            month="1",
+            day="1",
+            date_field="created_at",
+            month_format="%m",
+            object_id=1,
+        )
+        self.request.user.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertTrue(self.view_func.called)
 
-    def test_with_get_queryset(self):
-        # set object
-        get_object = lambda x, y: y.get(*x.args, **x.kwargs)
-        self.view_class.get_object = get_object
-        self.view_class_exc.get_object = get_object
-        self.view_class.get_queryset = MagicMock(
-                return_value=self.queryset)
-        self.view_class_exc.get_queryset = MagicMock(
-                return_value=self.queryset)
-
+    def test_date_based_slug(self):
+        self.view_func.called = False
+        self.handler.has_perm.return_value = False
         # has_perm always return False
-        self.view_class.as_view()(self.request, pk=1)
-        self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+        self.decorated(
+            self.request,
+            queryset=self.queryset,
+            year="2000",
+            month="1",
+            day="1",
+            date_field="created_at",
+            month_format="%m",
+            slug="permission_test_article1",
+            slug_field="title",
+        )
+        self.request.user.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertFalse(self.view_func.called)
-
-        self.assertRaises(PermissionDenied,
-                          self.view_class_exc.as_view(),
-                          self.request,
-                          pk=1)
-        self.assertFalse(self.view_func.called)
-
         # has_perm always return True
         self.handler.has_perm.return_value = True
-        self.view_class.as_view()(self.request, pk=1)
-        self.request.user.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
-        self.handler.has_perm.assert_called_with(
-                'permission.add_article',
-                obj=self.model_instance,
-            )
+        self.decorated(
+            self.request,
+            queryset=self.queryset,
+            year="2000",
+            month="1",
+            day="1",
+            date_field="created_at",
+            month_format="%m",
+            slug="permission_test_article1",
+            slug_field="title",
+        )
+        self.request.user.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
+        self.handler.has_perm.assert_called_with(
+            "permission.add_article",
+            obj=self.model_instance,
+        )
         self.assertTrue(self.view_func.called)
-
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_decorators/test_permission_required.py` & `django_permission2-2.1.0/src/permission/tests/test_decorators/test_permission_required.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,76 @@
-from django.test import TestCase
-from django.http import HttpRequest
 from django.core.exceptions import PermissionDenied
-from ...utils.handlers import registry
+from django.http import HttpRequest
+from django.test import TestCase
+
+from ...decorators import permission_required as p
+from ...decorators.classbase import permission_required as c
 from ...decorators.functionbase import permission_required as f
 from ...decorators.methodbase import permission_required as m
-from ...decorators.classbase import permission_required as c
-from ...decorators import permission_required as p
+from ...utils.handlers import registry
 from ..compat import MagicMock
 from .utils import (
     create_mock_handler,
-    create_mock_request,
-    create_mock_queryset,
     create_mock_model,
-    create_mock_view_func,
+    create_mock_queryset,
+    create_mock_request,
     create_mock_view_class,
+    create_mock_view_func,
 )
 
-p = p('permission.add_article')
-c = c('permission.add_article')
-m = m('permission.add_article')
-f = f('permission.add_article')
+p = p("permission.add_article")
+c = c("permission.add_article")
+m = m("permission.add_article")
+f = f("permission.add_article")
 
 model = create_mock_model()
 instance = model()
 
 
 def view_func(request, *args, **kwargs):
     assert isinstance(request, HttpRequest)
+
+
 try:
     from django.views.generic import View as BaseView
 except ImportError:
     # Classbased generic view related test will not be run so never mind.
     BaseView = object
 
 
 class View(BaseView):
     def dispatch(self, request, *args, **kwargs):
         assert isinstance(self, View)
         assert isinstance(request, HttpRequest)
+
     def get_object(self, queryset=None):
         return instance
 
 
 class PermissionDecoratorsTestCase(TestCase):
-
     def setUp(self):
         self.handler = create_mock_handler()
         self.request = create_mock_request(self.handler)
         self.queryset = create_mock_queryset(instance)
 
         # store original registry
         self._original_registry = registry._registry
 
         # clear registry and register mock handler
         registry._registry = {}
         registry.register(
-                model,
-                self.handler,
-            )
+            model,
+            self.handler,
+        )
 
     def tearDown(self):
         # restore original registry
         registry._registry = self._original_registry
 
     def test_function_views(self):
-
         # class decorator cannot handle
         self.assertRaises(AttributeError, c, view_func)
         # method decorator can handle
         method_view = m(view_func)
         method_view(self.request, self.queryset, object_id=1)
 
         # function decorator can handle
@@ -83,29 +85,28 @@
 
         # method decorator can handle
         method_view = m(View.dispatch)
         method_view(View(), self.request, pk=1)
 
         # function decorators cannot handle
         function_view = f(View.dispatch)
-        self.assertRaises(AttributeError, function_view,
-                          View(), self.request, pk=1)
+        self.assertRaises(AttributeError, function_view, View(), self.request, pk=1)
 
     def test_class_views(self):
         # class decorator can handle
         class_view = c(View)
         class_view.as_view()(self.request, pk=1)
 
         # method decorator cannot handle
         method_view = m(View)
-        self.assertFalse(hasattr(method_view, 'as_view'))
+        self.assertFalse(hasattr(method_view, "as_view"))
 
         # function decorator cannot handle
         function_view = f(View)
-        self.assertFalse(hasattr(method_view, 'as_view'))
+        self.assertFalse(hasattr(method_view, "as_view"))
 
     def test_permission_required(self):
         # function
         functional_view = p(view_func)
         functional_view(self.request, queryset=self.queryset, object_id=1)
 
         # method
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_decorators/utils.py` & `django_permission2-2.1.0/src/permission/tests/test_decorators/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,95 @@
 # coding=utf-8
 from django.db.models import Model
-from django.http import HttpRequest
-from django.http import HttpResponse
+from django.http import HttpRequest, HttpResponse
+
 from permission.handlers import PermissionHandler
 from permission.tests.compat import MagicMock
 
 
 def create_mock_class(name, base, instance=None):
     instance = instance or MagicMock()
-    mock_class = MagicMock(name=name,
-                           return_value=instance)
+    mock_class = MagicMock(name=name, return_value=instance)
     mock_class.__bases__ = (type, base)
     mock_class.__class__ = type
     return mock_class
 
+
 def create_mock_handler():
-    instance = MagicMock(**{
-            'has_perm.return_value': False,
-            'get_permissions.return_value': [
-                'permission.add_article',
+    instance = MagicMock(
+        **{
+            "has_perm.return_value": False,
+            "get_permissions.return_value": [
+                "permission.add_article",
             ],
-        })
-    handler = create_mock_class('MockPermissionHandler',
-                                base=PermissionHandler,
-                                instance=instance)
+        }
+    )
+    handler = create_mock_class(
+        "MockPermissionHandler", base=PermissionHandler, instance=instance
+    )
     return handler
 
 
 def create_mock_request(mock_permission_handler):
     request = MagicMock(spec=HttpRequest)
     request.build_absolute_uri = MagicMock(return_value="/")
     request.META = MagicMock()
-    request.user = MagicMock(**{
-            'is_active.return_value': True,
-            'is_authenticated.return_value': True,
-            'has_perm.side_effect': mock_permission_handler.has_perm,
-        })
+    request.user = MagicMock(
+        **{
+            "is_active.return_value": True,
+            "is_authenticated.return_value": True,
+            "has_perm.side_effect": mock_permission_handler.has_perm,
+        }
+    )
     return request
 
 
 def create_mock_view_func():
     response = MagicMock(spec=HttpResponse)
     function = MagicMock(return_value=response)
     return function
 
 
 def create_mock_view_class(view_func):
     from django.views.generic import View
-    view_class = type('MockView', (View,), {})
+
+    view_class = type("MockView", (View,), {})
     view_class.dispatch = view_func
     return view_class
 
 
 def create_mock_model():
     instance = MagicMock()
-    model = MagicMock(name='MockModel')
+    model = MagicMock(name="MockModel")
     model.__bases__ = (type,)
     model.__class__ = type
-    model._meta = MagicMock(**{
-            'abstract': False,
-        })
+    model._meta = MagicMock(
+        **{
+            "abstract": False,
+        }
+    )
     return model
 
 
 def create_mock_queryset(obj):
-    from django.db.models.query import QuerySet
     from django.core.exceptions import ObjectDoesNotExist
+    from django.db.models.query import QuerySet
+
     def get_side_effect(*args, **kwargs):
-        if kwargs.get('pk', None) == 1:
+        if kwargs.get("pk", None) == 1:
             return obj
-        if kwargs.get('title', None) == 'permission_test_article1':
+        if kwargs.get("title", None) == "permission_test_article1":
             return obj
-        if kwargs.get('title__exact', None) == 'permission_test_article1':
+        if kwargs.get("title__exact", None) == "permission_test_article1":
             return obj
         raise queryset.model.DoesNotEixst
-    queryset = MagicMock(spec=QuerySet, **{
-            'get.side_effect': get_side_effect,
-        })
+
+    queryset = MagicMock(
+        spec=QuerySet,
+        **{
+            "get.side_effect": get_side_effect,
+        }
+    )
     queryset.model = MagicMock()
     queryset.model.DoesNotEixst = ObjectDoesNotExist
-    queryset.model._meta = MagicMock(object_name='MockQuerysetModel')
+    queryset.model._meta = MagicMock(object_name="MockQuerysetModel")
     return queryset
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_logics/test_author.py` & `django_permission2-2.1.0/src/permission/tests/test_logics/test_author.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 # coding=utf-8
 from django.test import TestCase, override_settings
+
 from ... import add_permission_logic
 from ...logics import AuthorPermissionLogic
-from ..utils import create_user, create_anonymous, create_article
 from ..compat import MagicMock
+from ..utils import create_anonymous, create_article, create_user
 
 
 @override_settings(
-    PERMISSION_DEFAULT_APL_FIELD_NAME='author',
+    PERMISSION_DEFAULT_APL_FIELD_NAME="author",
     PERMISSION_DEFAULT_APL_ANY_PERMISSION=True,
     PERMISSION_DEFAULT_APL_CHANGE_PERMISSION=True,
     PERMISSION_DEFAULT_APL_DELETE_PERMISSION=True,
 )
 class PermissionLogicsAuthorPermissionLogicTestCase(TestCase):
     def setUp(self):
-        self.user1 = create_user('john')
-        self.user2 = create_user('tony')
+        self.user1 = create_user("john")
+        self.user2 = create_user("tony")
         self.anonymous = create_anonymous()
-        self.perm1 = 'permission.add_article'
-        self.perm2 = 'permission.change_article'
-        self.perm3 = 'permission.delete_article'
-        self.article = create_article('test', user=self.user2)
+        self.perm1 = "permission.add_article"
+        self.perm2 = "permission.change_article"
+        self.perm3 = "permission.delete_article"
+        self.article = create_article("test", user=self.user2)
 
     def test_constructor(self):
         permission_logic = AuthorPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertTrue(isinstance(permission_logic, AuthorPermissionLogic))
-        self.assertEqual(permission_logic.field_name, 'author')
+        self.assertEqual(permission_logic.field_name, "author")
         self.assertEqual(permission_logic.any_permission, True)
         self.assertEqual(permission_logic.change_permission, True)
         self.assertEqual(permission_logic.delete_permission, True)
 
     def test_constructor_with_specifing_field_name(self):
-        permission_logic = AuthorPermissionLogic(field_name='specified')
+        permission_logic = AuthorPermissionLogic(field_name="specified")
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertTrue(isinstance(permission_logic, AuthorPermissionLogic))
-        self.assertEqual(permission_logic.field_name, 'specified')
+        self.assertEqual(permission_logic.field_name, "specified")
 
     def test_constructor_with_specifing_any_permission(self):
         permission_logic = AuthorPermissionLogic(any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertTrue(isinstance(permission_logic, AuthorPermissionLogic))
         self.assertEqual(permission_logic.any_permission, False)
 
@@ -85,134 +86,147 @@
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(permission_logic.has_perm(self.anonymous, self.perm3))
 
     def test_has_perm_add_with_obj(self):
         permission_logic = AuthorPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user1, self.perm1, self.article))
+            permission_logic.has_perm(self.user1, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj(self):
         permission_logic = AuthorPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user1, self.perm2, self.article))
+            permission_logic.has_perm(self.user1, self.perm2, self.article)
+        )
 
     def test_has_perm_delete_with_obj(self):
         permission_logic = AuthorPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user1, self.perm3, self.article))
+            permission_logic.has_perm(self.user1, self.perm3, self.article)
+        )
 
     def test_has_perm_add_with_obj_with_anonymous(self):
         permission_logic = AuthorPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-            permission_logic.has_perm(self.anonymous, self.perm1, self.article))
+            permission_logic.has_perm(self.anonymous, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj_with_anonymous(self):
         permission_logic = AuthorPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-            permission_logic.has_perm(self.anonymous, self.perm2, self.article))
+            permission_logic.has_perm(self.anonymous, self.perm2, self.article)
+        )
 
     def test_has_perm_delete_with_obj_with_anonymous(self):
         permission_logic = AuthorPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-            permission_logic.has_perm(self.anonymous, self.perm3, self.article))
+            permission_logic.has_perm(self.anonymous, self.perm3, self.article)
+        )
 
     def test_has_perm_add_with_obj_author(self):
         permission_logic = AuthorPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm1, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm1, self.article))
 
     def test_has_perm_change_with_obj_author(self):
         permission_logic = AuthorPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm2, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm2, self.article))
 
     def test_has_perm_delete_with_obj_author(self):
         permission_logic = AuthorPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm3, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm3, self.article))
 
     def test_has_perm_add_with_obj_author_diff_field_name(self):
-        permission_logic = AuthorPermissionLogic(field_name='editor')
+        permission_logic = AuthorPermissionLogic(field_name="editor")
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm1, self.article))
+            permission_logic.has_perm(self.user2, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj_author_diff_field_name(self):
-        permission_logic = AuthorPermissionLogic(field_name='editor')
+        permission_logic = AuthorPermissionLogic(field_name="editor")
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm2, self.article))
+            permission_logic.has_perm(self.user2, self.perm2, self.article)
+        )
 
     def test_has_perm_delete_with_obj_author_diff_field_name(self):
-        permission_logic = AuthorPermissionLogic(field_name='editor')
+        permission_logic = AuthorPermissionLogic(field_name="editor")
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm3, self.article))
+            permission_logic.has_perm(self.user2, self.perm3, self.article)
+        )
 
     def test_has_perm_add_with_obj_author_non_any(self):
         permission_logic = AuthorPermissionLogic(any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm1, self.article))
+            permission_logic.has_perm(self.user2, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj_author_non_any(self):
         permission_logic = AuthorPermissionLogic(any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm2, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm2, self.article))
 
     def test_has_perm_delete_with_obj_non_any(self):
         permission_logic = AuthorPermissionLogic(any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm3, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm3, self.article))
 
     def test_has_perm_add_with_obj_author_non_any_no_change(self):
-        permission_logic = AuthorPermissionLogic(any_permission=False,
-                                                 change_permission=False)
+        permission_logic = AuthorPermissionLogic(
+            any_permission=False, change_permission=False
+        )
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm1, self.article))
+            permission_logic.has_perm(self.user2, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj_author_non_any_no_change(self):
-        permission_logic = AuthorPermissionLogic(any_permission=False,
-                                                 change_permission=False)
+        permission_logic = AuthorPermissionLogic(
+            any_permission=False, change_permission=False
+        )
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm2, self.article))
+            permission_logic.has_perm(self.user2, self.perm2, self.article)
+        )
 
     def test_has_perm_delete_with_obj_non_any_no_change(self):
-        permission_logic = AuthorPermissionLogic(any_permission=False,
-                                                 change_permission=False)
+        permission_logic = AuthorPermissionLogic(
+            any_permission=False, change_permission=False
+        )
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm3, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm3, self.article))
 
     def test_has_perm_add_with_obj_author_non_any_no_delete(self):
-        permission_logic = AuthorPermissionLogic(any_permission=False,
-                                                 delete_permission=False)
+        permission_logic = AuthorPermissionLogic(
+            any_permission=False, delete_permission=False
+        )
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm1, self.article))
+            permission_logic.has_perm(self.user2, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj_author_non_any_no_delete(self):
-        permission_logic = AuthorPermissionLogic(any_permission=False,
-                                                 delete_permission=False)
+        permission_logic = AuthorPermissionLogic(
+            any_permission=False, delete_permission=False
+        )
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm2, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm2, self.article))
 
     def test_has_perm_delete_with_obj_non_any_no_delete(self):
-        permission_logic = AuthorPermissionLogic(any_permission=False,
-                                                 delete_permission=False)
+        permission_logic = AuthorPermissionLogic(
+            any_permission=False, delete_permission=False
+        )
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm3, self.article))
+            permission_logic.has_perm(self.user2, self.perm3, self.article)
+        )
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_logics/test_base.py` & `django_permission2-2.1.0/src/permission/tests/test_logics/test_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,66 @@
 # coding=utf-8
 from django.test import TestCase
+
 from ...logics import PermissionLogic
-from ..utils import create_user, create_article
+from ..utils import create_article, create_user
 
 
 class PermissionLogicsPermissionLogicTestCase(TestCase):
-
     def setUp(self):
-        self.user = create_user('john')
-        self.perm1 = 'permission.add_article'
-        self.perm2 = 'permission.change_article'
-        self.perm3 = 'permission.delete_article'
-        self.article = create_article('test')
+        self.user = create_user("john")
+        self.perm1 = "permission.add_article"
+        self.perm2 = "permission.change_article"
+        self.perm3 = "permission.delete_article"
+        self.article = create_article("test")
 
     def test_constructor(self):
         permission_logic = PermissionLogic()
         self.assertTrue(isinstance(permission_logic, PermissionLogic))
 
     def test_has_perm_add_wihtout_obj(self):
         permission_logic = PermissionLogic()
-        self.assertRaises(NotImplementedError,
-                          permission_logic.has_perm,
-                          self.user, self.perm1)
+        self.assertRaises(
+            NotImplementedError, permission_logic.has_perm, self.user, self.perm1
+        )
 
     def test_has_perm_change_wihtout_obj(self):
         permission_logic = PermissionLogic()
-        self.assertRaises(NotImplementedError,
-                          permission_logic.has_perm,
-                          self.user, self.perm2)
+        self.assertRaises(
+            NotImplementedError, permission_logic.has_perm, self.user, self.perm2
+        )
 
     def test_has_perm_delete_wihtout_obj(self):
         permission_logic = PermissionLogic()
-        self.assertRaises(NotImplementedError,
-                          permission_logic.has_perm,
-                          self.user, self.perm3)
+        self.assertRaises(
+            NotImplementedError, permission_logic.has_perm, self.user, self.perm3
+        )
 
     def test_has_perm_add_wiht_obj(self):
         permission_logic = PermissionLogic()
-        self.assertRaises(NotImplementedError,
-                          permission_logic.has_perm,
-                          self.user, self.perm1, self.article)
+        self.assertRaises(
+            NotImplementedError,
+            permission_logic.has_perm,
+            self.user,
+            self.perm1,
+            self.article,
+        )
 
     def test_has_perm_change_wiht_obj(self):
         permission_logic = PermissionLogic()
-        self.assertRaises(NotImplementedError,
-                          permission_logic.has_perm,
-                          self.user, self.perm2, self.article)
+        self.assertRaises(
+            NotImplementedError,
+            permission_logic.has_perm,
+            self.user,
+            self.perm2,
+            self.article,
+        )
 
     def test_has_perm_delete_wiht_obj(self):
         permission_logic = PermissionLogic()
-        self.assertRaises(NotImplementedError,
-                          permission_logic.has_perm,
-                          self.user, self.perm3, self.article)
+        self.assertRaises(
+            NotImplementedError,
+            permission_logic.has_perm,
+            self.user,
+            self.perm3,
+            self.article,
+        )
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_logics/test_collaborators.py` & `django_permission2-2.1.0/src/permission/tests/test_logics/test_collaborators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 from django.test import TestCase, override_settings
+
 from ... import add_permission_logic
 from ...logics import CollaboratorsPermissionLogic
-from ..utils import create_user, create_anonymous, create_article
 from ..compat import MagicMock
+from ..utils import create_anonymous, create_article, create_user
 
 
 @override_settings(
-    PERMISSION_DEFAULT_CPL_FIELD_NAME='authors',
+    PERMISSION_DEFAULT_CPL_FIELD_NAME="authors",
     PERMISSION_DEFAULT_CPL_ANY_PERMISSION=True,
     PERMISSION_DEFAULT_CPL_CHANGE_PERMISSION=True,
     PERMISSION_DEFAULT_CPL_DELETE_PERMISSION=True,
 )
 class PermissionLogicsCollaboratorsPermissionLogicTestCase(TestCase):
     def setUp(self):
-        self.user1 = create_user('john')
-        self.user2 = create_user('tony')
+        self.user1 = create_user("john")
+        self.user2 = create_user("tony")
         self.anonymous = create_anonymous()
-        self.perm1 = 'permission.add_article'
-        self.perm2 = 'permission.change_article'
-        self.perm3 = 'permission.delete_article'
-        self.article = create_article('test')
+        self.perm1 = "permission.add_article"
+        self.perm2 = "permission.change_article"
+        self.perm3 = "permission.delete_article"
+        self.article = create_article("test")
         self.article.authors.add(self.user2)
 
     def test_constructor(self):
         permission_logic = CollaboratorsPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertTrue(isinstance(permission_logic, CollaboratorsPermissionLogic))
-        self.assertEqual(permission_logic.field_name, 'authors')
+        self.assertEqual(permission_logic.field_name, "authors")
         self.assertEqual(permission_logic.any_permission, True)
         self.assertEqual(permission_logic.change_permission, True)
         self.assertEqual(permission_logic.delete_permission, True)
 
     def test_constructor_with_specifing_field_name(self):
-        permission_logic = CollaboratorsPermissionLogic(field_name='specified')
+        permission_logic = CollaboratorsPermissionLogic(field_name="specified")
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertTrue(isinstance(permission_logic, CollaboratorsPermissionLogic))
-        self.assertEqual(permission_logic.field_name, 'specified')
+        self.assertEqual(permission_logic.field_name, "specified")
 
     def test_constructor_with_specifing_any_permission(self):
         permission_logic = CollaboratorsPermissionLogic(any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertTrue(isinstance(permission_logic, CollaboratorsPermissionLogic))
         self.assertEqual(permission_logic.any_permission, False)
 
@@ -70,27 +71,30 @@
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertTrue(permission_logic.has_perm(self.user1, self.perm3))
 
     def test_has_perm_add_with_obj(self):
         permission_logic = CollaboratorsPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user1, self.perm1, self.article))
+            permission_logic.has_perm(self.user1, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj(self):
         permission_logic = CollaboratorsPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user1, self.perm2, self.article))
+            permission_logic.has_perm(self.user1, self.perm2, self.article)
+        )
 
     def test_has_perm_delete_with_obj(self):
         permission_logic = CollaboratorsPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user1, self.perm3, self.article))
+            permission_logic.has_perm(self.user1, self.perm3, self.article)
+        )
 
     def test_has_perm_add_without_obj_with_anonymous(self):
         permission_logic = CollaboratorsPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(permission_logic.has_perm(self.anonymous, self.perm1))
 
     def test_has_perm_change_without_obj_with_anonymous(self):
@@ -103,116 +107,126 @@
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(permission_logic.has_perm(self.anonymous, self.perm3))
 
     def test_has_perm_add_with_obj_with_anonymous(self):
         permission_logic = CollaboratorsPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-            permission_logic.has_perm(self.anonymous, self.perm1, self.article))
+            permission_logic.has_perm(self.anonymous, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj_with_anonymous(self):
         permission_logic = CollaboratorsPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-            permission_logic.has_perm(self.anonymous, self.perm2, self.article))
+            permission_logic.has_perm(self.anonymous, self.perm2, self.article)
+        )
 
     def test_has_perm_delete_with_obj_with_anonymous(self):
         permission_logic = CollaboratorsPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-            permission_logic.has_perm(self.anonymous, self.perm3, self.article))
+            permission_logic.has_perm(self.anonymous, self.perm3, self.article)
+        )
 
     def test_has_perm_add_with_obj_collaborators(self):
         permission_logic = CollaboratorsPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm1, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm1, self.article))
 
     def test_has_perm_change_with_obj_collaborators(self):
         permission_logic = CollaboratorsPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm2, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm2, self.article))
 
     def test_has_perm_delete_with_obj_collaborators(self):
         permission_logic = CollaboratorsPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm3, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm3, self.article))
 
     def test_has_perm_add_with_obj_collaborators_diff_field_name(self):
-        permission_logic = CollaboratorsPermissionLogic(field_name='editors')
+        permission_logic = CollaboratorsPermissionLogic(field_name="editors")
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm1, self.article))
+            permission_logic.has_perm(self.user2, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj_collaborators_diff_field_name(self):
-        permission_logic = CollaboratorsPermissionLogic(field_name='editors')
+        permission_logic = CollaboratorsPermissionLogic(field_name="editors")
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm2, self.article))
+            permission_logic.has_perm(self.user2, self.perm2, self.article)
+        )
 
     def test_has_perm_delete_with_obj_collaborators_diff_field_name(self):
-        permission_logic = CollaboratorsPermissionLogic(field_name='editors')
+        permission_logic = CollaboratorsPermissionLogic(field_name="editors")
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm3, self.article))
+            permission_logic.has_perm(self.user2, self.perm3, self.article)
+        )
 
     def test_has_perm_add_with_obj_collaborators_non_any(self):
         permission_logic = CollaboratorsPermissionLogic(any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm1, self.article))
+            permission_logic.has_perm(self.user2, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj_collaborators_non_any(self):
         permission_logic = CollaboratorsPermissionLogic(any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm2, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm2, self.article))
 
     def test_has_perm_delete_with_obj_non_any(self):
         permission_logic = CollaboratorsPermissionLogic(any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm3, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm3, self.article))
 
     def test_has_perm_add_with_obj_collaborators_non_any_no_change(self):
-        permission_logic = CollaboratorsPermissionLogic(any_permission=False,
-                                                 change_permission=False)
+        permission_logic = CollaboratorsPermissionLogic(
+            any_permission=False, change_permission=False
+        )
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm1, self.article))
+            permission_logic.has_perm(self.user2, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj_collaborators_non_any_no_change(self):
-        permission_logic = CollaboratorsPermissionLogic(any_permission=False,
-                                                 change_permission=False)
+        permission_logic = CollaboratorsPermissionLogic(
+            any_permission=False, change_permission=False
+        )
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm2, self.article))
+            permission_logic.has_perm(self.user2, self.perm2, self.article)
+        )
 
     def test_has_perm_delete_with_obj_non_any_no_change(self):
-        permission_logic = CollaboratorsPermissionLogic(any_permission=False,
-                                                 change_permission=False)
+        permission_logic = CollaboratorsPermissionLogic(
+            any_permission=False, change_permission=False
+        )
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm3, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm3, self.article))
 
     def test_has_perm_add_with_obj_collaborators_non_any_no_delete(self):
-        permission_logic = CollaboratorsPermissionLogic(any_permission=False,
-                                                 delete_permission=False)
+        permission_logic = CollaboratorsPermissionLogic(
+            any_permission=False, delete_permission=False
+        )
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm1, self.article))
+            permission_logic.has_perm(self.user2, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj_collaborators_non_any_no_delete(self):
-        permission_logic = CollaboratorsPermissionLogic(any_permission=False,
-                                                 delete_permission=False)
+        permission_logic = CollaboratorsPermissionLogic(
+            any_permission=False, delete_permission=False
+        )
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm2, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm2, self.article))
 
     def test_has_perm_delete_with_obj_non_any_no_delete(self):
-        permission_logic = CollaboratorsPermissionLogic(any_permission=False,
-                                                 delete_permission=False)
+        permission_logic = CollaboratorsPermissionLogic(
+            any_permission=False, delete_permission=False
+        )
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm3, self.article))
+            permission_logic.has_perm(self.user2, self.perm3, self.article)
+        )
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_logics/test_groupin.py` & `django_permission2-2.1.0/src/permission/tests/test_logics/test_groupin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,278 +1,284 @@
 # coding=utf-8
 from django.test import TestCase, override_settings
+
 from ...logics import GroupInPermissionLogic
 from ...utils.logics import add_permission_logic
-from ..utils import create_user, create_anonymous, create_group, create_article
 from ..compat import MagicMock
+from ..utils import create_anonymous, create_article, create_group, create_user
 
 
 @override_settings(
     PERMISSION_DEFAULT_GIPL_ANY_PERMISSION=True,
     PERMISSION_DEFAULT_GIPL_ADD_PERMISSION=True,
     PERMISSION_DEFAULT_GIPL_CHANGE_PERMISSION=True,
     PERMISSION_DEFAULT_GIPL_DELETE_PERMISSION=True,
 )
 class PermissionLogicsAuthorPermissionLogicTestCase(TestCase):
     def setUp(self):
-        self.user1 = create_user('john')
-        self.user2 = create_user('tony')
-        self.user3 = create_user('peter')
+        self.user1 = create_user("john")
+        self.user2 = create_user("tony")
+        self.user3 = create_user("peter")
         self.anonymous = create_anonymous()
-        self.group1 = create_group('admin', self.user1)
-        self.group2 = create_group('staff', self.user2)
-        self.perm1 = 'permission.add_article'
-        self.perm2 = 'permission.change_article'
-        self.perm3 = 'permission.delete_article'
-        self.article = create_article('test')
+        self.group1 = create_group("admin", self.user1)
+        self.group2 = create_group("staff", self.user2)
+        self.perm1 = "permission.add_article"
+        self.perm2 = "permission.change_article"
+        self.perm3 = "permission.delete_article"
+        self.article = create_article("test")
 
     def test_constructor(self):
-        permission_logic = GroupInPermissionLogic('admin')
+        permission_logic = GroupInPermissionLogic("admin")
         add_permission_logic(self.article.__class__, permission_logic)
 
         self.assertTrue(isinstance(permission_logic, GroupInPermissionLogic))
-        self.assertEqual(permission_logic.group_names, ['admin'])
+        self.assertEqual(permission_logic.group_names, ["admin"])
         self.assertEqual(permission_logic.any_permission, True)
         self.assertEqual(permission_logic.add_permission, True)
         self.assertEqual(permission_logic.change_permission, True)
         self.assertEqual(permission_logic.delete_permission, True)
 
-        permission_logic = GroupInPermissionLogic(['admin', 'staff'])
+        permission_logic = GroupInPermissionLogic(["admin", "staff"])
         self.assertTrue(isinstance(permission_logic, GroupInPermissionLogic))
-        self.assertEqual(permission_logic.group_names, ['admin', 'staff'])
+        self.assertEqual(permission_logic.group_names, ["admin", "staff"])
         self.assertEqual(permission_logic.any_permission, True)
         self.assertEqual(permission_logic.add_permission, True)
         self.assertEqual(permission_logic.change_permission, True)
         self.assertEqual(permission_logic.delete_permission, True)
 
     def test_constructor_with_specifing_any_permission(self):
-        permission_logic = GroupInPermissionLogic('admin', any_permission=False)
+        permission_logic = GroupInPermissionLogic("admin", any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
 
         self.assertTrue(isinstance(permission_logic, GroupInPermissionLogic))
         self.assertEqual(permission_logic.any_permission, False)
 
     def test_constructor_with_specifing_add_permission(self):
-        permission_logic = GroupInPermissionLogic('admin', add_permission=False)
+        permission_logic = GroupInPermissionLogic("admin", add_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
 
         self.assertTrue(isinstance(permission_logic, GroupInPermissionLogic))
         self.assertEqual(permission_logic.add_permission, False)
 
     def test_constructor_with_specifing_change_permission(self):
-        permission_logic = GroupInPermissionLogic('admin', change_permission=False)
+        permission_logic = GroupInPermissionLogic("admin", change_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
 
         self.assertTrue(isinstance(permission_logic, GroupInPermissionLogic))
         self.assertEqual(permission_logic.change_permission, False)
 
     def test_constructor_with_specifing_delete_permission(self):
-        permission_logic = GroupInPermissionLogic('admin', delete_permission=False)
+        permission_logic = GroupInPermissionLogic("admin", delete_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
 
         self.assertTrue(isinstance(permission_logic, GroupInPermissionLogic))
         self.assertEqual(permission_logic.delete_permission, False)
 
     def test_has_perm_add_without_obj(self):
-        permission_logic = GroupInPermissionLogic('admin')
+        permission_logic = GroupInPermissionLogic("admin")
         add_permission_logic(self.article.__class__, permission_logic)
 
         self.assertTrue(permission_logic.has_perm(self.user1, self.perm1))
         self.assertFalse(permission_logic.has_perm(self.user2, self.perm1))
         self.assertFalse(permission_logic.has_perm(self.user3, self.perm1))
 
     def test_has_perm_change_without_obj(self):
-        permission_logic = GroupInPermissionLogic('admin')
+        permission_logic = GroupInPermissionLogic("admin")
         add_permission_logic(self.article.__class__, permission_logic)
 
         self.assertTrue(permission_logic.has_perm(self.user1, self.perm2))
         self.assertFalse(permission_logic.has_perm(self.user2, self.perm2))
         self.assertFalse(permission_logic.has_perm(self.user3, self.perm2))
 
     def test_has_perm_delete_without_obj(self):
-        permission_logic = GroupInPermissionLogic('admin')
+        permission_logic = GroupInPermissionLogic("admin")
         add_permission_logic(self.article.__class__, permission_logic)
 
         self.assertTrue(permission_logic.has_perm(self.user1, self.perm3))
         self.assertFalse(permission_logic.has_perm(self.user2, self.perm3))
         self.assertFalse(permission_logic.has_perm(self.user3, self.perm3))
 
     def test_has_perm_add_with_obj(self):
-        permission_logic = GroupInPermissionLogic('admin')
+        permission_logic = GroupInPermissionLogic("admin")
         add_permission_logic(self.article.__class__, permission_logic)
 
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm1, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm1, self.article))
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm1, self.article))
+            permission_logic.has_perm(self.user2, self.perm1, self.article)
+        )
         self.assertFalse(
-                permission_logic.has_perm(self.user3, self.perm1, self.article))
+            permission_logic.has_perm(self.user3, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj(self):
-        permission_logic = GroupInPermissionLogic('admin')
+        permission_logic = GroupInPermissionLogic("admin")
         add_permission_logic(self.article.__class__, permission_logic)
 
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm2, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm2, self.article))
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm2, self.article))
+            permission_logic.has_perm(self.user2, self.perm2, self.article)
+        )
         self.assertFalse(
-                permission_logic.has_perm(self.user3, self.perm2, self.article))
+            permission_logic.has_perm(self.user3, self.perm2, self.article)
+        )
 
     def test_has_perm_delete_with_obj(self):
-        permission_logic = GroupInPermissionLogic('admin')
+        permission_logic = GroupInPermissionLogic("admin")
         add_permission_logic(self.article.__class__, permission_logic)
 
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm3, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm3, self.article))
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm3, self.article))
+            permission_logic.has_perm(self.user2, self.perm3, self.article)
+        )
         self.assertFalse(
-                permission_logic.has_perm(self.user3, self.perm3, self.article))
+            permission_logic.has_perm(self.user3, self.perm3, self.article)
+        )
 
     def test_has_perm_add_without_obj_with_anonymous(self):
-        permission_logic = GroupInPermissionLogic('admin')
+        permission_logic = GroupInPermissionLogic("admin")
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(permission_logic.has_perm(self.anonymous, self.perm1))
 
     def test_has_perm_change_without_obj_with_anonymous(self):
-        permission_logic = GroupInPermissionLogic('admin')
+        permission_logic = GroupInPermissionLogic("admin")
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(permission_logic.has_perm(self.anonymous, self.perm2))
 
     def test_has_perm_delete_without_obj_with_anonymous(self):
-        permission_logic = GroupInPermissionLogic('admin')
+        permission_logic = GroupInPermissionLogic("admin")
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(permission_logic.has_perm(self.anonymous, self.perm3))
 
     def test_has_perm_add_with_obj_with_anonymous(self):
-        permission_logic = GroupInPermissionLogic('admin')
+        permission_logic = GroupInPermissionLogic("admin")
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-            permission_logic.has_perm(self.anonymous, self.perm1, self.article))
+            permission_logic.has_perm(self.anonymous, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj_with_anonymous(self):
-        permission_logic = GroupInPermissionLogic('admin')
+        permission_logic = GroupInPermissionLogic("admin")
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-            permission_logic.has_perm(self.anonymous, self.perm2, self.article))
+            permission_logic.has_perm(self.anonymous, self.perm2, self.article)
+        )
 
     def test_has_perm_delete_with_obj_with_anonymous(self):
-        permission_logic = GroupInPermissionLogic('admin')
+        permission_logic = GroupInPermissionLogic("admin")
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-            permission_logic.has_perm(self.anonymous, self.perm3, self.article))
+            permission_logic.has_perm(self.anonymous, self.perm3, self.article)
+        )
 
     def test_has_perm_add_without_obj_with_two_groups(self):
-        permission_logic = GroupInPermissionLogic(['admin', 'staff'])
+        permission_logic = GroupInPermissionLogic(["admin", "staff"])
         add_permission_logic(self.article.__class__, permission_logic)
 
         self.assertTrue(permission_logic.has_perm(self.user1, self.perm1))
         self.assertTrue(permission_logic.has_perm(self.user2, self.perm1))
         self.assertFalse(permission_logic.has_perm(self.user3, self.perm1))
 
     def test_has_perm_change_without_obj_with_two_groups(self):
-        permission_logic = GroupInPermissionLogic(['admin', 'staff'])
+        permission_logic = GroupInPermissionLogic(["admin", "staff"])
         add_permission_logic(self.article.__class__, permission_logic)
 
         self.assertTrue(permission_logic.has_perm(self.user1, self.perm2))
         self.assertTrue(permission_logic.has_perm(self.user2, self.perm2))
         self.assertFalse(permission_logic.has_perm(self.user3, self.perm2))
 
     def test_has_perm_delete_without_obj_with_two_groups(self):
-        permission_logic = GroupInPermissionLogic(['admin', 'staff'])
+        permission_logic = GroupInPermissionLogic(["admin", "staff"])
         add_permission_logic(self.article.__class__, permission_logic)
 
         self.assertTrue(permission_logic.has_perm(self.user1, self.perm3))
         self.assertTrue(permission_logic.has_perm(self.user2, self.perm3))
         self.assertFalse(permission_logic.has_perm(self.user3, self.perm3))
 
     def test_has_perm_add_with_obj_with_two_groups(self):
-        permission_logic = GroupInPermissionLogic(['admin', 'staff'])
+        permission_logic = GroupInPermissionLogic(["admin", "staff"])
         add_permission_logic(self.article.__class__, permission_logic)
 
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm1, self.article))
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm1, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm1, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm1, self.article))
         self.assertFalse(
-                permission_logic.has_perm(self.user3, self.perm1, self.article))
+            permission_logic.has_perm(self.user3, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj_with_two_groups(self):
-        permission_logic = GroupInPermissionLogic(['admin', 'staff'])
+        permission_logic = GroupInPermissionLogic(["admin", "staff"])
         add_permission_logic(self.article.__class__, permission_logic)
 
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm2, self.article))
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm2, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm2, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm2, self.article))
         self.assertFalse(
-                permission_logic.has_perm(self.user3, self.perm2, self.article))
+            permission_logic.has_perm(self.user3, self.perm2, self.article)
+        )
 
     def test_has_perm_delete_with_obj_with_two_groups(self):
-        permission_logic = GroupInPermissionLogic(['admin', 'staff'])
+        permission_logic = GroupInPermissionLogic(["admin", "staff"])
         add_permission_logic(self.article.__class__, permission_logic)
 
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm3, self.article))
-        self.assertTrue(
-                permission_logic.has_perm(self.user2, self.perm3, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm3, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user2, self.perm3, self.article))
         self.assertFalse(
-                permission_logic.has_perm(self.user3, self.perm3, self.article))
+            permission_logic.has_perm(self.user3, self.perm3, self.article)
+        )
 
     def test_has_perm_add_without_obj_without_any_permission(self):
-        permission_logic = GroupInPermissionLogic('admin', any_permission=False)
+        permission_logic = GroupInPermissionLogic("admin", any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
 
         self.assertTrue(permission_logic.has_perm(self.user1, self.perm1))
         self.assertFalse(permission_logic.has_perm(self.user2, self.perm1))
         self.assertFalse(permission_logic.has_perm(self.user3, self.perm1))
 
     def test_has_perm_change_without_obj_without_any_permission(self):
-        permission_logic = GroupInPermissionLogic('admin', any_permission=False)
+        permission_logic = GroupInPermissionLogic("admin", any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
 
         self.assertTrue(permission_logic.has_perm(self.user1, self.perm2))
         self.assertFalse(permission_logic.has_perm(self.user2, self.perm2))
         self.assertFalse(permission_logic.has_perm(self.user3, self.perm2))
 
     def test_has_perm_delete_without_obj_without_any_permission(self):
-        permission_logic = GroupInPermissionLogic('admin', any_permission=False)
+        permission_logic = GroupInPermissionLogic("admin", any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
 
         self.assertTrue(permission_logic.has_perm(self.user1, self.perm3))
         self.assertFalse(permission_logic.has_perm(self.user2, self.perm3))
         self.assertFalse(permission_logic.has_perm(self.user3, self.perm3))
 
     def test_has_perm_add_with_obj_without_any_permission(self):
-        permission_logic = GroupInPermissionLogic('admin', any_permission=False)
+        permission_logic = GroupInPermissionLogic("admin", any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
 
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm1, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm1, self.article))
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm1, self.article))
+            permission_logic.has_perm(self.user2, self.perm1, self.article)
+        )
         self.assertFalse(
-                permission_logic.has_perm(self.user3, self.perm1, self.article))
+            permission_logic.has_perm(self.user3, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj_without_any_permission(self):
-        permission_logic = GroupInPermissionLogic('admin', any_permission=False)
+        permission_logic = GroupInPermissionLogic("admin", any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
 
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm2, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm2, self.article))
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm2, self.article))
+            permission_logic.has_perm(self.user2, self.perm2, self.article)
+        )
         self.assertFalse(
-                permission_logic.has_perm(self.user3, self.perm2, self.article))
+            permission_logic.has_perm(self.user3, self.perm2, self.article)
+        )
 
     def test_has_perm_delete_with_obj_without_any_permission(self):
-        permission_logic = GroupInPermissionLogic('admin', any_permission=False)
+        permission_logic = GroupInPermissionLogic("admin", any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
 
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm3, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm3, self.article))
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm3, self.article))
+            permission_logic.has_perm(self.user2, self.perm3, self.article)
+        )
         self.assertFalse(
-                permission_logic.has_perm(self.user3, self.perm3, self.article))
-
+            permission_logic.has_perm(self.user3, self.perm3, self.article)
+        )
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_logics/test_oneself.py` & `django_permission2-2.1.0/src/permission/tests/test_logics/test_oneself.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # coding=utf-8
 from django.test import TestCase, override_settings
+
 from ... import add_permission_logic
 from ...logics import OneselfPermissionLogic
-from ..utils import create_user, create_anonymous, create_article
 from ..compat import MagicMock
+from ..utils import create_anonymous, create_article, create_user
 
 
 @override_settings(
     PERMISSION_DEFAULT_OSPL_ANY_PERMISSION=True,
     PERMISSION_DEFAULT_OSPL_CHANGE_PERMISSION=True,
     PERMISSION_DEFAULT_OSPL_DELETE_PERMISSION=True,
 )
 class PermissionLogicsOneselfPermissionLogicTestCase(TestCase):
     def setUp(self):
-        self.user1 = create_user('john')
-        self.user2 = create_user('tony')
+        self.user1 = create_user("john")
+        self.user2 = create_user("tony")
         self.anonymous = create_anonymous()
-        self.perm1 = 'auth.add_user'
-        self.perm2 = 'auth.change_user'
-        self.perm3 = 'auth.delete_user'
+        self.perm1 = "auth.add_user"
+        self.perm2 = "auth.change_user"
+        self.perm3 = "auth.delete_user"
 
     def test_constructor(self):
         permission_logic = OneselfPermissionLogic()
         add_permission_logic(self.user1.__class__, permission_logic)
         self.assertTrue(isinstance(permission_logic, OneselfPermissionLogic))
         self.assertEqual(permission_logic.any_permission, True)
         self.assertEqual(permission_logic.change_permission, True)
@@ -75,117 +76,111 @@
         permission_logic = OneselfPermissionLogic()
         add_permission_logic(self.user1.__class__, permission_logic)
         self.assertFalse(permission_logic.has_perm(self.anonymous, self.perm3))
 
     def test_has_perm_add_with_obj(self):
         permission_logic = OneselfPermissionLogic()
         add_permission_logic(self.user1.__class__, permission_logic)
-        self.assertFalse(
-                permission_logic.has_perm(self.user1, self.perm1, self.user2))
+        self.assertFalse(permission_logic.has_perm(self.user1, self.perm1, self.user2))
 
     def test_has_perm_change_with_obj(self):
         permission_logic = OneselfPermissionLogic()
         add_permission_logic(self.user1.__class__, permission_logic)
-        self.assertFalse(
-                permission_logic.has_perm(self.user1, self.perm2, self.user2))
+        self.assertFalse(permission_logic.has_perm(self.user1, self.perm2, self.user2))
 
     def test_has_perm_delete_with_obj(self):
         permission_logic = OneselfPermissionLogic()
         add_permission_logic(self.user1.__class__, permission_logic)
-        self.assertFalse(
-                permission_logic.has_perm(self.user1, self.perm3, self.user2))
+        self.assertFalse(permission_logic.has_perm(self.user1, self.perm3, self.user2))
 
     def test_has_perm_add_with_obj_with_anonymous(self):
         permission_logic = OneselfPermissionLogic()
         add_permission_logic(self.user1.__class__, permission_logic)
         self.assertFalse(
-            permission_logic.has_perm(self.anonymous, self.perm1, self.user1))
+            permission_logic.has_perm(self.anonymous, self.perm1, self.user1)
+        )
 
     def test_has_perm_change_with_obj_with_anonymous(self):
         permission_logic = OneselfPermissionLogic()
         add_permission_logic(self.user1.__class__, permission_logic)
         self.assertFalse(
-            permission_logic.has_perm(self.anonymous, self.perm2, self.user1))
+            permission_logic.has_perm(self.anonymous, self.perm2, self.user1)
+        )
 
     def test_has_perm_delete_with_obj_with_anonymous(self):
         permission_logic = OneselfPermissionLogic()
         add_permission_logic(self.user1.__class__, permission_logic)
         self.assertFalse(
-            permission_logic.has_perm(self.anonymous, self.perm3, self.user1))
+            permission_logic.has_perm(self.anonymous, self.perm3, self.user1)
+        )
 
     def test_has_perm_add_with_himself(self):
         permission_logic = OneselfPermissionLogic()
         add_permission_logic(self.user1.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm1, self.user1))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm1, self.user1))
 
     def test_has_perm_change_with_himself(self):
         permission_logic = OneselfPermissionLogic()
         add_permission_logic(self.user1.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm2, self.user1))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm2, self.user1))
 
     def test_has_perm_delete_with_himself(self):
         permission_logic = OneselfPermissionLogic()
         add_permission_logic(self.user1.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm3, self.user1))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm3, self.user1))
 
     def test_has_perm_add_with_himself_non_any(self):
         permission_logic = OneselfPermissionLogic(any_permission=False)
         add_permission_logic(self.user1.__class__, permission_logic)
-        self.assertFalse(
-                permission_logic.has_perm(self.user1, self.perm1, self.user1))
+        self.assertFalse(permission_logic.has_perm(self.user1, self.perm1, self.user1))
 
     def test_has_perm_change_with_himself_non_any(self):
         permission_logic = OneselfPermissionLogic(any_permission=False)
         add_permission_logic(self.user1.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm2, self.user1))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm2, self.user1))
 
     def test_has_perm_delete_with_obj_non_any(self):
         permission_logic = OneselfPermissionLogic(any_permission=False)
         add_permission_logic(self.user1.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm3, self.user1))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm3, self.user1))
 
     def test_has_perm_add_with_himself_non_any_no_change(self):
-        permission_logic = OneselfPermissionLogic(any_permission=False,
-                                                 change_permission=False)
+        permission_logic = OneselfPermissionLogic(
+            any_permission=False, change_permission=False
+        )
         add_permission_logic(self.user1.__class__, permission_logic)
-        self.assertFalse(
-                permission_logic.has_perm(self.user1, self.perm1, self.user1))
+        self.assertFalse(permission_logic.has_perm(self.user1, self.perm1, self.user1))
 
     def test_has_perm_change_with_himself_non_any_no_change(self):
-        permission_logic = OneselfPermissionLogic(any_permission=False,
-                                                 change_permission=False)
+        permission_logic = OneselfPermissionLogic(
+            any_permission=False, change_permission=False
+        )
         add_permission_logic(self.user1.__class__, permission_logic)
-        self.assertFalse(
-                permission_logic.has_perm(self.user1, self.perm2, self.user1))
+        self.assertFalse(permission_logic.has_perm(self.user1, self.perm2, self.user1))
 
     def test_has_perm_delete_with_himself_non_any_no_change(self):
-        permission_logic = OneselfPermissionLogic(any_permission=False,
-                                                 change_permission=False)
+        permission_logic = OneselfPermissionLogic(
+            any_permission=False, change_permission=False
+        )
         add_permission_logic(self.user1.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm3, self.user1))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm3, self.user1))
 
     def test_has_perm_add_with_himself_non_any_no_delete(self):
-        permission_logic = OneselfPermissionLogic(any_permission=False,
-                                                 delete_permission=False)
+        permission_logic = OneselfPermissionLogic(
+            any_permission=False, delete_permission=False
+        )
         add_permission_logic(self.user1.__class__, permission_logic)
-        self.assertFalse(
-                permission_logic.has_perm(self.user1, self.perm1, self.user1))
+        self.assertFalse(permission_logic.has_perm(self.user1, self.perm1, self.user1))
 
     def test_has_perm_change_with_himself_non_any_no_delete(self):
-        permission_logic = OneselfPermissionLogic(any_permission=False,
-                                                 delete_permission=False)
+        permission_logic = OneselfPermissionLogic(
+            any_permission=False, delete_permission=False
+        )
         add_permission_logic(self.user1.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm2, self.user1))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm2, self.user1))
 
     def test_has_perm_delete_with_himself_non_any_no_delete(self):
-        permission_logic = OneselfPermissionLogic(any_permission=False,
-                                                 delete_permission=False)
+        permission_logic = OneselfPermissionLogic(
+            any_permission=False, delete_permission=False
+        )
         add_permission_logic(self.user1.__class__, permission_logic)
-        self.assertFalse(
-                permission_logic.has_perm(self.user1, self.perm3, self.user1))
+        self.assertFalse(permission_logic.has_perm(self.user1, self.perm3, self.user1))
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_logics/test_staff.py` & `django_permission2-2.1.0/src/permission/tests/test_logics/test_staff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # coding=utf-8
 from django.test import TestCase, override_settings
+
 from ...logics import StaffPermissionLogic
 from ...utils.logics import add_permission_logic
-from ..utils import create_user, create_anonymous, create_article
+from ..utils import create_anonymous, create_article, create_user
 
 
 @override_settings(
     PERMISSION_DEFAULT_SPL_ANY_PERMISSION=True,
     PERMISSION_DEFAULT_SPL_ADD_PERMISSION=True,
     PERMISSION_DEFAULT_SPL_CHANGE_PERMISSION=True,
     PERMISSION_DEFAULT_SPL_DELETE_PERMISSION=True,
 )
 class PermissionLogicsStaffPermissionLogicTestCase(TestCase):
     def setUp(self):
-        self.user1 = create_user('john', is_staff=True)
-        self.user2 = create_user('tony')
+        self.user1 = create_user("john", is_staff=True)
+        self.user2 = create_user("tony")
         self.anonymous = create_anonymous()
-        self.perm1 = 'permission.add_article'
-        self.perm2 = 'permission.change_article'
-        self.perm3 = 'permission.delete_article'
-        self.article = create_article('test')
+        self.perm1 = "permission.add_article"
+        self.perm2 = "permission.change_article"
+        self.perm3 = "permission.delete_article"
+        self.article = create_article("test")
 
     def test_constructor(self):
         permission_logic = StaffPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
 
         self.assertTrue(isinstance(permission_logic, StaffPermissionLogic))
         self.assertEqual(permission_logic.any_permission, True)
@@ -72,34 +73,34 @@
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertTrue(permission_logic.has_perm(self.user1, self.perm3))
         self.assertFalse(permission_logic.has_perm(self.user2, self.perm3))
 
     def test_has_perm_add_with_obj(self):
         permission_logic = StaffPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm1, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm1, self.article))
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm1, self.article))
+            permission_logic.has_perm(self.user2, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj(self):
         permission_logic = StaffPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm2, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm2, self.article))
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm2, self.article))
+            permission_logic.has_perm(self.user2, self.perm2, self.article)
+        )
 
     def test_has_perm_delete_with_obj(self):
         permission_logic = StaffPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm3, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm3, self.article))
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm3, self.article))
+            permission_logic.has_perm(self.user2, self.perm3, self.article)
+        )
 
     def test_has_perm_add_without_obj_with_anonymous(self):
         permission_logic = StaffPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(permission_logic.has_perm(self.anonymous, self.perm1))
 
     def test_has_perm_change_without_obj_with_anonymous(self):
@@ -112,27 +113,30 @@
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(permission_logic.has_perm(self.anonymous, self.perm3))
 
     def test_has_perm_add_with_obj_with_anonymous(self):
         permission_logic = StaffPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-            permission_logic.has_perm(self.anonymous, self.perm1, self.article))
+            permission_logic.has_perm(self.anonymous, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj_with_anonymous(self):
         permission_logic = StaffPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-            permission_logic.has_perm(self.anonymous, self.perm2, self.article))
+            permission_logic.has_perm(self.anonymous, self.perm2, self.article)
+        )
 
     def test_has_perm_delete_with_obj_with_anonymous(self):
         permission_logic = StaffPermissionLogic()
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertFalse(
-            permission_logic.has_perm(self.anonymous, self.perm3, self.article))
+            permission_logic.has_perm(self.anonymous, self.perm3, self.article)
+        )
 
     def test_has_perm_add_without_obj_without_any(self):
         permission_logic = StaffPermissionLogic(any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertTrue(permission_logic.has_perm(self.user1, self.perm1))
         self.assertFalse(permission_logic.has_perm(self.user2, self.perm1))
 
@@ -147,27 +151,27 @@
         add_permission_logic(self.article.__class__, permission_logic)
         self.assertTrue(permission_logic.has_perm(self.user1, self.perm3))
         self.assertFalse(permission_logic.has_perm(self.user2, self.perm3))
 
     def test_has_perm_add_with_obj_without_any(self):
         permission_logic = StaffPermissionLogic(any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm1, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm1, self.article))
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm1, self.article))
+            permission_logic.has_perm(self.user2, self.perm1, self.article)
+        )
 
     def test_has_perm_change_with_obj_without_any(self):
         permission_logic = StaffPermissionLogic(any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm2, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm2, self.article))
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm2, self.article))
+            permission_logic.has_perm(self.user2, self.perm2, self.article)
+        )
 
     def test_has_perm_delete_with_obj_without_any(self):
         permission_logic = StaffPermissionLogic(any_permission=False)
         add_permission_logic(self.article.__class__, permission_logic)
-        self.assertTrue(
-                permission_logic.has_perm(self.user1, self.perm3, self.article))
+        self.assertTrue(permission_logic.has_perm(self.user1, self.perm3, self.article))
         self.assertFalse(
-                permission_logic.has_perm(self.user2, self.perm3, self.article))
+            permission_logic.has_perm(self.user2, self.perm3, self.article)
+        )
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_templatetags/test_permissionif.py` & `django_permission2-2.1.0/src/permission/tests/test_templatetags/test_permissionif.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,75 @@
 # coding=utf-8
-from django.test import TestCase, override_settings
 from django.template import Context, Template
-from ...utils.handlers import registry
+from django.test import TestCase, override_settings
+
 from ...templatetags.permissionif import replace_builtin_if
-from ..utils import create_user, create_article, create_permission
+from ...utils.handlers import registry
+from ..utils import create_article, create_permission, create_user
 
 
 @override_settings(
     AUTHENTICATION_BACKENDS=(
-        'django.contrib.auth.backends.ModelBackend',
-        'permission.backends.PermissionBackend',
+        "django.contrib.auth.backends.ModelBackend",
+        "permission.backends.PermissionBackend",
     ),
     PERMISSION_REPLACE_BUILTIN_IF=False,
 )
 class PermissionTemplateTagsTestCase(TestCase):
-
     def setUp(self):
         # store original registry
         self._original_registry = registry._registry
         # clear registry and register mock handler
         registry._registry = {}
         # Make sure builtin if is not replaced
         replace_builtin_if(False)
 
     def tearDown(self):
         # restore original registry
         registry._registry = self._original_registry
 
     def test_permissionif_tag(self):
-        user = create_user('permission_templatetag_test_user1')
-        perm = create_permission('permission_templatetag_test_perm1')
+        user = create_user("permission_templatetag_test_user1")
+        perm = create_permission("permission_templatetag_test_perm1")
 
         user.user_permissions.add(perm)
 
-        self.assertTrue(user.has_perm(
-            'permission.permission_templatetag_test_perm1'))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm1"))
 
-        context = Context({
-            'user': user,
-        })
+        context = Context(
+            {
+                "user": user,
+            }
+        )
 
         out = Template(
             "{% load permissionif %}"
             "{% permission user has "
             "'permission.permission_templatetag_test_perm1' %}"
             "Success"
             "{% else %}"
             "Fail"
             "{% endpermission %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_permissionif_tag_elif(self):
-        user = create_user('permission_templatetag_test_user1')
-        perm = create_permission('permission_templatetag_test_perm1')
+        user = create_user("permission_templatetag_test_user1")
+        perm = create_permission("permission_templatetag_test_perm1")
 
         user.user_permissions.add(perm)
 
-        self.assertTrue(user.has_perm(
-            'permission.permission_templatetag_test_perm1'))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm1"))
 
-        context = Context({
-            'user': user,
-        })
+        context = Context(
+            {
+                "user": user,
+            }
+        )
 
         out = Template(
             "{% load permissionif %}"
             "{% permission user has 'permission.unknown_permission' %}"
             "Fail"
             "{% elpermission user has 'permission.unknown_permisson2' %}"
             "Fail"
@@ -78,70 +80,71 @@
             "Fail"
             "{% endpermission %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_permissionif_tag_else(self):
-        user = create_user('permission_templatetag_test_user1')
-        perm = create_permission('permission_templatetag_test_perm1')
+        user = create_user("permission_templatetag_test_user1")
+        perm = create_permission("permission_templatetag_test_perm1")
 
         user.user_permissions.add(perm)
 
-        self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm1'))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm1"))
 
-        context = Context({
-            'user': user,
-        })
+        context = Context(
+            {
+                "user": user,
+            }
+        )
 
         out = Template(
             "{% load permissionif %}"
             "{% permission user has 'permission.unknown_permission' %}"
             "Fail"
             "{% else %}"
             "Success"
             "{% endpermission %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_permissionif_tag_with_obj(self):
-        from permission.tests.models import Article
         from permission.handlers import PermissionHandler
+        from permission.tests.models import Article
 
-        user = create_user('permission_templatetag_test_user1')
-        art1 = create_article('permission_templatetag_test_article1')
-        art2 = create_article('permission_templatetag_test_article2')
-        create_permission('permission_templatetag_test_perm1')
+        user = create_user("permission_templatetag_test_user1")
+        art1 = create_article("permission_templatetag_test_article1")
+        art2 = create_article("permission_templatetag_test_article2")
+        create_permission("permission_templatetag_test_perm1")
 
         class ArticlePermissionHandler(PermissionHandler):
-
             def has_perm(self, user_obj, perm, obj=None):
-                if perm == 'permission.permission_templatetag_test_perm1':
-                    if (obj and obj.title ==
-                            'permission_templatetag_test_article2'):
+                if perm == "permission.permission_templatetag_test_perm1":
+                    if obj and obj.title == "permission_templatetag_test_article2":
                         return True
                 return False
+
         registry.register(Article, ArticlePermissionHandler)
 
+        self.assertFalse(user.has_perm("permission.permission_templatetag_test_perm1"))
         self.assertFalse(
-            user.has_perm('permission.permission_templatetag_test_perm1'))
-        self.assertFalse(
-            user.has_perm('permission.permission_templatetag_test_perm1',
-                          art1))
+            user.has_perm("permission.permission_templatetag_test_perm1", art1)
+        )
         self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm1',
-                          art2))
+            user.has_perm("permission.permission_templatetag_test_perm1", art2)
+        )
 
-        context = Context({
-            'user': user,
-            'art1': art1,
-            'art2': art2,
-        })
+        context = Context(
+            {
+                "user": user,
+                "art1": art1,
+                "art2": art2,
+            }
+        )
 
         out = Template(
             "{% load permissionif %}"
             "{% permission user has "
             "'permission.permission_templatetag_test_perm1' %}"
             "Fail"
             "{% elpermission user has "
@@ -154,28 +157,28 @@
             "Fail"
             "{% endpermission %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_permissionif_tag_and(self):
-        user = create_user('permission_templatetag_test_user1')
-        perm1 = create_permission('permission_templatetag_test_perm1')
-        perm2 = create_permission('permission_templatetag_test_perm2')
+        user = create_user("permission_templatetag_test_user1")
+        perm1 = create_permission("permission_templatetag_test_perm1")
+        perm2 = create_permission("permission_templatetag_test_perm2")
 
         user.user_permissions.add(perm1, perm2)
 
-        self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm1'))
-        self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm2'))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm1"))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm2"))
 
-        context = Context({
-            'user': user,
-        })
+        context = Context(
+            {
+                "user": user,
+            }
+        )
 
         out = Template(
             "{% load permissionif %}"
             "{% permission user has 'permission.unknown_perm' "
             "and user has 'permission.permission_templatetag_test_perm2' %}"
             "Fail"
             "{% elpermission user has "
@@ -188,29 +191,28 @@
             "Success"
             "{% endpermission %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_permissionif_tag_or(self):
-
-        user = create_user('permission_templatetag_test_user1')
-        perm1 = create_permission('permission_templatetag_test_perm1')
-        create_permission('permission_templatetag_test_perm2')
+        user = create_user("permission_templatetag_test_user1")
+        perm1 = create_permission("permission_templatetag_test_perm1")
+        create_permission("permission_templatetag_test_perm2")
 
         user.user_permissions.add(perm1)
 
-        self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm1'))
-        self.assertFalse(
-            user.has_perm('permission.permission_templatetag_test_perm2'))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm1"))
+        self.assertFalse(user.has_perm("permission.permission_templatetag_test_perm2"))
 
-        context = Context({
-            'user': user,
-        })
+        context = Context(
+            {
+                "user": user,
+            }
+        )
 
         out = Template(
             "{% load permissionif %}"
             "{% permission user has "
             "'permission.permission_templatetag_test_perm1' "
             "and user has 'permission.permission_templatetag_test_perm2' %}"
             "Fail"
@@ -222,69 +224,70 @@
         ).render(context)
 
         self.assertEqual(out, "Success")
 
 
 @override_settings(
     AUTHENTICATION_BACKENDS=(
-        'django.contrib.auth.backends.ModelBackend',
-        'permission.backends.PermissionBackend',
+        "django.contrib.auth.backends.ModelBackend",
+        "permission.backends.PermissionBackend",
     ),
     PERMISSION_REPLACE_BUILTIN_IF=True,
 )
 class PermissionTemplateTagsWithBuiltinTestCase(TestCase):
-
     def setUp(self):
         # store original registry
         self._original_registry = registry._registry
         # clear registry and register mock handler
         registry._registry = {}
         # Make sure builtin if is replaced
         replace_builtin_if(True)
 
     def tearDown(self):
         # restore original registry
         registry._registry = self._original_registry
 
     def test_permissionif_tag(self):
-        user = create_user('permission_templatetag_test_user1')
-        perm = create_permission('permission_templatetag_test_perm1')
+        user = create_user("permission_templatetag_test_user1")
+        perm = create_permission("permission_templatetag_test_perm1")
 
         user.user_permissions.add(perm)
 
-        self.assertTrue(user.has_perm(
-            'permission.permission_templatetag_test_perm1'))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm1"))
 
-        context = Context({
-            'user': user,
-        })
+        context = Context(
+            {
+                "user": user,
+            }
+        )
 
         out = Template(
             "{% permission user has "
             "'permission.permission_templatetag_test_perm1' %}"
             "Success"
             "{% else %}"
             "Fail"
             "{% endpermission %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_permissionif_tag_elif(self):
-        user = create_user('permission_templatetag_test_user1')
-        perm = create_permission('permission_templatetag_test_perm1')
+        user = create_user("permission_templatetag_test_user1")
+        perm = create_permission("permission_templatetag_test_perm1")
 
         user.user_permissions.add(perm)
 
-        self.assertTrue(user.has_perm(
-            'permission.permission_templatetag_test_perm1'))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm1"))
 
-        context = Context({
-            'user': user,
-        })
+        context = Context(
+            {
+                "user": user,
+            }
+        )
 
         out = Template(
             "{% permission user has 'permission.unknown_permission' %}"
             "Fail"
             "{% elpermission user has 'permission.unknown_permission2' %}"
             "Fail"
             "{% elpermission user has "
@@ -294,69 +297,70 @@
             "Fail"
             "{% endpermission %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_permissionif_tag_else(self):
-        user = create_user('permission_templatetag_test_user1')
-        perm = create_permission('permission_templatetag_test_perm1')
+        user = create_user("permission_templatetag_test_user1")
+        perm = create_permission("permission_templatetag_test_perm1")
 
         user.user_permissions.add(perm)
 
-        self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm1'))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm1"))
 
-        context = Context({
-            'user': user,
-        })
+        context = Context(
+            {
+                "user": user,
+            }
+        )
 
         out = Template(
             "{% permission user has 'permission.unknown_permission' %}"
             "Fail"
             "{% else %}"
             "Success"
             "{% endpermission %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_permissionif_tag_with_obj(self):
-        from permission.tests.models import Article
         from permission.handlers import PermissionHandler
+        from permission.tests.models import Article
 
-        user = create_user('permission_templatetag_test_user1')
-        art1 = create_article('permission_templatetag_test_article1')
-        art2 = create_article('permission_templatetag_test_article2')
-        create_permission('permission_templatetag_test_perm1')
+        user = create_user("permission_templatetag_test_user1")
+        art1 = create_article("permission_templatetag_test_article1")
+        art2 = create_article("permission_templatetag_test_article2")
+        create_permission("permission_templatetag_test_perm1")
 
         class ArticlePermissionHandler(PermissionHandler):
-
             def has_perm(self, user_obj, perm, obj=None):
-                if perm == 'permission.permission_templatetag_test_perm1':
-                    if (obj and obj.title ==
-                            'permission_templatetag_test_article2'):
+                if perm == "permission.permission_templatetag_test_perm1":
+                    if obj and obj.title == "permission_templatetag_test_article2":
                         return True
                 return False
+
         registry.register(Article, ArticlePermissionHandler)
 
+        self.assertFalse(user.has_perm("permission.permission_templatetag_test_perm1"))
         self.assertFalse(
-            user.has_perm('permission.permission_templatetag_test_perm1'))
-        self.assertFalse(
-            user.has_perm('permission.permission_templatetag_test_perm1',
-                          art1))
+            user.has_perm("permission.permission_templatetag_test_perm1", art1)
+        )
         self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm1',
-                          art2))
+            user.has_perm("permission.permission_templatetag_test_perm1", art2)
+        )
 
-        context = Context({
-            'user': user,
-            'art1': art1,
-            'art2': art2,
-        })
+        context = Context(
+            {
+                "user": user,
+                "art1": art1,
+                "art2": art2,
+            }
+        )
 
         out = Template(
             "{% permission user has "
             "'permission.permission_templatetag_test_perm1' %}"
             "Fail"
             "{% elpermission user has "
             "'permission.permission_templatetag_test_perm1' of art1 %}"
@@ -368,28 +372,28 @@
             "Fail"
             "{% endpermission %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_permissionif_tag_and(self):
-        user = create_user('permission_templatetag_test_user1')
-        perm1 = create_permission('permission_templatetag_test_perm1')
-        perm2 = create_permission('permission_templatetag_test_perm2')
+        user = create_user("permission_templatetag_test_user1")
+        perm1 = create_permission("permission_templatetag_test_perm1")
+        perm2 = create_permission("permission_templatetag_test_perm2")
 
         user.user_permissions.add(perm1, perm2)
 
-        self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm1'))
-        self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm2'))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm1"))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm2"))
 
-        context = Context({
-            'user': user,
-        })
+        context = Context(
+            {
+                "user": user,
+            }
+        )
 
         out = Template(
             "{% permission user has 'permission.unknown_perm' "
             "and user has 'permission.permission_templatetag_test_perm2' %}"
             "Fail"
             "{% elpermission user has "
             "'permission.permission_templatetag_test_perm1' "
@@ -401,29 +405,28 @@
             "Success"
             "{% endpermission %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_permissionif_tag_or(self):
-
-        user = create_user('permission_templatetag_test_user1')
-        perm1 = create_permission('permission_templatetag_test_perm1')
-        create_permission('permission_templatetag_test_perm2')
+        user = create_user("permission_templatetag_test_user1")
+        perm1 = create_permission("permission_templatetag_test_perm1")
+        create_permission("permission_templatetag_test_perm2")
 
         user.user_permissions.add(perm1)
 
-        self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm1'))
-        self.assertFalse(
-            user.has_perm('permission.permission_templatetag_test_perm2'))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm1"))
+        self.assertFalse(user.has_perm("permission.permission_templatetag_test_perm2"))
 
-        context = Context({
-            'user': user,
-        })
+        context = Context(
+            {
+                "user": user,
+            }
+        )
 
         out = Template(
             "{% permission user has "
             "'permission.permission_templatetag_test_perm1' "
             "and user has 'permission.permission_templatetag_test_perm2' %}"
             "Fail"
             "{% elpermission user has "
@@ -432,48 +435,50 @@
             "Success"
             "{% endpermission %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_if_tag(self):
-        user = create_user('permission_templatetag_test_user1')
-        perm = create_permission('permission_templatetag_test_perm1')
+        user = create_user("permission_templatetag_test_user1")
+        perm = create_permission("permission_templatetag_test_perm1")
 
         user.user_permissions.add(perm)
 
-        self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm1'))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm1"))
 
-        context = Context({
-            'user': user,
-        })
+        context = Context(
+            {
+                "user": user,
+            }
+        )
 
         out = Template(
             "{% if user has 'permission.permission_templatetag_test_perm1' %}"
             "Success"
             "{% else %}"
             "Fail"
             "{% endif %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_if_tag_elif(self):
-        user = create_user('permission_templatetag_test_user1')
-        perm = create_permission('permission_templatetag_test_perm1')
+        user = create_user("permission_templatetag_test_user1")
+        perm = create_permission("permission_templatetag_test_perm1")
 
         user.user_permissions.add(perm)
 
-        self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm1'))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm1"))
 
-        context = Context({
-            'user': user,
-        })
+        context = Context(
+            {
+                "user": user,
+            }
+        )
 
         out = Template(
             "{% if user has 'permission.unknown_permission' %}"
             "Fail"
             "{% elif user has 'permission.unknown_permisson2' %}"
             "Fail"
             "{% elif user has "
@@ -483,68 +488,70 @@
             "Fail"
             "{% endif %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_if_tag_else(self):
-        user = create_user('permission_templatetag_test_user1')
-        perm = create_permission('permission_templatetag_test_perm1')
+        user = create_user("permission_templatetag_test_user1")
+        perm = create_permission("permission_templatetag_test_perm1")
 
         user.user_permissions.add(perm)
 
-        self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm1'))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm1"))
 
-        context = Context({
-            'user': user,
-        })
+        context = Context(
+            {
+                "user": user,
+            }
+        )
 
         out = Template(
             "{% if user has 'permission.unknown_permission' %}"
             "Fail"
             "{% else %}"
             "Success"
             "{% endif %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_if_tag_with_obj(self):
-        from permission.tests.models import Article
         from permission.handlers import PermissionHandler
+        from permission.tests.models import Article
 
-        user = create_user('permission_templatetag_test_user1')
-        art1 = create_article('permission_templatetag_test_article1')
-        art2 = create_article('permission_templatetag_test_article2')
-        create_permission('permission_templatetag_test_perm1')
+        user = create_user("permission_templatetag_test_user1")
+        art1 = create_article("permission_templatetag_test_article1")
+        art2 = create_article("permission_templatetag_test_article2")
+        create_permission("permission_templatetag_test_perm1")
 
         class ArticlePermissionHandler(PermissionHandler):
             def has_perm(self, user_obj, perm, obj=None):
-                if perm == 'permission.permission_templatetag_test_perm1':
-                    if (obj and obj.title ==
-                            'permission_templatetag_test_article2'):
+                if perm == "permission.permission_templatetag_test_perm1":
+                    if obj and obj.title == "permission_templatetag_test_article2":
                         return True
                 return False
+
         registry.register(Article, ArticlePermissionHandler)
 
+        self.assertFalse(user.has_perm("permission.permission_templatetag_test_perm1"))
         self.assertFalse(
-            user.has_perm('permission.permission_templatetag_test_perm1'))
-        self.assertFalse(
-            user.has_perm('permission.permission_templatetag_test_perm1',
-                          art1))
+            user.has_perm("permission.permission_templatetag_test_perm1", art1)
+        )
         self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm1',
-                          art2))
+            user.has_perm("permission.permission_templatetag_test_perm1", art2)
+        )
 
-        context = Context({
-            'user': user,
-            'art1': art1,
-            'art2': art2,
-        })
+        context = Context(
+            {
+                "user": user,
+                "art1": art1,
+                "art2": art2,
+            }
+        )
 
         out = Template(
             "{% if user has 'permission.permission_templatetag_test_perm1' %}"
             "Fail"
             "{% elif user has "
             "'permission.permission_templatetag_test_perm1' of art1 %}"
             "Fail"
@@ -555,28 +562,28 @@
             "Fail"
             "{% endif %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_if_tag_and(self):
-        user = create_user('permission_templatetag_test_user1')
-        perm1 = create_permission('permission_templatetag_test_perm1')
-        perm2 = create_permission('permission_templatetag_test_perm2')
+        user = create_user("permission_templatetag_test_user1")
+        perm1 = create_permission("permission_templatetag_test_perm1")
+        perm2 = create_permission("permission_templatetag_test_perm2")
 
         user.user_permissions.add(perm1, perm2)
 
-        self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm1'))
-        self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm2'))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm1"))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm2"))
 
-        context = Context({
-            'user': user,
-        })
+        context = Context(
+            {
+                "user": user,
+            }
+        )
 
         out = Template(
             "{% if user has 'permission.unknown_perm' "
             "and user has 'permission.permission_templatetag_test_perm2' %}"
             "Fail"
             "{% elif user has 'permission.permission_templatetag_test_perm1' "
             "and user has 'permission.unknown_perm' %}"
@@ -586,28 +593,28 @@
             "Success"
             "{% endif %}"
         ).render(context)
 
         self.assertEqual(out, "Success")
 
     def test_if_tag_or(self):
-        user = create_user('permission_templatetag_test_user1')
-        perm1 = create_permission('permission_templatetag_test_perm1')
-        create_permission('permission_templatetag_test_perm2')
+        user = create_user("permission_templatetag_test_user1")
+        perm1 = create_permission("permission_templatetag_test_perm1")
+        create_permission("permission_templatetag_test_perm2")
 
         user.user_permissions.add(perm1)
 
-        self.assertTrue(
-            user.has_perm('permission.permission_templatetag_test_perm1'))
-        self.assertFalse(
-            user.has_perm('permission.permission_templatetag_test_perm2'))
+        self.assertTrue(user.has_perm("permission.permission_templatetag_test_perm1"))
+        self.assertFalse(user.has_perm("permission.permission_templatetag_test_perm2"))
 
-        context = Context({
-            'user': user,
-        })
+        context = Context(
+            {
+                "user": user,
+            }
+        )
 
         out = Template(
             "{% if user has 'permission.permission_templatetag_test_perm1' "
             "and user has 'permission.permission_templatetag_test_perm2' %}"
             "Fail"
             "{% elif user has 'permission.permission_templatetag_test_perm1' "
             "or user has 'permission.permission_templatetag_test_perm2' %}"
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_utils/test_field_lookup.py` & `django_permission2-2.1.0/src/permission/tests/test_utils/test_field_lookup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,99 +1,92 @@
 # coding=utf-8
 from django.test import TestCase
+
 from ...utils.field_lookup import field_lookup
-from ..utils import create_user, create_bridge, create_article
+from ..utils import create_article, create_bridge, create_user
 
 
 class PermissionUtilsFieldLookupTestCase(TestCase):
     def setUp(self):
-        self.author = create_user('permission_test_articles_author')
-        self.editor1 = create_user(
-            'permission_test_articles_editor1')
-        self.editor2 = create_user(
-            'permission_test_articles_editor2')
+        self.author = create_user("permission_test_articles_author")
+        self.editor1 = create_user("permission_test_articles_editor1")
+        self.editor2 = create_user("permission_test_articles_editor2")
         self.bridge1 = create_bridge()
         self.bridge2 = create_bridge()
         self.bridge3 = create_bridge()
-        self.model = create_article('permission_test_article',
-                                    self.author, self.bridge1)
+        self.model = create_article(
+            "permission_test_article", self.author, self.bridge1
+        )
         self.model.editors.add(self.editor1)
         self.model.editors.add(self.editor2)
         self.model.multiple_bridge.add(self.bridge2)
         self.model.multiple_bridge.add(self.bridge3)
 
     def test_field_lookup_author(self):
-        field_value = field_lookup(self.model, 'author')
+        field_value = field_lookup(self.model, "author")
         self.assertEqual(field_value, self.author)
 
     def test_field_lookup_author_username(self):
-        field_value = field_lookup(self.model, 'author__username')
+        field_value = field_lookup(self.model, "author__username")
         self.assertEqual(field_value, self.author.username)
 
     def test_field_lookup_editors(self):
-        field_value = field_lookup(self.model, 'editors')
+        field_value = field_lookup(self.model, "editors")
         field_value = list(x for x in field_value.iterator())
         expected_value = list([self.editor1, self.editor2])
         self.assertEqual(field_value, expected_value)
 
     def test_field_lookup_editors_username(self):
-        field_value = list(field_lookup(self.model, 'editors__username'))
-        expected_value = [x.username for x in
-                          (self.editor1, self.editor2)]
+        field_value = list(field_lookup(self.model, "editors__username"))
+        expected_value = [x.username for x in (self.editor1, self.editor2)]
         self.assertEqual(field_value, expected_value)
 
     def test_field_lookup_single_bridge_author(self):
-        field_value = field_lookup(self.model, 'single_bridge__author')
+        field_value = field_lookup(self.model, "single_bridge__author")
         self.assertEqual(field_value, self.bridge1.author)
 
     def test_field_lookup_single_bridge_author_username(self):
-        field_value = field_lookup(self.model,
-                                   'single_bridge__author__username')
+        field_value = field_lookup(self.model, "single_bridge__author__username")
         self.assertEqual(field_value, self.bridge1.author.username)
 
     def test_field_lookup_single_bridge_editors(self):
-        field_value = field_lookup(self.model, 'single_bridge__editors')
+        field_value = field_lookup(self.model, "single_bridge__editors")
         field_value = list(x for x in field_value.iterator())
         expected_value = list(self.bridge1.editors.iterator())
         self.assertEqual(field_value, expected_value)
 
     def test_field_lookup_single_bridge_editors_username(self):
-        field_value = list(field_lookup(self.model,
-                                        'single_bridge__editors__username'))
+        field_value = list(field_lookup(self.model, "single_bridge__editors__username"))
         expected_value = [x.username for x in self.bridge1.editors.iterator()]
         self.assertEqual(field_value, expected_value)
 
     def test_field_lookup_multiple_bridge_author(self):
-        field_value = list(field_lookup(self.model, 'multiple_bridge__author'))
-        expected_value = list([self.bridge2.author,
-                                         self.bridge3.author])
+        field_value = list(field_lookup(self.model, "multiple_bridge__author"))
+        expected_value = list([self.bridge2.author, self.bridge3.author])
         self.assertEqual(field_value, expected_value)
 
     def test_field_lookup_multiple_bridge_author_username(self):
-        field_value = field_lookup(self.model,
-                                   'multiple_bridge__author__username')
+        field_value = field_lookup(self.model, "multiple_bridge__author__username")
         field_value = list(field_value)
-        expected_value = [x.username for x in (self.bridge2.author,
-                                               self.bridge3.author)]
+        expected_value = [
+            x.username for x in (self.bridge2.author, self.bridge3.author)
+        ]
         self.assertEqual(field_value, expected_value)
 
     def test_field_lookup_multiple_bridge_editors(self):
-        field_value = list(field_lookup(self.model,
-                                        'multiple_bridge__editors'))
+        field_value = list(field_lookup(self.model, "multiple_bridge__editors"))
         field_value = [
             [repr(x) for x in field_value[0].iterator()],
             [repr(x) for x in field_value[1].iterator()],
         ]
         expected_value1 = [repr(x) for x in self.bridge2.editors.iterator()]
         expected_value2 = [repr(x) for x in self.bridge3.editors.iterator()]
         expected_value = [expected_value1, expected_value2]
         self.assertEqual(field_value, expected_value)
 
     def test_field_lookup_multiple_bridge_editors__name(self):
-        field_value = field_lookup(self.model,
-                                   'multiple_bridge__editors__username')
+        field_value = field_lookup(self.model, "multiple_bridge__editors__username")
         field_value = list(map(list, field_value))
         expected_value1 = [x.username for x in self.bridge2.editors.iterator()]
         expected_value2 = [x.username for x in self.bridge3.editors.iterator()]
         expected_value = [expected_value1, expected_value2]
         self.assertEqual(field_value, expected_value)
-
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_utils/test_handlers.py` & `django_permission2-2.1.0/src/permission/tests/test_utils/test_handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,76 +1,69 @@
 from django.test import TestCase, override_settings
-from ...utils.handlers import PermissionHandlerRegistry
+
 from ...handlers import PermissionHandler
+from ...utils.handlers import PermissionHandlerRegistry
 from ..compat import MagicMock
 
 
-@override_settings(
-    PERMISSION_DEFAULT_PERMISSION_HANDLER=PermissionHandler
-)
+@override_settings(PERMISSION_DEFAULT_PERMISSION_HANDLER=PermissionHandler)
 class PermissionUtilsHandlersTestCase(TestCase):
     def setUp(self):
         self.registry = PermissionHandlerRegistry()
         self.model = MagicMock()
         self.model._meta = MagicMock()
         self.model._meta.abstract = False
         self.handler = PermissionHandler
 
     def test_register(self):
         self.registry.register(self.model, self.handler)
         self.assertTrue(self.model in self.registry._registry)
-        self.assertTrue(isinstance(self.registry._registry[self.model],
-                                   self.handler))
+        self.assertTrue(isinstance(self.registry._registry[self.model], self.handler))
 
     def test_register_without_specifing_handler(self):
         self.registry.register(self.model)
         self.assertTrue(self.model in self.registry._registry)
-        self.assertTrue(isinstance(self.registry._registry[self.model],
-                                   self.handler))
+        self.assertTrue(isinstance(self.registry._registry[self.model], self.handler))
 
     def test_register_with_abstract_model(self):
         from django.core.exceptions import ImproperlyConfigured
+
         abstract_model = MagicMock()
         abstract_model._meta = MagicMock()
         abstract_model._meta.abstract = True
-        self.assertRaises(ImproperlyConfigured,
-                          self.registry.register,
-                          abstract_model, self.handler)
+        self.assertRaises(
+            ImproperlyConfigured, self.registry.register, abstract_model, self.handler
+        )
 
     def test_register_duplicate(self):
         self.registry.register(self.model, self.handler)
-        self.assertRaises(KeyError,
-                          self.registry.register,
-                          self.model, self.handler)
+        self.assertRaises(KeyError, self.registry.register, self.model, self.handler)
 
     def test_register_permission_handler_instance(self):
         handler_instance = self.handler(self.model)
-        self.assertRaises(AttributeError,
-                          self.registry.register,
-                          self.model, handler_instance)
+        self.assertRaises(
+            AttributeError, self.registry.register, self.model, handler_instance
+        )
 
     def test_register_non_permission_handler(self):
-        self.assertRaises(AttributeError,
-                          self.registry.register,
-                          self.model, self.__class__)
+        self.assertRaises(
+            AttributeError, self.registry.register, self.model, self.__class__
+        )
 
     def test_unregister(self):
         self.registry.register(self.model, self.handler)
         self.registry.unregister(self.model)
         self.assertFalse(self.model in self.registry._registry)
 
     def test_unregister_absence(self):
-        self.assertRaises(KeyError,
-                          self.registry.unregister,
-                          self.model)
+        self.assertRaises(KeyError, self.registry.unregister, self.model)
 
     def test_get_handlers(self):
         results = self.registry.get_handlers()
         self.assertTrue(isinstance(results, tuple))
         self.assertTrue(len(results) == 0)
 
         self.registry.register(self.model, self.handler)
         results = self.registry.get_handlers()
         self.assertTrue(isinstance(results, tuple))
         self.assertTrue(len(results) == 1)
         self.assertTrue(isinstance(results[0], PermissionHandler))
-
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/test_utils/test_logics.py` & `django_permission2-2.1.0/src/permission/tests/test_utils/test_logics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,98 +1,104 @@
 # coding=utf-8
 from django.test import TestCase
-from ...logics import PermissionLogic
+
 from ...handlers import LogicalPermissionHandler
+from ...logics import PermissionLogic
 from ...utils.handlers import registry
 from ...utils.logics import add_permission_logic, remove_permission_logic
-from ..models import Article
 from ..compat import MagicMock
+from ..models import Article
 
 
 class PermissionUtilsLogicsTestCase(TestCase):
     def setUp(self):
         self.mock_logic = MagicMock(spec=PermissionLogic)
         self.mock_logic2 = MagicMock(spec=PermissionLogic)
         # clear registry
         self.registry_backup = registry._registry
         registry._registry = {}
         # clear attributes
-        if hasattr(Article, '_permission_logics'):
-            delattr(Article, '_permission_logics')
-        if hasattr(Article, '_permission_handler'):
-            delattr(Article, '_permission_handler')
+        if hasattr(Article, "_permission_logics"):
+            delattr(Article, "_permission_logics")
+        if hasattr(Article, "_permission_handler"):
+            delattr(Article, "_permission_handler")
 
     def tearDown(self):
         registry._registry = self.registry_backup
 
     def test_add_permission_logic_private_attributes(self):
         m = self.mock_logic
         # the following private attribute should not be exists in Article model
-        self.assertFalse(hasattr(Article, '_permission_logics'))
-        self.assertFalse(hasattr(Article, '_permission_handler'))
+        self.assertFalse(hasattr(Article, "_permission_logics"))
+        self.assertFalse(hasattr(Article, "_permission_handler"))
 
         # but after add permission logic, they will be appeared
         add_permission_logic(Article, m)
-        self.assertTrue(hasattr(Article, '_permission_logics'))
-        self.assertTrue(hasattr(Article, '_permission_handler'))
+        self.assertTrue(hasattr(Article, "_permission_logics"))
+        self.assertTrue(hasattr(Article, "_permission_handler"))
 
     def test_add_permission_logic_registry(self):
         m = self.mock_logic
         # nothing have been registered in registry
         self.assertEqual(registry._registry, {})
         # but after add permission logic, they will be appeared
         add_permission_logic(Article, m)
         self.assertEqual(Article._permission_logics, set([m]))
-        self.assertTrue(isinstance(registry._registry[Article],
-                                   LogicalPermissionHandler))
+        self.assertTrue(
+            isinstance(registry._registry[Article], LogicalPermissionHandler)
+        )
 
     def test_remove_permission_logic_private_attributes(self):
         m = self.mock_logic
         add_permission_logic(Article, m)
-        self.assertTrue(hasattr(Article, '_permission_logics'))
-        self.assertTrue(hasattr(Article, '_permission_handler'))
+        self.assertTrue(hasattr(Article, "_permission_logics"))
+        self.assertTrue(hasattr(Article, "_permission_handler"))
 
         # private attribute should not be disappeared
         remove_permission_logic(Article, m)
-        self.assertTrue(hasattr(Article, '_permission_logics'))
-        self.assertTrue(hasattr(Article, '_permission_handler'))
+        self.assertTrue(hasattr(Article, "_permission_logics"))
+        self.assertTrue(hasattr(Article, "_permission_handler"))
 
     def test_remove_permission_logic_registry(self):
         m = self.mock_logic
         add_permission_logic(Article, m)
         self.assertEqual(Article._permission_logics, set([m]))
-        self.assertTrue(isinstance(registry._registry[Article],
-                                   LogicalPermissionHandler))
+        self.assertTrue(
+            isinstance(registry._registry[Article], LogicalPermissionHandler)
+        )
 
         # permission_logics should be changed but registry
         # should not be changed
         remove_permission_logic(Article, m)
         self.assertEqual(Article._permission_logics, set())
-        self.assertTrue(isinstance(registry._registry[Article],
-                                   LogicalPermissionHandler))
+        self.assertTrue(
+            isinstance(registry._registry[Article], LogicalPermissionHandler)
+        )
 
     def test_remove_permission_logic_registry_with_class(self):
         m = self.mock_logic
         m2 = self.mock_logic2
         add_permission_logic(Article, m)
         add_permission_logic(Article, m2)
         self.assertEqual(Article._permission_logics, set([m, m2]))
-        self.assertTrue(isinstance(registry._registry[Article],
-                                   LogicalPermissionHandler))
+        self.assertTrue(
+            isinstance(registry._registry[Article], LogicalPermissionHandler)
+        )
 
         # permission_logics should be changed but registry
         # should not be changed
         remove_permission_logic(Article, PermissionLogic)
         self.assertEqual(Article._permission_logics, set())
-        self.assertTrue(isinstance(registry._registry[Article],
-                                   LogicalPermissionHandler))
+        self.assertTrue(
+            isinstance(registry._registry[Article], LogicalPermissionHandler)
+        )
 
     def test_remove_permission_logic_exception(self):
         m = self.mock_logic
         add_permission_logic(Article, m)
         remove_permission_logic(Article, m)
         # it should not raise exception
         remove_permission_logic(Article, m)
         # it should raise exception if fail_silently is False
-        self.assertRaises(KeyError,
-                remove_permission_logic, Article, m,
-                fail_silently=False)
+        self.assertRaises(
+            KeyError, remove_permission_logic, Article, m, fail_silently=False
+        )
```

### Comparing `django-permission2-2.0.0b4/src/permission/tests/utils.py` & `django_permission2-2.1.0/src/permission/tests/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,71 +1,75 @@
 # coding=utf-8
 
 
 def create_user(username, **kwargs):
     from django.contrib.auth.models import User
+
     user = User.objects.create_user(
         username=username,
         email="%s@test.com" % username,
         password="password",
     )
     # attribute assignment
     for key, value in kwargs.items():
         user.__dict__[key] = value
     user.save()
     return user
 
 
 def create_anonymous(**kwargs):
     from django.contrib.auth.models import AnonymousUser
+
     return AnonymousUser(**kwargs)
 
 
 def create_group(name, user=None):
     from django.contrib.auth.models import Group
+
     group = Group.objects.create(name=name)
     if user is not None:
         user.groups.add(group)
         user.save()
     group.save()
     return group
 
 
 def create_article(title, user=None, bridge=None):
     import datetime
+
     from permission.tests.models import Article
+
     user = user or create_user(str(datetime.datetime.now()))
     article = Article.objects.create(
-        title=title,
-        content=title*20,
-        author=user,
-        single_bridge=bridge
+        title=title, content=title * 20, author=user, single_bridge=bridge
     )
     article.save()
     return article
 
 
 def create_bridge(user=None, editors=None):
     import datetime
+
     from permission.tests.models import Bridge
+
     user = user or create_user(str(datetime.datetime.now()))
-    editors = editors or [create_user(str(datetime.datetime.now())+str(i))
-                          for i in range(2)]
+    editors = editors or [
+        create_user(str(datetime.datetime.now()) + str(i)) for i in range(2)
+    ]
     bridge = Bridge.objects.create(author=user)
     for editor in editors:
         bridge.editors.add(editor)
     bridge.save()
     return bridge
 
 
 def create_permission(name, model=None):
     from django.contrib.auth.models import Permission
     from django.contrib.contenttypes.models import ContentType
+
     from permission.tests.models import Article
+
     model = model or Article
     ct = ContentType.objects.get_for_model(model)
-    permission = Permission.objects.create(
-        name=name, codename=name,
-        content_type=ct
-    )
+    permission = Permission.objects.create(name=name, codename=name, content_type=ct)
     permission.save()
     return permission
```

### Comparing `django-permission2-2.0.0b4/src/permission/utils/autodiscover.py` & `django_permission2-2.1.0/src/permission/utils/autodiscover.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # coding=utf-8
 from __future__ import unicode_literals
+
 from django.apps import apps
 
 
 def autodiscover(module_name=None):
     """
     Autodiscover INSTALLED_APPS perms.py modules and fail silently when not
     present. This forces an import on them to register any permissions bits
     they may want.
     """
     from django.utils.module_loading import module_has_submodule
+
     from permission.compat import import_module
     from permission.conf import settings
 
     module_name = module_name or settings.PERMISSION_AUTODISCOVER_MODULE_NAME
     app_names = (app.name for app in apps.app_configs.values())
 
     for app in app_names:
@@ -45,27 +47,26 @@
         )
 
     Use this method to apply the permission logics enumerated in
     ``PERMISSION_LOGICS`` variable like:
 
         >>> discover('your_app')
     """
-    from permission.compat import import_module
-    from permission.compat import get_model
+    from permission.compat import get_model, import_module
     from permission.conf import settings
     from permission.utils.logics import add_permission_logic
 
     variable_name = settings.PERMISSION_AUTODISCOVER_VARIABLE_NAME
     module_name = module_name or settings.PERMISSION_AUTODISCOVER_MODULE_NAME
 
     # import the module
-    m = import_module('%s.%s' % (app, module_name))
+    m = import_module("%s.%s" % (app, module_name))
 
     # check if the module have PERMISSION_LOGICS variable
     if hasattr(m, variable_name):
         # apply permission logics automatically
         permission_logic_set = getattr(m, variable_name)
         for model, permission_logic in permission_logic_set:
             if isinstance(model, str):
                 # convert model string to model instance
-                model = get_model(*model.split('.', 1))
+                model = get_model(*model.split(".", 1))
             add_permission_logic(model, permission_logic)
```

### Comparing `django-permission2-2.0.0b4/src/permission/utils/field_lookup.py` & `django_permission2-2.1.0/src/permission/utils/field_lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """A module to lookup field of object."""
 from __future__ import unicode_literals
+
 from collections.abc import Iterable
 
 
 def field_lookup(obj, field_path):
     """
     Lookup django model field in similar way of django query lookup.
 
@@ -25,16 +26,16 @@
         ...                                  author=user)
         >>> article.editors.add(user)
         >>> assert 'test_article' == field_lookup(article, 'title')
         >>> assert 'test_user' == field_lookup(article, 'user__username')
         >>> assert ['test_user'] == list(field_lookup(article,
         ...                                           'editors__username'))
     """
-    if hasattr(obj, 'iterator'):
+    if hasattr(obj, "iterator"):
         return (field_lookup(x, field_path) for x in obj.iterator())
     elif isinstance(obj, Iterable):
         return (field_lookup(x, field_path) for x in iter(obj))
     # split the path
-    field_path = field_path.split('__', 1)
+    field_path = field_path.split("__", 1)
     if len(field_path) == 1:
         return getattr(obj, field_path[0], None)
     return field_lookup(field_lookup(obj, field_path[0]), field_path[1])
```

### Comparing `django-permission2-2.0.0b4/src/permission/utils/handlers.py` & `django_permission2-2.1.0/src/permission/utils/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # coding=utf-8
 """
 A utilities of permission handler
 """
 from __future__ import unicode_literals
+
 import inspect
+
 from django.core.exceptions import ImproperlyConfigured
+
+from permission.compat import import_string, isstr
 from permission.conf import settings
-from permission.compat import isstr
-from permission.compat import import_string
 
 
 class PermissionHandlerRegistry(object):
     """
     A registry class of permission handler
     """
+
     def __init__(self):
         self._registry = {}
 
     def register(self, model, handler=None):
         """
         Register a permission handler to the model
 
@@ -33,33 +36,37 @@
         ImproperlyConfigured
             Raise when the model is abstract model
         KeyError
             Raise when the model is already registered in registry
             The model cannot have more than one handler.
         """
         from permission.handlers import PermissionHandler
+
         if model._meta.abstract:
             raise ImproperlyConfigured(
-                    'The model %s is abstract, so it cannot be registered '
-                    'with permission.' % model)
+                "The model %s is abstract, so it cannot be registered "
+                "with permission." % model
+            )
         if model in self._registry:
-            raise KeyError("A permission handler class is already "
-                            "registered for '%s'" % model)
+            raise KeyError(
+                "A permission handler class is already " "registered for '%s'" % model
+            )
         if handler is None:
             handler = settings.PERMISSION_DEFAULT_PERMISSION_HANDLER
         if isstr(handler):
             handler = import_string(handler)
         if not inspect.isclass(handler):
             raise AttributeError(
-                    "`handler` attribute must be a class. "
-                    "An instance was specified.")
+                "`handler` attribute must be a class. " "An instance was specified."
+            )
         if not issubclass(handler, PermissionHandler):
             raise AttributeError(
-                    "`handler` attribute must be a subclass of "
-                    "`permission.handlers.PermissionHandler`")
+                "`handler` attribute must be a subclass of "
+                "`permission.handlers.PermissionHandler`"
+            )
 
         # Instantiate the handler to save in the registry
         instance = handler(model)
         self._registry[model] = instance
 
     def unregister(self, model):
         """
@@ -72,25 +79,28 @@
 
         Raises
         ------
         KeyError
             Raise when the model have not registered in registry yet.
         """
         if model not in self._registry:
-            raise KeyError("A permission handler class have not been "
-                           "registered for '%s' yet" % model)
+            raise KeyError(
+                "A permission handler class have not been "
+                "registered for '%s' yet" % model
+            )
         # remove from registry
         del self._registry[model]
 
     def get_handlers(self):
         """
         Get registered handler instances
 
         Returns
         -------
         tuple
             permission handler tuple
         """
         return tuple(self._registry.values())
 
+
+# Permission handler registry instance
 registry = PermissionHandlerRegistry()
-"""Permission handler registry instance"""
```

### Comparing `django-permission2-2.0.0b4/src/permission/utils/logics.py` & `django_permission2-2.1.0/src/permission/utils/logics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding=utf-8
 """
 Permission logic utilities
 """
 from __future__ import unicode_literals
+
 from permission.logics import PermissionLogic
 
 
 def add_permission_logic(model, permission_logic):
     """
     Add permission logic to the model
 
@@ -25,19 +26,21 @@
     >>> from permission.logics import PermissionLogic
     >>> class Mock(models.Model):
     ...     name = models.CharField('name', max_length=120)
     >>> add_permission_logic(Mock, PermissionLogic())
     """
     if not isinstance(permission_logic, PermissionLogic):
         raise AttributeError(
-        '`permission_logic` must be an instance of PermissionLogic')
-    if not hasattr(model, '_permission_logics'):
+            "`permission_logic` must be an instance of PermissionLogic"
+        )
+    if not hasattr(model, "_permission_logics"):
         model._permission_logics = set()
-    if not hasattr(model, '_permission_handler'):
+    if not hasattr(model, "_permission_handler"):
         from permission.utils.handlers import registry
+
         # register default permission handler
         registry.register(model, handler=None)
     model._permission_logics.add(permission_logic)
     # store target model to the permission_logic instance
     permission_logic.model = model
 
 
@@ -63,23 +66,22 @@
     >>> from permission.logics import PermissionLogic
     >>> class Mock(models.Model):
     ...     name = models.CharField('name', max_length=120)
     >>> logic = PermissionLogic()
     >>> add_permission_logic(Mock, logic)
     >>> remove_permission_logic(Mock, logic)
     """
-    if not hasattr(model, '_permission_logics'):
+    if not hasattr(model, "_permission_logics"):
         model._permission_logics = set()
     if not isinstance(permission_logic, PermissionLogic):
         # remove all permission logic of related
         remove_set = set()
         for _permission_logic in model._permission_logics:
             if _permission_logic.__class__ == permission_logic:
                 remove_set.add(_permission_logic)
         # difference
         model._permission_logics = model._permission_logics.difference(remove_set)
     else:
         if fail_silently and permission_logic not in model._permission_logics:
             pass
         else:
             model._permission_logics.remove(permission_logic)
-
```

### Comparing `django-permission2-2.0.0b4/src/permission/utils/permissions.py` & `django_permission2-2.1.0/src/permission/utils/permissions.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     'codename_model'
     >>> get_perm_codename('codename')
     'codename'
     >>> get_perm_codename('app_label.app_label.codename_model')
     'app_label.codename_model'
     """
     try:
-        perm = perm.split('.', 1)[1]
+        perm = perm.split(".", 1)[1]
     except IndexError as e:
         if not fail_silently:
             raise e
     return perm
 
 
 def permission_to_perm(permission):
@@ -44,15 +44,15 @@
     ...     codename='add_user',
     ... )
     >>> permission_to_perm(permission)
     'auth.add_user'
     """
     app_label = permission.content_type.app_label
     codename = permission.codename
-    return '%s.%s' % (app_label, codename)
+    return "%s.%s" % (app_label, codename)
 
 
 def perm_to_permission(perm):
     """
     Convert a permission-string to a permission instance.
 
     Examples
@@ -60,25 +60,25 @@
     >>> permission = perm_to_permission('auth.add_user')
     >>> permission.content_type.app_label
     'auth'
     >>> permission.codename
     'add_user'
     """
     from django.contrib.auth.models import Permission
+
     try:
-        app_label, codename = perm.split('.', 1)
+        app_label, codename = perm.split(".", 1)
     except (ValueError, IndexError):
         raise AttributeError(
-            'The format of identifier string permission (perm) is wrong. '
+            "The format of identifier string permission (perm) is wrong. "
             "It should be in 'app_label.codename'."
         )
     else:
         permission = Permission.objects.get(
-            content_type__app_label=app_label,
-            codename=codename
+            content_type__app_label=app_label, codename=codename
         )
         return permission
 
 
 def get_app_perms(model_or_app_label):
     """
     Get permission-string list of the specified django application.
@@ -98,21 +98,22 @@
     --------
     >>> perms1 = get_app_perms('auth')
     >>> perms2 = get_app_perms(Permission)
     >>> perms1 == perms2
     True
     """
     from django.contrib.auth.models import Permission
+
     if isinstance(model_or_app_label, str):
         app_label = model_or_app_label
     else:
         # assume model_or_app_label is model class
         app_label = model_or_app_label._meta.app_label
     qs = Permission.objects.filter(content_type__app_label=app_label)
-    perms = ('%s.%s' % (app_label, p.codename) for p in qs.iterator())
+    perms = ("%s.%s" % (app_label, p.codename) for p in qs.iterator())
     return set(perms)
 
 
 def get_model_perms(model):
     """
     Get permission-string list of a specified django model.
 
@@ -132,13 +133,15 @@
     ...     'auth.add_permission',
     ...     'auth.change_permission',
     ...     'auth.delete_permission'
     ... ]
     True
     """
     from django.contrib.auth.models import Permission
+
     app_label = model._meta.app_label
     model_name = model._meta.object_name.lower()
-    qs = Permission.objects.filter(content_type__app_label=app_label,
-                                   content_type__model=model_name)
-    perms = ('%s.%s' % (app_label, p.codename) for p in qs.iterator())
+    qs = Permission.objects.filter(
+        content_type__app_label=app_label, content_type__model=model_name
+    )
+    perms = ("%s.%s" % (app_label, p.codename) for p in qs.iterator())
     return set(perms)
```

