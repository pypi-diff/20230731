# Comparing `tmp/sqlx-exec-1.4.1.tar.gz` & `tmp/sqlx-exec-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.4.1.tar", last modified: Sun Jul 30 16:52:12 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.4.2.tar", last modified: Mon Jul 31 11:35:00 2023, max compression
```

## Comparing `sqlx-exec-1.4.1.tar` & `sqlx-exec-1.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.4.1/LICENSE
--rw-rw-rw-   0        0        0     3728 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3143 2023-07-30 08:20:16.000000 sqlx-exec-1.4.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1232 2023-07-30 16:51:57.000000 sqlx-exec-1.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/sqlexec/
--rw-rw-rw-   0        0        0      962 2023-07-30 16:50:50.000000 sqlx-exec-1.4.1/sqlexec/constant.py
--rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.4.1/sqlexec/engine.py
--rw-rw-rw-   0        0        0    14554 2023-07-30 16:50:50.000000 sqlx-exec-1.4.1/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1250 2023-07-30 16:40:52.000000 sqlx-exec-1.4.1/sqlexec/init_import.py
--rw-rw-rw-   0        0        0      989 2023-07-30 14:49:13.000000 sqlx-exec-1.4.1/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.4.1/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1772 2023-07-30 15:17:09.000000 sqlx-exec-1.4.1/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.4.1/sqlexec/support.py
--rw-rw-rw-   0        0        0      446 2023-07-30 15:33:50.000000 sqlx-exec-1.4.1/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.4.1/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3728 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-30 16:52:12.000000 sqlx-exec-1.4.1/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0     3728 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3143 2023-07-30 08:20:16.000000 sqlx-exec-1.4.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2023-07-31 11:21:49.000000 sqlx-exec-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/sqlexec/
+-rw-rw-rw-   0        0        0      962 2023-07-30 16:50:50.000000 sqlx-exec-1.4.2/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.4.2/sqlexec/engine.py
+-rw-rw-rw-   0        0        0    13957 2023-07-31 11:32:07.000000 sqlx-exec-1.4.2/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     2060 2023-07-31 10:39:13.000000 sqlx-exec-1.4.2/sqlexec/init_import.py
+-rw-rw-rw-   0        0        0      989 2023-07-30 14:49:13.000000 sqlx-exec-1.4.2/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.4.2/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1772 2023-07-30 15:17:09.000000 sqlx-exec-1.4.2/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.4.2/sqlexec/support.py
+-rw-rw-rw-   0        0        0      446 2023-07-30 15:33:50.000000 sqlx-exec-1.4.2/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.4.2/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3728 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 11:35:00.000000 sqlx-exec-1.4.2/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.4.1/LICENSE` & `sqlx-exec-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.1/PKG-INFO` & `sqlx-exec-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.4.1
+Version: 1.4.2
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
```

### Comparing `sqlx-exec-1.4.1/README.rst` & `sqlx-exec-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.1/setup.py` & `sqlx-exec-1.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.4.1',
+    version='1.4.2',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.4.1/sqlexec/constant.py` & `sqlx-exec-1.4.2/sqlexec/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.1/sqlexec/engine.py` & `sqlx-exec-1.4.2/sqlexec/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.1/sqlexec/exec.py` & `sqlx-exec-1.4.2/sqlexec/exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import functools
 from . import sql_support
 from .engine import Engine
-from .init_import import import_driver
+from .init_import import import_driver, get_engine
 from .log_support import logger, insert_log, save_log, get_log, sql_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
