# Comparing `tmp/excolor-0.0.2.tar.gz` & `tmp/excolor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excolor-0.0.2.tar", last modified: Tue Jul 25 13:41:40 2023, max compression
+gzip compressed data, was "excolor-0.0.3.tar", last modified: Mon Jul 31 17:56:13 2023, max compression
```

## Comparing `excolor-0.0.2.tar` & `excolor-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-25 13:41:40.920121 excolor-0.0.2/
--rw-r--r--   0 timpyrkov   (501) staff       (20)     1067 2023-07-15 06:34:27.000000 excolor-0.0.2/LICENSE
--rw-r--r--   0 timpyrkov   (501) staff       (20)     3068 2023-07-25 13:41:40.919948 excolor-0.0.2/PKG-INFO
--rw-r--r--   0 timpyrkov   (501) staff       (20)     2633 2023-07-18 11:05:42.000000 excolor-0.0.2/README.md
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-25 13:41:40.918769 excolor-0.0.2/excolor/
--rw-r--r--   0 timpyrkov   (501) staff       (20)      350 2023-07-25 04:09:40.000000 excolor-0.0.2/excolor/__init__.py
--rwxr--r--   0 timpyrkov   (501) staff       (20)    11406 2023-07-25 13:28:40.000000 excolor-0.0.2/excolor/background.py
--rwxr--r--   0 timpyrkov   (501) staff       (20)    12593 2023-07-24 17:19:21.000000 excolor-0.0.2/excolor/excolor.py
--rwxr--r--   0 timpyrkov   (501) staff       (20)     2663 2023-07-25 12:27:34.000000 excolor-0.0.2/excolor/geometry.py
--rw-r--r--   0 timpyrkov   (501) staff       (20)     9085 2023-07-25 13:39:43.000000 excolor-0.0.2/excolor/imagetools.py
--rwxr--r--   0 timpyrkov   (501) staff       (20)     9461 2023-07-25 04:17:01.000000 excolor-0.0.2/excolor/utils.py
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-25 13:41:40.919723 excolor-0.0.2/excolor.egg-info/
--rw-r--r--   0 timpyrkov   (501) staff       (20)     3068 2023-07-25 13:41:40.000000 excolor-0.0.2/excolor.egg-info/PKG-INFO
--rw-r--r--   0 timpyrkov   (501) staff       (20)      300 2023-07-25 13:41:40.000000 excolor-0.0.2/excolor.egg-info/SOURCES.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)        1 2023-07-25 13:41:40.000000 excolor-0.0.2/excolor.egg-info/dependency_links.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)       61 2023-07-25 13:41:40.000000 excolor-0.0.2/excolor.egg-info/requires.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)        8 2023-07-25 13:41:40.000000 excolor-0.0.2/excolor.egg-info/top_level.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)       38 2023-07-25 13:41:40.920172 excolor-0.0.2/setup.cfg
--rw-r--r--   0 timpyrkov   (501) staff       (20)      899 2023-07-25 13:20:04.000000 excolor-0.0.2/setup.py
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-31 17:56:13.230465 excolor-0.0.3/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     1067 2023-07-15 06:34:27.000000 excolor-0.0.3/LICENSE
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     3435 2023-07-31 17:56:13.230261 excolor-0.0.3/PKG-INFO
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     2981 2023-07-31 17:52:37.000000 excolor-0.0.3/README.md
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-31 17:56:13.229477 excolor-0.0.3/excolor/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      350 2023-07-25 04:09:40.000000 excolor-0.0.3/excolor/__init__.py
+-rwxr--r--   0 timpyrkov   (501) staff       (20)    12071 2023-07-25 21:36:31.000000 excolor-0.0.3/excolor/background.py
+-rwxr--r--   0 timpyrkov   (501) staff       (20)    12726 2023-07-25 19:44:55.000000 excolor-0.0.3/excolor/excolor.py
+-rwxr--r--   0 timpyrkov   (501) staff       (20)     2663 2023-07-25 12:27:34.000000 excolor-0.0.3/excolor/geometry.py
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     9404 2023-07-25 20:36:54.000000 excolor-0.0.3/excolor/imagetools.py
+-rwxr--r--   0 timpyrkov   (501) staff       (20)     9461 2023-07-25 04:17:01.000000 excolor-0.0.3/excolor/utils.py
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-31 17:56:13.230098 excolor-0.0.3/excolor.egg-info/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     3435 2023-07-31 17:56:12.000000 excolor-0.0.3/excolor.egg-info/PKG-INFO
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      300 2023-07-31 17:56:13.000000 excolor-0.0.3/excolor.egg-info/SOURCES.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)        1 2023-07-31 17:56:12.000000 excolor-0.0.3/excolor.egg-info/dependency_links.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)       61 2023-07-31 17:56:13.000000 excolor-0.0.3/excolor.egg-info/requires.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)        8 2023-07-31 17:56:13.000000 excolor-0.0.3/excolor.egg-info/top_level.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)       38 2023-07-31 17:56:13.230546 excolor-0.0.3/setup.cfg
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      899 2023-07-31 17:54:34.000000 excolor-0.0.3/setup.py
```

### Comparing `excolor-0.0.2/LICENSE` & `excolor-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `excolor-0.0.2/README.md` & `excolor-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: excolor
+Version: 0.0.3
+Summary: Extended colors for python
+Home-page: https://github.com/timpyrkov/excolor
+Author: Tim Pyrkov
+Author-email: tim.pyrkov@gmail.com
+License: MIT License
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Artistic Software
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Python Versions](https://img.shields.io/pypi/pyversions/excolor?style=plastic)](https://pypi.org/project/excolor/)
 [![PyPI](https://img.shields.io/pypi/v/excolor?style=plastic)](https://pypi.org/project/excolor/)
 [![License](https://img.shields.io/pypi/l/excolor?style=plastic)](https://opensource.org/licenses/MIT)
 [![Documentation Status](https://readthedocs.org/projects/excolor/badge/?version=latest)](https://excolor.readthedocs.io/en/latest/?badge=latest)
 
 # excolors
 
@@ -19,15 +35,15 @@
 ```
 import excolor
 
 cmap = plt.get_cmap("gruvbox")
 cmap
 ```
 
-![](img/colormap.png)
+![](https://github.com/timpyrkov/excolor/blob/master/img/colormap.png?raw=true)
 
 # Colorize black-and-white image
 
 - Hue and saturation cannot colorize black-and-white image. They only change pixels where levels of red, gree, blue are not the same. 
 
 - Colorize() function takes a greyscale or b&w image and adds colors to dark and light areas.
 
@@ -47,17 +63,17 @@
 plt.figure(figsize=(2,2), facecolor="#00000000")
 plt.imshow(img)
 plt.axis("off")
 plt.show()
 
 ```
 
