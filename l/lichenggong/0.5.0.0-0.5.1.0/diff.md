# Comparing `tmp/lichenggong-0.5.0.0.tar.gz` & `tmp/lichenggong-0.5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichenggong-0.5.0.0.tar", last modified: Wed Jul 19 23:28:03 2023, max compression
+gzip compressed data, was "lichenggong-0.5.1.0.tar", last modified: Mon Jul 31 02:05:36 2023, max compression
```

## Comparing `lichenggong-0.5.0.0.tar` & `lichenggong-0.5.1.0.tar`

### file list

```diff
@@ -1,33 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 23:28:03.278210 lichenggong-0.5.0.0/
--rw-rw-rw-   0        0        0      794 2023-07-19 23:28:03.276197 lichenggong-0.5.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-07-18 06:15:27.000000 lichenggong-0.5.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 23:28:03.185198 lichenggong-0.5.0.0/lichenggong/
-drwxrwxrwx   0        0        0        0 2023-07-19 23:28:03.224199 lichenggong-0.5.0.0/lichenggong/Noodows/
--rw-rw-rw-   0        0        0     3051 2023-07-18 07:03:53.000000 lichenggong-0.5.0.0/lichenggong/Noodows/__bios__.py
--rw-rw-rw-   0        0        0        0 2023-07-18 10:50:27.000000 lichenggong-0.5.0.0/lichenggong/Noodows/__init__.py
--rw-rw-rw-   0        0        0    11002 2023-07-19 23:07:31.000000 lichenggong-0.5.0.0/lichenggong/Noodows/__noodows__.py
--rw-rw-rw-   0        0        0        4 2023-05-01 01:01:06.000000 lichenggong-0.5.0.0/lichenggong/Noodows/first.txt
--rw-rw-rw-   0        0        0      372 2023-07-16 06:12:46.000000 lichenggong-0.5.0.0/lichenggong/Noodows/practice.py
--rw-rw-rw-   0        0        0        0 2023-07-16 12:12:38.000000 lichenggong-0.5.0.0/lichenggong/Noodows/python.txt
--rw-rw-rw-   0        0        0     2370 2023-07-19 23:27:57.000000 lichenggong-0.5.0.0/lichenggong/Noodows/update.log
-drwxrwxrwx   0        0        0        0 2023-07-19 23:28:03.231200 lichenggong-0.5.0.0/lichenggong/Noodows/version/
--rw-rw-rw-   0        0        0        9 2023-07-19 12:24:31.000000 lichenggong-0.5.0.0/lichenggong/Noodows/version/build_version.txt
--rw-rw-rw-   0        0        0        7 2023-07-19 23:26:31.000000 lichenggong-0.5.0.0/lichenggong/Noodows/version/version.txt
-drwxrwxrwx   0        0        0        0 2023-07-19 23:28:03.178200 lichenggong-0.5.0.0/lichenggong/Program_Files/
-drwxrwxrwx   0        0        0        0 2023-07-19 23:28:03.269197 lichenggong-0.5.0.0/lichenggong/Program_Files/System/
--rw-rw-rw-   0        0        0     5795 2023-07-19 23:22:45.000000 lichenggong-0.5.0.0/lichenggong/Program_Files/System/__calc__.py
--rw-rw-rw-   0        0        0     1699 2023-07-16 06:40:01.000000 lichenggong-0.5.0.0/lichenggong/Program_Files/System/__logo__.py
--rw-rw-rw-   0        0        0        0 2023-07-18 06:49:18.000000 lichenggong-0.5.0.0/lichenggong/Program_Files/System/__n_explorer__.py
--rw-rw-rw-   0        0        0     2468 2023-07-18 07:03:53.000000 lichenggong-0.5.0.0/lichenggong/Program_Files/System/__n_time__.py
--rw-rw-rw-   0        0        0      233 2023-07-18 06:21:05.000000 lichenggong-0.5.0.0/lichenggong/Program_Files/System/__thanks__.py
--rw-rw-rw-   0        0        0    24885 2023-07-19 23:01:43.000000 lichenggong-0.5.0.0/lichenggong/Program_Files/System/__user__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 23:28:03.272198 lichenggong-0.5.0.0/lichenggong/Program_Files/User/
--rw-rw-rw-   0        0        0        3 2023-07-08 09:50:30.000000 lichenggong-0.5.0.0/lichenggong/Program_Files/User/_.py
--rw-rw-rw-   0        0        0      874 2023-07-18 08:47:14.000000 lichenggong-0.5.0.0/lichenggong/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 23:28:03.198197 lichenggong-0.5.0.0/lichenggong.egg-info/
--rw-rw-rw-   0        0        0      794 2023-07-19 23:28:03.000000 lichenggong-0.5.0.0/lichenggong.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      807 2023-07-19 23:28:03.000000 lichenggong-0.5.0.0/lichenggong.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 23:28:03.000000 lichenggong-0.5.0.0/lichenggong.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-19 23:28:03.000000 lichenggong-0.5.0.0/lichenggong.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 23:28:03.279201 lichenggong-0.5.0.0/setup.cfg
--rw-rw-rw-   0        0        0      914 2023-07-18 10:24:28.000000 lichenggong-0.5.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:05:36.799138 lichenggong-0.5.1.0/
+-rw-rw-rw-   0        0        0      785 2023-07-31 02:05:36.799138 lichenggong-0.5.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-07-19 23:28:27.000000 lichenggong-0.5.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 02:05:36.580387 lichenggong-0.5.1.0/lichenggong/
+drwxrwxrwx   0        0        0        0 2023-07-31 02:05:36.752262 lichenggong-0.5.1.0/lichenggong/Noodows/
+-rw-rw-rw-   0        0        0     3162 2023-07-31 02:02:16.000000 lichenggong-0.5.1.0/lichenggong/Noodows/__bios__.py
+-rw-rw-rw-   0        0        0        0 2023-07-18 10:50:27.000000 lichenggong-0.5.1.0/lichenggong/Noodows/__init__.py
+-rw-rw-rw-   0        0        0    18219 2023-07-31 01:44:14.000000 lichenggong-0.5.1.0/lichenggong/Noodows/__noodows__.py
+-rw-rw-rw-   0        0        0        4 2023-05-01 01:01:06.000000 lichenggong-0.5.1.0/lichenggong/Noodows/first.txt
+-rw-rw-rw-   0        0        0      372 2023-07-16 06:12:46.000000 lichenggong-0.5.1.0/lichenggong/Noodows/practice.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 12:12:38.000000 lichenggong-0.5.1.0/lichenggong/Noodows/python.txt
+-rw-rw-rw-   0        0        0     2370 2023-07-19 23:27:57.000000 lichenggong-0.5.1.0/lichenggong/Noodows/update.log
+drwxrwxrwx   0        0        0        0 2023-07-31 02:05:36.752262 lichenggong-0.5.1.0/lichenggong/Noodows/version/
+-rw-rw-rw-   0        0        0        9 2023-07-19 12:24:31.000000 lichenggong-0.5.1.0/lichenggong/Noodows/version/build_version.txt
+-rw-rw-rw-   0        0        0        7 2023-07-31 02:03:53.000000 lichenggong-0.5.1.0/lichenggong/Noodows/version/version.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 02:05:36.564762 lichenggong-0.5.1.0/lichenggong/Program_Files/
+drwxrwxrwx   0        0        0        0 2023-07-31 02:05:36.799138 lichenggong-0.5.1.0/lichenggong/Program_Files/System/
+-rw-rw-rw-   0        0        0     5795 2023-07-19 23:22:45.000000 lichenggong-0.5.1.0/lichenggong/Program_Files/System/__calc__.py
+-rw-rw-rw-   0        0        0     1699 2023-07-16 06:40:01.000000 lichenggong-0.5.1.0/lichenggong/Program_Files/System/__logo__.py
+-rw-rw-rw-   0        0        0        0 2023-07-18 06:49:18.000000 lichenggong-0.5.1.0/lichenggong/Program_Files/System/__n_explorer__.py
+-rw-rw-rw-   0        0        0      233 2023-07-18 06:21:05.000000 lichenggong-0.5.1.0/lichenggong/Program_Files/System/__thanks__.py
+-rw-rw-rw-   0        0        0    24951 2023-07-31 01:44:14.000000 lichenggong-0.5.1.0/lichenggong/Program_Files/System/__user__.py
+-rw-rw-rw-   0        0        0      874 2023-07-18 08:47:14.000000 lichenggong-0.5.1.0/lichenggong/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:05:36.611641 lichenggong-0.5.1.0/lichenggong.egg-info/
+-rw-rw-rw-   0        0        0      785 2023-07-31 02:05:36.000000 lichenggong-0.5.1.0/lichenggong.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      724 2023-07-31 02:05:36.000000 lichenggong-0.5.1.0/lichenggong.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 02:05:36.000000 lichenggong-0.5.1.0/lichenggong.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-31 02:05:36.000000 lichenggong-0.5.1.0/lichenggong.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 02:05:36.799138 lichenggong-0.5.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      866 2023-07-31 02:05:32.000000 lichenggong-0.5.1.0/setup.py
```

### Comparing `lichenggong-0.5.0.0/PKG-INFO` & `lichenggong-0.5.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lichenggong
-Version: 0.5.0.0
+Version: 0.5.1.0
 Summary: python 3   windows 10 (best)
 Home-page: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -22,10 +22,10 @@
 3.wait for a little mins
 
 4.create new file "anything.py"
 
 5.(1).input "import lichenggong" and Enter in the file
 5.(2).input "lichenggong.start()" and Enter in the file
 
