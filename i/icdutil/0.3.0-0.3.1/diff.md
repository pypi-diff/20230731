# Comparing `tmp/icdutil-0.3.0.tar.gz` & `tmp/icdutil-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icdutil-0.3.0.tar", max compression
+gzip compressed data, was "icdutil-0.3.1.tar", max compression
```

## Comparing `icdutil-0.3.0.tar` & `icdutil-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-07-27 13:39:32.958471 icdutil-0.3.0/LICENSE
--rw-r--r--   0        0        0     1178 2023-07-27 13:39:32.958471 icdutil-0.3.0/README.md
--rw-r--r--   0        0        0     1177 2023-07-27 13:39:32.958471 icdutil-0.3.0/icdutil/__init__.py
--rw-r--r--   0        0        0    30406 2023-07-27 13:39:32.958471 icdutil-0.3.0/icdutil/addrmap.py
--rw-r--r--   0        0        0    15292 2023-07-27 13:39:32.958471 icdutil-0.3.0/icdutil/addrrange.py
--rw-r--r--   0        0        0    20747 2023-07-27 13:39:32.958471 icdutil-0.3.0/icdutil/num.py
--rw-r--r--   0        0        0     8151 2023-07-27 13:39:32.958471 icdutil-0.3.0/icdutil/slices.py
--rw-r--r--   0        0        0     2242 2023-07-27 13:39:32.958471 icdutil-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 icdutil-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-31 06:41:43.274390 icdutil-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1178 2023-07-31 06:41:43.274390 icdutil-0.3.1/README.md
+-rw-r--r--   0        0        0     1177 2023-07-31 06:41:43.274390 icdutil-0.3.1/icdutil/__init__.py
+-rw-r--r--   0        0        0    30047 2023-07-31 06:41:43.274390 icdutil-0.3.1/icdutil/addrmap.py
+-rw-r--r--   0        0        0    15275 2023-07-31 06:41:43.274390 icdutil-0.3.1/icdutil/addrrange.py
+-rw-r--r--   0        0        0    20750 2023-07-31 06:41:43.274390 icdutil-0.3.1/icdutil/num.py
+-rw-r--r--   0        0        0     8151 2023-07-31 06:41:43.274390 icdutil-0.3.1/icdutil/slices.py
+-rw-r--r--   0        0        0     2242 2023-07-31 06:41:43.274390 icdutil-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 icdutil-0.3.1/PKG-INFO
```

### Comparing `icdutil-0.3.0/LICENSE` & `icdutil-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `icdutil-0.3.0/README.md` & `icdutil-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `icdutil-0.3.0/icdutil/__init__.py` & `icdutil-0.3.1/icdutil/__init__.py`

 * *Files identical despite different names*

### Comparing `icdutil-0.3.0/icdutil/addrmap.py` & `icdutil-0.3.1/icdutil/addrmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,25 +78,25 @@
         ...
     icdutil.addrmap.Conflict: AddrRange('D', 0x2000, '8 KB'): overlaps with AddrRange('B', 0x2000, '4 KB').
     >>> a.add('D', 0x1800, '4 KB')
     Traceback (most recent call last):
         ...
     icdutil.addrmap.Conflict: AddrRange('D', 0x1800, '4 KB'): overlaps with AddrRange('B', 0x2000, '4 KB').
 
-    An iteration will serve :class:`AddrRange` objects sorted by baseaddr.
+    An iteration will serve :class:`AddrRange` objects sorted by baseaddr:
+
     >>> for addrrange in a:
     ...     addrrange
     AddrRange('T', 0x0, '1 KB')
     AddrRange('B', 0x2000, '4 KB')
     AddrRange('A', 0x5000, '4 KB')
     AddrRange('C', 0xD000, '2 KB')
     AddrRange('Z', 0xE000, '4 KB')
     AddrRange('X', 0xF0800000, '3 MB')
 
-
     The size is defined by the numer of entries:
 
     >>> len(a)
     6
 
     By using a `default` the gaps are filled with this item:
 
@@ -113,15 +113,15 @@
     AddrRange('Z', 0xE000, '4 KB')
     AddrRange('d', 0xF000, '3.76 GB')
     AddrRange('X', 0xF0800000, '3 MB')
     AddrRange('d', 0xF0B00000, '245 MB')
     >>> len(tuple(a.get('d')))
     12
 
-    The `is_sub` attribute defines the address range defaults.
+    The `is_sub` attribute defines the address range defaults:
 
     >>> b = AddrMap(addrwidth=32, is_sub=True)
     >>> b
     AddrMap(addrwidth=32, is_sub=True)
     >>> b.add('T', size=0x400)
     AddrRange('T', 0x00000000, '1 KB', addrwidth=32, is_sub=True)
     >>> b.add('A', 0x5000, 0x1000)
