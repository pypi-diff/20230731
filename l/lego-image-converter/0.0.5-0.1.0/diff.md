# Comparing `tmp/lego_image_converter-0.0.5.tar.gz` & `tmp/lego_image_converter-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lego_image_converter-0.0.5.tar", last modified: Mon Jul 31 01:43:49 2023, max compression
+gzip compressed data, was "lego_image_converter-0.1.0.tar", last modified: Mon Jul 31 02:57:26 2023, max compression
```

## Comparing `lego_image_converter-0.0.5.tar` & `lego_image_converter-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 01:43:49.906211 lego_image_converter-0.0.5/
--rw-r--r--   0 zequnli    (501) staff       (20)     1063 2023-07-30 23:49:22.000000 lego_image_converter-0.0.5/LICENSE
--rw-r--r--   0 zequnli    (501) staff       (20)     2517 2023-07-31 01:43:49.906271 lego_image_converter-0.0.5/PKG-INFO
--rw-r--r--   0 zequnli    (501) staff       (20)     1858 2023-07-31 00:48:36.000000 lego_image_converter-0.0.5/README.md
-drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 01:43:49.905498 lego_image_converter-0.0.5/lego_image_converter/
--rw-r--r--   0 zequnli    (501) staff       (20)     8936 2023-07-31 01:41:38.000000 lego_image_converter-0.0.5/lego_image_converter/__init__.py
--rw-r--r--   0 zequnli    (501) staff       (20)      688 2023-07-30 23:45:16.000000 lego_image_converter-0.0.5/lego_image_converter/config.py
--rw-r--r--   0 zequnli    (501) staff       (20)     1120 2023-07-30 13:48:25.000000 lego_image_converter-0.0.5/lego_image_converter/utility.py
-drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 01:43:49.906079 lego_image_converter-0.0.5/lego_image_converter.egg-info/
--rw-r--r--   0 zequnli    (501) staff       (20)     2517 2023-07-31 01:43:49.000000 lego_image_converter-0.0.5/lego_image_converter.egg-info/PKG-INFO
--rw-r--r--   0 zequnli    (501) staff       (20)      351 2023-07-31 01:43:49.000000 lego_image_converter-0.0.5/lego_image_converter.egg-info/SOURCES.txt
--rw-r--r--   0 zequnli    (501) staff       (20)        1 2023-07-31 01:43:49.000000 lego_image_converter-0.0.5/lego_image_converter.egg-info/dependency_links.txt
--rw-r--r--   0 zequnli    (501) staff       (20)       49 2023-07-31 01:43:49.000000 lego_image_converter-0.0.5/lego_image_converter.egg-info/requires.txt
--rw-r--r--   0 zequnli    (501) staff       (20)       21 2023-07-31 01:43:49.000000 lego_image_converter-0.0.5/lego_image_converter.egg-info/top_level.txt
--rw-r--r--   0 zequnli    (501) staff       (20)       79 2023-07-31 01:43:49.906488 lego_image_converter-0.0.5/setup.cfg
--rw-r--r--   0 zequnli    (501) staff       (20)     1278 2023-07-31 01:43:35.000000 lego_image_converter-0.0.5/setup.py
+drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 02:57:26.415434 lego_image_converter-0.1.0/
+-rw-r--r--   0 zequnli    (501) staff       (20)     1063 2023-07-30 23:49:22.000000 lego_image_converter-0.1.0/LICENSE
+-rw-r--r--   0 zequnli    (501) staff       (20)     4554 2023-07-31 02:57:26.415491 lego_image_converter-0.1.0/PKG-INFO
+-rw-r--r--   0 zequnli    (501) staff       (20)     3905 2023-07-31 02:56:50.000000 lego_image_converter-0.1.0/README.md
+drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 02:57:26.414794 lego_image_converter-0.1.0/lego_image_converter/
+-rw-r--r--   0 zequnli    (501) staff       (20)    10415 2023-07-31 02:56:50.000000 lego_image_converter-0.1.0/lego_image_converter/__init__.py
+-rw-r--r--   0 zequnli    (501) staff       (20)      688 2023-07-30 23:45:16.000000 lego_image_converter-0.1.0/lego_image_converter/config.py
+-rw-r--r--   0 zequnli    (501) staff       (20)     1120 2023-07-30 13:48:25.000000 lego_image_converter-0.1.0/lego_image_converter/utility.py
+drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 02:57:26.415341 lego_image_converter-0.1.0/lego_image_converter.egg-info/
+-rw-r--r--   0 zequnli    (501) staff       (20)     4554 2023-07-31 02:57:26.000000 lego_image_converter-0.1.0/lego_image_converter.egg-info/PKG-INFO
+-rw-r--r--   0 zequnli    (501) staff       (20)      351 2023-07-31 02:57:26.000000 lego_image_converter-0.1.0/lego_image_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)        1 2023-07-31 02:57:26.000000 lego_image_converter-0.1.0/lego_image_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)       49 2023-07-31 02:57:26.000000 lego_image_converter-0.1.0/lego_image_converter.egg-info/requires.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)       21 2023-07-31 02:57:26.000000 lego_image_converter-0.1.0/lego_image_converter.egg-info/top_level.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)       79 2023-07-31 02:57:26.415688 lego_image_converter-0.1.0/setup.cfg
+-rw-r--r--   0 zequnli    (501) staff       (20)      977 2023-07-31 02:53:07.000000 lego_image_converter-0.1.0/setup.py
```

### Comparing `lego_image_converter-0.0.5/LICENSE` & `lego_image_converter-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.0.5/lego_image_converter/__init__.py` & `lego_image_converter-0.1.0/lego_image_converter/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 
 if not os.path.exists('./upload'):
     os.makedirs('./upload')
 
 
 class Converter:
     def __init__(self, set_id='21226', use_only_colors=None, unlimited_blocks=True, verbose=False):
