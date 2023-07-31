# Comparing `tmp/gscrew-1.0.6.tar.gz` & `tmp/gscrew-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gscrew-1.0.6.tar", last modified: Wed Jul 26 22:01:36 2023, max compression
+gzip compressed data, was "gscrew-1.0.7.tar", last modified: Mon Jul 31 15:54:49 2023, max compression
```

## Comparing `gscrew-1.0.6.tar` & `gscrew-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:01:36.208686 gscrew-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 22:01:26.000000 gscrew-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-26 22:01:36.208686 gscrew-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-26 22:01:26.000000 gscrew-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:01:36.208686 gscrew-1.0.6/gscrew/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 22:01:26.000000 gscrew-1.0.6/gscrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-26 22:01:26.000000 gscrew-1.0.6/gscrew/geometric_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-07-26 22:01:26.000000 gscrew-1.0.6/gscrew/screw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:01:36.208686 gscrew-1.0.6/gscrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-26 22:01:36.000000 gscrew-1.0.6/gscrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-26 22:01:36.000000 gscrew-1.0.6/gscrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:01:36.000000 gscrew-1.0.6/gscrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 22:01:36.000000 gscrew-1.0.6/gscrew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 22:01:36.000000 gscrew-1.0.6/gscrew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-26 22:01:26.000000 gscrew-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 22:01:26.000000 gscrew-1.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 22:01:36.208686 gscrew-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 22:01:26.000000 gscrew-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:54:49.815842 gscrew-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-31 15:54:26.000000 gscrew-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-31 15:54:49.815842 gscrew-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-31 15:54:26.000000 gscrew-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:54:49.815842 gscrew-1.0.7/gscrew/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 15:54:26.000000 gscrew-1.0.7/gscrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22395 2023-07-31 15:54:26.000000 gscrew-1.0.7/gscrew/geometric_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-07-31 15:54:26.000000 gscrew-1.0.7/gscrew/screw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:54:49.815842 gscrew-1.0.7/gscrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-31 15:54:49.000000 gscrew-1.0.7/gscrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-31 15:54:49.000000 gscrew-1.0.7/gscrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:54:49.000000 gscrew-1.0.7/gscrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-31 15:54:49.000000 gscrew-1.0.7/gscrew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 15:54:49.000000 gscrew-1.0.7/gscrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-31 15:54:26.000000 gscrew-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 15:54:26.000000 gscrew-1.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:54:49.815842 gscrew-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 15:54:26.000000 gscrew-1.0.7/setup.py
```

### Comparing `gscrew-1.0.6/LICENSE` & `gscrew-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gscrew-1.0.6/PKG-INFO` & `gscrew-1.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: gscrew
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
 Author: Antoine Royer, Loris Delafosse
