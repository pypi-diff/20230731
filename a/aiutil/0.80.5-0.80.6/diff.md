# Comparing `tmp/aiutil-0.80.5.tar.gz` & `tmp/aiutil-0.80.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiutil-0.80.5.tar", max compression
+gzip compressed data, was "aiutil-0.80.6.tar", max compression
```

## Comparing `aiutil-0.80.5.tar` & `aiutil-0.80.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1081 2023-07-24 02:00:36.847561 aiutil-0.80.5/LICENSE
--rw-r--r--   0        0        0     1861 2023-07-24 02:00:36.847561 aiutil-0.80.5/README.md
--rw-r--r--   0        0        0       96 2023-07-24 02:00:36.847561 aiutil-0.80.5/aiutil/__init__.py
--rw-r--r--   0        0        0     1968 2023-07-24 02:00:36.847561 aiutil-0.80.5/aiutil/collections.py
--rw-r--r--   0        0        0    10716 2023-07-24 02:00:36.847561 aiutil-0.80.5/aiutil/cv.py
--rw-r--r--   0        0        0     3246 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/dataframe.py
--rw-r--r--   0        0        0     3501 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/datetime.py
--rw-r--r--   0        0        0     2092 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/dockerhub.py
--rw-r--r--   0        0        0    23197 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/filesystem.py
--rw-r--r--   0        0        0       81 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hadoop/__init__.py
--rw-r--r--   0        0        0     9194 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hadoop/hdfs.py
--rw-r--r--   0        0        0     5910 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hadoop/kerberos.py
--rw-r--r--   0        0        0    18754 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hadoop/log.py
--rw-r--r--   0        0        0     7473 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hadoop/logf.py
--rw-r--r--   0        0        0    16000 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hadoop/pyspark_submit.py
--rw-r--r--   0        0        0     1245 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hadoop/pyspark_submit.yaml
--rw-r--r--   0        0        0     1450 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/hash.py
--rw-r--r--   0        0        0     3950 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/memory.py
--rw-r--r--   0        0        0        0 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/notebook/__init__.py
--rwxr-xr-x   0        0        0     9614 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/notebook/search.py
--rw-r--r--   0        0        0     2337 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/notebook/util.py
--rw-r--r--   0        0        0     1612 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/pdf.py
--rw-r--r--   0        0        0    10890 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/poetry.py
--rw-r--r--   0        0        0     1102 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/pypi.py
--rw-r--r--   0        0        0     2111 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/shebang.py
--rw-r--r--   0        0        0     4637 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/shell.py
--rw-r--r--   0        0        0      660 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/sql.py
--rw-r--r--   0        0        0      651 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/url.py
--rw-r--r--   0        0        0     1159 2023-07-24 02:00:36.851560 aiutil-0.80.5/aiutil/utils.py
--rw-r--r--   0        0        0     2541 2023-07-24 02:00:36.855561 aiutil-0.80.5/pyproject.toml
--rw-r--r--   0        0        0     3859 1970-01-01 00:00:00.000000 aiutil-0.80.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-31 01:06:40.628882 aiutil-0.80.6/LICENSE
+-rw-r--r--   0        0        0     1861 2023-07-31 01:06:40.628882 aiutil-0.80.6/README.md
+-rw-r--r--   0        0        0       96 2023-07-31 01:06:40.628882 aiutil-0.80.6/aiutil/__init__.py
+-rw-r--r--   0        0        0     1968 2023-07-31 01:06:40.628882 aiutil-0.80.6/aiutil/collections.py
+-rw-r--r--   0        0        0    10716 2023-07-31 01:06:40.628882 aiutil-0.80.6/aiutil/cv.py
+-rw-r--r--   0        0        0     3246 2023-07-31 01:06:40.628882 aiutil-0.80.6/aiutil/dataframe.py
+-rw-r--r--   0        0        0     3501 2023-07-31 01:06:40.628882 aiutil-0.80.6/aiutil/datetime.py
+-rw-r--r--   0        0        0     2092 2023-07-31 01:06:40.628882 aiutil-0.80.6/aiutil/dockerhub.py
+-rw-r--r--   0        0        0    23197 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/filesystem.py
+-rw-r--r--   0        0        0       81 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hadoop/__init__.py
+-rw-r--r--   0        0        0     9194 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hadoop/hdfs.py
+-rw-r--r--   0        0        0     5910 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hadoop/kerberos.py
+-rw-r--r--   0        0        0    18754 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hadoop/log.py
+-rw-r--r--   0        0        0     7473 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hadoop/logf.py
+-rw-r--r--   0        0        0    16000 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hadoop/pyspark_submit.py
+-rw-r--r--   0        0        0     1245 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hadoop/pyspark_submit.yaml
+-rw-r--r--   0        0        0     1450 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/hash.py
+-rw-r--r--   0        0        0     3950 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/memory.py
+-rw-r--r--   0        0        0        0 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/notebook/__init__.py
+-rwxr-xr-x   0        0        0     9614 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/notebook/search.py
+-rw-r--r--   0        0        0     2337 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/notebook/util.py
+-rw-r--r--   0        0        0     1612 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/pdf.py
+-rw-r--r--   0        0        0    10900 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/poetry.py
+-rw-r--r--   0        0        0     1102 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/pypi.py
+-rw-r--r--   0        0        0     2111 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/shebang.py
+-rw-r--r--   0        0        0     4637 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/shell.py
+-rw-r--r--   0        0        0      660 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/sql.py
+-rw-r--r--   0        0        0      651 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/url.py
+-rw-r--r--   0        0        0     1159 2023-07-31 01:06:40.632882 aiutil-0.80.6/aiutil/utils.py
+-rw-r--r--   0        0        0     2541 2023-07-31 01:06:40.632882 aiutil-0.80.6/pyproject.toml
+-rw-r--r--   0        0        0     3859 1970-01-01 00:00:00.000000 aiutil-0.80.6/PKG-INFO
```

### Comparing `aiutil-0.80.5/LICENSE` & `aiutil-0.80.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/README.md` & `aiutil-0.80.6/README.md`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/collections.py` & `aiutil-0.80.6/aiutil/collections.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/cv.py` & `aiutil-0.80.6/aiutil/cv.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/dataframe.py` & `aiutil-0.80.6/aiutil/dataframe.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/datetime.py` & `aiutil-0.80.6/aiutil/datetime.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/dockerhub.py` & `aiutil-0.80.6/aiutil/dockerhub.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/filesystem.py` & `aiutil-0.80.6/aiutil/filesystem.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/hadoop/hdfs.py` & `aiutil-0.80.6/aiutil/hadoop/hdfs.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/hadoop/kerberos.py` & `aiutil-0.80.6/aiutil/hadoop/kerberos.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/hadoop/log.py` & `aiutil-0.80.6/aiutil/hadoop/log.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/hadoop/logf.py` & `aiutil-0.80.6/aiutil/hadoop/logf.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/hadoop/pyspark_submit.py` & `aiutil-0.80.6/aiutil/hadoop/pyspark_submit.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/hadoop/pyspark_submit.yaml` & `aiutil-0.80.6/aiutil/hadoop/pyspark_submit.yaml`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/hash.py` & `aiutil-0.80.6/aiutil/hash.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/memory.py` & `aiutil-0.80.6/aiutil/memory.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/notebook/search.py` & `aiutil-0.80.6/aiutil/notebook/search.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/notebook/util.py` & `aiutil-0.80.6/aiutil/notebook/util.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/pdf.py` & `aiutil-0.80.6/aiutil/pdf.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/poetry.py` & `aiutil-0.80.6/aiutil/poetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,17 +133,18 @@
     The tag is decided based on the current version of the project.
 
     :param proj_dir: The root directory of the Poetry project.
     :param tag: The tag (defaults to the current version of the package) to use.
     :param branch_release: The branch for releasing.
     :raises ValueError: If the tag to create already exists.
     """
-    if proj_dir is None:
-        proj_dir = _project_dir()
-    tag = tag if tag else ("v" + _project_version(proj_dir))
+    if not tag:
+        if proj_dir is None:
+            proj_dir = _project_dir()
+        tag = "v" + _project_version(proj_dir)
     repo = dulwich.repo.Repo(proj_dir)
     if tag.encode() in dulwich.porcelain.tag_list(repo):
         raise ValueError(
             f"The tag {tag} already exists! Please merge new changes to the {branch_release} branch first."
         )
     branch_old = dulwich.porcelain.active_branch(repo=repo).decode()
     # add tag to the release branch
```

### Comparing `aiutil-0.80.5/aiutil/pypi.py` & `aiutil-0.80.6/aiutil/pypi.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/shebang.py` & `aiutil-0.80.6/aiutil/shebang.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/shell.py` & `aiutil-0.80.6/aiutil/shell.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/sql.py` & `aiutil-0.80.6/aiutil/sql.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/url.py` & `aiutil-0.80.6/aiutil/url.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/aiutil/utils.py` & `aiutil-0.80.6/aiutil/utils.py`

 * *Files identical despite different names*

### Comparing `aiutil-0.80.5/pyproject.toml` & `aiutil-0.80.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiutil"
-version = "0.80.5"
+version = "0.80.6"
 description = "A utils Python package for data scientists."
 authors = ["Benjamin Du <longendu@yahoo.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/legendu-net/aiutil"
 keywords = ["AI", "Machine Learning", "tools", "utils"]
```

### Comparing `aiutil-0.80.5/PKG-INFO` & `aiutil-0.80.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiutil
-Version: 0.80.5
+Version: 0.80.6
 Summary: A utils Python package for data scientists.
 Home-page: https://github.com/legendu-net/aiutil
 License: MIT
 Keywords: AI,Machine Learning,tools,utils
 Author: Benjamin Du
 Author-email: longendu@yahoo.com
 Requires-Python: >=3.10,<3.12
```

