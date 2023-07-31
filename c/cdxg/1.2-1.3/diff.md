# Comparing `tmp/cdxg-1.2-py3-none-any.whl.zip` & `tmp/cdxg-1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 77669 bytes, number of entries: 56
--rw-rw-rw-  2.0 fat      450 b- defN 23-Jul-31 14:11 cdxg/__init__.py
+Zip file size: 77674 bytes, number of entries: 56
+-rw-rw-rw-  2.0 fat      448 b- defN 23-Jul-31 14:51 cdxg/__init__.py
 -rw-rw-rw-  2.0 fat     5186 b- defN 23-Jul-31 14:02 cdxg/appdriver.py
 -rw-rw-rw-  2.0 fat    10698 b- defN 23-Jul-31 14:02 cdxg/case.py
 -rw-rw-rw-  2.0 fat    12703 b- defN 23-Jul-31 14:11 cdxg/cli.py
 -rw-rw-rw-  2.0 fat     5529 b- defN 23-Jul-31 14:02 cdxg/driver.py
 -rw-rw-rw-  2.0 fat    12321 b- defN 23-Jul-31 14:02 cdxg/request.py
 -rw-rw-rw-  2.0 fat     2990 b- defN 23-Jul-30 07:42 cdxg/skip.py
 -rw-rw-rw-  2.0 fat    30903 b- defN 23-Jul-31 14:02 cdxg/webdriver.py
@@ -45,14 +45,14 @@
 -rw-rw-rw-  2.0 fat      231 b- defN 23-Jul-30 07:42 cdxg/utils/jmespath.py
 -rw-rw-rw-  2.0 fat    10147 b- defN 23-Jul-31 14:02 cdxg/utils/jsonpath.py
 -rw-rw-rw-  2.0 fat     3838 b- defN 23-Jul-31 14:02 cdxg/utils/klook.py
 -rw-rw-rw-  2.0 fat     1022 b- defN 23-Jul-31 14:04 cdxg/utils/send_extend.py
 -rw-rw-rw-  2.0 fat     1517 b- defN 23-Jul-31 14:02 cdxg/utils/thread_lab.py
 -rw-rw-rw-  2.0 fat     1540 b- defN 23-Jul-30 07:42 cdxg/utils/tomorrow.py
 -rw-rw-rw-  2.0 fat     2007 b- defN 23-Jul-30 07:42 cdxg/utils/webdriver_manager_extend.py
--rw-rw-rw-  2.0 fat    11365 b- defN 23-Jul-31 14:12 cdxg-1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1486 b- defN 23-Jul-31 14:12 cdxg-1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 14:12 cdxg-1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       39 b- defN 23-Jul-31 14:12 cdxg-1.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-31 14:12 cdxg-1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     4466 b- defN 23-Jul-31 14:12 cdxg-1.2.dist-info/RECORD
-56 files, 250401 bytes uncompressed, 70711 bytes compressed:  71.8%
+-rw-rw-rw-  2.0 fat    11365 b- defN 23-Jul-31 14:52 cdxg-1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1486 b- defN 23-Jul-31 14:52 cdxg-1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 14:52 cdxg-1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       39 b- defN 23-Jul-31 14:52 cdxg-1.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-31 14:52 cdxg-1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     4466 b- defN 23-Jul-31 14:52 cdxg-1.3.dist-info/RECORD
+56 files, 250399 bytes uncompressed, 70716 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -144,26 +144,26 @@
 
 Filename: cdxg/utils/tomorrow.py
 Comment: 
 
 Filename: cdxg/utils/webdriver_manager_extend.py
 Comment: 
 
-Filename: cdxg-1.2.dist-info/LICENSE
+Filename: cdxg-1.3.dist-info/LICENSE
 Comment: 
 
-Filename: cdxg-1.2.dist-info/METADATA
+Filename: cdxg-1.3.dist-info/METADATA
 Comment: 
 
-Filename: cdxg-1.2.dist-info/WHEEL
+Filename: cdxg-1.3.dist-info/WHEEL
 Comment: 
 
-Filename: cdxg-1.2.dist-info/entry_points.txt
+Filename: cdxg-1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: cdxg-1.2.dist-info/top_level.txt
+Filename: cdxg-1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: cdxg-1.2.dist-info/RECORD
+Filename: cdxg-1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cdxg/__init__.py

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/python
 
 from .case import TestCase
-from .running.config import Seldom
+from .running.config import Cdxg
 from .running.loader_extend import SeldomTestLoader
 from .running.runner import main, TestMainExtend
 from .utils.send_extend import SMTP
 from .webdriver_chaining import Steps
 
 from .skip import *
 from .driver import *
 from .testdata.parameterization import *
 
 
 __author__ = "mastersaa"
 
