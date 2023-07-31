# Comparing `tmp/phap-3.1.0a5.tar.gz` & `tmp/phap-3.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phap-3.1.0a5.tar", last modified: Sun Jul 30 02:41:07 2023, max compression
+gzip compressed data, was "phap-3.1.0rc1.tar", last modified: Mon Jul 31 04:31:18 2023, max compression
```

## Comparing `phap-3.1.0a5.tar` & `phap-3.1.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 02:41:07.874104 phap-3.1.0a5/
--rw-rw-rw-   0        0        0     1069 2023-05-25 04:31:47.000000 phap-3.1.0a5/LICENSE
--rw-rw-rw-   0        0        0     2504 2023-07-30 02:41:07.873075 phap-3.1.0a5/PKG-INFO
--rw-rw-rw-   0        0        0     1705 2023-07-25 04:29:06.000000 phap-3.1.0a5/README.md
--rw-rw-rw-   0        0        0       86 2022-03-12 07:02:40.000000 phap-3.1.0a5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-30 02:41:07.875077 phap-3.1.0a5/setup.cfg
--rw-rw-rw-   0        0        0     1685 2023-07-25 04:28:45.000000 phap-3.1.0a5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 02:41:07.819948 phap-3.1.0a5/src/
-drwxrwxrwx   0        0        0        0 2023-07-30 02:41:07.839978 phap-3.1.0a5/src/algo/
--rw-rw-rw-   0        0        0      210 2023-07-23 04:55:40.000000 phap-3.1.0a5/src/algo/__init__.py
--rw-rw-rw-   0        0        0      607 2023-07-25 04:12:52.000000 phap-3.1.0a5/src/algo/arraylib.py
--rw-rw-rw-   0        0        0     3267 2023-07-30 02:37:41.000000 phap-3.1.0a5/src/algo/treelib.py
-drwxrwxrwx   0        0        0        0 2023-07-30 02:41:07.842489 phap-3.1.0a5/src/phap/
--rw-rw-rw-   0        0        0       72 2023-07-24 11:39:49.000000 phap-3.1.0a5/src/phap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 02:41:07.852529 phap-3.1.0a5/src/phap.egg-info/
--rw-rw-rw-   0        0        0     2504 2023-07-30 02:41:07.000000 phap-3.1.0a5/src/phap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-07-30 02:41:07.000000 phap-3.1.0a5/src/phap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 02:41:07.000000 phap-3.1.0a5/src/phap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-30 02:41:07.000000 phap-3.1.0a5/src/phap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 02:41:07.854533 phap-3.1.0a5/src/phapbm/
--rw-rw-rw-   0        0        0     1013 2023-07-24 11:41:34.000000 phap-3.1.0a5/src/phapbm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 02:41:07.860552 phap-3.1.0a5/src/stralgo/
--rw-rw-rw-   0        0        0      718 2023-07-23 04:55:41.000000 phap-3.1.0a5/src/stralgo/__init__.py
--rw-rw-rw-   0        0        0     1021 2023-07-23 04:55:41.000000 phap-3.1.0a5/src/stralgo/base.py
-drwxrwxrwx   0        0        0        0 2023-07-30 02:41:07.866560 phap-3.1.0a5/src/stralgo/hash/
--rw-rw-rw-   0        0        0      354 2023-07-23 04:55:41.000000 phap-3.1.0a5/src/stralgo/hash/__init__.py
--rw-rw-rw-   0        0        0      508 2023-07-23 04:55:41.000000 phap-3.1.0a5/src/stralgo/hash/sha.py
-drwxrwxrwx   0        0        0        0 2023-07-30 02:41:07.871076 phap-3.1.0a5/src/stralgo/hash/sm/
--rw-rw-rw-   0        0        0      148 2023-07-23 04:55:41.000000 phap-3.1.0a5/src/stralgo/hash/sm/__init__.py
--rw-rw-rw-   0        0        0     6943 2023-07-24 11:35:14.000000 phap-3.1.0a5/src/stralgo/hash/sm/sm3libs.py
--rw-rw-rw-   0        0        0      233 2023-07-23 04:55:41.000000 phap-3.1.0a5/src/stralgo/json.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.032437 phap-3.1.0rc1/
+-rw-rw-rw-   0        0        0     1069 2023-05-25 04:31:47.000000 phap-3.1.0rc1/LICENSE
+-rw-rw-rw-   0        0        0     2502 2023-07-31 04:31:18.032437 phap-3.1.0rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     1702 2023-07-31 04:30:14.000000 phap-3.1.0rc1/README.md
+-rw-rw-rw-   0        0        0       86 2022-03-12 07:02:40.000000 phap-3.1.0rc1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 04:31:18.033437 phap-3.1.0rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1686 2023-07-31 04:30:32.000000 phap-3.1.0rc1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:31:17.960915 phap-3.1.0rc1/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.006471 phap-3.1.0rc1/src/algo/
+-rw-rw-rw-   0        0        0      210 2023-07-23 04:55:40.000000 phap-3.1.0rc1/src/algo/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-07-25 04:12:52.000000 phap-3.1.0rc1/src/algo/arraylib.py
+-rw-rw-rw-   0        0        0     4538 2023-07-31 04:28:39.000000 phap-3.1.0rc1/src/algo/treelib.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.008476 phap-3.1.0rc1/src/phap/
+-rw-rw-rw-   0        0        0       72 2023-07-24 11:39:49.000000 phap-3.1.0rc1/src/phap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.015472 phap-3.1.0rc1/src/phap.egg-info/
+-rw-rw-rw-   0        0        0     2502 2023-07-31 04:31:17.000000 phap-3.1.0rc1/src/phap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-07-31 04:31:17.000000 phap-3.1.0rc1/src/phap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 04:31:17.000000 phap-3.1.0rc1/src/phap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-31 04:31:17.000000 phap-3.1.0rc1/src/phap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.017440 phap-3.1.0rc1/src/phapbm/
+-rw-rw-rw-   0        0        0     1013 2023-07-24 11:41:34.000000 phap-3.1.0rc1/src/phapbm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.022434 phap-3.1.0rc1/src/stralgo/
+-rw-rw-rw-   0        0        0      718 2023-07-23 04:55:41.000000 phap-3.1.0rc1/src/stralgo/__init__.py
+-rw-rw-rw-   0        0        0     1021 2023-07-23 04:55:41.000000 phap-3.1.0rc1/src/stralgo/base.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.025435 phap-3.1.0rc1/src/stralgo/hash/
+-rw-rw-rw-   0        0        0      354 2023-07-23 04:55:41.000000 phap-3.1.0rc1/src/stralgo/hash/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-07-23 04:55:41.000000 phap-3.1.0rc1/src/stralgo/hash/sha.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:31:18.029440 phap-3.1.0rc1/src/stralgo/hash/sm/
+-rw-rw-rw-   0        0        0      148 2023-07-23 04:55:41.000000 phap-3.1.0rc1/src/stralgo/hash/sm/__init__.py
+-rw-rw-rw-   0        0        0     6943 2023-07-24 11:35:14.000000 phap-3.1.0rc1/src/stralgo/hash/sm/sm3libs.py
+-rw-rw-rw-   0        0        0      233 2023-07-23 04:55:41.000000 phap-3.1.0rc1/src/stralgo/json.py
```

### Comparing `phap-3.1.0a5/LICENSE` & `phap-3.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `phap-3.1.0a5/PKG-INFO` & `phap-3.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phap
-Version: 3.1.0a5
+Version: 3.1.0rc1
 Summary: Programing Helpful Algorithm Package
 Home-page: https://github.com/DashBing/phap/
 Author: DashBing
 Author-email: mcbbkf@outlook.com
 Project-URL: Github, https://github.com/DashBing/phap/
 Project-URL: Old Project Version(stralgo), https://pypi.org/project/stralgo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,15 +38,15 @@
 + v2.2.1
 
 ## Latest Available Version
 + v3.0.0
 
 ## Latest Version
 ### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
-+ v3.1.0-alpha5
++ v3.1.0-rc1
 
 # To Use
 ## Read our development document
 ### *(Click the [Github](https://github.com/DashBing/phap/ "Github") link to read this document，or you may can not to open the link)*
 + [Development Document](doc/README.md)
 
 # Build
```

