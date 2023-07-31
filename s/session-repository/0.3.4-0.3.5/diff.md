# Comparing `tmp/session-repository-0.3.4.tar.gz` & `tmp/session-repository-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.3.4.tar", last modified: Mon Jul 31 17:28:14 2023, max compression
+gzip compressed data, was "session-repository-0.3.5.tar", last modified: Mon Jul 31 17:32:10 2023, max compression
```

## Comparing `session-repository-0.3.4.tar` & `session-repository-0.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 17:28:14.665337 session-repository-0.3.4/
--rw-rw-rw-   0        0        0      599 2023-07-31 17:28:14.663303 session-repository-0.3.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-31 17:28:14.626177 session-repository-0.3.4/session_repository/
--rw-rw-rw-   0        0        0      191 2023-07-18 08:45:38.000000 session-repository-0.3.4/session_repository/__init__.py
--rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.3.4/session_repository/enum.py
-drwxrwxrwx   0        0        0        0 2023-07-31 17:28:14.658902 session-repository-0.3.4/session_repository/models/
--rw-rw-rw-   0        0        0     9768 2023-07-31 17:27:35.000000 session-repository-0.3.4/session_repository/models/repository.py
--rw-rw-rw-   0        0        0      496 2023-07-18 09:04:38.000000 session-repository-0.3.4/session_repository/models/service.py
--rw-rw-rw-   0        0        0     9582 2023-07-24 19:16:34.000000 session-repository-0.3.4/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 17:28:14.649918 session-repository-0.3.4/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-31 17:28:14.000000 session-repository-0.3.4/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-07-31 17:28:14.000000 session-repository-0.3.4/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 17:28:14.000000 session-repository-0.3.4/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-31 17:28:14.000000 session-repository-0.3.4/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-31 17:28:14.000000 session-repository-0.3.4/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 17:28:14.665979 session-repository-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-07-31 17:22:17.000000 session-repository-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:32:10.596607 session-repository-0.3.5/
+-rw-rw-rw-   0        0        0      599 2023-07-31 17:32:10.595024 session-repository-0.3.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-31 17:32:10.564366 session-repository-0.3.5/session_repository/
+-rw-rw-rw-   0        0        0      191 2023-07-18 08:45:38.000000 session-repository-0.3.5/session_repository/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.3.5/session_repository/enum.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:32:10.591837 session-repository-0.3.5/session_repository/models/
+-rw-rw-rw-   0        0        0     9769 2023-07-31 17:30:42.000000 session-repository-0.3.5/session_repository/models/repository.py
+-rw-rw-rw-   0        0        0      496 2023-07-18 09:04:38.000000 session-repository-0.3.5/session_repository/models/service.py
+-rw-rw-rw-   0        0        0     9582 2023-07-24 19:16:34.000000 session-repository-0.3.5/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:32:10.584137 session-repository-0.3.5/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-31 17:32:10.000000 session-repository-0.3.5/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-07-31 17:32:10.000000 session-repository-0.3.5/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 17:32:10.000000 session-repository-0.3.5/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-31 17:32:10.000000 session-repository-0.3.5/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-31 17:32:10.000000 session-repository-0.3.5/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 17:32:10.598672 session-repository-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-07-31 17:31:55.000000 session-repository-0.3.5/setup.py
```

### Comparing `session-repository-0.3.4/PKG-INFO` & `session-repository-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.3.4
+Version: 0.3.5
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.4.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.5.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.3.4/session_repository/enum.py` & `session-repository-0.3.5/session_repository/enum.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.3.4/session_repository/models/repository.py` & `session-repository-0.3.5/session_repository/models/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
     @with_session
     def _add(
         self,
         data: Union[List[T], T],
         flush: bool = False,
         commit: bool = False,
         current_session: Optional[Session] = None,
-    ) -> Union[List, Any]:
+    ) -> Union[List[T], T]:
         current_session.add_all(data) if isinstance(
             data, list
         ) else current_session.add(data)
         if flush:
             current_session.flush()
         if commit:
             current_session.commit()
```

### Comparing `session-repository-0.3.4/session_repository/utils.py` & `session-repository-0.3.5/session_repository/utils.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.3.4/session_repository.egg-info/PKG-INFO` & `session-repository-0.3.5/session_repository.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.3.4
+Version: 0.3.5
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.4.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.5.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

