# Comparing `tmp/finesse-ligo-1.0.8.tar.gz` & `tmp/finesse-ligo-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finesse-ligo-1.0.8.tar", last modified: Fri Mar 25 07:39:12 2022, max compression
+gzip compressed data, was "finesse-ligo-1.0.9.tar", last modified: Sun Mar 27 04:22:25 2022, max compression
```

## Comparing `finesse-ligo-1.0.8.tar` & `finesse-ligo-1.0.9.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 07:39:12.274787 finesse-ligo-1.0.8/
--rw-rw-rw-   0 root         (0) root         (0)     2761 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1360 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1943 2022-03-25 07:39:12.274787 finesse-ligo-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1225 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      143 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      938 2022-03-25 07:39:12.274787 finesse-ligo-1.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 07:39:12.270787 finesse-ligo-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 07:39:12.270787 finesse-ligo-1.0.8/src/finesse_ligo/
--rw-rw-rw-   0 root         (0) root         (0)       29 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/src/finesse_ligo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 07:39:12.270787 finesse-ligo-1.0.8/src/finesse_ligo/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/src/finesse_ligo/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 07:39:12.274787 finesse-ligo-1.0.8/src/finesse_ligo/data/suspensions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/src/finesse_ligo/data/suspensions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5222 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/src/finesse_ligo/data/suspensions/ligo_triple_suspension_ss.pbz2
--rw-rw-rw-   0 root         (0) root         (0)     6061 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/src/finesse_ligo/data/suspensions/quad_damped_ss.pbz2
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 07:39:12.274787 finesse-ligo-1.0.8/src/finesse_ligo/data/thermal/
--rw-rw-rw-   0 root         (0) root         (0)   163533 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/src/finesse_ligo/data/thermal/T2100329-v1-ringheater_FEA.npz
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/src/finesse_ligo/data/thermal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 07:39:12.274787 finesse-ligo-1.0.8/src/finesse_ligo/katscript/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/src/finesse_ligo/katscript/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6621 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/src/finesse_ligo/katscript/aligo.kat
--rw-rw-rw-   0 root         (0) root         (0)    15592 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/src/finesse_ligo/suspension.py
--rw-rw-rw-   0 root         (0) root         (0)    10263 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/src/finesse_ligo/thermal.py
--rw-rw-rw-   0 root         (0) root         (0)     8200 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/src/finesse_ligo/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 07:39:12.270787 finesse-ligo-1.0.8/src/finesse_ligo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1943 2022-03-25 07:39:11.000000 finesse-ligo-1.0.8/src/finesse_ligo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      770 2022-03-25 07:39:12.000000 finesse-ligo-1.0.8/src/finesse_ligo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-25 07:39:11.000000 finesse-ligo-1.0.8/src/finesse_ligo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2022-03-25 07:39:12.000000 finesse-ligo-1.0.8/src/finesse_ligo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-03-25 07:39:12.000000 finesse-ligo-1.0.8/src/finesse_ligo.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-25 07:39:12.274787 finesse-ligo-1.0.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2082 2022-03-25 07:38:54.000000 finesse-ligo-1.0.8/tests/test_ligo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-27 04:22:25.389721 finesse-ligo-1.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     2772 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1761 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      734 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     3893 2022-03-27 04:22:25.389721 finesse-ligo-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3175 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      321 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2022-03-27 04:22:25.389721 finesse-ligo-1.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-27 04:22:25.389721 finesse-ligo-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-27 04:22:25.389721 finesse-ligo-1.0.9/src/finesse_ligo/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/src/finesse_ligo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-27 04:22:25.389721 finesse-ligo-1.0.9/src/finesse_ligo/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/src/finesse_ligo/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-27 04:22:25.389721 finesse-ligo-1.0.9/src/finesse_ligo/data/suspensions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/src/finesse_ligo/data/suspensions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5222 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/src/finesse_ligo/data/suspensions/ligo_triple_suspension_ss.pbz2
+-rw-rw-rw-   0 root         (0) root         (0)     6061 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/src/finesse_ligo/data/suspensions/quad_damped_ss.pbz2
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-27 04:22:25.389721 finesse-ligo-1.0.9/src/finesse_ligo/data/thermal/
+-rw-rw-rw-   0 root         (0) root         (0)   163533 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/src/finesse_ligo/data/thermal/T2100329-v1-ringheater_FEA.npz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/src/finesse_ligo/data/thermal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-27 04:22:25.389721 finesse-ligo-1.0.9/src/finesse_ligo/katscript/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/src/finesse_ligo/katscript/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6622 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/src/finesse_ligo/katscript/aligo.kat
+-rw-rw-rw-   0 root         (0) root         (0)    15637 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/src/finesse_ligo/suspension.py
+-rw-rw-rw-   0 root         (0) root         (0)    10259 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/src/finesse_ligo/thermal.py
+-rw-rw-rw-   0 root         (0) root         (0)    10517 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/src/finesse_ligo/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-27 04:22:25.389721 finesse-ligo-1.0.9/src/finesse_ligo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3893 2022-03-27 04:22:24.000000 finesse-ligo-1.0.9/src/finesse_ligo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      794 2022-03-27 04:22:25.000000 finesse-ligo-1.0.9/src/finesse_ligo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-27 04:22:24.000000 finesse-ligo-1.0.9/src/finesse_ligo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2022-03-27 04:22:25.000000 finesse-ligo-1.0.9/src/finesse_ligo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-03-27 04:22:25.000000 finesse-ligo-1.0.9/src/finesse_ligo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-27 04:22:25.389721 finesse-ligo-1.0.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2022-03-27 04:22:08.000000 finesse-ligo-1.0.9/tests/test_ligo.py
```

### Comparing `finesse-ligo-1.0.8/.gitignore` & `finesse-ligo-1.0.9/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.DS_Store
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
@@ -145,8 +146,8 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+#.idea/
```

### Comparing `finesse-ligo-1.0.8/.gitlab-ci.yml` & `finesse-ligo-1.0.9/.gitlab-ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,34 @@
 stages:
