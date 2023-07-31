# Comparing `tmp/pih-mio-1.48014.tar.gz` & `tmp/pih-mio-1.48016.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48014.tar", last modified: Fri Jul 28 13:50:18 2023, max compression
+gzip compressed data, was "pih-mio-1.48016.tar", last modified: Mon Jul 31 08:46:10 2023, max compression
```

## Comparing `pih-mio-1.48014.tar` & `pih-mio-1.48016.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 13:50:17.175657 pih-mio-1.48014/
-drwxrwxrwx   0        0        0        0 2023-07-28 13:50:17.675640 pih-mio-1.48014/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48014/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48014/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165319 2023-07-28 13:49:12.000000 pih-mio-1.48014/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48014/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9431 2023-07-28 13:39:51.000000 pih-mio-1.48014/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48014/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-07-28 13:50:18.284998 pih-mio-1.48014/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 13:50:18.238127 pih-mio-1.48014/pih_MIO.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-28 13:50:16.000000 pih-mio-1.48014/pih_MIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-07-28 13:50:17.000000 pih-mio-1.48014/pih_MIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 13:50:16.000000 pih-mio-1.48014/pih_MIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-07-28 13:50:16.000000 pih-mio-1.48014/pih_MIO.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-07-28 13:50:16.000000 pih-mio-1.48014/pih_MIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 13:50:16.000000 pih-mio-1.48014/pih_MIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-mio-1.48014/pih_mio_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-28 13:50:18.284998 pih-mio-1.48014/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 08:46:09.922616 pih-mio-1.48016/
+drwxrwxrwx   0        0        0        0 2023-07-31 08:46:09.953856 pih-mio-1.48016/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48016/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48016/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165320 2023-07-31 03:28:09.000000 pih-mio-1.48016/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48016/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9431 2023-07-28 13:39:51.000000 pih-mio-1.48016/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48016/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-07-31 08:46:10.564175 pih-mio-1.48016/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-31 08:46:10.501675 pih-mio-1.48016/pih_MIO.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-07-31 08:46:08.000000 pih-mio-1.48016/pih_MIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-07-31 08:46:09.000000 pih-mio-1.48016/pih_MIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 08:46:08.000000 pih-mio-1.48016/pih_MIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-07-31 08:46:09.000000 pih-mio-1.48016/pih_MIO.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-31 08:46:09.000000 pih-mio-1.48016/pih_MIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-31 08:46:09.000000 pih-mio-1.48016/pih_MIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-mio-1.48016/pih_mio_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-31 08:46:10.579800 pih-mio-1.48016/setup.cfg
```

### Comparing `pih-mio-1.48014/MobileHelperCore/api.py` & `pih-mio-1.48016/MobileHelperCore/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1961,15 +1961,15 @@
         def sort_function(item: Mark) -> str:
             return item.TabNumber if sort_by_tab_number else item.GroupName
         self.output.write_result(A.R.sort(A.R_M.free_list(False), sort_function), False, title = "Свободные карты доступа:")
 
     def set_or_get_handler(self, get_action: bool = False) -> None:
         with self.output.personalized():
             storage_value_name: str | None = None if self.is_all else (self.arg() or self.input.input("Введите название"))
-            storage_value_holder_list: list[A.CT_S, A.CT_MR.TYPES] = A.D.find_variable(storage_value_name)
+            storage_value_holder_list: list[A.CT_S, A.CT_MR.TYPES] = A.D.find_variables(storage_value_name)
             def sort_function(item: A.CT_S | A.CT_MR.TYPES) -> int:
                 if isinstance(item, A.CT_S):
                     return 0
                 return 1
             storage_value_holder_list = sorted(storage_value_holder_list, key=sort_function)
             def label_function(item: A.CT_S | A.CT_MR.TYPES, _) -> str:
                 name: str = item.name
```

### Comparing `pih-mio-1.48014/MobileHelperCore/service.py` & `pih-mio-1.48016/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48014/MobileHelperCore/service_api.py` & `pih-mio-1.48016/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48014/MobileHelperCore/tools.py` & `pih-mio-1.48016/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48014/pih_MIO.egg-info/SOURCES.txt` & `pih-mio-1.48016/pih_MIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48014/pih_mio_setup.py` & `pih-mio-1.48016/pih_mio_setup.py`

 * *Files identical despite different names*