-__version__ = "1.2"
+__version__ = "1.3"
 
 __description__ = "WebUI/HTTP automation testing framework."
```

## Comparing `cdxg-1.2.dist-info/LICENSE` & `cdxg-1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cdxg-1.2.dist-info/METADATA` & `cdxg-1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdxg
-Version: 1.2
+Version: 1.3
 Summary: Cdxg automation testing framework.
 Home-page: https://github.com/saasaa831/cdxg/
 Author: mastersaa
 Author-email: mastersaa@saa.com
 License: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
```

## Comparing `cdxg-1.2.dist-info/RECORD` & `cdxg-1.3.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-cdxg/__init__.py,sha256=l8JGk4WswvG3B2iC8nuBBEWBBuJkZC_u3SKeAsN06h0,450
+cdxg/__init__.py,sha256=BEvPTFnmlN25U2Gf97SKYt54ys6xm-QQZtYeNWXXBYk,448
 cdxg/appdriver.py,sha256=EZ2ByvLOzCRwhE29u7soZ5DNFY6ijgz7HWqOQvbv3zM,5186
 cdxg/case.py,sha256=aS2NgvbHRQrWTjnjW4kOddhrgf1N5YUCHF4_ddB3FhA,10698
 cdxg/cli.py,sha256=qxY-iERiAFQtLHXi7HmMhpvNzng_LJHzsIIG8RiUupY,12703
 cdxg/driver.py,sha256=3wpc9WU15sHWhc6BGDN2PVToLm4dcSxdV8DHO65loSU,5529
 cdxg/request.py,sha256=qpnOEy-5BydiqVPXRxCXUkVdoqUACRKGUFAmRw7RBeo,12321
 cdxg/skip.py,sha256=s6uFNLBhpdjtvlc9SRUDnel86LGLFOOFc2eWdRCx38k,2990
 cdxg/webdriver.py,sha256=F5Dqsm0DU_69deHuFy0oH6xFFui0g2wYlbUsx0s8-g8,30903
@@ -44,13 +44,13 @@
 cdxg/utils/jmespath.py,sha256=w1oGyKDZeRadKs1VhfGxxSC0lA02WoWSRJFhsohWBdE,231
 cdxg/utils/jsonpath.py,sha256=v9a_Xa9mSb33_v9GosJzXEnkvZ12JlNfPO9HP_pwcLo,10147
 cdxg/utils/klook.py,sha256=yNj5fpTvXTrFcpG6QIdlfRyALiXvxv1SY3bOt73rH3w,3838
 cdxg/utils/send_extend.py,sha256=DQos54pJfKJWFZbOMArG9JfVd-X7cJImIFtZZdbKrGw,1022
 cdxg/utils/thread_lab.py,sha256=jg88RJWxxZ9KxwSM1D6WURf3dglGjI0fLK2jQ1juf0w,1517
 cdxg/utils/tomorrow.py,sha256=0n2HnZs3hgPvl4GSdWr67HKNavI4kolterQ4GO2OV3I,1540
 cdxg/utils/webdriver_manager_extend.py,sha256=cAt79207WjIK-HMyX0GtS6RHsihVJbqbPTeM7pcMpTA,2007
-cdxg-1.2.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
-cdxg-1.2.dist-info/METADATA,sha256=SxN_EY8McTJ2rNyY2hAwdbuppgLXhvZnomCLXEQb-Yk,1486
-cdxg-1.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-cdxg-1.2.dist-info/entry_points.txt,sha256=Y47sdYbkBUR5vlzktnMU9fG9omTvyDI3Zdl5Brm2Tak,39
-cdxg-1.2.dist-info/top_level.txt,sha256=R23-9xmHOZfvofHb5OY2Rgjnpm906bU4Ch-Rz2MCDpM,5
-cdxg-1.2.dist-info/RECORD,,
+cdxg-1.3.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
+cdxg-1.3.dist-info/METADATA,sha256=gIZ60k1TwwTxpx81JiK3fpwzxpRSzwhJ9MPOOnZDOyk,1486
+cdxg-1.3.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+cdxg-1.3.dist-info/entry_points.txt,sha256=Y47sdYbkBUR5vlzktnMU9fG9omTvyDI3Zdl5Brm2Tak,39
+cdxg-1.3.dist-info/top_level.txt,sha256=R23-9xmHOZfvofHb5OY2Rgjnpm906bU4Ch-Rz2MCDpM,5
+cdxg-1.3.dist-info/RECORD,,
```