-![](img/pacman.png)
-![](img/arrow.png)
-![](img/colorized.png)
+![](https://github.com/timpyrkov/excolor/blob/master/img/pacman.png?raw=true)
+![](https://github.com/timpyrkov/excolor/blob/master/img/arrow.png?raw=true)
+![](https://github.com/timpyrkov/excolor/blob/master/img/colorized.png?raw=true)
 
 # Color cycler
 
 Set ax color cycler based on cmap or list of colors
 
 ```
 from sklearn.metrics import confusion_matrix
@@ -87,15 +103,15 @@
     plt.scatter(x0[mask], x1[mask])
 plt.tight_layout()
 plt.show()
 
 
 ```
 
-![](img/charts.png)
+![](https://github.com/timpyrkov/excolor/blob/master/img/charts.png?raw=true)
 
 # Log-scaling colormaps
 
 Color perlin noise using log-scaled colormap to visualize water caustics
 
 ```
 from pythonperlin import perlin
@@ -109,12 +125,13 @@
 
 plt.figure(figsize=(6,6), facecolor="#00000000")
 plt.imshow( np.abs(x), cmap=cmap)
 plt.axis("off")
 plt.show()
 ```
 
-![](img/caustics.png)
+![](https://github.com/timpyrkov/excolor/blob/master/img/caustics.png?raw=true)
 
 # Documentation
 
-[https://excolor.readthedocs.io](https://excolor.readthedocs.io)
+[https://excolor.readthedocs.io](https://excolor.readthedocs.io)
+
```

### Comparing `excolor-0.0.2/excolor/background.py` & `excolor-0.0.3/excolor/background.py`

 * *Files 6% similar despite different names*

```diff
@@ -241,61 +241,69 @@
         plt.figure(facecolor="#00000000")
         plt.imshow(img)
         plt.gca().set_axis_off()
         plt.show()
     return img
 
 
-def background_concentric_lines(colors, background, fname=None, size=(16,9), dpi=80, center=(2,-2), seed=0, nrep=4):
+def background_concentric_lines(colors, background, fname=None, size=(1280,720), dpi=80, center=(0,0), seed=0, nrep=4):
     """
     Draws background with distorted concentric lines
 
     Parameters
     ----------
     colors : list
         List of colors
-    background : str or matplotlib.colors.Colormap
-        Background color
+    background : str, matplotlib.colors.Color or image
+        Background color or image
     fname : str or None, default None
         If fname given - saves image to file
-    size : tuple, default (16, 9)
-        Size of output background image [inches]
+    size : tuple, default (1280,720)
+        Size of output background image [pixels]
     dpi: int, default 80
         Resolution [dpi]
-    center : tuple, default (2, -2)
+    center : tuple, default (0,0)
         Coordinates of circle center from the right bottom corner [inches]
     seed : int, default 0
         Random seed for generation of distorting Perlin noise
     nreps : int, default 4
         Number of repeats for colorcycle
 
     Returns
     -------
     fig : matplotlib.figure.Figure
         Backgraound image
 
     """
     n_major = nrep
     n_minor = len(colors)
-    x_max = size[0] + center[0]
-    y_max = size[1] - center[1]
-    r_max = np.sqrt(x_max**2 + y_max**2) + .5
-    r_min = 2 * r_max / 3
+    x_max = size[0] + dpi * center[0]
+    y_max = size[1] - dpi * center[1]
+    r_max = np.sqrt(x_max**2 + y_max**2)
+    r_min = 0.6 * r_max
     dr_major = (r_max - r_min) / n_major
     dr_minor = dr_major / (n_minor + 1)
     dens = 20
     n = np.ceil(n_major * n_minor / dens).astype(int) + 1
     p = perlin((n,36), dens=dens, seed=seed)[dens//2:]
-    fig = plt.figure(figsize=size, facecolor=background)
+    inch_size = (size[0] / dpi, size[1] / dpi)
+    try:
+        bgcolor = mc.to_rgb(background)
+        fig = plt.figure(figsize=inch_size, facecolor=bgcolor)
+    except:
+        fig = plt.figure(figsize=inch_size, facecolor="#00000000")
+        img = image_to_array(background)
+        plt.imshow(img[::-1])
+    fig.set_dpi(dpi)
     for i in range(n_major):
         for j in range(n_minor):
             k = n_minor * i + j
             r = r_min + dr_major * i + dr_minor * j
             x, y = get_circle_dots(r, n=720)
-            x, y = distort_radius(x, y, 2 * p[k])
+            x, y = distort_radius(x, y, 2 * dpi * p[k])
             x += size[0] + center[0]
             y += center[1]
             lw = n_minor + 2 - 1 * (j % n_minor)
             plt.plot(x, y, lw=lw, color = colors[j])
     plt.xlim(0, size[0])
     plt.ylim(0, size[1])
     remove_margins()
@@ -306,78 +314,88 @@
     else:
         plt.show()
     return fig
 
 
     
 
-def background_concentric_patches(colors, bgcolor, fname=None, size=(16,9), dpi=80, center=(2,-2), seed=0):
+def background_concentric_patches(colors, background, fname=None, size=(1280,720), dpi=80, center=(0,0), seed=0):
     """
     Draws background with distorted concentric patches
 
     Parameters
     ----------
     colors : list
         List of colors
-    background : str or matplotlib.colors.Colormap
-        Background color
+    background : str, matplotlib.colors.Color or image
+        Background color or image
     fname : str or None, default None
         If fname given - saves image to file
-    size : tuple, default (16, 9)
-        Size of output background image [inches]
+    size : tuple, default (1280,720)
+        Size of output background image [pixels]
     dpi: int, default 80
         Resolution [dpi]
-    center : tuple, default (2, -2)
+    center : tuple, default (0,0)
         Coordinates of circle center from the right bottom corner [inches]
     seed : int, default 0
         Random seed for generation of distorting Perlin noise
 
     Returns
     -------
     fig : matplotlib.figure.Figure
         Backgraound image
 
     """
-    def _draw_patch(x, y, size, color):
-        mask = (x > -1) & (x < size[0] + 1) & (y > -1) & (y < size[1] + 1)
-        x, y = x[mask], y[mask]
-        x = np.concatenate([x, np.array([-1, -1, x[0], x[0]])])
-        y = np.concatenate([y, np.array([-1, size[1]+1,size[1]+1, y[0]])])
-        fig = plt.figure(figsize=size, facecolor="#00000000")
+    def _draw_patch(x, y, size, color, dpi):
+        inch_size = (size[0] / dpi, size[1] / dpi)
+        dx = np.array([size[0] + dpi, -dpi, -dpi, size[0] + dpi])
+        dy = np.array([-dpi, -dpi, size[1] + dpi, size[1] + dpi])
+        x = np.concatenate([x, dx])
+        y = np.concatenate([y, dy])
+        fig = plt.figure(figsize=inch_size, facecolor="#00000000")
+        fig.set_dpi(dpi)
         plt.fill(x, y, c=color)
         plt.xlim(0, size[0])
         plt.ylim(0, size[1])
         remove_margins()
         x = add_shadow(fig, kernel=(301,301), sigma=100, color="#000000")
         plt.close()
         return x
     n_major = len(colors)
-    x_max = size[0] + center[0]
-    y_max = size[1] - center[1]
-    r_max = np.sqrt(x_max**2 + y_max**2) + .5
-    r_min = 2 * r_max / 3
+    x_max = size[0] + dpi * center[0]
+    y_max = size[1] - dpi * center[1]
+    r_max = np.sqrt(x_max**2 + y_max**2)
+    r_min = 0.6 * r_max
     dr_major = (r_max - r_min) / n_major
     dens = 20
     n = np.ceil(n_major * 6 / dens).astype(int) + 1
     p = perlin((n,36), dens=dens, seed=seed)[dens//2:]
+    inch_size = (size[0] / dpi, size[1] / dpi)
     layers = []
     for i in range(n_major):
         k = 8 * i
         r = r_min + dr_major * i
         x, y = get_circle_dots(r, n=720)
-        x, y = distort_radius(x, y, 2 * p[k])
+        x, y = distort_radius(x, y, 2 * dpi * p[k])
         x += size[0] + center[0]
         y += center[1]
-        x = _draw_patch(x, y, size, colors[i])
+        x = _draw_patch(x, y, size, colors[i], dpi)
         layers.append(x)
-    plt.figure(figsize=size, facecolor=bgcolor)
+    try:
+        bgcolor = mc.to_rgb(background)
+        fig = plt.figure(figsize=inch_size, facecolor=bgcolor)
+    except:
+        fig = plt.figure(figsize=inch_size, facecolor="#00000000")
+        img = image_to_array(background)
+        plt.imshow(img[::-1])
+    fig.set_dpi(dpi)
     for layer in layers:
-        plt.imshow(layer)
-    # plt.xlim(0, size[0])
-    # plt.ylim(0, size[1])
+        plt.imshow(layer[::-1])
+    plt.xlim(0, size[0])
+    plt.ylim(0, size[1])
     remove_margins()
     if fname is not None:
         if len(fname) < 5 or fname[-4:] not in [".png", ".jpg", ".svg"]:
             fname = f"{fname}.png"
         plt.savefig(fname, dpi=dpi)
     else:
         plt.show()
```

### Comparing `excolor-0.0.2/excolor/excolor.py` & `excolor-0.0.3/excolor/excolor.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,34 +86,38 @@
     plt.yticks([])
     for e in ["top", "bottom", "right", "left"]:
         plt.gca().spines[e].set_color("#00000000")
     plt.tight_layout()
     return
 
 
-def show_colors(c, title="", cname=None):
+def show_colors(c, title="", cname=None, verbose=True):
     """
     Plots colors from list or a colormap
 
     Parameters
     ----------
     c : list, str, or matplotlib.colors.Colormap object
         List of colors or a colormap
-    title : str, optional
+    title : str, default ''
         Figure title
-    cname : list, optional
+    cname : list or None, default None
         List of color names
+    verbose : bool, default True
+        Flag to print color names
 
     """
     try:
         c = plt.get_cmap(c)
         colors = get_colors(c, exclude_extreme=False)
         title = c.name
     except:
         colors = c if _is_arraylike(c) else [c]
+    if verbose:
+        print(colors)
     d = 0.05
     width = 1  -2 * d
     n, m = aspect_ratio(len(colors), lmin=12)
     plt.figure(figsize=(2*n+4,2*m), facecolor="#00000000")
     plt.title(title, fontsize=20, color="grey")
     for k, color in enumerate(colors):
         i = k % n
```

### Comparing `excolor-0.0.2/excolor/geometry.py` & `excolor-0.0.3/excolor/geometry.py`

 * *Files identical despite different names*

### Comparing `excolor-0.0.2/excolor/imagetools.py` & `excolor-0.0.3/excolor/imagetools.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,33 +57,36 @@
     plt.figure(figsize=figsize, facecolor="#00000000")
     plt.imshow(image)
     remove_margins()
     plt.show()
     return
 
 
-def image_to_array(image):
+def image_to_array(image, dpi=72):
     """
     Converts image to numpy array
 
     Parameters
     ----------
-    image : str or PIL.PngImagePlugin.PngImageFile or matplotlib.figure.Figure
+    image : str, ndarray, PIL.PngImagePlugin.PngImageFile or matplotlib.figure.Figure
         Figure, image or image path or url
+    dpi : int, default 72
+        Image resolution [dpi]; only apllies to matplotlib.figure.Figure
 
     Returns
     -------
     x : ndarray
         Numpy array of size (height, width) or (height, width, nchannels)
         Data type: uint8, 0-255
 
     """
     if isinstance(image, str):
         image = load_image(image)
     try:
+        image.set_dpi(dpi)
         image.canvas.draw()
         x = np.asarray(image.canvas.renderer._renderer)
     except:
         x = np.asarray(image)
     return x
 
 
@@ -163,38 +166,40 @@
             imax = np.unique(imax)
             i = np.argmax(np.diff(imax))
             peaks = np.array([imax[i], imax[i+1]])
             break
     return peaks
 
 
-def get_mask(image, midpoint=None, grad_range=None, uint8=False):
+def get_mask(image, midpoint=None, grad_range=None, dpi=72, uint8=False):
     """
     Converts image to a mask
 
     Parameters
     ----------
-    image : ndarray
+    image : str, ndarray, PIL.PngImagePlugin.PngImageFile or matplotlib.figure.Figure
         1D array of data
     midpoint : float or None, default None
         Midpoint between dark and light areas in range (0,1)
     grad_range : float or None, default None
         Gradient range between dark and light
+    dpi : int, default 72
+        Image resolution [dpi]; only apllies to matplotlib.figure.Figure
     uint8 : bool, default False
         Flag to cast data to np.uint8 to save disk space.
 
     Returns
     -------
     mask : ndarray
         float: 1.0 - object, 0.0 - background, or
         uint8: 255 - object, 0 - background
 
     """
     # Read image and convert to numpy array
-    x = image_to_array(image)
+    x = image_to_array(image, dpi)
     # Skip if image is already a mask
     if x.max() <= 1 + 1e-5:
         mask = x
     else:
         # Convert 255 to 1.0
         x = x.astype(float) / 255 if x.max() > 1 else x
```

### Comparing `excolor-0.0.2/excolor/utils.py` & `excolor-0.0.3/excolor/utils.py`

 * *Files identical despite different names*

### Comparing `excolor-0.0.2/setup.py` & `excolor-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name="excolor",
-    version="0.0.2",
+    version="0.0.3",
     author="Tim Pyrkov",
     author_email="tim.pyrkov@gmail.com",
     description="Extended colors for python",
     long_description=read("README.md"),
     license = "MIT License",
     long_description_content_type="text/markdown",
     url="https://github.com/timpyrkov/excolor",
```

