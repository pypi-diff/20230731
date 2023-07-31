# Comparing `tmp/exotic-miri-0.0.1.tar.gz` & `tmp/exotic-miri-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exotic-miri-0.0.1.tar", last modified: Thu Apr 14 14:52:31 2022, max compression
+gzip compressed data, was "exotic-miri-1.0.0.tar", last modified: Mon Jul 31 09:41:56 2023, max compression
```

## Comparing `exotic-miri-0.0.1.tar` & `exotic-miri-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,41 @@
-drwxr-xr-x   0 davidgrant   (501) staff       (20)        0 2022-04-14 14:52:31.874854 exotic-miri-0.0.1/
--rw-r--r--   0 davidgrant   (501) staff       (20)     1064 2022-02-11 14:06:52.000000 exotic-miri-0.0.1/LICENSE
--rw-r--r--   0 davidgrant   (501) staff       (20)     1240 2022-04-14 14:52:31.874498 exotic-miri-0.0.1/PKG-INFO
--rw-r--r--   0 davidgrant   (501) staff       (20)      571 2022-04-14 14:36:20.000000 exotic-miri-0.0.1/README.rst
-drwxr-xr-x   0 davidgrant   (501) staff       (20)        0 2022-04-14 14:52:31.860681 exotic-miri-0.0.1/exotic_miri/
--rw-r--r--   0 davidgrant   (501) staff       (20)      366 2022-03-30 11:15:50.000000 exotic-miri-0.0.1/exotic_miri/__init__.py
--rw-r--r--   0 davidgrant   (501) staff       (20)     3737 2022-04-14 09:28:13.000000 exotic-miri-0.0.1/exotic_miri/drop_groups_step.py
--rw-r--r--   0 davidgrant   (501) staff       (20)     3984 2022-04-14 09:28:13.000000 exotic-miri-0.0.1/exotic_miri/drop_integrations_step.py
--rw-r--r--   0 davidgrant   (501) staff       (20)    32783 2022-04-14 09:52:16.000000 exotic-miri-0.0.1/exotic_miri/extract_1d_step.py
--rw-r--r--   0 davidgrant   (501) staff       (20)     4718 2022-04-14 09:28:13.000000 exotic-miri-0.0.1/exotic_miri/reference_pixel_step.py
--rw-r--r--   0 davidgrant   (501) staff       (20)     3597 2022-04-14 09:28:13.000000 exotic-miri-0.0.1/exotic_miri/regroup_step.py
-drwxr-xr-x   0 davidgrant   (501) staff       (20)        0 2022-04-14 14:52:31.873612 exotic-miri-0.0.1/exotic_miri.egg-info/
--rw-r--r--   0 davidgrant   (501) staff       (20)     1240 2022-04-14 14:52:31.000000 exotic-miri-0.0.1/exotic_miri.egg-info/PKG-INFO
--rw-r--r--   0 davidgrant   (501) staff       (20)      420 2022-04-14 14:52:31.000000 exotic-miri-0.0.1/exotic_miri.egg-info/SOURCES.txt
--rw-r--r--   0 davidgrant   (501) staff       (20)        1 2022-04-14 14:52:31.000000 exotic-miri-0.0.1/exotic_miri.egg-info/dependency_links.txt
--rw-r--r--   0 davidgrant   (501) staff       (20)       42 2022-04-14 14:52:31.000000 exotic-miri-0.0.1/exotic_miri.egg-info/requires.txt
--rw-r--r--   0 davidgrant   (501) staff       (20)       12 2022-04-14 14:52:31.000000 exotic-miri-0.0.1/exotic_miri.egg-info/top_level.txt
--rw-r--r--   0 davidgrant   (501) staff       (20)        1 2022-04-14 14:16:27.000000 exotic-miri-0.0.1/exotic_miri.egg-info/zip-safe
--rw-r--r--   0 davidgrant   (501) staff       (20)       38 2022-04-14 14:52:31.874981 exotic-miri-0.0.1/setup.cfg
--rw-r--r--   0 davidgrant   (501) staff       (20)     1164 2022-04-14 14:37:54.000000 exotic-miri-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:56.950228 exotic-miri-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-31 09:41:56.950228 exotic-miri-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:56.946228 exotic-miri-1.0.0/exotic_miri/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:56.946228 exotic-miri-1.0.0/exotic_miri/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/reference/get_default_gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/reference/get_default_readnoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/reference/get_integration_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/reference/get_wavelength_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/reference/set_custom_gain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/reference/set_custom_linearity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:56.950228 exotic-miri-1.0.0/exotic_miri/stage_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_1/drop_groups_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_1/drop_integrations_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_1/group_level_background_subtract_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_1/reference_pixel_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_1/regroup_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:56.950228 exotic-miri-1.0.0/exotic_miri/stage_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_2/align_spectra_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_2/background_subtract_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15133 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_2/clean_outliers_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_2/extract_1d_box_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_2/extract_1d_optimal_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/exotic_miri/stage_2/inspect_dq_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:56.946228 exotic-miri-1.0.0/exotic_miri.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-31 09:41:56.000000 exotic-miri-1.0.0/exotic_miri.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-31 09:41:56.000000 exotic-miri-1.0.0/exotic_miri.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:41:56.000000 exotic-miri-1.0.0/exotic_miri.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 09:41:56.000000 exotic-miri-1.0.0/exotic_miri.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 09:41:56.000000 exotic-miri-1.0.0/exotic_miri.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 09:41:56.950228 exotic-miri-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:41:56.950228 exotic-miri-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/tests/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/tests/test_stage_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-07-31 09:41:44.000000 exotic-miri-1.0.0/tests/test_stage_2.py
```

### Comparing `exotic-miri-0.0.1/LICENSE` & `exotic-miri-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exotic-miri-0.0.1/PKG-INFO` & `exotic-miri-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: exotic-miri
-Version: 0.0.1
+Version: 1.0.0
 Summary: ExoTiC MIRI data reduction steps
 Home-page: https://github.com/Exo-TiC/ExoTiC-MIRI
 Author: David Grant
 Author-email: david.grant@bristol.ac.uk
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ExoTiC-MIRI
 ===========
 