### Comparing `phap-3.1.0a5/README.md` & `phap-3.1.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 + v2.2.1
 
 ## Latest Available Version
 + v3.0.0
 
 ## Latest Version
 ### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
-+ v3.1.0-alpha5
++ v3.1.0-rc1
 
 # To Use
 ## Read our development document
 ### *(Click the [Github](https://github.com/DashBing/phap/ "Github") link to read this document，or you may can not to open the link)*
 + [Development Document](doc/README.md)
 
 # Build
```

### Comparing `phap-3.1.0a5/setup.py` & `phap-3.1.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="phap",
-    version="3.1.0a5",  #版本
+    version="3.1.0rc1",  #版本
     author="DashBing",
     author_email="mcbbkf@outlook.com",
     description="Programing Helpful Algorithm Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #scripts=[],
     url="https://github.com/DashBing/phap/",
```

### Comparing `phap-3.1.0a5/src/algo/arraylib.py` & `phap-3.1.0rc1/src/algo/arraylib.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0a5/src/algo/treelib.py` & `phap-3.1.0rc1/src/algo/treelib.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,54 @@
+from typing import Any
 from phapbm import ErrorTemplate
 
 class ValueTypeError(ErrorTemplate):  # 从phapbm包继承错误类模板，具体可见phapbm/__init__.py
     message = "The value's type must not be treenode."
     info_list = ['Try to change the type to "str" or "int".']
 
 class treenode:  # 二叉树类
     '''This class is used to make treenode easier to call and use'''
