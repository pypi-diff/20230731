# Comparing `tmp/lego_image_converter-0.1.0.tar.gz` & `tmp/lego_image_converter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lego_image_converter-0.1.0.tar", last modified: Mon Jul 31 02:57:26 2023, max compression
+gzip compressed data, was "lego_image_converter-0.1.1.tar", last modified: Mon Jul 31 03:05:54 2023, max compression
```

## Comparing `lego_image_converter-0.1.0.tar` & `lego_image_converter-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 02:57:26.415434 lego_image_converter-0.1.0/
--rw-r--r--   0 zequnli    (501) staff       (20)     1063 2023-07-30 23:49:22.000000 lego_image_converter-0.1.0/LICENSE
--rw-r--r--   0 zequnli    (501) staff       (20)     4554 2023-07-31 02:57:26.415491 lego_image_converter-0.1.0/PKG-INFO
--rw-r--r--   0 zequnli    (501) staff       (20)     3905 2023-07-31 02:56:50.000000 lego_image_converter-0.1.0/README.md
-drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 02:57:26.414794 lego_image_converter-0.1.0/lego_image_converter/
--rw-r--r--   0 zequnli    (501) staff       (20)    10415 2023-07-31 02:56:50.000000 lego_image_converter-0.1.0/lego_image_converter/__init__.py
--rw-r--r--   0 zequnli    (501) staff       (20)      688 2023-07-30 23:45:16.000000 lego_image_converter-0.1.0/lego_image_converter/config.py
--rw-r--r--   0 zequnli    (501) staff       (20)     1120 2023-07-30 13:48:25.000000 lego_image_converter-0.1.0/lego_image_converter/utility.py
-drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 02:57:26.415341 lego_image_converter-0.1.0/lego_image_converter.egg-info/
--rw-r--r--   0 zequnli    (501) staff       (20)     4554 2023-07-31 02:57:26.000000 lego_image_converter-0.1.0/lego_image_converter.egg-info/PKG-INFO
--rw-r--r--   0 zequnli    (501) staff       (20)      351 2023-07-31 02:57:26.000000 lego_image_converter-0.1.0/lego_image_converter.egg-info/SOURCES.txt
--rw-r--r--   0 zequnli    (501) staff       (20)        1 2023-07-31 02:57:26.000000 lego_image_converter-0.1.0/lego_image_converter.egg-info/dependency_links.txt
--rw-r--r--   0 zequnli    (501) staff       (20)       49 2023-07-31 02:57:26.000000 lego_image_converter-0.1.0/lego_image_converter.egg-info/requires.txt
--rw-r--r--   0 zequnli    (501) staff       (20)       21 2023-07-31 02:57:26.000000 lego_image_converter-0.1.0/lego_image_converter.egg-info/top_level.txt
--rw-r--r--   0 zequnli    (501) staff       (20)       79 2023-07-31 02:57:26.415688 lego_image_converter-0.1.0/setup.cfg
--rw-r--r--   0 zequnli    (501) staff       (20)      977 2023-07-31 02:53:07.000000 lego_image_converter-0.1.0/setup.py
+drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 03:05:54.028165 lego_image_converter-0.1.1/
+-rw-r--r--   0 zequnli    (501) staff       (20)     1063 2023-07-30 23:49:22.000000 lego_image_converter-0.1.1/LICENSE
+-rw-r--r--   0 zequnli    (501) staff       (20)     4573 2023-07-31 03:05:54.028232 lego_image_converter-0.1.1/PKG-INFO
+-rw-r--r--   0 zequnli    (501) staff       (20)     3905 2023-07-31 02:56:50.000000 lego_image_converter-0.1.1/README.md
+drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 03:05:54.027365 lego_image_converter-0.1.1/lego_image_converter/
+-rw-r--r--   0 zequnli    (501) staff       (20)    10415 2023-07-31 03:04:16.000000 lego_image_converter-0.1.1/lego_image_converter/__init__.py
+-rw-r--r--   0 zequnli    (501) staff       (20)      688 2023-07-30 23:45:16.000000 lego_image_converter-0.1.1/lego_image_converter/config.py
+-rw-r--r--   0 zequnli    (501) staff       (20)     1120 2023-07-30 13:48:25.000000 lego_image_converter-0.1.1/lego_image_converter/utility.py
+drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 03:05:54.028067 lego_image_converter-0.1.1/lego_image_converter.egg-info/
+-rw-r--r--   0 zequnli    (501) staff       (20)     4573 2023-07-31 03:05:54.000000 lego_image_converter-0.1.1/lego_image_converter.egg-info/PKG-INFO
+-rw-r--r--   0 zequnli    (501) staff       (20)      351 2023-07-31 03:05:54.000000 lego_image_converter-0.1.1/lego_image_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)        1 2023-07-31 03:05:54.000000 lego_image_converter-0.1.1/lego_image_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)       49 2023-07-31 03:05:54.000000 lego_image_converter-0.1.1/lego_image_converter.egg-info/requires.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)       21 2023-07-31 03:05:54.000000 lego_image_converter-0.1.1/lego_image_converter.egg-info/top_level.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)       79 2023-07-31 03:05:54.028439 lego_image_converter-0.1.1/setup.cfg
+-rw-r--r--   0 zequnli    (501) staff       (20)      996 2023-07-31 03:04:16.000000 lego_image_converter-0.1.1/setup.py
```

### Comparing `lego_image_converter-0.1.0/LICENSE` & `lego_image_converter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.1.0/PKG-INFO` & `lego_image_converter-0.1.1/lego_image_converter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: lego_image_converter
-Version: 0.1.0
-Summary: First formal release
+Name: lego-image-converter
+Version: 0.1.1
+Summary: First minor update after formal release
 Home-page: https://github.com/zl3311/lego_image_converter
 Author: Zequn Li
 Author-email: zequn1992@gmail.com
 License: MIT
