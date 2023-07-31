# Comparing `tmp/pythonperlin-0.0.7.tar.gz` & `tmp/pythonperlin-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonperlin-0.0.7.tar", last modified: Tue Jul 25 15:49:33 2023, max compression
+gzip compressed data, was "pythonperlin-0.0.8.tar", last modified: Mon Jul 31 18:06:43 2023, max compression
```

## Comparing `pythonperlin-0.0.7.tar` & `pythonperlin-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-25 15:49:33.660013 pythonperlin-0.0.7/
--rw-r--r--   0 timpyrkov   (501) staff       (20)     1067 2022-11-01 23:50:58.000000 pythonperlin-0.0.7/LICENSE
--rw-r--r--   0 timpyrkov   (501) staff       (20)     5144 2023-07-25 15:49:33.659854 pythonperlin-0.0.7/PKG-INFO
--rw-r--r--   0 timpyrkov   (501) staff       (20)     4648 2023-07-10 14:34:06.000000 pythonperlin-0.0.7/README.md
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-25 15:49:33.658601 pythonperlin-0.0.7/pythonperlin/
--rw-r--r--   0 timpyrkov   (501) staff       (20)      172 2023-07-11 14:05:32.000000 pythonperlin-0.0.7/pythonperlin/__init__.py
--rw-r--r--   0 timpyrkov   (501) staff       (20)     8488 2023-07-25 15:46:10.000000 pythonperlin-0.0.7/pythonperlin/perlin.py
-drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-25 15:49:33.659622 pythonperlin-0.0.7/pythonperlin.egg-info/
--rw-r--r--   0 timpyrkov   (501) staff       (20)     5144 2023-07-25 15:49:33.000000 pythonperlin-0.0.7/pythonperlin.egg-info/PKG-INFO
--rw-r--r--   0 timpyrkov   (501) staff       (20)      253 2023-07-25 15:49:33.000000 pythonperlin-0.0.7/pythonperlin.egg-info/SOURCES.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)        1 2023-07-25 15:49:33.000000 pythonperlin-0.0.7/pythonperlin.egg-info/dependency_links.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)        6 2023-07-25 15:49:33.000000 pythonperlin-0.0.7/pythonperlin.egg-info/requires.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)       13 2023-07-25 15:49:33.000000 pythonperlin-0.0.7/pythonperlin.egg-info/top_level.txt
--rw-r--r--   0 timpyrkov   (501) staff       (20)       38 2023-07-25 15:49:33.660071 pythonperlin-0.0.7/setup.cfg
--rw-r--r--   0 timpyrkov   (501) staff       (20)      832 2023-07-25 15:46:36.000000 pythonperlin-0.0.7/setup.py
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-31 18:06:43.085443 pythonperlin-0.0.8/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     1067 2022-11-01 23:50:58.000000 pythonperlin-0.0.8/LICENSE
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     5639 2023-07-31 18:06:43.085316 pythonperlin-0.0.8/PKG-INFO
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     5143 2023-07-31 18:05:14.000000 pythonperlin-0.0.8/README.md
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-31 18:06:43.084301 pythonperlin-0.0.8/pythonperlin/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      172 2023-07-11 14:05:32.000000 pythonperlin-0.0.8/pythonperlin/__init__.py
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     8488 2023-07-25 15:46:10.000000 pythonperlin-0.0.8/pythonperlin/perlin.py
+drwxr-xr-x   0 timpyrkov   (501) staff       (20)        0 2023-07-31 18:06:43.085143 pythonperlin-0.0.8/pythonperlin.egg-info/
+-rw-r--r--   0 timpyrkov   (501) staff       (20)     5639 2023-07-31 18:06:42.000000 pythonperlin-0.0.8/pythonperlin.egg-info/PKG-INFO
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      253 2023-07-31 18:06:42.000000 pythonperlin-0.0.8/pythonperlin.egg-info/SOURCES.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)        1 2023-07-31 18:06:42.000000 pythonperlin-0.0.8/pythonperlin.egg-info/dependency_links.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)        6 2023-07-31 18:06:42.000000 pythonperlin-0.0.8/pythonperlin.egg-info/requires.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)       13 2023-07-31 18:06:42.000000 pythonperlin-0.0.8/pythonperlin.egg-info/top_level.txt
+-rw-r--r--   0 timpyrkov   (501) staff       (20)       38 2023-07-31 18:06:43.085482 pythonperlin-0.0.8/setup.cfg
+-rw-r--r--   0 timpyrkov   (501) staff       (20)      832 2023-07-31 18:06:12.000000 pythonperlin-0.0.8/setup.py
```

### Comparing `pythonperlin-0.0.7/LICENSE` & `pythonperlin-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonperlin-0.0.7/PKG-INFO` & `pythonperlin-0.0.8/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonperlin
-Version: 0.0.7
+Version: 0.0.8
 Summary: Perlin noise in python - seamlessly tile in any dimensions
 Home-page: https://github.com/timpyrkov/pythonperlin
 Author: Tim Pyrkov
 Author-email: tim.pyrkov@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -56,15 +56,15 @@
 x = np.concatenate([x] * 2, axis=1)
 
 plt.figure(figsize=(12,6))
 plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 ```
-![](media/img_tile.png)
+![](https://github.com/timpyrkov/pythonperlin/blob/master/media/img_tile.png?raw=true)
 
 
 # Generate domain warping
 
 Add noise to grid coordinates and generate noise again
 ```
 dens = 32
