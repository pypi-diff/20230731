# Comparing `tmp/wfsx-1.1-py3-none-any.whl.zip` & `tmp/wfsx-1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 30934 bytes, number of entries: 19
+Zip file size: 31395 bytes, number of entries: 19
 -rw-rw-rw-  2.0 fat      413 b- defN 23-Jun-06 11:13 wfsx/CONST_j.py
 -rw-rw-rw-  2.0 fat     5163 b- defN 23-Jul-28 14:45 wfsx/Excel_x.py
 -rw-rw-rw-  2.0 fat     5280 b- defN 23-Jul-28 14:45 wfsx/Report.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 11:13 wfsx/__init__.py
 -rw-rw-rw-  2.0 fat     6310 b- defN 23-Jul-28 14:31 wfsx/api.py
 -rw-rw-rw-  2.0 fat     6019 b- defN 23-Jun-15 14:25 wfsx/apivalid.py
 -rw-rw-rw-  2.0 fat    16574 b- defN 23-Jul-28 14:41 wfsx/apivalidation.py
 -rw-rw-rw-  2.0 fat    20705 b- defN 23-Jul-28 16:02 wfsx/common.py
--rw-rw-rw-  2.0 fat     9505 b- defN 23-Jul-28 14:45 wfsx/dataextract.py
+-rw-rw-rw-  2.0 fat    12039 b- defN 23-Jul-31 14:22 wfsx/dataextract.py
 -rw-rw-rw-  2.0 fat     2808 b- defN 23-Jun-06 11:13 wfsx/excel_json_reader.py
 -rw-rw-rw-  2.0 fat     4189 b- defN 23-Jun-16 15:41 wfsx/ghelper.py
 -rw-rw-rw-  2.0 fat     5407 b- defN 23-Jun-06 11:13 wfsx/parseexcel.py
 -rw-rw-rw-  2.0 fat     7022 b- defN 23-Jun-13 11:44 wfsx/plite.py
 -rw-rw-rw-  2.0 fat    23242 b- defN 23-Jul-28 14:45 wfsx/results_validate.py
--rw-rw-rw-  2.0 fat    11365 b- defN 23-Jul-28 16:03 wfsx-1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1235 b- defN 23-Jul-28 16:03 wfsx-1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-28 16:03 wfsx-1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-28 16:03 wfsx-1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1394 b- defN 23-Jul-28 16:03 wfsx-1.1.dist-info/RECORD
-19 files, 126728 bytes uncompressed, 28728 bytes compressed:  77.3%
+-rw-rw-rw-  2.0 fat    11365 b- defN 23-Jul-31 14:22 wfsx-1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1260 b- defN 23-Jul-31 14:22 wfsx-1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 14:22 wfsx-1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-31 14:22 wfsx-1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1395 b- defN 23-Jul-31 14:22 wfsx-1.2.dist-info/RECORD
+19 files, 129288 bytes uncompressed, 29189 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: wfsx/plite.py
 Comment: 
 
 Filename: wfsx/results_validate.py
 Comment: 
 
-Filename: wfsx-1.1.dist-info/LICENSE
+Filename: wfsx-1.2.dist-info/LICENSE
 Comment: 
 
-Filename: wfsx-1.1.dist-info/METADATA
+Filename: wfsx-1.2.dist-info/METADATA
 Comment: 
 
-Filename: wfsx-1.1.dist-info/WHEEL
+Filename: wfsx-1.2.dist-info/WHEEL
 Comment: 
 
-Filename: wfsx-1.1.dist-info/top_level.txt
+Filename: wfsx-1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: wfsx-1.1.dist-info/RECORD
+Filename: wfsx-1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wfsx/dataextract.py

