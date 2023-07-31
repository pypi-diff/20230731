# Comparing `tmp/koning-8.tar.gz` & `tmp/koning-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/koning-8.tar", last modified: Sun May 31 05:01:14 2015, max compression
+gzip compressed data, was "dist/koning-9.tar", last modified: Tue Jun  2 12:58:26 2015, max compression
```

## Comparing `koning-8.tar` & `koning-9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-05-31 05:01:14.000000 koning-8/
--rw-rw-r--   0 bart      (1000) bart      (1000)       74 2015-05-23 21:00:46.000000 koning-8/MANIFEST.in
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-05-31 05:01:14.000000 koning-8/koning.egg-info/
--rw-rw-r--   0 bart      (1000) bart      (1000)      588 2015-05-31 05:01:13.000000 koning-8/koning.egg-info/PKG-INFO
--rw-rw-r--   0 bart      (1000) bart      (1000)        7 2015-05-31 05:01:13.000000 koning-8/koning.egg-info/top_level.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        4 2015-05-31 05:01:13.000000 koning-8/koning.egg-info/requires.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      542 2015-05-31 05:01:13.000000 koning-8/koning.egg-info/SOURCES.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        1 2015-05-31 05:01:13.000000 koning-8/koning.egg-info/dependency_links.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        1 2015-05-24 04:54:59.000000 koning-8/koning.egg-info/zip-safe
--rw-rw-r--   0 bart      (1000) bart      (1000)      588 2015-05-31 05:01:14.000000 koning-8/PKG-INFO
--rw-rw-r--   0 bart      (1000) bart      (1000)      179 2015-05-31 04:53:31.000000 koning-8/README
--rw-rw-r--   0 bart      (1000) bart      (1000)     1051 2015-05-31 04:53:03.000000 koning-8/setup.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-05-31 05:01:14.000000 koning-8/bin/
--rwxrwxr-x   0 bart      (1000) bart      (1000)      918 2015-05-23 21:00:46.000000 koning-8/bin/koning
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-05-31 05:01:14.000000 koning-8/docs/
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-05-31 05:01:14.000000 koning-8/docs/jpg/
--rw-rw-r--   0 bart      (1000) bart      (1000)   521122 2015-05-23 21:00:46.000000 koning-8/docs/jpg/20150406_001.jpg
--rw-rw-r--   0 bart      (1000) bart      (1000)   549426 2015-05-23 21:00:46.000000 koning-8/docs/jpg/20140730_011.jpg
--rw-rw-r--   0 bart      (1000) bart      (1000)     1034 2015-05-31 04:56:48.000000 koning-8/docs/LICENSE.rst
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-05-31 05:01:14.000000 koning-8/docs/txt/
--rw-rw-r--   0 bart      (1000) bart      (1000)     1129 2015-05-23 21:00:46.000000 koning-8/docs/txt/europa.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      853 2015-05-23 21:00:46.000000 koning-8/docs/txt/crisis.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      974 2015-05-23 21:00:46.000000 koning-8/docs/txt/urls.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      616 2015-05-23 21:00:46.000000 koning-8/docs/txt/overeenkomst.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)     1487 2015-05-23 21:00:46.000000 koning-8/docs/txt/ambulant.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)     1966 2015-05-23 21:00:46.000000 koning-8/docs/txt/ccaf.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)     1301 2015-05-23 21:00:46.000000 koning-8/docs/txt/preventief.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      706 2015-05-29 01:32:12.000000 koning-8/docs/index.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      179 2015-05-31 04:56:48.000000 koning-8/docs/README.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)       59 2015-05-31 05:01:14.000000 koning-8/setup.cfg
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-05-31 05:01:14.000000 koning-8/koning/
--rw-rw-r--   0 bart      (1000) bart      (1000)      339 2015-05-30 17:04:21.000000 koning-8/koning/version.py
--rw-rw-r--   0 bart      (1000) bart      (1000)       65 2015-05-30 16:34:08.000000 koning-8/koning/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3215 2015-05-29 11:02:02.000000 koning-8/koning/campagne.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1273 2015-05-30 16:37:47.000000 koning-8/koning/license.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1034 2015-05-30 16:37:17.000000 koning-8/LICENSE
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-06-02 12:58:26.000000 koning-9/
+-rw-rw-r--   0 bart      (1000) bart      (1000)       74 2015-05-23 21:00:46.000000 koning-9/MANIFEST.in
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-06-02 12:58:26.000000 koning-9/koning.egg-info/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      560 2015-06-02 12:58:26.000000 koning-9/koning.egg-info/PKG-INFO
+-rw-rw-r--   0 bart      (1000) bart      (1000)        7 2015-06-02 12:58:26.000000 koning-9/koning.egg-info/top_level.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)        4 2015-06-02 12:58:26.000000 koning-9/koning.egg-info/requires.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      542 2015-06-02 12:58:26.000000 koning-9/koning.egg-info/SOURCES.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)        1 2015-06-02 12:58:26.000000 koning-9/koning.egg-info/dependency_links.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)        1 2015-05-24 04:54:59.000000 koning-9/koning.egg-info/zip-safe
+-rw-rw-r--   0 bart      (1000) bart      (1000)      560 2015-06-02 12:58:26.000000 koning-9/PKG-INFO
+-rw-rw-r--   0 bart      (1000) bart      (1000)      224 2015-06-02 12:56:38.000000 koning-9/README
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1023 2015-06-02 12:38:24.000000 koning-9/setup.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-06-02 12:58:26.000000 koning-9/bin/
+-rwxrwxr-x   0 bart      (1000) bart      (1000)      918 2015-05-23 21:00:46.000000 koning-9/bin/koning
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-06-02 12:58:26.000000 koning-9/docs/
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-06-02 12:58:26.000000 koning-9/docs/jpg/
+-rw-rw-r--   0 bart      (1000) bart      (1000)   521122 2015-05-23 21:00:46.000000 koning-9/docs/jpg/20150406_001.jpg
+-rw-rw-r--   0 bart      (1000) bart      (1000)   549426 2015-05-23 21:00:46.000000 koning-9/docs/jpg/20140730_011.jpg
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1034 2015-06-02 12:56:44.000000 koning-9/docs/LICENSE.rst
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-06-02 12:58:26.000000 koning-9/docs/txt/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1129 2015-05-23 21:00:46.000000 koning-9/docs/txt/europa.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      853 2015-05-23 21:00:46.000000 koning-9/docs/txt/crisis.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      974 2015-05-23 21:00:46.000000 koning-9/docs/txt/urls.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      616 2015-05-23 21:00:46.000000 koning-9/docs/txt/overeenkomst.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1487 2015-05-23 21:00:46.000000 koning-9/docs/txt/ambulant.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1966 2015-05-23 21:00:46.000000 koning-9/docs/txt/ccaf.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1301 2015-05-23 21:00:46.000000 koning-9/docs/txt/preventief.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      706 2015-05-29 01:32:12.000000 koning-9/docs/index.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      224 2015-06-02 12:56:44.000000 koning-9/docs/README.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)       59 2015-06-02 12:58:26.000000 koning-9/setup.cfg
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-06-02 12:58:26.000000 koning-9/koning/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      367 2015-06-02 12:41:08.000000 koning-9/koning/version.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)       65 2015-06-02 12:41:44.000000 koning-9/koning/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3203 2015-06-02 12:50:16.000000 koning-9/koning/campagne.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1301 2015-06-02 12:39:42.000000 koning-9/koning/license.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1034 2015-05-30 16:37:17.000000 koning-9/LICENSE
```

### Comparing `koning-8/koning.egg-info/SOURCES.txt` & `koning-9/koning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `koning-8/setup.py` & `koning-9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 
 try:
     from setuptools import setup
 except Exception as ex: print(str(ex)) ; os._exit(1)
 
 setup(
     name='koning',
-    version='8',
+    version='9',
     url='https://pikacode.com/bthate/koning',
     author='Bart Thate',
     author_email='bthate@dds.nl',
-    description=""" Wetsvoorstel tot het strafbaar maken van behandeling met antipsychotica. """,
+    description=""" Nieuwe Grondwet """,
     license='MIT',
     include_package_data=True,
     zip_safe=True,
     install_requires=["wet", ],
     scripts=["bin/koning", ],
     packages=['koning',
              ],
-    long_description=""" Antipsychotica zijn dodelijk en behandeling zonder verpleging is moord. """,
+    long_description=""" Nieuwe grondwet ter strafbaar stelling van het plegen van een oordeel dat een enkel persoon betreft. """,
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
         'Operating System :: Unix',
         'Programming Language :: Python',
         'Topic :: Software Development :: Libraries :: Python Modules'],
 )
```

