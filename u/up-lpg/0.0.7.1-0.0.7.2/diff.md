# Comparing `tmp/up_lpg-0.0.7.1-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/up_lpg-0.0.7.2-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1190518 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       36 b- defN 23-Jul-06 13:00 up_lpg/__init__.py
--rw-rw-rw-  2.0 fat    10927 b- defN 23-Jul-06 13:00 up_lpg/lpg_planner.py
--rw-rw-rw-  2.0 fat  3881596 b- defN 23-Jul-06 13:00 up_lpg/winlpg.exe
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-06 13:10 up_lpg-0.0.7.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      336 b- defN 23-Jul-06 13:10 up_lpg-0.0.7.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-06 13:10 up_lpg-0.0.7.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-06 13:10 up_lpg-0.0.7.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      620 b- defN 23-Jul-06 13:10 up_lpg-0.0.7.1.dist-info/RECORD
-8 files, 3905187 bytes uncompressed, 1189448 bytes compressed:  69.5%
+Zip file size: 1190589 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       36 b- defN 23-Jul-31 09:48 up_lpg/__init__.py
+-rw-rw-rw-  2.0 fat    11111 b- defN 23-Jul-31 09:48 up_lpg/lpg_planner.py
+-rw-rw-rw-  2.0 fat  3881596 b- defN 23-Jul-31 09:48 up_lpg/winlpg.exe
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-31 09:55 up_lpg-0.0.7.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      336 b- defN 23-Jul-31 09:55 up_lpg-0.0.7.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-31 09:55 up_lpg-0.0.7.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-31 09:55 up_lpg-0.0.7.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      620 b- defN 23-Jul-31 09:55 up_lpg-0.0.7.2.dist-info/RECORD
+8 files, 3905371 bytes uncompressed, 1189519 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: up_lpg/lpg_planner.py
 Comment: 
 
 Filename: up_lpg/winlpg.exe
 Comment: 
 
-Filename: up_lpg-0.0.7.1.dist-info/LICENSE
+Filename: up_lpg-0.0.7.2.dist-info/LICENSE
 Comment: 
 
-Filename: up_lpg-0.0.7.1.dist-info/METADATA
+Filename: up_lpg-0.0.7.2.dist-info/METADATA
 Comment: 
 
-Filename: up_lpg-0.0.7.1.dist-info/WHEEL
+Filename: up_lpg-0.0.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: up_lpg-0.0.7.1.dist-info/top_level.txt
+Filename: up_lpg-0.0.7.2.dist-info/top_level.txt
 Comment: 
 
-Filename: up_lpg-0.0.7.1.dist-info/RECORD
+Filename: up_lpg-0.0.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## up_lpg/lpg_planner.py

```diff
@@ -23,27 +23,31 @@
                   'LPG (Local search for Planning Graphs) is a planner based on local search and planning graphs.')
 
 lpg_os = {'win32':'winlpg.exe',
           'linux': 'lpg'}
 
 LPG_EPSILON = 0.00025
 
-class LPGEngine(PDDLPlanner):
+class LPGEngine(PDDLPlanner): 
 
-    def __init__(self):
+    def __init__(self, **kwargs):
         super().__init__(needs_requirements=False)
-        self._options = []
+        self.parameter = []
+        for param, val in kwargs.items():
+            self.parameter.append(str(param))
+            if val != '':
+                self.parameter.append(str(val))
 
     @property
     def name(self) -> str:
         return 'lpg'
 
     def _get_cmd(self, domain_filename: str, problem_filename: str, plan_filename: str) -> List[str]:
-        base_command = [pkg_resources.resource_filename(__name__, lpg_os[sys.platform]), '-o', domain_filename, '-f', problem_filename, '-n', '1', '-out', plan_filename]  + self._options
-        return base_command
+            base_command = pkg_resources.resource_filename(__name__, lpg_os[sys.platform]), '-o', domain_filename, '-f', problem_filename, '-n', '1', '-out', plan_filename, *self.parameter
+            return base_command
 
     def  _get_engine_epsilon(self) -> Optional[Fraction]:
         return LPG_EPSILON
 
     def _plan_from_file(self, problem: 'up.model.Problem', plan_filename: str, get_item_named: Callable[[str],
             Union[
                 'up.model.Type',
```

## Comparing `up_lpg-0.0.7.1.dist-info/LICENSE` & `up_lpg-0.0.7.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `up_lpg-0.0.7.1.dist-info/RECORD` & `up_lpg-0.0.7.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 up_lpg/__init__.py,sha256=cD1uY16onwsxHOEI1I-lmF6WlYtDKB8YOie6BNUZji0,36
-up_lpg/lpg_planner.py,sha256=uijXYalCXE4L9prL3h7i6JYlIgS_GS8TygTUVR66YTQ,10927
+up_lpg/lpg_planner.py,sha256=xGXYxV0or_0rB5diYwxE5riyAHG4KKcvq-nWVDylLSs,11111
 up_lpg/winlpg.exe,sha256=Ut1frT86CopooTsvbc20MyQGGUrmRtWnVLObmzp4v4w,3881596
-up_lpg-0.0.7.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-up_lpg-0.0.7.1.dist-info/METADATA,sha256=68ECDsHWFdx6N0aqvIIMm9odsKovauJEmQ7nJfgmfq0,336
-up_lpg-0.0.7.1.dist-info/WHEEL,sha256=kbzA5tyEuvWcVsltnhCG02Vwq0RkG0K4o74bVDVA1mQ,107
-up_lpg-0.0.7.1.dist-info/top_level.txt,sha256=p4RjFqpyQ96YXeEcg2Qtkfgt61fd_rOwRCePcthjdUk,7
-up_lpg-0.0.7.1.dist-info/RECORD,,
+up_lpg-0.0.7.2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+up_lpg-0.0.7.2.dist-info/METADATA,sha256=A_BpFV3LdFImlbxhBvaBd4gVGJPk9S_kX4TjtI6LC3g,336
+up_lpg-0.0.7.2.dist-info/WHEEL,sha256=kbzA5tyEuvWcVsltnhCG02Vwq0RkG0K4o74bVDVA1mQ,107
+up_lpg-0.0.7.2.dist-info/top_level.txt,sha256=p4RjFqpyQ96YXeEcg2Qtkfgt61fd_rOwRCePcthjdUk,7
+up_lpg-0.0.7.2.dist-info/RECORD,,
```

