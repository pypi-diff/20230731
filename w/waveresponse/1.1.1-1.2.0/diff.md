# Comparing `tmp/waveresponse-1.1.1-py3-none-any.whl.zip` & `tmp/waveresponse-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 19049 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1012 b- defN 23-Feb-14 08:33 waveresponse/__init__.py
--rw-r--r--  2.0 unx    58937 b- defN 23-Feb-14 08:33 waveresponse/_core.py
--rw-r--r--  2.0 unx    17902 b- defN 23-Feb-14 08:33 waveresponse/_standardized1d.py
--rw-r--r--  2.0 unx     4849 b- defN 23-Feb-14 08:33 waveresponse/_transform.py
--rw-r--r--  2.0 unx     1064 b- defN 23-Feb-14 08:34 waveresponse-1.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2495 b- defN 23-Feb-14 08:34 waveresponse-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-14 08:34 waveresponse-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Feb-14 08:34 waveresponse-1.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      743 b- defN 23-Feb-14 08:34 waveresponse-1.1.1.dist-info/RECORD
-9 files, 87107 bytes uncompressed, 17771 bytes compressed:  79.6%
+Zip file size: 19413 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1012 b- defN 23-Jul-31 09:30 waveresponse/__init__.py
+-rw-r--r--  2.0 unx    60742 b- defN 23-Jul-31 09:29 waveresponse/_core.py
+-rw-r--r--  2.0 unx    17902 b- defN 23-Jul-31 09:29 waveresponse/_standardized1d.py
+-rw-r--r--  2.0 unx     4849 b- defN 23-Jul-31 09:29 waveresponse/_transform.py
+-rw-r--r--  2.0 unx     1064 b- defN 23-Jul-31 09:30 waveresponse-1.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2495 b- defN 23-Jul-31 09:30 waveresponse-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 09:30 waveresponse-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Jul-31 09:30 waveresponse-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      743 b- defN 23-Jul-31 09:30 waveresponse-1.2.0.dist-info/RECORD
+9 files, 88912 bytes uncompressed, 18135 bytes compressed:  79.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: waveresponse/_standardized1d.py
 Comment: 
 
 Filename: waveresponse/_transform.py
 Comment: 
 
-Filename: waveresponse-1.1.1.dist-info/LICENSE
+Filename: waveresponse-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: waveresponse-1.1.1.dist-info/METADATA
+Filename: waveresponse-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: waveresponse-1.1.1.dist-info/WHEEL
+Filename: waveresponse-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: waveresponse-1.1.1.dist-info/top_level.txt
+Filename: waveresponse-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: waveresponse-1.1.1.dist-info/RECORD
+Filename: waveresponse-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## waveresponse/__init__.py

```diff
@@ -22,15 +22,15 @@
 from ._transform import (
     rigid_transform,
     rigid_transform_heave,
     rigid_transform_surge,
     rigid_transform_sway,
 )
 
-__version__ = "1.1.1"
+__version__ = "1.2.0"
 
 __all__ = [
     "BasePMSpectrum",
     "BaseSpectrum1d",
     "calculate_response",
     "complex_to_polar",
     "CosineFullSpreading",
```

## waveresponse/_core.py