-**Custom steps for JWST MIRI data reduction. Interoperable with the STScI pipeline.**
+**Custom steps for JWST MIRI LRS data reduction. Interoperable with the STScI pipeline.**
 
 .. image:: https://github.com/DavoGrant/ExoTiC-MIRI/workflows/unittests/badge.svg
    :target: https://github.com/DavoGrant/ExoTiC-MIRI/actions/workflows/python-app.yml
    
 .. image:: https://readthedocs.org/projects/exotic-miri/badge/?version=latest
    :target: https://exotic-miri.readthedocs.io/en/latest/?badge=latest
 
 |
 
 ::
 
    pip install exotic-miri
 
 | Read the full documentation at: `exotic-miri.readthedocs.io <https://exotic-miri.readthedocs.io/>`_
-
-
```

### Comparing `exotic-miri-0.0.1/README.rst` & `exotic-miri-1.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ExoTiC-MIRI
 ===========
 
-**Custom steps for JWST MIRI data reduction. Interoperable with the STScI pipeline.**
+**Custom steps for JWST MIRI LRS data reduction. Interoperable with the STScI pipeline.**
 
 .. image:: https://github.com/DavoGrant/ExoTiC-MIRI/workflows/unittests/badge.svg
    :target: https://github.com/DavoGrant/ExoTiC-MIRI/actions/workflows/python-app.yml
    
 .. image:: https://readthedocs.org/projects/exotic-miri/badge/?version=latest
    :target: https://exotic-miri.readthedocs.io/en/latest/?badge=latest
```

### Comparing `exotic-miri-0.0.1/exotic_miri/drop_integrations_step.py` & `exotic-miri-1.0.0/exotic_miri/stage_1/drop_integrations_step.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 import numpy as np
 from jwst import datamodels
 from jwst.stpipe import Step
 
 
 class DropIntegrationsStep(Step):
