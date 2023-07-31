# Comparing `tmp/katalytic_images-0.9.1.tar.gz` & `tmp/katalytic_images-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic_images-0.9.1.tar", last modified: Mon Jul 10 20:59:20 2023, max compression
+gzip compressed data, was "katalytic_images-0.9.4.tar", last modified: Mon Jul 31 07:39:09 2023, max compression
```

## Comparing `katalytic_images-0.9.1.tar` & `katalytic_images-0.9.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic_images-0.9.1/LICENSE.txt
--rw-r--r--   0        0        0     2212 2023-07-10 04:57:46.112850 katalytic_images-0.9.1/README.md
--rw-r--r--   0        0        0     1598 2023-07-10 20:59:20.576380 katalytic_images-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    25507 2023-07-10 20:57:45.604107 katalytic_images-0.9.1/src/katalytic/images/__init__.py
--rw-r--r--   0        0        0    20549 2023-07-02 19:24:10.781971 katalytic_images-0.9.1/tests/test_images.py
--rw-r--r--   0        0        0     4821 1970-01-01 00:00:00.000000 katalytic_images-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic_images-0.9.4/LICENSE.txt
+-rw-r--r--   0        0        0     2235 2023-07-31 07:03:17.224349 katalytic_images-0.9.4/README.md
+-rw-r--r--   0        0        0     1601 2023-07-31 07:39:09.660673 katalytic_images-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0    26188 2023-07-31 07:20:39.387005 katalytic_images-0.9.4/src/katalytic/images/__init__.py
+-rw-r--r--   0        0        0    21867 2023-07-31 07:32:07.149847 katalytic_images-0.9.4/tests/test_images.py
+-rw-r--r--   0        0        0     4887 1970-01-01 00:00:00.000000 katalytic_images-0.9.4/PKG-INFO
```

### Comparing `katalytic_images-0.9.1/LICENSE.txt` & `katalytic_images-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.9.1/README.md` & `katalytic_images-0.9.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 - The functions accept numpy arrays and Pillow images as input and return the same type
 - defining the shapes to be drawn on top of an image in a declarative way as a list of dicts and passing it to draw()
 - Many more (TODO: Link to tocs)
 
 ## Example (TODO)
 
 ## Installation
-By itself
+First, install opencv
 ```bash
-pip install katalytic-images
+if [[ ! $(pip freeze | grep -Pi 'opencv') ]]; then 
+    pip install opencv-python 
+fi
 ```
-
-As part of the [katalytic](https://gitlab.com/katalytic/katalytic) collection
+Then, install this package
 ```bash
-pip install katalytic
+pip install katalytic-images
 ```
 
 ## Roadmap
 - make pillow an optional dependency.
    - setup_load_image() should pick opencv if pillow is not available
 - image thresholding and masking operations
 - interactive data exploration widgets (maybe as part of another package)
@@ -35,8 +36,7 @@
 ## Contributing
 We appreciate any form of contribution, including but not limited to:
 - **Code contributions**: Enhance our repository with your code and tests.
 - **Feature suggestions**: Your ideas can shape the future development of our package.
 - **Architectural improvements**: Help us optimize our system's design and API.
 - **Bug fixes**: Improve user experience by reporting or resolving issues.
 - **Documentation**: Help us maintain clear and up-to-date instructions for users.
-
```

### Comparing `katalytic_images-0.9.1/pyproject.toml` & `katalytic_images-0.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 
 [project]
 name = "katalytic-images"
-version = "0.9.1"
+version = "0.9.4"
 description = "This plugin adds utilities for working with images and videos to the katalytic namespace"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
@@ -37,23 +37,24 @@
 authors = [
     { name = "Valentin Neagu", email = "vali19th@protonmail.com" },
 ]
 requires-python = ">=3.6"
 dependencies = [
     "katalytic>=0.2.2",
     "numpy>=1.14",
-    "opencv-python>=4.0.0",
     "pillow>=8.4.0",
 ]
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.optional-dependencies]
 dev = [
+    "black",
+    "pre-commit",
     "pytest",
     "pytest-cov",
     "pytest-clarity",
     "pytest-randomly",
 ]
 
 [project.urls]
```

### Comparing `katalytic_images-0.9.1/src/katalytic/images/__init__.py` & `katalytic_images-0.9.4/src/katalytic/images/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import errno
 from pathlib import Path
 
-import cv2
-# noinspection PyProtectedMember
-from cv2 import (
-    imwrite as __cv2_imwrite,
-    cvtColor as __cv2_cvtColor
-)
+try:
+    import cv2
+except ImportError:  # pragma: no cover
+    msg = [
+        "Please install one of the following:",
+        "pip install opencv-python                   # the most popular",
+        "pip install opencv-python-headless          # the most popular, without GUI functionality (for servers)",
+        "pip install opencv-contrib-python           # extended functionality",
+        "pip install opencv-contrib-python-headless  # extended functionality, without GUI functionality (for servers)",
+    ]
+    raise ImportError("\n\t".join(msg))
+
+from cv2 import imwrite as __cv2_imwrite, cvtColor as __cv2_cvtColor
 
 import numpy as np
-from numpy import (
-    array as __np_array,
-    ndarray as __np_ndarray
-)
+from numpy import array as __np_array, ndarray as __np_ndarray
 
 import PIL.Image
+
 __PIL_Image_open = PIL.Image.open
 __PIL_Image_Image = PIL.Image.Image
 
 from katalytic.data.checks import is_iterable, is_number, is_sequence
+
 # noinspection PyProtectedMember
 from katalytic._pkg import get_version, mark, KatalyticInterrupt, _UNDEFINED
 
 __version__, __version_info__ = get_version(__name__)
 
 
 def bhwc(arr):
@@ -46,15 +52,15 @@
     elif arr.ndim == 2:
         return (1, *arr.shape, 1)
     elif arr.ndim == 3:
         return (1, *arr.shape)
     elif arr.ndim == 4:
         return arr.shape
     else:
-        raise ValueError(f'arr.ndim = {arr.ndim}')
+        raise ValueError(f"arr.ndim = {arr.ndim}")
 
 
 def convert_image(image, before, after):
     """
     Converts an image from one color space to another.
 
     Parameters:
@@ -67,31 +73,31 @@
 
     Raises:
         TypeError: If the 'before' or after' parameters are not a string.
         ValueError: If the conversion code is not found for the specified color space conversion.
 
     """
     if not isinstance(before, str):
-        raise TypeError(f'type(before) = {type(before)!r}')
+        raise TypeError(f"type(before) = {type(before)!r}")
     elif not isinstance(after, str):
-        raise TypeError(f'type(after) = {type(after)!r}')
+        raise TypeError(f"type(after) = {type(after)!r}")
 
     return_PIL = isinstance(image, PIL.Image.Image)
     if return_PIL:
         image = np.array(image)
     else:
         image = load_image(image)
 
-    conversion_code = f'COLOR_{before}2{after}'
-    conversion_code = conversion_code.replace('gray', 'GRAY')
+    conversion_code = f"COLOR_{before}2{after}"
+    conversion_code = conversion_code.replace("gray", "GRAY")
     conversion_code = getattr(cv2, conversion_code, None)
 
     if conversion_code:
         img = __cv2_cvtColor(image, conversion_code)
-    elif before.startswith('binary') or after.startswith('binary'):
+    elif before.startswith("binary") or after.startswith("binary"):
         raise NotImplementedError
     else:
         raise ValueError
 
     if return_PIL:
         return PIL.Image.fromarray(img)
     else:
@@ -110,20 +116,20 @@
         **kwargs: Additional keyword arguments that can be used to customize the shape.
 
     Returns:
         dict: A dictionary representing the line to be drawn
 
     """
     return {
-        'type': 'line',
-        'p1': tuple(map(int, p1)),
-        'p2': tuple(map(int, p2)),
-        'color': color,
-        'thickness': thickness,
-        **kwargs
+        "type": "line",
+        "p1": tuple(map(int, p1)),
+        "p2": tuple(map(int, p2)),
+        "color": color,
+        "thickness": thickness,
+        **kwargs,
     }
 
 
 def create_circle(center, radius, color, *, thickness=3, **kwargs):
     """
     Create a dict representing a circle shape to be used by draw()() or draw_inplace().
 
