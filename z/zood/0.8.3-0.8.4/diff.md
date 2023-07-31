# Comparing `tmp/zood-0.8.3.tar.gz` & `tmp/zood-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zood-0.8.3.tar", max compression
+gzip compressed data, was "zood-0.8.4.tar", max compression
```

## Comparing `zood-0.8.3.tar` & `zood-0.8.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      571 2023-07-30 13:37:12.332931 zood-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      657 2023-07-28 05:47:50.290823 zood-0.8.3/README.md
--rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.8.3/zood/__init__.py
--rw-r--r--   0        0        0     4975 2023-07-30 02:58:53.277878 zood-0.8.3/zood/config/_config.yml
--rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.8.3/zood/config/img/after_copy.png
--rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.8.3/zood/config/img/before_copy.png
--rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.8.3/zood/config/img/enter.png
--rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.8.3/zood/config/img/enter.svg
--rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.8.3/zood/config/img/moon.png
--rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.8.3/zood/config/img/search.svg
--rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.8.3/zood/config/img/sun.png
--rw-r--r--   0        0        0    15117 2023-07-30 13:32:42.852151 zood-0.8.3/zood/config/index.css
--rw-r--r--   0        0        0     3991 2023-07-13 02:52:54.473602 zood-0.8.3/zood/config/js/change_mode.js
--rw-r--r--   0        0        0     2646 2023-07-28 00:49:18.358387 zood-0.8.3/zood/config/js/copy_code.js
--rw-r--r--   0        0        0     1251 2023-07-28 01:20:50.114459 zood-0.8.3/zood/config/js/global_js_configuration.js
--rw-r--r--   0        0        0     2154 2023-07-13 02:53:27.953277 zood-0.8.3/zood/config/js/navigator.js
--rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.8.3/zood/config/js/next_front.js
--rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.8.3/zood/config/js/picture_preview.js
--rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.8.3/zood/config/js/picture_title.js
--rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.8.3/zood/config/js/prismjs/prism.css
--rw-r--r--   0        0        0    64866 2023-04-27 06:47:33.381797 zood-0.8.3/zood/config/js/prismjs/prism.js
--rw-r--r--   0        0        0     5999 2023-04-19 11:50:00.362712 zood-0.8.3/zood/config/js/search.js
--rw-r--r--   0        0        0      583 2023-07-29 15:25:41.350255 zood-0.8.3/zood/config/template.html
--rw-r--r--   0        0        0       69 2023-06-24 15:37:55.849962 zood-0.8.3/zood/extensions/__init__.py
--rw-r--r--   0        0        0     4109 2023-07-03 06:30:14.058101 zood-0.8.3/zood/extensions/poetry_update.py
--rw-r--r--   0        0        0     6914 2023-07-30 05:41:06.115498 zood-0.8.3/zood/gen_doc.py
--rw-r--r--   0        0        0     5547 2023-07-29 15:04:26.207636 zood-0.8.3/zood/main.py
--rw-r--r--   0        0        0     6809 2023-07-29 04:00:11.279113 zood-0.8.3/zood/util.py
--rw-r--r--   0        0        0     8041 2023-07-29 15:38:58.625505 zood-0.8.3/zood/zood.py
--rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 zood-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      571 2023-07-31 03:30:34.583191 zood-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0      657 2023-07-28 05:47:50.290823 zood-0.8.4/README.md
+-rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.8.4/zood/__init__.py
+-rw-r--r--   0        0        0     4975 2023-07-30 02:58:53.277878 zood-0.8.4/zood/config/_config.yml
+-rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.8.4/zood/config/img/after_copy.png
+-rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.8.4/zood/config/img/before_copy.png
+-rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.8.4/zood/config/img/enter.png
+-rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.8.4/zood/config/img/enter.svg
+-rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.8.4/zood/config/img/moon.png
+-rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.8.4/zood/config/img/search.svg
+-rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.8.4/zood/config/img/sun.png
+-rw-r--r--   0        0        0    15124 2023-07-31 03:30:14.314523 zood-0.8.4/zood/config/index.css
+-rw-r--r--   0        0        0     3991 2023-07-13 02:52:54.473602 zood-0.8.4/zood/config/js/change_mode.js
+-rw-r--r--   0        0        0     2646 2023-07-28 00:49:18.358387 zood-0.8.4/zood/config/js/copy_code.js
+-rw-r--r--   0        0        0     1251 2023-07-28 01:20:50.114459 zood-0.8.4/zood/config/js/global_js_configuration.js
+-rw-r--r--   0        0        0     2154 2023-07-13 02:53:27.953277 zood-0.8.4/zood/config/js/navigator.js
+-rw-r--r--   0        0        0     1000 2023-01-01 02:18:50.438286 zood-0.8.4/zood/config/js/next_front.js
+-rw-r--r--   0        0        0     1064 2023-01-02 14:54:02.515677 zood-0.8.4/zood/config/js/picture_preview.js
+-rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.8.4/zood/config/js/picture_title.js
+-rw-r--r--   0        0        0     2301 2023-02-17 14:35:29.225249 zood-0.8.4/zood/config/js/prismjs/prism.css
+-rw-r--r--   0        0        0    64866 2023-04-27 06:47:33.381797 zood-0.8.4/zood/config/js/prismjs/prism.js
+-rw-r--r--   0        0        0     5999 2023-04-19 11:50:00.362712 zood-0.8.4/zood/config/js/search.js
+-rw-r--r--   0        0        0      583 2023-07-29 15:25:41.350255 zood-0.8.4/zood/config/template.html
+-rw-r--r--   0        0        0       69 2023-06-24 15:37:55.849962 zood-0.8.4/zood/extensions/__init__.py
+-rw-r--r--   0        0        0     4109 2023-07-03 06:30:14.058101 zood-0.8.4/zood/extensions/poetry_update.py
+-rw-r--r--   0        0        0     6914 2023-07-30 05:41:06.115498 zood-0.8.4/zood/gen_doc.py
+-rw-r--r--   0        0        0     5547 2023-07-29 15:04:26.207636 zood-0.8.4/zood/main.py
+-rw-r--r--   0        0        0     6809 2023-07-29 04:00:11.279113 zood-0.8.4/zood/util.py
+-rw-r--r--   0        0        0     8041 2023-07-29 15:38:58.625505 zood-0.8.4/zood/zood.py
+-rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 zood-0.8.4/PKG-INFO
```

### Comparing `zood-0.8.3/pyproject.toml` & `zood-0.8.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zood"
-version = "0.8.3"
+version = "0.8.4"
 description = "web page documentation & comment generation documentation"
 license = "MIT"
 authors = ["kamilu <luzhixing12345@163.com>"]
 readme = "README.md"
 repository = "https://github.com/luzhixing12345/zood"
 documentation = "https://luzhixing12345.github.io/zood/"
