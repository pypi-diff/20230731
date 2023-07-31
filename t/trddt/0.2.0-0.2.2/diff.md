# Comparing `tmp/trddt-0.2.0.tar.gz` & `tmp/trddt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trddt-0.2.0.tar", last modified: Mon Jul 31 05:20:50 2023, max compression
+gzip compressed data, was "trddt-0.2.2.tar", last modified: Mon Jul 31 13:58:58 2023, max compression
```

## Comparing `trddt-0.2.0.tar` & `trddt-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:50.431042 trddt-0.2.0/
--rw-rw-rw-   0        0        0     1086 2023-07-31 05:08:10.000000 trddt-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      678 2023-07-31 05:20:50.430041 trddt-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-31 05:13:45.000000 trddt-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-31 05:20:50.432042 trddt-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      869 2023-07-31 05:12:43.000000 trddt-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:50.389033 trddt-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:50.399035 trddt-0.2.0/src/trddt/
--rw-rw-rw-   0        0        0    10486 2023-06-07 08:52:40.000000 trddt-0.2.0/src/trddt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:20:50.427042 trddt-0.2.0/src/trddt.egg-info/
--rw-rw-rw-   0        0        0      678 2023-07-31 05:20:50.000000 trddt-0.2.0/src/trddt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-07-31 05:20:50.000000 trddt-0.2.0/src/trddt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 05:20:50.000000 trddt-0.2.0/src/trddt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-31 05:20:50.000000 trddt-0.2.0/src/trddt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-31 05:20:50.000000 trddt-0.2.0/src/trddt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 13:58:58.183799 trddt-0.2.2/
+-rw-rw-rw-   0        0        0     1086 2023-07-31 05:08:10.000000 trddt-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      678 2023-07-31 13:58:58.181800 trddt-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-31 05:13:45.000000 trddt-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 13:58:58.183799 trddt-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      888 2023-07-31 13:57:58.000000 trddt-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 13:58:58.144791 trddt-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 13:58:58.153793 trddt-0.2.2/src/trddt/
+-rw-rw-rw-   0        0        0    10983 2023-07-31 13:54:56.000000 trddt-0.2.2/src/trddt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 13:58:58.179799 trddt-0.2.2/src/trddt.egg-info/
+-rw-rw-rw-   0        0        0      678 2023-07-31 13:58:58.000000 trddt-0.2.2/src/trddt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-07-31 13:58:58.000000 trddt-0.2.2/src/trddt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 13:58:58.000000 trddt-0.2.2/src/trddt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-31 13:58:58.000000 trddt-0.2.2/src/trddt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-31 13:58:58.000000 trddt-0.2.2/src/trddt.egg-info/top_level.txt
```

### Comparing `trddt-0.2.0/LICENSE` & `trddt-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trddt-0.2.0/PKG-INFO` & `trddt-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trddt
-Version: 0.2.0
+Version: 0.2.2
 Summary: 한국거래소 기준 Datetime Functions 패키지
 Home-page: https://github.com/innovata/TradeDatetime
 Author: innovata
 Author-email: iinnovata@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trddt-0.2.0/setup.py` & `trddt-0.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 SOURCE_DIRECTORY = 'src'
 
 setuptools.setup(
     name="trddt",
-    version="0.2.0",
+    version="0.2.2",
     author="innovata",
     author_email="iinnovata@gmail.com",
     description='한국거래소 기준 Datetime Functions 패키지',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/innovata/TradeDatetime",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": SOURCE_DIRECTORY},
     packages=setuptools.find_packages(SOURCE_DIRECTORY),
     python_requires=">=3.8",
-    install_requires=['ipylib', 'holidays', 'pandas'],
+    install_requires=['ipylib', 'holidays', 'pandas','xlrd', 'openpyxl'],
 )
```

### Comparing `trddt-0.2.0/src/trddt/__init__.py` & `trddt-0.2.2/src/trddt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,79 +1,91 @@
 # -*- coding: utf-8 -*-
 from datetime import datetime, date, timedelta, time, tzinfo, timezone
 import re
 import os 
-from zipfile import ZipFile
+import zipfile
 
 
 import pandas as pd
 import holidays
 
 
 from ipylib.idebug import *
 from ipylib import ipath
 from ipylib.idatetime import DatetimeParser
 
 
-import CONF_FILE
-
 
 File = {
     'InitYear':1980,
     'TimezoneName':'Asia/Seoul',
     'TimezoneHour':+9,
     'MarketTime':{
         '정규장 매매가능 시작시간':{'hour':8, 'minute':20},
         '장전 동시호가 시작시간':{'hour':8, 'minute':30},
     }
 }
 
 
 
