# Comparing `tmp/fovus-1.0.8-py3-none-any.whl.zip` & `tmp/fovus-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 55019 bytes, number of entries: 47
+Zip file size: 55033 bytes, number of entries: 47
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/__init__.py
 -rw-r--r--  2.0 unx       65 b- defN 23-Apr-05 06:40 fovus/root_config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/adapter/__init__.py
 -rw-r--r--  2.0 unx     3331 b- defN 23-Apr-05 06:40 fovus/adapter/aws_cognito_adapter.py
 -rw-r--r--  2.0 unx    24371 b- defN 23-Jul-29 02:07 fovus/adapter/fovus_api_adapter.py
 -rw-r--r--  2.0 unx     9663 b- defN 23-Jul-29 02:07 fovus/adapter/fovus_s3_adapter.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/cli/__init__.py
 -rw-r--r--  2.0 unx    13657 b- defN 23-Jul-05 01:09 fovus/cli/cli_action_runner.py
 -rw-r--r--  2.0 unx      161 b- defN 23-Apr-05 06:56 fovus/cli/documenter.py
 -rw-r--r--  2.0 unx      997 b- defN 23-Jul-05 00:58 fovus/cli/fovus_cli.py
 -rw-r--r--  2.0 unx    30481 b- defN 23-Jul-29 02:07 fovus/cli/fovus_cli_argument_parser.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/config/__init__.py
--rw-r--r--  2.0 unx      840 b- defN 23-Jul-29 02:15 fovus/config/config.py
+-rw-r--r--  2.0 unx      840 b- defN 23-Jul-31 16:19 fovus/config/config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/constants/__init__.py
 -rw-r--r--  2.0 unx     1658 b- defN 23-Jul-29 02:07 fovus/constants/benchmark_constants.py
 -rw-r--r--  2.0 unx      485 b- defN 23-Jul-05 00:58 fovus/constants/cli_action_runner_constants.py
 -rw-r--r--  2.0 unx     9350 b- defN 23-Jul-29 02:07 fovus/constants/cli_constants.py
 -rw-r--r--  2.0 unx     1966 b- defN 23-Jul-29 02:07 fovus/constants/fovus_api_constants.py
 -rw-r--r--  2.0 unx      194 b- defN 23-Apr-05 06:40 fovus/constants/util_constants.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/exception/__init__.py
@@ -29,21 +29,21 @@
 -rw-r--r--  2.0 unx       39 b- defN 23-Jul-05 00:58 fovus/fovus_provided_configs/FOVUS_user_config_template.json
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/fovus_provided_configs/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/schema/__init__.py
 -rw-r--r--  2.0 unx    11652 b- defN 23-Jul-05 00:58 fovus/schema/create_job_schema.json
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/util/__init__.py
 -rw-r--r--  2.0 unx     3389 b- defN 23-Apr-05 06:40 fovus/util/aws_util.py
 -rw-r--r--  2.0 unx      334 b- defN 23-Apr-05 06:40 fovus/util/cli_action_runner_util.py
--rw-r--r--  2.0 unx     6733 b- defN 23-Jul-29 02:07 fovus/util/file_util.py
--rw-r--r--  2.0 unx    15038 b- defN 23-Jul-29 02:15 fovus/util/fovus_api_util.py
+-rw-r--r--  2.0 unx     6797 b- defN 23-Jul-31 16:19 fovus/util/file_util.py
+-rw-r--r--  2.0 unx    15038 b- defN 23-Jul-31 16:19 fovus/util/fovus_api_util.py
 -rw-r--r--  2.0 unx     1956 b- defN 23-Jul-05 00:58 fovus/util/fovus_cli_argument_parser_util.py
 -rw-r--r--  2.0 unx     1519 b- defN 23-Apr-05 06:40 fovus/util/fovus_s3_adapter_util.py
 -rw-r--r--  2.0 unx     1240 b- defN 23-Jul-05 01:09 fovus/util/util.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/validator/__init__.py
 -rw-r--r--  2.0 unx     4284 b- defN 23-Jul-05 01:09 fovus/validator/fovus_api_validator.py
--rw-r--r--  2.0 unx    14101 b- defN 23-Jul-29 02:26 fovus-1.0.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    12401 b- defN 23-Jul-29 02:26 fovus-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 02:26 fovus-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-Jul-29 02:26 fovus-1.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-29 02:26 fovus-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4188 b- defN 23-Jul-29 02:26 fovus-1.0.8.dist-info/RECORD
-47 files, 179516 bytes uncompressed, 48211 bytes compressed:  73.1%
+-rw-r--r--  2.0 unx    14101 b- defN 23-Jul-31 17:18 fovus-1.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    12401 b- defN 23-Jul-31 17:18 fovus-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 17:18 fovus-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Jul-31 17:18 fovus-1.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-31 17:18 fovus-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4188 b- defN 23-Jul-31 17:18 fovus-1.0.9.dist-info/RECORD
+47 files, 179580 bytes uncompressed, 48225 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -117,26 +117,26 @@
 
 Filename: fovus/validator/__init__.py
 Comment: 
 
 Filename: fovus/validator/fovus_api_validator.py
 Comment: 
 