-    """ Drop integrations within data chunk.
-
-    This steps enables the user to drop integrations from a data chunk,
-    most likely because these groups are too severely affected by
-    systematics to be worth processing. This step may also be useful
-    if the user wants to test pipelines on only a small subset of data.
-
-    """
+    """ Drop integrations step. """
 
     spec = """
     drop_integrations = int_list(default=None)  # integrations to drop, zero-indexed.
     """
 
     def process(self, input):
-        """Execute the step.
+        """ Drop integrations from a data segment. The use of this step is
+        most likely because these integrations are too severely affected by
+        systematics to be worth processing, or this step may also be useful
+        if the user wants to test pipelines on only a small subset of data.
 
         Parameters
         ----------
-        input: JWST data model
-            A data model of type RampModel.
+        input: jwst.datamodels.RampModel
+            This is an uncal.fits loaded data segment.
+        drop_integrations: list of integers
+            These integers are the integrations to be dropped. The integers are
+            zero-indexed such that 0 is the first integration.
 
         Returns
         -------
-        JWST data model
-            A RampModel with updated integrations, unless the
-            step is skipped in which case `input_model` is returned.
+        output: jwst.datamodels.RampModel
+            A RampModel with [drop_integrations] removed.
+
         """
         with datamodels.open(input) as input_model:
 
             # Copy input model.
             thinned_model = input_model.copy()
 
             # Check input model type.
             if not isinstance(input_model, datamodels.RampModel):
-                self.log.error('Input is a {} which was not expected for _int'
-                               'egrations_step, skipping step.'.format(
+                self.log.error("Input is a {} which was not expected for _int"
+                               "egrations_step, skipping step.".format(
                                 str(type(input_model))))
-                thinned_model.meta.cal_step.drop_integrations = 'SKIPPED'
+                thinned_model.meta.cal_step.drop_integrations = "SKIPPED"
                 return thinned_model
 
             # Check the observation mode.
-            if not input_model.meta.exposure.type == 'MIR_LRS-SLITLESS':
-                self.log.error('Observation is a {} which is not supported by'
-                               ' ExoTic-MIRIs drop_integrations_step, skippin'
-                               'g step.'.format(
+            if not input_model.meta.exposure.type == "MIR_LRS-SLITLESS":
+                self.log.error("Observation is a {} which is not supported by"
+                               " ExoTic-MIRIs drop_integrations_step, skippin"
+                               "g step.".format(
                                 input_model.meta.exposure.type))
-                thinned_model.meta.cal_step.drop_integrations = 'SKIPPED'
+                thinned_model.meta.cal_step.drop_integrations = "SKIPPED"
                 return thinned_model
 
             # Check integrations to drop exist within data chunk.
             min_i_drop = np.min(self.drop_integrations)
             max_i_drop = np.max(self.drop_integrations)
             current_n_integrations = thinned_model.data.shape[0]
             if min_i_drop < 0 or max_i_drop > current_n_integrations - 1:
-                self.log.error('Not all integrations listed for dropping exis'
-                               't, requested to drop integrations between {} '
-                               'and {} when current integrations only span 0 '
-                               'to {}. Check your input list is zero indexed,'
-                               ' skipping step.'.format(
+                self.log.error("Not all integrations listed for dropping exis"
+                               "t, requested to drop integrations between {} "
+                               "and {} when current integrations only span 0 "
+                               "to {}. Check your input list is zero indexed,"
+                               " skipping step.".format(
                                 min_i_drop, max_i_drop,
                                 current_n_integrations - 1))
-                thinned_model.meta.cal_step.drop_integrations = 'SKIPPED'
+                thinned_model.meta.cal_step.drop_integrations = "SKIPPED"
                 return thinned_model
 
             # Compute wanted integrations.
             current_integrations = np.arange(0, current_n_integrations, 1)
             wanted_integrations = current_integrations[~np.isin(
                 current_integrations, self.drop_integrations)]
 
@@ -83,10 +82,10 @@
 
             # Update meta.
             thinned_model.meta.nints = thinned_model.data.shape[0]
             thinned_model.meta.nints_file = thinned_model.data.shape[0]
             thinned_model.meta.exposure.nints = thinned_model.data.shape[0]
             if thinned_model._shape:
                 thinned_model._shape = thinned_model.data.shape
-            thinned_model.meta.cal_step.drop_integrations = 'COMPLETE'
+            thinned_model.meta.cal_step.drop_integrations = "COMPLETE"
 
         return thinned_model
```

### Comparing `exotic-miri-0.0.1/exotic_miri/reference_pixel_step.py` & `exotic-miri-1.0.0/exotic_miri/stage_1/reference_pixel_step.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,82 +1,98 @@
+import matplotlib.pyplot as plt
 import numpy as np
 from jwst import datamodels
 from jwst.stpipe import Step
 
 
 class ReferencePixelStep(Step):
-    """ Reference pixel correction.
-
-    This steps enables the user to apply corrections to their group-
-    level images, using the reference pixels available to the MIRI LRS
-    subarray. The corrections can be made with a variety of options
-    for smoothing the values and/or separating odd and even rows.
-
-    """
+    """ Reference pixel step. """
 
     spec = """
     smoothing_length = integer(default=None)  # median smooth values over pixel length
     odd_even_rows = boolean(default=True)  # treat odd and even rows separately
