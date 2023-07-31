# Comparing `tmp/idev-pycolor-1.0.2.tar.gz` & `tmp/idev-pycolor-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idev-pycolor-1.0.2.tar", last modified: Mon Jul 31 03:32:47 2023, max compression
+gzip compressed data, was "idev-pycolor-1.0.3.tar", last modified: Mon Jul 31 06:35:56 2023, max compression
```

## Comparing `idev-pycolor-1.0.2.tar` & `idev-pycolor-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 03:32:47.643077 idev-pycolor-1.0.2/
--rw-rw-rw-   0        0        0     1083 2023-07-28 03:09:18.000000 idev-pycolor-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     7998 2023-07-31 03:32:47.643077 idev-pycolor-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     7252 2023-07-31 03:31:04.000000 idev-pycolor-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 03:32:47.612414 idev-pycolor-1.0.2/idev-pycolor/
-drwxrwxrwx   0        0        0        0 2023-07-31 03:32:47.626026 idev-pycolor-1.0.2/idev-pycolor/PyColor/
--rw-rw-rw-   0        0        0    37234 2023-07-31 03:25:15.000000 idev-pycolor-1.0.2/idev-pycolor/PyColor/Colors.py
--rw-rw-rw-   0        0        0     4265 2023-07-28 03:09:18.000000 idev-pycolor-1.0.2/idev-pycolor/PyColor/Palettes.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:09:18.000000 idev-pycolor-1.0.2/idev-pycolor/PyColor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 03:32:47.642076 idev-pycolor-1.0.2/idev-pycolor/idev_pycolor.egg-info/
--rw-rw-rw-   0        0        0     7998 2023-07-31 03:32:47.000000 idev-pycolor-1.0.2/idev-pycolor/idev_pycolor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-07-31 03:32:47.000000 idev-pycolor-1.0.2/idev-pycolor/idev_pycolor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 03:32:47.000000 idev-pycolor-1.0.2/idev-pycolor/idev_pycolor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 03:32:47.000000 idev-pycolor-1.0.2/idev-pycolor/idev_pycolor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      740 2023-07-31 03:32:24.000000 idev-pycolor-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      893 2023-07-31 03:32:47.645594 idev-pycolor-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      985 2023-07-31 03:32:18.000000 idev-pycolor-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:35:56.657070 idev-pycolor-1.0.3/
+-rw-rw-rw-   0        0        0     1083 2023-07-28 03:09:18.000000 idev-pycolor-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     7998 2023-07-31 06:35:56.658073 idev-pycolor-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7252 2023-07-31 03:31:04.000000 idev-pycolor-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 06:35:56.623524 idev-pycolor-1.0.3/idev-pycolor/
+drwxrwxrwx   0        0        0        0 2023-07-31 06:35:56.635035 idev-pycolor-1.0.3/idev-pycolor/PyColor/
+-rw-rw-rw-   0        0        0    37396 2023-07-31 06:29:08.000000 idev-pycolor-1.0.3/idev-pycolor/PyColor/Colors.py
+-rw-rw-rw-   0        0        0     4265 2023-07-28 03:09:18.000000 idev-pycolor-1.0.3/idev-pycolor/PyColor/Palettes.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:09:18.000000 idev-pycolor-1.0.3/idev-pycolor/PyColor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:35:56.656070 idev-pycolor-1.0.3/idev-pycolor/idev_pycolor.egg-info/
+-rw-rw-rw-   0        0        0     7998 2023-07-31 06:35:56.000000 idev-pycolor-1.0.3/idev-pycolor/idev_pycolor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-07-31 06:35:56.000000 idev-pycolor-1.0.3/idev-pycolor/idev_pycolor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 06:35:56.000000 idev-pycolor-1.0.3/idev-pycolor/idev_pycolor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 06:35:56.000000 idev-pycolor-1.0.3/idev-pycolor/idev_pycolor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      740 2023-07-31 06:35:15.000000 idev-pycolor-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      893 2023-07-31 06:35:56.665143 idev-pycolor-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      985 2023-07-31 06:35:22.000000 idev-pycolor-1.0.3/setup.py
```

### Comparing `idev-pycolor-1.0.2/LICENSE` & `idev-pycolor-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idev-pycolor-1.0.2/PKG-INFO` & `idev-pycolor-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idev-pycolor
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.
 Home-page: https://github.com/IrtsaDevelopment/PyColor
 Author: IrtsaDevelopment
 Author-email: Irtsa <irtsa.development@gmail.com>
 Project-URL: Homepage, https://github.com/IrtsaDevelopment/PyColor
 Project-URL: Bug Tracker, https://github.com/IrtsaDevelopment/PyColor/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `idev-pycolor-1.0.2/README.md` & `idev-pycolor-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `idev-pycolor-1.0.2/idev-pycolor/PyColor/Colors.py` & `idev-pycolor-1.0.3/idev-pycolor/PyColor/Colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,18 @@
     @property
     def grayscale(self) -> tuple:
         if not self.__valid: return None
 
         gv = int(round((self.red + self.green + self.blue) / 3.0))
 
         return RGB(gv, gv, gv)