-    def __init__(self, val = 0, left = 0, right = 0):  # 参数分别是，初始节点参数，初始节点左边和右边的值
+    def __init__(self, val:"Any != treenode" = 0, left:Any = 0, right:Any = 0) -> None:  # 参数分别是，初始节点参数，初始节点左边和右边的值
         self.__t = [str(self.__class__)]  # 定义一个保护类型的变量，用于识别构造函数参数的类型，用列表方便后期扩展以及其他类继承
         if str(type(val)) in self.__t:  # 如果初始节点参数是二叉树类，则报错
             self.val = 0
             raise ValueTypeError()
         else:
             self.val = val
         self.left = left  # 将本类初始节点的左右侧分别赋值
         self.right = right
 
-    def setfromlist(self, val:list):  # 支持从列表设置本二叉树的函数，结构为[参数,左,右]，可嵌套
+    def setfromlist(self, val:list) -> None:  # 支持从列表设置本二叉树的函数，结构为[参数,左,右]，可嵌套
         '''To set the node from list'''
         self.val = val[0]  # 设置本类初始节点参数
         if str(type(val[1])) == str(type([])):  # 如果初始节点左侧是嵌套的列表
             self.left = treenode().setfromlist(val[1])  # 则创建一个新的本类实例，并将所得列表传参给实例的本函数，并将本类左侧参数赋值
         else:
             self.left = val[1]
         if str(type(val[2])) == str(type([])):  # 原理同上
             self.right = treenode().setfromlist(val[2])
         else:
             self.right = val[2]
 
