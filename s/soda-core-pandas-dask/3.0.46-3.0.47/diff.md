# Comparing `tmp/soda-core-pandas-dask-3.0.46.tar.gz` & `tmp/soda-core-pandas-dask-3.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-pandas-dask-3.0.46.tar", last modified: Wed Jul 19 15:15:48 2023, max compression
+gzip compressed data, was "soda-core-pandas-dask-3.0.47.tar", last modified: Mon Jul 31 08:36:07 2023, max compression
```

## Comparing `soda-core-pandas-dask-3.0.46.tar` & `soda-core-pandas-dask-3.0.47.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:15:48.661539 soda-core-pandas-dask-3.0.46/
--rw-r--r--   0 vijay      (501) staff       (20)       66 2023-07-19 15:15:48.661244 soda-core-pandas-dask-3.0.46/PKG-INFO
--rw-r--r--   0 vijay      (501) staff       (20)       38 2023-07-19 15:15:48.661687 soda-core-pandas-dask-3.0.46/setup.cfg
--rw-r--r--   0 vijay      (501) staff       (20)      619 2023-07-19 13:37:16.000000 soda-core-pandas-dask-3.0.46/setup.py
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:15:48.655096 soda-core-pandas-dask-3.0.46/soda/
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:15:48.657924 soda-core-pandas-dask-3.0.46/soda/data_sources/
--rw-r--r--   0 vijay      (501) staff       (20)      386 2023-06-08 07:54:26.000000 soda-core-pandas-dask-3.0.46/soda/data_sources/dask_connection.py
--rw-r--r--   0 vijay      (501) staff       (20)     2732 2023-06-08 07:54:26.000000 soda-core-pandas-dask-3.0.46/soda/data_sources/dask_cursor.py
--rw-r--r--   0 vijay      (501) staff       (20)    13934 2023-06-08 07:54:26.000000 soda-core-pandas-dask-3.0.46/soda/data_sources/dask_data_source.py
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:15:48.660118 soda-core-pandas-dask-3.0.46/soda_core_pandas_dask.egg-info/
--rw-r--r--   0 vijay      (501) staff       (20)       66 2023-07-19 15:15:48.000000 soda-core-pandas-dask-3.0.46/soda_core_pandas_dask.egg-info/PKG-INFO
--rw-r--r--   0 vijay      (501) staff       (20)      359 2023-07-19 15:15:48.000000 soda-core-pandas-dask-3.0.46/soda_core_pandas_dask.egg-info/SOURCES.txt
--rw-r--r--   0 vijay      (501) staff       (20)        1 2023-07-19 15:15:48.000000 soda-core-pandas-dask-3.0.46/soda_core_pandas_dask.egg-info/dependency_links.txt
--rw-r--r--   0 vijay      (501) staff       (20)       64 2023-07-19 15:15:48.000000 soda-core-pandas-dask-3.0.46/soda_core_pandas_dask.egg-info/requires.txt
--rw-r--r--   0 vijay      (501) staff       (20)        5 2023-07-19 15:15:48.000000 soda-core-pandas-dask-3.0.46/soda_core_pandas_dask.egg-info/top_level.txt
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:15:48.660479 soda-core-pandas-dask-3.0.46/tests/
--rw-r--r--   0 vijay      (501) staff       (20)      139 2023-06-08 07:54:26.000000 soda-core-pandas-dask-3.0.46/tests/test_dask.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:07.623806 soda-core-pandas-dask-3.0.47/
+-rw-r--r--   0 vijay      (501) staff       (20)       66 2023-07-31 08:36:07.623598 soda-core-pandas-dask-3.0.47/PKG-INFO
+-rw-r--r--   0 vijay      (501) staff       (20)       38 2023-07-31 08:36:07.623882 soda-core-pandas-dask-3.0.47/setup.cfg
+-rw-r--r--   0 vijay      (501) staff       (20)      431 2023-07-28 11:01:31.000000 soda-core-pandas-dask-3.0.47/setup.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:07.621248 soda-core-pandas-dask-3.0.47/soda/
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:07.622249 soda-core-pandas-dask-3.0.47/soda/data_sources/
+-rw-r--r--   0 vijay      (501) staff       (20)      386 2023-06-13 14:41:04.000000 soda-core-pandas-dask-3.0.47/soda/data_sources/dask_connection.py
+-rw-r--r--   0 vijay      (501) staff       (20)     2732 2023-06-13 14:41:04.000000 soda-core-pandas-dask-3.0.47/soda/data_sources/dask_cursor.py
+-rw-r--r--   0 vijay      (501) staff       (20)    13940 2023-07-21 13:41:55.000000 soda-core-pandas-dask-3.0.47/soda/data_sources/dask_data_source.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:07.623363 soda-core-pandas-dask-3.0.47/soda_core_pandas_dask.egg-info/
+-rw-r--r--   0 vijay      (501) staff       (20)       66 2023-07-31 08:36:07.000000 soda-core-pandas-dask-3.0.47/soda_core_pandas_dask.egg-info/PKG-INFO
+-rw-r--r--   0 vijay      (501) staff       (20)      340 2023-07-31 08:36:07.000000 soda-core-pandas-dask-3.0.47/soda_core_pandas_dask.egg-info/SOURCES.txt
+-rw-r--r--   0 vijay      (501) staff       (20)        1 2023-07-31 08:36:07.000000 soda-core-pandas-dask-3.0.47/soda_core_pandas_dask.egg-info/dependency_links.txt
+-rw-r--r--   0 vijay      (501) staff       (20)       64 2023-07-31 08:36:07.000000 soda-core-pandas-dask-3.0.47/soda_core_pandas_dask.egg-info/requires.txt
+-rw-r--r--   0 vijay      (501) staff       (20)        5 2023-07-31 08:36:07.000000 soda-core-pandas-dask-3.0.47/soda_core_pandas_dask.egg-info/top_level.txt
```

### Comparing `soda-core-pandas-dask-3.0.46/soda/data_sources/dask_cursor.py` & `soda-core-pandas-dask-3.0.47/soda/data_sources/dask_cursor.py`

 * *Files identical despite different names*

### Comparing `soda-core-pandas-dask-3.0.46/soda/data_sources/dask_data_source.py` & `soda-core-pandas-dask-3.0.47/soda/data_sources/dask_data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
         for table_name in dd_show_tables["Table"].values:
             dd_show_columns_tmp = self.context.sql(f"show columns from {table_name}").compute()
             # Due to a bug in dask-sql we cannot use uppercases in column names
             dd_show_columns_tmp.columns = ["column_name", "data_type", "extra", "comment"]
             dd_show_columns_tmp["table_name"] = table_name
             dd_show_columns_tmp["ordinal_position"] = dd_show_columns_tmp.index + 1
-            dd_show_columns = dd_show_columns.append(dd_show_columns_tmp, ignore_index=True)
+            dd_show_columns = pd.concat([dd_show_columns, dd_show_columns_tmp], ignore_index=True)
 
         self.context.create_table(self.sql_information_schema_columns(), dd_show_columns)
         return super().sql_get_tables_columns_metadata(include_patterns, exclude_patterns, table_names_only)
 
     def sql_get_table_columns(
         self, table_name: str, included_columns: list[str] | None = None, excluded_columns: list[str] | None = None
     ) -> str:
```