+    - pre-commit-hooks
     - test
     - publish
-            
+
+pre-merge-checks:
+  stage: pre-commit-hooks
+  image: python
+  variables:
+    PRE_COMMIT_HOME: ${CI_PROJECT_DIR}/.cache/pre-commit
+  cache:
+    paths:
+      - ${PRE_COMMIT_HOME}
+      - .venv
+    key: "$CI_JOB_NAME"
+  script:
+    - |
+      if [ ! -e .venv ] ; then
+        python -m venv .venv
+      fi
+    - . .venv/bin/activate
+    - pip3 install pre-commit -U
+    - pre-commit run --all-files
+
 test/finesse-develop:
     stage: test
-    image: python:3.10
+    image: python
     rules:
         - if: '$CI_PIPELINE_SOURCE == "push"'
           when: always
         - when: never
     script:
         - python -V
         - ls wheelhouse
@@ -17,15 +37,15 @@
         - echo $CI_COMMIT_REF_NAME
         - echo $CI_COMMIT_TAG
         - echo $CI_PROJECT_PATH
         - python -m pip install wheelhouse/*manylinux*.whl
         - python -m pip install pytest
         - python -m pip install .
         - pytest tests
-    needs: 
+    needs:
         - project: finesse/finesse3
           job: build/manylinux/x86_64/py310
           ref: develop
           artifacts: true
 
 publish:
     rules:
```

### Comparing `finesse-ligo-1.0.8/setup.cfg` & `finesse-ligo-1.0.9/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -24,19 +24,31 @@
 python_requires = >=3.8
 install_requires = 
 	finesse
 	numpy
 	scipy
 	matplotlib
 	control
+	tqdm
 include_package_data = True
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = data/**/*, katscript/*
 
+[flake8]
+ignore = 
+	E203 # Whitespace before ':'
+	E266 # Too many leading '#' for block comment
+	E402 # Module level import not at top of file
+	E501 # Line too long
+	E731 # Do not assign a lambda expression, use a def
+	E741 # ambiguous variable name
+	E231 # missing whitespace after ','
+	W503 # line break before binary operator (soon deprecated; see https://www.flake8rules.com/rules/W503.html)
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `finesse-ligo-1.0.8/src/finesse_ligo/data/suspensions/ligo_triple_suspension_ss.pbz2` & `finesse-ligo-1.0.9/src/finesse_ligo/data/suspensions/ligo_triple_suspension_ss.pbz2`

 * *Files identical despite different names*

### Comparing `finesse-ligo-1.0.8/src/finesse_ligo/data/suspensions/quad_damped_ss.pbz2` & `finesse-ligo-1.0.9/src/finesse_ligo/data/suspensions/quad_damped_ss.pbz2`

 * *Files identical despite different names*

### Comparing `finesse-ligo-1.0.8/src/finesse_ligo/data/thermal/T2100329-v1-ringheater_FEA.npz` & `finesse-ligo-1.0.9/src/finesse_ligo/data/thermal/T2100329-v1-ringheater_FEA.npz`

 * *Files identical despite different names*

### Comparing `finesse-ligo-1.0.8/src/finesse_ligo/katscript/aligo.kat` & `finesse-ligo-1.0.9/src/finesse_ligo/katscript/aligo.kat`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -164,8 +164,8 @@
 ### DC power measurements
 ###############################################################################
 pd Px ETMX.p1.i
 pd Py ETMX.p1.i
 pd Pprc PRM.p2.o
 pd Psrc SRM.p1.i
 pd Prefl ETMX.p1.i
-pd Pas OMC_OC.p3.o
+pd Pas OMC_OC.p3.o
```

### Comparing `finesse-ligo-1.0.8/src/finesse_ligo/suspension.py` & `finesse-ligo-1.0.9/src/finesse_ligo/suspension.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,17 @@
             import bz2
             import control
             import pickle
             from .data import suspensions
 
             # Load some data in and process it
             ss = pickle.loads(
-                bz2.decompress(pkg_resources.read_binary(data, "quad_damped_ss.pbz2"))
+                bz2.decompress(
+                    pkg_resources.read_binary(suspensions, "quad_damped_ss.pbz2")
+                )
             )
             tfs = control.ss2tf(
                 ss["A"],
                 ss["B"],
                 ss["C"],
                 ss["D"],
             )
```

### Comparing `finesse-ligo-1.0.8/src/finesse_ligo/thermal.py` & `finesse-ligo-1.0.9/src/finesse_ligo/thermal.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     scale = -1 if mirror.ports[0] == HR_port else 1
     R_ap, h, x, y, r, X, Y, material, b, c, aperture = get_thermal_test_mass_params(
         N_samples
     )
 
     # Assumes static Rc parameters
     if include_Rc:
-        R_static = X ** 2 / 2 / float(mirror.Rcx) + Y ** 2 / 2 / float(mirror.Rcy)
+        R_static = X**2 / 2 / float(mirror.Rcx) + Y**2 / 2 / float(mirror.Rcy)
     else:
         R_static = np.zeros_like(X)
     if static_surface_offset is not None:
         static = static_surface_offset(X, Y)
         R_static += static
 
     aperture = circular_aperture(x, y, 0.163)
```

### Comparing `finesse-ligo-1.0.8/src/finesse_ligo.egg-info/SOURCES.txt` & `finesse-ligo-1.0.9/src/finesse_ligo.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 .gitlab-ci.yml
+.pre-commit-config.yaml
 README.md
 pyproject.toml
 setup.cfg
 src/finesse_ligo/__init__.py
 src/finesse_ligo/suspension.py
 src/finesse_ligo/thermal.py
 src/finesse_ligo/tools.py
```

### Comparing `finesse-ligo-1.0.8/tests/test_ligo.py` & `finesse-ligo-1.0.9/tests/test_ligo.py`

 * *Files identical despite different names*

