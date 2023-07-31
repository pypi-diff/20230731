# Comparing `tmp/lmpylib-mingsqtt-1.0.7.tar.gz` & `tmp/lmpylib-mingsqtt-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lmpylib-mingsqtt-1.0.7.tar", last modified: Wed Jul 19 03:37:22 2023, max compression
+gzip compressed data, was "dist/lmpylib-mingsqtt-1.0.8.tar", last modified: Mon Jul 31 03:19:09 2023, max compression
```

## Comparing `lmpylib-mingsqtt-1.0.7.tar` & `lmpylib-mingsqtt-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-07-19 03:37:22.000000 lmpylib-mingsqtt-1.0.7/
--rw-r--r--   0 liming     (501) staff       (20)      465 2023-07-19 03:37:22.000000 lmpylib-mingsqtt-1.0.7/PKG-INFO
--rw-r--r--   0 liming     (501) staff       (20)      167 2020-06-06 15:27:26.000000 lmpylib-mingsqtt-1.0.7/README.md
-drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-07-19 03:37:22.000000 lmpylib-mingsqtt-1.0.7/lmpylib/
--rw-r--r--   0 liming     (501) staff       (20)        0 2020-06-06 15:27:26.000000 lmpylib-mingsqtt-1.0.7/lmpylib/__init__.py
--rw-r--r--   0 liming     (501) staff       (20)     3750 2022-10-14 01:58:49.000000 lmpylib-mingsqtt-1.0.7/lmpylib/byteutil.py
--rw-r--r--   0 liming     (501) staff       (20)   147785 2023-07-19 03:37:17.000000 lmpylib-mingsqtt-1.0.7/lmpylib/core.py
--rw-r--r--   0 liming     (501) staff       (20)    15240 2020-06-06 15:27:26.000000 lmpylib-mingsqtt-1.0.7/lmpylib/cv.py
--rw-r--r--   0 liming     (501) staff       (20)    27267 2023-03-13 06:19:52.000000 lmpylib-mingsqtt-1.0.7/lmpylib/geo.py
--rw-r--r--   0 liming     (501) staff       (20)    52996 2021-01-12 09:44:49.000000 lmpylib-mingsqtt-1.0.7/lmpylib/nlp.py
--rw-r--r--   0 liming     (501) staff       (20)     5726 2020-06-14 13:47:01.000000 lmpylib-mingsqtt-1.0.7/lmpylib/sigproc.py
--rw-r--r--   0 liming     (501) staff       (20)       22 2023-07-19 03:37:17.000000 lmpylib-mingsqtt-1.0.7/lmpylib/version.py
-drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-07-19 03:37:22.000000 lmpylib-mingsqtt-1.0.7/lmpylib_mingsqtt.egg-info/
--rw-r--r--   0 liming     (501) staff       (20)      465 2023-07-19 03:37:21.000000 lmpylib-mingsqtt-1.0.7/lmpylib_mingsqtt.egg-info/PKG-INFO
--rw-r--r--   0 liming     (501) staff       (20)      316 2023-07-19 03:37:21.000000 lmpylib-mingsqtt-1.0.7/lmpylib_mingsqtt.egg-info/SOURCES.txt
--rw-r--r--   0 liming     (501) staff       (20)        1 2023-07-19 03:37:21.000000 lmpylib-mingsqtt-1.0.7/lmpylib_mingsqtt.egg-info/dependency_links.txt
--rw-r--r--   0 liming     (501) staff       (20)        8 2023-07-19 03:37:21.000000 lmpylib-mingsqtt-1.0.7/lmpylib_mingsqtt.egg-info/top_level.txt
--rw-r--r--   0 liming     (501) staff       (20)       38 2023-07-19 03:37:22.000000 lmpylib-mingsqtt-1.0.7/setup.cfg
--rw-r--r--   0 liming     (501) staff       (20)      820 2020-06-06 17:20:38.000000 lmpylib-mingsqtt-1.0.7/setup.py
+drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-07-31 03:19:09.000000 lmpylib-mingsqtt-1.0.8/
+-rw-r--r--   0 liming     (501) staff       (20)      465 2023-07-31 03:19:09.000000 lmpylib-mingsqtt-1.0.8/PKG-INFO
+-rw-r--r--   0 liming     (501) staff       (20)      167 2020-06-06 15:27:26.000000 lmpylib-mingsqtt-1.0.8/README.md
+drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-07-31 03:19:09.000000 lmpylib-mingsqtt-1.0.8/lmpylib/
+-rw-r--r--   0 liming     (501) staff       (20)        0 2020-06-06 15:27:26.000000 lmpylib-mingsqtt-1.0.8/lmpylib/__init__.py
+-rw-r--r--   0 liming     (501) staff       (20)     3750 2022-10-14 01:58:49.000000 lmpylib-mingsqtt-1.0.8/lmpylib/byteutil.py
+-rw-r--r--   0 liming     (501) staff       (20)   147791 2023-07-31 03:19:07.000000 lmpylib-mingsqtt-1.0.8/lmpylib/core.py
+-rw-r--r--   0 liming     (501) staff       (20)    15240 2020-06-06 15:27:26.000000 lmpylib-mingsqtt-1.0.8/lmpylib/cv.py
+-rw-r--r--   0 liming     (501) staff       (20)    27267 2023-03-13 06:19:52.000000 lmpylib-mingsqtt-1.0.8/lmpylib/geo.py
+-rw-r--r--   0 liming     (501) staff       (20)    52996 2021-01-12 09:44:49.000000 lmpylib-mingsqtt-1.0.8/lmpylib/nlp.py
+-rw-r--r--   0 liming     (501) staff       (20)     5726 2020-06-14 13:47:01.000000 lmpylib-mingsqtt-1.0.8/lmpylib/sigproc.py
+-rw-r--r--   0 liming     (501) staff       (20)       22 2023-07-31 03:19:07.000000 lmpylib-mingsqtt-1.0.8/lmpylib/version.py
+drwxr-xr-x   0 liming     (501) staff       (20)        0 2023-07-31 03:19:09.000000 lmpylib-mingsqtt-1.0.8/lmpylib_mingsqtt.egg-info/
+-rw-r--r--   0 liming     (501) staff       (20)      465 2023-07-31 03:19:09.000000 lmpylib-mingsqtt-1.0.8/lmpylib_mingsqtt.egg-info/PKG-INFO
+-rw-r--r--   0 liming     (501) staff       (20)      316 2023-07-31 03:19:09.000000 lmpylib-mingsqtt-1.0.8/lmpylib_mingsqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 liming     (501) staff       (20)        1 2023-07-31 03:19:09.000000 lmpylib-mingsqtt-1.0.8/lmpylib_mingsqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 liming     (501) staff       (20)        8 2023-07-31 03:19:09.000000 lmpylib-mingsqtt-1.0.8/lmpylib_mingsqtt.egg-info/top_level.txt
+-rw-r--r--   0 liming     (501) staff       (20)       38 2023-07-31 03:19:09.000000 lmpylib-mingsqtt-1.0.8/setup.cfg
+-rw-r--r--   0 liming     (501) staff       (20)      820 2020-06-06 17:20:38.000000 lmpylib-mingsqtt-1.0.8/setup.py
```

### Comparing `lmpylib-mingsqtt-1.0.7/lmpylib/byteutil.py` & `lmpylib-mingsqtt-1.0.8/lmpylib/byteutil.py`

 * *Files identical despite different names*

### Comparing `lmpylib-mingsqtt-1.0.7/lmpylib/core.py` & `lmpylib-mingsqtt-1.0.8/lmpylib/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     group = pd.DataFrame({"Value": data, "Count": [1] * len(data)}).groupby(by="Value", sort=False).count()
     if sort_by == "count":
         group = group.sort_values(by="Count", ascending=ascending)
     elif (sort_by == "label") or (sort_by == "index") or (sort_by == "text"):
         group = group.sort_index(ascending=ascending)
     group.index = group.index.astype("str")
     if (not include_na_only_if_exist) or (na_count > 0):