-6.double-click the file
+6.run the file
 
 python download by www.python.org/download
```

### Comparing `lichenggong-0.5.0.0/lichenggong/Noodows/__bios__.py` & `lichenggong-0.5.1.0/lichenggong/Noodows/__bios__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,16 @@
             elif filename.endswith('.txt'):
                 file_list.append(os.path.join(parent, filename))
                 # txt文件存储也算上
     for root, dirs, files in os.walk(files_dir):
         for file in files:
             size += os.path.getsize(os.path.join(root, file))
         count += len(files)
-    for f in file_list:
-        with open(f, encoding='UTF-8') as fp:
+    for i in file_list:
+        with open(i, encoding='UTF-8') as fp:
             code_num = 0  # 当前文件代码行数计数变量
             blank_num = 0  # 当前文件空行数计数变量
             annotate_num = 0  # 当前文件注释行数计数变量
             for content in fp.readlines():
                 content = content.strip()
                 # 统计空行
                 if content == '':
@@ -44,15 +44,15 @@
                     code_num += 1
         total_code_num += code_num
         total_blank_num += blank_num
         total_annotate_num += annotate_num
     # 返回代码行数，空行数，注释行数
     num = [total_code_num, total_blank_num, total_annotate_num]
     files = [num, count, size]
-    del size, count, fp, content, f
+    del size, count, fp, content, i
     del file_list, total_code_num, code_num, total_blank_num, blank_num, total_annotate_num, annotate_num
     gc.collect()
     return files
 
 
 def bios():
     __logo__.logo3_0()
