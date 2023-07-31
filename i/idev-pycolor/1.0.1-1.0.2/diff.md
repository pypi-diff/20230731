# Comparing `tmp/idev-pycolor-1.0.1.tar.gz` & `tmp/idev-pycolor-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idev-pycolor-1.0.1.tar", last modified: Fri Jul 28 20:30:49 2023, max compression
+gzip compressed data, was "idev-pycolor-1.0.2.tar", last modified: Mon Jul 31 03:32:47 2023, max compression
```

## Comparing `idev-pycolor-1.0.1.tar` & `idev-pycolor-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 20:30:49.479784 idev-pycolor-1.0.1/
--rw-rw-rw-   0        0        0     1083 2023-07-28 03:09:18.000000 idev-pycolor-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     7275 2023-07-28 20:30:49.480785 idev-pycolor-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6529 2023-07-28 20:30:17.000000 idev-pycolor-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 20:30:49.432784 idev-pycolor-1.0.1/idev-pycolor/
-drwxrwxrwx   0        0        0        0 2023-07-28 20:30:49.462783 idev-pycolor-1.0.1/idev-pycolor/PyColor/
--rw-rw-rw-   0        0        0    35141 2023-07-28 06:33:41.000000 idev-pycolor-1.0.1/idev-pycolor/PyColor/Colors.py
--rw-rw-rw-   0        0        0     4265 2023-07-28 03:09:18.000000 idev-pycolor-1.0.1/idev-pycolor/PyColor/Palettes.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:09:18.000000 idev-pycolor-1.0.1/idev-pycolor/PyColor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-28 20:30:49.478785 idev-pycolor-1.0.1/idev-pycolor/idev_pycolor.egg-info/
--rw-rw-rw-   0        0        0     7275 2023-07-28 20:30:49.000000 idev-pycolor-1.0.1/idev-pycolor/idev_pycolor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-07-28 20:30:49.000000 idev-pycolor-1.0.1/idev-pycolor/idev_pycolor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 20:30:49.000000 idev-pycolor-1.0.1/idev-pycolor/idev_pycolor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-28 20:30:49.000000 idev-pycolor-1.0.1/idev-pycolor/idev_pycolor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      740 2023-07-28 20:29:39.000000 idev-pycolor-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      893 2023-07-28 20:30:49.482029 idev-pycolor-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      985 2023-07-28 20:29:44.000000 idev-pycolor-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:32:47.643077 idev-pycolor-1.0.2/
+-rw-rw-rw-   0        0        0     1083 2023-07-28 03:09:18.000000 idev-pycolor-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     7998 2023-07-31 03:32:47.643077 idev-pycolor-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7252 2023-07-31 03:31:04.000000 idev-pycolor-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 03:32:47.612414 idev-pycolor-1.0.2/idev-pycolor/
+drwxrwxrwx   0        0        0        0 2023-07-31 03:32:47.626026 idev-pycolor-1.0.2/idev-pycolor/PyColor/
+-rw-rw-rw-   0        0        0    37234 2023-07-31 03:25:15.000000 idev-pycolor-1.0.2/idev-pycolor/PyColor/Colors.py
+-rw-rw-rw-   0        0        0     4265 2023-07-28 03:09:18.000000 idev-pycolor-1.0.2/idev-pycolor/PyColor/Palettes.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:09:18.000000 idev-pycolor-1.0.2/idev-pycolor/PyColor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:32:47.642076 idev-pycolor-1.0.2/idev-pycolor/idev_pycolor.egg-info/
+-rw-rw-rw-   0        0        0     7998 2023-07-31 03:32:47.000000 idev-pycolor-1.0.2/idev-pycolor/idev_pycolor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-07-31 03:32:47.000000 idev-pycolor-1.0.2/idev-pycolor/idev_pycolor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 03:32:47.000000 idev-pycolor-1.0.2/idev-pycolor/idev_pycolor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 03:32:47.000000 idev-pycolor-1.0.2/idev-pycolor/idev_pycolor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      740 2023-07-31 03:32:24.000000 idev-pycolor-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      893 2023-07-31 03:32:47.645594 idev-pycolor-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      985 2023-07-31 03:32:18.000000 idev-pycolor-1.0.2/setup.py
```

### Comparing `idev-pycolor-1.0.1/LICENSE` & `idev-pycolor-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idev-pycolor-1.0.1/PKG-INFO` & `idev-pycolor-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idev-pycolor
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.
 Home-page: https://github.com/IrtsaDevelopment/PyColor
 Author: IrtsaDevelopment
 Author-email: Irtsa <irtsa.development@gmail.com>
 Project-URL: Homepage, https://github.com/IrtsaDevelopment/PyColor
 Project-URL: Bug Tracker, https://github.com/IrtsaDevelopment/PyColor/issues
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 - **CMYK** (*cyan*, *magenta*, *yellow*, *key*)
 - **HEX** (*hexidecimal*)
 <br />
 <br />
 <br />
 
 ## Installation