```diff
@@ -45,18 +45,26 @@
     return amp, phase
 
 
 def polar_to_complex(amp, phase, phase_degrees=False):
     """
     Convert polar coordinates (i.e., amplitude and phase) to complex numbers.
 
+    Given as:
+
+        ``A * exp(j * phi)``
+
+    where, ``A`` is the amplitude and ``phi`` is the phase.
+
     Parameters
     ----------
-    complex_vals : array-like
-        Complex number values.
+    amp : array-like
+        Amplitude values.
+    phase : array-like
+        Phase angle values.
     phase_degrees : bool
         Whether the phase angles are given in 'degrees'. If ``False``, 'radians'
         is assumed.
 
     Returns
     -------
     array :
@@ -67,15 +75,15 @@
 
     if phase_degrees:
         phase = (np.pi / 180.0) * phase
 
     if amp.shape != phase.shape:
         raise ValueError()
 
-    return amp * (np.cos(phase) + 1j * np.sin(phase))
+    return amp * np.exp(1j * phase)
 
 
 def _check_is_similar(*grids, exact_type=True):
     """
     Check if grid objects are similar.
     """
     grids = list(grids)
@@ -959,23 +967,25 @@
             vals,
             freq_hz=freq_hz,
             degrees=degrees,
             clockwise=clockwise,
             waves_coming_from=waves_coming_from,
         )
         self._phase_degrees = False
+        self._phase_leading = True
 
     @classmethod
     def from_amp_phase(
         cls,
         freq,
         dirs,
         amp,
         phase,
         phase_degrees=False,
+        phase_leading=True,
         freq_hz=True,
         degrees=True,
         clockwise=True,
         waves_coming_from=True,
     ):
         """
         Construct an ``RAO`` object from amplitude and phase values.
@@ -995,14 +1005,21 @@
             of shape (N, M), such that ``N=len(freq)`` and ``M=len(dirs)``.
         phase : array-like (N, M)
             RAO phase values associated with the grid. Should be a 2-D array
             of shape (N, M), such that ``N=len(freq)`` and ``M=len(dirs)``.
         phase_degrees : bool
             If the RAO phase values are given in 'degrees'. If ``False``, 'radians'
             is assumed.
+        phase_leading : bool
+            Whether the phase values follow the 'leading' convention (``True``)
+            or the 'lagging' convention (``False``). Mathematically, an RAO with
+            phase lead convention is expressed as a complex number of the form
+            ``A * exp(j * phi)``, where ``A`` represents the amplitude and ``phi``
+            represents the phase angle. Whereas an RAO with phase lag convention
+            is expressed as ``A * exp(-j * phi)``.
         freq_hz : bool
             If frequency is given in 'Hz'. If ``False``, 'rad/s' is assumed.
         degrees : bool
             If direction is given in 'degrees'. If ``False``, 'radians' is assumed.
         clockwise : bool
             If positive directions are defined to be 'clockwise'. If ``False``,
             'counterclockwise' is assumed.
@@ -1021,26 +1038,30 @@
         with a wave spectrum to form a response spectrum), it is important that the
         RAO covers the full directional domain, i.e., [0, 360) degrees, with a sufficient
         resolution. If the RAO object only partly covers the directional domain, you
         can consider to use the :func:`mirror` function to 'expand' the RAO with values
         that are folded about a symmetry plane.
 
         """
+        if not phase_leading:
+            phase = -np.asarray_chkfinite(phase)
+
         rao_complex = polar_to_complex(amp, phase, phase_degrees=phase_degrees)
 
         rao = cls(
             freq,
             dirs,
             rao_complex,
             freq_hz=freq_hz,
             degrees=degrees,
             clockwise=clockwise,
             waves_coming_from=waves_coming_from,
         )
         rao._phase_degrees = phase_degrees
+        rao._phase_leading = phase_leading
         return rao
 
     def differentiate(self, n=1):
         """
         Return the nth derivative of the RAO.
 
         Parameters
@@ -1053,23 +1074,34 @@
         obj :
             Differentiated RAO object.
         """
         new = self.copy()
         new._vals = new._vals * ((1j * new._freq.reshape(-1, 1)) ** n)
         return new
 
-    def to_amp_phase(self, phase_degrees=None, freq_hz=None, degrees=None):
+    def to_amp_phase(
+        self, phase_degrees=None, phase_leading=None, freq_hz=None, degrees=None
+    ):
         """
         Return the RAO as amplitude and phase values.
 
         Parameters
         ----------
         phase_degrees : bool
             If phase values should be returned in 'degrees'. If ``False``, 'radians'
             is used. Defaults to original units used during initialization or ``False``.
+        phase_leading : bool
+            Whether the phase values should follow the 'leading' convention (``True``)
+            or the 'lagging' convention (``False``). If ``None``, it defaults to
+            the convention given during initialization, or the lagging convention
+            if no convention was specified during initialization. Mathematically,
+            an RAO with phase lead convention is expressed as a complex number of
+            the form ``A * exp(j * phi)``, where ``A`` represents the amplitude and
+            ``phi`` represents the phase angle. Whereas an RAO with phase lag convention
+            is expressed as ``A * exp(-j * phi)``.
         freq_hz : bool
             If frequencies should be returned in 'Hz'. If ``False``, 'rad/s' is used.
             Defaults to original units used during initialization.
         degrees : bool
             If directions should be returned in 'degrees'. If ``False``, 'radians'
             is used. Defaults to original units used during initialization.
 
@@ -1088,17 +1120,27 @@
         """
         if freq_hz is None:
             freq_hz = self._freq_hz
         if degrees is None:
             degrees = self._degrees
         if phase_degrees is None:
             phase_degrees = self._phase_degrees
+        if phase_leading is None:
+            phase_leading = self._phase_leading
 
         freq, dirs, vals = self.grid(freq_hz=freq_hz, degrees=degrees)
-        vals_amp, vals_phase = complex_to_polar(vals, phase_degrees=phase_degrees)
+        vals_amp, vals_phase = complex_to_polar(vals, phase_degrees=False)
+
+        if not phase_leading:
+            vals_phase = -vals_phase
+            vals_phase = np.where(np.isclose(vals_phase, -np.pi), np.pi, vals_phase)
+
+        if phase_degrees:
+            vals_phase = (180.0 / np.pi) * vals_phase
+
         return freq, dirs, vals_amp, vals_phase
 
     def __repr__(self):
         return "RAO"
 
 
 class DirectionalSpectrum(DisableComplexMixin, Grid):
```