@@ -63,21 +63,22 @@
         a = "|" * i
         b = "-" * (scale - i)
         c = (i / scale) * 100
         dur = t.perf_counter() - start
         print("Loading {:^3.0f}%[{}{}]{:.2f}s Noodows is coming".format(c, a, b, dur))
     print()
     a = file_dir('../')
-    print(' p() : {}'.format(a[0][0]))  # 返回代码行数
-    print(" ' '   : {}".format(a[0][1]))  # 返回空行数
-    print(' #   : {}'.format(a[0][2]))  # 返回注释行数
+    print('代码行: {}'.format(a[0][0]))  # 返回代码行数
+    print('空行数: {}'.format(a[0][1]))  # 返回空行数
+    print('注释行: {}'.format(a[0][2]))  # 返回注释行数
     for root, dirs, file in os.walk(file_name):
-        print(root)
-        print(dirs)
-        print(file)
+        print('File folder：{0}'.format(root))
+        print('Sub folders：{0}'.format(dirs))
+        print('Files:{0}'.format(file))
+        print('|' * 25)
     print('files:', a[1])
     print('large(MB)', a[2] / (1024 ** 2))
     print('hallo,world =) ')
     print()
     del a, root, dirs, file
     del i, scale, start, dur, b, c
     gc.collect()