-Filename: fovus-1.0.8.dist-info/LICENSE.txt
+Filename: fovus-1.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fovus-1.0.8.dist-info/METADATA
+Filename: fovus-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: fovus-1.0.8.dist-info/WHEEL
+Filename: fovus-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: fovus-1.0.8.dist-info/entry_points.txt
+Filename: fovus-1.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: fovus-1.0.8.dist-info/top_level.txt
+Filename: fovus-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: fovus-1.0.8.dist-info/RECORD
+Filename: fovus-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fovus/util/file_util.py

```diff
@@ -119,14 +119,16 @@
     def open(filepath, mode="r", encoding=UTF8):
         if mode.startswith("r") and not FileUtil.file_exists(filepath):
             raise UserException(
                 HTTPStatus.BAD_REQUEST,
                 FileUtil.__name__,
                 f"File does not exist: {filepath}",
             )
+        if "b" in mode:
+            return open(filepath, mode)
         return open(filepath, mode, encoding=encoding)
 
     @staticmethod
     def file_exists(filepath):
         return os.path.exists(filepath)
 
     @staticmethod
```

## Comparing `fovus-1.0.8.dist-info/LICENSE.txt` & `fovus-1.0.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fovus-1.0.8.dist-info/METADATA` & `fovus-1.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fovus
-Version: 1.0.8
+Version: 1.0.9
 Summary: The Fovus Python CLI
 Author: Fovus Corporation
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: boto3 (>=1.26.60)
 Requires-Dist: dateparser (>=1.1.8)
```

## Comparing `fovus-1.0.8.dist-info/RECORD` & `fovus-1.0.9.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 fovus/fovus_provided_configs/FOVUS_user_config_template.json,sha256=H7ePuIRbzYaTdL__NWh6XwRidLuN4Tue3yHY2lOArs4,39
 fovus/fovus_provided_configs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/schema/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/schema/create_job_schema.json,sha256=47IKcgmBu1y0j4edTW6LYnRvzTdy_hox99yuLkZe-k0,11652
 fovus/util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/util/aws_util.py,sha256=KX6DJIkwZ8ruToI8O0fK0TYEVxfyZI-p3NkRSSbGuVg,3389
 fovus/util/cli_action_runner_util.py,sha256=cPVVedOavu7nO_bbRS8wlipc2PCB-Q94BAMV3aopOYo,334
-fovus/util/file_util.py,sha256=_V9Bfai8xhyYIdO5Ht4IJH7-6vAG7tz8EdMdxtVtEYs,6733
+fovus/util/file_util.py,sha256=RYIY5OHNHI0GC5QsPpXl6GCVgngoD7st094bw5RzyTo,6797
 fovus/util/fovus_api_util.py,sha256=z_mH_yjeDmdq-V9jRc6G3tZQSoM66jytp0_9imd7yYQ,15038
 fovus/util/fovus_cli_argument_parser_util.py,sha256=XRLoaMCulYzh_Ew85imIwcZwb-8bEYT_gIpiodjwOuo,1956
 fovus/util/fovus_s3_adapter_util.py,sha256=WQwqgaeVttAUTJ2MyO9KFXpaIsVFwzcUM3K6xZ5oeFU,1519
 fovus/util/util.py,sha256=mjpVD723Uasdpq03TYGkn41NMmMG-0nO-HRXIzqmjFE,1240
 fovus/validator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/validator/fovus_api_validator.py,sha256=S5ZtFAb6dlJOcc-fgG5U-hJMo3xe8W20Yk3lpGOKnIc,4284
-fovus-1.0.8.dist-info/LICENSE.txt,sha256=fchJSAB0_4gOri4wW-wCs_gpi7L_-ece0Cr4YBsWojc,14101
-fovus-1.0.8.dist-info/METADATA,sha256=IvaTCGe5PQA64UTEakpGNyShfKZmB_rqtvSTB9rwPhg,12401
-fovus-1.0.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-fovus-1.0.8.dist-info/entry_points.txt,sha256=TjKfUkIuYlXaVbtONHkk38PSJmraR93NMOef9drKHu0,51
-fovus-1.0.8.dist-info/top_level.txt,sha256=oMIzxBylwDA2FvFy-uGFm6CKP6EhsbVzUlpaUdwtYGw,6
-fovus-1.0.8.dist-info/RECORD,,
+fovus-1.0.9.dist-info/LICENSE.txt,sha256=fchJSAB0_4gOri4wW-wCs_gpi7L_-ece0Cr4YBsWojc,14101
+fovus-1.0.9.dist-info/METADATA,sha256=gcIsjJ2xvSWLZ6ZO5BmkpwIKwbH2sg93sf98szi-DWE,12401
+fovus-1.0.9.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+fovus-1.0.9.dist-info/entry_points.txt,sha256=TjKfUkIuYlXaVbtONHkk38PSJmraR93NMOef9drKHu0,51
+fovus-1.0.9.dist-info/top_level.txt,sha256=oMIzxBylwDA2FvFy-uGFm6CKP6EhsbVzUlpaUdwtYGw,6
+fovus-1.0.9.dist-info/RECORD,,
```