@@ -72,15 +72,15 @@
 x = perlin(shape, dens=dens, seed=0, warp=2)
 
 plt.figure(figsize=(6,6))
 plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 ```
-![](media/img_warp.png)
+![](https://github.com/timpyrkov/pythonperlin/blob/master/media/img_warp.png?raw=true)
 
 
 # Generate octaves
 ```
 import pylab as plt
 from pythonperlin import perlin
 
@@ -102,15 +102,16 @@
 x = perlin(shape, dens=dens, seed=0, octaves=4)
 
 plt.figure(figsize=(6,6))
 plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 ```
-![](media/img_no_octaves.png) ![](media/img_with_octaves.png)
+![](https://github.com/timpyrkov/pythonperlin/blob/master/media/img_no_octaves.png?raw=true)
+![](https://github.com/timpyrkov/pythonperlin/blob/master/media/img_with_octaves.png?raw=true)
 
 
 # Generate water caustics
 
 Take absolute value of Perlin noise and apply log-scaled color gradient
 ```
 import numpy as np
@@ -129,15 +130,15 @@
 cmap = LinearSegmentedColormap.from_list('caustics', colors)
 
 plt.figure(figsize=(6,6))
 plt.imshow(x, cmap=cmap)
 plt.axis('off')
 plt.show()
 ```
-![](media/img_caustics.png)
+![](https://github.com/timpyrkov/pythonperlin/blob/master/media/img_caustics.png?raw=true)
 
 
 # Generate flower petals
 
 Take 1D Perlin noise as the varying radius along a circle
 ```
 dens = 32
@@ -157,15 +158,15 @@
     ax = plt.gca()
     zorder = max([ch.zorder for ch in ax.get_children()])
     plt.fill(z.real, z.imag, c=color[2*i], zorder=zorder+1)
     plt.plot(z.real, z.imag, c=color[2*i+1], lw=2, zorder=zorder+2)
 plt.axis('off')
 plt.show()
 ```
-![](media/img_flower.png)
+![](https://github.com/timpyrkov/pythonperlin/blob/master/media/img_flower.png?raw=true)
 
 
 # Generate vector field
 
 Take Perlin noise as the vector angle at each point of a grid
 ```
 dens = 6
@@ -181,15 +182,15 @@
         di = 0.5 * z[i,j].real
         dj = 0.5 * z[i,j].imag
         color = colors[(di > 0) + 2 * (dj > 0)]
         plt.arrow(i, j, di, dj, color=color, width=0.1)
 plt.axis('off')
 plt.show()
 ```
-![](media/img_vectors.png)
+![](https://github.com/timpyrkov/pythonperlin/blob/master/media/img_vectors.png?raw=true)
 
 
 # Sound of Perlin noise
 
 Perlin noise sounds nice and less buzzing than white noise
 ```
 import sounddevice as sd
@@ -205,14 +206,14 @@
 ```
 import IPython
 import soundfile as sf
 
 sf.write('perlin.wav', x, 22050)
 IPython.display.Audio('perlin.wav')
 ```