## Comparing `waveresponse-1.1.1.dist-info/LICENSE` & `waveresponse-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `waveresponse-1.1.1.dist-info/METADATA` & `waveresponse-1.2.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveresponse
-Version: 1.1.1
+Version: 1.2.0
 Summary: Vessel motion and wave utilities
 Author-email: 4Subsea <python@4subsea.com>
 License: MIT License
         
         Copyright (c) 2022 4Subsea
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

## Comparing `waveresponse-1.1.1.dist-info/RECORD` & `waveresponse-1.2.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-waveresponse/__init__.py,sha256=FHTbOzyLcL_IVieE8L4cm1y8NUHWvs8SUTQ9vF5K5uA,1012
-waveresponse/_core.py,sha256=z2ugbKYUIINzzWUFPp0JRBx0EFYEVpvKhYK-TEXFrIU,58937
+waveresponse/__init__.py,sha256=P84dA0JUGTXfv0nh6mE-0H3zglJ3kwUftB_qxR0VOdo,1012
+waveresponse/_core.py,sha256=8-QW9HwntZ1J8cJhCmIl_R0PZjPgYmF3Z7ml8u9IB_4,60742
 waveresponse/_standardized1d.py,sha256=75K_ETKIRnuWxQJdvg1xxHphgDI2sPUIcISH0ZzejEA,17902
 waveresponse/_transform.py,sha256=NCJRDjX17MNJ1ZvZumlTUSsIhPES1QXOrBhvs42itn0,4849
-waveresponse-1.1.1.dist-info/LICENSE,sha256=FzsK1Sgr3HN65J1DaVUUx4ZECq8ivLV9g7MxAgngXaw,1064
-waveresponse-1.1.1.dist-info/METADATA,sha256=aLCKDJx7kW8bYwuyDDUw0XLVMbMEFMpzgi_Ai9ip2R0,2495
-waveresponse-1.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-waveresponse-1.1.1.dist-info/top_level.txt,sha256=_o03ggxMLy5Sj33DRz3vngwLpqmhpyEDFZ7Y-PVexu4,13
-waveresponse-1.1.1.dist-info/RECORD,,
+waveresponse-1.2.0.dist-info/LICENSE,sha256=FzsK1Sgr3HN65J1DaVUUx4ZECq8ivLV9g7MxAgngXaw,1064
+waveresponse-1.2.0.dist-info/METADATA,sha256=JEPqsOYpjzpya9oXaBMRPSQbXNE8t9R7cg2VaqAIuuk,2495
+waveresponse-1.2.0.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+waveresponse-1.2.0.dist-info/top_level.txt,sha256=_o03ggxMLy5Sj33DRz3vngwLpqmhpyEDFZ7Y-PVexu4,13
+waveresponse-1.2.0.dist-info/RECORD,,
```