### Comparing `koning-8/bin/koning` & `koning-9/bin/koning`

 * *Files identical despite different names*

### Comparing `koning-8/docs/jpg/20150406_001.jpg` & `koning-9/docs/jpg/20150406_001.jpg`

 * *Files identical despite different names*

### Comparing `koning-8/docs/jpg/20140730_011.jpg` & `koning-9/docs/jpg/20140730_011.jpg`

 * *Files identical despite different names*

### Comparing `koning-8/docs/LICENSE.rst` & `koning-9/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `koning-8/docs/txt/europa.rst` & `koning-9/docs/txt/europa.rst`

 * *Files identical despite different names*

### Comparing `koning-8/docs/txt/crisis.rst` & `koning-9/docs/txt/crisis.rst`

 * *Files identical despite different names*

### Comparing `koning-8/docs/txt/urls.rst` & `koning-9/docs/txt/urls.rst`

 * *Files identical despite different names*

### Comparing `koning-8/docs/txt/overeenkomst.rst` & `koning-9/docs/txt/overeenkomst.rst`

 * *Files identical despite different names*

### Comparing `koning-8/docs/txt/ambulant.rst` & `koning-9/docs/txt/ambulant.rst`

 * *Files identical despite different names*

### Comparing `koning-8/docs/txt/ccaf.rst` & `koning-9/docs/txt/ccaf.rst`

 * *Files identical despite different names*