-from .constant import MYSQL_CONNECTOR_DRIVER, SQLITE, PARAM_DRIVER, PARAM_SHOW_SQL, PARAM_TRANS_PLACEHOLDER, PARAM_DEBUG, PARAM_POOL_SIZE, PARAM_PORT,\
-    MYSQL, POSTGRESQL, UNKNOW, MYSQL_PORT, POSTGRESQL_PORT
+from .constant import MYSQL_CONNECTOR_DRIVER, SQLITE, PARAM_DRIVER, PARAM_SHOW_SQL, PARAM_TRANS_PLACEHOLDER, PARAM_DEBUG, PARAM_POOL_SIZE
 
 _DB_CTX = None
 
 
 def init_db(*args, **kwargs):
     """
     Compliant with the Python DB API 2.0 (PEP-249).
@@ -33,22 +32,15 @@
 
     global _DB_CTX
     pool_size = 0
     driver = kwargs.pop(PARAM_DRIVER) if PARAM_DRIVER in kwargs else None
     show_sql = kwargs.pop(PARAM_SHOW_SQL) if PARAM_SHOW_SQL in kwargs else False
     trans_placeholder = kwargs.pop(PARAM_TRANS_PLACEHOLDER) if PARAM_TRANS_PLACEHOLDER in kwargs else True
 
-    curr_engine = Engine.current_engine()
-    if driver is None and (curr_engine is None or curr_engine == UNKNOW) and PARAM_PORT in kwargs:
-        port = kwargs[PARAM_PORT]
-        if port == MYSQL_PORT:
-            curr_engine = MYSQL
-        elif port == POSTGRESQL_PORT:
-            curr_engine = POSTGRESQL
-
+    curr_engine = get_engine(driver, *args, **kwargs)
     engine, driver, creator = import_driver(driver, curr_engine)
     prepared = MYSQL_CONNECTOR_DRIVER == driver
     if PARAM_DEBUG in kwargs and kwargs.pop(PARAM_DEBUG):
         from logging import DEBUG
         logger.setLevel(DEBUG)
 
     if PARAM_POOL_SIZE in kwargs:
@@ -132,32 +124,21 @@
     @functools.wraps(func)
     def _wrapper(*args, **kw):
         with TransactionCtx(_DB_CTX):
             return func(*args, **kw)
     return _wrapper
 
 
-@with_connection
-def execute(sql: str, *args):
+def execute(sql: str, *args, **kwargs):
     """
     Execute sql return effect rowcount
     sql: insert into person(name, age) values(?, ?)  -->  args: ('张三', 20)
     """
-    global _DB_CTX
-    cursor = None
-    sql = Engine.before_execute_intf('execute', sql.strip(), *args)
-    try:
-        cursor = _DB_CTX.connection.cursor()
-        cursor.execute(sql, args)
-        effect_rowcount = cursor.rowcount
-        try_commit(_DB_CTX)
-        return effect_rowcount
-    finally:
-        if cursor:
-            cursor.close()
+    sql, args = try_mapping('sqlexec.execute', sql, *args, **kwargs)
+    return do_execute(sql, *args)
 
 
 def insert(table: str, **kwargs):
     """
     Insert data into table, return effect rowcount.
     :param table: table name
     :param kwargs: name='张三', age=20}
@@ -234,51 +215,51 @@
 
 def get(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    sql, args = _try_mapping('sqlexec.get', sql, *args, **kwargs)
+    sql, args = try_mapping('sqlexec.get', sql, *args, **kwargs)
     return do_get(sql, *args)
 
 
 def select(sql: str, *args, **kwargs):
     """
     execute select SQL and return unique result or list results(tuple).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
-    sql, args = _try_mapping('sqlexec.select', sql, *args, **kwargs)
+    sql, args = try_mapping('sqlexec.select', sql, *args, **kwargs)
     return do_select(sql, *args)
 
 
 def select_one(sql: str, *args, **kwargs):
     """
     Execute select SQL and return unique result(tuple), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    sql, args = _try_mapping('sqlexec.select_one', sql, *args, **kwargs)
+    sql, args = try_mapping('sqlexec.select_one', sql, *args, **kwargs)
     return do_select_one(sql, *args)
 
 
 def query(sql: str, *args, **kwargs):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
-    sql, args = _try_mapping('sqlexec.query', sql, *args, **kwargs)
+    sql, args = try_mapping('sqlexec.query', sql, *args, **kwargs)
     return do_query(sql, *args)
 
 
 def query_one(sql: str, *args, **kwargs):
     """
     execute select SQL and return unique result(dict), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    sql, args = _try_mapping('sqlexec.query_one', sql, *args, **kwargs)
+    sql, args = try_mapping('sqlexec.query_one', sql, *args, **kwargs)
     return do_query_one(sql, *args)
 
 
 @with_connection
 def do_execute(sql: str, *args):
     """
     Execute sql return effect rowcount
@@ -325,16 +306,16 @@
 
 def do_get(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    get_log('get', sql, *args)
-    result = select_one(sql, *args)
+    get_log('do_get', sql, *args)
+    result = do_select_one(sql, *args)
     if result:
         if len(result) == 1:
             return result[0]
         msg = "Exec func 'sqlexec.%s' expect only one column but %d." % ('do_get', len(result))
         logger.error('%s  \n\t sql: %s \n\t args: %s' % (msg, sql, args))
         raise MultiColumnsError(msg)
     return None
@@ -423,10 +404,10 @@
 
 def get_connection():
     global _DB_CTX
     _DB_CTX.try_init()
     return _DB_CTX.connection
 
 
-def _try_mapping(function, sql, *args, **kwargs):
+def try_mapping(function, sql, *args, **kwargs):
     sql_log(function, sql, *args, **kwargs)
     return sql_support.get_mapping_sql_args(sql, *args, **kwargs)
```

### Comparing `sqlx-exec-1.4.1/sqlexec/log_support.py` & `sqlx-exec-1.4.2/sqlexec/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.1/sqlexec/pooling.py` & `sqlx-exec-1.4.2/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.1/sqlexec/sql_support.py` & `sqlx-exec-1.4.2/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.1/sqlexec/support.py` & `sqlx-exec-1.4.2/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.1/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.4.2/sqlx_exec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.4.1
+Version: 1.4.2
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
```

