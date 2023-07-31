# Comparing `tmp/yunxiao-0.3.6.tar.gz` & `tmp/yunxiao-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.3.6.tar", last modified: Sat Jul 29 16:41:37 2023, max compression
+gzip compressed data, was "yunxiao-0.3.7.tar", last modified: Mon Jul 31 20:18:13 2023, max compression
```

## Comparing `yunxiao-0.3.6.tar` & `yunxiao-0.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 16:41:37.417585 yunxiao-0.3.6/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.3.6/LICENSE
--rw-rw-rw-   0        0        0     6351 2023-07-29 16:41:37.416584 yunxiao-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     5860 2023-06-22 16:19:34.000000 yunxiao-0.3.6/README.md
--rw-rw-rw-   0        0        0     1594 2023-07-29 16:41:15.000000 yunxiao-0.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-29 16:41:37.417585 yunxiao-0.3.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-29 16:41:37.403571 yunxiao-0.3.6/test/
--rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.3.6/test/test.py
-drwxrwxrwx   0        0        0        0 2023-07-29 16:41:37.407576 yunxiao-0.3.6/yunxiao/
--rw-rw-rw-   0        0        0       37 2023-06-22 16:12:18.000000 yunxiao-0.3.6/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    41337 2023-07-29 16:40:10.000000 yunxiao-0.3.6/yunxiao/v2.py
--rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.3.6/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-07-29 16:41:37.415583 yunxiao-0.3.6/yunxiao.egg-info/
--rw-rw-rw-   0        0        0     6351 2023-07-29 16:41:37.000000 yunxiao-0.3.6/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-07-29 16:41:37.000000 yunxiao-0.3.6/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 16:41:37.000000 yunxiao-0.3.6/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-29 16:41:37.000000 yunxiao-0.3.6/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-29 16:41:37.000000 yunxiao-0.3.6/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 20:18:13.829495 yunxiao-0.3.7/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0     6351 2023-07-31 20:18:13.828494 yunxiao-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5860 2023-06-22 16:19:34.000000 yunxiao-0.3.7/README.md
+-rw-rw-rw-   0        0        0     1680 2023-07-31 20:17:56.000000 yunxiao-0.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 20:18:13.829495 yunxiao-0.3.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 20:18:13.816911 yunxiao-0.3.7/test/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.3.7/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-31 20:18:13.819913 yunxiao-0.3.7/yunxiao/
+-rw-rw-rw-   0        0        0       37 2023-06-22 16:12:18.000000 yunxiao-0.3.7/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    41371 2023-07-31 20:16:36.000000 yunxiao-0.3.7/yunxiao/v2.py
+-rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.3.7/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-07-31 20:18:13.827493 yunxiao-0.3.7/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0     6351 2023-07-31 20:18:13.000000 yunxiao-0.3.7/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-07-31 20:18:13.000000 yunxiao-0.3.7/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 20:18:13.000000 yunxiao-0.3.7/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 20:18:13.000000 yunxiao-0.3.7/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 20:18:13.000000 yunxiao-0.3.7/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.3.6/LICENSE` & `yunxiao-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.3.6/PKG-INFO` & `yunxiao-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.3.6
+Version: 0.3.7
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.3.6/README.md` & `yunxiao-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.3.6/pyproject.toml` & `yunxiao-0.3.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.3.6"
+version = "0.3.7"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
@@ -22,14 +22,15 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
+"0.3.7" = "修复翻页模块的一处bug，当返回空数据时，不再报错。"
 "0.3.6" = "更改日志，多页查询时，不再输出空日志。"
 "0.3.5" = "更新可用参数。"
 "0.3.4" = "修复BUG:拉取意向失败。"
 "0.3.3" = "修复BUG：班级查询根据名称检索失效。"
 "0.3.2" = "更新参数，修复BUG，新增意向管理API"
 "0.3.1" = "修复整合"
 "0.2.9" = "删除其他，只使用V2"
```

### Comparing `yunxiao-0.3.6/yunxiao/v2.py` & `yunxiao-0.3.7/yunxiao/v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,16 @@
                 page = kwargs.get("page")
                 size = kwargs.get("size")
                 while (now := len(result)) != count:
                     page += 1
                     kwargs["page"] = page
                     res = func(*args, **kwargs)
                     data = res["data"][KEY] if KEY else res["data"]
-                    result.extend(data)
+                    if data:
+                        result.extend(data)
                     count = res["page"]["totalCount"]
                     print(f"size: {size}, page: {page}, {now}/{count}")
                     size = size if (count - len(result)) > size else (count - len(result))
                     kwargs["size"] = size
                 if size != 0:
                     print(f"size: {size}, page: {page}, {now}/{count}")
                 return result
```

### Comparing `yunxiao-0.3.6/yunxiao/yunxiao.py` & `yunxiao-0.3.7/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.3.6/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.3.7/yunxiao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.3.6
+Version: 0.3.7
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

