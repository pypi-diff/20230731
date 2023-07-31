# Comparing `tmp/pandasmemuc-0.10.tar.gz` & `tmp/pandasmemuc-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasmemuc-0.10.tar", last modified: Sun Jul 30 22:23:09 2023, max compression
+gzip compressed data, was "pandasmemuc-0.11.tar", last modified: Mon Jul 31 02:49:49 2023, max compression
```

## Comparing `pandasmemuc-0.10.tar` & `pandasmemuc-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 22:23:09.850656 pandasmemuc-0.10/
--rw-rw-rw-   0        0        0     1148 2023-07-30 22:22:55.000000 pandasmemuc-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      104 2023-07-30 22:22:55.000000 pandasmemuc-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     2347 2023-07-30 22:23:09.850656 pandasmemuc-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 22:23:09.847664 pandasmemuc-0.10/pandasmemuc/
--rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.10/pandasmemuc/README.MD
--rw-rw-rw-   0        0        0    95382 2023-07-30 03:42:39.000000 pandasmemuc-0.10/pandasmemuc/__init__.py
--rw-rw-rw-   0        0        0      147 2023-07-30 22:23:08.000000 pandasmemuc-0.10/pandasmemuc/requirements.txt
--rw-rw-rw-   0        0        0    22457 2023-07-30 22:23:08.000000 pandasmemuc-0.10/pandasmemuc/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-30 22:23:09.850656 pandasmemuc-0.10/pandasmemuc.egg-info/
--rw-rw-rw-   0        0        0     2347 2023-07-30 22:23:09.000000 pandasmemuc-0.10/pandasmemuc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-07-30 22:23:09.000000 pandasmemuc-0.10/pandasmemuc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 22:23:09.000000 pandasmemuc-0.10/pandasmemuc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2023-07-30 22:23:09.000000 pandasmemuc-0.10/pandasmemuc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-30 22:23:09.000000 pandasmemuc-0.10/pandasmemuc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-30 22:23:09.851653 pandasmemuc-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1584 2023-07-30 22:23:08.000000 pandasmemuc-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:49:49.533095 pandasmemuc-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-07-31 02:49:37.000000 pandasmemuc-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      104 2023-07-31 02:49:35.000000 pandasmemuc-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     2347 2023-07-31 02:49:49.534071 pandasmemuc-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 02:49:49.529191 pandasmemuc-0.11/pandasmemuc/
+-rw-rw-rw-   0        0        0     1732 2023-07-30 22:20:11.000000 pandasmemuc-0.11/pandasmemuc/README.MD
+-rw-rw-rw-   0        0        0    95548 2023-07-31 02:44:44.000000 pandasmemuc-0.11/pandasmemuc/__init__.py
+-rw-rw-rw-   0        0        0      147 2023-07-31 02:49:48.000000 pandasmemuc-0.11/pandasmemuc/requirements.txt
+-rw-rw-rw-   0        0        0    22457 2023-07-31 02:49:48.000000 pandasmemuc-0.11/pandasmemuc/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-31 02:49:49.533095 pandasmemuc-0.11/pandasmemuc.egg-info/
+-rw-rw-rw-   0        0        0     2347 2023-07-31 02:49:49.000000 pandasmemuc-0.11/pandasmemuc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-07-31 02:49:49.000000 pandasmemuc-0.11/pandasmemuc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 02:49:49.000000 pandasmemuc-0.11/pandasmemuc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2023-07-31 02:49:49.000000 pandasmemuc-0.11/pandasmemuc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-31 02:49:49.000000 pandasmemuc-0.11/pandasmemuc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-31 02:49:49.535048 pandasmemuc-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1584 2023-07-31 02:49:48.000000 pandasmemuc-0.11/setup.py
```

### Comparing `pandasmemuc-0.10/LICENSE.rst` & `pandasmemuc-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pandasmemuc-0.10/PKG-INFO` & `pandasmemuc-0.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasmemuc
-Version: 0.10
+Version: 0.11
 Summary: Automating memu emulator with pandas
 Home-page: https://github.com/hansalemaos/pandasmemuc
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: memu,memnuc,pandas
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pandasmemuc-0.10/README.md` & `pandasmemuc-0.11/README.md`

 * *Files identical despite different names*

### Comparing `pandasmemuc-0.10/pandasmemuc/README.MD` & `pandasmemuc-0.11/pandasmemuc/README.MD`

 * *Files identical despite different names*

### Comparing `pandasmemuc-0.10/pandasmemuc/__init__.py` & `pandasmemuc-0.11/pandasmemuc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3058,15 +3058,20 @@
         swipe_variation_starty=10,
         swipe_variation_endy=10,
         sdcard="/storage/emulated/0/",
         tmp_folder_on_sd_card="AUTOMAT",
         bluestacks_divider=32767,
     ):
         df2 = self.df.loc[self.df.aa_index == i]
-        df2.bb_adbtools.iloc[0].aa_update_screenshot()
+        try:
+            df2.bb_adbtools.iloc[0].aa_update_screenshot()
+        except Exception:
+            print('Could not get screenshot')
+            save_screenshot = False
+            screenshotfolder = None
         df3 = df2.bb_adbtools.iloc[0].aa_get_all_displayed_items_from_uiautomator(
             screenshotfolder=screenshotfolder,
             max_variation_percent_x=max_variation_percent_x,
             max_variation_percent_y=max_variation_percent_y,
             loung_touch_delay=loung_touch_delay,
             swipe_variation_startx=swipe_variation_startx,
             swipe_variation_endx=swipe_variation_endx,
```

### Comparing `pandasmemuc-0.10/pandasmemuc/thirdparty.json` & `pandasmemuc-0.11/pandasmemuc/thirdparty.json`

 * *Files identical despite different names*

### Comparing `pandasmemuc-0.10/pandasmemuc.egg-info/PKG-INFO` & `pandasmemuc-0.11/pandasmemuc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasmemuc
-Version: 0.10
+Version: 0.11
 Summary: Automating memu emulator with pandas
 Home-page: https://github.com/hansalemaos/pandasmemuc
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: memu,memnuc,pandas
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pandasmemuc-0.10/setup.py` & `pandasmemuc-0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Automating memu emulator with pandas'''
 
 # Setting up
 setup(
     name="pandasmemuc",
     version=VERSION,
     license='MIT',
```