-Project-URL: Homepage, https://github.com/Shadow15510/GScrew
+Project-URL: Homepage, https://github.com/GenScrew/GScrew
 Project-URL: Documentation, http://gscrew.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 License-File: LICENSE
 
 # GScrew (Generalized Screw Calculus)
 [![Documentation Status](https://readthedocs.org/projects/gscrew/badge/?version=latest)](https://gscrew.readthedocs.io/en/latest/?badge=latest)
-[![Licence](https://img.shields.io/github/license/Shadow15510/GScrew?color=green)](https://github.com/Shadow15510/GScrew/blob/master/LICENSE)
-[![Build Status](https://github.com/Shadow15510/GScrew/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Shadow15510/GScrew/blob/master/.github/workflows/python-publish.yml)
+[![Licence](https://img.shields.io/github/license/GenScrew/GScrew?color=green)](https://github.com/GenScrew/GScrew/blob/master/LICENSE)
+[![Build Status](https://github.com/GenScrew/GScrew/actions/workflows/python-publish.yml/badge.svg)](https://github.com/GenScrew/GScrew/blob/master/.github/workflows/python-publish.yml)
 
 ## Description
 A Python module to manipulate generalized Screws and Coscrews with geometric algebras (real Clifford algebras).
 
-- [readthedocs Documentation](https://gscrew.readthedocs.io/en/latest/).
-- [Bug tracker](https://github.com/Shadow15510/GScrew/issues).
+- [readthedocs Documentation](https://gscrew.readthedocs.io/en/latest/)
+- [Bug tracker](https://github.com/GenScrew/GScrew/issues)
 
 ## Installation
 A Pypi package is available, please refer to the [Pypi page](https://pypi.org/project/GScrew/) or enter `pip install gscrew` in a terminal.
 
 ## Exemples
 First of all, you need to import the modules:
 ```
@@ -36,19 +36,19 @@
 The `screw` module also provides a `CoScrew` object and the `comoment` function for calculating the comoment between a coscrew and a screw.
 
 Once these modules have been imported, we can create the geometric algebra in which we will be working. For basic physical applications, a three-dimensionnal algebra should suffice:
 ```
 my_algebra = ga.GeometricAlgebra(3)
 locals().update(my_algebra.blades)
 ```
-The second line adds the basis blades to the local variables so that we will be able to create new multivectors just by performing linear combinations of these basis blades. For a 3D algebra, the basis blades are: e0, e1, e2, e3, e12, e13, e32, e123.
+The second line adds the basis blades to the local variables so that we will be able to create new multivectors just by performing linear combinations of these basis blades. For a 3D algebra, the basis blades are: s, e1, e2, e3, e12, e13, e32, e123.
 
 We can now start working with Screw and CoScrew classes:
 ```
-O = 0 * e0  # the origin of the reference frame
+O = 0 * s  # the origin of the reference frame
 S = 1 + (2*e2) + (3*e3)  # the direction of the screw
 M = (e1) + (5*e3)        # the moment of the screw
 my_screw = Screw(O, S, M)
 ```
 
 ## Licence
 All the code is provided under the GNU General Public Licence v3.0+ (GPLv3+)
```

### Comparing `gscrew-1.0.6/README.md` & `gscrew-1.0.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # GScrew (Generalized Screw Calculus)
 [![Documentation Status](https://readthedocs.org/projects/gscrew/badge/?version=latest)](https://gscrew.readthedocs.io/en/latest/?badge=latest)
-[![Licence](https://img.shields.io/github/license/Shadow15510/GScrew?color=green)](https://github.com/Shadow15510/GScrew/blob/master/LICENSE)
-[![Build Status](https://github.com/Shadow15510/GScrew/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Shadow15510/GScrew/blob/master/.github/workflows/python-publish.yml)
+[![Licence](https://img.shields.io/github/license/GenScrew/GScrew?color=green)](https://github.com/GenScrew/GScrew/blob/master/LICENSE)
+[![Build Status](https://github.com/GenScrew/GScrew/actions/workflows/python-publish.yml/badge.svg)](https://github.com/GenScrew/GScrew/blob/master/.github/workflows/python-publish.yml)
 
 ## Description
 A Python module to manipulate generalized Screws and Coscrews with geometric algebras (real Clifford algebras).
 
-- [readthedocs Documentation](https://gscrew.readthedocs.io/en/latest/).
-- [Bug tracker](https://github.com/Shadow15510/GScrew/issues).
+- [readthedocs Documentation](https://gscrew.readthedocs.io/en/latest/)
+- [Bug tracker](https://github.com/GenScrew/GScrew/issues)
 
 ## Installation
 A Pypi package is available, please refer to the [Pypi page](https://pypi.org/project/GScrew/) or enter `pip install gscrew` in a terminal.
 
 ## Exemples
 First of all, you need to import the modules:
 ```
@@ -21,19 +21,19 @@
 The `screw` module also provides a `CoScrew` object and the `comoment` function for calculating the comoment between a coscrew and a screw.
 
 Once these modules have been imported, we can create the geometric algebra in which we will be working. For basic physical applications, a three-dimensionnal algebra should suffice:
 ```
 my_algebra = ga.GeometricAlgebra(3)
 locals().update(my_algebra.blades)
 ```
-The second line adds the basis blades to the local variables so that we will be able to create new multivectors just by performing linear combinations of these basis blades. For a 3D algebra, the basis blades are: e0, e1, e2, e3, e12, e13, e32, e123.
+The second line adds the basis blades to the local variables so that we will be able to create new multivectors just by performing linear combinations of these basis blades. For a 3D algebra, the basis blades are: s, e1, e2, e3, e12, e13, e32, e123.
 
 We can now start working with Screw and CoScrew classes:
 ```
-O = 0 * e0  # the origin of the reference frame
+O = 0 * s  # the origin of the reference frame
 S = 1 + (2*e2) + (3*e3)  # the direction of the screw
 M = (e1) + (5*e3)        # the moment of the screw
 my_screw = Screw(O, S, M)
 ```
 
 ## Licence
 All the code is provided under the GNU General Public Licence v3.0+ (GPLv3+)
```

### Comparing `gscrew-1.0.6/gscrew/geometric_algebra.py` & `gscrew-1.0.7/gscrew/geometric_algebra.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,19 @@
     nb_blades : int
         The number of basis blades the algebra has.
     blades_by_grade : list
         The number of basis blades per grade.
         e.g. for a 3D-algebra, it will be ``[1, 3, 3, 1]``
     blades_ids : list
         It contains the ids of the basis blades.
-        e.g. for a 2D-algebra, the basis blades are: ``e0, e1, e2, e12`` so the ids will be:
+        e.g. for a 2D-algebra, the basis blades are: ``s, e1, e2, e12`` so the ids will be:
         ``[(), (1,), (2,), (1, 2)]``.
     blades : dict
         This dictionnary contains the basis blades: ``{name: value}`` where
-        ``name`` is a string (e.g. ``'e0'``, ``'e1'``, ``'e2'`` etc) and ``value`` the associated
+        ``name`` is a string (e.g. ``'s'``, ``'e1'``, ``'e2'`` etc) and ``value`` the associated
         MultiVector instance.
 
     Methods
     -------
     .. automethod:: __init__
     .. automethod:: get_grade
     """
@@ -80,15 +80,15 @@
             ))
 
         names = []
         for index, blade_name in enumerate(blades_names):
             if index:
                 names.append("e" + "".join(map(str, blade_name)))
             else:
-                names.append("e0")
+                names.append("s")
 
         value = np.zeros(self.nb_blades)
         for i in range(self.nb_blades):
             value[i] = 1
             self.blades[names[i]] = MultiVector(self, value)
             value[i] = 0
 
@@ -188,15 +188,15 @@
     Exemples
     --------
     Let's show you a complete exemple of a manipulation of MultiVector.
     You must start by importing the module::
 
         >>> import geometric_algebra as ga
         >>> geo_alg = ga.GeometricAlgebra(3)  # you should give the dimension of the algebra
-        >>> locals().update(geo_alg.blades)   # import the basis blades e.g. e0, e1, e2, e3, e12 etc
+        >>> locals().update(geo_alg.blades)   # import the basis blades e.g. s, e1, e2, e3, e12 etc
 
     Then you have fully initialize the module. To create a new MultiVector instance, you have two
     possibilities. The first one is also the easiest::
 
         >>> my_mv = 1 + 1*e1 + 5*e2 + (1/5) * e13
 
     You can also call the constructor method manually::
@@ -464,44 +464,32 @@
         return string.strip()
 
     def __rmul__(self, other):
         """Compute the right-hand geometrical product ``other * self``.
 
         Parameters
         ----------
-        other : MultiVector, scalar
-            The MultiVector or scalar to multiply.
+        other : scalar
+            The scalar to multiply.
 
         Returns
         -------
         out : MultiVector
             The result of the geometrical product.
 
         Raises
         ------
         TypeError
-            If ``other`` is neither a scalar nor a MultiVector instance.
+            If ``other`` is not a scalar.
         """
         if np.isscalar(other):
             return MultiVector(self.geo_alg, other * self.value)
 
-        if not isinstance(other, MultiVector):
-            raise TypeError(f"other must be a scalar or a MultiVector instance instead of "\
-                    f"{type(other)}"
-                )
-
-        new_value = np.zeros(self.geo_alg.nb_blades)
-        for i in range(self.geo_alg.nb_blades):
-            if other[i]:
-                for j in range(self.geo_alg.nb_blades):
-                    if self[j]:
-                        index, sgn = self.__mul_basis(j, i)
-                        new_value[index] += sgn * other[i] * self[j]
-
-        return MultiVector(self.geo_alg, new_value)
+        else:
+            raise TypeError(f"other must be a scalar instead of {type(other)}")
 
     def __rsub__(self, other):
         """Compute the subtraction ``other - self``.
 
         Parameters
         ----------
         other : MultiVector, scalar
@@ -555,17 +543,15 @@
             return other * self
 
         if not isinstance(other, MultiVector):
             raise TypeError(f"other must be a scalar or a MultiVector instance instead of "\
                     f"{type(other)}"
                 )
 
-        if self == other:
-            return MultiVector(self.geo_alg)
-        return (other * self) - (other | self)
+        return other ^ self
 
     __str__ = __repr__
 
     def __sub__(self, other):
         """Compute the subtraction ``self - other``.
 
         Parameters
@@ -648,17 +634,21 @@
             return self * other
 
         if not isinstance(other, MultiVector):
             raise TypeError(f"other must be a scalar or a MultiVector instance instead of "\
                     f"{type(other)}"
                 )
 
-        if self == other:
-            return MultiVector(self.geo_alg)
-        return (self * other) - (self | other)
+        new_mv = MultiVector(self.geo_alg)
+        for gd1 in range(self.geo_alg.dim):
+            for gd2 in range(self.geo_alg.dim):
+                if gd1 + gd2 <= self.geo_alg.dim:
+                    new_mv += (self(gd1) * other(gd2))(gd1 + gd2)
+
+        return new_mv
 
     def __mul_basis(self, index1: int, index2: int):
         """Compute the geometrical product between two basis blades.
 
         Parameters
         ----------
         index1 : int
```

### Comparing `gscrew-1.0.6/gscrew/screw.py` & `gscrew-1.0.7/gscrew/screw.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 Let's see a minimal exemple::
 
     >>> import geometric_algebra as ga
     >>> from screw import Screw
     >>> my_algebra = ga.GeometricAlgebra(3)  # a 3-D geometric algebra
     >>> locals().update(my_algebra.blades)   # add the basis blades to the locals (i.e. 1, e1, e2…)
-    >>> reference_point = 0*e0           # the point of reference for the screw (here, the origin)
+    >>> reference_point = 0*s            # the point of reference for the screw (here, the origin)
     >>> direction = 2 + (3*e1) + (6*e3)  # creates a MultiVector for the screw's direction
     >>> moment = (2*e1) + (5*e2) + e3    # creates another MultiVector for the screw's moment
     >>> my_screw = Screw(reference_point, direction, moment)  # finally we create a Screw instance
 """
 
 
 class ScrewBase:
```

### Comparing `gscrew-1.0.6/gscrew.egg-info/PKG-INFO` & `gscrew-1.0.7/gscrew.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: gscrew
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
 Author: Antoine Royer, Loris Delafosse
-Project-URL: Homepage, https://github.com/Shadow15510/GScrew
+Project-URL: Homepage, https://github.com/GenScrew/GScrew
 Project-URL: Documentation, http://gscrew.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 License-File: LICENSE
 
 # GScrew (Generalized Screw Calculus)
 [![Documentation Status](https://readthedocs.org/projects/gscrew/badge/?version=latest)](https://gscrew.readthedocs.io/en/latest/?badge=latest)
-[![Licence](https://img.shields.io/github/license/Shadow15510/GScrew?color=green)](https://github.com/Shadow15510/GScrew/blob/master/LICENSE)
-[![Build Status](https://github.com/Shadow15510/GScrew/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Shadow15510/GScrew/blob/master/.github/workflows/python-publish.yml)
+[![Licence](https://img.shields.io/github/license/GenScrew/GScrew?color=green)](https://github.com/GenScrew/GScrew/blob/master/LICENSE)
+[![Build Status](https://github.com/GenScrew/GScrew/actions/workflows/python-publish.yml/badge.svg)](https://github.com/GenScrew/GScrew/blob/master/.github/workflows/python-publish.yml)
 
 ## Description
 A Python module to manipulate generalized Screws and Coscrews with geometric algebras (real Clifford algebras).
 
-- [readthedocs Documentation](https://gscrew.readthedocs.io/en/latest/).
-- [Bug tracker](https://github.com/Shadow15510/GScrew/issues).
+- [readthedocs Documentation](https://gscrew.readthedocs.io/en/latest/)
+- [Bug tracker](https://github.com/GenScrew/GScrew/issues)
 
 ## Installation
 A Pypi package is available, please refer to the [Pypi page](https://pypi.org/project/GScrew/) or enter `pip install gscrew` in a terminal.
 
 ## Exemples
 First of all, you need to import the modules:
 ```
@@ -36,19 +36,19 @@
 The `screw` module also provides a `CoScrew` object and the `comoment` function for calculating the comoment between a coscrew and a screw.
 
 Once these modules have been imported, we can create the geometric algebra in which we will be working. For basic physical applications, a three-dimensionnal algebra should suffice:
 ```
 my_algebra = ga.GeometricAlgebra(3)
 locals().update(my_algebra.blades)
 ```
-The second line adds the basis blades to the local variables so that we will be able to create new multivectors just by performing linear combinations of these basis blades. For a 3D algebra, the basis blades are: e0, e1, e2, e3, e12, e13, e32, e123.
+The second line adds the basis blades to the local variables so that we will be able to create new multivectors just by performing linear combinations of these basis blades. For a 3D algebra, the basis blades are: s, e1, e2, e3, e12, e13, e32, e123.
 
 We can now start working with Screw and CoScrew classes:
 ```
-O = 0 * e0  # the origin of the reference frame
+O = 0 * s  # the origin of the reference frame
 S = 1 + (2*e2) + (3*e3)  # the direction of the screw
 M = (e1) + (5*e3)        # the moment of the screw
 my_screw = Screw(O, S, M)
 ```
 
 ## Licence
 All the code is provided under the GNU General Public Licence v3.0+ (GPLv3+)
```

### Comparing `gscrew-1.0.6/pyproject.toml` & `gscrew-1.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,9 +36,9 @@
 [tool.setuptools.dynamic.version]
 attr = "gscrew.__init__.__version__"
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
-Homepage = "https://github.com/Shadow15510/GScrew"
+Homepage = "https://github.com/GenScrew/GScrew"
 Documentation = "http://gscrew.readthedocs.io/"
```