@@ -135,20 +141,20 @@
         **kwargs: Additional keyword arguments that can be used to customize the circle object.
 
     Returns:
         dict: A dictionary representing the circle to be drawn
 
     """
     return {
-        'type': 'circle',
-        'center': tuple(map(int, center)),
-        'radius': int(radius),
-        'color': color,
-        'thickness': thickness,
-        **kwargs
+        "type": "circle",
+        "center": tuple(map(int, center)),
+        "radius": int(radius),
+        "color": color,
+        "thickness": thickness,
+        **kwargs,
     }
 
 
 def create_rectangle(p1, p2, color, *, thickness=3, **kwargs):
     """
     Create a dict representing a rectangle shape to be used by draw()() or draw_inplace().
 
@@ -160,24 +166,35 @@
         **kwargs: Additional keyword arguments that can be used to customize the shape.
 
     Returns:
         dict: A dictionary representing the rectangle to be drawn
 
     """
     return {
-        'type': 'rectangle',
-        'p1': tuple(map(int, p1)),
-        'p2': tuple(map(int, p2)),
-        'color': color,
-        'thickness': thickness,
-        **kwargs
+        "type": "rectangle",
+        "p1": tuple(map(int, p1)),
+        "p2": tuple(map(int, p2)),
+        "color": color,
+        "thickness": thickness,
+        **kwargs,
     }
 
 
-def create_text(text, origin, color, *, font=cv2.FONT_HERSHEY_SIMPLEX, scale=1.25, thickness=3, bg=None, bg_pad=None, **kwargs):
+def create_text(
+    text,
+    origin,
+    color,
+    *,
+    font=cv2.FONT_HERSHEY_SIMPLEX,
+    scale=1.25,
+    thickness=3,
+    bg=None,
+    bg_pad=None,
+    **kwargs,
+):
     """Create a text shape.
     The text shape represents a text string with its origin point, color, font, scale, and thickness. It can also include a background rectangle behind the text.
 
     Parameters:
         text (str): The text string to be displayed.
         origin (tuple or list): The (x, y) coordinates of the origin point.
         color: The color of the text. It can be specified in various formats supported by the underlying drawing library.
@@ -194,46 +211,48 @@
     Raises:
         ValueError: If the 'bg' parameter is None, but the 'bg_pad' parameter is set to a value.
         ValueError: If the 'bg_pad' parameter has an invalid format.
         TypeError: If the 'bg_pad' parameter has an unsupported type.
 
     """
     shape = {
-        'type': 'text',
-        'text': text,
-        'origin': tuple(map(int, origin)),
-        'color': color,
-        'font': font,
-        'font_scale': scale,
-        'thickness': thickness,
-        **kwargs
+        "type": "text",
+        "text": text,
+        "origin": tuple(map(int, origin)),
+        "color": color,
+        "font": font,
+        "font_scale": scale,
+        "thickness": thickness,
+        **kwargs,
     }
 
     if bg is None:
         if bg_pad is None:
             return shape
         else:
             # bg_pad is set to None by default instead of 5 ot alert the user
             # when he sets <bg_pad> and forgets <bg>.
             # Otherwise the mistake would be ignored silently
-            raise ValueError('<bg> is None, even though <bg_pad> is set to a value')
+            raise ValueError("<bg> is None, even though <bg_pad> is set to a value")
 
     if bg_pad is None:
         bg_pad = [5] * 4
     elif is_number(bg_pad):
         bg_pad = [bg_pad] * 4
     elif is_sequence(bg_pad):
         if len(bg_pad) == 2:
             bg_pad = [*bg_pad, *bg_pad]
         elif len(bg_pad) != 4:
-            raise ValueError(f'<bg_pad> expects None, a number or a sequence like (horizontal, vertical) or (left, top, right, bottom). Got a sequence of length {len(bg_pad)}')
+            raise ValueError(
+                f"<bg_pad> expects None, a number or a sequence like (horizontal, vertical) or (left, top, right, bottom). Got a sequence of length {len(bg_pad)}"
+            )
     else:
-        raise TypeError(f'type(bg_pad) = {type(bg_pad)!r}')
+        raise TypeError(f"type(bg_pad) = {type(bg_pad)!r}")
 
-    shape['background'] = {'color': bg, 'pad': bg_pad}
+    shape["background"] = {"color": bg, "pad": bg_pad}
     return shape
 
 
 def create_polylines(pts, color, *, thickness=3, is_closed=True, **kwargs):
     """
     Create a dict representing a polylines shape to be used by draw() or draw_inplace().
 
@@ -245,20 +264,20 @@
         **kwargs: Additional keyword arguments that can be used to customize the polylines object.
 
     Returns:
         dict: A dictionary representing the polylines to be drawn
 
     """
     return {
-        'type': 'polylines',
-        'pts': pts,
-        'color': color,
-        'thickness': thickness,
-        'is_closed': is_closed,
-        **kwargs
+        "type": "polylines",
+        "pts": pts,
+        "color": color,
+        "thickness": thickness,
+        "is_closed": is_closed,
+        **kwargs,
     }
 
 
 def create_mask(pts, color, **kwargs):
     """
     Create a dict representing a mask shape to be used by draw() or draw_inplace().
 
@@ -267,20 +286,15 @@
         color: The color of the polylines. It can be specified in various formats supported by the underlying drawing library.
         **kwargs: Additional keyword arguments that can be used to customize the polylines object.
 
     Returns:
         dict: A dictionary representing the mask to be drawn
 
     """
-    return {
-        'type': 'mask',
-        'pts': pts,
-        'color': color,
-        **kwargs
-    }
+    return {"type": "mask", "pts": pts, "color": color, **kwargs}
 
 
 def draw(image, data):
     """Draws shapes on a copy of the input image
 
     This function takes an image and an collection specifying the shapes to be drawn on the image.
     The shapes can include lines, circles, rectangles, text, masks, and polylines.
@@ -331,43 +345,42 @@
         ValueError: If the 'type' key in any shape dictionary has an invalid value.
         ValueError: If the 'pts' key in a mask or polylines shape dictionary has an invalid format.
 
     """
     if isinstance(data, dict):
         data = [data]
     elif not is_iterable(data):
-        raise TypeError(f'type(data) = {type(data)!r}')
+        raise TypeError(f"type(data) = {type(data)!r}")
 
     for shape in data:
-        draw_shape = _pick_draw_function(shape['type'])
+        draw_shape = _pick_draw_function(shape["type"])
         shape = _rename_kwargs(shape)
 
-        if shape['type'] == 'text':
+        if shape["type"] == "text":
             # extract background info only after the call to _rename_kwargs()
             # Otherwise you might miscalculate the bg size and position
             bg = _create_rectangle_for_text_background(
-                shape.pop('background', None),
-                shape
+                shape.pop("background", None), shape
             )
             if bg:
                 draw_inplace(image, bg)
-        elif shape['type'] in ('mask', 'polylines'):
-            pts = shape['pts']
+        elif shape["type"] in ("mask", "polylines"):
+            pts = shape["pts"]
             if is_iterable(pts):
                 if not is_iterable(pts[0][0]):
                     pts = [pts]
 
             if not isinstance(pts, np.ndarray):
                 pts = np.array(pts, dtype=np.int32)
             elif pts.dtype != np.int32:
                 pts = pts.astype(np.int32)
 
-            shape['pts'] = pts
+            shape["pts"] = pts
 
-        del shape['type']
+        del shape["type"]
         draw_shape(image, **shape)
 
 
 def _create_rectangle_for_text_background(bg, text):
     """Create a rectangle to act as background for the text.
 
     Parameters:
