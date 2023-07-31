# Comparing `tmp/carburetor-4.1.1.tar.gz` & `tmp/carburetor-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carburetor-4.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "carburetor-4.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `carburetor-4.1.1.tar` & `carburetor-4.1.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1379 2023-07-26 15:35:37.146394 carburetor-4.1.1/.gitignore
--rw-r--r--   0        0        0     1328 2023-07-26 15:35:37.146394 carburetor-4.1.1/.gitlab-ci.yml
--rw-r--r--   0        0        0     2086 2023-07-26 15:35:37.146394 carburetor-4.1.1/CHANGELOG
--rw-r--r--   0        0        0     1041 2023-07-26 15:35:37.146394 carburetor-4.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    35079 2023-07-26 15:35:37.146394 carburetor-4.1.1/LICENSE
--rw-r--r--   0        0        0      112 2023-07-26 15:35:37.146394 carburetor-4.1.1/MANIFEST.in
--rw-r--r--   0        0        0     1060 2023-07-26 15:35:37.146394 carburetor-4.1.1/README.md
--rw-r--r--   0        0        0      934 2023-07-26 15:35:37.146394 carburetor-4.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 15:35:37.174394 carburetor-4.1.1/src/carburetor/__init__.py
--rw-r--r--   0        0        0     6779 2023-07-26 15:35:37.146394 carburetor-4.1.1/src/carburetor/actions.py
--rwxr-xr-x   0        0        0     1142 2023-07-26 15:35:37.146394 carburetor-4.1.1/src/carburetor/carburetor.py
--rw-r--r--   0        0        0      972 2023-07-26 15:35:37.146394 carburetor-4.1.1/src/carburetor/config.py
--rw-r--r--   0        0        0      508 2023-07-26 15:35:37.146394 carburetor-4.1.1/src/carburetor/desktop/carburetor.1
--rw-r--r--   0        0        0    14735 2023-07-26 15:35:37.146394 carburetor-4.1.1/src/carburetor/desktop/carburetor.svg
--rw-r--r--   0        0        0      593 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/desktop/io.frama.tractor.carburetor.desktop
--rw-r--r--   0        0        0     3435 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/desktop/io.frama.tractor.carburetor.metainfo.xml
--rw-r--r--   0        0        0     6963 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/handler.py
--rw-r--r--   0        0        0     5283 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/carburetor.pot
--rw-r--r--   0        0        0     4459 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/de/LC_MESSAGES/carburetor.mo
--rw-r--r--   0        0        0     7992 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/de/LC_MESSAGES/carburetor.po
--rw-r--r--   0        0        0     2556 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/el/LC_MESSAGES/carburetor.mo
--rw-r--r--   0        0        0     8714 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/el/LC_MESSAGES/carburetor.po
--rw-r--r--   0        0        0     4401 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/es/LC_MESSAGES/carburetor.mo
--rw-r--r--   0        0        0     7949 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/es/LC_MESSAGES/carburetor.po
--rw-r--r--   0        0        0     5075 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/fa/LC_MESSAGES/carburetor.mo
--rw-r--r--   0        0        0     8676 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/fa/LC_MESSAGES/carburetor.po
--rw-r--r--   0        0        0     4372 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/fr/LC_MESSAGES/carburetor.mo
--rw-r--r--   0        0        0     7836 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/fr/LC_MESSAGES/carburetor.po
--rw-r--r--   0        0        0     4436 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/hr/LC_MESSAGES/carburetor.mo
--rw-r--r--   0        0        0     7744 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/hr/LC_MESSAGES/carburetor.po
--rw-r--r--   0        0        0     4253 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.mo
--rw-r--r--   0        0        0     7599 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.po
--rw-r--r--   0        0        0     4395 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/nl/LC_MESSAGES/carburetor.mo
--rw-r--r--   0        0        0     6706 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/nl/LC_MESSAGES/carburetor.po
--rw-r--r--   0        0        0     3300 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/pl/LC_MESSAGES/carburetor.mo
--rw-r--r--   0        0        0     7281 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/pl/LC_MESSAGES/carburetor.po
--rw-r--r--   0        0        0     4479 2023-07-26 15:35:37.150394 carburetor-4.1.1/src/carburetor/locales/pt/LC_MESSAGES/carburetor.mo
--rw-r--r--   0        0        0     7917 2023-07-26 15:35:37.154394 carburetor-4.1.1/src/carburetor/locales/pt/LC_MESSAGES/carburetor.po
--rw-r--r--   0        0        0     3921 2023-07-26 15:35:37.154394 carburetor-4.1.1/src/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.mo
--rw-r--r--   0        0        0     7864 2023-07-26 15:35:37.154394 carburetor-4.1.1/src/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.po
--rw-r--r--   0        0        0     4462 2023-07-26 15:35:37.154394 carburetor-4.1.1/src/carburetor/locales/tr/LC_MESSAGES/carburetor.mo
--rw-r--r--   0        0        0     7936 2023-07-26 15:35:37.154394 carburetor-4.1.1/src/carburetor/locales/tr/LC_MESSAGES/carburetor.po
--rw-r--r--   0        0        0     3608 2023-07-26 15:35:37.154394 carburetor-4.1.1/src/carburetor/tasks.py
--rw-r--r--   0        0        0      994 2023-07-26 15:35:37.154394 carburetor-4.1.1/src/carburetor/ui.py
--rw-r--r--   0        0        0     1903 2023-07-26 15:35:37.154394 carburetor-4.1.1/src/carburetor/ui/about.ui
--rw-r--r--   0        0        0     5162 2023-07-26 15:35:37.154394 carburetor-4.1.1/src/carburetor/ui/main.ui
--rw-r--r--   0        0        0    10821 2023-07-26 15:35:37.154394 carburetor-4.1.1/src/carburetor/ui/preferences.ui
--rw-r--r--   0        0        0      114 2023-07-26 15:35:37.154394 carburetor-4.1.1/src/carburetor/ui/style.css
--rwxr-xr-x   0        0        0      366 2023-07-26 15:35:37.154394 carburetor-4.1.1/update_pot
--rw-r--r--   0        0        0     1794 1970-01-01 00:00:00.000000 carburetor-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1379 2023-07-31 14:15:02.292286 carburetor-4.1.2/.gitignore
+-rw-r--r--   0        0        0     1328 2023-07-31 14:15:02.292286 carburetor-4.1.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2140 2023-07-31 14:15:02.292286 carburetor-4.1.2/CHANGELOG
+-rw-r--r--   0        0        0     1041 2023-07-31 14:15:02.292286 carburetor-4.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    35079 2023-07-31 14:15:02.292286 carburetor-4.1.2/LICENSE
+-rw-r--r--   0        0        0      124 2023-07-31 14:15:02.292286 carburetor-4.1.2/MANIFEST.in
+-rw-r--r--   0        0        0     1060 2023-07-31 14:15:02.292286 carburetor-4.1.2/README.md
+-rw-r--r--   0        0        0      934 2023-07-31 14:15:02.292286 carburetor-4.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 14:17:21.154301 carburetor-4.1.2/src/carburetor/__init__.py
+-rw-r--r--   0        0        0     6779 2023-07-31 14:15:02.292286 carburetor-4.1.2/src/carburetor/actions.py
+-rwxr-xr-x   0        0        0     1142 2023-07-31 14:15:02.292286 carburetor-4.1.2/src/carburetor/carburetor.py
+-rw-r--r--   0        0        0      972 2023-07-31 14:15:02.292286 carburetor-4.1.2/src/carburetor/config.py
+-rw-r--r--   0        0        0      508 2023-07-31 14:15:02.292286 carburetor-4.1.2/src/carburetor/desktop/carburetor.1
+-rw-r--r--   0        0        0    14735 2023-07-31 14:15:02.292286 carburetor-4.1.2/src/carburetor/desktop/carburetor.svg
+-rw-r--r--   0        0        0      593 2023-07-31 14:15:02.292286 carburetor-4.1.2/src/carburetor/desktop/io.frama.tractor.carburetor.desktop
+-rw-r--r--   0        0        0     3435 2023-07-31 14:15:02.292286 carburetor-4.1.2/src/carburetor/desktop/io.frama.tractor.carburetor.metainfo.xml
+-rw-r--r--   0        0        0     6963 2023-07-31 14:15:02.292286 carburetor-4.1.2/src/carburetor/handler.py
+-rw-r--r--   0        0        0     5283 2023-07-31 14:15:02.292286 carburetor-4.1.2/src/carburetor/locales/carburetor.pot
+-rw-r--r--   0        0        0     4459 2023-07-31 14:15:02.292286 carburetor-4.1.2/src/carburetor/locales/de/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7992 2023-07-31 14:15:02.292286 carburetor-4.1.2/src/carburetor/locales/de/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     2556 2023-07-31 14:15:02.292286 carburetor-4.1.2/src/carburetor/locales/el/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     8714 2023-07-31 14:15:02.292286 carburetor-4.1.2/src/carburetor/locales/el/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     4401 2023-07-31 14:15:02.292286 carburetor-4.1.2/src/carburetor/locales/es/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7949 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/es/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     5075 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/fa/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     8676 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/fa/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     4372 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/fr/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7836 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/fr/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     4436 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/hr/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7744 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/hr/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     4253 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7599 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     4395 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/nl/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     6706 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/nl/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     3300 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/pl/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7281 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/pl/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     4479 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/pt/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7917 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/pt/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     3921 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7864 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     4462 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/tr/LC_MESSAGES/carburetor.mo
+-rw-r--r--   0        0        0     7936 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/locales/tr/LC_MESSAGES/carburetor.po
+-rw-r--r--   0        0        0     3608 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/tasks.py
+-rw-r--r--   0        0        0      994 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/ui.py
+-rw-r--r--   0        0        0     1903 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/ui/about.ui
+-rw-r--r--   0        0        0     5162 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/ui/main.ui
+-rw-r--r--   0        0        0    10821 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/ui/preferences.ui
+-rw-r--r--   0        0        0      114 2023-07-31 14:15:02.296286 carburetor-4.1.2/src/carburetor/ui/style.css
+-rwxr-xr-x   0        0        0      366 2023-07-31 14:15:02.296286 carburetor-4.1.2/update_pot
+-rw-r--r--   0        0        0     1794 1970-01-01 00:00:00.000000 carburetor-4.1.2/PKG-INFO
```

### Comparing `carburetor-4.1.1/.gitignore` & `carburetor-4.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/.gitlab-ci.yml` & `carburetor-4.1.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/CHANGELOG` & `carburetor-4.1.2/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+carburetor (4.1.2) 31 Jul 2023
+  * Update Manifest.in
+
 carburetor (4.1.1) 26 Jul 2023
   * Use src-layout
 
