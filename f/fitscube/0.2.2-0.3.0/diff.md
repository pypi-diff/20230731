# Comparing `tmp/fitscube-0.2.2.tar.gz` & `tmp/fitscube-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitscube-0.2.2.tar", max compression
+gzip compressed data, was "fitscube-0.3.0.tar", max compression
```

## Comparing `fitscube-0.2.2.tar` & `fitscube-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1069 2022-11-30 13:17:10.782939 fitscube-0.2.2/LICENSE
--rw-r--r--   0        0        0     3410 2023-01-23 02:16:47.847865 fitscube-0.2.2/README.md
--rw-r--r--   0        0        0      140 2023-02-28 08:10:06.143488 fitscube-0.2.2/fitscube/__init__.py
--rw-r--r--   0        0        0     8900 2023-02-28 08:10:10.841507 fitscube-0.2.2/fitscube/fitscube.py
--rw-r--r--   0        0        0     4087 2023-02-28 08:10:10.328900 fitscube-0.2.2/fitscube/stokescube.py
--rw-r--r--   0        0        0      443 2023-02-28 08:11:09.936964 fitscube-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4325 1970-01-01 00:00:00.000000 fitscube-0.2.2/setup.py
--rw-r--r--   0        0        0     4024 1970-01-01 00:00:00.000000 fitscube-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-11-30 13:17:10.782000 fitscube-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3481 2023-07-31 08:59:54.128122 fitscube-0.3.0/README.md
+-rw-r--r--   0        0        0      124 2023-07-31 08:59:54.128719 fitscube-0.3.0/fitscube/__init__.py
+-rw-r--r--   0        0        0    12083 2023-07-31 08:59:54.129447 fitscube-0.3.0/fitscube/fitscube.py
+-rw-r--r--   0        0        0     4106 2023-07-31 08:59:54.130057 fitscube-0.3.0/fitscube/stokescube.py
+-rw-r--r--   0        0        0      443 2023-07-31 09:00:02.613665 fitscube-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4095 1970-01-01 00:00:00.000000 fitscube-0.3.0/PKG-INFO
```

### Comparing `fitscube-0.2.2/LICENSE` & `fitscube-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fitscube-0.2.2/README.md` & `fitscube-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,49 +24,50 @@
 ```
 
 ## Usage
 
 Command line:
 ```bash
 fitscube -h
-# usage: fitscube [-h] [-o] [--freq-file FREQ_FILE | --freqs FREQS [FREQS ...] | --ignore-freq] file_list [file_list ...] out_cube
+# usage: fitscube [-h] [-o] [--create-blanks] [--freq-file FREQ_FILE | --freqs FREQS [FREQS ...] | --ignore-freq] file_list [file_list ...] out_cube
 
-# Fitscube: Combine single-frequency FITS files into a cube. Assumes: - All files have the same WCS - All files have the same shape / pixel grid -
-# Frequency is either a WCS axis or in the REFFREQ header keyword - All the relevant information is in the first header of the first image
+# Fitscube: Combine single-frequency FITS files into a cube. Assumes: - All files have the same WCS - All files have the same shape / pixel grid - Frequency is either a WCS
+# axis or in the REFFREQ header keyword - All the relevant information is in the first header of the first image
 
 # positional arguments:
 #   file_list             List of FITS files to combine (in frequency order)
 #   out_cube              Output FITS file
 
-# optional arguments:
+# options:
 #   -h, --help            show this help message and exit
 #   -o, --overwrite       Overwrite output file if it exists
+#   --create-blanks       Try to create a blank cube with evenly spaced frequencies
 #   --freq-file FREQ_FILE
 #                         File containing frequencies in Hz
 #   --freqs FREQS [FREQS ...]
 #                         List of frequencies in Hz
 #   --ignore-freq         Ignore frequency information and just stack (probably not what you want)
 
 stokescube -h
-# usage: stokescube [-h] [-v STOKES_V_FILE] [--overwrite] stokes_I_file stokes_Q_file stokes_U_file output_file
+# usage: stokescube [-h] [-v STOKES_V_FILE] [-o] stokes_I_file stokes_Q_file stokes_U_file output_file
 
