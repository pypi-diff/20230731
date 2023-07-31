# Comparing `tmp/avlwrapper-0.3.4.tar.gz` & `tmp/avlwrapper-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avlwrapper-0.3.4.tar", last modified: Sat Jan 14 14:09:24 2023, max compression
+gzip compressed data, was "avlwrapper-0.3.5.tar", last modified: Mon Jul 31 10:15:29 2023, max compression
```

## Comparing `avlwrapper-0.3.4.tar` & `avlwrapper-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 reno       (501) staff       (20)        0 2023-01-14 14:09:24.387867 avlwrapper-0.3.4/
--rw-r--r--   0 reno       (501) staff       (20)    35147 2022-12-18 17:26:56.000000 avlwrapper-0.3.4/LICENSE
--rw-r--r--   0 reno       (501) staff       (20)     2603 2023-01-14 14:09:24.387716 avlwrapper-0.3.4/PKG-INFO
--rw-r--r--   0 reno       (501) staff       (20)     1936 2022-12-18 17:26:56.000000 avlwrapper-0.3.4/README.md
-drwxr-xr-x   0 reno       (501) staff       (20)        0 2023-01-14 14:09:24.386804 avlwrapper-0.3.4/avlwrapper/
--rw-r--r--   0 reno       (501) staff       (20)      499 2023-01-14 14:08:45.000000 avlwrapper-0.3.4/avlwrapper/__init__.py
--rw-r--r--   0 reno       (501) staff       (20)      288 2023-01-14 14:08:45.000000 avlwrapper-0.3.4/avlwrapper/config.cfg
--rw-r--r--   0 reno       (501) staff       (20)     3974 2023-01-03 17:23:07.000000 avlwrapper-0.3.4/avlwrapper/config.py
--rw-r--r--   0 reno       (501) staff       (20)    38049 2023-01-14 14:08:45.000000 avlwrapper-0.3.4/avlwrapper/model.py
--rw-r--r--   0 reno       (501) staff       (20)    12415 2023-01-14 14:08:45.000000 avlwrapper-0.3.4/avlwrapper/output.py
--rw-r--r--   0 reno       (501) staff       (20)    11726 2023-01-14 14:08:45.000000 avlwrapper-0.3.4/avlwrapper/session.py
--rw-r--r--   0 reno       (501) staff       (20)     1797 2023-01-03 17:23:07.000000 avlwrapper-0.3.4/avlwrapper/tools.py
-drwxr-xr-x   0 reno       (501) staff       (20)        0 2023-01-14 14:09:24.387413 avlwrapper-0.3.4/avlwrapper.egg-info/
--rw-r--r--   0 reno       (501) staff       (20)     2603 2023-01-14 14:09:24.000000 avlwrapper-0.3.4/avlwrapper.egg-info/PKG-INFO
--rw-r--r--   0 reno       (501) staff       (20)      311 2023-01-14 14:09:24.000000 avlwrapper-0.3.4/avlwrapper.egg-info/SOURCES.txt
--rw-r--r--   0 reno       (501) staff       (20)        1 2023-01-14 14:09:24.000000 avlwrapper-0.3.4/avlwrapper.egg-info/dependency_links.txt
--rw-r--r--   0 reno       (501) staff       (20)       11 2023-01-14 14:09:24.000000 avlwrapper-0.3.4/avlwrapper.egg-info/top_level.txt
--rw-r--r--   0 reno       (501) staff       (20)       38 2023-01-14 14:09:24.387914 avlwrapper-0.3.4/setup.cfg
--rw-r--r--   0 reno       (501) staff       (20)     1303 2022-12-18 17:26:56.000000 avlwrapper-0.3.4/setup.py
+drwxr-xr-x   0 reno       (501) staff       (20)        0 2023-07-31 10:15:29.454275 avlwrapper-0.3.5/
+-rw-r--r--   0 reno       (501) staff       (20)    35147 2022-12-18 17:26:56.000000 avlwrapper-0.3.5/LICENSE
+-rw-r--r--   0 reno       (501) staff       (20)     2603 2023-07-31 10:15:29.454171 avlwrapper-0.3.5/PKG-INFO
+-rw-r--r--   0 reno       (501) staff       (20)     1936 2022-12-18 17:26:56.000000 avlwrapper-0.3.5/README.md
+drwxr-xr-x   0 reno       (501) staff       (20)        0 2023-07-31 10:15:29.453480 avlwrapper-0.3.5/avlwrapper/
+-rw-r--r--   0 reno       (501) staff       (20)      499 2023-07-31 10:15:11.000000 avlwrapper-0.3.5/avlwrapper/__init__.py
+-rw-r--r--   0 reno       (501) staff       (20)      288 2023-01-14 14:08:45.000000 avlwrapper-0.3.5/avlwrapper/config.cfg
+-rw-r--r--   0 reno       (501) staff       (20)     3974 2023-01-03 17:23:07.000000 avlwrapper-0.3.5/avlwrapper/config.py
+-rw-r--r--   0 reno       (501) staff       (20)    38054 2023-07-31 10:15:11.000000 avlwrapper-0.3.5/avlwrapper/model.py
+-rw-r--r--   0 reno       (501) staff       (20)    12415 2023-01-14 14:08:45.000000 avlwrapper-0.3.5/avlwrapper/output.py
+-rw-r--r--   0 reno       (501) staff       (20)    11726 2023-01-14 14:08:45.000000 avlwrapper-0.3.5/avlwrapper/session.py
+-rw-r--r--   0 reno       (501) staff       (20)     1797 2023-01-03 17:23:07.000000 avlwrapper-0.3.5/avlwrapper/tools.py
+drwxr-xr-x   0 reno       (501) staff       (20)        0 2023-07-31 10:15:29.454029 avlwrapper-0.3.5/avlwrapper.egg-info/
+-rw-r--r--   0 reno       (501) staff       (20)     2603 2023-07-31 10:15:29.000000 avlwrapper-0.3.5/avlwrapper.egg-info/PKG-INFO
+-rw-r--r--   0 reno       (501) staff       (20)      311 2023-07-31 10:15:29.000000 avlwrapper-0.3.5/avlwrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 reno       (501) staff       (20)        1 2023-07-31 10:15:29.000000 avlwrapper-0.3.5/avlwrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 reno       (501) staff       (20)       11 2023-07-31 10:15:29.000000 avlwrapper-0.3.5/avlwrapper.egg-info/top_level.txt
+-rw-r--r--   0 reno       (501) staff       (20)       38 2023-07-31 10:15:29.454306 avlwrapper-0.3.5/setup.cfg
+-rw-r--r--   0 reno       (501) staff       (20)     1303 2022-12-18 17:26:56.000000 avlwrapper-0.3.5/setup.py
```

### Comparing `avlwrapper-0.3.4/LICENSE` & `avlwrapper-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `avlwrapper-0.3.4/PKG-INFO` & `avlwrapper-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avlwrapper
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python interface for MIT AVL (Athena Vortex Lattice)
 Home-page: https://github.com/renoelmendorp/AVLWrapper
 Author: Reno Elmendorp
 License: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
```