-
 carburetor (4.1.0) 26 Jul 2023
   * Change app id to comply with GNOME rules
   * Move to AdwAboutWindow
   * Migrate to PyProject
   * Update translations
 
 carburetor (4.0.3) 22 Mar 2023
```

### Comparing `carburetor-4.1.1/CONTRIBUTING.md` & `carburetor-4.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/LICENSE` & `carburetor-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/README.md` & `carburetor-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/pyproject.toml` & `carburetor-4.1.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "carburetor"
-version = "4.1.1"
+version = "4.1.2"
 authors = [
     {name = "Danial Behzadi", email = "dani.behzi@ubuntu.com"},
 ]
 description = "GTK frontend for Tractor"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `carburetor-4.1.1/src/carburetor/actions.py` & `carburetor-4.1.2/src/carburetor/actions.py`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/carburetor.py` & `carburetor-4.1.2/src/carburetor/carburetor.py`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/config.py` & `carburetor-4.1.2/src/carburetor/config.py`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/desktop/carburetor.svg` & `carburetor-4.1.2/src/carburetor/desktop/carburetor.svg`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/desktop/io.frama.tractor.carburetor.desktop` & `carburetor-4.1.2/src/carburetor/desktop/io.frama.tractor.carburetor.desktop`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/desktop/io.frama.tractor.carburetor.metainfo.xml` & `carburetor-4.1.2/src/carburetor/desktop/io.frama.tractor.carburetor.metainfo.xml`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/handler.py` & `carburetor-4.1.2/src/carburetor/handler.py`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/carburetor.pot` & `carburetor-4.1.2/src/carburetor/locales/carburetor.pot`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/de/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.2/src/carburetor/locales/de/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/de/LC_MESSAGES/carburetor.po` & `carburetor-4.1.2/src/carburetor/locales/de/LC_MESSAGES/carburetor.po`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/el/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.2/src/carburetor/locales/el/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/el/LC_MESSAGES/carburetor.po` & `carburetor-4.1.2/src/carburetor/locales/el/LC_MESSAGES/carburetor.po`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/es/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.2/src/carburetor/locales/es/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/es/LC_MESSAGES/carburetor.po` & `carburetor-4.1.2/src/carburetor/locales/es/LC_MESSAGES/carburetor.po`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/fa/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.2/src/carburetor/locales/fa/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/fa/LC_MESSAGES/carburetor.po` & `carburetor-4.1.2/src/carburetor/locales/fa/LC_MESSAGES/carburetor.po`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/fr/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.2/src/carburetor/locales/fr/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/fr/LC_MESSAGES/carburetor.po` & `carburetor-4.1.2/src/carburetor/locales/fr/LC_MESSAGES/carburetor.po`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/hr/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.2/src/carburetor/locales/hr/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/hr/LC_MESSAGES/carburetor.po` & `carburetor-4.1.2/src/carburetor/locales/hr/LC_MESSAGES/carburetor.po`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.2/src/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.po` & `carburetor-4.1.2/src/carburetor/locales/nb_NO/LC_MESSAGES/carburetor.po`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/nl/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.2/src/carburetor/locales/nl/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/nl/LC_MESSAGES/carburetor.po` & `carburetor-4.1.2/src/carburetor/locales/nl/LC_MESSAGES/carburetor.po`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/pl/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.2/src/carburetor/locales/pl/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/pl/LC_MESSAGES/carburetor.po` & `carburetor-4.1.2/src/carburetor/locales/pl/LC_MESSAGES/carburetor.po`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/pt/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.2/src/carburetor/locales/pt/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/pt/LC_MESSAGES/carburetor.po` & `carburetor-4.1.2/src/carburetor/locales/pt/LC_MESSAGES/carburetor.po`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.2/src/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.po` & `carburetor-4.1.2/src/carburetor/locales/pt_BR/LC_MESSAGES/carburetor.po`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/tr/LC_MESSAGES/carburetor.mo` & `carburetor-4.1.2/src/carburetor/locales/tr/LC_MESSAGES/carburetor.mo`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/locales/tr/LC_MESSAGES/carburetor.po` & `carburetor-4.1.2/src/carburetor/locales/tr/LC_MESSAGES/carburetor.po`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/tasks.py` & `carburetor-4.1.2/src/carburetor/tasks.py`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/ui.py` & `carburetor-4.1.2/src/carburetor/ui.py`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/ui/about.ui` & `carburetor-4.1.2/src/carburetor/ui/about.ui`

 * *Files 1% similar despite different names*

#### Comparing `carburetor-4.1.1/src/carburetor/ui/about.ui` & `carburetor-4.1.2/src/carburetor/ui/about.ui`

```diff
@@ -24,12 +24,12 @@
     <property name="comments" translatable="yes">GTK frontend for Tractor</property>
     <property name="copyright" translatable="yes">Copyright © 2019-2023, Tractor Team</property>
     <property name="developers">Danial Behzadi &lt;dani.behzi@ubuntu.com&gt;</property>
     <property name="hide-on-close">True</property>
     <property name="issue-url">https://framagit.org/tractor/carburetor/issues/new</property>
     <property name="license-type">gpl-3-0</property>
     <property name="modal">True</property>
-    <property name="version">4.1.1</property>
+    <property name="version">4.1.2</property>
     <property name="website">https://framagit.org/tractor/carburetor</property>
     <signal name="realize" handler="on_about_realize"/>
   </object>
 </interface>
```

### Comparing `carburetor-4.1.1/src/carburetor/ui/main.ui` & `carburetor-4.1.2/src/carburetor/ui/main.ui`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/src/carburetor/ui/preferences.ui` & `carburetor-4.1.2/src/carburetor/ui/preferences.ui`

 * *Files identical despite different names*

### Comparing `carburetor-4.1.1/PKG-INFO` & `carburetor-4.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carburetor
-Version: 4.1.1
+Version: 4.1.2
 Summary: GTK frontend for Tractor
 Keywords: Tor,onion,stem
 Author-email: Danial Behzadi <dani.behzi@ubuntu.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

