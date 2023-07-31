# Comparing `tmp/yplib-2.6.4.tar.gz` & `tmp/yplib-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.6.4.tar", last modified: Mon Jul 24 02:06:02 2023, max compression
+gzip compressed data, was "dist\yplib-2.6.5.tar", last modified: Mon Jul 31 00:58:41 2023, max compression
```

## Comparing `yplib-2.6.4.tar` & `yplib-2.6.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 02:06:02.874649 yplib-2.6.4/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.6.4/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-24 02:06:02.874649 yplib-2.6.4/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.6.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 02:06:02.875265 yplib-2.6.4/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-24 02:04:21.000000 yplib-2.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 02:06:02.864578 yplib-2.6.4/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.6.4/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.6.4/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-13 00:33:38.000000 yplib-2.6.4/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.6.4/yplib/db.py
--rw-rw-rw-   0        0        0     5292 2023-07-17 02:22:22.000000 yplib-2.6.4/yplib/file.py
--rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.6.4/yplib/http_util.py
--rw-rw-rw-   0        0        0    35649 2023-07-24 02:03:11.000000 yplib-2.6.4/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.6.4/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.6.4/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.6.4/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.6.4/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-24 02:06:02.874140 yplib-2.6.4/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-24 02:06:02.000000 yplib-2.6.4/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-24 02:06:02.000000 yplib-2.6.4/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 02:06:02.000000 yplib-2.6.4/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-24 02:06:02.000000 yplib-2.6.4/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 00:58:41.612387 yplib-2.6.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.6.5/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-31 00:58:41.611899 yplib-2.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 00:58:41.612387 yplib-2.6.5/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-31 00:57:33.000000 yplib-2.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:58:41.605932 yplib-2.6.5/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.6.5/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.6.5/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-13 00:33:38.000000 yplib-2.6.5/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.6.5/yplib/db.py
+-rw-rw-rw-   0        0        0     5292 2023-07-17 02:22:22.000000 yplib-2.6.5/yplib/file.py
+-rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.6.5/yplib/http_util.py
+-rw-rw-rw-   0        0        0    35897 2023-07-31 00:57:15.000000 yplib-2.6.5/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.6.5/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.6.5/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.6.5/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.6.5/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:58:41.611455 yplib-2.6.5/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-31 00:58:41.000000 yplib-2.6.5/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-31 00:58:41.000000 yplib-2.6.5/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 00:58:41.000000 yplib-2.6.5/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-31 00:58:41.000000 yplib-2.6.5/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.6.4/LICENSE` & `yplib-2.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.6.4/setup.py` & `yplib-2.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.6.4",
+  version="2.6.5",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.6.4/yplib/__init__.py` & `yplib-2.6.5/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.4/yplib/chart.py` & `yplib-2.6.5/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.4/yplib/chart_html.py` & `yplib-2.6.5/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.4/yplib/db.py` & `yplib-2.6.5/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.4/yplib/file.py` & `yplib-2.6.5/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.4/yplib/http_util.py` & `yplib-2.6.5/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.4/yplib/index.py` & `yplib-2.6.5/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -640,28 +640,30 @@
 # 当读取 txt 之类的文件的时候
 # 将 txt 文件读取到 list 中, 每一行自动过滤掉行前行后的特殊字符
 # sep               : 对每一行进行分割,将 list(str) 转化为 list(list(str)), 或者将 list(list(str)) 转化为 list(list(list(str)))
 # sep_line          : 这一行是一个分隔符, 分隔符与这行一样, 将 list(str) 转化为 list(list(str))
 # sep_line_contain  : 这一行是一个分隔符,包含这个行分隔符的做分割, 将 list(str) 转化为 list(list(str))
 # sep_line_prefix   : 这一行是一个分隔符,以这个分隔符作为前缀的, 将 list(str) 转化为 list(list(str))
 # sep_line_suffix   : 这一行是一个分隔符,以这个分隔符作为后缀的, 将 list(str) 转化为 list(list(str))