-With `git` [GitHub](https://github.com):
+With `git` [GitHub](https://github.com/IrtsaDevelopment/PyColor):
 ```
 git clone https://github.com/IrtsaDevelopment/PyColor.git
 ```
 or with `pip` [PyPi](https://pypi.org/project/idev-pycolor/):
 ```
 pip install idev-pycolor
 ```
@@ -76,14 +76,18 @@
 rgb.cmyk
 # Returns a tuple of the cmyk values from rgb.
 rgb.hexidecimal
 # Returns a string of the hexidecimal value from rgb.
 
 rgb.percentForm
 # Returns a tuple of the rgb values in a decimal percent form (0-1).
+rgb.grayscale
+# Returns a grayscaled version of the RGB class.
+rgb.greyscale
+# Is .grayscale
 ```
 ```py
 hsv.rgb
 # Returns a tuple of the rgb values from hsv.
 hsv.hsv
 # Returns a tuple of the hsv values from hsv.
 hsv.hsl
@@ -95,14 +99,18 @@
 hsv.cmyk
 # Returns a tuple of the cmyk values from hsv.
 hsv.hexidecimal
 # Returns a string of the hexidecimal value from hsv.
 
 hsv.percentForm
 # Returns a tuple of the hsv values in a decimal percent form (0-1).
+hsv.grayscale
+# Returns a grayscaled version of the HSV class.
+hsv.greyscale
+# Is .grayscale
 ```
 ```py
 hsl.rgb
 # Returns a tuple of the rgb values from hsl.
 hsl.hsv
 # Returns a tuple of the hsv values from hsl.
 hsl.hsl
@@ -114,14 +122,18 @@
 hsl.cmyk
 # Returns a tuple of the cmyk values from hsl.
 hsl.hexidecimal
 # Returns a string of the hexidecimal value from hsl.
 
 hsl.percentForm
 # Returns a tuple of the hsl values in a decimal percent form (0-1).
+hsl.grayscale
+# Returns a grayscaled version of the HSL class.
+hsl.greyscale
+# Is .grayscale
 ```
 ```py
 xyz.rgb
 # Returns a tuple of the rgb values from xyz.
 xyz.hsv
 # Returns a tuple of the hsv values from xyz.
 xyz.hsl
@@ -133,14 +145,18 @@
 xyz.cmyk
 # Returns a tuple of the cmyk values from xyz.
 xyz.hexidecimal
 # Returns a string of the hexidecimal value from xyz.
 
 xyz.percentForm
 # Returns a tuple of the xyz values in a decimal percent form (0-1).
+xyz.grayscale
+# Returns a grayscaled version of the XYZ class.
+xyz.greyscale
+# Is .grayscale
 ```
 ```py
 ycc.rgb
 # Returns a tuple of the rgb values from ycc.
 ycc.hsv
 # Returns a tuple of the hsv values from ycc.
 ycc.hsl
@@ -150,16 +166,20 @@
 ycc.ycc
 # Returns a tuple of the ycc values from ycc.
 ycc.cmyk
 # Returns a tuple of the cmyk values from ycc.
 ycc.hexidecimal
 # Returns a string of the hexidecimal value from ycc.
 
-hsl.percentForm
+ycc.percentForm
 # Returns a tuple of the ycc values in a decimal percent form (0-1).
+ycc.grayscale
+# Returns a grayscaled version of the YCC class.
+ycc.greyscale
+# Is .grayscale
 ```
 ```py
 cmyk.rgb
 # Returns a tuple of the rgb values from cmyk.
 cmyk.hsv
 # Returns a tuple of the hsv values from cmyk.
 cmyk.hsl
@@ -171,14 +191,18 @@
 cmyk.cmyk
 # Returns a tuple of the cmyk values from cmyk.
 cmyk.hexidecimal
 # Returns a string of the hexidecimal value from cmyk.
 
 cmyk.percentForm
 # Returns a tuple of the cmyk values in a decimal percent form (0-1).
+cmyk.grayscale
+# Returns a grayscaled version of the CMYK class.
+cmyk.greyscale
+# Is .grayscale
 ```
 ```py
 hexidecimal.rgb
 # Returns a tuple of the rgb values from hexidecimal.
 hexidecimal.hsv
 # Returns a tuple of the hsv values from hexidecimal.
 hexidecimal.hsl
@@ -190,14 +214,18 @@
 hexidecimal.cmyk
 # Returns a tuple of the cmyk values from hexidecimal.
 hexidecimal.hexidecimal
 # Returns a string of the hexidecimal value from hexidecimal.
 
 hexidecimal.percentForm
 # Returns a decimal percent form (0-1) of the hexidecimal value.
+hexidecimal.grayscale
+# Returns a grayscaled version of the HEX class.
+hexidecimal.greyscale
+# Is .grayscale
 ```
 ```py
 print(rgb)
 # Will print off a string representation of the rgb values.
 
 print(hsv)
 # Will print off a string representation of the hsv values.
```

### Comparing `idev-pycolor-1.0.1/README.md` & `idev-pycolor-1.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 - **CMYK** (*cyan*, *magenta*, *yellow*, *key*)
 - **HEX** (*hexidecimal*)
 <br />
 <br />
 <br />
 
 ## Installation
-With `git` [GitHub](https://github.com):
+With `git` [GitHub](https://github.com/IrtsaDevelopment/PyColor):
 ```
 git clone https://github.com/IrtsaDevelopment/PyColor.git
 ```
 or with `pip` [PyPi](https://pypi.org/project/idev-pycolor/):
 ```
 pip install idev-pycolor
 ```
@@ -60,14 +60,18 @@
 rgb.cmyk
 # Returns a tuple of the cmyk values from rgb.
 rgb.hexidecimal
 # Returns a string of the hexidecimal value from rgb.
 
 rgb.percentForm
 # Returns a tuple of the rgb values in a decimal percent form (0-1).
+rgb.grayscale
+# Returns a grayscaled version of the RGB class.
+rgb.greyscale
+# Is .grayscale
 ```
 ```py
 hsv.rgb
 # Returns a tuple of the rgb values from hsv.
 hsv.hsv
 # Returns a tuple of the hsv values from hsv.
 hsv.hsl
@@ -79,14 +83,18 @@
 hsv.cmyk
 # Returns a tuple of the cmyk values from hsv.
 hsv.hexidecimal
 # Returns a string of the hexidecimal value from hsv.
 
 hsv.percentForm
 # Returns a tuple of the hsv values in a decimal percent form (0-1).
+hsv.grayscale
+# Returns a grayscaled version of the HSV class.
+hsv.greyscale
+# Is .grayscale
 ```
 ```py
 hsl.rgb
 # Returns a tuple of the rgb values from hsl.
 hsl.hsv
 # Returns a tuple of the hsv values from hsl.
 hsl.hsl
@@ -98,14 +106,18 @@
 hsl.cmyk
 # Returns a tuple of the cmyk values from hsl.
 hsl.hexidecimal
 # Returns a string of the hexidecimal value from hsl.
 
 hsl.percentForm
 # Returns a tuple of the hsl values in a decimal percent form (0-1).
+hsl.grayscale
+# Returns a grayscaled version of the HSL class.
+hsl.greyscale
+# Is .grayscale
 ```
 ```py
 xyz.rgb
 # Returns a tuple of the rgb values from xyz.
 xyz.hsv
 # Returns a tuple of the hsv values from xyz.
 xyz.hsl
@@ -117,14 +129,18 @@
 xyz.cmyk
 # Returns a tuple of the cmyk values from xyz.
 xyz.hexidecimal
 # Returns a string of the hexidecimal value from xyz.
 
 xyz.percentForm
 # Returns a tuple of the xyz values in a decimal percent form (0-1).
+xyz.grayscale
+# Returns a grayscaled version of the XYZ class.
+xyz.greyscale
+# Is .grayscale
 ```
 ```py
 ycc.rgb
 # Returns a tuple of the rgb values from ycc.
 ycc.hsv
 # Returns a tuple of the hsv values from ycc.
 ycc.hsl
@@ -134,16 +150,20 @@
 ycc.ycc
 # Returns a tuple of the ycc values from ycc.
 ycc.cmyk
 # Returns a tuple of the cmyk values from ycc.
 ycc.hexidecimal
 # Returns a string of the hexidecimal value from ycc.
 
-hsl.percentForm
+ycc.percentForm
 # Returns a tuple of the ycc values in a decimal percent form (0-1).
+ycc.grayscale
+# Returns a grayscaled version of the YCC class.
+ycc.greyscale
+# Is .grayscale
 ```
 ```py
 cmyk.rgb
 # Returns a tuple of the rgb values from cmyk.
 cmyk.hsv
 # Returns a tuple of the hsv values from cmyk.
 cmyk.hsl
@@ -155,14 +175,18 @@
 cmyk.cmyk
 # Returns a tuple of the cmyk values from cmyk.
 cmyk.hexidecimal
 # Returns a string of the hexidecimal value from cmyk.
 
 cmyk.percentForm
 # Returns a tuple of the cmyk values in a decimal percent form (0-1).
+cmyk.grayscale
+# Returns a grayscaled version of the CMYK class.
+cmyk.greyscale
+# Is .grayscale
 ```
 ```py
 hexidecimal.rgb
 # Returns a tuple of the rgb values from hexidecimal.
 hexidecimal.hsv
 # Returns a tuple of the hsv values from hexidecimal.
 hexidecimal.hsl
@@ -174,14 +198,18 @@
 hexidecimal.cmyk
 # Returns a tuple of the cmyk values from hexidecimal.
 hexidecimal.hexidecimal
 # Returns a string of the hexidecimal value from hexidecimal.
 
 hexidecimal.percentForm
 # Returns a decimal percent form (0-1) of the hexidecimal value.
+hexidecimal.grayscale
+# Returns a grayscaled version of the HEX class.
+hexidecimal.greyscale
+# Is .grayscale
 ```
 ```py
 print(rgb)
 # Will print off a string representation of the rgb values.
 
 print(hsv)
 # Will print off a string representation of the hsv values.
```

### Comparing `idev-pycolor-1.0.1/idev-pycolor/PyColor/Colors.py` & `idev-pycolor-1.0.2/idev-pycolor/PyColor/Colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,23 @@
         if not self.__valid: return None
 
         r = round((self.red / 255.0), 2)
         g = round((self.green / 255.0), 2)
         b = round((self.blue / 255.0), 2)
 
         return (r, g, b)
+    
+
+    @property
+    def grayscale(self) -> tuple:
+        if not self.__valid: return None
+
+        gv = int(round((self.red + self.green + self.blue) / 3.0))
+
+        return RGB(gv, gv, gv)
         
 
 
     def __repr__(self):
         if not self.__valid: return 'Invalid RGB'
         return str(self.red) + ' ' + str(self.green) + ' ' + str(self.blue)
 
@@ -321,14 +330,24 @@
         if not self.__valid: return None
 
         y = round((16 + ((65.738 * self.rgb[0]) / 256) + ((129.057 * self.rgb[1]) / 256) + ((25.064 * self.rgb[2]) / 256)), 2)
         cb = round((128 - ((37.945 * self.rgb[0]) / 256) - ((74.494 * self.rgb[1]) / 256) + ((112.439 * self.rgb[2]) / 256)), 2)
         cr = round((128 + ((112.439 * self.rgb[0]) / 256) - ((94.154 * self.rgb[1]) / 256) - ((18.285 * self.rgb[2]) / 256)), 2)
 
         return (y, cb, cr)
+    
+
+    @property
+    def grayscale(self) -> tuple:
+        if not self.__valid: return None
+
+        gv = int(round((self.rgb[0] + self.rgb[1] + self.rgb[2]) / 3.0))
+        rgbGray = RGB(gv, gv, gv)
+
+        return HEX(rgbGray.hexidecimal)
       
 
     @property
     def cmyk(self):
         if not self.__valid: return None
 
         nr = self.rgb[0] / 255.0
@@ -522,14 +541,28 @@
         h = round((self.hue / 360.0), 2)
         s = round((self.saturation / 100.0), 2)
         v = round((self.value / 100.0), 2)
 
         return (h, s, v)
     
 
+    @property
+    def grayscale(self) -> tuple:
+        if not self.__valid: return None
+
+        gv = int(round((self.rgb[0] + self.rgb[1] + self.rgb[2]) / 3.0))
+        rgbGray = RGB(gv, gv, gv)
+
+        return HSV(*rgbGray.hsv)
+    
+
+    @property
+    def greyscale(self) -> tuple: return self.grayscale
+    
+
 
     def __repr__(self):
         if not self.__valid: return 'Invalid HSV'
         return str(self.hue) + '° ' + str(self.saturation) + '% ' + str(self.value) + '%'
 
 
 
@@ -691,14 +724,28 @@
         h = round((self.hue / 360.0), 2)
         s = round((self.saturation / 100.0), 2)
         l = round((self.lightness / 100.0), 2)
 
         return (h, s, l)
     
 
+    @property
+    def grayscale(self) -> tuple:
+        if not self.__valid: return None
+
+        gv = int(round((self.rgb[0] + self.rgb[1] + self.rgb[2]) / 3.0))
+        rgbGray = RGB(gv, gv, gv)
+
+        return HSL(*rgbGray.hsl)
+    
+
+    @property
+    def greyscale(self) -> tuple: return self.grayscale
+    
+
 
     def __repr__(self):
         if not self.__valid: return 'Invalid HSL'
         return str(self.hue) + '° ' + str(self.saturation) + '% ' + str(self.lightness) + '%'
 
 
 
@@ -867,14 +914,28 @@
     @property
     def percentForm(self) -> float:
         x = round((self.x / 95.05), 2)
         y = round((self.y / 100.0), 2)
         z = round((self.z / 108.9), 2)
 
         return (x, y, z)
+    
+
+    @property
+    def grayscale(self) -> tuple:
+        if not self.__valid: return None
+
+        gv = int(round((self.rgb[0] + self.rgb[1] + self.rgb[2]) / 3.0))
+        rgbGray = RGB(gv, gv, gv)
+
+        return XYZ(*rgbGray.xyz)
+    
+
+    @property
+    def greyscale(self) -> tuple: return self.grayscale
 
 
 
     def __repr__(self):
         if not self.__valid: return 'Invalid XYZ'
         return str(self.x) + '% ' + str(self.y) + '% ' + str(self.z) + '%'
 
@@ -1058,14 +1119,28 @@
         y = round((self.cyan / 255.0), 2)
         cb = round((self.magenta / 255.0), 2)
         cr = round((self.yellow / 255.0), 2)
 
         return (y, cb, cr)
     
 
+    @property
+    def grayscale(self) -> tuple:
+        if not self.__valid: return None
+
+        gv = int(round((self.rgb[0] + self.rgb[1] + self.rgb[2]) / 3.0))
+        rgbGray = RGB(gv, gv, gv)
+
+        return YCC(*rgbGray.ycc)
+    
+
+    @property
+    def greyscale(self) -> tuple: return self.grayscale
+    
+
     def __repr__(self):
         if not self.__valid: return 'Invalid YCC'
         return str(self.y) + ' ' + str(self.cb) + ' ' + str(self.cr)
     
 
 
 
@@ -1235,13 +1310,27 @@
 
         c = round((self.cyan / 100.0), 2)
         m = round((self.magenta / 100.0), 2)
         y = round((self.yellow / 100.0), 2)
         k = round((self.key / 100.0), 2)
 
         return (c, m, y, k)
+    
+
+    @property
+    def grayscale(self) -> tuple:
+        if not self.__valid: return None
+
+        gv = int(round((self.rgb[0] + self.rgb[1] + self.rgb[2]) / 3.0))
+        rgbGray = RGB(gv, gv, gv)
+
+        return CMYK(*rgbGray.cmyk)
+    
+
+    @property
+    def greyscale(self) -> tuple: return self.grayscale
 
 
     
     def __repr__(self):
         if not self.__valid: return 'Invalid CMYK'
-        return str(self.cyan) + '% ' + str(self.magenta) + '% ' + str(self.yellow) + '% ' + str(self.key) + '%'
+        return str(self.cyan) + '% ' + str(self.magenta) + '% ' + str(self.yellow) + '% ' + str(self.key) + '%'
```

### Comparing `idev-pycolor-1.0.1/idev-pycolor/PyColor/Palettes.py` & `idev-pycolor-1.0.2/idev-pycolor/PyColor/Palettes.py`

 * *Files identical despite different names*

### Comparing `idev-pycolor-1.0.1/idev-pycolor/idev_pycolor.egg-info/PKG-INFO` & `idev-pycolor-1.0.2/idev-pycolor/idev_pycolor.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idev-pycolor
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.
 Home-page: https://github.com/IrtsaDevelopment/PyColor
 Author: IrtsaDevelopment
 Author-email: Irtsa <irtsa.development@gmail.com>
 Project-URL: Homepage, https://github.com/IrtsaDevelopment/PyColor
 Project-URL: Bug Tracker, https://github.com/IrtsaDevelopment/PyColor/issues
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 - **CMYK** (*cyan*, *magenta*, *yellow*, *key*)
 - **HEX** (*hexidecimal*)
 <br />
 <br />
 <br />
 
 ## Installation
-With `git` [GitHub](https://github.com):
+With `git` [GitHub](https://github.com/IrtsaDevelopment/PyColor):
 ```
 git clone https://github.com/IrtsaDevelopment/PyColor.git
 ```
 or with `pip` [PyPi](https://pypi.org/project/idev-pycolor/):
 ```
 pip install idev-pycolor
 ```
@@ -76,14 +76,18 @@
 rgb.cmyk
 # Returns a tuple of the cmyk values from rgb.
 rgb.hexidecimal
 # Returns a string of the hexidecimal value from rgb.
 
 rgb.percentForm
 # Returns a tuple of the rgb values in a decimal percent form (0-1).
+rgb.grayscale
+# Returns a grayscaled version of the RGB class.
+rgb.greyscale
+# Is .grayscale
 ```
 ```py
 hsv.rgb
 # Returns a tuple of the rgb values from hsv.
 hsv.hsv
 # Returns a tuple of the hsv values from hsv.
 hsv.hsl
@@ -95,14 +99,18 @@
 hsv.cmyk
 # Returns a tuple of the cmyk values from hsv.
 hsv.hexidecimal
 # Returns a string of the hexidecimal value from hsv.
 
 hsv.percentForm
 # Returns a tuple of the hsv values in a decimal percent form (0-1).
+hsv.grayscale
+# Returns a grayscaled version of the HSV class.
+hsv.greyscale
+# Is .grayscale
 ```
 ```py
 hsl.rgb
 # Returns a tuple of the rgb values from hsl.
 hsl.hsv
 # Returns a tuple of the hsv values from hsl.
 hsl.hsl
@@ -114,14 +122,18 @@
 hsl.cmyk
 # Returns a tuple of the cmyk values from hsl.
 hsl.hexidecimal
 # Returns a string of the hexidecimal value from hsl.
 
 hsl.percentForm
 # Returns a tuple of the hsl values in a decimal percent form (0-1).
+hsl.grayscale
+# Returns a grayscaled version of the HSL class.
+hsl.greyscale
+# Is .grayscale
 ```
 ```py
 xyz.rgb
 # Returns a tuple of the rgb values from xyz.
 xyz.hsv
 # Returns a tuple of the hsv values from xyz.
 xyz.hsl
@@ -133,14 +145,18 @@
 xyz.cmyk
 # Returns a tuple of the cmyk values from xyz.
 xyz.hexidecimal
 # Returns a string of the hexidecimal value from xyz.
 
 xyz.percentForm
 # Returns a tuple of the xyz values in a decimal percent form (0-1).
+xyz.grayscale
+# Returns a grayscaled version of the XYZ class.
+xyz.greyscale
+# Is .grayscale
 ```
 ```py
 ycc.rgb
 # Returns a tuple of the rgb values from ycc.
 ycc.hsv
 # Returns a tuple of the hsv values from ycc.
 ycc.hsl
@@ -150,16 +166,20 @@
 ycc.ycc
 # Returns a tuple of the ycc values from ycc.
 ycc.cmyk
 # Returns a tuple of the cmyk values from ycc.
 ycc.hexidecimal
 # Returns a string of the hexidecimal value from ycc.
 
-hsl.percentForm
+ycc.percentForm
 # Returns a tuple of the ycc values in a decimal percent form (0-1).
+ycc.grayscale
+# Returns a grayscaled version of the YCC class.
+ycc.greyscale
+# Is .grayscale
 ```
 ```py
 cmyk.rgb
 # Returns a tuple of the rgb values from cmyk.
 cmyk.hsv
 # Returns a tuple of the hsv values from cmyk.
 cmyk.hsl
@@ -171,14 +191,18 @@
 cmyk.cmyk
 # Returns a tuple of the cmyk values from cmyk.
 cmyk.hexidecimal
 # Returns a string of the hexidecimal value from cmyk.
 
 cmyk.percentForm
 # Returns a tuple of the cmyk values in a decimal percent form (0-1).
+cmyk.grayscale
+# Returns a grayscaled version of the CMYK class.
+cmyk.greyscale
+# Is .grayscale
 ```
 ```py
 hexidecimal.rgb
 # Returns a tuple of the rgb values from hexidecimal.
 hexidecimal.hsv
 # Returns a tuple of the hsv values from hexidecimal.
 hexidecimal.hsl
@@ -190,14 +214,18 @@
 hexidecimal.cmyk
 # Returns a tuple of the cmyk values from hexidecimal.
 hexidecimal.hexidecimal
 # Returns a string of the hexidecimal value from hexidecimal.
 
 hexidecimal.percentForm
 # Returns a decimal percent form (0-1) of the hexidecimal value.
+hexidecimal.grayscale
+# Returns a grayscaled version of the HEX class.
+hexidecimal.greyscale
+# Is .grayscale
 ```
 ```py
 print(rgb)
 # Will print off a string representation of the rgb values.
 
 print(hsv)
 # Will print off a string representation of the hsv values.
```

### Comparing `idev-pycolor-1.0.1/pyproject.toml` & `idev-pycolor-1.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "idev-pycolor"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Irtsa", email="irtsa.development@gmail.com" },
 ]
 description = "A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `idev-pycolor-1.0.1/setup.cfg` & `idev-pycolor-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 6465 762d 7079 636f 6c6f 720d   = idev-pycolor.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e31  .version = 1.0.1
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e32  .version = 1.0.2
 00000030: 0d0a 6175 7468 6f72 203d 2049 7274 7361  ..author = Irtsa
 00000040: 4465 7665 6c6f 706d 656e 740d 0a61 7574  Development..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6972 7473  hor_email = irts
 00000060: 612e 6465 7665 6c6f 706d 656e 7440 676d  a.development@gm
 00000070: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000080: 7469 6f6e 203d 2041 2070 7974 686f 6e20  tion = A python 
 00000090: 636f 6c6c 6563 7469 6f6e 206f 6620 636c  collection of cl
```

### Comparing `idev-pycolor-1.0.1/setup.py` & `idev-pycolor-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "idev-pycolor",
-    version = "1.0.1",
+    version = "1.0.2",
     author = "IrtsaDevelopment",
     author_email = "irtsa.development@gmail.com",
     description = "A python collection of classes and functions to convert between rgb, hsv, hsl, xyz, ycc, cmyk, and hex color formats and generate palettes from said colors.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/IrtsaDevelopment/PyColor",
     project_urls = {
```

