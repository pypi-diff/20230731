# Comparing `tmp/session-repository-0.3.3.tar.gz` & `tmp/session-repository-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "session-repository-0.3.3.tar", last modified: Mon Jul 24 19:18:07 2023, max compression
+gzip compressed data, was "session-repository-0.3.4.tar", last modified: Mon Jul 31 17:28:14 2023, max compression
```

## Comparing `session-repository-0.3.3.tar` & `session-repository-0.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 19:18:07.472547 session-repository-0.3.3/
--rw-rw-rw-   0        0        0      599 2023-07-24 19:18:07.447488 session-repository-0.3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-24 19:18:07.294151 session-repository-0.3.3/session_repository/
--rw-rw-rw-   0        0        0      191 2023-07-18 08:45:38.000000 session-repository-0.3.3/session_repository/__init__.py
--rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.3.3/session_repository/enum.py
-drwxrwxrwx   0        0        0        0 2023-07-24 19:18:07.440371 session-repository-0.3.3/session_repository/models/
--rw-rw-rw-   0        0        0     9559 2023-07-24 16:33:49.000000 session-repository-0.3.3/session_repository/models/repository.py
--rw-rw-rw-   0        0        0      496 2023-07-18 09:04:38.000000 session-repository-0.3.3/session_repository/models/service.py
--rw-rw-rw-   0        0        0     9582 2023-07-24 19:16:34.000000 session-repository-0.3.3/session_repository/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-24 19:18:07.418950 session-repository-0.3.3/session_repository.egg-info/
--rw-rw-rw-   0        0        0      599 2023-07-24 19:18:06.000000 session-repository-0.3.3/session_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-07-24 19:18:06.000000 session-repository-0.3.3/session_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 19:18:06.000000 session-repository-0.3.3/session_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-24 19:18:06.000000 session-repository-0.3.3/session_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-24 19:18:06.000000 session-repository-0.3.3/session_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 19:18:07.473557 session-repository-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      877 2023-07-24 19:17:00.000000 session-repository-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:28:14.665337 session-repository-0.3.4/
+-rw-rw-rw-   0        0        0      599 2023-07-31 17:28:14.663303 session-repository-0.3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-31 17:28:14.626177 session-repository-0.3.4/session_repository/
+-rw-rw-rw-   0        0        0      191 2023-07-18 08:45:38.000000 session-repository-0.3.4/session_repository/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-07-13 16:45:09.000000 session-repository-0.3.4/session_repository/enum.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:28:14.658902 session-repository-0.3.4/session_repository/models/
+-rw-rw-rw-   0        0        0     9768 2023-07-31 17:27:35.000000 session-repository-0.3.4/session_repository/models/repository.py
+-rw-rw-rw-   0        0        0      496 2023-07-18 09:04:38.000000 session-repository-0.3.4/session_repository/models/service.py
+-rw-rw-rw-   0        0        0     9582 2023-07-24 19:16:34.000000 session-repository-0.3.4/session_repository/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:28:14.649918 session-repository-0.3.4/session_repository.egg-info/
+-rw-rw-rw-   0        0        0      599 2023-07-31 17:28:14.000000 session-repository-0.3.4/session_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-07-31 17:28:14.000000 session-repository-0.3.4/session_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 17:28:14.000000 session-repository-0.3.4/session_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-31 17:28:14.000000 session-repository-0.3.4/session_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-31 17:28:14.000000 session-repository-0.3.4/session_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 17:28:14.665979 session-repository-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-07-31 17:22:17.000000 session-repository-0.3.4/setup.py
```

### Comparing `session-repository-0.3.3/PKG-INFO` & `session-repository-0.3.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.3.3
+Version: 0.3.4
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.3.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.4.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.3.3/session_repository/enum.py` & `session-repository-0.3.4/session_repository/enum.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.3.3/session_repository/models/repository.py` & `session-repository-0.3.4/session_repository/models/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # MODULES
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TypeVar, Union
 from logging import Logger
 
 # CONNTEXTLIB
 from contextlib import AbstractContextManager
 
 # SQLALCHEMY