+# sep_is_front      : 这一行，分割行，是包含到前面，还是包含到
 # sep_all           : 将文件转化成一个字符串,然后对这个字符串,再次总体分割 将 list(str) 转化为 str , 然后再次转化成 list(str)
 # line_join         : 将 list(list(str)) 转化成 list(str) 类型的数据
 # line_json         : 将 list(str) 转化成 list(json) 类型的数据, 会自动过滤掉空格行
 # start_index       : 从这个地方开始读取,从1开始标号 , 包含这一行
 # start_line        : 从这个地方开始读取,从第一行开始找到这个字符串开始标记 , 包含这一行
 # end_index         : 读取到这个地方结束,从1开始标号 , 不包含这一行
 # end_line          : 读取到这个地方结束,从第一行开始找到这个字符串开始标记 , 不包含这一行
 # count             : 读取指定的行数
 def to_list_from_txt(file_name='a.txt',
                      sep=None,
                      sep_line=None,
                      sep_line_contain=None,
                      sep_line_prefix=None,
                      sep_line_suffix=None,
+                     sep_is_front=True,
                      sep_all=None,
                      line_join=None,
                      line_json=None,
                      start_index=None,
                      start_line=None,
                      end_index=None,
                      end_line=None,
@@ -704,42 +706,39 @@
             continue
         c += 1
         data_list.append(line)
     if sep_all is not None:
         # 全部划分, 重新分割成 list(str)
         data_list = ''.join(data_list).split(str(sep_all))
     # 有行分隔符, 将会把 list(str) 转化成 list(list)
-    if len(list(filter(lambda x: x is not None, [sep_line, sep_line_contain, sep_line_prefix, sep_line_suffix]))):
+    if len(list(filter(lambda x: x is not None, [sep_line, sep_line_prefix, sep_line_contain, sep_line_suffix]))):
+        # 当是这种情况的时候,返回的数据结果
         r_list = []
-        t_l = []
+        # 数据中的一行 list 数据
+        one_list = []
         for d_o in data_list:
-            n_l_f = False
+            # 过滤掉空行,无效行
+            if len(d_o.strip()) and sep_is_front:
+                one_list.append(d_o)
             # 这一行, 等于 sep_line
-            if sep_line is not None and d_o == sep_line:
-                n_l_f = True
-            # 这一行, 包含 sep_line_contain
-            elif sep_line_contain is not None and d_o.find(sep_line_contain) != -1:
-                t_l.append(d_o)
-                n_l_f = True
-            # 这一行, 是否是以 sep_line_prefix 开头
-            elif sep_line_prefix is not None and d_o.startswith(sep_line_prefix):
-                t_l.append(d_o)
-                n_l_f = True
-            # 这一行, 是否是以 sep_line_suffix 结尾
-            elif sep_line_suffix is not None and d_o.endswith(sep_line_suffix):
-                t_l.append(d_o)
-                n_l_f = True
-            if n_l_f:
-                if len(t_l):
-                    r_list.append(t_l)
-                t_l = []
-            elif len(d_o):
-                t_l.append(d_o)
-        if len(t_l):
-            r_list.append(t_l)
+            if ((sep_line is not None and d_o == sep_line) or
+                    # 这一行, 包含 sep_line_contain
+                    (sep_line_contain is not None and d_o.find(sep_line_contain) != -1) or
+                    # 这一行, 是否是以 sep_line_prefix 开头
+                    (sep_line_prefix is not None and d_o.startswith(sep_line_prefix)) or
+                    # 这一行, 是否是以 sep_line_suffix 结尾
+                    (sep_line_suffix is not None and d_o.endswith(sep_line_suffix))):
+                if len(one_list):
+                    r_list.append(one_list)
+                    one_list = []
+            if len(d_o.strip()) and not sep_is_front:
+                one_list.append(d_o)
+        # 最后的一条数据,兼容一下
+        if len(one_list):
+            r_list.append(one_list)
         data_list = r_list
     # 对这个 list 进行行内再次分割
     if sep is not None:
         r_list = []
         for line in data_list:
             # list(str) 情况
             if isinstance(line, str):
@@ -860,8 +859,8 @@
             if can_use_json(one_data):
                 s = json.dumps(one_data)
             else:
                 s = str(one_data)
             excel_obj_sheet.append([s])
 
     # 文件保存
-    excel_obj.save(file_path + '/' + get_file_name(file_name, '.xlsx'))
+    excel_obj.save(file_path + '/' + get_file_name(file_name, '.xlsx'))
```

### Comparing `yplib-2.6.4/yplib/mail.py` & `yplib-2.6.5/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.4/yplib/mail_html.py` & `yplib-2.6.5/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.6.4/yplib/markdown.py` & `yplib-2.6.5/yplib/markdown.py`

 * *Files identical despite different names*