@@ -237,15 +237,15 @@
             return None
 
     @property
     def eff_addrwidth(self) -> typing.Optional[int]:
         """
         Effective Address Width.
 
-        Return address with if explicitly set or calculated from existing entries.
+        Return address width, either explicitly set or calculated from existing entries.
 
         >>> a = AddrMap()
         >>> a.eff_addrwidth
         >>> a.add('A', 0x5000, '4 KB')
         AddrRange('A', 0x5000, '4 KB')
         >>> a.eff_addrwidth
         15
@@ -467,31 +467,26 @@
             last = cuts[-1]
             lastaddr = self.lastaddr
             # remove
             for idx in reversed(idxs):
                 addrranges.pop(idx)
             # re-add left overlap
             if addrrange.baseaddr:
-                # left = first.get_intersect(AddrRange(0, addrrange.baseaddr))
-                # print("BOZO", first, addrrange)
                 left = first.get_difference(addrrange)
                 if left:
                     self.__add(left[0])
             # re-add right overlap
             if lastaddr > addrrange.endaddr:
-                # right = last.get_intersect(AddrRange(addrrange.endaddr + 1, lastaddr - addrrange.endaddr))
                 right = last.get_difference(addrrange)
                 if right:
                     self.__add(right[0])
             # shrink cuts
             cuts[0] = first.get_intersect(addrrange)
-            # cuts[0] = first.get_difference(addrrange)[0]
             if first is not last:
                 cuts[-1] = last.get_intersect(addrrange)
-                # cuts[-1] = last.get_difference(addrrange)[0]
         return cuts
 
     def __match(self, addrrange: "AddrRange"):
         return [a for a in self if a.is_overlapping(addrrange)]
 
     @staticmethod
     def _align(addr, align):
@@ -664,15 +659,15 @@
         []
         >>> list(a.get(default="<default>"))
         []
         >>> a = AddrMap(addrwidth=16)
         >>> list(a.get(default="<default>"))
         [AddrRange('<default>', 0x0000, '64 KB', addrwidth=16)]
 
-        # default items before and after real AddrRange:
+        Default items before and after real AddrRange:
 
         >>> a.add('A', 0x5000, 0x1000)
         AddrRange('A', 0x5000, '4 KB', addrwidth=16)
         >>> for addrrange in a.get(default='reserved'):
         ...     addrrange
         AddrRange('reserved', 0x0000, '20 KB', addrwidth=16)
         AddrRange('A', 0x5000, '4 KB', addrwidth=16)
@@ -689,15 +684,15 @@
         """
         return self.__get(default)
 
     def cut(self, baseaddr, size=1) -> "AddrMap":
         """
         Cut out address range from `baseaddr` for `size`.
 
-        Return address map with cutted address ranges.
+        Return address map with cut address ranges.
 
         >>> a = AddrMap()
         >>> a.add('A', 0x0000, 0x1000)
         AddrRange('A', 0x0, '4 KB')
         >>> a.add('B', 0x1000, 0x1000)
         AddrRange('B', 0x1000, '4 KB')
         >>> a.add('C', 0x2000, 0x1000)
```

### Comparing `icdutil-0.3.0/icdutil/addrrange.py` & `icdutil-0.3.1/icdutil/addrrange.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,31 +72,35 @@
         >>> a
         AddrRange(0x00001000, '256 bytes', addrwidth=32)
         >>> str(a)
         '0x00001000-0x000010FF(256 bytes)'
         >>> str(a.nextaddr)
         '0x00001100'
 
-        Address ranges can be compared
+        Address ranges can be compared:
+
         >>> AddrRange(0x1000, 0x100) == AddrRange(0x1000, 0x100)
         True
         >>> AddrRange(0x1000, 0x100) == AddrRange(0x1000, 0x200)
         False
 
         Comparing an AddrRange against another type just returns False:
+
         >>> AddrRange(0x1000, 0x100) == 42
         False
 
-        Addresses can be checked whether they lie within the range
+        Addresses can be checked whether they lie within the range:
+
         >>> 0x1008 in a
         True
         >>> 0x1400 in a
         False
 
-        Address ranges can be iterated over
+        Address ranges can be iterated over:
+
         >>> for i in AddrRange(0x200, 6):
         ...     print(i)
         512
         513
         514
         515
         516
@@ -185,15 +189,16 @@
         Absolute AddrRanges just lead to the intersection:
 
         >>> AddrRange(0x1000, '4 KB').get_intersect(AddrRange(0x2000, '4 KB'))
         >>> AddrRange(0x1000, '4 KB').get_intersect(AddrRange(0x2000, 0x1))
         >>> AddrRange(0x1000, '4 KB').get_intersect(AddrRange(0x1FFF, 0x1))
         AddrRange(0x1FFF, '1 byte')
 
-        Remark: This should not be 4 KB, but 4095, this is a quirk of the humandfriendly package!
+        Remark: humandfriendly package is rounding 4095 bytes to 4 KB.
+
         >>> a = AddrRange(0x1000, '4 KB').get_intersect(AddrRange(0x1000, 0xFFF))
         >>> a
         AddrRange(0x1000, '4 KB')
         >>> int(a.size)
         4095
         >>> AddrRange(0x1000, '4 KB').get_intersect(AddrRange(0x1000, '4 KB'))
         AddrRange(0x1000, '4 KB')
@@ -296,14 +301,15 @@
         >>> AddrRange(0x1000, '4 KB', is_sub=True).get_difference(AddrRange(0x800, '12 KB', is_sub=True))
         []
         >>> AddrRange(0x1000, '4 KB', is_sub=True).get_difference(AddrRange(0x1FFF, 0x1, is_sub=True))
         [AddrRange(0x1000, '4 KB', is_sub=True)]
 
         If only one of the AddrRange is absolute, the sub range is taken relative to the absolute.
         If `self` is a subrange, then the difference is again a subrange w/r/t to the absolute range.
+
         >>> AddrRange(0x1000, '4 KB').get_difference(AddrRange(0x2000, '4 KB', is_sub=True))
         [AddrRange(0x1000, '4 KB')]
         >>> AddrRange(0x1000, '4 KB', is_sub=True).get_difference(AddrRange(0x2000, '4 KB'))
         [AddrRange(0x1000, '4 KB', is_sub=True)]
         >>> AddrRange(0x1000, '4 KB').get_difference(AddrRange(0x800, '2 KB', is_sub=True))
         [AddrRange(0x1000, '2 KB')]
         >>> AddrRange(0x1000, '4 KB').get_difference(AddrRange(0x800, '1 KB', is_sub=True))
@@ -311,14 +317,15 @@
         >>> AddrRange(0x1000, '4 KB', is_sub=True).get_difference(AddrRange(0x800, '4 KB'))
         [AddrRange(0x1000, '4 KB', is_sub=True)]
         >>> AddrRange(0x400, '4 KB', is_sub=True).get_difference(AddrRange(0xF0000800, '4 KB'))
         [AddrRange(0x1000, '1 KB', is_sub=True)]
 
         Regardless of the `other` range, the difference always inherits addrwidth, the item (if there is any) and
         the is_sub attribute:
+
         >>> AddrRange(0x1000, '4 KB', item='A').get_difference(AddrRange(0x1800, '4 KB', item='B'))
         [AddrRange('A', 0x1000, '2 KB')]
         >>> AddrRange(0x1000, '4 KB', addrwidth=16).get_difference(AddrRange(0x1800, '4 KB', addrwidth=18))
         [AddrRange(0x1000, '2 KB', addrwidth=16)]
         """
 
         res = []