+from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import Session, InstrumentedAttribute, Query
 
 # UTILS
 from session_repository.utils import (
     _FilterType,
     apply_no_load,
     apply_filters,
@@ -28,14 +29,17 @@
             kwargs["current_session"] = session
 
             return func(self, *args, **kwargs)
 
     return wrapper
 
 
+T = TypeVar("T", bound=declarative_base())
+
+
 class SessionRepository:
     def __init__(
         self,
         session_factory: Callable[..., AbstractContextManager[Session]],
         logger: Logger,
         literal_binds: bool = True,
     ) -> None:
@@ -62,20 +66,20 @@
 
     def session_manager(self):
         return self._session_factory()
 
     @with_session
     def _select(
         self,
-        model,
+        model: Type[T],
         filters: Optional[_FilterType] = None,
         optional_filters: Optional[_FilterType] = None,
         disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
         current_session: Optional[Session] = None,
-    ) -> Optional[Any]:
+    ) -> Optional[T]:
         query = current_session.query(model)
 
         return self._select_query(
             query=query,
             filters=filters,
             optional_filters=optional_filters,
             disabled_relationships=disabled_relationships,
@@ -110,23 +114,23 @@
         )
 
         return result
 
     @with_session
     def _select_all(
         self,
-        model,
+        model: Type[T],
         filters: Optional[_FilterType] = None,
         optional_filters: Optional[_FilterType] = None,
         disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[str] = None,
         limit: int = None,
         current_session: Optional[Session] = None,
-    ) -> List:
+    ) -> List[T]:
         query = current_session.query(model)
 
         return self._select_all_query(
             query=query,
             model=model,
             filters=filters,
             optional_filters=optional_filters,
@@ -135,22 +139,22 @@
             direction=direction,
             limit=limit,
         )
 
     def _select_all_query(
         self,
         query: Query,
-        model,
+        model: Type[T],
         filters: Optional[_FilterType] = None,
         optional_filters: Optional[_FilterType] = None,
         disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[str] = None,
         limit: int = None,
-    ) -> List:
+    ) -> List[T]:
         query = apply_no_load(
             query=query,
             relationship_dict=disabled_relationships,
         )
         query = apply_filters(
             query=query,
             filter_dict=filters,
@@ -180,25 +184,25 @@
         )
 
         return results
 
     @with_session
     def _select_paginate(
         self,
-        model,
+        model: Type[T],
         page: int,
         per_page: int,
         filters: Optional[_FilterType] = None,
         optional_filters: Optional[_FilterType] = None,
         disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[str] = None,
         limit: int = None,
         current_session: Optional[Session] = None,
-    ) -> Tuple[List, str]:
+    ) -> Tuple[List[T], str]:
         query = current_session.query(model)
 
         return self._select_paginate_query(
             query=query,
             model=model,
             page=page,
             per_page=per_page,
@@ -209,24 +213,24 @@
             direction=direction,
             limit=limit,
         )
 
     def _select_paginate_query(
         self,
         query: Query,
-        model,
+        model: Type[T],
         page: int,
         per_page: int,
         filters: Optional[_FilterType] = None,
         optional_filters: Optional[_FilterType] = None,
         disabled_relationships: Optional[Dict[InstrumentedAttribute, Any]] = None,
         order_by: Optional[Union[List[str], str]] = None,
         direction: Optional[str] = None,
         limit: int = None,
-    ) -> Tuple[List, str]:
+    ) -> Tuple[List[T], str]:
         query = apply_no_load(
             query=query,
             relationship_dict=disabled_relationships,
         )
         query = apply_filters(
             query=query,
             filter_dict=filters,
@@ -261,21 +265,21 @@
         )
 
         return results, pagination
 
     @with_session
     def _update(
         self,
-        model,
+        model: Type[T],
         values: Dict,
         filters: Optional[_FilterType] = None,
         flush: bool = False,
         commit: bool = False,
         current_session: Optional[Session] = None,
-    ) -> List:
+    ) -> List[T]:
         rows = self._select_all(
             model=model,
             filters=filters,
             current_session=current_session,
         )
 
         if len(rows) == 0:
@@ -293,15 +297,15 @@
         [current_session.refresh(row) for row in rows]
 
         return rows
 
     @with_session
     def _add(
         self,
-        data,
+        data: Union[List[T], T],
         flush: bool = False,
         commit: bool = False,
         current_session: Optional[Session] = None,
     ) -> Union[List, Any]:
         current_session.add_all(data) if isinstance(
             data, list
         ) else current_session.add(data)
@@ -314,15 +318,15 @@
             current_session.refresh(data)
 
         return data
 
     @with_session
     def _delete(
         self,
-        model,
+        model: T,
         filters: Optional[_FilterType] = None,
         flush: bool = True,
         commit: bool = False,
         current_session: Optional[Session] = None,
     ) -> bool:
         rows: List = self._select_all(
             model=model,
```

### Comparing `session-repository-0.3.3/session_repository/utils.py` & `session-repository-0.3.4/session_repository/utils.py`

 * *Files identical despite different names*

### Comparing `session-repository-0.3.3/session_repository.egg-info/PKG-INFO` & `session-repository-0.3.4/session_repository.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: session-repository
-Version: 0.3.3
+Version: 0.3.4
 Summary: A project to have a base repository class to permform select/insert/update/delete with dynamtic syntaxe
 Home-page: https://github.com/Impro02/session-repository
-Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.3.tar.gz
+Download-URL: https://github.com/Impro02/session-repository/archive/refs/tags/0.3.4.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `session-repository-0.3.3/setup.py` & `session-repository-0.3.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.3"
+version = "0.3.4"
 
 setup(
     name="session-repository",
     version=version,
     packages=[
         "session_repository",
         "session_repository.models",
```