-        group = group.append(pd.DataFrame({"Count": np.array([na_count], dtype=int)}, index=["NA"]), ignore_index=False)
+        group = pd.concat([group, pd.DataFrame({"Count": np.array([na_count], dtype=int)}, index=["NA"])], ignore_index=False)
     return group
 
 
 def _summarize_numeric(data, as_rows=False, outlier_iqr_multiplier=None, outlier_std_multiplier=None):
     without_na = np.array([val for val in data if (val is not None) and (not pd.isna(val))])
 
     if len(without_na) == 0:
```

### Comparing `lmpylib-mingsqtt-1.0.7/lmpylib/cv.py` & `lmpylib-mingsqtt-1.0.8/lmpylib/cv.py`

 * *Files identical despite different names*

### Comparing `lmpylib-mingsqtt-1.0.7/lmpylib/geo.py` & `lmpylib-mingsqtt-1.0.8/lmpylib/geo.py`

 * *Files identical despite different names*

### Comparing `lmpylib-mingsqtt-1.0.7/lmpylib/nlp.py` & `lmpylib-mingsqtt-1.0.8/lmpylib/nlp.py`

 * *Files identical despite different names*

### Comparing `lmpylib-mingsqtt-1.0.7/lmpylib/sigproc.py` & `lmpylib-mingsqtt-1.0.8/lmpylib/sigproc.py`

 * *Files identical despite different names*

### Comparing `lmpylib-mingsqtt-1.0.7/setup.py` & `lmpylib-mingsqtt-1.0.8/setup.py`

 * *Files identical despite different names*