```

### Comparing `icdutil-0.3.0/icdutil/num.py` & `icdutil-0.3.1/icdutil/num.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,29 +429,32 @@
     8
     >>> align(8, align=4)
     8
     >>> align(9, align=4)
     12
 
     A `minalign` without `align` forwards the value to the next multiple of `minalign`
+
     >>> align(5, minalign=4)
     8
     >>> align(8, minalign=4)
     8
     >>> align(9, minalign=4)
     12
 
     If both `align` and `minalign` are given, then the value is moved to the next multiple
     of whichever of the both align values is bigger
+
     >>> align(8, align=5, minalign=4)
     10
     >>> align(8, align=4, minalign=6)
     12
 
     If `offset` is given it is dominant over both `align` and `minalign`
+
     >>> align(8, offset=9, align=4, minalign=6)
     9
     """
     if offset is not None:
         if not rewind and value > offset:
             raise AlignError(f"Cannot use offset {offset} as we are already at {value}")
         return offset
```

### Comparing `icdutil-0.3.0/icdutil/slices.py` & `icdutil-0.3.1/icdutil/slices.py`

 * *Files identical despite different names*

### Comparing `icdutil-0.3.0/pyproject.toml` & `icdutil-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "icdutil"
-version = "0.3.0"
+version = "0.3.1"
 description = "IC Design Utilities"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `icdutil-0.3.0/PKG-INFO` & `icdutil-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icdutil
-Version: 0.3.0
+Version: 0.3.1
 Summary: IC Design Utilities
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