@@ -383,88 +396,88 @@
 
     """
     if not bg:
         return None
 
     if is_sequence(bg) or is_number(bg):
         color = bg
-        pad = 5 * text['fontScale']
+        pad = 5 * text["fontScale"]
     elif isinstance(bg, dict):
-        color = bg.pop('color')
-        pad = bg.pop('pad', 5 * text['fontScale'])
+        color = bg.pop("color")
+        pad = bg.pop("pad", 5 * text["fontScale"])
     else:
-        raise TypeError(f'type(background) = {type(bg).__name__!r}')
+        raise TypeError(f"type(background) = {type(bg).__name__!r}")
 
-    error_msg = f'Expected <pad> to be an int or a sequence like (horizontal, vertical) or (left, top, right, bottom). Got {pad!r}'
+    error_msg = f"Expected <pad> to be an int or a sequence like (horizontal, vertical) or (left, top, right, bottom). Got {pad!r}"
 
     if is_number(pad):
         pad = (pad, pad, pad, pad)
     elif is_sequence(pad):
         if len(pad) == 2:
             pad = (*pad, *pad)
         elif len(pad) == 4:
             pass
         else:
             raise ValueError(error_msg)
     else:
         raise ValueError(error_msg)
 
-    kwargs = {k: text[k] for k in ['text', 'fontFace', 'fontScale', 'thickness']}
+    kwargs = {k: text[k] for k in ["text", "fontFace", "fontScale", "thickness"]}
     (w, h), baseline = cv2.getTextSize(**kwargs)
-    baseline += text['thickness'] * text['fontScale']
-    if text.get('bottomLeftOrigin', False):
-        raise NotImplementedError('Calculate baseline for bottomLeftOrigin=True')
+    baseline += text["thickness"] * text["fontScale"]
+    if text.get("bottomLeftOrigin", False):
+        raise NotImplementedError("Calculate baseline for bottomLeftOrigin=True")
 
-    p1 = (text['org'][0] - pad[0], text['org'][1] - h - pad[1])
-    p2 = (text['org'][0] + w + pad[2], text['org'][1] + baseline + pad[3])
+    p1 = (text["org"][0] - pad[0], text["org"][1] - h - pad[1])
+    p2 = (text["org"][0] + w + pad[2], text["org"][1] + baseline + pad[3])
     return create_rectangle(p1, p2, color, thickness=-1)
 
 
 def _rename_kwargs(shape):
     """Rename the keys to match the corresponding OpenCV function parameters."""
     conversion = {
-        'font': 'fontFace',
-        'font_scale': 'fontScale',
-        'line_type': 'lineType',
-        'draw_above_origin': 'bottomLeftOrigin',
-        'p1': 'pt1',
-        'p2': 'pt2',
-        'origin': 'org',
-        'is_closed': 'isClosed',
+        "font": "fontFace",
+        "font_scale": "fontScale",
+        "line_type": "lineType",
+        "draw_above_origin": "bottomLeftOrigin",
+        "p1": "pt1",
+        "p2": "pt2",
+        "origin": "org",
+        "is_closed": "isClosed",
     }
 
     return {conversion.get(k, k): v for k, v in shape.items()}
 
 
 def _pick_draw_function(shape_type):
     """Pick the corresponding OpenCV drawing function based on the shape type."""
     fn = {
-        'arrowed_line': cv2.arrowedLine,
-        'circle': cv2.circle,
-        'contours': cv2.drawContours,
-        'convex_polygon': cv2.fillConvexPoly,
-        'ellipse': cv2.ellipse,
-        'ellipse_polygon': cv2.ellipse2Poly,
-        'line': cv2.line,
-        'marker': cv2.drawMarker,
-        'mask': cv2.fillPoly,
-        'polylines': cv2.polylines,
-        'rectangle': cv2.rectangle,
-        'text': cv2.putText,
+        "arrowed_line": cv2.arrowedLine,
+        "circle": cv2.circle,
+        "contours": cv2.drawContours,
+        "convex_polygon": cv2.fillConvexPoly,
+        "ellipse": cv2.ellipse,
+        "ellipse_polygon": cv2.ellipse2Poly,
+        "line": cv2.line,
+        "marker": cv2.drawMarker,
+        "mask": cv2.fillPoly,
+        "polylines": cv2.polylines,
+        "rectangle": cv2.rectangle,
+        "text": cv2.putText,
     }
 
     if shape_type not in fn:
-        raise ValueError(f'Unknown shape: {shape_type!r}')
+        raise ValueError(f"Unknown shape: {shape_type!r}")
     else:
         return fn[shape_type]
 
 
-@mark('load::png')
-@mark('load::jpg')
-@mark('load::jpeg')
+@mark("load::png")
+@mark("load::jpg")
+@mark("load::jpeg")
 def load_image(image, mode=None, *, default=_UNDEFINED):
     """
     Load an image and return it as a NumPy array.
 
     Parameters:
         image: The image to be loaded. It can be specified as a file path (string or Path object), a PIL Image object, or a NumPy array.
         mode (str, optional): The mode to be used when loading the image. It should be a string representing the desired mode, e.g., 'RGB', 'L', 'RGBA'. If None, the default mode of the image will be used.
@@ -475,31 +488,35 @@
         numpy.ndarray: The loaded image as a NumPy array.
 
     Raises:
         TypeError: If the 'mode' parameter is not None or a string.
         TypeError: If the 'image' parameter has an unsupported type.
 
     """
-    if not(mode is None or isinstance(mode, str)):
-        raise TypeError(f'mode expected None or str. Got {type(mode)!r}')
+    if not (mode is None or isinstance(mode, str)):
+        raise TypeError(f"mode expected None or str. Got {type(mode)!r}")
 
     if isinstance(image, (str, Path)):
         # noinspection PyProtectedMember
-        from katalytic.files import _warn_if_another_function_should_be_used, _load_funcs
+        from katalytic.files import (
+            _warn_if_another_function_should_be_used,
+            _load_funcs,
+        )
+
         _warn_if_another_function_should_be_used(str(image), _load_funcs)
         if not Path(image).exists() and default is not _UNDEFINED:
             return default
         else:
             return __np_array(__PIL_Image_open(image))
     elif isinstance(image, __PIL_Image_Image):
         return image.copy()
     elif isinstance(image, __np_ndarray):
         return image.copy()
     else:
-        raise TypeError(f'type(image) = {type(image)!r}')
+        raise TypeError(f"type(image) = {type(image)!r}")
 
 
 def hwc(arr):
     """
     Returns a tuple representing the shape of the input array in the HWC format: height, width, and channels. The missing dimensions are filled with 1s.
 
     Parameters:
@@ -554,18 +571,18 @@
     elif check_type and image_1.dtype != image_2.dtype:
         return False
     else:
         # noinspection PyUnresolvedReferences
         return (image_1 == image_2).all()
 
 
-@mark('save::png')
-@mark('save::jpg')
-@mark('save::jpeg')
-def save_image(image, path, *, exists='replace', make_dirs=True, mode='RGB'):
+@mark("save::png")
+@mark("save::jpg")
+@mark("save::jpeg")
+def save_image(image, path, *, exists="replace", make_dirs=True, mode="RGB"):
     """
     Save an image to the specified file path.
     The image can be provided as a PIL Image object, a NumPy array, or a file path.
     The function supports specifying the behavior when the target file already exists.
 
     Parameters:
         image: The image to be saved. It can be specified as a PIL Image object, a NumPy array, or a file path (string or Path object).
@@ -586,82 +603,93 @@
     Raises:
         TypeError: If the 'mode' parameter is not a string.
         ValueError: If the 'exists' parameter is not one of 'error', 'skip', 'replace'.
         FileExistsError: If the target file already exists and the 'exists' parameter is set to 'error'.
 
     """
     if not isinstance(mode, str):
-        raise TypeError(f'type(mode) = {type(mode)!r}')
-    elif exists not in ('error', 'skip', 'replace'):
-        raise ValueError(f'exists must be one of \'error\', \'skip\', \'replace\'. Got {exists!r}')
+        raise TypeError(f"type(mode) = {type(mode)!r}")
+    elif exists not in ("error", "skip", "replace"):
+        raise ValueError(
+            f"exists must be one of 'error', 'skip', 'replace'. Got {exists!r}"
+        )
 
     # noinspection PyProtectedMember
     from katalytic.files import _warn_if_another_function_should_be_used, _save_funcs
+
     _warn_if_another_function_should_be_used(str(path), _save_funcs)
     if Path(path).exists():
