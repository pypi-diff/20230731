# Comparing `tmp/sqlx-batis-0.1.9.tar.gz` & `tmp/sqlx-batis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.1.9.tar", last modified: Sun Jul 30 15:52:06 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-0.2.0.tar", last modified: Mon Jul 31 11:36:14 2023, max compression
```

## Comparing `sqlx-batis-0.1.9.tar` & `sqlx-batis-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/
--rw-rw-rw-   0        0        0     5701 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     5018 2023-07-30 08:42:44.000000 sqlx-batis-0.1.9/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1352 2023-07-30 15:51:52.000000 sqlx-batis-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/sqlbatis/
--rw-rw-rw-   0        0        0      894 2023-07-29 06:55:10.000000 sqlx-batis-0.1.9/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     8739 2023-07-30 15:39:23.000000 sqlx-batis-0.1.9/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6885 2023-07-30 15:46:56.000000 sqlx-batis-0.1.9/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0     6383 2023-07-30 01:39:32.000000 sqlx-batis-0.1.9/sqlbatis/engine.py
--rw-rw-rw-   0        0        0     3892 2023-07-30 15:46:56.000000 sqlx-batis-0.1.9/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.1.9/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.1.9/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.1.9/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     5272 2023-07-30 15:49:36.000000 sqlx-batis-0.1.9/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1757 2023-07-30 15:25:21.000000 sqlx-batis-0.1.9/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.1.9/sqlbatis/support.py
--rw-rw-rw-   0        0        0     1627 2023-07-29 10:34:32.000000 sqlx-batis-0.1.9/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-30 06:47:24.000000 sqlx-batis-0.1.9/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     5701 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      465 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 15:52:06.000000 sqlx-batis-0.1.9/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/
+-rw-rw-rw-   0        0        0     5701 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5018 2023-07-30 08:42:44.000000 sqlx-batis-0.2.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1352 2023-07-31 11:35:19.000000 sqlx-batis-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/sqlbatis/
+-rw-rw-rw-   0        0        0      902 2023-07-30 16:13:17.000000 sqlx-batis-0.2.0/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     8588 2023-07-31 11:27:17.000000 sqlx-batis-0.2.0/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6885 2023-07-30 15:46:56.000000 sqlx-batis-0.2.0/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0     6724 2023-07-30 16:13:17.000000 sqlx-batis-0.2.0/sqlbatis/engine.py
+-rw-rw-rw-   0        0        0     3883 2023-07-31 11:35:56.000000 sqlx-batis-0.2.0/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.2.0/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.2.0/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.2.0/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     5272 2023-07-30 15:49:36.000000 sqlx-batis-0.2.0/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1637 2023-07-31 11:12:07.000000 sqlx-batis-0.2.0/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.2.0/sqlbatis/support.py
+-rw-rw-rw-   0        0        0     1627 2023-07-29 10:34:32.000000 sqlx-batis-0.2.0/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 06:47:24.000000 sqlx-batis-0.2.0/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5701 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      465 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 11:36:14.000000 sqlx-batis-0.2.0/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.1.9/PKG-INFO` & `sqlx-batis-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.1.9
+Version: 0.2.0
 Summary: A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `sqlx-batis-0.1.9/README.rst` & `sqlx-batis-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.9/setup.py` & `sqlx-batis-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     name='sqlx-batis',
     packages=['sqlbatis'],
     description="A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'sqlx-exec>=1.4.0',
+        'sqlx-exec>=1.4.2',
     ],
-    version='0.1.9',
+    version='0.2.0',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.1.9/sqlbatis/constant.py` & `sqlx-batis-0.2.0/sqlbatis/constant.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlexec.constant import MYSQL, POSTGRESQL, SQLITE
+from sqlexec.constant import MYSQL, POSTGRESQL, SQLITE, ORACLE
 
 LIMIT_1 = 1
 
 NO_LIMIT = 0
 
 CACHE_SIZE = 256
```

### Comparing `sqlx-batis-0.1.9/sqlbatis/db.py` & `sqlx-batis-0.2.0/sqlbatis/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import sqlexec
+from sqlexec.exec import try_mapping
 from . import sql_support, Engine, DBError