```

### Comparing `zood-0.8.3/README.md` & `zood-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/config/_config.yml` & `zood-0.8.4/zood/config/_config.yml`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/config/img/enter.png` & `zood-0.8.4/zood/config/img/enter.png`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/config/index.css` & `zood-0.8.4/zood/config/index.css`

 * *Files 2% similar despite different names*

```diff
@@ -323,16 +323,16 @@
 .markdown-body pre {
     position: relative;
 }
 
 .markdown-body pre #code_copy {
     position: absolute;
     right: 10px;
-    top: 50%;
-    margin-top: -16px;
+    top: 10px;
+    /* margin-top: -16px; */
     padding: 3px;
     opacity: 0.9;
     border: 1px solid rgba(149, 157, 165, 0.2);
     border-radius: 5px;
     z-index: 1;
 }
```

### Comparing `zood-0.8.3/zood/config/js/change_mode.js` & `zood-0.8.4/zood/config/js/change_mode.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/config/js/copy_code.js` & `zood-0.8.4/zood/config/js/copy_code.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/config/js/global_js_configuration.js` & `zood-0.8.4/zood/config/js/global_js_configuration.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/config/js/navigator.js` & `zood-0.8.4/zood/config/js/navigator.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/config/js/next_front.js` & `zood-0.8.4/zood/config/js/next_front.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/config/js/picture_preview.js` & `zood-0.8.4/zood/config/js/picture_preview.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/config/js/prismjs/prism.css` & `zood-0.8.4/zood/config/js/prismjs/prism.css`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/config/js/prismjs/prism.js` & `zood-0.8.4/zood/config/js/prismjs/prism.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/config/js/search.js` & `zood-0.8.4/zood/config/js/search.js`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/config/template.html` & `zood-0.8.4/zood/config/template.html`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/extensions/poetry_update.py` & `zood-0.8.4/zood/extensions/poetry_update.py`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/gen_doc.py` & `zood-0.8.4/zood/gen_doc.py`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/main.py` & `zood-0.8.4/zood/main.py`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/util.py` & `zood-0.8.4/zood/util.py`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/zood/zood.py` & `zood-0.8.4/zood/zood.py`

 * *Files identical despite different names*

### Comparing `zood-0.8.3/PKG-INFO` & `zood-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zood
-Version: 0.8.3
+Version: 0.8.4
 Summary: web page documentation & comment generation documentation
 Home-page: https://github.com/luzhixing12345/zood
 License: MIT
 Author: kamilu
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