+    draw_correction = boolean(default=False)  # draw correction images
     """
 
     def process(self, input):
-        """Execute the step.
+        """ Reference pixel correction at the group level, using the
+        reference pixels available to the MIRI LRS subarray. The corrections
+        can be made with a variety of options for smoothing the values and/or
+        separating odd and even rows.
+
+        The default pipeline, at the time of programming, does not have
+        this option for subarrays. It assumes subarrays have no available
+        reference pixels, but the MIRI LRS subarray is against the edge of
+        the detector.
 
         Parameters
         ----------
-        input: JWST data model
-            A data model of type RampModel.
+        input: jwst.datamodels.RampModel
+            This is an uncal.fits loaded data segment.
+        smoothing_length: integer
+            If not None, the number of rows to median smooth the estimated
+            reference pixel values over. Default is no smoothing.
+        odd_even_rows: boolean
+            Treat the correction separately for odd and even rows. Default
+            is True.
+        draw_correction: boolean
+            Plot the correction images.
 
         Returns
         -------
-        JWST data model
-            A RampModel with the reference pixel correction applied, unless
-            the step is skipped in which case `input_model` is returned.
+        output: jwst.datamodels.RampModel
+            A RampModel with the reference pixel correction applied.
+
         """
         with datamodels.open(input) as input_model:
 
             # Copy input model.
             rpc_model = input_model.copy()
 
             # Check input model type.
             if not isinstance(input_model, datamodels.RampModel):
