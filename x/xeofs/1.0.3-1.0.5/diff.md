# Comparing `tmp/xeofs-1.0.3.tar.gz` & `tmp/xeofs-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeofs-1.0.3.tar", max compression
+gzip compressed data, was "xeofs-1.0.5.tar", max compression
```

## Comparing `xeofs-1.0.3.tar` & `xeofs-1.0.5.tar`

### file list

```diff
@@ -1,31 +1,41 @@
--rw-r--r--   0        0        0     1070 2023-07-10 14:25:12.149602 xeofs-1.0.3/LICENSE
--rw-r--r--   0        0        0     6380 2023-07-10 14:25:12.149602 xeofs-1.0.3/README.rst
--rw-r--r--   0        0        0     1137 2023-07-10 14:25:13.005613 xeofs-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       75 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/__init__.py
--rw-r--r--   0        0        0       70 2023-07-10 14:25:13.005613 xeofs-1.0.3/xeofs/_version.py
--rw-r--r--   0        0        0      219 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/__init__.py
--rw-r--r--   0        0        0     5791 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/_base_cross_model.py
--rw-r--r--   0        0        0     8790 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/_base_model.py
--rw-r--r--   0        0        0     3398 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/_base_rotator.py
--rw-r--r--   0        0        0     8778 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/decomposer.py
--rw-r--r--   0        0        0     7540 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/eof.py
--rw-r--r--   0        0        0     9859 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/eof_rotator.py
--rw-r--r--   0        0        0    24353 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/mca.py
--rw-r--r--   0        0        0    25201 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/mca_rotator.py
--rw-r--r--   0        0        0     2153 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/models/rotator_factory.py
--rw-r--r--   0        0        0        0 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/preprocessing/__init__.py
--rw-r--r--   0        0        0      812 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/preprocessing/_base_scaler.py
--rw-r--r--   0        0        0     3781 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/preprocessing/_base_stacker.py
--rw-r--r--   0        0        0    11193 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/preprocessing/scaler.py
--rw-r--r--   0        0        0    21232 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/preprocessing/stacker.py
--rw-r--r--   0        0        0        0 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/utils/__init__.py
--rw-r--r--   0        0        0      301 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/utils/constants.py
--rw-r--r--   0        0        0      631 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/utils/data_types.py
--rw-r--r--   0        0        0     5179 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/utils/rotation.py
--rw-r--r--   0        0        0     2201 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/utils/sanity_checks.py
--rw-r--r--   0        0        0     4681 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/utils/statistics.py
--rw-r--r--   0        0        0     6690 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/utils/xarray_utils.py
--rw-r--r--   0        0        0       41 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/validation/__init__.py
--rw-r--r--   0        0        0        1 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/validation/_base_bootstrapper.py
--rw-r--r--   0        0        0     4957 2023-07-10 14:25:12.189602 xeofs-1.0.3/xeofs/validation/bootstrapper.py
--rw-r--r--   0        0        0     7299 1970-01-01 00:00:00.000000 xeofs-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-31 01:00:00.852649 xeofs-1.0.5/LICENSE
+-rw-r--r--   0        0        0     6380 2023-07-31 01:00:00.852649 xeofs-1.0.5/README.rst
+-rw-r--r--   0        0        0     1137 2023-07-31 01:00:01.824649 xeofs-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-31 01:00:01.824649 xeofs-1.0.5/xeofs/_version.py
+-rw-r--r--   0        0        0      478 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/data_container/__init__.py
+-rw-r--r--   0        0        0     4450 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/data_container/_base_cross_model_data_container.py
+-rw-r--r--   0        0        0     2762 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/data_container/_base_model_data_container.py
+-rw-r--r--   0        0        0     1037 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/data_container/eof_bootstrapper_data_container.py
+-rw-r--r--   0        0        0     4814 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/data_container/eof_data_container.py
+-rw-r--r--   0        0        0     4054 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/data_container/eof_rotator_data_container.py
+-rw-r--r--   0        0        0     7978 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/data_container/mca_data_container.py
+-rw-r--r--   0        0        0     5122 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/data_container/mca_rotator_data_container.py
+-rw-r--r--   0        0        0      219 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/models/__init__.py
+-rw-r--r--   0        0        0     4658 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/models/_base_cross_model.py
+-rw-r--r--   0        0        0     3971 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/models/_base_model.py
+-rw-r--r--   0        0        0     8854 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/models/decomposer.py
+-rw-r--r--   0        0        0    14479 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/models/eof.py
+-rw-r--r--   0        0        0    11261 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/models/eof_rotator.py
+-rw-r--r--   0        0        0    26526 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/models/mca.py
+-rw-r--r--   0        0        0    18664 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/models/mca_rotator.py
+-rw-r--r--   0        0        0     2113 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/models/rotator_factory.py
+-rw-r--r--   0        0        0        0 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/preprocessing/__init__.py
+-rw-r--r--   0        0        0      895 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/preprocessing/_base_scaler.py
+-rw-r--r--   0        0        0     4575 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/preprocessing/_base_stacker.py
+-rw-r--r--   0        0        0     4677 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/preprocessing/preprocessor.py
+-rw-r--r--   0        0        0    14803 2023-07-31 01:00:00.900649 xeofs-1.0.5/xeofs/preprocessing/scaler.py
+-rw-r--r--   0        0        0      686 2023-07-31 01:00:00.904649 xeofs-1.0.5/xeofs/preprocessing/scaler_factory.py
+-rw-r--r--   0        0        0    23439 2023-07-31 01:00:00.904649 xeofs-1.0.5/xeofs/preprocessing/stacker.py
+-rw-r--r--   0        0        0      698 2023-07-31 01:00:00.904649 xeofs-1.0.5/xeofs/preprocessing/stacker_factory.py
+-rw-r--r--   0        0        0        0 2023-07-31 01:00:00.904649 xeofs-1.0.5/xeofs/utils/__init__.py
+-rw-r--r--   0        0        0      301 2023-07-31 01:00:00.904649 xeofs-1.0.5/xeofs/utils/constants.py
+-rw-r--r--   0        0        0      773 2023-07-31 01:00:00.904649 xeofs-1.0.5/xeofs/utils/data_types.py
+-rw-r--r--   0        0        0     5179 2023-07-31 01:00:00.904649 xeofs-1.0.5/xeofs/utils/rotation.py
+-rw-r--r--   0        0        0     2219 2023-07-31 01:00:00.904649 xeofs-1.0.5/xeofs/utils/sanity_checks.py
+-rw-r--r--   0        0        0     4681 2023-07-31 01:00:00.904649 xeofs-1.0.5/xeofs/utils/statistics.py
+-rw-r--r--   0        0        0     7775 2023-07-31 01:00:00.904649 xeofs-1.0.5/xeofs/utils/xarray_utils.py
+-rw-r--r--   0        0        0       41 2023-07-31 01:00:00.904649 xeofs-1.0.5/xeofs/validation/__init__.py
+-rw-r--r--   0        0        0        1 2023-07-31 01:00:00.904649 xeofs-1.0.5/xeofs/validation/_base_bootstrapper.py
+-rw-r--r--   0        0        0     6814 2023-07-31 01:00:00.904649 xeofs-1.0.5/xeofs/validation/bootstrapper.py
+-rw-r--r--   0        0        0     7299 1970-01-01 00:00:00.000000 xeofs-1.0.5/PKG-INFO
```

### Comparing `xeofs-1.0.3/LICENSE` & `xeofs-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.3/README.rst` & `xeofs-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.3/pyproject.toml` & `xeofs-1.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xeofs"
-version = "1.0.3"
+version = "1.0.5"
 description = "Collection of EOF analysis and related techniques for climate science"
 authors = ["Niclas Rieger <niclasrieger@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/nicrie/xeofs"
 repository = "https://github.com/nicrie/xeofs"
 documentation = "https://xeofs.readthedocs.io/en/latest/"
```

### Comparing `xeofs-1.0.3/xeofs/models/decomposer.py` & `xeofs-1.0.5/xeofs/models/decomposer.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,16 +144,17 @@
         for old, new in feature_dims_temp2.items():
             X2 = X2.rename({old: new})
 
         # Compute cross-covariance matrix
         # Assuming that X1 and X2 are centered
         cov_matrix = xr.dot(X1.conj(), X2, dims='sample') / (X1.sample.size - 1)
 
-        # Compute squared total variance
-        self.squared_total_variance_ = (cov_matrix**2).sum().compute()
+        # Compute (squared) total variance
+        self.total_covariance_ = (abs(cov_matrix)).sum().compute()
+        self.total_squared_covariance_ = (abs(cov_matrix)**2).sum().compute()
 
         is_dask = True if isinstance(cov_matrix.data, DaskArray) else False
         is_complex = True if np.iscomplexobj(cov_matrix.data) else False
                         
         svd_kwargs = {}
         if (not is_complex) and (not is_dask):
             svd_kwargs.update({
```

### Comparing `xeofs-1.0.3/xeofs/models/mca_rotator.py` & `xeofs-1.0.5/xeofs/models/mca.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,388 +1,310 @@
+from typing import Tuple
+
 import numpy as np
 import xarray as xr
 from dask.diagnostics.progress import ProgressBar
-from typing import List
 
-from ._base_rotator import _BaseRotator
-from .mca import MCA, ComplexMCA
-from ..utils.rotation import promax
-from ..utils.data_types import XarrayData, DataArrayList, Dataset, DataArray
+from ._base_cross_model import _BaseCrossModel
+from .decomposer import CrossDecomposer
+from ..utils.data_types import AnyDataObject, DataArray
+from ..data_container.mca_data_container import MCADataContainer, ComplexMCADataContainer
 from ..utils.statistics import pearson_correlation
+from ..utils.xarray_utils import hilbert_transform
+
 
+class MCA(_BaseCrossModel):
+    '''Maximum Covariance Analyis (MCA).
 
-class MCARotator(_BaseRotator):
-    '''Rotate a solution obtained from ``xe.models.MCA``.
+    MCA is a statistical method that finds patterns of maximum covariance between two datasets.
     
     Parameters
     ----------
-    n_modes : int
-        Number of modes to be rotated.
-    power : int
-        Defines the power of Promax rotation. Choosing ``power=1`` equals
-        a Varimax solution (the default is 1).
-    max_iter : int
-        Number of maximal iterations for obtaining the rotation matrix
-        (the default is 1000).
-    rtol : float
-        Relative tolerance to be achieved for early stopping the iteration
-        process (the default is 1e-8).
-    squared_loadings : bool, default=False
-        Determines the method of constructing the combined vectors of loadings. If set to True, the combined 
-        vectors are loaded with the singular values ("squared loadings"), conserving the squared covariance 
-        under rotation. This allows for estimation of mode importance after rotation. If set to False, 
-        follows the Cheng & Dunkerton method [1]_ of loading with the square root of singular values.
-    
+    n_modes: int, default=10
+        Number of modes to calculate.
+    standardize: bool, default=False
+        Whether to standardize the input data.
+    use_coslat: bool, default=False
+        Whether to use cosine of latitude for scaling.
+    use_weights: bool, default=False
+        Whether to use additional weights.
+
+    Notes
+    -----
+    MCA is similar to Principal Component Analysis (PCA) and Canonical Correlation Analysis (CCA), 
+    but while PCA finds modes of maximum variance and CCA finds modes of maximum correlation, 
+    MCA finds modes of maximum covariance. See [1]_ [2]_ for more details.
+
     References
     ----------
-    .. [1] Cheng, X., Dunkerton, T.J., 1995. Orthogonal Rotation of Spatial Patterns Derived from Singular Value Decomposition Analysis. J. Climate 8, 2631–2643. https://doi.org/10.1175/1520-0442(1995)008<2631:OROSPD>2.0.CO;2
+    .. [1] Bretherton, C., Smith, C., Wallace, J., 1992. An intercomparison of methods for finding coupled patterns in climate data. Journal of climate 5, 541–560.
+    .. [2] Cherry, S., 1996. Singular value decomposition analysis and canonical correlation analysis. Journal of Climate 9, 2003–2009.
 
+    Examples
+    --------
+    >>> model = MCA(n_modes=5, standardize=True)
+    >>> model.fit(data1, data2) 
+    
     '''
-
-    def __init__(self, squared_loadings: bool = False, **kwargs):
+    def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self._params.update({'squared_loadings': squared_loadings})
-        self.attrs.update({'model': 'Rotated MCA'})
-
-    def fit(self, model: MCA | ComplexMCA):
-        '''Fit the model.
-        
-        Parameters
-        ----------
-        model : xe.models.MCA
-            A MCA model solution.
-            
-        '''
-        self._model = model
-        
-        n_modes = self._params.get('n_modes')
-        power = self._params.get('power')
-        max_iter = self._params.get('max_iter')
-        rtol = self._params.get('rtol')
-        use_squared_loadings = self._params.get('squared_loadings')
-
-
-        # Construct the combined vector of loadings
-        # NOTE: In the methodology used by Cheng & Dunkerton (CD), the combined vectors are "loaded" or weighted 
-        # with the square root of the singular values, akin to what is done in standard Varimax rotation. This method 
-        # ensures that the total amount of covariance is conserved during the rotation process.
-        # However, in Maximum Covariance Analysis (MCA), the focus is usually on the squared covariance to determine
-        # the importance of a given mode. The approach adopted by CD does not preserve the squared covariance under
-        # rotation, making it impossible to estimate the importance of modes post-rotation.
-        # To resolve this issue, one possible workaround is to rotate the singular vectors that have been "loaded"
-        # or weighted with the singular values ("squared loadings"), as opposed to the square root of the singular values.
-        # In doing so, the squared covariance remains conserved under rotation, allowing for the estimation of the 
-        # modes' importance. 
-        if use_squared_loadings:
-            # Squared loadings approach conserving squared covariance
-            scaling = self._model._singular_values.sel(mode=slice(1, n_modes))
-        else:
-            # Cheng & Dunkerton approach conserving covariance
-            scaling = np.sqrt(self._model._singular_values.sel(mode=slice(1, n_modes)))
-
-        svecs1 = self._model._singular_vectors1.sel(mode=slice(1, n_modes))
-        svecs2 = self._model._singular_vectors2.sel(mode=slice(1, n_modes))
-        loadings = xr.concat([svecs1, svecs2], dim='feature') * scaling
-
-        # Rotate loadings
-        rot_loadings, rot_matrix, Phi =  xr.apply_ufunc(
-            promax,
-            loadings,
-            power,
-            input_core_dims=[['feature', 'mode'], []],
-            output_core_dims=[['feature', 'mode'], ['mode', 'mode1'], ['mode', 'mode1']],
-            kwargs={'max_iter': max_iter, 'rtol': rtol},
-            dask='allowed'
-        )
-        self._rotation_matrix = rot_matrix
+        self.attrs.update({'model': 'MCA'})
 
-        # Rotated (loaded) singular vectors
-        svecs1_rot = rot_loadings.isel(feature=slice(0, svecs1.coords['feature'].size))
-        svecs2_rot = rot_loadings.isel(feature=slice(svecs1.coords['feature'].size, None))
-
-        # Normalization factor of singular vectors
-        norm1 = xr.apply_ufunc(np.linalg.norm, svecs1_rot, input_core_dims=[['feature']], output_core_dims=[[]], kwargs={'axis': -1}, dask='allowed')
-        norm2 = xr.apply_ufunc(np.linalg.norm, svecs2_rot, input_core_dims=[['feature']], output_core_dims=[[]], kwargs={'axis': -1}, dask='allowed')
-
-        # Rotated (normalized) singular vectors
-        svecs1_rot = svecs1_rot / norm1
-        svecs2_rot = svecs2_rot / norm2
-
-        # Remove the squaring introduced by the squared loadings approach
-        if use_squared_loadings:
-            norm1 = norm1 ** 0.5
-            norm2 = norm2 ** 0.5
-        
-        # Explained variance (= "singular values")
-        expvar = norm1 * norm2
-
-        # Reorder according to variance
-        # NOTE: For delayed objects, the index must be computed. .values will rensure that the index is computed
-        # NOTE: The index must be computed before sorting since argsort is not (yet) implemented in dask
-        idx_sort = expvar.values.argsort()[::-1]
-        self._idx_expvar = idx_sort
-        
-        self._explained_variance = expvar.isel(mode=idx_sort).assign_coords(mode=expvar.mode)
-        self._squared_covariance_fraction = self._explained_variance ** 2 / self._model._squared_total_variance
-
-        self._norm1 = norm1.isel(mode=idx_sort).assign_coords(mode=norm1.mode)
-        self._norm2 = norm2.isel(mode=idx_sort).assign_coords(mode=norm2.mode)
-        
-        self._singular_vectors1 = svecs1_rot.isel(mode=idx_sort).assign_coords(mode=svecs1_rot.mode)
-        self._singular_vectors2 = svecs2_rot.isel(mode=idx_sort).assign_coords(mode=svecs2_rot.mode)
-
-        # Rotate scores using rotation matrix
-        scores1 = self._model._scores1.sel(mode=slice(1,n_modes))
-        scores2 = self._model._scores2.sel(mode=slice(1,n_modes))
-        R = self._get_rotation_matrix(inverse_transpose=True)
-        scores1 = xr.dot(scores1, R, dims='mode1')
-        scores2 = xr.dot(scores2, R, dims='mode1')
-
-        # Reorder scores according to variance
-        scores1 = scores1.isel(mode=idx_sort).assign_coords(mode=scores1.mode)
-        scores2 = scores2.isel(mode=idx_sort).assign_coords(mode=scores2.mode)
-        
-        self._scores1 = scores1
-        self._scores2 = scores2
-
-        # Ensure consitent signs for deterministic output
-        idx_max_value = abs(rot_loadings).argmax('feature').compute()
-        flip_signs = xr.apply_ufunc(np.sign, rot_loadings.isel(feature=idx_max_value), dask='allowed')
-        # Drop all dimensions except 'mode' so that the index is clean
-        for dim, coords in flip_signs.coords.items():
-            if dim != 'mode':
-                flip_signs = flip_signs.drop(dim)
-        self._singular_vectors1 *= flip_signs
-        self._singular_vectors2 *= flip_signs
-        self._scores1 *= flip_signs
-        self._scores2 *= flip_signs
-
-        self._mode_signs = flip_signs
+        # Initialize the DataContainer to store the results
+        self.data: MCADataContainer = MCADataContainer()
 
+    def fit(self, data1: AnyDataObject, data2: AnyDataObject, dim, weights1=None, weights2=None):
+        data1_processed: DataArray = self.preprocessor1.fit_transform(data1, dim, weights1)
+        data2_processed: DataArray = self.preprocessor2.fit_transform(data2, dim, weights2)
+
+        decomposer = CrossDecomposer(n_modes=self._params['n_modes'])
+        decomposer.fit(data1_processed, data2_processed)
+
+        # Note:
+        # - explained variance is given by the singular values of the SVD;
+        # - We use the term singular_values_pca as used in the context of PCA:
+        # Considering data X1 = X2, MCA is the same as PCA. In this case,
+        # singular_values_pca is equivalent to the singular values obtained
+        # when performing PCA of X1 or X2.
+        singular_values = decomposer.singular_values_
+        singular_vectors1 = decomposer.singular_vectors1_
+        singular_vectors2 = decomposer.singular_vectors2_
+
+        squared_covariance = singular_values**2
+        total_squared_covariance = decomposer.total_squared_covariance_
+
+        norm1 = np.sqrt(singular_values)
+        norm2 = np.sqrt(singular_values)
+
+        # Index of the sorted squared covariance
+        idx_sorted_modes = squared_covariance.compute().argsort()[::-1]
+        idx_sorted_modes.coords.update(squared_covariance.coords)
+
+        # Project the data onto the singular vectors
+        scores1 = xr.dot(data1_processed, singular_vectors1, dims='feature') / norm1
+        scores2 = xr.dot(data2_processed, singular_vectors2, dims='feature') / norm2
+
+        self.data.set_data(
+            input_data1=data1_processed,
+            input_data2=data2_processed,
+            components1=singular_vectors1,
+            components2=singular_vectors2,
+            scores1=scores1,
+            scores2=scores2,
+            squared_covariance=squared_covariance,
+            total_squared_covariance=total_squared_covariance,
+            idx_modes_sorted=idx_sorted_modes,
+            norm1=norm1,
+            norm2=norm2,
+        )
         # Assign analysis-relevant meta data
-        self._assign_meta_data()
+        self.data.set_attrs(self.attrs)
 
-
-    def transform(self, **kwargs) -> XarrayData | DataArrayList:
-        '''Project new "unseen" data onto the rotated singular vectors.
+    def transform(self, **kwargs):
+        '''Project new unseen data onto the singular vectors.
 
         Parameters
         ----------
-        data1 : xr.DataArray | xr.Dataset | xr.DataArraylist
-            Data to be projected onto the rotated singular vectors of the first dataset.
-        data2 : xr.DataArray | xr.Dataset | xr.DataArraylist
-            Data to be projected onto the rotated singular vectors of the second dataset.
+        data1: xr.DataArray or list of xarray.DataArray
+            Left input data. Must be provided if `data2` is not provided.
+        data2: xr.DataArray or list of xarray.DataArray
+            Right input data. Must be provided if `data1` is not provided.
 
         Returns
         -------
-        xr.DataArray | xr.Dataset | xr.DataArraylist
-            Projected data.
-        
-        '''
-        # raise error if no data is provided
-        if not kwargs:
-            raise ValueError('No data provided. Please provide data1 and/or data2.')
-    
-        n_modes = self._params['n_modes']
-        expvar = self._explained_variance.sel(mode=slice(1, self._params['n_modes']))
-        rot_matrix = self._get_rotation_matrix(inverse_transpose=True)
+        scores1: DataArray | Dataset | List[DataArray]
+            Left scores.
+        scores2: DataArray | Dataset | List[DataArray]
+            Right scores.
 
+        '''
         results = []
+        if 'data1' in kwargs.keys():
+            # Preprocess input data
+            data1 = kwargs['data1']
+            data1 = self.preprocessor1.transform(data1)
+            # Project data onto singular vectors
+            comps1 = self.data.components1
+            norm1 = self.data.norm1
+            scores1 = xr.dot(data1, comps1) / norm1
+            # Inverse transform scores
+            scores1 = self.preprocessor1.inverse_transform_scores(scores1)
+            results.append(scores1)
+
+        if 'data2' in kwargs.keys():
+            # Preprocess input data
+            data2 = kwargs['data2']
+            data2 = self.preprocessor2.transform(data2)
+            # Project data onto singular vectors
+            comps2 = self.data.components2
+            norm2 = self.data.norm2
+            scores2 = xr.dot(data2, comps2) / norm2
+            # Inverse transform scores
+            scores2 = self.preprocessor2.inverse_transform_scores(scores2)
+            results.append(scores2)
 
-        if 'data1' in kwargs:
+        return results
 
-            data1 = kwargs['data1']
-            # Select the (non-rotated) singular vectors of the first dataset
-            svecs1 = self._model._singular_vectors1.sel(mode=slice(1, n_modes))
-            
-            # Preprocess the data
-            data1 = self._model.scaler1.transform(data1)  #type: ignore
-            data1 = self._model.stacker1.transform(data1)  #type: ignore
-            
-            # Compute non-rotated scores by project the data onto non-rotated components
-            projections1 = xr.dot(data1, svecs1) / expvar**0.5
-            # Rotate the scores
-            projections1 = xr.dot(projections1, rot_matrix, dims='mode1')
-            # Reorder according to variance
-            projections1 = projections1.isel(mode=self._idx_expvar).assign_coords(mode=projections1.mode)
-            # Determine the sign of the scores
-            projections1 *= self._mode_signs
-
-            # Unstack the projections
-            projections1 = self._model.stacker1.inverse_transform_scores(projections1)
-
-            results.append(projections1)
-
-
-        if 'data2' in kwargs:
-
-            data2 = kwargs['data2']            
-            # Select the (non-rotated) singular vectors of the second dataset
-            svecs2 = self._model._singular_vectors2.sel(mode=slice(1, n_modes))
-            
-            # Preprocess the data
-            data2 = self._model.scaler2.transform(data2)  #type: ignore
-            data2 = self._model.stacker2.transform(data2)  #type: ignore
-            
-            # Compute non-rotated scores by project the data onto non-rotated components
-            projections2 = xr.dot(data2, svecs2) / expvar**0.5
-            # Rotate the scores
-            projections2 = xr.dot(projections2, rot_matrix, dims='mode1')
-            # Reorder according to variance
-            projections2 = projections2.isel(mode=self._idx_expvar).assign_coords(mode=projections2.mode)
-            # Determine the sign of the scores
-            projections2 *= self._mode_signs
-
-
-            # Unstack the projections
-            projections2 = self._model.stacker2.inverse_transform_scores(projections2)
-
-            results.append(projections2)
-        
-        if len(results) == 1:
-            return results[0]
-        else:
-            return results
+    def inverse_transform(self, mode):
+        '''Reconstruct the original data from transformed data.
 
-    def inverse_transform(self, mode: int | List[int] | slice = slice(None)):
-        '''Reconstruct the original data from the rotated singular vectors.
-        
         Parameters
         ----------
-        mode : int | list[int] | slice
-            Modes to be used for reconstruction.
-            
+        mode: scalars, slices or array of tick labels.
+            The mode(s) used to reconstruct the data. If a scalar is given,
+            the data will be reconstructed using the given mode. If a slice
+            is given, the data will be reconstructed using the modes in the
+            given slice. If a array is given, the data will be reconstructed
+            using the modes in the given array.
+
         Returns
         -------
-        xr.DataArray | xr.Dataset | xr.DataArraylist
-            Reconstructed data.
-            
+        Xrec1: DataArray | Dataset | List[DataArray]
+            Reconstructed data of left field.
+        Xrec2: DataArray | Dataset | List[DataArray]
+            Reconstructed data of right field.
+
         '''
         # Singular vectors
-        svecs1 = self._singular_vectors1.sel(mode=mode)
-        svecs2 = self._singular_vectors2.sel(mode=mode)
+        comps1 = self.data.components1.sel(mode=mode)
+        comps2 = self.data.components2.sel(mode=mode)
 
         # Scores = projections
-        scores1 = self._scores1.sel(mode=mode)
-        scores2 = self._scores2.sel(mode=mode)
+        scores1 = self.data.scores1.sel(mode=mode)
+        scores2 = self.data.scores2.sel(mode=mode)
+
+        # Norms
+        norm1 = self.data.norm1.sel(mode=mode)
+        norm2 = self.data.norm2.sel(mode=mode)
 
         # Reconstruct the data
-        data1 = xr.dot(scores1, svecs1.conj(), dims='mode')
-        data2 = xr.dot(scores2, svecs2.conj(), dims='mode')
+        data1 = xr.dot(scores1, comps1.conj() * norm1, dims='mode')
+        data2 = xr.dot(scores2, comps2.conj() * norm2, dims='mode')
 
-        # Unstack the data
-        data1 = self._model.stacker1.inverse_transform_data(data1)
-        data2 = self._model.stacker2.inverse_transform_data(data2)
-
-        # Rescale the data
-        data1 = self._model.scaler1.inverse_transform(data1)  # type: ignore
-        data2 = self._model.scaler2.inverse_transform(data2)  # type: ignore
+        # Enforce real output
+        data1 = data1.real
+        data2 = data2.real
+        
+        # Unstack and rescale the data
+        data1 = self.preprocessor1.inverse_transform_data(data1)
+        data2 = self.preprocessor2.inverse_transform_data(data2)
 
         return data1, data2
-    
-    def compute(self, verbose: bool = False):
-        '''Compute the rotated solution.
-        
-        Parameters
-        ----------
-        verbose : bool
-            If True, print information about the computation process.
+
+    def squared_covariance(self):
+        '''Get the squared covariance.
+
+        The squared covariance corresponds to the explained variance in PCA and is given by the 
+        squared singular values of the covariance matrix.
             
         '''
-        
-        self._model.compute(verbose=verbose)
-        if verbose:
-            with ProgressBar():                
-                print('Computing ROTATED MODEL...')
-                print('-'*80)
-                print('Explainned variance...')
-                self._explained_variance = self._explained_variance.compute()
-                print('Squared covariance fraction...')
-                self._squared_covariance_fraction = self._squared_covariance_fraction.compute()
-                print('Norms...')
-                self._norm1 = self._norm1.compute()
-                self._norm2 = self._norm2.compute()
-                print('Singular vectors...')
-                self._singular_vectors1 = self._singular_vectors1.compute()
-                self._singular_vectors2 = self._singular_vectors2.compute()
-                print('Rotation matrix...')
-                self._rotation_matrix = self._rotation_matrix.compute()
-                print('Scores...')
-                self._scores1 = self._scores1.compute()
-                self._scores2 = self._scores2.compute()
-        else:
-            self._explained_variance = self._explained_variance.compute()
-            self._squared_covariance_fraction = self._squared_covariance_fraction.compute()
-            self._norm1 = self._norm1.compute()
-            self._norm2 = self._norm2.compute()
-            self._singular_vectors1 = self._singular_vectors1.compute()
-            self._singular_vectors2 = self._singular_vectors2.compute()
-            self._rotation_matrix = self._rotation_matrix.compute()
-            self._scores1 = self._scores1.compute()
-            self._scores2 = self._scores2.compute()
-
-    def _assign_meta_data(self):
-        '''Assign analysis-relevant meta data.'''
-        # Attributes of fitted model
-        attrs = self._model.attrs.copy()
-        # Include meta data of the rotation
-        attrs.update(self.attrs)
-        self._explained_variance.attrs.update(attrs)
-        self._squared_covariance_fraction.attrs.update(attrs)
-        self._singular_vectors1.attrs.update(attrs)
-        self._singular_vectors2.attrs.update(attrs)
-        self._scores1.attrs.update(attrs)
-        self._scores2.attrs.update(attrs)
+        return self.data.squared_covariance
+    
+    def squared_covariance_fraction(self):
+        '''Calculate the squared covariance fraction (SCF).
 
-    def components(self) -> tuple[DataArray | Dataset | DataArrayList, DataArray | Dataset | DataArrayList]:
-        '''Return the rotated singular vectors.
+        The SCF is a measure of the proportion of the total squared covariance that is explained by each mode `i`. It is computed 
+        as follows:
+
+        .. math::
+        SCF_i = \\frac{\\sigma_i^2}{\\sum_{i=1}^{m} \\sigma_i^2}
+
+        where `m` is the total number of modes and :math:`\\sigma_i` is the `ith` singular value of the covariance matrix.
+
+        '''
+        return self.data.squared_covariance_fraction
+    
+    def singular_values(self):
+        '''Get the singular values of the cross-covariance matrix.
+
+        '''
+        return self.data.singular_values
+
+    def covariance_fraction(self):
+        '''Get the covariance fraction (CF).
+
+        Cheng and Dunkerton (1995) define the CF as follows:
+
+        .. math::
+        CF_i = \\frac{\\sigma_i}{\\sum_{i=1}^{m} \\sigma_i}
+
+        where `m` is the total number of modes and :math:`\\sigma_i` is the `ith` singular value of the covariance matrix.
+
+        In this implementation the sum of singular values is estimated from the first `n` modes, therefore one should aim to
+        retain as many modes as possible to get a good estimate of the covariance fraction.
+
+        Note
+        ----
+        It is important to differentiate the CF from the squared covariance fraction (SCF). While the SCF is an invariant quantity in MCA, the CF is not.
+        Therefore, the SCF is used to assess the relative importance of each mode. Cheng and Dunkerton (1995) [1]_ introduced the CF in the context of
+        Varimax-rotated MCA to compare the relative importance of each mode before and after rotation. In the special case of both data fields in MCA being identical,
+        the CF is equivalent to the explained variance ratio in EOF analysis.
+
+        References
+        ----------
+        .. [1] Cheng, X., Dunkerton, T.J., 1995. Orthogonal Rotation of Spatial Patterns Derived from Singular Value Decomposition Analysis. J. Climate 8, 2631–2643. https://doi.org/10.1175/1520-0442(1995)008<2631:OROSPD>2.0.CO;2
 
-        Returns
-        -------
-        xr.DataArray | xr.Dataset | xr.DataArraylist
-            Rotated singular vectors.
 
         '''
-        svecs1 = self._model.stacker1.inverse_transform_components(self._singular_vectors1)
-        svecs2 = self._model.stacker2.inverse_transform_components(self._singular_vectors2)
+        # Check how sensitive the CF is to the number of modes
+        svals = self.data.singular_values
+        cf = svals[0] / svals.cumsum()
+        change_per_mode = cf.shift({'mode': 1}) - cf
+        change_in_cf_in_last_mode = change_per_mode.isel(mode=-1)
+        if change_in_cf_in_last_mode > 0.001:
+            print(f'Warning: CF is sensitive to the number of modes retained. Please increase `n_modes` for a better estimate.')
+        return self.data.covariance_fraction
 
-        return svecs1, svecs2
+    def components(self):
+        '''Return the singular vectors of the left and right field.
+        
+        Returns
+        -------
+        components1: DataArray | Dataset | List[DataArray]
+            Left components of the fitted model.
+        components2: DataArray | Dataset | List[DataArray]
+            Right components of the fitted model.
 
+        '''
+        return super().components()
+    
     def scores(self):
-        '''Return the rotated scores.
+        '''Return the scores of the left and right field.
 
+        The scores in MCA are the projection of the left and right field onto the
+        left and right singular vector of the cross-covariance matrix.
+        
         Returns
         -------
-        xr.DataArray | xr.Dataset | xr.DataArraylist
-            Rotated scores.
+        scores1: DataArray
+            Left scores.
+        scores2: DataArray
+            Right scores.
 
         '''
-        scores1 = self._model.stacker1.inverse_transform_scores(self._scores1)
-        scores2 = self._model.stacker2.inverse_transform_scores(self._scores2)
+        return super().scores()
 
-        return scores1, scores2
-    
-    def homogeneous_patterns(self, correction='fdr_bh', alpha=.05):
-        '''Return the rotated homogeneous patterns.
+    def homogeneous_patterns(self, correction=None, alpha=0.05):
+        '''Return the homogeneous patterns of the left and right field.
 
         The homogeneous patterns are the correlation coefficients between the 
         input data and the scores.
 
         More precisely, the homogeneous patterns `r_{hom}` are defined as
 
         .. math::
-          r_{hom, x} = \\corr \\left(X, A_x \\right)
+          r_{hom, x} = corr \\left(X, A_x \\right)
         .. math::
-          r_{hom, y} = \\corr \\left(Y, A_y \\right)
+          r_{hom, y} = corr \\left(Y, A_y \\right)
 
         where :math:`X` and :math:`Y` are the input data, :math:`A_x` and :math:`A_y`
         are the scores of the left and right field, respectively.
 
-        Parameters:
-        -------------
+        Parameters
+        ----------
         correction: str, default=None
             Method to apply a multiple testing correction. If None, no correction
             is applied.  Available methods are:
             - bonferroni : one-step correction
             - sidak : one-step correction
             - holm-sidak : step down method using Sidak adjustments
             - holm : step-down method using Bonferroni adjustments
@@ -391,215 +313,352 @@
             - fdr_bh : Benjamini/Hochberg (non-negative) (default)
             - fdr_by : Benjamini/Yekutieli (negative)
             - fdr_tsbh : two stage fdr correction (non-negative)
             - fdr_tsbky : two stage fdr correction (non-negative)
         alpha: float, default=0.05
             The desired family-wise error rate. Not used if `correction` is None.
 
-        Returns:
-        ----------
+        Returns
+        -------
         patterns1: DataArray | Dataset | List[DataArray]
             Left homogenous patterns.
         patterns2: DataArray | Dataset | List[DataArray]
             Right homogenous patterns.
         pvals1: DataArray | Dataset | List[DataArray]
             Left p-values.
         pvals2: DataArray | Dataset | List[DataArray]
             Right p-values.
 
         '''
+        input_data1 = self.data.input_data1
+        input_data2 = self.data.input_data2
 
-        hom_pats1, pvals1 = pearson_correlation(self._model.data1, self._scores1, correction=correction, alpha=alpha)
-        hom_pats2, pvals2 = pearson_correlation(self._model.data2, self._scores2, correction=correction, alpha=alpha)
+        scores1 = self.data.scores1
+        scores2 = self.data.scores2
 
-        hom_pats1 = self._model.stacker1.inverse_transform_components(hom_pats1)
-        hom_pats2 = self._model.stacker2.inverse_transform_components(hom_pats2)
+        hom_pat1, pvals1 = pearson_correlation(input_data1, scores1, correction=correction, alpha=alpha)
+        hom_pat2, pvals2 = pearson_correlation(input_data2, scores2, correction=correction, alpha=alpha)
 
-        pvals1 = self._model.stacker1.inverse_transform_components(pvals1)
-        pvals2 = self._model.stacker2.inverse_transform_components(pvals2)
+        hom_pat1 = self.preprocessor1.inverse_transform_components(hom_pat1)
+        hom_pat2 = self.preprocessor2.inverse_transform_components(hom_pat2)
 
-        hom_pats1.name = 'homogeneous_patterns'
-        hom_pats2.name = 'homogeneous_patterns'
+        pvals1 = self.preprocessor1.inverse_transform_components(pvals1)
+        pvals2 = self.preprocessor2.inverse_transform_components(pvals2)
 
-        pvals1.name = 'pvalues'
-        pvals2.name = 'pvalues'
+        hom_pat1.name = 'left_homogeneous_patterns'
+        hom_pat2.name = 'right_homogeneous_patterns'
 
-        return (hom_pats1, hom_pats2), (pvals1, pvals2)
+        pvals1.name = 'pvalues_of_left_homogeneous_patterns'
+        pvals2.name = 'pvalues_of_right_homogeneous_patterns'
 
+        return (hom_pat1, hom_pat2), (pvals1, pvals2)
 
-    def heterogeneous_patterns(self, correction='fdr_bh', alpha=.05):
-        '''Return the rotated heterogeneous patterns.
-
-        The heterogeneous patterns are the correlation coefficients between the 
-        input data and the scores.
-
+    def heterogeneous_patterns(self, correction=None, alpha=0.05):
+        '''Return the heterogeneous patterns of the left and right field.
+        
+        The heterogeneous patterns are the correlation coefficients between the
+        input data and the scores of the other field.
+        
         More precisely, the heterogeneous patterns `r_{het}` are defined as
-
+        
         .. math::
-          r_{het, x} = \\corr \\left(X, A_x \\right)
+          r_{het, x} = corr \\left(X, A_y \\right)
         .. math::
-          r_{het, y} = \\corr \\left(Y, A_y \\right)
-
+          r_{het, y} = corr \\left(Y, A_x \\right)
+        
         where :math:`X` and :math:`Y` are the input data, :math:`A_x` and :math:`A_y`
         are the scores of the left and right field, respectively.
 
-        Parameters:
-        -------------
+        Parameters
+        ----------
         correction: str, default=None
             Method to apply a multiple testing correction. If None, no correction
-            is applied.  Available methods are:
+            is applied.  Available methods are: 
             - bonferroni : one-step correction
             - sidak : one-step correction
             - holm-sidak : step down method using Sidak adjustments
             - holm : step-down method using Bonferroni adjustments
             - simes-hochberg : step-up method (independent)
             - hommel : closed method based on Simes tests (non-negative)
             - fdr_bh : Benjamini/Hochberg (non-negative) (default)
             - fdr_by : Benjamini/Yekutieli (negative)
             - fdr_tsbh : two stage fdr correction (non-negative)
             - fdr_tsbky : two stage fdr correction (non-negative)
         alpha: float, default=0.05
             The desired family-wise error rate. Not used if `correction` is None.
 
-        Returns:
-        ----------
-        patterns1: DataArray | Dataset | List[DataArray]
-            Left heterogeneous patterns.
-        patterns2: DataArray | Dataset | List[DataArray]
-            Right heterogeneous patterns.
-        pvals1: DataArray | Dataset | List[DataArray]
-            Left p-values.
-        pvals2: DataArray | Dataset | List[DataArray]
-            Right p-values.
-
         '''
+        input_data1 = self.data.input_data1
+        input_data2 = self.data.input_data2
+
+        scores1 = self.data.scores1
+        scores2 = self.data.scores2
+
+        patterns1, pvals1 = pearson_correlation(input_data1, scores2, correction=correction, alpha=alpha)
+        patterns2, pvals2 = pearson_correlation(input_data2, scores1, correction=correction, alpha=alpha)
 
-        het_pats1, pvals1 = pearson_correlation(self._model.data1, self._scores1, correction=correction, alpha=alpha)
-        het_pats2, pvals2 = pearson_correlation(self._model.data2, self._scores2, correction=correction, alpha=alpha)
+        patterns1 = self.preprocessor1.inverse_transform_components(patterns1)
+        patterns2 = self.preprocessor2.inverse_transform_components(patterns2)
 
-        het_pats1 = self._model.stacker1.inverse_transform_components(het_pats1)
-        het_pats2 = self._model.stacker2.inverse_transform_components(het_pats2)
+        pvals1 = self.preprocessor1.inverse_transform_components(pvals1)
+        pvals2 = self.preprocessor2.inverse_transform_components(pvals2)
 
-        pvals1 = self._model.stacker1.inverse_transform_components(pvals1)
-        pvals2 = self._model.stacker2.inverse_transform_components(pvals2)
+        patterns1.name = 'left_heterogeneous_patterns'
+        patterns2.name = 'right_heterogeneous_patterns'
 
-        het_pats1.name = 'heterogeneous_patterns'
-        het_pats2.name = 'heterogeneous_patterns'
+        pvals1.name = 'pvalues_of_left_heterogeneous_patterns'
+        pvals2.name = 'pvalues_of_right_heterogeneous_patterns'
 
-        pvals1.name = 'pvalues'
-        pvals2.name = 'pvalues'
+        return (patterns1, patterns2), (pvals1, pvals2)
 
-        return (het_pats1, het_pats2), (pvals1, pvals2)
 
-class ComplexMCARotator(MCARotator):
-    '''Rotate a solution obtained from ``xe.models.ComplexMCA``.
+
+class ComplexMCA(MCA):
+    '''Complex Maximum Covariance Analysis (MCA). 
+
+    Complex MCA, also referred to as Analytical SVD (ASVD) by Shane et al. (2017)[1]_, 
+    enhances traditional MCA by accommodating both amplitude and phase information. 
+    It achieves this by utilizing the Hilbert transform to preprocess the data, 
+    thus allowing for a more comprehensive analysis in the subsequent MCA computation.
+
+    An optional padding with exponentially decaying values can be applied prior to
+    the Hilbert transform in order to mitigate the impact of spectral leakage.
 
     Parameters
     ----------
-    n_modes : int
-        Number of modes to be rotated.
-    power : int
-        Defines the power of Promax rotation. Choosing ``power=1`` equals
-        a Varimax solution (the default is 1).
-    max_iter : int
-        Number of maximal iterations for obtaining the rotation matrix
-        (the default is 1000).
-    rtol : float
-        Relative tolerance to be achieved for early stopping the iteration
-        process (the default is 1e-8).
-    squared_loadings : bool, default=False
-        Determines the method of constructing the combined vectors of loadings. If set to True, the combined 
-        vectors are loaded with the singular values ("squared loadings"), conserving the squared covariance 
-        under rotation. This allows for estimation of mode importance after rotation. If set to False, 
-        follows the Cheng & Dunkerton method [1]_ of loading with the square root of singular values.
+    n_modes: int, default=10
+        Number of modes to calculate.
+    standardize: bool, default=False
+        Whether to standardize the input data.
+    use_coslat: bool, default=False
+        Whether to use cosine of latitude for scaling.
+    use_weights: bool, default=False
+        Whether to use additional weights.
+    padding : str, optional
+        Specifies the method used for padding the data prior to applying the Hilbert
+        transform. This can help to mitigate the effect of spectral leakage. 
+        Currently, only 'exp' for exponential padding is supported. Default is 'exp'.
+    decay_factor : float, optional
+        Specifies the decay factor used in the exponential padding. This parameter
+        is only used if padding='exp'. The recommended value typically ranges between 0.05 to 0.2 
+        but ultimately depends on the variability in the data. 
+        A smaller value (e.g. 0.05) is recommended for
+        data with high variability, while a larger value (e.g. 0.2) is recommended
+        for data with low variability. Default is 0.2.
+
+    Notes
+    -----
+    Complex MCA extends MCA to complex-valued data that contain both magnitude and phase information. 
+    The Hilbert transform is used to transform real-valued data to complex-valued data, from which both 
+    amplitude and phase can be extracted.
+
+    Similar to MCA, Complex MCA is used in climate science to identify coupled patterns of variability 
+    between two different climate variables. But unlike MCA, Complex MCA can identify coupled patterns 
+    that involve phase shifts.
 
     References
     ----------
-    .. [1] Cheng, X., Dunkerton, T.J., 1995. Orthogonal Rotation of Spatial Patterns Derived from Singular Value Decomposition Analysis. J. Climate 8, 2631–2643. https://doi.org/10.1175/1520-0442(1995)008<2631:OROSPD>2.0.CO;2
+    [1]_: Elipot, S., Frajka-Williams, E., Hughes, C.W., Olhede, S., Lankhorst, M., 2017. Observed Basin-Scale Response of the North Atlantic Meridional Overturning Circulation to Wind Stress Forcing. Journal of Climate 30, 2029–2054. https://doi.org/10.1175/JCLI-D-16-0664.1
+
+    
+    Examples
+    --------
+    >>> model = ComplexMCA(n_modes=5, standardize=True)
+    >>> model.fit(data1, data2)
 
     '''
-    def __init__(self, **kwargs):
+    def __init__(self, padding='exp', decay_factor=.2, **kwargs):
         super().__init__(**kwargs)
-        self.attrs.update({'model': 'Rotated Complex MCA'})
+        self.attrs.update({'model': 'Complex MCA'})
+        self._params.update({'padding': padding, 'decay_factor': decay_factor})
 
-    def transform(self, **kwargs) -> XarrayData | DataArrayList:
-        raise NotImplementedError('Complex MCA does not support transform.')
-    
-    def components_amplitude(self) -> DataArray | Dataset | DataArrayList:
+        # Initialize the DataContainer to store the results
+        self.data: ComplexMCADataContainer = ComplexMCADataContainer()
+
+    def fit(self, data1: AnyDataObject, data2: AnyDataObject, dim, weights1=None, weights2=None):
+        '''Fit the model.
+
+        Parameters
+        ----------
+        data1: xr.DataArray or list of xarray.DataArray
+            Left input data.
+        data2: xr.DataArray or list of xarray.DataArray
+            Right input data.
+        dim: tuple
+            Tuple specifying the sample dimensions. The remaining dimensions 
+            will be treated as feature dimensions.
+        weights1: xr.DataArray or xr.Dataset or None, default=None
+            If specified, the left input data will be weighted by this array.
+        weights2: xr.DataArray or xr.Dataset or None, default=None
+            If specified, the right input data will be weighted by this array.
+
+        '''
+
+        data1_processed: DataArray = self.preprocessor1.fit_transform(data1, dim, weights2)
+        data2_processed: DataArray = self.preprocessor2.fit_transform(data2, dim, weights2)
+        
+        # apply hilbert transform:
+        padding = self._params['padding']
+        decay_factor = self._params['decay_factor']
+        data1_processed = hilbert_transform(data1_processed, dim='sample', padding=padding, decay_factor=decay_factor)
+        data2_processed = hilbert_transform(data2_processed, dim='sample', padding=padding, decay_factor=decay_factor)
+        
+        decomposer = CrossDecomposer(n_modes=self._params['n_modes'])
+        decomposer.fit(data1_processed, data2_processed)
+
+        # Note:
+        # - explained variance is given by the singular values of the SVD;
+        # - We use the term singular_values_pca as used in the context of PCA:
+        # Considering data X1 = X2, MCA is the same as PCA. In this case,
+        # singular_values_pca is equivalent to the singular values obtained
+        # when performing PCA of X1 or X2.
+        singular_values = decomposer.singular_values_
+        singular_vectors1 = decomposer.singular_vectors1_
+        singular_vectors2 = decomposer.singular_vectors2_
+        
+        squared_covariance = singular_values**2
+        total_squared_covariance = decomposer.total_squared_covariance_
+        
+        norm1 = np.sqrt(singular_values)
+        norm2 = np.sqrt(singular_values)
+
+        # Index of the sorted squared covariance
+        idx_sorted_modes = squared_covariance.compute().argsort()[::-1]
+        idx_sorted_modes.coords.update(squared_covariance.coords)
+
+        # Project the data onto the singular vectors
+        scores1 = xr.dot(data1_processed, singular_vectors1) / norm1
+        scores2 = xr.dot(data2_processed, singular_vectors2) / norm2
+
+        self.data.set_data(
+            input_data1=data1_processed,
+            input_data2=data2_processed,
+            components1=singular_vectors1,
+            components2=singular_vectors2,
+            scores1=scores1,
+            scores2=scores2,
+            squared_covariance=squared_covariance,
+            total_squared_covariance=total_squared_covariance,
+            idx_modes_sorted=idx_sorted_modes,
+            norm1=norm1,
+            norm2=norm2,
+        )
+        # Assign analysis relevant meta data
+        self.data.set_attrs(self.attrs)
+
+    def components_amplitude(self) -> Tuple[AnyDataObject, AnyDataObject]:
         '''Compute the amplitude of the components.
 
+        The amplitude of the components are defined as
+
+        .. math::
+            A_ij = |C_ij|
+
+        where :math:`C_{ij}` is the :math:`i`-th entry of the :math:`j`-th component and
+        :math:`|\\cdot|` denotes the absolute value.
+
         Returns
         -------
-        xr.DataArray
-            Amplitude of the components.
+        AnyDataObject
+            Amplitude of the left components.
+        AnyDataObject
+            Amplitude of the left components.
 
         '''
-        comps1 = abs(self._singular_vectors1)
-        comps2 = abs(self._singular_vectors2)
+        comps1 = self.data.components_amplitude1
+        comps2 = self.data.components_amplitude2
 
-        comps1.name = 'singular_vector_amplitudes'
-        comps2.name = 'singular_vector_amplitudes'
+        comps1 = self.preprocessor1.inverse_transform_components(comps1)
+        comps2 = self.preprocessor2.inverse_transform_components(comps2)
 
-        comps1 = self._model.stacker1.inverse_transform_components(comps1)
-        comps2 = self._model.stacker2.inverse_transform_components(comps2)
+        return (comps1, comps2)
 
-        return comps1, comps2  # type: ignore
-
-    def components_phase(self) -> DataArray | Dataset | DataArrayList:
+    def components_phase(self) -> Tuple[AnyDataObject, AnyDataObject]:
         '''Compute the phase of the components.
 
+        The phase of the components are defined as
+
+        .. math::
+            \\phi_{ij} = \\arg(C_{ij})
+
+        where :math:`C_{ij}` is the :math:`i`-th entry of the :math:`j`-th component and
+        :math:`\\arg(\\cdot)` denotes the argument of a complex number.
+
         Returns
         -------
-        xr.DataArray
-            Phase of the components.
+        AnyDataObject
+            Phase of the left components.
+        AnyDataObject
+            Phase of the right components.
 
         '''
-        comps1 = xr.apply_ufunc(np.angle, self._singular_vectors1, keep_attrs=True)
-        comps2 = xr.apply_ufunc(np.angle, self._singular_vectors2, keep_attrs=True)
-
-        comps1.name = 'singular_vector_phases'
-        comps2.name = 'singular_vector_phases'
+        comps1 = self.data.components_phase1
+        comps2 = self.data.components_phase2
 
-        comps1 = self._model.stacker1.inverse_transform_components(comps1)
-        comps2 = self._model.stacker2.inverse_transform_components(comps2)
+        comps1 = self.preprocessor1.inverse_transform_components(comps1)
+        comps2 = self.preprocessor2.inverse_transform_components(comps2)
 
-        return comps1, comps2  # type: ignore
+        return (comps1, comps2)
     
-    def scores_amplitude(self) -> DataArray | Dataset | DataArrayList:
+    def scores_amplitude(self) -> Tuple[DataArray, DataArray]:
         '''Compute the amplitude of the scores.
 
-        Returns
-        -------
-        xr.DataArray
-            Amplitude of the scores.
+        The amplitude of the scores are defined as
 
-        '''
-        scores1 = abs(self._scores1)
-        scores2 = abs(self._scores2)
+        .. math::
+            A_ij = |S_ij|
 
-        scores1.name = 'score_amplitudes'
-        scores2.name = 'score_amplitudes'
+        where :math:`S_{ij}` is the :math:`i`-th entry of the :math:`j`-th score and
+        :math:`|\\cdot|` denotes the absolute value.
 
-        scores1 = self._model.stacker1.inverse_transform_scores(scores1)
-        scores2 = self._model.stacker2.inverse_transform_scores(scores2)
+        Returns
+        -------
+        DataArray
+            Amplitude of the left scores.
+        DataArray
+            Amplitude of the right scores.
 
-        return scores1, scores2  # type: ignore
+        '''
+        scores1 = self.data.scores_amplitude1
+        scores2 = self.data.scores_amplitude2
+
+        scores1 = self.preprocessor1.inverse_transform_scores(scores1)
+        scores2 = self.preprocessor2.inverse_transform_scores(scores2)
+        return (scores1, scores2)
     
-    def scores_phase(self) -> DataArray | Dataset | DataArrayList:
+    def scores_phase(self) -> Tuple[DataArray, DataArray]:
         '''Compute the phase of the scores.
 
+        The phase of the scores are defined as
+        
+        .. math::
+            \\phi_{ij} = \\arg(S_{ij})
+
+        where :math:`S_{ij}` is the :math:`i`-th entry of the :math:`j`-th score and
+        :math:`\\arg(\\cdot)` denotes the argument of a complex number.
+
         Returns
         -------
-        xr.DataArray
-            Phase of the scores.
+        DataArray
+            Phase of the left scores.
+        DataArray
+            Phase of the right scores.
 
         '''
-        scores1 = xr.apply_ufunc(np.angle, self._scores1, keep_attrs=True)
-        scores2 = xr.apply_ufunc(np.angle, self._scores2, keep_attrs=True)
+        scores1 = self.data.scores_phase1
+        scores2 = self.data.scores_phase2
 
-        scores1.name = 'score_phases'
-        scores2.name = 'score_phases'
+        scores1 = self.preprocessor1.inverse_transform_scores(scores1)
+        scores2 = self.preprocessor2.inverse_transform_scores(scores2)
 
-        scores1 = self._model.stacker1.inverse_transform_scores(scores1)
-        scores2 = self._model.stacker2.inverse_transform_scores(scores2)
+        return (scores1, scores2)
+
+    
+    def transform(self, data1: AnyDataObject, data2: AnyDataObject):
+        raise NotImplementedError('Complex MCA does not support transform method.')
+
+    def homogeneous_patterns(self, correction=None, alpha=0.05):
+        raise NotImplementedError('Complex MCA does not support homogeneous_patterns method.')
+    
+    def heterogeneous_patterns(self, correction=None, alpha=0.05):
+        raise NotImplementedError('Complex MCA does not support heterogeneous_patterns method.')
 
-        return scores1, scores2  # type: ignore
```

### Comparing `xeofs-1.0.3/xeofs/models/rotator_factory.py` & `xeofs-1.0.5/xeofs/models/rotator_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from xeofs.utils.data_types import DataArrayList, XarrayData
 
 from .eof import EOF, ComplexEOF
 from .mca import MCA, ComplexMCA
 from .eof_rotator import EOFRotator, ComplexEOFRotator
 from .mca_rotator import MCARotator, ComplexMCARotator
-from ._base_rotator import _BaseRotator
 from ..utils.rotation import promax
 from ..utils.data_types import XarrayData, DataArrayList, Dataset, DataArray
 
 
 
 class RotatorFactory:
     '''Factory class for creating rotators.
```

### Comparing `xeofs-1.0.3/xeofs/preprocessing/_base_scaler.py` & `xeofs-1.0.5/xeofs/preprocessing/_base_scaler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from abc import ABC, abstractmethod
 
 
 class _BaseScaler(ABC):
-    def __init__(self, with_copy=True, with_std=True, with_coslat=False, with_weights=False):
+    def __init__(self, with_std=True, with_coslat=False, with_weights=False):
         self._params = dict(
-            with_copy=with_copy,
             with_std=with_std,
             with_coslat=with_coslat,
             with_weights=with_weights
         )
 
         self.mean = None
         self.std = None
@@ -20,12 +19,16 @@
         raise NotImplementedError
     
     @abstractmethod
     def transform(self, X):
         raise NotImplementedError
     
     @abstractmethod
+    def fit_transform(self, X, sample_dims, feature_dims, weights=None):
+        raise NotImplementedError
+    
+    @abstractmethod
     def inverse_transform(self, X):
         raise NotImplementedError
     
     def get_params(self):
         return self._params.copy()
```

### Comparing `xeofs-1.0.3/xeofs/preprocessing/_base_stacker.py` & `xeofs-1.0.5/xeofs/preprocessing/_base_stacker.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,14 +22,25 @@
     coords_out_ : dict['sample': ..., 'feature': ...]
         The coordinates of the stacked data. Typically consist of MultiIndex.
 
     '''
     def __init__(self):
         pass
 
+    def fit(self, data, sample_dims: Hashable | Sequence[Hashable], feature_dims: Hashable | Sequence[Hashable] | List[Sequence[Hashable]]):
+        ''' Invoking a `fit` operation for a stacker object isn't practical because it requires stacking the data, 
+        only to ascertain the output dimensions. This step is computationally expensive and unnecessary. 
+        Therefore, instead of using a separate `fit` method, we combine the fit and transform steps 
+        into the `fit_transform` method for efficiency. However, to maintain consistency with other classes 
+        that do utilize a `fit` method, we retain the `fit` method here, albeit unimplemented.
+
+        '''
+        raise NotImplementedError('Stacker does not implement fit method. Use fit_transform instead.')
+        
+
     @abstractmethod
     def fit_transform(
             self,
             data,
             sample_dims: Hashable | Sequence[Hashable],
             feature_dims: Hashable | Sequence[Hashable] | List[Sequence[Hashable]]
             ) -> xr.DataArray:
```

### Comparing `xeofs-1.0.3/xeofs/preprocessing/stacker.py` & `xeofs-1.0.5/xeofs/preprocessing/stacker.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,68 +3,35 @@
 import numpy as np
 import pandas as pd
 import xarray as xr
 
 from xeofs.utils.data_types import DataArray
 
 from ._base_stacker import _BaseStacker
-from ..utils.data_types import DataArray, DataArrayList, Dataset
+from ..utils.data_types import DataArray, DataArrayList, Dataset, SingleDataObject, AnyDataObject
 from ..utils.sanity_checks import ensure_tuple
 
 
-class DataArrayStacker(_BaseStacker):
-    ''' Converts a DataArray of any dimensionality into a 2D structure.
+class SingleDataStacker(_BaseStacker):
 
-    This operation generates a reshaped DataArray with two distinct dimensions: 'sample' and 'feature'.
+    def __init__(self):
+        super().__init__()
     
-    The handling of NaNs is specific: if they are found to populate an entire dimension (be it 'sample' or 'feature'), 
-    they are temporarily removed during transformations and subsequently reinstated. 
-    However, the presence of isolated NaNs will trigger an error.
-        
-    '''
-
-    @staticmethod
-    def _stack(data: DataArray, sample_dims, feature_dims) -> DataArray:
-        ''' Reshape a DataArray to 2D.
-
-        Parameters
-        ----------
-        data : DataArray
-            The data to be reshaped.
-        sample_dims : Hashable or Sequence[Hashable]
-            The dimensions of the data that will be stacked along the `sample` dimension.
-        feature_dims : Hashable or Sequence[Hashable]
-            The dimensions of the data that will be stacked along the `feature` dimension.
-
-        Returns
-        -------
-        data_stacked : DataArray
-            The reshaped 2d-data.
-        '''
-        # Raise error if dimensions feature/sample already exists in data
-        if 'feature' in data.dims:
-            raise ValueError('`feature` dimension already exists in data. Please rename.')
-        if 'sample' in data.dims:
-            raise ValueError('`sample` dimension already exists in data. Please rename.')
-
-        # Rename if sample/feature dimensions is one dimensional, otherwise stack
-        if len(feature_dims) == 1:
-            data = data.rename({feature_dims[0]: 'feature'})
-        else:
-            data = data.stack(feature=feature_dims)
-
-        if len(sample_dims) == 1:
-            data = data.rename({sample_dims[0]: 'sample'})
-        else:
-            data = data.stack(sample=sample_dims)
-
-        return data.transpose('sample', 'feature')
+    def _verify_dims(self, data: SingleDataObject):
+        ''' Verify that the dimensions of the data are consistent with the dimensions used to fit the stacker.'''
+        # Test whether sample and feature dimensions are present in data array
+        if not (set(self.dims_out_['sample'] + self.dims_out_['feature']) == set(data.dims)):
+            raise ValueError(f'One or more dimensions in {self.dims_out_["sample"] + self.dims_out_["feature"]} are not present in data.')
 
-    def _unstack(self, data: DataArray) -> DataArray:
-        ''' Unstack `sample` and `feature dimension of an DataArray to its original dimensions.
+    def _stack(self, data: SingleDataObject, sample_dims, feature_dims) -> DataArray:
+        ''' Reshape a SingleDataObject to 2D DataArray.'''
+        raise NotImplementedError
+    
+    def _unstack(self, data: SingleDataObject) -> SingleDataObject:
+        ''' Unstack `sample` and `feature` dimension of an DataArray to its original dimensions.
 
         Parameters
         ----------
         data : DataArray
             The data to be unstacked.
 
         Returns
@@ -89,15 +56,15 @@
         
         # Reorder dimensions to original order; catch ('mode') dimensions via ellipsis
         order_input_dims = [valid_dim for valid_dim in self.dims_in_ if valid_dim in data.dims]
         data = data.transpose(..., *order_input_dims)
         
         return data
 
-    def _reindex_dim(self, data: DataArray,  stacked_dim : str):
+    def _reindex_dim(self, data: SingleDataObject, stacked_dim: str) -> SingleDataObject:
         ''' Reindex data to original coordinates in case that some features at the boundaries were dropped
         
         Parameters
         ----------
         data : DataArray
             The data to be reindex.
         stacked_dim : str ['sample', 'feature']
@@ -116,20 +83,16 @@
         dims_in = self.dims_out_[stacked_dim]
         for dim in dims_in:
             if self.coords_in_[dim].size != data.coords[dim].size:
                 data = data.reindex({dim: self.coords_in_[dim]}, copy=False)
 
         return data
 
-    def fit_transform(
-            self,
-            data: DataArray,
-            sample_dims: Hashable | Sequence[Hashable],
-            feature_dims: Hashable | Sequence[Hashable]
-            ) -> xr.DataArray:
+
+    def fit_transform(self, data: SingleDataObject, sample_dims: Hashable | Sequence[Hashable], feature_dims: Hashable | Sequence[Hashable]) -> DataArray:
         ''' Fit the stacker and transform data to 2D.
         
         Parameters
         ----------
         data : DataArray
             The data to be reshaped.
         sample_dims : Hashable or Sequence[Hashable]
@@ -163,30 +126,30 @@
         # Set in/out dimensions
         self.dims_in_ = data.dims
         self.dims_out_ = {'sample': sample_dims, 'feature': feature_dims}
 
         # Set in/out coordinates
         self.coords_in_ = {dim: data.coords[dim] for dim in data.dims}
         # Stack data and remove NaN features
-        data = self._stack(data, self.dims_out_['sample'], self.dims_out_['feature'])
-        data = data.dropna('feature', how='all')
-        data = data.dropna('sample', how='all')
-        self.coords_out_ = {'sample': data.coords['sample'], 'feature': data.coords['feature']}
+        da: DataArray = self._stack(data, self.dims_out_['sample'], self.dims_out_['feature'])
+        da = da.dropna('feature', how='all')
+        da = da.dropna('sample', how='all')
+        self.coords_out_ = {'sample': da.coords['sample'], 'feature': da.coords['feature']}
 
         # Ensure that no NaNs are present in the data
-        if data.isnull().any():
+        if da.isnull().any():
             raise ValueError('Isolated NaNs are present in the data. Please remove them before fitting the model.')
 
         # Ensure that data is not empty
-        if data.size == 0:
+        if da.size == 0:
             raise ValueError('Data is empty.')
 
-        return data
+        return da
 
-    def transform(self, data: DataArray) -> DataArray:
+    def transform(self, data: SingleDataObject) -> DataArray:
         ''' Transform new "unseen" data to 2D version.
         
         Parameters
         ----------
         data : DataArray
             The data to be reshaped.
             
@@ -212,27 +175,106 @@
             raise ValueError(f'One or more dimensions in {self.dims_out_["sample"] + self.dims_out_["feature"]} are not present in data.')
 
         # Check if data to be transformed has the same feature coordinates as the data used to fit the stacker
         if not all([data.coords[dim].equals(self.coords_in_[dim]) for dim in self.dims_out_['feature']]):  #type: ignore
             raise ValueError('Data to be transformed has different coordinates than the data used to fit.')
 
         # Stack data and remove NaN features
-        data = self._stack(data, self.dims_out_['sample'], self.dims_out_['feature'])
-        data = data.dropna('feature', how='all')
-        data = data.dropna('sample', how='all')
+        da: DataArray = self._stack(data, self.dims_out_['sample'], self.dims_out_['feature'])
+        da = da.dropna('feature', how='all')
+        da = da.dropna('sample', how='all')
 
         # Ensure that no NaNs are present in the data
-        if data.isnull().any():
+        if da.isnull().any():
             raise ValueError('Isolated NaNs are present in the data. Please remove them before fitting the model.')
 
         # Ensure that data is not empty
-        if data.size == 0:
+        if da.size == 0:
             raise ValueError('Data is empty.')
 
-        return data
+        return da
+
+
+class SingleDataArrayStacker(SingleDataStacker):
+    ''' Converts a DataArray of any dimensionality into a 2D structure.
+
+    This operation generates a reshaped DataArray with two distinct dimensions: 'sample' and 'feature'.
+    
+    The handling of NaNs is specific: if they are found to populate an entire dimension (be it 'sample' or 'feature'), 
+    they are temporarily removed during transformations and subsequently reinstated. 
+    However, the presence of isolated NaNs will trigger an error.
+        
+    '''
+
+    @staticmethod
+    def _stack(data: DataArray, sample_dims, feature_dims) -> DataArray:
+        ''' Reshape a DataArray to 2D.
+
+        Parameters
+        ----------
+        data : DataArray
+            The data to be reshaped.
+        sample_dims : Hashable or Sequence[Hashable]
+            The dimensions of the data that will be stacked along the `sample` dimension.
+        feature_dims : Hashable or Sequence[Hashable]
+            The dimensions of the data that will be stacked along the `feature` dimension.
+
+        Returns
+        -------
+        data_stacked : DataArray
+            The reshaped 2d-data.
+        '''
+        # Raise error if dimensions feature/sample already exists in data
+        if 'feature' in data.dims:
+            raise ValueError('The dimension name `feature` conflicts with internal usage. Please rename this dimension before the analysis.')
+        if 'sample' in data.dims:
+            raise ValueError('The dimension name `sample` conflicts with internal usage. Please rename this dimension before the analysis.')
+
+        # Rename if sample/feature dimensions is one dimensional, otherwise stack
+        if len(feature_dims) == 1:
+            data = data.rename({feature_dims[0]: 'feature'})
+        else:
+            data = data.stack(feature=feature_dims)
+
+        if len(sample_dims) == 1:
+            data = data.rename({sample_dims[0]: 'sample'})
+        else:
+            data = data.stack(sample=sample_dims)
+
+        return data.transpose('sample', 'feature')
+
+    def _unstack(self, data: DataArray) -> DataArray:
+        ''' Unstack `sample` and `feature` dimension of an DataArray to its original dimensions.
+
+        Parameters
+        ----------
+        data : DataArray
+            The data to be unstacked.
+
+        Returns
+        -------
+        data_unstacked : DataArray
+            The unstacked data.
+        '''
+        return super()._unstack(data)
+
+    def _reindex_dim(self, data: DataArray,  stacked_dim : str) -> DataArray:
+        return super()._reindex_dim(data, stacked_dim)
+
+    def fit_transform(
+            self,
+            data: DataArray,
+            sample_dims: Hashable | Sequence[Hashable],
+            feature_dims: Hashable | Sequence[Hashable]
+            ) -> DataArray:
+        return super().fit_transform(data, sample_dims, feature_dims)
+
+    def transform(self, data: DataArray) -> DataArray:
+        return super().transform(data)
+
     
     def inverse_transform_data(self, data: DataArray) -> DataArray:
         ''' Reshape the 2D data (sample x feature) back into its original shape.'''
 
         data = self._unstack(data)
 
         # Reindex data to original coordinates in case that some features at the boundaries were dropped
@@ -258,15 +300,15 @@
 
         # Scores are not to be reindexed since they new data typically has different sample coordinates
         # than the original data used for fitting the model
 
         return data
 
 
-class DatasetStacker(DataArrayStacker):
+class SingleDatasetStacker(SingleDataStacker):
     ''' Converts a Dataset of any dimensionality into a 2D structure.
 
     This operation generates a reshaped Dataset with two distinct dimensions: 'sample' and 'feature'.
     
     The handling of NaNs is specific: if they are found to populate an entire dimension (be it 'sample' or 'feature'), 
     they are temporarily removed during transformations and subsequently reinstated. 
     However, the presence of isolated NaNs will trigger an error.
@@ -288,71 +330,76 @@
         Returns
         -------
         data_stacked : DataArray | Dataset
             The reshaped 2d-data.
         '''
         # Raise error if dimensions feature/sample already exists in data
         if 'feature' in data.dims:
-            raise ValueError('`feature` dimension already exists in data. Please rename.')
+            raise ValueError('The dimension name `feature` conflicts with internal usage. Please rename this dimension before the analysis.')
         if 'sample' in data.dims:
-            raise ValueError('`sample` dimension already exists in data. Please rename.')
+            raise ValueError('The dimension name `sample` conflicts with internal usage. Please rename this dimension before the analysis.')
 
-        data_da = data.to_stacked_array(new_dim='feature', sample_dims=sample_dims)
+        # Convert Dataset -> DataArray, stacking all non-sample dimensions to feature dimension, including data variables
+        data_da: DataArray = data.to_stacked_array(new_dim='feature', sample_dims=sample_dims)
 
         # Rename if sample dimensions is one dimensional, otherwise stack
         if len(sample_dims) == 1:
             data_da = data_da.rename({sample_dims[0]: 'sample'})
         else:
             data_da = data_da.stack(sample=sample_dims)
 
         return data_da.transpose('sample', 'feature')
-    
+
+    def _unstack(self, data: SingleDataObject) -> SingleDataObject:
+        ''' Unstack `sample` and `feature` dimension of an DataArray to its original dimensions.'''
+        return super()._unstack(data)
+
     def _reindex_dim(self, data: Dataset, model_dim: str) -> Dataset:
-        return super()._reindex_dim(data, model_dim)  # type: ignore
+        return super()._reindex_dim(data, model_dim)
 
     def fit_transform(self, data: Dataset, sample_dims: Hashable | Sequence[Hashable], feature_dims: Hashable | Sequence[Hashable] | List[Sequence[Hashable]]) -> xr.DataArray:
-        return super().fit_transform(data, sample_dims, feature_dims)  # type: ignore
+        return super().fit_transform(data, sample_dims, feature_dims)
 
     def transform(self, data: Dataset) -> DataArray:
-        return super().transform(data)  # type: ignore
+        return super().transform(data)
 
     def inverse_transform_data(self, data: DataArray) -> Dataset:
         ''' Reshape the 2D data (sample x feature) back into its original shape.'''
-        data_ds = data.to_unstacked_dataset('variable')
+        data_ds: Dataset = data.to_unstacked_dataset('variable')
         
-        data_ds = self._unstack(data_ds) # type: ignore
+        data_ds = self._unstack(data_ds)
 
         # Reindex data to original coordinates in case that some features at the boundaries were dropped
-        data_ds = self._reindex_dim(data_ds, 'feature')  # type: ignore
+        data_ds = self._reindex_dim(data_ds, 'feature')
         data_ds = self._reindex_dim(data_ds, 'sample')
 
         return data_ds
     
     def inverse_transform_components(self, data: DataArray) -> Dataset:
         ''' Reshape the 2D data (mode x feature) back into its original shape.'''
         data_ds = data.to_unstacked_dataset('feature')
         
-        data_ds = self._unstack(data_ds)  # type: ignore
+        data_ds = self._unstack(data_ds)
 
         # Reindex data to original coordinates in case that some features at the boundaries were dropped
-        data_ds = self._reindex_dim(data_ds, 'feature')  # type: ignore
+        data_ds = self._reindex_dim(data_ds, 'feature') 
 
         return data_ds
     
     def inverse_transform_scores(self, data: DataArray) -> DataArray:
         ''' Reshape the 2D data (sample x mode) back into its original shape.'''
         data = self._unstack(data)
 
         # Scores are not to be reindexed since they new data typically has different sample coordinates
         # than the original data used for fitting the model
 
         return data
 
 
-class DataArrayListStacker():
+class ListDataArrayStacker(_BaseStacker):
     ''' Converts a list of DataArrays of any dimensionality into a 2D structure.
 
     This operation generates a reshaped DataArray with two distinct dimensions: 'sample' and 'feature'.
     
     The handling of NaNs is specific: if they are found to populate an entire dimension (be it 'sample' or 'feature'), 
     they are temporarily removed during transformations and subsequently reinstated. 
     However, the presence of isolated NaNs will trigger an error.
@@ -398,25 +445,25 @@
         self.dims_in_ = [da.dims for da in data]
         self.dims_out_ = {'sample': sample_dims, 'feature': feature_dims}
 
         # Set in/out coordinates
         self.coords_in_ = [{dim: coords for dim, coords in da.coords.items()} for da in data]
 
         for da, fdims in zip(data, feature_dims):
-            stacker = DataArrayStacker()
+            stacker = SingleDataArrayStacker()
             da_stacked = stacker.fit_transform(da, sample_dims, fdims)
             self.stackers.append(stacker)
 
         stacked_data_list = []
         idx_coords_size = []
         dummy_feature_coords = []
 
         # Stack individual DataArrays
         for da, fdims in zip(data, feature_dims):
-            stacker = DataArrayStacker()
+            stacker = SingleDataArrayStacker()
             da_stacked = stacker.fit_transform(da, sample_dims, fdims)
             idx_coords_size.append(da_stacked.coords['feature'].size)
             stacked_data_list.append(da_stacked)
         
         # Create dummy feature coordinates for each DataArray
         idx_range = np.cumsum([0] + idx_coords_size)
         for i in range(len(idx_range) - 1):
@@ -506,9 +553,10 @@
             # Inverse transform the data using the corresponding stacker
             subda = stacker.inverse_transform_components(subda)
             dalist.append(subda)
         return dalist
     
     def inverse_transform_scores(self, data: DataArray) -> DataArray:
         ''' Reshape the 2D data (sample x mode) back into its original shape.'''
-        return data.unstack()
+        return self.stackers[0].inverse_transform_scores(data)
+
```

### Comparing `xeofs-1.0.3/xeofs/utils/data_types.py` & `xeofs-1.0.5/xeofs/utils/data_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import List, TypeAlias, TypedDict, Optional, Tuple, TypeVar
 
 import xarray as xr
 
 DataArray: TypeAlias = xr.DataArray
 Dataset: TypeAlias = xr.Dataset
-XarrayData: TypeAlias = DataArray | Dataset
 DataArrayList: TypeAlias = List[DataArray]
+SingleDataObject = TypeVar('SingleDataObject', DataArray, Dataset)
+AnyDataObject = TypeVar('AnyDataObject', DataArray, Dataset, DataArrayList)
 
-
+XarrayData: TypeAlias = DataArray | Dataset
 # Model dimensions are always 2-dimensional: sample and feature
 Dims: TypeAlias = Tuple[str]
 DimsList: TypeAlias = List[Dims]
 SampleDims: TypeAlias = Dims
 FeatureDims: TypeAlias = Dims | DimsList
 # can be either like ('lat', 'lon') (1 DataArray) or (('lat', 'lon'), ('lon')) (multiple DataArrays)
 ModelDims = TypedDict('ModelDims', {'sample': SampleDims, 'feature': FeatureDims})
```

### Comparing `xeofs-1.0.3/xeofs/utils/rotation.py` & `xeofs-1.0.5/xeofs/utils/rotation.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.3/xeofs/utils/sanity_checks.py` & `xeofs-1.0.5/xeofs/utils/sanity_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from typing import Sequence, Hashable, Tuple, Any
 
 import xarray as xr
 
-def assert_dataarray(da, name):
+def assert_single_dataarray(da, name):
     """Check if the given object is a DataArray.
 
     Args:
         da (DataArray): The object to check.
         name (str): The name of the object.
 
     Raises:
         TypeError: If the object is not a DataArray.
     """
     if not isinstance(da, xr.DataArray):
         raise TypeError(f"{name} must be a DataArray")
     
-def assert_list_of_dataarrays(da_list, name):
+def assert_list_dataarrays(da_list, name):
     """Check if the given object is a list of DataArrays.
 
     Args:
         da_list (list): The object to check.
         name (str): The name of the object.
 
     Raises:
         TypeError: If the object is not a list of DataArrays.
     """
     if not isinstance(da_list, list):
         raise TypeError(f"{name} must be a list of DataArrays")
     for da in da_list:
-        assert_dataarray(da, name)
+        assert_single_dataarray(da, name)
 
-def assert_dataset(ds, name):
+def assert_single_dataset(ds, name):
     """Check if the given object is a Dataset.
 
     Args:
         ds (Dataset): The object to check.
         name (str): The name of the object.
 
     Raises:
```

### Comparing `xeofs-1.0.3/xeofs/utils/statistics.py` & `xeofs-1.0.5/xeofs/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `xeofs-1.0.3/xeofs/utils/xarray_utils.py` & `xeofs-1.0.5/xeofs/utils/xarray_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,55 @@
 from typing import List, Sequence, Hashable, Tuple
 
 import numpy as np
 import xarray as xr
 from scipy.signal import hilbert    # type: ignore
 
 from .sanity_checks import ensure_tuple
-from .data_types import XarrayData, DataArray, Dataset
+from .data_types import XarrayData, DataArray, Dataset, SingleDataObject
+from .constants import VALID_LATITUDE_NAMES
+
+
+def compute_sqrt_cos_lat_weights(data: SingleDataObject, dim: Hashable | Sequence[Hashable]) -> SingleDataObject:
+        '''Compute the square root of cosine of latitude weights.
+
+        Parameters
+        ----------
+        data : xarray.DataArray or xarray.Dataset
+            Data to be scaled.
+        dim : sequence of hashable 
+            Dimensions along which the data is considered to be a feature.
+            
+        Returns
+        -------
+        xarray.DataArray or xarray.Dataset
+            Square root of cosine of latitude weights.
+
+        '''
+        dim = ensure_tuple(dim)
+
+        # Find latitude coordinate
+        is_lat_coord = np.isin(np.array(dim), VALID_LATITUDE_NAMES)
+
+        # Select latitude coordinate and compute coslat weights
+        lat_coord = np.array(dim)[is_lat_coord]
+        
+        if len(lat_coord) > 1:
+            raise ValueError(f'{lat_coord} are ambiguous latitude coordinates. Only ONE of the following is allowed for computing coslat weights: {VALID_LATITUDE_NAMES}')
+
+        if len(lat_coord) == 1:
+            latitudes = data.coords[lat_coord[0]]
+            weights = sqrt_cos_lat_weights(latitudes)
+            # Features that cannot be associated to a latitude receive a weight of 1
+            weights = weights.where(weights.notnull(), 1)
+        else:
+            raise ValueError('No latitude coordinate was found to compute coslat weights. Must be one of the following: {:}'.format(VALID_LATITUDE_NAMES))
+        weights.name = 'coslat_weights'
+        return weights
+
 
 def get_dims(
         data: DataArray | Dataset | List[DataArray],
         sample_dims: Hashable | Sequence[Hashable] | List[Sequence[Hashable]]
         ) -> Tuple[Hashable, Hashable]:
     '''Extracts the dimensions of a DataArray or Dataset that are not included in the sample dimensions.
 
@@ -60,15 +100,15 @@
         Feature dimensions.        
 
     '''
     feature_dims = tuple(dim for dim in data.dims if dim not in sample_dims)
     return feature_dims
 
 
-def sqrt_cos_lat_weights(data: DataArray | Dataset) -> DataArray | Dataset:
+def sqrt_cos_lat_weights(data: SingleDataObject) -> SingleDataObject:
     '''Compute the square root of the cosine of the latitude.
 
     Parameters:
     ------------
     data: xr.DataArray or xr.Dataset
         Input data.
 
@@ -82,39 +122,32 @@
         _np_sqrt_cos_lat_weights,
         data,
         vectorize=False,
         dask='allowed',
     )
 
 
-def total_variance(data: DataArray) -> DataArray:
+def total_variance(data: DataArray, dim) -> DataArray:
     '''Compute the total variance of the input data.
     
     Parameters:
     ------------
     data: DataArray
         Input data.
+    
+    dim: str
+        Dimension along which to compute the total variance.
 
     Returns:
     ---------
     tot_var: DataArray
         Total variance of the input data.
 
     '''
-    tot_var = xr.apply_ufunc(
-        _np_total_variance,
-        data,
-        input_core_dims=[['sample', 'feature']],
-        output_core_dims=[[]],
-        vectorize=False,
-        dask='allowed',
-        output_dtypes=[float],
-    )
-    tot_var.name = 'total_variance'
-    return tot_var
+    return data.var(dim, ddof=1).sum()
 
 def hilbert_transform(data: DataArray, dim, padding='exp', decay_factor=.2) -> DataArray:
     '''Hilbert transform with optional padding to mitigate spectral leakage.
 
     Parameters:
     ------------
     data: DataArray
@@ -154,31 +187,14 @@
     ---------
     sqrt_cos_lat: np.ndarray
         Square root of the cosine of the latitude.
 
     '''
     return np.sqrt(np.cos(np.deg2rad(data))).clip(0, 1)
 
-def _np_total_variance(arr):
-    '''Compute the total variance of the input data.
-
-    Parameters:
-    ------------
-    arr: np.ndarray
-        Input data.
-    
-    Returns:
-    ---------
-    tot_var: float
-        Total variance of the input data.
-
-    '''
-    C = (arr * arr.conj()).sum(axis=0) / (arr.shape[0] - 1)
-    return C.sum().real
-
 
 def _hilbert_transform_with_padding(y, padding='exp', decay_factor=.2):
     '''Hilbert transform with optional padding to mitigate spectral leakage.
     
     Parameters:
     ------------
     y: np.ndarray
```

### Comparing `xeofs-1.0.3/PKG-INFO` & `xeofs-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeofs
-Version: 1.0.3
+Version: 1.0.5
 Summary: Collection of EOF analysis and related techniques for climate science
 Home-page: https://github.com/nicrie/xeofs
 License: MIT
 Author: Niclas Rieger
 Author-email: niclasrieger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