### Comparing `avlwrapper-0.3.4/README.md` & `avlwrapper-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `avlwrapper-0.3.4/avlwrapper/config.py` & `avlwrapper-0.3.5/avlwrapper/config.py`

 * *Files identical despite different names*

### Comparing `avlwrapper-0.3.4/avlwrapper/model.py` & `avlwrapper-0.3.5/avlwrapper/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,15 +452,15 @@
     @classmethod
     def _from_lines(cls, lines_in):
         if len(lines_in) != 2:
             raise InputError(lines_in)
         params = [float(s) for s in lines_in[1].split()]
         if len(params) != 6:
             raise InputError(lines_in)
-        return cls(cl=params[:3], cd=params[3:])
+        return cls(cl=params[::2], cd=params[1::2])
 
 
 @dataclass
 class Section(ModelInput):
     """
     Wing surface section to be used in a Surface object.
 
@@ -1194,26 +1194,26 @@
         "YDUPLICATE": PT(None, "y_duplicate", AttrType.float),
         "SCALE": PT(None, "scaling", AttrType.vector),
         "TRANSLATE": PT(None, "translation", AttrType.vector),
         "ANGLE": PT(None, "angle", AttrType.float),
         "NOWAKE": PT(None, "no_wake", AttrType.boolean),
         "NOALBE": PT(None, "fixed", AttrType.boolean),
         "NOLOAD": PT(None, "no_loads", AttrType.boolean),
-        "CDCL": PT(ProfileDrag, "profile_drag", AttrType.float),
+        "CDCL": PT(ProfileDrag, "profile_drag", AttrType.single),
         "SECTION": PT(Section, "sections", AttrType.list),
     },
     Body: {
         "YDUPLICATE": PT(None, "y_duplicate", AttrType.float),
         "SCALE": PT(None, "scaling", AttrType.vector),
         "TRANSLATE": PT(None, "translation", AttrType.vector),
         "BFILE": PT(BodyProfile, "body_section", AttrType.single),
     },
     Section: {
         "NACA": PT(NacaAirfoil, "airfoil", AttrType.single),
         "AIRFOIL": PT(DataAirfoil, "airfoil", AttrType.single),
         "CLAF": PT(None, "cl_alpha_scaling", AttrType.float),
-        "CDCL": PT(ProfileDrag, "profile_drag", AttrType.float),
+        "CDCL": PT(ProfileDrag, "profile_drag", AttrType.single),
         "AFILE": PT(FileAirfoil, "airfoil", AttrType.single),
         "CONTROL": PT(Control, "controls", AttrType.list),
         "DESIGN": PT(DesignVar, "design_vars", AttrType.list),
     },
 }
```

### Comparing `avlwrapper-0.3.4/avlwrapper/output.py` & `avlwrapper-0.3.5/avlwrapper/output.py`

 * *Files identical despite different names*

### Comparing `avlwrapper-0.3.4/avlwrapper/session.py` & `avlwrapper-0.3.5/avlwrapper/session.py`

 * *Files identical despite different names*

### Comparing `avlwrapper-0.3.4/avlwrapper/tools.py` & `avlwrapper-0.3.5/avlwrapper/tools.py`

 * *Files identical despite different names*

### Comparing `avlwrapper-0.3.4/avlwrapper.egg-info/PKG-INFO` & `avlwrapper-0.3.5/avlwrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avlwrapper
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python interface for MIT AVL (Athena Vortex Lattice)
 Home-page: https://github.com/renoelmendorp/AVLWrapper
 Author: Reno Elmendorp
 License: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
```

### Comparing `avlwrapper-0.3.4/setup.py` & `avlwrapper-0.3.5/setup.py`

 * *Files identical despite different names*