+        """
+        Initializer of the Converter.
+        You need to specify
+            - set_id:str, the name of the Lego set, which defines the color and quantity of usable blocks.
+            - use_only_colors:bool, whether to restrict the color to be used. Useful for clean up the edges.
+            - unlimited_blocks:bool, whether to restrict the number of blocks. Useful for art effects.
+            - verbose:bool, whether to print out the logs.
+        """
         if set_id not in d_config:
             raise Exception('set_id is not found in predefined specs. Please manually add it to d_config in config.py.')
 
         self.verbose = verbose
         self.set_id = set_id
         self.unlimited_blocks = unlimited_blocks
 
@@ -37,14 +45,19 @@
 
         self.image_array_raw = None
         self.image_array_trimmed = None
         self.image_array_filtered = None
         self.image_array_converted = None
 
     def load_image(self, **kwargs):
+        """
+        Load an image to the Converter.
+        If you're loading the image from the Internet via an url, use 'url' param.
+        If you're using a local image, upload it to /upload folder first then use 'filename' param.
+        """
         try:
             self.session_id = str(int(time()))
             os.makedirs(f'./output/{self.session_id}')
             a = get_image_array(**kwargs)
             l, w, _ = a.shape
             if l <= self.config['frame_length'] * 10 or w <= self.config['frame_width'] * 10:
                 print("Warning: Image quality is low, and Mosaic effect may be nontrivial.")
@@ -52,14 +65,15 @@
             if self.verbose:
                 print(f"Image loaded successfully. session_id: {self.session_id}")
         except Exception as e:
             print(e)
         return
 
     def plot_image(self, image_type="raw", save=False, show=False):
+        """Plot images after different procedures."""
         if image_type not in ["raw", "trimmed", "filtered", "converted"]:
             raise Exception("Invalid image_type parameter! Eligible values are raw, trimmed, filtered and converted.")
 
         if image_type == "raw":
             assert self.image_array_raw is not None, 'No raw image is found. Please load an image first.'
             l, w, _ = self.image_array_raw.shape
             fig, ax = plt.subplots(1, 1, figsize=(fig_width, fig_length / w * l))
@@ -67,59 +81,71 @@
             _ = ax.axis('off')
 
             if save:
                 t = str(int(time()))
                 fig.savefig(f'./output/{self.session_id}/{t}_raw.png', dpi=default_dpi)
                 if self.verbose:
                     print(f"Raw image saved to /output/{self.session_id}/{t}_raw.png")
+            if not show:
+                fig.close()
+
         elif image_type == "trimmed":
             assert self.image_array_trimmed is not None, 'No trimmed image is found. Please trim an image first.'
             l, w, _ = self.image_array_trimmed.shape
             fig, ax = plt.subplots(1, 1, figsize=(fig_width, fig_length / w * l))
             _ = ax.imshow(self.image_array_trimmed)
             _ = ax.axis('off')
             if save:
                 t = str(int(time()))
                 fig.savefig(f'./output/{self.session_id}/{t}_trimmed.png', dpi=default_dpi)
                 if self.verbose:
                     print(f"Trimmed image saved to /output/{self.session_id}/{t}_trimmed.png")
+            if not show:
+                fig.close()
+
         elif image_type == "filtered":
             assert self.image_array_filtered is not None, 'No filtered image is found. Please filter an image first.'
             l, w, _ = self.image_array_filtered.shape
             fig, ax = plt.subplots(1, 1, figsize=(fig_width, fig_length / w * l))
             _ = ax.imshow(self.image_array_filtered.astype(np.uint8))
             _ = ax.axis('off')
             if save:
                 t = str(int(time()))
                 fig.savefig(f'./output/{self.session_id}/{t}_filtered.png', dpi=default_dpi)
                 if self.verbose:
                     print(f"Trimmed image saved to /output/{self.session_id}/{t}_filtered.png")
+            if not show:
+                fig.close()
         elif image_type == "converted":
             assert self.image_array_converted is not None, 'No converted image is found. Please convert an image first.'
             l, w, _ = self.image_array_converted.shape
             fig, ax = plt.subplots(1, 1, figsize=(fig_width, fig_length / w * l))
             _ = ax.set_facecolor('k')