```

### Comparing `lichenggong-0.5.0.0/lichenggong/Noodows/update.log` & `lichenggong-0.5.1.0/lichenggong/Noodows/update.log`

 * *Files identical despite different names*

### Comparing `lichenggong-0.5.0.0/lichenggong/Program_Files/System/__calc__.py` & `lichenggong-0.5.1.0/lichenggong/Program_Files/System/__calc__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.5.0.0/lichenggong/Program_Files/System/__logo__.py` & `lichenggong-0.5.1.0/lichenggong/Program_Files/System/__logo__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.5.0.0/lichenggong/Program_Files/System/__user__.py` & `lichenggong-0.5.1.0/lichenggong/Program_Files/System/__user__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def u_first():
     with open('../Noodows//version//version.txt', 'r') as Version_version:
         version = Version_version.readline()  # read the version
     with open('../Noodows//version//build_version.txt', 'r') as Build_version:
         build_version = Build_version.readline()  # read the version
     print()
-    print('您正在使用巨硬产品 noodows yee{0}(测试{1}) 无图像版 (用户创建区)'.format(version, build_version))
+    print('您正在使用巨硬产品 noodows {0}(测试{1}) 无图像版 (用户创建区)'.format(version, build_version))
     print("You're use noodows yee{0}(build{1}) no Image by Big-hard (setup user)".format(version, build_version))
     print()
     print("本系统基于交互环境")
     print()
     print('设置语言')
     print('Setup language')
     print()
@@ -67,17 +67,14 @@
             '需要密碼？         1.是 2.否',
             'password(first):',
             '密码(第一次):',
             '用戶密碼(初次):',
             'password(again):',
             '密码(第二次):',
             '用戶密碼(再次):',
-            "what's the user's power?         1.admin 2.user 3.visitor",
-            '此用户的权限是？         1.管理员 2.用户 3.游客',
-            '用戶權限？         1.管理 2.用戶 3.旅者',
             "that's your user,right?         1.yes 2.no",
             '这是否是你的用户？         1.是的 2.不是',
             '此是否是你的用戶？         1.是 2.否'
         ]
         if the_language == right_language:
             if model == 'print':
                 print(language_package[language_choose])
@@ -156,34 +153,34 @@
         # setup user password
         print()
         print('ID:{0}'.format(right_id))
         print('name:{0}'.format(right_name))
         print('password:{0}'.format(right_password))
         print('power:{0}'.format('admin'))
         print()
-        first_language_packager('US_en', 'input', 21)
-        first_language_packager('ZN_cn', 'input', 22)
-        first_language_packager('ZN_tw', 'input', 23)
+        first_language_packager('US_en', 'input', 18)
+        first_language_packager('ZN_cn', 'input', 19)
+        first_language_packager('ZN_tw', 'input', 20)
         choice = input()
         if choice == "1":
             print()
             print('马上就好')
             print("It'll only take a second")
             print()
             print('0%', end=" ")
-            folder = '../User//User' + right_id + '//'
-            folder_user_used = folder + 'User_used'
-            users_language = folder + 'language.txt'
-            users_name = folder + 'name.txt'
-            users_password = folder + 'password.txt'
-            users_power = folder + 'power.txt'
+            folder_user_used = '../User//User' + right_id + '//' + 'User_used'
+            users_language = '../User//User' + right_id + '//' + 'language.txt'
+            users_name = '../User//User' + right_id + '//' + 'name.txt'
+            users_password = '../User//User' + right_id + '//' + 'password.txt'
+            users_power = '../User//User' + right_id + '//' + 'power.txt'
+            users_use = '../Program_Files//User' + right_id + '//'
             print()
             print('10%', end=" ")
             try:
-                os.makedirs(folder)
+                os.makedirs('../User//User' + right_id + '//')
             except FileExistsError:
                 pass
             try:
                 os.makedirs(folder_user_used)
             except FileExistsError:
                 pass
             try:
@@ -226,23 +223,27 @@
             print('60%', end=" ")
             with open(users_power, 'w', encoding="utf-8") as Power:
                 Power.write('admin')
             with open('../User//UserPE//password.txt', 'w', encoding="utf-8") as Power:
                 Power.write('admin')
             print()
             print('100%')