-from .log_support import sql_log, do_sql_log, save_log, do_page_log, page_log
+from .log_support import do_sql_log, save_log, do_page_log, page_log
 
 # Don't remove. Import for not repetitive implementation
-from sqlexec import insert, save as save_select_key, save_sql, do_save_sql, batch_insert, batch_execute, do_execute as sqlexec_execute, \
-    do_get as sqlexec_get, do_query_one as sqlexec_query_one,do_query as sqlexec_query, do_select as sqlexec_select, do_select_one as sqlexec_select_one
+from sqlexec import insert, save as save_select_key, save_sql, do_save_sql, batch_insert, batch_execute
 
 
 def save(table: str, **kwargs):
     """
     Insert data into table, return primary key.
     :param table: table
     :param kwargs:
@@ -23,125 +24,125 @@
 
 def execute(sql: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
          INSERT INTO user(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
     """
-    sql, args = _try_dynamic_sql_args('sqlbatis.db.execute', sql, *args, **kwargs)
+    sql, args = _try_dynamic_sql('sqlbatis.db.execute', sql, *args, **kwargs)
     return do_execute(sql, *args)
 
 
 # ----------------------------------------------------------Query function------------------------------------------------------------------
 def get(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' after sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT count(1) FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql, args = _try_dynamic_sql_args('sqlbatis.db.get', sql, *args, **kwargs)
+    sql, args = _try_dynamic_sql('sqlbatis.db.get', sql, *args, **kwargs)
     return do_get(sql, *args)
 
 
 def query(sql: str, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql, args = _try_dynamic_sql_args('sqlbatis.db.query', sql, *args, **kwargs)
+    sql, args = _try_dynamic_sql('sqlbatis.db.query', sql, *args, **kwargs)
     return do_query(sql, *args)
 
 
 def query_one(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one row result(dict). Automatically add 'limit ?' after sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1 -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql, args = _try_dynamic_sql_args('sqlbatis.db.query_one', sql, *args, **kwargs)
+    sql, args = _try_dynamic_sql('sqlbatis.db.query_one', sql, *args, **kwargs)
     return do_query_one(sql, *args)
 
 
 def select(sql: str, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql, args = _try_dynamic_sql_args('sqlbatis.db.select', sql, *args, **kwargs)
+    sql, args = _try_dynamic_sql('sqlbatis.db.select', sql, *args, **kwargs)
     return do_select(sql, *args)
 
 
 def select_one(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one row result(tuple). Automatically add 'limit ?' after sql statement if not.
     If no result found, return None.
     If multiple results found, the first one returned.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    sql, args = _try_dynamic_sql_args('sqlbatis.db.select_one', sql, *args, **kwargs)
+    sql, args = _try_dynamic_sql('sqlbatis.db.select_one', sql, *args, **kwargs)
     return do_select_one(sql, *args)
 
 
 # ----------------------------------------------------------Do function------------------------------------------------------------------
 def do_execute(sql: str, *args):
     """
     Execute sql return effect rowcount
     sql: insert into user(name, age) values(?, ?)  -->  args: ('张三', 20)
     """
-    return sqlexec_execute(sql, *args)
+    return sqlexec.do_execute(sql, *args)
 
 
 def do_get(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     sql, args = _do_limit_sql_args('do_get', sql, *args)
-    return sqlexec_get(sql, *args)
+    return sqlexec.do_get(sql, *args)
 
 
 def do_query(sql: str, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
-    return sqlexec_query(sql, *args)
+    return sqlexec.do_query(sql, *args)
 
 
 def do_select(sql: str, *args):
     """
     execute select SQL and return unique result or list results(tuple).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
-    return sqlexec_select(sql, *args)
+    return sqlexec.do_select(sql, *args)
 
 
 def do_query_one(sql: str, *args):
     """
     execute select SQL and return unique result(dict). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     sql, args = _do_limit_sql_args('do_query_one', sql, *args)
-    return sqlexec_query_one(sql, *args)
+    return sqlexec.do_query_one(sql, *args)
 
 
 def do_select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple). Automatically add 'limit ?' behind the sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     sql, args = _do_limit_sql_args('do_select_one', sql, *args)
-    return sqlexec_select_one(sql, *args)
+    return sqlexec.do_select_one(sql, *args)
 
 
 # ----------------------------------------------------------Page function------------------------------------------------------------------
 def query_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
@@ -166,28 +167,28 @@
 def do_query_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     do_page_log('select_page', sql.strip(), page_num, page_size, args)
     sql, args = Engine.get_page_sql_args_intf(sql, page_num, page_size, *args)
-    return sqlexec_query(sql, *args)
+    return sqlexec.do_query(sql, *args)
 
 
 def do_select_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     do_page_log('do_select_page', sql.strip(), page_num, page_size, args)
     sql, args = Engine.get_page_sql_args_intf(sql, page_num, page_size, *args)
-    return sqlexec_select(sql, *args)
+    return sqlexec.do_select(sql, *args)
 
 
-def _try_dynamic_sql_args(function, sql, *args, **kwargs):
-    sql_log(function, sql, *args, **kwargs)
-    return sql_support.dynamic_sql(sql, *args, **kwargs)
+def _try_dynamic_sql(function, sql, *args, **kwargs):
+    sql = sql_support.dynamic_sql(sql, **kwargs)
+    return try_mapping(function, sql, *args, **kwargs)
 
 
 def _do_limit_sql_args(function, sql, *args):
     do_sql_log(function, sql, *args)
     return sql_support.limit_one_sql_args(sql, *args)
```

### Comparing `sqlx-batis-0.1.9/sqlbatis/dbx.py` & `sqlx-batis-0.2.0/sqlbatis/dbx.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.9/sqlbatis/engine.py` & `sqlx-batis-0.2.0/sqlbatis/engine.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .support import DBError
 from functools import lru_cache
 from .log_support import logger
 from sqlexec import get, query, select
 from sqlexec.engine import Engine as SupperEngine
 from .sql_support import require_limit, get_page_start
 from .constant import MYSQL_COLUMN_SQL, POSTGRES_COLUMN_SQL, MYSQL_SELECT_KEY, LIMIT_1, MYSQL, POSTGRESQL, DEFAULT_KEY_FIELD, CACHE_SIZE, SQLITE, \
-    SQLITE_SELECT_KEY
+    SQLITE_SELECT_KEY, ORACLE
 
 
 # Engin = Enum('Engin', ['MYSQL', 'POSTGRESQL', 'OTHER'])
 # class Engin(Enum):
 #     MYSQL = 'MySQL'
 #     POSTGRESQL = 'PostgreSQL'
 #     OTHER = 'Other'
@@ -64,14 +64,19 @@
             logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
         if '%' in sql and 'like' in sql.lower():
             sql = sql.replace('%', '%%').replace('%%%%', '%%')
         return sql.replace('?', '%s')
 
 
 class MySqlEngine(BaseEngine):
+
+    @classmethod
+    def init(cls, name=MYSQL):
+        super().init(name)
+
     @staticmethod
     def create_insert_sql(table: str, cols: Sequence[str]):
         columns, placeholders = zip(*[('`{}`'.format(col), '?') for col in cols])
         return 'INSERT INTO `{}`({}) VALUES({})'.format(table, ','.join(columns), ','.join(placeholders))
 
     @staticmethod
     def get_page_sql_args(sql: str, page_num: int, page_size: int, *args):
@@ -87,14 +92,18 @@
 
     @staticmethod
     def get_select_key():
         return MYSQL_SELECT_KEY
 
 
 class PostgresEngine(BaseEngine):
+
+    @classmethod
+    def init(cls, name=POSTGRESQL):
+        super().init(name)
     @staticmethod
     def get_table_columns(table: str):
         return get(POSTGRES_COLUMN_SQL, table, LIMIT_1)
 
     @staticmethod
     def get_select_key(key_seq: str = None, table: str = None, key: str =None, sql: str = None):
         if not key_seq:
@@ -119,14 +128,19 @@
         table = re.search('(?<=into )\w+', sql, re.I)
         key_seq = PostgresEngine.build_key_seq(table.group())
         logger.warning("'key_seq' is None, will use default '{}' from sql.".format(key_seq))
         return key_seq
 
 
 class OracleEngine(BaseEngine):
+
+    @classmethod
+    def init(cls, name=ORACLE):
+        super().init(name)
+
     @staticmethod
     def get_page_sql_args(sql: str, page_num: int, page_size: int, *args):
         start = get_page_start(page_num, page_size)
         end = start + page_size
         sql = 'SELECT * FROM (SELECT tmp.*, rownum row_num FROM ({}) tmp WHERE rownum <= >) WHERE row_num > :startRow '.format(sql)
         args = [*args, end, start]
         return sql, args
@@ -139,14 +153,19 @@
     @staticmethod
     def get_select_key(key_seq: str):
         # return get(f"SELECT {key_seq}.nextval FROM dual")
         raise NotImplementedError(f"Not implement method 'get_select_key' for {Engine.current_engine()}, you can use orm snowflake for primary key.")
 
 
 class SQLiteEngine(BaseEngine):
+
+    @classmethod
+    def init(cls, name=SQLITE):
+        super().init(name)
+
     @staticmethod
     def get_table_columns(table: str):
         results = query(f'PRAGMA table_info({table})')
         return ','.join([result['name'] for result in results])
 
     @staticmethod
     def get_select_key():
```

### Comparing `sqlx-batis-0.1.9/sqlbatis/log_support.py` & `sqlx-batis-0.2.0/sqlbatis/log_support.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlexec.log_support import logger, sql_log
+from sqlexec.log_support import logger
 
 
 def save_log(table, **kwargs):
     logger.debug("Exec func 'pgsqlx.db.save' \n\t Table: '%s', kwargs: %s" % (table, kwargs))
 
 
 def do_sql_log(function: str, sql: str, *args):
```

### Comparing `sqlx-batis-0.1.9/sqlbatis/orm.py` & `sqlx-batis-0.2.0/sqlbatis/orm.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.9/sqlbatis/snowflake.py` & `sqlx-batis-0.2.0/sqlbatis/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.9/sqlbatis/sql_holder.py` & `sqlx-batis-0.2.0/sqlbatis/sql_holder.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.9/sqlbatis/sql_mapper.py` & `sqlx-batis-0.2.0/sqlbatis/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.9/sqlbatis/sql_support.py` & `sqlx-batis-0.2.0/sqlbatis/sql_support.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,36 +8,33 @@
 from sqlexec.sql_support import get_named_args, get_named_sql, get_batch_args, get_named_sql_args, is_mapping
 
 
 def simple_sql(sql: str, *args, **kwargs):
     return get_named_sql_args(sql, **kwargs) if kwargs else (sql, args)
 
 
-def dynamic_sql(sql: str, *args, **kwargs):
-    sql_type = _get_sql_type(sql)
-    if sql_type >= 1 and not kwargs:
-        raise MapperError("Parameter 'kwargs' must not be empty when named mapping sql.")
-    if sql_type == 0:
-        return sql, args
-    if sql_type == 1:
-        sql = Template(sql).render(**kwargs)
-    return get_named_sql_args(sql, **kwargs)
+def dynamic_sql(sql: str, **kwargs):
+    if is_dynamic_sql(sql):
+        assert kwargs, "Parameter '**kwargs' must not be empty when named mapping sql."
+        return Template(sql).render(**kwargs)
+    return sql
 
 
 def get_page_start(page_num: int, page_size: int):
     assert page_num >= 1 and page_size >= 1, "'page_name' and 'page_size' should be higher or equal to 1"
     return (page_num - 1) * page_size
 
 
 def limit_one_sql_args(sql: str, *args):
     if require_limit(sql):
         return '{} LIMIT ?'.format(sql), [*args, LIMIT_1]
     return sql, args
 
 
+@lru_cache(maxsize=2*CACHE_SIZE)
 def is_dynamic_sql(sql: str):
     return re.search(DYNAMIC_REGEX, sql)
 
 
 def require_limit(sql: str):
     lower_sql = sql.lower()
     if 'limit' not in lower_sql:
```

### Comparing `sqlx-batis-0.1.9/sqlbatis/__init__.py` & `sqlx-batis-0.2.0/sqlbatis/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.1.9/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-0.2.0/sqlx_batis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.1.9
+Version: 0.2.0
 Summary: A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