-![perlin.wav](media/perlin.wav)
+![perlin.wav](https://github.com/timpyrkov/pythonperlin/blob/master/media/perlin.wav)
 
 
 # Documentation
 
 [https://pythonperlin.readthedocs.io](https://pythonperlin.readthedocs.io)
```

### Comparing `pythonperlin-0.0.7/pythonperlin/perlin.py` & `pythonperlin-0.0.8/pythonperlin/perlin.py`

 * *Files identical despite different names*

### Comparing `pythonperlin-0.0.7/pythonperlin.egg-info/PKG-INFO` & `pythonperlin-0.0.8/pythonperlin.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonperlin
-Version: 0.0.7
+Version: 0.0.8
 Summary: Perlin noise in python - seamlessly tile in any dimensions
 Home-page: https://github.com/timpyrkov/pythonperlin
 Author: Tim Pyrkov
 Author-email: tim.pyrkov@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -56,15 +56,15 @@
 x = np.concatenate([x] * 2, axis=1)
 
 plt.figure(figsize=(12,6))
 plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 ```
-![](media/img_tile.png)
+![](https://github.com/timpyrkov/pythonperlin/blob/master/media/img_tile.png?raw=true)
 
 
 # Generate domain warping
 
 Add noise to grid coordinates and generate noise again
 ```
 dens = 32
@@ -72,15 +72,15 @@
 x = perlin(shape, dens=dens, seed=0, warp=2)
 
 plt.figure(figsize=(6,6))
 plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 ```
-![](media/img_warp.png)
+![](https://github.com/timpyrkov/pythonperlin/blob/master/media/img_warp.png?raw=true)
 
 
 # Generate octaves
 ```
 import pylab as plt
 from pythonperlin import perlin
 
@@ -102,15 +102,16 @@
 x = perlin(shape, dens=dens, seed=0, octaves=4)
 
 plt.figure(figsize=(6,6))
 plt.imshow(x, cmap=plt.get_cmap('Accent_r'))
 plt.axis('off')
 plt.show()
 ```
-![](media/img_no_octaves.png) ![](media/img_with_octaves.png)
+![](https://github.com/timpyrkov/pythonperlin/blob/master/media/img_no_octaves.png?raw=true)
+![](https://github.com/timpyrkov/pythonperlin/blob/master/media/img_with_octaves.png?raw=true)
 
 
 # Generate water caustics
 
 Take absolute value of Perlin noise and apply log-scaled color gradient
 ```
 import numpy as np
@@ -129,15 +130,15 @@
 cmap = LinearSegmentedColormap.from_list('caustics', colors)
 
 plt.figure(figsize=(6,6))
 plt.imshow(x, cmap=cmap)
 plt.axis('off')
 plt.show()
 ```
-![](media/img_caustics.png)
+![](https://github.com/timpyrkov/pythonperlin/blob/master/media/img_caustics.png?raw=true)
 
 
 # Generate flower petals
 
 Take 1D Perlin noise as the varying radius along a circle
 ```
 dens = 32
@@ -157,15 +158,15 @@
     ax = plt.gca()
     zorder = max([ch.zorder for ch in ax.get_children()])
     plt.fill(z.real, z.imag, c=color[2*i], zorder=zorder+1)
     plt.plot(z.real, z.imag, c=color[2*i+1], lw=2, zorder=zorder+2)
 plt.axis('off')
 plt.show()
 ```
-![](media/img_flower.png)
+![](https://github.com/timpyrkov/pythonperlin/blob/master/media/img_flower.png?raw=true)
 
 
 # Generate vector field
 
 Take Perlin noise as the vector angle at each point of a grid
 ```
 dens = 6
@@ -181,15 +182,15 @@
         di = 0.5 * z[i,j].real
         dj = 0.5 * z[i,j].imag
         color = colors[(di > 0) + 2 * (dj > 0)]
         plt.arrow(i, j, di, dj, color=color, width=0.1)
 plt.axis('off')
 plt.show()
 ```
-![](media/img_vectors.png)
+![](https://github.com/timpyrkov/pythonperlin/blob/master/media/img_vectors.png?raw=true)
 
 
 # Sound of Perlin noise
 
 Perlin noise sounds nice and less buzzing than white noise
 ```
 import sounddevice as sd
@@ -205,14 +206,14 @@
 ```
 import IPython
 import soundfile as sf
 
 sf.write('perlin.wav', x, 22050)
 IPython.display.Audio('perlin.wav')
 ```
-![perlin.wav](media/perlin.wav)
+![perlin.wav](https://github.com/timpyrkov/pythonperlin/blob/master/media/perlin.wav)
 
 
 # Documentation
 
 [https://pythonperlin.readthedocs.io](https://pythonperlin.readthedocs.io)
```

### Comparing `pythonperlin-0.0.7/setup.py` & `pythonperlin-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name="pythonperlin",
-    version="0.0.7",
+    version="0.0.8",
     author="Tim Pyrkov",
     author_email="tim.pyrkov@gmail.com",
     description="Perlin noise in python - seamlessly tile in any dimensions",
     long_description=read("README.md"),
     license = "MIT License",
     long_description_content_type="text/markdown",
     url="https://github.com/timpyrkov/pythonperlin",
```