```diff
@@ -162,34 +162,47 @@
     # Use regular expressions to find the string inside the braces
     try:
         if '$' in ddata:
             xid = []
             match = re.findall(r'\$(.*?)\$', ddata)
             gnx = 0
             for variable in match:
+                if '|' in variable:
+                    dfile, dxt, appoint, gtxa = variable.split('|')
+                    if appoint != apipoint and appoint is not None:
+                        apipoint = appoint
+                    else:
+                        apipoint = apipoint
                 exresults, gnx, gxa = extractedValue(tdata=variable, apipoint=apipoint, gnx=gnx)
                 xid.append(exresults)
                 gnx = gnx
             keys, values = xid, match
             for pattern, replacements in zip(values, keys):
                 rpurl = ddata.replace('$' + pattern + '$', str(replacements))
                 ddata = rpurl
             return ddata
         else:
             if '{}' in ddata:
                 return ddata
             else:
                 match = re.search(r'{(.*?)}', ddata)
-                pattern = r'\{[^{}]+\}'
-                matching_variables = re.findall(pattern, ddata)
+                # pattern = r'\{[^{}]+\}'
+                # matching_variables = re.findall(pattern, ddata)
                 if match:
                     # Extract the string inside the braces
                     extracted_string = match.group(1)
+                    if '|' in extracted_string:
+                        dfile, dxt, appoint, gtxa = extracted_string.split('|')
+                        if appoint != apipoint and appoint is not None:
+                            apipoint = appoint
+                        else:
+                            apipoint = apipoint
+                        # print(dfile,dxt, apipoint, gtxa)
                     # exresults = get_nested_value(data=payload, keys=extracted_string)
-                    exresults, gnx, gxa = extractedValue(tdata=extracted_string, apipoint=str(apipoint).split(':')[1])
+                    exresults, gnx, gxa = extractedValue(tdata=extracted_string, apipoint=apipoint)
                     # replaced_string = re.sub(r'{(.*?)}', extracted_string, exresults)
                     replaced_string = ddata.replace(str('{' + extracted_string + '}'), str(exresults))
                     return replaced_string
                 else:
                     return ddata
     except Exception as e:
         return str(e)
@@ -198,30 +211,43 @@
 def get_defined_data(apipoint, ddata):
     # Use regular expressions to find the string inside the braces
     try:
         global dResults, extnurl
         if '$' in ddata:
             xid = []
             match = re.findall(r'\$(.*?)\$', ddata)
-            # print(match)
             gnx = 0
             for variable in match:
+                if '|' in variable:
+                    dfile, dxt, appoint, gtxa = variable.split('|')
+                    if appoint != apipoint and appoint is not None:
+                        apipoint = appoint
+                    else:
+                        apipoint = apipoint
                 exresults, gnx, gxa = extractedValue(tdata=variable, apipoint=apipoint, gnx=gnx)
                 xid.append(exresults)
                 gnx = gnx
             keys, values = xid, match
             for pattern, replacements in zip(values, keys):
                 rpurl = ddata.replace('$' + pattern + '$', str(replacements))
                 ddata = rpurl
             return ddata
         else:
             match = re.search(r'{(.*?)}', ddata)
             if match:
                 extracted_string = match.group(1)
+                if '|' in extracted_string:
+                    dfile, dxt, appoint, gtxa = extracted_string.split('|')
+                    if appoint != apipoint and appoint is not None:
+                        apipoint = appoint
+                    else:
+                        apipoint = apipoint
+                    # print(dfile,dxt, apipoint, gtxa)
                 exresults, gnx, gxa = extractedValue(tdata=extracted_string, apipoint=apipoint)
+                # print(exresults, gnx, gxa)
                 if gxa in ['S1', 'S2']:
                     dResults = exresults
                 else:
                     if type(exresults[0]) == list:
                         dResults = []
                         for xresults in exresults[0]:
                             dResults.append(str(xresults))
@@ -230,7 +256,41 @@
                         dResults = exresults[0]
                 replaced_string = ddata.replace('{' + extracted_string + '}', str(dResults))
                 return replaced_string
             else:
                 return ddata
     except Exception as e:
         return ddata
+
+def get_entries(apiendpoint):
+    if '/' in apiendpoint:
+        apoint = str(apiendpoint).split('/')
+        apiendpoint = get_defined_data(apipoint=getepoint(apoint), ddata=apiendpoint)
+        return apiendpoint, getepoint(apoint)  # apoint[len(apoint) - 1]
+    else:
+        return apiendpoint, apiendpoint
+
+def getDataSql(sQLx, dbname):
+    # Get results using Sqlite3
+    sqlx, tbname, query = str(sQLx).split('|')
+    global apipoint
+    if '_' in dbname:
+        xpoint = str(dbname).split('_')
+        if len(xpoint) > 2:
+            abx = []
+            for lex in range(0, 2):
+                abx.append(xpoint[lex])
+            apipoint = '_'.join(abx)
+        else:
+            apipoint = str(xpoint[0])
+    tbname = apipoint + '_' + tbname
+    getresult = engConnect(rindex=tbname, getdata=query, dbname=str(dbname) + '.db')
+    return getresult
+
+def getbaseUrl(ddata, urlString):
+    match = re.search(r'{(.*?)}', ddata)
+    print(match)
+    if match:
+        extracted_string = match.group(1)
+        replaced_string = ddata.replace(str('{' + extracted_string + '}'), str(urlString))
+        print(replaced_string)
+        return replaced_string
```