+            try:
+                os.makedirs(users_use)
+            except FileExistsError:
+                pass
             break
         elif choice == '2':
             print("OK!let's back")
     print()
     print('欢迎使用')
     print('Thank you for your support!')
     del Version_version, version, Build_version, build_version, input_language, check_language, first_language_packager
     del input_id, check_id, input_name, check_name, check_password
-    del right_language, right_id, right_name, right_password
+    del right_language, right_id, right_name, right_password, users_use
     del choice, users_language, users_name, users_password, users_power, Language, Name, Password, Power
     gc.collect()
 
 
 def change():
     with open('../Noodows//version//version.txt', 'r') as Version_version:
         version = Version_version.readline()  # read the version
@@ -292,27 +293,26 @@
         try:
             with open(root + '//name.txt', 'r', encoding="utf-8") as name:
                 user_list.append(['ID:' + root.lstrip('..//User//User'), 'name:' + name.readline()])
         except FileNotFoundError:
             pass
     print('users:')
     print()
+    i = 0  # 初始
     while 1:
         try:
-            i = 0
             while 1:
                 print(user_list[i])
-                print()
                 i += 1
         except IndexError:
             i = 0
         while 1:
             try:
                 input_id = input("your user's ID:")
-                if user_list[i][0] != 'ID:' + str(input_id):
+                if user_list[i][0] != 'ID:' + input_id:
                     i += 1
                 else:
                     right_id = input_id
                     break
             except IndexError:
                 print('error: input an undefined thing')
             except TypeError:
@@ -593,12 +593,14 @@
             print('100%')
             break
         elif choice == '2':
             print("OK!let's back")
     print()
     print('欢迎使用')
     print('Thank you for your support!')
-    del Version_version, version, Build_version, build_version, input_language, check_language, language_packager
+    del Version_version, version, Build_version, build_version
+    del input_language, check_language, language_packager
     del input_id, check_id, input_name, check_name, check_password
     del right_language, right_id, right_name, right_password, right_power
-    del choice, users_language, users_name, users_password, users_power, Language, Name, Password, Power
-    gc.collect()
+    del choice, users_language, users_name, users_password,
+    del users_power, Language, Name, Password, Power
+    gc.collect()
```

### Comparing `lichenggong-0.5.0.0/lichenggong/__init__.py` & `lichenggong-0.5.1.0/lichenggong/__init__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.5.0.0/lichenggong.egg-info/PKG-INFO` & `lichenggong-0.5.1.0/lichenggong.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lichenggong
-Version: 0.5.0.0
+Version: 0.5.1.0
 Summary: python 3   windows 10 (best)
 Home-page: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -22,10 +22,10 @@
 3.wait for a little mins
 
 4.create new file "anything.py"
 
 5.(1).input "import lichenggong" and Enter in the file
 5.(2).input "lichenggong.start()" and Enter in the file
 
-6.double-click the file
+6.run the file
 
 python download by www.python.org/download
```

### Comparing `lichenggong-0.5.0.0/lichenggong.egg-info/SOURCES.txt` & `lichenggong-0.5.1.0/lichenggong.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -13,11 +13,9 @@
 lichenggong/Noodows/python.txt
 lichenggong/Noodows/update.log
 lichenggong/Noodows/version/build_version.txt
 lichenggong/Noodows/version/version.txt
 lichenggong/Program_Files/System/__calc__.py
 lichenggong/Program_Files/System/__logo__.py
 lichenggong/Program_Files/System/__n_explorer__.py
-lichenggong/Program_Files/System/__n_time__.py
 lichenggong/Program_Files/System/__thanks__.py
-lichenggong/Program_Files/System/__user__.py
-lichenggong/Program_Files/User/_.py
+lichenggong/Program_Files/System/__user__.py
```

### Comparing `lichenggong-0.5.0.0/setup.py` & `lichenggong-0.5.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     packages=['lichenggong',
               'lichenggong.Noodows',
               'lichenggong.Noodows.version',
-              'lichenggong.Program_Files.System',
-              'lichenggong.Program_Files.User'],
+              'lichenggong.Program_Files.System',],
     name="lichenggong",
     version=version,
     description="python 3   windows 10 (best)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='',
     package_data={'': ['*.py', '*.txt', '*.log']},
```