-                self.log.error('Input is a {} which was not expected for '
-                               'reference_pixel_step, skipping step.'
+                self.log.error("Input is a {} which was not expected for "
+                               "reference_pixel_step, skipping step."
                                .format(str(type(input_model))))
-                rpc_model.meta.cal_step.refpix = 'SKIPPED'
+                rpc_model.meta.cal_step.refpix = "SKIPPED"
                 return rpc_model
 
             # Check the observation mode.
-            if not input_model.meta.exposure.type == 'MIR_LRS-SLITLESS':
-                self.log.error('Observation is a {} which is not supported '
-                               'by ExoTic-MIRIs reference_pixel_step, '
-                               'skipping step.'.format(
+            if not input_model.meta.exposure.type == "MIR_LRS-SLITLESS":
+                self.log.error("Observation is a {} which is not supported "
+                               "by ExoTic-MIRIs reference_pixel_step, "
+                               "skipping step.".format(
                                 input_model.meta.exposure.type))
-                rpc_model.meta.cal_step.refpix = 'SKIPPED'
+                rpc_model.meta.cal_step.refpix = "SKIPPED"
                 return rpc_model
 
             # Iterate integrations.
             for idx_int, integration in enumerate(rpc_model.data):
 
                 # Subtract first group from all groups.
                 int_ims = integration - integration[0]
 
                 # Compute and subtract the corrections.
-                # todo: mask/replace flagged ref pixels.
-                int_ims -= self.compute_reference_pixel_correction(int_ims)
+                # todo: mask flagged ref pixels.
+                ref_pixel_correction = self._compute_reference_pixel_correction(int_ims)
+
+                if self.draw_correction:
+                    self._draw_correction_images(idx_int, ref_pixel_correction)
+
+                int_ims -= ref_pixel_correction
 
                 # Add first group back to all groups.
                 rpc_model.data[idx_int] = int_ims + integration[0]
 
             # Update meta.
-            rpc_model.meta.cal_step.refpix = 'COMPLETE'
+            rpc_model.meta.cal_step.refpix = "COMPLETE"
 
         return rpc_model
 
-    def compute_reference_pixel_correction(self, int_ims):
+    def _compute_reference_pixel_correction(self, int_ims):
         """ Compute the reference pixel correction tiles. """
         ref_pixels = int_ims[:, :, 0:4]
         if not self.odd_even_rows:
             if self.smoothing_length is None:
                 return np.tile(
                     np.median(ref_pixels, axis=1)[:, np.newaxis, :],
                     (1, int_ims.shape[1], int(int_ims.shape[2] / 4)))
@@ -112,7 +128,17 @@
             end_row = min(n_rows - 1, idx_row + sm_radius)
 
             # Compute median in window.
             sm_ref_pixels[:, idx_row, :] = np.median(
                 ref_pixels[:, start_row:end_row + 1, :], axis=1)
 
         return sm_ref_pixels
+
+    def _draw_correction_images(self, idx_int, ref_pixel_correction):
+        for idx_grp, grp_correction in enumerate(ref_pixel_correction):
+            fig, ax1 = plt.subplots(1, 1, figsize=(5, 7))
+            ax1.imshow(grp_correction, origin="lower")
+            ax1.set_title("Integration={}, group={}".format(idx_int, idx_grp))
+            ax1.set_xlabel("Column pixels")
+            ax1.set_ylabel("Row pixels")
+            plt.tight_layout()
+            plt.show()
```

### Comparing `exotic-miri-0.0.1/exotic_miri/regroup_step.py` & `exotic-miri-1.0.0/exotic_miri/stage_1/regroup_step.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 from jwst import datamodels
 from jwst.stpipe import Step
 
 
 class RegroupStep(Step):
-    """ Regroup groups into integrations.
-
-    This steps enables the user to regroup integrations, comprised
-    of n groups, into several smaller integrations, comprised of m
-    groups, where n is a multiple of m.
-
-    """
+    """ Regroup long integrations into more shorter integrations. """
 
     spec = """
     n_groups = integer(default=10)  # new number of groups per integration
     """
 
     def process(self, input):
-        """Execute the step.
+        """ Regroup integrations, comprised of m groups, into several smaller
+        integrations, comprised of n groups, where m is a multiple of n. This
+        may not be helpful but it is here if you want to try it.
+        TODO: add support for non-multiples.
 
         Parameters
         ----------
-        input: JWST data model
-            A data model of type RampModel.
+        input: jwst.datamodels.RampModel
+            This is an uncal.fits loaded data segment.
+        n_groups: integer
+            The new number of groups per integration.
 
         Returns
         -------
-        JWST data model
-            A RampModel with updated integration groupings, unless the
-            step is skipped in which case `input_model` is returned.
+        output: jwst.datamodels.RampModel
+            A RampModel reshaped into n_groups.
+
         """
         with datamodels.open(input) as input_model:
 
             # Copy input model.
             regrouped_model = input_model.copy()
 
             # Check input model type.
             if not isinstance(input_model, datamodels.RampModel):
-                self.log.error('Input is a {} which was not expected for '
-                               'regroup_step, skipping step.'.format(
+                self.log.error("Input is a {} which was not expected for "
+                               "regroup_step, skipping step.".format(
                                 str(type(input_model))))
-                regrouped_model.meta.cal_step.regroup = 'SKIPPED'
+                regrouped_model.meta.cal_step.regroup = "SKIPPED"
                 return regrouped_model
 
             # Check the observation mode.
-            if not input_model.meta.exposure.type == 'MIR_LRS-SLITLESS':
-                self.log.error('Observation is a {} which is not supported '
-                               'by ExoTic-MIRIs regroup_step, skipping step.'
+            if not input_model.meta.exposure.type == "MIR_LRS-SLITLESS":
+                self.log.error("Observation is a {} which is not supported "
+                               "by ExoTic-MIRIs regroup_step, skipping step."
                                .format(input_model.meta.exposure.type))
-                regrouped_model.meta.cal_step.regroup = 'SKIPPED'
+                regrouped_model.meta.cal_step.regroup = "SKIPPED"
                 return regrouped_model
 
             # Check original number of groups is a multiple of n_groups.
             n = regrouped_model.meta.exposure.ngroups
             if not n % self.n_groups == 0:
-                self.log.error('Regrouping to {} groups is not possible for '
-                               'the original group number {}. It must be a '
-                               'multiple, skipping step.'.format(
+                self.log.error("Regrouping to {} groups is not possible for "
+                               "the original group number {}. It must be a "
+                               "multiple, skipping step.".format(
                                 self.n_groups, n))
-                regrouped_model.meta.cal_step.regroup = 'SKIPPED'
+                regrouped_model.meta.cal_step.regroup = "SKIPPED"
                 return regrouped_model
 
             # Compute change in integration sizes.
             d_factor = self.n_groups / regrouped_model.data.shape[1]
             n_int = int(regrouped_model.data.shape[0] / d_factor)
 
             # Regroup data.
@@ -79,10 +78,10 @@
             regrouped_model.meta.nints_file = n_int
             regrouped_model.meta.exposure.integration_time = \
                 regrouped_model.meta.exposure.integration_time * d_factor
             regrouped_model.meta.exposure.ngroups = self.n_groups
             regrouped_model.meta.exposure.nints = n_int
             if regrouped_model._shape:
                 regrouped_model._shape = regrouped_model.data.shape
-            regrouped_model.meta.cal_step.regroup = 'COMPLETE'
+            regrouped_model.meta.cal_step.regroup = "COMPLETE"
 
         return regrouped_model
```

### Comparing `exotic-miri-0.0.1/exotic_miri.egg-info/PKG-INFO` & `exotic-miri-1.0.0/exotic_miri.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: exotic-miri
-Version: 0.0.1
+Version: 1.0.0
 Summary: ExoTiC MIRI data reduction steps
 Home-page: https://github.com/Exo-TiC/ExoTiC-MIRI
 Author: David Grant
 Author-email: david.grant@bristol.ac.uk
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ExoTiC-MIRI
 ===========
 
-**Custom steps for JWST MIRI data reduction. Interoperable with the STScI pipeline.**
+**Custom steps for JWST MIRI LRS data reduction. Interoperable with the STScI pipeline.**
 
 .. image:: https://github.com/DavoGrant/ExoTiC-MIRI/workflows/unittests/badge.svg
    :target: https://github.com/DavoGrant/ExoTiC-MIRI/actions/workflows/python-app.yml
    
 .. image:: https://readthedocs.org/projects/exotic-miri/badge/?version=latest
    :target: https://exotic-miri.readthedocs.io/en/latest/?badge=latest
 
 |
 
 ::
 
    pip install exotic-miri
 
 | Read the full documentation at: `exotic-miri.readthedocs.io <https://exotic-miri.readthedocs.io/>`_
-
-
```