-            _ = ax.vlines(x=list(range(w+1)), ymin=0, ymax=l, colors='gray', linewidths=.5)
-            _ = ax.hlines(y=list(range(l+1)), xmin=0, xmax=w, colors='gray', linewidths=.5)
+            _ = ax.vlines(x=list(range(w+1)), ymin=0, ymax=l, colors='gray', linewidths=1)
+            _ = ax.hlines(y=list(range(l+1)), xmin=0, xmax=w, colors='gray', linewidths=1)
             for i in range(l):
                 for j in range(w):
                     c = plt.Circle((w-j-.5, i+.5), .35, color=tuple(self.image_array_converted[l-i-1, w-j-1, :]/255))
                     _ = ax.add_patch(c)
-            _ = ax.set_xlim([0, w+.5])
-            _ = ax.set_ylim([-.5, l])
-            _ = ax.axis('off')
+            _ = ax.set_xlim([0, w])
+            _ = ax.set_ylim([0, l])
+            _ = ax.get_xaxis().set_visible(False)
+            _ = ax.get_yaxis().set_visible(False)
 
             if save:
                 t = str(int(time()))
                 fig.savefig(f'./output/{self.session_id}/{t}_converted.png', dpi=default_dpi)
                 if self.verbose:
                     print(f"Converted image saved to /output/{self.session_id}/{t}_converted.png")
+            if not show:
+                fig.close()
         return
 
     def trim_image(self):
+        """trim the raw image for the Lego frame with very limited capability."""
         assert self.image_array_raw is not None, 'No raw image is found! Please load an image first.'
         l, w, _ = self.image_array_raw.shape
         l_, w_ = self.config['frame_length'], self.config['frame_width']
 
         if l / w > l_ / w_:
             unit = w // w_
             w_new = w_ * unit
@@ -131,14 +157,15 @@
 
         self.image_array_trimmed = self.image_array_raw[-l_new:, :w_new, :]
         if self.verbose:
             print(f"Raw image is trimmed from {l}×{w} to {l_new}×{w_new}, anchoring at lower left corner.")
         return
 
     def filter_image(self):
+        """apply a uniform 2D convolution/filter by taking simple mean values in R/G/B channels."""
         assert self.image_array_trimmed is not None, "No trimmed image is found! Please trim an image first."
         self.image_array_filtered = np.zeros([
             self.config['frame_length']
             , self.config['frame_width']
             , 3
         ])
         l, w, _ = self.image_array_trimmed.shape
@@ -154,14 +181,16 @@
                 ).astype(int)
 
         if self.verbose:
             print(f"Trimmed image is filtered from {l}×{w} to {l_}×{w_}.")
         return
 
     def convert_image(self):
+        """convert the filtered image into a similar and eligible color from
+        the Lego set using a nonlinear deltaE metric and a simple heap sort algorithm."""
         assert self.image_array_filtered is not None, "No filtered image is found! Please filter an image first."
         self.image_array_converted = np.zeros_like(self.image_array_filtered)
         l, w, _ = self.image_array_filtered.shape
         colors = list(self.config['n_blocks'].keys())
         d_image = {(i, j): {'is_matched': False} for i in range(l) for j in range(w)}
         d_blocks = {c: {'n': self.config['n_blocks'][c], 'heap': []} for c in colors}
 
@@ -194,11 +223,12 @@
             n_matched_blocks -= 1
 
         if self.verbose:
             print(f"Filtered image has been matched to a set of Lego blocks.")
         return
 
     def process_image(self):
+        """the meta function of all processing procedures after loading an image."""
         self.trim_image()
         self.filter_image()
         self.convert_image()
         return
```

### Comparing `lego_image_converter-0.0.5/lego_image_converter/config.py` & `lego_image_converter-0.1.0/lego_image_converter/config.py`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.0.5/lego_image_converter/utility.py` & `lego_image_converter-0.1.0/lego_image_converter/utility.py`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.0.5/setup.py` & `lego_image_converter-0.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name='lego_image_converter',  # should match the package folder
-    packages=['lego_image_converter'],  # should match the package folder
-    version='0.0.5',  # important for updates
-    license='MIT',  # should match your chosen license
-    description='Testing installation of Package 3',
-    long_description=long_description,  # loads your README.md
-    long_description_content_type="text/markdown",  # README.md is of type 'markdown'
+    name='lego_image_converter',
+    packages=['lego_image_converter'],
+    version='0.1.0',
+    license='MIT',
+    description='First formal release',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     author='Zequn Li',
     author_email='zequn1992@gmail.com',
-    url='https://github.com/mike-huls/toolbox_public',
-    install_requires=['requests', 'numpy', 'matplotlib', 'pillow', 'basic_colormath'],  # list all packages that your package uses
-    keywords=["pypi", "lego_image_converter", "Lego", "image", "8bit", "art"],  # descriptive meta-data
-    classifiers=[  # https://pypi.org/classifiers
+    url='https://github.com/zl3311/lego_image_converter',
+    install_requires=['requests', 'numpy', 'matplotlib', 'pillow', 'basic_colormath'],
+    keywords=["pypi", "lego_image_converter", "lego", "image", "8bit", "art"],
+    classifiers=[
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Documentation',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
 
-    download_url="https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.0.5.tar.gz",
+    download_url="https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.1.0.tar.gz",
 )
```