-def download_file(): pass 
+     
+
+
+DATA_PATH = os.path.dirname(__file__)
 
 
-def build_HolidaysCSV():
-    """압축파일풀기 & 엑셀파일 읽어들이기"""
-    data_path = os.path.join(CONF_FILE.PROJECT_PATH, 'Data')
-    zip_file = os.path.join(data_path, 'Holidays.xlsx.zip')
-    ZipFile(zip_file).extractall(data_path)
-    xls_file, ext = os.path.splitext(zip_file)
-    df = pd.read_excel(xls_file)
+@ftracer
+def build_HolidaysCSV(file='C:\pypjts\TradeDatetime\Holidays.xlsx'):
+    """Zip파일인지, 엑셀파일인지 감지 후 자동으로 압축풀기"""
+    root, ext = os.path.splitext(os.path.basename(file))
+    if ext == '.xlsx':
+        xls_path = os.path.realpath(file)
+        # print({'xls_path': xls_path})
+        xls_dir = os.path.dirname(xls_path)
+        xls_file = os.path.basename(xls_path)
+        # pp.pprint([xls_path, xls_dir, xls_file])
+    elif ext == '.zip':
+        """압축파일풀기"""
+        zip_path = os.path.abspath(file)
+        zip_dir = os.path.dirname(zip_path)
+        zip_file = os.path.basename(zip_path)
+        xls_file, ext = os.path.splitext(zip_file)
+        xls_path = os.path.join(zip_dir, xls_file)
+        # pp.pprint([zip_dir, zip_file, xls_file, ext, xls_path])
+        zipfile.ZipFile(zip_path).extractall(zip_dir)
+
+    """엑셀파일 읽기"""
+    filename, ext = os.path.splitext(xls_file)
+    # pp.pprint([filename, ext])
+    df = pd.read_excel(xls_path)
+    print(df)
     
     """CSV파일로 변환저장"""
-    filename, ext = os.path.splitext(xls_file)
-    csv_file = filename + '.csv'
-    csv_file = os.path.join(data_path, csv_file)
-    df.to_csv(csv_file, index=False)
-
-    """엑셀파일삭제"""
-    try:
-        os.remove(xls_file)
-    except Exception as e:
-        logger.error(e)
-    return df 
-
+    csv_path = os.path.join(DATA_PATH, filename+'.csv')
+    df.to_csv(csv_path, index=False)
 
 
 def get_Holidays():
-    data_path = os.path.join(CONF_FILE.PROJECT_PATH, 'Data')
-    csv_file = os.path.join(data_path, 'Holidays.csv')
+    csv_file = os.path.join(DATA_PATH, 'Holidays.csv')
     df = pd.read_csv(csv_file)
     # df.info()
     # print(df)
     # return df 
     days = list(df.Date)
-    days = [datetime.strptime(t, '%Y-%m-%d') for t in days]
+    days = [datetime.strptime(t, "%Y-%m-%d").astimezone() for t in days]
     return days
 
 
 HOLIDAYS = get_Holidays()
 
 
+def isin_holiday(t):
+    # _t = t.strftime('%Y-%m-%d')
+    return True if t in HOLIDAYS else False
+
 
 def now(microsecond=True, testnow=None):
     t = datetime.today().astimezone()
     if microsecond: pass
     else: t = t.replace(microsecond=0)
 
     # if testnow is None: pass
@@ -92,18 +104,14 @@
 def today(): return now().replace(hour=0, minute=0, second=0, microsecond=0)
 
 
 """법정공휴일 or 주말 제외"""
 def _exclude(t, unit):
     
 
-    def isin_holiday(t):
-        _t = t.strftime('%Y-%m-%d')
-        return True if _t in HOLIDAYS else False
-
     while t.weekday() in [5,6] or isin_holiday(t):
         t += timedelta(days=unit)
     return t
 
 """증권시스템상 새벽시간은 이전날짜로 취급한다"""
 def _adjust_midnight(t, **kw):
     _now = now()
@@ -131,15 +139,15 @@
 def time(t=None, delta=0):
     t = now() if t is None else DatetimeParser(t)
     t = _adjust_midnight(t, hours=6)
     t = _exclude(t, -1)
     return t
 
 
-"""예측일|거래예정일"""
+"""예측일|거래예정일::최종거래일을 입력하면 거래예정일을 반환한다"""
 def predict_day(lastday=None):
 
     # 시간대에 따른 조정
     _now = now()
     if 0 <= _now.hour < 7:
         day = date(lastday, delta=+1)
     elif 7<= _now.hour < 20:
```

### Comparing `trddt-0.2.0/src/trddt.egg-info/PKG-INFO` & `trddt-0.2.2/src/trddt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trddt
-Version: 0.2.0
+Version: 0.2.2
 Summary: 한국거래소 기준 Datetime Functions 패키지
 Home-page: https://github.com/innovata/TradeDatetime
 Author: innovata
 Author-email: iinnovata@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