-        if exists == 'error':
-            raise FileExistsError(f'[Errno {errno.EEXIST}] File exists: {str(path)!r}')
-        elif exists == 'replace':
+        if exists == "error":
+            raise FileExistsError(f"[Errno {errno.EEXIST}] File exists: {str(path)!r}")
+        elif exists == "replace":
             pass  # continue executing
-        elif exists == 'skip':
+        elif exists == "skip":
             return
 
     try:
         dest_dir = Path(path).parent
         if make_dirs:
             from katalytic.files import make_dir
+
             make_dir(dest_dir, create_parents=True, exists_ok=True)
         elif not dest_dir.exists():
-            raise FileNotFoundError(f'[Errno {errno.ENOENT}] Directory does not exist: {str(dest_dir)!r}')
+            raise FileNotFoundError(
+                f"[Errno {errno.ENOENT}] Directory does not exist: {str(dest_dir)!r}"
+            )
         elif dest_dir.is_file():
-            raise NotADirectoryError(f'[Errno {errno.ENOTDIR}] Not a directory: {str(dest_dir)!r}')
+            raise NotADirectoryError(
+                f"[Errno {errno.ENOTDIR}] Not a directory: {str(dest_dir)!r}"
+            )
 
         if isinstance(image, __PIL_Image_Image):
             image = __np_array(image)
 
         if isinstance(image, __np_ndarray):
-            if mode != 'BGR':
-                image = convert_image(image, mode, 'BGR')
+            if mode != "BGR":
+                image = convert_image(image, mode, "BGR")
 
-            ext = str(path).rpartition('.')[2]
-            tmp_path = f'{path}.part.{ext}'
+            ext = str(path).rpartition(".")[2]
+            tmp_path = f"{path}.part.{ext}"
             __cv2_imwrite(tmp_path, image)
 
             if save_image.__katalytic_test_atomicity_race_condition__:
                 save_image.__katalytic_test_atomicity_race_condition__ = False
 
                 # I can't use save_image('race condition', path) directly
                 # It would replace the tmp_path = f'{path}.part' created above
                 # and then move it to the target `path`. This function wouldn't
                 # be able to find the tmp_path anymore and will throw an error
                 # at the end of the function: `Path(tmp_path).rename(path)`
-                tmp_path_2 = f'{path}.part2.{ext}'
-                save_image(np.array([[[0,255,0]]], dtype=np.uint8), tmp_path_2)
+                tmp_path_2 = f"{path}.part2.{ext}"
+                save_image(np.array([[[0, 255, 0]]], dtype=np.uint8), tmp_path_2)
                 Path(tmp_path_2).rename(path)
 
             # Checking these conditions again to make the function
             # as robust as possible against race conditions
             if Path(path).exists():
-                if exists == 'error':
-                    raise FileExistsError(f'[Errno {errno.EEXIST}] File exists: {str(path)!r}')
-                elif exists == 'replace':
+                if exists == "error":
+                    raise FileExistsError(
+                        f"[Errno {errno.EEXIST}] File exists: {str(path)!r}"
+                    )
+                elif exists == "replace":
                     pass  # continue executing
-                elif exists == 'skip':
+                elif exists == "skip":
                     return
 
             if save_image.__katalytic_test_atomicity_interrupt__:
                 save_image.__katalytic_test_atomicity_interrupt__ = False
-                raise KatalyticInterrupt(f'Testing atomicity ...')
+                raise KatalyticInterrupt(f"Testing atomicity ...")
 
             Path(tmp_path).rename(path)
         elif isinstance(image, (str, Path)):
             from katalytic.files import copy_file
+
             copy_file(image, path, exists=exists)
         else:
-            raise TypeError(f'type(image) = {type(image)!r}')
+            raise TypeError(f"type(image) = {type(image)!r}")
     except BaseException as e:
         if not isinstance(e, KatalyticInterrupt):
             raise
 
 
 save_image.__katalytic_test_atomicity_interrupt__ = False
 save_image.__katalytic_test_atomicity_race_condition__ = False
```

### Comparing `katalytic_images-0.9.1/tests/test_images.py` & `katalytic_images-0.9.4/tests/test_images.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,71 +3,110 @@
 
 import cv2
 import numpy as np
 import PIL.Image
 import pytest
 from PIL import Image
 
-from katalytic.data import all_types_besides
-from katalytic.files import delete_file, get_unique_path, load, load_csv, load_json, load_text, move_file, save, save_csv, save_json, save_text
-from katalytic.images import bhwc, convert_image, create_circle, create_line, create_mask, create_polylines, create_rectangle, create_text, draw, hw, hwc, are_arrays_equal, load_image, save_image
+from katalytic._pkg import all_types_besides
+from katalytic.files import (
+    delete_file,
+    get_unique_path,
+    load,
+    load_csv,
+    load_json,
+    load_text,
+    move_file,
+    save,
+    save_csv,
+    save_json,
+    save_text,
+)
+from katalytic.images import (
+    bhwc,
+    convert_image,
+    create_circle,
+    create_line,
+    create_mask,
+    create_polylines,
+    create_rectangle,
+    create_text,
+    draw,
+    hw,
+    hwc,
+    are_arrays_equal,
+    load_image,
+    save_image,
+)
 
 
 def _create_RGB(dtype=np.uint8):
-    return np.array([
-        [[255, 0, 0], [0, 255, 0], [0, 0, 255]],        # RGB
-        [[0, 255, 255], [255, 0, 255], [255, 255, 0]],  # CMY
-        [[0, 0, 255], [0, 255, 0], [255, 0, 0]],        # BGR
-        [[0, 0, 0], [128, 128, 128], [255, 255, 255]],  # black, gray, white
-    ], dtype=dtype)
+    return np.array(
+        [
+            [[255, 0, 0], [0, 255, 0], [0, 0, 255]],  # RGB
+            [[0, 255, 255], [255, 0, 255], [255, 255, 0]],  # CMY
+            [[0, 0, 255], [0, 255, 0], [255, 0, 0]],  # BGR
+            [[0, 0, 0], [128, 128, 128], [255, 255, 255]],  # black, gray, white
+        ],
+        dtype=dtype,
+    )
 
 
 class Test_bhwc:
-    @pytest.mark.parametrize('ndim', [5, 10, 100])
+    @pytest.mark.parametrize("ndim", [5, 10, 100])
     def test_bhwc_error(self, ndim):
         with pytest.raises(ValueError):
             bhwc(np.zeros(range(ndim)))
 
-    @pytest.mark.parametrize('data, expected', [
-        ([], (0, 0, 0, 0)),
-        ([1], (1, 1, 1, 1)),
-        ([1,2], (1, 2, 1, 1)),
-        ([[1,2], [3,4], [5,6]], (1, 3, 2, 1)),
-        ([[1,2,3], [4,5,6]], (1, 2, 3, 1)),
-        (_create_RGB(), (1, 4, 3, 3)),
-        (np.zeros((2, 3, 4, 5)), (2, 3, 4, 5)),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ([], (0, 0, 0, 0)),
+            ([1], (1, 1, 1, 1)),
+            ([1, 2], (1, 2, 1, 1)),
+            ([[1, 2], [3, 4], [5, 6]], (1, 3, 2, 1)),
+            ([[1, 2, 3], [4, 5, 6]], (1, 2, 3, 1)),
+            (_create_RGB(), (1, 4, 3, 3)),
+            (np.zeros((2, 3, 4, 5)), (2, 3, 4, 5)),
+        ],
+    )
     def test_bhwc(self, data, expected):
         if isinstance(data, list):
             data = np.array(data)
 
         assert bhwc(data) == expected
 
-    @pytest.mark.parametrize('data, expected', [
-        ([], (0, 0, 0)),
-        ([1], (1, 1, 1)),
-        ([1,2], (2, 1, 1)),
-        ([[1,2], [3,4], [5,6]], (3, 2, 1)),
-        ([[1,2,3], [4,5,6]], (2, 3, 1)),
-        (_create_RGB(), (4, 3, 3)),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ([], (0, 0, 0)),
+            ([1], (1, 1, 1)),
+            ([1, 2], (2, 1, 1)),
+            ([[1, 2], [3, 4], [5, 6]], (3, 2, 1)),
+            ([[1, 2, 3], [4, 5, 6]], (2, 3, 1)),
+            (_create_RGB(), (4, 3, 3)),
+        ],
+    )
     def test_hwc(self, data, expected):
         if isinstance(data, list):
             data = np.array(data)
 
         assert hwc(data) == expected
 