-# Fitscube: Combine single-Stokes FITS files into a Stokes cube. Assumes: - All files have the same WCS - All files have the same shape / pixel
-# grid - All the relevant information is in the first header of the first image
+# Fitscube: Combine single-Stokes FITS files into a Stokes cube. Assumes: - All files have the same WCS - All files have the same shape / pixel grid - All the relevant
+# information is in the first header of the first image
 
 # positional arguments:
 #   stokes_I_file         Stokes I file
 #   stokes_Q_file         Stokes Q file
 #   stokes_U_file         Stokes U file
 #   output_file           Output file
 
-# optional arguments:
+# options:
 #   -h, --help            show this help message and exit
 #   -v STOKES_V_FILE, --stokes_V_file STOKES_V_FILE
 #                         Stokes V file
-#   --overwrite           Overwrite output file if it exists
+#   -o, --overwrite       Overwrite output file if it exists
 ```
 
 Python:
 ```python
 from fitscube import combine_fits, combine_stokes
 
 hdu_list, frequencies = combine_fits(
```

### Comparing `fitscube-0.2.2/fitscube/fitscube.py` & `fitscube-0.3.0/fitscube/fitscube.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,26 +6,104 @@
 - All files have the same shape / pixel grid
 - Frequency is either a WCS axis or in the REFFREQ header keyword
 - All the relevant information is in the first header of the first image
 
 """
 
 import os
-from collections import namedtuple
-from typing import List, Tuple, Union
+from typing import List, NamedTuple, Optional, Tuple, Union
 
 import astropy.units as u
 import numpy as np
 from astropy.io import fits
 from astropy.wcs import WCS
 from tqdm.auto import tqdm
 
-InitResult = namedtuple(
-    "InitResult", ["data_cube", "header", "idx", "fits_idx", "is_2d"]
-)
+
+class InitResult(NamedTuple):
+    data_cube: np.ndarray
+    """Output data cube"""
+    header: fits.Header
+    """Output header"""
+    idx: int
+    """Index of frequency axis"""
+    fits_idx: int
+    """FITS index of frequency axis"""
+    is_2d: bool
+    """Whether the input is 2D"""
+
+
+def isin_close(element: np.ndarray, test_element: np.ndarray) -> np.ndarray:
+    """Check if element is in test_element, within a tolerance.
+
+    Args:
+        element (np.ndarray): Element to check
+        test_element (np.ndarray): Element to check against
+
+    Returns:
+        np.ndarray: Boolean array
+    """
+    return np.isclose(element[:, None], test_element).any(1)
+
+
+def even_spacing(freqs: u.Quantity) -> Tuple[u.Quantity, np.ndarray]:
+    """Make the frequencies evenly spaced.
+
+    Args:
+        freqs (u.Quantity): Original frequencies
+
+    Returns:
+        Tuple[u.Quantity, np.ndarray]: Evenly spaced frequencies and missing channel indices
+    """    
+    freqs_arr = freqs.value.astype(np.longdouble)
+    diffs = np.diff(freqs_arr)
+    min_diff = np.min(diffs)
+    # Create a new array with the minimum difference
+    new_freqs = np.arange(freqs_arr[0], freqs_arr[-1], min_diff)
+    missing_chan_idx = ~isin_close(new_freqs, freqs_arr)
+    
+    return new_freqs * freqs.unit, missing_chan_idx
+
+
+def create_blank_data(
+    data_cube: np.ndarray,
+    freqs: u.Quantity,
+    idx: int,
+) -> Tuple[Optional[np.ndarray], u.Quantity]:
+    """Create a new data cube with evenly spaced frequencies, and fill in the missing channels with NaNs.
+
+    Args:
+        data_cube (np.ndarray): Original data cube
+        freqs (u.Quantity): Original frequencies
+        idx: Index of frequency axis
+
+    Returns:
+        Tuple[Optional[np.ndarray], u.Quantity]: New data cube and frequencies
+    """
+    new_freqs, missing_chan_idx = even_spacing(freqs)
+    # Check if all frequencies present
+    all_there = isin_close(freqs, new_freqs).all()
+    if not all_there:
+        return None, new_freqs
+
+    # Create a new data cube with the new frequencies
+    new_shape = list(data_cube.shape)
+    new_shape[idx] = len(new_freqs)
+    new_data_cube = np.empty(new_shape) * np.nan
+    for old_chan, freq in enumerate(freqs):
+        new_chans = np.where(np.isclose(new_freqs, freq))[0]
+        assert len(new_chans) == 1, "Too many matching channels"
+        new_chan = new_chans[0]
+        new_slice = [slice(None)] * len(new_shape)
+        new_slice[idx] = new_chan
+        old_slice = [slice(None)] * len(new_shape)
+        old_slice[idx] = old_chan
+        new_data_cube[tuple(new_slice)] = data_cube[tuple(old_slice)]
+
+    return new_data_cube, new_freqs
 
 
 def init_cube(
     old_name: str,
     n_chan: int,
 ) -> InitResult:
     """Initialize the data cube.
@@ -127,19 +205,20 @@
                     raise ValueError(
                         "No FREQ axis found in WCS. Cannot combine ND images without frequency information."
                     ) from e
 
     return freqs
 
 
-def main(
+def combine_fits(
     file_list: List[str],
     freq_file: Union[str, None] = None,
     freq_list: Union[List[float], None] = None,
     ignore_freq: bool = False,
+    create_blanks: bool = False,
 ) -> Tuple[fits.HDUList, u.Quantity]:
     """Combine FITS files into a cube.
 
     Args:
         file_list (List[str]): List of FITS files to combine
         overwrite (bool, optional): Whether to overwrite output cube. Defaults to False.
 
@@ -193,14 +272,26 @@
         if is_2d:
             slicer.insert(0, chan)
         else:
             slicer[idx] = chan
         data_cube[tuple(slicer)] = plane
     # Write out cubes
     even_freq = np.diff(freqs).std() < 1e-6 * u.Hz
+    if not even_freq and create_blanks:
+        print("Trying to create a blank cube with evenly spaced frequencies")
+        new_data_cube, new_freqs = create_blank_data(
+            data_cube=data_cube,
+            freqs=freqs,
+            idx=idx,
+        )
+        if new_data_cube is not None:
+            even_freq = True
+            data_cube = new_data_cube
+            freqs = new_freqs
+
     if not even_freq:
         print("WARNING: Frequencies are not evenly spaced")
         print("Use the frequency file to specify the frequencies")
 
     new_header = old_header.copy()
     wcs = WCS(old_header)
     new_header["NAXIS"] = len(data_cube.shape)
@@ -231,14 +322,19 @@
     parser.add_argument("out_cube", help="Output FITS file")
     parser.add_argument(
         "-o",
         "--overwrite",
         action="store_true",
         help="Overwrite output file if it exists",
     )
+    parser.add_argument(
+        "--create-blanks",
+        action="store_true",
+        help="Try to create a blank cube with evenly spaced frequencies",
+    )
     # Add options for specifying frequencies
     group = parser.add_mutually_exclusive_group()
     group.add_argument(
         "--freq-file",
         help="File containing frequencies in Hz",
         type=str,
         default=None,
@@ -270,19 +366,20 @@
         raise FileExistsError(
             f"Output file {freqs_file} already exists. Use --overwrite to overwrite."
         )
 
     if overwrite:
         print("Overwriting output files")
 
-    hdul, freqs = main(
+    hdul, freqs = combine_fits(
         file_list=args.file_list,
         freq_file=args.freq_file,
         freq_list=args.freqs,
         ignore_freq=args.ignore_freq,
+        create_blanks=args.create_blanks,
     )
 
     hdul.writeto(out_cube, overwrite=overwrite)
     print(f"Written cube to {out_cube}")
     np.savetxt(freqs_file, freqs.to(u.Hz).value)
     print(f"Written frequencies to {freqs_file}")
```

### Comparing `fitscube-0.2.2/fitscube/stokescube.py` & `fitscube-0.3.0/fitscube/stokescube.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,20 @@
 from typing import List, Tuple, Union
 
 import numpy as np
 from astropy.io import fits
 from astropy.wcs import WCS
 
 
-def main(
+def combine_stokes(
     stokes_I_file: str,
     stokes_Q_file: str,
     stokes_U_file: str,
     stokes_V_file: Union[str, None] = None,
 ) -> fits.HDUList:
-
     # Read in the data
     stokes_I = fits.getdata(stokes_I_file)
     stokes_Q = fits.getdata(stokes_Q_file)
     stokes_U = fits.getdata(stokes_U_file)
     if stokes_V_file is not None:
         stokes_V = fits.getdata(stokes_V_file)
 
@@ -111,15 +110,15 @@
     overwrite = args.overwrite
     output_file = args.output_file
     if not overwrite and os.path.exists(output_file):
         raise FileExistsError(
             f"Output file {output_file} already exists. Use --overwrite to overwrite."
         )
 
-    hdul = main(
+    hdul = combine_stokes(
         stokes_I_file=args.stokes_I_file,
         stokes_Q_file=args.stokes_Q_file,
         stokes_U_file=args.stokes_U_file,
         stokes_V_file=args.stokes_V_file,
     )
     hdul.writeto(output_file, overwrite=overwrite)
     print(f"Written cube to {output_file}")
```

### Comparing `fitscube-0.2.2/setup.py` & `fitscube-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,114 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['fitscube']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['astropy>=5.0,<6.0', 'numpy>=1.20,<2.0', 'tqdm']
-
-entry_points = \
-{'console_scripts': ['fitscube = fitscube.fitscube:cli',
-                     'stokescube = fitscube.stokescube:cli']}
-
-setup_kwargs = {
-    'name': 'fitscube',
-    'version': '0.2.2',
-    'description': '',
-    'long_description': "# FITSCUBE\n\nFrom the [wsclean](https://wsclean.readthedocs.io/) docs:\n> WSClean does not output these images in a normal “imaging cube” like CASA does, i.e., a single fits file with several images in it. For now I’ve decided not to implement this (one of the reasons for this is that information about the synthesized beam is not properly stored in a multi-frequency fits file). One has of course the option to combine the output manually, e.g. with a simple Python script.\n\nThis is a simple Python script to combine (single-frequency or single-Stokes) FITS images manually.\n\nCurrent assumptions:\n- All files have the same WCS\n- All files have the same shape / pixel grid\n- Frequency is either a WCS axis or in the REFFREQ header keyword\n- All the relevant information is in the first header of the first image\n\n## Installation\n\nInstall from PyPI (stable):\n```\npip install fitscube\n```\n\nOr, onstall from this git repo (latest):\n```bash\npip install git+https://github.com/AlecThomson/fitscube.git\n```\n\n## Usage\n\nCommand line:\n```bash\nfitscube -h\n# usage: fitscube [-h] [-o] [--freq-file FREQ_FILE | --freqs FREQS [FREQS ...] | --ignore-freq] file_list [file_list ...] out_cube\n\n# Fitscube: Combine single-frequency FITS files into a cube. Assumes: - All files have the same WCS - All files have the same shape / pixel grid -\n# Frequency is either a WCS axis or in the REFFREQ header keyword - All the relevant information is in the first header of the first image\n\n# positional arguments:\n#   file_list             List of FITS files to combine (in frequency order)\n#   out_cube              Output FITS file\n\n# optional arguments:\n#   -h, --help            show this help message and exit\n#   -o, --overwrite       Overwrite output file if it exists\n#   --freq-file FREQ_FILE\n#                         File containing frequencies in Hz\n#   --freqs FREQS [FREQS ...]\n#                         List of frequencies in Hz\n#   --ignore-freq         Ignore frequency information and just stack (probably not what you want)\n\nstokescube -h\n# usage: stokescube [-h] [-v STOKES_V_FILE] [--overwrite] stokes_I_file stokes_Q_file stokes_U_file output_file\n\n# Fitscube: Combine single-Stokes FITS files into a Stokes cube. Assumes: - All files have the same WCS - All files have the same shape / pixel\n# grid - All the relevant information is in the first header of the first image\n\n# positional arguments:\n#   stokes_I_file         Stokes I file\n#   stokes_Q_file         Stokes Q file\n#   stokes_U_file         Stokes U file\n#   output_file           Output file\n\n# optional arguments:\n#   -h, --help            show this help message and exit\n#   -v STOKES_V_FILE, --stokes_V_file STOKES_V_FILE\n#                         Stokes V file\n#   --overwrite           Overwrite output file if it exists\n```\n\nPython:\n```python\nfrom fitscube import combine_fits, combine_stokes\n\nhdu_list, frequencies = combine_fits(\n    ['file1.fits', 'file2.fits', 'file3.fits'],\n)\nhdus_list = combine_stokes(\n    'stokes_I.fits',\n    'stokes_Q.fits',\n    'stokes_U.fits',\n)\n\n```\n\n## Convolving to a common resolution\nSee [RACS-Tools](https://github.com/AlecThomson/RACS-tools).\n\n## License\nMIT\n\n## Contributing\nContributions are welcome. Please open an issue or pull request.\n\n## TODO\n- [ ] Add support for non-frequency axes\n- [ ] Add tracking of the PSF in header / beamtable\n- [ ] Add convolution to a common resolution via RACS-Tools",
-    'author': 'Thomson, Alec (S&A, Kensington)',
-    'author_email': 'AlecThomson@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: fitscube
+Version: 0.3.0
+Summary: 
+Author: Thomson, Alec (S&A, Kensington)
+Author-email: AlecThomson@users.noreply.github.com
+Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: astropy (>=5.0,<6.0)
+Requires-Dist: numpy (>=1.20,<2.0)
+Requires-Dist: tqdm
+Description-Content-Type: text/markdown
+
+# FITSCUBE
+
+From the [wsclean](https://wsclean.readthedocs.io/) docs:
+> WSClean does not output these images in a normal “imaging cube” like CASA does, i.e., a single fits file with several images in it. For now I’ve decided not to implement this (one of the reasons for this is that information about the synthesized beam is not properly stored in a multi-frequency fits file). One has of course the option to combine the output manually, e.g. with a simple Python script.
+
+This is a simple Python script to combine (single-frequency or single-Stokes) FITS images manually.
+
+Current assumptions:
+- All files have the same WCS
+- All files have the same shape / pixel grid
+- Frequency is either a WCS axis or in the REFFREQ header keyword
+- All the relevant information is in the first header of the first image
+
+## Installation
+
+Install from PyPI (stable):
+```
+pip install fitscube
+```
+
+Or, onstall from this git repo (latest):
+```bash
+pip install git+https://github.com/AlecThomson/fitscube.git
+```
+
+## Usage
+
+Command line:
+```bash
+fitscube -h
+# usage: fitscube [-h] [-o] [--create-blanks] [--freq-file FREQ_FILE | --freqs FREQS [FREQS ...] | --ignore-freq] file_list [file_list ...] out_cube
+
+# Fitscube: Combine single-frequency FITS files into a cube. Assumes: - All files have the same WCS - All files have the same shape / pixel grid - Frequency is either a WCS
+# axis or in the REFFREQ header keyword - All the relevant information is in the first header of the first image
+
+# positional arguments:
+#   file_list             List of FITS files to combine (in frequency order)
+#   out_cube              Output FITS file
+
+# options:
+#   -h, --help            show this help message and exit
+#   -o, --overwrite       Overwrite output file if it exists
+#   --create-blanks       Try to create a blank cube with evenly spaced frequencies
+#   --freq-file FREQ_FILE
+#                         File containing frequencies in Hz
+#   --freqs FREQS [FREQS ...]
+#                         List of frequencies in Hz
+#   --ignore-freq         Ignore frequency information and just stack (probably not what you want)
+
+stokescube -h
+# usage: stokescube [-h] [-v STOKES_V_FILE] [-o] stokes_I_file stokes_Q_file stokes_U_file output_file
+
+# Fitscube: Combine single-Stokes FITS files into a Stokes cube. Assumes: - All files have the same WCS - All files have the same shape / pixel grid - All the relevant
+# information is in the first header of the first image
+
+# positional arguments:
+#   stokes_I_file         Stokes I file
+#   stokes_Q_file         Stokes Q file
+#   stokes_U_file         Stokes U file
+#   output_file           Output file
+
+# options:
+#   -h, --help            show this help message and exit
+#   -v STOKES_V_FILE, --stokes_V_file STOKES_V_FILE
+#                         Stokes V file
+#   -o, --overwrite       Overwrite output file if it exists
+```
+
+Python:
+```python
+from fitscube import combine_fits, combine_stokes
+
+hdu_list, frequencies = combine_fits(
+    ['file1.fits', 'file2.fits', 'file3.fits'],
+)
+hdus_list = combine_stokes(
+    'stokes_I.fits',
+    'stokes_Q.fits',
+    'stokes_U.fits',
+)
+
+```
+
+## Convolving to a common resolution
+See [RACS-Tools](https://github.com/AlecThomson/RACS-tools).
+
+## License
+MIT
+
+## Contributing
+Contributions are welcome. Please open an issue or pull request.
+
+## TODO
+- [ ] Add support for non-frequency axes
+- [ ] Add tracking of the PSF in header / beamtable
+- [ ] Add convolution to a common resolution via RACS-Tools
```