## Comparing `wfsx-1.1.dist-info/LICENSE` & `wfsx-1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wfsx-1.1.dist-info/METADATA` & `wfsx-1.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfsx
-Version: 1.1
+Version: 1.2
 Summary: api automation testing framework based on unittest.
 Home-page: https://github.com/saasaa831/wfsx/
 Author: saasaa
 Author-email: saasaa@saa.com
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
@@ -23,13 +23,14 @@
 Requires-Dist: openpyxl
 Requires-Dist: urllib3
 Requires-Dist: ijson
 Requires-Dist: pandas
 Requires-Dist: SQLAlchemy
 Requires-Dist: configparser
 Requires-Dist: numpy
+Requires-Dist: selenium
 Requires-Dist: cdxg (==1.1)
 Requires-Dist: CXRunner (==1.0.6)
 
 # Accelerate API Generic functions
 Automation Framework desgined to test api's.
 * API functionality to be tested
```

## Comparing `wfsx-1.1.dist-info/RECORD` & `wfsx-1.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 wfsx/Excel_x.py,sha256=-RhqrKWTi2ias2f8sMpembEYSectGn6zvhlDEaGIkIc,5163
 wfsx/Report.py,sha256=kbydYbBv0YmoOdgCQ2y92nuBNUZmYcwq4gbajGUbKMc,5280
 wfsx/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wfsx/api.py,sha256=4RvVwxzel6i3jpIWOw8pzM_LOCc9P9lqk8QKrvOJGXM,6310
 wfsx/apivalid.py,sha256=OZz8aFjH9BSmrvJNY7XwV1yjUYHpd7Fa6pyO-X0z0G8,6019
 wfsx/apivalidation.py,sha256=Hl6G6bv66BVnlN6iZjxATfe19LyB7yfvSHQQZ_Ue0Sg,16574
 wfsx/common.py,sha256=JMA43pYw9PAaAotrKs9wTiPUdqbKeti_MqEmVqCpqmo,20705
-wfsx/dataextract.py,sha256=OtbdeKfQXC4BT1ye7Kxp0zfjnZgitkU2kYF3X-xqbso,9505
+wfsx/dataextract.py,sha256=C5lm_ZV1QmkfKK9VbzFwKSaGo44SduJl7DfA9ZJWjzI,12039
 wfsx/excel_json_reader.py,sha256=z4vQkNRLKCO7x3UAeI8EVd9vjY5GDTEYDOVTj2jqICA,2808
 wfsx/ghelper.py,sha256=oYgGDv8YZOKAX6vg4gel0kjpaAwZ40137AQhAFDFnW8,4189
 wfsx/parseexcel.py,sha256=uXXUcI9AiDHqdaKd8oGAxu_3OXFmuw66CLRXvJRXHtc,5407
 wfsx/plite.py,sha256=d2yNK_XkO17OFQbr4Ecf_OSkDgys9vzdefnm03Lm3Ck,7022
 wfsx/results_validate.py,sha256=Jzx6xUHcbrTQuKhc9q48vKR7BXmSrEbD8T7SB45c_NM,23242
-wfsx-1.1.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
-wfsx-1.1.dist-info/METADATA,sha256=l921sY1rrSiQoqk98_ImDXm9loVnx9WQ1F7lAFyNzlo,1235
-wfsx-1.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-wfsx-1.1.dist-info/top_level.txt,sha256=ylpSMw0AVSmfULYBvc6iiXmLKtra7xinB3IPH0sBALs,5
-wfsx-1.1.dist-info/RECORD,,
+wfsx-1.2.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
+wfsx-1.2.dist-info/METADATA,sha256=54tNXs8gqsTeG1HnDEdzMa-4u98PkA9tSK_li8Mki0U,1260
+wfsx-1.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+wfsx-1.2.dist-info/top_level.txt,sha256=ylpSMw0AVSmfULYBvc6iiXmLKtra7xinB3IPH0sBALs,5
+wfsx-1.2.dist-info/RECORD,,
```