+    
+
+    @property
+    def greyscale(self) -> tuple: return self.grayscale
         
 
 
     def __repr__(self):
         if not self.__valid: return 'Invalid RGB'
         return str(self.red) + ' ' + str(self.green) + ' ' + str(self.blue)
 
@@ -330,24 +334,15 @@
         if not self.__valid: return None
 
         y = round((16 + ((65.738 * self.rgb[0]) / 256) + ((129.057 * self.rgb[1]) / 256) + ((25.064 * self.rgb[2]) / 256)), 2)
         cb = round((128 - ((37.945 * self.rgb[0]) / 256) - ((74.494 * self.rgb[1]) / 256) + ((112.439 * self.rgb[2]) / 256)), 2)
         cr = round((128 + ((112.439 * self.rgb[0]) / 256) - ((94.154 * self.rgb[1]) / 256) - ((18.285 * self.rgb[2]) / 256)), 2)
 
         return (y, cb, cr)
-    
 
-    @property
-    def grayscale(self) -> tuple:
-        if not self.__valid: return None
-
-        gv = int(round((self.rgb[0] + self.rgb[1] + self.rgb[2]) / 3.0))
-        rgbGray = RGB(gv, gv, gv)
-
-        return HEX(rgbGray.hexidecimal)
       
 
     @property
     def cmyk(self):
         if not self.__valid: return None
 
         nr = self.rgb[0] / 255.0
@@ -371,14 +366,28 @@
         Numbers = [((16 ** i) * Numbers[i]) for i in range(len(Numbers))]
 
         number = sum(Numbers)
 
         return round((number / 16777215.0), 3)
     
 
+    @property
+    def grayscale(self) -> tuple:
+        if not self.__valid: return None
+
+        gv = int(round((self.rgb[0] + self.rgb[1] + self.rgb[2]) / 3.0))
+        rgbGray = RGB(gv, gv, gv)
+
+        return HEX(rgbGray.hexidecimal)
+    
+
+    @property
+    def greyscale(self) -> tuple: return self.grayscale
+    
+
 
     def __repr__(self):
         if not self.__valid: return 'Invalid HEX'
         return self.hexicode
```

### Comparing `idev-pycolor-1.0.2/idev-pycolor/PyColor/Palettes.py` & `idev-pycolor-1.0.3/idev-pycolor/PyColor/Palettes.py`

 * *Files identical despite different names*

### Comparing `idev-pycolor-1.0.2/idev-pycolor/idev_pycolor.egg-info/PKG-INFO` & `idev-pycolor-1.0.3/idev-pycolor/idev_pycolor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idev-pycolor
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.
 Home-page: https://github.com/IrtsaDevelopment/PyColor
 Author: IrtsaDevelopment
 Author-email: Irtsa <irtsa.development@gmail.com>
 Project-URL: Homepage, https://github.com/IrtsaDevelopment/PyColor
 Project-URL: Bug Tracker, https://github.com/IrtsaDevelopment/PyColor/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `idev-pycolor-1.0.2/pyproject.toml` & `idev-pycolor-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "idev-pycolor"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Irtsa", email="irtsa.development@gmail.com" },
 ]
 description = "A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `idev-pycolor-1.0.2/setup.cfg` & `idev-pycolor-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 6465 762d 7079 636f 6c6f 720d   = idev-pycolor.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e32  .version = 1.0.2
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e33  .version = 1.0.3
 00000030: 0d0a 6175 7468 6f72 203d 2049 7274 7361  ..author = Irtsa
 00000040: 4465 7665 6c6f 706d 656e 740d 0a61 7574  Development..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6972 7473  hor_email = irts
 00000060: 612e 6465 7665 6c6f 706d 656e 7440 676d  a.development@gm
 00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000080: 7469 6f6e 203d 2041 2070 7974 686f 6e20  tion = A python 
 00000090: 636f 6c6c 6563 7469 6f6e 206f 6620 636c  collection of cl
```

### Comparing `idev-pycolor-1.0.2/setup.py` & `idev-pycolor-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "idev-pycolor",
-    version = "1.0.2",
+    version = "1.0.3",
     author = "IrtsaDevelopment",
     author_email = "irtsa.development@gmail.com",
     description = "A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/IrtsaDevelopment/PyColor",
     project_urls = {
```