### Comparing `koning-8/docs/txt/preventief.rst` & `koning-9/docs/txt/preventief.rst`

 * *Files identical despite different names*

### Comparing `koning-8/docs/index.rst` & `koning-9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `koning-8/koning/campagne.py` & `koning-9/koning/campagne.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,41 +79,41 @@
     l = []
     while 1:
         c = random.choice(tags)
         if c not in l: l.append(c)
         if len(l) == args[0]: break
     return " ".join(l)
 
-def genocide(*args, **kwargs):
+def heden(*args, **kwargs):
     time_diff = time.time() - today()
     aantalmin = time_diff/ 60
     crisis = int(aantalmin * crisismin)
     politie = int(aantalmin * politiemin)
     hap = int(aantalmin * hapmin)
     keten = int(aantalmin * ketenmin)
     verwijs = int(aantalmin * verwijsmin)
     uitstroom = int(aantalmin * uitstroommin)
     opname = int(aantalmin * opnamemin)
     suicide = int(aantalmin * suicidemin)
     elapsed = elapsed_days(time_diff)
     lastcrisis = 0
     if crisis > lastcrisis:
-        txt = "CRISIS %s POLITIE %s HAP %s KETEN %s VERWIJS %s UITSTROOM %s OPNAME %s SUICIDE %s %s %s" % (crisis, politie, hap, keten, verwijs, uitstroom, opname, suicide, url, elapsed)
+        txt = "CRISIS %s POLITIE %s HAP %s KETEN %s - VERWIJS %s UITSTROOM %s OPNAME %s SUICIDE %s %s %s" % (crisis, politie, hap, keten, verwijs, uitstroom, opname, suicide, url, elapsed)
         lastcrisis = crisis
         kernel.announce(txt)
 
-kernel.register("campagne.genocide", genocide)
+kernel.register("campagne.heden",heden)
 
 ## Campagne class
 
 class CRISIS(Repeater): pass
 class VERWIJS(Repeater): pass
 class UITSTROOM(Repeater): pass
 class OPNAME(Repeater): pass
 class SUICIDE(Repeater): pass
 class CRISIS(Repeater): pass
 
 ## campagne init
 
 def init(*args, **kwargs):
-    todo = CRISIS(genocide, int(60 * 60 * 24 / suicidedag))
+    todo = CRISIS(heden, int(60 * 60 * 24 / crisisdag))
     kernel.put(todo.start)
```

### Comparing `koning-8/koning/license.py` & `koning-9/koning/license.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 ## TXT
 
 license_txt = """
 
 Copyright 2015, B.H.J. Thate
 
-KONING %s - Wetsvoorstel tot het strafbaar maken van behandeling met antipsychotica.
+KONING %s - Nieuwe grondwet ter strafbaar stelling van het plegen van een oordeel dat een enkel persoon betreft.
 
 Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation
 files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the
```

### Comparing `koning-8/LICENSE` & `koning-9/LICENSE`

 * *Files identical despite different names*