+    def __eq__(self, value:object) -> bool:  # 简化赋值的运算符重载
+        try:
+            if str(type(value)) in self.__t:  # 如果赋值表达式的右值为二叉树类
+                self.val = value.val  # 从该类获取必要信息并赋值本类
+                self.left = value.left
+                self.right = value.right
+            else:  # 否则调用setfromlist函数
+                self.setfromlist(value)
+        except:
+            return(False)
+        else:
+            return(True)
+    
+    #def __setattr__(self, __name: str, __value: Any) -> None:  # 用于对一些关键的常量禁止赋值
+    #    pass
+
     def get_list(self) -> list:  # 从本类获得列表（结构同上）
         l = []  # 定义一个临时的列表
         l.append(self.val)  # 将初始节点参数加入列表
         if str(type(self.left)) in self.__t:  # 如果本类左值的类型也是本类
             l.append(self.left.get_list())  # 则调用该类的本函数取得列表，并加入临时列表
         else:
             l.append(self.left)  # 否则直接加入
@@ -40,14 +57,25 @@
         else:
             l.append(self.right)
         return(l)
 
     @property
     def listdata(self) -> list:  # 用于获取数的列表信息的只读属性
         return(self.get_list())
+    
+    #def get_list_from_depth(self, depth:int) -> list:  # 获取特定深度上的所有内容
+    #    if self.depth > depth:
+    #        pass
+    #    elif self.depth == depth:
+    #        pass
+    #    else:
+    #        return(None)
+
+    #def __getitem__(self, key:int) -> list:
+    #    return(self.get_list_from_depth(key))
 
     @property
     def depth(self) -> int:  # 用于获取数的深度信息的只读属性
         ld = 0
         if str(type(self.left)) in self.__t:  # 统计左树深度，如果左数类型是二叉树，则调用该类统计深度的属性
             ld += self.left.depth
         else:  # 否则加一
@@ -57,12 +85,18 @@
             rd += self.right.depth
         else:
             rd += 1
         return(max(ld, rd))  # 返回左右中的最大值
 
     def get_depth(self) -> int:  # 对于depth只读属性的函数封装
         return(self.depth)
-    #def getnode(self) -> str:
-    #    l = self.getlist()
+    
+    #@property
+    #def node(self) -> str:  # 返回一个简洁明了的二叉树字符串
+    #    #l = self.getlist()
     #    return("")
-    #def __str__(self) -> str:
-    #    return(self.getnode())
+    
+    #def getnode(self) -> str:
+    #    return(self.node)
+
+    #def __str__(self) -> str:  # 使开发者可以直接使用print函数打印二叉树
+    #    return(self.node)
```

### Comparing `phap-3.1.0a5/src/phap.egg-info/PKG-INFO` & `phap-3.1.0rc1/src/phap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phap
-Version: 3.1.0a5
+Version: 3.1.0rc1
 Summary: Programing Helpful Algorithm Package
 Home-page: https://github.com/DashBing/phap/
 Author: DashBing
 Author-email: mcbbkf@outlook.com
 Project-URL: Github, https://github.com/DashBing/phap/
 Project-URL: Old Project Version(stralgo), https://pypi.org/project/stralgo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,15 +38,15 @@
 + v2.2.1
 
 ## Latest Available Version
 + v3.0.0
 
 ## Latest Version
 ### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
-+ v3.1.0-alpha5
++ v3.1.0-rc1
 
 # To Use
 ## Read our development document
 ### *(Click the [Github](https://github.com/DashBing/phap/ "Github") link to read this document，or you may can not to open the link)*
 + [Development Document](doc/README.md)
 
 # Build
```

### Comparing `phap-3.1.0a5/src/phapbm/__init__.py` & `phap-3.1.0rc1/src/phapbm/__init__.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0a5/src/stralgo/__init__.py` & `phap-3.1.0rc1/src/stralgo/__init__.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0a5/src/stralgo/base.py` & `phap-3.1.0rc1/src/stralgo/base.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0a5/src/stralgo/hash/sm/sm3libs.py` & `phap-3.1.0rc1/src/stralgo/hash/sm/sm3libs.py`

 * *Files identical despite different names*