-    @pytest.mark.parametrize('data, expected', [
-        ([], (0, 0)),
-        ([1], (1, 1)),
-        ([1,2], (2, 1)),
-        ([[1,2], [3,4], [5,6]], (3, 2)),
-        ([[1,2,3], [4,5,6]], (2, 3)),
-        (_create_RGB(), (4, 3)),
-    ])
+    @pytest.mark.parametrize(
+        "data, expected",
+        [
+            ([], (0, 0)),
+            ([1], (1, 1)),
+            ([1, 2], (2, 1)),
+            ([[1, 2], [3, 4], [5, 6]], (3, 2)),
+            ([[1, 2, 3], [4, 5, 6]], (2, 3)),
+            (_create_RGB(), (4, 3)),
+        ],
+    )
     def test_hw(self, data, expected):
         if isinstance(data, list):
             data = np.array(data)
 
         assert hw(data) == expected
 
 
@@ -87,452 +126,514 @@
         - this will let me handle all cases with less code
         - e.g. 'binary_otsu_True_inv'.split('_') -> ['binary', 'otsu', 'True', 'inv'] ->
             - type = bool
             - values = False/True
             - invert bg with fg
             - use otsu
     """
+
     def test_returns_PIL_if_PIL(self):
         img = PIL.Image.fromarray(_create_RGB())
-        img2 = convert_image(img, 'RGB', 'BGR')
+        img2 = convert_image(img, "RGB", "BGR")
         assert isinstance(img2, PIL.Image.Image)
 
     def test_returns_numpy_if_numpy(self):
         img = _create_RGB()
-        img2 = convert_image(img, 'RGB', 'BGR')
+        img2 = convert_image(img, "RGB", "BGR")
         assert isinstance(img2, np.ndarray)
 
     def test_returns_numpy_if_str(self):
-        path = get_unique_path('{}.png')
+        path = get_unique_path("{}.png")
         save_image(_create_RGB(), path)
-        img2 = convert_image(path, 'RGB', 'BGR')
+        img2 = convert_image(path, "RGB", "BGR")
         assert isinstance(img2, np.ndarray)
 
     def test_returns_numpy_if_Path(self):
-        path = Path(get_unique_path('{}.png'))
+        path = Path(get_unique_path("{}.png"))
         save_image(_create_RGB(), path)
-        img2 = convert_image(path, 'RGB', 'BGR')
+        img2 = convert_image(path, "RGB", "BGR")
         assert isinstance(img2, np.ndarray)
 
-    @pytest.mark.xfail(reason='Not implemented')
+    @pytest.mark.xfail(reason="Not implemented")
     def test_convert_binary(self):
         img = np.array([[[0, 0, 0], [255, 255, 255]]])
-        img2 = convert_image(img, 'RGB', 'binary')
+        img2 = convert_image(img, "RGB", "binary")
         assert np.all(img2 == img.astype(bool).astype(np.uint8))
 
     def test_convert_to_unknown(self):
         img = np.array([[[0, 0, 0], [255, 255, 255]]])
         with pytest.raises(ValueError):
-            _ = convert_image(img, 'RGB', 'unknown')
+            _ = convert_image(img, "RGB", "unknown")
 
     def test_convert_from_unknown(self):
         img = np.array([[[0, 0, 0], [255, 255, 255]]])
         with pytest.raises(ValueError):
-            _ = convert_image(img, 'unknown', 'RGB')
+            _ = convert_image(img, "unknown", "RGB")
 
-    @pytest.mark.parametrize('before', all_types_besides('str'))
+    @pytest.mark.parametrize("before", all_types_besides("str"))
     def test_save_raises_TypeError_for_before(self, before):
         with pytest.raises(TypeError):
             # noinspection PyTypeChecker
-            convert_image(_create_RGB(), before, 'RGB')
+            convert_image(_create_RGB(), before, "RGB")
 
-    @pytest.mark.parametrize('after', all_types_besides('str'))
+    @pytest.mark.parametrize("after", all_types_besides("str"))
     def test_save_raises_TypeError_for_after(self, after):
         with pytest.raises(TypeError):
             # noinspection PyTypeChecker
-            convert_image(_create_RGB(), 'RGB', after)
+            convert_image(_create_RGB(), "RGB", after)
 
 
 class Test_draw:
-    @pytest.mark.parametrize('wrong_type', all_types_besides('iterables'))
+    @pytest.mark.parametrize("wrong_type", all_types_besides("iterables"))
     def test_wrong_type(self, wrong_type):
         with pytest.raises(TypeError):
             draw(np.zeros((5, 5)), wrong_type)
 
     def test_returns_PIL_if_PIL(self):
         img = np.zeros((5, 5, 3), dtype=np.uint8)
         img = PIL.Image.fromarray(img)
-        shape = create_circle((4,4), 2, (0, 0, 255))
+        shape = create_circle((4, 4), 2, (0, 0, 255))
 
         img2 = draw(img, shape)
         assert isinstance(img2, PIL.Image.Image)
 
     def test_draws_on_a_copy(self):
         img = np.zeros((5, 5, 3), dtype=np.uint8)
         img_copy = img.copy()
         shapes = [
-            create_line((0,0), (0,3), (0, 255, 0), thickness=1),
-            create_rectangle([1,1], (3,3), (255, 0, 0), thickness=-1),
-            create_circle((4,4), 2, (0, 0, 255))
+            create_line((0, 0), (0, 3), (0, 255, 0), thickness=1),
+            create_rectangle([1, 1], (3, 3), (255, 0, 0), thickness=-1),
+            create_circle((4, 4), 2, (0, 0, 255)),
         ]
 
         img = draw(img, shapes)
         assert (img == [255, 0, 0]).all(axis=2).any()
         assert (img == [0, 255, 0]).all(axis=2).any()
         assert (img == [0, 0, 255]).all(axis=2).any()
 
         assert not (img_copy == [255, 0, 0]).all(axis=2).any()
         assert not (img_copy == [0, 255, 0]).all(axis=2).any()
         assert not (img_copy == [0, 0, 255]).all(axis=2).any()
 
     def test_converts_to_type_expected_by_opencv(self):
         line = create_line([0.0, 0.0], [0.0, 3.0], (0, 255, 0), thickness=1)
-        assert isinstance(line['p1'], tuple)
-        assert isinstance(line['p2'], tuple)
-        assert all([isinstance(x, int) for x in line['p1'] + line['p2']])
+        assert isinstance(line["p1"], tuple)
+        assert isinstance(line["p2"], tuple)
+        assert all([isinstance(x, int) for x in line["p1"] + line["p2"]])
 
         rect = create_rectangle([1.0, 1.0], [3.0, 3.0], (255, 0, 0), thickness=-1)
-        assert isinstance(rect['p1'], tuple)
-        assert isinstance(rect['p2'], tuple)
-        assert all([isinstance(x, int) for x in rect['p1'] + rect['p2']])
+        assert isinstance(rect["p1"], tuple)
+        assert isinstance(rect["p2"], tuple)
+        assert all([isinstance(x, int) for x in rect["p1"] + rect["p2"]])
 
         circle = create_circle([4.0, 4.0], 2, (0, 0, 255))
-        assert isinstance(circle['center'], tuple)
-        assert all([isinstance(x, int) for x in circle['center']])
+        assert isinstance(circle["center"], tuple)
+        assert all([isinstance(x, int) for x in circle["center"]])
 
-        text = create_text('hello', [0.0, 50.0], (0, 255, 0))
-        assert isinstance(text['origin'], tuple)
-        assert all([isinstance(x, int) for x in text['origin']])
+        text = create_text("hello", [0.0, 50.0], (0, 255, 0))
+        assert isinstance(text["origin"], tuple)
+        assert all([isinstance(x, int) for x in text["origin"]])
 
         # This will raise an error if anything else goes wrong
         img = np.zeros((100, 100, 3), dtype=np.uint8)
         draw(img, [line, rect, circle, text])
 
     def test_maintains_order_if_sequence(self):
         data = [
-            create_line((0,0), (0,2), (0, 255, 0), thickness=1),
-            create_line((0,1), (0,3), (0, 0, 255), thickness=1),
+            create_line((0, 0), (0, 2), (0, 255, 0), thickness=1),
+            create_line((0, 1), (0, 3), (0, 0, 255), thickness=1),
         ]
-        expected = np.array([
-            [[0, 255, 0]],
-            [[0, 0, 255]],
-            [[0, 0, 255]],
-            [[0, 0, 255]],
-        ])
+        expected = np.array(
+            [
+                [[0, 255, 0]],
+                [[0, 0, 255]],
+                [[0, 0, 255]],
+                [[0, 0, 255]],
+            ]
+        )
 
         img = np.zeros((4, 1, 3), dtype=np.uint8)
         img = draw(img, copy.deepcopy(data))
         assert are_arrays_equal(img, expected)
 
-        expected = np.array([
-            [[0, 255, 0]],
-            [[0, 255, 0]],
-            [[0, 255, 0]],
-            [[0, 0, 255]],
-        ])
+        expected = np.array(
+            [
+                [[0, 255, 0]],
+                [[0, 255, 0]],
+                [[0, 255, 0]],
+                [[0, 0, 255]],
+            ]
+        )
 
         img = np.zeros((4, 1, 3), dtype=np.uint8)
         img = draw(img, data[::-1])
         assert are_arrays_equal(img, expected)
 
     def test_text_with_background_color(self):
         original = 255 * np.ones((100, 100, 3), dtype=np.uint8)
-        shape = create_text('hello', (0, 50), (0, 255, 0), bg=(255, 0, 255), bg_pad=(5, 10, 15, 20))
+        shape = create_text(
+            "hello", (0, 50), (0, 255, 0), bg=(255, 0, 255), bg_pad=(5, 10, 15, 20)
+        )
 
         processed = draw(original, shape)
         assert not are_arrays_equal(original, processed)
         assert (processed == (0, 255, 0)).any()
         assert (processed == (255, 0, 255)).any()
 
     def test_text_with_pad_but_without_bg_color(self):
         with pytest.raises(ValueError):
-            create_text('hello', (0, 50), (0, 255, 0), bg_pad=(5, 10, 15, 20))
+            create_text("hello", (0, 50), (0, 255, 0), bg_pad=(5, 10, 15, 20))
 
-    @pytest.mark.parametrize('pad', [(1,2,3), (1,2,3,4,5)])
+    @pytest.mark.parametrize("pad", [(1, 2, 3), (1, 2, 3, 4, 5)])
     def test_text_with_invalid_pad_values(self, pad):
         with pytest.raises(ValueError):
-            create_text('hello', (0, 50), (0, 255, 0), bg=(0,0,255), bg_pad=pad)
+            create_text("hello", (0, 50), (0, 255, 0), bg=(0, 0, 255), bg_pad=pad)
 
-    @pytest.mark.parametrize('pad', all_types_besides(['none', 'numbers', 'sequences']))
+    @pytest.mark.parametrize("pad", all_types_besides(["none", "numbers", "sequences"]))
     def test_text_with_invalid_pad_types(self, pad):
         with pytest.raises(TypeError):
-            create_text('hello', (0, 50), (0, 255, 0), bg=(0,0,255), bg_pad=pad)
+            create_text("hello", (0, 50), (0, 255, 0), bg=(0, 0, 255), bg_pad=pad)
 
-    @pytest.mark.parametrize('input_pad, expected_pad', [
-        (None, [5,5,5,5]),
-        (1, [1,1,1,1]),
-        ((1,2), [1,2,1,2]),
-        ((1,2,3,4), (1,2,3,4)),
-    ])
+    @pytest.mark.parametrize(
+        "input_pad, expected_pad",
+        [
+            (None, [5, 5, 5, 5]),
+            (1, [1, 1, 1, 1]),
+            ((1, 2), [1, 2, 1, 2]),
+            ((1, 2, 3, 4), (1, 2, 3, 4)),
+        ],
+    )
     def test_text_with_different_pad_values(self, input_pad, expected_pad):
-        shape = create_text('hello', (0, 50), (0, 255, 0), bg=(0,0,255), bg_pad=input_pad)
+        shape = create_text(
+            "hello", (0, 50), (0, 255, 0), bg=(0, 0, 255), bg_pad=input_pad
+        )
         assert shape == {
-            'type': 'text',
-            'text': 'hello',
-            'origin': (0, 50),
-            'color': (0, 255, 0),
-            'font': cv2.FONT_HERSHEY_SIMPLEX,
-            'font_scale': 1.25,
-            'thickness': 3,
-            'background': {
-                'color': (0, 0, 255),
-                'pad': expected_pad
-            },
+            "type": "text",
+            "text": "hello",
+            "origin": (0, 50),
+            "color": (0, 255, 0),
+            "font": cv2.FONT_HERSHEY_SIMPLEX,
+            "font_scale": 1.25,
+            "thickness": 3,
+            "background": {"color": (0, 0, 255), "pad": expected_pad},
         }
 
     def test_text_without_bg_color_or_pad(self):
-        shape = create_text('hello', (0, 50), (0, 255, 0))
+        shape = create_text("hello", (0, 50), (0, 255, 0))
         assert shape == {
-            'type': 'text',
-            'text': 'hello',
-            'origin': (0, 50),
-            'color': (0, 255, 0),
-            'font': cv2.FONT_HERSHEY_SIMPLEX,
-            'font_scale': 1.25,
-            'thickness': 3,
+            "type": "text",
+            "text": "hello",
+            "origin": (0, 50),
+            "color": (0, 255, 0),
+            "font": cv2.FONT_HERSHEY_SIMPLEX,
+            "font_scale": 1.25,
+            "thickness": 3,
         }
 
-    @pytest.mark.parametrize('shape', [
-        create_mask([(100,100), (250,250), (250,100), (150,200)], (0, 255, 0)),
-        create_mask([[(100,100), (250,250), (250,100), (150,200)], ((0,0), (0,1), (1,0), (2,0))], (0, 255, 0)),
-        create_mask(np.array([[(100,100), (250,250), (250,100), (150,200)]]), (0, 255, 0)),
-        create_mask(np.array([[(100,100), (250,250), (250,100), (150,200)]], dtype=np.uint8), (0, 255, 0)),
-        create_polylines([(100,100), (250,250), (250,100), (150,200)], (0, 255, 0)),
-        create_polylines([[(100,100), (250,250), (250,100), (150,200)], ((0,0), (0,1), (1,0), (2,0))], (0, 255, 0)),
-        create_polylines(np.array([[(100,100), (250,250), (250,100), (150,200)]]), (0, 255, 0)),
-        create_polylines(np.array([[(100,100), (250,250), (250,100), (150,200)]], dtype=np.uint8), (0, 255, 0)),
-    ])
+    @pytest.mark.parametrize(
+        "shape",
+        [
+            create_mask([(100, 100), (250, 250), (250, 100), (150, 200)], (0, 255, 0)),
+            create_mask(
+                [
+                    [(100, 100), (250, 250), (250, 100), (150, 200)],
+                    ((0, 0), (0, 1), (1, 0), (2, 0)),
+                ],
+                (0, 255, 0),
+            ),
+            create_mask(
+                np.array([[(100, 100), (250, 250), (250, 100), (150, 200)]]),
+                (0, 255, 0),
+            ),
+            create_mask(
+                np.array(
+                    [[(100, 100), (250, 250), (250, 100), (150, 200)]], dtype=np.uint8
+                ),
+                (0, 255, 0),
+            ),
+            create_polylines(
+                [(100, 100), (250, 250), (250, 100), (150, 200)], (0, 255, 0)
+            ),
+            create_polylines(
+                [
+                    [(100, 100), (250, 250), (250, 100), (150, 200)],
+                    ((0, 0), (0, 1), (1, 0), (2, 0)),
+                ],
+                (0, 255, 0),
+            ),
+            create_polylines(
+                np.array([[(100, 100), (250, 250), (250, 100), (150, 200)]]),
+                (0, 255, 0),
+            ),
+            create_polylines(
+                np.array(
+                    [[(100, 100), (250, 250), (250, 100), (150, 200)]], dtype=np.uint8
+                ),
+                (0, 255, 0),
+            ),
+        ],
+    )
     def test_masks_and_polylines(self, shape):
         original = 255 * np.ones((1000, 1000, 3), dtype=np.uint8)
         processed = draw(original, shape)
         assert not are_arrays_equal(original, processed)
 
 
 class Test_are_arrays_equal:
-    @pytest.mark.parametrize('img_1, img_2', [
-        (_create_RGB(), _create_RGB()),
-        (_create_RGB(np.float32), _create_RGB(np.uint8)),
-        (_create_RGB(np.float32), _create_RGB(np.uint8)),
-        (np.array([[0,1], [2,3]]), np.array([[0,1], [2,3]])),
-    ])
+    @pytest.mark.parametrize(
+        "img_1, img_2",
+        [
+            (_create_RGB(), _create_RGB()),
+            (_create_RGB(np.float32), _create_RGB(np.uint8)),
+            (_create_RGB(np.float32), _create_RGB(np.uint8)),
+            (np.array([[0, 1], [2, 3]]), np.array([[0, 1], [2, 3]])),
+        ],
+    )
     def test_equal(self, img_1, img_2):
         assert are_arrays_equal(img_1, img_2)
 
-    @pytest.mark.parametrize('img_1, img_2', [
-        (np.zeros((5, 5, 3)), np.zeros((5, 5))),
-        (np.array([[1, 2], [3, 4]]), np.array([[3, 4], [1, 2]])),
-    ])
+    @pytest.mark.parametrize(
+        "img_1, img_2",
+        [
+            (np.zeros((5, 5, 3)), np.zeros((5, 5))),
+            (np.array([[1, 2], [3, 4]]), np.array([[3, 4], [1, 2]])),
+        ],
+    )
     def test_not_equal(self, img_1, img_2):
         assert not are_arrays_equal(img_1, img_2)
 
     def test_not_equal_type(self):
         assert not are_arrays_equal(
-            _create_RGB(np.float32),
-            _create_RGB(np.uint8),
-            check_type=True
+            _create_RGB(np.float32), _create_RGB(np.uint8), check_type=True
         )
 
 
 class Test_load_and_save:
     def test_atomicity_interrupt(self):
-        path = get_unique_path('{}.png')
+        path = get_unique_path("{}.png")
         data = _create_RGB()
 
         save_image.__katalytic_test_atomicity_interrupt__ = True
         save_image(data, path)
         assert not Path(path).exists()
 
         # make sure it's still working after the test
         # the atomicity flag is set back to False inside the function
         save_image(data, path)
         assert are_arrays_equal(load(path), data)
 
     def test_atomicity_race_condition_error(self):
-        path = get_unique_path('{}.png')
+        path = get_unique_path("{}.png")
         data = _create_RGB()
 
         save_image.__katalytic_test_atomicity_race_condition__ = True
         assert not Path(path).exists()
         with pytest.raises(FileExistsError):
-            save_image(data, path, exists='error')
+            save_image(data, path, exists="error")
 
-        expected = np.array([[[0,255,0]]], dtype=np.uint8)
+        expected = np.array([[[0, 255, 0]]], dtype=np.uint8)
         assert are_arrays_equal(load(path), expected)
 
         # make sure it's still working after the test
         # the atomicity flag is set back to False inside the function
         delete_file(path)
         assert not Path(path).exists()
-        save_image(data, path, exists='error')
+        save_image(data, path, exists="error")
         assert are_arrays_equal(load(path), data)
 
     def test_atomicity_race_condition_replace(self):
-        path = get_unique_path('{}.png')
+        path = get_unique_path("{}.png")
         data = _create_RGB()
 
         save_image.__katalytic_test_atomicity_race_condition__ = True
         assert not Path(path).exists()
-        save_image(data, path, exists='replace')
+        save_image(data, path, exists="replace")
         assert are_arrays_equal(load(path), data)
 
         # make sure it's still working after the test
         # the atomicity flag is set back to False inside the function
         delete_file(path)
         assert not Path(path).exists()
-        save_image(data, path, exists='replace')
+        save_image(data, path, exists="replace")
         assert are_arrays_equal(load(path), data)
 
     def test_atomicity_race_condition_skip(self):
-        path = get_unique_path('{}.png')
+        path = get_unique_path("{}.png")
         data = _create_RGB()
 
         save_image.__katalytic_test_atomicity_race_condition__ = True
         assert not Path(path).exists()
-        save_image(data, path, exists='skip')
-        expected = np.array([[[0,255,0]]], dtype=np.uint8)
+        save_image(data, path, exists="skip")
+        expected = np.array([[[0, 255, 0]]], dtype=np.uint8)
         assert are_arrays_equal(load(path), expected)
 
         # make sure it's still working after the test
         # the atomicity flag is set back to False inside the function
         delete_file(path)
         assert not Path(path).exists()
-        save_image(data, path, exists='skip')
+        save_image(data, path, exists="skip")
         assert are_arrays_equal(load(path), data)
 
     # noinspection PyBroadException
-    @pytest.mark.parametrize('ext, wrong_load, correct_load', [
-        ('jpeg', load_csv, 'load_image'),
-        ('jpg', load_json, 'load_image'),
-        ('png', load_text, 'load_image'),
-    ])
-    def test_using_the_wrong_loader_should_always_warn(self, ext, wrong_load, correct_load):
+    @pytest.mark.parametrize(
+        "ext, wrong_load, correct_load",
+        [
+            ("jpeg", load_csv, "load_image"),
+            ("jpg", load_json, "load_image"),
+            ("png", load_text, "load_image"),
+        ],
+    )
+    def test_using_the_wrong_loader_should_always_warn(
+        self, ext, wrong_load, correct_load
+    ):
         # The warning should be triggered regardless of whether the file exists or not.
-        with pytest.warns(UserWarning, match=f'Use "{correct_load}" for ".{ext}" files.'):
+        with pytest.warns(
+            UserWarning, match=f'Use "{correct_load}" for ".{ext}" files.'
+        ):
             try:
-                wrong_load(get_unique_path('{}.' + ext))
+                wrong_load(get_unique_path("{}." + ext))
             except Exception:
                 pass
 
     # noinspection PyBroadException
-    @pytest.mark.parametrize('ext, wrong_save, correct_save', [
-        ('jpeg', save_csv, 'save_image'),
-        ('jpg', save_json, 'save_image'),
-        ('png', save_text, 'save_image'),
-    ])
-    def test_using_the_wrong_saver_should_always_warn(self, ext, wrong_save, correct_save):
-        with pytest.warns(UserWarning, match=f'Use "{correct_save}" for ".{ext}" files.'):
+    @pytest.mark.parametrize(
+        "ext, wrong_save, correct_save",
+        [
+            ("jpeg", save_csv, "save_image"),
+            ("jpg", save_json, "save_image"),
+            ("png", save_text, "save_image"),
+        ],
+    )
+    def test_using_the_wrong_saver_should_always_warn(
+        self, ext, wrong_save, correct_save
+    ):
+        with pytest.warns(
+            UserWarning, match=f'Use "{correct_save}" for ".{ext}" files.'
+        ):
             try:
-                wrong_save(_create_RGB(), get_unique_path('{}.' + ext))
+                wrong_save(_create_RGB(), get_unique_path("{}." + ext))
             except Exception:
                 pass
 
     def test_str(self):
         image_1 = _create_RGB()
-        path = get_unique_path('{}.png')
+        path = get_unique_path("{}.png")
         save_image(image_1, path)
         assert are_arrays_equal(image_1, load_image(path))
 
     def test_Path(self):
         image_1 = _create_RGB()
-        path = Path(get_unique_path('{}.png'))
+        path = Path(get_unique_path("{}.png"))
         save_image(image_1, path)
         assert are_arrays_equal(image_1, load_image(path))
 
     def test_save_PIL_Image(self):
         image_1 = _create_RGB()
-        path = Path(get_unique_path('{}.png'))
+        path = Path(get_unique_path("{}.png"))
         save_image(Image.fromarray(image_1), path)
         assert are_arrays_equal(image_1, load_image(path))
 
     def test_load_PIL_Image(self):
         image_1 = _create_RGB()
-        path = Path(get_unique_path('{}.png'))
+        path = Path(get_unique_path("{}.png"))
         save_image(image_1, path)
 
         image_2 = load_image(Image.fromarray(image_1))
         assert are_arrays_equal(image_1, np.array(image_2))
         assert isinstance(image_2, PIL.Image.Image)
 
     def test_load_returns_copy(self):
         img = _create_RGB()
         img_copy = load_image(img)
         img[0][0] = [255, 255, 255]
         assert not are_arrays_equal(img, img_copy)
 
     def test_path_exists_replace(self):
-        path = get_unique_path('{}.png')
+        path = get_unique_path("{}.png")
         Path(path).touch()
 
         img = _create_RGB()
-        save_image(img, path, exists='replace')
+        save_image(img, path, exists="replace")
         assert are_arrays_equal(load_image(path), img)
 
     def test_save_uses_copy_file(self):
-        path = get_unique_path('{}.png')
+        path = get_unique_path("{}.png")
         save_image(_create_RGB(), path)
 
-        path2 = get_unique_path('{}.png')
-        save_image(path, path2, exists='replace')
+        path2 = get_unique_path("{}.png")
+        save_image(path, path2, exists="replace")
 
         assert are_arrays_equal(load_image(path2), load_image(path))
 
     def test_path_exists_skip(self):
-        path = get_unique_path('{}.png')
+        path = get_unique_path("{}.png")
         img = _create_RGB()
         save_image(img, path)
 
-        img2 = convert_image(img, 'RGB', 'BGR')
-        save_image(img2, path, exists='skip')
+        img2 = convert_image(img, "RGB", "BGR")
+        save_image(img2, path, exists="skip")
         assert not are_arrays_equal(load_image(path), img2)
 
     def test_path_exists_error(self):
-        path = get_unique_path('{}.png')
+        path = get_unique_path("{}.png")
         Path(path).touch()
 
         with pytest.raises(FileExistsError):
-            save_image(_create_RGB(), path, exists='error')
+            save_image(_create_RGB(), path, exists="error")
 
     def test_universal_load_and_save(self):
-        path = get_unique_path('{}.png')
+        path = get_unique_path("{}.png")
         img = _create_RGB()
         save(img, path)
         assert are_arrays_equal(load(path), img)
 
     def test_default(self):
-        path = get_unique_path('{}.png')
+        path = get_unique_path("{}.png")
         img = load_image(path, default=_create_RGB())
         assert are_arrays_equal(img, _create_RGB())
 
     def test_make_dirs_False(self):
         img = _create_RGB()
-        path = get_unique_path('{}/data.png')
+        path = get_unique_path("{}/data.png")
         with pytest.raises(FileNotFoundError):
             save_image(img, path, make_dirs=False)
 
         # save image, then move it to a filename without extension
-        path = get_unique_path('{}/data')
-        save_image(img, f'{path}.png', make_dirs=True)
-        move_file(f'{path}.png', path)
+        path = get_unique_path("{}/data")
+        save_image(img, f"{path}.png", make_dirs=True)
+        move_file(f"{path}.png", path)
 
         # then try to use that filename as a directory
         with pytest.raises(NotADirectoryError):
-            save_image(img, f'{path}/x.png', make_dirs=False)
+            save_image(img, f"{path}/x.png", make_dirs=False)
 
-    @pytest.mark.parametrize('img', [1, True, None, [], {}, (), object()])
+    @pytest.mark.parametrize("img", [1, True, None, [], {}, (), object()])
     def test_load_raises_TypeError_for_image(self, img):
         with pytest.raises(TypeError):
             load_image(img)
 
-    @pytest.mark.parametrize('mode', [1, True, [], {}, (), object()])
+    @pytest.mark.parametrize("mode", [1, True, [], {}, (), object()])
     def test_load_raises_TypeError_for_mode(self, mode):
         with pytest.raises(TypeError):
-            load_image('img.png', mode)
+            load_image("img.png", mode)
 
-    @pytest.mark.parametrize('path', [1, True, None, [], {}, (), object()])
+    @pytest.mark.parametrize("path", [1, True, None, [], {}, (), object()])
     def test_save_raises_TypeError_for_path(self, path):
         with pytest.raises(TypeError):
             save_image(_create_RGB(), path)
 
-    @pytest.mark.parametrize('image', [1, True, None, [], {}, (), object()])
+    @pytest.mark.parametrize("image", [1, True, None, [], {}, (), object()])
     def test_save_raises_TypeError_for_image(self, image):
         with pytest.raises(TypeError):
-            save_image(image, get_unique_path('{}.png'))
+            save_image(image, get_unique_path("{}.png"))
 
-    @pytest.mark.parametrize('mode', [1, True, None, [], {}, (), object()])
+    @pytest.mark.parametrize("mode", [1, True, None, [], {}, (), object()])
     def test_save_raises_ValueError_for_mode(self, mode):
         with pytest.raises(TypeError):
-            save_image(_create_RGB(), get_unique_path('{}.png'), mode=mode)
+            save_image(_create_RGB(), get_unique_path("{}.png"), mode=mode)
 
-    @pytest.mark.parametrize('exists', ['unkonwn', '', 1, True, None, [], {}, (), object()])
+    @pytest.mark.parametrize(
+        "exists", ["unkonwn", "", 1, True, None, [], {}, (), object()]
+    )
     def test_save_raises_ValueError_for_exists(self, exists):
         with pytest.raises(ValueError):
-            save_image(_create_RGB(), get_unique_path('{}.png'), exists=exists)
+            save_image(_create_RGB(), get_unique_path("{}.png"), exists=exists)
```

### Comparing `katalytic_images-0.9.1/PKG-INFO` & `katalytic_images-0.9.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-images
-Version: 0.9.1
+Version: 0.9.4
 Summary: This plugin adds utilities for working with images and videos to the katalytic namespace
 Author-Email: Valentin Neagu <vali19th@protonmail.com>
 License: Copyright 2023 - present, Valentin Neagu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -25,16 +25,17 @@
 Classifier: Topic :: Utilities
 Project-URL: Changelog, https://gitlab.com/katalytic/katalytic-images/-/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://gitlab.com/katalytic/katalytic-images.git
 Project-URL: Repository, https://gitlab.com/katalytic/katalytic-images.git
 Requires-Python: >=3.6
 Requires-Dist: katalytic>=0.2.2
 Requires-Dist: numpy>=1.14
-Requires-Dist: opencv-python>=4.0.0
 Requires-Dist: pillow>=8.4.0
+Requires-Dist: black; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-clarity; extra == "dev"
 Requires-Dist: pytest-randomly; extra == "dev"
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
@@ -50,22 +51,23 @@
 - The functions accept numpy arrays and Pillow images as input and return the same type
 - defining the shapes to be drawn on top of an image in a declarative way as a list of dicts and passing it to draw()
 - Many more (TODO: Link to tocs)
 
 ## Example (TODO)
 
 ## Installation
-By itself
+First, install opencv
 ```bash
-pip install katalytic-images
+if [[ ! $(pip freeze | grep -Pi 'opencv') ]]; then 
+    pip install opencv-python 
+fi
 ```
-
-As part of the [katalytic](https://gitlab.com/katalytic/katalytic) collection
+Then, install this package
 ```bash
-pip install katalytic
+pip install katalytic-images
 ```
 
 ## Roadmap
 - make pillow an optional dependency.
    - setup_load_image() should pick opencv if pillow is not available
 - image thresholding and masking operations
 - interactive data exploration widgets (maybe as part of another package)
@@ -75,8 +77,7 @@
 ## Contributing
 We appreciate any form of contribution, including but not limited to:
 - **Code contributions**: Enhance our repository with your code and tests.
 - **Feature suggestions**: Your ideas can shape the future development of our package.
 - **Architectural improvements**: Help us optimize our system's design and API.
 - **Bug fixes**: Improve user experience by reporting or resolving issues.
 - **Documentation**: Help us maintain clear and up-to-date instructions for users.
-
```