-Download-URL: https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.1.0.tar.gz
+Download-URL: https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.1.1.tar.gz
 Keywords: pypi,lego_image_converter,lego,image,8bit,art
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `lego_image_converter-0.1.0/README.md` & `lego_image_converter-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.1.0/lego_image_converter/__init__.py` & `lego_image_converter-0.1.1/lego_image_converter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,43 +82,43 @@
 
             if save:
                 t = str(int(time()))
                 fig.savefig(f'./output/{self.session_id}/{t}_raw.png', dpi=default_dpi)
                 if self.verbose:
                     print(f"Raw image saved to /output/{self.session_id}/{t}_raw.png")
             if not show:
-                fig.close()
+                plt.close()
 
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
             if not show:
-                fig.close()
+                plt.close()
 
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
             if not show:
-                fig.close()
+                plt.close()
         elif image_type == "converted":
             assert self.image_array_converted is not None, 'No converted image is found. Please convert an image first.'
             l, w, _ = self.image_array_converted.shape
             fig, ax = plt.subplots(1, 1, figsize=(fig_width, fig_length / w * l))
             _ = ax.set_facecolor('k')
             _ = ax.vlines(x=list(range(w+1)), ymin=0, ymax=l, colors='gray', linewidths=1)
             _ = ax.hlines(y=list(range(l+1)), xmin=0, xmax=w, colors='gray', linewidths=1)
@@ -133,15 +133,15 @@
 
             if save:
                 t = str(int(time()))
                 fig.savefig(f'./output/{self.session_id}/{t}_converted.png', dpi=default_dpi)
                 if self.verbose:
                     print(f"Converted image saved to /output/{self.session_id}/{t}_converted.png")
             if not show:
-                fig.close()
+                plt.close()
         return
 
     def trim_image(self):
         """trim the raw image for the Lego frame with very limited capability."""
         assert self.image_array_raw is not None, 'No raw image is found! Please load an image first.'
         l, w, _ = self.image_array_raw.shape
         l_, w_ = self.config['frame_length'], self.config['frame_width']
```

### Comparing `lego_image_converter-0.1.0/lego_image_converter/config.py` & `lego_image_converter-0.1.1/lego_image_converter/config.py`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.1.0/lego_image_converter/utility.py` & `lego_image_converter-0.1.1/lego_image_converter/utility.py`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.1.0/lego_image_converter.egg-info/PKG-INFO` & `lego_image_converter-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: lego-image-converter
-Version: 0.1.0
-Summary: First formal release
+Name: lego_image_converter
+Version: 0.1.1
+Summary: First minor update after formal release
 Home-page: https://github.com/zl3311/lego_image_converter
 Author: Zequn Li
 Author-email: zequn1992@gmail.com
 License: MIT
-Download-URL: https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.1.0.tar.gz
+Download-URL: https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.1.1.tar.gz
 Keywords: pypi,lego_image_converter,lego,image,8bit,art
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `lego_image_converter-0.1.0/setup.py` & `lego_image_converter-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='lego_image_converter',
     packages=['lego_image_converter'],
-    version='0.1.0',
+    version='0.1.1',
     license='MIT',
-    description='First formal release',
+    description='First minor update after formal release',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Zequn Li',
     author_email='zequn1992@gmail.com',
     url='https://github.com/zl3311/lego_image_converter',
     install_requires=['requests', 'numpy', 'matplotlib', 'pillow', 'basic_colormath'],
     keywords=["pypi", "lego_image_converter", "lego", "image", "8bit", "art"],
     classifiers=[
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Documentation',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
 
-    download_url="https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.1.0.tar.gz",
+    download_url="https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.1.1.tar.gz",
 )
```

