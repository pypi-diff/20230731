# Comparing `tmp/py3afipws-0.8.tar.gz` & `tmp/py3afipws-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py3afipws-0.8.tar", last modified: Thu Jul  4 02:18:38 2019, max compression
+gzip compressed data, was "dist/py3afipws-0.9.tar", last modified: Thu Jul  4 03:03:46 2019, max compression
```

## Comparing `py3afipws-0.8.tar` & `py3afipws-0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 jovix     (1000) jovix     (1000)        0 2019-07-04 02:18:38.000000 py3afipws-0.8/
--rw-r--r--   0 jovix     (1000) jovix     (1000)      610 2019-07-04 02:18:38.000000 py3afipws-0.8/PKG-INFO
-drwxr-xr-x   0 jovix     (1000) jovix     (1000)        0 2019-07-04 02:18:38.000000 py3afipws-0.8/py3afipws/
--rw-r--r--   0 jovix     (1000) jovix     (1000)      684 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/__init__.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    10635 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/cot.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    11723 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/iibb.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    10989 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/nsis.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    19163 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/padron.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)     1279 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/php.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    48164 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/pyafipws.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)     9744 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/pyemail.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)     7242 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/pyi25.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    46225 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/pyrece.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    10487 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/pyrece.rsrc.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)     9041 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/rece.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    29268 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/rece1.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    12825 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/receb.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    12916 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/receb1.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    25194 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/recem.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    15541 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/recex.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    19480 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/recex1.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    35892 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/sired.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)     9357 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/soap.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    21880 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/trazafito.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    40414 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/trazamed.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    14237 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/trazarenpre.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    22106 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/trazavet.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    36597 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/utils.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)     6589 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/wdigdepfiel.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    14200 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/ws_sr_padron.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    20316 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/wsaa.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    20235 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/wsbfe.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    24867 2019-07-04 01:22:54.000000 py3afipws-0.8/py3afipws/wsbfev1.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    16450 2019-07-04 01:56:34.000000 py3afipws-0.8/py3afipws/wscdc.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    43069 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/wscoc.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    52287 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/wsctgv3.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)     7221 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/wsfe.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    66278 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/wsfev1.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    29525 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/wsfex.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    34532 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/wsfexv1.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    39331 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/wsltv.py
--rw-r--r--   0 jovix     (1000) jovix     (1000)    57880 2019-04-17 02:34:34.000000 py3afipws-0.8/py3afipws/wsmtx.py
-drwxr-xr-x   0 jovix     (1000) jovix     (1000)        0 2019-07-04 02:18:38.000000 py3afipws-0.8/py3afipws.egg-info/
--rw-r--r--   0 jovix     (1000) jovix     (1000)      610 2019-07-04 02:18:38.000000 py3afipws-0.8/py3afipws.egg-info/PKG-INFO
--rw-r--r--   0 jovix     (1000) jovix     (1000)      935 2019-07-04 02:18:38.000000 py3afipws-0.8/py3afipws.egg-info/SOURCES.txt
--rw-r--r--   0 jovix     (1000) jovix     (1000)        1 2019-07-04 02:18:38.000000 py3afipws-0.8/py3afipws.egg-info/dependency_links.txt
--rw-r--r--   0 jovix     (1000) jovix     (1000)       10 2019-07-04 02:18:38.000000 py3afipws-0.8/py3afipws.egg-info/top_level.txt
--rw-r--r--   0 jovix     (1000) jovix     (1000)      108 2019-07-04 02:18:38.000000 py3afipws-0.8/setup.cfg
--rw-r--r--   0 jovix     (1000) jovix     (1000)      819 2019-07-04 02:16:30.000000 py3afipws-0.8/setup.py
+drwxr-xr-x   0 jovix     (1000) jovix     (1000)        0 2019-07-04 03:03:46.000000 py3afipws-0.9/
+-rw-r--r--   0 jovix     (1000) jovix     (1000)      610 2019-07-04 03:03:46.000000 py3afipws-0.9/PKG-INFO
+drwxr-xr-x   0 jovix     (1000) jovix     (1000)        0 2019-07-04 03:03:46.000000 py3afipws-0.9/py3afipws/
+-rw-r--r--   0 jovix     (1000) jovix     (1000)      707 2019-07-04 02:59:03.000000 py3afipws-0.9/py3afipws/__init__.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    10659 2019-07-04 02:59:20.000000 py3afipws-0.9/py3afipws/cot.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    11747 2019-07-04 02:59:24.000000 py3afipws-0.9/py3afipws/iibb.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    11013 2019-07-04 02:59:29.000000 py3afipws-0.9/py3afipws/nsis.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    19185 2019-07-04 02:59:38.000000 py3afipws-0.9/py3afipws/padron.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)     1303 2019-07-04 02:59:45.000000 py3afipws-0.9/py3afipws/php.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    48188 2019-07-04 02:59:49.000000 py3afipws-0.9/py3afipws/pyafipws.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)     9768 2019-07-04 02:59:54.000000 py3afipws-0.9/py3afipws/pyemail.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)     7266 2019-07-04 02:59:57.000000 py3afipws-0.9/py3afipws/pyi25.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    46249 2019-07-04 03:00:00.000000 py3afipws-0.9/py3afipws/pyrece.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    10534 2019-07-04 03:00:12.000000 py3afipws-0.9/py3afipws/pyrece.rsrc.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)     9065 2019-07-04 03:00:18.000000 py3afipws-0.9/py3afipws/rece.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    29292 2019-07-04 03:00:21.000000 py3afipws-0.9/py3afipws/rece1.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    12849 2019-07-04 03:00:25.000000 py3afipws-0.9/py3afipws/receb.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    12940 2019-07-04 03:00:28.000000 py3afipws-0.9/py3afipws/receb1.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    25218 2019-07-04 03:00:32.000000 py3afipws-0.9/py3afipws/recem.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    15565 2019-07-04 03:00:36.000000 py3afipws-0.9/py3afipws/recex.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    19504 2019-07-04 03:00:40.000000 py3afipws-0.9/py3afipws/recex1.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    35916 2019-07-04 03:00:45.000000 py3afipws-0.9/py3afipws/sired.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)     9381 2019-07-04 03:00:49.000000 py3afipws-0.9/py3afipws/soap.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    21904 2019-07-04 03:00:52.000000 py3afipws-0.9/py3afipws/trazafito.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    40438 2019-07-04 03:00:55.000000 py3afipws-0.9/py3afipws/trazamed.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    14261 2019-07-04 03:00:58.000000 py3afipws-0.9/py3afipws/trazarenpre.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    22130 2019-07-04 03:01:03.000000 py3afipws-0.9/py3afipws/trazavet.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    36621 2019-07-04 03:01:11.000000 py3afipws-0.9/py3afipws/utils.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)     6613 2019-07-04 03:01:16.000000 py3afipws-0.9/py3afipws/wdigdepfiel.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    14224 2019-07-04 03:01:20.000000 py3afipws-0.9/py3afipws/ws_sr_padron.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    20340 2019-07-04 03:01:22.000000 py3afipws-0.9/py3afipws/wsaa.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    20259 2019-07-04 03:01:26.000000 py3afipws-0.9/py3afipws/wsbfe.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    24891 2019-07-04 03:01:29.000000 py3afipws-0.9/py3afipws/wsbfev1.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    16474 2019-07-04 03:01:38.000000 py3afipws-0.9/py3afipws/wscdc.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    43093 2019-07-04 03:01:42.000000 py3afipws-0.9/py3afipws/wscoc.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    52311 2019-07-04 03:01:46.000000 py3afipws-0.9/py3afipws/wsctgv3.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)     7245 2019-07-04 03:01:49.000000 py3afipws-0.9/py3afipws/wsfe.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    66302 2019-07-04 03:01:56.000000 py3afipws-0.9/py3afipws/wsfev1.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    29549 2019-07-04 03:01:59.000000 py3afipws-0.9/py3afipws/wsfex.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    34556 2019-07-04 03:02:03.000000 py3afipws-0.9/py3afipws/wsfexv1.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    39355 2019-07-04 03:02:05.000000 py3afipws-0.9/py3afipws/wsltv.py
+-rw-r--r--   0 jovix     (1000) jovix     (1000)    57904 2019-07-04 03:02:09.000000 py3afipws-0.9/py3afipws/wsmtx.py
+drwxr-xr-x   0 jovix     (1000) jovix     (1000)        0 2019-07-04 03:03:46.000000 py3afipws-0.9/py3afipws.egg-info/
+-rw-r--r--   0 jovix     (1000) jovix     (1000)      610 2019-07-04 03:03:46.000000 py3afipws-0.9/py3afipws.egg-info/PKG-INFO
+-rw-r--r--   0 jovix     (1000) jovix     (1000)      935 2019-07-04 03:03:46.000000 py3afipws-0.9/py3afipws.egg-info/SOURCES.txt
+-rw-r--r--   0 jovix     (1000) jovix     (1000)        1 2019-07-04 03:03:46.000000 py3afipws-0.9/py3afipws.egg-info/dependency_links.txt
+-rw-r--r--   0 jovix     (1000) jovix     (1000)       10 2019-07-04 03:03:46.000000 py3afipws-0.9/py3afipws.egg-info/top_level.txt
+-rw-r--r--   0 jovix     (1000) jovix     (1000)      108 2019-07-04 03:03:46.000000 py3afipws-0.9/setup.cfg
+-rw-r--r--   0 jovix     (1000) jovix     (1000)      819 2019-07-04 03:03:15.000000 py3afipws-0.9/setup.py
```

### Comparing `py3afipws-0.8/PKG-INFO` & `py3afipws-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: py3afipws
-Version: 0.8
+Version: 0.9
 Summary: pyafipws for python3
 Home-page: https://github.com/odoo-mastercore/pyafipws
 Author: Mastercore
 Author-email: far@mastercore.net
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: py3afipws,py3
```

### Comparing `py3afipws-0.8/py3afipws/__init__.py` & `py3afipws-0.9/py3afipws/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
 # or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License
 # for more details.
 
-"""Módulo para acceder a web services de la afip
-"""
+"""Módulo para acceder a web services de la afip"""
 __author__ = "Mariano Reingart (mariano@gmail.com)"
 __copyright__ = "Copyright (C) 2008-2015 Mariano Reingart"
 __license__ = "GPL 3.0"
```

### Comparing `py3afipws-0.8/py3afipws/cot.py` & `py3afipws-0.9/py3afipws/cot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/iibb.py` & `py3afipws-0.9/py3afipws/iibb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/nsis.py` & `py3afipws-0.9/py3afipws/nsis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
```

### Comparing `py3afipws-0.8/py3afipws/padron.py` & `py3afipws-0.9/py3afipws/padron.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
 # or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License
 # for more details.
 
 "Herramienta para procesar y consultar el Padrón Unico de Contribuyentes AFIP"
 
-# Documentación e información adicional: 
+# Documentación e información adicional:
 #    http://www.sistemasagiles.com.ar/trac/wiki/PadronContribuyentesAFIP
 
 __author__ = "Mariano Reingart <reingart@gmail.com>"
 __copyright__ = "Copyright (C) 2014 Mariano Reingart"
 __license__ = "GPL 3.0"
 __version__ = "1.05b"
 
@@ -86,15 +87,15 @@
     _public_methods_ = ['Buscar', 'Descargar', 'Procesar', 'Guardar',
                         'ConsultarDomicilios', 'Consultar', 'Conectar',
                         'DescargarConstancia', 'MostrarPDF',
                         'ObtenerTablaParametros',
                         ]
     _public_attrs_ = ['InstallDir', 'Traceback', 'Excepcion', 'Version',
                       'cuit', 'dni', 'denominacion', 'imp_ganancias',
-                      'imp_iva', 'monotributo', 'integrante_soc', 'empleador', 
+                      'imp_iva', 'monotributo', 'integrante_soc', 'empleador',
                       'actividad_monotributo', 'cat_iva', 'domicilios',
                       'tipo_doc', 'nro_doc', 'LanzarExcepciones',
                       'tipo_persona', 'estado', 'impuestos', 'actividades',
                       'direccion', 'localidad', 'provincia', 'cod_postal',
                       'data', 'response']
     _readonly_attrs_ = _public_attrs_[3:-1]
     _reg_progid_ = "PadronAFIP"
```

### Comparing `py3afipws-0.8/py3afipws/php.py` & `py3afipws-0.9/py3afipws/php.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/pyafipws.py` & `py3afipws-0.9/py3afipws/pyafipws.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/pyemail.py` & `py3afipws-0.9/py3afipws/pyemail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/pyi25.py` & `py3afipws-0.9/py3afipws/pyi25.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/pyrece.py` & `py3afipws-0.9/py3afipws/pyrece.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/pyrece.rsrc.py` & `py3afipws-0.9/py3afipws/pyrece.rsrc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
 [{'components': [{'components': [{'items': [{'label': u'Abrir',
                                              'name': 'abrir',
                                              'type': 'MenuItem'},
                                             {'label': u'ReCargar',
                                              'name': 'cargar',
                                              'type': 'MenuItem'},
                                             {'label': u'Guardar',
```

### Comparing `py3afipws-0.8/py3afipws/rece.py` & `py3afipws-0.9/py3afipws/rece.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/rece1.py` & `py3afipws-0.9/py3afipws/rece1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/receb.py` & `py3afipws-0.9/py3afipws/receb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/receb1.py` & `py3afipws-0.9/py3afipws/receb1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/recem.py` & `py3afipws-0.9/py3afipws/recem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/recex.py` & `py3afipws-0.9/py3afipws/recex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/recex1.py` & `py3afipws-0.9/py3afipws/recex1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/sired.py` & `py3afipws-0.9/py3afipws/sired.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/soap.py` & `py3afipws-0.9/py3afipws/soap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/trazafito.py` & `py3afipws-0.9/py3afipws/trazafito.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,1368 +1,1369 @@
 00000000: 2321 2f75 7372 2f62 696e 2f70 7974 686f  #!/usr/bin/pytho
-00000010: 6e0a 2320 5468 6973 2070 726f 6772 616d  n.# This program
-00000020: 2069 7320 6672 6565 2073 6f66 7477 6172   is free softwar
-00000030: 653b 2079 6f75 2063 616e 2072 6564 6973  e; you can redis
-00000040: 7472 6962 7574 6520 6974 2061 6e64 2f6f  tribute it and/o
-00000050: 7220 6d6f 6469 6679 0a23 2069 7420 756e  r modify.# it un
-00000060: 6465 7220 7468 6520 7465 726d 7320 6f66  der the terms of
-00000070: 2074 6865 2047 4e55 2047 656e 6572 616c   the GNU General
-00000080: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
-00000090: 6173 2070 7562 6c69 7368 6564 2062 7920  as published by 
-000000a0: 7468 650a 2320 4672 6565 2053 6f66 7477  the.# Free Softw
-000000b0: 6172 6520 466f 756e 6461 7469 6f6e 3b20  are Foundation; 
-000000c0: 6569 7468 6572 2076 6572 7369 6f6e 2033  either version 3
-000000d0: 2c20 6f72 2028 6174 2079 6f75 7220 6f70  , or (at your op
-000000e0: 7469 6f6e 2920 616e 7920 6c61 7465 720a  tion) any later.
-000000f0: 2320 7665 7273 696f 6e2e 0a23 0a23 2054  # version..#.# T
-00000100: 6869 7320 7072 6f67 7261 6d20 6973 2064  his program is d
-00000110: 6973 7472 6962 7574 6564 2069 6e20 7468  istributed in th
-00000120: 6520 686f 7065 2074 6861 7420 6974 2077  e hope that it w
-00000130: 696c 6c20 6265 2075 7365 6675 6c2c 2062  ill be useful, b
-00000140: 7574 0a23 2057 4954 484f 5554 2041 4e59  ut.# WITHOUT ANY
-00000150: 2057 4152 5241 4e54 593b 2077 6974 686f   WARRANTY; witho
-00000160: 7574 2065 7665 6e20 7468 6520 696d 706c  ut even the impl
-00000170: 6965 6420 7761 7272 616e 7479 206f 6620  ied warranty of 
-00000180: 4d45 5243 4841 4e54 4942 494c 4954 590a  MERCHANTIBILITY.
-00000190: 2320 6f72 2046 4954 4e45 5353 2046 4f52  # or FITNESS FOR
-000001a0: 2041 2050 4152 5449 4355 4c41 5220 5055   A PARTICULAR PU
-000001b0: 5250 4f53 452e 2020 5365 6520 7468 6520  RPOSE.  See the 
-000001c0: 474e 5520 4765 6e65 7261 6c20 5075 626c  GNU General Publ
-000001d0: 6963 204c 6963 656e 7365 0a23 2066 6f72  ic License.# for
-000001e0: 206d 6f72 6520 6465 7461 696c 732e 0a0a   more details...
-000001f0: 224d f364 756c 6f20 5472 617a 6162 696c  "M.dulo Trazabil
-00000200: 6964 6164 2064 6520 5072 6f64 7563 746f  idad de Producto
-00000210: 7320 4669 746f 7361 6e69 7461 7269 6f73  s Fitosanitarios
-00000220: 2053 454e 4153 4120 5265 736f 6c75 6369   SENASA Resoluci
-00000230: f36e 2033 3639 2f32 3031 3322 0a0a 2320  .n 369/2013"..# 
-00000240: 496e 666f 726d 6163 69f3 6e20 6164 6963  Informaci.n adic
-00000250: 696f 6e61 6c20 7920 646f 6375 6d65 6e74  ional y document
-00000260: 6163 69f3 6e3a 0a23 2068 7474 703a 2f2f  aci.n:.# http://
-00000270: 7777 772e 7369 7374 656d 6173 6167 696c  www.sistemasagil
-00000280: 6573 2e63 6f6d 2e61 722f 7472 6163 2f77  es.com.ar/trac/w
-00000290: 696b 692f 5472 617a 6162 696c 6964 6164  iki/Trazabilidad
-000002a0: 5072 6f64 7563 746f 7346 6974 6f73 616e  ProductosFitosan
-000002b0: 6974 6172 696f 730a 0a5f 5f61 7574 686f  itarios..__autho
-000002c0: 725f 5f20 3d20 224d 6172 6961 6e6f 2052  r__ = "Mariano R
-000002d0: 6569 6e67 6172 7420 3c72 6569 6e67 6172  eingart <reingar
-000002e0: 7440 676d 6169 6c2e 636f 6d3e 220a 5f5f  t@gmail.com>".__
-000002f0: 636f 7079 7269 6768 745f 5f20 3d20 2243  copyright__ = "C
-00000300: 6f70 7972 6967 6874 2028 4329 2032 3031  opyright (C) 201
-00000310: 3420 4d61 7269 616e 6f20 5265 696e 6761  4 Mariano Reinga
-00000320: 7274 220a 5f5f 6c69 6365 6e73 655f 5f20  rt".__license__ 
-00000330: 3d20 2247 504c 2033 2e30 2b22 0a5f 5f76  = "GPL 3.0+".__v
-00000340: 6572 7369 6f6e 5f5f 203d 2022 312e 3131  ersion__ = "1.11
-00000350: 6422 0a0a 2320 6874 7470 3a2f 2f73 656e  d"..# http://sen
-00000360: 6173 612e 7365 7276 6963 696f 732e 7061  asa.servicios.pa
-00000370: 6d69 2e6f 7267 2e61 722f 0a0a 696d 706f  mi.org.ar/..impo
-00000380: 7274 206f 730a 696d 706f 7274 2073 6f63  rt os.import soc
-00000390: 6b65 740a 696d 706f 7274 2073 7973 0a69  ket.import sys.i
-000003a0: 6d70 6f72 7420 6461 7465 7469 6d65 2c20  mport datetime, 
-000003b0: 7469 6d65 0a69 6d70 6f72 7420 7472 6163  time.import trac
-000003c0: 6562 6163 6b0a 696d 706f 7274 2070 7933  eback.import py3
-000003d0: 7369 6d70 6c65 736f 6170 2e63 6c69 656e  simplesoap.clien
-000003e0: 740a 6672 6f6d 2070 7933 7369 6d70 6c65  t.from py3simple
-000003f0: 736f 6170 2e63 6c69 656e 7420 696d 706f  soap.client impo
-00000400: 7274 2053 6f61 7043 6c69 656e 742c 2053  rt SoapClient, S
-00000410: 6f61 7046 6175 6c74 2c20 7061 7273 655f  oapFault, parse_
-00000420: 7072 6f78 792c 205c 0a20 2020 2020 2020  proxy, \.       
-00000430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000440: 2020 2020 2020 2020 2073 6574 5f68 7474           set_htt
-00000450: 705f 7772 6170 7065 720a 6672 6f6d 2070  p_wrapper.from p
-00000460: 7933 7369 6d70 6c65 736f 6170 2e73 696d  y3simplesoap.sim
-00000470: 706c 6578 6d6c 2069 6d70 6f72 7420 5369  plexml import Si
-00000480: 6d70 6c65 584d 4c45 6c65 6d65 6e74 0a66  mpleXMLElement.f
-00000490: 726f 6d20 6353 7472 696e 6749 4f20 696d  rom cStringIO im
-000004a0: 706f 7274 2053 7472 696e 6749 4f0a 0a23  port StringIO..#
-000004b0: 2069 6d70 6f72 746f 2066 756e 6369 6f6e   importo funcion
-000004c0: 6573 2063 6f6d 7061 7274 6964 6173 3a0a  es compartidas:.
-000004d0: 6672 6f6d 202e 7574 696c 7320 696d 706f  from .utils impo
-000004e0: 7274 206c 6565 722c 2065 7363 7269 6269  rt leer, escribi
-000004f0: 722c 206c 6565 725f 6462 662c 2067 7561  r, leer_dbf, gua
-00000500: 7264 6172 5f64 6266 2c20 4e2c 2041 2c20  rdar_dbf, N, A, 
-00000510: 492c 206a 736f 6e2c 205c 0a20 2020 2020  I, json, \.     
-00000520: 2020 2020 2020 2020 2020 2020 2064 6172               dar
-00000530: 5f6e 6f6d 6272 655f 6361 6d70 6f5f 6462  _nombre_campo_db
-00000540: 662c 2067 6574 5f69 6e73 7461 6c6c 5f64  f, get_install_d
-00000550: 6972 2c20 4261 7365 5753 2c20 5c0a 2020  ir, BaseWS, \.  
-00000560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000570: 696e 6963 6961 6c69 7a61 725f 795f 6361  inicializar_y_ca
-00000580: 7074 7572 6172 5f65 7863 6570 6369 6f6e  pturar_excepcion
-00000590: 6573 0a0a 484f 4d4f 203d 2046 616c 7365  es..HOMO = False
-000005a0: 0a54 5950 454c 4942 203d 2046 616c 7365  .TYPELIB = False
-000005b0: 0a0a 5753 444c 203d 2022 6874 7470 733a  ..WSDL = "https:
-000005c0: 2f2f 7365 7276 6963 696f 732e 7061 6d69  //servicios.pami
-000005d0: 2e6f 7267 2e61 722f 7472 617a 6165 6e61  .org.ar/trazaena
-000005e0: 6772 2e57 6562 5365 7276 6963 653f 7773  gr.WebService?ws
-000005f0: 646c 220a 4c4f 4341 5449 4f4e 203d 2022  dl".LOCATION = "
-00000600: 6874 7470 733a 2f2f 7365 7276 6963 696f  https://servicio
-00000610: 732e 7061 6d69 2e6f 7267 2e61 722f 7472  s.pami.org.ar/tr
-00000620: 617a 6165 6e61 6772 2e57 6562 5365 7276  azaenagr.WebServ
-00000630: 6963 6522 0a0a 2320 466f 726d 6174 6f20  ice"..# Formato 
-00000640: 6465 2054 7261 6e73 6163 6369 6f6e 5365  de TransaccionSe
-00000650: 6e61 7361 4454 4f20 2853 6176 6554 7261  nasaDTO (SaveTra
-00000660: 6e73 6163 6369 6f6e 290a 5452 414e 5341  nsaccion).TRANSA
-00000670: 4343 494f 4e5f 4454 4f20 3d20 5b0a 2020  CCION_DTO = [.  
-00000680: 2020 2827 676c 6e5f 6f72 6967 656e 272c    ('gln_origen',
-00000690: 2031 332c 2041 292c 0a20 2020 2028 2767   13, A),.    ('g
-000006a0: 6c6e 5f64 6573 7469 6e6f 272c 2031 332c  ln_destino', 13,
-000006b0: 2041 292c 0a20 2020 2028 2766 5f6f 7065   A),.    ('f_ope
-000006c0: 7261 6369 6f6e 272c 2031 302c 2041 292c  racion', 10, A),
-000006d0: 0a20 2020 2028 2766 5f65 6c61 626f 7261  .    ('f_elabora
-000006e0: 6369 6f6e 272c 2031 302c 2041 292c 0a20  cion', 10, A),. 
-000006f0: 2020 2028 2766 5f76 746f 272c 2031 302c     ('f_vto', 10,
-00000700: 2041 292c 0a20 2020 2028 2769 645f 6576   A),.    ('id_ev
-00000710: 656e 746f 272c 2031 352c 204e 292c 0a20  ento', 15, N),. 
-00000720: 2020 2028 2763 6f64 5f70 726f 6475 6374     ('cod_product
-00000730: 6f27 2c20 3134 2c20 4129 2c0a 2020 2020  o', 14, A),.    
-00000740: 2827 6e5f 6361 6e74 6964 6164 272c 2033  ('n_cantidad', 3
-00000750: 302c 204e 292c 0a20 2020 2028 276e 5f73  0, N),.    ('n_s
-00000760: 6572 6965 272c 2032 302c 2041 292c 0a20  erie', 20, A),. 
-00000770: 2020 2028 276e 5f6c 6f74 6527 2c20 3530     ('n_lote', 50
-00000780: 2c20 4129 2c0a 2020 2020 2827 6e5f 6361  , A),.    ('n_ca
-00000790: 6927 2c20 3135 2c20 4129 2c0a 2020 2020  i', 15, A),.    
-000007a0: 2827 6e5f 6361 6527 2c20 3135 2c20 4129  ('n_cae', 15, A)
-000007b0: 2c0a 2020 2020 2827 6964 5f6d 6f74 6976  ,.    ('id_motiv
-000007c0: 6f5f 6465 7374 7275 6363 696f 6e27 2c20  o_destruccion', 
-000007d0: 352c 2041 292c 0a20 2020 2028 276e 5f6d  5, A),.    ('n_m
-000007e0: 616e 6966 6965 7374 6f27 2c20 3135 2c20  anifiesto', 15, 
-000007f0: 4e29 2c0a 2020 2020 2827 656e 5f74 7261  N),.    ('en_tra
-00000800: 6e73 706f 7274 6527 2c20 312c 2041 292c  nsporte', 1, A),
-00000810: 2023 2062 6f6f 6c65 616e 0a20 2020 2028   # boolean.    (
-00000820: 276e 5f72 656d 6974 6f27 2c20 3135 2c20  'n_remito', 15, 
-00000830: 4129 2c0a 2020 2020 2827 6d6f 7469 766f  A),.    ('motivo
-00000840: 5f64 6576 6f6c 7563 696f 6e27 2c20 3130  _devolucion', 10
-00000850: 302c 2041 292c 0a20 2020 2028 276f 6273  0, A),.    ('obs
-00000860: 6572 7661 6369 6f6e 6573 272c 2031 3030  ervaciones', 100
-00000870: 302c 2041 292c 0a20 2020 2028 276e 5f76  0, A),.    ('n_v
-00000880: 616c 655f 636f 6d70 7261 272c 2031 352c  ale_compra', 15,
-00000890: 2041 292c 0a20 2020 2028 2761 7065 6c6c   A),.    ('apell
-000008a0: 6964 6f4e 6f6d 6272 6573 272c 2032 3535  idoNombres', 255
-000008b0: 2c20 4129 2c0a 2020 2020 2827 6469 7265  , A),.    ('dire
-000008c0: 6363 696f 6e27 2c20 3230 302c 2041 292c  ccion', 200, A),
-000008d0: 0a20 2020 2028 276e 756d 6572 6f27 2c20  .    ('numero', 
-000008e0: 362c 204e 292c 0a20 2020 2028 276c 6f63  6, N),.    ('loc
-000008f0: 616c 6964 6164 272c 2031 352c 2041 292c  alidad', 15, A),
-00000900: 0a20 2020 2028 2770 726f 7669 6e63 6961  .    ('provincia
-00000910: 272c 2031 352c 2041 292c 0a20 2020 2028  ', 15, A),.    (
-00000920: 276e 5f70 6f73 7461 6c27 2c20 382c 2041  'n_postal', 8, A
-00000930: 292c 0a20 2020 2028 2763 7569 7427 2c20  ),.    ('cuit', 
-00000940: 3131 2c20 4129 2c0a 2020 2020 2827 636f  11, A),.    ('co
-00000950: 6469 676f 5f74 7261 6e73 6163 6369 6f6e  digo_transaccion
-00000960: 272c 2031 342c 2041 292c 0a5d 0a0a 2320  ', 14, A),.]..# 
-00000970: 466f 726d 6174 6f20 7061 7261 2054 7261  Formato para Tra
-00000980: 6e73 6163 6369 6f6e 5365 6e61 7361 2028  nsaccionSenasa (
-00000990: 6765 7454 7261 6e73 6163 6369 6f6e 6573  getTransacciones
-000009a0: 290a 5452 414e 5341 4343 494f 4e45 5320  ).TRANSACCIONES 
-000009b0: 3d20 5b0a 2020 2020 2827 6964 5f74 7261  = [.    ('id_tra
-000009c0: 6e73 6163 6369 6f6e 5f67 6c6f 6261 6c27  nsaccion_global'
-000009d0: 2c20 3135 2c20 4e29 2c0a 2020 2020 2827  , 15, N),.    ('
-000009e0: 6964 5f74 7261 6e73 6163 6369 6f6e 272c  id_transaccion',
-000009f0: 2031 352c 204e 292c 0a20 2020 2028 2766   15, N),.    ('f
-00000a00: 5f74 7261 6e73 6163 6369 6f6e 272c 2031  _transaccion', 1
-00000a10: 302c 2041 292c 0a20 2020 2028 2766 5f6f  0, A),.    ('f_o
-00000a20: 7065 7261 6369 6f6e 272c 2031 302c 2041  peracion', 10, A
-00000a30: 292c 0a20 2020 2028 2766 5f76 656e 6369  ),.    ('f_venci
-00000a40: 6d69 656e 746f 272c 2031 302c 2041 292c  miento', 10, A),
-00000a50: 0a20 2020 2028 2766 5f65 6c61 626f 7261  .    ('f_elabora
-00000a60: 6369 6f6e 272c 2031 302c 2041 292c 0a20  cion', 10, A),. 
-00000a70: 2020 2028 2764 5f65 7665 6e74 6f27 2c20     ('d_evento', 
-00000a80: 3130 302c 2041 292c 0a20 2020 2028 2763  100, A),.    ('c
-00000a90: 616e 7469 6461 6427 2c20 3330 2c20 4e29  antidad', 30, N)
-00000aa0: 2c0a 2020 2020 2827 6964 5f75 6e69 6461  ,.    ('id_unida
-00000ab0: 6427 2c20 3135 2c20 4e29 2c0a 2020 2020  d', 15, N),.    
-00000ac0: 2827 645f 756e 6964 6164 272c 2031 3030  ('d_unidad', 100
-00000ad0: 2c20 4129 2c0a 2020 2020 2827 636f 645f  , A),.    ('cod_
-00000ae0: 7072 6f64 7563 746f 272c 2031 342c 2041  producto', 14, A
-00000af0: 292c 0a20 2020 2028 2769 645f 756e 6964  ),.    ('id_unid
-00000b00: 6164 272c 2031 352c 204e 292c 0a20 2020  ad', 15, N),.   
-00000b10: 2028 276e 5f73 6572 6965 272c 2032 302c   ('n_serie', 20,
-00000b20: 2041 292c 0a20 2020 2028 276e 5f6c 6f74   A),.    ('n_lot
-00000b30: 6527 2c20 3530 2c20 4129 2c0a 2020 2020  e', 50, A),.    
-00000b40: 2827 6e5f 6361 6927 2c20 3135 2c20 4129  ('n_cai', 15, A)
-00000b50: 2c0a 2020 2020 2827 6e5f 6361 6527 2c20  ,.    ('n_cae', 
-00000b60: 3135 2c20 4129 2c0a 2020 2020 2827 645f  15, A),.    ('d_
-00000b70: 6d6f 7469 766f 5f64 6573 7472 7563 6369  motivo_destrucci
-00000b80: 6f6e 272c 2035 302c 2041 292c 0a20 2020  on', 50, A),.   
-00000b90: 2028 2764 5f6d 616e 6966 6965 7374 6f27   ('d_manifiesto'
-00000ba0: 2c20 3135 2c20 4129 2c0a 2020 2020 2827  , 15, A),.    ('
-00000bb0: 656e 5f74 7261 6e73 706f 7274 6527 2c20  en_transporte', 
-00000bc0: 312c 2041 292c 0a20 2020 2028 276e 5f72  1, A),.    ('n_r
-00000bd0: 656d 6974 6f27 2c20 3330 2c20 4129 2c0a  emito', 30, A),.
-00000be0: 2020 2020 2827 6d6f 7469 766f 5f64 6576      ('motivo_dev
-00000bf0: 6f6c 7563 696f 6e27 2c20 3230 302c 2041  olucion', 200, A
-00000c00: 292c 0a20 2020 2028 276f 6273 6572 7661  ),.    ('observa
-00000c10: 6369 6f6e 6573 272c 2031 3030 302c 2041  ciones', 1000, A
-00000c20: 292c 0a20 2020 2028 276e 5f76 616c 655f  ),.    ('n_vale_
-00000c30: 636f 6d70 7261 272c 2031 352c 2041 292c  compra', 15, A),
-00000c40: 0a20 2020 2028 2761 7065 6c6c 6964 6f4e  .    ('apellidoN
-00000c50: 6f6d 6272 6573 272c 2032 3535 2c20 4129  ombres', 255, A)
-00000c60: 2c0a 2020 2020 2827 6469 7265 6363 696f  ,.    ('direccio
-00000c70: 6e27 2c20 3230 302c 2041 292c 0a20 2020  n', 200, A),.   
-00000c80: 2028 276e 756d 6572 6f27 2c20 362c 2041   ('numero', 6, A
-00000c90: 292c 0a20 2020 2028 276c 6f63 616c 6964  ),.    ('localid
-00000ca0: 6164 272c 2032 3530 2c20 4129 2c0a 2020  ad', 250, A),.  
-00000cb0: 2020 2827 7072 6f76 696e 6369 6127 2c20    ('provincia', 
-00000cc0: 3235 302c 2041 292c 0a20 2020 2028 276e  250, A),.    ('n
-00000cd0: 5f70 6f73 7461 6c27 2c20 382c 2041 292c  _postal', 8, A),
-00000ce0: 0a20 2020 2028 2763 7569 7427 2c20 3131  .    ('cuit', 11
-00000cf0: 2c20 4129 2c0a 2020 2020 2827 645f 6167  , A),.    ('d_ag
-00000d00: 656e 7465 5f69 6e66 6f72 6d61 646f 7227  ente_informador'
-00000d10: 2c20 3235 352c 2041 292c 0a20 2020 2028  , 255, A),.    (
-00000d20: 2764 5f61 6765 6e74 655f 6f72 6967 656e  'd_agente_origen
-00000d30: 272c 2032 3535 2c20 4129 2c0a 2020 2020  ', 255, A),.    
-00000d40: 2827 645f 6167 656e 7465 5f64 6573 7469  ('d_agente_desti
-00000d50: 6e6f 272c 2032 3535 2c20 4129 2c0a 2020  no', 255, A),.  
-00000d60: 2020 2827 645f 7072 6f64 7563 746f 272c    ('d_producto',
-00000d70: 2032 3530 2c20 4129 2c0a 2020 2020 2827   250, A),.    ('
-00000d80: 645f 6573 7461 646f 5f74 7261 6e73 6163  d_estado_transac
-00000d90: 6369 6f6e 272c 2033 302c 2041 292c 0a20  cion', 30, A),. 
-00000da0: 2020 2028 2764 5f74 6970 6f5f 7472 616e     ('d_tipo_tran
-00000db0: 7361 6363 696f 6e27 2c20 3330 2c20 4129  saccion', 30, A)
-00000dc0: 2c0a 5d0a 0a23 2046 6f72 6d61 746f 2070  ,.]..# Formato p
-00000dd0: 6172 6120 4572 726f 7265 730a 4552 524f  ara Errores.ERRO
-00000de0: 5245 5320 3d20 5b0a 2020 2020 2827 5f63  RES = [.    ('_c
-00000df0: 5f65 7272 6f72 272c 2034 2c20 4129 2c20  _error', 4, A), 
-00000e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e10: 2320 63f3 6469 676f 0a20 2020 2028 275f  # c.digo.    ('_
-00000e20: 645f 6572 726f 7227 2c20 3235 302c 2041  d_error', 250, A
-00000e30: 292c 2020 2020 2020 2020 2020 2020 2020  ),              
-00000e40: 2023 2064 6573 6372 6970 6369 f36e 0a20   # descripci.n. 
-00000e50: 2020 205d 0a0a 0a63 6c61 7373 2054 7261     ]...class Tra
-00000e60: 7a61 4669 746f 2842 6173 6557 5329 3a0a  zaFito(BaseWS):.
-00000e70: 2020 2020 2249 6e74 6572 6661 7a20 7061      "Interfaz pa
-00000e80: 7261 2065 6c20 5765 6253 6572 7669 6365  ra el WebService
-00000e90: 2064 6520 5472 617a 6162 696c 6964 6164   de Trazabilidad
-00000ea0: 2064 6520 4669 746f 7361 6e69 7461 7269   de Fitosanitari
-00000eb0: 6f73 2053 454e 4153 4122 0a0a 2020 2020  os SENASA"..    
-00000ec0: 5f70 7562 6c69 635f 6d65 7468 6f64 735f  _public_methods_
-00000ed0: 203d 205b 2753 6176 6554 7261 6e73 6163   = ['SaveTransac
-00000ee0: 6369 6f6e 272c 2027 5365 6e64 4361 6e63  cion', 'SendCanc
-00000ef0: 656c 6154 7261 6e73 6163 272c 0a20 2020  elaTransac',.   
-00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f10: 2020 2020 2027 5365 6e64 436f 6e66 6972       'SendConfir
-00000f20: 6d61 5472 616e 7361 6363 272c 2027 5365  maTransacc', 'Se
-00000f30: 6e64 416c 6572 7461 5472 616e 7361 6363  ndAlertaTransacc
-00000f40: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00000f50: 2020 2020 2020 2020 2020 2027 4765 7454             'GetT
-00000f60: 7261 6e73 6163 6369 6f6e 6573 272c 0a20  ransacciones',. 
-00000f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f80: 2020 2020 2020 2027 436f 6e65 6374 6172         'Conectar
-00000f90: 272c 2027 4c65 6572 4572 726f 7227 2c20  ', 'LeerError', 
-00000fa0: 274c 6565 7254 7261 6e73 6163 6369 6f6e  'LeerTransaccion
-00000fb0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00000fc0: 2020 2020 2020 2020 2020 2027 5365 7455             'SetU
-00000fd0: 7365 726e 616d 6527 2c0a 2020 2020 2020  sername',.      
-00000fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ff0: 2020 2753 6574 5061 7261 6d65 7472 6f27    'SetParametro'
-00001000: 2c20 2747 6574 5061 7261 6d65 7472 6f27  , 'GetParametro'
-00001010: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001020: 2020 2020 2020 2020 2020 2747 6574 436f            'GetCo
-00001030: 6469 676f 5472 616e 7361 6363 696f 6e27  digoTransaccion'
-00001040: 2c20 2747 6574 5265 7375 6c74 6164 6f27  , 'GetResultado'
-00001050: 2c20 274c 6f61 6454 6573 7458 4d4c 275d  , 'LoadTestXML']
-00001060: 0a0a 2020 2020 5f70 7562 6c69 635f 6174  ..    _public_at
-00001070: 7472 735f 203d 205b 0a20 2020 2020 2020  trs_ = [.       
-00001080: 2027 5573 6572 6e61 6d65 272c 2027 5061   'Username', 'Pa
-00001090: 7373 776f 7264 272c 0a20 2020 2020 2020  ssword',.       
-000010a0: 2027 436f 6469 676f 5472 616e 7361 6363   'CodigoTransacc
-000010b0: 696f 6e27 2c20 2745 7272 6f72 6573 272c  ion', 'Errores',
-000010c0: 2027 5265 7375 6c74 6164 6f27 2c0a 2020   'Resultado',.  
-000010d0: 2020 2020 2020 2758 6d6c 5265 7175 6573        'XmlReques
-000010e0: 7427 2c20 2758 6d6c 5265 7370 6f6e 7365  t', 'XmlResponse
-000010f0: 272c 0a20 2020 2020 2020 2027 5665 7273  ',.        'Vers
-00001100: 696f 6e27 2c20 2749 6e73 7461 6c6c 4469  ion', 'InstallDi
-00001110: 7227 2c0a 2020 2020 2020 2020 2754 7261  r',.        'Tra
-00001120: 6365 6261 636b 272c 2027 4578 6365 7063  ceback', 'Excepc
-00001130: 696f 6e27 2c20 274c 616e 7a61 7245 7863  ion', 'LanzarExc
-00001140: 6570 6369 6f6e 6573 272c 0a20 2020 2020  epciones',.     
-00001150: 2020 2027 4361 6e74 5061 6769 6e61 7327     'CantPaginas'
-00001160: 2c20 2748 6179 4572 726f 7227 2c20 2754  , 'HayError', 'T
-00001170: 7261 6e73 6163 6369 6f6e 5365 6e61 7361  ransaccionSenasa
-00001180: 272c 0a20 2020 2020 2020 205d 0a0a 2020  ',.        ]..  
-00001190: 2020 5f72 6567 5f70 726f 6769 645f 203d    _reg_progid_ =
-000011a0: 2022 5472 617a 6146 6974 6f22 0a20 2020   "TrazaFito".   
-000011b0: 205f 7265 675f 636c 7369 645f 203d 2022   _reg_clsid_ = "
-000011c0: 7b33 3937 3933 3933 312d 3435 3041 2d34  {39793931-450A-4
-000011d0: 4636 362d 3933 3234 2d44 3444 3938 3146  F66-9324-D4D981F
-000011e0: 4335 3331 397d 220a 0a20 2020 2023 2056  C5319}"..    # V
-000011f0: 6172 6961 626c 6573 2067 6c6f 6261 6c65  ariables globale
-00001200: 7320 7061 7261 2042 6173 6557 533a 0a20  s para BaseWS:. 
-00001210: 2020 2048 4f4d 4f20 3d20 484f 4d4f 0a20     HOMO = HOMO. 
-00001220: 2020 2057 5344 4c20 3d20 5753 444c 0a20     WSDL = WSDL. 
-00001230: 2020 2056 6572 7369 6f6e 203d 2022 2573     Version = "%s
-00001240: 2025 7320 2573 2220 2520 285f 5f76 6572   %s %s" % (__ver
-00001250: 7369 6f6e 5f5f 2c20 484f 4d4f 2061 6e64  sion__, HOMO and
-00001260: 2027 486f 6d6f 6c6f 6761 6369 f36e 2720   'Homologaci.n' 
-00001270: 6f72 2027 272c 0a20 2020 2020 2020 2020  or '',.         
-00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001290: 2020 2070 7933 7369 6d70 6c65 736f 6170     py3simplesoap
-000012a0: 2e63 6c69 656e 742e 5f5f 7665 7273 696f  .client.__versio
-000012b0: 6e5f 5f29 0a0a 2020 2020 6465 6620 5f5f  n__)..    def __
-000012c0: 696e 6974 5f5f 2873 656c 662c 2072 6569  init__(self, rei
-000012d0: 6e74 656e 746f 733d 3129 3a0a 2020 2020  ntentos=1):.    
-000012e0: 2020 2020 7365 6c66 2e55 7365 726e 616d      self.Usernam
-000012f0: 6520 3d20 7365 6c66 2e50 6173 7377 6f72  e = self.Passwor
-00001300: 6420 3d20 4e6f 6e65 0a20 2020 2020 2020  d = None.       
-00001310: 2073 656c 662e 5472 616e 7361 6363 696f   self.Transaccio
-00001320: 6e53 656e 6173 6120 3d20 5b5d 0a20 2020  nSenasa = [].   
-00001330: 2020 2020 2042 6173 6557 532e 5f5f 696e       BaseWS.__in
-00001340: 6974 5f5f 2873 656c 662c 2072 6569 6e74  it__(self, reint
-00001350: 656e 746f 7329 0a0a 2020 2020 6465 6620  entos)..    def 
-00001360: 696e 6963 6961 6c69 7a61 7228 7365 6c66  inicializar(self
-00001370: 293a 0a20 2020 2020 2020 2042 6173 6557  ):.        BaseW
-00001380: 532e 696e 6963 6961 6c69 7a61 7228 7365  S.inicializar(se
-00001390: 6c66 290a 2020 2020 2020 2020 7365 6c66  lf).        self
-000013a0: 2e43 6f64 6967 6f54 7261 6e73 6163 6369  .CodigoTransacci
-000013b0: 6f6e 203d 2073 656c 662e 4572 726f 7265  on = self.Errore
-000013c0: 7320 3d20 7365 6c66 2e52 6573 756c 7461  s = self.Resulta
-000013d0: 646f 203d 204e 6f6e 650a 2020 2020 2020  do = None.      
-000013e0: 2020 7365 6c66 2e52 6573 756c 7461 646f    self.Resultado
-000013f0: 203d 2027 270a 2020 2020 2020 2020 7365   = ''.        se
-00001400: 6c66 2e45 7272 6f72 6573 203d 205b 5d20  lf.Errores = [] 
-00001410: 2020 2320 6c69 7374 6120 6465 2073 7472    # lista de str
-00001420: 696e 6773 2070 6172 6120 6c61 2069 6e74  ings para la int
-00001430: 6572 6661 7a0a 2020 2020 2020 2020 7365  erfaz.        se
-00001440: 6c66 2e65 7272 6f72 6573 203d 205b 5d20  lf.errores = [] 
-00001450: 2020 2320 6c69 7374 6120 6465 2064 6963    # lista de dic
-00001460: 6369 6f6e 6172 696f 7320 2875 736f 2069  cionarios (uso i
-00001470: 6e74 6572 6e6f 290a 2020 2020 2020 2020  nterno).        
-00001480: 7365 6c66 2e43 616e 7450 6167 696e 6173  self.CantPaginas
-00001490: 203d 2073 656c 662e 4861 7945 7272 6f72   = self.HayError
-000014a0: 203d 204e 6f6e 650a 0a20 2020 2064 6566   = None..    def
-000014b0: 205f 5f61 6e61 6c69 7a61 725f 6572 726f   __analizar_erro
-000014c0: 7265 7328 7365 6c66 2c20 7265 7429 3a0a  res(self, ret):.
-000014d0: 2020 2020 2020 2020 2243 6f6d 7072 7565          "Comprue
-000014e0: 6261 2079 2065 7874 7261 6520 6572 726f  ba y extrae erro
-000014f0: 7265 7320 7369 2065 7869 7374 656e 2065  res si existen e
-00001500: 6e20 6c61 2072 6573 7075 6573 7461 2058  n la respuesta X
-00001510: 4d4c 220a 2020 2020 2020 2020 7365 6c66  ML".        self
-00001520: 2e65 7272 6f72 6573 203d 2072 6574 2e67  .errores = ret.g
-00001530: 6574 2827 6572 726f 7265 7327 2c20 5b5d  et('errores', []
-00001540: 290a 2020 2020 2020 2020 7365 6c66 2e45  ).        self.E
-00001550: 7272 6f72 6573 203d 205b 2225 733a 2025  rrores = ["%s: %
-00001560: 7322 2025 2028 6974 5b27 635f 6572 726f  s" % (it['c_erro
-00001570: 7227 5d2c 2069 745b 2764 5f65 7272 6f72  r'], it['d_error
-00001580: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
-00001590: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000015a0: 6974 2069 6e20 7265 742e 6765 7428 2765  it in ret.get('e
-000015b0: 7272 6f72 6573 272c 205b 5d29 5d0a 2020  rrores', [])].  
-000015c0: 2020 2020 2020 7365 6c66 2e52 6573 756c        self.Resul
-000015d0: 7461 646f 203d 2072 6574 2e67 6574 2827  tado = ret.get('
-000015e0: 7265 7375 6c74 6164 6f27 290a 0a20 2020  resultado')..   
-000015f0: 2064 6566 2043 6f6e 6563 7461 7228 7365   def Conectar(se
-00001600: 6c66 2c20 6361 6368 653d 4e6f 6e65 2c20  lf, cache=None, 
-00001610: 7773 646c 3d4e 6f6e 652c 2070 726f 7879  wsdl=None, proxy
-00001620: 3d22 222c 2077 7261 7070 6572 3d4e 6f6e  ="", wrapper=Non
-00001630: 652c 2063 6163 6572 743d 4e6f 6e65 2c20  e, cacert=None, 
-00001640: 7469 6d65 6f75 743d 3330 293a 0a20 2020  timeout=30):.   
-00001650: 2020 2020 2023 2043 6f6e 6563 746f 2075       # Conecto u
-00001660: 7361 6e64 6f20 656c 206d e974 6f64 6f20  sando el m.todo 
-00001670: 6573 7461 6e64 6172 643a 0a20 2020 2020  estandard:.     
-00001680: 2020 206f 6b20 3d20 4261 7365 5753 2e43     ok = BaseWS.C
-00001690: 6f6e 6563 7461 7228 7365 6c66 2c20 6361  onectar(self, ca
-000016a0: 6368 652c 2077 7364 6c2c 2070 726f 7879  che, wsdl, proxy
-000016b0: 2c20 7772 6170 7065 722c 2063 6163 6572  , wrapper, cacer
-000016c0: 742c 2074 696d 656f 7574 2c0a 2020 2020  t, timeout,.    
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 2020 2020 2020 2020 2020 736f 6170 5f73            soap_s
-000016f0: 6572 7665 723d 226a 6574 7479 2229 0a20  erver="jetty"). 
-00001700: 2020 2020 2020 2069 6620 6f6b 3a0a 2020         if ok:.  
-00001710: 2020 2020 2020 2020 2020 2320 7369 2065            # si e
-00001720: 6c20 6172 6368 6976 6f20 6573 206c 6f63  l archivo es loc
-00001730: 616c 2c20 6173 756d 6f20 7175 6520 7961  al, asumo que ya
-00001740: 2065 7374 6120 636f 7272 6567 6964 6f3a   esta corregido:
-00001750: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00001760: 6e6f 7420 7365 6c66 2e77 7364 6c2e 7374  not self.wsdl.st
-00001770: 6172 7473 7769 7468 2822 6669 6c65 2229  artswith("file")
-00001780: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001790: 2020 2320 636f 7272 696a 6f20 7562 6963    # corrijo ubic
-000017a0: 6163 69f3 6e20 6465 6c20 7365 7276 6964  aci.n del servid
-000017b0: 6f72 2028 6c6f 6361 6c68 6f73 743a 3930  or (localhost:90
-000017c0: 3530 2065 6e20 656c 2057 5344 4c29 0a20  50 en el WSDL). 
-000017d0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000017e0: 6f63 6174 696f 6e20 3d20 7365 6c66 2e77  ocation = self.w
-000017f0: 7364 6c5b 3a2d 355d 0a20 2020 2020 2020  sdl[:-5].       
-00001800: 2020 2020 2020 2020 2077 7320 3d20 7365           ws = se
-00001810: 6c66 2e63 6c69 656e 742e 7365 7276 6963  lf.client.servic
-00001820: 6573 5b27 4957 6562 5365 7276 6963 6553  es['IWebServiceS
-00001830: 656e 6173 6127 5d0a 2020 2020 2020 2020  enasa'].        
-00001840: 2020 2020 2020 2020 7773 5b27 706f 7274          ws['port
-00001850: 7327 5d5b 2749 5765 6253 6572 7669 6365  s']['IWebService
-00001860: 5365 6e61 7361 506f 7274 275d 5b27 6c6f  SenasaPort']['lo
-00001870: 6361 7469 6f6e 275d 203d 206c 6f63 6174  cation'] = locat
-00001880: 696f 6e0a 0a20 2020 2020 2020 2020 2020  ion..           
-00001890: 2023 2045 7374 6162 6c65 6365 7220 6372   # Establecer cr
-000018a0: 6564 656e 6369 616c 6573 2064 6520 7365  edenciales de se
-000018b0: 6775 7269 6461 643a 0a20 2020 2020 2020  guridad:.       
-000018c0: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
-000018d0: 5b27 7773 7365 3a53 6563 7572 6974 7927  ['wsse:Security'
-000018e0: 5d20 3d20 7b0a 2020 2020 2020 2020 2020  ] = {.          
-000018f0: 2020 2020 2020 2777 7373 653a 5573 6572        'wsse:User
-00001900: 6e61 6d65 546f 6b65 6e27 3a20 7b0a 2020  nameToken': {.  
-00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001920: 2020 2777 7373 653a 5573 6572 6e61 6d65    'wsse:Username
-00001930: 273a 2073 656c 662e 5573 6572 6e61 6d65  ': self.Username
-00001940: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001950: 2020 2020 2020 2777 7373 653a 5061 7373        'wsse:Pass
-00001960: 776f 7264 273a 2073 656c 662e 5061 7373  word': self.Pass
-00001970: 776f 7264 2c0a 2020 2020 2020 2020 2020  word,.          
-00001980: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00001990: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-000019a0: 2020 2020 2020 7265 7475 726e 206f 6b0a        return ok.
-000019b0: 0a20 2020 2040 696e 6963 6961 6c69 7a61  .    @inicializa
-000019c0: 725f 795f 6361 7074 7572 6172 5f65 7863  r_y_capturar_exc
-000019d0: 6570 6369 6f6e 6573 0a20 2020 2064 6566  epciones.    def
-000019e0: 2053 6176 6554 7261 6e73 6163 6369 6f6e   SaveTransaccion
-000019f0: 2873 656c 662c 2075 7375 6172 696f 2c20  (self, usuario, 
-00001a00: 7061 7373 776f 7264 2c0a 2020 2020 2020  password,.      
-00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a20: 2020 676c 6e5f 6f72 6967 656e 3d4e 6f6e    gln_origen=Non
-00001a30: 652c 2067 6c6e 5f64 6573 7469 6e6f 3d4e  e, gln_destino=N
-00001a40: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00001a50: 2020 2020 2020 2020 2020 2020 2066 5f6f               f_o
-00001a60: 7065 7261 6369 6f6e 3d4e 6f6e 652c 2066  peracion=None, f
-00001a70: 5f65 6c61 626f 7261 6369 6f6e 3d4e 6f6e  _elaboracion=Non
-00001a80: 652c 2066 5f76 746f 3d4e 6f6e 652c 0a20  e, f_vto=None,. 
-00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001aa0: 2020 2020 2020 2069 645f 6576 656e 746f         id_evento
-00001ab0: 3d4e 6f6e 652c 2063 6f64 5f70 726f 6475  =None, cod_produ
-00001ac0: 6374 6f3d 4e6f 6e65 2c20 6e5f 6361 6e74  cto=None, n_cant
-00001ad0: 6964 6164 3d4e 6f6e 652c 0a20 2020 2020  idad=None,.     
-00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001af0: 2020 206e 5f73 6572 6965 3d4e 6f6e 652c     n_serie=None,
-00001b00: 206e 5f6c 6f74 653d 4e6f 6e65 2c20 6e5f   n_lote=None, n_
-00001b10: 6361 693d 4e6f 6e65 2c20 6e5f 6361 653d  cai=None, n_cae=
-00001b20: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00001b30: 2020 2020 2020 2020 2020 2020 2020 6964                id
-00001b40: 5f6d 6f74 6976 6f5f 6465 7374 7275 6363  _motivo_destrucc
-00001b50: 696f 6e3d 4e6f 6e65 2c20 6e5f 6d61 6e69  ion=None, n_mani
-00001b60: 6669 6573 746f 3d4e 6f6e 652c 0a20 2020  fiesto=None,.   
-00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b80: 2020 2020 2065 6e5f 7472 616e 7370 6f72       en_transpor
-00001b90: 7465 3d4e 6f6e 652c 206e 5f72 656d 6974  te=None, n_remit
-00001ba0: 6f3d 4e6f 6e65 2c0a 2020 2020 2020 2020  o=None,.        
-00001bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bc0: 6d6f 7469 766f 5f64 6576 6f6c 7563 696f  motivo_devolucio
-00001bd0: 6e3d 4e6f 6e65 2c20 6f62 7365 7276 6163  n=None, observac
-00001be0: 696f 6e65 733d 4e6f 6e65 2c0a 2020 2020  iones=None,.    
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c00: 2020 2020 6e5f 7661 6c65 5f63 6f6d 7072      n_vale_compr
-00001c10: 613d 4e6f 6e65 2c20 6170 656c 6c69 646f  a=None, apellido
-00001c20: 4e6f 6d62 7265 733d 4e6f 6e65 2c0a 2020  Nombres=None,.  
-00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c40: 2020 2020 2020 6469 7265 6363 696f 6e3d        direccion=
-00001c50: 4e6f 6e65 2c20 6e75 6d65 726f 3d4e 6f6e  None, numero=Non
-00001c60: 652c 206c 6f63 616c 6964 6164 3d4e 6f6e  e, localidad=Non
-00001c70: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00001c80: 2020 2020 2020 2020 2020 2070 726f 7669             provi
-00001c90: 6e63 6961 3d4e 6f6e 652c 206e 5f70 6f73  ncia=None, n_pos
-00001ca0: 7461 6c3d 4e6f 6e65 2c20 6375 6974 3d4e  tal=None, cuit=N
-00001cb0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-00001cc0: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
-00001cd0: 2020 2020 2020 2020 2252 6561 6c69 7a61          "Realiza
-00001ce0: 2065 6c20 7265 6769 7374 726f 2064 6520   el registro de 
-00001cf0: 756e 6120 7472 616e 7361 6363 69f3 6e20  una transacci.n 
-00001d00: 6465 2070 726f 6475 6374 6f73 2066 6974  de productos fit
-00001d10: 6f73 616e 6974 6172 696f 732e 2022 0a20  osanitarios. ". 
-00001d20: 2020 2020 2020 2023 2063 7265 6f20 6c6f         # creo lo
-00001d30: 7320 7061 72e1 6d65 7472 6f73 2070 6172  s par.metros par
-00001d40: 6120 6573 7461 206c 6c61 6d61 6461 0a20  a esta llamada. 
-00001d50: 2020 2020 2020 2070 6172 616d 7320 3d20         params = 
-00001d60: 7b20 2027 676c 6e5f 6f72 6967 656e 273a  {  'gln_origen':
-00001d70: 2067 6c6e 5f6f 7269 6765 6e2c 0a20 2020   gln_origen,.   
-00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d90: 2027 676c 6e5f 6465 7374 696e 6f27 3a20   'gln_destino': 
-00001da0: 676c 6e5f 6465 7374 696e 6f2c 0a20 2020  gln_destino,.   
-00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001dc0: 2027 665f 6f70 6572 6163 696f 6e27 3a20   'f_operacion': 
-00001dd0: 665f 6f70 6572 6163 696f 6e2c 0a20 2020  f_operacion,.   
-00001de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001df0: 2027 665f 656c 6162 6f72 6163 696f 6e27   'f_elaboracion'
-00001e00: 3a20 665f 656c 6162 6f72 6163 696f 6e2c  : f_elaboracion,
-00001e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001e20: 2020 2020 2027 665f 7674 6f27 3a20 665f       'f_vto': f_
-00001e30: 7674 6f2c 0a20 2020 2020 2020 2020 2020  vto,.           
-00001e40: 2020 2020 2020 2020 2027 6964 5f65 7665           'id_eve
-00001e50: 6e74 6f27 3a20 6964 5f65 7665 6e74 6f2c  nto': id_evento,
-00001e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001e70: 2020 2020 2027 636f 645f 7072 6f64 7563       'cod_produc
-00001e80: 746f 273a 2063 6f64 5f70 726f 6475 6374  to': cod_product
-00001e90: 6f2c 0a20 2020 2020 2020 2020 2020 2020  o,.             
-00001ea0: 2020 2020 2020 2027 6e5f 6361 6e74 6964         'n_cantid
-00001eb0: 6164 273a 206e 5f63 616e 7469 6461 642c  ad': n_cantidad,
-00001ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ed0: 2020 2020 2027 6e5f 7365 7269 6527 3a20       'n_serie': 
-00001ee0: 6e5f 7365 7269 652c 0a20 2020 2020 2020  n_serie,.       
-00001ef0: 2020 2020 2020 2020 2020 2020 2027 6e5f               'n_
-00001f00: 6c6f 7465 273a 206e 5f6c 6f74 652c 0a20  lote': n_lote,. 
-00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f20: 2020 2027 6e5f 6361 6927 3a20 6e5f 6361     'n_cai': n_ca
-00001f30: 6920 6f72 204e 6f6e 652c 0a20 2020 2020  i or None,.     
-00001f40: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001f50: 6e5f 6361 6527 3a20 6e5f 6361 6520 6f72  n_cae': n_cae or
-00001f60: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00001f70: 2020 2020 2020 2020 2020 2027 6964 5f6d             'id_m
-00001f80: 6f74 6976 6f5f 6465 7374 7275 6363 696f  otivo_destruccio
-00001f90: 6e27 3a20 6964 5f6d 6f74 6976 6f5f 6465  n': id_motivo_de
-00001fa0: 7374 7275 6363 696f 6e20 6f72 204e 6f6e  struccion or Non
-00001fb0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00001fc0: 2020 2020 2020 2027 6e5f 6d61 6e69 6669         'n_manifi
-00001fd0: 6573 746f 273a 206e 5f6d 616e 6966 6965  esto': n_manifie
-00001fe0: 7374 6f20 6f72 204e 6f6e 652c 0a20 2020  sto or None,.   
-00001ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002000: 2027 656e 5f74 7261 6e73 706f 7274 6527   'en_transporte'
-00002010: 3a20 656e 5f74 7261 6e73 706f 7274 6520  : en_transporte 
-00002020: 6f72 204e 6f6e 652c 0a20 2020 2020 2020  or None,.       
-00002030: 2020 2020 2020 2020 2020 2020 2027 6e5f               'n_
-00002040: 7265 6d69 746f 273a 206e 5f72 656d 6974  remito': n_remit
-00002050: 6f20 6f72 204e 6f6e 652c 0a20 2020 2020  o or None,.     
-00002060: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00002070: 6d6f 7469 766f 5f64 6576 6f6c 7563 696f  motivo_devolucio
-00002080: 6e27 3a20 6d6f 7469 766f 5f64 6576 6f6c  n': motivo_devol
-00002090: 7563 696f 6e20 6f72 204e 6f6e 652c 0a20  ucion or None,. 
-000020a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020b0: 2020 2027 6f62 7365 7276 6163 696f 6e65     'observacione
-000020c0: 7327 3a20 6f62 7365 7276 6163 696f 6e65  s': observacione
-000020d0: 7320 6f72 204e 6f6e 652c 0a20 2020 2020  s or None,.     
-000020e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000020f0: 6e5f 7661 6c65 5f63 6f6d 7072 6127 3a20  n_vale_compra': 
-00002100: 6e5f 7661 6c65 5f63 6f6d 7072 6120 6f72  n_vale_compra or
-00002110: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00002120: 2020 2020 2020 2020 2020 2027 6170 656c             'apel
-00002130: 6c69 646f 4e6f 6d62 7265 7327 3a20 6170  lidoNombres': ap
-00002140: 656c 6c69 646f 4e6f 6d62 7265 7320 6f72  ellidoNombres or
-00002150: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00002160: 2020 2020 2020 2020 2020 2027 6469 7265             'dire
-00002170: 6363 696f 6e27 3a20 6469 7265 6363 696f  ccion': direccio
-00002180: 6e20 6f72 204e 6f6e 652c 0a20 2020 2020  n or None,.     
-00002190: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000021a0: 6e75 6d65 726f 273a 206e 756d 6572 6f20  numero': numero 
-000021b0: 6f72 204e 6f6e 652c 0a20 2020 2020 2020  or None,.       
-000021c0: 2020 2020 2020 2020 2020 2020 2027 6c6f               'lo
-000021d0: 6361 6c69 6461 6427 3a20 6c6f 6361 6c69  calidad': locali
-000021e0: 6461 6420 6f72 204e 6f6e 652c 0a20 2020  dad or None,.   
-000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002200: 2027 7072 6f76 696e 6369 6127 3a20 7072   'provincia': pr
-00002210: 6f76 696e 6369 6120 6f72 204e 6f6e 652c  ovincia or None,
-00002220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002230: 2020 2020 2027 6e5f 706f 7374 616c 273a       'n_postal':
-00002240: 206e 5f70 6f73 7461 6c20 6f72 204e 6f6e   n_postal or Non
-00002250: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00002260: 2020 2020 2020 2027 6375 6974 273a 2063         'cuit': c
-00002270: 7569 7420 6f72 204e 6f6e 652c 0a20 2020  uit or None,.   
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 207d 0a20 2020 2020 2020 2072 6573 203d   }.        res =
-000022a0: 2073 656c 662e 636c 6965 6e74 2e73 6176   self.client.sav
-000022b0: 6554 7261 6e73 6163 6369 6f6e 6573 280a  eTransacciones(.
-000022c0: 2020 2020 2020 2020 2020 2020 6172 6730              arg0
-000022d0: 3d70 6172 616d 732c 0a20 2020 2020 2020  =params,.       
-000022e0: 2020 2020 2061 7267 313d 7573 7561 7269       arg1=usuari
-000022f0: 6f2c 0a20 2020 2020 2020 2020 2020 2061  o,.            a
-00002300: 7267 323d 7061 7373 776f 7264 2c0a 2020  rg2=password,.  
-00002310: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00002320: 7265 7420 3d20 7265 735b 2772 6574 7572  ret = res['retur
-00002330: 6e27 5d0a 2020 2020 2020 2020 7365 6c66  n'].        self
-00002340: 2e43 6f64 6967 6f54 7261 6e73 6163 6369  .CodigoTransacci
-00002350: 6f6e 203d 2072 6574 2e67 6574 2827 636f  on = ret.get('co
-00002360: 6469 676f 5472 616e 7361 6363 696f 6e27  digoTransaccion'
-00002370: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-00002380: 5f61 6e61 6c69 7a61 725f 6572 726f 7265  _analizar_errore
-00002390: 7328 7265 7429 0a20 2020 2020 2020 2072  s(ret).        r
-000023a0: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
-000023b0: 4069 6e69 6369 616c 697a 6172 5f79 5f63  @inicializar_y_c
-000023c0: 6170 7475 7261 725f 6578 6365 7063 696f  apturar_excepcio
-000023d0: 6e65 730a 2020 2020 6465 6620 5365 6e64  nes.    def Send
-000023e0: 4361 6e63 656c 6154 7261 6e73 6163 2873  CancelaTransac(s
-000023f0: 656c 662c 2075 7375 6172 696f 2c20 7061  elf, usuario, pa
-00002400: 7373 776f 7264 2c20 636f 6469 676f 5f74  ssword, codigo_t
-00002410: 7261 6e73 6163 6369 6f6e 293a 0a20 2020  ransaccion):.   
-00002420: 2020 2020 2022 2052 6561 6c69 7a61 206c       " Realiza l
-00002430: 6120 6361 6e63 656c 6163 69f3 6e20 6465  a cancelaci.n de
-00002440: 2075 6e61 2074 7261 6e73 6163 6369 f36e   una transacci.n
-00002450: 220a 2020 2020 2020 2020 7265 7320 3d20  ".        res = 
-00002460: 7365 6c66 2e63 6c69 656e 742e 7365 6e64  self.client.send
-00002470: 4361 6e63 656c 6154 7261 6e73 6163 280a  CancelaTransac(.
-00002480: 2020 2020 2020 2020 2020 2020 6172 6730              arg0
-00002490: 3d63 6f64 6967 6f5f 7472 616e 7361 6363  =codigo_transacc
-000024a0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-000024b0: 2061 7267 313d 7573 7561 7269 6f2c 0a20   arg1=usuario,. 
-000024c0: 2020 2020 2020 2020 2020 2061 7267 323d             arg2=
-000024d0: 7061 7373 776f 7264 2c0a 2020 2020 2020  password,.      
-000024e0: 2020 290a 2020 2020 2020 2020 7265 7420    ).        ret 
-000024f0: 3d20 7265 735b 2772 6574 7572 6e27 5d0a  = res['return'].
-00002500: 2020 2020 2020 2020 7365 6c66 2e43 6f64          self.Cod
-00002510: 6967 6f54 7261 6e73 6163 6369 6f6e 203d  igoTransaccion =
-00002520: 2072 6574 2e67 6574 2827 636f 6469 676f   ret.get('codigo
-00002530: 5472 616e 7361 6363 696f 6e27 290a 2020  Transaccion').  
-00002540: 2020 2020 2020 7365 6c66 2e5f 5f61 6e61        self.__ana
-00002550: 6c69 7a61 725f 6572 726f 7265 7328 7265  lizar_errores(re
-00002560: 7429 0a20 2020 2020 2020 2072 6574 7572  t).        retur
-00002570: 6e20 5472 7565 0a0a 2020 2020 4069 6e69  n True..    @ini
-00002580: 6369 616c 697a 6172 5f79 5f63 6170 7475  cializar_y_captu
-00002590: 7261 725f 6578 6365 7063 696f 6e65 730a  rar_excepciones.
-000025a0: 2020 2020 6465 6620 5365 6e64 436f 6e66      def SendConf
-000025b0: 6972 6d61 5472 616e 7361 6363 2873 656c  irmaTransacc(sel
-000025c0: 662c 2075 7375 6172 696f 2c20 7061 7373  f, usuario, pass
-000025d0: 776f 7264 2c20 705f 6964 735f 7472 616e  word, p_ids_tran
-000025e0: 7361 632c 2066 5f6f 7065 7261 6369 6f6e  sac, f_operacion
-000025f0: 2c20 6e5f 6361 6e74 6964 6164 3d4e 6f6e  , n_cantidad=Non
-00002600: 6529 3a0a 2020 2020 2020 2020 2243 6f6e  e):.        "Con
-00002610: 6669 726d 6120 6c61 2072 6563 6570 6369  firma la recepci
-00002620: f36e 2064 6520 756e 206d 6564 6963 616d  .n de un medicam
-00002630: 656e 746f 220a 2020 2020 2020 2020 7265  ento".        re
-00002640: 7320 3d20 7365 6c66 2e63 6c69 656e 742e  s = self.client.
-00002650: 7365 6e64 436f 6e66 6972 6d61 5472 616e  sendConfirmaTran
-00002660: 7361 6363 280a 2020 2020 2020 2020 2020  sacc(.          
-00002670: 2020 6172 6730 3d75 7375 6172 696f 2c0a    arg0=usuario,.
-00002680: 2020 2020 2020 2020 2020 2020 6172 6731              arg1
-00002690: 3d70 6173 7377 6f72 642c 0a20 2020 2020  =password,.     
-000026a0: 2020 2020 2020 2061 7267 323d 7b27 705f         arg2={'p_
-000026b0: 6964 735f 7472 616e 7361 6327 3a20 705f  ids_transac': p_
-000026c0: 6964 735f 7472 616e 7361 632c 2027 665f  ids_transac, 'f_
-000026d0: 6f70 6572 6163 696f 6e27 3a20 665f 6f70  operacion': f_op
-000026e0: 6572 6163 696f 6e2c 0a20 2020 2020 2020  eracion,.       
-000026f0: 2020 2020 2020 2020 2020 2027 6e5f 6361             'n_ca
-00002700: 6e74 6964 6164 273a 206e 5f63 616e 7469  ntidad': n_canti
-00002710: 6461 642c 0a20 2020 2020 2020 2020 2020  dad,.           
-00002720: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00002730: 2029 0a20 2020 2020 2020 2072 6574 203d   ).        ret =
-00002740: 2072 6573 5b27 7265 7475 726e 275d 0a20   res['return']. 
-00002750: 2020 2020 2020 2073 656c 662e 436f 6469         self.Codi
-00002760: 676f 5472 616e 7361 6363 696f 6e20 3d20  goTransaccion = 
-00002770: 7265 742e 6765 7428 2763 6f64 6967 6f54  ret.get('codigoT
-00002780: 7261 6e73 6163 6369 6f6e 2729 0a20 2020  ransaccion').   
-00002790: 2020 2020 2073 656c 662e 5f5f 616e 616c       self.__anal
-000027a0: 697a 6172 5f65 7272 6f72 6573 2872 6574  izar_errores(ret
-000027b0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000027c0: 2054 7275 650a 0a20 2020 2040 696e 6963   True..    @inic
-000027d0: 6961 6c69 7a61 725f 795f 6361 7074 7572  ializar_y_captur
-000027e0: 6172 5f65 7863 6570 6369 6f6e 6573 0a20  ar_excepciones. 
-000027f0: 2020 2064 6566 2053 656e 6441 6c65 7274     def SendAlert
-00002800: 6154 7261 6e73 6163 6328 7365 6c66 2c20  aTransacc(self, 
-00002810: 7573 7561 7269 6f2c 2070 6173 7377 6f72  usuario, passwor
-00002820: 642c 2070 5f69 6473 5f74 7261 6e73 6163  d, p_ids_transac
-00002830: 5f77 7329 3a0a 2020 2020 2020 2020 2241  _ws):.        "A
-00002840: 6c65 7274 6120 756e 206d 6564 6963 616d  lerta un medicam
-00002850: 656e 746f 2c20 6163 6369 f36e 2063 6f6e  ento, acci.n con
-00002860: 7472 6172 6961 2061 2093 636f 6e66 6972  traria a .confir
-00002870: 6d61 7220 6c61 2074 7261 6e73 6163 6369  mar la transacci
-00002880: f36e 942e 220a 2020 2020 2020 2020 7265  .n..".        re
-00002890: 7320 3d20 7365 6c66 2e63 6c69 656e 742e  s = self.client.
-000028a0: 7365 6e64 416c 6572 7461 5472 616e 7361  sendAlertaTransa
-000028b0: 6363 280a 2020 2020 2020 2020 2020 2020  cc(.            
-000028c0: 6172 6730 3d75 7375 6172 696f 2c0a 2020  arg0=usuario,.  
-000028d0: 2020 2020 2020 2020 2020 6172 6731 3d70            arg1=p
-000028e0: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
-000028f0: 2020 2020 2061 7267 323d 705f 6964 735f       arg2=p_ids_
-00002900: 7472 616e 7361 635f 7773 2c0a 2020 2020  transac_ws,.    
-00002910: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
-00002920: 7420 3d20 7265 735b 2772 6574 7572 6e27  t = res['return'
-00002930: 5d0a 2020 2020 2020 2020 7365 6c66 2e43  ].        self.C
-00002940: 6f64 6967 6f54 7261 6e73 6163 6369 6f6e  odigoTransaccion
-00002950: 203d 2072 6574 2e67 6574 2827 6964 5f74   = ret.get('id_t
-00002960: 7261 6e73 6163 5f61 736f 6369 6164 6127  ransac_asociada'
-00002970: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-00002980: 5f61 6e61 6c69 7a61 725f 6572 726f 7265  _analizar_errore
-00002990: 7328 7265 7429 0a20 2020 2020 2020 2072  s(ret).        r
-000029a0: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
-000029b0: 4069 6e69 6369 616c 697a 6172 5f79 5f63  @inicializar_y_c
-000029c0: 6170 7475 7261 725f 6578 6365 7063 696f  apturar_excepcio
-000029d0: 6e65 730a 2020 2020 6465 6620 4765 7454  nes.    def GetT
-000029e0: 7261 6e73 6163 6369 6f6e 6573 2873 656c  ransacciones(sel
-000029f0: 662c 2075 7375 6172 696f 2c20 7061 7373  f, usuario, pass
-00002a00: 776f 7264 2c0a 2020 2020 2020 2020 2020  word,.          
-00002a10: 2020 2020 2020 6964 5f74 7261 6e73 6163        id_transac
-00002a20: 6369 6f6e 3d4e 6f6e 652c 2069 645f 6576  cion=None, id_ev
-00002a30: 656e 746f 3d4e 6f6e 652c 2067 6c6e 5f6f  ento=None, gln_o
-00002a40: 7269 6765 6e3d 4e6f 6e65 2c0a 2020 2020  rigen=None,.    
-00002a50: 2020 2020 2020 2020 2020 2020 6665 6368              fech
-00002a60: 615f 6465 7364 655f 743d 4e6f 6e65 2c20  a_desde_t=None, 
-00002a70: 6665 6368 615f 6861 7374 615f 743d 4e6f  fecha_hasta_t=No
-00002a80: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00002a90: 2020 2020 6665 6368 615f 6465 7364 655f      fecha_desde_
-00002aa0: 763d 4e6f 6e65 2c20 6665 6368 615f 6861  v=None, fecha_ha
-00002ab0: 7374 615f 763d 4e6f 6e65 2c0a 2020 2020  sta_v=None,.    
-00002ac0: 2020 2020 2020 2020 2020 2020 676c 6e5f              gln_
-00002ad0: 696e 666f 726d 6164 6f72 3d4e 6f6e 652c  informador=None,
-00002ae0: 2069 645f 7469 706f 5f74 7261 6e73 6163   id_tipo_transac
-00002af0: 6369 6f6e 3d4e 6f6e 652c 0a20 2020 2020  cion=None,.     
-00002b00: 2020 2020 2020 2020 2020 2067 7469 6e5f             gtin_
-00002b10: 656c 656d 656e 746f 3d4e 6f6e 652c 206e  elemento=None, n
-00002b20: 5f6c 6f74 653d 4e6f 6e65 2c20 6e5f 7365  _lote=None, n_se
-00002b30: 7269 653d 4e6f 6e65 2c0a 2020 2020 2020  rie=None,.      
-00002b40: 2020 2020 2020 2020 2020 6e5f 7265 6d69            n_remi
-00002b50: 746f 5f66 6163 7475 7261 3d4e 6f6e 652c  to_factura=None,
-00002b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002b70: 2029 3a0a 2020 2020 2020 2020 2254 7261   ):.        "Tra
-00002b80: 6520 756e 206c 6973 7461 646f 2064 6520  e un listado de 
-00002b90: 6c61 7320 7472 616e 7361 6363 696f 6e65  las transaccione
-00002ba0: 7320 7175 6520 6e6f 2065 7374 e16e 2063  s que no est.n c
-00002bb0: 6f6e 6669 726d 6164 6173 220a 0a20 2020  onfirmadas"..   
-00002bc0: 2020 2020 2023 2070 7265 7061 726f 206c       # preparo l
-00002bd0: 6f73 2070 6172 616d 6574 726f 7320 6465  os parametros de
-00002be0: 2065 6e74 7261 6461 206f 7063 696f 6e61   entrada opciona
-00002bf0: 6c65 733a 0a20 2020 2020 2020 206b 7761  les:.        kwa
-00002c00: 7267 7320 3d20 7b7d 0a20 2020 2020 2020  rgs = {}.       
-00002c10: 2069 6620 6964 5f74 7261 6e73 6163 6369   if id_transacci
-00002c20: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
-00002c30: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-00002c40: 6773 5b27 6172 6732 275d 203d 2069 645f  gs['arg2'] = id_
-00002c50: 7472 616e 7361 6363 696f 6e0a 2020 2020  transaccion.    
-00002c60: 2020 2020 6966 2069 645f 6576 656e 746f      if id_evento
-00002c70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00002c80: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
-00002c90: 5b27 6172 6733 275d 203d 2069 645f 6576  ['arg3'] = id_ev
-00002ca0: 656e 746f 0a20 2020 2020 2020 2069 6620  ento.        if 
-00002cb0: 676c 6e5f 6f72 6967 656e 2069 7320 6e6f  gln_origen is no
-00002cc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00002cd0: 2020 2020 6b77 6172 6773 5b27 6172 6734      kwargs['arg4
-00002ce0: 275d 203d 2067 6c6e 5f6f 7269 6765 6e0a  '] = gln_origen.
-00002cf0: 2020 2020 2020 2020 6966 2066 6563 6861          if fecha
-00002d00: 5f64 6573 6465 5f74 2069 7320 6e6f 7420  _desde_t is not 
-00002d10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00002d20: 2020 6b77 6172 6773 5b27 6172 6735 275d    kwargs['arg5']
-00002d30: 203d 2066 6563 6861 5f64 6573 6465 5f74   = fecha_desde_t
-00002d40: 0a20 2020 2020 2020 2069 6620 6665 6368  .        if fech
-00002d50: 615f 6861 7374 615f 7420 6973 206e 6f74  a_hasta_t is not
-00002d60: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00002d70: 2020 206b 7761 7267 735b 2761 7267 3627     kwargs['arg6'
-00002d80: 5d20 3d20 6665 6368 615f 6861 7374 615f  ] = fecha_hasta_
-00002d90: 740a 2020 2020 2020 2020 6966 2066 6563  t.        if fec
-00002da0: 6861 5f64 6573 6465 5f76 2069 7320 6e6f  ha_desde_v is no
-00002db0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00002dc0: 2020 2020 6b77 6172 6773 5b27 6172 6737      kwargs['arg7
-00002dd0: 275d 203d 2066 6563 6861 5f64 6573 6465  '] = fecha_desde
-00002de0: 5f76 0a20 2020 2020 2020 2069 6620 6665  _v.        if fe
-00002df0: 6368 615f 6861 7374 615f 7620 6973 206e  cha_hasta_v is n
-00002e00: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00002e10: 2020 2020 206b 7761 7267 735b 2761 7267       kwargs['arg
-00002e20: 3827 5d20 3d20 6665 6368 615f 6861 7374  8'] = fecha_hast
-00002e30: 615f 760a 2020 2020 2020 2020 6966 2067  a_v.        if g
-00002e40: 6c6e 5f69 6e66 6f72 6d61 646f 7220 6973  ln_informador is
-00002e50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00002e60: 2020 2020 2020 206b 7761 7267 735b 2761         kwargs['a
-00002e70: 7267 3927 5d20 3d20 676c 6e5f 696e 666f  rg9'] = gln_info
-00002e80: 726d 6164 6f72 0a20 2020 2020 2020 2069  rmador.        i
-00002e90: 6620 6964 5f74 6970 6f5f 7472 616e 7361  f id_tipo_transa
-00002ea0: 6363 696f 6e20 6973 206e 6f74 204e 6f6e  ccion is not Non
-00002eb0: 653a 0a20 2020 2020 2020 2020 2020 206b  e:.            k
-00002ec0: 7761 7267 735b 2761 7267 3130 275d 203d  wargs['arg10'] =
-00002ed0: 2069 645f 7469 706f 5f74 7261 6e73 6163   id_tipo_transac
-00002ee0: 6369 6f6e 0a20 2020 2020 2020 2069 6620  cion.        if 
-00002ef0: 6774 696e 5f65 6c65 6d65 6e74 6f20 6973  gtin_elemento is
-00002f00: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00002f10: 2020 2020 2020 206b 7761 7267 735b 2761         kwargs['a
-00002f20: 7267 3131 275d 203d 2067 7469 6e5f 656c  rg11'] = gtin_el
-00002f30: 656d 656e 746f 0a20 2020 2020 2020 2069  emento.        i
-00002f40: 6620 6e5f 6c6f 7465 2069 7320 6e6f 7420  f n_lote is not 
-00002f50: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00002f60: 2020 6b77 6172 6773 5b27 6172 6731 3227    kwargs['arg12'
-00002f70: 5d20 3d20 6e5f 6c6f 7465 0a20 2020 2020  ] = n_lote.     
-00002f80: 2020 2069 6620 6e5f 7365 7269 6520 6973     if n_serie is
-00002f90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00002fa0: 2020 2020 2020 206b 7761 7267 735b 2761         kwargs['a
-00002fb0: 7267 3133 275d 203d 206e 5f73 6572 6965  rg13'] = n_serie
-00002fc0: 0a20 2020 2020 2020 2069 6620 6e5f 7265  .        if n_re
-00002fd0: 6d69 746f 5f66 6163 7475 7261 2069 7320  mito_factura is 
-00002fe0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00002ff0: 2020 2020 2020 6b77 6172 6773 5b27 6172        kwargs['ar
-00003000: 6731 3427 5d20 3d20 6e5f 7265 6d69 746f  g14'] = n_remito
-00003010: 5f66 6163 7475 7261 0a0a 2020 2020 2020  _factura..      
-00003020: 2020 2320 6c6c 616d 6f20 616c 2077 6562    # llamo al web
-00003030: 7365 7276 6963 650a 2020 2020 2020 2020  service.        
-00003040: 7265 7320 3d20 7365 6c66 2e63 6c69 656e  res = self.clien
-00003050: 742e 6765 7454 7261 6e73 6163 6369 6f6e  t.getTransaccion
-00003060: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
-00003070: 6172 6730 3d75 7375 6172 696f 2c0a 2020  arg0=usuario,.  
-00003080: 2020 2020 2020 2020 2020 6172 6731 3d70            arg1=p
-00003090: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
-000030a0: 2020 2020 202a 2a6b 7761 7267 730a 2020       **kwargs.  
-000030b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000030c0: 7265 7420 3d20 7265 735b 2772 6574 7572  ret = res['retur
-000030d0: 6e27 5d0a 2020 2020 2020 2020 6966 2072  n'].        if r
-000030e0: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
-000030f0: 7365 6c66 2e5f 5f61 6e61 6c69 7a61 725f  self.__analizar_
-00003100: 6572 726f 7265 7328 7265 7429 0a20 2020  errores(ret).   
-00003110: 2020 2020 2020 2020 2073 656c 662e 4361           self.Ca
-00003120: 6e74 5061 6769 6e61 7320 3d20 7265 742e  ntPaginas = ret.
-00003130: 6765 7428 2763 616e 7450 6167 696e 6173  get('cantPaginas
-00003140: 2729 0a20 2020 2020 2020 2020 2020 2073  ').            s
-00003150: 656c 662e 4861 7945 7272 6f72 203d 2072  elf.HayError = r
-00003160: 6574 2e67 6574 2827 6861 795f 6572 726f  et.get('hay_erro
-00003170: 7227 290a 2020 2020 2020 2020 2020 2020  r').            
-00003180: 7365 6c66 2e54 7261 6e73 6163 6369 6f6e  self.Transaccion
-00003190: 5365 6e61 7361 203d 205b 6974 2066 6f72  Senasa = [it for
-000031a0: 2069 7420 696e 2072 6574 2e67 6574 2827   it in ret.get('
-000031b0: 6c69 7374 272c 205b 5d29 5d0a 2020 2020  list', [])].    
-000031c0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-000031d0: 0a20 2020 2064 6566 2020 4c65 6572 5472  .    def  LeerTr
-000031e0: 616e 7361 6363 696f 6e28 7365 6c66 293a  ansaccion(self):
-000031f0: 0a20 2020 2020 2020 2022 5265 636f 7272  .        "Recorr
-00003200: 6f20 5472 616e 7361 6363 696f 6e53 656e  o TransaccionSen
-00003210: 6173 6120 6465 7675 656c 746f 2070 6f72  asa devuelto por
-00003220: 2047 6574 5472 616e 7361 6363 696f 6e65   GetTransaccione
-00003230: 7322 0a20 2020 2020 2020 2020 2320 7573  s".         # us
-00003240: 6172 2047 6574 5061 7261 6d65 7472 6f20  ar GetParametro 
-00003250: 7061 7261 2063 6f6e 7375 6c74 6172 2065  para consultar e
-00003260: 6c20 7661 6c6f 7220 7265 746f 726e 6164  l valor retornad
-00003270: 6f20 706f 7220 656c 2077 6562 7365 7276  o por el webserv
-00003280: 6963 650a 0a20 2020 2020 2020 2069 6620  ice..        if 
-00003290: 7365 6c66 2e54 7261 6e73 6163 6369 6f6e  self.Transaccion
-000032a0: 5365 6e61 7361 3a0a 2020 2020 2020 2020  Senasa:.        
-000032b0: 2020 2020 2320 6578 7472 6169 676f 2065      # extraigo e
-000032c0: 6c20 7072 696d 6572 2069 7465 6d0a 2020  l primer item.  
-000032d0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-000032e0: 6172 616d 735f 6f75 7420 3d20 7365 6c66  arams_out = self
-000032f0: 2e54 7261 6e73 6163 6369 6f6e 5365 6e61  .TransaccionSena
-00003300: 7361 2e70 6f70 2830 290a 2020 2020 2020  sa.pop(0).      
-00003310: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00003320: 650a 2020 2020 2020 2020 656c 7365 3a0a  e.        else:.
-00003330: 2020 2020 2020 2020 2020 2020 2320 6c69              # li
-00003340: 6d70 696f 206c 6f73 2070 6172 e16d 6574  mpio los par.met
-00003350: 726f 730a 2020 2020 2020 2020 2020 2020  ros.            
-00003360: 7365 6c66 2e70 6172 616d 735f 6f75 7420  self.params_out 
-00003370: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
-00003380: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
-00003390: 2020 2064 6566 204c 6565 7245 7272 6f72     def LeerError
-000033a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000033b0: 2252 6563 6f72 726f 206c 6f73 2065 7272  "Recorro los err
-000033c0: 6f72 6573 2064 6576 7565 6c74 6f73 2079  ores devueltos y
-000033d0: 2064 6576 7565 6c76 6f20 656c 2070 7269   devuelvo el pri
-000033e0: 6d65 726f 2073 6920 6578 6973 7465 220a  mero si existe".
-000033f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00003400: 2e45 7272 6f72 6573 3a0a 2020 2020 2020  .Errores:.      
-00003410: 2020 2020 2020 2320 6578 7472 6169 676f        # extraigo
-00003420: 2065 6c20 7072 696d 6572 2069 7465 6d0a   el primer item.
-00003430: 2020 2020 2020 2020 2020 2020 6572 203d              er =
-00003440: 2073 656c 662e 4572 726f 7265 732e 706f   self.Errores.po
-00003450: 7028 3029 0a20 2020 2020 2020 2020 2020  p(0).           
-00003460: 2072 6574 7572 6e20 6572 0a20 2020 2020   return er.     
-00003470: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00003480: 2020 2020 2072 6574 7572 6e20 2222 0a0a       return ""..
-00003490: 2020 2020 6465 6620 5365 7455 7365 726e      def SetUsern
-000034a0: 616d 6528 7365 6c66 2c20 7573 6572 6e61  ame(self, userna
-000034b0: 6d65 293a 0a20 2020 2020 2020 2022 4573  me):.        "Es
-000034c0: 7461 626c 657a 636f 2065 6c20 6e6f 6d62  tablezco el nomb
-000034d0: 7265 2064 6520 7573 7561 7269 6f22 0a20  re de usuario". 
-000034e0: 2020 2020 2020 2073 656c 662e 5573 6572         self.User
-000034f0: 6e61 6d65 203d 2075 7365 726e 616d 650a  name = username.
-00003500: 0a20 2020 2064 6566 2053 6574 5061 7373  .    def SetPass
-00003510: 776f 7264 2873 656c 662c 2070 6173 7377  word(self, passw
-00003520: 6f72 6429 3a0a 2020 2020 2020 2020 2245  ord):.        "E
-00003530: 7374 6162 6c65 7a63 6f20 6c61 2063 6f6e  stablezco la con
-00003540: 7472 6173 65f1 6122 0a20 2020 2020 2020  trase.a".       
-00003550: 2073 656c 662e 5061 7373 776f 7264 203d   self.Password =
-00003560: 2070 6173 7377 6f72 640a 0a20 2020 2064   password..    d
-00003570: 6566 2047 6574 436f 6469 676f 5472 616e  ef GetCodigoTran
-00003580: 7361 6363 696f 6e28 7365 6c66 293a 0a20  saccion(self):. 
-00003590: 2020 2020 2020 2022 4465 7675 656c 766f         "Devuelvo
-000035a0: 2065 6c20 63f3 6469 676f 2064 6520 7472   el c.digo de tr
-000035b0: 616e 7361 6363 69f3 6e22 0a20 2020 2020  ansacci.n".     
-000035c0: 2020 2072 6574 7572 6e20 7365 6c66 2e43     return self.C
-000035d0: 6f64 6967 6f54 7261 6e73 6163 6369 6f6e  odigoTransaccion
-000035e0: 0a0a 2020 2020 6465 6620 4765 7452 6573  ..    def GetRes
-000035f0: 756c 7461 646f 2873 656c 6629 3a0a 2020  ultado(self):.  
-00003600: 2020 2020 2020 2244 6576 7565 6c76 6f20        "Devuelvo 
-00003610: 656c 2072 6573 756c 7461 646f 220a 2020  el resultado".  
-00003620: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00003630: 662e 5265 7375 6c74 6164 6f0a 0a0a 6465  f.Resultado...de
-00003640: 6620 6d61 696e 2829 3a0a 2020 2020 2246  f main():.    "F
-00003650: 756e 6369 f36e 2070 7269 6e63 6970 616c  unci.n principal
-00003660: 2064 6520 7072 7565 6261 7320 286f 6274   de pruebas (obt
-00003670: 656e 6572 2043 4145 2922 0a20 2020 2069  ener CAE)".    i
-00003680: 6d70 6f72 7420 6f73 2c20 7469 6d65 2c20  mport os, time, 
-00003690: 7379 730a 2020 2020 676c 6f62 616c 2057  sys.    global W
-000036a0: 5344 4c2c 204c 4f43 4154 494f 4e0a 0a20  SDL, LOCATION.. 
-000036b0: 2020 2044 4542 5547 203d 2027 2d2d 6465     DEBUG = '--de
-000036c0: 6275 6727 2069 6e20 7379 732e 6172 6776  bug' in sys.argv
-000036d0: 0a0a 2020 2020 7773 203d 2054 7261 7a61  ..    ws = Traza
-000036e0: 4669 746f 2829 0a0a 2020 2020 7773 2e55  Fito()..    ws.U
-000036f0: 7365 726e 616d 6520 3d20 2774 6573 7477  sername = 'testw
-00003700: 7365 7276 6963 6527 0a20 2020 2077 732e  service'.    ws.
-00003710: 5061 7373 776f 7264 203d 2027 7465 7374  Password = 'test
-00003720: 7773 6572 7669 6365 7073 7727 0a0a 2020  wservicepsw'..  
-00003730: 2020 6966 2027 2d2d 7072 6f64 2720 696e    if '--prod' in
-00003740: 2073 7973 2e61 7267 7620 616e 6420 6e6f   sys.argv and no
-00003750: 7420 484f 4d4f 3a0a 2020 2020 2020 2020  t HOMO:.        
-00003760: 5753 444c 203d 2022 6874 7470 733a 2f2f  WSDL = "https://
-00003770: 7365 7276 6963 696f 732e 7061 6d69 2e6f  servicios.pami.o
-00003780: 7267 2e61 722f 7472 617a 6161 6772 2e57  rg.ar/trazaagr.W
-00003790: 6562 5365 7276 6963 653f 7773 646c 220a  ebService?wsdl".
-000037a0: 2020 2020 2020 2020 7072 696e 7428 2255          print("U
-000037b0: 7361 6e64 6f20 5753 444c 3a22 2c20 5753  sando WSDL:", WS
-000037c0: 444c 290a 2020 2020 2020 2020 7379 732e  DL).        sys.
-000037d0: 6172 6776 2e70 6f70 2873 7973 2e61 7267  argv.pop(sys.arg
-000037e0: 762e 696e 6465 7828 222d 2d70 726f 6422  v.index("--prod"
-000037f0: 2929 0a0a 2020 2020 2320 496e 6963 6961  ))..    # Inicia
-00003800: 6c69 7a6f 206c 6173 2076 6172 6961 626c  lizo las variabl
-00003810: 6573 2079 2065 7374 7275 6374 7572 6173  es y estructuras
-00003820: 2070 6172 6120 656c 2061 7263 6869 766f   para el archivo
-00003830: 2064 6520 696e 7465 7263 616d 6269 6f3a   de intercambio:
-00003840: 0a20 2020 2074 7261 6e73 6163 6369 6f6e  .    transaccion
-00003850: 5f64 746f 203d 205b 5d0a 2020 2020 7472  _dto = [].    tr
-00003860: 616e 7361 6363 696f 6e65 7320 3d20 5b5d  ansacciones = []
-00003870: 0a20 2020 2065 7272 6f72 6573 203d 205b  .    errores = [
-00003880: 5d0a 2020 2020 666f 726d 6174 6f73 203d  ].    formatos =
-00003890: 205b 2827 5472 616e 7361 6363 696f 6e44   [('TransaccionD
-000038a0: 544f 272c 2054 5241 4e53 4143 4349 4f4e  TO', TRANSACCION
-000038b0: 5f44 544f 2c20 7472 616e 7361 6363 696f  _DTO, transaccio
-000038c0: 6e5f 6474 6f29 2c0a 2020 2020 2020 2020  n_dto),.        
-000038d0: 2020 2020 2020 2020 2827 5472 616e 7361          ('Transa
-000038e0: 6363 696f 6e65 7327 2c20 5452 414e 5341  cciones', TRANSA
-000038f0: 4343 494f 4e45 532c 2074 7261 6e73 6163  CCIONES, transac
-00003900: 6369 6f6e 6573 292c 0a20 2020 2020 2020  ciones),.       
-00003910: 2020 2020 2020 2020 2028 2745 7272 6f72           ('Error
-00003920: 6573 272c 2045 5252 4f52 4553 2c20 6572  es', ERRORES, er
-00003930: 726f 7265 7329 2c0a 2020 2020 2020 2020  rores),.        
-00003940: 2020 2020 2020 205d 0a0a 2020 2020 6966         ]..    if
-00003950: 2027 2d2d 666f 726d 6174 6f27 2069 6e20   '--formato' in 
-00003960: 7379 732e 6172 6776 3a0a 2020 2020 2020  sys.argv:.      
-00003970: 2020 7072 696e 7428 2246 6f72 6d61 746f    print("Formato
-00003980: 3a22 290a 2020 2020 2020 2020 666f 7220  :").        for 
-00003990: 6d73 672c 2066 6f72 6d61 746f 2c20 6c69  msg, formato, li
-000039a0: 7374 6120 696e 2066 6f72 6d61 746f 733a  sta in formatos:
-000039b0: 0a20 2020 2020 2020 2020 2020 2063 6f6d  .            com
-000039c0: 6965 6e7a 6f20 3d20 310a 2020 2020 2020  ienzo = 1.      
-000039d0: 2020 2020 2020 7072 696e 7428 223d 3d3d        print("===
-000039e0: 2025 7320 3d3d 3d22 2025 206d 7367 290a   %s ===" % msg).
-000039f0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00003a00: 7428 227c 7c20 252d 3235 7320 7c7c 2025  t("|| %-25s || %
-00003a10: 2d31 3273 207c 7c20 252d 3573 207c 7c20  -12s || %-5s || 
-00003a20: 252d 3473 207c 7c20 252d 3130 7320 7c7c  %-4s || %-10s ||
-00003a30: 2220 2520 280a 2020 2020 2020 2020 2020  " % (.          
-00003a40: 2020 2020 2020 224e 6f6d 6272 6522 2c20        "Nombre", 
-00003a50: 2254 6970 6f22 2c20 224c 6f6e 672e 222c  "Tipo", "Long.",
-00003a60: 2022 506f 7328 7478 7429 222c 2022 4361   "Pos(txt)", "Ca
-00003a70: 6d70 6f28 6462 6629 2229 290a 2020 2020  mpo(dbf)")).    
-00003a80: 2020 2020 2020 2020 636c 6176 6573 203d          claves =
-00003a90: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
-00003aa0: 666f 7220 666d 7420 696e 2066 6f72 6d61  for fmt in forma
-00003ab0: 746f 3a0a 2020 2020 2020 2020 2020 2020  to:.            
-00003ac0: 2020 2020 636c 6176 652c 206c 6f6e 6769      clave, longi
-00003ad0: 7475 642c 2074 6970 6f20 3d20 666d 745b  tud, tipo = fmt[
-00003ae0: 303a 335d 0a20 2020 2020 2020 2020 2020  0:3].           
-00003af0: 2020 2020 2063 6c61 7665 5f64 6266 203d       clave_dbf =
-00003b00: 2064 6172 5f6e 6f6d 6272 655f 6361 6d70   dar_nombre_camp
-00003b10: 6f5f 6462 6628 636c 6176 652c 2063 6c61  o_dbf(clave, cla
-00003b20: 7665 7329 0a20 2020 2020 2020 2020 2020  ves).           
-00003b30: 2020 2020 2063 6c61 7665 732e 6170 7065       claves.appe
-00003b40: 6e64 2863 6c61 7665 5f64 6266 290a 2020  nd(clave_dbf).  
-00003b50: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00003b60: 696e 7428 227c 7c20 252d 3235 7320 7c7c  int("|| %-25s ||
-00003b70: 2025 2d31 3273 207c 7c20 2535 6420 7c7c   %-12s || %5d ||
-00003b80: 2020 2025 3464 2020 207c 7c20 252d 3130     %4d   || %-10
-00003b90: 7320 7c7c 2220 2520 280a 2020 2020 2020  s ||" % (.      
-00003ba0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-00003bb0: 6176 652c 2074 6970 6f2c 206c 6f6e 6769  ave, tipo, longi
-00003bc0: 7475 642c 2063 6f6d 6965 6e7a 6f2c 2063  tud, comienzo, c
-00003bd0: 6c61 7665 5f64 6266 2929 0a20 2020 2020  lave_dbf)).     
-00003be0: 2020 2020 2020 2020 2020 2063 6f6d 6965             comie
-00003bf0: 6e7a 6f20 2b3d 206c 6f6e 6769 7475 640a  nzo += longitud.
-00003c00: 2020 2020 2020 2020 7379 732e 6578 6974          sys.exit
-00003c10: 2830 290a 0a20 2020 2069 6620 272d 2d63  (0)..    if '--c
-00003c20: 6172 6761 7227 2069 6e20 7379 732e 6172  argar' in sys.ar
-00003c30: 6776 3a0a 2020 2020 2020 2020 6966 2027  gv:.        if '
-00003c40: 2d2d 6462 6627 2069 6e20 7379 732e 6172  --dbf' in sys.ar
-00003c50: 6776 3a0a 2020 2020 2020 2020 2020 2020  gv:.            
-00003c60: 6c65 6572 5f64 6266 2866 6f72 6d61 746f  leer_dbf(formato
-00003c70: 735b 3a31 5d2c 207b 7d29 0a20 2020 2020  s[:1], {}).     
-00003c80: 2020 2065 6c69 6620 272d 2d6a 736f 6e27     elif '--json'
-00003c90: 2069 6e20 7379 732e 6172 6776 3a0a 2020   in sys.argv:.  
-00003ca0: 2020 2020 2020 2020 2020 666f 7220 666f            for fo
-00003cb0: 726d 6174 6f20 696e 2066 6f72 6d61 746f  rmato in formato
-00003cc0: 735b 3a31 5d3a 0a20 2020 2020 2020 2020  s[:1]:.         
-00003cd0: 2020 2020 2020 2061 7263 6869 766f 203d         archivo =
-00003ce0: 206f 7065 6e28 666f 726d 6174 6f5b 305d   open(formato[0]
-00003cf0: 2e6c 6f77 6572 2829 202b 2022 2e6a 736f  .lower() + ".jso
-00003d00: 6e22 2c20 2272 2229 0a20 2020 2020 2020  n", "r").       
-00003d10: 2020 2020 2020 2020 2064 203d 206a 736f           d = jso
-00003d20: 6e2e 6c6f 6164 2861 7263 6869 766f 290a  n.load(archivo).
-00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d40: 666f 726d 6174 6f5b 325d 2e65 7874 656e  formato[2].exten
-00003d50: 6428 6429 0a20 2020 2020 2020 2020 2020  d(d).           
-00003d60: 2020 2020 2061 7263 6869 766f 2e63 6c6f       archivo.clo
-00003d70: 7365 2829 0a20 2020 2020 2020 2065 6c73  se().        els
-00003d80: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
-00003d90: 6f72 2066 6f72 6d61 746f 2069 6e20 666f  or formato in fo
-00003da0: 726d 6174 6f73 5b3a 315d 3a0a 2020 2020  rmatos[:1]:.    
-00003db0: 2020 2020 2020 2020 2020 2020 6172 6368              arch
-00003dc0: 6976 6f20 3d20 6f70 656e 2866 6f72 6d61  ivo = open(forma
-00003dd0: 746f 5b30 5d2e 6c6f 7765 7228 2920 2b20  to[0].lower() + 
-00003de0: 222e 7478 7422 2c20 2272 2229 0a20 2020  ".txt", "r").   
-00003df0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00003e00: 206c 696e 6561 2069 6e20 6172 6368 6976   linea in archiv
-00003e10: 6f3a 0a20 2020 2020 2020 2020 2020 2020  o:.             
-00003e20: 2020 2020 2020 2064 203d 206c 6565 7228         d = leer(
-00003e30: 6c69 6e65 612c 2066 6f72 6d61 746f 5b31  linea, formato[1
-00003e40: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00003e50: 2020 2020 2020 2066 6f72 6d61 746f 5b32         formato[2
-00003e60: 5d2e 6170 7065 6e64 2864 290a 2020 2020  ].append(d).    
-00003e70: 2020 2020 2020 2020 2020 2020 6172 6368              arch
-00003e80: 6976 6f2e 636c 6f73 6528 290a 0a20 2020  ivo.close()..   
-00003e90: 2077 732e 436f 6e65 6374 6172 2822 222c   ws.Conectar("",
-00003ea0: 2057 5344 4c29 0a0a 2020 2020 6966 2077   WSDL)..    if w
-00003eb0: 732e 4578 6365 7063 696f 6e3a 0a20 2020  s.Excepcion:.   
-00003ec0: 2020 2020 2070 7269 6e74 2877 732e 4578       print(ws.Ex
-00003ed0: 6365 7063 696f 6e29 0a20 2020 2020 2020  cepcion).       
-00003ee0: 2070 7269 6e74 2877 732e 5472 6163 6562   print(ws.Traceb
-00003ef0: 6163 6b29 0a20 2020 2020 2020 2073 7973  ack).        sys
-00003f00: 2e65 7869 7428 2d31 290a 0a20 2020 2023  .exit(-1)..    #
-00003f10: 2044 6174 6f73 2064 6520 7072 7565 6261   Datos de prueba
-00003f20: 733a 0a0a 2020 2020 6966 2027 2d2d 7465  s:..    if '--te
-00003f30: 7374 2720 696e 2073 7973 2e61 7267 763a  st' in sys.argv:
-00003f40: 0a20 2020 2020 2020 2074 7261 6e73 6163  .        transac
-00003f50: 6369 6f6e 5f64 746f 2e61 7070 656e 6428  cion_dto.append(
-00003f60: 6469 6374 280a 2020 2020 2020 2020 2020  dict(.          
-00003f70: 2020 676c 6e5f 6f72 6967 656e 3d22 3938    gln_origen="98
-00003f80: 3736 3534 3332 3130 3938 3222 2c20 676c  76543210982", gl
-00003f90: 6e5f 6465 7374 696e 6f3d 2233 3639 3235  n_destino="36925
-00003fa0: 3831 3437 3336 3933 222c 0a20 2020 2020  81473693",.     
-00003fb0: 2020 2020 2020 2066 5f6f 7065 7261 6369         f_operaci
-00003fc0: 6f6e 3d64 6174 6574 696d 652e 6461 7465  on=datetime.date
-00003fd0: 7469 6d65 2e6e 6f77 2829 2e73 7472 6674  time.now().strft
-00003fe0: 696d 6528 2225 642f 256d 2f25 5922 292c  ime("%d/%m/%Y"),
-00003ff0: 0a20 2020 2020 2020 2020 2020 2066 5f65  .            f_e
-00004000: 6c61 626f 7261 6369 6f6e 3d64 6174 6574  laboracion=datet
-00004010: 696d 652e 6461 7465 7469 6d65 2e6e 6f77  ime.datetime.now
-00004020: 2829 2e73 7472 6674 696d 6528 2225 642f  ().strftime("%d/
-00004030: 256d 2f25 5922 292c 0a20 2020 2020 2020  %m/%Y"),.       
-00004040: 2020 2020 2066 5f76 746f 3d28 6461 7465       f_vto=(date
-00004050: 7469 6d65 2e64 6174 6574 696d 652e 6e6f  time.datetime.no
-00004060: 7728 292b 6461 7465 7469 6d65 2e74 696d  w()+datetime.tim
-00004070: 6564 656c 7461 2833 3029 292e 7374 7266  edelta(30)).strf
-00004080: 7469 6d65 2822 2564 2f25 6d2f 2559 2229  time("%d/%m/%Y")
-00004090: 2c0a 2020 2020 2020 2020 2020 2020 6964  ,.            id
-000040a0: 5f65 7665 6e74 6f3d 3131 2c0a 2020 2020  _evento=11,.    
-000040b0: 2020 2020 2020 2020 636f 645f 7072 6f64          cod_prod
-000040c0: 7563 746f 3d22 3838 3930 3030 3030 3030  ucto="8890000000
-000040d0: 3030 3031 222c 0a20 2020 2020 2020 2020  0001",.         
-000040e0: 2020 206e 5f63 616e 7469 6461 643d 312c     n_cantidad=1,
-000040f0: 0a20 2020 2020 2020 2020 2020 206e 5f73  .            n_s
-00004100: 6572 6965 3d69 6e74 2874 696d 652e 7469  erie=int(time.ti
-00004110: 6d65 2829 2a31 3029 2c0a 2020 2020 2020  me()*10),.      
-00004120: 2020 2020 2020 6e5f 6c6f 7465 3d64 6174        n_lote=dat
-00004130: 6574 696d 652e 6461 7465 7469 6d65 2e6e  etime.datetime.n
-00004140: 6f77 2829 2e73 7472 6674 696d 6528 2225  ow().strftime("%
-00004150: 5922 292c 0a20 2020 2020 2020 2020 2020  Y"),.           
-00004160: 206e 5f63 6169 3d22 3132 3334 3536 3738   n_cai="12345678
-00004170: 3930 3132 3334 3522 2c0a 2020 2020 2020  9012345",.      
-00004180: 2020 2020 2020 6e5f 6361 653d 2222 2c0a        n_cae="",.
-00004190: 2020 2020 2020 2020 2020 2020 6964 5f6d              id_m
-000041a0: 6f74 6976 6f5f 6465 7374 7275 6363 696f  otivo_destruccio
-000041b0: 6e3d 302c 0a20 2020 2020 2020 2020 2020  n=0,.           
-000041c0: 206e 5f6d 616e 6966 6965 7374 6f3d 2222   n_manifiesto=""
-000041d0: 2c0a 2020 2020 2020 2020 2020 2020 656e  ,.            en
-000041e0: 5f74 7261 6e73 706f 7274 653d 224e 222c  _transporte="N",
-000041f0: 0a20 2020 2020 2020 2020 2020 206e 5f72  .            n_r
-00004200: 656d 6974 6f3d 2231 3233 3422 2c0a 2020  emito="1234",.  
-00004210: 2020 2020 2020 2020 2020 6d6f 7469 766f            motivo
-00004220: 5f64 6576 6f6c 7563 696f 6e3d 2222 2c0a  _devolucion="",.
-00004230: 2020 2020 2020 2020 2020 2020 6f62 7365              obse
-00004240: 7276 6163 696f 6e65 733d 2270 7275 6562  rvaciones="prueb
-00004250: 6122 2c0a 2020 2020 2020 2020 2020 2020  a",.            
-00004260: 6e5f 7661 6c65 5f63 6f6d 7072 613d 2222  n_vale_compra=""
-00004270: 2c0a 2020 2020 2020 2020 2020 2020 6170  ,.            ap
-00004280: 656c 6c69 646f 4e6f 6d62 7265 733d 224a  ellidoNombres="J
-00004290: 7561 6e20 5065 7265 7322 2c0a 2020 2020  uan Peres",.    
-000042a0: 2020 2020 2020 2020 6469 7265 6363 696f          direccio
-000042b0: 6e3d 2253 6172 617a 6122 2c20 6e75 6d65  n="Saraza", nume
-000042c0: 726f 3d22 3132 3334 222c 0a20 2020 2020  ro="1234",.     
-000042d0: 2020 2020 2020 206c 6f63 616c 6964 6164         localidad
-000042e0: 3d22 4875 726c 696e 6768 616d 222c 2070  ="Hurlingham", p
-000042f0: 726f 7669 6e63 6961 3d22 4275 656e 6f73  rovincia="Buenos
-00004300: 2041 6972 6573 222c 0a20 2020 2020 2020   Aires",.       
-00004310: 2020 2020 206e 5f70 6f73 7461 6c3d 2231       n_postal="1
-00004320: 3638 3822 2c0a 2020 2020 2020 2020 2020  688",.          
-00004330: 2020 6375 6974 3d22 3230 3236 3735 3635    cuit="20267565
-00004340: 3339 3322 2c0a 2020 2020 2020 2020 2020  393",.          
-00004350: 2020 636f 6469 676f 5f74 7261 6e73 6163    codigo_transac
-00004360: 6369 6f6e 3d4e 6f6e 652c 0a20 2020 2020  cion=None,.     
-00004370: 2020 2029 290a 0a20 2020 2023 204f 7063     ))..    # Opc
-00004380: 696f 6e65 7320 7072 696e 6369 7061 6c65  iones principale
-00004390: 733a 0a0a 2020 2020 6966 2027 2d2d 636f  s:..    if '--co
-000043a0: 6e66 6972 6d61 2720 696e 2073 7973 2e61  nfirma' in sys.a
-000043b0: 7267 763a 0a20 2020 2020 2020 2069 6620  rgv:.        if 
-000043c0: 272d 2d6c 6f61 6478 6d6c 2720 696e 2073  '--loadxml' in s
-000043d0: 7973 2e61 7267 763a 0a20 2020 2020 2020  ys.argv:.       
-000043e0: 2020 2020 2077 732e 4c6f 6164 5465 7374       ws.LoadTest
-000043f0: 584d 4c28 2274 7261 7a61 6d65 645f 636f  XML("trazamed_co
-00004400: 6e66 6972 6d61 2e78 6d6c 2229 2020 2320  nfirma.xml")  # 
-00004410: 6361 7267 6f20 7265 7370 7565 7374 610a  cargo respuesta.
-00004420: 2020 2020 2020 2020 2020 2020 6f6b 203d              ok =
-00004430: 2077 732e 5365 6e64 436f 6e66 6972 6d61   ws.SendConfirma
-00004440: 5472 616e 7361 6363 2875 7375 6172 696f  Transacc(usuario
-00004450: 3d22 7072 7565 6261 7377 7322 2c20 7061  ="pruebasws", pa
-00004460: 7373 776f 7264 3d22 7072 7565 6261 7377  ssword="pruebasw
-00004470: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00004480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004490: 2020 2020 2020 2070 5f69 6473 5f74 7261         p_ids_tra
-000044a0: 6e73 6163 3d22 3122 2c20 665f 6f70 6572  nsac="1", f_oper
-000044b0: 6163 696f 6e3d 2233 312d 3132 2d32 3031  acion="31-12-201
-000044c0: 3322 290a 2020 2020 2020 2020 2020 2020  3").            
-000044d0: 6966 206e 6f74 206f 6b3a 0a20 2020 2020  if not ok:.     
-000044e0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000044f0: 2052 756e 7469 6d65 4572 726f 7228 7773   RuntimeError(ws
-00004500: 2e45 7863 6570 6369 6f6e 290a 2020 2020  .Excepcion).    
-00004510: 2020 2020 7773 2e53 656e 6443 6f6e 6669      ws.SendConfi
-00004520: 726d 6154 7261 6e73 6163 6328 2a73 7973  rmaTransacc(*sys
-00004530: 2e61 7267 765b 7379 732e 6172 6776 2e69  .argv[sys.argv.i
-00004540: 6e64 6578 2822 2d2d 636f 6e66 6972 6d61  ndex("--confirma
-00004550: 2229 2b31 3a5d 290a 2020 2020 656c 6966  ")+1:]).    elif
-00004560: 2027 2d2d 616c 6572 7461 2720 696e 2073   '--alerta' in s
-00004570: 7973 2e61 7267 763a 0a20 2020 2020 2020  ys.argv:.       
-00004580: 2077 732e 5365 6e64 416c 6572 7461 5472   ws.SendAlertaTr
-00004590: 616e 7361 6363 282a 7379 732e 6172 6776  ansacc(*sys.argv
-000045a0: 5b73 7973 2e61 7267 762e 696e 6465 7828  [sys.argv.index(
-000045b0: 222d 2d61 6c65 7274 6122 292b 313a 5d29  "--alerta")+1:])
-000045c0: 0a20 2020 2065 6c69 6620 272d 2d63 616e  .    elif '--can
-000045d0: 6365 6c61 2720 696e 2073 7973 2e61 7267  cela' in sys.arg
-000045e0: 763a 0a20 2020 2020 2020 2077 732e 5365  v:.        ws.Se
-000045f0: 6e64 4361 6e63 656c 6154 7261 6e73 6163  ndCancelaTransac
-00004600: 282a 7379 732e 6172 6776 5b73 7973 2e61  (*sys.argv[sys.a
-00004610: 7267 762e 696e 6465 7828 222d 2d63 616e  rgv.index("--can
-00004620: 6365 6c61 2229 2b31 3a5d 290a 2020 2020  cela")+1:]).    
-00004630: 656c 6966 2027 2d2d 636f 6e73 756c 7461  elif '--consulta
-00004640: 2720 696e 2073 7973 2e61 7267 763a 0a20  ' in sys.argv:. 
-00004650: 2020 2020 2020 2077 732e 4765 7454 7261         ws.GetTra
-00004660: 6e73 6163 6369 6f6e 6573 280a 2020 2020  nsacciones(.    
-00004670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004680: 2020 2020 2020 2020 2a73 7973 2e61 7267          *sys.arg
-00004690: 765b 7379 732e 6172 6776 2e69 6e64 6578  v[sys.argv.index
-000046a0: 2822 2d2d 636f 6e73 756c 7461 2229 2b31  ("--consulta")+1
-000046b0: 3a5d 0a20 2020 2020 2020 2020 2020 2020  :].             
-000046c0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000046d0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-000046e0: 4361 6e74 5061 6769 6e61 7322 2c20 7773  CantPaginas", ws
-000046f0: 2e43 616e 7450 6167 696e 6173 290a 2020  .CantPaginas).  
-00004700: 2020 2020 2020 7072 696e 7428 2248 6179        print("Hay
-00004710: 4572 726f 7222 2c20 7773 2e48 6179 4572  Error", ws.HayEr
-00004720: 726f 7229 0a20 2020 2020 2020 2023 2070  ror).        # p
-00004730: 7269 6e74 2822 5472 616e 7361 6363 696f  rint("Transaccio
-00004740: 6e53 656e 6173 6122 2c20 7773 2e54 7261  nSenasa", ws.Tra
-00004750: 6e73 6163 6369 6f6e 5365 6e61 7361 290a  nsaccionSenasa).
-00004760: 2020 2020 2020 2020 2320 7061 7261 6d65          # parame
-00004770: 7472 6f73 2063 6f6d 756e 6573 2064 6520  tros comunes de 
-00004780: 7361 6c69 6461 2028 636f 6c75 6d6e 6173  salida (columnas
-00004790: 2064 6520 6c61 2074 6162 6c61 293a 0a20   de la tabla):. 
-000047a0: 2020 2020 2020 2063 6c61 7665 7320 3d20         claves = 
-000047b0: 5b6b 2066 6f72 206b 2c20 762c 206c 2069  [k for k, v, l i
-000047c0: 6e20 5452 414e 5341 4343 494f 4e45 535d  n TRANSACCIONES]
-000047d0: 0a20 2020 2020 2020 2023 2065 7874 6965  .        # extie
-000047e0: 6e64 6f20 6c61 206c 6973 7461 2064 6520  ndo la lista de 
-000047f0: 7265 7375 6c74 6164 6f20 7061 7261 2065  resultado para e
-00004800: 6c20 6172 6368 6976 6f20 6465 2069 6e74  l archivo de int
-00004810: 6572 6361 6d62 696f 3a0a 2020 2020 2020  ercambio:.      
-00004820: 2020 7472 616e 7361 6363 696f 6e65 732e    transacciones.
-00004830: 6578 7465 6e64 2877 732e 5472 616e 7361  extend(ws.Transa
-00004840: 6363 696f 6e53 656e 6173 6129 0a20 2020  ccionSenasa).   
-00004850: 2020 2020 2023 2065 6e63 6162 657a 6164       # encabezad
-00004860: 6f20 6465 206c 6120 7461 626c 613a 0a20  o de la tabla:. 
-00004870: 2020 2020 2020 2070 7269 6e74 2822 7c7c         print("||
-00004880: 222c 2022 7c7c 222e 6a6f 696e 285b 2225  ", "||".join(["%
-00004890: 7322 2025 2063 6c61 7665 2066 6f72 2063  s" % clave for c
-000048a0: 6c61 7665 2069 6e20 636c 6176 6573 5d29  lave in claves])
-000048b0: 2c20 227c 7c22 290a 2020 2020 2020 2020  , "||").        
-000048c0: 2320 7265 636f 7272 6f20 6c6f 7320 6461  # recorro los da
-000048d0: 746f 7320 6465 7675 656c 746f 7320 2854  tos devueltos (T
-000048e0: 7261 6e73 6163 6369 6f6e 5365 6e61 7361  ransaccionSenasa
-000048f0: 293a 0a20 2020 2020 2020 2077 6869 6c65  ):.        while
-00004900: 2077 732e 4c65 6572 5472 616e 7361 6363   ws.LeerTransacc
-00004910: 696f 6e28 293a 0a20 2020 2020 2020 2020  ion():.         
-00004920: 2020 2066 6f72 2063 6c61 7665 2069 6e20     for clave in 
-00004930: 636c 6176 6573 3a0a 2020 2020 2020 2020  claves:.        
-00004940: 2020 2020 2020 2020 7072 696e 7428 227c          print("|
-00004950: 7c22 2c20 7773 2e47 6574 5061 7261 6d65  |", ws.GetParame
-00004960: 7472 6f28 636c 6176 6529 2920 2020 2020  tro(clave))     
-00004970: 2020 2023 2069 6d70 7269 6d6f 2063 6164     # imprimo cad
-00004980: 6120 6669 6c61 290a 2020 2020 2020 2020  a fila).        
-00004990: 2020 2020 7072 696e 7428 227c 7c22 290a      print("||").
-000049a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000049b0: 2020 6172 6776 203d 205b 6172 6776 2066    argv = [argv f
-000049c0: 6f72 2061 7267 7620 696e 2073 7973 2e61  or argv in sys.a
-000049d0: 7267 7620 6966 206e 6f74 2061 7267 762e  rgv if not argv.
-000049e0: 7374 6172 7473 7769 7468 2822 2d2d 2229  startswith("--")
-000049f0: 5d0a 2020 2020 2020 2020 6966 206e 6f74  ].        if not
-00004a00: 2074 7261 6e73 6163 6369 6f6e 5f64 746f   transaccion_dto
-00004a10: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00004a20: 206c 656e 2861 7267 7629 3e31 303a 0a20   len(argv)>10:. 
-00004a30: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00004a40: 732e 5361 7665 5472 616e 7361 6363 696f  s.SaveTransaccio
-00004a50: 6e28 2a61 7267 765b 313a 5d29 0a20 2020  n(*argv[1:]).   
-00004a60: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00004a70: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00004a80: 7269 6e74 2822 4552 524f 523a 206e 6f20  rint("ERROR: no 
-00004a90: 7365 2069 6e64 6963 6172 6f6e 2074 6f64  se indicaron tod
-00004aa0: 6f73 206c 6f73 2070 6172 e16d 6574 726f  os los par.metro
-00004ab0: 7320 7265 7175 6572 6964 6f73 2229 0a20  s requeridos"). 
-00004ac0: 2020 2020 2020 2065 6c69 6620 7472 616e         elif tran
-00004ad0: 7361 6363 696f 6e5f 6474 6f3a 0a20 2020  saccion_dto:.   
-00004ae0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-00004af0: 2020 2020 2020 2020 2020 2020 2020 7573                us
-00004b00: 7561 7269 6f2c 2070 6173 7377 6f72 6420  uario, password 
-00004b10: 3d20 6172 6776 5b2d 323a 5d0a 2020 2020  = argv[-2:].    
-00004b20: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
-00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b40: 7072 696e 7428 2241 4456 4552 5445 4e43  print("ADVERTENC
-00004b50: 4941 3a20 6e6f 2073 6520 696e 6469 636f  IA: no se indico
-00004b60: 2070 6172 e16d 6574 726f 7320 7573 7561   par.metros usua
-00004b70: 7269 6f20 7920 7061 7373 6f77 6f72 6422  rio y passoword"
-00004b80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004b90: 2020 7573 7561 7269 6f2c 2070 6173 7377    usuario, passw
-00004ba0: 6f72 6420 3d20 2273 656e 6173 6177 7322  ord = "senasaws"
-00004bb0: 2c20 2243 6c61 7665 3230 3133 220a 2020  , "Clave2013".  
-00004bc0: 2020 2020 2020 2020 2020 666f 7220 692c            for i,
-00004bd0: 2064 746f 2069 6e20 656e 756d 6572 6174   dto in enumerat
-00004be0: 6528 7472 616e 7361 6363 696f 6e5f 6474  e(transaccion_dt
-00004bf0: 6f29 3a0a 2020 2020 2020 2020 2020 2020  o):.            
-00004c00: 2020 2020 7072 696e 7428 2250 726f 6365      print("Proce
-00004c10: 7361 6e64 6f20 7265 6769 7374 726f 222c  sando registro",
-00004c20: 2069 290a 2020 2020 2020 2020 2020 2020   i).            
-00004c30: 2020 2020 6465 6c20 6474 6f5b 2763 6f64      del dto['cod
-00004c40: 6967 6f5f 7472 616e 7361 6363 696f 6e27  igo_transaccion'
-00004c50: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00004c60: 2020 7773 2e53 6176 6554 7261 6e73 6163    ws.SaveTransac
-00004c70: 6369 6f6e 2875 7375 6172 696f 2c20 7061  cion(usuario, pa
-00004c80: 7373 776f 7264 2c20 2a2a 6474 6f29 0a20  ssword, **dto). 
-00004c90: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004ca0: 746f 5b27 636f 6469 676f 5f74 7261 6e73  to['codigo_trans
-00004cb0: 6163 6369 6f6e 275d 203d 2077 732e 436f  accion'] = ws.Co
-00004cc0: 6469 676f 5472 616e 7361 6363 696f 6e0a  digoTransaccion.
-00004cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ce0: 6572 726f 7265 732e 6578 7465 6e64 2877  errores.extend(w
-00004cf0: 732e 6572 726f 7265 7329 0a20 2020 2020  s.errores).     
-00004d00: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00004d10: 2822 7c52 6573 756c 7461 646f 2025 3573  ("|Resultado %5s
-00004d20: 7c43 6f64 6967 6f54 7261 6e73 6163 6369  |CodigoTransacci
-00004d30: 6f6e 2025 3130 737c 4572 726f 7265 737c  on %10s|Errores|
-00004d40: 2573 7c22 2025 2028 0a20 2020 2020 2020  %s|" % (.       
-00004d50: 2020 2020 2020 2020 2020 2020 2077 732e               ws.
-00004d60: 5265 7375 6c74 6164 6f2c 0a20 2020 2020  Resultado,.     
-00004d70: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00004d80: 732e 436f 6469 676f 5472 616e 7361 6363  s.CodigoTransacc
-00004d90: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00004da0: 2020 2020 2020 2020 2027 7c27 2e6a 6f69           '|'.joi
-00004db0: 6e28 7773 2e45 7272 6f72 6573 206f 7220  n(ws.Errores or 
-00004dc0: 5b5d 292c 0a20 2020 2020 2020 2020 2020  []),.           
-00004dd0: 2020 2020 2029 290a 2020 2020 2020 2020       )).        
-00004de0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00004df0: 2020 7072 696e 7428 2245 5252 4f52 3a20    print("ERROR: 
-00004e00: 6e6f 2073 6520 6573 7065 6369 6669 6361  no se especifica
-00004e10: 726f 6e20 7072 6f64 7563 746f 7320 6120  ron productos a 
-00004e20: 696e 666f 726d 6172 2229 0a0a 2020 2020  informar")..    
-00004e30: 6966 206e 6f74 2074 7261 6e73 6163 6369  if not transacci
-00004e40: 6f6e 5f64 746f 3a0a 2020 2020 2020 2020  on_dto:.        
-00004e50: 7072 696e 7428 227c 5265 7375 6c74 6164  print("|Resultad
-00004e60: 6f20 2535 737c 436f 6469 676f 5472 616e  o %5s|CodigoTran
-00004e70: 7361 6363 696f 6e20 2531 3073 7c45 7272  saccion %10s|Err
-00004e80: 6f72 6573 7c25 737c 2220 2520 280a 2020  ores|%s|" % (.  
-00004e90: 2020 2020 2020 2020 2020 7773 2e52 6573            ws.Res
-00004ea0: 756c 7461 646f 2c0a 2020 2020 2020 2020  ultado,.        
-00004eb0: 2020 2020 7773 2e43 6f64 6967 6f54 7261      ws.CodigoTra
-00004ec0: 6e73 6163 6369 6f6e 2c0a 2020 2020 2020  nsaccion,.      
-00004ed0: 2020 2020 2020 277c 272e 6a6f 696e 2877        '|'.join(w
-00004ee0: 732e 4572 726f 7265 7320 6f72 205b 5d29  s.Errores or [])
-00004ef0: 2c0a 2020 2020 2020 2020 2929 0a0a 2020  ,.        ))..  
-00004f00: 2020 6966 2077 732e 4578 6365 7063 696f    if ws.Excepcio
-00004f10: 6e3a 0a20 2020 2020 2020 2070 7269 6e74  n:.        print
-00004f20: 2877 732e 5472 6163 6562 6163 6b29 0a0a  (ws.Traceback)..
-00004f30: 2020 2020 6966 2027 2d2d 6772 6162 6172      if '--grabar
-00004f40: 2720 696e 2073 7973 2e61 7267 763a 0a20  ' in sys.argv:. 
-00004f50: 2020 2020 2020 2069 6620 272d 2d64 6266         if '--dbf
-00004f60: 2720 696e 2073 7973 2e61 7267 763a 0a20  ' in sys.argv:. 
-00004f70: 2020 2020 2020 2020 2020 2067 7561 7264             guard
-00004f80: 6172 5f64 6266 2866 6f72 6d61 746f 732c  ar_dbf(formatos,
-00004f90: 2054 7275 652c 207b 7d29 0a20 2020 2020   True, {}).     
-00004fa0: 2020 2065 6c69 6620 272d 2d6a 736f 6e27     elif '--json'
-00004fb0: 2069 6e20 7379 732e 6172 6776 3a0a 2020   in sys.argv:.  
-00004fc0: 2020 2020 2020 2020 2020 666f 7220 666f            for fo
-00004fd0: 726d 6174 6f20 696e 2066 6f72 6d61 746f  rmato in formato
-00004fe0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00004ff0: 2020 2061 7263 6869 766f 203d 206f 7065     archivo = ope
-00005000: 6e28 666f 726d 6174 6f5b 305d 2e6c 6f77  n(formato[0].low
-00005010: 6572 2829 202b 2022 2e6a 736f 6e22 2c20  er() + ".json", 
-00005020: 2277 2229 0a20 2020 2020 2020 2020 2020  "w").           
-00005030: 2020 2020 206a 736f 6e2e 6475 6d70 2866       json.dump(f
-00005040: 6f72 6d61 746f 5b32 5d2c 2061 7263 6869  ormato[2], archi
-00005050: 766f 2c20 736f 7274 5f6b 6579 733d 5472  vo, sort_keys=Tr
-00005060: 7565 2c20 696e 6465 6e74 3d34 290a 2020  ue, indent=4).  
-00005070: 2020 2020 2020 2020 2020 2020 2020 6172                ar
-00005080: 6368 6976 6f2e 636c 6f73 6528 290a 2020  chivo.close().  
-00005090: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000050a0: 2020 2020 2020 2020 666f 7220 666f 726d          for form
-000050b0: 6174 6f20 696e 2066 6f72 6d61 746f 733a  ato in formatos:
-000050c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000050d0: 2061 7263 6869 766f 203d 206f 7065 6e28   archivo = open(
-000050e0: 666f 726d 6174 6f5b 305d 2e6c 6f77 6572  formato[0].lower
-000050f0: 2829 202b 2022 2e74 7874 222c 2022 7722  () + ".txt", "w"
-00005100: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00005110: 2020 666f 7220 6974 2069 6e20 666f 726d    for it in form
-00005120: 6174 6f5b 325d 3a0a 2020 2020 2020 2020  ato[2]:.        
-00005130: 2020 2020 2020 2020 2020 2020 6172 6368              arch
-00005140: 6976 6f2e 7772 6974 6528 6573 6372 6962  ivo.write(escrib
-00005150: 6972 2869 742c 2066 6f72 6d61 746f 5b31  ir(it, formato[1
-00005160: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-00005170: 6172 6368 6976 6f2e 636c 6f73 6528 290a  archivo.close().
-00005180: 0a0a 2320 6275 7363 6f20 656c 2064 6972  ..# busco el dir
-00005190: 6563 746f 7269 6f20 6465 2069 6e73 7461  ectorio de insta
-000051a0: 6c61 6369 f36e 2028 676c 6f62 616c 2070  laci.n (global p
-000051b0: 6172 6120 7175 6520 6e6f 2063 616d 6269  ara que no cambi
-000051c0: 6520 7369 2075 7361 6e20 6f74 7261 2064  e si usan otra d
-000051d0: 6c6c 290a 494e 5354 414c 4c5f 4449 5220  ll).INSTALL_DIR 
-000051e0: 3d20 5472 617a 6146 6974 6f2e 496e 7374  = TrazaFito.Inst
-000051f0: 616c 6c44 6972 203d 2067 6574 5f69 6e73  allDir = get_ins
-00005200: 7461 6c6c 5f64 6972 2829 0a0a 0a69 6620  tall_dir()...if 
-00005210: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
-00005220: 6169 6e5f 5f27 3a0a 0a20 2020 2023 2061  ain__':..    # a
-00005230: 6a75 7374 6f20 656c 2065 6e63 6f64 696e  justo el encodin
-00005240: 6720 706f 7220 6465 6665 6374 6f20 2873  g por defecto (s
-00005250: 6920 7365 2072 6564 6972 696a 6520 6c61  i se redirije la
-00005260: 2073 616c 6964 6129 0a20 2020 2069 6620   salida).    if 
-00005270: 6e6f 7420 6861 7361 7474 7228 7379 732e  not hasattr(sys.
-00005280: 7374 646f 7574 2c20 2265 6e63 6f64 696e  stdout, "encodin
-00005290: 6722 2920 6f72 2073 7973 2e73 7464 6f75  g") or sys.stdou
-000052a0: 742e 656e 636f 6469 6e67 2069 7320 4e6f  t.encoding is No
-000052b0: 6e65 3a0a 2020 2020 2020 2020 696d 706f  ne:.        impo
-000052c0: 7274 2063 6f64 6563 732c 206c 6f63 616c  rt codecs, local
-000052d0: 650a 2020 2020 2020 2020 7379 732e 7374  e.        sys.st
-000052e0: 646f 7574 203d 2063 6f64 6563 732e 6765  dout = codecs.ge
-000052f0: 7477 7269 7465 7228 6c6f 6361 6c65 2e67  twriter(locale.g
-00005300: 6574 7072 6566 6572 7265 6465 6e63 6f64  etpreferredencod
-00005310: 696e 6728 2929 2873 7973 2e73 7464 6f75  ing())(sys.stdou
-00005320: 742c 2272 6570 6c61 6365 2229 3b0a 2020  t,"replace");.  
-00005330: 2020 2020 2020 7379 732e 7374 6465 7272        sys.stderr
-00005340: 203d 2063 6f64 6563 732e 6765 7477 7269   = codecs.getwri
-00005350: 7465 7228 6c6f 6361 6c65 2e67 6574 7072  ter(locale.getpr
-00005360: 6566 6572 7265 6465 6e63 6f64 696e 6728  eferredencoding(
-00005370: 2929 2873 7973 2e73 7464 6572 722c 2272  ))(sys.stderr,"r
-00005380: 6570 6c61 6365 2229 3b0a 0a20 2020 2069  eplace");..    i
-00005390: 6620 272d 2d72 6567 6973 7465 7227 2069  f '--register' i
-000053a0: 6e20 7379 732e 6172 6776 206f 7220 272d  n sys.argv or '-
-000053b0: 2d75 6e72 6567 6973 7465 7227 2069 6e20  -unregister' in 
-000053c0: 7379 732e 6172 6776 3a0a 2020 2020 2020  sys.argv:.      
-000053d0: 2020 696d 706f 7274 2070 7974 686f 6e63    import pythonc
-000053e0: 6f6d 0a20 2020 2020 2020 2069 6d70 6f72  om.        impor
-000053f0: 7420 7769 6e33 3263 6f6d 2e73 6572 7665  t win32com.serve
-00005400: 722e 7265 6769 7374 6572 0a20 2020 2020  r.register.     
-00005410: 2020 2077 696e 3332 636f 6d2e 7365 7276     win32com.serv
-00005420: 6572 2e72 6567 6973 7465 722e 5573 6543  er.register.UseC
-00005430: 6f6d 6d61 6e64 4c69 6e65 2854 7261 7a61  ommandLine(Traza
-00005440: 4669 746f 290a 2020 2020 656c 6966 2022  Fito).    elif "
-00005450: 2f41 7574 6f6d 6174 6522 2069 6e20 7379  /Automate" in sy
-00005460: 732e 6172 6776 3a0a 2020 2020 2020 2020  s.argv:.        
-00005470: 2320 4d53 2073 6565 6d73 2074 6f20 6c69  # MS seems to li
-00005480: 6b65 202f 6175 746f 6d61 7465 2074 6f20  ke /automate to 
-00005490: 7275 6e20 7468 6520 636c 6173 7320 6661  run the class fa
-000054a0: 6374 6f72 6965 732e 0a20 2020 2020 2020  ctories..       
-000054b0: 2069 6d70 6f72 7420 7769 6e33 3263 6f6d   import win32com
-000054c0: 2e73 6572 7665 722e 6c6f 6361 6c73 6572  .server.localser
-000054d0: 7665 720a 2020 2020 2020 2020 2377 696e  ver.        #win
-000054e0: 3332 636f 6d2e 7365 7276 6572 2e6c 6f63  32com.server.loc
-000054f0: 616c 7365 7276 6572 2e6d 6169 6e28 290a  alserver.main().
-00005500: 2020 2020 2020 2020 2320 7374 6172 7420          # start 
-00005510: 7468 6520 7365 7276 6572 2e0a 2020 2020  the server..    
-00005520: 2020 2020 7769 6e33 3263 6f6d 2e73 6572      win32com.ser
-00005530: 7665 722e 6c6f 6361 6c73 6572 7665 722e  ver.localserver.
-00005540: 7365 7276 6528 5b54 7261 7a61 4669 746f  serve([TrazaFito
-00005550: 2e5f 7265 675f 636c 7369 645f 5d29 0a20  ._reg_clsid_]). 
-00005560: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00005570: 206d 6169 6e28 290a                       main().
+00000010: 6e0a 2320 2d2a 2d20 636f 6469 6e67 3a20  n.# -*- coding: 
+00000020: 7574 662d 3820 2d2a 2d0a 2320 5468 6973  utf-8 -*-.# This
+00000030: 2070 726f 6772 616d 2069 7320 6672 6565   program is free
+00000040: 2073 6f66 7477 6172 653b 2079 6f75 2063   software; you c
+00000050: 616e 2072 6564 6973 7472 6962 7574 6520  an redistribute 
+00000060: 6974 2061 6e64 2f6f 7220 6d6f 6469 6679  it and/or modify
+00000070: 0a23 2069 7420 756e 6465 7220 7468 6520  .# it under the 
+00000080: 7465 726d 7320 6f66 2074 6865 2047 4e55  terms of the GNU
+00000090: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
+000000a0: 4c69 6365 6e73 6520 6173 2070 7562 6c69  License as publi
+000000b0: 7368 6564 2062 7920 7468 650a 2320 4672  shed by the.# Fr
+000000c0: 6565 2053 6f66 7477 6172 6520 466f 756e  ee Software Foun
+000000d0: 6461 7469 6f6e 3b20 6569 7468 6572 2076  dation; either v
+000000e0: 6572 7369 6f6e 2033 2c20 6f72 2028 6174  ersion 3, or (at
+000000f0: 2079 6f75 7220 6f70 7469 6f6e 2920 616e   your option) an
+00000100: 7920 6c61 7465 720a 2320 7665 7273 696f  y later.# versio
+00000110: 6e2e 0a23 0a23 2054 6869 7320 7072 6f67  n..#.# This prog
+00000120: 7261 6d20 6973 2064 6973 7472 6962 7574  ram is distribut
+00000130: 6564 2069 6e20 7468 6520 686f 7065 2074  ed in the hope t
+00000140: 6861 7420 6974 2077 696c 6c20 6265 2075  hat it will be u
+00000150: 7365 6675 6c2c 2062 7574 0a23 2057 4954  seful, but.# WIT
+00000160: 484f 5554 2041 4e59 2057 4152 5241 4e54  HOUT ANY WARRANT
+00000170: 593b 2077 6974 686f 7574 2065 7665 6e20  Y; without even 
+00000180: 7468 6520 696d 706c 6965 6420 7761 7272  the implied warr
+00000190: 616e 7479 206f 6620 4d45 5243 4841 4e54  anty of MERCHANT
+000001a0: 4942 494c 4954 590a 2320 6f72 2046 4954  IBILITY.# or FIT
+000001b0: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
+000001c0: 4355 4c41 5220 5055 5250 4f53 452e 2020  CULAR PURPOSE.  
+000001d0: 5365 6520 7468 6520 474e 5520 4765 6e65  See the GNU Gene
+000001e0: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
+000001f0: 7365 0a23 2066 6f72 206d 6f72 6520 6465  se.# for more de
+00000200: 7461 696c 732e 0a0a 224d f364 756c 6f20  tails..."M.dulo 
+00000210: 5472 617a 6162 696c 6964 6164 2064 6520  Trazabilidad de 
+00000220: 5072 6f64 7563 746f 7320 4669 746f 7361  Productos Fitosa
+00000230: 6e69 7461 7269 6f73 2053 454e 4153 4120  nitarios SENASA 
+00000240: 5265 736f 6c75 6369 f36e 2033 3639 2f32  Resoluci.n 369/2
+00000250: 3031 3322 0a0a 2320 496e 666f 726d 6163  013"..# Informac
+00000260: 69f3 6e20 6164 6963 696f 6e61 6c20 7920  i.n adicional y 
+00000270: 646f 6375 6d65 6e74 6163 69f3 6e3a 0a23  documentaci.n:.#
+00000280: 2068 7474 703a 2f2f 7777 772e 7369 7374   http://www.sist
+00000290: 656d 6173 6167 696c 6573 2e63 6f6d 2e61  emasagiles.com.a
+000002a0: 722f 7472 6163 2f77 696b 692f 5472 617a  r/trac/wiki/Traz
+000002b0: 6162 696c 6964 6164 5072 6f64 7563 746f  abilidadProducto
+000002c0: 7346 6974 6f73 616e 6974 6172 696f 730a  sFitosanitarios.
+000002d0: 0a5f 5f61 7574 686f 725f 5f20 3d20 224d  .__author__ = "M
+000002e0: 6172 6961 6e6f 2052 6569 6e67 6172 7420  ariano Reingart 
+000002f0: 3c72 6569 6e67 6172 7440 676d 6169 6c2e  <reingart@gmail.
+00000300: 636f 6d3e 220a 5f5f 636f 7079 7269 6768  com>".__copyrigh
+00000310: 745f 5f20 3d20 2243 6f70 7972 6967 6874  t__ = "Copyright
+00000320: 2028 4329 2032 3031 3420 4d61 7269 616e   (C) 2014 Marian
+00000330: 6f20 5265 696e 6761 7274 220a 5f5f 6c69  o Reingart".__li
+00000340: 6365 6e73 655f 5f20 3d20 2247 504c 2033  cense__ = "GPL 3
+00000350: 2e30 2b22 0a5f 5f76 6572 7369 6f6e 5f5f  .0+".__version__
+00000360: 203d 2022 312e 3131 6422 0a0a 2320 6874   = "1.11d"..# ht
+00000370: 7470 3a2f 2f73 656e 6173 612e 7365 7276  tp://senasa.serv
+00000380: 6963 696f 732e 7061 6d69 2e6f 7267 2e61  icios.pami.org.a
+00000390: 722f 0a0a 696d 706f 7274 206f 730a 696d  r/..import os.im
+000003a0: 706f 7274 2073 6f63 6b65 740a 696d 706f  port socket.impo
+000003b0: 7274 2073 7973 0a69 6d70 6f72 7420 6461  rt sys.import da
+000003c0: 7465 7469 6d65 2c20 7469 6d65 0a69 6d70  tetime, time.imp
+000003d0: 6f72 7420 7472 6163 6562 6163 6b0a 696d  ort traceback.im
+000003e0: 706f 7274 2070 7933 7369 6d70 6c65 736f  port py3simpleso
+000003f0: 6170 2e63 6c69 656e 740a 6672 6f6d 2070  ap.client.from p
+00000400: 7933 7369 6d70 6c65 736f 6170 2e63 6c69  y3simplesoap.cli
+00000410: 656e 7420 696d 706f 7274 2053 6f61 7043  ent import SoapC
+00000420: 6c69 656e 742c 2053 6f61 7046 6175 6c74  lient, SoapFault
+00000430: 2c20 7061 7273 655f 7072 6f78 792c 205c  , parse_proxy, \
+00000440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000460: 2073 6574 5f68 7474 705f 7772 6170 7065   set_http_wrappe
+00000470: 720a 6672 6f6d 2070 7933 7369 6d70 6c65  r.from py3simple
+00000480: 736f 6170 2e73 696d 706c 6578 6d6c 2069  soap.simplexml i
+00000490: 6d70 6f72 7420 5369 6d70 6c65 584d 4c45  mport SimpleXMLE
+000004a0: 6c65 6d65 6e74 0a66 726f 6d20 6353 7472  lement.from cStr
+000004b0: 696e 6749 4f20 696d 706f 7274 2053 7472  ingIO import Str
+000004c0: 696e 6749 4f0a 0a23 2069 6d70 6f72 746f  ingIO..# importo
+000004d0: 2066 756e 6369 6f6e 6573 2063 6f6d 7061   funciones compa
+000004e0: 7274 6964 6173 3a0a 6672 6f6d 202e 7574  rtidas:.from .ut
+000004f0: 696c 7320 696d 706f 7274 206c 6565 722c  ils import leer,
+00000500: 2065 7363 7269 6269 722c 206c 6565 725f   escribir, leer_
+00000510: 6462 662c 2067 7561 7264 6172 5f64 6266  dbf, guardar_dbf
+00000520: 2c20 4e2c 2041 2c20 492c 206a 736f 6e2c  , N, A, I, json,
+00000530: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+00000540: 2020 2020 2064 6172 5f6e 6f6d 6272 655f       dar_nombre_
+00000550: 6361 6d70 6f5f 6462 662c 2067 6574 5f69  campo_dbf, get_i
+00000560: 6e73 7461 6c6c 5f64 6972 2c20 4261 7365  nstall_dir, Base
+00000570: 5753 2c20 5c0a 2020 2020 2020 2020 2020  WS, \.          
+00000580: 2020 2020 2020 2020 696e 6963 6961 6c69          iniciali
+00000590: 7a61 725f 795f 6361 7074 7572 6172 5f65  zar_y_capturar_e
+000005a0: 7863 6570 6369 6f6e 6573 0a0a 484f 4d4f  xcepciones..HOMO
+000005b0: 203d 2046 616c 7365 0a54 5950 454c 4942   = False.TYPELIB
+000005c0: 203d 2046 616c 7365 0a0a 5753 444c 203d   = False..WSDL =
+000005d0: 2022 6874 7470 733a 2f2f 7365 7276 6963   "https://servic
+000005e0: 696f 732e 7061 6d69 2e6f 7267 2e61 722f  ios.pami.org.ar/
+000005f0: 7472 617a 6165 6e61 6772 2e57 6562 5365  trazaenagr.WebSe
+00000600: 7276 6963 653f 7773 646c 220a 4c4f 4341  rvice?wsdl".LOCA
+00000610: 5449 4f4e 203d 2022 6874 7470 733a 2f2f  TION = "https://
+00000620: 7365 7276 6963 696f 732e 7061 6d69 2e6f  servicios.pami.o
+00000630: 7267 2e61 722f 7472 617a 6165 6e61 6772  rg.ar/trazaenagr
+00000640: 2e57 6562 5365 7276 6963 6522 0a0a 2320  .WebService"..# 
+00000650: 466f 726d 6174 6f20 6465 2054 7261 6e73  Formato de Trans
+00000660: 6163 6369 6f6e 5365 6e61 7361 4454 4f20  accionSenasaDTO 
+00000670: 2853 6176 6554 7261 6e73 6163 6369 6f6e  (SaveTransaccion
+00000680: 290a 5452 414e 5341 4343 494f 4e5f 4454  ).TRANSACCION_DT
+00000690: 4f20 3d20 5b0a 2020 2020 2827 676c 6e5f  O = [.    ('gln_
+000006a0: 6f72 6967 656e 272c 2031 332c 2041 292c  origen', 13, A),
+000006b0: 0a20 2020 2028 2767 6c6e 5f64 6573 7469  .    ('gln_desti
+000006c0: 6e6f 272c 2031 332c 2041 292c 0a20 2020  no', 13, A),.   
+000006d0: 2028 2766 5f6f 7065 7261 6369 6f6e 272c   ('f_operacion',
+000006e0: 2031 302c 2041 292c 0a20 2020 2028 2766   10, A),.    ('f
+000006f0: 5f65 6c61 626f 7261 6369 6f6e 272c 2031  _elaboracion', 1
+00000700: 302c 2041 292c 0a20 2020 2028 2766 5f76  0, A),.    ('f_v
+00000710: 746f 272c 2031 302c 2041 292c 0a20 2020  to', 10, A),.   
+00000720: 2028 2769 645f 6576 656e 746f 272c 2031   ('id_evento', 1
+00000730: 352c 204e 292c 0a20 2020 2028 2763 6f64  5, N),.    ('cod
+00000740: 5f70 726f 6475 6374 6f27 2c20 3134 2c20  _producto', 14, 
+00000750: 4129 2c0a 2020 2020 2827 6e5f 6361 6e74  A),.    ('n_cant
+00000760: 6964 6164 272c 2033 302c 204e 292c 0a20  idad', 30, N),. 
+00000770: 2020 2028 276e 5f73 6572 6965 272c 2032     ('n_serie', 2
+00000780: 302c 2041 292c 0a20 2020 2028 276e 5f6c  0, A),.    ('n_l
+00000790: 6f74 6527 2c20 3530 2c20 4129 2c0a 2020  ote', 50, A),.  
+000007a0: 2020 2827 6e5f 6361 6927 2c20 3135 2c20    ('n_cai', 15, 
+000007b0: 4129 2c0a 2020 2020 2827 6e5f 6361 6527  A),.    ('n_cae'
+000007c0: 2c20 3135 2c20 4129 2c0a 2020 2020 2827  , 15, A),.    ('
+000007d0: 6964 5f6d 6f74 6976 6f5f 6465 7374 7275  id_motivo_destru
+000007e0: 6363 696f 6e27 2c20 352c 2041 292c 0a20  ccion', 5, A),. 
+000007f0: 2020 2028 276e 5f6d 616e 6966 6965 7374     ('n_manifiest
+00000800: 6f27 2c20 3135 2c20 4e29 2c0a 2020 2020  o', 15, N),.    
+00000810: 2827 656e 5f74 7261 6e73 706f 7274 6527  ('en_transporte'
+00000820: 2c20 312c 2041 292c 2023 2062 6f6f 6c65  , 1, A), # boole
+00000830: 616e 0a20 2020 2028 276e 5f72 656d 6974  an.    ('n_remit
+00000840: 6f27 2c20 3135 2c20 4129 2c0a 2020 2020  o', 15, A),.    
+00000850: 2827 6d6f 7469 766f 5f64 6576 6f6c 7563  ('motivo_devoluc
+00000860: 696f 6e27 2c20 3130 302c 2041 292c 0a20  ion', 100, A),. 
+00000870: 2020 2028 276f 6273 6572 7661 6369 6f6e     ('observacion
+00000880: 6573 272c 2031 3030 302c 2041 292c 0a20  es', 1000, A),. 
+00000890: 2020 2028 276e 5f76 616c 655f 636f 6d70     ('n_vale_comp
+000008a0: 7261 272c 2031 352c 2041 292c 0a20 2020  ra', 15, A),.   
+000008b0: 2028 2761 7065 6c6c 6964 6f4e 6f6d 6272   ('apellidoNombr
+000008c0: 6573 272c 2032 3535 2c20 4129 2c0a 2020  es', 255, A),.  
+000008d0: 2020 2827 6469 7265 6363 696f 6e27 2c20    ('direccion', 
+000008e0: 3230 302c 2041 292c 0a20 2020 2028 276e  200, A),.    ('n
+000008f0: 756d 6572 6f27 2c20 362c 204e 292c 0a20  umero', 6, N),. 
+00000900: 2020 2028 276c 6f63 616c 6964 6164 272c     ('localidad',
+00000910: 2031 352c 2041 292c 0a20 2020 2028 2770   15, A),.    ('p
+00000920: 726f 7669 6e63 6961 272c 2031 352c 2041  rovincia', 15, A
+00000930: 292c 0a20 2020 2028 276e 5f70 6f73 7461  ),.    ('n_posta
+00000940: 6c27 2c20 382c 2041 292c 0a20 2020 2028  l', 8, A),.    (
+00000950: 2763 7569 7427 2c20 3131 2c20 4129 2c0a  'cuit', 11, A),.
+00000960: 2020 2020 2827 636f 6469 676f 5f74 7261      ('codigo_tra
+00000970: 6e73 6163 6369 6f6e 272c 2031 342c 2041  nsaccion', 14, A
+00000980: 292c 0a5d 0a0a 2320 466f 726d 6174 6f20  ),.]..# Formato 
+00000990: 7061 7261 2054 7261 6e73 6163 6369 6f6e  para Transaccion
+000009a0: 5365 6e61 7361 2028 6765 7454 7261 6e73  Senasa (getTrans
+000009b0: 6163 6369 6f6e 6573 290a 5452 414e 5341  acciones).TRANSA
+000009c0: 4343 494f 4e45 5320 3d20 5b0a 2020 2020  CCIONES = [.    
+000009d0: 2827 6964 5f74 7261 6e73 6163 6369 6f6e  ('id_transaccion
+000009e0: 5f67 6c6f 6261 6c27 2c20 3135 2c20 4e29  _global', 15, N)
+000009f0: 2c0a 2020 2020 2827 6964 5f74 7261 6e73  ,.    ('id_trans
+00000a00: 6163 6369 6f6e 272c 2031 352c 204e 292c  accion', 15, N),
+00000a10: 0a20 2020 2028 2766 5f74 7261 6e73 6163  .    ('f_transac
+00000a20: 6369 6f6e 272c 2031 302c 2041 292c 0a20  cion', 10, A),. 
+00000a30: 2020 2028 2766 5f6f 7065 7261 6369 6f6e     ('f_operacion
+00000a40: 272c 2031 302c 2041 292c 0a20 2020 2028  ', 10, A),.    (
+00000a50: 2766 5f76 656e 6369 6d69 656e 746f 272c  'f_vencimiento',
+00000a60: 2031 302c 2041 292c 0a20 2020 2028 2766   10, A),.    ('f
+00000a70: 5f65 6c61 626f 7261 6369 6f6e 272c 2031  _elaboracion', 1
+00000a80: 302c 2041 292c 0a20 2020 2028 2764 5f65  0, A),.    ('d_e
+00000a90: 7665 6e74 6f27 2c20 3130 302c 2041 292c  vento', 100, A),
+00000aa0: 0a20 2020 2028 2763 616e 7469 6461 6427  .    ('cantidad'
+00000ab0: 2c20 3330 2c20 4e29 2c0a 2020 2020 2827  , 30, N),.    ('
+00000ac0: 6964 5f75 6e69 6461 6427 2c20 3135 2c20  id_unidad', 15, 
+00000ad0: 4e29 2c0a 2020 2020 2827 645f 756e 6964  N),.    ('d_unid
+00000ae0: 6164 272c 2031 3030 2c20 4129 2c0a 2020  ad', 100, A),.  
+00000af0: 2020 2827 636f 645f 7072 6f64 7563 746f    ('cod_producto
+00000b00: 272c 2031 342c 2041 292c 0a20 2020 2028  ', 14, A),.    (
+00000b10: 2769 645f 756e 6964 6164 272c 2031 352c  'id_unidad', 15,
+00000b20: 204e 292c 0a20 2020 2028 276e 5f73 6572   N),.    ('n_ser
+00000b30: 6965 272c 2032 302c 2041 292c 0a20 2020  ie', 20, A),.   
+00000b40: 2028 276e 5f6c 6f74 6527 2c20 3530 2c20   ('n_lote', 50, 
+00000b50: 4129 2c0a 2020 2020 2827 6e5f 6361 6927  A),.    ('n_cai'
+00000b60: 2c20 3135 2c20 4129 2c0a 2020 2020 2827  , 15, A),.    ('
+00000b70: 6e5f 6361 6527 2c20 3135 2c20 4129 2c0a  n_cae', 15, A),.
+00000b80: 2020 2020 2827 645f 6d6f 7469 766f 5f64      ('d_motivo_d
+00000b90: 6573 7472 7563 6369 6f6e 272c 2035 302c  estruccion', 50,
+00000ba0: 2041 292c 0a20 2020 2028 2764 5f6d 616e   A),.    ('d_man
+00000bb0: 6966 6965 7374 6f27 2c20 3135 2c20 4129  ifiesto', 15, A)
+00000bc0: 2c0a 2020 2020 2827 656e 5f74 7261 6e73  ,.    ('en_trans
+00000bd0: 706f 7274 6527 2c20 312c 2041 292c 0a20  porte', 1, A),. 
+00000be0: 2020 2028 276e 5f72 656d 6974 6f27 2c20     ('n_remito', 
+00000bf0: 3330 2c20 4129 2c0a 2020 2020 2827 6d6f  30, A),.    ('mo
+00000c00: 7469 766f 5f64 6576 6f6c 7563 696f 6e27  tivo_devolucion'
+00000c10: 2c20 3230 302c 2041 292c 0a20 2020 2028  , 200, A),.    (
+00000c20: 276f 6273 6572 7661 6369 6f6e 6573 272c  'observaciones',
+00000c30: 2031 3030 302c 2041 292c 0a20 2020 2028   1000, A),.    (
+00000c40: 276e 5f76 616c 655f 636f 6d70 7261 272c  'n_vale_compra',
+00000c50: 2031 352c 2041 292c 0a20 2020 2028 2761   15, A),.    ('a
+00000c60: 7065 6c6c 6964 6f4e 6f6d 6272 6573 272c  pellidoNombres',
+00000c70: 2032 3535 2c20 4129 2c0a 2020 2020 2827   255, A),.    ('
+00000c80: 6469 7265 6363 696f 6e27 2c20 3230 302c  direccion', 200,
+00000c90: 2041 292c 0a20 2020 2028 276e 756d 6572   A),.    ('numer
+00000ca0: 6f27 2c20 362c 2041 292c 0a20 2020 2028  o', 6, A),.    (
+00000cb0: 276c 6f63 616c 6964 6164 272c 2032 3530  'localidad', 250
+00000cc0: 2c20 4129 2c0a 2020 2020 2827 7072 6f76  , A),.    ('prov
+00000cd0: 696e 6369 6127 2c20 3235 302c 2041 292c  incia', 250, A),
+00000ce0: 0a20 2020 2028 276e 5f70 6f73 7461 6c27  .    ('n_postal'
+00000cf0: 2c20 382c 2041 292c 0a20 2020 2028 2763  , 8, A),.    ('c
+00000d00: 7569 7427 2c20 3131 2c20 4129 2c0a 2020  uit', 11, A),.  
+00000d10: 2020 2827 645f 6167 656e 7465 5f69 6e66    ('d_agente_inf
+00000d20: 6f72 6d61 646f 7227 2c20 3235 352c 2041  ormador', 255, A
+00000d30: 292c 0a20 2020 2028 2764 5f61 6765 6e74  ),.    ('d_agent
+00000d40: 655f 6f72 6967 656e 272c 2032 3535 2c20  e_origen', 255, 
+00000d50: 4129 2c0a 2020 2020 2827 645f 6167 656e  A),.    ('d_agen
+00000d60: 7465 5f64 6573 7469 6e6f 272c 2032 3535  te_destino', 255
+00000d70: 2c20 4129 2c0a 2020 2020 2827 645f 7072  , A),.    ('d_pr
+00000d80: 6f64 7563 746f 272c 2032 3530 2c20 4129  oducto', 250, A)
+00000d90: 2c0a 2020 2020 2827 645f 6573 7461 646f  ,.    ('d_estado
+00000da0: 5f74 7261 6e73 6163 6369 6f6e 272c 2033  _transaccion', 3
+00000db0: 302c 2041 292c 0a20 2020 2028 2764 5f74  0, A),.    ('d_t
+00000dc0: 6970 6f5f 7472 616e 7361 6363 696f 6e27  ipo_transaccion'
+00000dd0: 2c20 3330 2c20 4129 2c0a 5d0a 0a23 2046  , 30, A),.]..# F
+00000de0: 6f72 6d61 746f 2070 6172 6120 4572 726f  ormato para Erro
+00000df0: 7265 730a 4552 524f 5245 5320 3d20 5b0a  res.ERRORES = [.
+00000e00: 2020 2020 2827 5f63 5f65 7272 6f72 272c      ('_c_error',
+00000e10: 2034 2c20 4129 2c20 2020 2020 2020 2020   4, A),         
+00000e20: 2020 2020 2020 2020 2320 63f3 6469 676f          # c.digo
+00000e30: 0a20 2020 2028 275f 645f 6572 726f 7227  .    ('_d_error'
+00000e40: 2c20 3235 302c 2041 292c 2020 2020 2020  , 250, A),      
+00000e50: 2020 2020 2020 2020 2023 2064 6573 6372           # descr
+00000e60: 6970 6369 f36e 0a20 2020 205d 0a0a 0a63  ipci.n.    ]...c
+00000e70: 6c61 7373 2054 7261 7a61 4669 746f 2842  lass TrazaFito(B
+00000e80: 6173 6557 5329 3a0a 2020 2020 2249 6e74  aseWS):.    "Int
+00000e90: 6572 6661 7a20 7061 7261 2065 6c20 5765  erfaz para el We
+00000ea0: 6253 6572 7669 6365 2064 6520 5472 617a  bService de Traz
+00000eb0: 6162 696c 6964 6164 2064 6520 4669 746f  abilidad de Fito
+00000ec0: 7361 6e69 7461 7269 6f73 2053 454e 4153  sanitarios SENAS
+00000ed0: 4122 0a0a 2020 2020 5f70 7562 6c69 635f  A"..    _public_
+00000ee0: 6d65 7468 6f64 735f 203d 205b 2753 6176  methods_ = ['Sav
+00000ef0: 6554 7261 6e73 6163 6369 6f6e 272c 2027  eTransaccion', '
+00000f00: 5365 6e64 4361 6e63 656c 6154 7261 6e73  SendCancelaTrans
+00000f10: 6163 272c 0a20 2020 2020 2020 2020 2020  ac',.           
+00000f20: 2020 2020 2020 2020 2020 2020 2027 5365               'Se
+00000f30: 6e64 436f 6e66 6972 6d61 5472 616e 7361  ndConfirmaTransa
+00000f40: 6363 272c 2027 5365 6e64 416c 6572 7461  cc', 'SendAlerta
+00000f50: 5472 616e 7361 6363 272c 0a20 2020 2020  Transacc',.     
+00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f70: 2020 2027 4765 7454 7261 6e73 6163 6369     'GetTransacci
+00000f80: 6f6e 6573 272c 0a20 2020 2020 2020 2020  ones',.         
+00000f90: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00000fa0: 436f 6e65 6374 6172 272c 2027 4c65 6572  Conectar', 'Leer
+00000fb0: 4572 726f 7227 2c20 274c 6565 7254 7261  Error', 'LeerTra
+00000fc0: 6e73 6163 6369 6f6e 272c 0a20 2020 2020  nsaccion',.     
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fe0: 2020 2027 5365 7455 7365 726e 616d 6527     'SetUsername'
+00000ff0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001000: 2020 2020 2020 2020 2020 2753 6574 5061            'SetPa
+00001010: 7261 6d65 7472 6f27 2c20 2747 6574 5061  rametro', 'GetPa
+00001020: 7261 6d65 7472 6f27 2c0a 2020 2020 2020  rametro',.      
+00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001040: 2020 2747 6574 436f 6469 676f 5472 616e    'GetCodigoTran
+00001050: 7361 6363 696f 6e27 2c20 2747 6574 5265  saccion', 'GetRe
+00001060: 7375 6c74 6164 6f27 2c20 274c 6f61 6454  sultado', 'LoadT
+00001070: 6573 7458 4d4c 275d 0a0a 2020 2020 5f70  estXML']..    _p
+00001080: 7562 6c69 635f 6174 7472 735f 203d 205b  ublic_attrs_ = [
+00001090: 0a20 2020 2020 2020 2027 5573 6572 6e61  .        'Userna
+000010a0: 6d65 272c 2027 5061 7373 776f 7264 272c  me', 'Password',
+000010b0: 0a20 2020 2020 2020 2027 436f 6469 676f  .        'Codigo
+000010c0: 5472 616e 7361 6363 696f 6e27 2c20 2745  Transaccion', 'E
+000010d0: 7272 6f72 6573 272c 2027 5265 7375 6c74  rrores', 'Result
+000010e0: 6164 6f27 2c0a 2020 2020 2020 2020 2758  ado',.        'X
+000010f0: 6d6c 5265 7175 6573 7427 2c20 2758 6d6c  mlRequest', 'Xml
+00001100: 5265 7370 6f6e 7365 272c 0a20 2020 2020  Response',.     
+00001110: 2020 2027 5665 7273 696f 6e27 2c20 2749     'Version', 'I
+00001120: 6e73 7461 6c6c 4469 7227 2c0a 2020 2020  nstallDir',.    
+00001130: 2020 2020 2754 7261 6365 6261 636b 272c      'Traceback',
+00001140: 2027 4578 6365 7063 696f 6e27 2c20 274c   'Excepcion', 'L
+00001150: 616e 7a61 7245 7863 6570 6369 6f6e 6573  anzarExcepciones
+00001160: 272c 0a20 2020 2020 2020 2027 4361 6e74  ',.        'Cant
+00001170: 5061 6769 6e61 7327 2c20 2748 6179 4572  Paginas', 'HayEr
+00001180: 726f 7227 2c20 2754 7261 6e73 6163 6369  ror', 'Transacci
+00001190: 6f6e 5365 6e61 7361 272c 0a20 2020 2020  onSenasa',.     
+000011a0: 2020 205d 0a0a 2020 2020 5f72 6567 5f70     ]..    _reg_p
+000011b0: 726f 6769 645f 203d 2022 5472 617a 6146  rogid_ = "TrazaF
+000011c0: 6974 6f22 0a20 2020 205f 7265 675f 636c  ito".    _reg_cl
+000011d0: 7369 645f 203d 2022 7b33 3937 3933 3933  sid_ = "{3979393
+000011e0: 312d 3435 3041 2d34 4636 362d 3933 3234  1-450A-4F66-9324
+000011f0: 2d44 3444 3938 3146 4335 3331 397d 220a  -D4D981FC5319}".
+00001200: 0a20 2020 2023 2056 6172 6961 626c 6573  .    # Variables
+00001210: 2067 6c6f 6261 6c65 7320 7061 7261 2042   globales para B
+00001220: 6173 6557 533a 0a20 2020 2048 4f4d 4f20  aseWS:.    HOMO 
+00001230: 3d20 484f 4d4f 0a20 2020 2057 5344 4c20  = HOMO.    WSDL 
+00001240: 3d20 5753 444c 0a20 2020 2056 6572 7369  = WSDL.    Versi
+00001250: 6f6e 203d 2022 2573 2025 7320 2573 2220  on = "%s %s %s" 
+00001260: 2520 285f 5f76 6572 7369 6f6e 5f5f 2c20  % (__version__, 
+00001270: 484f 4d4f 2061 6e64 2027 486f 6d6f 6c6f  HOMO and 'Homolo
+00001280: 6761 6369 f36e 2720 6f72 2027 272c 0a20  gaci.n' or '',. 
+00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012a0: 2020 2020 2020 2020 2020 2070 7933 7369             py3si
+000012b0: 6d70 6c65 736f 6170 2e63 6c69 656e 742e  mplesoap.client.
+000012c0: 5f5f 7665 7273 696f 6e5f 5f29 0a0a 2020  __version__)..  
+000012d0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+000012e0: 656c 662c 2072 6569 6e74 656e 746f 733d  elf, reintentos=
+000012f0: 3129 3a0a 2020 2020 2020 2020 7365 6c66  1):.        self
+00001300: 2e55 7365 726e 616d 6520 3d20 7365 6c66  .Username = self
+00001310: 2e50 6173 7377 6f72 6420 3d20 4e6f 6e65  .Password = None
+00001320: 0a20 2020 2020 2020 2073 656c 662e 5472  .        self.Tr
+00001330: 616e 7361 6363 696f 6e53 656e 6173 6120  ansaccionSenasa 
+00001340: 3d20 5b5d 0a20 2020 2020 2020 2042 6173  = [].        Bas
+00001350: 6557 532e 5f5f 696e 6974 5f5f 2873 656c  eWS.__init__(sel
+00001360: 662c 2072 6569 6e74 656e 746f 7329 0a0a  f, reintentos)..
+00001370: 2020 2020 6465 6620 696e 6963 6961 6c69      def iniciali
+00001380: 7a61 7228 7365 6c66 293a 0a20 2020 2020  zar(self):.     
+00001390: 2020 2042 6173 6557 532e 696e 6963 6961     BaseWS.inicia
+000013a0: 6c69 7a61 7228 7365 6c66 290a 2020 2020  lizar(self).    
+000013b0: 2020 2020 7365 6c66 2e43 6f64 6967 6f54      self.CodigoT
+000013c0: 7261 6e73 6163 6369 6f6e 203d 2073 656c  ransaccion = sel
+000013d0: 662e 4572 726f 7265 7320 3d20 7365 6c66  f.Errores = self
+000013e0: 2e52 6573 756c 7461 646f 203d 204e 6f6e  .Resultado = Non
+000013f0: 650a 2020 2020 2020 2020 7365 6c66 2e52  e.        self.R
+00001400: 6573 756c 7461 646f 203d 2027 270a 2020  esultado = ''.  
+00001410: 2020 2020 2020 7365 6c66 2e45 7272 6f72        self.Error
+00001420: 6573 203d 205b 5d20 2020 2320 6c69 7374  es = []   # list
+00001430: 6120 6465 2073 7472 696e 6773 2070 6172  a de strings par
+00001440: 6120 6c61 2069 6e74 6572 6661 7a0a 2020  a la interfaz.  
+00001450: 2020 2020 2020 7365 6c66 2e65 7272 6f72        self.error
+00001460: 6573 203d 205b 5d20 2020 2320 6c69 7374  es = []   # list
+00001470: 6120 6465 2064 6963 6369 6f6e 6172 696f  a de diccionario
+00001480: 7320 2875 736f 2069 6e74 6572 6e6f 290a  s (uso interno).
+00001490: 2020 2020 2020 2020 7365 6c66 2e43 616e          self.Can
+000014a0: 7450 6167 696e 6173 203d 2073 656c 662e  tPaginas = self.
+000014b0: 4861 7945 7272 6f72 203d 204e 6f6e 650a  HayError = None.
+000014c0: 0a20 2020 2064 6566 205f 5f61 6e61 6c69  .    def __anali
+000014d0: 7a61 725f 6572 726f 7265 7328 7365 6c66  zar_errores(self
+000014e0: 2c20 7265 7429 3a0a 2020 2020 2020 2020  , ret):.        
+000014f0: 2243 6f6d 7072 7565 6261 2079 2065 7874  "Comprueba y ext
+00001500: 7261 6520 6572 726f 7265 7320 7369 2065  rae errores si e
+00001510: 7869 7374 656e 2065 6e20 6c61 2072 6573  xisten en la res
+00001520: 7075 6573 7461 2058 4d4c 220a 2020 2020  puesta XML".    
+00001530: 2020 2020 7365 6c66 2e65 7272 6f72 6573      self.errores
+00001540: 203d 2072 6574 2e67 6574 2827 6572 726f   = ret.get('erro
+00001550: 7265 7327 2c20 5b5d 290a 2020 2020 2020  res', []).      
+00001560: 2020 7365 6c66 2e45 7272 6f72 6573 203d    self.Errores =
+00001570: 205b 2225 733a 2025 7322 2025 2028 6974   ["%s: %s" % (it
+00001580: 5b27 635f 6572 726f 7227 5d2c 2069 745b  ['c_error'], it[
+00001590: 2764 5f65 7272 6f72 275d 290a 2020 2020  'd_error']).    
+000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015b0: 2020 2020 666f 7220 6974 2069 6e20 7265      for it in re
+000015c0: 742e 6765 7428 2765 7272 6f72 6573 272c  t.get('errores',
+000015d0: 205b 5d29 5d0a 2020 2020 2020 2020 7365   [])].        se
+000015e0: 6c66 2e52 6573 756c 7461 646f 203d 2072  lf.Resultado = r
+000015f0: 6574 2e67 6574 2827 7265 7375 6c74 6164  et.get('resultad
+00001600: 6f27 290a 0a20 2020 2064 6566 2043 6f6e  o')..    def Con
+00001610: 6563 7461 7228 7365 6c66 2c20 6361 6368  ectar(self, cach
+00001620: 653d 4e6f 6e65 2c20 7773 646c 3d4e 6f6e  e=None, wsdl=Non
+00001630: 652c 2070 726f 7879 3d22 222c 2077 7261  e, proxy="", wra
+00001640: 7070 6572 3d4e 6f6e 652c 2063 6163 6572  pper=None, cacer
+00001650: 743d 4e6f 6e65 2c20 7469 6d65 6f75 743d  t=None, timeout=
+00001660: 3330 293a 0a20 2020 2020 2020 2023 2043  30):.        # C
+00001670: 6f6e 6563 746f 2075 7361 6e64 6f20 656c  onecto usando el
+00001680: 206d e974 6f64 6f20 6573 7461 6e64 6172   m.todo estandar
+00001690: 643a 0a20 2020 2020 2020 206f 6b20 3d20  d:.        ok = 
+000016a0: 4261 7365 5753 2e43 6f6e 6563 7461 7228  BaseWS.Conectar(
+000016b0: 7365 6c66 2c20 6361 6368 652c 2077 7364  self, cache, wsd
+000016c0: 6c2c 2070 726f 7879 2c20 7772 6170 7065  l, proxy, wrappe
+000016d0: 722c 2063 6163 6572 742c 2074 696d 656f  r, cacert, timeo
+000016e0: 7574 2c0a 2020 2020 2020 2020 2020 2020  ut,.            
+000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001700: 2020 736f 6170 5f73 6572 7665 723d 226a    soap_server="j
+00001710: 6574 7479 2229 0a20 2020 2020 2020 2069  etty").        i
+00001720: 6620 6f6b 3a0a 2020 2020 2020 2020 2020  f ok:.          
+00001730: 2020 2320 7369 2065 6c20 6172 6368 6976    # si el archiv
+00001740: 6f20 6573 206c 6f63 616c 2c20 6173 756d  o es local, asum
+00001750: 6f20 7175 6520 7961 2065 7374 6120 636f  o que ya esta co
+00001760: 7272 6567 6964 6f3a 0a20 2020 2020 2020  rregido:.       
+00001770: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00001780: 2e77 7364 6c2e 7374 6172 7473 7769 7468  .wsdl.startswith
+00001790: 2822 6669 6c65 2229 3a0a 2020 2020 2020  ("file"):.      
+000017a0: 2020 2020 2020 2020 2020 2320 636f 7272            # corr
+000017b0: 696a 6f20 7562 6963 6163 69f3 6e20 6465  ijo ubicaci.n de
+000017c0: 6c20 7365 7276 6964 6f72 2028 6c6f 6361  l servidor (loca
+000017d0: 6c68 6f73 743a 3930 3530 2065 6e20 656c  lhost:9050 en el
+000017e0: 2057 5344 4c29 0a20 2020 2020 2020 2020   WSDL).         
+000017f0: 2020 2020 2020 206c 6f63 6174 696f 6e20         location 
+00001800: 3d20 7365 6c66 2e77 7364 6c5b 3a2d 355d  = self.wsdl[:-5]
+00001810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001820: 2077 7320 3d20 7365 6c66 2e63 6c69 656e   ws = self.clien
+00001830: 742e 7365 7276 6963 6573 5b27 4957 6562  t.services['IWeb
+00001840: 5365 7276 6963 6553 656e 6173 6127 5d0a  ServiceSenasa'].
+00001850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001860: 7773 5b27 706f 7274 7327 5d5b 2749 5765  ws['ports']['IWe
+00001870: 6253 6572 7669 6365 5365 6e61 7361 506f  bServiceSenasaPo
+00001880: 7274 275d 5b27 6c6f 6361 7469 6f6e 275d  rt']['location']
+00001890: 203d 206c 6f63 6174 696f 6e0a 0a20 2020   = location..   
+000018a0: 2020 2020 2020 2020 2023 2045 7374 6162           # Estab
+000018b0: 6c65 6365 7220 6372 6564 656e 6369 616c  lecer credencial
+000018c0: 6573 2064 6520 7365 6775 7269 6461 643a  es de seguridad:
+000018d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000018e0: 662e 636c 6965 6e74 5b27 7773 7365 3a53  f.client['wsse:S
+000018f0: 6563 7572 6974 7927 5d20 3d20 7b0a 2020  ecurity'] = {.  
+00001900: 2020 2020 2020 2020 2020 2020 2020 2777                'w
+00001910: 7373 653a 5573 6572 6e61 6d65 546f 6b65  sse:UsernameToke
+00001920: 6e27 3a20 7b0a 2020 2020 2020 2020 2020  n': {.          
+00001930: 2020 2020 2020 2020 2020 2777 7373 653a            'wsse:
+00001940: 5573 6572 6e61 6d65 273a 2073 656c 662e  Username': self.
+00001950: 5573 6572 6e61 6d65 2c0a 2020 2020 2020  Username,.      
+00001960: 2020 2020 2020 2020 2020 2020 2020 2777                'w
+00001970: 7373 653a 5061 7373 776f 7264 273a 2073  sse:Password': s
+00001980: 656c 662e 5061 7373 776f 7264 2c0a 2020  elf.Password,.  
+00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019a0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+000019b0: 2020 2020 7d0a 2020 2020 2020 2020 7265      }.        re
+000019c0: 7475 726e 206f 6b0a 0a20 2020 2040 696e  turn ok..    @in
+000019d0: 6963 6961 6c69 7a61 725f 795f 6361 7074  icializar_y_capt
+000019e0: 7572 6172 5f65 7863 6570 6369 6f6e 6573  urar_excepciones
+000019f0: 0a20 2020 2064 6566 2053 6176 6554 7261  .    def SaveTra
+00001a00: 6e73 6163 6369 6f6e 2873 656c 662c 2075  nsaccion(self, u
+00001a10: 7375 6172 696f 2c20 7061 7373 776f 7264  suario, password
+00001a20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001a30: 2020 2020 2020 2020 2020 676c 6e5f 6f72            gln_or
+00001a40: 6967 656e 3d4e 6f6e 652c 2067 6c6e 5f64  igen=None, gln_d
+00001a50: 6573 7469 6e6f 3d4e 6f6e 652c 0a20 2020  estino=None,.   
+00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a70: 2020 2020 2066 5f6f 7065 7261 6369 6f6e       f_operacion
+00001a80: 3d4e 6f6e 652c 2066 5f65 6c61 626f 7261  =None, f_elabora
+00001a90: 6369 6f6e 3d4e 6f6e 652c 2066 5f76 746f  cion=None, f_vto
+00001aa0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+00001ab0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00001ac0: 645f 6576 656e 746f 3d4e 6f6e 652c 2063  d_evento=None, c
+00001ad0: 6f64 5f70 726f 6475 6374 6f3d 4e6f 6e65  od_producto=None
+00001ae0: 2c20 6e5f 6361 6e74 6964 6164 3d4e 6f6e  , n_cantidad=Non
+00001af0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00001b00: 2020 2020 2020 2020 2020 206e 5f73 6572             n_ser
+00001b10: 6965 3d4e 6f6e 652c 206e 5f6c 6f74 653d  ie=None, n_lote=
+00001b20: 4e6f 6e65 2c20 6e5f 6361 693d 4e6f 6e65  None, n_cai=None
+00001b30: 2c20 6e5f 6361 653d 4e6f 6e65 2c0a 2020  , n_cae=None,.  
+00001b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b50: 2020 2020 2020 6964 5f6d 6f74 6976 6f5f        id_motivo_
+00001b60: 6465 7374 7275 6363 696f 6e3d 4e6f 6e65  destruccion=None
+00001b70: 2c20 6e5f 6d61 6e69 6669 6573 746f 3d4e  , n_manifiesto=N
+00001b80: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00001b90: 2020 2020 2020 2020 2020 2020 2065 6e5f               en_
+00001ba0: 7472 616e 7370 6f72 7465 3d4e 6f6e 652c  transporte=None,
+00001bb0: 206e 5f72 656d 6974 6f3d 4e6f 6e65 2c0a   n_remito=None,.
+00001bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bd0: 2020 2020 2020 2020 6d6f 7469 766f 5f64          motivo_d
+00001be0: 6576 6f6c 7563 696f 6e3d 4e6f 6e65 2c20  evolucion=None, 
+00001bf0: 6f62 7365 7276 6163 696f 6e65 733d 4e6f  observaciones=No
+00001c00: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00001c10: 2020 2020 2020 2020 2020 2020 6e5f 7661              n_va
+00001c20: 6c65 5f63 6f6d 7072 613d 4e6f 6e65 2c20  le_compra=None, 
+00001c30: 6170 656c 6c69 646f 4e6f 6d62 7265 733d  apellidoNombres=
+00001c40: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00001c50: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00001c60: 7265 6363 696f 6e3d 4e6f 6e65 2c20 6e75  reccion=None, nu
+00001c70: 6d65 726f 3d4e 6f6e 652c 206c 6f63 616c  mero=None, local
+00001c80: 6964 6164 3d4e 6f6e 652c 0a20 2020 2020  idad=None,.     
+00001c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ca0: 2020 2070 726f 7669 6e63 6961 3d4e 6f6e     provincia=Non
+00001cb0: 652c 206e 5f70 6f73 7461 6c3d 4e6f 6e65  e, n_postal=None
+00001cc0: 2c20 6375 6974 3d4e 6f6e 650a 2020 2020  , cuit=None.    
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ce0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+00001cf0: 2252 6561 6c69 7a61 2065 6c20 7265 6769  "Realiza el regi
+00001d00: 7374 726f 2064 6520 756e 6120 7472 616e  stro de una tran
+00001d10: 7361 6363 69f3 6e20 6465 2070 726f 6475  sacci.n de produ
+00001d20: 6374 6f73 2066 6974 6f73 616e 6974 6172  ctos fitosanitar
+00001d30: 696f 732e 2022 0a20 2020 2020 2020 2023  ios. ".        #
+00001d40: 2063 7265 6f20 6c6f 7320 7061 72e1 6d65   creo los par.me
+00001d50: 7472 6f73 2070 6172 6120 6573 7461 206c  tros para esta l
+00001d60: 6c61 6d61 6461 0a20 2020 2020 2020 2070  lamada.        p
+00001d70: 6172 616d 7320 3d20 7b20 2027 676c 6e5f  arams = {  'gln_
+00001d80: 6f72 6967 656e 273a 2067 6c6e 5f6f 7269  origen': gln_ori
+00001d90: 6765 6e2c 0a20 2020 2020 2020 2020 2020  gen,.           
+00001da0: 2020 2020 2020 2020 2027 676c 6e5f 6465           'gln_de
+00001db0: 7374 696e 6f27 3a20 676c 6e5f 6465 7374  stino': gln_dest
+00001dc0: 696e 6f2c 0a20 2020 2020 2020 2020 2020  ino,.           
+00001dd0: 2020 2020 2020 2020 2027 665f 6f70 6572           'f_oper
+00001de0: 6163 696f 6e27 3a20 665f 6f70 6572 6163  acion': f_operac
+00001df0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00001e00: 2020 2020 2020 2020 2027 665f 656c 6162           'f_elab
+00001e10: 6f72 6163 696f 6e27 3a20 665f 656c 6162  oracion': f_elab
+00001e20: 6f72 6163 696f 6e2c 0a20 2020 2020 2020  oracion,.       
+00001e30: 2020 2020 2020 2020 2020 2020 2027 665f               'f_
+00001e40: 7674 6f27 3a20 665f 7674 6f2c 0a20 2020  vto': f_vto,.   
+00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e60: 2027 6964 5f65 7665 6e74 6f27 3a20 6964   'id_evento': id
+00001e70: 5f65 7665 6e74 6f2c 0a20 2020 2020 2020  _evento,.       
+00001e80: 2020 2020 2020 2020 2020 2020 2027 636f               'co
+00001e90: 645f 7072 6f64 7563 746f 273a 2063 6f64  d_producto': cod
+00001ea0: 5f70 726f 6475 6374 6f2c 0a20 2020 2020  _producto,.     
+00001eb0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001ec0: 6e5f 6361 6e74 6964 6164 273a 206e 5f63  n_cantidad': n_c
+00001ed0: 616e 7469 6461 642c 0a20 2020 2020 2020  antidad,.       
+00001ee0: 2020 2020 2020 2020 2020 2020 2027 6e5f               'n_
+00001ef0: 7365 7269 6527 3a20 6e5f 7365 7269 652c  serie': n_serie,
+00001f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001f10: 2020 2020 2027 6e5f 6c6f 7465 273a 206e       'n_lote': n
+00001f20: 5f6c 6f74 652c 0a20 2020 2020 2020 2020  _lote,.         
+00001f30: 2020 2020 2020 2020 2020 2027 6e5f 6361             'n_ca
+00001f40: 6927 3a20 6e5f 6361 6920 6f72 204e 6f6e  i': n_cai or Non
+00001f50: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00001f60: 2020 2020 2020 2027 6e5f 6361 6527 3a20         'n_cae': 
+00001f70: 6e5f 6361 6520 6f72 204e 6f6e 652c 0a20  n_cae or None,. 
+00001f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f90: 2020 2027 6964 5f6d 6f74 6976 6f5f 6465     'id_motivo_de
+00001fa0: 7374 7275 6363 696f 6e27 3a20 6964 5f6d  struccion': id_m
+00001fb0: 6f74 6976 6f5f 6465 7374 7275 6363 696f  otivo_destruccio
+00001fc0: 6e20 6f72 204e 6f6e 652c 0a20 2020 2020  n or None,.     
+00001fd0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001fe0: 6e5f 6d61 6e69 6669 6573 746f 273a 206e  n_manifiesto': n
+00001ff0: 5f6d 616e 6966 6965 7374 6f20 6f72 204e  _manifiesto or N
+00002000: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00002010: 2020 2020 2020 2020 2027 656e 5f74 7261           'en_tra
+00002020: 6e73 706f 7274 6527 3a20 656e 5f74 7261  nsporte': en_tra
+00002030: 6e73 706f 7274 6520 6f72 204e 6f6e 652c  nsporte or None,
+00002040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002050: 2020 2020 2027 6e5f 7265 6d69 746f 273a       'n_remito':
+00002060: 206e 5f72 656d 6974 6f20 6f72 204e 6f6e   n_remito or Non
+00002070: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00002080: 2020 2020 2020 2027 6d6f 7469 766f 5f64         'motivo_d
+00002090: 6576 6f6c 7563 696f 6e27 3a20 6d6f 7469  evolucion': moti
+000020a0: 766f 5f64 6576 6f6c 7563 696f 6e20 6f72  vo_devolucion or
+000020b0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+000020c0: 2020 2020 2020 2020 2020 2027 6f62 7365             'obse
+000020d0: 7276 6163 696f 6e65 7327 3a20 6f62 7365  rvaciones': obse
+000020e0: 7276 6163 696f 6e65 7320 6f72 204e 6f6e  rvaciones or Non
+000020f0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00002100: 2020 2020 2020 2027 6e5f 7661 6c65 5f63         'n_vale_c
+00002110: 6f6d 7072 6127 3a20 6e5f 7661 6c65 5f63  ompra': n_vale_c
+00002120: 6f6d 7072 6120 6f72 204e 6f6e 652c 0a20  ompra or None,. 
+00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002140: 2020 2027 6170 656c 6c69 646f 4e6f 6d62     'apellidoNomb
+00002150: 7265 7327 3a20 6170 656c 6c69 646f 4e6f  res': apellidoNo
+00002160: 6d62 7265 7320 6f72 204e 6f6e 652c 0a20  mbres or None,. 
+00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002180: 2020 2027 6469 7265 6363 696f 6e27 3a20     'direccion': 
+00002190: 6469 7265 6363 696f 6e20 6f72 204e 6f6e  direccion or Non
+000021a0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000021b0: 2020 2020 2020 2027 6e75 6d65 726f 273a         'numero':
+000021c0: 206e 756d 6572 6f20 6f72 204e 6f6e 652c   numero or None,
+000021d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000021e0: 2020 2020 2027 6c6f 6361 6c69 6461 6427       'localidad'
+000021f0: 3a20 6c6f 6361 6c69 6461 6420 6f72 204e  : localidad or N
+00002200: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00002210: 2020 2020 2020 2020 2027 7072 6f76 696e           'provin
+00002220: 6369 6127 3a20 7072 6f76 696e 6369 6120  cia': provincia 
+00002230: 6f72 204e 6f6e 652c 0a20 2020 2020 2020  or None,.       
+00002240: 2020 2020 2020 2020 2020 2020 2027 6e5f               'n_
+00002250: 706f 7374 616c 273a 206e 5f70 6f73 7461  postal': n_posta
+00002260: 6c20 6f72 204e 6f6e 652c 0a20 2020 2020  l or None,.     
+00002270: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00002280: 6375 6974 273a 2063 7569 7420 6f72 204e  cuit': cuit or N
+00002290: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+000022a0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+000022b0: 2020 2072 6573 203d 2073 656c 662e 636c     res = self.cl
+000022c0: 6965 6e74 2e73 6176 6554 7261 6e73 6163  ient.saveTransac
+000022d0: 6369 6f6e 6573 280a 2020 2020 2020 2020  ciones(.        
+000022e0: 2020 2020 6172 6730 3d70 6172 616d 732c      arg0=params,
+000022f0: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
+00002300: 313d 7573 7561 7269 6f2c 0a20 2020 2020  1=usuario,.     
+00002310: 2020 2020 2020 2061 7267 323d 7061 7373         arg2=pass
+00002320: 776f 7264 2c0a 2020 2020 2020 2020 290a  word,.        ).
+00002330: 2020 2020 2020 2020 7265 7420 3d20 7265          ret = re
+00002340: 735b 2772 6574 7572 6e27 5d0a 2020 2020  s['return'].    
+00002350: 2020 2020 7365 6c66 2e43 6f64 6967 6f54      self.CodigoT
+00002360: 7261 6e73 6163 6369 6f6e 203d 2072 6574  ransaccion = ret
+00002370: 2e67 6574 2827 636f 6469 676f 5472 616e  .get('codigoTran
+00002380: 7361 6363 696f 6e27 290a 2020 2020 2020  saccion').      
+00002390: 2020 7365 6c66 2e5f 5f61 6e61 6c69 7a61    self.__analiza
+000023a0: 725f 6572 726f 7265 7328 7265 7429 0a20  r_errores(ret). 
+000023b0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+000023c0: 7565 0a0a 2020 2020 4069 6e69 6369 616c  ue..    @inicial
+000023d0: 697a 6172 5f79 5f63 6170 7475 7261 725f  izar_y_capturar_
+000023e0: 6578 6365 7063 696f 6e65 730a 2020 2020  excepciones.    
+000023f0: 6465 6620 5365 6e64 4361 6e63 656c 6154  def SendCancelaT
+00002400: 7261 6e73 6163 2873 656c 662c 2075 7375  ransac(self, usu
+00002410: 6172 696f 2c20 7061 7373 776f 7264 2c20  ario, password, 
+00002420: 636f 6469 676f 5f74 7261 6e73 6163 6369  codigo_transacci
+00002430: 6f6e 293a 0a20 2020 2020 2020 2022 2052  on):.        " R
+00002440: 6561 6c69 7a61 206c 6120 6361 6e63 656c  ealiza la cancel
+00002450: 6163 69f3 6e20 6465 2075 6e61 2074 7261  aci.n de una tra
+00002460: 6e73 6163 6369 f36e 220a 2020 2020 2020  nsacci.n".      
+00002470: 2020 7265 7320 3d20 7365 6c66 2e63 6c69    res = self.cli
+00002480: 656e 742e 7365 6e64 4361 6e63 656c 6154  ent.sendCancelaT
+00002490: 7261 6e73 6163 280a 2020 2020 2020 2020  ransac(.        
+000024a0: 2020 2020 6172 6730 3d63 6f64 6967 6f5f      arg0=codigo_
+000024b0: 7472 616e 7361 6363 696f 6e2c 0a20 2020  transaccion,.   
+000024c0: 2020 2020 2020 2020 2061 7267 313d 7573           arg1=us
+000024d0: 7561 7269 6f2c 0a20 2020 2020 2020 2020  uario,.         
+000024e0: 2020 2061 7267 323d 7061 7373 776f 7264     arg2=password
+000024f0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00002500: 2020 2020 7265 7420 3d20 7265 735b 2772      ret = res['r
+00002510: 6574 7572 6e27 5d0a 2020 2020 2020 2020  eturn'].        
+00002520: 7365 6c66 2e43 6f64 6967 6f54 7261 6e73  self.CodigoTrans
+00002530: 6163 6369 6f6e 203d 2072 6574 2e67 6574  accion = ret.get
+00002540: 2827 636f 6469 676f 5472 616e 7361 6363  ('codigoTransacc
+00002550: 696f 6e27 290a 2020 2020 2020 2020 7365  ion').        se
+00002560: 6c66 2e5f 5f61 6e61 6c69 7a61 725f 6572  lf.__analizar_er
+00002570: 726f 7265 7328 7265 7429 0a20 2020 2020  rores(ret).     
+00002580: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
+00002590: 2020 2020 4069 6e69 6369 616c 697a 6172      @inicializar
+000025a0: 5f79 5f63 6170 7475 7261 725f 6578 6365  _y_capturar_exce
+000025b0: 7063 696f 6e65 730a 2020 2020 6465 6620  pciones.    def 
+000025c0: 5365 6e64 436f 6e66 6972 6d61 5472 616e  SendConfirmaTran
+000025d0: 7361 6363 2873 656c 662c 2075 7375 6172  sacc(self, usuar
+000025e0: 696f 2c20 7061 7373 776f 7264 2c20 705f  io, password, p_
+000025f0: 6964 735f 7472 616e 7361 632c 2066 5f6f  ids_transac, f_o
+00002600: 7065 7261 6369 6f6e 2c20 6e5f 6361 6e74  peracion, n_cant
+00002610: 6964 6164 3d4e 6f6e 6529 3a0a 2020 2020  idad=None):.    
+00002620: 2020 2020 2243 6f6e 6669 726d 6120 6c61      "Confirma la
+00002630: 2072 6563 6570 6369 f36e 2064 6520 756e   recepci.n de un
+00002640: 206d 6564 6963 616d 656e 746f 220a 2020   medicamento".  
+00002650: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
+00002660: 2e63 6c69 656e 742e 7365 6e64 436f 6e66  .client.sendConf
+00002670: 6972 6d61 5472 616e 7361 6363 280a 2020  irmaTransacc(.  
+00002680: 2020 2020 2020 2020 2020 6172 6730 3d75            arg0=u
+00002690: 7375 6172 696f 2c0a 2020 2020 2020 2020  suario,.        
+000026a0: 2020 2020 6172 6731 3d70 6173 7377 6f72      arg1=passwor
+000026b0: 642c 0a20 2020 2020 2020 2020 2020 2061  d,.            a
+000026c0: 7267 323d 7b27 705f 6964 735f 7472 616e  rg2={'p_ids_tran
+000026d0: 7361 6327 3a20 705f 6964 735f 7472 616e  sac': p_ids_tran
+000026e0: 7361 632c 2027 665f 6f70 6572 6163 696f  sac, 'f_operacio
+000026f0: 6e27 3a20 665f 6f70 6572 6163 696f 6e2c  n': f_operacion,
+00002700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002710: 2020 2027 6e5f 6361 6e74 6964 6164 273a     'n_cantidad':
+00002720: 206e 5f63 616e 7469 6461 642c 0a20 2020   n_cantidad,.   
+00002730: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00002740: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00002750: 2020 2072 6574 203d 2072 6573 5b27 7265     ret = res['re
+00002760: 7475 726e 275d 0a20 2020 2020 2020 2073  turn'].        s
+00002770: 656c 662e 436f 6469 676f 5472 616e 7361  elf.CodigoTransa
+00002780: 6363 696f 6e20 3d20 7265 742e 6765 7428  ccion = ret.get(
+00002790: 2763 6f64 6967 6f54 7261 6e73 6163 6369  'codigoTransacci
+000027a0: 6f6e 2729 0a20 2020 2020 2020 2073 656c  on').        sel
+000027b0: 662e 5f5f 616e 616c 697a 6172 5f65 7272  f.__analizar_err
+000027c0: 6f72 6573 2872 6574 290a 2020 2020 2020  ores(ret).      
+000027d0: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
+000027e0: 2020 2040 696e 6963 6961 6c69 7a61 725f     @inicializar_
+000027f0: 795f 6361 7074 7572 6172 5f65 7863 6570  y_capturar_excep
+00002800: 6369 6f6e 6573 0a20 2020 2064 6566 2053  ciones.    def S
+00002810: 656e 6441 6c65 7274 6154 7261 6e73 6163  endAlertaTransac
+00002820: 6328 7365 6c66 2c20 7573 7561 7269 6f2c  c(self, usuario,
+00002830: 2070 6173 7377 6f72 642c 2070 5f69 6473   password, p_ids
+00002840: 5f74 7261 6e73 6163 5f77 7329 3a0a 2020  _transac_ws):.  
+00002850: 2020 2020 2020 2241 6c65 7274 6120 756e        "Alerta un
+00002860: 206d 6564 6963 616d 656e 746f 2c20 6163   medicamento, ac
+00002870: 6369 f36e 2063 6f6e 7472 6172 6961 2061  ci.n contraria a
+00002880: 2093 636f 6e66 6972 6d61 7220 6c61 2074   .confirmar la t
+00002890: 7261 6e73 6163 6369 f36e 942e 220a 2020  ransacci.n..".  
+000028a0: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
+000028b0: 2e63 6c69 656e 742e 7365 6e64 416c 6572  .client.sendAler
+000028c0: 7461 5472 616e 7361 6363 280a 2020 2020  taTransacc(.    
+000028d0: 2020 2020 2020 2020 6172 6730 3d75 7375          arg0=usu
+000028e0: 6172 696f 2c0a 2020 2020 2020 2020 2020  ario,.          
+000028f0: 2020 6172 6731 3d70 6173 7377 6f72 642c    arg1=password,
+00002900: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
+00002910: 323d 705f 6964 735f 7472 616e 7361 635f  2=p_ids_transac_
+00002920: 7773 2c0a 2020 2020 2020 2020 290a 2020  ws,.        ).  
+00002930: 2020 2020 2020 7265 7420 3d20 7265 735b        ret = res[
+00002940: 2772 6574 7572 6e27 5d0a 2020 2020 2020  'return'].      
+00002950: 2020 7365 6c66 2e43 6f64 6967 6f54 7261    self.CodigoTra
+00002960: 6e73 6163 6369 6f6e 203d 2072 6574 2e67  nsaccion = ret.g
+00002970: 6574 2827 6964 5f74 7261 6e73 6163 5f61  et('id_transac_a
+00002980: 736f 6369 6164 6127 290a 2020 2020 2020  sociada').      
+00002990: 2020 7365 6c66 2e5f 5f61 6e61 6c69 7a61    self.__analiza
+000029a0: 725f 6572 726f 7265 7328 7265 7429 0a20  r_errores(ret). 
+000029b0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+000029c0: 7565 0a0a 2020 2020 4069 6e69 6369 616c  ue..    @inicial
+000029d0: 697a 6172 5f79 5f63 6170 7475 7261 725f  izar_y_capturar_
+000029e0: 6578 6365 7063 696f 6e65 730a 2020 2020  excepciones.    
+000029f0: 6465 6620 4765 7454 7261 6e73 6163 6369  def GetTransacci
+00002a00: 6f6e 6573 2873 656c 662c 2075 7375 6172  ones(self, usuar
+00002a10: 696f 2c20 7061 7373 776f 7264 2c0a 2020  io, password,.  
+00002a20: 2020 2020 2020 2020 2020 2020 2020 6964                id
+00002a30: 5f74 7261 6e73 6163 6369 6f6e 3d4e 6f6e  _transaccion=Non
+00002a40: 652c 2069 645f 6576 656e 746f 3d4e 6f6e  e, id_evento=Non
+00002a50: 652c 2067 6c6e 5f6f 7269 6765 6e3d 4e6f  e, gln_origen=No
+00002a60: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00002a70: 2020 2020 6665 6368 615f 6465 7364 655f      fecha_desde_
+00002a80: 743d 4e6f 6e65 2c20 6665 6368 615f 6861  t=None, fecha_ha
+00002a90: 7374 615f 743d 4e6f 6e65 2c0a 2020 2020  sta_t=None,.    
+00002aa0: 2020 2020 2020 2020 2020 2020 6665 6368              fech
+00002ab0: 615f 6465 7364 655f 763d 4e6f 6e65 2c20  a_desde_v=None, 
+00002ac0: 6665 6368 615f 6861 7374 615f 763d 4e6f  fecha_hasta_v=No
+00002ad0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00002ae0: 2020 2020 676c 6e5f 696e 666f 726d 6164      gln_informad
+00002af0: 6f72 3d4e 6f6e 652c 2069 645f 7469 706f  or=None, id_tipo
+00002b00: 5f74 7261 6e73 6163 6369 6f6e 3d4e 6f6e  _transaccion=Non
+00002b10: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00002b20: 2020 2067 7469 6e5f 656c 656d 656e 746f     gtin_elemento
+00002b30: 3d4e 6f6e 652c 206e 5f6c 6f74 653d 4e6f  =None, n_lote=No
+00002b40: 6e65 2c20 6e5f 7365 7269 653d 4e6f 6e65  ne, n_serie=None
+00002b50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002b60: 2020 6e5f 7265 6d69 746f 5f66 6163 7475    n_remito_factu
+00002b70: 7261 3d4e 6f6e 652c 0a20 2020 2020 2020  ra=None,.       
+00002b80: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
+00002b90: 2020 2020 2254 7261 6520 756e 206c 6973      "Trae un lis
+00002ba0: 7461 646f 2064 6520 6c61 7320 7472 616e  tado de las tran
+00002bb0: 7361 6363 696f 6e65 7320 7175 6520 6e6f  sacciones que no
+00002bc0: 2065 7374 e16e 2063 6f6e 6669 726d 6164   est.n confirmad
+00002bd0: 6173 220a 0a20 2020 2020 2020 2023 2070  as"..        # p
+00002be0: 7265 7061 726f 206c 6f73 2070 6172 616d  reparo los param
+00002bf0: 6574 726f 7320 6465 2065 6e74 7261 6461  etros de entrada
+00002c00: 206f 7063 696f 6e61 6c65 733a 0a20 2020   opcionales:.   
+00002c10: 2020 2020 206b 7761 7267 7320 3d20 7b7d       kwargs = {}
+00002c20: 0a20 2020 2020 2020 2069 6620 6964 5f74  .        if id_t
+00002c30: 7261 6e73 6163 6369 6f6e 2069 7320 6e6f  ransaccion is no
+00002c40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00002c50: 2020 2020 6b77 6172 6773 5b27 6172 6732      kwargs['arg2
+00002c60: 275d 203d 2069 645f 7472 616e 7361 6363  '] = id_transacc
+00002c70: 696f 6e0a 2020 2020 2020 2020 6966 2069  ion.        if i
+00002c80: 645f 6576 656e 746f 2069 7320 6e6f 7420  d_evento is not 
+00002c90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00002ca0: 2020 6b77 6172 6773 5b27 6172 6733 275d    kwargs['arg3']
+00002cb0: 203d 2069 645f 6576 656e 746f 0a20 2020   = id_evento.   
+00002cc0: 2020 2020 2069 6620 676c 6e5f 6f72 6967       if gln_orig
+00002cd0: 656e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  en is not None:.
+00002ce0: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
+00002cf0: 6773 5b27 6172 6734 275d 203d 2067 6c6e  gs['arg4'] = gln
+00002d00: 5f6f 7269 6765 6e0a 2020 2020 2020 2020  _origen.        
+00002d10: 6966 2066 6563 6861 5f64 6573 6465 5f74  if fecha_desde_t
+00002d20: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00002d30: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
+00002d40: 5b27 6172 6735 275d 203d 2066 6563 6861  ['arg5'] = fecha
+00002d50: 5f64 6573 6465 5f74 0a20 2020 2020 2020  _desde_t.       
+00002d60: 2069 6620 6665 6368 615f 6861 7374 615f   if fecha_hasta_
+00002d70: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
+00002d80: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
+00002d90: 735b 2761 7267 3627 5d20 3d20 6665 6368  s['arg6'] = fech
+00002da0: 615f 6861 7374 615f 740a 2020 2020 2020  a_hasta_t.      
+00002db0: 2020 6966 2066 6563 6861 5f64 6573 6465    if fecha_desde
+00002dc0: 5f76 2069 7320 6e6f 7420 4e6f 6e65 3a0a  _v is not None:.
+00002dd0: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
+00002de0: 6773 5b27 6172 6737 275d 203d 2066 6563  gs['arg7'] = fec
+00002df0: 6861 5f64 6573 6465 5f76 0a20 2020 2020  ha_desde_v.     
+00002e00: 2020 2069 6620 6665 6368 615f 6861 7374     if fecha_hast
+00002e10: 615f 7620 6973 206e 6f74 204e 6f6e 653a  a_v is not None:
+00002e20: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
+00002e30: 7267 735b 2761 7267 3827 5d20 3d20 6665  rgs['arg8'] = fe
+00002e40: 6368 615f 6861 7374 615f 760a 2020 2020  cha_hasta_v.    
+00002e50: 2020 2020 6966 2067 6c6e 5f69 6e66 6f72      if gln_infor
+00002e60: 6d61 646f 7220 6973 206e 6f74 204e 6f6e  mador is not Non
+00002e70: 653a 0a20 2020 2020 2020 2020 2020 206b  e:.            k
+00002e80: 7761 7267 735b 2761 7267 3927 5d20 3d20  wargs['arg9'] = 
+00002e90: 676c 6e5f 696e 666f 726d 6164 6f72 0a20  gln_informador. 
+00002ea0: 2020 2020 2020 2069 6620 6964 5f74 6970         if id_tip
+00002eb0: 6f5f 7472 616e 7361 6363 696f 6e20 6973  o_transaccion is
+00002ec0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00002ed0: 2020 2020 2020 206b 7761 7267 735b 2761         kwargs['a
+00002ee0: 7267 3130 275d 203d 2069 645f 7469 706f  rg10'] = id_tipo
+00002ef0: 5f74 7261 6e73 6163 6369 6f6e 0a20 2020  _transaccion.   
+00002f00: 2020 2020 2069 6620 6774 696e 5f65 6c65       if gtin_ele
+00002f10: 6d65 6e74 6f20 6973 206e 6f74 204e 6f6e  mento is not Non
+00002f20: 653a 0a20 2020 2020 2020 2020 2020 206b  e:.            k
+00002f30: 7761 7267 735b 2761 7267 3131 275d 203d  wargs['arg11'] =
+00002f40: 2067 7469 6e5f 656c 656d 656e 746f 0a20   gtin_elemento. 
+00002f50: 2020 2020 2020 2069 6620 6e5f 6c6f 7465         if n_lote
+00002f60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00002f70: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
+00002f80: 5b27 6172 6731 3227 5d20 3d20 6e5f 6c6f  ['arg12'] = n_lo
+00002f90: 7465 0a20 2020 2020 2020 2069 6620 6e5f  te.        if n_
+00002fa0: 7365 7269 6520 6973 206e 6f74 204e 6f6e  serie is not Non
+00002fb0: 653a 0a20 2020 2020 2020 2020 2020 206b  e:.            k
+00002fc0: 7761 7267 735b 2761 7267 3133 275d 203d  wargs['arg13'] =
+00002fd0: 206e 5f73 6572 6965 0a20 2020 2020 2020   n_serie.       
+00002fe0: 2069 6620 6e5f 7265 6d69 746f 5f66 6163   if n_remito_fac
+00002ff0: 7475 7261 2069 7320 6e6f 7420 4e6f 6e65  tura is not None
+00003000: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
+00003010: 6172 6773 5b27 6172 6731 3427 5d20 3d20  args['arg14'] = 
+00003020: 6e5f 7265 6d69 746f 5f66 6163 7475 7261  n_remito_factura
+00003030: 0a0a 2020 2020 2020 2020 2320 6c6c 616d  ..        # llam
+00003040: 6f20 616c 2077 6562 7365 7276 6963 650a  o al webservice.
+00003050: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
+00003060: 6c66 2e63 6c69 656e 742e 6765 7454 7261  lf.client.getTra
+00003070: 6e73 6163 6369 6f6e 6573 280a 2020 2020  nsacciones(.    
+00003080: 2020 2020 2020 2020 6172 6730 3d75 7375          arg0=usu
+00003090: 6172 696f 2c0a 2020 2020 2020 2020 2020  ario,.          
+000030a0: 2020 6172 6731 3d70 6173 7377 6f72 642c    arg1=password,
+000030b0: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
+000030c0: 7761 7267 730a 2020 2020 2020 2020 290a  wargs.        ).
+000030d0: 2020 2020 2020 2020 7265 7420 3d20 7265          ret = re
+000030e0: 735b 2772 6574 7572 6e27 5d0a 2020 2020  s['return'].    
+000030f0: 2020 2020 6966 2072 6574 3a0a 2020 2020      if ret:.    
+00003100: 2020 2020 2020 2020 7365 6c66 2e5f 5f61          self.__a
+00003110: 6e61 6c69 7a61 725f 6572 726f 7265 7328  nalizar_errores(
+00003120: 7265 7429 0a20 2020 2020 2020 2020 2020  ret).           
+00003130: 2073 656c 662e 4361 6e74 5061 6769 6e61   self.CantPagina
+00003140: 7320 3d20 7265 742e 6765 7428 2763 616e  s = ret.get('can
+00003150: 7450 6167 696e 6173 2729 0a20 2020 2020  tPaginas').     
+00003160: 2020 2020 2020 2073 656c 662e 4861 7945         self.HayE
+00003170: 7272 6f72 203d 2072 6574 2e67 6574 2827  rror = ret.get('
+00003180: 6861 795f 6572 726f 7227 290a 2020 2020  hay_error').    
+00003190: 2020 2020 2020 2020 7365 6c66 2e54 7261          self.Tra
+000031a0: 6e73 6163 6369 6f6e 5365 6e61 7361 203d  nsaccionSenasa =
+000031b0: 205b 6974 2066 6f72 2069 7420 696e 2072   [it for it in r
+000031c0: 6574 2e67 6574 2827 6c69 7374 272c 205b  et.get('list', [
+000031d0: 5d29 5d0a 2020 2020 2020 2020 7265 7475  ])].        retu
+000031e0: 726e 2054 7275 650a 0a20 2020 2064 6566  rn True..    def
+000031f0: 2020 4c65 6572 5472 616e 7361 6363 696f    LeerTransaccio
+00003200: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
+00003210: 2022 5265 636f 7272 6f20 5472 616e 7361   "Recorro Transa
+00003220: 6363 696f 6e53 656e 6173 6120 6465 7675  ccionSenasa devu
+00003230: 656c 746f 2070 6f72 2047 6574 5472 616e  elto por GetTran
+00003240: 7361 6363 696f 6e65 7322 0a20 2020 2020  sacciones".     
+00003250: 2020 2020 2320 7573 6172 2047 6574 5061      # usar GetPa
+00003260: 7261 6d65 7472 6f20 7061 7261 2063 6f6e  rametro para con
+00003270: 7375 6c74 6172 2065 6c20 7661 6c6f 7220  sultar el valor 
+00003280: 7265 746f 726e 6164 6f20 706f 7220 656c  retornado por el
+00003290: 2077 6562 7365 7276 6963 650a 0a20 2020   webservice..   
+000032a0: 2020 2020 2069 6620 7365 6c66 2e54 7261       if self.Tra
+000032b0: 6e73 6163 6369 6f6e 5365 6e61 7361 3a0a  nsaccionSenasa:.
+000032c0: 2020 2020 2020 2020 2020 2020 2320 6578              # ex
+000032d0: 7472 6169 676f 2065 6c20 7072 696d 6572  traigo el primer
+000032e0: 2069 7465 6d0a 2020 2020 2020 2020 2020   item.          
+000032f0: 2020 7365 6c66 2e70 6172 616d 735f 6f75    self.params_ou
+00003300: 7420 3d20 7365 6c66 2e54 7261 6e73 6163  t = self.Transac
+00003310: 6369 6f6e 5365 6e61 7361 2e70 6f70 2830  cionSenasa.pop(0
+00003320: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00003330: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+00003340: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00003350: 2020 2020 2320 6c69 6d70 696f 206c 6f73      # limpio los
+00003360: 2070 6172 e16d 6574 726f 730a 2020 2020   par.metros.    
+00003370: 2020 2020 2020 2020 7365 6c66 2e70 6172          self.par
+00003380: 616d 735f 6f75 7420 3d20 7b7d 0a20 2020  ams_out = {}.   
+00003390: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000033a0: 4661 6c73 650a 0a20 2020 2064 6566 204c  False..    def L
+000033b0: 6565 7245 7272 6f72 2873 656c 6629 3a0a  eerError(self):.
+000033c0: 2020 2020 2020 2020 2252 6563 6f72 726f          "Recorro
+000033d0: 206c 6f73 2065 7272 6f72 6573 2064 6576   los errores dev
+000033e0: 7565 6c74 6f73 2079 2064 6576 7565 6c76  ueltos y devuelv
+000033f0: 6f20 656c 2070 7269 6d65 726f 2073 6920  o el primero si 
+00003400: 6578 6973 7465 220a 0a20 2020 2020 2020  existe"..       
+00003410: 2069 6620 7365 6c66 2e45 7272 6f72 6573   if self.Errores
+00003420: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00003430: 6578 7472 6169 676f 2065 6c20 7072 696d  extraigo el prim
+00003440: 6572 2069 7465 6d0a 2020 2020 2020 2020  er item.        
+00003450: 2020 2020 6572 203d 2073 656c 662e 4572      er = self.Er
+00003460: 726f 7265 732e 706f 7028 3029 0a20 2020  rores.pop(0).   
+00003470: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00003480: 6572 0a20 2020 2020 2020 2065 6c73 653a  er.        else:
+00003490: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000034a0: 7572 6e20 2222 0a0a 2020 2020 6465 6620  urn ""..    def 
+000034b0: 5365 7455 7365 726e 616d 6528 7365 6c66  SetUsername(self
+000034c0: 2c20 7573 6572 6e61 6d65 293a 0a20 2020  , username):.   
+000034d0: 2020 2020 2022 4573 7461 626c 657a 636f       "Establezco
+000034e0: 2065 6c20 6e6f 6d62 7265 2064 6520 7573   el nombre de us
+000034f0: 7561 7269 6f22 0a20 2020 2020 2020 2073  uario".        s
+00003500: 656c 662e 5573 6572 6e61 6d65 203d 2075  elf.Username = u
+00003510: 7365 726e 616d 650a 0a20 2020 2064 6566  sername..    def
+00003520: 2053 6574 5061 7373 776f 7264 2873 656c   SetPassword(sel
+00003530: 662c 2070 6173 7377 6f72 6429 3a0a 2020  f, password):.  
+00003540: 2020 2020 2020 2245 7374 6162 6c65 7a63        "Establezc
+00003550: 6f20 6c61 2063 6f6e 7472 6173 65f1 6122  o la contrase.a"
+00003560: 0a20 2020 2020 2020 2073 656c 662e 5061  .        self.Pa
+00003570: 7373 776f 7264 203d 2070 6173 7377 6f72  ssword = passwor
+00003580: 640a 0a20 2020 2064 6566 2047 6574 436f  d..    def GetCo
+00003590: 6469 676f 5472 616e 7361 6363 696f 6e28  digoTransaccion(
+000035a0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+000035b0: 4465 7675 656c 766f 2065 6c20 63f3 6469  Devuelvo el c.di
+000035c0: 676f 2064 6520 7472 616e 7361 6363 69f3  go de transacci.
+000035d0: 6e22 0a20 2020 2020 2020 2072 6574 7572  n".        retur
+000035e0: 6e20 7365 6c66 2e43 6f64 6967 6f54 7261  n self.CodigoTra
+000035f0: 6e73 6163 6369 6f6e 0a0a 2020 2020 6465  nsaccion..    de
+00003600: 6620 4765 7452 6573 756c 7461 646f 2873  f GetResultado(s
+00003610: 656c 6629 3a0a 2020 2020 2020 2020 2244  elf):.        "D
+00003620: 6576 7565 6c76 6f20 656c 2072 6573 756c  evuelvo el resul
+00003630: 7461 646f 220a 2020 2020 2020 2020 7265  tado".        re
+00003640: 7475 726e 2073 656c 662e 5265 7375 6c74  turn self.Result
+00003650: 6164 6f0a 0a0a 6465 6620 6d61 696e 2829  ado...def main()
+00003660: 3a0a 2020 2020 2246 756e 6369 f36e 2070  :.    "Funci.n p
+00003670: 7269 6e63 6970 616c 2064 6520 7072 7565  rincipal de prue
+00003680: 6261 7320 286f 6274 656e 6572 2043 4145  bas (obtener CAE
+00003690: 2922 0a20 2020 2069 6d70 6f72 7420 6f73  )".    import os
+000036a0: 2c20 7469 6d65 2c20 7379 730a 2020 2020  , time, sys.    
+000036b0: 676c 6f62 616c 2057 5344 4c2c 204c 4f43  global WSDL, LOC
+000036c0: 4154 494f 4e0a 0a20 2020 2044 4542 5547  ATION..    DEBUG
+000036d0: 203d 2027 2d2d 6465 6275 6727 2069 6e20   = '--debug' in 
+000036e0: 7379 732e 6172 6776 0a0a 2020 2020 7773  sys.argv..    ws
+000036f0: 203d 2054 7261 7a61 4669 746f 2829 0a0a   = TrazaFito()..
+00003700: 2020 2020 7773 2e55 7365 726e 616d 6520      ws.Username 
+00003710: 3d20 2774 6573 7477 7365 7276 6963 6527  = 'testwservice'
+00003720: 0a20 2020 2077 732e 5061 7373 776f 7264  .    ws.Password
+00003730: 203d 2027 7465 7374 7773 6572 7669 6365   = 'testwservice
+00003740: 7073 7727 0a0a 2020 2020 6966 2027 2d2d  psw'..    if '--
+00003750: 7072 6f64 2720 696e 2073 7973 2e61 7267  prod' in sys.arg
+00003760: 7620 616e 6420 6e6f 7420 484f 4d4f 3a0a  v and not HOMO:.
+00003770: 2020 2020 2020 2020 5753 444c 203d 2022          WSDL = "
+00003780: 6874 7470 733a 2f2f 7365 7276 6963 696f  https://servicio
+00003790: 732e 7061 6d69 2e6f 7267 2e61 722f 7472  s.pami.org.ar/tr
+000037a0: 617a 6161 6772 2e57 6562 5365 7276 6963  azaagr.WebServic
+000037b0: 653f 7773 646c 220a 2020 2020 2020 2020  e?wsdl".        
+000037c0: 7072 696e 7428 2255 7361 6e64 6f20 5753  print("Usando WS
+000037d0: 444c 3a22 2c20 5753 444c 290a 2020 2020  DL:", WSDL).    
+000037e0: 2020 2020 7379 732e 6172 6776 2e70 6f70      sys.argv.pop
+000037f0: 2873 7973 2e61 7267 762e 696e 6465 7828  (sys.argv.index(
+00003800: 222d 2d70 726f 6422 2929 0a0a 2020 2020  "--prod"))..    
+00003810: 2320 496e 6963 6961 6c69 7a6f 206c 6173  # Inicializo las
+00003820: 2076 6172 6961 626c 6573 2079 2065 7374   variables y est
+00003830: 7275 6374 7572 6173 2070 6172 6120 656c  ructuras para el
+00003840: 2061 7263 6869 766f 2064 6520 696e 7465   archivo de inte
+00003850: 7263 616d 6269 6f3a 0a20 2020 2074 7261  rcambio:.    tra
+00003860: 6e73 6163 6369 6f6e 5f64 746f 203d 205b  nsaccion_dto = [
+00003870: 5d0a 2020 2020 7472 616e 7361 6363 696f  ].    transaccio
+00003880: 6e65 7320 3d20 5b5d 0a20 2020 2065 7272  nes = [].    err
+00003890: 6f72 6573 203d 205b 5d0a 2020 2020 666f  ores = [].    fo
+000038a0: 726d 6174 6f73 203d 205b 2827 5472 616e  rmatos = [('Tran
+000038b0: 7361 6363 696f 6e44 544f 272c 2054 5241  saccionDTO', TRA
+000038c0: 4e53 4143 4349 4f4e 5f44 544f 2c20 7472  NSACCION_DTO, tr
+000038d0: 616e 7361 6363 696f 6e5f 6474 6f29 2c0a  ansaccion_dto),.
+000038e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038f0: 2827 5472 616e 7361 6363 696f 6e65 7327  ('Transacciones'
+00003900: 2c20 5452 414e 5341 4343 494f 4e45 532c  , TRANSACCIONES,
+00003910: 2074 7261 6e73 6163 6369 6f6e 6573 292c   transacciones),
+00003920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003930: 2028 2745 7272 6f72 6573 272c 2045 5252   ('Errores', ERR
+00003940: 4f52 4553 2c20 6572 726f 7265 7329 2c0a  ORES, errores),.
+00003950: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00003960: 0a0a 2020 2020 6966 2027 2d2d 666f 726d  ..    if '--form
+00003970: 6174 6f27 2069 6e20 7379 732e 6172 6776  ato' in sys.argv
+00003980: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+00003990: 2246 6f72 6d61 746f 3a22 290a 2020 2020  "Formato:").    
+000039a0: 2020 2020 666f 7220 6d73 672c 2066 6f72      for msg, for
+000039b0: 6d61 746f 2c20 6c69 7374 6120 696e 2066  mato, lista in f
+000039c0: 6f72 6d61 746f 733a 0a20 2020 2020 2020  ormatos:.       
+000039d0: 2020 2020 2063 6f6d 6965 6e7a 6f20 3d20       comienzo = 
+000039e0: 310a 2020 2020 2020 2020 2020 2020 7072  1.            pr
+000039f0: 696e 7428 223d 3d3d 2025 7320 3d3d 3d22  int("=== %s ==="
+00003a00: 2025 206d 7367 290a 2020 2020 2020 2020   % msg).        
+00003a10: 2020 2020 7072 696e 7428 227c 7c20 252d      print("|| %-
+00003a20: 3235 7320 7c7c 2025 2d31 3273 207c 7c20  25s || %-12s || 
+00003a30: 252d 3573 207c 7c20 252d 3473 207c 7c20  %-5s || %-4s || 
+00003a40: 252d 3130 7320 7c7c 2220 2520 280a 2020  %-10s ||" % (.  
+00003a50: 2020 2020 2020 2020 2020 2020 2020 224e                "N
+00003a60: 6f6d 6272 6522 2c20 2254 6970 6f22 2c20  ombre", "Tipo", 
+00003a70: 224c 6f6e 672e 222c 2022 506f 7328 7478  "Long.", "Pos(tx
+00003a80: 7429 222c 2022 4361 6d70 6f28 6462 6629  t)", "Campo(dbf)
+00003a90: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
+00003aa0: 636c 6176 6573 203d 205b 5d0a 2020 2020  claves = [].    
+00003ab0: 2020 2020 2020 2020 666f 7220 666d 7420          for fmt 
+00003ac0: 696e 2066 6f72 6d61 746f 3a0a 2020 2020  in formato:.    
+00003ad0: 2020 2020 2020 2020 2020 2020 636c 6176              clav
+00003ae0: 652c 206c 6f6e 6769 7475 642c 2074 6970  e, longitud, tip
+00003af0: 6f20 3d20 666d 745b 303a 335d 0a20 2020  o = fmt[0:3].   
+00003b00: 2020 2020 2020 2020 2020 2020 2063 6c61               cla
+00003b10: 7665 5f64 6266 203d 2064 6172 5f6e 6f6d  ve_dbf = dar_nom
+00003b20: 6272 655f 6361 6d70 6f5f 6462 6628 636c  bre_campo_dbf(cl
+00003b30: 6176 652c 2063 6c61 7665 7329 0a20 2020  ave, claves).   
+00003b40: 2020 2020 2020 2020 2020 2020 2063 6c61               cla
+00003b50: 7665 732e 6170 7065 6e64 2863 6c61 7665  ves.append(clave
+00003b60: 5f64 6266 290a 2020 2020 2020 2020 2020  _dbf).          
+00003b70: 2020 2020 2020 7072 696e 7428 227c 7c20        print("|| 
+00003b80: 252d 3235 7320 7c7c 2025 2d31 3273 207c  %-25s || %-12s |
+00003b90: 7c20 2535 6420 7c7c 2020 2025 3464 2020  | %5d ||   %4d  
+00003ba0: 207c 7c20 252d 3130 7320 7c7c 2220 2520   || %-10s ||" % 
+00003bb0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00003bc0: 2020 2020 2020 636c 6176 652c 2074 6970        clave, tip
+00003bd0: 6f2c 206c 6f6e 6769 7475 642c 2063 6f6d  o, longitud, com
+00003be0: 6965 6e7a 6f2c 2063 6c61 7665 5f64 6266  ienzo, clave_dbf
+00003bf0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00003c00: 2020 2063 6f6d 6965 6e7a 6f20 2b3d 206c     comienzo += l
+00003c10: 6f6e 6769 7475 640a 2020 2020 2020 2020  ongitud.        
+00003c20: 7379 732e 6578 6974 2830 290a 0a20 2020  sys.exit(0)..   
+00003c30: 2069 6620 272d 2d63 6172 6761 7227 2069   if '--cargar' i
+00003c40: 6e20 7379 732e 6172 6776 3a0a 2020 2020  n sys.argv:.    
+00003c50: 2020 2020 6966 2027 2d2d 6462 6627 2069      if '--dbf' i
+00003c60: 6e20 7379 732e 6172 6776 3a0a 2020 2020  n sys.argv:.    
+00003c70: 2020 2020 2020 2020 6c65 6572 5f64 6266          leer_dbf
+00003c80: 2866 6f72 6d61 746f 735b 3a31 5d2c 207b  (formatos[:1], {
+00003c90: 7d29 0a20 2020 2020 2020 2065 6c69 6620  }).        elif 
+00003ca0: 272d 2d6a 736f 6e27 2069 6e20 7379 732e  '--json' in sys.
+00003cb0: 6172 6776 3a0a 2020 2020 2020 2020 2020  argv:.          
+00003cc0: 2020 666f 7220 666f 726d 6174 6f20 696e    for formato in
+00003cd0: 2066 6f72 6d61 746f 735b 3a31 5d3a 0a20   formatos[:1]:. 
+00003ce0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00003cf0: 7263 6869 766f 203d 206f 7065 6e28 666f  rchivo = open(fo
+00003d00: 726d 6174 6f5b 305d 2e6c 6f77 6572 2829  rmato[0].lower()
+00003d10: 202b 2022 2e6a 736f 6e22 2c20 2272 2229   + ".json", "r")
+00003d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003d30: 2064 203d 206a 736f 6e2e 6c6f 6164 2861   d = json.load(a
+00003d40: 7263 6869 766f 290a 2020 2020 2020 2020  rchivo).        
+00003d50: 2020 2020 2020 2020 666f 726d 6174 6f5b          formato[
+00003d60: 325d 2e65 7874 656e 6428 6429 0a20 2020  2].extend(d).   
+00003d70: 2020 2020 2020 2020 2020 2020 2061 7263               arc
+00003d80: 6869 766f 2e63 6c6f 7365 2829 0a20 2020  hivo.close().   
+00003d90: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00003da0: 2020 2020 2020 2066 6f72 2066 6f72 6d61         for forma
+00003db0: 746f 2069 6e20 666f 726d 6174 6f73 5b3a  to in formatos[:
+00003dc0: 315d 3a0a 2020 2020 2020 2020 2020 2020  1]:.            
+00003dd0: 2020 2020 6172 6368 6976 6f20 3d20 6f70      archivo = op
+00003de0: 656e 2866 6f72 6d61 746f 5b30 5d2e 6c6f  en(formato[0].lo
+00003df0: 7765 7228 2920 2b20 222e 7478 7422 2c20  wer() + ".txt", 
+00003e00: 2272 2229 0a20 2020 2020 2020 2020 2020  "r").           
+00003e10: 2020 2020 2066 6f72 206c 696e 6561 2069       for linea i
+00003e20: 6e20 6172 6368 6976 6f3a 0a20 2020 2020  n archivo:.     
+00003e30: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00003e40: 203d 206c 6565 7228 6c69 6e65 612c 2066   = leer(linea, f
+00003e50: 6f72 6d61 746f 5b31 5d29 0a20 2020 2020  ormato[1]).     
+00003e60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00003e70: 6f72 6d61 746f 5b32 5d2e 6170 7065 6e64  ormato[2].append
+00003e80: 2864 290a 2020 2020 2020 2020 2020 2020  (d).            
+00003e90: 2020 2020 6172 6368 6976 6f2e 636c 6f73      archivo.clos
+00003ea0: 6528 290a 0a20 2020 2077 732e 436f 6e65  e()..    ws.Cone
+00003eb0: 6374 6172 2822 222c 2057 5344 4c29 0a0a  ctar("", WSDL)..
+00003ec0: 2020 2020 6966 2077 732e 4578 6365 7063      if ws.Excepc
+00003ed0: 696f 6e3a 0a20 2020 2020 2020 2070 7269  ion:.        pri
+00003ee0: 6e74 2877 732e 4578 6365 7063 696f 6e29  nt(ws.Excepcion)
+00003ef0: 0a20 2020 2020 2020 2070 7269 6e74 2877  .        print(w
+00003f00: 732e 5472 6163 6562 6163 6b29 0a20 2020  s.Traceback).   
+00003f10: 2020 2020 2073 7973 2e65 7869 7428 2d31       sys.exit(-1
+00003f20: 290a 0a20 2020 2023 2044 6174 6f73 2064  )..    # Datos d
+00003f30: 6520 7072 7565 6261 733a 0a0a 2020 2020  e pruebas:..    
+00003f40: 6966 2027 2d2d 7465 7374 2720 696e 2073  if '--test' in s
+00003f50: 7973 2e61 7267 763a 0a20 2020 2020 2020  ys.argv:.       
+00003f60: 2074 7261 6e73 6163 6369 6f6e 5f64 746f   transaccion_dto
+00003f70: 2e61 7070 656e 6428 6469 6374 280a 2020  .append(dict(.  
+00003f80: 2020 2020 2020 2020 2020 676c 6e5f 6f72            gln_or
+00003f90: 6967 656e 3d22 3938 3736 3534 3332 3130  igen="9876543210
+00003fa0: 3938 3222 2c20 676c 6e5f 6465 7374 696e  982", gln_destin
+00003fb0: 6f3d 2233 3639 3235 3831 3437 3336 3933  o="3692581473693
+00003fc0: 222c 0a20 2020 2020 2020 2020 2020 2066  ",.            f
+00003fd0: 5f6f 7065 7261 6369 6f6e 3d64 6174 6574  _operacion=datet
+00003fe0: 696d 652e 6461 7465 7469 6d65 2e6e 6f77  ime.datetime.now
+00003ff0: 2829 2e73 7472 6674 696d 6528 2225 642f  ().strftime("%d/
+00004000: 256d 2f25 5922 292c 0a20 2020 2020 2020  %m/%Y"),.       
+00004010: 2020 2020 2066 5f65 6c61 626f 7261 6369       f_elaboraci
+00004020: 6f6e 3d64 6174 6574 696d 652e 6461 7465  on=datetime.date
+00004030: 7469 6d65 2e6e 6f77 2829 2e73 7472 6674  time.now().strft
+00004040: 696d 6528 2225 642f 256d 2f25 5922 292c  ime("%d/%m/%Y"),
+00004050: 0a20 2020 2020 2020 2020 2020 2066 5f76  .            f_v
+00004060: 746f 3d28 6461 7465 7469 6d65 2e64 6174  to=(datetime.dat
+00004070: 6574 696d 652e 6e6f 7728 292b 6461 7465  etime.now()+date
+00004080: 7469 6d65 2e74 696d 6564 656c 7461 2833  time.timedelta(3
+00004090: 3029 292e 7374 7266 7469 6d65 2822 2564  0)).strftime("%d
+000040a0: 2f25 6d2f 2559 2229 2c0a 2020 2020 2020  /%m/%Y"),.      
+000040b0: 2020 2020 2020 6964 5f65 7665 6e74 6f3d        id_evento=
+000040c0: 3131 2c0a 2020 2020 2020 2020 2020 2020  11,.            
+000040d0: 636f 645f 7072 6f64 7563 746f 3d22 3838  cod_producto="88
+000040e0: 3930 3030 3030 3030 3030 3031 222c 0a20  900000000001",. 
+000040f0: 2020 2020 2020 2020 2020 206e 5f63 616e             n_can
+00004100: 7469 6461 643d 312c 0a20 2020 2020 2020  tidad=1,.       
+00004110: 2020 2020 206e 5f73 6572 6965 3d69 6e74       n_serie=int
+00004120: 2874 696d 652e 7469 6d65 2829 2a31 3029  (time.time()*10)
+00004130: 2c0a 2020 2020 2020 2020 2020 2020 6e5f  ,.            n_
+00004140: 6c6f 7465 3d64 6174 6574 696d 652e 6461  lote=datetime.da
+00004150: 7465 7469 6d65 2e6e 6f77 2829 2e73 7472  tetime.now().str
+00004160: 6674 696d 6528 2225 5922 292c 0a20 2020  ftime("%Y"),.   
+00004170: 2020 2020 2020 2020 206e 5f63 6169 3d22           n_cai="
+00004180: 3132 3334 3536 3738 3930 3132 3334 3522  123456789012345"
+00004190: 2c0a 2020 2020 2020 2020 2020 2020 6e5f  ,.            n_
+000041a0: 6361 653d 2222 2c0a 2020 2020 2020 2020  cae="",.        
+000041b0: 2020 2020 6964 5f6d 6f74 6976 6f5f 6465      id_motivo_de
+000041c0: 7374 7275 6363 696f 6e3d 302c 0a20 2020  struccion=0,.   
+000041d0: 2020 2020 2020 2020 206e 5f6d 616e 6966           n_manif
+000041e0: 6965 7374 6f3d 2222 2c0a 2020 2020 2020  iesto="",.      
+000041f0: 2020 2020 2020 656e 5f74 7261 6e73 706f        en_transpo
+00004200: 7274 653d 224e 222c 0a20 2020 2020 2020  rte="N",.       
+00004210: 2020 2020 206e 5f72 656d 6974 6f3d 2231       n_remito="1
+00004220: 3233 3422 2c0a 2020 2020 2020 2020 2020  234",.          
+00004230: 2020 6d6f 7469 766f 5f64 6576 6f6c 7563    motivo_devoluc
+00004240: 696f 6e3d 2222 2c0a 2020 2020 2020 2020  ion="",.        
+00004250: 2020 2020 6f62 7365 7276 6163 696f 6e65      observacione
+00004260: 733d 2270 7275 6562 6122 2c0a 2020 2020  s="prueba",.    
+00004270: 2020 2020 2020 2020 6e5f 7661 6c65 5f63          n_vale_c
+00004280: 6f6d 7072 613d 2222 2c0a 2020 2020 2020  ompra="",.      
+00004290: 2020 2020 2020 6170 656c 6c69 646f 4e6f        apellidoNo
+000042a0: 6d62 7265 733d 224a 7561 6e20 5065 7265  mbres="Juan Pere
+000042b0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+000042c0: 6469 7265 6363 696f 6e3d 2253 6172 617a  direccion="Saraz
+000042d0: 6122 2c20 6e75 6d65 726f 3d22 3132 3334  a", numero="1234
+000042e0: 222c 0a20 2020 2020 2020 2020 2020 206c  ",.            l
+000042f0: 6f63 616c 6964 6164 3d22 4875 726c 696e  ocalidad="Hurlin
+00004300: 6768 616d 222c 2070 726f 7669 6e63 6961  gham", provincia
+00004310: 3d22 4275 656e 6f73 2041 6972 6573 222c  ="Buenos Aires",
+00004320: 0a20 2020 2020 2020 2020 2020 206e 5f70  .            n_p
+00004330: 6f73 7461 6c3d 2231 3638 3822 2c0a 2020  ostal="1688",.  
+00004340: 2020 2020 2020 2020 2020 6375 6974 3d22            cuit="
+00004350: 3230 3236 3735 3635 3339 3322 2c0a 2020  20267565393",.  
+00004360: 2020 2020 2020 2020 2020 636f 6469 676f            codigo
+00004370: 5f74 7261 6e73 6163 6369 6f6e 3d4e 6f6e  _transaccion=Non
+00004380: 652c 0a20 2020 2020 2020 2029 290a 0a20  e,.        )).. 
+00004390: 2020 2023 204f 7063 696f 6e65 7320 7072     # Opciones pr
+000043a0: 696e 6369 7061 6c65 733a 0a0a 2020 2020  incipales:..    
+000043b0: 6966 2027 2d2d 636f 6e66 6972 6d61 2720  if '--confirma' 
+000043c0: 696e 2073 7973 2e61 7267 763a 0a20 2020  in sys.argv:.   
+000043d0: 2020 2020 2069 6620 272d 2d6c 6f61 6478       if '--loadx
+000043e0: 6d6c 2720 696e 2073 7973 2e61 7267 763a  ml' in sys.argv:
+000043f0: 0a20 2020 2020 2020 2020 2020 2077 732e  .            ws.
+00004400: 4c6f 6164 5465 7374 584d 4c28 2274 7261  LoadTestXML("tra
+00004410: 7a61 6d65 645f 636f 6e66 6972 6d61 2e78  zamed_confirma.x
+00004420: 6d6c 2229 2020 2320 6361 7267 6f20 7265  ml")  # cargo re
+00004430: 7370 7565 7374 610a 2020 2020 2020 2020  spuesta.        
+00004440: 2020 2020 6f6b 203d 2077 732e 5365 6e64      ok = ws.Send
+00004450: 436f 6e66 6972 6d61 5472 616e 7361 6363  ConfirmaTransacc
+00004460: 2875 7375 6172 696f 3d22 7072 7565 6261  (usuario="prueba
+00004470: 7377 7322 2c20 7061 7373 776f 7264 3d22  sws", password="
+00004480: 7072 7565 6261 7377 7322 2c0a 2020 2020  pruebasws",.    
+00004490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000044b0: 5f69 6473 5f74 7261 6e73 6163 3d22 3122  _ids_transac="1"
+000044c0: 2c20 665f 6f70 6572 6163 696f 6e3d 2233  , f_operacion="3
+000044d0: 312d 3132 2d32 3031 3322 290a 2020 2020  1-12-2013").    
+000044e0: 2020 2020 2020 2020 6966 206e 6f74 206f          if not o
+000044f0: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
+00004500: 2020 2072 6169 7365 2052 756e 7469 6d65     raise Runtime
+00004510: 4572 726f 7228 7773 2e45 7863 6570 6369  Error(ws.Excepci
+00004520: 6f6e 290a 2020 2020 2020 2020 7773 2e53  on).        ws.S
+00004530: 656e 6443 6f6e 6669 726d 6154 7261 6e73  endConfirmaTrans
+00004540: 6163 6328 2a73 7973 2e61 7267 765b 7379  acc(*sys.argv[sy
+00004550: 732e 6172 6776 2e69 6e64 6578 2822 2d2d  s.argv.index("--
+00004560: 636f 6e66 6972 6d61 2229 2b31 3a5d 290a  confirma")+1:]).
+00004570: 2020 2020 656c 6966 2027 2d2d 616c 6572      elif '--aler
+00004580: 7461 2720 696e 2073 7973 2e61 7267 763a  ta' in sys.argv:
+00004590: 0a20 2020 2020 2020 2077 732e 5365 6e64  .        ws.Send
+000045a0: 416c 6572 7461 5472 616e 7361 6363 282a  AlertaTransacc(*
+000045b0: 7379 732e 6172 6776 5b73 7973 2e61 7267  sys.argv[sys.arg
+000045c0: 762e 696e 6465 7828 222d 2d61 6c65 7274  v.index("--alert
+000045d0: 6122 292b 313a 5d29 0a20 2020 2065 6c69  a")+1:]).    eli
+000045e0: 6620 272d 2d63 616e 6365 6c61 2720 696e  f '--cancela' in
+000045f0: 2073 7973 2e61 7267 763a 0a20 2020 2020   sys.argv:.     
+00004600: 2020 2077 732e 5365 6e64 4361 6e63 656c     ws.SendCancel
+00004610: 6154 7261 6e73 6163 282a 7379 732e 6172  aTransac(*sys.ar
+00004620: 6776 5b73 7973 2e61 7267 762e 696e 6465  gv[sys.argv.inde
+00004630: 7828 222d 2d63 616e 6365 6c61 2229 2b31  x("--cancela")+1
+00004640: 3a5d 290a 2020 2020 656c 6966 2027 2d2d  :]).    elif '--
+00004650: 636f 6e73 756c 7461 2720 696e 2073 7973  consulta' in sys
+00004660: 2e61 7267 763a 0a20 2020 2020 2020 2077  .argv:.        w
+00004670: 732e 4765 7454 7261 6e73 6163 6369 6f6e  s.GetTransaccion
+00004680: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
+00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046a0: 2a73 7973 2e61 7267 765b 7379 732e 6172  *sys.argv[sys.ar
+000046b0: 6776 2e69 6e64 6578 2822 2d2d 636f 6e73  gv.index("--cons
+000046c0: 756c 7461 2229 2b31 3a5d 0a20 2020 2020  ulta")+1:].     
+000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000046f0: 2070 7269 6e74 2822 4361 6e74 5061 6769   print("CantPagi
+00004700: 6e61 7322 2c20 7773 2e43 616e 7450 6167  nas", ws.CantPag
+00004710: 696e 6173 290a 2020 2020 2020 2020 7072  inas).        pr
+00004720: 696e 7428 2248 6179 4572 726f 7222 2c20  int("HayError", 
+00004730: 7773 2e48 6179 4572 726f 7229 0a20 2020  ws.HayError).   
+00004740: 2020 2020 2023 2070 7269 6e74 2822 5472       # print("Tr
+00004750: 616e 7361 6363 696f 6e53 656e 6173 6122  ansaccionSenasa"
+00004760: 2c20 7773 2e54 7261 6e73 6163 6369 6f6e  , ws.Transaccion
+00004770: 5365 6e61 7361 290a 2020 2020 2020 2020  Senasa).        
+00004780: 2320 7061 7261 6d65 7472 6f73 2063 6f6d  # parametros com
+00004790: 756e 6573 2064 6520 7361 6c69 6461 2028  unes de salida (
+000047a0: 636f 6c75 6d6e 6173 2064 6520 6c61 2074  columnas de la t
+000047b0: 6162 6c61 293a 0a20 2020 2020 2020 2063  abla):.        c
+000047c0: 6c61 7665 7320 3d20 5b6b 2066 6f72 206b  laves = [k for k
+000047d0: 2c20 762c 206c 2069 6e20 5452 414e 5341  , v, l in TRANSA
+000047e0: 4343 494f 4e45 535d 0a20 2020 2020 2020  CCIONES].       
+000047f0: 2023 2065 7874 6965 6e64 6f20 6c61 206c   # extiendo la l
+00004800: 6973 7461 2064 6520 7265 7375 6c74 6164  ista de resultad
+00004810: 6f20 7061 7261 2065 6c20 6172 6368 6976  o para el archiv
+00004820: 6f20 6465 2069 6e74 6572 6361 6d62 696f  o de intercambio
+00004830: 3a0a 2020 2020 2020 2020 7472 616e 7361  :.        transa
+00004840: 6363 696f 6e65 732e 6578 7465 6e64 2877  cciones.extend(w
+00004850: 732e 5472 616e 7361 6363 696f 6e53 656e  s.TransaccionSen
+00004860: 6173 6129 0a20 2020 2020 2020 2023 2065  asa).        # e
+00004870: 6e63 6162 657a 6164 6f20 6465 206c 6120  ncabezado de la 
+00004880: 7461 626c 613a 0a20 2020 2020 2020 2070  tabla:.        p
+00004890: 7269 6e74 2822 7c7c 222c 2022 7c7c 222e  rint("||", "||".
+000048a0: 6a6f 696e 285b 2225 7322 2025 2063 6c61  join(["%s" % cla
+000048b0: 7665 2066 6f72 2063 6c61 7665 2069 6e20  ve for clave in 
+000048c0: 636c 6176 6573 5d29 2c20 227c 7c22 290a  claves]), "||").
+000048d0: 2020 2020 2020 2020 2320 7265 636f 7272          # recorr
+000048e0: 6f20 6c6f 7320 6461 746f 7320 6465 7675  o los datos devu
+000048f0: 656c 746f 7320 2854 7261 6e73 6163 6369  eltos (Transacci
+00004900: 6f6e 5365 6e61 7361 293a 0a20 2020 2020  onSenasa):.     
+00004910: 2020 2077 6869 6c65 2077 732e 4c65 6572     while ws.Leer
+00004920: 5472 616e 7361 6363 696f 6e28 293a 0a20  Transaccion():. 
+00004930: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
+00004940: 6c61 7665 2069 6e20 636c 6176 6573 3a0a  lave in claves:.
+00004950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004960: 7072 696e 7428 227c 7c22 2c20 7773 2e47  print("||", ws.G
+00004970: 6574 5061 7261 6d65 7472 6f28 636c 6176  etParametro(clav
+00004980: 6529 2920 2020 2020 2020 2023 2069 6d70  e))        # imp
+00004990: 7269 6d6f 2063 6164 6120 6669 6c61 290a  rimo cada fila).
+000049a0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000049b0: 7428 227c 7c22 290a 2020 2020 656c 7365  t("||").    else
+000049c0: 3a0a 2020 2020 2020 2020 6172 6776 203d  :.        argv =
+000049d0: 205b 6172 6776 2066 6f72 2061 7267 7620   [argv for argv 
+000049e0: 696e 2073 7973 2e61 7267 7620 6966 206e  in sys.argv if n
+000049f0: 6f74 2061 7267 762e 7374 6172 7473 7769  ot argv.startswi
+00004a00: 7468 2822 2d2d 2229 5d0a 2020 2020 2020  th("--")].      
+00004a10: 2020 6966 206e 6f74 2074 7261 6e73 6163    if not transac
+00004a20: 6369 6f6e 5f64 746f 3a0a 2020 2020 2020  cion_dto:.      
+00004a30: 2020 2020 2020 6966 206c 656e 2861 7267        if len(arg
+00004a40: 7629 3e31 303a 0a20 2020 2020 2020 2020  v)>10:.         
+00004a50: 2020 2020 2020 2077 732e 5361 7665 5472         ws.SaveTr
+00004a60: 616e 7361 6363 696f 6e28 2a61 7267 765b  ansaccion(*argv[
+00004a70: 313a 5d29 0a20 2020 2020 2020 2020 2020  1:]).           
+00004a80: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00004a90: 2020 2020 2020 2070 7269 6e74 2822 4552         print("ER
+00004aa0: 524f 523a 206e 6f20 7365 2069 6e64 6963  ROR: no se indic
+00004ab0: 6172 6f6e 2074 6f64 6f73 206c 6f73 2070  aron todos los p
+00004ac0: 6172 e16d 6574 726f 7320 7265 7175 6572  ar.metros requer
+00004ad0: 6964 6f73 2229 0a20 2020 2020 2020 2065  idos").        e
+00004ae0: 6c69 6620 7472 616e 7361 6363 696f 6e5f  lif transaccion_
+00004af0: 6474 6f3a 0a20 2020 2020 2020 2020 2020  dto:.           
+00004b00: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00004b10: 2020 2020 2020 7573 7561 7269 6f2c 2070        usuario, p
+00004b20: 6173 7377 6f72 6420 3d20 6172 6776 5b2d  assword = argv[-
+00004b30: 323a 5d0a 2020 2020 2020 2020 2020 2020  2:].            
+00004b40: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+00004b50: 2020 2020 2020 2020 7072 696e 7428 2241          print("A
+00004b60: 4456 4552 5445 4e43 4941 3a20 6e6f 2073  DVERTENCIA: no s
+00004b70: 6520 696e 6469 636f 2070 6172 e16d 6574  e indico par.met
+00004b80: 726f 7320 7573 7561 7269 6f20 7920 7061  ros usuario y pa
+00004b90: 7373 6f77 6f72 6422 290a 2020 2020 2020  ssoword").      
+00004ba0: 2020 2020 2020 2020 2020 7573 7561 7269            usuari
+00004bb0: 6f2c 2070 6173 7377 6f72 6420 3d20 2273  o, password = "s
+00004bc0: 656e 6173 6177 7322 2c20 2243 6c61 7665  enasaws", "Clave
+00004bd0: 3230 3133 220a 2020 2020 2020 2020 2020  2013".          
+00004be0: 2020 666f 7220 692c 2064 746f 2069 6e20    for i, dto in 
+00004bf0: 656e 756d 6572 6174 6528 7472 616e 7361  enumerate(transa
+00004c00: 6363 696f 6e5f 6474 6f29 3a0a 2020 2020  ccion_dto):.    
+00004c10: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00004c20: 7428 2250 726f 6365 7361 6e64 6f20 7265  t("Procesando re
+00004c30: 6769 7374 726f 222c 2069 290a 2020 2020  gistro", i).    
+00004c40: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
+00004c50: 6474 6f5b 2763 6f64 6967 6f5f 7472 616e  dto['codigo_tran
+00004c60: 7361 6363 696f 6e27 5d0a 2020 2020 2020  saccion'].      
+00004c70: 2020 2020 2020 2020 2020 7773 2e53 6176            ws.Sav
+00004c80: 6554 7261 6e73 6163 6369 6f6e 2875 7375  eTransaccion(usu
+00004c90: 6172 696f 2c20 7061 7373 776f 7264 2c20  ario, password, 
+00004ca0: 2a2a 6474 6f29 0a20 2020 2020 2020 2020  **dto).         
+00004cb0: 2020 2020 2020 2064 746f 5b27 636f 6469         dto['codi
+00004cc0: 676f 5f74 7261 6e73 6163 6369 6f6e 275d  go_transaccion']
+00004cd0: 203d 2077 732e 436f 6469 676f 5472 616e   = ws.CodigoTran
+00004ce0: 7361 6363 696f 6e0a 2020 2020 2020 2020  saccion.        
+00004cf0: 2020 2020 2020 2020 6572 726f 7265 732e          errores.
+00004d00: 6578 7465 6e64 2877 732e 6572 726f 7265  extend(ws.errore
+00004d10: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+00004d20: 2020 2070 7269 6e74 2822 7c52 6573 756c     print("|Resul
+00004d30: 7461 646f 2025 3573 7c43 6f64 6967 6f54  tado %5s|CodigoT
+00004d40: 7261 6e73 6163 6369 6f6e 2025 3130 737c  ransaccion %10s|
+00004d50: 4572 726f 7265 737c 2573 7c22 2025 2028  Errores|%s|" % (
+00004d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004d70: 2020 2020 2077 732e 5265 7375 6c74 6164       ws.Resultad
+00004d80: 6f2c 0a20 2020 2020 2020 2020 2020 2020  o,.             
+00004d90: 2020 2020 2020 2077 732e 436f 6469 676f         ws.Codigo
+00004da0: 5472 616e 7361 6363 696f 6e2c 0a20 2020  Transaccion,.   
+00004db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004dc0: 2027 7c27 2e6a 6f69 6e28 7773 2e45 7272   '|'.join(ws.Err
+00004dd0: 6f72 6573 206f 7220 5b5d 292c 0a20 2020  ores or []),.   
+00004de0: 2020 2020 2020 2020 2020 2020 2029 290a               )).
+00004df0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00004e00: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00004e10: 2245 5252 4f52 3a20 6e6f 2073 6520 6573  "ERROR: no se es
+00004e20: 7065 6369 6669 6361 726f 6e20 7072 6f64  pecificaron prod
+00004e30: 7563 746f 7320 6120 696e 666f 726d 6172  uctos a informar
+00004e40: 2229 0a0a 2020 2020 6966 206e 6f74 2074  ")..    if not t
+00004e50: 7261 6e73 6163 6369 6f6e 5f64 746f 3a0a  ransaccion_dto:.
+00004e60: 2020 2020 2020 2020 7072 696e 7428 227c          print("|
+00004e70: 5265 7375 6c74 6164 6f20 2535 737c 436f  Resultado %5s|Co
+00004e80: 6469 676f 5472 616e 7361 6363 696f 6e20  digoTransaccion 
+00004e90: 2531 3073 7c45 7272 6f72 6573 7c25 737c  %10s|Errores|%s|
+00004ea0: 2220 2520 280a 2020 2020 2020 2020 2020  " % (.          
+00004eb0: 2020 7773 2e52 6573 756c 7461 646f 2c0a    ws.Resultado,.
+00004ec0: 2020 2020 2020 2020 2020 2020 7773 2e43              ws.C
+00004ed0: 6f64 6967 6f54 7261 6e73 6163 6369 6f6e  odigoTransaccion
+00004ee0: 2c0a 2020 2020 2020 2020 2020 2020 277c  ,.            '|
+00004ef0: 272e 6a6f 696e 2877 732e 4572 726f 7265  '.join(ws.Errore
+00004f00: 7320 6f72 205b 5d29 2c0a 2020 2020 2020  s or []),.      
+00004f10: 2020 2929 0a0a 2020 2020 6966 2077 732e    ))..    if ws.
+00004f20: 4578 6365 7063 696f 6e3a 0a20 2020 2020  Excepcion:.     
+00004f30: 2020 2070 7269 6e74 2877 732e 5472 6163     print(ws.Trac
+00004f40: 6562 6163 6b29 0a0a 2020 2020 6966 2027  eback)..    if '
+00004f50: 2d2d 6772 6162 6172 2720 696e 2073 7973  --grabar' in sys
+00004f60: 2e61 7267 763a 0a20 2020 2020 2020 2069  .argv:.        i
+00004f70: 6620 272d 2d64 6266 2720 696e 2073 7973  f '--dbf' in sys
+00004f80: 2e61 7267 763a 0a20 2020 2020 2020 2020  .argv:.         
+00004f90: 2020 2067 7561 7264 6172 5f64 6266 2866     guardar_dbf(f
+00004fa0: 6f72 6d61 746f 732c 2054 7275 652c 207b  ormatos, True, {
+00004fb0: 7d29 0a20 2020 2020 2020 2065 6c69 6620  }).        elif 
+00004fc0: 272d 2d6a 736f 6e27 2069 6e20 7379 732e  '--json' in sys.
+00004fd0: 6172 6776 3a0a 2020 2020 2020 2020 2020  argv:.          
+00004fe0: 2020 666f 7220 666f 726d 6174 6f20 696e    for formato in
+00004ff0: 2066 6f72 6d61 746f 733a 0a20 2020 2020   formatos:.     
+00005000: 2020 2020 2020 2020 2020 2061 7263 6869             archi
+00005010: 766f 203d 206f 7065 6e28 666f 726d 6174  vo = open(format
+00005020: 6f5b 305d 2e6c 6f77 6572 2829 202b 2022  o[0].lower() + "
+00005030: 2e6a 736f 6e22 2c20 2277 2229 0a20 2020  .json", "w").   
+00005040: 2020 2020 2020 2020 2020 2020 206a 736f               jso
+00005050: 6e2e 6475 6d70 2866 6f72 6d61 746f 5b32  n.dump(formato[2
+00005060: 5d2c 2061 7263 6869 766f 2c20 736f 7274  ], archivo, sort
+00005070: 5f6b 6579 733d 5472 7565 2c20 696e 6465  _keys=True, inde
+00005080: 6e74 3d34 290a 2020 2020 2020 2020 2020  nt=4).          
+00005090: 2020 2020 2020 6172 6368 6976 6f2e 636c        archivo.cl
+000050a0: 6f73 6528 290a 2020 2020 2020 2020 656c  ose().        el
+000050b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000050c0: 666f 7220 666f 726d 6174 6f20 696e 2066  for formato in f
+000050d0: 6f72 6d61 746f 733a 0a20 2020 2020 2020  ormatos:.       
+000050e0: 2020 2020 2020 2020 2061 7263 6869 766f           archivo
+000050f0: 203d 206f 7065 6e28 666f 726d 6174 6f5b   = open(formato[
+00005100: 305d 2e6c 6f77 6572 2829 202b 2022 2e74  0].lower() + ".t
+00005110: 7874 222c 2022 7722 290a 2020 2020 2020  xt", "w").      
+00005120: 2020 2020 2020 2020 2020 666f 7220 6974            for it
+00005130: 2069 6e20 666f 726d 6174 6f5b 325d 3a0a   in formato[2]:.
+00005140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005150: 2020 2020 6172 6368 6976 6f2e 7772 6974      archivo.writ
+00005160: 6528 6573 6372 6962 6972 2869 742c 2066  e(escribir(it, f
+00005170: 6f72 6d61 746f 5b31 5d29 290a 2020 2020  ormato[1])).    
+00005180: 2020 2020 2020 2020 6172 6368 6976 6f2e          archivo.
+00005190: 636c 6f73 6528 290a 0a0a 2320 6275 7363  close()...# busc
+000051a0: 6f20 656c 2064 6972 6563 746f 7269 6f20  o el directorio 
+000051b0: 6465 2069 6e73 7461 6c61 6369 f36e 2028  de instalaci.n (
+000051c0: 676c 6f62 616c 2070 6172 6120 7175 6520  global para que 
+000051d0: 6e6f 2063 616d 6269 6520 7369 2075 7361  no cambie si usa
+000051e0: 6e20 6f74 7261 2064 6c6c 290a 494e 5354  n otra dll).INST
+000051f0: 414c 4c5f 4449 5220 3d20 5472 617a 6146  ALL_DIR = TrazaF
+00005200: 6974 6f2e 496e 7374 616c 6c44 6972 203d  ito.InstallDir =
+00005210: 2067 6574 5f69 6e73 7461 6c6c 5f64 6972   get_install_dir
+00005220: 2829 0a0a 0a69 6620 5f5f 6e61 6d65 5f5f  ()...if __name__
+00005230: 203d 3d20 275f 5f6d 6169 6e5f 5f27 3a0a   == '__main__':.
+00005240: 0a20 2020 2023 2061 6a75 7374 6f20 656c  .    # ajusto el
+00005250: 2065 6e63 6f64 696e 6720 706f 7220 6465   encoding por de
+00005260: 6665 6374 6f20 2873 6920 7365 2072 6564  fecto (si se red
+00005270: 6972 696a 6520 6c61 2073 616c 6964 6129  irije la salida)
+00005280: 0a20 2020 2069 6620 6e6f 7420 6861 7361  .    if not hasa
+00005290: 7474 7228 7379 732e 7374 646f 7574 2c20  ttr(sys.stdout, 
+000052a0: 2265 6e63 6f64 696e 6722 2920 6f72 2073  "encoding") or s
+000052b0: 7973 2e73 7464 6f75 742e 656e 636f 6469  ys.stdout.encodi
+000052c0: 6e67 2069 7320 4e6f 6e65 3a0a 2020 2020  ng is None:.    
+000052d0: 2020 2020 696d 706f 7274 2063 6f64 6563      import codec
+000052e0: 732c 206c 6f63 616c 650a 2020 2020 2020  s, locale.      
+000052f0: 2020 7379 732e 7374 646f 7574 203d 2063    sys.stdout = c
+00005300: 6f64 6563 732e 6765 7477 7269 7465 7228  odecs.getwriter(
+00005310: 6c6f 6361 6c65 2e67 6574 7072 6566 6572  locale.getprefer
+00005320: 7265 6465 6e63 6f64 696e 6728 2929 2873  redencoding())(s
+00005330: 7973 2e73 7464 6f75 742c 2272 6570 6c61  ys.stdout,"repla
+00005340: 6365 2229 3b0a 2020 2020 2020 2020 7379  ce");.        sy
+00005350: 732e 7374 6465 7272 203d 2063 6f64 6563  s.stderr = codec
+00005360: 732e 6765 7477 7269 7465 7228 6c6f 6361  s.getwriter(loca
+00005370: 6c65 2e67 6574 7072 6566 6572 7265 6465  le.getpreferrede
+00005380: 6e63 6f64 696e 6728 2929 2873 7973 2e73  ncoding())(sys.s
+00005390: 7464 6572 722c 2272 6570 6c61 6365 2229  tderr,"replace")
+000053a0: 3b0a 0a20 2020 2069 6620 272d 2d72 6567  ;..    if '--reg
+000053b0: 6973 7465 7227 2069 6e20 7379 732e 6172  ister' in sys.ar
+000053c0: 6776 206f 7220 272d 2d75 6e72 6567 6973  gv or '--unregis
+000053d0: 7465 7227 2069 6e20 7379 732e 6172 6776  ter' in sys.argv
+000053e0: 3a0a 2020 2020 2020 2020 696d 706f 7274  :.        import
+000053f0: 2070 7974 686f 6e63 6f6d 0a20 2020 2020   pythoncom.     
+00005400: 2020 2069 6d70 6f72 7420 7769 6e33 3263     import win32c
+00005410: 6f6d 2e73 6572 7665 722e 7265 6769 7374  om.server.regist
+00005420: 6572 0a20 2020 2020 2020 2077 696e 3332  er.        win32
+00005430: 636f 6d2e 7365 7276 6572 2e72 6567 6973  com.server.regis
+00005440: 7465 722e 5573 6543 6f6d 6d61 6e64 4c69  ter.UseCommandLi
+00005450: 6e65 2854 7261 7a61 4669 746f 290a 2020  ne(TrazaFito).  
+00005460: 2020 656c 6966 2022 2f41 7574 6f6d 6174    elif "/Automat
+00005470: 6522 2069 6e20 7379 732e 6172 6776 3a0a  e" in sys.argv:.
+00005480: 2020 2020 2020 2020 2320 4d53 2073 6565          # MS see
+00005490: 6d73 2074 6f20 6c69 6b65 202f 6175 746f  ms to like /auto
+000054a0: 6d61 7465 2074 6f20 7275 6e20 7468 6520  mate to run the 
+000054b0: 636c 6173 7320 6661 6374 6f72 6965 732e  class factories.
+000054c0: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
+000054d0: 7769 6e33 3263 6f6d 2e73 6572 7665 722e  win32com.server.
+000054e0: 6c6f 6361 6c73 6572 7665 720a 2020 2020  localserver.    
+000054f0: 2020 2020 2377 696e 3332 636f 6d2e 7365      #win32com.se
+00005500: 7276 6572 2e6c 6f63 616c 7365 7276 6572  rver.localserver
+00005510: 2e6d 6169 6e28 290a 2020 2020 2020 2020  .main().        
+00005520: 2320 7374 6172 7420 7468 6520 7365 7276  # start the serv
+00005530: 6572 2e0a 2020 2020 2020 2020 7769 6e33  er..        win3
+00005540: 3263 6f6d 2e73 6572 7665 722e 6c6f 6361  2com.server.loca
+00005550: 6c73 6572 7665 722e 7365 7276 6528 5b54  lserver.serve([T
+00005560: 7261 7a61 4669 746f 2e5f 7265 675f 636c  razaFito._reg_cl
+00005570: 7369 645f 5d29 0a20 2020 2065 6c73 653a  sid_]).    else:
+00005580: 0a20 2020 2020 2020 206d 6169 6e28 290a  .        main().
```

### Comparing `py3afipws-0.8/py3afipws/trazamed.py` & `py3afipws-0.9/py3afipws/trazamed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,2526 +1,2528 @@
 00000000: 2321 2f75 7372 2f62 696e 2f70 7974 686f  #!/usr/bin/pytho
-00000010: 6e0a 2320 5468 6973 2070 726f 6772 616d  n.# This program
-00000020: 2069 7320 6672 6565 2073 6f66 7477 6172   is free softwar
-00000030: 653b 2079 6f75 2063 616e 2072 6564 6973  e; you can redis
-00000040: 7472 6962 7574 6520 6974 2061 6e64 2f6f  tribute it and/o
-00000050: 7220 6d6f 6469 6679 0a23 2069 7420 756e  r modify.# it un
-00000060: 6465 7220 7468 6520 7465 726d 7320 6f66  der the terms of
-00000070: 2074 6865 2047 4e55 2047 656e 6572 616c   the GNU General
-00000080: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
-00000090: 6173 2070 7562 6c69 7368 6564 2062 7920  as published by 
-000000a0: 7468 650a 2320 4672 6565 2053 6f66 7477  the.# Free Softw
-000000b0: 6172 6520 466f 756e 6461 7469 6f6e 3b20  are Foundation; 
-000000c0: 6569 7468 6572 2076 6572 7369 6f6e 2033  either version 3
-000000d0: 2c20 6f72 2028 6174 2079 6f75 7220 6f70  , or (at your op
-000000e0: 7469 6f6e 2920 616e 7920 6c61 7465 720a  tion) any later.
-000000f0: 2320 7665 7273 696f 6e2e 0a23 0a23 2054  # version..#.# T
-00000100: 6869 7320 7072 6f67 7261 6d20 6973 2064  his program is d
-00000110: 6973 7472 6962 7574 6564 2069 6e20 7468  istributed in th
-00000120: 6520 686f 7065 2074 6861 7420 6974 2077  e hope that it w
-00000130: 696c 6c20 6265 2075 7365 6675 6c2c 2062  ill be useful, b
-00000140: 7574 0a23 2057 4954 484f 5554 2041 4e59  ut.# WITHOUT ANY
-00000150: 2057 4152 5241 4e54 593b 2077 6974 686f   WARRANTY; witho
-00000160: 7574 2065 7665 6e20 7468 6520 696d 706c  ut even the impl
-00000170: 6965 6420 7761 7272 616e 7479 206f 6620  ied warranty of 
-00000180: 4d45 5243 4841 4e54 4942 494c 4954 590a  MERCHANTIBILITY.
-00000190: 2320 6f72 2046 4954 4e45 5353 2046 4f52  # or FITNESS FOR
-000001a0: 2041 2050 4152 5449 4355 4c41 5220 5055   A PARTICULAR PU
-000001b0: 5250 4f53 452e 2020 5365 6520 7468 6520  RPOSE.  See the 
-000001c0: 474e 5520 4765 6e65 7261 6c20 5075 626c  GNU General Publ
-000001d0: 6963 204c 6963 656e 7365 0a23 2066 6f72  ic License.# for
-000001e0: 206d 6f72 6520 6465 7461 696c 732e 0a0a   more details...
-000001f0: 2222 224d f364 756c 6f20 7061 7261 2054  """M.dulo para T
-00000200: 7261 7a61 6269 6c69 6461 6420 6465 204d  razabilidad de M
-00000210: 6564 6963 616d 656e 746f 7320 414e 4d41  edicamentos ANMA
-00000220: 5420 2d20 5041 4d49 202d 2049 4e53 534a  T - PAMI - INSSJ
-00000230: 5020 4469 7370 2e20 3336 3833 2f31 310a  P Disp. 3683/11.
-00000240: 7365 67fa 6e20 4573 7065 6369 6669 6361  seg.n Especifica
-00000250: 6369 f36e 2054 e963 6e69 6361 2070 6172  ci.n T.cnica par
-00000260: 6120 5072 7565 6261 7320 6465 2053 6572  a Pruebas de Ser
-00000270: 7669 6369 6f73 2076 3220 2832 3031 3329  vicios v2 (2013)
-00000280: 2222 220a 0a23 2049 6e66 6f72 6d61 6369  """..# Informaci
-00000290: f36e 2061 6469 6369 6f6e 616c 2079 2064  .n adicional y d
-000002a0: 6f63 756d 656e 7461 6369 f36e 3a0a 2320  ocumentaci.n:.# 
-000002b0: 6874 7470 3a2f 2f77 7777 2e73 6973 7465  http://www.siste
-000002c0: 6d61 7361 6769 6c65 732e 636f 6d2e 6172  masagiles.com.ar
-000002d0: 2f74 7261 632f 7769 6b69 2f54 7261 7a61  /trac/wiki/Traza
-000002e0: 6269 6c69 6461 644d 6564 6963 616d 656e  bilidadMedicamen
-000002f0: 746f 730a 0a5f 5f61 7574 686f 725f 5f20  tos..__author__ 
-00000300: 3d20 224d 6172 6961 6e6f 2052 6569 6e67  = "Mariano Reing
-00000310: 6172 7420 3c72 6569 6e67 6172 7440 676d  art <reingart@gm
-00000320: 6169 6c2e 636f 6d3e 220a 5f5f 636f 7079  ail.com>".__copy
-00000330: 7269 6768 745f 5f20 3d20 2243 6f70 7972  right__ = "Copyr
-00000340: 6967 6874 2028 4329 2032 3031 3120 4d61  ight (C) 2011 Ma
-00000350: 7269 616e 6f20 5265 696e 6761 7274 220a  riano Reingart".
-00000360: 5f5f 6c69 6365 6e73 655f 5f20 3d20 2247  __license__ = "G
-00000370: 504c 2033 2e30 220a 5f5f 7665 7273 696f  PL 3.0".__versio
-00000380: 6e5f 5f20 3d20 2231 2e31 3662 220a 0a69  n__ = "1.16b"..i
-00000390: 6d70 6f72 7420 6f73 0a69 6d70 6f72 7420  mport os.import 
-000003a0: 736f 636b 6574 0a69 6d70 6f72 7420 7379  socket.import sy
-000003b0: 730a 696d 706f 7274 2064 6174 6574 696d  s.import datetim
-000003c0: 650a 696d 706f 7274 2074 696d 650a 696d  e.import time.im
-000003d0: 706f 7274 2074 7261 6365 6261 636b 0a69  port traceback.i
-000003e0: 6d70 6f72 7420 7079 3373 696d 706c 6573  mport py3simples
-000003f0: 6f61 702e 636c 6965 6e74 0a66 726f 6d20  oap.client.from 
-00000400: 7079 3373 696d 706c 6573 6f61 702e 636c  py3simplesoap.cl
-00000410: 6965 6e74 2069 6d70 6f72 7420 536f 6170  ient import Soap
-00000420: 436c 6965 6e74 2c20 536f 6170 4661 756c  Client, SoapFaul
-00000430: 742c 2070 6172 7365 5f70 726f 7879 2c20  t, parse_proxy, 
-00000440: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
-00000450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000460: 2020 7365 745f 6874 7470 5f77 7261 7070    set_http_wrapp
-00000470: 6572 0a66 726f 6d20 7079 3373 696d 706c  er.from py3simpl
-00000480: 6573 6f61 702e 7369 6d70 6c65 786d 6c20  esoap.simplexml 
-00000490: 696d 706f 7274 2053 696d 706c 6558 4d4c  import SimpleXML
-000004a0: 456c 656d 656e 740a 6672 6f6d 2063 5374  Element.from cSt
-000004b0: 7269 6e67 494f 2069 6d70 6f72 7420 5374  ringIO import St
-000004c0: 7269 6e67 494f 0a0a 2320 696d 706f 7274  ringIO..# import
-000004d0: 6f20 6675 6e63 696f 6e65 7320 636f 6d70  o funciones comp
-000004e0: 6172 7469 6461 733a 0a66 726f 6d20 2e75  artidas:.from .u
-000004f0: 7469 6c73 2069 6d70 6f72 7420 280a 2020  tils import (.  
-00000500: 2020 6c65 6572 2c20 6573 6372 6962 6972    leer, escribir
-00000510: 2c20 6c65 6572 5f64 6266 2c20 6775 6172  , leer_dbf, guar
-00000520: 6461 725f 6462 662c 204e 2c20 412c 2049  dar_dbf, N, A, I
-00000530: 2c20 6a73 6f6e 2c0a 2020 2020 6461 725f  , json,.    dar_
-00000540: 6e6f 6d62 7265 5f63 616d 706f 5f64 6266  nombre_campo_dbf
-00000550: 2c20 6765 745f 696e 7374 616c 6c5f 6469  , get_install_di
-00000560: 722c 2042 6173 6557 532c 0a20 2020 2069  r, BaseWS,.    i
-00000570: 6e69 6369 616c 697a 6172 5f79 5f63 6170  nicializar_y_cap
-00000580: 7475 7261 725f 6578 6365 7063 696f 6e65  turar_excepcione
-00000590: 730a 290a 0a48 4f4d 4f20 3d20 4661 6c73  s.)..HOMO = Fals
-000005a0: 650a 5459 5045 4c49 4220 3d20 4661 6c73  e.TYPELIB = Fals
-000005b0: 650a 0a57 5344 4c20 3d20 2268 7474 7073  e..WSDL = "https
-000005c0: 3a2f 2f73 6572 7669 6369 6f73 2e70 616d  ://servicios.pam
-000005d0: 692e 6f72 672e 6172 2f74 7261 7a61 6d65  i.org.ar/trazame
-000005e0: 642e 5765 6253 6572 7669 6365 3f77 7364  d.WebService?wsd
-000005f0: 6c22 0a4c 4f43 4154 494f 4e20 3d20 2268  l".LOCATION = "h
-00000600: 7474 7073 3a2f 2f73 6572 7669 6369 6f73  ttps://servicios
-00000610: 2e70 616d 692e 6f72 672e 6172 2f74 7261  .pami.org.ar/tra
-00000620: 7a61 6d65 642e 5765 6253 6572 7669 6365  zamed.WebService
-00000630: 220a 2320 5753 444c 203d 2022 6874 7470  ".# WSDL = "http
-00000640: 733a 2f2f 7472 617a 6162 696c 6964 6164  s://trazabilidad
-00000650: 2e70 616d 692e 6f72 672e 6172 3a39 3035  .pami.org.ar:905
-00000660: 302f 7472 617a 616d 6564 2e57 6562 5365  0/trazamed.WebSe
-00000670: 7276 6963 653f 7773 646c 220a 0a23 2046  rvice?wsdl"..# F
-00000680: 6f72 6d61 746f 2064 6520 4d65 6469 6361  ormato de Medica
-00000690: 6d65 6e74 6f73 4454 4f2c 204d 6564 6963  mentosDTO, Medic
-000006a0: 616d 656e 746f 7344 544f 4448 5365 7269  amentosDTODHSeri
-000006b0: 652c 204d 6564 6963 616d 656e 746f 7344  e, MedicamentosD
-000006c0: 544f 4672 6163 6369 6f6e 0a4d 4544 4943  TOFraccion.MEDIC
-000006d0: 414d 454e 544f 5320 3d20 5b0a 2020 2020  AMENTOS = [.    
-000006e0: 2827 665f 6576 656e 746f 272c 2031 302c  ('f_evento', 10,
-000006f0: 2041 292c 2020 2020 2020 2020 2020 2020   A),            
-00000700: 2020 2020 2320 666f 726d 6174 6f20 4444      # formato DD
-00000710: 2f4d 4d2f 4141 4141 0a20 2020 2028 2768  /MM/AAAA.    ('h
-00000720: 5f65 7665 6e74 6f27 2c20 352c 2041 292c  _evento', 5, A),
-00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000740: 2023 2066 6f72 6d61 746f 2048 483a 4d4d   # formato HH:MM
-00000750: 0a20 2020 2028 2767 6c6e 5f6f 7269 6765  .    ('gln_orige
-00000760: 6e27 2c20 3133 2c20 4129 2c0a 2020 2020  n', 13, A),.    
-00000770: 2827 676c 6e5f 6465 7374 696e 6f27 2c20  ('gln_destino', 
-00000780: 3133 2c20 4129 2c0a 2020 2020 2827 6e5f  13, A),.    ('n_
-00000790: 7265 6d69 746f 272c 2032 302c 2041 292c  remito', 20, A),
-000007a0: 0a20 2020 2028 276e 5f66 6163 7475 7261  .    ('n_factura
-000007b0: 272c 2032 302c 2041 292c 0a20 2020 2028  ', 20, A),.    (
-000007c0: 2776 656e 6369 6d69 656e 746f 272c 2031  'vencimiento', 1
-000007d0: 302c 2041 292c 0a20 2020 2028 2767 7469  0, A),.    ('gti
-000007e0: 6e27 2c20 3134 2c20 4129 2c0a 2020 2020  n', 14, A),.    
-000007f0: 2827 6c6f 7465 272c 2032 302c 2041 292c  ('lote', 20, A),
-00000800: 0a20 2020 2028 276e 756d 6572 6f5f 7365  .    ('numero_se
-00000810: 7269 616c 272c 2032 302c 2041 292c 0a20  rial', 20, A),. 
-00000820: 2020 2028 2764 6573 6465 5f6e 756d 6572     ('desde_numer
-00000830: 6f5f 7365 7269 616c 272c 2032 302c 2041  o_serial', 20, A
-00000840: 292c 2020 2020 2023 2073 656e 644d 6564  ),     # sendMed
-00000850: 6963 616d 656e 746f 7344 4853 6572 6965  icamentosDHSerie
-00000860: 0a20 2020 2028 2768 6173 7461 5f6e 756d  .    ('hasta_num
-00000870: 6572 6f5f 7365 7269 616c 272c 2032 302c  ero_serial', 20,
-00000880: 2041 292c 2020 2020 2023 2073 656e 644d   A),     # sendM
-00000890: 6564 6963 616d 656e 746f 7344 4853 6572  edicamentosDHSer
-000008a0: 6965 0a20 2020 2028 2769 645f 6f62 7261  ie.    ('id_obra
-000008b0: 5f73 6f63 6961 6c27 2c20 392c 204e 292c  _social', 9, N),
-000008c0: 0a20 2020 2028 2769 645f 6576 656e 746f  .    ('id_evento
-000008d0: 272c 2033 2c20 4e29 2c0a 2020 2020 2827  ', 3, N),.    ('
-000008e0: 6375 6974 5f6f 7269 6765 6e27 2c20 3131  cuit_origen', 11
-000008f0: 2c20 4129 2c0a 2020 2020 2827 6375 6974  , A),.    ('cuit
-00000900: 5f64 6573 7469 6e6f 272c 2031 312c 2041  _destino', 11, A
-00000910: 292c 0a20 2020 2028 2761 7065 6c6c 6964  ),.    ('apellid
-00000920: 6f27 2c20 3530 2c20 4129 2c0a 2020 2020  o', 50, A),.    
-00000930: 2827 6e6f 6d62 7265 7327 2c20 3130 302c  ('nombres', 100,
-00000940: 2041 292c 0a20 2020 2028 2774 6970 6f5f   A),.    ('tipo_
-00000950: 646f 6375 6d65 6e74 6f27 2c20 322c 204e  documento', 2, N
-00000960: 292c 2020 2020 2020 2020 2020 2023 2039  ),           # 9
-00000970: 363a 2044 4e49 2c38 303a 2043 5549 540a  6: DNI,80: CUIT.
-00000980: 2020 2020 2827 6e5f 646f 6375 6d65 6e74      ('n_document
-00000990: 6f27 2c20 3130 2c20 4129 2c0a 2020 2020  o', 10, A),.    
-000009a0: 2827 7365 786f 272c 2031 2c20 4129 2c20  ('sexo', 1, A), 
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 2020 2020 2320 4d20 6f20 460a 2020 2020      # M o F.    
-000009d0: 2827 6469 7265 6363 696f 6e27 2c20 3130  ('direccion', 10
-000009e0: 302c 2041 292c 0a20 2020 2028 276e 756d  0, A),.    ('num
-000009f0: 6572 6f27 2c20 3130 2c20 4129 2c0a 2020  ero', 10, A),.  
-00000a00: 2020 2827 7069 736f 272c 2035 2c20 4129    ('piso', 5, A)
-00000a10: 2c0a 2020 2020 2827 6465 7074 6f27 2c20  ,.    ('depto', 
-00000a20: 352c 2041 292c 0a20 2020 2028 276c 6f63  5, A),.    ('loc
-00000a30: 616c 6964 6164 272c 2035 302c 2041 292c  alidad', 50, A),
-00000a40: 0a20 2020 2028 2770 726f 7669 6e63 6961  .    ('provincia
-00000a50: 272c 2031 3030 2c20 4129 2c0a 2020 2020  ', 100, A),.    
-00000a60: 2827 6e5f 706f 7374 616c 272c 2038 2c20  ('n_postal', 8, 
-00000a70: 4129 2c0a 2020 2020 2827 6665 6368 615f  A),.    ('fecha_
-00000a80: 6e61 6369 6d69 656e 746f 272c 2031 3030  nacimiento', 100
-00000a90: 2c20 4129 2c0a 2020 2020 2827 7465 6c65  , A),.    ('tele
-00000aa0: 666f 6e6f 272c 2033 302c 2041 292c 0a20  fono', 30, A),. 
-00000ab0: 2020 2028 276e 726f 5f61 736f 6369 6164     ('nro_asociad
-00000ac0: 6f27 2c20 3330 2c20 4129 2c0a 2020 2020  o', 30, A),.    
-00000ad0: 2827 6361 6e74 6964 6164 272c 2033 2c20  ('cantidad', 3, 
-00000ae0: 4e29 2c20 2020 2020 2020 2020 2020 2020  N),             
-00000af0: 2020 2020 2320 7365 6e64 4d65 6469 6361      # sendMedica
-00000b00: 6d65 6e74 6f73 4672 6163 6369 6f6e 0a20  mentosFraccion. 
-00000b10: 2020 2028 2763 6f64 6967 6f5f 7472 616e     ('codigo_tran
-00000b20: 7361 6363 696f 6e27 2c20 3134 2c20 4129  saccion', 14, A)
-00000b30: 2c0a 5d0a 0a23 2046 6f72 6d61 746f 2070  ,.]..# Formato p
-00000b40: 6172 6120 5472 616e 7361 6363 696f 6e50  ara TransaccionP
-00000b50: 6c61 696e 5753 2028 6765 7454 7261 6e73  lainWS (getTrans
-00000b60: 6163 6369 6f6e 6573 4e6f 436f 6e66 6972  accionesNoConfir
-00000b70: 6d61 6461 7329 0a54 5241 4e53 4143 4349  madas).TRANSACCI
-00000b80: 4f4e 4553 203d 205b 0a20 2020 2028 275f  ONES = [.    ('_
-00000b90: 6964 5f74 7261 6e73 6163 6369 6f6e 272c  id_transaccion',
-00000ba0: 2031 342c 2041 292c 0a20 2020 2028 275f   14, A),.    ('_
-00000bb0: 6964 5f74 7261 6e73 6163 6369 6f6e 5f67  id_transaccion_g
-00000bc0: 6c6f 6261 6c27 2c20 3134 2c20 4129 2c0a  lobal', 14, A),.
-00000bd0: 2020 2020 2827 5f66 5f65 7665 6e74 6f27      ('_f_evento'
-00000be0: 2c20 3130 2c20 4129 2c0a 2020 2020 2827  , 10, A),.    ('
-00000bf0: 5f66 5f74 7261 6e73 6163 6369 6f6e 272c  _f_transaccion',
-00000c00: 2031 362c 2041 292c 2020 2020 2020 2020   16, A),        
-00000c10: 2020 2320 666f 726d 6174 6f20 4444 2f4d    # formato DD/M
-00000c20: 4d2f 4141 4141 2048 483a 4d4d 0a20 2020  M/AAAA HH:MM.   
-00000c30: 2028 275f 6774 696e 272c 2031 342c 2041   ('_gtin', 14, A
-00000c40: 292c 0a20 2020 2028 275f 6c6f 7465 272c  ),.    ('_lote',
-00000c50: 2032 302c 2041 292c 0a20 2020 2028 275f   20, A),.    ('_
-00000c60: 6e75 6d65 726f 5f73 6572 6961 6c27 2c20  numero_serial', 
-00000c70: 3230 2c20 4129 2c0a 2020 2020 2827 5f6e  20, A),.    ('_n
-00000c80: 6f6d 6272 6527 2c20 3230 302c 2041 292c  ombre', 200, A),
-00000c90: 0a20 2020 2028 275f 645f 6576 656e 746f  .    ('_d_evento
-00000ca0: 272c 2031 3030 2c20 4129 2c0a 2020 2020  ', 100, A),.    
-00000cb0: 2827 5f67 6c6e 5f6f 7269 6765 6e27 2c20  ('_gln_origen', 
-00000cc0: 3133 2c20 4129 2c0a 2020 2020 2827 5f72  13, A),.    ('_r
-00000cd0: 617a 6f6e 5f73 6f63 6961 6c5f 6f72 6967  azon_social_orig
-00000ce0: 656e 272c 2032 3030 2c20 4129 2c0a 2020  en', 200, A),.  
-00000cf0: 2020 2827 5f67 6c6e 5f64 6573 7469 6e6f    ('_gln_destino
-00000d00: 272c 2031 332c 2041 292c 0a20 2020 2028  ', 13, A),.    (
-00000d10: 275f 7261 7a6f 6e5f 736f 6369 616c 5f64  '_razon_social_d
-00000d20: 6573 7469 6e6f 272c 2032 3030 2c20 4129  estino', 200, A)
-00000d30: 2c0a 2020 2020 2827 5f6e 5f72 656d 6974  ,.    ('_n_remit
-00000d40: 6f27 2c20 3230 2c20 4129 2c0a 2020 2020  o', 20, A),.    
-00000d50: 2827 5f6e 5f66 6163 7475 7261 272c 2032  ('_n_factura', 2
-00000d60: 302c 2041 292c 0a20 2020 2028 275f 7665  0, A),.    ('_ve
-00000d70: 6e63 696d 6965 6e74 6f27 2c20 3130 2c20  ncimiento', 10, 
-00000d80: 4129 2c0a 2020 2020 2827 5f69 645f 6576  A),.    ('_id_ev
-00000d90: 656e 746f 272c 2033 2c20 4e29 2c20 2020  ento', 3, N),   
-00000da0: 2020 2020 2020 2020 2020 2020 2320 6167              # ag
-00000db0: 7265 6761 646f 2065 6c20 3330 2f30 312f  regado el 30/01/
-00000dc0: 3230 3134 0a5d 0a0a 2320 466f 726d 6174  2014.]..# Format
-00000dd0: 6f20 7061 7261 2045 7272 6f72 6573 0a45  o para Errores.E
-00000de0: 5252 4f52 4553 203d 205b 0a20 2020 2028  RRORES = [.    (
-00000df0: 2763 5f65 7272 6f72 272c 2034 2c20 4129  'c_error', 4, A)
-00000e00: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
-00000e10: 2020 2320 63f3 6469 676f 0a20 2020 2028    # c.digo.    (
-00000e20: 2764 5f65 7272 6f72 272c 2032 3530 2c20  'd_error', 250, 
-00000e30: 4129 2c20 2020 2020 2020 2020 2020 2020  A),             
-00000e40: 2020 2320 6465 7363 7269 7063 69f3 6e0a    # descripci.n.
-00000e50: 2020 2020 5d0a 0a0a 636c 6173 7320 5472      ]...class Tr
-00000e60: 617a 614d 6564 2842 6173 6557 5329 3a0a  azaMed(BaseWS):.
-00000e70: 2020 2020 2249 6e74 6572 6661 7a20 7061      "Interfaz pa
-00000e80: 7261 2065 6c20 5765 6253 6572 7669 6365  ra el WebService
-00000e90: 2064 6520 5472 617a 6162 696c 6964 6164   de Trazabilidad
-00000ea0: 2064 6520 4d65 6469 6361 6d65 6e74 6f73   de Medicamentos
-00000eb0: 2041 4e4d 4154 202d 205c 0a20 2020 2050   ANMAT - \.    P
-00000ec0: 414d 4920 2d20 494e 5353 4a50 220a 2020  AMI - INSSJP".  
-00000ed0: 2020 5f70 7562 6c69 635f 6d65 7468 6f64    _public_method
-00000ee0: 735f 203d 205b 2753 656e 644d 6564 6963  s_ = ['SendMedic
-00000ef0: 616d 656e 746f 7327 2c0a 2020 2020 2020  amentos',.      
-00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f10: 2020 2753 656e 6443 616e 6365 6c61 6354    'SendCancelacT
-00000f20: 7261 6e73 6163 6327 2c20 2753 656e 6443  ransacc', 'SendC
-00000f30: 616e 6365 6c61 6354 7261 6e73 6163 6350  ancelacTransaccP
-00000f40: 6172 6369 616c 272c 0a20 2020 2020 2020  arcial',.       
-00000f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f60: 2027 5365 6e64 4d65 6469 6361 6d65 6e74   'SendMedicament
-00000f70: 6f73 4448 5365 7269 6527 2c0a 2020 2020  osDHSerie',.    
-00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f90: 2020 2020 2753 656e 644d 6564 6963 616d      'SendMedicam
-00000fa0: 656e 746f 7346 7261 6363 696f 6e27 2c0a  entosFraccion',.
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2020 2020 2020 2020 2753 656e 6443 6f6e          'SendCon
-00000fd0: 6669 726d 6154 7261 6e73 6163 6327 2c20  firmaTransacc', 
-00000fe0: 2753 656e 6441 6c65 7274 6154 7261 6e73  'SendAlertaTrans
-00000ff0: 6163 6327 2c0a 2020 2020 2020 2020 2020  acc',.          
-00001000: 2020 2020 2020 2020 2020 2020 2020 2747                'G
-00001010: 6574 5472 616e 7361 6363 696f 6e65 734e  etTransaccionesN
-00001020: 6f43 6f6e 6669 726d 6164 6173 272c 0a20  oConfirmadas',. 
-00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001040: 2020 2020 2020 2027 4765 7445 6e76 696f         'GetEnvio
-00001050: 7350 726f 7069 6f73 416c 6572 7461 646f  sPropiosAlertado
-00001060: 7327 2c20 2747 6574 436f 6e73 756c 7461  s', 'GetConsulta
-00001070: 5374 6f63 6b27 2c0a 2020 2020 2020 2020  Stock',.        
-00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001090: 2747 6574 5472 616e 7361 6363 696f 6e65  'GetTransaccione
-000010a0: 7357 5327 2c20 2747 6574 4361 7461 6c6f  sWS', 'GetCatalo
-000010b0: 676f 456c 6563 7472 6f6e 6963 6f42 7947  goElectronicoByG
-000010c0: 5449 4e27 2c0a 2020 2020 2020 2020 2020  TIN',.          
-000010d0: 2020 2020 2020 2020 2020 2020 2020 2743                'C
-000010e0: 6f6e 6563 7461 7227 2c20 274c 6565 7245  onectar', 'LeerE
-000010f0: 7272 6f72 272c 2027 4c65 6572 5472 616e  rror', 'LeerTran
-00001100: 7361 6363 696f 6e27 2c0a 2020 2020 2020  saccion',.      
-00001110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001120: 2020 2753 6574 5573 6572 6e61 6d65 272c    'SetUsername',
-00001130: 2027 5365 7450 6173 7377 6f72 6427 2c0a   'SetPassword',.
-00001140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001150: 2020 2020 2020 2020 2753 6574 5061 7261          'SetPara
-00001160: 6d65 7472 6f27 2c20 2747 6574 5061 7261  metro', 'GetPara
-00001170: 6d65 7472 6f27 2c0a 2020 2020 2020 2020  metro',.        
-00001180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001190: 2747 6574 436f 6469 676f 5472 616e 7361  'GetCodigoTransa
-000011a0: 6363 696f 6e27 2c20 2747 6574 5265 7375  ccion', 'GetResu
-000011b0: 6c74 6164 6f27 2c20 274c 6f61 6454 6573  ltado', 'LoadTes
-000011c0: 7458 4d4c 275d 0a0a 2020 2020 5f70 7562  tXML']..    _pub
-000011d0: 6c69 635f 6174 7472 735f 203d 205b 0a20  lic_attrs_ = [. 
-000011e0: 2020 2020 2020 2027 5573 6572 6e61 6d65         'Username
-000011f0: 272c 2027 5061 7373 776f 7264 272c 0a20  ', 'Password',. 
-00001200: 2020 2020 2020 2027 436f 6469 676f 5472         'CodigoTr
-00001210: 616e 7361 6363 696f 6e27 2c20 2745 7272  ansaccion', 'Err
-00001220: 6f72 6573 272c 2027 5265 7375 6c74 6164  ores', 'Resultad
-00001230: 6f27 2c0a 2020 2020 2020 2020 2758 6d6c  o',.        'Xml
-00001240: 5265 7175 6573 7427 2c20 2758 6d6c 5265  Request', 'XmlRe
-00001250: 7370 6f6e 7365 272c 0a20 2020 2020 2020  sponse',.       
-00001260: 2027 5665 7273 696f 6e27 2c20 2749 6e73   'Version', 'Ins
-00001270: 7461 6c6c 4469 7227 2c0a 2020 2020 2020  tallDir',.      
-00001280: 2020 2754 7261 6365 6261 636b 272c 2027    'Traceback', '
-00001290: 4578 6365 7063 696f 6e27 2c20 274c 616e  Excepcion', 'Lan
-000012a0: 7a61 7245 7863 6570 6369 6f6e 6573 272c  zarExcepciones',
-000012b0: 0a20 2020 2020 2020 2027 4361 6e74 5061  .        'CantPa
-000012c0: 6769 6e61 7327 2c20 2748 6179 4572 726f  ginas', 'HayErro
-000012d0: 7227 2c20 2754 7261 6e73 6163 6369 6f6e  r', 'Transaccion
-000012e0: 506c 6169 6e57 5327 2c0a 2020 2020 2020  PlainWS',.      
-000012f0: 2020 5d0a 0a20 2020 205f 7265 675f 7072    ]..    _reg_pr
-00001300: 6f67 6964 5f20 3d20 2254 7261 7a61 4d65  ogid_ = "TrazaMe
-00001310: 6422 0a20 2020 205f 7265 675f 636c 7369  d".    _reg_clsi
-00001320: 645f 203d 2022 7b38 3437 3238 3637 412d  d_ = "{8472867A-
-00001330: 4145 3646 2d34 3837 462d 3835 3534 2d43  AE6F-487F-8554-C
-00001340: 3243 3839 3643 4646 4333 457d 220a 0a20  2C896CFFC3E}".. 
-00001350: 2020 2069 6620 5459 5045 4c49 423a 0a20     if TYPELIB:. 
-00001360: 2020 2020 2020 205f 7479 7065 6c69 625f         _typelib_
-00001370: 6775 6964 5f20 3d20 277b 4639 3932 4542  guid_ = '{F992EB
-00001380: 3745 2d41 4642 442d 3431 4242 2d42 3731  7E-AFBD-41BB-B71
-00001390: 372d 3536 3933 4433 4132 4241 4442 7d27  7-5693D3A2BADB}'
-000013a0: 0a20 2020 2020 2020 205f 7479 7065 6c69  .        _typeli
-000013b0: 625f 7665 7273 696f 6e5f 203d 2031 2c20  b_version_ = 1, 
-000013c0: 340a 2020 2020 2020 2020 5f63 6f6d 5f69  4.        _com_i
-000013d0: 6e74 6572 6661 6365 735f 203d 205b 2749  nterfaces_ = ['I
-000013e0: 5472 617a 614d 6564 275d 0a0a 2020 2020  TrazaMed']..    
-000013f0: 2320 5661 7269 6162 6c65 7320 676c 6f62  # Variables glob
-00001400: 616c 6573 2070 6172 6120 4261 7365 5753  ales para BaseWS
-00001410: 3a0a 2020 2020 484f 4d4f 203d 2048 4f4d  :.    HOMO = HOM
-00001420: 4f0a 2020 2020 5753 444c 203d 2057 5344  O.    WSDL = WSD
-00001430: 4c0a 2020 2020 5665 7273 696f 6e20 3d20  L.    Version = 
-00001440: 2225 7320 2573 2025 7322 2025 2028 5f5f  "%s %s %s" % (__
-00001450: 7665 7273 696f 6e5f 5f2c 2048 4f4d 4f20  version__, HOMO 
-00001460: 616e 6420 2748 6f6d 6f6c 6f67 6163 69f3  and 'Homologaci.
-00001470: 6e27 206f 7220 2727 2c0a 2020 2020 2020  n' or '',.      
-00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001490: 2020 2020 2020 7079 3373 696d 706c 6573        py3simples
-000014a0: 6f61 702e 636c 6965 6e74 2e5f 5f76 6572  oap.client.__ver
-000014b0: 7369 6f6e 5f5f 290a 0a20 2020 2064 6566  sion__)..    def
-000014c0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-000014d0: 7265 696e 7465 6e74 6f73 3d31 293a 0a20  reintentos=1):. 
-000014e0: 2020 2020 2020 2073 656c 662e 5573 6572         self.User
-000014f0: 6e61 6d65 203d 2073 656c 662e 5061 7373  name = self.Pass
-00001500: 776f 7264 203d 204e 6f6e 650a 2020 2020  word = None.    
-00001510: 2020 2020 7365 6c66 2e54 7261 6e73 6163      self.Transac
-00001520: 6369 6f6e 506c 6169 6e57 5320 3d20 5b5d  cionPlainWS = []
-00001530: 0a20 2020 2020 2020 2042 6173 6557 532e  .        BaseWS.
-00001540: 5f5f 696e 6974 5f5f 2873 656c 662c 2072  __init__(self, r
-00001550: 6569 6e74 656e 746f 7329 0a0a 2020 2020  eintentos)..    
-00001560: 6465 6620 696e 6963 6961 6c69 7a61 7228  def inicializar(
-00001570: 7365 6c66 293a 0a20 2020 2020 2020 2042  self):.        B
-00001580: 6173 6557 532e 696e 6963 6961 6c69 7a61  aseWS.inicializa
-00001590: 7228 7365 6c66 290a 2020 2020 2020 2020  r(self).        
-000015a0: 7365 6c66 2e43 6f64 6967 6f54 7261 6e73  self.CodigoTrans
-000015b0: 6163 6369 6f6e 203d 2073 656c 662e 4572  accion = self.Er
-000015c0: 726f 7265 7320 3d20 7365 6c66 2e52 6573  rores = self.Res
-000015d0: 756c 7461 646f 203d 204e 6f6e 650a 2020  ultado = None.  
-000015e0: 2020 2020 2020 7365 6c66 2e52 6573 756c        self.Resul
-000015f0: 7461 646f 203d 2027 270a 2020 2020 2020  tado = ''.      
-00001600: 2020 7365 6c66 2e45 7272 6f72 6573 203d    self.Errores =
-00001610: 205b 5d20 2020 2320 6c69 7374 6120 6465   []   # lista de
-00001620: 2073 7472 696e 6773 2070 6172 6120 6c61   strings para la
-00001630: 2069 6e74 6572 6661 7a0a 2020 2020 2020   interfaz.      
-00001640: 2020 7365 6c66 2e65 7272 6f72 6573 203d    self.errores =
-00001650: 205b 5d20 2020 2320 6c69 7374 6120 6465   []   # lista de
-00001660: 2064 6963 6369 6f6e 6172 696f 7320 2875   diccionarios (u
-00001670: 736f 2069 6e74 6572 6e6f 290a 2020 2020  so interno).    
-00001680: 2020 2020 7365 6c66 2e43 616e 7450 6167      self.CantPag
-00001690: 696e 6173 203d 2073 656c 662e 4861 7945  inas = self.HayE
-000016a0: 7272 6f72 203d 204e 6f6e 650a 0a20 2020  rror = None..   
-000016b0: 2064 6566 205f 5f61 6e61 6c69 7a61 725f   def __analizar_
-000016c0: 6572 726f 7265 7328 7365 6c66 2c20 7265  errores(self, re
-000016d0: 7429 3a0a 2020 2020 2020 2020 2243 6f6d  t):.        "Com
-000016e0: 7072 7565 6261 2079 2065 7874 7261 6520  prueba y extrae 
-000016f0: 6572 726f 7265 7320 7369 2065 7869 7374  errores si exist
-00001700: 656e 2065 6e20 6c61 2072 6573 7075 6573  en en la respues
-00001710: 7461 2058 4d4c 220a 2020 2020 2020 2020  ta XML".        
-00001720: 7365 6c66 2e65 7272 6f72 6573 203d 2072  self.errores = r
-00001730: 6574 2e67 6574 2827 6572 726f 7265 7327  et.get('errores'
-00001740: 2c20 5b5d 290a 2020 2020 2020 2020 7365  , []).        se
-00001750: 6c66 2e45 7272 6f72 6573 203d 205b 2225  lf.Errores = ["%
-00001760: 733a 2025 7322 2025 2028 6974 5b27 5f63  s: %s" % (it['_c
-00001770: 5f65 7272 6f72 275d 2c20 6974 5b27 5f64  _error'], it['_d
-00001780: 5f65 7272 6f72 275d 290a 2020 2020 2020  _error']).      
-00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017a0: 2020 666f 7220 6974 2069 6e20 7265 742e    for it in ret.
-000017b0: 6765 7428 2765 7272 6f72 6573 272c 205b  get('errores', [
-000017c0: 5d29 5d0a 2020 2020 2020 2020 7365 6c66  ])].        self
-000017d0: 2e52 6573 756c 7461 646f 203d 2072 6574  .Resultado = ret
-000017e0: 2e67 6574 2827 7265 7375 6c74 6164 6f27  .get('resultado'
-000017f0: 290a 0a20 2020 2064 6566 2043 6f6e 6563  )..    def Conec
-00001800: 7461 7228 0a20 2020 2020 2020 2073 656c  tar(.        sel
-00001810: 662c 2063 6163 6865 3d4e 6f6e 652c 2077  f, cache=None, w
-00001820: 7364 6c3d 4e6f 6e65 2c20 7072 6f78 793d  sdl=None, proxy=
-00001830: 2222 2c20 7772 6170 7065 723d 4e6f 6e65  "", wrapper=None
-00001840: 2c0a 2020 2020 2020 2020 6361 6365 7274  ,.        cacert
-00001850: 3d4e 6f6e 652c 2074 696d 656f 7574 3d33  =None, timeout=3
-00001860: 300a 2020 2020 293a 0a20 2020 2020 2020  0.    ):.       
-00001870: 2023 2043 6f6e 6563 746f 2075 7361 6e64   # Conecto usand
-00001880: 6f20 656c 206d e974 6f64 6f20 6573 7461  o el m.todo esta
-00001890: 6e64 6172 643a 0a20 2020 2020 2020 206f  ndard:.        o
-000018a0: 6b20 3d20 4261 7365 5753 2e43 6f6e 6563  k = BaseWS.Conec
-000018b0: 7461 7228 7365 6c66 2c20 6361 6368 652c  tar(self, cache,
-000018c0: 2077 7364 6c2c 2070 726f 7879 2c20 7772   wsdl, proxy, wr
-000018d0: 6170 7065 722c 2063 6163 6572 742c 0a20  apper, cacert,. 
-000018e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018f0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00001900: 6f75 742c 2073 6f61 705f 7365 7276 6572  out, soap_server
-00001910: 3d22 6a65 7474 7922 290a 0a20 2020 2020  ="jetty")..     
-00001920: 2020 2069 6620 6f6b 3a0a 2020 2020 2020     if ok:.      
-00001930: 2020 2020 2020 2320 7369 2065 6c20 6172        # si el ar
-00001940: 6368 6976 6f20 6573 206c 6f63 616c 2c20  chivo es local, 
-00001950: 6173 756d 6f20 7175 6520 7961 2065 7374  asumo que ya est
-00001960: 6120 636f 7272 6567 6964 6f3a 0a20 2020  a corregido:.   
-00001970: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00001980: 7365 6c66 2e77 7364 6c2e 7374 6172 7473  self.wsdl.starts
-00001990: 7769 7468 2822 6669 6c65 2229 3a0a 2020  with("file"):.  
-000019a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000019b0: 636f 7272 696a 6f20 7562 6963 6163 69f3  corrijo ubicaci.
-000019c0: 6e20 6465 6c20 7365 7276 6964 6f72 2028  n del servidor (
-000019d0: 6c6f 6361 6c68 6f73 743a 3930 3530 2065  localhost:9050 e
-000019e0: 6e20 656c 2057 5344 4c29 0a20 2020 2020  n el WSDL).     
-000019f0: 2020 2020 2020 2020 2020 206c 6f63 6174             locat
-00001a00: 696f 6e20 3d20 7365 6c66 2e77 7364 6c5b  ion = self.wsdl[
-00001a10: 3a2d 355d 0a20 2020 2020 2020 2020 2020  :-5].           
-00001a20: 2020 2020 2069 6620 2749 5765 6253 6572       if 'IWebSer
-00001a30: 7669 6365 5365 7276 6963 6527 2069 6e20  viceService' in 
-00001a40: 7365 6c66 2e63 6c69 656e 742e 7365 7276  self.client.serv
-00001a50: 6963 6573 3a0a 2020 2020 2020 2020 2020  ices:.          
-00001a60: 2020 2020 2020 2020 2020 2320 7665 7273            # vers
-00001a70: 696f 6e20 310a 2020 2020 2020 2020 2020  ion 1.          
-00001a80: 2020 2020 2020 2020 2020 7773 203d 2073            ws = s
-00001a90: 656c 662e 636c 6965 6e74 2e73 6572 7669  elf.client.servi
-00001aa0: 6365 735b 2749 5765 6253 6572 7669 6365  ces['IWebService
-00001ab0: 5365 7276 6963 6527 5d0a 2020 2020 2020  Service'].      
-00001ac0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ae0: 2020 2020 7773 203d 2073 656c 662e 636c      ws = self.cl
-00001af0: 6965 6e74 2e73 6572 7669 6365 735b 2749  ient.services['I
-00001b00: 5765 6253 6572 7669 6365 275d 2020 2023  WebService']   #
-00001b10: 2076 6572 7369 6f6e 2032 0a20 2020 2020   version 2.     
-00001b20: 2020 2020 2020 2020 2020 2077 735b 2770             ws['p
-00001b30: 6f72 7473 275d 5b27 4957 6562 5365 7276  orts']['IWebServ
-00001b40: 6963 6550 6f72 7427 5d5b 276c 6f63 6174  icePort']['locat
-00001b50: 696f 6e27 5d20 3d20 6c6f 6361 7469 6f6e  ion'] = location
-00001b60: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00001b70: 4573 7461 626c 6563 6572 2063 7265 6465  Establecer crede
-00001b80: 6e63 6961 6c65 7320 6465 2073 6567 7572  nciales de segur
-00001b90: 6964 6164 3a0a 2020 2020 2020 2020 2020  idad:.          
-00001ba0: 2020 7365 6c66 2e63 6c69 656e 745b 2777    self.client['w
-00001bb0: 7373 653a 5365 6375 7269 7479 275d 203d  sse:Security'] =
-00001bc0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00001bd0: 2020 2027 7773 7365 3a55 7365 726e 616d     'wsse:Usernam
-00001be0: 6554 6f6b 656e 273a 207b 0a20 2020 2020  eToken': {.     
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001c00: 7773 7365 3a55 7365 726e 616d 6527 3a20  wsse:Username': 
-00001c10: 7365 6c66 2e55 7365 726e 616d 652c 0a20  self.Username,. 
-00001c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c30: 2020 2027 7773 7365 3a50 6173 7377 6f72     'wsse:Passwor
-00001c40: 6427 3a20 7365 6c66 2e50 6173 7377 6f72  d': self.Passwor
-00001c50: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00001c60: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00001c70: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00001c80: 2020 2072 6574 7572 6e20 6f6b 0a0a 2020     return ok..  
-00001c90: 2020 4069 6e69 6369 616c 697a 6172 5f79    @inicializar_y
-00001ca0: 5f63 6170 7475 7261 725f 6578 6365 7063  _capturar_excepc
-00001cb0: 696f 6e65 730a 2020 2020 6465 6620 5365  iones.    def Se
-00001cc0: 6e64 4d65 6469 6361 6d65 6e74 6f73 2873  ndMedicamentos(s
-00001cd0: 656c 662c 2075 7375 6172 696f 2c20 7061  elf, usuario, pa
-00001ce0: 7373 776f 7264 2c0a 2020 2020 2020 2020  ssword,.        
-00001cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d00: 2066 5f65 7665 6e74 6f2c 2068 5f65 7665   f_evento, h_eve
-00001d10: 6e74 6f2c 2067 6c6e 5f6f 7269 6765 6e2c  nto, gln_origen,
-00001d20: 2067 6c6e 5f64 6573 7469 6e6f 2c0a 2020   gln_destino,.  
-00001d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d40: 2020 2020 2020 206e 5f72 656d 6974 6f2c         n_remito,
-00001d50: 206e 5f66 6163 7475 7261 2c20 7665 6e63   n_factura, venc
-00001d60: 696d 6965 6e74 6f2c 2067 7469 6e2c 206c  imiento, gtin, l
-00001d70: 6f74 652c 0a20 2020 2020 2020 2020 2020  ote,.           
-00001d80: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00001d90: 6d65 726f 5f73 6572 6961 6c2c 2069 645f  mero_serial, id_
-00001da0: 6f62 7261 5f73 6f63 6961 6c2c 2069 645f  obra_social, id_
-00001db0: 6576 656e 746f 2c0a 2020 2020 2020 2020  evento,.        
-00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001dd0: 2063 7569 745f 6f72 6967 656e 3d27 272c   cuit_origen='',
-00001de0: 2063 7569 745f 6465 7374 696e 6f3d 2727   cuit_destino=''
-00001df0: 2c20 6170 656c 6c69 646f 3d27 272c 0a20  , apellido='',. 
-00001e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e10: 2020 2020 2020 2020 6e6f 6d62 7265 733d          nombres=
-00001e20: 2727 2c20 7469 706f 5f64 6f63 756d 656e  '', tipo_documen
-00001e30: 746f 3d27 272c 206e 5f64 6f63 756d 656e  to='', n_documen
-00001e40: 746f 3d27 272c 0a20 2020 2020 2020 2020  to='',.         
-00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e60: 7365 786f 3d27 272c 2064 6972 6563 6369  sexo='', direcci
-00001e70: 6f6e 3d27 272c 206e 756d 6572 6f3d 2727  on='', numero=''
-00001e80: 2c20 7069 736f 3d27 272c 0a20 2020 2020  , piso='',.     
-00001e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ea0: 2020 2020 6465 7074 6f3d 2727 2c20 6c6f      depto='', lo
-00001eb0: 6361 6c69 6461 643d 2727 2c20 7072 6f76  calidad='', prov
-00001ec0: 696e 6369 613d 2727 2c0a 2020 2020 2020  incia='',.      
-00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ee0: 2020 206e 5f70 6f73 7461 6c3d 2727 2c20     n_postal='', 
-00001ef0: 6665 6368 615f 6e61 6369 6d69 656e 746f  fecha_nacimiento
-00001f00: 3d27 272c 2074 656c 6566 6f6e 6f3d 2727  ='', telefono=''
-00001f10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001f20: 2020 2020 2020 2020 2020 206e 726f 5f61             nro_a
-00001f30: 736f 6369 6164 6f3d 4e6f 6e65 2c0a 2020  sociado=None,.  
-00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f50: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00001f60: 2020 2252 6561 6c69 7a61 2065 6c20 7265    "Realiza el re
-00001f70: 6769 7374 726f 2064 6520 756e 6120 7472  gistro de una tr
-00001f80: 616e 7361 6363 69f3 6e20 6465 206d 6564  ansacci.n de med
-00001f90: 6963 616d 656e 746f 732e 2022 0a20 2020  icamentos. ".   
-00001fa0: 2020 2020 2023 2063 7265 6f20 6c6f 7320       # creo los 
-00001fb0: 7061 72e1 6d65 7472 6f73 2070 6172 6120  par.metros para 
-00001fc0: 6573 7461 206c 6c61 6d61 6461 0a20 2020  esta llamada.   
-00001fd0: 2020 2020 2070 6172 616d 7320 3d20 7b0a       params = {.
-00001fe0: 2020 2020 2020 2020 2020 2020 2766 5f65              'f_e
-00001ff0: 7665 6e74 6f27 3a20 665f 6576 656e 746f  vento': f_evento
-00002000: 2c0a 2020 2020 2020 2020 2020 2020 2768  ,.            'h
-00002010: 5f65 7665 6e74 6f27 3a20 685f 6576 656e  _evento': h_even
-00002020: 746f 2c0a 2020 2020 2020 2020 2020 2020  to,.            
-00002030: 2767 6c6e 5f6f 7269 6765 6e27 3a20 676c  'gln_origen': gl
-00002040: 6e5f 6f72 6967 656e 2c0a 2020 2020 2020  n_origen,.      
-00002050: 2020 2020 2020 2767 6c6e 5f64 6573 7469        'gln_desti
-00002060: 6e6f 273a 2067 6c6e 5f64 6573 7469 6e6f  no': gln_destino
-00002070: 2c0a 2020 2020 2020 2020 2020 2020 276e  ,.            'n
-00002080: 5f72 656d 6974 6f27 3a20 6e5f 7265 6d69  _remito': n_remi
-00002090: 746f 2c0a 2020 2020 2020 2020 2020 2020  to,.            
-000020a0: 276e 5f66 6163 7475 7261 273a 206e 5f66  'n_factura': n_f
-000020b0: 6163 7475 7261 2c0a 2020 2020 2020 2020  actura,.        
-000020c0: 2020 2020 2776 656e 6369 6d69 656e 746f      'vencimiento
-000020d0: 273a 2076 656e 6369 6d69 656e 746f 2c0a  ': vencimiento,.
-000020e0: 2020 2020 2020 2020 2020 2020 2767 7469              'gti
-000020f0: 6e27 3a20 6774 696e 2c0a 2020 2020 2020  n': gtin,.      
-00002100: 2020 2020 2020 276c 6f74 6527 3a20 6c6f        'lote': lo
-00002110: 7465 2c0a 2020 2020 2020 2020 2020 2020  te,.            
-00002120: 276e 756d 6572 6f5f 7365 7269 616c 273a  'numero_serial':
-00002130: 206e 756d 6572 6f5f 7365 7269 616c 2c0a   numero_serial,.
-00002140: 2020 2020 2020 2020 2020 2020 2769 645f              'id_
-00002150: 6f62 7261 5f73 6f63 6961 6c27 3a20 6964  obra_social': id
-00002160: 5f6f 6272 615f 736f 6369 616c 206f 7220  _obra_social or 
-00002170: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00002180: 2020 2769 645f 6576 656e 746f 273a 2069    'id_evento': i
-00002190: 645f 6576 656e 746f 2c0a 2020 2020 2020  d_evento,.      
-000021a0: 2020 2020 2020 2763 7569 745f 6f72 6967        'cuit_orig
-000021b0: 656e 273a 2063 7569 745f 6f72 6967 656e  en': cuit_origen
-000021c0: 2c0a 2020 2020 2020 2020 2020 2020 2763  ,.            'c
-000021d0: 7569 745f 6465 7374 696e 6f27 3a20 6375  uit_destino': cu
-000021e0: 6974 5f64 6573 7469 6e6f 2c0a 2020 2020  it_destino,.    
-000021f0: 2020 2020 2020 2020 2761 7065 6c6c 6964          'apellid
-00002200: 6f27 3a20 6170 656c 6c69 646f 2c0a 2020  o': apellido,.  
-00002210: 2020 2020 2020 2020 2020 276e 6f6d 6272            'nombr
-00002220: 6573 273a 206e 6f6d 6272 6573 2c0a 2020  es': nombres,.  
-00002230: 2020 2020 2020 2020 2020 2774 6970 6f5f            'tipo_
-00002240: 646f 6375 6d65 6e74 6f27 3a20 7469 706f  documento': tipo
-00002250: 5f64 6f63 756d 656e 746f 2c0a 2020 2020  _documento,.    
-00002260: 2020 2020 2020 2020 276e 5f64 6f63 756d          'n_docum
-00002270: 656e 746f 273a 206e 5f64 6f63 756d 656e  ento': n_documen
-00002280: 746f 2c0a 2020 2020 2020 2020 2020 2020  to,.            
-00002290: 2773 6578 6f27 3a20 7365 786f 2c0a 2020  'sexo': sexo,.  
-000022a0: 2020 2020 2020 2020 2020 2764 6972 6563            'direc
-000022b0: 6369 6f6e 273a 2064 6972 6563 6369 6f6e  cion': direccion
-000022c0: 2c0a 2020 2020 2020 2020 2020 2020 276e  ,.            'n
-000022d0: 756d 6572 6f27 3a20 6e75 6d65 726f 2c0a  umero': numero,.
-000022e0: 2020 2020 2020 2020 2020 2020 2770 6973              'pis
-000022f0: 6f27 3a20 7069 736f 2c0a 2020 2020 2020  o': piso,.      
-00002300: 2020 2020 2020 2764 6570 746f 273a 2064        'depto': d
-00002310: 6570 746f 2c0a 2020 2020 2020 2020 2020  epto,.          
-00002320: 2020 276c 6f63 616c 6964 6164 273a 206c    'localidad': l
-00002330: 6f63 616c 6964 6164 2c0a 2020 2020 2020  ocalidad,.      
-00002340: 2020 2020 2020 2770 726f 7669 6e63 6961        'provincia
-00002350: 273a 2070 726f 7669 6e63 6961 2c0a 2020  ': provincia,.  
-00002360: 2020 2020 2020 2020 2020 276e 5f70 6f73            'n_pos
-00002370: 7461 6c27 3a20 6e5f 706f 7374 616c 2c0a  tal': n_postal,.
-00002380: 2020 2020 2020 2020 2020 2020 2766 6563              'fec
-00002390: 6861 5f6e 6163 696d 6965 6e74 6f27 3a20  ha_nacimiento': 
-000023a0: 6665 6368 615f 6e61 6369 6d69 656e 746f  fecha_nacimiento
-000023b0: 2c0a 2020 2020 2020 2020 2020 2020 2774  ,.            't
-000023c0: 656c 6566 6f6e 6f27 3a20 7465 6c65 666f  elefono': telefo
-000023d0: 6e6f 2c0a 2020 2020 2020 2020 2020 2020  no,.            
-000023e0: 276e 726f 5f61 736f 6369 6164 6f27 3a20  'nro_asociado': 
-000023f0: 6e72 6f5f 6173 6f63 6961 646f 2c0a 2020  nro_asociado,.  
-00002400: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00002410: 7265 7320 3d20 7365 6c66 2e63 6c69 656e  res = self.clien
-00002420: 742e 7365 6e64 4d65 6469 6361 6d65 6e74  t.sendMedicament
-00002430: 6f73 280a 2020 2020 2020 2020 2020 2020  os(.            
-00002440: 6172 6730 3d70 6172 616d 732c 0a20 2020  arg0=params,.   
-00002450: 2020 2020 2020 2020 2061 7267 313d 7573           arg1=us
-00002460: 7561 7269 6f2c 0a20 2020 2020 2020 2020  uario,.         
-00002470: 2020 2061 7267 323d 7061 7373 776f 7264     arg2=password
-00002480: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00002490: 2020 2020 2072 6574 203d 2072 6573 5b27       ret = res['
-000024a0: 7265 7475 726e 275d 0a0a 2020 2020 2020  return']..      
-000024b0: 2020 7365 6c66 2e43 6f64 6967 6f54 7261    self.CodigoTra
-000024c0: 6e73 6163 6369 6f6e 203d 2072 6574 5b27  nsaccion = ret['
-000024d0: 636f 6469 676f 5472 616e 7361 6363 696f  codigoTransaccio
-000024e0: 6e27 5d0a 2020 2020 2020 2020 7365 6c66  n'].        self
-000024f0: 2e5f 5f61 6e61 6c69 7a61 725f 6572 726f  .__analizar_erro
-00002500: 7265 7328 7265 7429 0a0a 2020 2020 2020  res(ret)..      
-00002510: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
-00002520: 2020 2040 696e 6963 6961 6c69 7a61 725f     @inicializar_
-00002530: 795f 6361 7074 7572 6172 5f65 7863 6570  y_capturar_excep
-00002540: 6369 6f6e 6573 0a20 2020 2064 6566 2053  ciones.    def S
-00002550: 656e 644d 6564 6963 616d 656e 746f 7346  endMedicamentosF
-00002560: 7261 6363 696f 6e28 0a20 2020 2020 2020  raccion(.       
-00002570: 2073 656c 662c 2075 7375 6172 696f 2c20   self, usuario, 
-00002580: 7061 7373 776f 7264 2c0a 2020 2020 2020  password,.      
-00002590: 2020 665f 6576 656e 746f 2c20 685f 6576    f_evento, h_ev
-000025a0: 656e 746f 2c20 676c 6e5f 6f72 6967 656e  ento, gln_origen
-000025b0: 2c20 676c 6e5f 6465 7374 696e 6f2c 0a20  , gln_destino,. 
-000025c0: 2020 2020 2020 206e 5f72 656d 6974 6f2c         n_remito,
-000025d0: 206e 5f66 6163 7475 7261 2c20 7665 6e63   n_factura, venc
-000025e0: 696d 6965 6e74 6f2c 2067 7469 6e2c 206c  imiento, gtin, l
-000025f0: 6f74 652c 0a20 2020 2020 2020 206e 756d  ote,.        num
-00002600: 6572 6f5f 7365 7269 616c 2c20 6964 5f6f  ero_serial, id_o
-00002610: 6272 615f 736f 6369 616c 2c20 6964 5f65  bra_social, id_e
-00002620: 7665 6e74 6f2c 0a20 2020 2020 2020 2063  vento,.        c
-00002630: 7569 745f 6f72 6967 656e 3d27 272c 2063  uit_origen='', c
-00002640: 7569 745f 6465 7374 696e 6f3d 2727 2c20  uit_destino='', 
-00002650: 6170 656c 6c69 646f 3d27 272c 206e 6f6d  apellido='', nom
-00002660: 6272 6573 3d27 272c 0a20 2020 2020 2020  bres='',.       
-00002670: 2074 6970 6f5f 646f 6375 6d65 6e74 6f3d   tipo_documento=
-00002680: 2727 2c20 6e5f 646f 6375 6d65 6e74 6f3d  '', n_documento=
-00002690: 2727 2c20 7365 786f 3d27 272c 0a20 2020  '', sexo='',.   
-000026a0: 2020 2020 2064 6972 6563 6369 6f6e 3d27       direccion='
-000026b0: 272c 206e 756d 6572 6f3d 2727 2c20 7069  ', numero='', pi
-000026c0: 736f 3d27 272c 2064 6570 746f 3d27 272c  so='', depto='',
-000026d0: 206c 6f63 616c 6964 6164 3d27 272c 2070   localidad='', p
-000026e0: 726f 7669 6e63 6961 3d27 272c 0a20 2020  rovincia='',.   
-000026f0: 2020 2020 206e 5f70 6f73 7461 6c3d 2727       n_postal=''
-00002700: 2c20 6665 6368 615f 6e61 6369 6d69 656e  , fecha_nacimien
-00002710: 746f 3d27 272c 2074 656c 6566 6f6e 6f3d  to='', telefono=
-00002720: 2727 2c0a 2020 2020 2020 2020 6e72 6f5f  '',.        nro_
-00002730: 6173 6f63 6961 646f 3d4e 6f6e 652c 2063  asociado=None, c
-00002740: 616e 7469 6461 643d 4e6f 6e65 2c0a 2020  antidad=None,.  
-00002750: 2020 293a 0a20 2020 2020 2020 2022 5265    ):.        "Re
-00002760: 616c 697a 6120 656c 2072 6567 6973 7472  aliza el registr
-00002770: 6f20 6465 2075 6e61 2074 7261 6e73 6163  o de una transac
-00002780: 6369 f36e 2064 6520 6d65 6469 6361 6d65  ci.n de medicame
-00002790: 6e74 6f73 2066 7261 6363 696f 6e61 646f  ntos fraccionado
-000027a0: 7322 0a20 2020 2020 2020 2023 2063 7265  s".        # cre
-000027b0: 6f20 6c6f 7320 7061 72e1 6d65 7472 6f73  o los par.metros
-000027c0: 2070 6172 6120 6573 7461 206c 6c61 6d61   para esta llama
-000027d0: 6461 0a20 2020 2020 2020 2070 6172 616d  da.        param
-000027e0: 7320 3d20 7b0a 2020 2020 2020 2020 2020  s = {.          
-000027f0: 2020 2766 5f65 7665 6e74 6f27 3a20 665f    'f_evento': f_
-00002800: 6576 656e 746f 2c0a 2020 2020 2020 2020  evento,.        
-00002810: 2020 2020 2768 5f65 7665 6e74 6f27 3a20      'h_evento': 
-00002820: 685f 6576 656e 746f 2c0a 2020 2020 2020  h_evento,.      
-00002830: 2020 2020 2020 2767 6c6e 5f6f 7269 6765        'gln_orige
-00002840: 6e27 3a20 676c 6e5f 6f72 6967 656e 2c0a  n': gln_origen,.
-00002850: 2020 2020 2020 2020 2020 2020 2767 6c6e              'gln
-00002860: 5f64 6573 7469 6e6f 273a 2067 6c6e 5f64  _destino': gln_d
-00002870: 6573 7469 6e6f 2c0a 2020 2020 2020 2020  estino,.        
-00002880: 2020 2020 276e 5f72 656d 6974 6f27 3a20      'n_remito': 
-00002890: 6e5f 7265 6d69 746f 2c0a 2020 2020 2020  n_remito,.      
-000028a0: 2020 2020 2020 276e 5f66 6163 7475 7261        'n_factura
-000028b0: 273a 206e 5f66 6163 7475 7261 2c0a 2020  ': n_factura,.  
-000028c0: 2020 2020 2020 2020 2020 2776 656e 6369            'venci
-000028d0: 6d69 656e 746f 273a 2076 656e 6369 6d69  miento': vencimi
-000028e0: 656e 746f 2c0a 2020 2020 2020 2020 2020  ento,.          
-000028f0: 2020 2767 7469 6e27 3a20 6774 696e 2c0a    'gtin': gtin,.
-00002900: 2020 2020 2020 2020 2020 2020 276c 6f74              'lot
-00002910: 6527 3a20 6c6f 7465 2c0a 2020 2020 2020  e': lote,.      
-00002920: 2020 2020 2020 276e 756d 6572 6f5f 7365        'numero_se
-00002930: 7269 616c 273a 206e 756d 6572 6f5f 7365  rial': numero_se
-00002940: 7269 616c 2c0a 2020 2020 2020 2020 2020  rial,.          
-00002950: 2020 2769 645f 6f62 7261 5f73 6f63 6961    'id_obra_socia
-00002960: 6c27 3a20 6964 5f6f 6272 615f 736f 6369  l': id_obra_soci
-00002970: 616c 206f 7220 4e6f 6e65 2c0a 2020 2020  al or None,.    
-00002980: 2020 2020 2020 2020 2769 645f 6576 656e          'id_even
-00002990: 746f 273a 2069 645f 6576 656e 746f 2c0a  to': id_evento,.
-000029a0: 2020 2020 2020 2020 2020 2020 2763 7569              'cui
-000029b0: 745f 6f72 6967 656e 273a 2063 7569 745f  t_origen': cuit_
-000029c0: 6f72 6967 656e 2c0a 2020 2020 2020 2020  origen,.        
-000029d0: 2020 2020 2763 7569 745f 6465 7374 696e      'cuit_destin
-000029e0: 6f27 3a20 6375 6974 5f64 6573 7469 6e6f  o': cuit_destino
-000029f0: 2c0a 2020 2020 2020 2020 2020 2020 2761  ,.            'a
-00002a00: 7065 6c6c 6964 6f27 3a20 6170 656c 6c69  pellido': apelli
-00002a10: 646f 2c0a 2020 2020 2020 2020 2020 2020  do,.            
-00002a20: 276e 6f6d 6272 6573 273a 206e 6f6d 6272  'nombres': nombr
-00002a30: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00002a40: 2774 6970 6f5f 646f 6375 6d65 6e74 6f27  'tipo_documento'
-00002a50: 3a20 7469 706f 5f64 6f63 756d 656e 746f  : tipo_documento
-00002a60: 2c0a 2020 2020 2020 2020 2020 2020 276e  ,.            'n
-00002a70: 5f64 6f63 756d 656e 746f 273a 206e 5f64  _documento': n_d
-00002a80: 6f63 756d 656e 746f 2c0a 2020 2020 2020  ocumento,.      
-00002a90: 2020 2020 2020 2773 6578 6f27 3a20 7365        'sexo': se
-00002aa0: 786f 2c0a 2020 2020 2020 2020 2020 2020  xo,.            
-00002ab0: 2764 6972 6563 6369 6f6e 273a 2064 6972  'direccion': dir
-00002ac0: 6563 6369 6f6e 2c0a 2020 2020 2020 2020  eccion,.        
-00002ad0: 2020 2020 276e 756d 6572 6f27 3a20 6e75      'numero': nu
-00002ae0: 6d65 726f 2c0a 2020 2020 2020 2020 2020  mero,.          
-00002af0: 2020 2770 6973 6f27 3a20 7069 736f 2c0a    'piso': piso,.
-00002b00: 2020 2020 2020 2020 2020 2020 2764 6570              'dep
-00002b10: 746f 273a 2064 6570 746f 2c0a 2020 2020  to': depto,.    
-00002b20: 2020 2020 2020 2020 276c 6f63 616c 6964          'localid
-00002b30: 6164 273a 206c 6f63 616c 6964 6164 2c0a  ad': localidad,.
-00002b40: 2020 2020 2020 2020 2020 2020 2770 726f              'pro
-00002b50: 7669 6e63 6961 273a 2070 726f 7669 6e63  vincia': provinc
-00002b60: 6961 2c0a 2020 2020 2020 2020 2020 2020  ia,.            
-00002b70: 276e 5f70 6f73 7461 6c27 3a20 6e5f 706f  'n_postal': n_po
-00002b80: 7374 616c 2c0a 2020 2020 2020 2020 2020  stal,.          
-00002b90: 2020 2766 6563 6861 5f6e 6163 696d 6965    'fecha_nacimie
-00002ba0: 6e74 6f27 3a20 6665 6368 615f 6e61 6369  nto': fecha_naci
-00002bb0: 6d69 656e 746f 2c0a 2020 2020 2020 2020  miento,.        
-00002bc0: 2020 2020 2774 656c 6566 6f6e 6f27 3a20      'telefono': 
-00002bd0: 7465 6c65 666f 6e6f 2c0a 2020 2020 2020  telefono,.      
-00002be0: 2020 2020 2020 276e 726f 5f61 736f 6369        'nro_asoci
-00002bf0: 6164 6f27 3a20 6e72 6f5f 6173 6f63 6961  ado': nro_asocia
-00002c00: 646f 2c0a 2020 2020 2020 2020 2020 2020  do,.            
-00002c10: 2763 616e 7469 6461 6427 3a20 6361 6e74  'cantidad': cant
-00002c20: 6964 6164 2c0a 2020 2020 2020 2020 7d0a  idad,.        }.
-00002c30: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
-00002c40: 6c66 2e63 6c69 656e 742e 7365 6e64 4d65  lf.client.sendMe
-00002c50: 6469 6361 6d65 6e74 6f73 4672 6163 6369  dicamentosFracci
-00002c60: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00002c70: 6172 6730 3d70 6172 616d 732c 0a20 2020  arg0=params,.   
-00002c80: 2020 2020 2020 2020 2061 7267 313d 7573           arg1=us
-00002c90: 7561 7269 6f2c 0a20 2020 2020 2020 2020  uario,.         
-00002ca0: 2020 2061 7267 323d 7061 7373 776f 7264     arg2=password
-00002cb0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00002cc0: 2020 2020 2072 6574 203d 2072 6573 5b27       ret = res['
-00002cd0: 7265 7475 726e 275d 0a0a 2020 2020 2020  return']..      
-00002ce0: 2020 7365 6c66 2e43 6f64 6967 6f54 7261    self.CodigoTra
-00002cf0: 6e73 6163 6369 6f6e 203d 2072 6574 5b27  nsaccion = ret['
-00002d00: 636f 6469 676f 5472 616e 7361 6363 696f  codigoTransaccio
-00002d10: 6e27 5d0a 2020 2020 2020 2020 7365 6c66  n'].        self
-00002d20: 2e5f 5f61 6e61 6c69 7a61 725f 6572 726f  .__analizar_erro
-00002d30: 7265 7328 7265 7429 0a0a 2020 2020 2020  res(ret)..      
-00002d40: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
-00002d50: 2020 2040 696e 6963 6961 6c69 7a61 725f     @inicializar_
-00002d60: 795f 6361 7074 7572 6172 5f65 7863 6570  y_capturar_excep
-00002d70: 6369 6f6e 6573 0a20 2020 2064 6566 2053  ciones.    def S
-00002d80: 656e 644d 6564 6963 616d 656e 746f 7344  endMedicamentosD
-00002d90: 4853 6572 6965 280a 2020 2020 2020 2020  HSerie(.        
-00002da0: 7365 6c66 2c20 7573 7561 7269 6f2c 2070  self, usuario, p
-00002db0: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
-00002dc0: 2066 5f65 7665 6e74 6f2c 2068 5f65 7665   f_evento, h_eve
-00002dd0: 6e74 6f2c 2067 6c6e 5f6f 7269 6765 6e2c  nto, gln_origen,
-00002de0: 2067 6c6e 5f64 6573 7469 6e6f 2c0a 2020   gln_destino,.  
-00002df0: 2020 2020 2020 6e5f 7265 6d69 746f 2c20        n_remito, 
-00002e00: 6e5f 6661 6374 7572 612c 2076 656e 6369  n_factura, venci
-00002e10: 6d69 656e 746f 2c20 6774 696e 2c20 6c6f  miento, gtin, lo
-00002e20: 7465 2c0a 2020 2020 2020 2020 6465 7364  te,.        desd
-00002e30: 655f 6e75 6d65 726f 5f73 6572 6961 6c2c  e_numero_serial,
-00002e40: 2068 6173 7461 5f6e 756d 6572 6f5f 7365   hasta_numero_se
-00002e50: 7269 616c 2c0a 2020 2020 2020 2020 6964  rial,.        id
-00002e60: 5f6f 6272 615f 736f 6369 616c 2c20 6964  _obra_social, id
-00002e70: 5f65 7665 6e74 6f2c 0a20 2020 2020 2020  _evento,.       
-00002e80: 2063 7569 745f 6f72 6967 656e 3d27 272c   cuit_origen='',
-00002e90: 2063 7569 745f 6465 7374 696e 6f3d 2727   cuit_destino=''
-00002ea0: 2c20 6170 656c 6c69 646f 3d27 272c 206e  , apellido='', n
-00002eb0: 6f6d 6272 6573 3d27 272c 0a20 2020 2020  ombres='',.     
-00002ec0: 2020 2074 6970 6f5f 646f 6375 6d65 6e74     tipo_document
-00002ed0: 6f3d 2727 2c20 6e5f 646f 6375 6d65 6e74  o='', n_document
-00002ee0: 6f3d 2727 2c20 7365 786f 3d27 272c 0a20  o='', sexo='',. 
-00002ef0: 2020 2020 2020 2064 6972 6563 6369 6f6e         direccion
-00002f00: 3d27 272c 206e 756d 6572 6f3d 2727 2c20  ='', numero='', 
-00002f10: 7069 736f 3d27 272c 2064 6570 746f 3d27  piso='', depto='
-00002f20: 272c 206c 6f63 616c 6964 6164 3d27 272c  ', localidad='',
-00002f30: 2070 726f 7669 6e63 6961 3d27 272c 0a20   provincia='',. 
-00002f40: 2020 2020 2020 206e 5f70 6f73 7461 6c3d         n_postal=
-00002f50: 2727 2c20 6665 6368 615f 6e61 6369 6d69  '', fecha_nacimi
-00002f60: 656e 746f 3d27 272c 2074 656c 6566 6f6e  ento='', telefon
-00002f70: 6f3d 2727 2c0a 2020 2020 2020 2020 6e72  o='',.        nr
-00002f80: 6f5f 6173 6f63 6961 646f 3d4e 6f6e 652c  o_asociado=None,
-00002f90: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00002fa0: 2245 6e76 ed61 2075 6e20 6c6f 7465 2064  "Env.a un lote d
-00002fb0: 6520 6d65 6469 6361 6d65 6e74 6f73 2069  e medicamentos i
-00002fc0: 6e66 6f72 6d61 6e64 6f20 656c 2064 6573  nformando el des
-00002fd0: 6465 2d68 6173 7461 206e fa6d 6572 6f20  de-hasta n.mero 
-00002fe0: 6465 205c 0a20 2020 2020 2020 2020 2020  de \.           
-00002ff0: 2073 6572 6965 220a 2020 2020 2020 2020   serie".        
-00003000: 2320 6372 656f 206c 6f73 2070 6172 e16d  # creo los par.m
-00003010: 6574 726f 7320 7061 7261 2065 7374 6120  etros para esta 
-00003020: 6c6c 616d 6164 610a 2020 2020 2020 2020  llamada.        
-00003030: 7061 7261 6d73 203d 207b 0a20 2020 2020  params = {.     
-00003040: 2020 2020 2020 2027 665f 6576 656e 746f         'f_evento
-00003050: 273a 2066 5f65 7665 6e74 6f2c 0a20 2020  ': f_evento,.   
-00003060: 2020 2020 2020 2020 2027 685f 6576 656e           'h_even
-00003070: 746f 273a 2068 5f65 7665 6e74 6f2c 0a20  to': h_evento,. 
-00003080: 2020 2020 2020 2020 2020 2027 676c 6e5f             'gln_
-00003090: 6f72 6967 656e 273a 2067 6c6e 5f6f 7269  origen': gln_ori
-000030a0: 6765 6e2c 0a20 2020 2020 2020 2020 2020  gen,.           
-000030b0: 2027 676c 6e5f 6465 7374 696e 6f27 3a20   'gln_destino': 
-000030c0: 676c 6e5f 6465 7374 696e 6f2c 0a20 2020  gln_destino,.   
-000030d0: 2020 2020 2020 2020 2027 6e5f 7265 6d69           'n_remi
-000030e0: 746f 273a 206e 5f72 656d 6974 6f2c 0a20  to': n_remito,. 
-000030f0: 2020 2020 2020 2020 2020 2027 6e5f 6661             'n_fa
-00003100: 6374 7572 6127 3a20 6e5f 6661 6374 7572  ctura': n_factur
-00003110: 612c 0a20 2020 2020 2020 2020 2020 2027  a,.            '
-00003120: 7665 6e63 696d 6965 6e74 6f27 3a20 7665  vencimiento': ve
-00003130: 6e63 696d 6965 6e74 6f2c 0a20 2020 2020  ncimiento,.     
-00003140: 2020 2020 2020 2027 6774 696e 273a 2067         'gtin': g
-00003150: 7469 6e2c 0a20 2020 2020 2020 2020 2020  tin,.           
-00003160: 2027 6c6f 7465 273a 206c 6f74 652c 0a20   'lote': lote,. 
-00003170: 2020 2020 2020 2020 2020 2027 6465 7364             'desd
-00003180: 655f 6e75 6d65 726f 5f73 6572 6961 6c27  e_numero_serial'
-00003190: 3a20 6465 7364 655f 6e75 6d65 726f 5f73  : desde_numero_s
-000031a0: 6572 6961 6c2c 0a20 2020 2020 2020 2020  erial,.         
-000031b0: 2020 2027 6861 7374 615f 6e75 6d65 726f     'hasta_numero
-000031c0: 5f73 6572 6961 6c27 3a20 6861 7374 615f  _serial': hasta_
-000031d0: 6e75 6d65 726f 5f73 6572 6961 6c2c 0a20  numero_serial,. 
-000031e0: 2020 2020 2020 2020 2020 2027 6964 5f6f             'id_o
-000031f0: 6272 615f 736f 6369 616c 273a 2069 645f  bra_social': id_
-00003200: 6f62 7261 5f73 6f63 6961 6c20 6f72 204e  obra_social or N
-00003210: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00003220: 2027 6964 5f65 7665 6e74 6f27 3a20 6964   'id_evento': id
-00003230: 5f65 7665 6e74 6f2c 0a20 2020 2020 2020  _evento,.       
-00003240: 2020 2020 2027 6375 6974 5f6f 7269 6765       'cuit_orige
-00003250: 6e27 3a20 6375 6974 5f6f 7269 6765 6e2c  n': cuit_origen,
-00003260: 0a20 2020 2020 2020 2020 2020 2027 6375  .            'cu
-00003270: 6974 5f64 6573 7469 6e6f 273a 2063 7569  it_destino': cui
-00003280: 745f 6465 7374 696e 6f2c 0a20 2020 2020  t_destino,.     
-00003290: 2020 2020 2020 2027 6170 656c 6c69 646f         'apellido
-000032a0: 273a 2061 7065 6c6c 6964 6f2c 0a20 2020  ': apellido,.   
-000032b0: 2020 2020 2020 2020 2027 6e6f 6d62 7265           'nombre
-000032c0: 7327 3a20 6e6f 6d62 7265 732c 0a20 2020  s': nombres,.   
-000032d0: 2020 2020 2020 2020 2027 7469 706f 5f64           'tipo_d
-000032e0: 6f63 756d 656e 746f 273a 2074 6970 6f5f  ocumento': tipo_
-000032f0: 646f 6375 6d65 6e74 6f2c 0a20 2020 2020  documento,.     
-00003300: 2020 2020 2020 2027 6e5f 646f 6375 6d65         'n_docume
-00003310: 6e74 6f27 3a20 6e5f 646f 6375 6d65 6e74  nto': n_document
-00003320: 6f2c 0a20 2020 2020 2020 2020 2020 2027  o,.            '
-00003330: 7365 786f 273a 2073 6578 6f2c 0a20 2020  sexo': sexo,.   
-00003340: 2020 2020 2020 2020 2027 6469 7265 6363           'direcc
-00003350: 696f 6e27 3a20 6469 7265 6363 696f 6e2c  ion': direccion,
-00003360: 0a20 2020 2020 2020 2020 2020 2027 6e75  .            'nu
-00003370: 6d65 726f 273a 206e 756d 6572 6f2c 0a20  mero': numero,. 
-00003380: 2020 2020 2020 2020 2020 2027 7069 736f             'piso
-00003390: 273a 2070 6973 6f2c 0a20 2020 2020 2020  ': piso,.       
-000033a0: 2020 2020 2027 6465 7074 6f27 3a20 6465       'depto': de
-000033b0: 7074 6f2c 0a20 2020 2020 2020 2020 2020  pto,.           
-000033c0: 2027 6c6f 6361 6c69 6461 6427 3a20 6c6f   'localidad': lo
-000033d0: 6361 6c69 6461 642c 0a20 2020 2020 2020  calidad,.       
-000033e0: 2020 2020 2027 7072 6f76 696e 6369 6127       'provincia'
-000033f0: 3a20 7072 6f76 696e 6369 612c 0a20 2020  : provincia,.   
-00003400: 2020 2020 2020 2020 2027 6e5f 706f 7374           'n_post
-00003410: 616c 273a 206e 5f70 6f73 7461 6c2c 0a20  al': n_postal,. 
-00003420: 2020 2020 2020 2020 2020 2027 6665 6368             'fech
-00003430: 615f 6e61 6369 6d69 656e 746f 273a 2066  a_nacimiento': f
-00003440: 6563 6861 5f6e 6163 696d 6965 6e74 6f2c  echa_nacimiento,
-00003450: 0a20 2020 2020 2020 2020 2020 2027 7465  .            'te
-00003460: 6c65 666f 6e6f 273a 2074 656c 6566 6f6e  lefono': telefon
-00003470: 6f2c 0a20 2020 2020 2020 2020 2020 2027  o,.            '
-00003480: 6e72 6f5f 6173 6f63 6961 646f 273a 206e  nro_asociado': n
-00003490: 726f 5f61 736f 6369 6164 6f2c 0a20 2020  ro_asociado,.   
-000034a0: 2020 2020 207d 0a20 2020 2020 2020 2072       }.        r
-000034b0: 6573 203d 2073 656c 662e 636c 6965 6e74  es = self.client
-000034c0: 2e73 656e 644d 6564 6963 616d 656e 746f  .sendMedicamento
-000034d0: 7344 4853 6572 6965 280a 2020 2020 2020  sDHSerie(.      
-000034e0: 2020 2020 2020 6172 6730 3d70 6172 616d        arg0=param
-000034f0: 732c 0a20 2020 2020 2020 2020 2020 2061  s,.            a
-00003500: 7267 313d 7573 7561 7269 6f2c 0a20 2020  rg1=usuario,.   
-00003510: 2020 2020 2020 2020 2061 7267 323d 7061           arg2=pa
-00003520: 7373 776f 7264 2c0a 2020 2020 2020 2020  ssword,.        
-00003530: 290a 0a20 2020 2020 2020 2072 6574 203d  )..        ret =
-00003540: 2072 6573 5b27 7265 7475 726e 275d 0a0a   res['return']..
-00003550: 2020 2020 2020 2020 7365 6c66 2e43 6f64          self.Cod
-00003560: 6967 6f54 7261 6e73 6163 6369 6f6e 203d  igoTransaccion =
-00003570: 2072 6574 5b27 636f 6469 676f 5472 616e   ret['codigoTran
-00003580: 7361 6363 696f 6e27 5d0a 2020 2020 2020  saccion'].      
-00003590: 2020 7365 6c66 2e5f 5f61 6e61 6c69 7a61    self.__analiza
-000035a0: 725f 6572 726f 7265 7328 7265 7429 0a0a  r_errores(ret)..
-000035b0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-000035c0: 7275 650a 0a20 2020 2040 696e 6963 6961  rue..    @inicia
-000035d0: 6c69 7a61 725f 795f 6361 7074 7572 6172  lizar_y_capturar
-000035e0: 5f65 7863 6570 6369 6f6e 6573 0a20 2020  _excepciones.   
-000035f0: 2064 6566 2053 656e 6443 616e 6365 6c61   def SendCancela
-00003600: 6354 7261 6e73 6163 6328 7365 6c66 2c20  cTransacc(self, 
-00003610: 7573 7561 7269 6f2c 2070 6173 7377 6f72  usuario, passwor
-00003620: 642c 2063 6f64 6967 6f5f 7472 616e 7361  d, codigo_transa
-00003630: 6363 696f 6e29 3a0a 2020 2020 2020 2020  ccion):.        
-00003640: 2220 5265 616c 697a 6120 6c61 2063 616e  " Realiza la can
-00003650: 6365 6c61 6369 f36e 2064 6520 756e 6120  celaci.n de una 
-00003660: 7472 616e 7361 6363 69f3 6e22 0a20 2020  transacci.n".   
-00003670: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
-00003680: 636c 6965 6e74 2e73 656e 6443 616e 6365  client.sendCance
-00003690: 6c61 6354 7261 6e73 6163 6328 0a20 2020  lacTransacc(.   
-000036a0: 2020 2020 2020 2020 2061 7267 303d 636f           arg0=co
-000036b0: 6469 676f 5f74 7261 6e73 6163 6369 6f6e  digo_transaccion
-000036c0: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
-000036d0: 6731 3d75 7375 6172 696f 2c0a 2020 2020  g1=usuario,.    
-000036e0: 2020 2020 2020 2020 6172 6732 3d70 6173          arg2=pas
-000036f0: 7377 6f72 642c 0a20 2020 2020 2020 2029  sword,.        )
-00003700: 0a0a 2020 2020 2020 2020 7265 7420 3d20  ..        ret = 
-00003710: 7265 735b 2772 6574 7572 6e27 5d0a 0a20  res['return'].. 
-00003720: 2020 2020 2020 2073 656c 662e 436f 6469         self.Codi
-00003730: 676f 5472 616e 7361 6363 696f 6e20 3d20  goTransaccion = 
-00003740: 7265 742e 6765 7428 2763 6f64 6967 6f54  ret.get('codigoT
-00003750: 7261 6e73 6163 6369 6f6e 2729 0a20 2020  ransaccion').   
-00003760: 2020 2020 2073 656c 662e 5f5f 616e 616c       self.__anal
-00003770: 697a 6172 5f65 7272 6f72 6573 2872 6574  izar_errores(ret
-00003780: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00003790: 6e20 5472 7565 0a0a 2020 2020 4069 6e69  n True..    @ini
-000037a0: 6369 616c 697a 6172 5f79 5f63 6170 7475  cializar_y_captu
-000037b0: 7261 725f 6578 6365 7063 696f 6e65 730a  rar_excepciones.
-000037c0: 2020 2020 6465 6620 5365 6e64 4361 6e63      def SendCanc
-000037d0: 656c 6163 5472 616e 7361 6363 5061 7263  elacTransaccParc
-000037e0: 6961 6c28 0a20 2020 2020 2020 2073 656c  ial(.        sel
-000037f0: 662c 2075 7375 6172 696f 2c20 7061 7373  f, usuario, pass
-00003800: 776f 7264 2c20 636f 6469 676f 5f74 7261  word, codigo_tra
-00003810: 6e73 6163 6369 6f6e 2c0a 2020 2020 2020  nsaccion,.      
-00003820: 2020 6774 696e 5f6d 6564 6963 616d 656e    gtin_medicamen
-00003830: 746f 3d4e 6f6e 652c 206e 756d 6572 6f5f  to=None, numero_
-00003840: 7365 7269 616c 3d4e 6f6e 650a 2020 2020  serial=None.    
-00003850: 293a 0a20 2020 2020 2020 2022 2052 6561  ):.        " Rea
-00003860: 6c69 7a61 206c 6120 6361 6e63 656c 6163  liza la cancelac
-00003870: 69f3 6e20 7061 7263 6961 6c20 6465 2075  i.n parcial de u
-00003880: 6e61 2074 7261 6e73 6163 6369 f36e 220a  na transacci.n".
-00003890: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
-000038a0: 6c66 2e63 6c69 656e 742e 7365 6e64 4361  lf.client.sendCa
-000038b0: 6e63 656c 6163 5472 616e 7361 6363 5061  ncelacTransaccPa
-000038c0: 7263 6961 6c28 0a20 2020 2020 2020 2020  rcial(.         
-000038d0: 2020 2061 7267 303d 636f 6469 676f 5f74     arg0=codigo_t
-000038e0: 7261 6e73 6163 6369 6f6e 2c0a 2020 2020  ransaccion,.    
-000038f0: 2020 2020 2020 2020 6172 6731 3d75 7375          arg1=usu
-00003900: 6172 696f 2c0a 2020 2020 2020 2020 2020  ario,.          
-00003910: 2020 6172 6732 3d70 6173 7377 6f72 642c    arg2=password,
-00003920: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
-00003930: 333d 6774 696e 5f6d 6564 6963 616d 656e  3=gtin_medicamen
-00003940: 746f 2c0a 2020 2020 2020 2020 2020 2020  to,.            
-00003950: 6172 6734 3d6e 756d 6572 6f5f 7365 7269  arg4=numero_seri
-00003960: 616c 2c0a 2020 2020 2020 2020 290a 2020  al,.        ).  
-00003970: 2020 2020 2020 7265 7420 3d20 7265 735b        ret = res[
-00003980: 2772 6574 7572 6e27 5d0a 2020 2020 2020  'return'].      
-00003990: 2020 7365 6c66 2e43 6f64 6967 6f54 7261    self.CodigoTra
-000039a0: 6e73 6163 6369 6f6e 203d 2072 6574 2e67  nsaccion = ret.g
-000039b0: 6574 2827 636f 6469 676f 5472 616e 7361  et('codigoTransa
-000039c0: 6363 696f 6e27 290a 2020 2020 2020 2020  ccion').        
-000039d0: 7365 6c66 2e5f 5f61 6e61 6c69 7a61 725f  self.__analizar_
-000039e0: 6572 726f 7265 7328 7265 7429 0a20 2020  errores(ret).   
-000039f0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00003a00: 0a0a 2020 2020 4069 6e69 6369 616c 697a  ..    @inicializ
-00003a10: 6172 5f79 5f63 6170 7475 7261 725f 6578  ar_y_capturar_ex
-00003a20: 6365 7063 696f 6e65 730a 2020 2020 6465  cepciones.    de
-00003a30: 6620 5365 6e64 436f 6e66 6972 6d61 5472  f SendConfirmaTr
-00003a40: 616e 7361 6363 280a 2020 2020 2020 2020  ansacc(.        
-00003a50: 7365 6c66 2c20 7573 7561 7269 6f2c 2070  self, usuario, p
-00003a60: 6173 7377 6f72 642c 2070 5f69 6473 5f74  assword, p_ids_t
-00003a70: 7261 6e73 6163 2c20 665f 6f70 6572 6163  ransac, f_operac
-00003a80: 696f 6e0a 2020 2020 293a 0a20 2020 2020  ion.    ):.     
-00003a90: 2020 2022 436f 6e66 6972 6d61 206c 6120     "Confirma la 
-00003aa0: 7265 6365 7063 69f3 6e20 6465 2075 6e20  recepci.n de un 
-00003ab0: 6d65 6469 6361 6d65 6e74 6f22 0a20 2020  medicamento".   
-00003ac0: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
-00003ad0: 636c 6965 6e74 2e73 656e 6443 6f6e 6669  client.sendConfi
-00003ae0: 726d 6154 7261 6e73 6163 6328 0a20 2020  rmaTransacc(.   
-00003af0: 2020 2020 2020 2020 2061 7267 303d 7573           arg0=us
-00003b00: 7561 7269 6f2c 0a20 2020 2020 2020 2020  uario,.         
-00003b10: 2020 2061 7267 313d 7061 7373 776f 7264     arg1=password
-00003b20: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
-00003b30: 6732 3d7b 2770 5f69 6473 5f74 7261 6e73  g2={'p_ids_trans
-00003b40: 6163 273a 2070 5f69 6473 5f74 7261 6e73  ac': p_ids_trans
-00003b50: 6163 2c20 2766 5f6f 7065 7261 6369 6f6e  ac, 'f_operacion
-00003b60: 273a 2066 5f6f 7065 7261 6369 6f6e 7d2c  ': f_operacion},
-00003b70: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00003b80: 2020 2072 6574 203d 2072 6573 5b27 7265     ret = res['re
-00003b90: 7475 726e 275d 0a20 2020 2020 2020 2073  turn'].        s
-00003ba0: 656c 662e 436f 6469 676f 5472 616e 7361  elf.CodigoTransa
-00003bb0: 6363 696f 6e20 3d20 7265 742e 6765 7428  ccion = ret.get(
-00003bc0: 2769 645f 7472 616e 7361 635f 6173 6f63  'id_transac_asoc
-00003bd0: 6961 6461 2729 0a20 2020 2020 2020 2073  iada').        s
-00003be0: 656c 662e 5f5f 616e 616c 697a 6172 5f65  elf.__analizar_e
-00003bf0: 7272 6f72 6573 2872 6574 290a 2020 2020  rrores(ret).    
-00003c00: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-00003c10: 0a20 2020 2040 696e 6963 6961 6c69 7a61  .    @inicializa
-00003c20: 725f 795f 6361 7074 7572 6172 5f65 7863  r_y_capturar_exc
-00003c30: 6570 6369 6f6e 6573 0a20 2020 2064 6566  epciones.    def
-00003c40: 2053 656e 6441 6c65 7274 6154 7261 6e73   SendAlertaTrans
-00003c50: 6163 6328 7365 6c66 2c20 7573 7561 7269  acc(self, usuari
-00003c60: 6f2c 2070 6173 7377 6f72 642c 2070 5f69  o, password, p_i
-00003c70: 6473 5f74 7261 6e73 6163 5f77 7329 3a0a  ds_transac_ws):.
-00003c80: 2020 2020 2020 2020 2241 6c65 7274 6120          "Alerta 
-00003c90: 756e 206d 6564 6963 616d 656e 746f 2c20  un medicamento, 
-00003ca0: 6163 6369 f36e 2063 6f6e 7472 6172 6961  acci.n contraria
-00003cb0: 2061 2093 636f 6e66 6972 6d61 7220 6c61   a .confirmar la
-00003cc0: 205c 0a20 2020 2020 2020 2020 2020 2074   \.            t
-00003cd0: 7261 6e73 6163 6369 f36e 942e 220a 2020  ransacci.n..".  
-00003ce0: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
-00003cf0: 2e63 6c69 656e 742e 7365 6e64 416c 6572  .client.sendAler
-00003d00: 7461 5472 616e 7361 6363 280a 2020 2020  taTransacc(.    
-00003d10: 2020 2020 2020 2020 6172 6730 3d75 7375          arg0=usu
-00003d20: 6172 696f 2c0a 2020 2020 2020 2020 2020  ario,.          
-00003d30: 2020 6172 6731 3d70 6173 7377 6f72 642c    arg1=password,
-00003d40: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
-00003d50: 323d 705f 6964 735f 7472 616e 7361 635f  2=p_ids_transac_
-00003d60: 7773 2c0a 2020 2020 2020 2020 290a 2020  ws,.        ).  
-00003d70: 2020 2020 2020 7265 7420 3d20 7265 735b        ret = res[
-00003d80: 2772 6574 7572 6e27 5d0a 2020 2020 2020  'return'].      
-00003d90: 2020 7365 6c66 2e43 6f64 6967 6f54 7261    self.CodigoTra
-00003da0: 6e73 6163 6369 6f6e 203d 2072 6574 2e67  nsaccion = ret.g
-00003db0: 6574 2827 6964 5f74 7261 6e73 6163 5f61  et('id_transac_a
-00003dc0: 736f 6369 6164 6127 290a 2020 2020 2020  sociada').      
-00003dd0: 2020 7365 6c66 2e5f 5f61 6e61 6c69 7a61    self.__analiza
-00003de0: 725f 6572 726f 7265 7328 7265 7429 0a20  r_errores(ret). 
-00003df0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00003e00: 7565 0a0a 2020 2020 4069 6e69 6369 616c  ue..    @inicial
-00003e10: 697a 6172 5f79 5f63 6170 7475 7261 725f  izar_y_capturar_
-00003e20: 6578 6365 7063 696f 6e65 730a 2020 2020  excepciones.    
-00003e30: 6465 6620 4765 7454 7261 6e73 6163 6369  def GetTransacci
-00003e40: 6f6e 6573 4e6f 436f 6e66 6972 6d61 6461  onesNoConfirmada
-00003e50: 7328 0a20 2020 2020 2020 2073 656c 662c  s(.        self,
-00003e60: 2075 7375 6172 696f 2c20 7061 7373 776f   usuario, passwo
-00003e70: 7264 2c0a 2020 2020 2020 2020 705f 6964  rd,.        p_id
-00003e80: 5f74 7261 6e73 6163 6369 6f6e 5f67 6c6f  _transaccion_glo
-00003e90: 6261 6c3d 4e6f 6e65 2c20 6964 5f61 6765  bal=None, id_age
-00003ea0: 6e74 655f 696e 666f 726d 6164 6f72 3d4e  nte_informador=N
-00003eb0: 6f6e 652c 0a20 2020 2020 2020 2069 645f  one,.        id_
-00003ec0: 6167 656e 7465 5f6f 7269 6765 6e3d 4e6f  agente_origen=No
-00003ed0: 6e65 2c20 6964 5f61 6765 6e74 655f 6465  ne, id_agente_de
-00003ee0: 7374 696e 6f3d 4e6f 6e65 2c0a 2020 2020  stino=None,.    
-00003ef0: 2020 2020 6964 5f6d 6564 6963 616d 656e      id_medicamen
-00003f00: 746f 3d4e 6f6e 652c 2069 645f 6576 656e  to=None, id_even
-00003f10: 746f 3d4e 6f6e 652c 0a20 2020 2020 2020  to=None,.       
-00003f20: 2066 6563 6861 5f64 6573 6465 5f6f 703d   fecha_desde_op=
-00003f30: 4e6f 6e65 2c20 6665 6368 615f 6861 7374  None, fecha_hast
-00003f40: 615f 6f70 3d4e 6f6e 652c 0a20 2020 2020  a_op=None,.     
-00003f50: 2020 2066 6563 6861 5f64 6573 6465 5f74     fecha_desde_t
-00003f60: 3d4e 6f6e 652c 2066 6563 6861 5f68 6173  =None, fecha_has
-00003f70: 7461 5f74 3d4e 6f6e 652c 0a20 2020 2020  ta_t=None,.     
-00003f80: 2020 2066 6563 6861 5f64 6573 6465 5f76     fecha_desde_v
-00003f90: 3d4e 6f6e 652c 2066 6563 6861 5f68 6173  =None, fecha_has
-00003fa0: 7461 5f76 3d4e 6f6e 652c 0a20 2020 2020  ta_v=None,.     
-00003fb0: 2020 206e 5f72 656d 6974 6f3d 4e6f 6e65     n_remito=None
-00003fc0: 2c20 6e5f 6661 6374 7572 613d 4e6f 6e65  , n_factura=None
-00003fd0: 2c0a 2020 2020 2020 2020 6573 7461 646f  ,.        estado
-00003fe0: 3d4e 6f6e 652c 206c 6f74 653d 4e6f 6e65  =None, lote=None
-00003ff0: 2c20 6e75 6d65 726f 5f73 6572 6961 6c3d  , numero_serial=
-00004000: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-00004010: 2020 2020 2022 5472 6165 2075 6e20 6c69       "Trae un li
-00004020: 7374 6164 6f20 6465 206c 6173 2074 7261  stado de las tra
-00004030: 6e73 6163 6369 6f6e 6573 2071 7565 206e  nsacciones que n
-00004040: 6f20 6573 74e1 6e20 636f 6e66 6972 6d61  o est.n confirma
-00004050: 6461 7322 0a0a 2020 2020 2020 2020 2320  das"..        # 
-00004060: 7072 6570 6172 6f20 6c6f 7320 7061 7261  preparo los para
-00004070: 6d65 7472 6f73 2064 6520 656e 7472 6164  metros de entrad
-00004080: 6120 6f70 6369 6f6e 616c 6573 3a0a 2020  a opcionales:.  
-00004090: 2020 2020 2020 6b77 6172 6773 203d 207b        kwargs = {
-000040a0: 7d0a 2020 2020 2020 2020 6966 2070 5f69  }.        if p_i
-000040b0: 645f 7472 616e 7361 6363 696f 6e5f 676c  d_transaccion_gl
-000040c0: 6f62 616c 2069 7320 6e6f 7420 4e6f 6e65  obal is not None
-000040d0: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
-000040e0: 6172 6773 5b27 6172 6732 275d 203d 2070  args['arg2'] = p
-000040f0: 5f69 645f 7472 616e 7361 6363 696f 6e5f  _id_transaccion_
-00004100: 676c 6f62 616c 0a20 2020 2020 2020 2069  global.        i
-00004110: 6620 6964 5f61 6765 6e74 655f 696e 666f  f id_agente_info
-00004120: 726d 6164 6f72 2069 7320 6e6f 7420 4e6f  rmador is not No
-00004130: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00004140: 6b77 6172 6773 5b27 6172 6733 275d 203d  kwargs['arg3'] =
-00004150: 2069 645f 6167 656e 7465 5f69 6e66 6f72   id_agente_infor
-00004160: 6d61 646f 720a 2020 2020 2020 2020 6966  mador.        if
-00004170: 2069 645f 6167 656e 7465 5f6f 7269 6765   id_agente_orige
-00004180: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-00004190: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
-000041a0: 735b 2761 7267 3427 5d20 3d20 6964 5f61  s['arg4'] = id_a
-000041b0: 6765 6e74 655f 6f72 6967 656e 0a20 2020  gente_origen.   
-000041c0: 2020 2020 2069 6620 6964 5f61 6765 6e74       if id_agent
-000041d0: 655f 6465 7374 696e 6f20 6973 206e 6f74  e_destino is not
-000041e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000041f0: 2020 206b 7761 7267 735b 2761 7267 3527     kwargs['arg5'
-00004200: 5d20 3d20 6964 5f61 6765 6e74 655f 6465  ] = id_agente_de
-00004210: 7374 696e 6f0a 2020 2020 2020 2020 6966  stino.        if
-00004220: 2069 645f 6d65 6469 6361 6d65 6e74 6f20   id_medicamento 
-00004230: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00004240: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
-00004250: 2761 7267 3627 5d20 3d20 6964 5f6d 6564  'arg6'] = id_med
-00004260: 6963 616d 656e 746f 0a20 2020 2020 2020  icamento.       
-00004270: 2069 6620 6964 5f65 7665 6e74 6f20 6973   if id_evento is
-00004280: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00004290: 2020 2020 2020 206b 7761 7267 735b 2761         kwargs['a
-000042a0: 7267 3727 5d20 3d20 6964 5f65 7665 6e74  rg7'] = id_event
-000042b0: 6f0a 2020 2020 2020 2020 6966 2066 6563  o.        if fec
-000042c0: 6861 5f64 6573 6465 5f6f 7020 6973 206e  ha_desde_op is n
-000042d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000042e0: 2020 2020 206b 7761 7267 735b 2761 7267       kwargs['arg
-000042f0: 3827 5d20 3d20 6665 6368 615f 6465 7364  8'] = fecha_desd
-00004300: 655f 6f70 0a20 2020 2020 2020 2069 6620  e_op.        if 
-00004310: 6665 6368 615f 6861 7374 615f 6f70 2069  fecha_hasta_op i
-00004320: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00004330: 2020 2020 2020 2020 6b77 6172 6773 5b27          kwargs['
-00004340: 6172 6739 275d 203d 2066 6563 6861 5f68  arg9'] = fecha_h
-00004350: 6173 7461 5f6f 700a 2020 2020 2020 2020  asta_op.        
-00004360: 6966 2066 6563 6861 5f64 6573 6465 5f74  if fecha_desde_t
-00004370: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00004380: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
-00004390: 5b27 6172 6731 3027 5d20 3d20 6665 6368  ['arg10'] = fech
-000043a0: 615f 6465 7364 655f 740a 2020 2020 2020  a_desde_t.      
-000043b0: 2020 6966 2066 6563 6861 5f68 6173 7461    if fecha_hasta
-000043c0: 5f74 2069 7320 6e6f 7420 4e6f 6e65 3a0a  _t is not None:.
-000043d0: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-000043e0: 6773 5b27 6172 6731 3127 5d20 3d20 6665  gs['arg11'] = fe
-000043f0: 6368 615f 6861 7374 615f 740a 2020 2020  cha_hasta_t.    
-00004400: 2020 2020 6966 2066 6563 6861 5f64 6573      if fecha_des
-00004410: 6465 5f76 2069 7320 6e6f 7420 4e6f 6e65  de_v is not None
-00004420: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
-00004430: 6172 6773 5b27 6172 6731 3227 5d20 3d20  args['arg12'] = 
-00004440: 6665 6368 615f 6465 7364 655f 760a 2020  fecha_desde_v.  
-00004450: 2020 2020 2020 6966 2066 6563 6861 5f68        if fecha_h
-00004460: 6173 7461 5f76 2069 7320 6e6f 7420 4e6f  asta_v is not No
-00004470: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00004480: 6b77 6172 6773 5b27 6172 6731 3327 5d20  kwargs['arg13'] 
-00004490: 3d20 6665 6368 615f 6861 7374 615f 760a  = fecha_hasta_v.
-000044a0: 2020 2020 2020 2020 6966 206e 5f72 656d          if n_rem
-000044b0: 6974 6f20 6973 206e 6f74 204e 6f6e 653a  ito is not None:
-000044c0: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
-000044d0: 7267 735b 2761 7267 3134 275d 203d 206e  rgs['arg14'] = n
-000044e0: 5f72 656d 6974 6f0a 2020 2020 2020 2020  _remito.        
-000044f0: 6966 206e 5f66 6163 7475 7261 2069 7320  if n_factura is 
-00004500: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00004510: 2020 2020 2020 6b77 6172 6773 5b27 6172        kwargs['ar
-00004520: 6731 3527 5d20 3d20 6e5f 6661 6374 7572  g15'] = n_factur
-00004530: 610a 2020 2020 2020 2020 6966 2065 7374  a.        if est
-00004540: 6164 6f20 6973 206e 6f74 204e 6f6e 653a  ado is not None:
-00004550: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
-00004560: 7267 735b 2761 7267 3136 275d 203d 2065  rgs['arg16'] = e
-00004570: 7374 6164 6f0a 2020 2020 2020 2020 6966  stado.        if
-00004580: 206c 6f74 6520 6973 206e 6f74 204e 6f6e   lote is not Non
-00004590: 653a 0a20 2020 2020 2020 2020 2020 206b  e:.            k
-000045a0: 7761 7267 735b 2761 7267 3137 275d 203d  wargs['arg17'] =
-000045b0: 206c 6f74 650a 2020 2020 2020 2020 6966   lote.        if
-000045c0: 206e 756d 6572 6f5f 7365 7269 616c 2069   numero_serial i
-000045d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000045e0: 2020 2020 2020 2020 6b77 6172 6773 5b27          kwargs['
-000045f0: 6172 6731 3827 5d20 3d20 6e75 6d65 726f  arg18'] = numero
-00004600: 5f73 6572 6961 6c0a 0a20 2020 2020 2020  _serial..       
-00004610: 2023 206c 6c61 6d6f 2061 6c20 7765 6273   # llamo al webs
-00004620: 6572 7669 6365 0a20 2020 2020 2020 2072  ervice.        r
-00004630: 6573 203d 2073 656c 662e 636c 6965 6e74  es = self.client
-00004640: 2e67 6574 5472 616e 7361 6363 696f 6e65  .getTransaccione
-00004650: 734e 6f43 6f6e 6669 726d 6164 6173 280a  sNoConfirmadas(.
-00004660: 2020 2020 2020 2020 2020 2020 6172 6730              arg0
-00004670: 3d75 7375 6172 696f 2c0a 2020 2020 2020  =usuario,.      
-00004680: 2020 2020 2020 6172 6731 3d70 6173 7377        arg1=passw
-00004690: 6f72 642c 0a20 2020 2020 2020 2020 2020  ord,.           
-000046a0: 202a 2a6b 7761 7267 730a 2020 2020 2020   **kwargs.      
-000046b0: 2020 290a 2020 2020 2020 2020 7265 7420    ).        ret 
-000046c0: 3d20 7265 735b 2772 6574 7572 6e27 5d0a  = res['return'].
-000046d0: 2020 2020 2020 2020 6966 2072 6574 3a0a          if ret:.
-000046e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000046f0: 2e5f 5f61 6e61 6c69 7a61 725f 6572 726f  .__analizar_erro
-00004700: 7265 7328 7265 7429 0a20 2020 2020 2020  res(ret).       
-00004710: 2020 2020 2073 656c 662e 4361 6e74 5061       self.CantPa
-00004720: 6769 6e61 7320 3d20 7265 742e 6765 7428  ginas = ret.get(
-00004730: 2763 616e 7450 6167 696e 6173 2729 0a20  'cantPaginas'). 
-00004740: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004750: 4861 7945 7272 6f72 203d 2072 6574 2e67  HayError = ret.g
-00004760: 6574 2827 6861 795f 6572 726f 7227 290a  et('hay_error').
-00004770: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004780: 2e54 7261 6e73 6163 6369 6f6e 506c 6169  .TransaccionPlai
-00004790: 6e57 5320 3d20 5b69 7420 666f 7220 6974  nWS = [it for it
-000047a0: 2069 6e20 7265 742e 6765 7428 276c 6973   in ret.get('lis
-000047b0: 7427 2c20 5b5d 295d 0a20 2020 2020 2020  t', [])].       
-000047c0: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
-000047d0: 2020 6465 6620 4c65 6572 5472 616e 7361    def LeerTransa
-000047e0: 6363 696f 6e28 7365 6c66 293a 0a20 2020  ccion(self):.   
-000047f0: 2020 2020 2022 5265 636f 7272 6f20 5472       "Recorro Tr
-00004800: 616e 7361 6363 696f 6e50 6c61 696e 5753  ansaccionPlainWS
-00004810: 2064 6576 7565 6c74 6f20 706f 7220 4765   devuelto por Ge
-00004820: 7454 7261 6e73 6163 6369 6f6e 6573 4e6f  tTransaccionesNo
-00004830: 436f 6e66 6972 6d61 6461 7322 0a20 2020  Confirmadas".   
-00004840: 2020 2020 2023 2075 7361 7220 4765 7450       # usar GetP
-00004850: 6172 616d 6574 726f 2070 6172 6120 636f  arametro para co
-00004860: 6e73 756c 7461 7220 656c 2076 616c 6f72  nsultar el valor
-00004870: 2072 6574 6f72 6e61 646f 2070 6f72 2065   retornado por e
-00004880: 6c0a 2020 2020 2020 2020 2320 7765 6273  l.        # webs
-00004890: 6572 7669 6365 0a0a 2020 2020 2020 2020  ervice..        
-000048a0: 6966 2073 656c 662e 5472 616e 7361 6363  if self.Transacc
-000048b0: 696f 6e50 6c61 696e 5753 3a0a 2020 2020  ionPlainWS:.    
-000048c0: 2020 2020 2020 2020 2320 6578 7472 6169          # extrai
-000048d0: 676f 2065 6c20 7072 696d 6572 2069 7465  go el primer ite
-000048e0: 6d0a 2020 2020 2020 2020 2020 2020 7365  m.            se
-000048f0: 6c66 2e70 6172 616d 735f 6f75 7420 3d20  lf.params_out = 
-00004900: 7365 6c66 2e54 7261 6e73 6163 6369 6f6e  self.Transaccion
-00004910: 506c 6169 6e57 532e 706f 7028 3029 0a20  PlainWS.pop(0). 
-00004920: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00004930: 6e20 5472 7565 0a20 2020 2020 2020 2065  n True.        e
-00004940: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00004950: 2023 206c 696d 7069 6f20 6c6f 7320 7061   # limpio los pa
-00004960: 72e1 6d65 7472 6f73 0a20 2020 2020 2020  r.metros.       
-00004970: 2020 2020 2073 656c 662e 7061 7261 6d73       self.params
-00004980: 5f6f 7574 203d 207b 7d0a 2020 2020 2020  _out = {}.      
-00004990: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-000049a0: 7365 0a0a 2020 2020 6465 6620 4c65 6572  se..    def Leer
-000049b0: 4572 726f 7228 7365 6c66 293a 0a20 2020  Error(self):.   
-000049c0: 2020 2020 2022 5265 636f 7272 6f20 6c6f       "Recorro lo
-000049d0: 7320 6572 726f 7265 7320 6465 7675 656c  s errores devuel
-000049e0: 746f 7320 7920 6465 7675 656c 766f 2065  tos y devuelvo e
-000049f0: 6c20 7072 696d 6572 6f20 7369 2065 7869  l primero si exi
-00004a00: 7374 6522 0a0a 2020 2020 2020 2020 6966  ste"..        if
-00004a10: 2073 656c 662e 4572 726f 7265 733a 0a20   self.Errores:. 
-00004a20: 2020 2020 2020 2020 2020 2023 2065 7874             # ext
-00004a30: 7261 6967 6f20 656c 2070 7269 6d65 7220  raigo el primer 
-00004a40: 6974 656d 0a20 2020 2020 2020 2020 2020  item.           
-00004a50: 2065 7220 3d20 7365 6c66 2e45 7272 6f72   er = self.Error
-00004a60: 6573 2e70 6f70 2830 290a 2020 2020 2020  es.pop(0).      
-00004a70: 2020 2020 2020 7265 7475 726e 2065 720a        return er.
-00004a80: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00004a90: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00004aa0: 2022 220a 0a20 2020 2040 696e 6963 6961   ""..    @inicia
-00004ab0: 6c69 7a61 725f 795f 6361 7074 7572 6172  lizar_y_capturar
-00004ac0: 5f65 7863 6570 6369 6f6e 6573 0a20 2020  _excepciones.   
-00004ad0: 2064 6566 2047 6574 456e 7669 6f73 5072   def GetEnviosPr
-00004ae0: 6f70 696f 7341 6c65 7274 6164 6f73 280a  opiosAlertados(.
-00004af0: 2020 2020 2020 2020 7365 6c66 2c20 7573          self, us
-00004b00: 7561 7269 6f2c 2070 6173 7377 6f72 642c  uario, password,
-00004b10: 0a20 2020 2020 2020 2070 5f69 645f 7472  .        p_id_tr
-00004b20: 616e 7361 6363 696f 6e5f 676c 6f62 616c  ansaccion_global
-00004b30: 3d4e 6f6e 652c 2069 645f 6167 656e 7465  =None, id_agente
-00004b40: 5f69 6e66 6f72 6d61 646f 723d 4e6f 6e65  _informador=None
-00004b50: 2c0a 2020 2020 2020 2020 6964 5f61 6765  ,.        id_age
-00004b60: 6e74 655f 6f72 6967 656e 3d4e 6f6e 652c  nte_origen=None,
-00004b70: 2069 645f 6167 656e 7465 5f64 6573 7469   id_agente_desti
-00004b80: 6e6f 3d4e 6f6e 652c 0a20 2020 2020 2020  no=None,.       
-00004b90: 2069 645f 6d65 6469 6361 6d65 6e74 6f3d   id_medicamento=
-00004ba0: 4e6f 6e65 2c20 6964 5f65 7665 6e74 6f3d  None, id_evento=
-00004bb0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6665  None,.        fe
-00004bc0: 6368 615f 6465 7364 655f 6f70 3d4e 6f6e  cha_desde_op=Non
-00004bd0: 652c 2066 6563 6861 5f68 6173 7461 5f6f  e, fecha_hasta_o
-00004be0: 703d 4e6f 6e65 2c0a 2020 2020 2020 2020  p=None,.        
-00004bf0: 6665 6368 615f 6465 7364 655f 743d 4e6f  fecha_desde_t=No
-00004c00: 6e65 2c20 6665 6368 615f 6861 7374 615f  ne, fecha_hasta_
-00004c10: 743d 4e6f 6e65 2c0a 2020 2020 2020 2020  t=None,.        
-00004c20: 6665 6368 615f 6465 7364 655f 763d 4e6f  fecha_desde_v=No
-00004c30: 6e65 2c20 6665 6368 615f 6861 7374 615f  ne, fecha_hasta_
-00004c40: 763d 4e6f 6e65 2c0a 2020 2020 2020 2020  v=None,.        
-00004c50: 6e5f 7265 6d69 746f 3d4e 6f6e 652c 206e  n_remito=None, n
-00004c60: 5f66 6163 7475 7261 3d4e 6f6e 652c 0a20  _factura=None,. 
-00004c70: 2020 2029 3a0a 2020 2020 2020 2020 224f     ):.        "O
-00004c80: 6274 6965 6e65 206c 6173 2064 6973 7472  btiene las distr
-00004c90: 6962 7563 696f 6e65 7320 7920 656e 76ed  ibuciones y env.
-00004ca0: 6f73 2070 726f 7069 6f73 2071 7565 2068  os propios que h
-00004cb0: 616e 2073 6964 6f20 616c 6572 7461 646f  an sido alertado
-00004cc0: 7322 0a0a 2020 2020 2020 2020 2320 7072  s"..        # pr
-00004cd0: 6570 6172 6f20 6c6f 7320 7061 7261 6d65  eparo los parame
-00004ce0: 7472 6f73 2064 6520 656e 7472 6164 6120  tros de entrada 
-00004cf0: 6f70 6369 6f6e 616c 6573 3a0a 2020 2020  opcionales:.    
-00004d00: 2020 2020 6b77 6172 6773 203d 207b 7d0a      kwargs = {}.
-00004d10: 2020 2020 2020 2020 6966 2070 5f69 645f          if p_id_
-00004d20: 7472 616e 7361 6363 696f 6e5f 676c 6f62  transaccion_glob
-00004d30: 616c 2069 7320 6e6f 7420 4e6f 6e65 3a0a  al is not None:.
-00004d40: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-00004d50: 6773 5b27 6172 6732 275d 203d 2070 5f69  gs['arg2'] = p_i
-00004d60: 645f 7472 616e 7361 6363 696f 6e5f 676c  d_transaccion_gl
-00004d70: 6f62 616c 0a20 2020 2020 2020 2069 6620  obal.        if 
-00004d80: 6964 5f61 6765 6e74 655f 696e 666f 726d  id_agente_inform
-00004d90: 6164 6f72 2069 7320 6e6f 7420 4e6f 6e65  ador is not None
-00004da0: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
-00004db0: 6172 6773 5b27 6172 6733 275d 203d 2069  args['arg3'] = i
-00004dc0: 645f 6167 656e 7465 5f69 6e66 6f72 6d61  d_agente_informa
-00004dd0: 646f 720a 2020 2020 2020 2020 6966 2069  dor.        if i
-00004de0: 645f 6167 656e 7465 5f6f 7269 6765 6e20  d_agente_origen 
-00004df0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00004e00: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
-00004e10: 2761 7267 3427 5d20 3d20 6964 5f61 6765  'arg4'] = id_age
-00004e20: 6e74 655f 6f72 6967 656e 0a20 2020 2020  nte_origen.     
-00004e30: 2020 2069 6620 6964 5f61 6765 6e74 655f     if id_agente_
-00004e40: 6465 7374 696e 6f20 6973 206e 6f74 204e  destino is not N
-00004e50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00004e60: 206b 7761 7267 735b 2761 7267 3527 5d20   kwargs['arg5'] 
-00004e70: 3d20 6964 5f61 6765 6e74 655f 6465 7374  = id_agente_dest
-00004e80: 696e 6f0a 2020 2020 2020 2020 6966 2069  ino.        if i
-00004e90: 645f 6d65 6469 6361 6d65 6e74 6f20 6973  d_medicamento is
-00004ea0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00004eb0: 2020 2020 2020 206b 7761 7267 735b 2761         kwargs['a
-00004ec0: 7267 3627 5d20 3d20 6964 5f6d 6564 6963  rg6'] = id_medic
-00004ed0: 616d 656e 746f 0a20 2020 2020 2020 2069  amento.        i
-00004ee0: 6620 6964 5f65 7665 6e74 6f20 6973 206e  f id_evento is n
-00004ef0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00004f00: 2020 2020 206b 7761 7267 735b 2761 7267       kwargs['arg
-00004f10: 3727 5d20 3d20 6964 5f65 7665 6e74 6f0a  7'] = id_evento.
-00004f20: 2020 2020 2020 2020 6966 2066 6563 6861          if fecha
-00004f30: 5f64 6573 6465 5f6f 7020 6973 206e 6f74  _desde_op is not
-00004f40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00004f50: 2020 206b 7761 7267 735b 2761 7267 3827     kwargs['arg8'
-00004f60: 5d20 3d20 6665 6368 615f 6465 7364 655f  ] = fecha_desde_
-00004f70: 6f70 0a20 2020 2020 2020 2069 6620 6665  op.        if fe
-00004f80: 6368 615f 6861 7374 615f 6f70 2069 7320  cha_hasta_op is 
-00004f90: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00004fa0: 2020 2020 2020 6b77 6172 6773 5b27 6172        kwargs['ar
-00004fb0: 6739 275d 203d 2066 6563 6861 5f68 6173  g9'] = fecha_has
-00004fc0: 7461 5f6f 700a 2020 2020 2020 2020 6966  ta_op.        if
-00004fd0: 2066 6563 6861 5f64 6573 6465 5f74 2069   fecha_desde_t i
-00004fe0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00004ff0: 2020 2020 2020 2020 6b77 6172 6773 5b27          kwargs['
-00005000: 6172 6731 3027 5d20 3d20 6665 6368 615f  arg10'] = fecha_
-00005010: 6465 7364 655f 740a 2020 2020 2020 2020  desde_t.        
-00005020: 6966 2066 6563 6861 5f68 6173 7461 5f74  if fecha_hasta_t
-00005030: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00005040: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
-00005050: 5b27 6172 6731 3127 5d20 3d20 6665 6368  ['arg11'] = fech
-00005060: 615f 6861 7374 615f 740a 2020 2020 2020  a_hasta_t.      
-00005070: 2020 6966 2066 6563 6861 5f64 6573 6465    if fecha_desde
-00005080: 5f76 2069 7320 6e6f 7420 4e6f 6e65 3a0a  _v is not None:.
-00005090: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-000050a0: 6773 5b27 6172 6731 3227 5d20 3d20 6665  gs['arg12'] = fe
-000050b0: 6368 615f 6465 7364 655f 760a 2020 2020  cha_desde_v.    
-000050c0: 2020 2020 6966 2066 6563 6861 5f68 6173      if fecha_has
-000050d0: 7461 5f76 2069 7320 6e6f 7420 4e6f 6e65  ta_v is not None
-000050e0: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
-000050f0: 6172 6773 5b27 6172 6731 3327 5d20 3d20  args['arg13'] = 
-00005100: 6665 6368 615f 6861 7374 615f 760a 2020  fecha_hasta_v.  
-00005110: 2020 2020 2020 6966 206e 5f72 656d 6974        if n_remit
-00005120: 6f20 6973 206e 6f74 204e 6f6e 653a 0a20  o is not None:. 
-00005130: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
-00005140: 735b 2761 7267 3134 275d 203d 206e 5f72  s['arg14'] = n_r
-00005150: 656d 6974 6f0a 2020 2020 2020 2020 6966  emito.        if
-00005160: 206e 5f66 6163 7475 7261 2069 7320 6e6f   n_factura is no
-00005170: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00005180: 2020 2020 6b77 6172 6773 5b27 6172 6731      kwargs['arg1
-00005190: 3527 5d20 3d20 6e5f 6661 6374 7572 610a  5'] = n_factura.
-000051a0: 0a20 2020 2020 2020 2023 206c 6c61 6d6f  .        # llamo
-000051b0: 2061 6c20 7765 6273 6572 7669 6365 0a20   al webservice. 
-000051c0: 2020 2020 2020 2072 6573 203d 2073 656c         res = sel
-000051d0: 662e 636c 6965 6e74 2e67 6574 456e 7669  f.client.getEnvi
-000051e0: 6f73 5072 6f70 696f 7341 6c65 7274 6164  osPropiosAlertad
-000051f0: 6f73 280a 2020 2020 2020 2020 2020 2020  os(.            
-00005200: 6172 6730 3d75 7375 6172 696f 2c0a 2020  arg0=usuario,.  
-00005210: 2020 2020 2020 2020 2020 6172 6731 3d70            arg1=p
-00005220: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
-00005230: 2020 2020 202a 2a6b 7761 7267 730a 2020       **kwargs.  
-00005240: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00005250: 7265 7420 3d20 7265 735b 2772 6574 7572  ret = res['retur
-00005260: 6e27 5d0a 2020 2020 2020 2020 6966 2072  n'].        if r
-00005270: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
-00005280: 7365 6c66 2e5f 5f61 6e61 6c69 7a61 725f  self.__analizar_
-00005290: 6572 726f 7265 7328 7265 7429 0a20 2020  errores(ret).   
-000052a0: 2020 2020 2020 2020 2073 656c 662e 4361           self.Ca
-000052b0: 6e74 5061 6769 6e61 7320 3d20 7265 742e  ntPaginas = ret.
-000052c0: 6765 7428 2763 616e 7450 6167 696e 6173  get('cantPaginas
-000052d0: 2729 0a20 2020 2020 2020 2020 2020 2073  ').            s
-000052e0: 656c 662e 4861 7945 7272 6f72 203d 2072  elf.HayError = r
-000052f0: 6574 2e67 6574 2827 6861 795f 6572 726f  et.get('hay_erro
-00005300: 7227 290a 2020 2020 2020 2020 2020 2020  r').            
-00005310: 7365 6c66 2e54 7261 6e73 6163 6369 6f6e  self.Transaccion
-00005320: 506c 6169 6e57 5320 3d20 5b69 7420 666f  PlainWS = [it fo
-00005330: 7220 6974 2069 6e20 7265 742e 6765 7428  r it in ret.get(
-00005340: 276c 6973 7427 2c20 5b5d 295d 0a20 2020  'list', [])].   
-00005350: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00005360: 0a0a 2020 2020 4069 6e69 6369 616c 697a  ..    @inicializ
-00005370: 6172 5f79 5f63 6170 7475 7261 725f 6578  ar_y_capturar_ex
-00005380: 6365 7063 696f 6e65 730a 2020 2020 6465  cepciones.    de
-00005390: 6620 4765 7454 7261 6e73 6163 6369 6f6e  f GetTransaccion
-000053a0: 6573 5753 280a 2020 2020 2020 2020 7365  esWS(.        se
-000053b0: 6c66 2c20 7573 7561 7269 6f2c 2070 6173  lf, usuario, pas
-000053c0: 7377 6f72 642c 0a20 2020 2020 2020 2070  sword,.        p
-000053d0: 5f69 645f 7472 616e 7361 6363 696f 6e5f  _id_transaccion_
-000053e0: 676c 6f62 616c 3d4e 6f6e 652c 0a20 2020  global=None,.   
-000053f0: 2020 2020 2069 645f 6167 656e 7465 5f6f       id_agente_o
-00005400: 7269 6765 6e3d 4e6f 6e65 2c20 6964 5f61  rigen=None, id_a
-00005410: 6765 6e74 655f 6465 7374 696e 6f3d 4e6f  gente_destino=No
-00005420: 6e65 2c0a 2020 2020 2020 2020 6964 5f6d  ne,.        id_m
-00005430: 6564 6963 616d 656e 746f 3d4e 6f6e 652c  edicamento=None,
-00005440: 2069 645f 6576 656e 746f 3d4e 6f6e 652c   id_evento=None,
-00005450: 0a20 2020 2020 2020 2066 6563 6861 5f64  .        fecha_d
-00005460: 6573 6465 5f6f 703d 4e6f 6e65 2c20 6665  esde_op=None, fe
-00005470: 6368 615f 6861 7374 615f 6f70 3d4e 6f6e  cha_hasta_op=Non
-00005480: 652c 0a20 2020 2020 2020 2066 6563 6861  e,.        fecha
-00005490: 5f64 6573 6465 5f74 3d4e 6f6e 652c 2066  _desde_t=None, f
-000054a0: 6563 6861 5f68 6173 7461 5f74 3d4e 6f6e  echa_hasta_t=Non
-000054b0: 652c 0a20 2020 2020 2020 2066 6563 6861  e,.        fecha
-000054c0: 5f64 6573 6465 5f76 3d4e 6f6e 652c 2066  _desde_v=None, f
-000054d0: 6563 6861 5f68 6173 7461 5f76 3d4e 6f6e  echa_hasta_v=Non
-000054e0: 652c 0a20 2020 2020 2020 206e 5f72 656d  e,.        n_rem
-000054f0: 6974 6f3d 4e6f 6e65 2c20 6e5f 6661 6374  ito=None, n_fact
-00005500: 7572 613d 4e6f 6e65 2c0a 2020 2020 2020  ura=None,.      
-00005510: 2020 6964 5f65 7374 6164 6f3d 4e6f 6e65    id_estado=None
-00005520: 2c20 6e72 6f5f 7061 673d 4e6f 6e65 2c0a  , nro_pag=None,.
-00005530: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-00005540: 4f62 7469 656e 6520 6c6f 7320 6d6f 7669  Obtiene los movi
-00005550: 6d69 656e 746f 7320 7265 616c 697a 6164  mientos realizad
-00005560: 6f73 2079 2070 6572 6d69 7465 2066 696c  os y permite fil
-00005570: 7472 6f73 2064 6520 62fa 7371 7565 6461  tros de b.squeda
-00005580: 220a 0a20 2020 2020 2020 2023 2070 7265  "..        # pre
-00005590: 7061 726f 206c 6f73 2070 6172 616d 6574  paro los paramet
-000055a0: 726f 7320 6465 2065 6e74 7261 6461 206f  ros de entrada o
-000055b0: 7063 696f 6e61 6c65 733a 0a20 2020 2020  pcionales:.     
-000055c0: 2020 206b 7761 7267 7320 3d20 7b7d 0a20     kwargs = {}. 
-000055d0: 2020 2020 2020 2069 6620 705f 6964 5f74         if p_id_t
-000055e0: 7261 6e73 6163 6369 6f6e 5f67 6c6f 6261  ransaccion_globa
-000055f0: 6c20 6973 206e 6f74 204e 6f6e 653a 0a20  l is not None:. 
-00005600: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
-00005610: 735b 2761 7267 3227 5d20 3d20 705f 6964  s['arg2'] = p_id
-00005620: 5f74 7261 6e73 6163 6369 6f6e 5f67 6c6f  _transaccion_glo
-00005630: 6261 6c0a 2020 2020 2020 2020 6966 2069  bal.        if i
-00005640: 645f 6167 656e 7465 5f6f 7269 6765 6e20  d_agente_origen 
-00005650: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00005660: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
-00005670: 2761 7267 3327 5d20 3d20 6964 5f61 6765  'arg3'] = id_age
-00005680: 6e74 655f 6f72 6967 656e 0a20 2020 2020  nte_origen.     
-00005690: 2020 2069 6620 6964 5f61 6765 6e74 655f     if id_agente_
-000056a0: 6465 7374 696e 6f20 6973 206e 6f74 204e  destino is not N
-000056b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000056c0: 206b 7761 7267 735b 2761 7267 3427 5d20   kwargs['arg4'] 
-000056d0: 3d20 6964 5f61 6765 6e74 655f 6465 7374  = id_agente_dest
-000056e0: 696e 6f0a 2020 2020 2020 2020 6966 2069  ino.        if i
-000056f0: 645f 6d65 6469 6361 6d65 6e74 6f20 6973  d_medicamento is
-00005700: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00005710: 2020 2020 2020 206b 7761 7267 735b 2761         kwargs['a
-00005720: 7267 3527 5d20 3d20 6964 5f6d 6564 6963  rg5'] = id_medic
-00005730: 616d 656e 746f 0a20 2020 2020 2020 2069  amento.        i
-00005740: 6620 6964 5f65 7665 6e74 6f20 6973 206e  f id_evento is n
-00005750: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00005760: 2020 2020 206b 7761 7267 735b 2761 7267       kwargs['arg
-00005770: 3627 5d20 3d20 6964 5f65 7665 6e74 6f0a  6'] = id_evento.
-00005780: 2020 2020 2020 2020 6966 2066 6563 6861          if fecha
-00005790: 5f64 6573 6465 5f6f 7020 6973 206e 6f74  _desde_op is not
-000057a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000057b0: 2020 206b 7761 7267 735b 2761 7267 3727     kwargs['arg7'
-000057c0: 5d20 3d20 6665 6368 615f 6465 7364 655f  ] = fecha_desde_
-000057d0: 6f70 0a20 2020 2020 2020 2069 6620 6665  op.        if fe
-000057e0: 6368 615f 6861 7374 615f 6f70 2069 7320  cha_hasta_op is 
-000057f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00005800: 2020 2020 2020 6b77 6172 6773 5b27 6172        kwargs['ar
-00005810: 6738 275d 203d 2066 6563 6861 5f68 6173  g8'] = fecha_has
-00005820: 7461 5f6f 700a 2020 2020 2020 2020 6966  ta_op.        if
-00005830: 2066 6563 6861 5f64 6573 6465 5f74 2069   fecha_desde_t i
-00005840: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00005850: 2020 2020 2020 2020 6b77 6172 6773 5b27          kwargs['
-00005860: 6172 6739 275d 203d 2066 6563 6861 5f64  arg9'] = fecha_d
-00005870: 6573 6465 5f74 0a20 2020 2020 2020 2069  esde_t.        i
-00005880: 6620 6665 6368 615f 6861 7374 615f 7420  f fecha_hasta_t 
-00005890: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000058a0: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
-000058b0: 2761 7267 3130 275d 203d 2066 6563 6861  'arg10'] = fecha
-000058c0: 5f68 6173 7461 5f74 0a20 2020 2020 2020  _hasta_t.       
-000058d0: 2069 6620 6665 6368 615f 6465 7364 655f   if fecha_desde_
-000058e0: 7620 6973 206e 6f74 204e 6f6e 653a 0a20  v is not None:. 
-000058f0: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
-00005900: 735b 2761 7267 3131 275d 203d 2066 6563  s['arg11'] = fec
-00005910: 6861 5f64 6573 6465 5f76 0a20 2020 2020  ha_desde_v.     
-00005920: 2020 2069 6620 6665 6368 615f 6861 7374     if fecha_hast
-00005930: 615f 7620 6973 206e 6f74 204e 6f6e 653a  a_v is not None:
-00005940: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
-00005950: 7267 735b 2761 7267 3132 275d 203d 2066  rgs['arg12'] = f
-00005960: 6563 6861 5f68 6173 7461 5f76 0a20 2020  echa_hasta_v.   
-00005970: 2020 2020 2069 6620 6e5f 7265 6d69 746f       if n_remito
-00005980: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00005990: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
-000059a0: 5b27 6172 6731 3327 5d20 3d20 6e5f 7265  ['arg13'] = n_re
-000059b0: 6d69 746f 0a20 2020 2020 2020 2069 6620  mito.        if 
-000059c0: 6e5f 6661 6374 7572 6120 6973 206e 6f74  n_factura is not
-000059d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000059e0: 2020 206b 7761 7267 735b 2761 7267 3134     kwargs['arg14
-000059f0: 275d 203d 206e 5f66 6163 7475 7261 0a20  '] = n_factura. 
-00005a00: 2020 2020 2020 2069 6620 6964 5f65 7374         if id_est
-00005a10: 6164 6f20 6973 206e 6f74 204e 6f6e 653a  ado is not None:
-00005a20: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
-00005a30: 7267 735b 2761 7267 3135 275d 203d 2069  rgs['arg15'] = i
-00005a40: 645f 6573 7461 646f 0a20 2020 2020 2020  d_estado.       
-00005a50: 2069 6620 6e72 6f5f 7061 6720 6973 206e   if nro_pag is n
-00005a60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00005a70: 2020 2020 206b 7761 7267 735b 2761 7267       kwargs['arg
-00005a80: 3136 275d 203d 206e 726f 5f70 6167 0a0a  16'] = nro_pag..
-00005a90: 2020 2020 2020 2020 2320 6c6c 616d 6f20          # llamo 
-00005aa0: 616c 2077 6562 7365 7276 6963 650a 2020  al webservice.  
-00005ab0: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
-00005ac0: 2e63 6c69 656e 742e 6765 7454 7261 6e73  .client.getTrans
-00005ad0: 6163 6369 6f6e 6573 5753 280a 2020 2020  accionesWS(.    
-00005ae0: 2020 2020 2020 2020 6172 6730 3d75 7375          arg0=usu
-00005af0: 6172 696f 2c0a 2020 2020 2020 2020 2020  ario,.          
-00005b00: 2020 6172 6731 3d70 6173 7377 6f72 642c    arg1=password,
-00005b10: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
-00005b20: 7761 7267 730a 2020 2020 2020 2020 290a  wargs.        ).
-00005b30: 2020 2020 2020 2020 7265 7420 3d20 7265          ret = re
-00005b40: 735b 2772 6574 7572 6e27 5d0a 2020 2020  s['return'].    
-00005b50: 2020 2020 6966 2072 6574 3a0a 2020 2020      if ret:.    
-00005b60: 2020 2020 2020 2020 7365 6c66 2e5f 5f61          self.__a
-00005b70: 6e61 6c69 7a61 725f 6572 726f 7265 7328  nalizar_errores(
-00005b80: 7265 7429 0a20 2020 2020 2020 2020 2020  ret).           
-00005b90: 2073 656c 662e 4361 6e74 5061 6769 6e61   self.CantPagina
-00005ba0: 7320 3d20 7265 742e 6765 7428 2763 616e  s = ret.get('can
-00005bb0: 7450 6167 696e 6173 2729 0a20 2020 2020  tPaginas').     
-00005bc0: 2020 2020 2020 2073 656c 662e 4861 7945         self.HayE
-00005bd0: 7272 6f72 203d 2072 6574 2e67 6574 2827  rror = ret.get('
-00005be0: 6861 795f 6572 726f 7227 290a 2020 2020  hay_error').    
-00005bf0: 2020 2020 2020 2020 7365 6c66 2e54 7261          self.Tra
-00005c00: 6e73 6163 6369 6f6e 506c 6169 6e57 5320  nsaccionPlainWS 
-00005c10: 3d20 5b69 7420 666f 7220 6974 2069 6e20  = [it for it in 
-00005c20: 7265 742e 6765 7428 276c 6973 7427 2c20  ret.get('list', 
-00005c30: 5b5d 295d 0a20 2020 2020 2020 2072 6574  [])].        ret
-00005c40: 7572 6e20 5472 7565 0a0a 2020 2020 4069  urn True..    @i
-00005c50: 6e69 6369 616c 697a 6172 5f79 5f63 6170  nicializar_y_cap
-00005c60: 7475 7261 725f 6578 6365 7063 696f 6e65  turar_excepcione
-00005c70: 730a 2020 2020 6465 6620 4765 7443 6174  s.    def GetCat
-00005c80: 616c 6f67 6f45 6c65 6374 726f 6e69 636f  alogoElectronico
-00005c90: 4279 4754 494e 280a 2020 2020 2020 2020  ByGTIN(.        
-00005ca0: 7365 6c66 2c20 7573 7561 7269 6f2c 2070  self, usuario, p
-00005cb0: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
-00005cc0: 2063 7569 745f 6661 6272 6963 616e 7465   cuit_fabricante
-00005cd0: 3d4e 6f6e 652c 2067 7469 6e3d 4e6f 6e65  =None, gtin=None
-00005ce0: 2c20 6465 7363 7269 7063 696f 6e3d 4e6f  , descripcion=No
-00005cf0: 6e65 2c0a 2020 2020 2020 2020 6964 5f6d  ne,.        id_m
-00005d00: 6f6e 6f64 726f 6761 3d4e 6f6e 652c 0a20  onodroga=None,. 
-00005d10: 2020 2029 3a0a 2020 2020 2020 2020 224f     ):.        "O
-00005d20: 6274 6965 6e65 2065 6c20 4361 74e1 6c6f  btiene el Cat.lo
-00005d30: 676f 2045 6c65 6374 72f3 6e69 636f 2064  go Electr.nico d
-00005d40: 6520 4d65 6469 6361 6d65 6e74 6f73 220a  e Medicamentos".
-00005d50: 0a20 2020 2020 2020 2023 2070 7265 7061  .        # prepa
-00005d60: 726f 206c 6f73 2070 6172 616d 6574 726f  ro los parametro
-00005d70: 7320 6465 2065 6e74 7261 6461 206f 7063  s de entrada opc
-00005d80: 696f 6e61 6c65 733a 0a20 2020 2020 2020  ionales:.       
-00005d90: 206b 7761 7267 7320 3d20 7b7d 0a20 2020   kwargs = {}.   
-00005da0: 2020 2020 2069 6620 6375 6974 5f66 6162       if cuit_fab
-00005db0: 7269 6361 6e74 6520 6973 206e 6f74 204e  ricante is not N
-00005dc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00005dd0: 206b 7761 7267 735b 2761 7267 3227 5d20   kwargs['arg2'] 
-00005de0: 3d20 6375 6974 5f66 6162 7269 6361 6e74  = cuit_fabricant
-00005df0: 650a 2020 2020 2020 2020 6966 2067 7469  e.        if gti
-00005e00: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-00005e10: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
-00005e20: 735b 2761 7267 3327 5d20 3d20 6774 696e  s['arg3'] = gtin
-00005e30: 0a20 2020 2020 2020 2069 6620 6465 7363  .        if desc
-00005e40: 7269 7063 696f 6e20 6973 206e 6f74 204e  ripcion is not N
-00005e50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00005e60: 206b 7761 7267 735b 2761 7267 3427 5d20   kwargs['arg4'] 
-00005e70: 3d20 6465 7363 7269 7063 696f 6e0a 2020  = descripcion.  
-00005e80: 2020 2020 2020 6966 2069 645f 6d6f 6e6f        if id_mono
-00005e90: 6472 6f67 6120 6973 206e 6f74 204e 6f6e  droga is not Non
-00005ea0: 653a 0a20 2020 2020 2020 2020 2020 206b  e:.            k
-00005eb0: 7761 7267 735b 2761 7267 3527 5d20 3d20  wargs['arg5'] = 
-00005ec0: 6964 5f6d 6f6e 6f64 726f 6761 0a0a 2020  id_monodroga..  
-00005ed0: 2020 2020 2020 2320 6c6c 616d 6f20 616c        # llamo al
-00005ee0: 2077 6562 7365 7276 6963 650a 2020 2020   webservice.    
-00005ef0: 2020 2020 7265 7320 3d20 7365 6c66 2e63      res = self.c
-00005f00: 6c69 656e 742e 6765 7443 6174 616c 6f67  lient.getCatalog
-00005f10: 6f45 6c65 6374 726f 6e69 636f 4279 4754  oElectronicoByGT
-00005f20: 494e 280a 2020 2020 2020 2020 2020 2020  IN(.            
-00005f30: 6172 6730 3d75 7375 6172 696f 2c0a 2020  arg0=usuario,.  
-00005f40: 2020 2020 2020 2020 2020 6172 6731 3d70            arg1=p
-00005f50: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
-00005f60: 2020 2020 202a 2a6b 7761 7267 730a 2020       **kwargs.  
-00005f70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00005f80: 7265 7420 3d20 7265 735b 2772 6574 7572  ret = res['retur
-00005f90: 6e27 5d0a 2020 2020 2020 2020 6966 2072  n'].        if r
-00005fa0: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
-00005fb0: 7365 6c66 2e5f 5f61 6e61 6c69 7a61 725f  self.__analizar_
-00005fc0: 6572 726f 7265 7328 7265 7429 0a20 2020  errores(ret).   
-00005fd0: 2020 2020 2020 2020 2073 656c 662e 4361           self.Ca
-00005fe0: 6e74 5061 6769 6e61 7320 3d20 7265 742e  ntPaginas = ret.
-00005ff0: 6765 7428 2763 616e 7450 6167 696e 6173  get('cantPaginas
-00006000: 2729 0a20 2020 2020 2020 2020 2020 2073  ').            s
-00006010: 656c 662e 4861 7945 7272 6f72 203d 2072  elf.HayError = r
-00006020: 6574 2e67 6574 2827 6861 795f 6572 726f  et.get('hay_erro
-00006030: 7227 290a 2020 2020 2020 2020 2020 2020  r').            
-00006040: 7365 6c66 2e70 6172 616d 735f 6f75 7420  self.params_out 
-00006050: 3d20 6469 6374 280a 2020 2020 2020 2020  = dict(.        
-00006060: 2020 2020 2020 2020 5b28 692c 2069 7429          [(i, it)
-00006070: 2066 6f72 2069 2c20 6974 2069 6e20 656e   for i, it in en
-00006080: 756d 6572 6174 6528 7265 742e 6765 7428  umerate(ret.get(
-00006090: 276c 6973 7427 2c20 5b5d 2929 5d29 0a20  'list', []))]). 
-000060a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000060b0: 6e20 6c65 6e28 7365 6c66 2e70 6172 616d  n len(self.param
-000060c0: 735f 6f75 7429 0a20 2020 2020 2020 2065  s_out).        e
-000060d0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000060e0: 2072 6574 7572 6e20 300a 0a20 2020 2040   return 0..    @
-000060f0: 696e 6963 6961 6c69 7a61 725f 795f 6361  inicializar_y_ca
-00006100: 7074 7572 6172 5f65 7863 6570 6369 6f6e  pturar_excepcion
-00006110: 6573 0a20 2020 2064 6566 2047 6574 436f  es.    def GetCo
-00006120: 6e73 756c 7461 5374 6f63 6b28 0a20 2020  nsultaStock(.   
-00006130: 2020 2020 2073 656c 662c 2075 7375 6172       self, usuar
-00006140: 696f 2c20 7061 7373 776f 7264 2c0a 2020  io, password,.  
-00006150: 2020 2020 2020 6964 5f6d 6564 6963 616d        id_medicam
-00006160: 656e 746f 3d4e 6f6e 652c 2069 645f 6167  ento=None, id_ag
-00006170: 656e 7465 3d4e 6f6e 652c 2064 6573 6372  ente=None, descr
-00006180: 6970 6369 6f6e 3d4e 6f6e 652c 0a20 2020  ipcion=None,.   
-00006190: 2020 2020 2063 616e 7469 6461 643d 4e6f       cantidad=No
-000061a0: 6e65 2c20 7072 6573 656e 7461 6369 6f6e  ne, presentacion
-000061b0: 3d4e 6f6e 652c 0a20 2020 2020 2020 206c  =None,.        l
-000061c0: 6f74 653d 4e6f 6e65 2c20 6e75 6d65 726f  ote=None, numero
-000061d0: 5f73 6572 6961 6c3d 4e6f 6e65 2c0a 2020  _serial=None,.  
-000061e0: 2020 2020 2020 6e72 6f5f 7061 673d 312c        nro_pag=1,
-000061f0: 2063 616e 745f 7265 673d 3130 302c 0a20   cant_reg=100,. 
-00006200: 2020 2029 3a0a 2020 2020 2020 2020 2250     ):.        "P
-00006210: 6572 6d69 7465 2063 6f6e 7375 6c74 6172  ermite consultar
-00006220: 2065 6c20 7374 6f63 6b20 6163 7475 616c   el stock actual
-00006230: 2064 656c 2061 6765 6e74 652e 220a 0a20   del agente.".. 
-00006240: 2020 2020 2020 2023 2070 7265 7061 726f         # preparo
-00006250: 206c 6f73 2070 6172 616d 6574 726f 7320   los parametros 
-00006260: 6465 2065 6e74 7261 6461 206f 7063 696f  de entrada opcio
-00006270: 6e61 6c65 733a 0a20 2020 2020 2020 206b  nales:.        k
-00006280: 7761 7267 7320 3d20 7b7d 0a20 2020 2020  wargs = {}.     
-00006290: 2020 2069 6620 6964 5f6d 6564 6963 616d     if id_medicam
-000062a0: 656e 746f 2069 7320 6e6f 7420 4e6f 6e65  ento is not None
-000062b0: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
-000062c0: 6172 6773 5b27 6172 6732 275d 203d 2069  args['arg2'] = i
-000062d0: 645f 6d65 6469 6361 6d65 6e74 6f0a 2020  d_medicamento.  
-000062e0: 2020 2020 2020 6966 2069 645f 6167 656e        if id_agen
-000062f0: 7465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  te is not None:.
-00006300: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-00006310: 6773 5b27 6172 6733 275d 203d 2069 645f  gs['arg3'] = id_
-00006320: 6167 656e 7465 0a20 2020 2020 2020 2069  agente.        i
-00006330: 6620 6465 7363 7269 7063 696f 6e20 6973  f descripcion is
-00006340: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00006350: 2020 2020 2020 206b 7761 7267 735b 2761         kwargs['a
-00006360: 7267 3427 5d20 3d20 6465 7363 7269 7063  rg4'] = descripc
-00006370: 696f 6e0a 2020 2020 2020 2020 6966 2063  ion.        if c
-00006380: 616e 7469 6461 6420 6973 206e 6f74 204e  antidad is not N
-00006390: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000063a0: 206b 7761 7267 735b 2761 7267 3527 5d20   kwargs['arg5'] 
-000063b0: 3d20 6361 6e74 6964 6164 0a20 2020 2020  = cantidad.     
-000063c0: 2020 2069 6620 7072 6573 656e 7461 6369     if presentaci
-000063d0: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
-000063e0: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-000063f0: 6773 5b27 6172 6736 275d 203d 2070 7265  gs['arg6'] = pre
-00006400: 7365 6e74 6163 696f 6e0a 2020 2020 2020  sentacion.      
-00006410: 2020 6966 206c 6f74 6520 6973 206e 6f74    if lote is not
-00006420: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00006430: 2020 206b 7761 7267 735b 2761 7267 3727     kwargs['arg7'
-00006440: 5d20 3d20 6c6f 7465 0a20 2020 2020 2020  ] = lote.       
-00006450: 2069 6620 6e75 6d65 726f 5f73 6572 6961   if numero_seria
-00006460: 6c20 6973 206e 6f74 204e 6f6e 653a 0a20  l is not None:. 
-00006470: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
-00006480: 735b 2761 7267 3827 5d20 3d20 6e75 6d65  s['arg8'] = nume
-00006490: 726f 5f73 6572 6961 6c0a 2020 2020 2020  ro_serial.      
-000064a0: 2020 6966 206e 726f 5f70 6167 2069 7320    if nro_pag is 
-000064b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000064c0: 2020 2020 2020 6b77 6172 6773 5b27 6172        kwargs['ar
-000064d0: 6739 275d 203d 206e 726f 5f70 6167 0a20  g9'] = nro_pag. 
-000064e0: 2020 2020 2020 2069 6620 6361 6e74 5f72         if cant_r
-000064f0: 6567 2069 7320 6e6f 7420 4e6f 6e65 3a0a  eg is not None:.
-00006500: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-00006510: 6773 5b27 6172 6731 3027 5d20 3d20 6361  gs['arg10'] = ca
-00006520: 6e74 5f72 6567 0a0a 2020 2020 2020 2020  nt_reg..        
-00006530: 2320 6c6c 616d 6f20 616c 2077 6562 7365  # llamo al webse
-00006540: 7276 6963 650a 2020 2020 2020 2020 7265  rvice.        re
-00006550: 7320 3d20 7365 6c66 2e63 6c69 656e 742e  s = self.client.
-00006560: 6765 7443 6f6e 7375 6c74 6153 746f 636b  getConsultaStock
-00006570: 280a 2020 2020 2020 2020 2020 2020 6172  (.            ar
-00006580: 6730 3d75 7375 6172 696f 2c0a 2020 2020  g0=usuario,.    
-00006590: 2020 2020 2020 2020 6172 6731 3d70 6173          arg1=pas
-000065a0: 7377 6f72 642c 0a20 2020 2020 2020 2020  sword,.         
-000065b0: 2020 202a 2a6b 7761 7267 730a 2020 2020     **kwargs.    
-000065c0: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
-000065d0: 7420 3d20 7265 735b 2772 6574 7572 6e27  t = res['return'
-000065e0: 5d0a 2020 2020 2020 2020 6966 2072 6574  ].        if ret
-000065f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00006600: 6c66 2e5f 5f61 6e61 6c69 7a61 725f 6572  lf.__analizar_er
-00006610: 726f 7265 7328 7265 7429 0a20 2020 2020  rores(ret).     
-00006620: 2020 2020 2020 2073 656c 662e 4361 6e74         self.Cant
-00006630: 5061 6769 6e61 7320 3d20 7265 742e 6765  Paginas = ret.ge
-00006640: 7428 2763 616e 7450 6167 696e 6173 2729  t('cantPaginas')
-00006650: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006660: 662e 4861 7945 7272 6f72 203d 2072 6574  f.HayError = ret
-00006670: 2e67 6574 2827 6861 795f 6572 726f 7227  .get('hay_error'
-00006680: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00006690: 6c66 2e70 6172 616d 735f 6f75 7420 3d20  lf.params_out = 
-000066a0: 6469 6374 280a 2020 2020 2020 2020 2020  dict(.          
-000066b0: 2020 2020 2020 5b28 692c 2069 7429 2066        [(i, it) f
-000066c0: 6f72 2069 2c20 6974 2069 6e20 656e 756d  or i, it in enum
-000066d0: 6572 6174 6528 7265 742e 6765 7428 276c  erate(ret.get('l
-000066e0: 6973 7427 2c20 5b5d 2929 5d29 0a20 2020  ist', []))]).   
-000066f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00006700: 6c65 6e28 7365 6c66 2e70 6172 616d 735f  len(self.params_
-00006710: 6f75 7429 0a20 2020 2020 2020 2065 6c73  out).        els
-00006720: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00006730: 6574 7572 6e20 300a 0a20 2020 2064 6566  eturn 0..    def
-00006740: 2053 6574 5573 6572 6e61 6d65 2873 656c   SetUsername(sel
-00006750: 662c 2075 7365 726e 616d 6529 3a0a 2020  f, username):.  
-00006760: 2020 2020 2020 2245 7374 6162 6c65 7a63        "Establezc
-00006770: 6f20 656c 206e 6f6d 6272 6520 6465 2075  o el nombre de u
-00006780: 7375 6172 696f 220a 2020 2020 2020 2020  suario".        
-00006790: 7365 6c66 2e55 7365 726e 616d 6520 3d20  self.Username = 
-000067a0: 7573 6572 6e61 6d65 0a0a 2020 2020 6465  username..    de
-000067b0: 6620 5365 7450 6173 7377 6f72 6428 7365  f SetPassword(se
-000067c0: 6c66 2c20 7061 7373 776f 7264 293a 0a20  lf, password):. 
-000067d0: 2020 2020 2020 2022 4573 7461 626c 657a         "Establez
-000067e0: 636f 206c 6120 636f 6e74 7261 7365 f161  co la contrase.a
-000067f0: 220a 2020 2020 2020 2020 7365 6c66 2e50  ".        self.P
-00006800: 6173 7377 6f72 6420 3d20 7061 7373 776f  assword = passwo
-00006810: 7264 0a0a 2020 2020 6465 6620 4765 7443  rd..    def GetC
-00006820: 6f64 6967 6f54 7261 6e73 6163 6369 6f6e  odigoTransaccion
-00006830: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00006840: 2244 6576 7565 6c76 6f20 656c 2063 f364  "Devuelvo el c.d
-00006850: 6967 6f20 6465 2074 7261 6e73 6163 6369  igo de transacci
-00006860: f36e 220a 2020 2020 2020 2020 7265 7475  .n".        retu
-00006870: 726e 2073 656c 662e 436f 6469 676f 5472  rn self.CodigoTr
-00006880: 616e 7361 6363 696f 6e0a 0a20 2020 2064  ansaccion..    d
-00006890: 6566 2047 6574 5265 7375 6c74 6164 6f28  ef GetResultado(
-000068a0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000068b0: 4465 7675 656c 766f 2065 6c20 7265 7375  Devuelvo el resu
-000068c0: 6c74 6164 6f22 0a20 2020 2020 2020 2072  ltado".        r
-000068d0: 6574 7572 6e20 7365 6c66 2e52 6573 756c  eturn self.Resul
-000068e0: 7461 646f 0a0a 0a64 6566 206d 6169 6e28  tado...def main(
-000068f0: 293a 0a20 2020 2022 4675 6e63 69f3 6e20  ):.    "Funci.n 
-00006900: 7072 696e 6369 7061 6c20 6465 2070 7275  principal de pru
-00006910: 6562 6173 2028 6f62 7465 6e65 7220 4341  ebas (obtener CA
-00006920: 4529 220a 2020 2020 696d 706f 7274 206f  E)".    import o
-00006930: 730a 2020 2020 696d 706f 7274 2074 696d  s.    import tim
-00006940: 650a 2020 2020 696d 706f 7274 2073 7973  e.    import sys
-00006950: 0a20 2020 2067 6c6f 6261 6c20 5753 444c  .    global WSDL
-00006960: 2c20 4c4f 4341 5449 4f4e 0a0a 2020 2020  , LOCATION..    
-00006970: 4445 4255 4720 3d20 272d 2d64 6562 7567  DEBUG = '--debug
-00006980: 2720 696e 2073 7973 2e61 7267 760a 2020  ' in sys.argv.  
-00006990: 2020 7072 696e 7428 4445 4255 4729 0a0a    print(DEBUG)..
-000069a0: 2020 2020 7773 203d 2054 7261 7a61 4d65      ws = TrazaMe
-000069b0: 6428 290a 0a20 2020 2077 732e 5573 6572  d()..    ws.User
-000069c0: 6e61 6d65 203d 2027 7465 7374 7773 6572  name = 'testwser
-000069d0: 7669 6365 270a 2020 2020 7773 2e50 6173  vice'.    ws.Pas
-000069e0: 7377 6f72 6420 3d20 2774 6573 7477 7365  sword = 'testwse
-000069f0: 7276 6963 6570 7377 270a 0a20 2020 2069  rvicepsw'..    i
-00006a00: 6620 272d 2d70 726f 6427 2069 6e20 7379  f '--prod' in sy
-00006a10: 732e 6172 6776 2061 6e64 206e 6f74 2048  s.argv and not H
-00006a20: 4f4d 4f3a 0a20 2020 2020 2020 2057 5344  OMO:.        WSD
-00006a30: 4c20 3d20 2268 7474 7073 3a2f 2f74 7261  L = "https://tra
-00006a40: 7a61 6269 6c69 6461 642e 7061 6d69 2e6f  zabilidad.pami.o
-00006a50: 7267 2e61 723a 3930 3530 2f74 7261 7a61  rg.ar:9050/traza
-00006a60: 6d65 642e 5765 6253 6572 7669 6365 220a  med.WebService".
-00006a70: 2020 2020 2020 2020 7072 696e 7428 2255          print("U
-00006a80: 7361 6e64 6f20 5753 444c 3a22 2c20 5753  sando WSDL:", WS
-00006a90: 444c 290a 2020 2020 2020 2020 7379 732e  DL).        sys.
-00006aa0: 6172 6776 2e70 6f70 2873 7973 2e61 7267  argv.pop(sys.arg
-00006ab0: 762e 696e 6465 7828 222d 2d70 726f 6422  v.index("--prod"
-00006ac0: 2929 0a0a 2020 2020 2320 496e 6963 6961  ))..    # Inicia
-00006ad0: 6c69 7a6f 206c 6173 2076 6172 6961 626c  lizo las variabl
-00006ae0: 6573 2079 2065 7374 7275 6374 7572 6173  es y estructuras
-00006af0: 2070 6172 6120 656c 2061 7263 6869 766f   para el archivo
-00006b00: 2064 6520 696e 7465 7263 616d 6269 6f3a   de intercambio:
-00006b10: 0a20 2020 206d 6564 6963 616d 656e 746f  .    medicamento
-00006b20: 7320 3d20 5b5d 0a20 2020 2074 7261 6e73  s = [].    trans
-00006b30: 6163 6369 6f6e 6573 203d 205b 5d0a 2020  acciones = [].  
-00006b40: 2020 6572 726f 7265 7320 3d20 5b5d 0a20    errores = []. 
-00006b50: 2020 2066 6f72 6d61 746f 7320 3d20 5b0a     formatos = [.
-00006b60: 2020 2020 2020 2020 2827 4d65 6469 6361          ('Medica
-00006b70: 6d65 6e74 6f73 272c 204d 4544 4943 414d  mentos', MEDICAM
-00006b80: 454e 544f 532c 206d 6564 6963 616d 656e  ENTOS, medicamen
-00006b90: 746f 7329 2c0a 2020 2020 2020 2020 2827  tos),.        ('
-00006ba0: 5472 616e 7361 6363 696f 6e65 7327 2c20  Transacciones', 
-00006bb0: 5452 414e 5341 4343 494f 4e45 532c 2074  TRANSACCIONES, t
-00006bc0: 7261 6e73 6163 6369 6f6e 6573 292c 0a20  ransacciones),. 
-00006bd0: 2020 2020 2020 2028 2745 7272 6f72 6573         ('Errores
-00006be0: 272c 2045 5252 4f52 4553 2c20 6572 726f  ', ERRORES, erro
-00006bf0: 7265 7329 2c0a 2020 2020 5d0a 0a20 2020  res),.    ]..   
-00006c00: 2069 6620 272d 2d66 6f72 6d61 746f 2720   if '--formato' 
-00006c10: 696e 2073 7973 2e61 7267 763a 0a20 2020  in sys.argv:.   
-00006c20: 2020 2020 2070 7269 6e74 2822 466f 726d       print("Form
-00006c30: 6174 6f3a 2229 0a20 2020 2020 2020 2066  ato:").        f
-00006c40: 6f72 206d 7367 2c20 666f 726d 6174 6f2c  or msg, formato,
-00006c50: 206c 6973 7461 2069 6e20 666f 726d 6174   lista in format
-00006c60: 6f73 3a0a 2020 2020 2020 2020 2020 2020  os:.            
-00006c70: 636f 6d69 656e 7a6f 203d 2031 0a20 2020  comienzo = 1.   
-00006c80: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-00006c90: 3d3d 3d20 2573 203d 3d3d 2220 2520 6d73  === %s ===" % ms
-00006ca0: 6729 0a20 2020 2020 2020 2020 2020 2070  g).            p
-00006cb0: 7269 6e74 2822 7c7c 2025 2d32 3573 207c  rint("|| %-25s |
-00006cc0: 7c20 252d 3132 7320 7c7c 2025 2d35 7320  | %-12s || %-5s 
-00006cd0: 7c7c 2025 2d34 7320 7c7c 2025 2d31 3073  || %-4s || %-10s
-00006ce0: 207c 7c22 2025 2028 0a20 2020 2020 2020   ||" % (.       
-00006cf0: 2020 2020 2020 2020 2022 4e6f 6d62 7265           "Nombre
-00006d00: 222c 2022 5469 706f 222c 2022 4c6f 6e67  ", "Tipo", "Long
-00006d10: 2e22 2c20 2250 6f73 2874 7874 2922 2c20  .", "Pos(txt)", 
-00006d20: 2243 616d 706f 2864 6266 2922 2929 0a20  "Campo(dbf)")). 
-00006d30: 2020 2020 2020 2020 2020 2063 6c61 7665             clave
-00006d40: 7320 3d20 5b5d 0a20 2020 2020 2020 2020  s = [].         
-00006d50: 2020 2066 6f72 2066 6d74 2069 6e20 666f     for fmt in fo
-00006d60: 726d 6174 6f3a 0a20 2020 2020 2020 2020  rmato:.         
-00006d70: 2020 2020 2020 2063 6c61 7665 2c20 6c6f         clave, lo
-00006d80: 6e67 6974 7564 2c20 7469 706f 203d 2066  ngitud, tipo = f
-00006d90: 6d74 5b30 3a33 5d0a 2020 2020 2020 2020  mt[0:3].        
-00006da0: 2020 2020 2020 2020 636c 6176 655f 6462          clave_db
-00006db0: 6620 3d20 6461 725f 6e6f 6d62 7265 5f63  f = dar_nombre_c
-00006dc0: 616d 706f 5f64 6266 2863 6c61 7665 2c20  ampo_dbf(clave, 
-00006dd0: 636c 6176 6573 290a 2020 2020 2020 2020  claves).        
-00006de0: 2020 2020 2020 2020 636c 6176 6573 2e61          claves.a
-00006df0: 7070 656e 6428 636c 6176 655f 6462 6629  ppend(clave_dbf)
-00006e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006e10: 2070 7269 6e74 2822 7c7c 2025 2d32 3573   print("|| %-25s
-00006e20: 207c 7c20 252d 3132 7320 7c7c 2025 3564   || %-12s || %5d
-00006e30: 207c 7c20 2020 2534 6420 2020 7c7c 2025   ||   %4d   || %
-00006e40: 2d31 3073 207c 7c22 2025 2028 0a20 2020  -10s ||" % (.   
-00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e60: 2063 6c61 7665 2c20 7469 706f 2c20 6c6f   clave, tipo, lo
-00006e70: 6e67 6974 7564 2c20 636f 6d69 656e 7a6f  ngitud, comienzo
-00006e80: 2c20 636c 6176 655f 6462 6629 290a 2020  , clave_dbf)).  
-00006e90: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00006ea0: 6d69 656e 7a6f 202b 3d20 6c6f 6e67 6974  mienzo += longit
-00006eb0: 7564 0a20 2020 2020 2020 2073 7973 2e65  ud.        sys.e
-00006ec0: 7869 7428 3029 0a0a 2020 2020 6966 2027  xit(0)..    if '
-00006ed0: 2d2d 6361 7267 6172 2720 696e 2073 7973  --cargar' in sys
-00006ee0: 2e61 7267 763a 0a20 2020 2020 2020 2069  .argv:.        i
-00006ef0: 6620 272d 2d64 6266 2720 696e 2073 7973  f '--dbf' in sys
-00006f00: 2e61 7267 763a 0a20 2020 2020 2020 2020  .argv:.         
-00006f10: 2020 206c 6565 725f 6462 6628 666f 726d     leer_dbf(form
-00006f20: 6174 6f73 5b3a 315d 2c20 7b7d 290a 2020  atos[:1], {}).  
-00006f30: 2020 2020 2020 656c 6966 2027 2d2d 6a73        elif '--js
-00006f40: 6f6e 2720 696e 2073 7973 2e61 7267 763a  on' in sys.argv:
-00006f50: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00006f60: 2066 6f72 6d61 746f 2069 6e20 666f 726d   formato in form
-00006f70: 6174 6f73 5b3a 315d 3a0a 2020 2020 2020  atos[:1]:.      
-00006f80: 2020 2020 2020 2020 2020 6172 6368 6976            archiv
-00006f90: 6f20 3d20 6f70 656e 2866 6f72 6d61 746f  o = open(formato
-00006fa0: 5b30 5d2e 6c6f 7765 7228 2920 2b20 222e  [0].lower() + ".
-00006fb0: 6a73 6f6e 222c 2022 7222 290a 2020 2020  json", "r").    
-00006fc0: 2020 2020 2020 2020 2020 2020 6420 3d20              d = 
-00006fd0: 6a73 6f6e 2e6c 6f61 6428 6172 6368 6976  json.load(archiv
-00006fe0: 6f29 0a20 2020 2020 2020 2020 2020 2020  o).             
-00006ff0: 2020 2066 6f72 6d61 746f 5b32 5d2e 6578     formato[2].ex
-00007000: 7465 6e64 2864 290a 2020 2020 2020 2020  tend(d).        
-00007010: 2020 2020 2020 2020 6172 6368 6976 6f2e          archivo.
-00007020: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
-00007030: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00007040: 2020 666f 7220 666f 726d 6174 6f20 696e    for formato in
-00007050: 2066 6f72 6d61 746f 735b 3a31 5d3a 0a20   formatos[:1]:. 
-00007060: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00007070: 7263 6869 766f 203d 206f 7065 6e28 666f  rchivo = open(fo
-00007080: 726d 6174 6f5b 305d 2e6c 6f77 6572 2829  rmato[0].lower()
-00007090: 202b 2022 2e74 7874 222c 2022 7222 290a   + ".txt", "r").
-000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070b0: 666f 7220 6c69 6e65 6120 696e 2061 7263  for linea in arc
-000070c0: 6869 766f 3a0a 2020 2020 2020 2020 2020  hivo:.          
-000070d0: 2020 2020 2020 2020 2020 6420 3d20 6c65            d = le
-000070e0: 6572 286c 696e 6561 2c20 666f 726d 6174  er(linea, format
-000070f0: 6f5b 315d 290a 2020 2020 2020 2020 2020  o[1]).          
-00007100: 2020 2020 2020 2020 2020 666f 726d 6174            format
-00007110: 6f5b 325d 2e61 7070 656e 6428 6429 0a20  o[2].append(d). 
-00007120: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00007130: 7263 6869 766f 2e63 6c6f 7365 2829 0a0a  rchivo.close()..
-00007140: 2020 2020 7773 2e43 6f6e 6563 7461 7228      ws.Conectar(
-00007150: 2222 2c20 5753 444c 290a 0a20 2020 2069  "", WSDL)..    i
-00007160: 6620 7773 2e45 7863 6570 6369 6f6e 3a0a  f ws.Excepcion:.
-00007170: 2020 2020 2020 2020 7072 696e 7428 7773          print(ws
-00007180: 2e45 7863 6570 6369 6f6e 290a 2020 2020  .Excepcion).    
-00007190: 2020 2020 7072 696e 7428 7773 2e54 7261      print(ws.Tra
-000071a0: 6365 6261 636b 290a 2020 2020 2020 2020  ceback).        
-000071b0: 7379 732e 6578 6974 282d 3129 0a0a 2020  sys.exit(-1)..  
-000071c0: 2020 2320 4461 746f 7320 6465 2070 7275    # Datos de pru
-000071d0: 6562 6173 3a0a 0a20 2020 2069 6620 272d  ebas:..    if '-
-000071e0: 2d74 6573 7427 2069 6e20 7379 732e 6172  -test' in sys.ar
-000071f0: 6776 3a0a 2020 2020 2020 2020 6d65 6469  gv:.        medi
-00007200: 6361 6d65 6e74 6f73 2e61 7070 656e 6428  camentos.append(
-00007210: 6469 6374 280a 2020 2020 2020 2020 2020  dict(.          
-00007220: 2020 665f 6576 656e 746f 3d64 6174 6574    f_evento=datet
-00007230: 696d 652e 6461 7465 7469 6d65 2e6e 6f77  ime.datetime.now
-00007240: 2829 2e73 7472 6674 696d 6528 2225 642f  ().strftime("%d/
-00007250: 256d 2f25 5922 292c 0a20 2020 2020 2020  %m/%Y"),.       
-00007260: 2020 2020 2068 5f65 7665 6e74 6f3d 6461       h_evento=da
-00007270: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
-00007280: 6e6f 7728 292e 7374 7266 7469 6d65 2822  now().strftime("
-00007290: 2548 3a25 4d22 292c 0a20 2020 2020 2020  %H:%M"),.       
-000072a0: 2020 2020 2067 6c6e 5f6f 7269 6765 6e3d       gln_origen=
-000072b0: 2239 3939 3939 3939 3939 3939 3138 222c  "9999999999918",
-000072c0: 2067 6c6e 5f64 6573 7469 6e6f 3d22 676c   gln_destino="gl
-000072d0: 6e77 7322 2c0a 2020 2020 2020 2020 2020  nws",.          
-000072e0: 2020 6e5f 7265 6d69 746f 3d22 5230 3030    n_remito="R000
-000072f0: 3130 3030 3031 3233 3422 2c20 6e5f 6661  100001234", n_fa
-00007300: 6374 7572 613d 2241 3030 3031 3030 3030  ctura="A00010000
-00007310: 3132 3334 222c 0a20 2020 2020 2020 2020  1234",.         
-00007320: 2020 2076 656e 6369 6d69 656e 746f 3d28     vencimiento=(
-00007330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007340: 2064 6174 6574 696d 652e 6461 7465 7469   datetime.dateti
-00007350: 6d65 2e6e 6f77 2829 2b64 6174 6574 696d  me.now()+datetim
-00007360: 652e 7469 6d65 6465 6c74 6128 3330 290a  e.timedelta(30).
-00007370: 2020 2020 2020 2020 2020 2020 292e 7374              ).st
-00007380: 7266 7469 6d65 2822 2564 2f25 6d2f 2559  rftime("%d/%m/%Y
-00007390: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-000073a0: 6774 696e 3d22 4754 494e 3122 2c20 6c6f  gtin="GTIN1", lo
-000073b0: 7465 3d64 6174 6574 696d 652e 6461 7465  te=datetime.date
-000073c0: 7469 6d65 2e6e 6f77 2829 2e73 7472 6674  time.now().strft
-000073d0: 696d 6528 2225 5922 292c 0a20 2020 2020  ime("%Y"),.     
-000073e0: 2020 2020 2020 206e 756d 6572 6f5f 7365         numero_se
-000073f0: 7269 616c 3d69 6e74 2874 696d 652e 7469  rial=int(time.ti
-00007400: 6d65 2829 2a31 3029 2c0a 2020 2020 2020  me()*10),.      
-00007410: 2020 2020 2020 6964 5f6f 6272 615f 736f        id_obra_so
-00007420: 6369 616c 3d4e 6f6e 652c 2069 645f 6576  cial=None, id_ev
-00007430: 656e 746f 3d31 3334 2c0a 2020 2020 2020  ento=134,.      
-00007440: 2020 2020 2020 6375 6974 5f6f 7269 6765        cuit_orige
-00007450: 6e3d 2232 3032 3637 3536 3533 3933 222c  n="20267565393",
-00007460: 2063 7569 745f 6465 7374 696e 6f3d 2232   cuit_destino="2
-00007470: 3032 3637 3536 3533 3933 222c 0a20 2020  0267565393",.   
-00007480: 2020 2020 2020 2020 2061 7065 6c6c 6964           apellid
-00007490: 6f3d 2252 6569 6e67 6172 7422 2c20 6e6f  o="Reingart", no
-000074a0: 6d62 7265 733d 224d 6172 6961 6e6f 222c  mbres="Mariano",
-000074b0: 0a20 2020 2020 2020 2020 2020 2074 6970  .            tip
-000074c0: 6f5f 646f 6375 6d65 6e74 6f3d 2239 3622  o_documento="96"
-000074d0: 2c20 6e5f 646f 6375 6d65 6e74 6f3d 2232  , n_documento="2
-000074e0: 3637 3536 3533 3922 2c20 7365 786f 3d22  6756539", sexo="
-000074f0: 4d22 2c0a 2020 2020 2020 2020 2020 2020  M",.            
-00007500: 6469 7265 6363 696f 6e3d 2253 6172 617a  direccion="Saraz
-00007510: 6122 2c20 6e75 6d65 726f 3d22 3132 3334  a", numero="1234
-00007520: 222c 2070 6973 6f3d 2222 2c20 6465 7074  ", piso="", dept
-00007530: 6f3d 2222 2c0a 2020 2020 2020 2020 2020  o="",.          
-00007540: 2020 6c6f 6361 6c69 6461 643d 2248 7572    localidad="Hur
-00007550: 6c69 6e67 6861 6d22 2c20 7072 6f76 696e  lingham", provin
-00007560: 6369 613d 2242 7565 6e6f 7320 4169 7265  cia="Buenos Aire
-00007570: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00007580: 6e5f 706f 7374 616c 3d22 3136 3838 222c  n_postal="1688",
-00007590: 2066 6563 6861 5f6e 6163 696d 6965 6e74   fecha_nacimient
-000075a0: 6f3d 2230 312f 3031 2f32 3030 3022 2c0a  o="01/01/2000",.
-000075b0: 2020 2020 2020 2020 2020 2020 7465 6c65              tele
-000075c0: 666f 6e6f 3d22 3535 3535 2d35 3535 3522  fono="5555-5555"
-000075d0: 2c0a 2020 2020 2020 2020 2020 2020 6e72  ,.            nr
-000075e0: 6f5f 6173 6f63 6961 646f 3d22 3939 3939  o_asociado="9999
-000075f0: 3939 3939 3939 3939 3922 2c0a 2020 2020  999999999",.    
-00007600: 2020 2020 2020 2020 6361 6e74 6964 6164          cantidad
-00007610: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-00007620: 2020 2064 6573 6465 5f6e 756d 6572 6f5f     desde_numero_
-00007630: 7365 7269 616c 3d4e 6f6e 652c 2068 6173  serial=None, has
-00007640: 7461 5f6e 756d 6572 6f5f 7365 7269 616c  ta_numero_serial
-00007650: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-00007660: 2020 2063 6f64 6967 6f5f 7472 616e 7361     codigo_transa
-00007670: 6363 696f 6e3d 4e6f 6e65 2c0a 2020 2020  ccion=None,.    
-00007680: 2020 2020 2929 0a20 2020 2069 6620 272d      )).    if '-
-00007690: 2d74 6573 7466 7261 6363 696f 6e27 2069  -testfraccion' i
-000076a0: 6e20 7379 732e 6172 6776 3a0a 2020 2020  n sys.argv:.    
-000076b0: 2020 2020 6d65 6469 6361 6d65 6e74 6f73      medicamentos
-000076c0: 2e61 7070 656e 6428 6469 6374 280a 2020  .append(dict(.  
-000076d0: 2020 2020 2020 2020 2020 665f 6576 656e            f_even
-000076e0: 746f 3d64 6174 6574 696d 652e 6461 7465  to=datetime.date
-000076f0: 7469 6d65 2e6e 6f77 2829 2e73 7472 6674  time.now().strft
-00007700: 696d 6528 2225 642f 256d 2f25 5922 292c  ime("%d/%m/%Y"),
-00007710: 0a20 2020 2020 2020 2020 2020 2068 5f65  .            h_e
-00007720: 7665 6e74 6f3d 6461 7465 7469 6d65 2e64  vento=datetime.d
-00007730: 6174 6574 696d 652e 6e6f 7728 292e 7374  atetime.now().st
-00007740: 7266 7469 6d65 2822 2548 3a25 4d22 292c  rftime("%H:%M"),
-00007750: 0a20 2020 2020 2020 2020 2020 2067 6c6e  .            gln
-00007760: 5f6f 7269 6765 6e3d 2239 3939 3939 3939  _origen="9999999
-00007770: 3939 3939 3138 222c 2067 6c6e 5f64 6573  999918", gln_des
-00007780: 7469 6e6f 3d22 676c 6e77 7322 2c0a 2020  tino="glnws",.  
-00007790: 2020 2020 2020 2020 2020 6e5f 7265 6d69            n_remi
-000077a0: 746f 3d22 3132 3334 222c 206e 5f66 6163  to="1234", n_fac
-000077b0: 7475 7261 3d22 3132 3334 222c 0a20 2020  tura="1234",.   
-000077c0: 2020 2020 2020 2020 2076 656e 6369 6d69           vencimi
-000077d0: 656e 746f 3d28 0a20 2020 2020 2020 2020  ento=(.         
-000077e0: 2020 2020 2020 2064 6174 6574 696d 652e         datetime.
-000077f0: 6461 7465 7469 6d65 2e6e 6f77 2829 2b64  datetime.now()+d
-00007800: 6174 6574 696d 652e 7469 6d65 6465 6c74  atetime.timedelt
-00007810: 6128 3330 290a 2020 2020 2020 2020 2020  a(30).          
-00007820: 2020 292e 7374 7266 7469 6d65 2822 2564    ).strftime("%d
-00007830: 2f25 6d2f 2559 2229 2c0a 2020 2020 2020  /%m/%Y"),.      
-00007840: 2020 2020 2020 6774 696e 3d22 4754 494e        gtin="GTIN
-00007850: 3122 2c20 6c6f 7465 3d64 6174 6574 696d  1", lote=datetim
-00007860: 652e 6461 7465 7469 6d65 2e6e 6f77 2829  e.datetime.now()
-00007870: 2e73 7472 6674 696d 6528 2225 5922 292c  .strftime("%Y"),
-00007880: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
-00007890: 6572 6f5f 7365 7269 616c 3d69 6e74 2874  ero_serial=int(t
-000078a0: 696d 652e 7469 6d65 2829 2a31 3029 2c0a  ime.time()*10),.
-000078b0: 2020 2020 2020 2020 2020 2020 6964 5f6f              id_o
-000078c0: 6272 615f 736f 6369 616c 3d4e 6f6e 652c  bra_social=None,
-000078d0: 2069 645f 6576 656e 746f 3d31 3334 2c0a   id_evento=134,.
-000078e0: 2020 2020 2020 2020 2020 2020 6375 6974              cuit
-000078f0: 5f6f 7269 6765 6e3d 2232 3032 3637 3536  _origen="2026756
-00007900: 3533 3933 222c 2063 7569 745f 6465 7374  5393", cuit_dest
-00007910: 696e 6f3d 2232 3032 3637 3536 3533 3933  ino="20267565393
-00007920: 222c 0a20 2020 2020 2020 2020 2020 2061  ",.            a
-00007930: 7065 6c6c 6964 6f3d 2252 6569 6e67 6172  pellido="Reingar
-00007940: 7422 2c20 6e6f 6d62 7265 733d 224d 6172  t", nombres="Mar
-00007950: 6961 6e6f 222c 0a20 2020 2020 2020 2020  iano",.         
-00007960: 2020 2074 6970 6f5f 646f 6375 6d65 6e74     tipo_document
-00007970: 6f3d 2239 3622 2c20 6e5f 646f 6375 6d65  o="96", n_docume
-00007980: 6e74 6f3d 2232 3637 3536 3533 3922 2c20  nto="26756539", 
-00007990: 7365 786f 3d22 4d22 2c0a 2020 2020 2020  sexo="M",.      
-000079a0: 2020 2020 2020 6469 7265 6363 696f 6e3d        direccion=
-000079b0: 2253 6172 617a 6122 2c20 6e75 6d65 726f  "Saraza", numero
-000079c0: 3d22 3132 3334 222c 2070 6973 6f3d 2222  ="1234", piso=""
-000079d0: 2c20 6465 7074 6f3d 2222 2c0a 2020 2020  , depto="",.    
-000079e0: 2020 2020 2020 2020 6c6f 6361 6c69 6461          localida
-000079f0: 643d 2248 7572 6c69 6e67 6861 6d22 2c20  d="Hurlingham", 
-00007a00: 7072 6f76 696e 6369 613d 2242 7565 6e6f  provincia="Bueno
-00007a10: 7320 4169 7265 7322 2c0a 2020 2020 2020  s Aires",.      
-00007a20: 2020 2020 2020 6e5f 706f 7374 616c 3d22        n_postal="
-00007a30: 3136 3838 222c 2066 6563 6861 5f6e 6163  1688", fecha_nac
-00007a40: 696d 6965 6e74 6f3d 2230 312f 3031 2f32  imiento="01/01/2
-00007a50: 3030 3022 2c0a 2020 2020 2020 2020 2020  000",.          
-00007a60: 2020 7465 6c65 666f 6e6f 3d22 3535 3535    telefono="5555
-00007a70: 2d35 3535 3522 2c0a 2020 2020 2020 2020  -5555",.        
-00007a80: 2020 2020 6e72 6f5f 6173 6f63 6961 646f      nro_asociado
-00007a90: 3d22 3939 3939 3939 3939 3939 3939 3922  ="9999999999999"
-00007aa0: 2c0a 2020 2020 2020 2020 2020 2020 6361  ,.            ca
-00007ab0: 6e74 6964 6164 3d35 2c0a 2020 2020 2020  ntidad=5,.      
-00007ac0: 2020 2020 2020 6465 7364 655f 6e75 6d65        desde_nume
-00007ad0: 726f 5f73 6572 6961 6c3d 4e6f 6e65 2c20  ro_serial=None, 
-00007ae0: 6861 7374 615f 6e75 6d65 726f 5f73 6572  hasta_numero_ser
-00007af0: 6961 6c3d 4e6f 6e65 2c0a 2020 2020 2020  ial=None,.      
-00007b00: 2020 2020 2020 636f 6469 676f 5f74 7261        codigo_tra
-00007b10: 6e73 6163 6369 6f6e 3d4e 6f6e 652c 0a20  nsaccion=None,. 
-00007b20: 2020 2020 2020 2029 290a 2020 2020 6966         )).    if
-00007b30: 2027 2d2d 7465 7374 6468 2720 696e 2073   '--testdh' in s
-00007b40: 7973 2e61 7267 763a 0a20 2020 2020 2020  ys.argv:.       
-00007b50: 206d 6564 6963 616d 656e 746f 732e 6170   medicamentos.ap
-00007b60: 7065 6e64 2864 6963 7428 0a20 2020 2020  pend(dict(.     
-00007b70: 2020 2020 2020 2066 5f65 7665 6e74 6f3d         f_evento=
-00007b80: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
-00007b90: 652e 6e6f 7728 292e 7374 7266 7469 6d65  e.now().strftime
-00007ba0: 2822 2564 2f25 6d2f 2559 2229 2c0a 2020  ("%d/%m/%Y"),.  
-00007bb0: 2020 2020 2020 2020 2020 685f 6576 656e            h_even
-00007bc0: 746f 3d64 6174 6574 696d 652e 6461 7465  to=datetime.date
-00007bd0: 7469 6d65 2e6e 6f77 2829 2e73 7472 6674  time.now().strft
-00007be0: 696d 6528 2225 483a 254d 2229 2c0a 2020  ime("%H:%M"),.  
-00007bf0: 2020 2020 2020 2020 2020 676c 6e5f 6f72            gln_or
-00007c00: 6967 656e 3d22 3939 3939 3939 3939 3939  igen="9999999999
-00007c10: 3931 3822 2c20 676c 6e5f 6465 7374 696e  918", gln_destin
-00007c20: 6f3d 2267 6c6e 7773 222c 0a20 2020 2020  o="glnws",.     
-00007c30: 2020 2020 2020 206e 5f72 656d 6974 6f3d         n_remito=
-00007c40: 2231 3233 3422 2c20 6e5f 6661 6374 7572  "1234", n_factur
-00007c50: 613d 2231 3233 3422 2c0a 2020 2020 2020  a="1234",.      
-00007c60: 2020 2020 2020 7665 6e63 696d 6965 6e74        vencimient
-00007c70: 6f3d 280a 2020 2020 2020 2020 2020 2020  o=(.            
-00007c80: 2020 2020 6461 7465 7469 6d65 2e64 6174      datetime.dat
-00007c90: 6574 696d 652e 6e6f 7728 292b 6461 7465  etime.now()+date
-00007ca0: 7469 6d65 2e74 696d 6564 656c 7461 2833  time.timedelta(3
-00007cb0: 3029 0a20 2020 2020 2020 2020 2020 2029  0).            )
-00007cc0: 2e73 7472 6674 696d 6528 2225 642f 256d  .strftime("%d/%m
-00007cd0: 2f25 5922 292c 0a20 2020 2020 2020 2020  /%Y"),.         
-00007ce0: 2020 2067 7469 6e3d 2247 5449 4e31 222c     gtin="GTIN1",
-00007cf0: 206c 6f74 653d 6461 7465 7469 6d65 2e64   lote=datetime.d
-00007d00: 6174 6574 696d 652e 6e6f 7728 292e 7374  atetime.now().st
-00007d10: 7266 7469 6d65 2822 2559 2229 2c0a 2020  rftime("%Y"),.  
-00007d20: 2020 2020 2020 2020 2020 6465 7364 655f            desde_
-00007d30: 6e75 6d65 726f 5f73 6572 6961 6c3d 696e  numero_serial=in
-00007d40: 7428 7469 6d65 2e74 696d 6528 292a 3130  t(time.time()*10
-00007d50: 292d 312c 0a20 2020 2020 2020 2020 2020  )-1,.           
-00007d60: 2068 6173 7461 5f6e 756d 6572 6f5f 7365   hasta_numero_se
-00007d70: 7269 616c 3d69 6e74 2874 696d 652e 7469  rial=int(time.ti
-00007d80: 6d65 2829 2a31 3029 2b31 2c0a 2020 2020  me()*10)+1,.    
-00007d90: 2020 2020 2020 2020 6964 5f6f 6272 615f          id_obra_
-00007da0: 736f 6369 616c 3d4e 6f6e 652c 2069 645f  social=None, id_
-00007db0: 6576 656e 746f 3d31 3334 2c0a 2020 2020  evento=134,.    
-00007dc0: 2020 2020 2020 2020 6e72 6f5f 6173 6f63          nro_asoc
-00007dd0: 6961 646f 3d22 3132 3334 222c 0a20 2020  iado="1234",.   
-00007de0: 2020 2020 2020 2020 2063 616e 7469 6461           cantida
-00007df0: 643d 4e6f 6e65 2c20 6e75 6d65 726f 5f73  d=None, numero_s
-00007e00: 6572 6961 6c3d 4e6f 6e65 2c0a 2020 2020  erial=None,.    
-00007e10: 2020 2020 2020 2020 636f 6469 676f 5f74          codigo_t
-00007e20: 7261 6e73 6163 6369 6f6e 3d4e 6f6e 652c  ransaccion=None,
-00007e30: 0a20 2020 2020 2020 2029 290a 0a20 2020  .        ))..   
-00007e40: 2023 204f 7063 696f 6e65 7320 7072 696e   # Opciones prin
-00007e50: 6369 7061 6c65 733a 0a0a 2020 2020 6966  cipales:..    if
-00007e60: 2027 2d2d 6361 6e63 656c 6127 2069 6e20   '--cancela' in 
-00007e70: 7379 732e 6172 6776 3a0a 2020 2020 2020  sys.argv:.      
-00007e80: 2020 6966 2027 2d2d 6c6f 6164 786d 6c27    if '--loadxml'
-00007e90: 2069 6e20 7379 732e 6172 6776 3a0a 2020   in sys.argv:.  
-00007ea0: 2020 2020 2020 2020 2020 7773 2e4c 6f61            ws.Loa
-00007eb0: 6454 6573 7458 4d4c 2822 7472 617a 616d  dTestXML("trazam
-00007ec0: 6564 5f63 616e 6365 6c61 5f65 7272 2e78  ed_cancela_err.x
-00007ed0: 6d6c 2229 2020 2320 6361 7267 6f20 7265  ml")  # cargo re
-00007ee0: 7370 7565 7374 610a 2020 2020 2020 2020  spuesta.        
-00007ef0: 7773 2e53 656e 6443 616e 6365 6c61 6354  ws.SendCancelacT
-00007f00: 7261 6e73 6163 6328 2a73 7973 2e61 7267  ransacc(*sys.arg
-00007f10: 765b 7379 732e 6172 6776 2e69 6e64 6578  v[sys.argv.index
-00007f20: 2822 2d2d 6361 6e63 656c 6122 292b 313a  ("--cancela")+1:
-00007f30: 5d29 0a20 2020 2065 6c69 6620 272d 2d63  ]).    elif '--c
-00007f40: 616e 6365 6c61 5f70 6172 6369 616c 2720  ancela_parcial' 
-00007f50: 696e 2073 7973 2e61 7267 763a 0a20 2020  in sys.argv:.   
-00007f60: 2020 2020 2077 732e 5365 6e64 4361 6e63       ws.SendCanc
-00007f70: 656c 6163 5472 616e 7361 6363 5061 7263  elacTransaccParc
-00007f80: 6961 6c28 0a20 2020 2020 2020 2020 2020  ial(.           
-00007f90: 202a 7379 732e 6172 6776 5b73 7973 2e61   *sys.argv[sys.a
-00007fa0: 7267 762e 696e 6465 7828 222d 2d63 616e  rgv.index("--can
-00007fb0: 6365 6c61 5f70 6172 6369 616c 2229 2b31  cela_parcial")+1
-00007fc0: 3a5d 290a 2020 2020 656c 6966 2027 2d2d  :]).    elif '--
-00007fd0: 636f 6e66 6972 6d61 2720 696e 2073 7973  confirma' in sys
-00007fe0: 2e61 7267 763a 0a20 2020 2020 2020 2069  .argv:.        i
-00007ff0: 6620 272d 2d6c 6f61 6478 6d6c 2720 696e  f '--loadxml' in
-00008000: 2073 7973 2e61 7267 763a 0a20 2020 2020   sys.argv:.     
-00008010: 2020 2020 2020 2077 732e 4c6f 6164 5465         ws.LoadTe
-00008020: 7374 584d 4c28 2274 7261 7a61 6d65 645f  stXML("trazamed_
-00008030: 636f 6e66 6972 6d61 2e78 6d6c 2229 2020  confirma.xml")  
-00008040: 2320 6361 7267 6f20 7265 7370 7565 7374  # cargo respuest
-00008050: 610a 2020 2020 2020 2020 2020 2020 6f6b  a.            ok
-00008060: 203d 2077 732e 5365 6e64 436f 6e66 6972   = ws.SendConfir
-00008070: 6d61 5472 616e 7361 6363 280a 2020 2020  maTransacc(.    
-00008080: 2020 2020 2020 2020 2020 2020 7573 7561              usua
-00008090: 7269 6f3d 2270 7275 6562 6173 7773 222c  rio="pruebasws",
-000080a0: 2070 6173 7377 6f72 643d 2270 7275 6562   password="prueb
-000080b0: 6173 7773 222c 0a20 2020 2020 2020 2020  asws",.         
-000080c0: 2020 2020 2020 2070 5f69 6473 5f74 7261         p_ids_tra
-000080d0: 6e73 6163 3d22 3122 2c20 665f 6f70 6572  nsac="1", f_oper
-000080e0: 6163 696f 6e3d 2233 312d 3132 2d32 3031  acion="31-12-201
-000080f0: 3322 290a 2020 2020 2020 2020 2020 2020  3").            
-00008100: 6966 206e 6f74 206f 6b3a 0a20 2020 2020  if not ok:.     
-00008110: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00008120: 2052 756e 7469 6d65 4572 726f 7228 7773   RuntimeError(ws
-00008130: 2e45 7863 6570 6369 6f6e 290a 2020 2020  .Excepcion).    
-00008140: 2020 2020 7773 2e53 656e 6443 6f6e 6669      ws.SendConfi
-00008150: 726d 6154 7261 6e73 6163 6328 2a73 7973  rmaTransacc(*sys
-00008160: 2e61 7267 765b 7379 732e 6172 6776 2e69  .argv[sys.argv.i
-00008170: 6e64 6578 2822 2d2d 636f 6e66 6972 6d61  ndex("--confirma
-00008180: 2229 2b31 3a5d 290a 2020 2020 656c 6966  ")+1:]).    elif
-00008190: 2027 2d2d 616c 6572 7461 2720 696e 2073   '--alerta' in s
-000081a0: 7973 2e61 7267 763a 0a20 2020 2020 2020  ys.argv:.       
-000081b0: 2077 732e 5365 6e64 416c 6572 7461 5472   ws.SendAlertaTr
-000081c0: 616e 7361 6363 282a 7379 732e 6172 6776  ansacc(*sys.argv
-000081d0: 5b73 7973 2e61 7267 762e 696e 6465 7828  [sys.argv.index(
-000081e0: 222d 2d61 6c65 7274 6122 292b 313a 5d29  "--alerta")+1:])
-000081f0: 0a20 2020 2065 6c69 6620 272d 2d63 6f6e  .    elif '--con
-00008200: 7375 6c74 6127 2069 6e20 7379 732e 6172  sulta' in sys.ar
-00008210: 6776 3a0a 2020 2020 2020 2020 6966 2027  gv:.        if '
-00008220: 2d2d 616c 6572 7461 646f 7327 2069 6e20  --alertados' in 
-00008230: 7379 732e 6172 6776 3a0a 2020 2020 2020  sys.argv:.      
-00008240: 2020 2020 2020 7773 2e47 6574 456e 7669        ws.GetEnvi
-00008250: 6f73 5072 6f70 696f 7341 6c65 7274 6164  osPropiosAlertad
-00008260: 6f73 280a 2020 2020 2020 2020 2020 2020  os(.            
-00008270: 2020 2020 2a73 7973 2e61 7267 765b 7379      *sys.argv[sy
-00008280: 732e 6172 6776 2e69 6e64 6578 2822 2d2d  s.argv.index("--
-00008290: 616c 6572 7461 646f 7322 292b 313a 5d0a  alertados")+1:].
-000082a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000082b0: 2020 2020 2020 656c 6966 2027 2d2d 6d6f        elif '--mo
-000082c0: 7669 6d69 656e 746f 7327 2069 6e20 7379  vimientos' in sy
-000082d0: 732e 6172 6776 3a0a 2020 2020 2020 2020  s.argv:.        
-000082e0: 2020 2020 7773 2e47 6574 5472 616e 7361      ws.GetTransa
-000082f0: 6363 696f 6e65 7357 5328 0a20 2020 2020  ccionesWS(.     
-00008300: 2020 2020 2020 2020 2020 202a 7379 732e             *sys.
-00008310: 6172 6776 5b73 7973 2e61 7267 762e 696e  argv[sys.argv.in
-00008320: 6465 7828 222d 2d6d 6f76 696d 6965 6e74  dex("--movimient
-00008330: 6f73 2229 2b31 3a5d 0a20 2020 2020 2020  os")+1:].       
-00008340: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
-00008350: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00008360: 2077 732e 4765 7454 7261 6e73 6163 6369   ws.GetTransacci
-00008370: 6f6e 6573 4e6f 436f 6e66 6972 6d61 6461  onesNoConfirmada
-00008380: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-00008390: 2020 202a 7379 732e 6172 6776 5b73 7973     *sys.argv[sys
-000083a0: 2e61 7267 762e 696e 6465 7828 222d 2d63  .argv.index("--c
-000083b0: 6f6e 7375 6c74 6122 292b 313a 5d0a 2020  onsulta")+1:].  
-000083c0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000083d0: 7573 7561 7269 6f3d 2270 7275 6562 6173  usuario="pruebas
-000083e0: 7773 222c 2070 6173 7377 6f72 643d 2270  ws", password="p
-000083f0: 7275 6562 6173 7773 222c 0a20 2020 2020  ruebasws",.     
-00008400: 2020 2020 2020 2020 2020 2023 2070 5f69             # p_i
-00008410: 645f 7472 616e 7361 6363 696f 6e5f 676c  d_transaccion_gl
-00008420: 6f62 616c 3d22 3132 3334 222c 0a20 2020  obal="1234",.   
-00008430: 2020 2020 2020 2020 2020 2020 2023 2069               # i
-00008440: 645f 6167 656e 7465 5f69 6e66 6f72 6d61  d_agente_informa
-00008450: 646f 723d 2231 222c 0a20 2020 2020 2020  dor="1",.       
-00008460: 2020 2020 2020 2020 2023 2069 645f 6167           # id_ag
-00008470: 656e 7465 5f6f 7269 6765 6e3d 2231 222c  ente_origen="1",
-00008480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008490: 2023 2069 645f 6167 656e 7465 5f64 6573   # id_agente_des
-000084a0: 7469 6e6f 3d22 3122 2c0a 2020 2020 2020  tino="1",.      
-000084b0: 2020 2020 2020 2020 2020 2320 6964 5f6d            # id_m
-000084c0: 6564 6963 616d 656e 746f 3d22 3122 2c0a  edicamento="1",.
-000084d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084e0: 2320 6964 5f65 7665 6e74 6f3d 2231 222c  # id_evento="1",
-000084f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008500: 2023 2066 6563 6861 5f64 6573 6465 5f6f   # fecha_desde_o
-00008510: 703d 2230 312f 3031 2f32 3031 3522 2c0a  p="01/01/2015",.
-00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008530: 2320 6665 6368 615f 6861 7374 615f 6f70  # fecha_hasta_op
-00008540: 3d22 3331 2f31 322f 3230 3133 222c 0a20  ="31/12/2013",. 
-00008550: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00008560: 2066 6563 6861 5f64 6573 6465 5f74 3d22   fecha_desde_t="
-00008570: 3031 2f30 312f 3230 3133 222c 0a20 2020  01/01/2013",.   
-00008580: 2020 2020 2020 2020 2020 2020 2023 2066               # f
-00008590: 6563 6861 5f68 6173 7461 5f74 3d22 3331  echa_hasta_t="31
-000085a0: 2f31 322f 3230 3133 222c 0a20 2020 2020  /12/2013",.     
-000085b0: 2020 2020 2020 2020 2020 2023 2066 6563             # fec
-000085c0: 6861 5f64 6573 6465 5f76 3d22 3031 2f30  ha_desde_v="01/0
-000085d0: 342f 3230 3133 222c 0a20 2020 2020 2020  4/2013",.       
-000085e0: 2020 2020 2020 2020 2023 2066 6563 6861           # fecha
-000085f0: 5f68 6173 7461 5f76 3d22 3330 2f30 342f  _hasta_v="30/04/
-00008600: 3230 3133 222c 0a20 2020 2020 2020 2020  2013",.         
-00008610: 2020 2020 2020 2023 206e 5f66 6163 7475         # n_factu
-00008620: 7261 3d35 2c20 6e5f 7265 6d69 746f 3d36  ra=5, n_remito=6
-00008630: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008640: 2020 2320 6573 7461 646f 3d31 2c0a 2020    # estado=1,.  
-00008650: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00008660: 6c6f 7465 3d38 3837 3435 2c0a 2020 2020  lote=88745,.    
-00008670: 2020 2020 2020 2020 2020 2020 2320 6e75              # nu
-00008680: 6d65 726f 5f73 6572 6961 6c3d 3839 3431  mero_serial=8941
-00008690: 3234 3738 382c 0a20 2020 2020 2020 2020  24788,.         
-000086a0: 2020 2029 0a20 2020 2020 2020 2070 7269     ).        pri
-000086b0: 6e74 2822 4361 6e74 5061 6769 6e61 7322  nt("CantPaginas"
-000086c0: 2c20 7773 2e43 616e 7450 6167 696e 6173  , ws.CantPaginas
-000086d0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-000086e0: 2248 6179 4572 726f 7222 2c20 7773 2e48  "HayError", ws.H
-000086f0: 6179 4572 726f 7229 0a20 2020 2020 2020  ayError).       
-00008700: 2023 2070 7269 6e74 2822 5472 616e 7361   # print("Transa
-00008710: 6363 696f 6e50 6c61 696e 5753 222c 2077  ccionPlainWS", w
-00008720: 732e 5472 616e 7361 6363 696f 6e50 6c61  s.TransaccionPla
-00008730: 696e 5753 290a 2020 2020 2020 2020 2320  inWS).        # 
-00008740: 7061 7261 6d65 7472 6f73 2063 6f6d 756e  parametros comun
-00008750: 6573 2064 6520 7361 6c69 6461 2028 636f  es de salida (co
-00008760: 6c75 6d6e 6173 2064 6520 6c61 2074 6162  lumnas de la tab
-00008770: 6c61 293a 0a20 2020 2020 2020 2063 6c61  la):.        cla
-00008780: 7665 7320 3d20 5b6b 2066 6f72 206b 2c20  ves = [k for k, 
-00008790: 762c 206c 2069 6e20 5452 414e 5341 4343  v, l in TRANSACC
-000087a0: 494f 4e45 535d 0a20 2020 2020 2020 2023  IONES].        #
-000087b0: 2065 7874 6965 6e64 6f20 6c61 206c 6973   extiendo la lis
-000087c0: 7461 2064 6520 7265 7375 6c74 6164 6f20  ta de resultado 
-000087d0: 7061 7261 2065 6c20 6172 6368 6976 6f20  para el archivo 
-000087e0: 6465 2069 6e74 6572 6361 6d62 696f 3a0a  de intercambio:.
-000087f0: 2020 2020 2020 2020 7472 616e 7361 6363          transacc
-00008800: 696f 6e65 732e 6578 7465 6e64 2877 732e  iones.extend(ws.
-00008810: 5472 616e 7361 6363 696f 6e50 6c61 696e  TransaccionPlain
-00008820: 5753 290a 2020 2020 2020 2020 2320 656e  WS).        # en
-00008830: 6361 6265 7a61 646f 2064 6520 6c61 2074  cabezado de la t
-00008840: 6162 6c61 3a0a 2020 2020 2020 2020 7072  abla:.        pr
-00008850: 696e 7428 227c 7c22 2c20 227c 7c22 2e6a  int("||", "||".j
-00008860: 6f69 6e28 5b22 2573 2220 2520 636c 6176  oin(["%s" % clav
-00008870: 6520 666f 7220 636c 6176 6520 696e 2063  e for clave in c
-00008880: 6c61 7665 735d 292c 2022 7c7c 2229 0a20  laves]), "||"). 
-00008890: 2020 2020 2020 2023 2072 6563 6f72 726f         # recorro
-000088a0: 206c 6f73 2064 6174 6f73 2064 6576 7565   los datos devue
-000088b0: 6c74 6f73 2028 5472 616e 7361 6363 696f  ltos (Transaccio
-000088c0: 6e50 6c61 696e 5753 293a 0a20 2020 2020  nPlainWS):.     
-000088d0: 2020 2077 6869 6c65 2077 732e 4c65 6572     while ws.Leer
-000088e0: 5472 616e 7361 6363 696f 6e28 293a 0a20  Transaccion():. 
-000088f0: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-00008900: 6c61 7665 2069 6e20 636c 6176 6573 3a0a  lave in claves:.
-00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008920: 7072 696e 7428 227c 7c22 2c20 7773 2e47  print("||", ws.G
-00008930: 6574 5061 7261 6d65 7472 6f28 636c 6176  etParametro(clav
-00008940: 6529 2920 2020 2020 2020 2020 2320 696d  e))         # im
-00008950: 7072 696d 6f20 6361 6461 2066 696c 610a  primo cada fila.
-00008960: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00008970: 7428 227c 7c22 290a 2020 2020 656c 6966  t("||").    elif
-00008980: 2027 2d2d 6361 7461 6c6f 676f 2720 696e   '--catalogo' in
-00008990: 2073 7973 2e61 7267 763a 0a20 2020 2020   sys.argv:.     
-000089a0: 2020 2072 6574 203d 2077 732e 4765 7443     ret = ws.GetC
-000089b0: 6174 616c 6f67 6f45 6c65 6374 726f 6e69  atalogoElectroni
-000089c0: 636f 4279 4754 494e 280a 2020 2020 2020  coByGTIN(.      
-000089d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089e0: 2020 2020 2020 2020 2020 2a73 7973 2e61            *sys.a
-000089f0: 7267 765b 7379 732e 6172 6776 2e69 6e64  rgv[sys.argv.ind
-00008a00: 6578 2822 2d2d 6361 7461 6c6f 676f 2229  ex("--catalogo")
-00008a10: 2b31 3a5d 0a20 2020 2020 2020 2020 2020  +1:].           
-00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a30: 2020 2020 2029 0a20 2020 2020 2020 2066       ).        f
-00008a40: 6f72 2063 6174 616c 6f67 6f20 696e 2077  or catalogo in w
-00008a50: 732e 7061 7261 6d73 5f6f 7574 2e76 616c  s.params_out.val
-00008a60: 7565 7328 293a 0a20 2020 2020 2020 2020  ues():.         
-00008a70: 2020 2070 7269 6e74 2863 6174 616c 6f67     print(catalog
-00008a80: 6f29 2020 2020 2020 2020 2320 696d 7072  o)        # impr
-00008a90: 696d 6f20 6361 6461 2066 696c 6129 0a20  imo cada fila). 
-00008aa0: 2020 2065 6c69 6620 272d 2d73 746f 636b     elif '--stock
-00008ab0: 2720 696e 2073 7973 2e61 7267 763a 0a20  ' in sys.argv:. 
-00008ac0: 2020 2020 2020 2072 6574 203d 2077 732e         ret = ws.
-00008ad0: 4765 7443 6f6e 7375 6c74 6153 746f 636b  GetConsultaStock
-00008ae0: 280a 2020 2020 2020 2020 2020 2020 2a73  (.            *s
-00008af0: 7973 2e61 7267 765b 7379 732e 6172 6776  ys.argv[sys.argv
-00008b00: 2e69 6e64 6578 2822 2d2d 7374 6f63 6b22  .index("--stock"
-00008b10: 292b 313a 5d0a 2020 2020 2020 2020 290a  )+1:].        ).
-00008b20: 2020 2020 2020 2020 7072 696e 7428 7265          print(re
-00008b30: 7429 0a20 2020 2020 2020 2070 7269 6e74  t).        print
-00008b40: 2822 5c6e 222e 6a6f 696e 285b 7374 7228  ("\n".join([str(
-00008b50: 7329 2066 6f72 2073 2069 6e20 7773 2e70  s) for s in ws.p
-00008b60: 6172 616d 735f 6f75 742e 7661 6c75 6573  arams_out.values
-00008b70: 2829 5d29 290a 2020 2020 656c 7365 3a0a  ()])).    else:.
-00008b80: 2020 2020 2020 2020 6172 6776 203d 205b          argv = [
-00008b90: 6172 6776 2066 6f72 2061 7267 7620 696e  argv for argv in
-00008ba0: 2073 7973 2e61 7267 7620 6966 206e 6f74   sys.argv if not
-00008bb0: 2061 7267 762e 7374 6172 7473 7769 7468   argv.startswith
-00008bc0: 2822 2d2d 2229 5d0a 2020 2020 2020 2020  ("--")].        
-00008bd0: 6966 206e 6f74 206d 6564 6963 616d 656e  if not medicamen
-00008be0: 746f 733a 0a20 2020 2020 2020 2020 2020  tos:.           
-00008bf0: 2069 6620 6c65 6e28 6172 6776 2920 3e20   if len(argv) > 
-00008c00: 3136 3a0a 2020 2020 2020 2020 2020 2020  16:.            
-00008c10: 2020 2020 6966 2027 2d2d 6468 2720 696e      if '--dh' in
-00008c20: 2073 7973 2e61 7267 763a 0a20 2020 2020   sys.argv:.     
-00008c30: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00008c40: 732e 5365 6e64 4d65 6469 6361 6d65 6e74  s.SendMedicament
-00008c50: 6f73 4448 5365 7269 6528 2a61 7267 765b  osDHSerie(*argv[
-00008c60: 313a 5d29 0a20 2020 2020 2020 2020 2020  1:]).           
-00008c70: 2020 2020 2065 6c69 6620 272d 2d66 7261       elif '--fra
-00008c80: 6363 696f 6e27 2069 6e20 7379 732e 6172  ccion' in sys.ar
-00008c90: 6776 3a0a 2020 2020 2020 2020 2020 2020  gv:.            
-00008ca0: 2020 2020 2020 2020 7773 2e53 656e 644d          ws.SendM
-00008cb0: 6564 6963 616d 656e 746f 7346 7261 6363  edicamentosFracc
-00008cc0: 696f 6e28 2a61 7267 765b 313a 5d29 0a20  ion(*argv[1:]). 
-00008cd0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00008ce0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00008cf0: 2020 2020 2020 2020 2077 732e 5365 6e64           ws.Send
-00008d00: 4d65 6469 6361 6d65 6e74 6f73 282a 6172  Medicamentos(*ar
-00008d10: 6776 5b31 3a5d 290a 2020 2020 2020 2020  gv[1:]).        
-00008d20: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00008d30: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00008d40: 2245 5252 4f52 3a20 6e6f 2073 6520 696e  "ERROR: no se in
-00008d50: 6469 6361 726f 6e20 746f 646f 7320 6c6f  dicaron todos lo
-00008d60: 7320 7061 72e1 6d65 7472 6f73 2072 6571  s par.metros req
-00008d70: 7565 7269 646f 7322 290a 2020 2020 2020  ueridos").      
-00008d80: 2020 656c 6966 206d 6564 6963 616d 656e    elif medicamen
-00008d90: 746f 733a 0a20 2020 2020 2020 2020 2020  tos:.           
-00008da0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00008db0: 2020 2020 2020 7573 7561 7269 6f2c 2070        usuario, p
-00008dc0: 6173 7377 6f72 6420 3d20 6172 6776 5b31  assword = argv[1
-00008dd0: 3a33 5d0a 2020 2020 2020 2020 2020 2020  :3].            
-00008de0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00008df0: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
-00008e00: 2020 2020 2020 2070 7269 6e74 280a 2020         print(.  
-00008e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e20: 2020 2241 4456 4552 5445 4e43 4941 3a20    "ADVERTENCIA: 
-00008e30: 6e6f 2073 6520 696e 6469 636f 2070 6172  no se indico par
-00008e40: e16d 6574 726f 7320 7573 7561 7269 6f20  .metros usuario 
-00008e50: 7920 7061 7373 6f77 6f72 6422 0a20 2020  y passoword".   
-00008e60: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00008e70: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00008e80: 7269 6e74 2865 290a 2020 2020 2020 2020  rint(e).        
-00008e90: 2020 2020 2020 2020 7573 7561 7269 6f20          usuario 
-00008ea0: 3d20 7061 7373 776f 7264 203d 2022 7072  = password = "pr
-00008eb0: 7565 6261 7377 7322 0a20 2020 2020 2020  uebasws".       
-00008ec0: 2020 2020 2066 6f72 2069 2c20 6d65 6420       for i, med 
-00008ed0: 696e 2065 6e75 6d65 7261 7465 286d 6564  in enumerate(med
-00008ee0: 6963 616d 656e 746f 7329 3a0a 2020 2020  icamentos):.    
-00008ef0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00008f00: 7428 2250 726f 6365 7361 6e64 6f20 7265  t("Procesando re
-00008f10: 6769 7374 726f 222c 2069 290a 2020 2020  gistro", i).    
-00008f20: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
-00008f30: 6d65 645b 2763 6f64 6967 6f5f 7472 616e  med['codigo_tran
-00008f40: 7361 6363 696f 6e27 5d0a 2020 2020 2020  saccion'].      
-00008f50: 2020 2020 2020 2020 2020 6966 206d 6564            if med
-00008f60: 2e67 6574 2822 6361 6e74 6964 6164 2229  .get("cantidad")
-00008f70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008f80: 2020 2020 2020 6465 6c20 6d65 645b 2264        del med["d
-00008f90: 6573 6465 5f6e 756d 6572 6f5f 7365 7269  esde_numero_seri
-00008fa0: 616c 225d 0a20 2020 2020 2020 2020 2020  al"].           
-00008fb0: 2020 2020 2020 2020 2064 656c 206d 6564           del med
-00008fc0: 5b22 6861 7374 615f 6e75 6d65 726f 5f73  ["hasta_numero_s
-00008fd0: 6572 6961 6c22 5d0a 2020 2020 2020 2020  erial"].        
-00008fe0: 2020 2020 2020 2020 2020 2020 7773 2e53              ws.S
-00008ff0: 656e 644d 6564 6963 616d 656e 746f 7346  endMedicamentosF
-00009000: 7261 6363 696f 6e28 7573 7561 7269 6f2c  raccion(usuario,
-00009010: 2070 6173 7377 6f72 642c 202a 2a6d 6564   password, **med
-00009020: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009030: 2020 656c 6966 206d 6564 2e67 6574 2822    elif med.get("
-00009040: 6465 7364 655f 6e75 6d65 726f 5f73 6572  desde_numero_ser
-00009050: 6961 6c22 293a 0a20 2020 2020 2020 2020  ial"):.         
-00009060: 2020 2020 2020 2020 2020 2064 656c 206d             del m
-00009070: 6564 5b22 6361 6e74 6964 6164 225d 0a20  ed["cantidad"]. 
-00009080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009090: 2020 2064 656c 206d 6564 5b22 6e75 6d65     del med["nume
-000090a0: 726f 5f73 6572 6961 6c22 5d0a 2020 2020  ro_serial"].    
-000090b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090c0: 7773 2e53 656e 644d 6564 6963 616d 656e  ws.SendMedicamen
-000090d0: 746f 7344 4853 6572 6965 2875 7375 6172  tosDHSerie(usuar
-000090e0: 696f 2c20 7061 7373 776f 7264 2c20 2a2a  io, password, **
-000090f0: 6d65 6429 0a20 2020 2020 2020 2020 2020  med).           
-00009100: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00009110: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00009120: 656c 206d 6564 5b22 6361 6e74 6964 6164  el med["cantidad
-00009130: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-00009140: 2020 2020 2020 2064 656c 206d 6564 5b22         del med["
-00009150: 6465 7364 655f 6e75 6d65 726f 5f73 6572  desde_numero_ser
-00009160: 6961 6c22 5d0a 2020 2020 2020 2020 2020  ial"].          
-00009170: 2020 2020 2020 2020 2020 6465 6c20 6d65            del me
-00009180: 645b 2268 6173 7461 5f6e 756d 6572 6f5f  d["hasta_numero_
-00009190: 7365 7269 616c 225d 0a20 2020 2020 2020  serial"].       
-000091a0: 2020 2020 2020 2020 2020 2020 2077 732e               ws.
-000091b0: 5365 6e64 4d65 6469 6361 6d65 6e74 6f73  SendMedicamentos
-000091c0: 2875 7375 6172 696f 2c20 7061 7373 776f  (usuario, passwo
-000091d0: 7264 2c20 2a2a 6d65 6429 0a20 2020 2020  rd, **med).     
-000091e0: 2020 2020 2020 2020 2020 206d 6564 5b27             med['
-000091f0: 636f 6469 676f 5f74 7261 6e73 6163 6369  codigo_transacci
-00009200: 6f6e 275d 203d 2077 732e 436f 6469 676f  on'] = ws.Codigo
-00009210: 5472 616e 7361 6363 696f 6e0a 2020 2020  Transaccion.    
-00009220: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-00009230: 7265 732e 6578 7465 6e64 2877 732e 6572  res.extend(ws.er
-00009240: 726f 7265 7329 0a20 2020 2020 2020 2020  rores).         
-00009250: 2020 2020 2020 2070 7269 6e74 2822 7c52         print("|R
-00009260: 6573 756c 7461 646f 2025 3573 7c43 6f64  esultado %5s|Cod
-00009270: 6967 6f54 7261 6e73 6163 6369 6f6e 2025  igoTransaccion %
-00009280: 3130 737c 4572 726f 7265 737c 2573 7c22  10s|Errores|%s|"
-00009290: 2025 2028 0a20 2020 2020 2020 2020 2020   % (.           
-000092a0: 2020 2020 2020 2020 2077 732e 5265 7375           ws.Resu
-000092b0: 6c74 6164 6f2c 0a20 2020 2020 2020 2020  ltado,.         
-000092c0: 2020 2020 2020 2020 2020 2077 732e 436f             ws.Co
-000092d0: 6469 676f 5472 616e 7361 6363 696f 6e2c  digoTransaccion,
-000092e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000092f0: 2020 2020 2027 7c27 2e6a 6f69 6e28 7773       '|'.join(ws
-00009300: 2e45 7272 6f72 6573 206f 7220 5b5d 292c  .Errores or []),
-00009310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009320: 2029 290a 2020 2020 2020 2020 656c 7365   )).        else
-00009330: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00009340: 696e 7428 2245 5252 4f52 3a20 6e6f 2073  int("ERROR: no s
-00009350: 6520 6573 7065 6369 6669 6361 726f 6e20  e especificaron 
-00009360: 6d65 6469 6361 6d65 6e74 6f73 2061 2069  medicamentos a i
-00009370: 6e66 6f72 6d61 7222 290a 0a20 2020 2069  nformar")..    i
-00009380: 6620 6e6f 7420 6d65 6469 6361 6d65 6e74  f not medicament
-00009390: 6f73 3a0a 2020 2020 2020 2020 7072 696e  os:.        prin
-000093a0: 7428 227c 5265 7375 6c74 6164 6f20 2535  t("|Resultado %5
-000093b0: 737c 436f 6469 676f 5472 616e 7361 6363  s|CodigoTransacc
-000093c0: 696f 6e20 2531 3073 7c45 7272 6f72 6573  ion %10s|Errores
-000093d0: 7c25 737c 2220 2520 280a 2020 2020 2020  |%s|" % (.      
-000093e0: 2020 2020 2020 7773 2e52 6573 756c 7461        ws.Resulta
-000093f0: 646f 2c0a 2020 2020 2020 2020 2020 2020  do,.            
-00009400: 7773 2e43 6f64 6967 6f54 7261 6e73 6163  ws.CodigoTransac
-00009410: 6369 6f6e 2c0a 2020 2020 2020 2020 2020  cion,.          
-00009420: 2020 277c 272e 6a6f 696e 2877 732e 4572    '|'.join(ws.Er
-00009430: 726f 7265 7320 6f72 205b 5d29 2c0a 2020  rores or []),.  
-00009440: 2020 2020 2020 2929 0a0a 2020 2020 6966        ))..    if
-00009450: 2077 732e 4578 6365 7063 696f 6e3a 0a20   ws.Excepcion:. 
-00009460: 2020 2020 2020 2070 7269 6e74 2877 732e         print(ws.
-00009470: 5472 6163 6562 6163 6b29 0a0a 2020 2020  Traceback)..    
-00009480: 6966 2027 2d2d 6772 6162 6172 2720 696e  if '--grabar' in
-00009490: 2073 7973 2e61 7267 763a 0a20 2020 2020   sys.argv:.     
-000094a0: 2020 2069 6620 272d 2d64 6266 2720 696e     if '--dbf' in
-000094b0: 2073 7973 2e61 7267 763a 0a20 2020 2020   sys.argv:.     
-000094c0: 2020 2020 2020 2067 7561 7264 6172 5f64         guardar_d
-000094d0: 6266 2866 6f72 6d61 746f 732c 2054 7275  bf(formatos, Tru
-000094e0: 652c 207b 7d29 0a20 2020 2020 2020 2065  e, {}).        e
-000094f0: 6c69 6620 272d 2d6a 736f 6e27 2069 6e20  lif '--json' in 
-00009500: 7379 732e 6172 6776 3a0a 2020 2020 2020  sys.argv:.      
-00009510: 2020 2020 2020 666f 7220 666f 726d 6174        for format
-00009520: 6f20 696e 2066 6f72 6d61 746f 733a 0a20  o in formatos:. 
-00009530: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00009540: 7263 6869 766f 203d 206f 7065 6e28 666f  rchivo = open(fo
-00009550: 726d 6174 6f5b 305d 2e6c 6f77 6572 2829  rmato[0].lower()
-00009560: 202b 2022 2e6a 736f 6e22 2c20 2277 2229   + ".json", "w")
-00009570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009580: 206a 736f 6e2e 6475 6d70 2866 6f72 6d61   json.dump(forma
-00009590: 746f 5b32 5d2c 2061 7263 6869 766f 2c20  to[2], archivo, 
-000095a0: 736f 7274 5f6b 6579 733d 5472 7565 2c20  sort_keys=True, 
-000095b0: 696e 6465 6e74 3d34 290a 2020 2020 2020  indent=4).      
-000095c0: 2020 2020 2020 2020 2020 6172 6368 6976            archiv
-000095d0: 6f2e 636c 6f73 6528 290a 2020 2020 2020  o.close().      
-000095e0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000095f0: 2020 2020 666f 7220 666f 726d 6174 6f20      for formato 
-00009600: 696e 2066 6f72 6d61 746f 733a 0a20 2020  in formatos:.   
-00009610: 2020 2020 2020 2020 2020 2020 2061 7263               arc
-00009620: 6869 766f 203d 206f 7065 6e28 666f 726d  hivo = open(form
-00009630: 6174 6f5b 305d 2e6c 6f77 6572 2829 202b  ato[0].lower() +
-00009640: 2022 2e74 7874 222c 2022 7722 290a 2020   ".txt", "w").  
-00009650: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00009660: 7220 6974 2069 6e20 666f 726d 6174 6f5b  r it in formato[
-00009670: 325d 3a0a 2020 2020 2020 2020 2020 2020  2]:.            
-00009680: 2020 2020 2020 2020 6172 6368 6976 6f2e          archivo.
-00009690: 7772 6974 6528 6573 6372 6962 6972 2869  write(escribir(i
-000096a0: 742c 2066 6f72 6d61 746f 5b31 5d29 290a  t, formato[1])).
-000096b0: 2020 2020 2020 2020 2020 2020 6172 6368              arch
-000096c0: 6976 6f2e 636c 6f73 6528 290a 0a0a 2320  ivo.close()...# 
-000096d0: 6275 7363 6f20 656c 2064 6972 6563 746f  busco el directo
-000096e0: 7269 6f20 6465 2069 6e73 7461 6c61 6369  rio de instalaci
-000096f0: f36e 2028 676c 6f62 616c 2070 6172 6120  .n (global para 
-00009700: 7175 6520 6e6f 2063 616d 6269 6520 7369  que no cambie si
-00009710: 0a23 2075 7361 6e20 6f74 7261 2064 6c6c  .# usan otra dll
-00009720: 290a 494e 5354 414c 4c5f 4449 5220 3d20  ).INSTALL_DIR = 
-00009730: 5472 617a 614d 6564 2e49 6e73 7461 6c6c  TrazaMed.Install
-00009740: 4469 7220 3d20 6765 745f 696e 7374 616c  Dir = get_instal
-00009750: 6c5f 6469 7228 290a 0a0a 6966 205f 5f6e  l_dir()...if __n
-00009760: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
-00009770: 5f5f 273a 0a0a 2020 2020 2320 616a 7573  __':..    # ajus
-00009780: 746f 2065 6c20 656e 636f 6469 6e67 2070  to el encoding p
-00009790: 6f72 2064 6566 6563 746f 2028 7369 2073  or defecto (si s
-000097a0: 6520 7265 6469 7269 6a65 206c 6120 7361  e redirije la sa
-000097b0: 6c69 6461 290a 2020 2020 6966 206e 6f74  lida).    if not
-000097c0: 2068 6173 6174 7472 2873 7973 2e73 7464   hasattr(sys.std
-000097d0: 6f75 742c 2022 656e 636f 6469 6e67 2229  out, "encoding")
-000097e0: 206f 7220 7379 732e 7374 646f 7574 2e65   or sys.stdout.e
-000097f0: 6e63 6f64 696e 6720 6973 204e 6f6e 653a  ncoding is None:
-00009800: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00009810: 636f 6465 6373 0a20 2020 2020 2020 2069  codecs.        i
-00009820: 6d70 6f72 7420 6c6f 6361 6c65 0a20 2020  mport locale.   
-00009830: 2020 2020 2073 7973 2e73 7464 6f75 7420       sys.stdout 
-00009840: 3d20 636f 6465 6373 2e67 6574 7772 6974  = codecs.getwrit
-00009850: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-00009860: 6c6f 6361 6c65 2e67 6574 7072 6566 6572  locale.getprefer
-00009870: 7265 6465 6e63 6f64 696e 6728 2929 2873  redencoding())(s
-00009880: 7973 2e73 7464 6f75 742c 2022 7265 706c  ys.stdout, "repl
-00009890: 6163 6522 290a 2020 2020 2020 2020 7379  ace").        sy
-000098a0: 732e 7374 6465 7272 203d 2063 6f64 6563  s.stderr = codec
-000098b0: 732e 6765 7477 7269 7465 7228 0a20 2020  s.getwriter(.   
-000098c0: 2020 2020 2020 2020 206c 6f63 616c 652e           locale.
-000098d0: 6765 7470 7265 6665 7272 6564 656e 636f  getpreferredenco
-000098e0: 6469 6e67 2829 2928 7379 732e 7374 6465  ding())(sys.stde
-000098f0: 7272 2c20 2272 6570 6c61 6365 2229 0a0a  rr, "replace")..
-00009900: 2020 2020 6966 2027 2d2d 7265 6769 7374      if '--regist
-00009910: 6572 2720 696e 2073 7973 2e61 7267 7620  er' in sys.argv 
-00009920: 6f72 2027 2d2d 756e 7265 6769 7374 6572  or '--unregister
-00009930: 2720 696e 2073 7973 2e61 7267 763a 0a20  ' in sys.argv:. 
-00009940: 2020 2020 2020 2069 6d70 6f72 7420 7079         import py
-00009950: 7468 6f6e 636f 6d0a 2020 2020 2020 2020  thoncom.        
-00009960: 6966 2054 5950 454c 4942 3a0a 2020 2020  if TYPELIB:.    
-00009970: 2020 2020 2020 2020 6966 2027 2d2d 7265          if '--re
-00009980: 6769 7374 6572 2720 696e 2073 7973 2e61  gister' in sys.a
-00009990: 7267 763a 0a20 2020 2020 2020 2020 2020  rgv:.           
-000099a0: 2020 2020 2074 6c62 203d 206f 732e 7061       tlb = os.pa
-000099b0: 7468 2e61 6273 7061 7468 280a 2020 2020  th.abspath(.    
-000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099d0: 6f73 2e70 6174 682e 6a6f 696e 2849 4e53  os.path.join(INS
-000099e0: 5441 4c4c 5f44 4952 2c20 2274 7970 656c  TALL_DIR, "typel
-000099f0: 6962 222c 2022 7472 617a 616d 6564 2e74  ib", "trazamed.t
-00009a00: 6c62 2229 290a 2020 2020 2020 2020 2020  lb")).          
-00009a10: 2020 2020 2020 7072 696e 7428 2252 6567        print("Reg
-00009a20: 6973 7465 7269 6e67 2025 7322 2025 2028  istering %s" % (
-00009a30: 746c 622c 2929 0a20 2020 2020 2020 2020  tlb,)).         
-00009a40: 2020 2020 2020 2074 6c69 203d 2070 7974         tli = pyt
-00009a50: 686f 6e63 6f6d 2e4c 6f61 6454 7970 654c  honcom.LoadTypeL
-00009a60: 6962 2874 6c62 290a 2020 2020 2020 2020  ib(tlb).        
-00009a70: 2020 2020 2020 2020 7079 7468 6f6e 636f          pythonco
-00009a80: 6d2e 5265 6769 7374 6572 5479 7065 4c69  m.RegisterTypeLi
-00009a90: 6228 746c 692c 2074 6c62 290a 2020 2020  b(tli, tlb).    
-00009aa0: 2020 2020 2020 2020 656c 6966 2027 2d2d          elif '--
-00009ab0: 756e 7265 6769 7374 6572 2720 696e 2073  unregister' in s
-00009ac0: 7973 2e61 7267 763a 0a20 2020 2020 2020  ys.argv:.       
-00009ad0: 2020 2020 2020 2020 206b 203d 2054 7261           k = Tra
-00009ae0: 7a61 4d65 640a 2020 2020 2020 2020 2020  zaMed.          
-00009af0: 2020 2020 2020 7079 7468 6f6e 636f 6d2e        pythoncom.
-00009b00: 556e 5265 6769 7374 6572 5479 7065 4c69  UnRegisterTypeLi
-00009b10: 6228 6b2e 5f74 7970 656c 6962 5f67 7569  b(k._typelib_gui
-00009b20: 645f 2c0a 2020 2020 2020 2020 2020 2020  d_,.            
-00009b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000010: 6e0a 2320 2d2a 2d20 636f 6469 6e67 3a20  n.# -*- coding: 
+00000020: 7574 662d 3820 2d2a 2d0a 2320 5468 6973  utf-8 -*-.# This
+00000030: 2070 726f 6772 616d 2069 7320 6672 6565   program is free
+00000040: 2073 6f66 7477 6172 653b 2079 6f75 2063   software; you c
+00000050: 616e 2072 6564 6973 7472 6962 7574 6520  an redistribute 
+00000060: 6974 2061 6e64 2f6f 7220 6d6f 6469 6679  it and/or modify
+00000070: 0a23 2069 7420 756e 6465 7220 7468 6520  .# it under the 
+00000080: 7465 726d 7320 6f66 2074 6865 2047 4e55  terms of the GNU
+00000090: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
+000000a0: 4c69 6365 6e73 6520 6173 2070 7562 6c69  License as publi
+000000b0: 7368 6564 2062 7920 7468 650a 2320 4672  shed by the.# Fr
+000000c0: 6565 2053 6f66 7477 6172 6520 466f 756e  ee Software Foun
+000000d0: 6461 7469 6f6e 3b20 6569 7468 6572 2076  dation; either v
+000000e0: 6572 7369 6f6e 2033 2c20 6f72 2028 6174  ersion 3, or (at
+000000f0: 2079 6f75 7220 6f70 7469 6f6e 2920 616e   your option) an
+00000100: 7920 6c61 7465 720a 2320 7665 7273 696f  y later.# versio
+00000110: 6e2e 0a23 0a23 2054 6869 7320 7072 6f67  n..#.# This prog
+00000120: 7261 6d20 6973 2064 6973 7472 6962 7574  ram is distribut
+00000130: 6564 2069 6e20 7468 6520 686f 7065 2074  ed in the hope t
+00000140: 6861 7420 6974 2077 696c 6c20 6265 2075  hat it will be u
+00000150: 7365 6675 6c2c 2062 7574 0a23 2057 4954  seful, but.# WIT
+00000160: 484f 5554 2041 4e59 2057 4152 5241 4e54  HOUT ANY WARRANT
+00000170: 593b 2077 6974 686f 7574 2065 7665 6e20  Y; without even 
+00000180: 7468 6520 696d 706c 6965 6420 7761 7272  the implied warr
+00000190: 616e 7479 206f 6620 4d45 5243 4841 4e54  anty of MERCHANT
+000001a0: 4942 494c 4954 590a 2320 6f72 2046 4954  IBILITY.# or FIT
+000001b0: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
+000001c0: 4355 4c41 5220 5055 5250 4f53 452e 2020  CULAR PURPOSE.  
+000001d0: 5365 6520 7468 6520 474e 5520 4765 6e65  See the GNU Gene
+000001e0: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
+000001f0: 7365 0a23 2066 6f72 206d 6f72 6520 6465  se.# for more de
+00000200: 7461 696c 732e 0a0a 2222 224d f364 756c  tails..."""M.dul
+00000210: 6f20 7061 7261 2054 7261 7a61 6269 6c69  o para Trazabili
+00000220: 6461 6420 6465 204d 6564 6963 616d 656e  dad de Medicamen
+00000230: 746f 7320 414e 4d41 5420 2d20 5041 4d49  tos ANMAT - PAMI
+00000240: 202d 2049 4e53 534a 5020 4469 7370 2e20   - INSSJP Disp. 
+00000250: 3336 3833 2f31 310a 7365 67fa 6e20 4573  3683/11.seg.n Es
+00000260: 7065 6369 6669 6361 6369 f36e 2054 e963  pecificaci.n T.c
+00000270: 6e69 6361 2070 6172 6120 5072 7565 6261  nica para Prueba
+00000280: 7320 6465 2053 6572 7669 6369 6f73 2076  s de Servicios v
+00000290: 3220 2832 3031 3329 2222 220a 0a23 2049  2 (2013)"""..# I
+000002a0: 6e66 6f72 6d61 6369 f36e 2061 6469 6369  nformaci.n adici
+000002b0: 6f6e 616c 2079 2064 6f63 756d 656e 7461  onal y documenta
+000002c0: 6369 f36e 3a0a 2320 6874 7470 3a2f 2f77  ci.n:.# http://w
+000002d0: 7777 2e73 6973 7465 6d61 7361 6769 6c65  ww.sistemasagile
+000002e0: 732e 636f 6d2e 6172 2f74 7261 632f 7769  s.com.ar/trac/wi
+000002f0: 6b69 2f54 7261 7a61 6269 6c69 6461 644d  ki/TrazabilidadM
+00000300: 6564 6963 616d 656e 746f 730a 0a5f 5f61  edicamentos..__a
+00000310: 7574 686f 725f 5f20 3d20 224d 6172 6961  uthor__ = "Maria
+00000320: 6e6f 2052 6569 6e67 6172 7420 3c72 6569  no Reingart <rei
+00000330: 6e67 6172 7440 676d 6169 6c2e 636f 6d3e  ngart@gmail.com>
+00000340: 220a 5f5f 636f 7079 7269 6768 745f 5f20  ".__copyright__ 
+00000350: 3d20 2243 6f70 7972 6967 6874 2028 4329  = "Copyright (C)
+00000360: 2032 3031 3120 4d61 7269 616e 6f20 5265   2011 Mariano Re
+00000370: 696e 6761 7274 220a 5f5f 6c69 6365 6e73  ingart".__licens
+00000380: 655f 5f20 3d20 2247 504c 2033 2e30 220a  e__ = "GPL 3.0".
+00000390: 5f5f 7665 7273 696f 6e5f 5f20 3d20 2231  __version__ = "1
+000003a0: 2e31 3662 220a 0a69 6d70 6f72 7420 6f73  .16b"..import os
+000003b0: 0a69 6d70 6f72 7420 736f 636b 6574 0a69  .import socket.i
+000003c0: 6d70 6f72 7420 7379 730a 696d 706f 7274  mport sys.import
+000003d0: 2064 6174 6574 696d 650a 696d 706f 7274   datetime.import
+000003e0: 2074 696d 650a 696d 706f 7274 2074 7261   time.import tra
+000003f0: 6365 6261 636b 0a69 6d70 6f72 7420 7079  ceback.import py
+00000400: 3373 696d 706c 6573 6f61 702e 636c 6965  3simplesoap.clie
+00000410: 6e74 0a66 726f 6d20 7079 3373 696d 706c  nt.from py3simpl
+00000420: 6573 6f61 702e 636c 6965 6e74 2069 6d70  esoap.client imp
+00000430: 6f72 7420 536f 6170 436c 6965 6e74 2c20  ort SoapClient, 
+00000440: 536f 6170 4661 756c 742c 2070 6172 7365  SoapFault, parse
+00000450: 5f70 726f 7879 2c20 5c0a 2020 2020 2020  _proxy, \.      
+00000460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000470: 2020 2020 2020 2020 2020 7365 745f 6874            set_ht
+00000480: 7470 5f77 7261 7070 6572 0a66 726f 6d20  tp_wrapper.from 
+00000490: 7079 3373 696d 706c 6573 6f61 702e 7369  py3simplesoap.si
+000004a0: 6d70 6c65 786d 6c20 696d 706f 7274 2053  mplexml import S
+000004b0: 696d 706c 6558 4d4c 456c 656d 656e 740a  impleXMLElement.
+000004c0: 6672 6f6d 2063 5374 7269 6e67 494f 2069  from cStringIO i
+000004d0: 6d70 6f72 7420 5374 7269 6e67 494f 0a0a  mport StringIO..
+000004e0: 2320 696d 706f 7274 6f20 6675 6e63 696f  # importo funcio
+000004f0: 6e65 7320 636f 6d70 6172 7469 6461 733a  nes compartidas:
+00000500: 0a66 726f 6d20 2e75 7469 6c73 2069 6d70  .from .utils imp
+00000510: 6f72 7420 280a 2020 2020 6c65 6572 2c20  ort (.    leer, 
+00000520: 6573 6372 6962 6972 2c20 6c65 6572 5f64  escribir, leer_d
+00000530: 6266 2c20 6775 6172 6461 725f 6462 662c  bf, guardar_dbf,
+00000540: 204e 2c20 412c 2049 2c20 6a73 6f6e 2c0a   N, A, I, json,.
+00000550: 2020 2020 6461 725f 6e6f 6d62 7265 5f63      dar_nombre_c
+00000560: 616d 706f 5f64 6266 2c20 6765 745f 696e  ampo_dbf, get_in
+00000570: 7374 616c 6c5f 6469 722c 2042 6173 6557  stall_dir, BaseW
+00000580: 532c 0a20 2020 2069 6e69 6369 616c 697a  S,.    inicializ
+00000590: 6172 5f79 5f63 6170 7475 7261 725f 6578  ar_y_capturar_ex
+000005a0: 6365 7063 696f 6e65 730a 290a 0a48 4f4d  cepciones.)..HOM
+000005b0: 4f20 3d20 4661 6c73 650a 5459 5045 4c49  O = False.TYPELI
+000005c0: 4220 3d20 4661 6c73 650a 0a57 5344 4c20  B = False..WSDL 
+000005d0: 3d20 2268 7474 7073 3a2f 2f73 6572 7669  = "https://servi
+000005e0: 6369 6f73 2e70 616d 692e 6f72 672e 6172  cios.pami.org.ar
+000005f0: 2f74 7261 7a61 6d65 642e 5765 6253 6572  /trazamed.WebSer
+00000600: 7669 6365 3f77 7364 6c22 0a4c 4f43 4154  vice?wsdl".LOCAT
+00000610: 494f 4e20 3d20 2268 7474 7073 3a2f 2f73  ION = "https://s
+00000620: 6572 7669 6369 6f73 2e70 616d 692e 6f72  ervicios.pami.or
+00000630: 672e 6172 2f74 7261 7a61 6d65 642e 5765  g.ar/trazamed.We
+00000640: 6253 6572 7669 6365 220a 2320 5753 444c  bService".# WSDL
+00000650: 203d 2022 6874 7470 733a 2f2f 7472 617a   = "https://traz
+00000660: 6162 696c 6964 6164 2e70 616d 692e 6f72  abilidad.pami.or
+00000670: 672e 6172 3a39 3035 302f 7472 617a 616d  g.ar:9050/trazam
+00000680: 6564 2e57 6562 5365 7276 6963 653f 7773  ed.WebService?ws
+00000690: 646c 220a 0a23 2046 6f72 6d61 746f 2064  dl"..# Formato d
+000006a0: 6520 4d65 6469 6361 6d65 6e74 6f73 4454  e MedicamentosDT
+000006b0: 4f2c 204d 6564 6963 616d 656e 746f 7344  O, MedicamentosD
+000006c0: 544f 4448 5365 7269 652c 204d 6564 6963  TODHSerie, Medic
+000006d0: 616d 656e 746f 7344 544f 4672 6163 6369  amentosDTOFracci
+000006e0: 6f6e 0a4d 4544 4943 414d 454e 544f 5320  on.MEDICAMENTOS 
+000006f0: 3d20 5b0a 2020 2020 2827 665f 6576 656e  = [.    ('f_even
+00000700: 746f 272c 2031 302c 2041 292c 2020 2020  to', 10, A),    
+00000710: 2020 2020 2020 2020 2020 2020 2320 666f              # fo
+00000720: 726d 6174 6f20 4444 2f4d 4d2f 4141 4141  rmato DD/MM/AAAA
+00000730: 0a20 2020 2028 2768 5f65 7665 6e74 6f27  .    ('h_evento'
+00000740: 2c20 352c 2041 292c 2020 2020 2020 2020  , 5, A),        
+00000750: 2020 2020 2020 2020 2023 2066 6f72 6d61           # forma
+00000760: 746f 2048 483a 4d4d 0a20 2020 2028 2767  to HH:MM.    ('g
+00000770: 6c6e 5f6f 7269 6765 6e27 2c20 3133 2c20  ln_origen', 13, 
+00000780: 4129 2c0a 2020 2020 2827 676c 6e5f 6465  A),.    ('gln_de
+00000790: 7374 696e 6f27 2c20 3133 2c20 4129 2c0a  stino', 13, A),.
+000007a0: 2020 2020 2827 6e5f 7265 6d69 746f 272c      ('n_remito',
+000007b0: 2032 302c 2041 292c 0a20 2020 2028 276e   20, A),.    ('n
+000007c0: 5f66 6163 7475 7261 272c 2032 302c 2041  _factura', 20, A
+000007d0: 292c 0a20 2020 2028 2776 656e 6369 6d69  ),.    ('vencimi
+000007e0: 656e 746f 272c 2031 302c 2041 292c 0a20  ento', 10, A),. 
+000007f0: 2020 2028 2767 7469 6e27 2c20 3134 2c20     ('gtin', 14, 
+00000800: 4129 2c0a 2020 2020 2827 6c6f 7465 272c  A),.    ('lote',
+00000810: 2032 302c 2041 292c 0a20 2020 2028 276e   20, A),.    ('n
+00000820: 756d 6572 6f5f 7365 7269 616c 272c 2032  umero_serial', 2
+00000830: 302c 2041 292c 0a20 2020 2028 2764 6573  0, A),.    ('des
+00000840: 6465 5f6e 756d 6572 6f5f 7365 7269 616c  de_numero_serial
+00000850: 272c 2032 302c 2041 292c 2020 2020 2023  ', 20, A),     #
+00000860: 2073 656e 644d 6564 6963 616d 656e 746f   sendMedicamento
+00000870: 7344 4853 6572 6965 0a20 2020 2028 2768  sDHSerie.    ('h
+00000880: 6173 7461 5f6e 756d 6572 6f5f 7365 7269  asta_numero_seri
+00000890: 616c 272c 2032 302c 2041 292c 2020 2020  al', 20, A),    
+000008a0: 2023 2073 656e 644d 6564 6963 616d 656e   # sendMedicamen
+000008b0: 746f 7344 4853 6572 6965 0a20 2020 2028  tosDHSerie.    (
+000008c0: 2769 645f 6f62 7261 5f73 6f63 6961 6c27  'id_obra_social'
+000008d0: 2c20 392c 204e 292c 0a20 2020 2028 2769  , 9, N),.    ('i
+000008e0: 645f 6576 656e 746f 272c 2033 2c20 4e29  d_evento', 3, N)
+000008f0: 2c0a 2020 2020 2827 6375 6974 5f6f 7269  ,.    ('cuit_ori
+00000900: 6765 6e27 2c20 3131 2c20 4129 2c0a 2020  gen', 11, A),.  
+00000910: 2020 2827 6375 6974 5f64 6573 7469 6e6f    ('cuit_destino
+00000920: 272c 2031 312c 2041 292c 0a20 2020 2028  ', 11, A),.    (
+00000930: 2761 7065 6c6c 6964 6f27 2c20 3530 2c20  'apellido', 50, 
+00000940: 4129 2c0a 2020 2020 2827 6e6f 6d62 7265  A),.    ('nombre
+00000950: 7327 2c20 3130 302c 2041 292c 0a20 2020  s', 100, A),.   
+00000960: 2028 2774 6970 6f5f 646f 6375 6d65 6e74   ('tipo_document
+00000970: 6f27 2c20 322c 204e 292c 2020 2020 2020  o', 2, N),      
+00000980: 2020 2020 2023 2039 363a 2044 4e49 2c38       # 96: DNI,8
+00000990: 303a 2043 5549 540a 2020 2020 2827 6e5f  0: CUIT.    ('n_
+000009a0: 646f 6375 6d65 6e74 6f27 2c20 3130 2c20  documento', 10, 
+000009b0: 4129 2c0a 2020 2020 2827 7365 786f 272c  A),.    ('sexo',
+000009c0: 2031 2c20 4129 2c20 2020 2020 2020 2020   1, A),         
+000009d0: 2020 2020 2020 2020 2020 2020 2320 4d20              # M 
+000009e0: 6f20 460a 2020 2020 2827 6469 7265 6363  o F.    ('direcc
+000009f0: 696f 6e27 2c20 3130 302c 2041 292c 0a20  ion', 100, A),. 
+00000a00: 2020 2028 276e 756d 6572 6f27 2c20 3130     ('numero', 10
+00000a10: 2c20 4129 2c0a 2020 2020 2827 7069 736f  , A),.    ('piso
+00000a20: 272c 2035 2c20 4129 2c0a 2020 2020 2827  ', 5, A),.    ('
+00000a30: 6465 7074 6f27 2c20 352c 2041 292c 0a20  depto', 5, A),. 
+00000a40: 2020 2028 276c 6f63 616c 6964 6164 272c     ('localidad',
+00000a50: 2035 302c 2041 292c 0a20 2020 2028 2770   50, A),.    ('p
+00000a60: 726f 7669 6e63 6961 272c 2031 3030 2c20  rovincia', 100, 
+00000a70: 4129 2c0a 2020 2020 2827 6e5f 706f 7374  A),.    ('n_post
+00000a80: 616c 272c 2038 2c20 4129 2c0a 2020 2020  al', 8, A),.    
+00000a90: 2827 6665 6368 615f 6e61 6369 6d69 656e  ('fecha_nacimien
+00000aa0: 746f 272c 2031 3030 2c20 4129 2c0a 2020  to', 100, A),.  
+00000ab0: 2020 2827 7465 6c65 666f 6e6f 272c 2033    ('telefono', 3
+00000ac0: 302c 2041 292c 0a20 2020 2028 276e 726f  0, A),.    ('nro
+00000ad0: 5f61 736f 6369 6164 6f27 2c20 3330 2c20  _asociado', 30, 
+00000ae0: 4129 2c0a 2020 2020 2827 6361 6e74 6964  A),.    ('cantid
+00000af0: 6164 272c 2033 2c20 4e29 2c20 2020 2020  ad', 3, N),     
+00000b00: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+00000b10: 6e64 4d65 6469 6361 6d65 6e74 6f73 4672  ndMedicamentosFr
+00000b20: 6163 6369 6f6e 0a20 2020 2028 2763 6f64  accion.    ('cod
+00000b30: 6967 6f5f 7472 616e 7361 6363 696f 6e27  igo_transaccion'
+00000b40: 2c20 3134 2c20 4129 2c0a 5d0a 0a23 2046  , 14, A),.]..# F
+00000b50: 6f72 6d61 746f 2070 6172 6120 5472 616e  ormato para Tran
+00000b60: 7361 6363 696f 6e50 6c61 696e 5753 2028  saccionPlainWS (
+00000b70: 6765 7454 7261 6e73 6163 6369 6f6e 6573  getTransacciones
+00000b80: 4e6f 436f 6e66 6972 6d61 6461 7329 0a54  NoConfirmadas).T
+00000b90: 5241 4e53 4143 4349 4f4e 4553 203d 205b  RANSACCIONES = [
+00000ba0: 0a20 2020 2028 275f 6964 5f74 7261 6e73  .    ('_id_trans
+00000bb0: 6163 6369 6f6e 272c 2031 342c 2041 292c  accion', 14, A),
+00000bc0: 0a20 2020 2028 275f 6964 5f74 7261 6e73  .    ('_id_trans
+00000bd0: 6163 6369 6f6e 5f67 6c6f 6261 6c27 2c20  accion_global', 
+00000be0: 3134 2c20 4129 2c0a 2020 2020 2827 5f66  14, A),.    ('_f
+00000bf0: 5f65 7665 6e74 6f27 2c20 3130 2c20 4129  _evento', 10, A)
+00000c00: 2c0a 2020 2020 2827 5f66 5f74 7261 6e73  ,.    ('_f_trans
+00000c10: 6163 6369 6f6e 272c 2031 362c 2041 292c  accion', 16, A),
+00000c20: 2020 2020 2020 2020 2020 2320 666f 726d            # form
+00000c30: 6174 6f20 4444 2f4d 4d2f 4141 4141 2048  ato DD/MM/AAAA H
+00000c40: 483a 4d4d 0a20 2020 2028 275f 6774 696e  H:MM.    ('_gtin
+00000c50: 272c 2031 342c 2041 292c 0a20 2020 2028  ', 14, A),.    (
+00000c60: 275f 6c6f 7465 272c 2032 302c 2041 292c  '_lote', 20, A),
+00000c70: 0a20 2020 2028 275f 6e75 6d65 726f 5f73  .    ('_numero_s
+00000c80: 6572 6961 6c27 2c20 3230 2c20 4129 2c0a  erial', 20, A),.
+00000c90: 2020 2020 2827 5f6e 6f6d 6272 6527 2c20      ('_nombre', 
+00000ca0: 3230 302c 2041 292c 0a20 2020 2028 275f  200, A),.    ('_
+00000cb0: 645f 6576 656e 746f 272c 2031 3030 2c20  d_evento', 100, 
+00000cc0: 4129 2c0a 2020 2020 2827 5f67 6c6e 5f6f  A),.    ('_gln_o
+00000cd0: 7269 6765 6e27 2c20 3133 2c20 4129 2c0a  rigen', 13, A),.
+00000ce0: 2020 2020 2827 5f72 617a 6f6e 5f73 6f63      ('_razon_soc
+00000cf0: 6961 6c5f 6f72 6967 656e 272c 2032 3030  ial_origen', 200
+00000d00: 2c20 4129 2c0a 2020 2020 2827 5f67 6c6e  , A),.    ('_gln
+00000d10: 5f64 6573 7469 6e6f 272c 2031 332c 2041  _destino', 13, A
+00000d20: 292c 0a20 2020 2028 275f 7261 7a6f 6e5f  ),.    ('_razon_
+00000d30: 736f 6369 616c 5f64 6573 7469 6e6f 272c  social_destino',
+00000d40: 2032 3030 2c20 4129 2c0a 2020 2020 2827   200, A),.    ('
+00000d50: 5f6e 5f72 656d 6974 6f27 2c20 3230 2c20  _n_remito', 20, 
+00000d60: 4129 2c0a 2020 2020 2827 5f6e 5f66 6163  A),.    ('_n_fac
+00000d70: 7475 7261 272c 2032 302c 2041 292c 0a20  tura', 20, A),. 
+00000d80: 2020 2028 275f 7665 6e63 696d 6965 6e74     ('_vencimient
+00000d90: 6f27 2c20 3130 2c20 4129 2c0a 2020 2020  o', 10, A),.    
+00000da0: 2827 5f69 645f 6576 656e 746f 272c 2033  ('_id_evento', 3
+00000db0: 2c20 4e29 2c20 2020 2020 2020 2020 2020  , N),           
+00000dc0: 2020 2020 2320 6167 7265 6761 646f 2065      # agregado e
+00000dd0: 6c20 3330 2f30 312f 3230 3134 0a5d 0a0a  l 30/01/2014.]..
+00000de0: 2320 466f 726d 6174 6f20 7061 7261 2045  # Formato para E
+00000df0: 7272 6f72 6573 0a45 5252 4f52 4553 203d  rrores.ERRORES =
+00000e00: 205b 0a20 2020 2028 2763 5f65 7272 6f72   [.    ('c_error
+00000e10: 272c 2034 2c20 4129 2c20 2020 2020 2020  ', 4, A),       
+00000e20: 2020 2020 2020 2020 2020 2320 63f3 6469            # c.di
+00000e30: 676f 0a20 2020 2028 2764 5f65 7272 6f72  go.    ('d_error
+00000e40: 272c 2032 3530 2c20 4129 2c20 2020 2020  ', 250, A),     
+00000e50: 2020 2020 2020 2020 2020 2320 6465 7363            # desc
+00000e60: 7269 7063 69f3 6e0a 2020 2020 5d0a 0a0a  ripci.n.    ]...
+00000e70: 636c 6173 7320 5472 617a 614d 6564 2842  class TrazaMed(B
+00000e80: 6173 6557 5329 3a0a 2020 2020 2249 6e74  aseWS):.    "Int
+00000e90: 6572 6661 7a20 7061 7261 2065 6c20 5765  erfaz para el We
+00000ea0: 6253 6572 7669 6365 2064 6520 5472 617a  bService de Traz
+00000eb0: 6162 696c 6964 6164 2064 6520 4d65 6469  abilidad de Medi
+00000ec0: 6361 6d65 6e74 6f73 2041 4e4d 4154 202d  camentos ANMAT -
+00000ed0: 205c 0a20 2020 2050 414d 4920 2d20 494e   \.    PAMI - IN
+00000ee0: 5353 4a50 220a 2020 2020 5f70 7562 6c69  SSJP".    _publi
+00000ef0: 635f 6d65 7468 6f64 735f 203d 205b 2753  c_methods_ = ['S
+00000f00: 656e 644d 6564 6963 616d 656e 746f 7327  endMedicamentos'
+00000f10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000f20: 2020 2020 2020 2020 2020 2753 656e 6443            'SendC
+00000f30: 616e 6365 6c61 6354 7261 6e73 6163 6327  ancelacTransacc'
+00000f40: 2c20 2753 656e 6443 616e 6365 6c61 6354  , 'SendCancelacT
+00000f50: 7261 6e73 6163 6350 6172 6369 616c 272c  ransaccParcial',
+00000f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000f70: 2020 2020 2020 2020 2027 5365 6e64 4d65           'SendMe
+00000f80: 6469 6361 6d65 6e74 6f73 4448 5365 7269  dicamentosDHSeri
+00000f90: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
+00000fa0: 2020 2020 2020 2020 2020 2020 2753 656e              'Sen
+00000fb0: 644d 6564 6963 616d 656e 746f 7346 7261  dMedicamentosFra
+00000fc0: 6363 696f 6e27 2c0a 2020 2020 2020 2020  ccion',.        
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fe0: 2753 656e 6443 6f6e 6669 726d 6154 7261  'SendConfirmaTra
+00000ff0: 6e73 6163 6327 2c20 2753 656e 6441 6c65  nsacc', 'SendAle
+00001000: 7274 6154 7261 6e73 6163 6327 2c0a 2020  rtaTransacc',.  
+00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001020: 2020 2020 2020 2747 6574 5472 616e 7361        'GetTransa
+00001030: 6363 696f 6e65 734e 6f43 6f6e 6669 726d  ccionesNoConfirm
+00001040: 6164 6173 272c 0a20 2020 2020 2020 2020  adas',.         
+00001050: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001060: 4765 7445 6e76 696f 7350 726f 7069 6f73  GetEnviosPropios
+00001070: 416c 6572 7461 646f 7327 2c20 2747 6574  Alertados', 'Get
+00001080: 436f 6e73 756c 7461 5374 6f63 6b27 2c0a  ConsultaStock',.
+00001090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010a0: 2020 2020 2020 2020 2747 6574 5472 616e          'GetTran
+000010b0: 7361 6363 696f 6e65 7357 5327 2c20 2747  saccionesWS', 'G
+000010c0: 6574 4361 7461 6c6f 676f 456c 6563 7472  etCatalogoElectr
+000010d0: 6f6e 6963 6f42 7947 5449 4e27 2c0a 2020  onicoByGTIN',.  
+000010e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010f0: 2020 2020 2020 2743 6f6e 6563 7461 7227        'Conectar'
+00001100: 2c20 274c 6565 7245 7272 6f72 272c 2027  , 'LeerError', '
+00001110: 4c65 6572 5472 616e 7361 6363 696f 6e27  LeerTransaccion'
+00001120: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001130: 2020 2020 2020 2020 2020 2753 6574 5573            'SetUs
+00001140: 6572 6e61 6d65 272c 2027 5365 7450 6173  ername', 'SetPas
+00001150: 7377 6f72 6427 2c0a 2020 2020 2020 2020  sword',.        
+00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001170: 2753 6574 5061 7261 6d65 7472 6f27 2c20  'SetParametro', 
+00001180: 2747 6574 5061 7261 6d65 7472 6f27 2c0a  'GetParametro',.
+00001190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011a0: 2020 2020 2020 2020 2747 6574 436f 6469          'GetCodi
+000011b0: 676f 5472 616e 7361 6363 696f 6e27 2c20  goTransaccion', 
+000011c0: 2747 6574 5265 7375 6c74 6164 6f27 2c20  'GetResultado', 
+000011d0: 274c 6f61 6454 6573 7458 4d4c 275d 0a0a  'LoadTestXML']..
+000011e0: 2020 2020 5f70 7562 6c69 635f 6174 7472      _public_attr
+000011f0: 735f 203d 205b 0a20 2020 2020 2020 2027  s_ = [.        '
+00001200: 5573 6572 6e61 6d65 272c 2027 5061 7373  Username', 'Pass
+00001210: 776f 7264 272c 0a20 2020 2020 2020 2027  word',.        '
+00001220: 436f 6469 676f 5472 616e 7361 6363 696f  CodigoTransaccio
+00001230: 6e27 2c20 2745 7272 6f72 6573 272c 2027  n', 'Errores', '
+00001240: 5265 7375 6c74 6164 6f27 2c0a 2020 2020  Resultado',.    
+00001250: 2020 2020 2758 6d6c 5265 7175 6573 7427      'XmlRequest'
+00001260: 2c20 2758 6d6c 5265 7370 6f6e 7365 272c  , 'XmlResponse',
+00001270: 0a20 2020 2020 2020 2027 5665 7273 696f  .        'Versio
+00001280: 6e27 2c20 2749 6e73 7461 6c6c 4469 7227  n', 'InstallDir'
+00001290: 2c0a 2020 2020 2020 2020 2754 7261 6365  ,.        'Trace
+000012a0: 6261 636b 272c 2027 4578 6365 7063 696f  back', 'Excepcio
+000012b0: 6e27 2c20 274c 616e 7a61 7245 7863 6570  n', 'LanzarExcep
+000012c0: 6369 6f6e 6573 272c 0a20 2020 2020 2020  ciones',.       
+000012d0: 2027 4361 6e74 5061 6769 6e61 7327 2c20   'CantPaginas', 
+000012e0: 2748 6179 4572 726f 7227 2c20 2754 7261  'HayError', 'Tra
+000012f0: 6e73 6163 6369 6f6e 506c 6169 6e57 5327  nsaccionPlainWS'
+00001300: 2c0a 2020 2020 2020 2020 5d0a 0a20 2020  ,.        ]..   
+00001310: 205f 7265 675f 7072 6f67 6964 5f20 3d20   _reg_progid_ = 
+00001320: 2254 7261 7a61 4d65 6422 0a20 2020 205f  "TrazaMed".    _
+00001330: 7265 675f 636c 7369 645f 203d 2022 7b38  reg_clsid_ = "{8
+00001340: 3437 3238 3637 412d 4145 3646 2d34 3837  472867A-AE6F-487
+00001350: 462d 3835 3534 2d43 3243 3839 3643 4646  F-8554-C2C896CFF
+00001360: 4333 457d 220a 0a20 2020 2069 6620 5459  C3E}"..    if TY
+00001370: 5045 4c49 423a 0a20 2020 2020 2020 205f  PELIB:.        _
+00001380: 7479 7065 6c69 625f 6775 6964 5f20 3d20  typelib_guid_ = 
+00001390: 277b 4639 3932 4542 3745 2d41 4642 442d  '{F992EB7E-AFBD-
+000013a0: 3431 4242 2d42 3731 372d 3536 3933 4433  41BB-B717-5693D3
+000013b0: 4132 4241 4442 7d27 0a20 2020 2020 2020  A2BADB}'.       
+000013c0: 205f 7479 7065 6c69 625f 7665 7273 696f   _typelib_versio
+000013d0: 6e5f 203d 2031 2c20 340a 2020 2020 2020  n_ = 1, 4.      
+000013e0: 2020 5f63 6f6d 5f69 6e74 6572 6661 6365    _com_interface
+000013f0: 735f 203d 205b 2749 5472 617a 614d 6564  s_ = ['ITrazaMed
+00001400: 275d 0a0a 2020 2020 2320 5661 7269 6162  ']..    # Variab
+00001410: 6c65 7320 676c 6f62 616c 6573 2070 6172  les globales par
+00001420: 6120 4261 7365 5753 3a0a 2020 2020 484f  a BaseWS:.    HO
+00001430: 4d4f 203d 2048 4f4d 4f0a 2020 2020 5753  MO = HOMO.    WS
+00001440: 444c 203d 2057 5344 4c0a 2020 2020 5665  DL = WSDL.    Ve
+00001450: 7273 696f 6e20 3d20 2225 7320 2573 2025  rsion = "%s %s %
+00001460: 7322 2025 2028 5f5f 7665 7273 696f 6e5f  s" % (__version_
+00001470: 5f2c 2048 4f4d 4f20 616e 6420 2748 6f6d  _, HOMO and 'Hom
+00001480: 6f6c 6f67 6163 69f3 6e27 206f 7220 2727  ologaci.n' or ''
+00001490: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000014a0: 2020 2020 2020 2020 2020 2020 2020 7079                py
+000014b0: 3373 696d 706c 6573 6f61 702e 636c 6965  3simplesoap.clie
+000014c0: 6e74 2e5f 5f76 6572 7369 6f6e 5f5f 290a  nt.__version__).
+000014d0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000014e0: 5f28 7365 6c66 2c20 7265 696e 7465 6e74  _(self, reintent
+000014f0: 6f73 3d31 293a 0a20 2020 2020 2020 2073  os=1):.        s
+00001500: 656c 662e 5573 6572 6e61 6d65 203d 2073  elf.Username = s
+00001510: 656c 662e 5061 7373 776f 7264 203d 204e  elf.Password = N
+00001520: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+00001530: 2e54 7261 6e73 6163 6369 6f6e 506c 6169  .TransaccionPlai
+00001540: 6e57 5320 3d20 5b5d 0a20 2020 2020 2020  nWS = [].       
+00001550: 2042 6173 6557 532e 5f5f 696e 6974 5f5f   BaseWS.__init__
+00001560: 2873 656c 662c 2072 6569 6e74 656e 746f  (self, reintento
+00001570: 7329 0a0a 2020 2020 6465 6620 696e 6963  s)..    def inic
+00001580: 6961 6c69 7a61 7228 7365 6c66 293a 0a20  ializar(self):. 
+00001590: 2020 2020 2020 2042 6173 6557 532e 696e         BaseWS.in
+000015a0: 6963 6961 6c69 7a61 7228 7365 6c66 290a  icializar(self).
+000015b0: 2020 2020 2020 2020 7365 6c66 2e43 6f64          self.Cod
+000015c0: 6967 6f54 7261 6e73 6163 6369 6f6e 203d  igoTransaccion =
+000015d0: 2073 656c 662e 4572 726f 7265 7320 3d20   self.Errores = 
+000015e0: 7365 6c66 2e52 6573 756c 7461 646f 203d  self.Resultado =
+000015f0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+00001600: 6c66 2e52 6573 756c 7461 646f 203d 2027  lf.Resultado = '
+00001610: 270a 2020 2020 2020 2020 7365 6c66 2e45  '.        self.E
+00001620: 7272 6f72 6573 203d 205b 5d20 2020 2320  rrores = []   # 
+00001630: 6c69 7374 6120 6465 2073 7472 696e 6773  lista de strings
+00001640: 2070 6172 6120 6c61 2069 6e74 6572 6661   para la interfa
+00001650: 7a0a 2020 2020 2020 2020 7365 6c66 2e65  z.        self.e
+00001660: 7272 6f72 6573 203d 205b 5d20 2020 2320  rrores = []   # 
+00001670: 6c69 7374 6120 6465 2064 6963 6369 6f6e  lista de diccion
+00001680: 6172 696f 7320 2875 736f 2069 6e74 6572  arios (uso inter
+00001690: 6e6f 290a 2020 2020 2020 2020 7365 6c66  no).        self
+000016a0: 2e43 616e 7450 6167 696e 6173 203d 2073  .CantPaginas = s
+000016b0: 656c 662e 4861 7945 7272 6f72 203d 204e  elf.HayError = N
+000016c0: 6f6e 650a 0a20 2020 2064 6566 205f 5f61  one..    def __a
+000016d0: 6e61 6c69 7a61 725f 6572 726f 7265 7328  nalizar_errores(
+000016e0: 7365 6c66 2c20 7265 7429 3a0a 2020 2020  self, ret):.    
+000016f0: 2020 2020 2243 6f6d 7072 7565 6261 2079      "Comprueba y
+00001700: 2065 7874 7261 6520 6572 726f 7265 7320   extrae errores 
+00001710: 7369 2065 7869 7374 656e 2065 6e20 6c61  si existen en la
+00001720: 2072 6573 7075 6573 7461 2058 4d4c 220a   respuesta XML".
+00001730: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
+00001740: 6f72 6573 203d 2072 6574 2e67 6574 2827  ores = ret.get('
+00001750: 6572 726f 7265 7327 2c20 5b5d 290a 2020  errores', []).  
+00001760: 2020 2020 2020 7365 6c66 2e45 7272 6f72        self.Error
+00001770: 6573 203d 205b 2225 733a 2025 7322 2025  es = ["%s: %s" %
+00001780: 2028 6974 5b27 5f63 5f65 7272 6f72 275d   (it['_c_error']
+00001790: 2c20 6974 5b27 5f64 5f65 7272 6f72 275d  , it['_d_error']
+000017a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000017b0: 2020 2020 2020 2020 2020 666f 7220 6974            for it
+000017c0: 2069 6e20 7265 742e 6765 7428 2765 7272   in ret.get('err
+000017d0: 6f72 6573 272c 205b 5d29 5d0a 2020 2020  ores', [])].    
+000017e0: 2020 2020 7365 6c66 2e52 6573 756c 7461      self.Resulta
+000017f0: 646f 203d 2072 6574 2e67 6574 2827 7265  do = ret.get('re
+00001800: 7375 6c74 6164 6f27 290a 0a20 2020 2064  sultado')..    d
+00001810: 6566 2043 6f6e 6563 7461 7228 0a20 2020  ef Conectar(.   
+00001820: 2020 2020 2073 656c 662c 2063 6163 6865       self, cache
+00001830: 3d4e 6f6e 652c 2077 7364 6c3d 4e6f 6e65  =None, wsdl=None
+00001840: 2c20 7072 6f78 793d 2222 2c20 7772 6170  , proxy="", wrap
+00001850: 7065 723d 4e6f 6e65 2c0a 2020 2020 2020  per=None,.      
+00001860: 2020 6361 6365 7274 3d4e 6f6e 652c 2074    cacert=None, t
+00001870: 696d 656f 7574 3d33 300a 2020 2020 293a  imeout=30.    ):
+00001880: 0a20 2020 2020 2020 2023 2043 6f6e 6563  .        # Conec
+00001890: 746f 2075 7361 6e64 6f20 656c 206d e974  to usando el m.t
+000018a0: 6f64 6f20 6573 7461 6e64 6172 643a 0a20  odo estandard:. 
+000018b0: 2020 2020 2020 206f 6b20 3d20 4261 7365         ok = Base
+000018c0: 5753 2e43 6f6e 6563 7461 7228 7365 6c66  WS.Conectar(self
+000018d0: 2c20 6361 6368 652c 2077 7364 6c2c 2070  , cache, wsdl, p
+000018e0: 726f 7879 2c20 7772 6170 7065 722c 2063  roxy, wrapper, c
+000018f0: 6163 6572 742c 0a20 2020 2020 2020 2020  acert,.         
+00001900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001910: 2020 2020 7469 6d65 6f75 742c 2073 6f61      timeout, soa
+00001920: 705f 7365 7276 6572 3d22 6a65 7474 7922  p_server="jetty"
+00001930: 290a 0a20 2020 2020 2020 2069 6620 6f6b  )..        if ok
+00001940: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00001950: 7369 2065 6c20 6172 6368 6976 6f20 6573  si el archivo es
+00001960: 206c 6f63 616c 2c20 6173 756d 6f20 7175   local, asumo qu
+00001970: 6520 7961 2065 7374 6120 636f 7272 6567  e ya esta correg
+00001980: 6964 6f3a 0a20 2020 2020 2020 2020 2020  ido:.           
+00001990: 2069 6620 6e6f 7420 7365 6c66 2e77 7364   if not self.wsd
+000019a0: 6c2e 7374 6172 7473 7769 7468 2822 6669  l.startswith("fi
+000019b0: 6c65 2229 3a0a 2020 2020 2020 2020 2020  le"):.          
+000019c0: 2020 2020 2020 2320 636f 7272 696a 6f20        # corrijo 
+000019d0: 7562 6963 6163 69f3 6e20 6465 6c20 7365  ubicaci.n del se
+000019e0: 7276 6964 6f72 2028 6c6f 6361 6c68 6f73  rvidor (localhos
+000019f0: 743a 3930 3530 2065 6e20 656c 2057 5344  t:9050 en el WSD
+00001a00: 4c29 0a20 2020 2020 2020 2020 2020 2020  L).             
+00001a10: 2020 206c 6f63 6174 696f 6e20 3d20 7365     location = se
+00001a20: 6c66 2e77 7364 6c5b 3a2d 355d 0a20 2020  lf.wsdl[:-5].   
+00001a30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00001a40: 2749 5765 6253 6572 7669 6365 5365 7276  'IWebServiceServ
+00001a50: 6963 6527 2069 6e20 7365 6c66 2e63 6c69  ice' in self.cli
+00001a60: 656e 742e 7365 7276 6963 6573 3a0a 2020  ent.services:.  
+00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a80: 2020 2320 7665 7273 696f 6e20 310a 2020    # version 1.  
+00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001aa0: 2020 7773 203d 2073 656c 662e 636c 6965    ws = self.clie
+00001ab0: 6e74 2e73 6572 7669 6365 735b 2749 5765  nt.services['IWe
+00001ac0: 6253 6572 7669 6365 5365 7276 6963 6527  bServiceService'
+00001ad0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00001ae0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00001af0: 2020 2020 2020 2020 2020 2020 7773 203d              ws =
+00001b00: 2073 656c 662e 636c 6965 6e74 2e73 6572   self.client.ser
+00001b10: 7669 6365 735b 2749 5765 6253 6572 7669  vices['IWebServi
+00001b20: 6365 275d 2020 2023 2076 6572 7369 6f6e  ce']   # version
+00001b30: 2032 0a20 2020 2020 2020 2020 2020 2020   2.             
+00001b40: 2020 2077 735b 2770 6f72 7473 275d 5b27     ws['ports']['
+00001b50: 4957 6562 5365 7276 6963 6550 6f72 7427  IWebServicePort'
+00001b60: 5d5b 276c 6f63 6174 696f 6e27 5d20 3d20  ]['location'] = 
+00001b70: 6c6f 6361 7469 6f6e 0a0a 2020 2020 2020  location..      
+00001b80: 2020 2020 2020 2320 4573 7461 626c 6563        # Establec
+00001b90: 6572 2063 7265 6465 6e63 6961 6c65 7320  er credenciales 
+00001ba0: 6465 2073 6567 7572 6964 6164 3a0a 2020  de seguridad:.  
+00001bb0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00001bc0: 6c69 656e 745b 2777 7373 653a 5365 6375  lient['wsse:Secu
+00001bd0: 7269 7479 275d 203d 207b 0a20 2020 2020  rity'] = {.     
+00001be0: 2020 2020 2020 2020 2020 2027 7773 7365             'wsse
+00001bf0: 3a55 7365 726e 616d 6554 6f6b 656e 273a  :UsernameToken':
+00001c00: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00001c10: 2020 2020 2020 2027 7773 7365 3a55 7365         'wsse:Use
+00001c20: 726e 616d 6527 3a20 7365 6c66 2e55 7365  rname': self.Use
+00001c30: 726e 616d 652c 0a20 2020 2020 2020 2020  rname,.         
+00001c40: 2020 2020 2020 2020 2020 2027 7773 7365             'wsse
+00001c50: 3a50 6173 7377 6f72 6427 3a20 7365 6c66  :Password': self
+00001c60: 2e50 6173 7377 6f72 642c 0a20 2020 2020  .Password,.     
+00001c70: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00001c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001c90: 207d 0a20 2020 2020 2020 2072 6574 7572   }.        retur
+00001ca0: 6e20 6f6b 0a0a 2020 2020 4069 6e69 6369  n ok..    @inici
+00001cb0: 616c 697a 6172 5f79 5f63 6170 7475 7261  alizar_y_captura
+00001cc0: 725f 6578 6365 7063 696f 6e65 730a 2020  r_excepciones.  
+00001cd0: 2020 6465 6620 5365 6e64 4d65 6469 6361    def SendMedica
+00001ce0: 6d65 6e74 6f73 2873 656c 662c 2075 7375  mentos(self, usu
+00001cf0: 6172 696f 2c20 7061 7373 776f 7264 2c0a  ario, password,.
+00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d10: 2020 2020 2020 2020 2066 5f65 7665 6e74           f_event
+00001d20: 6f2c 2068 5f65 7665 6e74 6f2c 2067 6c6e  o, h_evento, gln
+00001d30: 5f6f 7269 6765 6e2c 2067 6c6e 5f64 6573  _origen, gln_des
+00001d40: 7469 6e6f 2c0a 2020 2020 2020 2020 2020  tino,.          
+00001d50: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00001d60: 5f72 656d 6974 6f2c 206e 5f66 6163 7475  _remito, n_factu
+00001d70: 7261 2c20 7665 6e63 696d 6965 6e74 6f2c  ra, vencimiento,
+00001d80: 2067 7469 6e2c 206c 6f74 652c 0a20 2020   gtin, lote,.   
+00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001da0: 2020 2020 2020 6e75 6d65 726f 5f73 6572        numero_ser
+00001db0: 6961 6c2c 2069 645f 6f62 7261 5f73 6f63  ial, id_obra_soc
+00001dc0: 6961 6c2c 2069 645f 6576 656e 746f 2c0a  ial, id_evento,.
+00001dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001de0: 2020 2020 2020 2020 2063 7569 745f 6f72           cuit_or
+00001df0: 6967 656e 3d27 272c 2063 7569 745f 6465  igen='', cuit_de
+00001e00: 7374 696e 6f3d 2727 2c20 6170 656c 6c69  stino='', apelli
+00001e10: 646f 3d27 272c 0a20 2020 2020 2020 2020  do='',.         
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e30: 6e6f 6d62 7265 733d 2727 2c20 7469 706f  nombres='', tipo
+00001e40: 5f64 6f63 756d 656e 746f 3d27 272c 206e  _documento='', n
+00001e50: 5f64 6f63 756d 656e 746f 3d27 272c 0a20  _documento='',. 
+00001e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e70: 2020 2020 2020 2020 7365 786f 3d27 272c          sexo='',
+00001e80: 2064 6972 6563 6369 6f6e 3d27 272c 206e   direccion='', n
+00001e90: 756d 6572 6f3d 2727 2c20 7069 736f 3d27  umero='', piso='
+00001ea0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00001eb0: 2020 2020 2020 2020 2020 2020 6465 7074              dept
+00001ec0: 6f3d 2727 2c20 6c6f 6361 6c69 6461 643d  o='', localidad=
+00001ed0: 2727 2c20 7072 6f76 696e 6369 613d 2727  '', provincia=''
+00001ee0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001ef0: 2020 2020 2020 2020 2020 206e 5f70 6f73             n_pos
+00001f00: 7461 6c3d 2727 2c20 6665 6368 615f 6e61  tal='', fecha_na
+00001f10: 6369 6d69 656e 746f 3d27 272c 2074 656c  cimiento='', tel
+00001f20: 6566 6f6e 6f3d 2727 2c0a 2020 2020 2020  efono='',.      
+00001f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f40: 2020 206e 726f 5f61 736f 6369 6164 6f3d     nro_asociado=
+00001f50: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00001f60: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00001f70: 3a0a 2020 2020 2020 2020 2252 6561 6c69  :.        "Reali
+00001f80: 7a61 2065 6c20 7265 6769 7374 726f 2064  za el registro d
+00001f90: 6520 756e 6120 7472 616e 7361 6363 69f3  e una transacci.
+00001fa0: 6e20 6465 206d 6564 6963 616d 656e 746f  n de medicamento
+00001fb0: 732e 2022 0a20 2020 2020 2020 2023 2063  s. ".        # c
+00001fc0: 7265 6f20 6c6f 7320 7061 72e1 6d65 7472  reo los par.metr
+00001fd0: 6f73 2070 6172 6120 6573 7461 206c 6c61  os para esta lla
+00001fe0: 6d61 6461 0a20 2020 2020 2020 2070 6172  mada.        par
+00001ff0: 616d 7320 3d20 7b0a 2020 2020 2020 2020  ams = {.        
+00002000: 2020 2020 2766 5f65 7665 6e74 6f27 3a20      'f_evento': 
+00002010: 665f 6576 656e 746f 2c0a 2020 2020 2020  f_evento,.      
+00002020: 2020 2020 2020 2768 5f65 7665 6e74 6f27        'h_evento'
+00002030: 3a20 685f 6576 656e 746f 2c0a 2020 2020  : h_evento,.    
+00002040: 2020 2020 2020 2020 2767 6c6e 5f6f 7269          'gln_ori
+00002050: 6765 6e27 3a20 676c 6e5f 6f72 6967 656e  gen': gln_origen
+00002060: 2c0a 2020 2020 2020 2020 2020 2020 2767  ,.            'g
+00002070: 6c6e 5f64 6573 7469 6e6f 273a 2067 6c6e  ln_destino': gln
+00002080: 5f64 6573 7469 6e6f 2c0a 2020 2020 2020  _destino,.      
+00002090: 2020 2020 2020 276e 5f72 656d 6974 6f27        'n_remito'
+000020a0: 3a20 6e5f 7265 6d69 746f 2c0a 2020 2020  : n_remito,.    
+000020b0: 2020 2020 2020 2020 276e 5f66 6163 7475          'n_factu
+000020c0: 7261 273a 206e 5f66 6163 7475 7261 2c0a  ra': n_factura,.
+000020d0: 2020 2020 2020 2020 2020 2020 2776 656e              'ven
+000020e0: 6369 6d69 656e 746f 273a 2076 656e 6369  cimiento': venci
+000020f0: 6d69 656e 746f 2c0a 2020 2020 2020 2020  miento,.        
+00002100: 2020 2020 2767 7469 6e27 3a20 6774 696e      'gtin': gtin
+00002110: 2c0a 2020 2020 2020 2020 2020 2020 276c  ,.            'l
+00002120: 6f74 6527 3a20 6c6f 7465 2c0a 2020 2020  ote': lote,.    
+00002130: 2020 2020 2020 2020 276e 756d 6572 6f5f          'numero_
+00002140: 7365 7269 616c 273a 206e 756d 6572 6f5f  serial': numero_
+00002150: 7365 7269 616c 2c0a 2020 2020 2020 2020  serial,.        
+00002160: 2020 2020 2769 645f 6f62 7261 5f73 6f63      'id_obra_soc
+00002170: 6961 6c27 3a20 6964 5f6f 6272 615f 736f  ial': id_obra_so
+00002180: 6369 616c 206f 7220 4e6f 6e65 2c0a 2020  cial or None,.  
+00002190: 2020 2020 2020 2020 2020 2769 645f 6576            'id_ev
+000021a0: 656e 746f 273a 2069 645f 6576 656e 746f  ento': id_evento
+000021b0: 2c0a 2020 2020 2020 2020 2020 2020 2763  ,.            'c
+000021c0: 7569 745f 6f72 6967 656e 273a 2063 7569  uit_origen': cui
+000021d0: 745f 6f72 6967 656e 2c0a 2020 2020 2020  t_origen,.      
+000021e0: 2020 2020 2020 2763 7569 745f 6465 7374        'cuit_dest
+000021f0: 696e 6f27 3a20 6375 6974 5f64 6573 7469  ino': cuit_desti
+00002200: 6e6f 2c0a 2020 2020 2020 2020 2020 2020  no,.            
+00002210: 2761 7065 6c6c 6964 6f27 3a20 6170 656c  'apellido': apel
+00002220: 6c69 646f 2c0a 2020 2020 2020 2020 2020  lido,.          
+00002230: 2020 276e 6f6d 6272 6573 273a 206e 6f6d    'nombres': nom
+00002240: 6272 6573 2c0a 2020 2020 2020 2020 2020  bres,.          
+00002250: 2020 2774 6970 6f5f 646f 6375 6d65 6e74    'tipo_document
+00002260: 6f27 3a20 7469 706f 5f64 6f63 756d 656e  o': tipo_documen
+00002270: 746f 2c0a 2020 2020 2020 2020 2020 2020  to,.            
+00002280: 276e 5f64 6f63 756d 656e 746f 273a 206e  'n_documento': n
+00002290: 5f64 6f63 756d 656e 746f 2c0a 2020 2020  _documento,.    
+000022a0: 2020 2020 2020 2020 2773 6578 6f27 3a20          'sexo': 
+000022b0: 7365 786f 2c0a 2020 2020 2020 2020 2020  sexo,.          
+000022c0: 2020 2764 6972 6563 6369 6f6e 273a 2064    'direccion': d
+000022d0: 6972 6563 6369 6f6e 2c0a 2020 2020 2020  ireccion,.      
+000022e0: 2020 2020 2020 276e 756d 6572 6f27 3a20        'numero': 
+000022f0: 6e75 6d65 726f 2c0a 2020 2020 2020 2020  numero,.        
+00002300: 2020 2020 2770 6973 6f27 3a20 7069 736f      'piso': piso
+00002310: 2c0a 2020 2020 2020 2020 2020 2020 2764  ,.            'd
+00002320: 6570 746f 273a 2064 6570 746f 2c0a 2020  epto': depto,.  
+00002330: 2020 2020 2020 2020 2020 276c 6f63 616c            'local
+00002340: 6964 6164 273a 206c 6f63 616c 6964 6164  idad': localidad
+00002350: 2c0a 2020 2020 2020 2020 2020 2020 2770  ,.            'p
+00002360: 726f 7669 6e63 6961 273a 2070 726f 7669  rovincia': provi
+00002370: 6e63 6961 2c0a 2020 2020 2020 2020 2020  ncia,.          
+00002380: 2020 276e 5f70 6f73 7461 6c27 3a20 6e5f    'n_postal': n_
+00002390: 706f 7374 616c 2c0a 2020 2020 2020 2020  postal,.        
+000023a0: 2020 2020 2766 6563 6861 5f6e 6163 696d      'fecha_nacim
+000023b0: 6965 6e74 6f27 3a20 6665 6368 615f 6e61  iento': fecha_na
+000023c0: 6369 6d69 656e 746f 2c0a 2020 2020 2020  cimiento,.      
+000023d0: 2020 2020 2020 2774 656c 6566 6f6e 6f27        'telefono'
+000023e0: 3a20 7465 6c65 666f 6e6f 2c0a 2020 2020  : telefono,.    
+000023f0: 2020 2020 2020 2020 276e 726f 5f61 736f          'nro_aso
+00002400: 6369 6164 6f27 3a20 6e72 6f5f 6173 6f63  ciado': nro_asoc
+00002410: 6961 646f 2c0a 2020 2020 2020 2020 7d0a  iado,.        }.
+00002420: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
+00002430: 6c66 2e63 6c69 656e 742e 7365 6e64 4d65  lf.client.sendMe
+00002440: 6469 6361 6d65 6e74 6f73 280a 2020 2020  dicamentos(.    
+00002450: 2020 2020 2020 2020 6172 6730 3d70 6172          arg0=par
+00002460: 616d 732c 0a20 2020 2020 2020 2020 2020  ams,.           
+00002470: 2061 7267 313d 7573 7561 7269 6f2c 0a20   arg1=usuario,. 
+00002480: 2020 2020 2020 2020 2020 2061 7267 323d             arg2=
+00002490: 7061 7373 776f 7264 2c0a 2020 2020 2020  password,.      
+000024a0: 2020 290a 0a20 2020 2020 2020 2072 6574    )..        ret
+000024b0: 203d 2072 6573 5b27 7265 7475 726e 275d   = res['return']
+000024c0: 0a0a 2020 2020 2020 2020 7365 6c66 2e43  ..        self.C
+000024d0: 6f64 6967 6f54 7261 6e73 6163 6369 6f6e  odigoTransaccion
+000024e0: 203d 2072 6574 5b27 636f 6469 676f 5472   = ret['codigoTr
+000024f0: 616e 7361 6363 696f 6e27 5d0a 2020 2020  ansaccion'].    
+00002500: 2020 2020 7365 6c66 2e5f 5f61 6e61 6c69      self.__anali
+00002510: 7a61 725f 6572 726f 7265 7328 7265 7429  zar_errores(ret)
+00002520: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00002530: 2054 7275 650a 0a20 2020 2040 696e 6963   True..    @inic
+00002540: 6961 6c69 7a61 725f 795f 6361 7074 7572  ializar_y_captur
+00002550: 6172 5f65 7863 6570 6369 6f6e 6573 0a20  ar_excepciones. 
+00002560: 2020 2064 6566 2053 656e 644d 6564 6963     def SendMedic
+00002570: 616d 656e 746f 7346 7261 6363 696f 6e28  amentosFraccion(
+00002580: 0a20 2020 2020 2020 2073 656c 662c 2075  .        self, u
+00002590: 7375 6172 696f 2c20 7061 7373 776f 7264  suario, password
+000025a0: 2c0a 2020 2020 2020 2020 665f 6576 656e  ,.        f_even
+000025b0: 746f 2c20 685f 6576 656e 746f 2c20 676c  to, h_evento, gl
+000025c0: 6e5f 6f72 6967 656e 2c20 676c 6e5f 6465  n_origen, gln_de
+000025d0: 7374 696e 6f2c 0a20 2020 2020 2020 206e  stino,.        n
+000025e0: 5f72 656d 6974 6f2c 206e 5f66 6163 7475  _remito, n_factu
+000025f0: 7261 2c20 7665 6e63 696d 6965 6e74 6f2c  ra, vencimiento,
+00002600: 2067 7469 6e2c 206c 6f74 652c 0a20 2020   gtin, lote,.   
+00002610: 2020 2020 206e 756d 6572 6f5f 7365 7269       numero_seri
+00002620: 616c 2c20 6964 5f6f 6272 615f 736f 6369  al, id_obra_soci
+00002630: 616c 2c20 6964 5f65 7665 6e74 6f2c 0a20  al, id_evento,. 
+00002640: 2020 2020 2020 2063 7569 745f 6f72 6967         cuit_orig
+00002650: 656e 3d27 272c 2063 7569 745f 6465 7374  en='', cuit_dest
+00002660: 696e 6f3d 2727 2c20 6170 656c 6c69 646f  ino='', apellido
+00002670: 3d27 272c 206e 6f6d 6272 6573 3d27 272c  ='', nombres='',
+00002680: 0a20 2020 2020 2020 2074 6970 6f5f 646f  .        tipo_do
+00002690: 6375 6d65 6e74 6f3d 2727 2c20 6e5f 646f  cumento='', n_do
+000026a0: 6375 6d65 6e74 6f3d 2727 2c20 7365 786f  cumento='', sexo
+000026b0: 3d27 272c 0a20 2020 2020 2020 2064 6972  ='',.        dir
+000026c0: 6563 6369 6f6e 3d27 272c 206e 756d 6572  eccion='', numer
+000026d0: 6f3d 2727 2c20 7069 736f 3d27 272c 2064  o='', piso='', d
+000026e0: 6570 746f 3d27 272c 206c 6f63 616c 6964  epto='', localid
+000026f0: 6164 3d27 272c 2070 726f 7669 6e63 6961  ad='', provincia
+00002700: 3d27 272c 0a20 2020 2020 2020 206e 5f70  ='',.        n_p
+00002710: 6f73 7461 6c3d 2727 2c20 6665 6368 615f  ostal='', fecha_
+00002720: 6e61 6369 6d69 656e 746f 3d27 272c 2074  nacimiento='', t
+00002730: 656c 6566 6f6e 6f3d 2727 2c0a 2020 2020  elefono='',.    
+00002740: 2020 2020 6e72 6f5f 6173 6f63 6961 646f      nro_asociado
+00002750: 3d4e 6f6e 652c 2063 616e 7469 6461 643d  =None, cantidad=
+00002760: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00002770: 2020 2020 2022 5265 616c 697a 6120 656c       "Realiza el
+00002780: 2072 6567 6973 7472 6f20 6465 2075 6e61   registro de una
+00002790: 2074 7261 6e73 6163 6369 f36e 2064 6520   transacci.n de 
+000027a0: 6d65 6469 6361 6d65 6e74 6f73 2066 7261  medicamentos fra
+000027b0: 6363 696f 6e61 646f 7322 0a20 2020 2020  ccionados".     
+000027c0: 2020 2023 2063 7265 6f20 6c6f 7320 7061     # creo los pa
+000027d0: 72e1 6d65 7472 6f73 2070 6172 6120 6573  r.metros para es
+000027e0: 7461 206c 6c61 6d61 6461 0a20 2020 2020  ta llamada.     
+000027f0: 2020 2070 6172 616d 7320 3d20 7b0a 2020     params = {.  
+00002800: 2020 2020 2020 2020 2020 2766 5f65 7665            'f_eve
+00002810: 6e74 6f27 3a20 665f 6576 656e 746f 2c0a  nto': f_evento,.
+00002820: 2020 2020 2020 2020 2020 2020 2768 5f65              'h_e
+00002830: 7665 6e74 6f27 3a20 685f 6576 656e 746f  vento': h_evento
+00002840: 2c0a 2020 2020 2020 2020 2020 2020 2767  ,.            'g
+00002850: 6c6e 5f6f 7269 6765 6e27 3a20 676c 6e5f  ln_origen': gln_
+00002860: 6f72 6967 656e 2c0a 2020 2020 2020 2020  origen,.        
+00002870: 2020 2020 2767 6c6e 5f64 6573 7469 6e6f      'gln_destino
+00002880: 273a 2067 6c6e 5f64 6573 7469 6e6f 2c0a  ': gln_destino,.
+00002890: 2020 2020 2020 2020 2020 2020 276e 5f72              'n_r
+000028a0: 656d 6974 6f27 3a20 6e5f 7265 6d69 746f  emito': n_remito
+000028b0: 2c0a 2020 2020 2020 2020 2020 2020 276e  ,.            'n
+000028c0: 5f66 6163 7475 7261 273a 206e 5f66 6163  _factura': n_fac
+000028d0: 7475 7261 2c0a 2020 2020 2020 2020 2020  tura,.          
+000028e0: 2020 2776 656e 6369 6d69 656e 746f 273a    'vencimiento':
+000028f0: 2076 656e 6369 6d69 656e 746f 2c0a 2020   vencimiento,.  
+00002900: 2020 2020 2020 2020 2020 2767 7469 6e27            'gtin'
+00002910: 3a20 6774 696e 2c0a 2020 2020 2020 2020  : gtin,.        
+00002920: 2020 2020 276c 6f74 6527 3a20 6c6f 7465      'lote': lote
+00002930: 2c0a 2020 2020 2020 2020 2020 2020 276e  ,.            'n
+00002940: 756d 6572 6f5f 7365 7269 616c 273a 206e  umero_serial': n
+00002950: 756d 6572 6f5f 7365 7269 616c 2c0a 2020  umero_serial,.  
+00002960: 2020 2020 2020 2020 2020 2769 645f 6f62            'id_ob
+00002970: 7261 5f73 6f63 6961 6c27 3a20 6964 5f6f  ra_social': id_o
+00002980: 6272 615f 736f 6369 616c 206f 7220 4e6f  bra_social or No
+00002990: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+000029a0: 2769 645f 6576 656e 746f 273a 2069 645f  'id_evento': id_
+000029b0: 6576 656e 746f 2c0a 2020 2020 2020 2020  evento,.        
+000029c0: 2020 2020 2763 7569 745f 6f72 6967 656e      'cuit_origen
+000029d0: 273a 2063 7569 745f 6f72 6967 656e 2c0a  ': cuit_origen,.
+000029e0: 2020 2020 2020 2020 2020 2020 2763 7569              'cui
+000029f0: 745f 6465 7374 696e 6f27 3a20 6375 6974  t_destino': cuit
+00002a00: 5f64 6573 7469 6e6f 2c0a 2020 2020 2020  _destino,.      
+00002a10: 2020 2020 2020 2761 7065 6c6c 6964 6f27        'apellido'
+00002a20: 3a20 6170 656c 6c69 646f 2c0a 2020 2020  : apellido,.    
+00002a30: 2020 2020 2020 2020 276e 6f6d 6272 6573          'nombres
+00002a40: 273a 206e 6f6d 6272 6573 2c0a 2020 2020  ': nombres,.    
+00002a50: 2020 2020 2020 2020 2774 6970 6f5f 646f          'tipo_do
+00002a60: 6375 6d65 6e74 6f27 3a20 7469 706f 5f64  cumento': tipo_d
+00002a70: 6f63 756d 656e 746f 2c0a 2020 2020 2020  ocumento,.      
+00002a80: 2020 2020 2020 276e 5f64 6f63 756d 656e        'n_documen
+00002a90: 746f 273a 206e 5f64 6f63 756d 656e 746f  to': n_documento
+00002aa0: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
+00002ab0: 6578 6f27 3a20 7365 786f 2c0a 2020 2020  exo': sexo,.    
+00002ac0: 2020 2020 2020 2020 2764 6972 6563 6369          'direcci
+00002ad0: 6f6e 273a 2064 6972 6563 6369 6f6e 2c0a  on': direccion,.
+00002ae0: 2020 2020 2020 2020 2020 2020 276e 756d              'num
+00002af0: 6572 6f27 3a20 6e75 6d65 726f 2c0a 2020  ero': numero,.  
+00002b00: 2020 2020 2020 2020 2020 2770 6973 6f27            'piso'
+00002b10: 3a20 7069 736f 2c0a 2020 2020 2020 2020  : piso,.        
+00002b20: 2020 2020 2764 6570 746f 273a 2064 6570      'depto': dep
+00002b30: 746f 2c0a 2020 2020 2020 2020 2020 2020  to,.            
+00002b40: 276c 6f63 616c 6964 6164 273a 206c 6f63  'localidad': loc
+00002b50: 616c 6964 6164 2c0a 2020 2020 2020 2020  alidad,.        
+00002b60: 2020 2020 2770 726f 7669 6e63 6961 273a      'provincia':
+00002b70: 2070 726f 7669 6e63 6961 2c0a 2020 2020   provincia,.    
+00002b80: 2020 2020 2020 2020 276e 5f70 6f73 7461          'n_posta
+00002b90: 6c27 3a20 6e5f 706f 7374 616c 2c0a 2020  l': n_postal,.  
+00002ba0: 2020 2020 2020 2020 2020 2766 6563 6861            'fecha
+00002bb0: 5f6e 6163 696d 6965 6e74 6f27 3a20 6665  _nacimiento': fe
+00002bc0: 6368 615f 6e61 6369 6d69 656e 746f 2c0a  cha_nacimiento,.
+00002bd0: 2020 2020 2020 2020 2020 2020 2774 656c              'tel
+00002be0: 6566 6f6e 6f27 3a20 7465 6c65 666f 6e6f  efono': telefono
+00002bf0: 2c0a 2020 2020 2020 2020 2020 2020 276e  ,.            'n
+00002c00: 726f 5f61 736f 6369 6164 6f27 3a20 6e72  ro_asociado': nr
+00002c10: 6f5f 6173 6f63 6961 646f 2c0a 2020 2020  o_asociado,.    
+00002c20: 2020 2020 2020 2020 2763 616e 7469 6461          'cantida
+00002c30: 6427 3a20 6361 6e74 6964 6164 2c0a 2020  d': cantidad,.  
+00002c40: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00002c50: 7265 7320 3d20 7365 6c66 2e63 6c69 656e  res = self.clien
+00002c60: 742e 7365 6e64 4d65 6469 6361 6d65 6e74  t.sendMedicament
+00002c70: 6f73 4672 6163 6369 6f6e 280a 2020 2020  osFraccion(.    
+00002c80: 2020 2020 2020 2020 6172 6730 3d70 6172          arg0=par
+00002c90: 616d 732c 0a20 2020 2020 2020 2020 2020  ams,.           
+00002ca0: 2061 7267 313d 7573 7561 7269 6f2c 0a20   arg1=usuario,. 
+00002cb0: 2020 2020 2020 2020 2020 2061 7267 323d             arg2=
+00002cc0: 7061 7373 776f 7264 2c0a 2020 2020 2020  password,.      
+00002cd0: 2020 290a 0a20 2020 2020 2020 2072 6574    )..        ret
+00002ce0: 203d 2072 6573 5b27 7265 7475 726e 275d   = res['return']
+00002cf0: 0a0a 2020 2020 2020 2020 7365 6c66 2e43  ..        self.C
+00002d00: 6f64 6967 6f54 7261 6e73 6163 6369 6f6e  odigoTransaccion
+00002d10: 203d 2072 6574 5b27 636f 6469 676f 5472   = ret['codigoTr
+00002d20: 616e 7361 6363 696f 6e27 5d0a 2020 2020  ansaccion'].    
+00002d30: 2020 2020 7365 6c66 2e5f 5f61 6e61 6c69      self.__anali
+00002d40: 7a61 725f 6572 726f 7265 7328 7265 7429  zar_errores(ret)
+00002d50: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00002d60: 2054 7275 650a 0a20 2020 2040 696e 6963   True..    @inic
+00002d70: 6961 6c69 7a61 725f 795f 6361 7074 7572  ializar_y_captur
+00002d80: 6172 5f65 7863 6570 6369 6f6e 6573 0a20  ar_excepciones. 
+00002d90: 2020 2064 6566 2053 656e 644d 6564 6963     def SendMedic
+00002da0: 616d 656e 746f 7344 4853 6572 6965 280a  amentosDHSerie(.
+00002db0: 2020 2020 2020 2020 7365 6c66 2c20 7573          self, us
+00002dc0: 7561 7269 6f2c 2070 6173 7377 6f72 642c  uario, password,
+00002dd0: 0a20 2020 2020 2020 2066 5f65 7665 6e74  .        f_event
+00002de0: 6f2c 2068 5f65 7665 6e74 6f2c 2067 6c6e  o, h_evento, gln
+00002df0: 5f6f 7269 6765 6e2c 2067 6c6e 5f64 6573  _origen, gln_des
+00002e00: 7469 6e6f 2c0a 2020 2020 2020 2020 6e5f  tino,.        n_
+00002e10: 7265 6d69 746f 2c20 6e5f 6661 6374 7572  remito, n_factur
+00002e20: 612c 2076 656e 6369 6d69 656e 746f 2c20  a, vencimiento, 
+00002e30: 6774 696e 2c20 6c6f 7465 2c0a 2020 2020  gtin, lote,.    
+00002e40: 2020 2020 6465 7364 655f 6e75 6d65 726f      desde_numero
+00002e50: 5f73 6572 6961 6c2c 2068 6173 7461 5f6e  _serial, hasta_n
+00002e60: 756d 6572 6f5f 7365 7269 616c 2c0a 2020  umero_serial,.  
+00002e70: 2020 2020 2020 6964 5f6f 6272 615f 736f        id_obra_so
+00002e80: 6369 616c 2c20 6964 5f65 7665 6e74 6f2c  cial, id_evento,
+00002e90: 0a20 2020 2020 2020 2063 7569 745f 6f72  .        cuit_or
+00002ea0: 6967 656e 3d27 272c 2063 7569 745f 6465  igen='', cuit_de
+00002eb0: 7374 696e 6f3d 2727 2c20 6170 656c 6c69  stino='', apelli
+00002ec0: 646f 3d27 272c 206e 6f6d 6272 6573 3d27  do='', nombres='
+00002ed0: 272c 0a20 2020 2020 2020 2074 6970 6f5f  ',.        tipo_
+00002ee0: 646f 6375 6d65 6e74 6f3d 2727 2c20 6e5f  documento='', n_
+00002ef0: 646f 6375 6d65 6e74 6f3d 2727 2c20 7365  documento='', se
+00002f00: 786f 3d27 272c 0a20 2020 2020 2020 2064  xo='',.        d
+00002f10: 6972 6563 6369 6f6e 3d27 272c 206e 756d  ireccion='', num
+00002f20: 6572 6f3d 2727 2c20 7069 736f 3d27 272c  ero='', piso='',
+00002f30: 2064 6570 746f 3d27 272c 206c 6f63 616c   depto='', local
+00002f40: 6964 6164 3d27 272c 2070 726f 7669 6e63  idad='', provinc
+00002f50: 6961 3d27 272c 0a20 2020 2020 2020 206e  ia='',.        n
+00002f60: 5f70 6f73 7461 6c3d 2727 2c20 6665 6368  _postal='', fech
+00002f70: 615f 6e61 6369 6d69 656e 746f 3d27 272c  a_nacimiento='',
+00002f80: 2074 656c 6566 6f6e 6f3d 2727 2c0a 2020   telefono='',.  
+00002f90: 2020 2020 2020 6e72 6f5f 6173 6f63 6961        nro_asocia
+00002fa0: 646f 3d4e 6f6e 652c 0a20 2020 2029 3a0a  do=None,.    ):.
+00002fb0: 2020 2020 2020 2020 2245 6e76 ed61 2075          "Env.a u
+00002fc0: 6e20 6c6f 7465 2064 6520 6d65 6469 6361  n lote de medica
+00002fd0: 6d65 6e74 6f73 2069 6e66 6f72 6d61 6e64  mentos informand
+00002fe0: 6f20 656c 2064 6573 6465 2d68 6173 7461  o el desde-hasta
+00002ff0: 206e fa6d 6572 6f20 6465 205c 0a20 2020   n.mero de \.   
+00003000: 2020 2020 2020 2020 2073 6572 6965 220a           serie".
+00003010: 2020 2020 2020 2020 2320 6372 656f 206c          # creo l
+00003020: 6f73 2070 6172 e16d 6574 726f 7320 7061  os par.metros pa
+00003030: 7261 2065 7374 6120 6c6c 616d 6164 610a  ra esta llamada.
+00003040: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
+00003050: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
+00003060: 665f 6576 656e 746f 273a 2066 5f65 7665  f_evento': f_eve
+00003070: 6e74 6f2c 0a20 2020 2020 2020 2020 2020  nto,.           
+00003080: 2027 685f 6576 656e 746f 273a 2068 5f65   'h_evento': h_e
+00003090: 7665 6e74 6f2c 0a20 2020 2020 2020 2020  vento,.         
+000030a0: 2020 2027 676c 6e5f 6f72 6967 656e 273a     'gln_origen':
+000030b0: 2067 6c6e 5f6f 7269 6765 6e2c 0a20 2020   gln_origen,.   
+000030c0: 2020 2020 2020 2020 2027 676c 6e5f 6465           'gln_de
+000030d0: 7374 696e 6f27 3a20 676c 6e5f 6465 7374  stino': gln_dest
+000030e0: 696e 6f2c 0a20 2020 2020 2020 2020 2020  ino,.           
+000030f0: 2027 6e5f 7265 6d69 746f 273a 206e 5f72   'n_remito': n_r
+00003100: 656d 6974 6f2c 0a20 2020 2020 2020 2020  emito,.         
+00003110: 2020 2027 6e5f 6661 6374 7572 6127 3a20     'n_factura': 
+00003120: 6e5f 6661 6374 7572 612c 0a20 2020 2020  n_factura,.     
+00003130: 2020 2020 2020 2027 7665 6e63 696d 6965         'vencimie
+00003140: 6e74 6f27 3a20 7665 6e63 696d 6965 6e74  nto': vencimient
+00003150: 6f2c 0a20 2020 2020 2020 2020 2020 2027  o,.            '
+00003160: 6774 696e 273a 2067 7469 6e2c 0a20 2020  gtin': gtin,.   
+00003170: 2020 2020 2020 2020 2027 6c6f 7465 273a           'lote':
+00003180: 206c 6f74 652c 0a20 2020 2020 2020 2020   lote,.         
+00003190: 2020 2027 6465 7364 655f 6e75 6d65 726f     'desde_numero
+000031a0: 5f73 6572 6961 6c27 3a20 6465 7364 655f  _serial': desde_
+000031b0: 6e75 6d65 726f 5f73 6572 6961 6c2c 0a20  numero_serial,. 
+000031c0: 2020 2020 2020 2020 2020 2027 6861 7374             'hast
+000031d0: 615f 6e75 6d65 726f 5f73 6572 6961 6c27  a_numero_serial'
+000031e0: 3a20 6861 7374 615f 6e75 6d65 726f 5f73  : hasta_numero_s
+000031f0: 6572 6961 6c2c 0a20 2020 2020 2020 2020  erial,.         
+00003200: 2020 2027 6964 5f6f 6272 615f 736f 6369     'id_obra_soci
+00003210: 616c 273a 2069 645f 6f62 7261 5f73 6f63  al': id_obra_soc
+00003220: 6961 6c20 6f72 204e 6f6e 652c 0a20 2020  ial or None,.   
+00003230: 2020 2020 2020 2020 2027 6964 5f65 7665           'id_eve
+00003240: 6e74 6f27 3a20 6964 5f65 7665 6e74 6f2c  nto': id_evento,
+00003250: 0a20 2020 2020 2020 2020 2020 2027 6375  .            'cu
+00003260: 6974 5f6f 7269 6765 6e27 3a20 6375 6974  it_origen': cuit
+00003270: 5f6f 7269 6765 6e2c 0a20 2020 2020 2020  _origen,.       
+00003280: 2020 2020 2027 6375 6974 5f64 6573 7469       'cuit_desti
+00003290: 6e6f 273a 2063 7569 745f 6465 7374 696e  no': cuit_destin
+000032a0: 6f2c 0a20 2020 2020 2020 2020 2020 2027  o,.            '
+000032b0: 6170 656c 6c69 646f 273a 2061 7065 6c6c  apellido': apell
+000032c0: 6964 6f2c 0a20 2020 2020 2020 2020 2020  ido,.           
+000032d0: 2027 6e6f 6d62 7265 7327 3a20 6e6f 6d62   'nombres': nomb
+000032e0: 7265 732c 0a20 2020 2020 2020 2020 2020  res,.           
+000032f0: 2027 7469 706f 5f64 6f63 756d 656e 746f   'tipo_documento
+00003300: 273a 2074 6970 6f5f 646f 6375 6d65 6e74  ': tipo_document
+00003310: 6f2c 0a20 2020 2020 2020 2020 2020 2027  o,.            '
+00003320: 6e5f 646f 6375 6d65 6e74 6f27 3a20 6e5f  n_documento': n_
+00003330: 646f 6375 6d65 6e74 6f2c 0a20 2020 2020  documento,.     
+00003340: 2020 2020 2020 2027 7365 786f 273a 2073         'sexo': s
+00003350: 6578 6f2c 0a20 2020 2020 2020 2020 2020  exo,.           
+00003360: 2027 6469 7265 6363 696f 6e27 3a20 6469   'direccion': di
+00003370: 7265 6363 696f 6e2c 0a20 2020 2020 2020  reccion,.       
+00003380: 2020 2020 2027 6e75 6d65 726f 273a 206e       'numero': n
+00003390: 756d 6572 6f2c 0a20 2020 2020 2020 2020  umero,.         
+000033a0: 2020 2027 7069 736f 273a 2070 6973 6f2c     'piso': piso,
+000033b0: 0a20 2020 2020 2020 2020 2020 2027 6465  .            'de
+000033c0: 7074 6f27 3a20 6465 7074 6f2c 0a20 2020  pto': depto,.   
+000033d0: 2020 2020 2020 2020 2027 6c6f 6361 6c69           'locali
+000033e0: 6461 6427 3a20 6c6f 6361 6c69 6461 642c  dad': localidad,
+000033f0: 0a20 2020 2020 2020 2020 2020 2027 7072  .            'pr
+00003400: 6f76 696e 6369 6127 3a20 7072 6f76 696e  ovincia': provin
+00003410: 6369 612c 0a20 2020 2020 2020 2020 2020  cia,.           
+00003420: 2027 6e5f 706f 7374 616c 273a 206e 5f70   'n_postal': n_p
+00003430: 6f73 7461 6c2c 0a20 2020 2020 2020 2020  ostal,.         
+00003440: 2020 2027 6665 6368 615f 6e61 6369 6d69     'fecha_nacimi
+00003450: 656e 746f 273a 2066 6563 6861 5f6e 6163  ento': fecha_nac
+00003460: 696d 6965 6e74 6f2c 0a20 2020 2020 2020  imiento,.       
+00003470: 2020 2020 2027 7465 6c65 666f 6e6f 273a       'telefono':
+00003480: 2074 656c 6566 6f6e 6f2c 0a20 2020 2020   telefono,.     
+00003490: 2020 2020 2020 2027 6e72 6f5f 6173 6f63         'nro_asoc
+000034a0: 6961 646f 273a 206e 726f 5f61 736f 6369  iado': nro_asoci
+000034b0: 6164 6f2c 0a20 2020 2020 2020 207d 0a20  ado,.        }. 
+000034c0: 2020 2020 2020 2072 6573 203d 2073 656c         res = sel
+000034d0: 662e 636c 6965 6e74 2e73 656e 644d 6564  f.client.sendMed
+000034e0: 6963 616d 656e 746f 7344 4853 6572 6965  icamentosDHSerie
+000034f0: 280a 2020 2020 2020 2020 2020 2020 6172  (.            ar
+00003500: 6730 3d70 6172 616d 732c 0a20 2020 2020  g0=params,.     
+00003510: 2020 2020 2020 2061 7267 313d 7573 7561         arg1=usua
+00003520: 7269 6f2c 0a20 2020 2020 2020 2020 2020  rio,.           
+00003530: 2061 7267 323d 7061 7373 776f 7264 2c0a   arg2=password,.
+00003540: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00003550: 2020 2072 6574 203d 2072 6573 5b27 7265     ret = res['re
+00003560: 7475 726e 275d 0a0a 2020 2020 2020 2020  turn']..        
+00003570: 7365 6c66 2e43 6f64 6967 6f54 7261 6e73  self.CodigoTrans
+00003580: 6163 6369 6f6e 203d 2072 6574 5b27 636f  accion = ret['co
+00003590: 6469 676f 5472 616e 7361 6363 696f 6e27  digoTransaccion'
+000035a0: 5d0a 2020 2020 2020 2020 7365 6c66 2e5f  ].        self._
+000035b0: 5f61 6e61 6c69 7a61 725f 6572 726f 7265  _analizar_errore
+000035c0: 7328 7265 7429 0a0a 2020 2020 2020 2020  s(ret)..        
+000035d0: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+000035e0: 2040 696e 6963 6961 6c69 7a61 725f 795f   @inicializar_y_
+000035f0: 6361 7074 7572 6172 5f65 7863 6570 6369  capturar_excepci
+00003600: 6f6e 6573 0a20 2020 2064 6566 2053 656e  ones.    def Sen
+00003610: 6443 616e 6365 6c61 6354 7261 6e73 6163  dCancelacTransac
+00003620: 6328 7365 6c66 2c20 7573 7561 7269 6f2c  c(self, usuario,
+00003630: 2070 6173 7377 6f72 642c 2063 6f64 6967   password, codig
+00003640: 6f5f 7472 616e 7361 6363 696f 6e29 3a0a  o_transaccion):.
+00003650: 2020 2020 2020 2020 2220 5265 616c 697a          " Realiz
+00003660: 6120 6c61 2063 616e 6365 6c61 6369 f36e  a la cancelaci.n
+00003670: 2064 6520 756e 6120 7472 616e 7361 6363   de una transacc
+00003680: 69f3 6e22 0a20 2020 2020 2020 2072 6573  i.n".        res
+00003690: 203d 2073 656c 662e 636c 6965 6e74 2e73   = self.client.s
+000036a0: 656e 6443 616e 6365 6c61 6354 7261 6e73  endCancelacTrans
+000036b0: 6163 6328 0a20 2020 2020 2020 2020 2020  acc(.           
+000036c0: 2061 7267 303d 636f 6469 676f 5f74 7261   arg0=codigo_tra
+000036d0: 6e73 6163 6369 6f6e 2c0a 2020 2020 2020  nsaccion,.      
+000036e0: 2020 2020 2020 6172 6731 3d75 7375 6172        arg1=usuar
+000036f0: 696f 2c0a 2020 2020 2020 2020 2020 2020  io,.            
+00003700: 6172 6732 3d70 6173 7377 6f72 642c 0a20  arg2=password,. 
+00003710: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00003720: 2020 7265 7420 3d20 7265 735b 2772 6574    ret = res['ret
+00003730: 7572 6e27 5d0a 0a20 2020 2020 2020 2073  urn']..        s
+00003740: 656c 662e 436f 6469 676f 5472 616e 7361  elf.CodigoTransa
+00003750: 6363 696f 6e20 3d20 7265 742e 6765 7428  ccion = ret.get(
+00003760: 2763 6f64 6967 6f54 7261 6e73 6163 6369  'codigoTransacci
+00003770: 6f6e 2729 0a20 2020 2020 2020 2073 656c  on').        sel
+00003780: 662e 5f5f 616e 616c 697a 6172 5f65 7272  f.__analizar_err
+00003790: 6f72 6573 2872 6574 290a 0a20 2020 2020  ores(ret)..     
+000037a0: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
+000037b0: 2020 2020 4069 6e69 6369 616c 697a 6172      @inicializar
+000037c0: 5f79 5f63 6170 7475 7261 725f 6578 6365  _y_capturar_exce
+000037d0: 7063 696f 6e65 730a 2020 2020 6465 6620  pciones.    def 
+000037e0: 5365 6e64 4361 6e63 656c 6163 5472 616e  SendCancelacTran
+000037f0: 7361 6363 5061 7263 6961 6c28 0a20 2020  saccParcial(.   
+00003800: 2020 2020 2073 656c 662c 2075 7375 6172       self, usuar
+00003810: 696f 2c20 7061 7373 776f 7264 2c20 636f  io, password, co
+00003820: 6469 676f 5f74 7261 6e73 6163 6369 6f6e  digo_transaccion
+00003830: 2c0a 2020 2020 2020 2020 6774 696e 5f6d  ,.        gtin_m
+00003840: 6564 6963 616d 656e 746f 3d4e 6f6e 652c  edicamento=None,
+00003850: 206e 756d 6572 6f5f 7365 7269 616c 3d4e   numero_serial=N
+00003860: 6f6e 650a 2020 2020 293a 0a20 2020 2020  one.    ):.     
+00003870: 2020 2022 2052 6561 6c69 7a61 206c 6120     " Realiza la 
+00003880: 6361 6e63 656c 6163 69f3 6e20 7061 7263  cancelaci.n parc
+00003890: 6961 6c20 6465 2075 6e61 2074 7261 6e73  ial de una trans
+000038a0: 6163 6369 f36e 220a 2020 2020 2020 2020  acci.n".        
+000038b0: 7265 7320 3d20 7365 6c66 2e63 6c69 656e  res = self.clien
+000038c0: 742e 7365 6e64 4361 6e63 656c 6163 5472  t.sendCancelacTr
+000038d0: 616e 7361 6363 5061 7263 6961 6c28 0a20  ansaccParcial(. 
+000038e0: 2020 2020 2020 2020 2020 2061 7267 303d             arg0=
+000038f0: 636f 6469 676f 5f74 7261 6e73 6163 6369  codigo_transacci
+00003900: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+00003910: 6172 6731 3d75 7375 6172 696f 2c0a 2020  arg1=usuario,.  
+00003920: 2020 2020 2020 2020 2020 6172 6732 3d70            arg2=p
+00003930: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
+00003940: 2020 2020 2061 7267 333d 6774 696e 5f6d       arg3=gtin_m
+00003950: 6564 6963 616d 656e 746f 2c0a 2020 2020  edicamento,.    
+00003960: 2020 2020 2020 2020 6172 6734 3d6e 756d          arg4=num
+00003970: 6572 6f5f 7365 7269 616c 2c0a 2020 2020  ero_serial,.    
+00003980: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
+00003990: 7420 3d20 7265 735b 2772 6574 7572 6e27  t = res['return'
+000039a0: 5d0a 2020 2020 2020 2020 7365 6c66 2e43  ].        self.C
+000039b0: 6f64 6967 6f54 7261 6e73 6163 6369 6f6e  odigoTransaccion
+000039c0: 203d 2072 6574 2e67 6574 2827 636f 6469   = ret.get('codi
+000039d0: 676f 5472 616e 7361 6363 696f 6e27 290a  goTransaccion').
+000039e0: 2020 2020 2020 2020 7365 6c66 2e5f 5f61          self.__a
+000039f0: 6e61 6c69 7a61 725f 6572 726f 7265 7328  nalizar_errores(
+00003a00: 7265 7429 0a20 2020 2020 2020 2072 6574  ret).        ret
+00003a10: 7572 6e20 5472 7565 0a0a 2020 2020 4069  urn True..    @i
+00003a20: 6e69 6369 616c 697a 6172 5f79 5f63 6170  nicializar_y_cap
+00003a30: 7475 7261 725f 6578 6365 7063 696f 6e65  turar_excepcione
+00003a40: 730a 2020 2020 6465 6620 5365 6e64 436f  s.    def SendCo
+00003a50: 6e66 6972 6d61 5472 616e 7361 6363 280a  nfirmaTransacc(.
+00003a60: 2020 2020 2020 2020 7365 6c66 2c20 7573          self, us
+00003a70: 7561 7269 6f2c 2070 6173 7377 6f72 642c  uario, password,
+00003a80: 2070 5f69 6473 5f74 7261 6e73 6163 2c20   p_ids_transac, 
+00003a90: 665f 6f70 6572 6163 696f 6e0a 2020 2020  f_operacion.    
+00003aa0: 293a 0a20 2020 2020 2020 2022 436f 6e66  ):.        "Conf
+00003ab0: 6972 6d61 206c 6120 7265 6365 7063 69f3  irma la recepci.
+00003ac0: 6e20 6465 2075 6e20 6d65 6469 6361 6d65  n de un medicame
+00003ad0: 6e74 6f22 0a20 2020 2020 2020 2072 6573  nto".        res
+00003ae0: 203d 2073 656c 662e 636c 6965 6e74 2e73   = self.client.s
+00003af0: 656e 6443 6f6e 6669 726d 6154 7261 6e73  endConfirmaTrans
+00003b00: 6163 6328 0a20 2020 2020 2020 2020 2020  acc(.           
+00003b10: 2061 7267 303d 7573 7561 7269 6f2c 0a20   arg0=usuario,. 
+00003b20: 2020 2020 2020 2020 2020 2061 7267 313d             arg1=
+00003b30: 7061 7373 776f 7264 2c0a 2020 2020 2020  password,.      
+00003b40: 2020 2020 2020 6172 6732 3d7b 2770 5f69        arg2={'p_i
+00003b50: 6473 5f74 7261 6e73 6163 273a 2070 5f69  ds_transac': p_i
+00003b60: 6473 5f74 7261 6e73 6163 2c20 2766 5f6f  ds_transac, 'f_o
+00003b70: 7065 7261 6369 6f6e 273a 2066 5f6f 7065  peracion': f_ope
+00003b80: 7261 6369 6f6e 7d2c 0a20 2020 2020 2020  racion},.       
+00003b90: 2029 0a20 2020 2020 2020 2072 6574 203d   ).        ret =
+00003ba0: 2072 6573 5b27 7265 7475 726e 275d 0a20   res['return']. 
+00003bb0: 2020 2020 2020 2073 656c 662e 436f 6469         self.Codi
+00003bc0: 676f 5472 616e 7361 6363 696f 6e20 3d20  goTransaccion = 
+00003bd0: 7265 742e 6765 7428 2769 645f 7472 616e  ret.get('id_tran
+00003be0: 7361 635f 6173 6f63 6961 6461 2729 0a20  sac_asociada'). 
+00003bf0: 2020 2020 2020 2073 656c 662e 5f5f 616e         self.__an
+00003c00: 616c 697a 6172 5f65 7272 6f72 6573 2872  alizar_errores(r
+00003c10: 6574 290a 2020 2020 2020 2020 7265 7475  et).        retu
+00003c20: 726e 2054 7275 650a 0a20 2020 2040 696e  rn True..    @in
+00003c30: 6963 6961 6c69 7a61 725f 795f 6361 7074  icializar_y_capt
+00003c40: 7572 6172 5f65 7863 6570 6369 6f6e 6573  urar_excepciones
+00003c50: 0a20 2020 2064 6566 2053 656e 6441 6c65  .    def SendAle
+00003c60: 7274 6154 7261 6e73 6163 6328 7365 6c66  rtaTransacc(self
+00003c70: 2c20 7573 7561 7269 6f2c 2070 6173 7377  , usuario, passw
+00003c80: 6f72 642c 2070 5f69 6473 5f74 7261 6e73  ord, p_ids_trans
+00003c90: 6163 5f77 7329 3a0a 2020 2020 2020 2020  ac_ws):.        
+00003ca0: 2241 6c65 7274 6120 756e 206d 6564 6963  "Alerta un medic
+00003cb0: 616d 656e 746f 2c20 6163 6369 f36e 2063  amento, acci.n c
+00003cc0: 6f6e 7472 6172 6961 2061 2093 636f 6e66  ontraria a .conf
+00003cd0: 6972 6d61 7220 6c61 205c 0a20 2020 2020  irmar la \.     
+00003ce0: 2020 2020 2020 2074 7261 6e73 6163 6369         transacci
+00003cf0: f36e 942e 220a 2020 2020 2020 2020 7265  .n..".        re
+00003d00: 7320 3d20 7365 6c66 2e63 6c69 656e 742e  s = self.client.
+00003d10: 7365 6e64 416c 6572 7461 5472 616e 7361  sendAlertaTransa
+00003d20: 6363 280a 2020 2020 2020 2020 2020 2020  cc(.            
+00003d30: 6172 6730 3d75 7375 6172 696f 2c0a 2020  arg0=usuario,.  
+00003d40: 2020 2020 2020 2020 2020 6172 6731 3d70            arg1=p
+00003d50: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
+00003d60: 2020 2020 2061 7267 323d 705f 6964 735f       arg2=p_ids_
+00003d70: 7472 616e 7361 635f 7773 2c0a 2020 2020  transac_ws,.    
+00003d80: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
+00003d90: 7420 3d20 7265 735b 2772 6574 7572 6e27  t = res['return'
+00003da0: 5d0a 2020 2020 2020 2020 7365 6c66 2e43  ].        self.C
+00003db0: 6f64 6967 6f54 7261 6e73 6163 6369 6f6e  odigoTransaccion
+00003dc0: 203d 2072 6574 2e67 6574 2827 6964 5f74   = ret.get('id_t
+00003dd0: 7261 6e73 6163 5f61 736f 6369 6164 6127  ransac_asociada'
+00003de0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+00003df0: 5f61 6e61 6c69 7a61 725f 6572 726f 7265  _analizar_errore
+00003e00: 7328 7265 7429 0a20 2020 2020 2020 2072  s(ret).        r
+00003e10: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
+00003e20: 4069 6e69 6369 616c 697a 6172 5f79 5f63  @inicializar_y_c
+00003e30: 6170 7475 7261 725f 6578 6365 7063 696f  apturar_excepcio
+00003e40: 6e65 730a 2020 2020 6465 6620 4765 7454  nes.    def GetT
+00003e50: 7261 6e73 6163 6369 6f6e 6573 4e6f 436f  ransaccionesNoCo
+00003e60: 6e66 6972 6d61 6461 7328 0a20 2020 2020  nfirmadas(.     
+00003e70: 2020 2073 656c 662c 2075 7375 6172 696f     self, usuario
+00003e80: 2c20 7061 7373 776f 7264 2c0a 2020 2020  , password,.    
+00003e90: 2020 2020 705f 6964 5f74 7261 6e73 6163      p_id_transac
+00003ea0: 6369 6f6e 5f67 6c6f 6261 6c3d 4e6f 6e65  cion_global=None
+00003eb0: 2c20 6964 5f61 6765 6e74 655f 696e 666f  , id_agente_info
+00003ec0: 726d 6164 6f72 3d4e 6f6e 652c 0a20 2020  rmador=None,.   
+00003ed0: 2020 2020 2069 645f 6167 656e 7465 5f6f       id_agente_o
+00003ee0: 7269 6765 6e3d 4e6f 6e65 2c20 6964 5f61  rigen=None, id_a
+00003ef0: 6765 6e74 655f 6465 7374 696e 6f3d 4e6f  gente_destino=No
+00003f00: 6e65 2c0a 2020 2020 2020 2020 6964 5f6d  ne,.        id_m
+00003f10: 6564 6963 616d 656e 746f 3d4e 6f6e 652c  edicamento=None,
+00003f20: 2069 645f 6576 656e 746f 3d4e 6f6e 652c   id_evento=None,
+00003f30: 0a20 2020 2020 2020 2066 6563 6861 5f64  .        fecha_d
+00003f40: 6573 6465 5f6f 703d 4e6f 6e65 2c20 6665  esde_op=None, fe
+00003f50: 6368 615f 6861 7374 615f 6f70 3d4e 6f6e  cha_hasta_op=Non
+00003f60: 652c 0a20 2020 2020 2020 2066 6563 6861  e,.        fecha
+00003f70: 5f64 6573 6465 5f74 3d4e 6f6e 652c 2066  _desde_t=None, f
+00003f80: 6563 6861 5f68 6173 7461 5f74 3d4e 6f6e  echa_hasta_t=Non
+00003f90: 652c 0a20 2020 2020 2020 2066 6563 6861  e,.        fecha
+00003fa0: 5f64 6573 6465 5f76 3d4e 6f6e 652c 2066  _desde_v=None, f
+00003fb0: 6563 6861 5f68 6173 7461 5f76 3d4e 6f6e  echa_hasta_v=Non
+00003fc0: 652c 0a20 2020 2020 2020 206e 5f72 656d  e,.        n_rem
+00003fd0: 6974 6f3d 4e6f 6e65 2c20 6e5f 6661 6374  ito=None, n_fact
+00003fe0: 7572 613d 4e6f 6e65 2c0a 2020 2020 2020  ura=None,.      
+00003ff0: 2020 6573 7461 646f 3d4e 6f6e 652c 206c    estado=None, l
+00004000: 6f74 653d 4e6f 6e65 2c20 6e75 6d65 726f  ote=None, numero
+00004010: 5f73 6572 6961 6c3d 4e6f 6e65 2c0a 2020  _serial=None,.  
+00004020: 2020 293a 0a20 2020 2020 2020 2022 5472    ):.        "Tr
+00004030: 6165 2075 6e20 6c69 7374 6164 6f20 6465  ae un listado de
+00004040: 206c 6173 2074 7261 6e73 6163 6369 6f6e   las transaccion
+00004050: 6573 2071 7565 206e 6f20 6573 74e1 6e20  es que no est.n 
+00004060: 636f 6e66 6972 6d61 6461 7322 0a0a 2020  confirmadas"..  
+00004070: 2020 2020 2020 2320 7072 6570 6172 6f20        # preparo 
+00004080: 6c6f 7320 7061 7261 6d65 7472 6f73 2064  los parametros d
+00004090: 6520 656e 7472 6164 6120 6f70 6369 6f6e  e entrada opcion
+000040a0: 616c 6573 3a0a 2020 2020 2020 2020 6b77  ales:.        kw
+000040b0: 6172 6773 203d 207b 7d0a 2020 2020 2020  args = {}.      
+000040c0: 2020 6966 2070 5f69 645f 7472 616e 7361    if p_id_transa
+000040d0: 6363 696f 6e5f 676c 6f62 616c 2069 7320  ccion_global is 
+000040e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000040f0: 2020 2020 2020 6b77 6172 6773 5b27 6172        kwargs['ar
+00004100: 6732 275d 203d 2070 5f69 645f 7472 616e  g2'] = p_id_tran
+00004110: 7361 6363 696f 6e5f 676c 6f62 616c 0a20  saccion_global. 
+00004120: 2020 2020 2020 2069 6620 6964 5f61 6765         if id_age
+00004130: 6e74 655f 696e 666f 726d 6164 6f72 2069  nte_informador i
+00004140: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00004150: 2020 2020 2020 2020 6b77 6172 6773 5b27          kwargs['
+00004160: 6172 6733 275d 203d 2069 645f 6167 656e  arg3'] = id_agen
+00004170: 7465 5f69 6e66 6f72 6d61 646f 720a 2020  te_informador.  
+00004180: 2020 2020 2020 6966 2069 645f 6167 656e        if id_agen
+00004190: 7465 5f6f 7269 6765 6e20 6973 206e 6f74  te_origen is not
+000041a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000041b0: 2020 206b 7761 7267 735b 2761 7267 3427     kwargs['arg4'
+000041c0: 5d20 3d20 6964 5f61 6765 6e74 655f 6f72  ] = id_agente_or
+000041d0: 6967 656e 0a20 2020 2020 2020 2069 6620  igen.        if 
+000041e0: 6964 5f61 6765 6e74 655f 6465 7374 696e  id_agente_destin
+000041f0: 6f20 6973 206e 6f74 204e 6f6e 653a 0a20  o is not None:. 
+00004200: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
+00004210: 735b 2761 7267 3527 5d20 3d20 6964 5f61  s['arg5'] = id_a
+00004220: 6765 6e74 655f 6465 7374 696e 6f0a 2020  gente_destino.  
+00004230: 2020 2020 2020 6966 2069 645f 6d65 6469        if id_medi
+00004240: 6361 6d65 6e74 6f20 6973 206e 6f74 204e  camento is not N
+00004250: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00004260: 206b 7761 7267 735b 2761 7267 3627 5d20   kwargs['arg6'] 
+00004270: 3d20 6964 5f6d 6564 6963 616d 656e 746f  = id_medicamento
+00004280: 0a20 2020 2020 2020 2069 6620 6964 5f65  .        if id_e
+00004290: 7665 6e74 6f20 6973 206e 6f74 204e 6f6e  vento is not Non
+000042a0: 653a 0a20 2020 2020 2020 2020 2020 206b  e:.            k
+000042b0: 7761 7267 735b 2761 7267 3727 5d20 3d20  wargs['arg7'] = 
+000042c0: 6964 5f65 7665 6e74 6f0a 2020 2020 2020  id_evento.      
+000042d0: 2020 6966 2066 6563 6861 5f64 6573 6465    if fecha_desde
+000042e0: 5f6f 7020 6973 206e 6f74 204e 6f6e 653a  _op is not None:
+000042f0: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
+00004300: 7267 735b 2761 7267 3827 5d20 3d20 6665  rgs['arg8'] = fe
+00004310: 6368 615f 6465 7364 655f 6f70 0a20 2020  cha_desde_op.   
+00004320: 2020 2020 2069 6620 6665 6368 615f 6861       if fecha_ha
+00004330: 7374 615f 6f70 2069 7320 6e6f 7420 4e6f  sta_op is not No
+00004340: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00004350: 6b77 6172 6773 5b27 6172 6739 275d 203d  kwargs['arg9'] =
+00004360: 2066 6563 6861 5f68 6173 7461 5f6f 700a   fecha_hasta_op.
+00004370: 2020 2020 2020 2020 6966 2066 6563 6861          if fecha
+00004380: 5f64 6573 6465 5f74 2069 7320 6e6f 7420  _desde_t is not 
+00004390: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000043a0: 2020 6b77 6172 6773 5b27 6172 6731 3027    kwargs['arg10'
+000043b0: 5d20 3d20 6665 6368 615f 6465 7364 655f  ] = fecha_desde_
+000043c0: 740a 2020 2020 2020 2020 6966 2066 6563  t.        if fec
+000043d0: 6861 5f68 6173 7461 5f74 2069 7320 6e6f  ha_hasta_t is no
+000043e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000043f0: 2020 2020 6b77 6172 6773 5b27 6172 6731      kwargs['arg1
+00004400: 3127 5d20 3d20 6665 6368 615f 6861 7374  1'] = fecha_hast
+00004410: 615f 740a 2020 2020 2020 2020 6966 2066  a_t.        if f
+00004420: 6563 6861 5f64 6573 6465 5f76 2069 7320  echa_desde_v is 
+00004430: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00004440: 2020 2020 2020 6b77 6172 6773 5b27 6172        kwargs['ar
+00004450: 6731 3227 5d20 3d20 6665 6368 615f 6465  g12'] = fecha_de
+00004460: 7364 655f 760a 2020 2020 2020 2020 6966  sde_v.        if
+00004470: 2066 6563 6861 5f68 6173 7461 5f76 2069   fecha_hasta_v i
+00004480: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00004490: 2020 2020 2020 2020 6b77 6172 6773 5b27          kwargs['
+000044a0: 6172 6731 3327 5d20 3d20 6665 6368 615f  arg13'] = fecha_
+000044b0: 6861 7374 615f 760a 2020 2020 2020 2020  hasta_v.        
+000044c0: 6966 206e 5f72 656d 6974 6f20 6973 206e  if n_remito is n
+000044d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000044e0: 2020 2020 206b 7761 7267 735b 2761 7267       kwargs['arg
+000044f0: 3134 275d 203d 206e 5f72 656d 6974 6f0a  14'] = n_remito.
+00004500: 2020 2020 2020 2020 6966 206e 5f66 6163          if n_fac
+00004510: 7475 7261 2069 7320 6e6f 7420 4e6f 6e65  tura is not None
+00004520: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
+00004530: 6172 6773 5b27 6172 6731 3527 5d20 3d20  args['arg15'] = 
+00004540: 6e5f 6661 6374 7572 610a 2020 2020 2020  n_factura.      
+00004550: 2020 6966 2065 7374 6164 6f20 6973 206e    if estado is n
+00004560: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00004570: 2020 2020 206b 7761 7267 735b 2761 7267       kwargs['arg
+00004580: 3136 275d 203d 2065 7374 6164 6f0a 2020  16'] = estado.  
+00004590: 2020 2020 2020 6966 206c 6f74 6520 6973        if lote is
+000045a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000045b0: 2020 2020 2020 206b 7761 7267 735b 2761         kwargs['a
+000045c0: 7267 3137 275d 203d 206c 6f74 650a 2020  rg17'] = lote.  
+000045d0: 2020 2020 2020 6966 206e 756d 6572 6f5f        if numero_
+000045e0: 7365 7269 616c 2069 7320 6e6f 7420 4e6f  serial is not No
+000045f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00004600: 6b77 6172 6773 5b27 6172 6731 3827 5d20  kwargs['arg18'] 
+00004610: 3d20 6e75 6d65 726f 5f73 6572 6961 6c0a  = numero_serial.
+00004620: 0a20 2020 2020 2020 2023 206c 6c61 6d6f  .        # llamo
+00004630: 2061 6c20 7765 6273 6572 7669 6365 0a20   al webservice. 
+00004640: 2020 2020 2020 2072 6573 203d 2073 656c         res = sel
+00004650: 662e 636c 6965 6e74 2e67 6574 5472 616e  f.client.getTran
+00004660: 7361 6363 696f 6e65 734e 6f43 6f6e 6669  saccionesNoConfi
+00004670: 726d 6164 6173 280a 2020 2020 2020 2020  rmadas(.        
+00004680: 2020 2020 6172 6730 3d75 7375 6172 696f      arg0=usuario
+00004690: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
+000046a0: 6731 3d70 6173 7377 6f72 642c 0a20 2020  g1=password,.   
+000046b0: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
+000046c0: 730a 2020 2020 2020 2020 290a 2020 2020  s.        ).    
+000046d0: 2020 2020 7265 7420 3d20 7265 735b 2772      ret = res['r
+000046e0: 6574 7572 6e27 5d0a 2020 2020 2020 2020  eturn'].        
+000046f0: 6966 2072 6574 3a0a 2020 2020 2020 2020  if ret:.        
+00004700: 2020 2020 7365 6c66 2e5f 5f61 6e61 6c69      self.__anali
+00004710: 7a61 725f 6572 726f 7265 7328 7265 7429  zar_errores(ret)
+00004720: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00004730: 662e 4361 6e74 5061 6769 6e61 7320 3d20  f.CantPaginas = 
+00004740: 7265 742e 6765 7428 2763 616e 7450 6167  ret.get('cantPag
+00004750: 696e 6173 2729 0a20 2020 2020 2020 2020  inas').         
+00004760: 2020 2073 656c 662e 4861 7945 7272 6f72     self.HayError
+00004770: 203d 2072 6574 2e67 6574 2827 6861 795f   = ret.get('hay_
+00004780: 6572 726f 7227 290a 2020 2020 2020 2020  error').        
+00004790: 2020 2020 7365 6c66 2e54 7261 6e73 6163      self.Transac
+000047a0: 6369 6f6e 506c 6169 6e57 5320 3d20 5b69  cionPlainWS = [i
+000047b0: 7420 666f 7220 6974 2069 6e20 7265 742e  t for it in ret.
+000047c0: 6765 7428 276c 6973 7427 2c20 5b5d 295d  get('list', [])]
+000047d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000047e0: 5472 7565 0a0a 2020 2020 6465 6620 4c65  True..    def Le
+000047f0: 6572 5472 616e 7361 6363 696f 6e28 7365  erTransaccion(se
+00004800: 6c66 293a 0a20 2020 2020 2020 2022 5265  lf):.        "Re
+00004810: 636f 7272 6f20 5472 616e 7361 6363 696f  corro Transaccio
+00004820: 6e50 6c61 696e 5753 2064 6576 7565 6c74  nPlainWS devuelt
+00004830: 6f20 706f 7220 4765 7454 7261 6e73 6163  o por GetTransac
+00004840: 6369 6f6e 6573 4e6f 436f 6e66 6972 6d61  cionesNoConfirma
+00004850: 6461 7322 0a20 2020 2020 2020 2023 2075  das".        # u
+00004860: 7361 7220 4765 7450 6172 616d 6574 726f  sar GetParametro
+00004870: 2070 6172 6120 636f 6e73 756c 7461 7220   para consultar 
+00004880: 656c 2076 616c 6f72 2072 6574 6f72 6e61  el valor retorna
+00004890: 646f 2070 6f72 2065 6c0a 2020 2020 2020  do por el.      
+000048a0: 2020 2320 7765 6273 6572 7669 6365 0a0a    # webservice..
+000048b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000048c0: 5472 616e 7361 6363 696f 6e50 6c61 696e  TransaccionPlain
+000048d0: 5753 3a0a 2020 2020 2020 2020 2020 2020  WS:.            
+000048e0: 2320 6578 7472 6169 676f 2065 6c20 7072  # extraigo el pr
+000048f0: 696d 6572 2069 7465 6d0a 2020 2020 2020  imer item.      
+00004900: 2020 2020 2020 7365 6c66 2e70 6172 616d        self.param
+00004910: 735f 6f75 7420 3d20 7365 6c66 2e54 7261  s_out = self.Tra
+00004920: 6e73 6163 6369 6f6e 506c 6169 6e57 532e  nsaccionPlainWS.
+00004930: 706f 7028 3029 0a20 2020 2020 2020 2020  pop(0).         
+00004940: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
+00004950: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00004960: 2020 2020 2020 2020 2023 206c 696d 7069           # limpi
+00004970: 6f20 6c6f 7320 7061 72e1 6d65 7472 6f73  o los par.metros
+00004980: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00004990: 662e 7061 7261 6d73 5f6f 7574 203d 207b  f.params_out = {
+000049a0: 7d0a 2020 2020 2020 2020 2020 2020 7265  }.            re
+000049b0: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
+000049c0: 6465 6620 4c65 6572 4572 726f 7228 7365  def LeerError(se
+000049d0: 6c66 293a 0a20 2020 2020 2020 2022 5265  lf):.        "Re
+000049e0: 636f 7272 6f20 6c6f 7320 6572 726f 7265  corro los errore
+000049f0: 7320 6465 7675 656c 746f 7320 7920 6465  s devueltos y de
+00004a00: 7675 656c 766f 2065 6c20 7072 696d 6572  vuelvo el primer
+00004a10: 6f20 7369 2065 7869 7374 6522 0a0a 2020  o si existe"..  
+00004a20: 2020 2020 2020 6966 2073 656c 662e 4572        if self.Er
+00004a30: 726f 7265 733a 0a20 2020 2020 2020 2020  rores:.         
+00004a40: 2020 2023 2065 7874 7261 6967 6f20 656c     # extraigo el
+00004a50: 2070 7269 6d65 7220 6974 656d 0a20 2020   primer item.   
+00004a60: 2020 2020 2020 2020 2065 7220 3d20 7365           er = se
+00004a70: 6c66 2e45 7272 6f72 6573 2e70 6f70 2830  lf.Errores.pop(0
+00004a80: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00004a90: 7475 726e 2065 720a 2020 2020 2020 2020  turn er.        
+00004aa0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00004ab0: 2020 7265 7475 726e 2022 220a 0a20 2020    return ""..   
+00004ac0: 2040 696e 6963 6961 6c69 7a61 725f 795f   @inicializar_y_
+00004ad0: 6361 7074 7572 6172 5f65 7863 6570 6369  capturar_excepci
+00004ae0: 6f6e 6573 0a20 2020 2064 6566 2047 6574  ones.    def Get
+00004af0: 456e 7669 6f73 5072 6f70 696f 7341 6c65  EnviosPropiosAle
+00004b00: 7274 6164 6f73 280a 2020 2020 2020 2020  rtados(.        
+00004b10: 7365 6c66 2c20 7573 7561 7269 6f2c 2070  self, usuario, p
+00004b20: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
+00004b30: 2070 5f69 645f 7472 616e 7361 6363 696f   p_id_transaccio
+00004b40: 6e5f 676c 6f62 616c 3d4e 6f6e 652c 2069  n_global=None, i
+00004b50: 645f 6167 656e 7465 5f69 6e66 6f72 6d61  d_agente_informa
+00004b60: 646f 723d 4e6f 6e65 2c0a 2020 2020 2020  dor=None,.      
+00004b70: 2020 6964 5f61 6765 6e74 655f 6f72 6967    id_agente_orig
+00004b80: 656e 3d4e 6f6e 652c 2069 645f 6167 656e  en=None, id_agen
+00004b90: 7465 5f64 6573 7469 6e6f 3d4e 6f6e 652c  te_destino=None,
+00004ba0: 0a20 2020 2020 2020 2069 645f 6d65 6469  .        id_medi
+00004bb0: 6361 6d65 6e74 6f3d 4e6f 6e65 2c20 6964  camento=None, id
+00004bc0: 5f65 7665 6e74 6f3d 4e6f 6e65 2c0a 2020  _evento=None,.  
+00004bd0: 2020 2020 2020 6665 6368 615f 6465 7364        fecha_desd
+00004be0: 655f 6f70 3d4e 6f6e 652c 2066 6563 6861  e_op=None, fecha
+00004bf0: 5f68 6173 7461 5f6f 703d 4e6f 6e65 2c0a  _hasta_op=None,.
+00004c00: 2020 2020 2020 2020 6665 6368 615f 6465          fecha_de
+00004c10: 7364 655f 743d 4e6f 6e65 2c20 6665 6368  sde_t=None, fech
+00004c20: 615f 6861 7374 615f 743d 4e6f 6e65 2c0a  a_hasta_t=None,.
+00004c30: 2020 2020 2020 2020 6665 6368 615f 6465          fecha_de
+00004c40: 7364 655f 763d 4e6f 6e65 2c20 6665 6368  sde_v=None, fech
+00004c50: 615f 6861 7374 615f 763d 4e6f 6e65 2c0a  a_hasta_v=None,.
+00004c60: 2020 2020 2020 2020 6e5f 7265 6d69 746f          n_remito
+00004c70: 3d4e 6f6e 652c 206e 5f66 6163 7475 7261  =None, n_factura
+00004c80: 3d4e 6f6e 652c 0a20 2020 2029 3a0a 2020  =None,.    ):.  
+00004c90: 2020 2020 2020 224f 6274 6965 6e65 206c        "Obtiene l
+00004ca0: 6173 2064 6973 7472 6962 7563 696f 6e65  as distribucione
+00004cb0: 7320 7920 656e 76ed 6f73 2070 726f 7069  s y env.os propi
+00004cc0: 6f73 2071 7565 2068 616e 2073 6964 6f20  os que han sido 
+00004cd0: 616c 6572 7461 646f 7322 0a0a 2020 2020  alertados"..    
+00004ce0: 2020 2020 2320 7072 6570 6172 6f20 6c6f      # preparo lo
+00004cf0: 7320 7061 7261 6d65 7472 6f73 2064 6520  s parametros de 
+00004d00: 656e 7472 6164 6120 6f70 6369 6f6e 616c  entrada opcional
+00004d10: 6573 3a0a 2020 2020 2020 2020 6b77 6172  es:.        kwar
+00004d20: 6773 203d 207b 7d0a 2020 2020 2020 2020  gs = {}.        
+00004d30: 6966 2070 5f69 645f 7472 616e 7361 6363  if p_id_transacc
+00004d40: 696f 6e5f 676c 6f62 616c 2069 7320 6e6f  ion_global is no
+00004d50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00004d60: 2020 2020 6b77 6172 6773 5b27 6172 6732      kwargs['arg2
+00004d70: 275d 203d 2070 5f69 645f 7472 616e 7361  '] = p_id_transa
+00004d80: 6363 696f 6e5f 676c 6f62 616c 0a20 2020  ccion_global.   
+00004d90: 2020 2020 2069 6620 6964 5f61 6765 6e74       if id_agent
+00004da0: 655f 696e 666f 726d 6164 6f72 2069 7320  e_informador is 
+00004db0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00004dc0: 2020 2020 2020 6b77 6172 6773 5b27 6172        kwargs['ar
+00004dd0: 6733 275d 203d 2069 645f 6167 656e 7465  g3'] = id_agente
+00004de0: 5f69 6e66 6f72 6d61 646f 720a 2020 2020  _informador.    
+00004df0: 2020 2020 6966 2069 645f 6167 656e 7465      if id_agente
+00004e00: 5f6f 7269 6765 6e20 6973 206e 6f74 204e  _origen is not N
+00004e10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00004e20: 206b 7761 7267 735b 2761 7267 3427 5d20   kwargs['arg4'] 
+00004e30: 3d20 6964 5f61 6765 6e74 655f 6f72 6967  = id_agente_orig
+00004e40: 656e 0a20 2020 2020 2020 2069 6620 6964  en.        if id
+00004e50: 5f61 6765 6e74 655f 6465 7374 696e 6f20  _agente_destino 
+00004e60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00004e70: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
+00004e80: 2761 7267 3527 5d20 3d20 6964 5f61 6765  'arg5'] = id_age
+00004e90: 6e74 655f 6465 7374 696e 6f0a 2020 2020  nte_destino.    
+00004ea0: 2020 2020 6966 2069 645f 6d65 6469 6361      if id_medica
+00004eb0: 6d65 6e74 6f20 6973 206e 6f74 204e 6f6e  mento is not Non
+00004ec0: 653a 0a20 2020 2020 2020 2020 2020 206b  e:.            k
+00004ed0: 7761 7267 735b 2761 7267 3627 5d20 3d20  wargs['arg6'] = 
+00004ee0: 6964 5f6d 6564 6963 616d 656e 746f 0a20  id_medicamento. 
+00004ef0: 2020 2020 2020 2069 6620 6964 5f65 7665         if id_eve
+00004f00: 6e74 6f20 6973 206e 6f74 204e 6f6e 653a  nto is not None:
+00004f10: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
+00004f20: 7267 735b 2761 7267 3727 5d20 3d20 6964  rgs['arg7'] = id
+00004f30: 5f65 7665 6e74 6f0a 2020 2020 2020 2020  _evento.        
+00004f40: 6966 2066 6563 6861 5f64 6573 6465 5f6f  if fecha_desde_o
+00004f50: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00004f60: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
+00004f70: 735b 2761 7267 3827 5d20 3d20 6665 6368  s['arg8'] = fech
+00004f80: 615f 6465 7364 655f 6f70 0a20 2020 2020  a_desde_op.     
+00004f90: 2020 2069 6620 6665 6368 615f 6861 7374     if fecha_hast
+00004fa0: 615f 6f70 2069 7320 6e6f 7420 4e6f 6e65  a_op is not None
+00004fb0: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
+00004fc0: 6172 6773 5b27 6172 6739 275d 203d 2066  args['arg9'] = f
+00004fd0: 6563 6861 5f68 6173 7461 5f6f 700a 2020  echa_hasta_op.  
+00004fe0: 2020 2020 2020 6966 2066 6563 6861 5f64        if fecha_d
+00004ff0: 6573 6465 5f74 2069 7320 6e6f 7420 4e6f  esde_t is not No
+00005000: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00005010: 6b77 6172 6773 5b27 6172 6731 3027 5d20  kwargs['arg10'] 
+00005020: 3d20 6665 6368 615f 6465 7364 655f 740a  = fecha_desde_t.
+00005030: 2020 2020 2020 2020 6966 2066 6563 6861          if fecha
+00005040: 5f68 6173 7461 5f74 2069 7320 6e6f 7420  _hasta_t is not 
+00005050: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00005060: 2020 6b77 6172 6773 5b27 6172 6731 3127    kwargs['arg11'
+00005070: 5d20 3d20 6665 6368 615f 6861 7374 615f  ] = fecha_hasta_
+00005080: 740a 2020 2020 2020 2020 6966 2066 6563  t.        if fec
+00005090: 6861 5f64 6573 6465 5f76 2069 7320 6e6f  ha_desde_v is no
+000050a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000050b0: 2020 2020 6b77 6172 6773 5b27 6172 6731      kwargs['arg1
+000050c0: 3227 5d20 3d20 6665 6368 615f 6465 7364  2'] = fecha_desd
+000050d0: 655f 760a 2020 2020 2020 2020 6966 2066  e_v.        if f
+000050e0: 6563 6861 5f68 6173 7461 5f76 2069 7320  echa_hasta_v is 
+000050f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00005100: 2020 2020 2020 6b77 6172 6773 5b27 6172        kwargs['ar
+00005110: 6731 3327 5d20 3d20 6665 6368 615f 6861  g13'] = fecha_ha
+00005120: 7374 615f 760a 2020 2020 2020 2020 6966  sta_v.        if
+00005130: 206e 5f72 656d 6974 6f20 6973 206e 6f74   n_remito is not
+00005140: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005150: 2020 206b 7761 7267 735b 2761 7267 3134     kwargs['arg14
+00005160: 275d 203d 206e 5f72 656d 6974 6f0a 2020  '] = n_remito.  
+00005170: 2020 2020 2020 6966 206e 5f66 6163 7475        if n_factu
+00005180: 7261 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ra is not None:.
+00005190: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
+000051a0: 6773 5b27 6172 6731 3527 5d20 3d20 6e5f  gs['arg15'] = n_
+000051b0: 6661 6374 7572 610a 0a20 2020 2020 2020  factura..       
+000051c0: 2023 206c 6c61 6d6f 2061 6c20 7765 6273   # llamo al webs
+000051d0: 6572 7669 6365 0a20 2020 2020 2020 2072  ervice.        r
+000051e0: 6573 203d 2073 656c 662e 636c 6965 6e74  es = self.client
+000051f0: 2e67 6574 456e 7669 6f73 5072 6f70 696f  .getEnviosPropio
+00005200: 7341 6c65 7274 6164 6f73 280a 2020 2020  sAlertados(.    
+00005210: 2020 2020 2020 2020 6172 6730 3d75 7375          arg0=usu
+00005220: 6172 696f 2c0a 2020 2020 2020 2020 2020  ario,.          
+00005230: 2020 6172 6731 3d70 6173 7377 6f72 642c    arg1=password,
+00005240: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
+00005250: 7761 7267 730a 2020 2020 2020 2020 290a  wargs.        ).
+00005260: 2020 2020 2020 2020 7265 7420 3d20 7265          ret = re
+00005270: 735b 2772 6574 7572 6e27 5d0a 2020 2020  s['return'].    
+00005280: 2020 2020 6966 2072 6574 3a0a 2020 2020      if ret:.    
+00005290: 2020 2020 2020 2020 7365 6c66 2e5f 5f61          self.__a
+000052a0: 6e61 6c69 7a61 725f 6572 726f 7265 7328  nalizar_errores(
+000052b0: 7265 7429 0a20 2020 2020 2020 2020 2020  ret).           
+000052c0: 2073 656c 662e 4361 6e74 5061 6769 6e61   self.CantPagina
+000052d0: 7320 3d20 7265 742e 6765 7428 2763 616e  s = ret.get('can
+000052e0: 7450 6167 696e 6173 2729 0a20 2020 2020  tPaginas').     
+000052f0: 2020 2020 2020 2073 656c 662e 4861 7945         self.HayE
+00005300: 7272 6f72 203d 2072 6574 2e67 6574 2827  rror = ret.get('
+00005310: 6861 795f 6572 726f 7227 290a 2020 2020  hay_error').    
+00005320: 2020 2020 2020 2020 7365 6c66 2e54 7261          self.Tra
+00005330: 6e73 6163 6369 6f6e 506c 6169 6e57 5320  nsaccionPlainWS 
+00005340: 3d20 5b69 7420 666f 7220 6974 2069 6e20  = [it for it in 
+00005350: 7265 742e 6765 7428 276c 6973 7427 2c20  ret.get('list', 
+00005360: 5b5d 295d 0a20 2020 2020 2020 2072 6574  [])].        ret
+00005370: 7572 6e20 5472 7565 0a0a 2020 2020 4069  urn True..    @i
+00005380: 6e69 6369 616c 697a 6172 5f79 5f63 6170  nicializar_y_cap
+00005390: 7475 7261 725f 6578 6365 7063 696f 6e65  turar_excepcione
+000053a0: 730a 2020 2020 6465 6620 4765 7454 7261  s.    def GetTra
+000053b0: 6e73 6163 6369 6f6e 6573 5753 280a 2020  nsaccionesWS(.  
+000053c0: 2020 2020 2020 7365 6c66 2c20 7573 7561        self, usua
+000053d0: 7269 6f2c 2070 6173 7377 6f72 642c 0a20  rio, password,. 
+000053e0: 2020 2020 2020 2070 5f69 645f 7472 616e         p_id_tran
+000053f0: 7361 6363 696f 6e5f 676c 6f62 616c 3d4e  saccion_global=N
+00005400: 6f6e 652c 0a20 2020 2020 2020 2069 645f  one,.        id_
+00005410: 6167 656e 7465 5f6f 7269 6765 6e3d 4e6f  agente_origen=No
+00005420: 6e65 2c20 6964 5f61 6765 6e74 655f 6465  ne, id_agente_de
+00005430: 7374 696e 6f3d 4e6f 6e65 2c0a 2020 2020  stino=None,.    
+00005440: 2020 2020 6964 5f6d 6564 6963 616d 656e      id_medicamen
+00005450: 746f 3d4e 6f6e 652c 2069 645f 6576 656e  to=None, id_even
+00005460: 746f 3d4e 6f6e 652c 0a20 2020 2020 2020  to=None,.       
+00005470: 2066 6563 6861 5f64 6573 6465 5f6f 703d   fecha_desde_op=
+00005480: 4e6f 6e65 2c20 6665 6368 615f 6861 7374  None, fecha_hast
+00005490: 615f 6f70 3d4e 6f6e 652c 0a20 2020 2020  a_op=None,.     
+000054a0: 2020 2066 6563 6861 5f64 6573 6465 5f74     fecha_desde_t
+000054b0: 3d4e 6f6e 652c 2066 6563 6861 5f68 6173  =None, fecha_has
+000054c0: 7461 5f74 3d4e 6f6e 652c 0a20 2020 2020  ta_t=None,.     
+000054d0: 2020 2066 6563 6861 5f64 6573 6465 5f76     fecha_desde_v
+000054e0: 3d4e 6f6e 652c 2066 6563 6861 5f68 6173  =None, fecha_has
+000054f0: 7461 5f76 3d4e 6f6e 652c 0a20 2020 2020  ta_v=None,.     
+00005500: 2020 206e 5f72 656d 6974 6f3d 4e6f 6e65     n_remito=None
+00005510: 2c20 6e5f 6661 6374 7572 613d 4e6f 6e65  , n_factura=None
+00005520: 2c0a 2020 2020 2020 2020 6964 5f65 7374  ,.        id_est
+00005530: 6164 6f3d 4e6f 6e65 2c20 6e72 6f5f 7061  ado=None, nro_pa
+00005540: 673d 4e6f 6e65 2c0a 2020 2020 293a 0a20  g=None,.    ):. 
+00005550: 2020 2020 2020 2022 4f62 7469 656e 6520         "Obtiene 
+00005560: 6c6f 7320 6d6f 7669 6d69 656e 746f 7320  los movimientos 
+00005570: 7265 616c 697a 6164 6f73 2079 2070 6572  realizados y per
+00005580: 6d69 7465 2066 696c 7472 6f73 2064 6520  mite filtros de 
+00005590: 62fa 7371 7565 6461 220a 0a20 2020 2020  b.squeda"..     
+000055a0: 2020 2023 2070 7265 7061 726f 206c 6f73     # preparo los
+000055b0: 2070 6172 616d 6574 726f 7320 6465 2065   parametros de e
+000055c0: 6e74 7261 6461 206f 7063 696f 6e61 6c65  ntrada opcionale
+000055d0: 733a 0a20 2020 2020 2020 206b 7761 7267  s:.        kwarg
+000055e0: 7320 3d20 7b7d 0a20 2020 2020 2020 2069  s = {}.        i
+000055f0: 6620 705f 6964 5f74 7261 6e73 6163 6369  f p_id_transacci
+00005600: 6f6e 5f67 6c6f 6261 6c20 6973 206e 6f74  on_global is not
+00005610: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005620: 2020 206b 7761 7267 735b 2761 7267 3227     kwargs['arg2'
+00005630: 5d20 3d20 705f 6964 5f74 7261 6e73 6163  ] = p_id_transac
+00005640: 6369 6f6e 5f67 6c6f 6261 6c0a 2020 2020  cion_global.    
+00005650: 2020 2020 6966 2069 645f 6167 656e 7465      if id_agente
+00005660: 5f6f 7269 6765 6e20 6973 206e 6f74 204e  _origen is not N
+00005670: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00005680: 206b 7761 7267 735b 2761 7267 3327 5d20   kwargs['arg3'] 
+00005690: 3d20 6964 5f61 6765 6e74 655f 6f72 6967  = id_agente_orig
+000056a0: 656e 0a20 2020 2020 2020 2069 6620 6964  en.        if id
+000056b0: 5f61 6765 6e74 655f 6465 7374 696e 6f20  _agente_destino 
+000056c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000056d0: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
+000056e0: 2761 7267 3427 5d20 3d20 6964 5f61 6765  'arg4'] = id_age
+000056f0: 6e74 655f 6465 7374 696e 6f0a 2020 2020  nte_destino.    
+00005700: 2020 2020 6966 2069 645f 6d65 6469 6361      if id_medica
+00005710: 6d65 6e74 6f20 6973 206e 6f74 204e 6f6e  mento is not Non
+00005720: 653a 0a20 2020 2020 2020 2020 2020 206b  e:.            k
+00005730: 7761 7267 735b 2761 7267 3527 5d20 3d20  wargs['arg5'] = 
+00005740: 6964 5f6d 6564 6963 616d 656e 746f 0a20  id_medicamento. 
+00005750: 2020 2020 2020 2069 6620 6964 5f65 7665         if id_eve
+00005760: 6e74 6f20 6973 206e 6f74 204e 6f6e 653a  nto is not None:
+00005770: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
+00005780: 7267 735b 2761 7267 3627 5d20 3d20 6964  rgs['arg6'] = id
+00005790: 5f65 7665 6e74 6f0a 2020 2020 2020 2020  _evento.        
+000057a0: 6966 2066 6563 6861 5f64 6573 6465 5f6f  if fecha_desde_o
+000057b0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+000057c0: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
+000057d0: 735b 2761 7267 3727 5d20 3d20 6665 6368  s['arg7'] = fech
+000057e0: 615f 6465 7364 655f 6f70 0a20 2020 2020  a_desde_op.     
+000057f0: 2020 2069 6620 6665 6368 615f 6861 7374     if fecha_hast
+00005800: 615f 6f70 2069 7320 6e6f 7420 4e6f 6e65  a_op is not None
+00005810: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
+00005820: 6172 6773 5b27 6172 6738 275d 203d 2066  args['arg8'] = f
+00005830: 6563 6861 5f68 6173 7461 5f6f 700a 2020  echa_hasta_op.  
+00005840: 2020 2020 2020 6966 2066 6563 6861 5f64        if fecha_d
+00005850: 6573 6465 5f74 2069 7320 6e6f 7420 4e6f  esde_t is not No
+00005860: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00005870: 6b77 6172 6773 5b27 6172 6739 275d 203d  kwargs['arg9'] =
+00005880: 2066 6563 6861 5f64 6573 6465 5f74 0a20   fecha_desde_t. 
+00005890: 2020 2020 2020 2069 6620 6665 6368 615f         if fecha_
+000058a0: 6861 7374 615f 7420 6973 206e 6f74 204e  hasta_t is not N
+000058b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000058c0: 206b 7761 7267 735b 2761 7267 3130 275d   kwargs['arg10']
+000058d0: 203d 2066 6563 6861 5f68 6173 7461 5f74   = fecha_hasta_t
+000058e0: 0a20 2020 2020 2020 2069 6620 6665 6368  .        if fech
+000058f0: 615f 6465 7364 655f 7620 6973 206e 6f74  a_desde_v is not
+00005900: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005910: 2020 206b 7761 7267 735b 2761 7267 3131     kwargs['arg11
+00005920: 275d 203d 2066 6563 6861 5f64 6573 6465  '] = fecha_desde
+00005930: 5f76 0a20 2020 2020 2020 2069 6620 6665  _v.        if fe
+00005940: 6368 615f 6861 7374 615f 7620 6973 206e  cha_hasta_v is n
+00005950: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00005960: 2020 2020 206b 7761 7267 735b 2761 7267       kwargs['arg
+00005970: 3132 275d 203d 2066 6563 6861 5f68 6173  12'] = fecha_has
+00005980: 7461 5f76 0a20 2020 2020 2020 2069 6620  ta_v.        if 
+00005990: 6e5f 7265 6d69 746f 2069 7320 6e6f 7420  n_remito is not 
+000059a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000059b0: 2020 6b77 6172 6773 5b27 6172 6731 3327    kwargs['arg13'
+000059c0: 5d20 3d20 6e5f 7265 6d69 746f 0a20 2020  ] = n_remito.   
+000059d0: 2020 2020 2069 6620 6e5f 6661 6374 7572       if n_factur
+000059e0: 6120 6973 206e 6f74 204e 6f6e 653a 0a20  a is not None:. 
+000059f0: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
+00005a00: 735b 2761 7267 3134 275d 203d 206e 5f66  s['arg14'] = n_f
+00005a10: 6163 7475 7261 0a20 2020 2020 2020 2069  actura.        i
+00005a20: 6620 6964 5f65 7374 6164 6f20 6973 206e  f id_estado is n
+00005a30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00005a40: 2020 2020 206b 7761 7267 735b 2761 7267       kwargs['arg
+00005a50: 3135 275d 203d 2069 645f 6573 7461 646f  15'] = id_estado
+00005a60: 0a20 2020 2020 2020 2069 6620 6e72 6f5f  .        if nro_
+00005a70: 7061 6720 6973 206e 6f74 204e 6f6e 653a  pag is not None:
+00005a80: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
+00005a90: 7267 735b 2761 7267 3136 275d 203d 206e  rgs['arg16'] = n
+00005aa0: 726f 5f70 6167 0a0a 2020 2020 2020 2020  ro_pag..        
+00005ab0: 2320 6c6c 616d 6f20 616c 2077 6562 7365  # llamo al webse
+00005ac0: 7276 6963 650a 2020 2020 2020 2020 7265  rvice.        re
+00005ad0: 7320 3d20 7365 6c66 2e63 6c69 656e 742e  s = self.client.
+00005ae0: 6765 7454 7261 6e73 6163 6369 6f6e 6573  getTransacciones
+00005af0: 5753 280a 2020 2020 2020 2020 2020 2020  WS(.            
+00005b00: 6172 6730 3d75 7375 6172 696f 2c0a 2020  arg0=usuario,.  
+00005b10: 2020 2020 2020 2020 2020 6172 6731 3d70            arg1=p
+00005b20: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
+00005b30: 2020 2020 202a 2a6b 7761 7267 730a 2020       **kwargs.  
+00005b40: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00005b50: 7265 7420 3d20 7265 735b 2772 6574 7572  ret = res['retur
+00005b60: 6e27 5d0a 2020 2020 2020 2020 6966 2072  n'].        if r
+00005b70: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
+00005b80: 7365 6c66 2e5f 5f61 6e61 6c69 7a61 725f  self.__analizar_
+00005b90: 6572 726f 7265 7328 7265 7429 0a20 2020  errores(ret).   
+00005ba0: 2020 2020 2020 2020 2073 656c 662e 4361           self.Ca
+00005bb0: 6e74 5061 6769 6e61 7320 3d20 7265 742e  ntPaginas = ret.
+00005bc0: 6765 7428 2763 616e 7450 6167 696e 6173  get('cantPaginas
+00005bd0: 2729 0a20 2020 2020 2020 2020 2020 2073  ').            s
+00005be0: 656c 662e 4861 7945 7272 6f72 203d 2072  elf.HayError = r
+00005bf0: 6574 2e67 6574 2827 6861 795f 6572 726f  et.get('hay_erro
+00005c00: 7227 290a 2020 2020 2020 2020 2020 2020  r').            
+00005c10: 7365 6c66 2e54 7261 6e73 6163 6369 6f6e  self.Transaccion
+00005c20: 506c 6169 6e57 5320 3d20 5b69 7420 666f  PlainWS = [it fo
+00005c30: 7220 6974 2069 6e20 7265 742e 6765 7428  r it in ret.get(
+00005c40: 276c 6973 7427 2c20 5b5d 295d 0a20 2020  'list', [])].   
+00005c50: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00005c60: 0a0a 2020 2020 4069 6e69 6369 616c 697a  ..    @inicializ
+00005c70: 6172 5f79 5f63 6170 7475 7261 725f 6578  ar_y_capturar_ex
+00005c80: 6365 7063 696f 6e65 730a 2020 2020 6465  cepciones.    de
+00005c90: 6620 4765 7443 6174 616c 6f67 6f45 6c65  f GetCatalogoEle
+00005ca0: 6374 726f 6e69 636f 4279 4754 494e 280a  ctronicoByGTIN(.
+00005cb0: 2020 2020 2020 2020 7365 6c66 2c20 7573          self, us
+00005cc0: 7561 7269 6f2c 2070 6173 7377 6f72 642c  uario, password,
+00005cd0: 0a20 2020 2020 2020 2063 7569 745f 6661  .        cuit_fa
+00005ce0: 6272 6963 616e 7465 3d4e 6f6e 652c 2067  bricante=None, g
+00005cf0: 7469 6e3d 4e6f 6e65 2c20 6465 7363 7269  tin=None, descri
+00005d00: 7063 696f 6e3d 4e6f 6e65 2c0a 2020 2020  pcion=None,.    
+00005d10: 2020 2020 6964 5f6d 6f6e 6f64 726f 6761      id_monodroga
+00005d20: 3d4e 6f6e 652c 0a20 2020 2029 3a0a 2020  =None,.    ):.  
+00005d30: 2020 2020 2020 224f 6274 6965 6e65 2065        "Obtiene e
+00005d40: 6c20 4361 74e1 6c6f 676f 2045 6c65 6374  l Cat.logo Elect
+00005d50: 72f3 6e69 636f 2064 6520 4d65 6469 6361  r.nico de Medica
+00005d60: 6d65 6e74 6f73 220a 0a20 2020 2020 2020  mentos"..       
+00005d70: 2023 2070 7265 7061 726f 206c 6f73 2070   # preparo los p
+00005d80: 6172 616d 6574 726f 7320 6465 2065 6e74  arametros de ent
+00005d90: 7261 6461 206f 7063 696f 6e61 6c65 733a  rada opcionales:
+00005da0: 0a20 2020 2020 2020 206b 7761 7267 7320  .        kwargs 
+00005db0: 3d20 7b7d 0a20 2020 2020 2020 2069 6620  = {}.        if 
+00005dc0: 6375 6974 5f66 6162 7269 6361 6e74 6520  cuit_fabricante 
+00005dd0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00005de0: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
+00005df0: 2761 7267 3227 5d20 3d20 6375 6974 5f66  'arg2'] = cuit_f
+00005e00: 6162 7269 6361 6e74 650a 2020 2020 2020  abricante.      
+00005e10: 2020 6966 2067 7469 6e20 6973 206e 6f74    if gtin is not
+00005e20: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005e30: 2020 206b 7761 7267 735b 2761 7267 3327     kwargs['arg3'
+00005e40: 5d20 3d20 6774 696e 0a20 2020 2020 2020  ] = gtin.       
+00005e50: 2069 6620 6465 7363 7269 7063 696f 6e20   if descripcion 
+00005e60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00005e70: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
+00005e80: 2761 7267 3427 5d20 3d20 6465 7363 7269  'arg4'] = descri
+00005e90: 7063 696f 6e0a 2020 2020 2020 2020 6966  pcion.        if
+00005ea0: 2069 645f 6d6f 6e6f 6472 6f67 6120 6973   id_monodroga is
+00005eb0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00005ec0: 2020 2020 2020 206b 7761 7267 735b 2761         kwargs['a
+00005ed0: 7267 3527 5d20 3d20 6964 5f6d 6f6e 6f64  rg5'] = id_monod
+00005ee0: 726f 6761 0a0a 2020 2020 2020 2020 2320  roga..        # 
+00005ef0: 6c6c 616d 6f20 616c 2077 6562 7365 7276  llamo al webserv
+00005f00: 6963 650a 2020 2020 2020 2020 7265 7320  ice.        res 
+00005f10: 3d20 7365 6c66 2e63 6c69 656e 742e 6765  = self.client.ge
+00005f20: 7443 6174 616c 6f67 6f45 6c65 6374 726f  tCatalogoElectro
+00005f30: 6e69 636f 4279 4754 494e 280a 2020 2020  nicoByGTIN(.    
+00005f40: 2020 2020 2020 2020 6172 6730 3d75 7375          arg0=usu
+00005f50: 6172 696f 2c0a 2020 2020 2020 2020 2020  ario,.          
+00005f60: 2020 6172 6731 3d70 6173 7377 6f72 642c    arg1=password,
+00005f70: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
+00005f80: 7761 7267 730a 2020 2020 2020 2020 290a  wargs.        ).
+00005f90: 2020 2020 2020 2020 7265 7420 3d20 7265          ret = re
+00005fa0: 735b 2772 6574 7572 6e27 5d0a 2020 2020  s['return'].    
+00005fb0: 2020 2020 6966 2072 6574 3a0a 2020 2020      if ret:.    
+00005fc0: 2020 2020 2020 2020 7365 6c66 2e5f 5f61          self.__a
+00005fd0: 6e61 6c69 7a61 725f 6572 726f 7265 7328  nalizar_errores(
+00005fe0: 7265 7429 0a20 2020 2020 2020 2020 2020  ret).           
+00005ff0: 2073 656c 662e 4361 6e74 5061 6769 6e61   self.CantPagina
+00006000: 7320 3d20 7265 742e 6765 7428 2763 616e  s = ret.get('can
+00006010: 7450 6167 696e 6173 2729 0a20 2020 2020  tPaginas').     
+00006020: 2020 2020 2020 2073 656c 662e 4861 7945         self.HayE
+00006030: 7272 6f72 203d 2072 6574 2e67 6574 2827  rror = ret.get('
+00006040: 6861 795f 6572 726f 7227 290a 2020 2020  hay_error').    
+00006050: 2020 2020 2020 2020 7365 6c66 2e70 6172          self.par
+00006060: 616d 735f 6f75 7420 3d20 6469 6374 280a  ams_out = dict(.
+00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006080: 5b28 692c 2069 7429 2066 6f72 2069 2c20  [(i, it) for i, 
+00006090: 6974 2069 6e20 656e 756d 6572 6174 6528  it in enumerate(
+000060a0: 7265 742e 6765 7428 276c 6973 7427 2c20  ret.get('list', 
+000060b0: 5b5d 2929 5d29 0a20 2020 2020 2020 2020  []))]).         
+000060c0: 2020 2072 6574 7572 6e20 6c65 6e28 7365     return len(se
+000060d0: 6c66 2e70 6172 616d 735f 6f75 7429 0a20  lf.params_out). 
+000060e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000060f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00006100: 300a 0a20 2020 2040 696e 6963 6961 6c69  0..    @iniciali
+00006110: 7a61 725f 795f 6361 7074 7572 6172 5f65  zar_y_capturar_e
+00006120: 7863 6570 6369 6f6e 6573 0a20 2020 2064  xcepciones.    d
+00006130: 6566 2047 6574 436f 6e73 756c 7461 5374  ef GetConsultaSt
+00006140: 6f63 6b28 0a20 2020 2020 2020 2073 656c  ock(.        sel
+00006150: 662c 2075 7375 6172 696f 2c20 7061 7373  f, usuario, pass
+00006160: 776f 7264 2c0a 2020 2020 2020 2020 6964  word,.        id
+00006170: 5f6d 6564 6963 616d 656e 746f 3d4e 6f6e  _medicamento=Non
+00006180: 652c 2069 645f 6167 656e 7465 3d4e 6f6e  e, id_agente=Non
+00006190: 652c 2064 6573 6372 6970 6369 6f6e 3d4e  e, descripcion=N
+000061a0: 6f6e 652c 0a20 2020 2020 2020 2063 616e  one,.        can
+000061b0: 7469 6461 643d 4e6f 6e65 2c20 7072 6573  tidad=None, pres
+000061c0: 656e 7461 6369 6f6e 3d4e 6f6e 652c 0a20  entacion=None,. 
+000061d0: 2020 2020 2020 206c 6f74 653d 4e6f 6e65         lote=None
+000061e0: 2c20 6e75 6d65 726f 5f73 6572 6961 6c3d  , numero_serial=
+000061f0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6e72  None,.        nr
+00006200: 6f5f 7061 673d 312c 2063 616e 745f 7265  o_pag=1, cant_re
+00006210: 673d 3130 302c 0a20 2020 2029 3a0a 2020  g=100,.    ):.  
+00006220: 2020 2020 2020 2250 6572 6d69 7465 2063        "Permite c
+00006230: 6f6e 7375 6c74 6172 2065 6c20 7374 6f63  onsultar el stoc
+00006240: 6b20 6163 7475 616c 2064 656c 2061 6765  k actual del age
+00006250: 6e74 652e 220a 0a20 2020 2020 2020 2023  nte."..        #
+00006260: 2070 7265 7061 726f 206c 6f73 2070 6172   preparo los par
+00006270: 616d 6574 726f 7320 6465 2065 6e74 7261  ametros de entra
+00006280: 6461 206f 7063 696f 6e61 6c65 733a 0a20  da opcionales:. 
+00006290: 2020 2020 2020 206b 7761 7267 7320 3d20         kwargs = 
+000062a0: 7b7d 0a20 2020 2020 2020 2069 6620 6964  {}.        if id
+000062b0: 5f6d 6564 6963 616d 656e 746f 2069 7320  _medicamento is 
+000062c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000062d0: 2020 2020 2020 6b77 6172 6773 5b27 6172        kwargs['ar
+000062e0: 6732 275d 203d 2069 645f 6d65 6469 6361  g2'] = id_medica
+000062f0: 6d65 6e74 6f0a 2020 2020 2020 2020 6966  mento.        if
+00006300: 2069 645f 6167 656e 7465 2069 7320 6e6f   id_agente is no
+00006310: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00006320: 2020 2020 6b77 6172 6773 5b27 6172 6733      kwargs['arg3
+00006330: 275d 203d 2069 645f 6167 656e 7465 0a20  '] = id_agente. 
+00006340: 2020 2020 2020 2069 6620 6465 7363 7269         if descri
+00006350: 7063 696f 6e20 6973 206e 6f74 204e 6f6e  pcion is not Non
+00006360: 653a 0a20 2020 2020 2020 2020 2020 206b  e:.            k
+00006370: 7761 7267 735b 2761 7267 3427 5d20 3d20  wargs['arg4'] = 
+00006380: 6465 7363 7269 7063 696f 6e0a 2020 2020  descripcion.    
+00006390: 2020 2020 6966 2063 616e 7469 6461 6420      if cantidad 
+000063a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000063b0: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
+000063c0: 2761 7267 3527 5d20 3d20 6361 6e74 6964  'arg5'] = cantid
+000063d0: 6164 0a20 2020 2020 2020 2069 6620 7072  ad.        if pr
+000063e0: 6573 656e 7461 6369 6f6e 2069 7320 6e6f  esentacion is no
+000063f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00006400: 2020 2020 6b77 6172 6773 5b27 6172 6736      kwargs['arg6
+00006410: 275d 203d 2070 7265 7365 6e74 6163 696f  '] = presentacio
+00006420: 6e0a 2020 2020 2020 2020 6966 206c 6f74  n.        if lot
+00006430: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00006440: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
+00006450: 735b 2761 7267 3727 5d20 3d20 6c6f 7465  s['arg7'] = lote
+00006460: 0a20 2020 2020 2020 2069 6620 6e75 6d65  .        if nume
+00006470: 726f 5f73 6572 6961 6c20 6973 206e 6f74  ro_serial is not
+00006480: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00006490: 2020 206b 7761 7267 735b 2761 7267 3827     kwargs['arg8'
+000064a0: 5d20 3d20 6e75 6d65 726f 5f73 6572 6961  ] = numero_seria
+000064b0: 6c0a 2020 2020 2020 2020 6966 206e 726f  l.        if nro
+000064c0: 5f70 6167 2069 7320 6e6f 7420 4e6f 6e65  _pag is not None
+000064d0: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
+000064e0: 6172 6773 5b27 6172 6739 275d 203d 206e  args['arg9'] = n
+000064f0: 726f 5f70 6167 0a20 2020 2020 2020 2069  ro_pag.        i
+00006500: 6620 6361 6e74 5f72 6567 2069 7320 6e6f  f cant_reg is no
+00006510: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00006520: 2020 2020 6b77 6172 6773 5b27 6172 6731      kwargs['arg1
+00006530: 3027 5d20 3d20 6361 6e74 5f72 6567 0a0a  0'] = cant_reg..
+00006540: 2020 2020 2020 2020 2320 6c6c 616d 6f20          # llamo 
+00006550: 616c 2077 6562 7365 7276 6963 650a 2020  al webservice.  
+00006560: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
+00006570: 2e63 6c69 656e 742e 6765 7443 6f6e 7375  .client.getConsu
+00006580: 6c74 6153 746f 636b 280a 2020 2020 2020  ltaStock(.      
+00006590: 2020 2020 2020 6172 6730 3d75 7375 6172        arg0=usuar
+000065a0: 696f 2c0a 2020 2020 2020 2020 2020 2020  io,.            
+000065b0: 6172 6731 3d70 6173 7377 6f72 642c 0a20  arg1=password,. 
+000065c0: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
+000065d0: 7267 730a 2020 2020 2020 2020 290a 2020  rgs.        ).  
+000065e0: 2020 2020 2020 7265 7420 3d20 7265 735b        ret = res[
+000065f0: 2772 6574 7572 6e27 5d0a 2020 2020 2020  'return'].      
+00006600: 2020 6966 2072 6574 3a0a 2020 2020 2020    if ret:.      
+00006610: 2020 2020 2020 7365 6c66 2e5f 5f61 6e61        self.__ana
+00006620: 6c69 7a61 725f 6572 726f 7265 7328 7265  lizar_errores(re
+00006630: 7429 0a20 2020 2020 2020 2020 2020 2073  t).            s
+00006640: 656c 662e 4361 6e74 5061 6769 6e61 7320  elf.CantPaginas 
+00006650: 3d20 7265 742e 6765 7428 2763 616e 7450  = ret.get('cantP
+00006660: 6167 696e 6173 2729 0a20 2020 2020 2020  aginas').       
+00006670: 2020 2020 2073 656c 662e 4861 7945 7272       self.HayErr
+00006680: 6f72 203d 2072 6574 2e67 6574 2827 6861  or = ret.get('ha
+00006690: 795f 6572 726f 7227 290a 2020 2020 2020  y_error').      
+000066a0: 2020 2020 2020 7365 6c66 2e70 6172 616d        self.param
+000066b0: 735f 6f75 7420 3d20 6469 6374 280a 2020  s_out = dict(.  
+000066c0: 2020 2020 2020 2020 2020 2020 2020 5b28                [(
+000066d0: 692c 2069 7429 2066 6f72 2069 2c20 6974  i, it) for i, it
+000066e0: 2069 6e20 656e 756d 6572 6174 6528 7265   in enumerate(re
+000066f0: 742e 6765 7428 276c 6973 7427 2c20 5b5d  t.get('list', []
+00006700: 2929 5d29 0a20 2020 2020 2020 2020 2020  ))]).           
+00006710: 2072 6574 7572 6e20 6c65 6e28 7365 6c66   return len(self
+00006720: 2e70 6172 616d 735f 6f75 7429 0a20 2020  .params_out).   
+00006730: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00006740: 2020 2020 2020 2072 6574 7572 6e20 300a         return 0.
+00006750: 0a20 2020 2064 6566 2053 6574 5573 6572  .    def SetUser
+00006760: 6e61 6d65 2873 656c 662c 2075 7365 726e  name(self, usern
+00006770: 616d 6529 3a0a 2020 2020 2020 2020 2245  ame):.        "E
+00006780: 7374 6162 6c65 7a63 6f20 656c 206e 6f6d  stablezco el nom
+00006790: 6272 6520 6465 2075 7375 6172 696f 220a  bre de usuario".
+000067a0: 2020 2020 2020 2020 7365 6c66 2e55 7365          self.Use
+000067b0: 726e 616d 6520 3d20 7573 6572 6e61 6d65  rname = username
+000067c0: 0a0a 2020 2020 6465 6620 5365 7450 6173  ..    def SetPas
+000067d0: 7377 6f72 6428 7365 6c66 2c20 7061 7373  sword(self, pass
+000067e0: 776f 7264 293a 0a20 2020 2020 2020 2022  word):.        "
+000067f0: 4573 7461 626c 657a 636f 206c 6120 636f  Establezco la co
+00006800: 6e74 7261 7365 f161 220a 2020 2020 2020  ntrase.a".      
+00006810: 2020 7365 6c66 2e50 6173 7377 6f72 6420    self.Password 
+00006820: 3d20 7061 7373 776f 7264 0a0a 2020 2020  = password..    
+00006830: 6465 6620 4765 7443 6f64 6967 6f54 7261  def GetCodigoTra
+00006840: 6e73 6163 6369 6f6e 2873 656c 6629 3a0a  nsaccion(self):.
+00006850: 2020 2020 2020 2020 2244 6576 7565 6c76          "Devuelv
+00006860: 6f20 656c 2063 f364 6967 6f20 6465 2074  o el c.digo de t
+00006870: 7261 6e73 6163 6369 f36e 220a 2020 2020  ransacci.n".    
+00006880: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00006890: 436f 6469 676f 5472 616e 7361 6363 696f  CodigoTransaccio
+000068a0: 6e0a 0a20 2020 2064 6566 2047 6574 5265  n..    def GetRe
+000068b0: 7375 6c74 6164 6f28 7365 6c66 293a 0a20  sultado(self):. 
+000068c0: 2020 2020 2020 2022 4465 7675 656c 766f         "Devuelvo
+000068d0: 2065 6c20 7265 7375 6c74 6164 6f22 0a20   el resultado". 
+000068e0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000068f0: 6c66 2e52 6573 756c 7461 646f 0a0a 0a64  lf.Resultado...d
+00006900: 6566 206d 6169 6e28 293a 0a20 2020 2022  ef main():.    "
+00006910: 4675 6e63 69f3 6e20 7072 696e 6369 7061  Funci.n principa
+00006920: 6c20 6465 2070 7275 6562 6173 2028 6f62  l de pruebas (ob
+00006930: 7465 6e65 7220 4341 4529 220a 2020 2020  tener CAE)".    
+00006940: 696d 706f 7274 206f 730a 2020 2020 696d  import os.    im
+00006950: 706f 7274 2074 696d 650a 2020 2020 696d  port time.    im
+00006960: 706f 7274 2073 7973 0a20 2020 2067 6c6f  port sys.    glo
+00006970: 6261 6c20 5753 444c 2c20 4c4f 4341 5449  bal WSDL, LOCATI
+00006980: 4f4e 0a0a 2020 2020 4445 4255 4720 3d20  ON..    DEBUG = 
+00006990: 272d 2d64 6562 7567 2720 696e 2073 7973  '--debug' in sys
+000069a0: 2e61 7267 760a 2020 2020 7072 696e 7428  .argv.    print(
+000069b0: 4445 4255 4729 0a0a 2020 2020 7773 203d  DEBUG)..    ws =
+000069c0: 2054 7261 7a61 4d65 6428 290a 0a20 2020   TrazaMed()..   
+000069d0: 2077 732e 5573 6572 6e61 6d65 203d 2027   ws.Username = '
+000069e0: 7465 7374 7773 6572 7669 6365 270a 2020  testwservice'.  
+000069f0: 2020 7773 2e50 6173 7377 6f72 6420 3d20    ws.Password = 
+00006a00: 2774 6573 7477 7365 7276 6963 6570 7377  'testwservicepsw
+00006a10: 270a 0a20 2020 2069 6620 272d 2d70 726f  '..    if '--pro
+00006a20: 6427 2069 6e20 7379 732e 6172 6776 2061  d' in sys.argv a
+00006a30: 6e64 206e 6f74 2048 4f4d 4f3a 0a20 2020  nd not HOMO:.   
+00006a40: 2020 2020 2057 5344 4c20 3d20 2268 7474       WSDL = "htt
+00006a50: 7073 3a2f 2f74 7261 7a61 6269 6c69 6461  ps://trazabilida
+00006a60: 642e 7061 6d69 2e6f 7267 2e61 723a 3930  d.pami.org.ar:90
+00006a70: 3530 2f74 7261 7a61 6d65 642e 5765 6253  50/trazamed.WebS
+00006a80: 6572 7669 6365 220a 2020 2020 2020 2020  ervice".        
+00006a90: 7072 696e 7428 2255 7361 6e64 6f20 5753  print("Usando WS
+00006aa0: 444c 3a22 2c20 5753 444c 290a 2020 2020  DL:", WSDL).    
+00006ab0: 2020 2020 7379 732e 6172 6776 2e70 6f70      sys.argv.pop
+00006ac0: 2873 7973 2e61 7267 762e 696e 6465 7828  (sys.argv.index(
+00006ad0: 222d 2d70 726f 6422 2929 0a0a 2020 2020  "--prod"))..    
+00006ae0: 2320 496e 6963 6961 6c69 7a6f 206c 6173  # Inicializo las
+00006af0: 2076 6172 6961 626c 6573 2079 2065 7374   variables y est
+00006b00: 7275 6374 7572 6173 2070 6172 6120 656c  ructuras para el
+00006b10: 2061 7263 6869 766f 2064 6520 696e 7465   archivo de inte
+00006b20: 7263 616d 6269 6f3a 0a20 2020 206d 6564  rcambio:.    med
+00006b30: 6963 616d 656e 746f 7320 3d20 5b5d 0a20  icamentos = []. 
+00006b40: 2020 2074 7261 6e73 6163 6369 6f6e 6573     transacciones
+00006b50: 203d 205b 5d0a 2020 2020 6572 726f 7265   = [].    errore
+00006b60: 7320 3d20 5b5d 0a20 2020 2066 6f72 6d61  s = [].    forma
+00006b70: 746f 7320 3d20 5b0a 2020 2020 2020 2020  tos = [.        
+00006b80: 2827 4d65 6469 6361 6d65 6e74 6f73 272c  ('Medicamentos',
+00006b90: 204d 4544 4943 414d 454e 544f 532c 206d   MEDICAMENTOS, m
+00006ba0: 6564 6963 616d 656e 746f 7329 2c0a 2020  edicamentos),.  
+00006bb0: 2020 2020 2020 2827 5472 616e 7361 6363        ('Transacc
+00006bc0: 696f 6e65 7327 2c20 5452 414e 5341 4343  iones', TRANSACC
+00006bd0: 494f 4e45 532c 2074 7261 6e73 6163 6369  IONES, transacci
+00006be0: 6f6e 6573 292c 0a20 2020 2020 2020 2028  ones),.        (
+00006bf0: 2745 7272 6f72 6573 272c 2045 5252 4f52  'Errores', ERROR
+00006c00: 4553 2c20 6572 726f 7265 7329 2c0a 2020  ES, errores),.  
+00006c10: 2020 5d0a 0a20 2020 2069 6620 272d 2d66    ]..    if '--f
+00006c20: 6f72 6d61 746f 2720 696e 2073 7973 2e61  ormato' in sys.a
+00006c30: 7267 763a 0a20 2020 2020 2020 2070 7269  rgv:.        pri
+00006c40: 6e74 2822 466f 726d 6174 6f3a 2229 0a20  nt("Formato:"). 
+00006c50: 2020 2020 2020 2066 6f72 206d 7367 2c20         for msg, 
+00006c60: 666f 726d 6174 6f2c 206c 6973 7461 2069  formato, lista i
+00006c70: 6e20 666f 726d 6174 6f73 3a0a 2020 2020  n formatos:.    
+00006c80: 2020 2020 2020 2020 636f 6d69 656e 7a6f          comienzo
+00006c90: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
+00006ca0: 2070 7269 6e74 2822 3d3d 3d20 2573 203d   print("=== %s =
+00006cb0: 3d3d 2220 2520 6d73 6729 0a20 2020 2020  ==" % msg).     
+00006cc0: 2020 2020 2020 2070 7269 6e74 2822 7c7c         print("||
+00006cd0: 2025 2d32 3573 207c 7c20 252d 3132 7320   %-25s || %-12s 
+00006ce0: 7c7c 2025 2d35 7320 7c7c 2025 2d34 7320  || %-5s || %-4s 
+00006cf0: 7c7c 2025 2d31 3073 207c 7c22 2025 2028  || %-10s ||" % (
+00006d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006d10: 2022 4e6f 6d62 7265 222c 2022 5469 706f   "Nombre", "Tipo
+00006d20: 222c 2022 4c6f 6e67 2e22 2c20 2250 6f73  ", "Long.", "Pos
+00006d30: 2874 7874 2922 2c20 2243 616d 706f 2864  (txt)", "Campo(d
+00006d40: 6266 2922 2929 0a20 2020 2020 2020 2020  bf)")).         
+00006d50: 2020 2063 6c61 7665 7320 3d20 5b5d 0a20     claves = []. 
+00006d60: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
+00006d70: 6d74 2069 6e20 666f 726d 6174 6f3a 0a20  mt in formato:. 
+00006d80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00006d90: 6c61 7665 2c20 6c6f 6e67 6974 7564 2c20  lave, longitud, 
+00006da0: 7469 706f 203d 2066 6d74 5b30 3a33 5d0a  tipo = fmt[0:3].
+00006db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006dc0: 636c 6176 655f 6462 6620 3d20 6461 725f  clave_dbf = dar_
+00006dd0: 6e6f 6d62 7265 5f63 616d 706f 5f64 6266  nombre_campo_dbf
+00006de0: 2863 6c61 7665 2c20 636c 6176 6573 290a  (clave, claves).
+00006df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e00: 636c 6176 6573 2e61 7070 656e 6428 636c  claves.append(cl
+00006e10: 6176 655f 6462 6629 0a20 2020 2020 2020  ave_dbf).       
+00006e20: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00006e30: 7c7c 2025 2d32 3573 207c 7c20 252d 3132  || %-25s || %-12
+00006e40: 7320 7c7c 2025 3564 207c 7c20 2020 2534  s || %5d ||   %4
+00006e50: 6420 2020 7c7c 2025 2d31 3073 207c 7c22  d   || %-10s ||"
+00006e60: 2025 2028 0a20 2020 2020 2020 2020 2020   % (.           
+00006e70: 2020 2020 2020 2020 2063 6c61 7665 2c20           clave, 
+00006e80: 7469 706f 2c20 6c6f 6e67 6974 7564 2c20  tipo, longitud, 
+00006e90: 636f 6d69 656e 7a6f 2c20 636c 6176 655f  comienzo, clave_
+00006ea0: 6462 6629 290a 2020 2020 2020 2020 2020  dbf)).          
+00006eb0: 2020 2020 2020 636f 6d69 656e 7a6f 202b        comienzo +
+00006ec0: 3d20 6c6f 6e67 6974 7564 0a20 2020 2020  = longitud.     
+00006ed0: 2020 2073 7973 2e65 7869 7428 3029 0a0a     sys.exit(0)..
+00006ee0: 2020 2020 6966 2027 2d2d 6361 7267 6172      if '--cargar
+00006ef0: 2720 696e 2073 7973 2e61 7267 763a 0a20  ' in sys.argv:. 
+00006f00: 2020 2020 2020 2069 6620 272d 2d64 6266         if '--dbf
+00006f10: 2720 696e 2073 7973 2e61 7267 763a 0a20  ' in sys.argv:. 
+00006f20: 2020 2020 2020 2020 2020 206c 6565 725f             leer_
+00006f30: 6462 6628 666f 726d 6174 6f73 5b3a 315d  dbf(formatos[:1]
+00006f40: 2c20 7b7d 290a 2020 2020 2020 2020 656c  , {}).        el
+00006f50: 6966 2027 2d2d 6a73 6f6e 2720 696e 2073  if '--json' in s
+00006f60: 7973 2e61 7267 763a 0a20 2020 2020 2020  ys.argv:.       
+00006f70: 2020 2020 2066 6f72 2066 6f72 6d61 746f       for formato
+00006f80: 2069 6e20 666f 726d 6174 6f73 5b3a 315d   in formatos[:1]
+00006f90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006fa0: 2020 6172 6368 6976 6f20 3d20 6f70 656e    archivo = open
+00006fb0: 2866 6f72 6d61 746f 5b30 5d2e 6c6f 7765  (formato[0].lowe
+00006fc0: 7228 2920 2b20 222e 6a73 6f6e 222c 2022  r() + ".json", "
+00006fd0: 7222 290a 2020 2020 2020 2020 2020 2020  r").            
+00006fe0: 2020 2020 6420 3d20 6a73 6f6e 2e6c 6f61      d = json.loa
+00006ff0: 6428 6172 6368 6976 6f29 0a20 2020 2020  d(archivo).     
+00007000: 2020 2020 2020 2020 2020 2066 6f72 6d61             forma
+00007010: 746f 5b32 5d2e 6578 7465 6e64 2864 290a  to[2].extend(d).
+00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007030: 6172 6368 6976 6f2e 636c 6f73 6528 290a  archivo.close().
+00007040: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00007050: 2020 2020 2020 2020 2020 666f 7220 666f            for fo
+00007060: 726d 6174 6f20 696e 2066 6f72 6d61 746f  rmato in formato
+00007070: 735b 3a31 5d3a 0a20 2020 2020 2020 2020  s[:1]:.         
+00007080: 2020 2020 2020 2061 7263 6869 766f 203d         archivo =
+00007090: 206f 7065 6e28 666f 726d 6174 6f5b 305d   open(formato[0]
+000070a0: 2e6c 6f77 6572 2829 202b 2022 2e74 7874  .lower() + ".txt
+000070b0: 222c 2022 7222 290a 2020 2020 2020 2020  ", "r").        
+000070c0: 2020 2020 2020 2020 666f 7220 6c69 6e65          for line
+000070d0: 6120 696e 2061 7263 6869 766f 3a0a 2020  a in archivo:.  
+000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070f0: 2020 6420 3d20 6c65 6572 286c 696e 6561    d = leer(linea
+00007100: 2c20 666f 726d 6174 6f5b 315d 290a 2020  , formato[1]).  
+00007110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007120: 2020 666f 726d 6174 6f5b 325d 2e61 7070    formato[2].app
+00007130: 656e 6428 6429 0a20 2020 2020 2020 2020  end(d).         
+00007140: 2020 2020 2020 2061 7263 6869 766f 2e63         archivo.c
+00007150: 6c6f 7365 2829 0a0a 2020 2020 7773 2e43  lose()..    ws.C
+00007160: 6f6e 6563 7461 7228 2222 2c20 5753 444c  onectar("", WSDL
+00007170: 290a 0a20 2020 2069 6620 7773 2e45 7863  )..    if ws.Exc
+00007180: 6570 6369 6f6e 3a0a 2020 2020 2020 2020  epcion:.        
+00007190: 7072 696e 7428 7773 2e45 7863 6570 6369  print(ws.Excepci
+000071a0: 6f6e 290a 2020 2020 2020 2020 7072 696e  on).        prin
+000071b0: 7428 7773 2e54 7261 6365 6261 636b 290a  t(ws.Traceback).
+000071c0: 2020 2020 2020 2020 7379 732e 6578 6974          sys.exit
+000071d0: 282d 3129 0a0a 2020 2020 2320 4461 746f  (-1)..    # Dato
+000071e0: 7320 6465 2070 7275 6562 6173 3a0a 0a20  s de pruebas:.. 
+000071f0: 2020 2069 6620 272d 2d74 6573 7427 2069     if '--test' i
+00007200: 6e20 7379 732e 6172 6776 3a0a 2020 2020  n sys.argv:.    
+00007210: 2020 2020 6d65 6469 6361 6d65 6e74 6f73      medicamentos
+00007220: 2e61 7070 656e 6428 6469 6374 280a 2020  .append(dict(.  
+00007230: 2020 2020 2020 2020 2020 665f 6576 656e            f_even
+00007240: 746f 3d64 6174 6574 696d 652e 6461 7465  to=datetime.date
+00007250: 7469 6d65 2e6e 6f77 2829 2e73 7472 6674  time.now().strft
+00007260: 696d 6528 2225 642f 256d 2f25 5922 292c  ime("%d/%m/%Y"),
+00007270: 0a20 2020 2020 2020 2020 2020 2068 5f65  .            h_e
+00007280: 7665 6e74 6f3d 6461 7465 7469 6d65 2e64  vento=datetime.d
+00007290: 6174 6574 696d 652e 6e6f 7728 292e 7374  atetime.now().st
+000072a0: 7266 7469 6d65 2822 2548 3a25 4d22 292c  rftime("%H:%M"),
+000072b0: 0a20 2020 2020 2020 2020 2020 2067 6c6e  .            gln
+000072c0: 5f6f 7269 6765 6e3d 2239 3939 3939 3939  _origen="9999999
+000072d0: 3939 3939 3138 222c 2067 6c6e 5f64 6573  999918", gln_des
+000072e0: 7469 6e6f 3d22 676c 6e77 7322 2c0a 2020  tino="glnws",.  
+000072f0: 2020 2020 2020 2020 2020 6e5f 7265 6d69            n_remi
+00007300: 746f 3d22 5230 3030 3130 3030 3031 3233  to="R00010000123
+00007310: 3422 2c20 6e5f 6661 6374 7572 613d 2241  4", n_factura="A
+00007320: 3030 3031 3030 3030 3132 3334 222c 0a20  000100001234",. 
+00007330: 2020 2020 2020 2020 2020 2076 656e 6369             venci
+00007340: 6d69 656e 746f 3d28 0a20 2020 2020 2020  miento=(.       
+00007350: 2020 2020 2020 2020 2064 6174 6574 696d           datetim
+00007360: 652e 6461 7465 7469 6d65 2e6e 6f77 2829  e.datetime.now()
+00007370: 2b64 6174 6574 696d 652e 7469 6d65 6465  +datetime.timede
+00007380: 6c74 6128 3330 290a 2020 2020 2020 2020  lta(30).        
+00007390: 2020 2020 292e 7374 7266 7469 6d65 2822      ).strftime("
+000073a0: 2564 2f25 6d2f 2559 2229 2c0a 2020 2020  %d/%m/%Y"),.    
+000073b0: 2020 2020 2020 2020 6774 696e 3d22 4754          gtin="GT
+000073c0: 494e 3122 2c20 6c6f 7465 3d64 6174 6574  IN1", lote=datet
+000073d0: 696d 652e 6461 7465 7469 6d65 2e6e 6f77  ime.datetime.now
+000073e0: 2829 2e73 7472 6674 696d 6528 2225 5922  ().strftime("%Y"
+000073f0: 292c 0a20 2020 2020 2020 2020 2020 206e  ),.            n
+00007400: 756d 6572 6f5f 7365 7269 616c 3d69 6e74  umero_serial=int
+00007410: 2874 696d 652e 7469 6d65 2829 2a31 3029  (time.time()*10)
+00007420: 2c0a 2020 2020 2020 2020 2020 2020 6964  ,.            id
+00007430: 5f6f 6272 615f 736f 6369 616c 3d4e 6f6e  _obra_social=Non
+00007440: 652c 2069 645f 6576 656e 746f 3d31 3334  e, id_evento=134
+00007450: 2c0a 2020 2020 2020 2020 2020 2020 6375  ,.            cu
+00007460: 6974 5f6f 7269 6765 6e3d 2232 3032 3637  it_origen="20267
+00007470: 3536 3533 3933 222c 2063 7569 745f 6465  565393", cuit_de
+00007480: 7374 696e 6f3d 2232 3032 3637 3536 3533  stino="202675653
+00007490: 3933 222c 0a20 2020 2020 2020 2020 2020  93",.           
+000074a0: 2061 7065 6c6c 6964 6f3d 2252 6569 6e67   apellido="Reing
+000074b0: 6172 7422 2c20 6e6f 6d62 7265 733d 224d  art", nombres="M
+000074c0: 6172 6961 6e6f 222c 0a20 2020 2020 2020  ariano",.       
+000074d0: 2020 2020 2074 6970 6f5f 646f 6375 6d65       tipo_docume
+000074e0: 6e74 6f3d 2239 3622 2c20 6e5f 646f 6375  nto="96", n_docu
+000074f0: 6d65 6e74 6f3d 2232 3637 3536 3533 3922  mento="26756539"
+00007500: 2c20 7365 786f 3d22 4d22 2c0a 2020 2020  , sexo="M",.    
+00007510: 2020 2020 2020 2020 6469 7265 6363 696f          direccio
+00007520: 6e3d 2253 6172 617a 6122 2c20 6e75 6d65  n="Saraza", nume
+00007530: 726f 3d22 3132 3334 222c 2070 6973 6f3d  ro="1234", piso=
+00007540: 2222 2c20 6465 7074 6f3d 2222 2c0a 2020  "", depto="",.  
+00007550: 2020 2020 2020 2020 2020 6c6f 6361 6c69            locali
+00007560: 6461 643d 2248 7572 6c69 6e67 6861 6d22  dad="Hurlingham"
+00007570: 2c20 7072 6f76 696e 6369 613d 2242 7565  , provincia="Bue
+00007580: 6e6f 7320 4169 7265 7322 2c0a 2020 2020  nos Aires",.    
+00007590: 2020 2020 2020 2020 6e5f 706f 7374 616c          n_postal
+000075a0: 3d22 3136 3838 222c 2066 6563 6861 5f6e  ="1688", fecha_n
+000075b0: 6163 696d 6965 6e74 6f3d 2230 312f 3031  acimiento="01/01
+000075c0: 2f32 3030 3022 2c0a 2020 2020 2020 2020  /2000",.        
+000075d0: 2020 2020 7465 6c65 666f 6e6f 3d22 3535      telefono="55
+000075e0: 3535 2d35 3535 3522 2c0a 2020 2020 2020  55-5555",.      
+000075f0: 2020 2020 2020 6e72 6f5f 6173 6f63 6961        nro_asocia
+00007600: 646f 3d22 3939 3939 3939 3939 3939 3939  do="999999999999
+00007610: 3922 2c0a 2020 2020 2020 2020 2020 2020  9",.            
+00007620: 6361 6e74 6964 6164 3d4e 6f6e 652c 0a20  cantidad=None,. 
+00007630: 2020 2020 2020 2020 2020 2064 6573 6465             desde
+00007640: 5f6e 756d 6572 6f5f 7365 7269 616c 3d4e  _numero_serial=N
+00007650: 6f6e 652c 2068 6173 7461 5f6e 756d 6572  one, hasta_numer
+00007660: 6f5f 7365 7269 616c 3d4e 6f6e 652c 0a20  o_serial=None,. 
+00007670: 2020 2020 2020 2020 2020 2063 6f64 6967             codig
+00007680: 6f5f 7472 616e 7361 6363 696f 6e3d 4e6f  o_transaccion=No
+00007690: 6e65 2c0a 2020 2020 2020 2020 2929 0a20  ne,.        )). 
+000076a0: 2020 2069 6620 272d 2d74 6573 7466 7261     if '--testfra
+000076b0: 6363 696f 6e27 2069 6e20 7379 732e 6172  ccion' in sys.ar
+000076c0: 6776 3a0a 2020 2020 2020 2020 6d65 6469  gv:.        medi
+000076d0: 6361 6d65 6e74 6f73 2e61 7070 656e 6428  camentos.append(
+000076e0: 6469 6374 280a 2020 2020 2020 2020 2020  dict(.          
+000076f0: 2020 665f 6576 656e 746f 3d64 6174 6574    f_evento=datet
+00007700: 696d 652e 6461 7465 7469 6d65 2e6e 6f77  ime.datetime.now
+00007710: 2829 2e73 7472 6674 696d 6528 2225 642f  ().strftime("%d/
+00007720: 256d 2f25 5922 292c 0a20 2020 2020 2020  %m/%Y"),.       
+00007730: 2020 2020 2068 5f65 7665 6e74 6f3d 6461       h_evento=da
+00007740: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
+00007750: 6e6f 7728 292e 7374 7266 7469 6d65 2822  now().strftime("
+00007760: 2548 3a25 4d22 292c 0a20 2020 2020 2020  %H:%M"),.       
+00007770: 2020 2020 2067 6c6e 5f6f 7269 6765 6e3d       gln_origen=
+00007780: 2239 3939 3939 3939 3939 3939 3138 222c  "9999999999918",
+00007790: 2067 6c6e 5f64 6573 7469 6e6f 3d22 676c   gln_destino="gl
+000077a0: 6e77 7322 2c0a 2020 2020 2020 2020 2020  nws",.          
+000077b0: 2020 6e5f 7265 6d69 746f 3d22 3132 3334    n_remito="1234
+000077c0: 222c 206e 5f66 6163 7475 7261 3d22 3132  ", n_factura="12
+000077d0: 3334 222c 0a20 2020 2020 2020 2020 2020  34",.           
+000077e0: 2076 656e 6369 6d69 656e 746f 3d28 0a20   vencimiento=(. 
+000077f0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00007800: 6174 6574 696d 652e 6461 7465 7469 6d65  atetime.datetime
+00007810: 2e6e 6f77 2829 2b64 6174 6574 696d 652e  .now()+datetime.
+00007820: 7469 6d65 6465 6c74 6128 3330 290a 2020  timedelta(30).  
+00007830: 2020 2020 2020 2020 2020 292e 7374 7266            ).strf
+00007840: 7469 6d65 2822 2564 2f25 6d2f 2559 2229  time("%d/%m/%Y")
+00007850: 2c0a 2020 2020 2020 2020 2020 2020 6774  ,.            gt
+00007860: 696e 3d22 4754 494e 3122 2c20 6c6f 7465  in="GTIN1", lote
+00007870: 3d64 6174 6574 696d 652e 6461 7465 7469  =datetime.dateti
+00007880: 6d65 2e6e 6f77 2829 2e73 7472 6674 696d  me.now().strftim
+00007890: 6528 2225 5922 292c 0a20 2020 2020 2020  e("%Y"),.       
+000078a0: 2020 2020 206e 756d 6572 6f5f 7365 7269       numero_seri
+000078b0: 616c 3d69 6e74 2874 696d 652e 7469 6d65  al=int(time.time
+000078c0: 2829 2a31 3029 2c0a 2020 2020 2020 2020  ()*10),.        
+000078d0: 2020 2020 6964 5f6f 6272 615f 736f 6369      id_obra_soci
+000078e0: 616c 3d4e 6f6e 652c 2069 645f 6576 656e  al=None, id_even
+000078f0: 746f 3d31 3334 2c0a 2020 2020 2020 2020  to=134,.        
+00007900: 2020 2020 6375 6974 5f6f 7269 6765 6e3d      cuit_origen=
+00007910: 2232 3032 3637 3536 3533 3933 222c 2063  "20267565393", c
+00007920: 7569 745f 6465 7374 696e 6f3d 2232 3032  uit_destino="202
+00007930: 3637 3536 3533 3933 222c 0a20 2020 2020  67565393",.     
+00007940: 2020 2020 2020 2061 7065 6c6c 6964 6f3d         apellido=
+00007950: 2252 6569 6e67 6172 7422 2c20 6e6f 6d62  "Reingart", nomb
+00007960: 7265 733d 224d 6172 6961 6e6f 222c 0a20  res="Mariano",. 
+00007970: 2020 2020 2020 2020 2020 2074 6970 6f5f             tipo_
+00007980: 646f 6375 6d65 6e74 6f3d 2239 3622 2c20  documento="96", 
+00007990: 6e5f 646f 6375 6d65 6e74 6f3d 2232 3637  n_documento="267
+000079a0: 3536 3533 3922 2c20 7365 786f 3d22 4d22  56539", sexo="M"
+000079b0: 2c0a 2020 2020 2020 2020 2020 2020 6469  ,.            di
+000079c0: 7265 6363 696f 6e3d 2253 6172 617a 6122  reccion="Saraza"
+000079d0: 2c20 6e75 6d65 726f 3d22 3132 3334 222c  , numero="1234",
+000079e0: 2070 6973 6f3d 2222 2c20 6465 7074 6f3d   piso="", depto=
+000079f0: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
+00007a00: 6c6f 6361 6c69 6461 643d 2248 7572 6c69  localidad="Hurli
+00007a10: 6e67 6861 6d22 2c20 7072 6f76 696e 6369  ngham", provinci
+00007a20: 613d 2242 7565 6e6f 7320 4169 7265 7322  a="Buenos Aires"
+00007a30: 2c0a 2020 2020 2020 2020 2020 2020 6e5f  ,.            n_
+00007a40: 706f 7374 616c 3d22 3136 3838 222c 2066  postal="1688", f
+00007a50: 6563 6861 5f6e 6163 696d 6965 6e74 6f3d  echa_nacimiento=
+00007a60: 2230 312f 3031 2f32 3030 3022 2c0a 2020  "01/01/2000",.  
+00007a70: 2020 2020 2020 2020 2020 7465 6c65 666f            telefo
+00007a80: 6e6f 3d22 3535 3535 2d35 3535 3522 2c0a  no="5555-5555",.
+00007a90: 2020 2020 2020 2020 2020 2020 6e72 6f5f              nro_
+00007aa0: 6173 6f63 6961 646f 3d22 3939 3939 3939  asociado="999999
+00007ab0: 3939 3939 3939 3922 2c0a 2020 2020 2020  9999999",.      
+00007ac0: 2020 2020 2020 6361 6e74 6964 6164 3d35        cantidad=5
+00007ad0: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
+00007ae0: 7364 655f 6e75 6d65 726f 5f73 6572 6961  sde_numero_seria
+00007af0: 6c3d 4e6f 6e65 2c20 6861 7374 615f 6e75  l=None, hasta_nu
+00007b00: 6d65 726f 5f73 6572 6961 6c3d 4e6f 6e65  mero_serial=None
+00007b10: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
+00007b20: 6469 676f 5f74 7261 6e73 6163 6369 6f6e  digo_transaccion
+00007b30: 3d4e 6f6e 652c 0a20 2020 2020 2020 2029  =None,.        )
+00007b40: 290a 2020 2020 6966 2027 2d2d 7465 7374  ).    if '--test
+00007b50: 6468 2720 696e 2073 7973 2e61 7267 763a  dh' in sys.argv:
+00007b60: 0a20 2020 2020 2020 206d 6564 6963 616d  .        medicam
+00007b70: 656e 746f 732e 6170 7065 6e64 2864 6963  entos.append(dic
+00007b80: 7428 0a20 2020 2020 2020 2020 2020 2066  t(.            f
+00007b90: 5f65 7665 6e74 6f3d 6461 7465 7469 6d65  _evento=datetime
+00007ba0: 2e64 6174 6574 696d 652e 6e6f 7728 292e  .datetime.now().
+00007bb0: 7374 7266 7469 6d65 2822 2564 2f25 6d2f  strftime("%d/%m/
+00007bc0: 2559 2229 2c0a 2020 2020 2020 2020 2020  %Y"),.          
+00007bd0: 2020 685f 6576 656e 746f 3d64 6174 6574    h_evento=datet
+00007be0: 696d 652e 6461 7465 7469 6d65 2e6e 6f77  ime.datetime.now
+00007bf0: 2829 2e73 7472 6674 696d 6528 2225 483a  ().strftime("%H:
+00007c00: 254d 2229 2c0a 2020 2020 2020 2020 2020  %M"),.          
+00007c10: 2020 676c 6e5f 6f72 6967 656e 3d22 3939    gln_origen="99
+00007c20: 3939 3939 3939 3939 3931 3822 2c20 676c  99999999918", gl
+00007c30: 6e5f 6465 7374 696e 6f3d 2267 6c6e 7773  n_destino="glnws
+00007c40: 222c 0a20 2020 2020 2020 2020 2020 206e  ",.            n
+00007c50: 5f72 656d 6974 6f3d 2231 3233 3422 2c20  _remito="1234", 
+00007c60: 6e5f 6661 6374 7572 613d 2231 3233 3422  n_factura="1234"
+00007c70: 2c0a 2020 2020 2020 2020 2020 2020 7665  ,.            ve
+00007c80: 6e63 696d 6965 6e74 6f3d 280a 2020 2020  ncimiento=(.    
+00007c90: 2020 2020 2020 2020 2020 2020 6461 7465              date
+00007ca0: 7469 6d65 2e64 6174 6574 696d 652e 6e6f  time.datetime.no
+00007cb0: 7728 292b 6461 7465 7469 6d65 2e74 696d  w()+datetime.tim
+00007cc0: 6564 656c 7461 2833 3029 0a20 2020 2020  edelta(30).     
+00007cd0: 2020 2020 2020 2029 2e73 7472 6674 696d         ).strftim
+00007ce0: 6528 2225 642f 256d 2f25 5922 292c 0a20  e("%d/%m/%Y"),. 
+00007cf0: 2020 2020 2020 2020 2020 2067 7469 6e3d             gtin=
+00007d00: 2247 5449 4e31 222c 206c 6f74 653d 6461  "GTIN1", lote=da
+00007d10: 7465 7469 6d65 2e64 6174 6574 696d 652e  tetime.datetime.
+00007d20: 6e6f 7728 292e 7374 7266 7469 6d65 2822  now().strftime("
+00007d30: 2559 2229 2c0a 2020 2020 2020 2020 2020  %Y"),.          
+00007d40: 2020 6465 7364 655f 6e75 6d65 726f 5f73    desde_numero_s
+00007d50: 6572 6961 6c3d 696e 7428 7469 6d65 2e74  erial=int(time.t
+00007d60: 696d 6528 292a 3130 292d 312c 0a20 2020  ime()*10)-1,.   
+00007d70: 2020 2020 2020 2020 2068 6173 7461 5f6e           hasta_n
+00007d80: 756d 6572 6f5f 7365 7269 616c 3d69 6e74  umero_serial=int
+00007d90: 2874 696d 652e 7469 6d65 2829 2a31 3029  (time.time()*10)
+00007da0: 2b31 2c0a 2020 2020 2020 2020 2020 2020  +1,.            
+00007db0: 6964 5f6f 6272 615f 736f 6369 616c 3d4e  id_obra_social=N
+00007dc0: 6f6e 652c 2069 645f 6576 656e 746f 3d31  one, id_evento=1
+00007dd0: 3334 2c0a 2020 2020 2020 2020 2020 2020  34,.            
+00007de0: 6e72 6f5f 6173 6f63 6961 646f 3d22 3132  nro_asociado="12
+00007df0: 3334 222c 0a20 2020 2020 2020 2020 2020  34",.           
+00007e00: 2063 616e 7469 6461 643d 4e6f 6e65 2c20   cantidad=None, 
+00007e10: 6e75 6d65 726f 5f73 6572 6961 6c3d 4e6f  numero_serial=No
+00007e20: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00007e30: 636f 6469 676f 5f74 7261 6e73 6163 6369  codigo_transacci
+00007e40: 6f6e 3d4e 6f6e 652c 0a20 2020 2020 2020  on=None,.       
+00007e50: 2029 290a 0a20 2020 2023 204f 7063 696f   ))..    # Opcio
+00007e60: 6e65 7320 7072 696e 6369 7061 6c65 733a  nes principales:
+00007e70: 0a0a 2020 2020 6966 2027 2d2d 6361 6e63  ..    if '--canc
+00007e80: 656c 6127 2069 6e20 7379 732e 6172 6776  ela' in sys.argv
+00007e90: 3a0a 2020 2020 2020 2020 6966 2027 2d2d  :.        if '--
+00007ea0: 6c6f 6164 786d 6c27 2069 6e20 7379 732e  loadxml' in sys.
+00007eb0: 6172 6776 3a0a 2020 2020 2020 2020 2020  argv:.          
+00007ec0: 2020 7773 2e4c 6f61 6454 6573 7458 4d4c    ws.LoadTestXML
+00007ed0: 2822 7472 617a 616d 6564 5f63 616e 6365  ("trazamed_cance
+00007ee0: 6c61 5f65 7272 2e78 6d6c 2229 2020 2320  la_err.xml")  # 
+00007ef0: 6361 7267 6f20 7265 7370 7565 7374 610a  cargo respuesta.
+00007f00: 2020 2020 2020 2020 7773 2e53 656e 6443          ws.SendC
+00007f10: 616e 6365 6c61 6354 7261 6e73 6163 6328  ancelacTransacc(
+00007f20: 2a73 7973 2e61 7267 765b 7379 732e 6172  *sys.argv[sys.ar
+00007f30: 6776 2e69 6e64 6578 2822 2d2d 6361 6e63  gv.index("--canc
+00007f40: 656c 6122 292b 313a 5d29 0a20 2020 2065  ela")+1:]).    e
+00007f50: 6c69 6620 272d 2d63 616e 6365 6c61 5f70  lif '--cancela_p
+00007f60: 6172 6369 616c 2720 696e 2073 7973 2e61  arcial' in sys.a
+00007f70: 7267 763a 0a20 2020 2020 2020 2077 732e  rgv:.        ws.
+00007f80: 5365 6e64 4361 6e63 656c 6163 5472 616e  SendCancelacTran
+00007f90: 7361 6363 5061 7263 6961 6c28 0a20 2020  saccParcial(.   
+00007fa0: 2020 2020 2020 2020 202a 7379 732e 6172           *sys.ar
+00007fb0: 6776 5b73 7973 2e61 7267 762e 696e 6465  gv[sys.argv.inde
+00007fc0: 7828 222d 2d63 616e 6365 6c61 5f70 6172  x("--cancela_par
+00007fd0: 6369 616c 2229 2b31 3a5d 290a 2020 2020  cial")+1:]).    
+00007fe0: 656c 6966 2027 2d2d 636f 6e66 6972 6d61  elif '--confirma
+00007ff0: 2720 696e 2073 7973 2e61 7267 763a 0a20  ' in sys.argv:. 
+00008000: 2020 2020 2020 2069 6620 272d 2d6c 6f61         if '--loa
+00008010: 6478 6d6c 2720 696e 2073 7973 2e61 7267  dxml' in sys.arg
+00008020: 763a 0a20 2020 2020 2020 2020 2020 2077  v:.            w
+00008030: 732e 4c6f 6164 5465 7374 584d 4c28 2274  s.LoadTestXML("t
+00008040: 7261 7a61 6d65 645f 636f 6e66 6972 6d61  razamed_confirma
+00008050: 2e78 6d6c 2229 2020 2320 6361 7267 6f20  .xml")  # cargo 
+00008060: 7265 7370 7565 7374 610a 2020 2020 2020  respuesta.      
+00008070: 2020 2020 2020 6f6b 203d 2077 732e 5365        ok = ws.Se
+00008080: 6e64 436f 6e66 6972 6d61 5472 616e 7361  ndConfirmaTransa
+00008090: 6363 280a 2020 2020 2020 2020 2020 2020  cc(.            
+000080a0: 2020 2020 7573 7561 7269 6f3d 2270 7275      usuario="pru
+000080b0: 6562 6173 7773 222c 2070 6173 7377 6f72  ebasws", passwor
+000080c0: 643d 2270 7275 6562 6173 7773 222c 0a20  d="pruebasws",. 
+000080d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000080e0: 5f69 6473 5f74 7261 6e73 6163 3d22 3122  _ids_transac="1"
+000080f0: 2c20 665f 6f70 6572 6163 696f 6e3d 2233  , f_operacion="3
+00008100: 312d 3132 2d32 3031 3322 290a 2020 2020  1-12-2013").    
+00008110: 2020 2020 2020 2020 6966 206e 6f74 206f          if not o
+00008120: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
+00008130: 2020 2072 6169 7365 2052 756e 7469 6d65     raise Runtime
+00008140: 4572 726f 7228 7773 2e45 7863 6570 6369  Error(ws.Excepci
+00008150: 6f6e 290a 2020 2020 2020 2020 7773 2e53  on).        ws.S
+00008160: 656e 6443 6f6e 6669 726d 6154 7261 6e73  endConfirmaTrans
+00008170: 6163 6328 2a73 7973 2e61 7267 765b 7379  acc(*sys.argv[sy
+00008180: 732e 6172 6776 2e69 6e64 6578 2822 2d2d  s.argv.index("--
+00008190: 636f 6e66 6972 6d61 2229 2b31 3a5d 290a  confirma")+1:]).
+000081a0: 2020 2020 656c 6966 2027 2d2d 616c 6572      elif '--aler
+000081b0: 7461 2720 696e 2073 7973 2e61 7267 763a  ta' in sys.argv:
+000081c0: 0a20 2020 2020 2020 2077 732e 5365 6e64  .        ws.Send
+000081d0: 416c 6572 7461 5472 616e 7361 6363 282a  AlertaTransacc(*
+000081e0: 7379 732e 6172 6776 5b73 7973 2e61 7267  sys.argv[sys.arg
+000081f0: 762e 696e 6465 7828 222d 2d61 6c65 7274  v.index("--alert
+00008200: 6122 292b 313a 5d29 0a20 2020 2065 6c69  a")+1:]).    eli
+00008210: 6620 272d 2d63 6f6e 7375 6c74 6127 2069  f '--consulta' i
+00008220: 6e20 7379 732e 6172 6776 3a0a 2020 2020  n sys.argv:.    
+00008230: 2020 2020 6966 2027 2d2d 616c 6572 7461      if '--alerta
+00008240: 646f 7327 2069 6e20 7379 732e 6172 6776  dos' in sys.argv
+00008250: 3a0a 2020 2020 2020 2020 2020 2020 7773  :.            ws
+00008260: 2e47 6574 456e 7669 6f73 5072 6f70 696f  .GetEnviosPropio
+00008270: 7341 6c65 7274 6164 6f73 280a 2020 2020  sAlertados(.    
+00008280: 2020 2020 2020 2020 2020 2020 2a73 7973              *sys
+00008290: 2e61 7267 765b 7379 732e 6172 6776 2e69  .argv[sys.argv.i
+000082a0: 6e64 6578 2822 2d2d 616c 6572 7461 646f  ndex("--alertado
+000082b0: 7322 292b 313a 5d0a 2020 2020 2020 2020  s")+1:].        
+000082c0: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
+000082d0: 6966 2027 2d2d 6d6f 7669 6d69 656e 746f  if '--movimiento
+000082e0: 7327 2069 6e20 7379 732e 6172 6776 3a0a  s' in sys.argv:.
+000082f0: 2020 2020 2020 2020 2020 2020 7773 2e47              ws.G
+00008300: 6574 5472 616e 7361 6363 696f 6e65 7357  etTransaccionesW
+00008310: 5328 0a20 2020 2020 2020 2020 2020 2020  S(.             
+00008320: 2020 202a 7379 732e 6172 6776 5b73 7973     *sys.argv[sys
+00008330: 2e61 7267 762e 696e 6465 7828 222d 2d6d  .argv.index("--m
+00008340: 6f76 696d 6965 6e74 6f73 2229 2b31 3a5d  ovimientos")+1:]
+00008350: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00008360: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00008370: 2020 2020 2020 2020 2077 732e 4765 7454           ws.GetT
+00008380: 7261 6e73 6163 6369 6f6e 6573 4e6f 436f  ransaccionesNoCo
+00008390: 6e66 6972 6d61 6461 7328 0a20 2020 2020  nfirmadas(.     
+000083a0: 2020 2020 2020 2020 2020 202a 7379 732e             *sys.
+000083b0: 6172 6776 5b73 7973 2e61 7267 762e 696e  argv[sys.argv.in
+000083c0: 6465 7828 222d 2d63 6f6e 7375 6c74 6122  dex("--consulta"
+000083d0: 292b 313a 5d0a 2020 2020 2020 2020 2020  )+1:].          
+000083e0: 2020 2020 2020 2320 7573 7561 7269 6f3d        # usuario=
+000083f0: 2270 7275 6562 6173 7773 222c 2070 6173  "pruebasws", pas
+00008400: 7377 6f72 643d 2270 7275 6562 6173 7773  sword="pruebasws
+00008410: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00008420: 2020 2023 2070 5f69 645f 7472 616e 7361     # p_id_transa
+00008430: 6363 696f 6e5f 676c 6f62 616c 3d22 3132  ccion_global="12
+00008440: 3334 222c 0a20 2020 2020 2020 2020 2020  34",.           
+00008450: 2020 2020 2023 2069 645f 6167 656e 7465       # id_agente
+00008460: 5f69 6e66 6f72 6d61 646f 723d 2231 222c  _informador="1",
+00008470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008480: 2023 2069 645f 6167 656e 7465 5f6f 7269   # id_agente_ori
+00008490: 6765 6e3d 2231 222c 0a20 2020 2020 2020  gen="1",.       
+000084a0: 2020 2020 2020 2020 2023 2069 645f 6167           # id_ag
+000084b0: 656e 7465 5f64 6573 7469 6e6f 3d22 3122  ente_destino="1"
+000084c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000084d0: 2020 2320 6964 5f6d 6564 6963 616d 656e    # id_medicamen
+000084e0: 746f 3d22 3122 2c0a 2020 2020 2020 2020  to="1",.        
+000084f0: 2020 2020 2020 2020 2320 6964 5f65 7665          # id_eve
+00008500: 6e74 6f3d 2231 222c 0a20 2020 2020 2020  nto="1",.       
+00008510: 2020 2020 2020 2020 2023 2066 6563 6861           # fecha
+00008520: 5f64 6573 6465 5f6f 703d 2230 312f 3031  _desde_op="01/01
+00008530: 2f32 3031 3522 2c0a 2020 2020 2020 2020  /2015",.        
+00008540: 2020 2020 2020 2020 2320 6665 6368 615f          # fecha_
+00008550: 6861 7374 615f 6f70 3d22 3331 2f31 322f  hasta_op="31/12/
+00008560: 3230 3133 222c 0a20 2020 2020 2020 2020  2013",.         
+00008570: 2020 2020 2020 2023 2066 6563 6861 5f64         # fecha_d
+00008580: 6573 6465 5f74 3d22 3031 2f30 312f 3230  esde_t="01/01/20
+00008590: 3133 222c 0a20 2020 2020 2020 2020 2020  13",.           
+000085a0: 2020 2020 2023 2066 6563 6861 5f68 6173       # fecha_has
+000085b0: 7461 5f74 3d22 3331 2f31 322f 3230 3133  ta_t="31/12/2013
+000085c0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000085d0: 2020 2023 2066 6563 6861 5f64 6573 6465     # fecha_desde
+000085e0: 5f76 3d22 3031 2f30 342f 3230 3133 222c  _v="01/04/2013",
+000085f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008600: 2023 2066 6563 6861 5f68 6173 7461 5f76   # fecha_hasta_v
+00008610: 3d22 3330 2f30 342f 3230 3133 222c 0a20  ="30/04/2013",. 
+00008620: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00008630: 206e 5f66 6163 7475 7261 3d35 2c20 6e5f   n_factura=5, n_
+00008640: 7265 6d69 746f 3d36 2c0a 2020 2020 2020  remito=6,.      
+00008650: 2020 2020 2020 2020 2020 2320 6573 7461            # esta
+00008660: 646f 3d31 2c0a 2020 2020 2020 2020 2020  do=1,.          
+00008670: 2020 2020 2020 2320 6c6f 7465 3d38 3837        # lote=887
+00008680: 3435 2c0a 2020 2020 2020 2020 2020 2020  45,.            
+00008690: 2020 2020 2320 6e75 6d65 726f 5f73 6572      # numero_ser
+000086a0: 6961 6c3d 3839 3431 3234 3738 382c 0a20  ial=894124788,. 
+000086b0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000086c0: 2020 2020 2070 7269 6e74 2822 4361 6e74       print("Cant
+000086d0: 5061 6769 6e61 7322 2c20 7773 2e43 616e  Paginas", ws.Can
+000086e0: 7450 6167 696e 6173 290a 2020 2020 2020  tPaginas).      
+000086f0: 2020 7072 696e 7428 2248 6179 4572 726f    print("HayErro
+00008700: 7222 2c20 7773 2e48 6179 4572 726f 7229  r", ws.HayError)
+00008710: 0a20 2020 2020 2020 2023 2070 7269 6e74  .        # print
+00008720: 2822 5472 616e 7361 6363 696f 6e50 6c61  ("TransaccionPla
+00008730: 696e 5753 222c 2077 732e 5472 616e 7361  inWS", ws.Transa
+00008740: 6363 696f 6e50 6c61 696e 5753 290a 2020  ccionPlainWS).  
+00008750: 2020 2020 2020 2320 7061 7261 6d65 7472        # parametr
+00008760: 6f73 2063 6f6d 756e 6573 2064 6520 7361  os comunes de sa
+00008770: 6c69 6461 2028 636f 6c75 6d6e 6173 2064  lida (columnas d
+00008780: 6520 6c61 2074 6162 6c61 293a 0a20 2020  e la tabla):.   
+00008790: 2020 2020 2063 6c61 7665 7320 3d20 5b6b       claves = [k
+000087a0: 2066 6f72 206b 2c20 762c 206c 2069 6e20   for k, v, l in 
+000087b0: 5452 414e 5341 4343 494f 4e45 535d 0a20  TRANSACCIONES]. 
+000087c0: 2020 2020 2020 2023 2065 7874 6965 6e64         # extiend
+000087d0: 6f20 6c61 206c 6973 7461 2064 6520 7265  o la lista de re
+000087e0: 7375 6c74 6164 6f20 7061 7261 2065 6c20  sultado para el 
+000087f0: 6172 6368 6976 6f20 6465 2069 6e74 6572  archivo de inter
+00008800: 6361 6d62 696f 3a0a 2020 2020 2020 2020  cambio:.        
+00008810: 7472 616e 7361 6363 696f 6e65 732e 6578  transacciones.ex
+00008820: 7465 6e64 2877 732e 5472 616e 7361 6363  tend(ws.Transacc
+00008830: 696f 6e50 6c61 696e 5753 290a 2020 2020  ionPlainWS).    
+00008840: 2020 2020 2320 656e 6361 6265 7a61 646f      # encabezado
+00008850: 2064 6520 6c61 2074 6162 6c61 3a0a 2020   de la tabla:.  
+00008860: 2020 2020 2020 7072 696e 7428 227c 7c22        print("||"
+00008870: 2c20 227c 7c22 2e6a 6f69 6e28 5b22 2573  , "||".join(["%s
+00008880: 2220 2520 636c 6176 6520 666f 7220 636c  " % clave for cl
+00008890: 6176 6520 696e 2063 6c61 7665 735d 292c  ave in claves]),
+000088a0: 2022 7c7c 2229 0a20 2020 2020 2020 2023   "||").        #
+000088b0: 2072 6563 6f72 726f 206c 6f73 2064 6174   recorro los dat
+000088c0: 6f73 2064 6576 7565 6c74 6f73 2028 5472  os devueltos (Tr
+000088d0: 616e 7361 6363 696f 6e50 6c61 696e 5753  ansaccionPlainWS
+000088e0: 293a 0a20 2020 2020 2020 2077 6869 6c65  ):.        while
+000088f0: 2077 732e 4c65 6572 5472 616e 7361 6363   ws.LeerTransacc
+00008900: 696f 6e28 293a 0a20 2020 2020 2020 2020  ion():.         
+00008910: 2020 2066 6f72 2063 6c61 7665 2069 6e20     for clave in 
+00008920: 636c 6176 6573 3a0a 2020 2020 2020 2020  claves:.        
+00008930: 2020 2020 2020 2020 7072 696e 7428 227c          print("|
+00008940: 7c22 2c20 7773 2e47 6574 5061 7261 6d65  |", ws.GetParame
+00008950: 7472 6f28 636c 6176 6529 2920 2020 2020  tro(clave))     
+00008960: 2020 2020 2320 696d 7072 696d 6f20 6361      # imprimo ca
+00008970: 6461 2066 696c 610a 2020 2020 2020 2020  da fila.        
+00008980: 2020 2020 7072 696e 7428 227c 7c22 290a      print("||").
+00008990: 2020 2020 656c 6966 2027 2d2d 6361 7461      elif '--cata
+000089a0: 6c6f 676f 2720 696e 2073 7973 2e61 7267  logo' in sys.arg
+000089b0: 763a 0a20 2020 2020 2020 2072 6574 203d  v:.        ret =
+000089c0: 2077 732e 4765 7443 6174 616c 6f67 6f45   ws.GetCatalogoE
+000089d0: 6c65 6374 726f 6e69 636f 4279 4754 494e  lectronicoByGTIN
+000089e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000089f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a00: 2020 2a73 7973 2e61 7267 765b 7379 732e    *sys.argv[sys.
+00008a10: 6172 6776 2e69 6e64 6578 2822 2d2d 6361  argv.index("--ca
+00008a20: 7461 6c6f 676f 2229 2b31 3a5d 0a20 2020  talogo")+1:].   
+00008a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a40: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00008a50: 2020 2020 2020 2066 6f72 2063 6174 616c         for catal
+00008a60: 6f67 6f20 696e 2077 732e 7061 7261 6d73  ogo in ws.params
+00008a70: 5f6f 7574 2e76 616c 7565 7328 293a 0a20  _out.values():. 
+00008a80: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00008a90: 2863 6174 616c 6f67 6f29 2020 2020 2020  (catalogo)      
+00008aa0: 2020 2320 696d 7072 696d 6f20 6361 6461    # imprimo cada
+00008ab0: 2066 696c 6129 0a20 2020 2065 6c69 6620   fila).    elif 
+00008ac0: 272d 2d73 746f 636b 2720 696e 2073 7973  '--stock' in sys
+00008ad0: 2e61 7267 763a 0a20 2020 2020 2020 2072  .argv:.        r
+00008ae0: 6574 203d 2077 732e 4765 7443 6f6e 7375  et = ws.GetConsu
+00008af0: 6c74 6153 746f 636b 280a 2020 2020 2020  ltaStock(.      
+00008b00: 2020 2020 2020 2a73 7973 2e61 7267 765b        *sys.argv[
+00008b10: 7379 732e 6172 6776 2e69 6e64 6578 2822  sys.argv.index("
+00008b20: 2d2d 7374 6f63 6b22 292b 313a 5d0a 2020  --stock")+1:].  
+00008b30: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00008b40: 7072 696e 7428 7265 7429 0a20 2020 2020  print(ret).     
+00008b50: 2020 2070 7269 6e74 2822 5c6e 222e 6a6f     print("\n".jo
+00008b60: 696e 285b 7374 7228 7329 2066 6f72 2073  in([str(s) for s
+00008b70: 2069 6e20 7773 2e70 6172 616d 735f 6f75   in ws.params_ou
+00008b80: 742e 7661 6c75 6573 2829 5d29 290a 2020  t.values()])).  
+00008b90: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00008ba0: 6172 6776 203d 205b 6172 6776 2066 6f72  argv = [argv for
+00008bb0: 2061 7267 7620 696e 2073 7973 2e61 7267   argv in sys.arg
+00008bc0: 7620 6966 206e 6f74 2061 7267 762e 7374  v if not argv.st
+00008bd0: 6172 7473 7769 7468 2822 2d2d 2229 5d0a  artswith("--")].
+00008be0: 2020 2020 2020 2020 6966 206e 6f74 206d          if not m
+00008bf0: 6564 6963 616d 656e 746f 733a 0a20 2020  edicamentos:.   
+00008c00: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00008c10: 6172 6776 2920 3e20 3136 3a0a 2020 2020  argv) > 16:.    
+00008c20: 2020 2020 2020 2020 2020 2020 6966 2027              if '
+00008c30: 2d2d 6468 2720 696e 2073 7973 2e61 7267  --dh' in sys.arg
+00008c40: 763a 0a20 2020 2020 2020 2020 2020 2020  v:.             
+00008c50: 2020 2020 2020 2077 732e 5365 6e64 4d65         ws.SendMe
+00008c60: 6469 6361 6d65 6e74 6f73 4448 5365 7269  dicamentosDHSeri
+00008c70: 6528 2a61 7267 765b 313a 5d29 0a20 2020  e(*argv[1:]).   
+00008c80: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00008c90: 6620 272d 2d66 7261 6363 696f 6e27 2069  f '--fraccion' i
+00008ca0: 6e20 7379 732e 6172 6776 3a0a 2020 2020  n sys.argv:.    
+00008cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008cc0: 7773 2e53 656e 644d 6564 6963 616d 656e  ws.SendMedicamen
+00008cd0: 746f 7346 7261 6363 696f 6e28 2a61 7267  tosFraccion(*arg
+00008ce0: 765b 313a 5d29 0a20 2020 2020 2020 2020  v[1:]).         
+00008cf0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00008d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d10: 2077 732e 5365 6e64 4d65 6469 6361 6d65   ws.SendMedicame
+00008d20: 6e74 6f73 282a 6172 6776 5b31 3a5d 290a  ntos(*argv[1:]).
+00008d30: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00008d40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00008d50: 2020 7072 696e 7428 2245 5252 4f52 3a20    print("ERROR: 
+00008d60: 6e6f 2073 6520 696e 6469 6361 726f 6e20  no se indicaron 
+00008d70: 746f 646f 7320 6c6f 7320 7061 72e1 6d65  todos los par.me
+00008d80: 7472 6f73 2072 6571 7565 7269 646f 7322  tros requeridos"
+00008d90: 290a 2020 2020 2020 2020 656c 6966 206d  ).        elif m
+00008da0: 6564 6963 616d 656e 746f 733a 0a20 2020  edicamentos:.   
+00008db0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+00008dc0: 2020 2020 2020 2020 2020 2020 2020 7573                us
+00008dd0: 7561 7269 6f2c 2070 6173 7377 6f72 6420  uario, password 
+00008de0: 3d20 6172 6776 5b31 3a33 5d0a 2020 2020  = argv[1:3].    
+00008df0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00008e00: 7863 6570 7469 6f6e 2061 7320 653a 0a20  xception as e:. 
+00008e10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00008e20: 7269 6e74 280a 2020 2020 2020 2020 2020  rint(.          
+00008e30: 2020 2020 2020 2020 2020 2241 4456 4552            "ADVER
+00008e40: 5445 4e43 4941 3a20 6e6f 2073 6520 696e  TENCIA: no se in
+00008e50: 6469 636f 2070 6172 e16d 6574 726f 7320  dico par.metros 
+00008e60: 7573 7561 7269 6f20 7920 7061 7373 6f77  usuario y passow
+00008e70: 6f72 6422 0a20 2020 2020 2020 2020 2020  ord".           
+00008e80: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00008e90: 2020 2020 2020 2070 7269 6e74 2865 290a         print(e).
+00008ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008eb0: 7573 7561 7269 6f20 3d20 7061 7373 776f  usuario = passwo
+00008ec0: 7264 203d 2022 7072 7565 6261 7377 7322  rd = "pruebasws"
+00008ed0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00008ee0: 2069 2c20 6d65 6420 696e 2065 6e75 6d65   i, med in enume
+00008ef0: 7261 7465 286d 6564 6963 616d 656e 746f  rate(medicamento
+00008f00: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00008f10: 2020 2020 7072 696e 7428 2250 726f 6365      print("Proce
+00008f20: 7361 6e64 6f20 7265 6769 7374 726f 222c  sando registro",
+00008f30: 2069 290a 2020 2020 2020 2020 2020 2020   i).            
+00008f40: 2020 2020 6465 6c20 6d65 645b 2763 6f64      del med['cod
+00008f50: 6967 6f5f 7472 616e 7361 6363 696f 6e27  igo_transaccion'
+00008f60: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00008f70: 2020 6966 206d 6564 2e67 6574 2822 6361    if med.get("ca
+00008f80: 6e74 6964 6164 2229 3a0a 2020 2020 2020  ntidad"):.      
+00008f90: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00008fa0: 6c20 6d65 645b 2264 6573 6465 5f6e 756d  l med["desde_num
+00008fb0: 6572 6f5f 7365 7269 616c 225d 0a20 2020  ero_serial"].   
+00008fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fd0: 2064 656c 206d 6564 5b22 6861 7374 615f   del med["hasta_
+00008fe0: 6e75 6d65 726f 5f73 6572 6961 6c22 5d0a  numero_serial"].
+00008ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009000: 2020 2020 7773 2e53 656e 644d 6564 6963      ws.SendMedic
+00009010: 616d 656e 746f 7346 7261 6363 696f 6e28  amentosFraccion(
+00009020: 7573 7561 7269 6f2c 2070 6173 7377 6f72  usuario, passwor
+00009030: 642c 202a 2a6d 6564 290a 2020 2020 2020  d, **med).      
+00009040: 2020 2020 2020 2020 2020 656c 6966 206d            elif m
+00009050: 6564 2e67 6574 2822 6465 7364 655f 6e75  ed.get("desde_nu
+00009060: 6d65 726f 5f73 6572 6961 6c22 293a 0a20  mero_serial"):. 
+00009070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009080: 2020 2064 656c 206d 6564 5b22 6361 6e74     del med["cant
+00009090: 6964 6164 225d 0a20 2020 2020 2020 2020  idad"].         
+000090a0: 2020 2020 2020 2020 2020 2064 656c 206d             del m
+000090b0: 6564 5b22 6e75 6d65 726f 5f73 6572 6961  ed["numero_seria
+000090c0: 6c22 5d0a 2020 2020 2020 2020 2020 2020  l"].            
+000090d0: 2020 2020 2020 2020 7773 2e53 656e 644d          ws.SendM
+000090e0: 6564 6963 616d 656e 746f 7344 4853 6572  edicamentosDHSer
+000090f0: 6965 2875 7375 6172 696f 2c20 7061 7373  ie(usuario, pass
+00009100: 776f 7264 2c20 2a2a 6d65 6429 0a20 2020  word, **med).   
+00009110: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00009120: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00009130: 2020 2020 2020 2064 656c 206d 6564 5b22         del med["
+00009140: 6361 6e74 6964 6164 225d 0a20 2020 2020  cantidad"].     
+00009150: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00009160: 656c 206d 6564 5b22 6465 7364 655f 6e75  el med["desde_nu
+00009170: 6d65 726f 5f73 6572 6961 6c22 5d0a 2020  mero_serial"].  
+00009180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009190: 2020 6465 6c20 6d65 645b 2268 6173 7461    del med["hasta
+000091a0: 5f6e 756d 6572 6f5f 7365 7269 616c 225d  _numero_serial"]
+000091b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000091c0: 2020 2020 2077 732e 5365 6e64 4d65 6469       ws.SendMedi
+000091d0: 6361 6d65 6e74 6f73 2875 7375 6172 696f  camentos(usuario
+000091e0: 2c20 7061 7373 776f 7264 2c20 2a2a 6d65  , password, **me
+000091f0: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
+00009200: 2020 206d 6564 5b27 636f 6469 676f 5f74     med['codigo_t
+00009210: 7261 6e73 6163 6369 6f6e 275d 203d 2077  ransaccion'] = w
+00009220: 732e 436f 6469 676f 5472 616e 7361 6363  s.CodigoTransacc
+00009230: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+00009240: 2020 2020 6572 726f 7265 732e 6578 7465      errores.exte
+00009250: 6e64 2877 732e 6572 726f 7265 7329 0a20  nd(ws.errores). 
+00009260: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00009270: 7269 6e74 2822 7c52 6573 756c 7461 646f  rint("|Resultado
+00009280: 2025 3573 7c43 6f64 6967 6f54 7261 6e73   %5s|CodigoTrans
+00009290: 6163 6369 6f6e 2025 3130 737c 4572 726f  accion %10s|Erro
+000092a0: 7265 737c 2573 7c22 2025 2028 0a20 2020  res|%s|" % (.   
+000092b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092c0: 2077 732e 5265 7375 6c74 6164 6f2c 0a20   ws.Resultado,. 
+000092d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092e0: 2020 2077 732e 436f 6469 676f 5472 616e     ws.CodigoTran
+000092f0: 7361 6363 696f 6e2c 0a20 2020 2020 2020  saccion,.       
+00009300: 2020 2020 2020 2020 2020 2020 2027 7c27               '|'
+00009310: 2e6a 6f69 6e28 7773 2e45 7272 6f72 6573  .join(ws.Errores
+00009320: 206f 7220 5b5d 292c 0a20 2020 2020 2020   or []),.       
+00009330: 2020 2020 2020 2020 2029 290a 2020 2020           )).    
+00009340: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00009350: 2020 2020 2020 7072 696e 7428 2245 5252        print("ERR
+00009360: 4f52 3a20 6e6f 2073 6520 6573 7065 6369  OR: no se especi
+00009370: 6669 6361 726f 6e20 6d65 6469 6361 6d65  ficaron medicame
+00009380: 6e74 6f73 2061 2069 6e66 6f72 6d61 7222  ntos a informar"
+00009390: 290a 0a20 2020 2069 6620 6e6f 7420 6d65  )..    if not me
+000093a0: 6469 6361 6d65 6e74 6f73 3a0a 2020 2020  dicamentos:.    
+000093b0: 2020 2020 7072 696e 7428 227c 5265 7375      print("|Resu
+000093c0: 6c74 6164 6f20 2535 737c 436f 6469 676f  ltado %5s|Codigo
+000093d0: 5472 616e 7361 6363 696f 6e20 2531 3073  Transaccion %10s
+000093e0: 7c45 7272 6f72 6573 7c25 737c 2220 2520  |Errores|%s|" % 
+000093f0: 280a 2020 2020 2020 2020 2020 2020 7773  (.            ws
+00009400: 2e52 6573 756c 7461 646f 2c0a 2020 2020  .Resultado,.    
+00009410: 2020 2020 2020 2020 7773 2e43 6f64 6967          ws.Codig
+00009420: 6f54 7261 6e73 6163 6369 6f6e 2c0a 2020  oTransaccion,.  
+00009430: 2020 2020 2020 2020 2020 277c 272e 6a6f            '|'.jo
+00009440: 696e 2877 732e 4572 726f 7265 7320 6f72  in(ws.Errores or
+00009450: 205b 5d29 2c0a 2020 2020 2020 2020 2929   []),.        ))
+00009460: 0a0a 2020 2020 6966 2077 732e 4578 6365  ..    if ws.Exce
+00009470: 7063 696f 6e3a 0a20 2020 2020 2020 2070  pcion:.        p
+00009480: 7269 6e74 2877 732e 5472 6163 6562 6163  rint(ws.Tracebac
+00009490: 6b29 0a0a 2020 2020 6966 2027 2d2d 6772  k)..    if '--gr
+000094a0: 6162 6172 2720 696e 2073 7973 2e61 7267  abar' in sys.arg
+000094b0: 763a 0a20 2020 2020 2020 2069 6620 272d  v:.        if '-
+000094c0: 2d64 6266 2720 696e 2073 7973 2e61 7267  -dbf' in sys.arg
+000094d0: 763a 0a20 2020 2020 2020 2020 2020 2067  v:.            g
+000094e0: 7561 7264 6172 5f64 6266 2866 6f72 6d61  uardar_dbf(forma
+000094f0: 746f 732c 2054 7275 652c 207b 7d29 0a20  tos, True, {}). 
+00009500: 2020 2020 2020 2065 6c69 6620 272d 2d6a         elif '--j
+00009510: 736f 6e27 2069 6e20 7379 732e 6172 6776  son' in sys.argv
+00009520: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00009530: 7220 666f 726d 6174 6f20 696e 2066 6f72  r formato in for
+00009540: 6d61 746f 733a 0a20 2020 2020 2020 2020  matos:.         
+00009550: 2020 2020 2020 2061 7263 6869 766f 203d         archivo =
+00009560: 206f 7065 6e28 666f 726d 6174 6f5b 305d   open(formato[0]
+00009570: 2e6c 6f77 6572 2829 202b 2022 2e6a 736f  .lower() + ".jso
+00009580: 6e22 2c20 2277 2229 0a20 2020 2020 2020  n", "w").       
+00009590: 2020 2020 2020 2020 206a 736f 6e2e 6475           json.du
+000095a0: 6d70 2866 6f72 6d61 746f 5b32 5d2c 2061  mp(formato[2], a
+000095b0: 7263 6869 766f 2c20 736f 7274 5f6b 6579  rchivo, sort_key
+000095c0: 733d 5472 7565 2c20 696e 6465 6e74 3d34  s=True, indent=4
+000095d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000095e0: 2020 6172 6368 6976 6f2e 636c 6f73 6528    archivo.close(
+000095f0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00009600: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00009610: 666f 726d 6174 6f20 696e 2066 6f72 6d61  formato in forma
+00009620: 746f 733a 0a20 2020 2020 2020 2020 2020  tos:.           
+00009630: 2020 2020 2061 7263 6869 766f 203d 206f       archivo = o
+00009640: 7065 6e28 666f 726d 6174 6f5b 305d 2e6c  pen(formato[0].l
+00009650: 6f77 6572 2829 202b 2022 2e74 7874 222c  ower() + ".txt",
+00009660: 2022 7722 290a 2020 2020 2020 2020 2020   "w").          
+00009670: 2020 2020 2020 666f 7220 6974 2069 6e20        for it in 
+00009680: 666f 726d 6174 6f5b 325d 3a0a 2020 2020  formato[2]:.    
+00009690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096a0: 6172 6368 6976 6f2e 7772 6974 6528 6573  archivo.write(es
+000096b0: 6372 6962 6972 2869 742c 2066 6f72 6d61  cribir(it, forma
+000096c0: 746f 5b31 5d29 290a 2020 2020 2020 2020  to[1])).        
+000096d0: 2020 2020 6172 6368 6976 6f2e 636c 6f73      archivo.clos
+000096e0: 6528 290a 0a0a 2320 6275 7363 6f20 656c  e()...# busco el
+000096f0: 2064 6972 6563 746f 7269 6f20 6465 2069   directorio de i
+00009700: 6e73 7461 6c61 6369 f36e 2028 676c 6f62  nstalaci.n (glob
+00009710: 616c 2070 6172 6120 7175 6520 6e6f 2063  al para que no c
+00009720: 616d 6269 6520 7369 0a23 2075 7361 6e20  ambie si.# usan 
+00009730: 6f74 7261 2064 6c6c 290a 494e 5354 414c  otra dll).INSTAL
+00009740: 4c5f 4449 5220 3d20 5472 617a 614d 6564  L_DIR = TrazaMed
+00009750: 2e49 6e73 7461 6c6c 4469 7220 3d20 6765  .InstallDir = ge
+00009760: 745f 696e 7374 616c 6c5f 6469 7228 290a  t_install_dir().
+00009770: 0a0a 6966 205f 5f6e 616d 655f 5f20 3d3d  ..if __name__ ==
+00009780: 2027 5f5f 6d61 696e 5f5f 273a 0a0a 2020   '__main__':..  
+00009790: 2020 2320 616a 7573 746f 2065 6c20 656e    # ajusto el en
+000097a0: 636f 6469 6e67 2070 6f72 2064 6566 6563  coding por defec
+000097b0: 746f 2028 7369 2073 6520 7265 6469 7269  to (si se rediri
+000097c0: 6a65 206c 6120 7361 6c69 6461 290a 2020  je la salida).  
+000097d0: 2020 6966 206e 6f74 2068 6173 6174 7472    if not hasattr
+000097e0: 2873 7973 2e73 7464 6f75 742c 2022 656e  (sys.stdout, "en
+000097f0: 636f 6469 6e67 2229 206f 7220 7379 732e  coding") or sys.
+00009800: 7374 646f 7574 2e65 6e63 6f64 696e 6720  stdout.encoding 
+00009810: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00009820: 2069 6d70 6f72 7420 636f 6465 6373 0a20   import codecs. 
+00009830: 2020 2020 2020 2069 6d70 6f72 7420 6c6f         import lo
+00009840: 6361 6c65 0a20 2020 2020 2020 2073 7973  cale.        sys
+00009850: 2e73 7464 6f75 7420 3d20 636f 6465 6373  .stdout = codecs
+00009860: 2e67 6574 7772 6974 6572 280a 2020 2020  .getwriter(.    
+00009870: 2020 2020 2020 2020 6c6f 6361 6c65 2e67          locale.g
+00009880: 6574 7072 6566 6572 7265 6465 6e63 6f64  etpreferredencod
+00009890: 696e 6728 2929 2873 7973 2e73 7464 6f75  ing())(sys.stdou
+000098a0: 742c 2022 7265 706c 6163 6522 290a 2020  t, "replace").  
+000098b0: 2020 2020 2020 7379 732e 7374 6465 7272        sys.stderr
+000098c0: 203d 2063 6f64 6563 732e 6765 7477 7269   = codecs.getwri
+000098d0: 7465 7228 0a20 2020 2020 2020 2020 2020  ter(.           
+000098e0: 206c 6f63 616c 652e 6765 7470 7265 6665   locale.getprefe
+000098f0: 7272 6564 656e 636f 6469 6e67 2829 2928  rredencoding())(
+00009900: 7379 732e 7374 6465 7272 2c20 2272 6570  sys.stderr, "rep
+00009910: 6c61 6365 2229 0a0a 2020 2020 6966 2027  lace")..    if '
+00009920: 2d2d 7265 6769 7374 6572 2720 696e 2073  --register' in s
+00009930: 7973 2e61 7267 7620 6f72 2027 2d2d 756e  ys.argv or '--un
+00009940: 7265 6769 7374 6572 2720 696e 2073 7973  register' in sys
+00009950: 2e61 7267 763a 0a20 2020 2020 2020 2069  .argv:.        i
+00009960: 6d70 6f72 7420 7079 7468 6f6e 636f 6d0a  mport pythoncom.
+00009970: 2020 2020 2020 2020 6966 2054 5950 454c          if TYPEL
+00009980: 4942 3a0a 2020 2020 2020 2020 2020 2020  IB:.            
+00009990: 6966 2027 2d2d 7265 6769 7374 6572 2720  if '--register' 
+000099a0: 696e 2073 7973 2e61 7267 763a 0a20 2020  in sys.argv:.   
+000099b0: 2020 2020 2020 2020 2020 2020 2074 6c62               tlb
+000099c0: 203d 206f 732e 7061 7468 2e61 6273 7061   = os.path.abspa
+000099d0: 7468 280a 2020 2020 2020 2020 2020 2020  th(.            
+000099e0: 2020 2020 2020 2020 6f73 2e70 6174 682e          os.path.
+000099f0: 6a6f 696e 2849 4e53 5441 4c4c 5f44 4952  join(INSTALL_DIR
+00009a00: 2c20 2274 7970 656c 6962 222c 2022 7472  , "typelib", "tr
+00009a10: 617a 616d 6564 2e74 6c62 2229 290a 2020  azamed.tlb")).  
+00009a20: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00009a30: 696e 7428 2252 6567 6973 7465 7269 6e67  int("Registering
+00009a40: 2025 7322 2025 2028 746c 622c 2929 0a20   %s" % (tlb,)). 
+00009a50: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00009a60: 6c69 203d 2070 7974 686f 6e63 6f6d 2e4c  li = pythoncom.L
+00009a70: 6f61 6454 7970 654c 6962 2874 6c62 290a  oadTypeLib(tlb).
+00009a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a90: 7079 7468 6f6e 636f 6d2e 5265 6769 7374  pythoncom.Regist
+00009aa0: 6572 5479 7065 4c69 6228 746c 692c 2074  erTypeLib(tli, t
+00009ab0: 6c62 290a 2020 2020 2020 2020 2020 2020  lb).            
+00009ac0: 656c 6966 2027 2d2d 756e 7265 6769 7374  elif '--unregist
+00009ad0: 6572 2720 696e 2073 7973 2e61 7267 763a  er' in sys.argv:
+00009ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009af0: 206b 203d 2054 7261 7a61 4d65 640a 2020   k = TrazaMed.  
+00009b00: 2020 2020 2020 2020 2020 2020 2020 7079                py
+00009b10: 7468 6f6e 636f 6d2e 556e 5265 6769 7374  thoncom.UnRegist
+00009b20: 6572 5479 7065 4c69 6228 6b2e 5f74 7970  erTypeLib(k._typ
+00009b30: 656c 6962 5f67 7569 645f 2c0a 2020 2020  elib_guid_,.    
 00009b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b50: 6b2e 5f74 7970 656c 6962 5f76 6572 7369  k._typelib_versi
-00009b60: 6f6e 5f5b 305d 2c0a 2020 2020 2020 2020  on_[0],.        
-00009b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b60: 2020 2020 2020 2020 6b2e 5f74 7970 656c          k._typel
+00009b70: 6962 5f76 6572 7369 6f6e 5f5b 305d 2c0a  ib_version_[0],.
 00009b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b90: 2020 2020 6b2e 5f74 7970 656c 6962 5f76      k._typelib_v
-00009ba0: 6572 7369 6f6e 5f5b 315d 2c0a 2020 2020  ersion_[1],.    
-00009bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bd0: 2020 2020 2020 2020 302c 0a20 2020 2020          0,.     
+00009b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ba0: 2020 2020 2020 2020 2020 2020 6b2e 5f74              k._t
+00009bb0: 7970 656c 6962 5f76 6572 7369 6f6e 5f5b  ypelib_version_[
+00009bc0: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
+00009bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c00: 2020 2020 2020 2070 7974 686f 6e63 6f6d         pythoncom
-00009c10: 2e53 5953 5f57 494e 3332 290a 2020 2020  .SYS_WIN32).    
-00009c20: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00009c30: 7428 2255 6e72 6567 6973 7465 7265 6420  t("Unregistered 
-00009c40: 7479 7065 6c69 6222 290a 2020 2020 2020  typelib").      
-00009c50: 2020 696d 706f 7274 2077 696e 3332 636f    import win32co
-00009c60: 6d2e 7365 7276 6572 2e72 6567 6973 7465  m.server.registe
-00009c70: 720a 2020 2020 2020 2020 7769 6e33 3263  r.        win32c
-00009c80: 6f6d 2e73 6572 7665 722e 7265 6769 7374  om.server.regist
-00009c90: 6572 2e55 7365 436f 6d6d 616e 644c 696e  er.UseCommandLin
-00009ca0: 6528 5472 617a 614d 6564 290a 2020 2020  e(TrazaMed).    
-00009cb0: 656c 6966 2022 2f41 7574 6f6d 6174 6522  elif "/Automate"
-00009cc0: 2069 6e20 7379 732e 6172 6776 3a0a 2020   in sys.argv:.  
-00009cd0: 2020 2020 2020 2320 4d53 2073 6565 6d73        # MS seems
-00009ce0: 2074 6f20 6c69 6b65 202f 6175 746f 6d61   to like /automa
-00009cf0: 7465 2074 6f20 7275 6e20 7468 6520 636c  te to run the cl
-00009d00: 6173 7320 6661 6374 6f72 6965 732e 0a20  ass factories.. 
-00009d10: 2020 2020 2020 2069 6d70 6f72 7420 7769         import wi
-00009d20: 6e33 3263 6f6d 2e73 6572 7665 722e 6c6f  n32com.server.lo
-00009d30: 6361 6c73 6572 7665 720a 2020 2020 2020  calserver.      
-00009d40: 2020 2320 7769 6e33 3263 6f6d 2e73 6572    # win32com.ser
-00009d50: 7665 722e 6c6f 6361 6c73 6572 7665 722e  ver.localserver.
-00009d60: 6d61 696e 2829 0a20 2020 2020 2020 2023  main().        #
-00009d70: 2073 7461 7274 2074 6865 2073 6572 7665   start the serve
-00009d80: 722e 0a20 2020 2020 2020 2077 696e 3332  r..        win32
-00009d90: 636f 6d2e 7365 7276 6572 2e6c 6f63 616c  com.server.local
-00009da0: 7365 7276 6572 2e73 6572 7665 285b 5472  server.serve([Tr
-00009db0: 617a 614d 6564 2e5f 7265 675f 636c 7369  azaMed._reg_clsi
-00009dc0: 645f 5d29 0a20 2020 2065 6c73 653a 0a20  d_]).    else:. 
-00009dd0: 2020 2020 2020 206d 6169 6e28 290a              main().
+00009bf0: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+00009c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00009c20: 7974 686f 6e63 6f6d 2e53 5953 5f57 494e  ythoncom.SYS_WIN
+00009c30: 3332 290a 2020 2020 2020 2020 2020 2020  32).            
+00009c40: 2020 2020 7072 696e 7428 2255 6e72 6567      print("Unreg
+00009c50: 6973 7465 7265 6420 7479 7065 6c69 6222  istered typelib"
+00009c60: 290a 2020 2020 2020 2020 696d 706f 7274  ).        import
+00009c70: 2077 696e 3332 636f 6d2e 7365 7276 6572   win32com.server
+00009c80: 2e72 6567 6973 7465 720a 2020 2020 2020  .register.      
+00009c90: 2020 7769 6e33 3263 6f6d 2e73 6572 7665    win32com.serve
+00009ca0: 722e 7265 6769 7374 6572 2e55 7365 436f  r.register.UseCo
+00009cb0: 6d6d 616e 644c 696e 6528 5472 617a 614d  mmandLine(TrazaM
+00009cc0: 6564 290a 2020 2020 656c 6966 2022 2f41  ed).    elif "/A
+00009cd0: 7574 6f6d 6174 6522 2069 6e20 7379 732e  utomate" in sys.
+00009ce0: 6172 6776 3a0a 2020 2020 2020 2020 2320  argv:.        # 
+00009cf0: 4d53 2073 6565 6d73 2074 6f20 6c69 6b65  MS seems to like
+00009d00: 202f 6175 746f 6d61 7465 2074 6f20 7275   /automate to ru
+00009d10: 6e20 7468 6520 636c 6173 7320 6661 6374  n the class fact
+00009d20: 6f72 6965 732e 0a20 2020 2020 2020 2069  ories..        i
+00009d30: 6d70 6f72 7420 7769 6e33 3263 6f6d 2e73  mport win32com.s
+00009d40: 6572 7665 722e 6c6f 6361 6c73 6572 7665  erver.localserve
+00009d50: 720a 2020 2020 2020 2020 2320 7769 6e33  r.        # win3
+00009d60: 3263 6f6d 2e73 6572 7665 722e 6c6f 6361  2com.server.loca
+00009d70: 6c73 6572 7665 722e 6d61 696e 2829 0a20  lserver.main(). 
+00009d80: 2020 2020 2020 2023 2073 7461 7274 2074         # start t
+00009d90: 6865 2073 6572 7665 722e 0a20 2020 2020  he server..     
+00009da0: 2020 2077 696e 3332 636f 6d2e 7365 7276     win32com.serv
+00009db0: 6572 2e6c 6f63 616c 7365 7276 6572 2e73  er.localserver.s
+00009dc0: 6572 7665 285b 5472 617a 614d 6564 2e5f  erve([TrazaMed._
+00009dd0: 7265 675f 636c 7369 645f 5d29 0a20 2020  reg_clsid_]).   
+00009de0: 2065 6c73 653a 0a20 2020 2020 2020 206d   else:.        m
+00009df0: 6169 6e28 290a                           ain().
```

### Comparing `py3afipws-0.8/py3afipws/trazarenpre.py` & `py3afipws-0.9/py3afipws/trazarenpre.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,890 +1,892 @@
 00000000: 2321 2f75 7372 2f62 696e 2f70 7974 686f  #!/usr/bin/pytho
-00000010: 6e0a 2320 5468 6973 2070 726f 6772 616d  n.# This program
-00000020: 2069 7320 6672 6565 2073 6f66 7477 6172   is free softwar
-00000030: 653b 2079 6f75 2063 616e 2072 6564 6973  e; you can redis
-00000040: 7472 6962 7574 6520 6974 2061 6e64 2f6f  tribute it and/o
-00000050: 7220 6d6f 6469 6679 0a23 2069 7420 756e  r modify.# it un
-00000060: 6465 7220 7468 6520 7465 726d 7320 6f66  der the terms of
-00000070: 2074 6865 2047 4e55 2047 656e 6572 616c   the GNU General
-00000080: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
-00000090: 6173 2070 7562 6c69 7368 6564 2062 7920  as published by 
-000000a0: 7468 650a 2320 4672 6565 2053 6f66 7477  the.# Free Softw
-000000b0: 6172 6520 466f 756e 6461 7469 6f6e 3b20  are Foundation; 
-000000c0: 6569 7468 6572 2076 6572 7369 6f6e 2033  either version 3
-000000d0: 2c20 6f72 2028 6174 2079 6f75 7220 6f70  , or (at your op
-000000e0: 7469 6f6e 2920 616e 7920 6c61 7465 720a  tion) any later.
-000000f0: 2320 7665 7273 696f 6e2e 0a23 0a23 2054  # version..#.# T
-00000100: 6869 7320 7072 6f67 7261 6d20 6973 2064  his program is d
-00000110: 6973 7472 6962 7574 6564 2069 6e20 7468  istributed in th
-00000120: 6520 686f 7065 2074 6861 7420 6974 2077  e hope that it w
-00000130: 696c 6c20 6265 2075 7365 6675 6c2c 2062  ill be useful, b
-00000140: 7574 0a23 2057 4954 484f 5554 2041 4e59  ut.# WITHOUT ANY
-00000150: 2057 4152 5241 4e54 593b 2077 6974 686f   WARRANTY; witho
-00000160: 7574 2065 7665 6e20 7468 6520 696d 706c  ut even the impl
-00000170: 6965 6420 7761 7272 616e 7479 206f 6620  ied warranty of 
-00000180: 4d45 5243 4841 4e54 4942 494c 4954 590a  MERCHANTIBILITY.
-00000190: 2320 6f72 2046 4954 4e45 5353 2046 4f52  # or FITNESS FOR
-000001a0: 2041 2050 4152 5449 4355 4c41 5220 5055   A PARTICULAR PU
-000001b0: 5250 4f53 452e 2020 5365 6520 7468 6520  RPOSE.  See the 
-000001c0: 474e 5520 4765 6e65 7261 6c20 5075 626c  GNU General Publ
-000001d0: 6963 204c 6963 656e 7365 0a23 2066 6f72  ic License.# for
-000001e0: 206d 6f72 6520 6465 7461 696c 732e 0a0a   more details...
-000001f0: 224d f364 756c 6f20 7061 7261 2054 7261  "M.dulo para Tra
-00000200: 7a61 6269 6c69 6461 6420 6465 2050 7265  zabilidad de Pre
-00000210: 6375 7273 6f72 6573 2051 75ed 6d69 636f  cursores Qu.mico
-00000220: 7320 5245 4e50 5245 2052 6573 6f6c 7563  s RENPRE Resoluc
-00000230: 69f3 6e20 3930 302f 3132 220a 0a23 2049  i.n 900/12"..# I
-00000240: 6e66 6f72 6d61 6369 f36e 2061 6469 6369  nformaci.n adici
-00000250: 6f6e 616c 2079 2064 6f63 756d 656e 7461  onal y documenta
-00000260: 6369 f36e 3a0a 2320 6874 7470 3a2f 2f77  ci.n:.# http://w
-00000270: 7777 2e73 6973 7465 6d61 7361 6769 6c65  ww.sistemasagile
-00000280: 732e 636f 6d2e 6172 2f74 7261 632f 7769  s.com.ar/trac/wi
-00000290: 6b69 2f54 7261 7a61 6269 6c69 6461 6450  ki/TrazabilidadP
-000002a0: 7265 6375 7273 6f72 6573 5175 696d 6963  recursoresQuimic
-000002b0: 6f73 0a0a 5f5f 6175 7468 6f72 5f5f 203d  os..__author__ =
-000002c0: 2022 4d61 7269 616e 6f20 5265 696e 6761   "Mariano Reinga
-000002d0: 7274 203c 7265 696e 6761 7274 4067 6d61  rt <reingart@gma
-000002e0: 696c 2e63 6f6d 3e22 0a5f 5f63 6f70 7972  il.com>".__copyr
-000002f0: 6967 6874 5f5f 203d 2022 436f 7079 7269  ight__ = "Copyri
-00000300: 6768 7420 2843 2920 3230 3131 204d 6172  ght (C) 2011 Mar
-00000310: 6961 6e6f 2052 6569 6e67 6172 7422 0a5f  iano Reingart"._
-00000320: 5f6c 6963 656e 7365 5f5f 203d 2022 4750  _license__ = "GP
-00000330: 4c20 332e 302b 220a 5f5f 7665 7273 696f  L 3.0+".__versio
-00000340: 6e5f 5f20 3d20 2231 2e31 3261 220a 0a23  n__ = "1.12a"..#
-00000350: 6874 7470 3a2f 2f72 656e 7072 652e 7365  http://renpre.se
-00000360: 7276 6963 696f 732e 7061 6d69 2e6f 7267  rvicios.pami.org
-00000370: 2e61 722f 706f 7274 616c 5f74 7261 7a61  .ar/portal_traza
-00000380: 5f72 656e 7072 652f 7061 736f 352e 6874  _renpre/paso5.ht
-00000390: 6d6c 0a0a 696d 706f 7274 206f 730a 696d  ml..import os.im
-000003a0: 706f 7274 2073 6f63 6b65 740a 696d 706f  port socket.impo
-000003b0: 7274 2073 7973 0a69 6d70 6f72 7420 6461  rt sys.import da
-000003c0: 7465 7469 6d65 2c20 7469 6d65 0a69 6d70  tetime, time.imp
-000003d0: 6f72 7420 7079 3373 696d 706c 6573 6f61  ort py3simplesoa
-000003e0: 702e 636c 6965 6e74 0a66 726f 6d20 7079  p.client.from py
-000003f0: 3373 696d 706c 6573 6f61 702e 636c 6965  3simplesoap.clie
-00000400: 6e74 2069 6d70 6f72 7420 536f 6170 4661  nt import SoapFa
-00000410: 756c 740a 6672 6f6d 202e 7574 696c 7320  ult.from .utils 
-00000420: 696d 706f 7274 2042 6173 6557 532c 2069  import BaseWS, i
-00000430: 6e69 6369 616c 697a 6172 5f79 5f63 6170  nicializar_y_cap
-00000440: 7475 7261 725f 6578 6365 7063 696f 6e65  turar_excepcione
-00000450: 732c 2067 6574 5f69 6e73 7461 6c6c 5f64  s, get_install_d
-00000460: 6972 0a0a 484f 4d4f 203d 2046 616c 7365  ir..HOMO = False
-00000470: 0a54 5950 454c 4942 203d 2046 616c 7365  .TYPELIB = False
-00000480: 0a0a 5753 444c 203d 2022 6874 7470 733a  ..WSDL = "https:
-00000490: 2f2f 7365 7276 6963 696f 732e 7061 6d69  //servicios.pami
-000004a0: 2e6f 7267 2e61 722f 7472 617a 616d 6564  .org.ar/trazamed
-000004b0: 2e57 6562 5365 7276 6963 6553 4452 4e3f  .WebServiceSDRN?
-000004c0: 7773 646c 220a 4c4f 4341 5449 4f4e 203d  wsdl".LOCATION =
-000004d0: 2022 6874 7470 733a 2f2f 7365 7276 6963   "https://servic
-000004e0: 696f 732e 7061 6d69 2e6f 7267 2e61 722f  ios.pami.org.ar/
-000004f0: 7472 617a 616d 6564 2e57 6562 5365 7276  trazamed.WebServ
-00000500: 6963 6553 4452 4e3f 7773 646c 220a 2323  iceSDRN?wsdl".##
-00000510: 5753 444c 203d 2022 6874 7470 733a 2f2f  WSDL = "https://
-00000520: 7472 617a 6162 696c 6964 6164 2e70 616d  trazabilidad.pam
-00000530: 692e 6f72 672e 6172 3a35 3930 3530 2f74  i.org.ar:59050/t
-00000540: 7261 7a61 6d65 642e 5765 6253 6572 7669  razamed.WebServi
-00000550: 6365 5344 524e 3f77 7364 6c22 2020 2320  ceSDRN?wsdl"  # 
-00000560: 7072 6f64 2e0a 0a63 6c61 7373 2054 7261  prod...class Tra
-00000570: 7a61 5265 6e70 7265 2842 6173 6557 5329  zaRenpre(BaseWS)
-00000580: 3a0a 2020 2020 2249 6e74 6572 6661 7a20  :.    "Interfaz 
-00000590: 7061 7261 2065 6c20 5765 6253 6572 7669  para el WebServi
-000005a0: 6365 2064 6520 5472 617a 6162 696c 6964  ce de Trazabilid
-000005b0: 6164 2064 6520 5072 6563 7572 736f 7265  ad de Precursore
-000005c0: 7320 5175 696d 6963 6f73 2053 4544 524f  s Quimicos SEDRO
-000005d0: 4e41 5220 534e 5422 0a20 2020 205f 7075  NAR SNT".    _pu
-000005e0: 626c 6963 5f6d 6574 686f 6473 5f20 3d20  blic_methods_ = 
-000005f0: 5b27 5361 7665 5472 616e 7361 6363 696f  ['SaveTransaccio
-00000600: 6e65 7327 2c0a 2020 2020 2020 2020 2020  nes',.          
-00000610: 2020 2020 2020 2020 2020 2020 2020 2753                'S
-00000620: 656e 6443 616e 6365 6c61 6354 7261 6e73  endCancelacTrans
-00000630: 6163 6327 2c20 2747 6574 5472 616e 7361  acc', 'GetTransa
-00000640: 6363 696f 6e65 7357 5327 2c0a 2020 2020  ccionesWS',.    
-00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000660: 2020 2020 2743 6f6e 6563 7461 7227 2c20      'Conectar', 
-00000670: 274c 6565 7245 7272 6f72 272c 2027 4c65  'LeerError', 'Le
-00000680: 6572 5472 616e 7361 6363 696f 6e27 2c0a  erTransaccion',.
-00000690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006a0: 2020 2020 2020 2020 2753 6574 5573 6572          'SetUser
-000006b0: 6e61 6d65 272c 0a20 2020 2020 2020 2020  name',.         
-000006c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000006d0: 5365 7450 6172 616d 6574 726f 272c 2027  SetParametro', '
-000006e0: 4765 7450 6172 616d 6574 726f 272c 0a20  GetParametro',. 
-000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000700: 2020 2020 2020 2027 4765 7443 6f64 6967         'GetCodig
-00000710: 6f54 7261 6e73 6163 6369 6f6e 272c 2027  oTransaccion', '
-00000720: 4765 7452 6573 756c 7461 646f 272c 2027  GetResultado', '
-00000730: 4c6f 6164 5465 7374 584d 4c27 5d0a 0a20  LoadTestXML'].. 
-00000740: 2020 205f 7075 626c 6963 5f61 7474 7273     _public_attrs
-00000750: 5f20 3d20 5b0a 2020 2020 2020 2020 2755  _ = [.        'U
-00000760: 7365 726e 616d 6527 2c20 2750 6173 7377  sername', 'Passw
-00000770: 6f72 6427 2c0a 2020 2020 2020 2020 2743  ord',.        'C
-00000780: 6f64 6967 6f54 7261 6e73 6163 6369 6f6e  odigoTransaccion
-00000790: 272c 2027 4572 726f 7265 7327 2c20 2752  ', 'Errores', 'R
-000007a0: 6573 756c 7461 646f 272c 0a20 2020 2020  esultado',.     
-000007b0: 2020 2027 586d 6c52 6571 7565 7374 272c     'XmlRequest',
-000007c0: 2027 586d 6c52 6573 706f 6e73 6527 2c0a   'XmlResponse',.
-000007d0: 2020 2020 2020 2020 2756 6572 7369 6f6e          'Version
-000007e0: 272c 2027 496e 7374 616c 6c44 6972 272c  ', 'InstallDir',
-000007f0: 0a20 2020 2020 2020 2027 5472 6163 6562  .        'Traceb
-00000800: 6163 6b27 2c20 2745 7863 6570 6369 6f6e  ack', 'Excepcion
-00000810: 272c 2027 4c61 6e7a 6172 4578 6365 7063  ', 'LanzarExcepc
-00000820: 696f 6e65 7327 2c0a 2020 2020 2020 2020  iones',.        
-00000830: 5d0a 0a20 2020 205f 7265 675f 7072 6f67  ]..    _reg_prog
-00000840: 6964 5f20 3d20 2254 7261 7a61 5265 6e70  id_ = "TrazaRenp
-00000850: 7265 220a 2020 2020 5f72 6567 5f63 6c73  re".    _reg_cls
-00000860: 6964 5f20 3d20 227b 3436 3132 3938 4442  id_ = "{461298DB
-00000870: 2d30 3533 312d 3437 4341 2d42 3344 392d  -0531-47CA-B3D9-
-00000880: 4233 3646 4536 3936 3732 3039 7d22 0a0a  B36FE6967209}"..
-00000890: 2020 2020 2320 5661 7269 6162 6c65 7320      # Variables 
-000008a0: 676c 6f62 616c 6573 2070 6172 6120 4261  globales para Ba
-000008b0: 7365 5753 3a0a 2020 2020 484f 4d4f 203d  seWS:.    HOMO =
-000008c0: 2048 4f4d 4f0a 2020 2020 5753 444c 203d   HOMO.    WSDL =
-000008d0: 2057 5344 4c0a 2020 2020 5665 7273 696f   WSDL.    Versio
-000008e0: 6e20 3d20 2225 7320 2573 2025 7322 2025  n = "%s %s %s" %
-000008f0: 2028 5f5f 7665 7273 696f 6e5f 5f2c 2048   (__version__, H
-00000900: 4f4d 4f20 616e 6420 2748 6f6d 6f6c 6f67  OMO and 'Homolog
-00000910: 6163 69f3 6e27 206f 7220 2727 2c0a 2020  aci.n' or '',.  
-00000920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000930: 2020 2020 2020 2020 2020 7079 3373 696d            py3sim
-00000940: 706c 6573 6f61 702e 636c 6965 6e74 2e5f  plesoap.client._
-00000950: 5f76 6572 7369 6f6e 5f5f 290a 0a20 2020  _version__)..   
-00000960: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00000970: 6c66 2c20 7265 696e 7465 6e74 6f73 3d31  lf, reintentos=1
-00000980: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00000990: 5573 6572 6e61 6d65 203d 2073 656c 662e  Username = self.
-000009a0: 5061 7373 776f 7264 203d 204e 6f6e 650a  Password = None.
-000009b0: 2020 2020 2020 2020 4261 7365 5753 2e5f          BaseWS._
-000009c0: 5f69 6e69 745f 5f28 7365 6c66 2c20 7265  _init__(self, re
-000009d0: 696e 7465 6e74 6f73 290a 0a20 2020 2064  intentos)..    d
-000009e0: 6566 2069 6e69 6369 616c 697a 6172 2873  ef inicializar(s
-000009f0: 656c 6629 3a0a 2020 2020 2020 2020 4261  elf):.        Ba
-00000a00: 7365 5753 2e69 6e69 6369 616c 697a 6172  seWS.inicializar
-00000a10: 2873 656c 6629 0a20 2020 2020 2020 2073  (self).        s
-00000a20: 656c 662e 436f 6469 676f 5472 616e 7361  elf.CodigoTransa
-00000a30: 6363 696f 6e20 3d20 7365 6c66 2e45 7272  ccion = self.Err
-00000a40: 6f72 6573 203d 2073 656c 662e 5265 7375  ores = self.Resu
-00000a50: 6c74 6164 6f20 3d20 4e6f 6e65 0a0a 2020  ltado = None..  
-00000a60: 2020 6465 6620 5f5f 616e 616c 697a 6172    def __analizar
-00000a70: 5f65 7272 6f72 6573 2873 656c 662c 2072  _errores(self, r
-00000a80: 6574 293a 0a20 2020 2020 2020 2022 436f  et):.        "Co
-00000a90: 6d70 7275 6562 6120 7920 6578 7472 6165  mprueba y extrae
-00000aa0: 2065 7272 6f72 6573 2073 6920 6578 6973   errores si exis
-00000ab0: 7465 6e20 656e 206c 6120 7265 7370 7565  ten en la respue
-00000ac0: 7374 6120 584d 4c22 0a20 2020 2020 2020  sta XML".       
-00000ad0: 2073 656c 662e 4572 726f 7265 7320 3d20   self.Errores = 
-00000ae0: 5b22 2573 3a20 2573 2220 2520 2869 742e  ["%s: %s" % (it.
-00000af0: 6765 7428 275f 635f 6572 726f 7227 2c20  get('_c_error', 
-00000b00: 2222 292c 2069 742e 6765 7428 275f 645f  ""), it.get('_d_
-00000b10: 6572 726f 7227 2c20 2222 2929 0a20 2020  error', "")).   
-00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b30: 2020 2020 2066 6f72 2069 7420 696e 2072       for it in r
-00000b40: 6574 2e67 6574 2827 6572 726f 7265 7327  et.get('errores'
-00000b50: 2c20 5b5d 295d 0a20 2020 2020 2020 2073  , [])].        s
-00000b60: 656c 662e 5265 7375 6c74 6164 6f20 3d20  elf.Resultado = 
-00000b70: 7265 742e 6765 7428 2772 6573 756c 7461  ret.get('resulta
-00000b80: 646f 2729 0a0a 2020 2020 6465 6620 436f  do')..    def Co
-00000b90: 6e65 6374 6172 2873 656c 662c 2063 6163  nectar(self, cac
-00000ba0: 6865 3d4e 6f6e 652c 2077 7364 6c3d 4e6f  he=None, wsdl=No
-00000bb0: 6e65 2c20 7072 6f78 793d 2222 2c20 7772  ne, proxy="", wr
-00000bc0: 6170 7065 723d 4e6f 6e65 2c20 6361 6365  apper=None, cace
-00000bd0: 7274 3d4e 6f6e 652c 2074 696d 656f 7574  rt=None, timeout
-00000be0: 3d33 3029 3a0a 2020 2020 2020 2020 2320  =30):.        # 
-00000bf0: 436f 6e65 6374 6f20 7573 616e 646f 2065  Conecto usando e
-00000c00: 6c20 6de9 746f 646f 2065 7374 616e 6461  l m.todo estanda
-00000c10: 7264 3a0a 2020 2020 2020 2020 6f6b 203d  rd:.        ok =
-00000c20: 2042 6173 6557 532e 436f 6e65 6374 6172   BaseWS.Conectar
-00000c30: 2873 656c 662c 2063 6163 6865 2c20 7773  (self, cache, ws
-00000c40: 646c 2c20 7072 6f78 792c 2077 7261 7070  dl, proxy, wrapp
-00000c50: 6572 2c20 6361 6365 7274 2c20 7469 6d65  er, cacert, time
-00000c60: 6f75 742c 0a20 2020 2020 2020 2020 2020  out,.           
-00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c80: 2020 736f 6170 5f73 6572 7665 723d 226a    soap_server="j
-00000c90: 6574 7479 2229 0a20 2020 2020 2020 2069  etty").        i
-00000ca0: 6620 6f6b 3a0a 2020 2020 2020 2020 2020  f ok:.          
-00000cb0: 2020 2320 7369 2065 6c20 6172 6368 6976    # si el archiv
-00000cc0: 6f20 6573 206c 6f63 616c 2c20 6173 756d  o es local, asum
-00000cd0: 6f20 7175 6520 7961 2065 7374 6120 636f  o que ya esta co
-00000ce0: 7272 6567 6964 6f3a 0a20 2020 2020 2020  rregido:.       
-00000cf0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00000d00: 2e77 7364 6c2e 7374 6172 7473 7769 7468  .wsdl.startswith
-00000d10: 2822 6669 6c65 2229 3a0a 2020 2020 2020  ("file"):.      
-00000d20: 2020 2020 2020 2020 2020 2320 636f 7272            # corr
-00000d30: 696a 6f20 7562 6963 6163 69f3 6e20 6465  ijo ubicaci.n de
-00000d40: 6c20 7365 7276 6964 6f72 2028 6c6f 6361  l servidor (loca
-00000d50: 6c68 6f73 743a 3930 3530 2065 6e20 656c  lhost:9050 en el
-00000d60: 2057 5344 4c29 0a20 2020 2020 2020 2020   WSDL).         
-00000d70: 2020 2020 2020 206c 6f63 6174 696f 6e20         location 
-00000d80: 3d20 7365 6c66 2e77 7364 6c5b 3a2d 355d  = self.wsdl[:-5]
-00000d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000da0: 2069 6620 2749 5765 6253 6572 7669 6365   if 'IWebService
-00000db0: 5344 524e 5365 7276 6963 6527 2069 6e20  SDRNService' in 
-00000dc0: 7365 6c66 2e63 6c69 656e 742e 7365 7276  self.client.serv
-00000dd0: 6963 6573 3a0a 2020 2020 2020 2020 2020  ices:.          
-00000de0: 2020 2020 2020 2020 2020 7773 203d 2073            ws = s
-00000df0: 656c 662e 636c 6965 6e74 2e73 6572 7669  elf.client.servi
-00000e00: 6365 735b 2749 5765 6253 6572 7669 6365  ces['IWebService
-00000e10: 5344 524e 5365 7276 6963 6527 5d0a 2020  SDRNService'].  
-00000e20: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00000e30: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00000e40: 2020 2020 2020 2020 7773 203d 2073 656c          ws = sel
-00000e50: 662e 636c 6965 6e74 2e73 6572 7669 6365  f.client.service
-00000e60: 735b 2749 5765 6253 6572 7669 6365 5344  s['IWebServiceSD
-00000e70: 524e 275d 0a20 2020 2020 2020 2020 2020  RN'].           
-00000e80: 2020 2020 2077 735b 2770 6f72 7473 275d       ws['ports']
-00000e90: 5b27 4957 6562 5365 7276 6963 6553 4452  ['IWebServiceSDR
-00000ea0: 4e50 6f72 7427 5d5b 276c 6f63 6174 696f  NPort']['locatio
-00000eb0: 6e27 5d20 3d20 6c6f 6361 7469 6f6e 0a20  n'] = location. 
-00000ec0: 2020 2020 2020 2020 2020 2023 2045 7374             # Est
-00000ed0: 6162 6c65 6365 7220 6372 6564 656e 6369  ablecer credenci
-00000ee0: 616c 6573 2064 6520 7365 6775 7269 6461  ales de segurida
-00000ef0: 643a 0a20 2020 2020 2020 2020 2020 2073  d:.            s
-00000f00: 656c 662e 636c 6965 6e74 5b27 7773 7365  elf.client['wsse
-00000f10: 3a53 6563 7572 6974 7927 5d20 3d20 7b0a  :Security'] = {.
-00000f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f30: 2777 7373 653a 5573 6572 6e61 6d65 546f  'wsse:UsernameTo
-00000f40: 6b65 6e27 3a20 7b0a 2020 2020 2020 2020  ken': {.        
-00000f50: 2020 2020 2020 2020 2020 2020 2777 7373              'wss
-00000f60: 653a 5573 6572 6e61 6d65 273a 2073 656c  e:Username': sel
-00000f70: 662e 5573 6572 6e61 6d65 2c0a 2020 2020  f.Username,.    
-00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f90: 2777 7373 653a 5061 7373 776f 7264 273a  'wsse:Password':
-00000fa0: 2073 656c 662e 5061 7373 776f 7264 2c0a   self.Password,.
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00000fd0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00000fe0: 7265 7475 726e 206f 6b0a 0a20 2020 2040  return ok..    @
-00000ff0: 696e 6963 6961 6c69 7a61 725f 795f 6361  inicializar_y_ca
-00001000: 7074 7572 6172 5f65 7863 6570 6369 6f6e  pturar_excepcion
-00001010: 6573 0a20 2020 2064 6566 2053 6176 6554  es.    def SaveT
-00001020: 7261 6e73 6163 6369 6f6e 6573 2873 656c  ransacciones(sel
-00001030: 662c 2075 7375 6172 696f 2c20 7061 7373  f, usuario, pass
-00001040: 776f 7264 2c0a 2020 2020 2020 2020 2020  word,.          
-00001050: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00001060: 6c6e 5f6f 7269 6765 6e3d 4e6f 6e65 2c20  ln_origen=None, 
-00001070: 676c 6e5f 6465 7374 696e 6f3d 4e6f 6e65  gln_destino=None
-00001080: 2c20 665f 6f70 6572 6163 696f 6e3d 4e6f  , f_operacion=No
-00001090: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-000010a0: 2020 2020 2020 2020 2020 2020 2069 645f               id_
-000010b0: 6576 656e 746f 3d4e 6f6e 652c 2063 6f64  evento=None, cod
-000010c0: 5f70 726f 6475 6374 6f3d 4e6f 6e65 2c20  _producto=None, 
-000010d0: 6e5f 6361 6e74 6964 6164 3d4e 6f6e 652c  n_cantidad=None,
-000010e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000010f0: 2020 2020 2020 2020 2020 6e5f 646f 6375            n_docu
-00001100: 6d65 6e74 6f5f 6f70 6572 6163 696f 6e3d  mento_operacion=
-00001110: 4e6f 6e65 2c20 6e5f 7265 6d69 746f 3d4e  None, n_remito=N
-00001120: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00001130: 2020 2020 2020 2020 2020 2020 2020 6964                id
-00001140: 5f74 6970 6f5f 7472 616e 7370 6f72 7465  _tipo_transporte
-00001150: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001170: 6964 5f70 6173 6f5f 6672 6f6e 7465 7261  id_paso_frontera
-00001180: 5f69 6e67 7265 736f 3d4e 6f6e 652c 0a20  _ingreso=None,. 
-00001190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011a0: 2020 2020 2020 2020 6964 5f70 6173 6f5f          id_paso_
-000011b0: 6672 6f6e 7465 7261 5f65 6772 6573 6f3d  frontera_egreso=
-000011c0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-000011d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000011e0: 645f 7469 706f 5f64 6f63 756d 656e 746f  d_tipo_documento
-000011f0: 5f6f 7065 7261 6369 6f6e 3d4e 6f6e 652c  _operacion=None,
-00001200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001210: 2020 2020 2020 2020 2020 645f 646f 6d69            d_domi
-00001220: 6e69 6f5f 7472 6163 746f 723d 4e6f 6e65  nio_tractor=None
-00001230: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001240: 2020 2020 2020 2020 2020 2064 5f64 6f6d             d_dom
-00001250: 696e 696f 5f73 656d 693d 4e6f 6e65 2c0a  inio_semi=None,.
-00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001270: 2020 2020 2020 2020 206e 5f73 6572 6965           n_serie
-00001280: 3d4e 6f6e 652c 206e 5f6c 6f74 653d 4e6f  =None, n_lote=No
-00001290: 6e65 2c20 646f 635f 6465 7370 6163 686f  ne, doc_despacho
-000012a0: 5f70 6c61 7a61 3d4e 6f6e 652c 0a20 2020  _plaza=None,.   
-000012b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012c0: 2020 2020 2020 646a 6169 3d4e 6f6e 652c        djai=None,
-000012d0: 206e 5f63 6572 745f 696d 706f 5f65 7870   n_cert_impo_exp
-000012e0: 6f3d 4e6f 6e65 2c0a 2020 2020 2020 2020  o=None,.        
-000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001300: 2069 645f 7469 706f 5f64 6f63 756d 656e   id_tipo_documen
-00001310: 746f 3d4e 6f6e 652c 206e 5f64 6f63 756d  to=None, n_docum
-00001320: 656e 746f 3d4e 6f6e 652c 0a20 2020 2020  ento=None,.     
-00001330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001340: 2020 2020 6d5f 6361 6c69 6461 645f 616e      m_calidad_an
-00001350: 616c 6974 6963 613d 4e6f 6e65 2c20 6d5f  alitica=None, m_
-00001360: 656e 7472 6567 615f 7061 7263 6961 6c3d  entrega_parcial=
-00001370: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00001380: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00001390: 6f63 5f70 6572 6d69 736f 5f65 6d62 6172  oc_permiso_embar
-000013a0: 7175 653d 4e6f 6e65 2c20 676c 6e5f 7472  que=None, gln_tr
-000013b0: 616e 7370 6f72 7469 7374 613d 4e6f 6e65  ansportista=None
-000013c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000013d0: 2020 2020 2020 2020 2020 206f 7065 7261             opera
-000013e0: 6369 6f6e 5f65 7863 656e 746f 5f64 6a61  cion_excento_dja
-000013f0: 693d 4e6f 6e65 2c20 636f 6e74 726f 6c5f  i=None, control_
-00001400: 6475 706c 6963 6964 6164 3d4e 6f6e 652c  duplicidad=None,
-00001410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001420: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-00001430: 2020 2020 2022 5065 726d 6974 6520 696e       "Permite in
-00001440: 666f 726d 6520 706f 7220 7061 7274 6520  forme por parte 
-00001450: 6465 2075 6e20 6167 656e 7465 2064 6520  de un agente de 
-00001460: 756e 6120 6f20 7661 7269 6173 2074 7261  una o varias tra
-00001470: 6e73 6163 6369 6f6e 6573 220a 2020 2020  nsacciones".    
-00001480: 2020 2020 2320 6372 656f 206c 6f73 2070      # creo los p
-00001490: 6172 e16d 6574 726f 7320 7061 7261 2065  ar.metros para e
-000014a0: 7374 6120 6c6c 616d 6164 610a 2020 2020  sta llamada.    
-000014b0: 2020 2020 7061 7261 6d73 203d 207b 2020      params = {  
-000014c0: 2767 6c6e 5f6f 7269 6765 6e27 3a20 676c  'gln_origen': gl
-000014d0: 6e5f 6f72 6967 656e 2c20 2767 6c6e 5f64  n_origen, 'gln_d
-000014e0: 6573 7469 6e6f 273a 2067 6c6e 5f64 6573  estino': gln_des
-000014f0: 7469 6e6f 2c0a 2020 2020 2020 2020 2020  tino,.          
-00001500: 2020 2020 2020 2020 2020 2766 5f6f 7065            'f_ope
-00001510: 7261 6369 6f6e 273a 2066 5f6f 7065 7261  racion': f_opera
-00001520: 6369 6f6e 2c20 2769 645f 6576 656e 746f  cion, 'id_evento
-00001530: 273a 2069 645f 6576 656e 746f 2c0a 2020  ': id_evento,.  
-00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001550: 2020 2763 6f64 5f70 726f 6475 6374 6f27    'cod_producto'
-00001560: 3a20 636f 645f 7072 6f64 7563 746f 2c20  : cod_producto, 
-00001570: 276e 5f63 616e 7469 6461 6427 3a20 6e5f  'n_cantidad': n_
-00001580: 6361 6e74 6964 6164 2c0a 2020 2020 2020  cantidad,.      
-00001590: 2020 2020 2020 2020 2020 2020 2020 276e                'n
-000015a0: 5f64 6f63 756d 656e 746f 5f6f 7065 7261  _documento_opera
-000015b0: 6369 6f6e 273a 206e 5f64 6f63 756d 656e  cion': n_documen
-000015c0: 746f 5f6f 7065 7261 6369 6f6e 2c0a 2020  to_operacion,.  
-000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015e0: 2020 276e 5f72 656d 6974 6f27 3a20 6e5f    'n_remito': n_
-000015f0: 7265 6d69 746f 2c0a 2020 2020 2020 2020  remito,.        
-00001600: 2020 2020 2020 2020 2020 2020 2769 645f              'id_
-00001610: 7469 706f 5f74 7261 6e73 706f 7274 6527  tipo_transporte'
-00001620: 3a20 6964 5f74 6970 6f5f 7472 616e 7370  : id_tipo_transp
-00001630: 6f72 7465 2c0a 2020 2020 2020 2020 2020  orte,.          
-00001640: 2020 2020 2020 2020 2020 2769 645f 7061            'id_pa
-00001650: 736f 5f66 726f 6e74 6572 615f 696e 6772  so_frontera_ingr
-00001660: 6573 6f27 3a20 6964 5f70 6173 6f5f 6672  eso': id_paso_fr
-00001670: 6f6e 7465 7261 5f69 6e67 7265 736f 2c0a  ontera_ingreso,.
-00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001690: 2020 2020 2769 645f 7061 736f 5f66 726f      'id_paso_fro
-000016a0: 6e74 6572 615f 6567 7265 736f 273a 2069  ntera_egreso': i
-000016b0: 645f 7061 736f 5f66 726f 6e74 6572 615f  d_paso_frontera_
-000016c0: 6567 7265 736f 2c0a 2020 2020 2020 2020  egreso,.        
-000016d0: 2020 2020 2020 2020 2020 2020 2769 645f              'id_
-000016e0: 7469 706f 5f64 6f63 756d 656e 746f 5f6f  tipo_documento_o
-000016f0: 7065 7261 6369 6f6e 273a 2069 645f 7469  peracion': id_ti
-00001700: 706f 5f64 6f63 756d 656e 746f 5f6f 7065  po_documento_ope
-00001710: 7261 6369 6f6e 2c0a 2020 2020 2020 2020  racion,.        
-00001720: 2020 2020 2020 2020 2020 2020 2764 5f64              'd_d
-00001730: 6f6d 696e 696f 5f74 7261 6374 6f72 273a  ominio_tractor':
-00001740: 2064 5f64 6f6d 696e 696f 5f74 7261 6374   d_dominio_tract
-00001750: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
-00001760: 2020 2020 2020 2020 2764 5f64 6f6d 696e          'd_domin
-00001770: 696f 5f73 656d 6927 3a20 645f 646f 6d69  io_semi': d_domi
-00001780: 6e69 6f5f 7365 6d69 2c0a 2020 2020 2020  nio_semi,.      
-00001790: 2020 2020 2020 2020 2020 2020 2020 276e                'n
-000017a0: 5f73 6572 6965 273a 206e 5f73 6572 6965  _serie': n_serie
-000017b0: 2c20 276e 5f6c 6f74 6527 3a20 6e5f 6c6f  , 'n_lote': n_lo
-000017c0: 7465 2c0a 2020 2020 2020 2020 2020 2020  te,.            
-000017d0: 2020 2020 2020 2020 2764 6f63 5f64 6573          'doc_des
-000017e0: 7061 6368 6f5f 706c 617a 6127 3a20 646f  pacho_plaza': do
-000017f0: 635f 6465 7370 6163 686f 5f70 6c61 7a61  c_despacho_plaza
-00001800: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001810: 2020 2020 2020 2764 6a61 6927 3a20 646a        'djai': dj
-00001820: 6169 2c20 276e 5f63 6572 745f 696d 706f  ai, 'n_cert_impo
-00001830: 5f65 7870 6f27 3a20 6e5f 6365 7274 5f69  _expo': n_cert_i
-00001840: 6d70 6f5f 6578 706f 2c0a 2020 2020 2020  mpo_expo,.      
-00001850: 2020 2020 2020 2020 2020 2020 2020 2769                'i
-00001860: 645f 7469 706f 5f64 6f63 756d 656e 746f  d_tipo_documento
-00001870: 273a 2069 645f 7469 706f 5f64 6f63 756d  ': id_tipo_docum
-00001880: 656e 746f 2c0a 2020 2020 2020 2020 2020  ento,.          
-00001890: 2020 2020 2020 2020 2020 276e 5f64 6f63            'n_doc
-000018a0: 756d 656e 746f 273a 206e 5f64 6f63 756d  umento': n_docum
-000018b0: 656e 746f 2c0a 2020 2020 2020 2020 2020  ento,.          
-000018c0: 2020 2020 2020 2020 2020 276d 5f63 616c            'm_cal
-000018d0: 6964 6164 5f61 6e61 6c69 7469 6361 273a  idad_analitica':
-000018e0: 206d 5f63 616c 6964 6164 5f61 6e61 6c69   m_calidad_anali
-000018f0: 7469 6361 2c0a 2020 2020 2020 2020 2020  tica,.          
-00001900: 2020 2020 2020 2020 2020 276d 5f65 6e74            'm_ent
-00001910: 7265 6761 5f70 6172 6369 616c 273a 206d  rega_parcial': m
-00001920: 5f65 6e74 7265 6761 5f70 6172 6369 616c  _entrega_parcial
-00001930: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001940: 2020 2020 2020 2764 6f63 5f70 6572 6d69        'doc_permi
-00001950: 736f 5f65 6d62 6172 7175 6527 3a20 646f  so_embarque': do
-00001960: 635f 7065 726d 6973 6f5f 656d 6261 7271  c_permiso_embarq
-00001970: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00001980: 2020 2020 2020 2020 2767 6c6e 5f74 7261          'gln_tra
-00001990: 6e73 706f 7274 6973 7461 273a 2067 6c6e  nsportista': gln
-000019a0: 5f74 7261 6e73 706f 7274 6973 7461 2c0a  _transportista,.
-000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019c0: 2020 2020 276f 7065 7261 6369 6f6e 5f65      'operacion_e
-000019d0: 7863 656e 746f 5f64 6a61 6927 3a20 6f70  xcento_djai': op
-000019e0: 6572 6163 696f 6e5f 6578 6365 6e74 6f5f  eracion_excento_
-000019f0: 646a 6169 2c0a 2020 2020 2020 2020 2020  djai,.          
-00001a00: 2020 2020 2020 2020 2020 2763 6f6e 7472            'contr
-00001a10: 6f6c 5f64 7570 6c69 6369 6461 6427 3a20  ol_duplicidad': 
-00001a20: 636f 6e74 726f 6c5f 6475 706c 6963 6964  control_duplicid
-00001a30: 6164 2c0a 2020 2020 2020 2020 2020 2020  ad,.            
-00001a40: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00001a50: 2020 2320 6163 7475 616c 697a 6f20 636f    # actualizo co
-00001a60: 6e20 7061 72e1 6d65 7472 6f73 2067 656e  n par.metros gen
-00001a70: 6572 616c 6573 3a0a 2020 2020 2020 2020  erales:.        
-00001a80: 7061 7261 6d73 2e75 7064 6174 6528 7365  params.update(se
-00001a90: 6c66 2e70 6172 616d 735f 696e 290a 2020  lf.params_in).  
-00001aa0: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
-00001ab0: 2e63 6c69 656e 742e 7361 7665 5472 616e  .client.saveTran
-00001ac0: 7361 6363 696f 6e65 7328 0a20 2020 2020  sacciones(.     
-00001ad0: 2020 2020 2020 2061 7267 303d 7061 7261         arg0=para
-00001ae0: 6d73 2c0a 2020 2020 2020 2020 2020 2020  ms,.            
-00001af0: 6172 6731 3d75 7375 6172 696f 2c0a 2020  arg1=usuario,.  
-00001b00: 2020 2020 2020 2020 2020 6172 6732 3d70            arg2=p
-00001b10: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
-00001b20: 2029 0a20 2020 2020 2020 2072 6574 203d   ).        ret =
-00001b30: 2072 6573 5b27 7265 7475 726e 275d 0a20   res['return']. 
-00001b40: 2020 2020 2020 2073 656c 662e 436f 6469         self.Codi
-00001b50: 676f 5472 616e 7361 6363 696f 6e20 3d20  goTransaccion = 
-00001b60: 7265 742e 6765 7428 2763 6f64 6967 6f54  ret.get('codigoT
-00001b70: 7261 6e73 6163 6369 6f6e 2729 0a20 2020  ransaccion').   
-00001b80: 2020 2020 2073 656c 662e 5f5f 616e 616c       self.__anal
-00001b90: 697a 6172 5f65 7272 6f72 6573 2872 6574  izar_errores(ret
-00001ba0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00001bb0: 2054 7275 650a 0a20 2020 2040 696e 6963   True..    @inic
-00001bc0: 6961 6c69 7a61 725f 795f 6361 7074 7572  ializar_y_captur
-00001bd0: 6172 5f65 7863 6570 6369 6f6e 6573 0a20  ar_excepciones. 
-00001be0: 2020 2064 6566 2053 656e 6443 616e 6365     def SendCance
-00001bf0: 6c61 6354 7261 6e73 6163 6328 7365 6c66  lacTransacc(self
-00001c00: 2c20 7573 7561 7269 6f2c 2070 6173 7377  , usuario, passw
-00001c10: 6f72 642c 2063 6f64 6967 6f5f 7472 616e  ord, codigo_tran
-00001c20: 7361 6363 696f 6e29 3a0a 2020 2020 2020  saccion):.      
-00001c30: 2020 2220 5265 616c 697a 6120 6c61 2063    " Realiza la c
-00001c40: 616e 6365 6c61 6369 f36e 2064 6520 756e  ancelaci.n de un
-00001c50: 6120 7472 616e 7361 6363 69f3 6e22 0a20  a transacci.n". 
-00001c60: 2020 2020 2020 2072 6573 203d 2073 656c         res = sel
-00001c70: 662e 636c 6965 6e74 2e73 656e 6443 616e  f.client.sendCan
-00001c80: 6365 6c61 5472 616e 7361 6328 0a20 2020  celaTransac(.   
-00001c90: 2020 2020 2020 2020 2061 7267 303d 636f           arg0=co
-00001ca0: 6469 676f 5f74 7261 6e73 6163 6369 6f6e  digo_transaccion
-00001cb0: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
-00001cc0: 6731 3d75 7375 6172 696f 2c0a 2020 2020  g1=usuario,.    
-00001cd0: 2020 2020 2020 2020 6172 6732 3d70 6173          arg2=pas
-00001ce0: 7377 6f72 642c 0a20 2020 2020 2020 2029  sword,.        )
-00001cf0: 0a0a 2020 2020 2020 2020 7265 7420 3d20  ..        ret = 
-00001d00: 7265 735b 2772 6574 7572 6e27 5d0a 0a20  res['return'].. 
-00001d10: 2020 2020 2020 2073 656c 662e 436f 6469         self.Codi
-00001d20: 676f 5472 616e 7361 6363 696f 6e20 3d20  goTransaccion = 
-00001d30: 7265 745b 2763 6f64 6967 6f54 7261 6e73  ret['codigoTrans
-00001d40: 6163 6369 6f6e 275d 0a20 2020 2020 2020  accion'].       
-00001d50: 2073 656c 662e 5f5f 616e 616c 697a 6172   self.__analizar
-00001d60: 5f65 7272 6f72 6573 2872 6574 290a 0a20  _errores(ret).. 
-00001d70: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00001d80: 7565 0a0a 2020 2020 4069 6e69 6369 616c  ue..    @inicial
-00001d90: 697a 6172 5f79 5f63 6170 7475 7261 725f  izar_y_capturar_
-00001da0: 6578 6365 7063 696f 6e65 730a 2020 2020  excepciones.    
-00001db0: 6465 6620 5365 6e64 436f 6e66 6972 6d61  def SendConfirma
-00001dc0: 5472 616e 7361 6363 2873 656c 662c 2075  Transacc(self, u
-00001dd0: 7375 6172 696f 2c20 7061 7373 776f 7264  suario, password
-00001de0: 2c20 705f 6964 735f 7472 616e 7361 632c  , p_ids_transac,
-00001df0: 2066 5f6f 7065 7261 6369 6f6e 293a 0a20   f_operacion):. 
-00001e00: 2020 2020 2020 2022 436f 6e66 6972 6d61         "Confirma
-00001e10: 206c 6120 7265 6365 7063 69f3 6e20 6465   la recepci.n de
-00001e20: 2075 6e20 6d65 6469 6361 6d65 6e74 6f22   un medicamento"
-00001e30: 0a20 2020 2020 2020 2072 6573 203d 2073  .        res = s
-00001e40: 656c 662e 636c 6965 6e74 2e73 656e 6443  elf.client.sendC
-00001e50: 6f6e 6669 726d 6154 7261 6e73 6163 6328  onfirmaTransacc(
-00001e60: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
-00001e70: 303d 7573 7561 7269 6f2c 0a20 2020 2020  0=usuario,.     
-00001e80: 2020 2020 2020 2061 7267 313d 7061 7373         arg1=pass
-00001e90: 776f 7264 2c0a 2020 2020 2020 2020 2020  word,.          
-00001ea0: 2020 6172 6732 3d7b 2770 5f69 6473 5f74    arg2={'p_ids_t
-00001eb0: 7261 6e73 6163 273a 2070 5f69 6473 5f74  ransac': p_ids_t
-00001ec0: 7261 6e73 6163 2c20 2766 5f6f 7065 7261  ransac, 'f_opera
-00001ed0: 6369 6f6e 273a 2066 5f6f 7065 7261 6369  cion': f_operaci
-00001ee0: 6f6e 7d2c 0a20 2020 2020 2020 2029 0a20  on},.        ). 
-00001ef0: 2020 2020 2020 2072 6574 203d 2072 6573         ret = res
-00001f00: 5b27 7265 7475 726e 275d 0a20 2020 2020  ['return'].     
-00001f10: 2020 2073 656c 662e 436f 6469 676f 5472     self.CodigoTr
-00001f20: 616e 7361 6363 696f 6e20 3d20 7265 742e  ansaccion = ret.
-00001f30: 6765 7428 2769 645f 7472 616e 7361 635f  get('id_transac_
-00001f40: 6173 6f63 6961 6461 2729 0a20 2020 2020  asociada').     
-00001f50: 2020 2073 656c 662e 5f5f 616e 616c 697a     self.__analiz
-00001f60: 6172 5f65 7272 6f72 6573 2872 6574 290a  ar_errores(ret).
-00001f70: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00001f80: 7275 650a 0a20 2020 2040 696e 6963 6961  rue..    @inicia
-00001f90: 6c69 7a61 725f 795f 6361 7074 7572 6172  lizar_y_capturar
-00001fa0: 5f65 7863 6570 6369 6f6e 6573 0a20 2020  _excepciones.   
-00001fb0: 2064 6566 2053 656e 6441 6c65 7274 6154   def SendAlertaT
-00001fc0: 7261 6e73 6163 6328 7365 6c66 2c20 7573  ransacc(self, us
-00001fd0: 7561 7269 6f2c 2070 6173 7377 6f72 642c  uario, password,
-00001fe0: 2070 5f69 6473 5f74 7261 6e73 6163 5f77   p_ids_transac_w
-00001ff0: 7329 3a0a 2020 2020 2020 2020 2241 6c65  s):.        "Ale
-00002000: 7274 6120 756e 206d 6564 6963 616d 656e  rta un medicamen
-00002010: 746f 2c20 6163 6369 f36e 2063 6f6e 7472  to, acci.n contr
-00002020: 6172 6961 2061 2093 636f 6e66 6972 6d61  aria a .confirma
-00002030: 7220 6c61 2074 7261 6e73 6163 6369 f36e  r la transacci.n
-00002040: 942e 220a 2020 2020 2020 2020 7265 7320  ..".        res 
-00002050: 3d20 7365 6c66 2e63 6c69 656e 742e 7365  = self.client.se
-00002060: 6e64 416c 6572 7461 5472 616e 7361 6363  ndAlertaTransacc
-00002070: 280a 2020 2020 2020 2020 2020 2020 6172  (.            ar
-00002080: 6730 3d75 7375 6172 696f 2c0a 2020 2020  g0=usuario,.    
-00002090: 2020 2020 2020 2020 6172 6731 3d70 6173          arg1=pas
-000020a0: 7377 6f72 642c 0a20 2020 2020 2020 2020  sword,.         
-000020b0: 2020 2061 7267 323d 705f 6964 735f 7472     arg2=p_ids_tr
-000020c0: 616e 7361 635f 7773 2c0a 2020 2020 2020  ansac_ws,.      
-000020d0: 2020 290a 2020 2020 2020 2020 7265 7420    ).        ret 
-000020e0: 3d20 7265 735b 2772 6574 7572 6e27 5d0a  = res['return'].
-000020f0: 2020 2020 2020 2020 7365 6c66 2e43 6f64          self.Cod
-00002100: 6967 6f54 7261 6e73 6163 6369 6f6e 203d  igoTransaccion =
-00002110: 2072 6574 2e67 6574 2827 6964 5f74 7261   ret.get('id_tra
-00002120: 6e73 6163 5f61 736f 6369 6164 6127 290a  nsac_asociada').
-00002130: 2020 2020 2020 2020 7365 6c66 2e5f 5f61          self.__a
-00002140: 6e61 6c69 7a61 725f 6572 726f 7265 7328  nalizar_errores(
-00002150: 7265 7429 0a20 2020 2020 2020 2072 6574  ret).        ret
-00002160: 7572 6e20 5472 7565 0a0a 2020 2020 4069  urn True..    @i
-00002170: 6e69 6369 616c 697a 6172 5f79 5f63 6170  nicializar_y_cap
-00002180: 7475 7261 725f 6578 6365 7063 696f 6e65  turar_excepcione
-00002190: 730a 2020 2020 6465 6620 4765 7454 7261  s.    def GetTra
-000021a0: 6e73 6163 6369 6f6e 6573 5753 2873 656c  nsaccionesWS(sel
-000021b0: 662c 2075 7375 6172 696f 2c20 7061 7373  f, usuario, pass
-000021c0: 776f 7264 2c0a 2020 2020 2020 2020 2020  word,.          
-000021d0: 2020 2020 2020 705f 6964 5f74 7261 6e73        p_id_trans
-000021e0: 6163 6369 6f6e 5f67 6c6f 6261 6c3d 4e6f  accion_global=No
-000021f0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00002200: 2020 2020 6964 5f61 6765 6e74 655f 6f72      id_agente_or
-00002210: 6967 656e 3d4e 6f6e 652c 2069 645f 6167  igen=None, id_ag
-00002220: 656e 7465 5f64 6573 7469 6e6f 3d4e 6f6e  ente_destino=Non
-00002230: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00002240: 2020 2069 645f 6167 656e 7465 5f69 6e66     id_agente_inf
-00002250: 6f72 6d61 646f 723d 4e6f 6e65 2c0a 2020  ormador=None,.  
-00002260: 2020 2020 2020 2020 2020 2020 2020 6774                gt
-00002270: 696e 3d4e 6f6e 652c 2069 645f 6576 656e  in=None, id_even
-00002280: 746f 3d4e 6f6e 652c 2063 616e 745f 616e  to=None, cant_an
-00002290: 616c 6974 6963 613d 4e6f 6e65 2c0a 2020  alitica=None,.  
-000022a0: 2020 2020 2020 2020 2020 2020 2020 6665                fe
-000022b0: 6368 615f 6465 7364 655f 6f70 3d4e 6f6e  cha_desde_op=Non
-000022c0: 652c 2066 6563 6861 5f68 6173 7461 5f6f  e, fecha_hasta_o
-000022d0: 703d 4e6f 6e65 2c0a 2020 2020 2020 2020  p=None,.        
-000022e0: 2020 2020 2020 2020 6665 6368 615f 6465          fecha_de
-000022f0: 7364 655f 743d 4e6f 6e65 2c20 6665 6368  sde_t=None, fech
-00002300: 615f 6861 7374 615f 743d 4e6f 6e65 2c0a  a_hasta_t=None,.
-00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002320: 6964 5f74 6970 6f3d 4e6f 6e65 2c0a 2020  id_tipo=None,.  
-00002330: 2020 2020 2020 2020 2020 2020 2020 6964                id
-00002340: 5f65 7374 6164 6f3d 4e6f 6e65 2c20 6e72  _estado=None, nr
-00002350: 6f5f 7061 673d 312c 2063 616e 745f 7265  o_pag=1, cant_re
-00002360: 673d 3130 302c 0a20 2020 2020 2020 2020  g=100,.         
-00002370: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00002380: 2020 224f 6274 6965 6e65 206c 6f73 206d    "Obtiene los m
-00002390: 6f76 696d 6965 6e74 6f73 2072 6561 6c69  ovimientos reali
-000023a0: 7a61 646f 7320 7920 7065 726d 6974 6520  zados y permite 
-000023b0: 6669 6c74 726f 7320 6465 2062 fa73 7175  filtros de b.squ
-000023c0: 6564 6122 0a0a 2020 2020 2020 2020 2320  eda"..        # 
-000023d0: 7072 6570 6172 6f20 6c6f 7320 7061 7261  preparo los para
-000023e0: 6d65 7472 6f73 2064 6520 656e 7472 6164  metros de entrad
-000023f0: 6120 6f70 6369 6f6e 616c 6573 3a0a 2020  a opcionales:.  
-00002400: 2020 2020 2020 6b77 6172 6773 203d 207b        kwargs = {
-00002410: 7d0a 2020 2020 2020 2020 6966 2070 5f69  }.        if p_i
-00002420: 645f 7472 616e 7361 6363 696f 6e5f 676c  d_transaccion_gl
-00002430: 6f62 616c 2069 7320 6e6f 7420 4e6f 6e65  obal is not None
-00002440: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
-00002450: 6172 6773 5b27 6172 6732 275d 203d 2070  args['arg2'] = p
-00002460: 5f69 645f 7472 616e 7361 6363 696f 6e5f  _id_transaccion_
-00002470: 676c 6f62 616c 0a20 2020 2020 2020 2069  global.        i
-00002480: 6620 6964 5f61 6765 6e74 655f 6f72 6967  f id_agente_orig
-00002490: 656e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  en is not None:.
-000024a0: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-000024b0: 6773 5b27 6172 6733 275d 203d 2069 645f  gs['arg3'] = id_
-000024c0: 6167 656e 7465 5f6f 7269 6765 6e0a 2020  agente_origen.  
-000024d0: 2020 2020 2020 6966 2069 645f 6167 656e        if id_agen
-000024e0: 7465 5f64 6573 7469 6e6f 2069 7320 6e6f  te_destino is no
-000024f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00002500: 2020 2020 6b77 6172 6773 5b27 6172 6734      kwargs['arg4
-00002510: 275d 203d 2069 645f 6167 656e 7465 5f64  '] = id_agente_d
-00002520: 6573 7469 6e6f 0a20 2020 2020 2020 2069  estino.        i
-00002530: 6620 6964 5f61 6765 6e74 655f 6465 7374  f id_agente_dest
-00002540: 696e 6f20 6973 206e 6f74 204e 6f6e 653a  ino is not None:
-00002550: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
-00002560: 7267 735b 2761 7267 3527 5d20 3d20 6964  rgs['arg5'] = id
-00002570: 5f61 6765 6e74 655f 696e 666f 726d 6164  _agente_informad
-00002580: 6f72 0a20 2020 2020 2020 2069 6620 6774  or.        if gt
-00002590: 696e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  in is not None:.
-000025a0: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-000025b0: 6773 5b27 6172 6736 275d 203d 2067 7469  gs['arg6'] = gti
-000025c0: 6e0a 2020 2020 2020 2020 6966 2069 645f  n.        if id_
-000025d0: 6576 656e 746f 2069 7320 6e6f 7420 4e6f  evento is not No
-000025e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000025f0: 6b77 6172 6773 5b27 6172 6737 275d 203d  kwargs['arg7'] =
-00002600: 2069 645f 6576 656e 746f 0a20 2020 2020   id_evento.     
-00002610: 2020 2069 6620 6361 6e74 5f61 6e61 6c69     if cant_anali
-00002620: 7469 6361 2069 7320 6e6f 7420 4e6f 6e65  tica is not None
-00002630: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
-00002640: 6172 6773 5b27 6172 6738 275d 203d 2063  args['arg8'] = c
-00002650: 616e 745f 616e 616c 6974 6963 610a 2020  ant_analitica.  
-00002660: 2020 2020 2020 6966 2066 6563 6861 5f64        if fecha_d
-00002670: 6573 6465 5f6f 7020 6973 206e 6f74 204e  esde_op is not N
-00002680: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00002690: 206b 7761 7267 735b 2761 7267 3927 5d20   kwargs['arg9'] 
-000026a0: 3d20 6665 6368 615f 6465 7364 655f 6f70  = fecha_desde_op
-000026b0: 0a20 2020 2020 2020 2069 6620 6665 6368  .        if fech
-000026c0: 615f 6861 7374 615f 6f70 2069 7320 6e6f  a_hasta_op is no
-000026d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000026e0: 2020 2020 6b77 6172 6773 5b27 6172 6731      kwargs['arg1
-000026f0: 3027 5d20 3d20 6665 6368 615f 6861 7374  0'] = fecha_hast
-00002700: 615f 6f70 0a20 2020 2020 2020 2069 6620  a_op.        if 
-00002710: 6665 6368 615f 6465 7364 655f 7420 6973  fecha_desde_t is
-00002720: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00002730: 2020 2020 2020 206b 7761 7267 735b 2761         kwargs['a
-00002740: 7267 3131 275d 203d 2066 6563 6861 5f64  rg11'] = fecha_d
-00002750: 6573 6465 5f74 0a20 2020 2020 2020 2069  esde_t.        i
-00002760: 6620 6665 6368 615f 6861 7374 615f 7420  f fecha_hasta_t 
-00002770: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00002780: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
-00002790: 2761 7267 3132 275d 203d 2066 6563 6861  'arg12'] = fecha
-000027a0: 5f68 6173 7461 5f74 0a20 2020 2020 2020  _hasta_t.       
-000027b0: 2069 6620 6964 5f74 6970 6f20 6973 206e   if id_tipo is n
-000027c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000027d0: 2020 2020 206b 7761 7267 735b 2761 7267       kwargs['arg
-000027e0: 3133 275d 203d 2069 645f 7469 706f 0a20  13'] = id_tipo. 
-000027f0: 2020 2020 2020 2069 6620 6964 5f65 7374         if id_est
-00002800: 6164 6f20 6973 206e 6f74 204e 6f6e 653a  ado is not None:
-00002810: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
-00002820: 7267 735b 2761 7267 3134 275d 203d 2069  rgs['arg14'] = i
-00002830: 645f 6573 7461 646f 0a20 2020 2020 2020  d_estado.       
-00002840: 2069 6620 6e72 6f5f 7061 6720 6973 206e   if nro_pag is n
-00002850: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00002860: 2020 2020 206b 7761 7267 735b 2761 7267       kwargs['arg
-00002870: 3135 275d 203d 206e 726f 5f70 6167 0a20  15'] = nro_pag. 
-00002880: 2020 2020 2020 2069 6620 6361 6e74 5f72         if cant_r
-00002890: 6567 2069 7320 6e6f 7420 4e6f 6e65 3a0a  eg is not None:.
-000028a0: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-000028b0: 6773 5b27 6172 6731 3627 5d20 3d20 6361  gs['arg16'] = ca
-000028c0: 6e74 5f72 6567 0a0a 2020 2020 2020 2020  nt_reg..        
-000028d0: 2320 6c6c 616d 6f20 616c 2077 6562 7365  # llamo al webse
-000028e0: 7276 6963 650a 2020 2020 2020 2020 7265  rvice.        re
-000028f0: 7320 3d20 7365 6c66 2e63 6c69 656e 742e  s = self.client.
-00002900: 6765 7454 7261 6e73 6163 6369 6f6e 6573  getTransacciones
-00002910: 5773 280a 2020 2020 2020 2020 2020 2020  Ws(.            
-00002920: 6172 6730 3d75 7375 6172 696f 2c0a 2020  arg0=usuario,.  
-00002930: 2020 2020 2020 2020 2020 6172 6731 3d70            arg1=p
-00002940: 6173 7377 6f72 642c 0a20 2020 2020 2020  assword,.       
-00002950: 2020 2020 202a 2a6b 7761 7267 730a 2020       **kwargs.  
-00002960: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00002970: 7265 7420 3d20 7265 735b 2772 6574 7572  ret = res['retur
-00002980: 6e27 5d0a 2020 2020 2020 2020 6966 2072  n'].        if r
-00002990: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
-000029a0: 7365 6c66 2e5f 5f61 6e61 6c69 7a61 725f  self.__analizar_
-000029b0: 6572 726f 7265 7328 7265 7429 0a20 2020  errores(ret).   
-000029c0: 2020 2020 2020 2020 2073 656c 662e 4361           self.Ca
-000029d0: 6e74 5061 6769 6e61 7320 3d20 7265 742e  ntPaginas = ret.
-000029e0: 6765 7428 2763 616e 7450 6167 696e 6173  get('cantPaginas
-000029f0: 2729 0a20 2020 2020 2020 2020 2020 2073  ').            s
-00002a00: 656c 662e 4861 7945 7272 6f72 203d 2072  elf.HayError = r
-00002a10: 6574 2e67 6574 2827 6861 795f 6572 726f  et.get('hay_erro
-00002a20: 7227 290a 2020 2020 2020 2020 2020 2020  r').            
-00002a30: 7365 6c66 2e54 7261 6e73 6163 6369 6f6e  self.Transaccion
-00002a40: 506c 6169 6e57 5320 3d20 5b69 7420 666f  PlainWS = [it fo
-00002a50: 7220 6974 2069 6e20 7265 742e 6765 7428  r it in ret.get(
-00002a60: 276c 6973 7427 2c20 5b5d 295d 0a20 2020  'list', [])].   
-00002a70: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00002a80: 0a0a 2020 2020 6465 6620 5365 7455 7365  ..    def SetUse
-00002a90: 726e 616d 6528 7365 6c66 2c20 7573 6572  rname(self, user
-00002aa0: 6e61 6d65 293a 0a20 2020 2020 2020 2022  name):.        "
-00002ab0: 4573 7461 626c 657a 636f 2065 6c20 6e6f  Establezco el no
-00002ac0: 6d62 7265 2064 6520 7573 7561 7269 6f22  mbre de usuario"
-00002ad0: 0a20 2020 2020 2020 2073 656c 662e 5573  .        self.Us
-00002ae0: 6572 6e61 6d65 203d 2075 7365 726e 616d  ername = usernam
-00002af0: 650a 0a20 2020 2064 6566 2053 6574 5061  e..    def SetPa
-00002b00: 7373 776f 7264 2873 656c 662c 2070 6173  ssword(self, pas
-00002b10: 7377 6f72 6429 3a0a 2020 2020 2020 2020  sword):.        
-00002b20: 2245 7374 6162 6c65 7a63 6f20 6c61 2063  "Establezco la c
-00002b30: 6f6e 7472 6173 65f1 6122 0a20 2020 2020  ontrase.a".     
-00002b40: 2020 2073 656c 662e 5061 7373 776f 7264     self.Password
-00002b50: 203d 2070 6173 7377 6f72 640a 0a20 2020   = password..   
-00002b60: 2064 6566 2047 6574 436f 6469 676f 5472   def GetCodigoTr
-00002b70: 616e 7361 6363 696f 6e28 7365 6c66 293a  ansaccion(self):
-00002b80: 0a20 2020 2020 2020 2022 4465 7675 656c  .        "Devuel
-00002b90: 766f 2065 6c20 63f3 6469 676f 2064 6520  vo el c.digo de 
-00002ba0: 7472 616e 7361 6363 69f3 6e22 0a20 2020  transacci.n".   
-00002bb0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00002bc0: 2e43 6f64 6967 6f54 7261 6e73 6163 6369  .CodigoTransacci
-00002bd0: 6f6e 0a0a 2020 2020 6465 6620 4765 7452  on..    def GetR
-00002be0: 6573 756c 7461 646f 2873 656c 6629 3a0a  esultado(self):.
-00002bf0: 2020 2020 2020 2020 2244 6576 7565 6c76          "Devuelv
-00002c00: 6f20 656c 2072 6573 756c 7461 646f 220a  o el resultado".
-00002c10: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002c20: 656c 662e 5265 7375 6c74 6164 6f0a 0a0a  elf.Resultado...
-00002c30: 0a64 6566 206d 6169 6e28 293a 0a20 2020  .def main():.   
-00002c40: 2022 4675 6e63 69f3 6e20 7072 696e 6369   "Funci.n princi
-00002c50: 7061 6c20 6465 2070 7275 6562 6173 2028  pal de pruebas (
-00002c60: 7472 616e 7361 6363 696f 6e61 7221 2922  transaccionar!)"
-00002c70: 0a20 2020 2069 6d70 6f72 7420 6f73 2c20  .    import os, 
-00002c80: 7469 6d65 2c20 7379 730a 2020 2020 676c  time, sys.    gl
-00002c90: 6f62 616c 2057 5344 4c2c 204c 4f43 4154  obal WSDL, LOCAT
-00002ca0: 494f 4e0a 0a20 2020 2044 4542 5547 203d  ION..    DEBUG =
-00002cb0: 2027 2d2d 6465 6275 6727 2069 6e20 7379   '--debug' in sy
-00002cc0: 732e 6172 6776 0a0a 2020 2020 7773 203d  s.argv..    ws =
-00002cd0: 2054 7261 7a61 5265 6e70 7265 2829 0a0a   TrazaRenpre()..
-00002ce0: 2020 2020 7773 2e55 7365 726e 616d 6520      ws.Username 
-00002cf0: 3d20 2774 6573 7477 7365 7276 6963 6527  = 'testwservice'
-00002d00: 0a20 2020 2077 732e 5061 7373 776f 7264  .    ws.Password
-00002d10: 203d 2027 7465 7374 7773 6572 7669 6365   = 'testwservice
-00002d20: 7073 7727 0a0a 2020 2020 6966 2027 2d2d  psw'..    if '--
-00002d30: 7072 6f64 2720 696e 2073 7973 2e61 7267  prod' in sys.arg
-00002d40: 7620 616e 6420 6e6f 7420 484f 4d4f 3a0a  v and not HOMO:.
-00002d50: 2020 2020 2020 2020 5753 444c 203d 2022          WSDL = "
-00002d60: 6874 7470 733a 2f2f 7472 617a 6162 696c  https://trazabil
-00002d70: 6964 6164 2e70 616d 692e 6f72 672e 6172  idad.pami.org.ar
-00002d80: 3a35 3930 3530 2f74 7261 7a61 6d65 642e  :59050/trazamed.
-00002d90: 5765 6253 6572 7669 6365 5344 524e 3f77  WebServiceSDRN?w
-00002da0: 7364 6c22 0a20 2020 2020 2020 2070 7269  sdl".        pri
-00002db0: 6e74 2822 5573 616e 646f 2057 5344 4c3a  nt("Usando WSDL:
-00002dc0: 222c 2057 5344 4c29 0a20 2020 2020 2020  ", WSDL).       
-00002dd0: 2073 7973 2e61 7267 762e 706f 7028 3029   sys.argv.pop(0)
-00002de0: 0a0a 2020 2020 7773 2e43 6f6e 6563 7461  ..    ws.Conecta
-00002df0: 7228 2222 2c20 5753 444c 290a 0a20 2020  r("", WSDL)..   
-00002e00: 2069 6620 7773 2e45 7863 6570 6369 6f6e   if ws.Excepcion
-00002e10: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
-00002e20: 7773 2e45 7863 6570 6369 6f6e 290a 2020  ws.Excepcion).  
-00002e30: 2020 2020 2020 7072 696e 7428 7773 2e54        print(ws.T
-00002e40: 7261 6365 6261 636b 290a 2020 2020 2020  raceback).      
-00002e50: 2020 7379 732e 6578 6974 282d 3129 0a0a    sys.exit(-1)..
-00002e60: 2020 2020 2320 7072 696e 7428 7773 2e63      # print(ws.c
-00002e70: 6c69 656e 742e 7365 7276 6963 6573 290a  lient.services).
-00002e80: 2020 2020 2320 6f70 203d 2077 732e 636c      # op = ws.cl
-00002e90: 6965 6e74 2e67 6574 5f6f 7065 7261 7469  ient.get_operati
-00002ea0: 6f6e 2822 7365 6e64 4d65 6469 6361 6d65  on("sendMedicame
-00002eb0: 6e74 6f73 2229 0a20 2020 2023 2069 6d70  ntos").    # imp
-00002ec0: 6f72 7420 7064 623b 7064 622e 7365 745f  ort pdb;pdb.set_
-00002ed0: 7472 6163 6528 290a 2020 2020 6966 2027  trace().    if '
-00002ee0: 2d2d 7465 7374 2720 696e 2073 7973 2e61  --test' in sys.a
-00002ef0: 7267 763a 0a20 2020 2020 2020 2077 732e  rgv:.        ws.
-00002f00: 5361 7665 5472 616e 7361 6363 696f 6e65  SaveTransaccione
-00002f10: 7328 0a20 2020 2020 2020 2020 2020 2075  s(.            u
-00002f20: 7375 6172 696f 3d27 7072 7565 6261 7377  suario='pruebasw
-00002f30: 7327 2c20 7061 7373 776f 7264 3d27 7072  s', password='pr
-00002f40: 7565 6261 7377 7327 2c0a 2020 2020 2020  uebasws',.      
-00002f50: 2020 2020 2020 676c 6e5f 6f72 6967 656e        gln_origen
-00002f60: 3d38 3838 3838 3838 3838 3838 3838 2c0a  =8888888888888,.
-00002f70: 2020 2020 2020 2020 2020 2020 676c 6e5f              gln_
-00002f80: 6465 7374 696e 6f3d 3838 3838 3838 3838  destino=88888888
-00002f90: 3838 3838 382c 0a20 2020 2020 2020 2020  88888,.         
-00002fa0: 2020 2066 5f6f 7065 7261 6369 6f6e 3d22     f_operacion="
-00002fb0: 3230 2f30 352f 3230 3134 222c 0a20 2020  20/05/2014",.   
-00002fc0: 2020 2020 2020 2020 2069 645f 6576 656e           id_even
-00002fd0: 746f 3d34 342c 0a20 2020 2020 2020 2020  to=44,.         
-00002fe0: 2020 2063 6f64 5f70 726f 6475 6374 6f3d     cod_producto=
-00002ff0: 3838 3830 3030 3030 3030 3030 3335 2c20  88800000000035, 
-00003000: 2320 6163 6964 6f20 7375 6c66 fa72 6963  # acido sulf.ric
-00003010: 6f0a 2020 2020 2020 2020 2020 2020 6e5f  o.            n_
-00003020: 6361 6e74 6964 6164 3d31 2c0a 2020 2020  cantidad=1,.    
-00003030: 2020 2020 2020 2020 6e5f 646f 6375 6d65          n_docume
-00003040: 6e74 6f5f 6f70 6572 6163 696f 6e3d 312c  nto_operacion=1,
-00003050: 0a20 2020 2020 2020 2020 2020 2023 6d5f  .            #m_
-00003060: 656e 7472 6567 615f 7061 7263 6961 6c3d  entrega_parcial=
-00003070: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
-00003080: 6e5f 7265 6d69 746f 3d31 3233 2c0a 2020  n_remito=123,.  
-00003090: 2020 2020 2020 2020 2020 6e5f 7365 7269            n_seri
-000030a0: 653d 3131 322c 0a20 2020 2020 2020 2020  e=112,.         
-000030b0: 2020 2029 0a20 2020 2020 2020 2070 7269     ).        pri
-000030c0: 6e74 2822 5265 7375 6c74 6164 6f22 2c20  nt("Resultado", 
-000030d0: 7773 2e52 6573 756c 7461 646f 290a 2020  ws.Resultado).  
-000030e0: 2020 2020 2020 7072 696e 7428 2243 6f64        print("Cod
-000030f0: 6967 6f54 7261 6e73 6163 6369 6f6e 222c  igoTransaccion",
-00003100: 2077 732e 436f 6469 676f 5472 616e 7361   ws.CodigoTransa
-00003110: 6363 696f 6e29 0a20 2020 2020 2020 2070  ccion).        p
-00003120: 7269 6e74 2822 4578 6365 7063 696f 6e65  rint("Excepcione
-00003130: 7322 2c20 7773 2e45 7863 6570 6369 6f6e  s", ws.Excepcion
-00003140: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-00003150: 2245 7272 6f65 7322 2c20 7773 2e45 7272  "Erroes", ws.Err
-00003160: 6f72 6573 290a 2020 2020 656c 6966 2027  ores).    elif '
-00003170: 2d2d 6361 6e63 656c 6127 2069 6e20 7379  --cancela' in sy
-00003180: 732e 6172 6776 3a0a 2020 2020 2020 2020  s.argv:.        
-00003190: 7773 2e53 656e 6443 616e 6365 6c61 6354  ws.SendCancelacT
-000031a0: 7261 6e73 6163 6328 2a73 7973 2e61 7267  ransacc(*sys.arg
-000031b0: 765b 7379 732e 6172 6776 2e69 6e64 6578  v[sys.argv.index
-000031c0: 2822 2d2d 6361 6e63 656c 6122 292b 313a  ("--cancela")+1:
-000031d0: 5d29 0a20 2020 2065 6c69 6620 272d 2d63  ]).    elif '--c
-000031e0: 6f6e 7375 6c74 6127 2069 6e20 7379 732e  onsulta' in sys.
-000031f0: 6172 6776 3a0a 2020 2020 2020 2020 6966  argv:.        if
-00003200: 2027 2d2d 6d6f 7669 6d69 656e 746f 7327   '--movimientos'
-00003210: 2069 6e20 7379 732e 6172 6776 3a0a 2020   in sys.argv:.  
-00003220: 2020 2020 2020 2020 2020 7773 2e47 6574            ws.Get
-00003230: 5472 616e 7361 6363 696f 6e65 7357 5328  TransaccionesWS(
-00003240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003260: 202a 7379 732e 6172 6776 5b73 7973 2e61   *sys.argv[sys.a
-00003270: 7267 762e 696e 6465 7828 222d 2d6d 6f76  rgv.index("--mov
-00003280: 696d 6965 6e74 6f73 2229 2b31 3a5d 0a20  imientos")+1:]. 
-00003290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032a0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000032b0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-000032c0: 2020 2077 732e 5361 7665 5472 616e 7361     ws.SaveTransa
-000032d0: 6363 696f 6e65 7328 2a73 7973 2e61 7267  cciones(*sys.arg
-000032e0: 765b 313a 5d29 0a20 2020 2070 7269 6e74  v[1:]).    print
-000032f0: 2822 7c52 6573 756c 7461 646f 2025 3573  ("|Resultado %5s
-00003300: 7c43 6f64 6967 6f54 7261 6e73 6163 6369  |CodigoTransacci
-00003310: 6f6e 2025 3130 737c 4572 726f 7265 737c  on %10s|Errores|
-00003320: 2573 7c22 2025 2028 0a20 2020 2020 2020  %s|" % (.       
-00003330: 2020 2020 2077 732e 5265 7375 6c74 6164       ws.Resultad
-00003340: 6f2c 0a20 2020 2020 2020 2020 2020 2077  o,.            w
-00003350: 732e 436f 6469 676f 5472 616e 7361 6363  s.CodigoTransacc
-00003360: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00003370: 2027 7c27 2e6a 6f69 6e28 7773 2e45 7272   '|'.join(ws.Err
-00003380: 6f72 6573 292c 0a20 2020 2020 2020 2020  ores),.         
-00003390: 2020 2029 290a 2020 2020 6966 2077 732e     )).    if ws.
-000033a0: 4578 6365 7063 696f 6e3a 0a20 2020 2020  Excepcion:.     
-000033b0: 2020 2070 7269 6e74 2877 732e 5472 6163     print(ws.Trac
-000033c0: 6562 6163 6b29 0a0a 2320 6275 7363 6f20  eback)..# busco 
-000033d0: 656c 2064 6972 6563 746f 7269 6f20 6465  el directorio de
-000033e0: 2069 6e73 7461 6c61 6369 f36e 2028 676c   instalaci.n (gl
-000033f0: 6f62 616c 2070 6172 6120 7175 6520 6e6f  obal para que no
-00003400: 2063 616d 6269 6520 7369 2075 7361 6e20   cambie si usan 
-00003410: 6f74 7261 2064 6c6c 290a 494e 5354 414c  otra dll).INSTAL
-00003420: 4c5f 4449 5220 3d20 5472 617a 6152 656e  L_DIR = TrazaRen
-00003430: 7072 652e 496e 7374 616c 6c44 6972 203d  pre.InstallDir =
-00003440: 2067 6574 5f69 6e73 7461 6c6c 5f64 6972   get_install_dir
-00003450: 2829 0a0a 0a69 6620 5f5f 6e61 6d65 5f5f  ()...if __name__
-00003460: 203d 3d20 275f 5f6d 6169 6e5f 5f27 3a0a   == '__main__':.
-00003470: 0a20 2020 2023 2061 6a75 7374 6f20 656c  .    # ajusto el
-00003480: 2065 6e63 6f64 696e 6720 706f 7220 6465   encoding por de
-00003490: 6665 6374 6f20 2873 6920 7365 2072 6564  fecto (si se red
-000034a0: 6972 696a 6520 6c61 2073 616c 6964 6129  irije la salida)
-000034b0: 0a20 2020 2069 6620 7379 732e 7374 646f  .    if sys.stdo
-000034c0: 7574 2e65 6e63 6f64 696e 6720 6973 204e  ut.encoding is N
-000034d0: 6f6e 653a 0a20 2020 2020 2020 2069 6d70  one:.        imp
-000034e0: 6f72 7420 636f 6465 6373 2c20 6c6f 6361  ort codecs, loca
-000034f0: 6c65 0a20 2020 2020 2020 2073 7973 2e73  le.        sys.s
-00003500: 7464 6f75 7420 3d20 636f 6465 6373 2e67  tdout = codecs.g
-00003510: 6574 7772 6974 6572 286c 6f63 616c 652e  etwriter(locale.
-00003520: 6765 7470 7265 6665 7272 6564 656e 636f  getpreferredenco
-00003530: 6469 6e67 2829 2928 7379 732e 7374 646f  ding())(sys.stdo
-00003540: 7574 2c22 7265 706c 6163 6522 293b 0a20  ut,"replace");. 
-00003550: 2020 2020 2020 2073 7973 2e73 7464 6572         sys.stder
-00003560: 7220 3d20 636f 6465 6373 2e67 6574 7772  r = codecs.getwr
-00003570: 6974 6572 286c 6f63 616c 652e 6765 7470  iter(locale.getp
-00003580: 7265 6665 7272 6564 656e 636f 6469 6e67  referredencoding
-00003590: 2829 2928 7379 732e 7374 6465 7272 2c22  ())(sys.stderr,"
-000035a0: 7265 706c 6163 6522 293b 0a0a 2020 2020  replace");..    
-000035b0: 6966 2027 2d2d 7265 6769 7374 6572 2720  if '--register' 
-000035c0: 696e 2073 7973 2e61 7267 7620 6f72 2027  in sys.argv or '
-000035d0: 2d2d 756e 7265 6769 7374 6572 2720 696e  --unregister' in
-000035e0: 2073 7973 2e61 7267 763a 0a20 2020 2020   sys.argv:.     
-000035f0: 2020 2069 6d70 6f72 7420 7079 7468 6f6e     import python
-00003600: 636f 6d0a 2020 2020 2020 2020 696d 706f  com.        impo
-00003610: 7274 2077 696e 3332 636f 6d2e 7365 7276  rt win32com.serv
-00003620: 6572 2e72 6567 6973 7465 720a 2020 2020  er.register.    
-00003630: 2020 2020 7769 6e33 3263 6f6d 2e73 6572      win32com.ser
-00003640: 7665 722e 7265 6769 7374 6572 2e55 7365  ver.register.Use
-00003650: 436f 6d6d 616e 644c 696e 6528 5472 617a  CommandLine(Traz
-00003660: 6152 656e 7072 6529 0a20 2020 2065 6c69  aRenpre).    eli
-00003670: 6620 222f 4175 746f 6d61 7465 2220 696e  f "/Automate" in
-00003680: 2073 7973 2e61 7267 763a 0a20 2020 2020   sys.argv:.     
-00003690: 2020 2023 204d 5320 7365 656d 7320 746f     # MS seems to
-000036a0: 206c 696b 6520 2f61 7574 6f6d 6174 6520   like /automate 
-000036b0: 746f 2072 756e 2074 6865 2063 6c61 7373  to run the class
-000036c0: 2066 6163 746f 7269 6573 2e0a 2020 2020   factories..    
-000036d0: 2020 2020 696d 706f 7274 2077 696e 3332      import win32
-000036e0: 636f 6d2e 7365 7276 6572 2e6c 6f63 616c  com.server.local
-000036f0: 7365 7276 6572 0a20 2020 2020 2020 2023  server.        #
-00003700: 7769 6e33 3263 6f6d 2e73 6572 7665 722e  win32com.server.
-00003710: 6c6f 6361 6c73 6572 7665 722e 6d61 696e  localserver.main
-00003720: 2829 0a20 2020 2020 2020 2023 2073 7461  ().        # sta
-00003730: 7274 2074 6865 2073 6572 7665 722e 0a20  rt the server.. 
-00003740: 2020 2020 2020 2077 696e 3332 636f 6d2e         win32com.
-00003750: 7365 7276 6572 2e6c 6f63 616c 7365 7276  server.localserv
-00003760: 6572 2e73 6572 7665 285b 5472 617a 6152  er.serve([TrazaR
-00003770: 656e 7072 652e 5f72 6567 5f63 6c73 6964  enpre._reg_clsid
-00003780: 5f5d 290a 2020 2020 656c 7365 3a0a 2020  _]).    else:.  
-00003790: 2020 2020 2020 6d61 696e 2829 0a               main().
+00000010: 6e0a 2320 2d2a 2d20 636f 6469 6e67 3a20  n.# -*- coding: 
+00000020: 7574 662d 3820 2d2a 2d0a 2320 5468 6973  utf-8 -*-.# This
+00000030: 2070 726f 6772 616d 2069 7320 6672 6565   program is free
+00000040: 2073 6f66 7477 6172 653b 2079 6f75 2063   software; you c
+00000050: 616e 2072 6564 6973 7472 6962 7574 6520  an redistribute 
+00000060: 6974 2061 6e64 2f6f 7220 6d6f 6469 6679  it and/or modify
+00000070: 0a23 2069 7420 756e 6465 7220 7468 6520  .# it under the 
+00000080: 7465 726d 7320 6f66 2074 6865 2047 4e55  terms of the GNU
+00000090: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
+000000a0: 4c69 6365 6e73 6520 6173 2070 7562 6c69  License as publi
+000000b0: 7368 6564 2062 7920 7468 650a 2320 4672  shed by the.# Fr
+000000c0: 6565 2053 6f66 7477 6172 6520 466f 756e  ee Software Foun
+000000d0: 6461 7469 6f6e 3b20 6569 7468 6572 2076  dation; either v
+000000e0: 6572 7369 6f6e 2033 2c20 6f72 2028 6174  ersion 3, or (at
+000000f0: 2079 6f75 7220 6f70 7469 6f6e 2920 616e   your option) an
+00000100: 7920 6c61 7465 720a 2320 7665 7273 696f  y later.# versio
+00000110: 6e2e 0a23 0a23 2054 6869 7320 7072 6f67  n..#.# This prog
+00000120: 7261 6d20 6973 2064 6973 7472 6962 7574  ram is distribut
+00000130: 6564 2069 6e20 7468 6520 686f 7065 2074  ed in the hope t
+00000140: 6861 7420 6974 2077 696c 6c20 6265 2075  hat it will be u
+00000150: 7365 6675 6c2c 2062 7574 0a23 2057 4954  seful, but.# WIT
+00000160: 484f 5554 2041 4e59 2057 4152 5241 4e54  HOUT ANY WARRANT
+00000170: 593b 2077 6974 686f 7574 2065 7665 6e20  Y; without even 
+00000180: 7468 6520 696d 706c 6965 6420 7761 7272  the implied warr
+00000190: 616e 7479 206f 6620 4d45 5243 4841 4e54  anty of MERCHANT
+000001a0: 4942 494c 4954 590a 2320 6f72 2046 4954  IBILITY.# or FIT
+000001b0: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
+000001c0: 4355 4c41 5220 5055 5250 4f53 452e 2020  CULAR PURPOSE.  
+000001d0: 5365 6520 7468 6520 474e 5520 4765 6e65  See the GNU Gene
+000001e0: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
+000001f0: 7365 0a23 2066 6f72 206d 6f72 6520 6465  se.# for more de
+00000200: 7461 696c 732e 0a0a 224d f364 756c 6f20  tails..."M.dulo 
+00000210: 7061 7261 2054 7261 7a61 6269 6c69 6461  para Trazabilida
+00000220: 6420 6465 2050 7265 6375 7273 6f72 6573  d de Precursores
+00000230: 2051 75ed 6d69 636f 7320 5245 4e50 5245   Qu.micos RENPRE
+00000240: 2052 6573 6f6c 7563 69f3 6e20 3930 302f   Resoluci.n 900/
+00000250: 3132 220a 0a23 2049 6e66 6f72 6d61 6369  12"..# Informaci
+00000260: f36e 2061 6469 6369 6f6e 616c 2079 2064  .n adicional y d
+00000270: 6f63 756d 656e 7461 6369 f36e 3a0a 2320  ocumentaci.n:.# 
+00000280: 6874 7470 3a2f 2f77 7777 2e73 6973 7465  http://www.siste
+00000290: 6d61 7361 6769 6c65 732e 636f 6d2e 6172  masagiles.com.ar
+000002a0: 2f74 7261 632f 7769 6b69 2f54 7261 7a61  /trac/wiki/Traza
+000002b0: 6269 6c69 6461 6450 7265 6375 7273 6f72  bilidadPrecursor
+000002c0: 6573 5175 696d 6963 6f73 0a0a 5f5f 6175  esQuimicos..__au
+000002d0: 7468 6f72 5f5f 203d 2022 4d61 7269 616e  thor__ = "Marian
+000002e0: 6f20 5265 696e 6761 7274 203c 7265 696e  o Reingart <rein
+000002f0: 6761 7274 4067 6d61 696c 2e63 6f6d 3e22  gart@gmail.com>"
+00000300: 0a5f 5f63 6f70 7972 6967 6874 5f5f 203d  .__copyright__ =
+00000310: 2022 436f 7079 7269 6768 7420 2843 2920   "Copyright (C) 
+00000320: 3230 3131 204d 6172 6961 6e6f 2052 6569  2011 Mariano Rei
+00000330: 6e67 6172 7422 0a5f 5f6c 6963 656e 7365  ngart".__license
+00000340: 5f5f 203d 2022 4750 4c20 332e 302b 220a  __ = "GPL 3.0+".
+00000350: 5f5f 7665 7273 696f 6e5f 5f20 3d20 2231  __version__ = "1
+00000360: 2e31 3261 220a 0a23 6874 7470 3a2f 2f72  .12a"..#http://r
+00000370: 656e 7072 652e 7365 7276 6963 696f 732e  enpre.servicios.
+00000380: 7061 6d69 2e6f 7267 2e61 722f 706f 7274  pami.org.ar/port
+00000390: 616c 5f74 7261 7a61 5f72 656e 7072 652f  al_traza_renpre/
+000003a0: 7061 736f 352e 6874 6d6c 0a0a 696d 706f  paso5.html..impo
+000003b0: 7274 206f 730a 696d 706f 7274 2073 6f63  rt os.import soc
+000003c0: 6b65 740a 696d 706f 7274 2073 7973 0a69  ket.import sys.i
+000003d0: 6d70 6f72 7420 6461 7465 7469 6d65 2c20  mport datetime, 
+000003e0: 7469 6d65 0a69 6d70 6f72 7420 7079 3373  time.import py3s
+000003f0: 696d 706c 6573 6f61 702e 636c 6965 6e74  implesoap.client
+00000400: 0a66 726f 6d20 7079 3373 696d 706c 6573  .from py3simples
+00000410: 6f61 702e 636c 6965 6e74 2069 6d70 6f72  oap.client impor
+00000420: 7420 536f 6170 4661 756c 740a 6672 6f6d  t SoapFault.from
+00000430: 202e 7574 696c 7320 696d 706f 7274 2042   .utils import B
+00000440: 6173 6557 532c 2069 6e69 6369 616c 697a  aseWS, inicializ
+00000450: 6172 5f79 5f63 6170 7475 7261 725f 6578  ar_y_capturar_ex
+00000460: 6365 7063 696f 6e65 732c 2067 6574 5f69  cepciones, get_i
+00000470: 6e73 7461 6c6c 5f64 6972 0a0a 484f 4d4f  nstall_dir..HOMO
+00000480: 203d 2046 616c 7365 0a54 5950 454c 4942   = False.TYPELIB
+00000490: 203d 2046 616c 7365 0a0a 5753 444c 203d   = False..WSDL =
+000004a0: 2022 6874 7470 733a 2f2f 7365 7276 6963   "https://servic
+000004b0: 696f 732e 7061 6d69 2e6f 7267 2e61 722f  ios.pami.org.ar/
+000004c0: 7472 617a 616d 6564 2e57 6562 5365 7276  trazamed.WebServ
+000004d0: 6963 6553 4452 4e3f 7773 646c 220a 4c4f  iceSDRN?wsdl".LO
+000004e0: 4341 5449 4f4e 203d 2022 6874 7470 733a  CATION = "https:
+000004f0: 2f2f 7365 7276 6963 696f 732e 7061 6d69  //servicios.pami
+00000500: 2e6f 7267 2e61 722f 7472 617a 616d 6564  .org.ar/trazamed
+00000510: 2e57 6562 5365 7276 6963 6553 4452 4e3f  .WebServiceSDRN?
+00000520: 7773 646c 220a 2323 5753 444c 203d 2022  wsdl".##WSDL = "
+00000530: 6874 7470 733a 2f2f 7472 617a 6162 696c  https://trazabil
+00000540: 6964 6164 2e70 616d 692e 6f72 672e 6172  idad.pami.org.ar
+00000550: 3a35 3930 3530 2f74 7261 7a61 6d65 642e  :59050/trazamed.
+00000560: 5765 6253 6572 7669 6365 5344 524e 3f77  WebServiceSDRN?w
+00000570: 7364 6c22 2020 2320 7072 6f64 2e0a 0a63  sdl"  # prod...c
+00000580: 6c61 7373 2054 7261 7a61 5265 6e70 7265  lass TrazaRenpre
+00000590: 2842 6173 6557 5329 3a0a 2020 2020 2249  (BaseWS):.    "I
+000005a0: 6e74 6572 6661 7a20 7061 7261 2065 6c20  nterfaz para el 
+000005b0: 5765 6253 6572 7669 6365 2064 6520 5472  WebService de Tr
+000005c0: 617a 6162 696c 6964 6164 2064 6520 5072  azabilidad de Pr
+000005d0: 6563 7572 736f 7265 7320 5175 696d 6963  ecursores Quimic
+000005e0: 6f73 2053 4544 524f 4e41 5220 534e 5422  os SEDRONAR SNT"
+000005f0: 0a20 2020 205f 7075 626c 6963 5f6d 6574  .    _public_met
+00000600: 686f 6473 5f20 3d20 5b27 5361 7665 5472  hods_ = ['SaveTr
+00000610: 616e 7361 6363 696f 6e65 7327 2c0a 2020  ansacciones',.  
+00000620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000630: 2020 2020 2020 2753 656e 6443 616e 6365        'SendCance
+00000640: 6c61 6354 7261 6e73 6163 6327 2c20 2747  lacTransacc', 'G
+00000650: 6574 5472 616e 7361 6363 696f 6e65 7357  etTransaccionesW
+00000660: 5327 2c0a 2020 2020 2020 2020 2020 2020  S',.            
+00000670: 2020 2020 2020 2020 2020 2020 2743 6f6e              'Con
+00000680: 6563 7461 7227 2c20 274c 6565 7245 7272  ectar', 'LeerErr
+00000690: 6f72 272c 2027 4c65 6572 5472 616e 7361  or', 'LeerTransa
+000006a0: 6363 696f 6e27 2c0a 2020 2020 2020 2020  ccion',.        
+000006b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006c0: 2753 6574 5573 6572 6e61 6d65 272c 0a20  'SetUsername',. 
+000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006e0: 2020 2020 2020 2027 5365 7450 6172 616d         'SetParam
+000006f0: 6574 726f 272c 2027 4765 7450 6172 616d  etro', 'GetParam
+00000700: 6574 726f 272c 0a20 2020 2020 2020 2020  etro',.         
+00000710: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00000720: 4765 7443 6f64 6967 6f54 7261 6e73 6163  GetCodigoTransac
+00000730: 6369 6f6e 272c 2027 4765 7452 6573 756c  cion', 'GetResul
+00000740: 7461 646f 272c 2027 4c6f 6164 5465 7374  tado', 'LoadTest
+00000750: 584d 4c27 5d0a 0a20 2020 205f 7075 626c  XML']..    _publ
+00000760: 6963 5f61 7474 7273 5f20 3d20 5b0a 2020  ic_attrs_ = [.  
+00000770: 2020 2020 2020 2755 7365 726e 616d 6527        'Username'
+00000780: 2c20 2750 6173 7377 6f72 6427 2c0a 2020  , 'Password',.  
+00000790: 2020 2020 2020 2743 6f64 6967 6f54 7261        'CodigoTra
+000007a0: 6e73 6163 6369 6f6e 272c 2027 4572 726f  nsaccion', 'Erro
+000007b0: 7265 7327 2c20 2752 6573 756c 7461 646f  res', 'Resultado
+000007c0: 272c 0a20 2020 2020 2020 2027 586d 6c52  ',.        'XmlR
+000007d0: 6571 7565 7374 272c 2027 586d 6c52 6573  equest', 'XmlRes
+000007e0: 706f 6e73 6527 2c0a 2020 2020 2020 2020  ponse',.        
+000007f0: 2756 6572 7369 6f6e 272c 2027 496e 7374  'Version', 'Inst
+00000800: 616c 6c44 6972 272c 0a20 2020 2020 2020  allDir',.       
+00000810: 2027 5472 6163 6562 6163 6b27 2c20 2745   'Traceback', 'E
+00000820: 7863 6570 6369 6f6e 272c 2027 4c61 6e7a  xcepcion', 'Lanz
+00000830: 6172 4578 6365 7063 696f 6e65 7327 2c0a  arExcepciones',.
+00000840: 2020 2020 2020 2020 5d0a 0a20 2020 205f          ]..    _
+00000850: 7265 675f 7072 6f67 6964 5f20 3d20 2254  reg_progid_ = "T
+00000860: 7261 7a61 5265 6e70 7265 220a 2020 2020  razaRenpre".    
+00000870: 5f72 6567 5f63 6c73 6964 5f20 3d20 227b  _reg_clsid_ = "{
+00000880: 3436 3132 3938 4442 2d30 3533 312d 3437  461298DB-0531-47
+00000890: 4341 2d42 3344 392d 4233 3646 4536 3936  CA-B3D9-B36FE696
+000008a0: 3732 3039 7d22 0a0a 2020 2020 2320 5661  7209}"..    # Va
+000008b0: 7269 6162 6c65 7320 676c 6f62 616c 6573  riables globales
+000008c0: 2070 6172 6120 4261 7365 5753 3a0a 2020   para BaseWS:.  
+000008d0: 2020 484f 4d4f 203d 2048 4f4d 4f0a 2020    HOMO = HOMO.  
+000008e0: 2020 5753 444c 203d 2057 5344 4c0a 2020    WSDL = WSDL.  
+000008f0: 2020 5665 7273 696f 6e20 3d20 2225 7320    Version = "%s 
+00000900: 2573 2025 7322 2025 2028 5f5f 7665 7273  %s %s" % (__vers
+00000910: 696f 6e5f 5f2c 2048 4f4d 4f20 616e 6420  ion__, HOMO and 
+00000920: 2748 6f6d 6f6c 6f67 6163 69f3 6e27 206f  'Homologaci.n' o
+00000930: 7220 2727 2c0a 2020 2020 2020 2020 2020  r '',.          
+00000940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000950: 2020 7079 3373 696d 706c 6573 6f61 702e    py3simplesoap.
+00000960: 636c 6965 6e74 2e5f 5f76 6572 7369 6f6e  client.__version
+00000970: 5f5f 290a 0a20 2020 2064 6566 205f 5f69  __)..    def __i
+00000980: 6e69 745f 5f28 7365 6c66 2c20 7265 696e  nit__(self, rein
+00000990: 7465 6e74 6f73 3d31 293a 0a20 2020 2020  tentos=1):.     
+000009a0: 2020 2073 656c 662e 5573 6572 6e61 6d65     self.Username
+000009b0: 203d 2073 656c 662e 5061 7373 776f 7264   = self.Password
+000009c0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+000009d0: 4261 7365 5753 2e5f 5f69 6e69 745f 5f28  BaseWS.__init__(
+000009e0: 7365 6c66 2c20 7265 696e 7465 6e74 6f73  self, reintentos
+000009f0: 290a 0a20 2020 2064 6566 2069 6e69 6369  )..    def inici
+00000a00: 616c 697a 6172 2873 656c 6629 3a0a 2020  alizar(self):.  
+00000a10: 2020 2020 2020 4261 7365 5753 2e69 6e69        BaseWS.ini
+00000a20: 6369 616c 697a 6172 2873 656c 6629 0a20  cializar(self). 
+00000a30: 2020 2020 2020 2073 656c 662e 436f 6469         self.Codi
+00000a40: 676f 5472 616e 7361 6363 696f 6e20 3d20  goTransaccion = 
+00000a50: 7365 6c66 2e45 7272 6f72 6573 203d 2073  self.Errores = s
+00000a60: 656c 662e 5265 7375 6c74 6164 6f20 3d20  elf.Resultado = 
+00000a70: 4e6f 6e65 0a0a 2020 2020 6465 6620 5f5f  None..    def __
+00000a80: 616e 616c 697a 6172 5f65 7272 6f72 6573  analizar_errores
+00000a90: 2873 656c 662c 2072 6574 293a 0a20 2020  (self, ret):.   
+00000aa0: 2020 2020 2022 436f 6d70 7275 6562 6120       "Comprueba 
+00000ab0: 7920 6578 7472 6165 2065 7272 6f72 6573  y extrae errores
+00000ac0: 2073 6920 6578 6973 7465 6e20 656e 206c   si existen en l
+00000ad0: 6120 7265 7370 7565 7374 6120 584d 4c22  a respuesta XML"
+00000ae0: 0a20 2020 2020 2020 2073 656c 662e 4572  .        self.Er
+00000af0: 726f 7265 7320 3d20 5b22 2573 3a20 2573  rores = ["%s: %s
+00000b00: 2220 2520 2869 742e 6765 7428 275f 635f  " % (it.get('_c_
+00000b10: 6572 726f 7227 2c20 2222 292c 2069 742e  error', ""), it.
+00000b20: 6765 7428 275f 645f 6572 726f 7227 2c20  get('_d_error', 
+00000b30: 2222 2929 0a20 2020 2020 2020 2020 2020  "")).           
+00000b40: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00000b50: 2069 7420 696e 2072 6574 2e67 6574 2827   it in ret.get('
+00000b60: 6572 726f 7265 7327 2c20 5b5d 295d 0a20  errores', [])]. 
+00000b70: 2020 2020 2020 2073 656c 662e 5265 7375         self.Resu
+00000b80: 6c74 6164 6f20 3d20 7265 742e 6765 7428  ltado = ret.get(
+00000b90: 2772 6573 756c 7461 646f 2729 0a0a 2020  'resultado')..  
+00000ba0: 2020 6465 6620 436f 6e65 6374 6172 2873    def Conectar(s
+00000bb0: 656c 662c 2063 6163 6865 3d4e 6f6e 652c  elf, cache=None,
+00000bc0: 2077 7364 6c3d 4e6f 6e65 2c20 7072 6f78   wsdl=None, prox
+00000bd0: 793d 2222 2c20 7772 6170 7065 723d 4e6f  y="", wrapper=No
+00000be0: 6e65 2c20 6361 6365 7274 3d4e 6f6e 652c  ne, cacert=None,
+00000bf0: 2074 696d 656f 7574 3d33 3029 3a0a 2020   timeout=30):.  
+00000c00: 2020 2020 2020 2320 436f 6e65 6374 6f20        # Conecto 
+00000c10: 7573 616e 646f 2065 6c20 6de9 746f 646f  usando el m.todo
+00000c20: 2065 7374 616e 6461 7264 3a0a 2020 2020   estandard:.    
+00000c30: 2020 2020 6f6b 203d 2042 6173 6557 532e      ok = BaseWS.
+00000c40: 436f 6e65 6374 6172 2873 656c 662c 2063  Conectar(self, c
+00000c50: 6163 6865 2c20 7773 646c 2c20 7072 6f78  ache, wsdl, prox
+00000c60: 792c 2077 7261 7070 6572 2c20 6361 6365  y, wrapper, cace
+00000c70: 7274 2c20 7469 6d65 6f75 742c 0a20 2020  rt, timeout,.   
+00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c90: 2020 2020 2020 2020 2020 736f 6170 5f73            soap_s
+00000ca0: 6572 7665 723d 226a 6574 7479 2229 0a20  erver="jetty"). 
+00000cb0: 2020 2020 2020 2069 6620 6f6b 3a0a 2020         if ok:.  
+00000cc0: 2020 2020 2020 2020 2020 2320 7369 2065            # si e
+00000cd0: 6c20 6172 6368 6976 6f20 6573 206c 6f63  l archivo es loc
+00000ce0: 616c 2c20 6173 756d 6f20 7175 6520 7961  al, asumo que ya
+00000cf0: 2065 7374 6120 636f 7272 6567 6964 6f3a   esta corregido:
+00000d00: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00000d10: 6e6f 7420 7365 6c66 2e77 7364 6c2e 7374  not self.wsdl.st
+00000d20: 6172 7473 7769 7468 2822 6669 6c65 2229  artswith("file")
+00000d30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000d40: 2020 2320 636f 7272 696a 6f20 7562 6963    # corrijo ubic
+00000d50: 6163 69f3 6e20 6465 6c20 7365 7276 6964  aci.n del servid
+00000d60: 6f72 2028 6c6f 6361 6c68 6f73 743a 3930  or (localhost:90
+00000d70: 3530 2065 6e20 656c 2057 5344 4c29 0a20  50 en el WSDL). 
+00000d80: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00000d90: 6f63 6174 696f 6e20 3d20 7365 6c66 2e77  ocation = self.w
+00000da0: 7364 6c5b 3a2d 355d 0a20 2020 2020 2020  sdl[:-5].       
+00000db0: 2020 2020 2020 2020 2069 6620 2749 5765           if 'IWe
+00000dc0: 6253 6572 7669 6365 5344 524e 5365 7276  bServiceSDRNServ
+00000dd0: 6963 6527 2069 6e20 7365 6c66 2e63 6c69  ice' in self.cli
+00000de0: 656e 742e 7365 7276 6963 6573 3a0a 2020  ent.services:.  
+00000df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e00: 2020 7773 203d 2073 656c 662e 636c 6965    ws = self.clie
+00000e10: 6e74 2e73 6572 7669 6365 735b 2749 5765  nt.services['IWe
+00000e20: 6253 6572 7669 6365 5344 524e 5365 7276  bServiceSDRNServ
+00000e30: 6963 6527 5d0a 2020 2020 2020 2020 2020  ice'].          
+00000e40: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e60: 7773 203d 2073 656c 662e 636c 6965 6e74  ws = self.client
+00000e70: 2e73 6572 7669 6365 735b 2749 5765 6253  .services['IWebS
+00000e80: 6572 7669 6365 5344 524e 275d 0a20 2020  erviceSDRN'].   
+00000e90: 2020 2020 2020 2020 2020 2020 2077 735b               ws[
+00000ea0: 2770 6f72 7473 275d 5b27 4957 6562 5365  'ports']['IWebSe
+00000eb0: 7276 6963 6553 4452 4e50 6f72 7427 5d5b  rviceSDRNPort'][
+00000ec0: 276c 6f63 6174 696f 6e27 5d20 3d20 6c6f  'location'] = lo
+00000ed0: 6361 7469 6f6e 0a20 2020 2020 2020 2020  cation.         
+00000ee0: 2020 2023 2045 7374 6162 6c65 6365 7220     # Establecer 
+00000ef0: 6372 6564 656e 6369 616c 6573 2064 6520  credenciales de 
+00000f00: 7365 6775 7269 6461 643a 0a20 2020 2020  seguridad:.     
+00000f10: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+00000f20: 6e74 5b27 7773 7365 3a53 6563 7572 6974  nt['wsse:Securit
+00000f30: 7927 5d20 3d20 7b0a 2020 2020 2020 2020  y'] = {.        
+00000f40: 2020 2020 2020 2020 2777 7373 653a 5573          'wsse:Us
+00000f50: 6572 6e61 6d65 546f 6b65 6e27 3a20 7b0a  ernameToken': {.
+00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f70: 2020 2020 2777 7373 653a 5573 6572 6e61      'wsse:Userna
+00000f80: 6d65 273a 2073 656c 662e 5573 6572 6e61  me': self.Userna
+00000f90: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00000fa0: 2020 2020 2020 2020 2777 7373 653a 5061          'wsse:Pa
+00000fb0: 7373 776f 7264 273a 2073 656c 662e 5061  ssword': self.Pa
+00000fc0: 7373 776f 7264 2c0a 2020 2020 2020 2020  ssword,.        
+00000fd0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00000fe0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00000ff0: 2020 2020 2020 2020 7265 7475 726e 206f          return o
+00001000: 6b0a 0a20 2020 2040 696e 6963 6961 6c69  k..    @iniciali
+00001010: 7a61 725f 795f 6361 7074 7572 6172 5f65  zar_y_capturar_e
+00001020: 7863 6570 6369 6f6e 6573 0a20 2020 2064  xcepciones.    d
+00001030: 6566 2053 6176 6554 7261 6e73 6163 6369  ef SaveTransacci
+00001040: 6f6e 6573 2873 656c 662c 2075 7375 6172  ones(self, usuar
+00001050: 696f 2c20 7061 7373 776f 7264 2c0a 2020  io, password,.  
+00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001070: 2020 2020 2020 2067 6c6e 5f6f 7269 6765         gln_orige
+00001080: 6e3d 4e6f 6e65 2c20 676c 6e5f 6465 7374  n=None, gln_dest
+00001090: 696e 6f3d 4e6f 6e65 2c20 665f 6f70 6572  ino=None, f_oper
+000010a0: 6163 696f 6e3d 4e6f 6e65 2c0a 2020 2020  acion=None,.    
+000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010c0: 2020 2020 2069 645f 6576 656e 746f 3d4e       id_evento=N
+000010d0: 6f6e 652c 2063 6f64 5f70 726f 6475 6374  one, cod_product
+000010e0: 6f3d 4e6f 6e65 2c20 6e5f 6361 6e74 6964  o=None, n_cantid
+000010f0: 6164 3d4e 6f6e 652c 0a20 2020 2020 2020  ad=None,.       
+00001100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001110: 2020 6e5f 646f 6375 6d65 6e74 6f5f 6f70    n_documento_op
+00001120: 6572 6163 696f 6e3d 4e6f 6e65 2c20 6e5f  eracion=None, n_
+00001130: 7265 6d69 746f 3d4e 6f6e 652c 0a20 2020  remito=None,.   
+00001140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001150: 2020 2020 2020 6964 5f74 6970 6f5f 7472        id_tipo_tr
+00001160: 616e 7370 6f72 7465 3d4e 6f6e 652c 0a20  ansporte=None,. 
+00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001180: 2020 2020 2020 2020 6964 5f70 6173 6f5f          id_paso_
+00001190: 6672 6f6e 7465 7261 5f69 6e67 7265 736f  frontera_ingreso
+000011a0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+000011b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011c0: 6964 5f70 6173 6f5f 6672 6f6e 7465 7261  id_paso_frontera
+000011d0: 5f65 6772 6573 6f3d 4e6f 6e65 2c0a 2020  _egreso=None,.  
+000011e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011f0: 2020 2020 2020 2069 645f 7469 706f 5f64         id_tipo_d
+00001200: 6f63 756d 656e 746f 5f6f 7065 7261 6369  ocumento_operaci
+00001210: 6f6e 3d4e 6f6e 652c 0a20 2020 2020 2020  on=None,.       
+00001220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001230: 2020 645f 646f 6d69 6e69 6f5f 7472 6163    d_dominio_trac
+00001240: 746f 723d 4e6f 6e65 2c0a 2020 2020 2020  tor=None,.      
+00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001260: 2020 2064 5f64 6f6d 696e 696f 5f73 656d     d_dominio_sem
+00001270: 693d 4e6f 6e65 2c0a 2020 2020 2020 2020  i=None,.        
+00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001290: 206e 5f73 6572 6965 3d4e 6f6e 652c 206e   n_serie=None, n
+000012a0: 5f6c 6f74 653d 4e6f 6e65 2c20 646f 635f  _lote=None, doc_
+000012b0: 6465 7370 6163 686f 5f70 6c61 7a61 3d4e  despacho_plaza=N
+000012c0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+000012d0: 2020 2020 2020 2020 2020 2020 2020 646a                dj
+000012e0: 6169 3d4e 6f6e 652c 206e 5f63 6572 745f  ai=None, n_cert_
+000012f0: 696d 706f 5f65 7870 6f3d 4e6f 6e65 2c0a  impo_expo=None,.
+00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001310: 2020 2020 2020 2020 2069 645f 7469 706f           id_tipo
+00001320: 5f64 6f63 756d 656e 746f 3d4e 6f6e 652c  _documento=None,
+00001330: 206e 5f64 6f63 756d 656e 746f 3d4e 6f6e   n_documento=Non
+00001340: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00001350: 2020 2020 2020 2020 2020 2020 6d5f 6361              m_ca
+00001360: 6c69 6461 645f 616e 616c 6974 6963 613d  lidad_analitica=
+00001370: 4e6f 6e65 2c20 6d5f 656e 7472 6567 615f  None, m_entrega_
+00001380: 7061 7263 6961 6c3d 4e6f 6e65 2c0a 2020  parcial=None,.  
+00001390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013a0: 2020 2020 2020 2064 6f63 5f70 6572 6d69         doc_permi
+000013b0: 736f 5f65 6d62 6172 7175 653d 4e6f 6e65  so_embarque=None
+000013c0: 2c20 676c 6e5f 7472 616e 7370 6f72 7469  , gln_transporti
+000013d0: 7374 613d 4e6f 6e65 2c0a 2020 2020 2020  sta=None,.      
+000013e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013f0: 2020 206f 7065 7261 6369 6f6e 5f65 7863     operacion_exc
+00001400: 656e 746f 5f64 6a61 693d 4e6f 6e65 2c20  ento_djai=None, 
+00001410: 636f 6e74 726f 6c5f 6475 706c 6963 6964  control_duplicid
+00001420: 6164 3d4e 6f6e 652c 0a20 2020 2020 2020  ad=None,.       
+00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001440: 2020 293a 0a20 2020 2020 2020 2022 5065    ):.        "Pe
+00001450: 726d 6974 6520 696e 666f 726d 6520 706f  rmite informe po
+00001460: 7220 7061 7274 6520 6465 2075 6e20 6167  r parte de un ag
+00001470: 656e 7465 2064 6520 756e 6120 6f20 7661  ente de una o va
+00001480: 7269 6173 2074 7261 6e73 6163 6369 6f6e  rias transaccion
+00001490: 6573 220a 2020 2020 2020 2020 2320 6372  es".        # cr
+000014a0: 656f 206c 6f73 2070 6172 e16d 6574 726f  eo los par.metro
+000014b0: 7320 7061 7261 2065 7374 6120 6c6c 616d  s para esta llam
+000014c0: 6164 610a 2020 2020 2020 2020 7061 7261  ada.        para
+000014d0: 6d73 203d 207b 2020 2767 6c6e 5f6f 7269  ms = {  'gln_ori
+000014e0: 6765 6e27 3a20 676c 6e5f 6f72 6967 656e  gen': gln_origen
+000014f0: 2c20 2767 6c6e 5f64 6573 7469 6e6f 273a  , 'gln_destino':
+00001500: 2067 6c6e 5f64 6573 7469 6e6f 2c0a 2020   gln_destino,.  
+00001510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001520: 2020 2766 5f6f 7065 7261 6369 6f6e 273a    'f_operacion':
+00001530: 2066 5f6f 7065 7261 6369 6f6e 2c20 2769   f_operacion, 'i
+00001540: 645f 6576 656e 746f 273a 2069 645f 6576  d_evento': id_ev
+00001550: 656e 746f 2c0a 2020 2020 2020 2020 2020  ento,.          
+00001560: 2020 2020 2020 2020 2020 2763 6f64 5f70            'cod_p
+00001570: 726f 6475 6374 6f27 3a20 636f 645f 7072  roducto': cod_pr
+00001580: 6f64 7563 746f 2c20 276e 5f63 616e 7469  oducto, 'n_canti
+00001590: 6461 6427 3a20 6e5f 6361 6e74 6964 6164  dad': n_cantidad
+000015a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000015b0: 2020 2020 2020 276e 5f64 6f63 756d 656e        'n_documen
+000015c0: 746f 5f6f 7065 7261 6369 6f6e 273a 206e  to_operacion': n
+000015d0: 5f64 6f63 756d 656e 746f 5f6f 7065 7261  _documento_opera
+000015e0: 6369 6f6e 2c0a 2020 2020 2020 2020 2020  cion,.          
+000015f0: 2020 2020 2020 2020 2020 276e 5f72 656d            'n_rem
+00001600: 6974 6f27 3a20 6e5f 7265 6d69 746f 2c0a  ito': n_remito,.
+00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001620: 2020 2020 2769 645f 7469 706f 5f74 7261      'id_tipo_tra
+00001630: 6e73 706f 7274 6527 3a20 6964 5f74 6970  nsporte': id_tip
+00001640: 6f5f 7472 616e 7370 6f72 7465 2c0a 2020  o_transporte,.  
+00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001660: 2020 2769 645f 7061 736f 5f66 726f 6e74    'id_paso_front
+00001670: 6572 615f 696e 6772 6573 6f27 3a20 6964  era_ingreso': id
+00001680: 5f70 6173 6f5f 6672 6f6e 7465 7261 5f69  _paso_frontera_i
+00001690: 6e67 7265 736f 2c0a 2020 2020 2020 2020  ngreso,.        
+000016a0: 2020 2020 2020 2020 2020 2020 2769 645f              'id_
+000016b0: 7061 736f 5f66 726f 6e74 6572 615f 6567  paso_frontera_eg
+000016c0: 7265 736f 273a 2069 645f 7061 736f 5f66  reso': id_paso_f
+000016d0: 726f 6e74 6572 615f 6567 7265 736f 2c0a  rontera_egreso,.
+000016e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016f0: 2020 2020 2769 645f 7469 706f 5f64 6f63      'id_tipo_doc
+00001700: 756d 656e 746f 5f6f 7065 7261 6369 6f6e  umento_operacion
+00001710: 273a 2069 645f 7469 706f 5f64 6f63 756d  ': id_tipo_docum
+00001720: 656e 746f 5f6f 7065 7261 6369 6f6e 2c0a  ento_operacion,.
+00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001740: 2020 2020 2764 5f64 6f6d 696e 696f 5f74      'd_dominio_t
+00001750: 7261 6374 6f72 273a 2064 5f64 6f6d 696e  ractor': d_domin
+00001760: 696f 5f74 7261 6374 6f72 2c0a 2020 2020  io_tractor,.    
+00001770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001780: 2764 5f64 6f6d 696e 696f 5f73 656d 6927  'd_dominio_semi'
+00001790: 3a20 645f 646f 6d69 6e69 6f5f 7365 6d69  : d_dominio_semi
+000017a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000017b0: 2020 2020 2020 276e 5f73 6572 6965 273a        'n_serie':
+000017c0: 206e 5f73 6572 6965 2c20 276e 5f6c 6f74   n_serie, 'n_lot
+000017d0: 6527 3a20 6e5f 6c6f 7465 2c0a 2020 2020  e': n_lote,.    
+000017e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017f0: 2764 6f63 5f64 6573 7061 6368 6f5f 706c  'doc_despacho_pl
+00001800: 617a 6127 3a20 646f 635f 6465 7370 6163  aza': doc_despac
+00001810: 686f 5f70 6c61 7a61 2c0a 2020 2020 2020  ho_plaza,.      
+00001820: 2020 2020 2020 2020 2020 2020 2020 2764                'd
+00001830: 6a61 6927 3a20 646a 6169 2c20 276e 5f63  jai': djai, 'n_c
+00001840: 6572 745f 696d 706f 5f65 7870 6f27 3a20  ert_impo_expo': 
+00001850: 6e5f 6365 7274 5f69 6d70 6f5f 6578 706f  n_cert_impo_expo
+00001860: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001870: 2020 2020 2020 2769 645f 7469 706f 5f64        'id_tipo_d
+00001880: 6f63 756d 656e 746f 273a 2069 645f 7469  ocumento': id_ti
+00001890: 706f 5f64 6f63 756d 656e 746f 2c0a 2020  po_documento,.  
+000018a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018b0: 2020 276e 5f64 6f63 756d 656e 746f 273a    'n_documento':
+000018c0: 206e 5f64 6f63 756d 656e 746f 2c0a 2020   n_documento,.  
+000018d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018e0: 2020 276d 5f63 616c 6964 6164 5f61 6e61    'm_calidad_ana
+000018f0: 6c69 7469 6361 273a 206d 5f63 616c 6964  litica': m_calid
+00001900: 6164 5f61 6e61 6c69 7469 6361 2c0a 2020  ad_analitica,.  
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2020 276d 5f65 6e74 7265 6761 5f70 6172    'm_entrega_par
+00001930: 6369 616c 273a 206d 5f65 6e74 7265 6761  cial': m_entrega
+00001940: 5f70 6172 6369 616c 2c0a 2020 2020 2020  _parcial,.      
+00001950: 2020 2020 2020 2020 2020 2020 2020 2764                'd
+00001960: 6f63 5f70 6572 6d69 736f 5f65 6d62 6172  oc_permiso_embar
+00001970: 7175 6527 3a20 646f 635f 7065 726d 6973  que': doc_permis
+00001980: 6f5f 656d 6261 7271 7565 2c0a 2020 2020  o_embarque,.    
+00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019a0: 2767 6c6e 5f74 7261 6e73 706f 7274 6973  'gln_transportis
+000019b0: 7461 273a 2067 6c6e 5f74 7261 6e73 706f  ta': gln_transpo
+000019c0: 7274 6973 7461 2c0a 2020 2020 2020 2020  rtista,.        
+000019d0: 2020 2020 2020 2020 2020 2020 276f 7065              'ope
+000019e0: 7261 6369 6f6e 5f65 7863 656e 746f 5f64  racion_excento_d
+000019f0: 6a61 6927 3a20 6f70 6572 6163 696f 6e5f  jai': operacion_
+00001a00: 6578 6365 6e74 6f5f 646a 6169 2c0a 2020  excento_djai,.  
+00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a20: 2020 2763 6f6e 7472 6f6c 5f64 7570 6c69    'control_dupli
+00001a30: 6369 6461 6427 3a20 636f 6e74 726f 6c5f  cidad': control_
+00001a40: 6475 706c 6963 6964 6164 2c0a 2020 2020  duplicidad,.    
+00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a60: 7d0a 2020 2020 2020 2020 2320 6163 7475  }.        # actu
+00001a70: 616c 697a 6f20 636f 6e20 7061 72e1 6d65  alizo con par.me
+00001a80: 7472 6f73 2067 656e 6572 616c 6573 3a0a  tros generales:.
+00001a90: 2020 2020 2020 2020 7061 7261 6d73 2e75          params.u
+00001aa0: 7064 6174 6528 7365 6c66 2e70 6172 616d  pdate(self.param
+00001ab0: 735f 696e 290a 2020 2020 2020 2020 7265  s_in).        re
+00001ac0: 7320 3d20 7365 6c66 2e63 6c69 656e 742e  s = self.client.
+00001ad0: 7361 7665 5472 616e 7361 6363 696f 6e65  saveTransaccione
+00001ae0: 7328 0a20 2020 2020 2020 2020 2020 2061  s(.            a
+00001af0: 7267 303d 7061 7261 6d73 2c0a 2020 2020  rg0=params,.    
+00001b00: 2020 2020 2020 2020 6172 6731 3d75 7375          arg1=usu
+00001b10: 6172 696f 2c0a 2020 2020 2020 2020 2020  ario,.          
+00001b20: 2020 6172 6732 3d70 6173 7377 6f72 642c    arg2=password,
+00001b30: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00001b40: 2020 2072 6574 203d 2072 6573 5b27 7265     ret = res['re
+00001b50: 7475 726e 275d 0a20 2020 2020 2020 2073  turn'].        s
+00001b60: 656c 662e 436f 6469 676f 5472 616e 7361  elf.CodigoTransa
+00001b70: 6363 696f 6e20 3d20 7265 742e 6765 7428  ccion = ret.get(
+00001b80: 2763 6f64 6967 6f54 7261 6e73 6163 6369  'codigoTransacci
+00001b90: 6f6e 2729 0a20 2020 2020 2020 2073 656c  on').        sel
+00001ba0: 662e 5f5f 616e 616c 697a 6172 5f65 7272  f.__analizar_err
+00001bb0: 6f72 6573 2872 6574 290a 2020 2020 2020  ores(ret).      
+00001bc0: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
+00001bd0: 2020 2040 696e 6963 6961 6c69 7a61 725f     @inicializar_
+00001be0: 795f 6361 7074 7572 6172 5f65 7863 6570  y_capturar_excep
+00001bf0: 6369 6f6e 6573 0a20 2020 2064 6566 2053  ciones.    def S
+00001c00: 656e 6443 616e 6365 6c61 6354 7261 6e73  endCancelacTrans
+00001c10: 6163 6328 7365 6c66 2c20 7573 7561 7269  acc(self, usuari
+00001c20: 6f2c 2070 6173 7377 6f72 642c 2063 6f64  o, password, cod
+00001c30: 6967 6f5f 7472 616e 7361 6363 696f 6e29  igo_transaccion)
+00001c40: 3a0a 2020 2020 2020 2020 2220 5265 616c  :.        " Real
+00001c50: 697a 6120 6c61 2063 616e 6365 6c61 6369  iza la cancelaci
+00001c60: f36e 2064 6520 756e 6120 7472 616e 7361  .n de una transa
+00001c70: 6363 69f3 6e22 0a20 2020 2020 2020 2072  cci.n".        r
+00001c80: 6573 203d 2073 656c 662e 636c 6965 6e74  es = self.client
+00001c90: 2e73 656e 6443 616e 6365 6c61 5472 616e  .sendCancelaTran
+00001ca0: 7361 6328 0a20 2020 2020 2020 2020 2020  sac(.           
+00001cb0: 2061 7267 303d 636f 6469 676f 5f74 7261   arg0=codigo_tra
+00001cc0: 6e73 6163 6369 6f6e 2c0a 2020 2020 2020  nsaccion,.      
+00001cd0: 2020 2020 2020 6172 6731 3d75 7375 6172        arg1=usuar
+00001ce0: 696f 2c0a 2020 2020 2020 2020 2020 2020  io,.            
+00001cf0: 6172 6732 3d70 6173 7377 6f72 642c 0a20  arg2=password,. 
+00001d00: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00001d10: 2020 7265 7420 3d20 7265 735b 2772 6574    ret = res['ret
+00001d20: 7572 6e27 5d0a 0a20 2020 2020 2020 2073  urn']..        s
+00001d30: 656c 662e 436f 6469 676f 5472 616e 7361  elf.CodigoTransa
+00001d40: 6363 696f 6e20 3d20 7265 745b 2763 6f64  ccion = ret['cod
+00001d50: 6967 6f54 7261 6e73 6163 6369 6f6e 275d  igoTransaccion']
+00001d60: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
+00001d70: 616e 616c 697a 6172 5f65 7272 6f72 6573  analizar_errores
+00001d80: 2872 6574 290a 0a20 2020 2020 2020 2072  (ret)..        r
+00001d90: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
+00001da0: 4069 6e69 6369 616c 697a 6172 5f79 5f63  @inicializar_y_c
+00001db0: 6170 7475 7261 725f 6578 6365 7063 696f  apturar_excepcio
+00001dc0: 6e65 730a 2020 2020 6465 6620 5365 6e64  nes.    def Send
+00001dd0: 436f 6e66 6972 6d61 5472 616e 7361 6363  ConfirmaTransacc
+00001de0: 2873 656c 662c 2075 7375 6172 696f 2c20  (self, usuario, 
+00001df0: 7061 7373 776f 7264 2c20 705f 6964 735f  password, p_ids_
+00001e00: 7472 616e 7361 632c 2066 5f6f 7065 7261  transac, f_opera
+00001e10: 6369 6f6e 293a 0a20 2020 2020 2020 2022  cion):.        "
+00001e20: 436f 6e66 6972 6d61 206c 6120 7265 6365  Confirma la rece
+00001e30: 7063 69f3 6e20 6465 2075 6e20 6d65 6469  pci.n de un medi
+00001e40: 6361 6d65 6e74 6f22 0a20 2020 2020 2020  camento".       
+00001e50: 2072 6573 203d 2073 656c 662e 636c 6965   res = self.clie
+00001e60: 6e74 2e73 656e 6443 6f6e 6669 726d 6154  nt.sendConfirmaT
+00001e70: 7261 6e73 6163 6328 0a20 2020 2020 2020  ransacc(.       
+00001e80: 2020 2020 2061 7267 303d 7573 7561 7269       arg0=usuari
+00001e90: 6f2c 0a20 2020 2020 2020 2020 2020 2061  o,.            a
+00001ea0: 7267 313d 7061 7373 776f 7264 2c0a 2020  rg1=password,.  
+00001eb0: 2020 2020 2020 2020 2020 6172 6732 3d7b            arg2={
+00001ec0: 2770 5f69 6473 5f74 7261 6e73 6163 273a  'p_ids_transac':
+00001ed0: 2070 5f69 6473 5f74 7261 6e73 6163 2c20   p_ids_transac, 
+00001ee0: 2766 5f6f 7065 7261 6369 6f6e 273a 2066  'f_operacion': f
+00001ef0: 5f6f 7065 7261 6369 6f6e 7d2c 0a20 2020  _operacion},.   
+00001f00: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
+00001f10: 6574 203d 2072 6573 5b27 7265 7475 726e  et = res['return
+00001f20: 275d 0a20 2020 2020 2020 2073 656c 662e  '].        self.
+00001f30: 436f 6469 676f 5472 616e 7361 6363 696f  CodigoTransaccio
+00001f40: 6e20 3d20 7265 742e 6765 7428 2769 645f  n = ret.get('id_
+00001f50: 7472 616e 7361 635f 6173 6f63 6961 6461  transac_asociada
+00001f60: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+00001f70: 5f5f 616e 616c 697a 6172 5f65 7272 6f72  __analizar_error
+00001f80: 6573 2872 6574 290a 2020 2020 2020 2020  es(ret).        
+00001f90: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+00001fa0: 2040 696e 6963 6961 6c69 7a61 725f 795f   @inicializar_y_
+00001fb0: 6361 7074 7572 6172 5f65 7863 6570 6369  capturar_excepci
+00001fc0: 6f6e 6573 0a20 2020 2064 6566 2053 656e  ones.    def Sen
+00001fd0: 6441 6c65 7274 6154 7261 6e73 6163 6328  dAlertaTransacc(
+00001fe0: 7365 6c66 2c20 7573 7561 7269 6f2c 2070  self, usuario, p
+00001ff0: 6173 7377 6f72 642c 2070 5f69 6473 5f74  assword, p_ids_t
+00002000: 7261 6e73 6163 5f77 7329 3a0a 2020 2020  ransac_ws):.    
+00002010: 2020 2020 2241 6c65 7274 6120 756e 206d      "Alerta un m
+00002020: 6564 6963 616d 656e 746f 2c20 6163 6369  edicamento, acci
+00002030: f36e 2063 6f6e 7472 6172 6961 2061 2093  .n contraria a .
+00002040: 636f 6e66 6972 6d61 7220 6c61 2074 7261  confirmar la tra
+00002050: 6e73 6163 6369 f36e 942e 220a 2020 2020  nsacci.n..".    
+00002060: 2020 2020 7265 7320 3d20 7365 6c66 2e63      res = self.c
+00002070: 6c69 656e 742e 7365 6e64 416c 6572 7461  lient.sendAlerta
+00002080: 5472 616e 7361 6363 280a 2020 2020 2020  Transacc(.      
+00002090: 2020 2020 2020 6172 6730 3d75 7375 6172        arg0=usuar
+000020a0: 696f 2c0a 2020 2020 2020 2020 2020 2020  io,.            
+000020b0: 6172 6731 3d70 6173 7377 6f72 642c 0a20  arg1=password,. 
+000020c0: 2020 2020 2020 2020 2020 2061 7267 323d             arg2=
+000020d0: 705f 6964 735f 7472 616e 7361 635f 7773  p_ids_transac_ws
+000020e0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+000020f0: 2020 2020 7265 7420 3d20 7265 735b 2772      ret = res['r
+00002100: 6574 7572 6e27 5d0a 2020 2020 2020 2020  eturn'].        
+00002110: 7365 6c66 2e43 6f64 6967 6f54 7261 6e73  self.CodigoTrans
+00002120: 6163 6369 6f6e 203d 2072 6574 2e67 6574  accion = ret.get
+00002130: 2827 6964 5f74 7261 6e73 6163 5f61 736f  ('id_transac_aso
+00002140: 6369 6164 6127 290a 2020 2020 2020 2020  ciada').        
+00002150: 7365 6c66 2e5f 5f61 6e61 6c69 7a61 725f  self.__analizar_
+00002160: 6572 726f 7265 7328 7265 7429 0a20 2020  errores(ret).   
+00002170: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00002180: 0a0a 2020 2020 4069 6e69 6369 616c 697a  ..    @inicializ
+00002190: 6172 5f79 5f63 6170 7475 7261 725f 6578  ar_y_capturar_ex
+000021a0: 6365 7063 696f 6e65 730a 2020 2020 6465  cepciones.    de
+000021b0: 6620 4765 7454 7261 6e73 6163 6369 6f6e  f GetTransaccion
+000021c0: 6573 5753 2873 656c 662c 2075 7375 6172  esWS(self, usuar
+000021d0: 696f 2c20 7061 7373 776f 7264 2c0a 2020  io, password,.  
+000021e0: 2020 2020 2020 2020 2020 2020 2020 705f                p_
+000021f0: 6964 5f74 7261 6e73 6163 6369 6f6e 5f67  id_transaccion_g
+00002200: 6c6f 6261 6c3d 4e6f 6e65 2c0a 2020 2020  lobal=None,.    
+00002210: 2020 2020 2020 2020 2020 2020 6964 5f61              id_a
+00002220: 6765 6e74 655f 6f72 6967 656e 3d4e 6f6e  gente_origen=Non
+00002230: 652c 2069 645f 6167 656e 7465 5f64 6573  e, id_agente_des
+00002240: 7469 6e6f 3d4e 6f6e 652c 0a20 2020 2020  tino=None,.     
+00002250: 2020 2020 2020 2020 2020 2069 645f 6167             id_ag
+00002260: 656e 7465 5f69 6e66 6f72 6d61 646f 723d  ente_informador=
+00002270: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00002280: 2020 2020 2020 6774 696e 3d4e 6f6e 652c        gtin=None,
+00002290: 2069 645f 6576 656e 746f 3d4e 6f6e 652c   id_evento=None,
+000022a0: 2063 616e 745f 616e 616c 6974 6963 613d   cant_analitica=
+000022b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+000022c0: 2020 2020 2020 6665 6368 615f 6465 7364        fecha_desd
+000022d0: 655f 6f70 3d4e 6f6e 652c 2066 6563 6861  e_op=None, fecha
+000022e0: 5f68 6173 7461 5f6f 703d 4e6f 6e65 2c0a  _hasta_op=None,.
+000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002300: 6665 6368 615f 6465 7364 655f 743d 4e6f  fecha_desde_t=No
+00002310: 6e65 2c20 6665 6368 615f 6861 7374 615f  ne, fecha_hasta_
+00002320: 743d 4e6f 6e65 2c0a 2020 2020 2020 2020  t=None,.        
+00002330: 2020 2020 2020 2020 6964 5f74 6970 6f3d          id_tipo=
+00002340: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00002350: 2020 2020 2020 6964 5f65 7374 6164 6f3d        id_estado=
+00002360: 4e6f 6e65 2c20 6e72 6f5f 7061 673d 312c  None, nro_pag=1,
+00002370: 2063 616e 745f 7265 673d 3130 302c 0a20   cant_reg=100,. 
+00002380: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00002390: 3a0a 2020 2020 2020 2020 224f 6274 6965  :.        "Obtie
+000023a0: 6e65 206c 6f73 206d 6f76 696d 6965 6e74  ne los movimient
+000023b0: 6f73 2072 6561 6c69 7a61 646f 7320 7920  os realizados y 
+000023c0: 7065 726d 6974 6520 6669 6c74 726f 7320  permite filtros 
+000023d0: 6465 2062 fa73 7175 6564 6122 0a0a 2020  de b.squeda"..  
+000023e0: 2020 2020 2020 2320 7072 6570 6172 6f20        # preparo 
+000023f0: 6c6f 7320 7061 7261 6d65 7472 6f73 2064  los parametros d
+00002400: 6520 656e 7472 6164 6120 6f70 6369 6f6e  e entrada opcion
+00002410: 616c 6573 3a0a 2020 2020 2020 2020 6b77  ales:.        kw
+00002420: 6172 6773 203d 207b 7d0a 2020 2020 2020  args = {}.      
+00002430: 2020 6966 2070 5f69 645f 7472 616e 7361    if p_id_transa
+00002440: 6363 696f 6e5f 676c 6f62 616c 2069 7320  ccion_global is 
+00002450: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00002460: 2020 2020 2020 6b77 6172 6773 5b27 6172        kwargs['ar
+00002470: 6732 275d 203d 2070 5f69 645f 7472 616e  g2'] = p_id_tran
+00002480: 7361 6363 696f 6e5f 676c 6f62 616c 0a20  saccion_global. 
+00002490: 2020 2020 2020 2069 6620 6964 5f61 6765         if id_age
+000024a0: 6e74 655f 6f72 6967 656e 2069 7320 6e6f  nte_origen is no
+000024b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000024c0: 2020 2020 6b77 6172 6773 5b27 6172 6733      kwargs['arg3
+000024d0: 275d 203d 2069 645f 6167 656e 7465 5f6f  '] = id_agente_o
+000024e0: 7269 6765 6e0a 2020 2020 2020 2020 6966  rigen.        if
+000024f0: 2069 645f 6167 656e 7465 5f64 6573 7469   id_agente_desti
+00002500: 6e6f 2069 7320 6e6f 7420 4e6f 6e65 3a0a  no is not None:.
+00002510: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
+00002520: 6773 5b27 6172 6734 275d 203d 2069 645f  gs['arg4'] = id_
+00002530: 6167 656e 7465 5f64 6573 7469 6e6f 0a20  agente_destino. 
+00002540: 2020 2020 2020 2069 6620 6964 5f61 6765         if id_age
+00002550: 6e74 655f 6465 7374 696e 6f20 6973 206e  nte_destino is n
+00002560: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00002570: 2020 2020 206b 7761 7267 735b 2761 7267       kwargs['arg
+00002580: 3527 5d20 3d20 6964 5f61 6765 6e74 655f  5'] = id_agente_
+00002590: 696e 666f 726d 6164 6f72 0a20 2020 2020  informador.     
+000025a0: 2020 2069 6620 6774 696e 2069 7320 6e6f     if gtin is no
+000025b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000025c0: 2020 2020 6b77 6172 6773 5b27 6172 6736      kwargs['arg6
+000025d0: 275d 203d 2067 7469 6e0a 2020 2020 2020  '] = gtin.      
+000025e0: 2020 6966 2069 645f 6576 656e 746f 2069    if id_evento i
+000025f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00002600: 2020 2020 2020 2020 6b77 6172 6773 5b27          kwargs['
+00002610: 6172 6737 275d 203d 2069 645f 6576 656e  arg7'] = id_even
+00002620: 746f 0a20 2020 2020 2020 2069 6620 6361  to.        if ca
+00002630: 6e74 5f61 6e61 6c69 7469 6361 2069 7320  nt_analitica is 
+00002640: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00002650: 2020 2020 2020 6b77 6172 6773 5b27 6172        kwargs['ar
+00002660: 6738 275d 203d 2063 616e 745f 616e 616c  g8'] = cant_anal
+00002670: 6974 6963 610a 2020 2020 2020 2020 6966  itica.        if
+00002680: 2066 6563 6861 5f64 6573 6465 5f6f 7020   fecha_desde_op 
+00002690: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000026a0: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
+000026b0: 2761 7267 3927 5d20 3d20 6665 6368 615f  'arg9'] = fecha_
+000026c0: 6465 7364 655f 6f70 0a20 2020 2020 2020  desde_op.       
+000026d0: 2069 6620 6665 6368 615f 6861 7374 615f   if fecha_hasta_
+000026e0: 6f70 2069 7320 6e6f 7420 4e6f 6e65 3a0a  op is not None:.
+000026f0: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
+00002700: 6773 5b27 6172 6731 3027 5d20 3d20 6665  gs['arg10'] = fe
+00002710: 6368 615f 6861 7374 615f 6f70 0a20 2020  cha_hasta_op.   
+00002720: 2020 2020 2069 6620 6665 6368 615f 6465       if fecha_de
+00002730: 7364 655f 7420 6973 206e 6f74 204e 6f6e  sde_t is not Non
+00002740: 653a 0a20 2020 2020 2020 2020 2020 206b  e:.            k
+00002750: 7761 7267 735b 2761 7267 3131 275d 203d  wargs['arg11'] =
+00002760: 2066 6563 6861 5f64 6573 6465 5f74 0a20   fecha_desde_t. 
+00002770: 2020 2020 2020 2069 6620 6665 6368 615f         if fecha_
+00002780: 6861 7374 615f 7420 6973 206e 6f74 204e  hasta_t is not N
+00002790: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000027a0: 206b 7761 7267 735b 2761 7267 3132 275d   kwargs['arg12']
+000027b0: 203d 2066 6563 6861 5f68 6173 7461 5f74   = fecha_hasta_t
+000027c0: 0a20 2020 2020 2020 2069 6620 6964 5f74  .        if id_t
+000027d0: 6970 6f20 6973 206e 6f74 204e 6f6e 653a  ipo is not None:
+000027e0: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
+000027f0: 7267 735b 2761 7267 3133 275d 203d 2069  rgs['arg13'] = i
+00002800: 645f 7469 706f 0a20 2020 2020 2020 2069  d_tipo.        i
+00002810: 6620 6964 5f65 7374 6164 6f20 6973 206e  f id_estado is n
+00002820: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00002830: 2020 2020 206b 7761 7267 735b 2761 7267       kwargs['arg
+00002840: 3134 275d 203d 2069 645f 6573 7461 646f  14'] = id_estado
+00002850: 0a20 2020 2020 2020 2069 6620 6e72 6f5f  .        if nro_
+00002860: 7061 6720 6973 206e 6f74 204e 6f6e 653a  pag is not None:
+00002870: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
+00002880: 7267 735b 2761 7267 3135 275d 203d 206e  rgs['arg15'] = n
+00002890: 726f 5f70 6167 0a20 2020 2020 2020 2069  ro_pag.        i
+000028a0: 6620 6361 6e74 5f72 6567 2069 7320 6e6f  f cant_reg is no
+000028b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000028c0: 2020 2020 6b77 6172 6773 5b27 6172 6731      kwargs['arg1
+000028d0: 3627 5d20 3d20 6361 6e74 5f72 6567 0a0a  6'] = cant_reg..
+000028e0: 2020 2020 2020 2020 2320 6c6c 616d 6f20          # llamo 
+000028f0: 616c 2077 6562 7365 7276 6963 650a 2020  al webservice.  
+00002900: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
+00002910: 2e63 6c69 656e 742e 6765 7454 7261 6e73  .client.getTrans
+00002920: 6163 6369 6f6e 6573 5773 280a 2020 2020  accionesWs(.    
+00002930: 2020 2020 2020 2020 6172 6730 3d75 7375          arg0=usu
+00002940: 6172 696f 2c0a 2020 2020 2020 2020 2020  ario,.          
+00002950: 2020 6172 6731 3d70 6173 7377 6f72 642c    arg1=password,
+00002960: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
+00002970: 7761 7267 730a 2020 2020 2020 2020 290a  wargs.        ).
+00002980: 2020 2020 2020 2020 7265 7420 3d20 7265          ret = re
+00002990: 735b 2772 6574 7572 6e27 5d0a 2020 2020  s['return'].    
+000029a0: 2020 2020 6966 2072 6574 3a0a 2020 2020      if ret:.    
+000029b0: 2020 2020 2020 2020 7365 6c66 2e5f 5f61          self.__a
+000029c0: 6e61 6c69 7a61 725f 6572 726f 7265 7328  nalizar_errores(
+000029d0: 7265 7429 0a20 2020 2020 2020 2020 2020  ret).           
+000029e0: 2073 656c 662e 4361 6e74 5061 6769 6e61   self.CantPagina
+000029f0: 7320 3d20 7265 742e 6765 7428 2763 616e  s = ret.get('can
+00002a00: 7450 6167 696e 6173 2729 0a20 2020 2020  tPaginas').     
+00002a10: 2020 2020 2020 2073 656c 662e 4861 7945         self.HayE
+00002a20: 7272 6f72 203d 2072 6574 2e67 6574 2827  rror = ret.get('
+00002a30: 6861 795f 6572 726f 7227 290a 2020 2020  hay_error').    
+00002a40: 2020 2020 2020 2020 7365 6c66 2e54 7261          self.Tra
+00002a50: 6e73 6163 6369 6f6e 506c 6169 6e57 5320  nsaccionPlainWS 
+00002a60: 3d20 5b69 7420 666f 7220 6974 2069 6e20  = [it for it in 
+00002a70: 7265 742e 6765 7428 276c 6973 7427 2c20  ret.get('list', 
+00002a80: 5b5d 295d 0a20 2020 2020 2020 2072 6574  [])].        ret
+00002a90: 7572 6e20 5472 7565 0a0a 2020 2020 6465  urn True..    de
+00002aa0: 6620 5365 7455 7365 726e 616d 6528 7365  f SetUsername(se
+00002ab0: 6c66 2c20 7573 6572 6e61 6d65 293a 0a20  lf, username):. 
+00002ac0: 2020 2020 2020 2022 4573 7461 626c 657a         "Establez
+00002ad0: 636f 2065 6c20 6e6f 6d62 7265 2064 6520  co el nombre de 
+00002ae0: 7573 7561 7269 6f22 0a20 2020 2020 2020  usuario".       
+00002af0: 2073 656c 662e 5573 6572 6e61 6d65 203d   self.Username =
+00002b00: 2075 7365 726e 616d 650a 0a20 2020 2064   username..    d
+00002b10: 6566 2053 6574 5061 7373 776f 7264 2873  ef SetPassword(s
+00002b20: 656c 662c 2070 6173 7377 6f72 6429 3a0a  elf, password):.
+00002b30: 2020 2020 2020 2020 2245 7374 6162 6c65          "Estable
+00002b40: 7a63 6f20 6c61 2063 6f6e 7472 6173 65f1  zco la contrase.
+00002b50: 6122 0a20 2020 2020 2020 2073 656c 662e  a".        self.
+00002b60: 5061 7373 776f 7264 203d 2070 6173 7377  Password = passw
+00002b70: 6f72 640a 0a20 2020 2064 6566 2047 6574  ord..    def Get
+00002b80: 436f 6469 676f 5472 616e 7361 6363 696f  CodigoTransaccio
+00002b90: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
+00002ba0: 2022 4465 7675 656c 766f 2065 6c20 63f3   "Devuelvo el c.
+00002bb0: 6469 676f 2064 6520 7472 616e 7361 6363  digo de transacc
+00002bc0: 69f3 6e22 0a20 2020 2020 2020 2072 6574  i.n".        ret
+00002bd0: 7572 6e20 7365 6c66 2e43 6f64 6967 6f54  urn self.CodigoT
+00002be0: 7261 6e73 6163 6369 6f6e 0a0a 2020 2020  ransaccion..    
+00002bf0: 6465 6620 4765 7452 6573 756c 7461 646f  def GetResultado
+00002c00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00002c10: 2244 6576 7565 6c76 6f20 656c 2072 6573  "Devuelvo el res
+00002c20: 756c 7461 646f 220a 2020 2020 2020 2020  ultado".        
+00002c30: 7265 7475 726e 2073 656c 662e 5265 7375  return self.Resu
+00002c40: 6c74 6164 6f0a 0a0a 0a64 6566 206d 6169  ltado....def mai
+00002c50: 6e28 293a 0a20 2020 2022 4675 6e63 69f3  n():.    "Funci.
+00002c60: 6e20 7072 696e 6369 7061 6c20 6465 2070  n principal de p
+00002c70: 7275 6562 6173 2028 7472 616e 7361 6363  ruebas (transacc
+00002c80: 696f 6e61 7221 2922 0a20 2020 2069 6d70  ionar!)".    imp
+00002c90: 6f72 7420 6f73 2c20 7469 6d65 2c20 7379  ort os, time, sy
+00002ca0: 730a 2020 2020 676c 6f62 616c 2057 5344  s.    global WSD
+00002cb0: 4c2c 204c 4f43 4154 494f 4e0a 0a20 2020  L, LOCATION..   
+00002cc0: 2044 4542 5547 203d 2027 2d2d 6465 6275   DEBUG = '--debu
+00002cd0: 6727 2069 6e20 7379 732e 6172 6776 0a0a  g' in sys.argv..
+00002ce0: 2020 2020 7773 203d 2054 7261 7a61 5265      ws = TrazaRe
+00002cf0: 6e70 7265 2829 0a0a 2020 2020 7773 2e55  npre()..    ws.U
+00002d00: 7365 726e 616d 6520 3d20 2774 6573 7477  sername = 'testw
+00002d10: 7365 7276 6963 6527 0a20 2020 2077 732e  service'.    ws.
+00002d20: 5061 7373 776f 7264 203d 2027 7465 7374  Password = 'test
+00002d30: 7773 6572 7669 6365 7073 7727 0a0a 2020  wservicepsw'..  
+00002d40: 2020 6966 2027 2d2d 7072 6f64 2720 696e    if '--prod' in
+00002d50: 2073 7973 2e61 7267 7620 616e 6420 6e6f   sys.argv and no
+00002d60: 7420 484f 4d4f 3a0a 2020 2020 2020 2020  t HOMO:.        
+00002d70: 5753 444c 203d 2022 6874 7470 733a 2f2f  WSDL = "https://
+00002d80: 7472 617a 6162 696c 6964 6164 2e70 616d  trazabilidad.pam
+00002d90: 692e 6f72 672e 6172 3a35 3930 3530 2f74  i.org.ar:59050/t
+00002da0: 7261 7a61 6d65 642e 5765 6253 6572 7669  razamed.WebServi
+00002db0: 6365 5344 524e 3f77 7364 6c22 0a20 2020  ceSDRN?wsdl".   
+00002dc0: 2020 2020 2070 7269 6e74 2822 5573 616e       print("Usan
+00002dd0: 646f 2057 5344 4c3a 222c 2057 5344 4c29  do WSDL:", WSDL)
+00002de0: 0a20 2020 2020 2020 2073 7973 2e61 7267  .        sys.arg
+00002df0: 762e 706f 7028 3029 0a0a 2020 2020 7773  v.pop(0)..    ws
+00002e00: 2e43 6f6e 6563 7461 7228 2222 2c20 5753  .Conectar("", WS
+00002e10: 444c 290a 0a20 2020 2069 6620 7773 2e45  DL)..    if ws.E
+00002e20: 7863 6570 6369 6f6e 3a0a 2020 2020 2020  xcepcion:.      
+00002e30: 2020 7072 696e 7428 7773 2e45 7863 6570    print(ws.Excep
+00002e40: 6369 6f6e 290a 2020 2020 2020 2020 7072  cion).        pr
+00002e50: 696e 7428 7773 2e54 7261 6365 6261 636b  int(ws.Traceback
+00002e60: 290a 2020 2020 2020 2020 7379 732e 6578  ).        sys.ex
+00002e70: 6974 282d 3129 0a0a 2020 2020 2320 7072  it(-1)..    # pr
+00002e80: 696e 7428 7773 2e63 6c69 656e 742e 7365  int(ws.client.se
+00002e90: 7276 6963 6573 290a 2020 2020 2320 6f70  rvices).    # op
+00002ea0: 203d 2077 732e 636c 6965 6e74 2e67 6574   = ws.client.get
+00002eb0: 5f6f 7065 7261 7469 6f6e 2822 7365 6e64  _operation("send
+00002ec0: 4d65 6469 6361 6d65 6e74 6f73 2229 0a20  Medicamentos"). 
+00002ed0: 2020 2023 2069 6d70 6f72 7420 7064 623b     # import pdb;
+00002ee0: 7064 622e 7365 745f 7472 6163 6528 290a  pdb.set_trace().
+00002ef0: 2020 2020 6966 2027 2d2d 7465 7374 2720      if '--test' 
+00002f00: 696e 2073 7973 2e61 7267 763a 0a20 2020  in sys.argv:.   
+00002f10: 2020 2020 2077 732e 5361 7665 5472 616e       ws.SaveTran
+00002f20: 7361 6363 696f 6e65 7328 0a20 2020 2020  sacciones(.     
+00002f30: 2020 2020 2020 2075 7375 6172 696f 3d27         usuario='
+00002f40: 7072 7565 6261 7377 7327 2c20 7061 7373  pruebasws', pass
+00002f50: 776f 7264 3d27 7072 7565 6261 7377 7327  word='pruebasws'
+00002f60: 2c0a 2020 2020 2020 2020 2020 2020 676c  ,.            gl
+00002f70: 6e5f 6f72 6967 656e 3d38 3838 3838 3838  n_origen=8888888
+00002f80: 3838 3838 3838 2c0a 2020 2020 2020 2020  888888,.        
+00002f90: 2020 2020 676c 6e5f 6465 7374 696e 6f3d      gln_destino=
+00002fa0: 3838 3838 3838 3838 3838 3838 382c 0a20  8888888888888,. 
+00002fb0: 2020 2020 2020 2020 2020 2066 5f6f 7065             f_ope
+00002fc0: 7261 6369 6f6e 3d22 3230 2f30 352f 3230  racion="20/05/20
+00002fd0: 3134 222c 0a20 2020 2020 2020 2020 2020  14",.           
+00002fe0: 2069 645f 6576 656e 746f 3d34 342c 0a20   id_evento=44,. 
+00002ff0: 2020 2020 2020 2020 2020 2063 6f64 5f70             cod_p
+00003000: 726f 6475 6374 6f3d 3838 3830 3030 3030  roducto=88800000
+00003010: 3030 3030 3335 2c20 2320 6163 6964 6f20  000035, # acido 
+00003020: 7375 6c66 fa72 6963 6f0a 2020 2020 2020  sulf.rico.      
+00003030: 2020 2020 2020 6e5f 6361 6e74 6964 6164        n_cantidad
+00003040: 3d31 2c0a 2020 2020 2020 2020 2020 2020  =1,.            
+00003050: 6e5f 646f 6375 6d65 6e74 6f5f 6f70 6572  n_documento_oper
+00003060: 6163 696f 6e3d 312c 0a20 2020 2020 2020  acion=1,.       
+00003070: 2020 2020 2023 6d5f 656e 7472 6567 615f       #m_entrega_
+00003080: 7061 7263 6961 6c3d 2222 2c0a 2020 2020  parcial="",.    
+00003090: 2020 2020 2020 2020 6e5f 7265 6d69 746f          n_remito
+000030a0: 3d31 3233 2c0a 2020 2020 2020 2020 2020  =123,.          
+000030b0: 2020 6e5f 7365 7269 653d 3131 322c 0a20    n_serie=112,. 
+000030c0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000030d0: 2020 2020 2070 7269 6e74 2822 5265 7375       print("Resu
+000030e0: 6c74 6164 6f22 2c20 7773 2e52 6573 756c  ltado", ws.Resul
+000030f0: 7461 646f 290a 2020 2020 2020 2020 7072  tado).        pr
+00003100: 696e 7428 2243 6f64 6967 6f54 7261 6e73  int("CodigoTrans
+00003110: 6163 6369 6f6e 222c 2077 732e 436f 6469  accion", ws.Codi
+00003120: 676f 5472 616e 7361 6363 696f 6e29 0a20  goTransaccion). 
+00003130: 2020 2020 2020 2070 7269 6e74 2822 4578         print("Ex
+00003140: 6365 7063 696f 6e65 7322 2c20 7773 2e45  cepciones", ws.E
+00003150: 7863 6570 6369 6f6e 290a 2020 2020 2020  xcepcion).      
+00003160: 2020 7072 696e 7428 2245 7272 6f65 7322    print("Erroes"
+00003170: 2c20 7773 2e45 7272 6f72 6573 290a 2020  , ws.Errores).  
+00003180: 2020 656c 6966 2027 2d2d 6361 6e63 656c    elif '--cancel
+00003190: 6127 2069 6e20 7379 732e 6172 6776 3a0a  a' in sys.argv:.
+000031a0: 2020 2020 2020 2020 7773 2e53 656e 6443          ws.SendC
+000031b0: 616e 6365 6c61 6354 7261 6e73 6163 6328  ancelacTransacc(
+000031c0: 2a73 7973 2e61 7267 765b 7379 732e 6172  *sys.argv[sys.ar
+000031d0: 6776 2e69 6e64 6578 2822 2d2d 6361 6e63  gv.index("--canc
+000031e0: 656c 6122 292b 313a 5d29 0a20 2020 2065  ela")+1:]).    e
+000031f0: 6c69 6620 272d 2d63 6f6e 7375 6c74 6127  lif '--consulta'
+00003200: 2069 6e20 7379 732e 6172 6776 3a0a 2020   in sys.argv:.  
+00003210: 2020 2020 2020 6966 2027 2d2d 6d6f 7669        if '--movi
+00003220: 6d69 656e 746f 7327 2069 6e20 7379 732e  mientos' in sys.
+00003230: 6172 6776 3a0a 2020 2020 2020 2020 2020  argv:.          
+00003240: 2020 7773 2e47 6574 5472 616e 7361 6363    ws.GetTransacc
+00003250: 696f 6e65 7357 5328 0a20 2020 2020 2020  ionesWS(.       
+00003260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003270: 2020 2020 2020 2020 202a 7379 732e 6172           *sys.ar
+00003280: 6776 5b73 7973 2e61 7267 762e 696e 6465  gv[sys.argv.inde
+00003290: 7828 222d 2d6d 6f76 696d 6965 6e74 6f73  x("--movimientos
+000032a0: 2229 2b31 3a5d 0a20 2020 2020 2020 2020  ")+1:].         
+000032b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032c0: 2020 2020 2020 2029 0a20 2020 2065 6c73         ).    els
+000032d0: 653a 0a20 2020 2020 2020 2077 732e 5361  e:.        ws.Sa
+000032e0: 7665 5472 616e 7361 6363 696f 6e65 7328  veTransacciones(
+000032f0: 2a73 7973 2e61 7267 765b 313a 5d29 0a20  *sys.argv[1:]). 
+00003300: 2020 2070 7269 6e74 2822 7c52 6573 756c     print("|Resul
+00003310: 7461 646f 2025 3573 7c43 6f64 6967 6f54  tado %5s|CodigoT
+00003320: 7261 6e73 6163 6369 6f6e 2025 3130 737c  ransaccion %10s|
+00003330: 4572 726f 7265 737c 2573 7c22 2025 2028  Errores|%s|" % (
+00003340: 0a20 2020 2020 2020 2020 2020 2077 732e  .            ws.
+00003350: 5265 7375 6c74 6164 6f2c 0a20 2020 2020  Resultado,.     
+00003360: 2020 2020 2020 2077 732e 436f 6469 676f         ws.Codigo
+00003370: 5472 616e 7361 6363 696f 6e2c 0a20 2020  Transaccion,.   
+00003380: 2020 2020 2020 2020 2027 7c27 2e6a 6f69           '|'.joi
+00003390: 6e28 7773 2e45 7272 6f72 6573 292c 0a20  n(ws.Errores),. 
+000033a0: 2020 2020 2020 2020 2020 2029 290a 2020             )).  
+000033b0: 2020 6966 2077 732e 4578 6365 7063 696f    if ws.Excepcio
+000033c0: 6e3a 0a20 2020 2020 2020 2070 7269 6e74  n:.        print
+000033d0: 2877 732e 5472 6163 6562 6163 6b29 0a0a  (ws.Traceback)..
+000033e0: 2320 6275 7363 6f20 656c 2064 6972 6563  # busco el direc
+000033f0: 746f 7269 6f20 6465 2069 6e73 7461 6c61  torio de instala
+00003400: 6369 f36e 2028 676c 6f62 616c 2070 6172  ci.n (global par
+00003410: 6120 7175 6520 6e6f 2063 616d 6269 6520  a que no cambie 
+00003420: 7369 2075 7361 6e20 6f74 7261 2064 6c6c  si usan otra dll
+00003430: 290a 494e 5354 414c 4c5f 4449 5220 3d20  ).INSTALL_DIR = 
+00003440: 5472 617a 6152 656e 7072 652e 496e 7374  TrazaRenpre.Inst
+00003450: 616c 6c44 6972 203d 2067 6574 5f69 6e73  allDir = get_ins
+00003460: 7461 6c6c 5f64 6972 2829 0a0a 0a69 6620  tall_dir()...if 
+00003470: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
+00003480: 6169 6e5f 5f27 3a0a 0a20 2020 2023 2061  ain__':..    # a
+00003490: 6a75 7374 6f20 656c 2065 6e63 6f64 696e  justo el encodin
+000034a0: 6720 706f 7220 6465 6665 6374 6f20 2873  g por defecto (s
+000034b0: 6920 7365 2072 6564 6972 696a 6520 6c61  i se redirije la
+000034c0: 2073 616c 6964 6129 0a20 2020 2069 6620   salida).    if 
+000034d0: 7379 732e 7374 646f 7574 2e65 6e63 6f64  sys.stdout.encod
+000034e0: 696e 6720 6973 204e 6f6e 653a 0a20 2020  ing is None:.   
+000034f0: 2020 2020 2069 6d70 6f72 7420 636f 6465       import code
+00003500: 6373 2c20 6c6f 6361 6c65 0a20 2020 2020  cs, locale.     
+00003510: 2020 2073 7973 2e73 7464 6f75 7420 3d20     sys.stdout = 
+00003520: 636f 6465 6373 2e67 6574 7772 6974 6572  codecs.getwriter
+00003530: 286c 6f63 616c 652e 6765 7470 7265 6665  (locale.getprefe
+00003540: 7272 6564 656e 636f 6469 6e67 2829 2928  rredencoding())(
+00003550: 7379 732e 7374 646f 7574 2c22 7265 706c  sys.stdout,"repl
+00003560: 6163 6522 293b 0a20 2020 2020 2020 2073  ace");.        s
+00003570: 7973 2e73 7464 6572 7220 3d20 636f 6465  ys.stderr = code
+00003580: 6373 2e67 6574 7772 6974 6572 286c 6f63  cs.getwriter(loc
+00003590: 616c 652e 6765 7470 7265 6665 7272 6564  ale.getpreferred
+000035a0: 656e 636f 6469 6e67 2829 2928 7379 732e  encoding())(sys.
+000035b0: 7374 6465 7272 2c22 7265 706c 6163 6522  stderr,"replace"
+000035c0: 293b 0a0a 2020 2020 6966 2027 2d2d 7265  );..    if '--re
+000035d0: 6769 7374 6572 2720 696e 2073 7973 2e61  gister' in sys.a
+000035e0: 7267 7620 6f72 2027 2d2d 756e 7265 6769  rgv or '--unregi
+000035f0: 7374 6572 2720 696e 2073 7973 2e61 7267  ster' in sys.arg
+00003600: 763a 0a20 2020 2020 2020 2069 6d70 6f72  v:.        impor
+00003610: 7420 7079 7468 6f6e 636f 6d0a 2020 2020  t pythoncom.    
+00003620: 2020 2020 696d 706f 7274 2077 696e 3332      import win32
+00003630: 636f 6d2e 7365 7276 6572 2e72 6567 6973  com.server.regis
+00003640: 7465 720a 2020 2020 2020 2020 7769 6e33  ter.        win3
+00003650: 3263 6f6d 2e73 6572 7665 722e 7265 6769  2com.server.regi
+00003660: 7374 6572 2e55 7365 436f 6d6d 616e 644c  ster.UseCommandL
+00003670: 696e 6528 5472 617a 6152 656e 7072 6529  ine(TrazaRenpre)
+00003680: 0a20 2020 2065 6c69 6620 222f 4175 746f  .    elif "/Auto
+00003690: 6d61 7465 2220 696e 2073 7973 2e61 7267  mate" in sys.arg
+000036a0: 763a 0a20 2020 2020 2020 2023 204d 5320  v:.        # MS 
+000036b0: 7365 656d 7320 746f 206c 696b 6520 2f61  seems to like /a
+000036c0: 7574 6f6d 6174 6520 746f 2072 756e 2074  utomate to run t
+000036d0: 6865 2063 6c61 7373 2066 6163 746f 7269  he class factori
+000036e0: 6573 2e0a 2020 2020 2020 2020 696d 706f  es..        impo
+000036f0: 7274 2077 696e 3332 636f 6d2e 7365 7276  rt win32com.serv
+00003700: 6572 2e6c 6f63 616c 7365 7276 6572 0a20  er.localserver. 
+00003710: 2020 2020 2020 2023 7769 6e33 3263 6f6d         #win32com
+00003720: 2e73 6572 7665 722e 6c6f 6361 6c73 6572  .server.localser
+00003730: 7665 722e 6d61 696e 2829 0a20 2020 2020  ver.main().     
+00003740: 2020 2023 2073 7461 7274 2074 6865 2073     # start the s
+00003750: 6572 7665 722e 0a20 2020 2020 2020 2077  erver..        w
+00003760: 696e 3332 636f 6d2e 7365 7276 6572 2e6c  in32com.server.l
+00003770: 6f63 616c 7365 7276 6572 2e73 6572 7665  ocalserver.serve
+00003780: 285b 5472 617a 6152 656e 7072 652e 5f72  ([TrazaRenpre._r
+00003790: 6567 5f63 6c73 6964 5f5d 290a 2020 2020  eg_clsid_]).    
+000037a0: 656c 7365 3a0a 2020 2020 2020 2020 6d61  else:.        ma
+000037b0: 696e 2829 0a                             in().
```

### Comparing `py3afipws-0.8/py3afipws/trazavet.py` & `py3afipws-0.9/py3afipws/trazavet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,1382 +1,1384 @@
 00000000: 2321 2f75 7372 2f62 696e 2f70 7974 686f  #!/usr/bin/pytho
-00000010: 6e0a 2320 5468 6973 2070 726f 6772 616d  n.# This program
-00000020: 2069 7320 6672 6565 2073 6f66 7477 6172   is free softwar
-00000030: 653b 2079 6f75 2063 616e 2072 6564 6973  e; you can redis
-00000040: 7472 6962 7574 6520 6974 2061 6e64 2f6f  tribute it and/o
-00000050: 7220 6d6f 6469 6679 0a23 2069 7420 756e  r modify.# it un
-00000060: 6465 7220 7468 6520 7465 726d 7320 6f66  der the terms of
-00000070: 2074 6865 2047 4e55 2047 656e 6572 616c   the GNU General
-00000080: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
-00000090: 6173 2070 7562 6c69 7368 6564 2062 7920  as published by 
-000000a0: 7468 650a 2320 4672 6565 2053 6f66 7477  the.# Free Softw
-000000b0: 6172 6520 466f 756e 6461 7469 6f6e 3b20  are Foundation; 
-000000c0: 6569 7468 6572 2076 6572 7369 6f6e 2033  either version 3
-000000d0: 2c20 6f72 2028 6174 2079 6f75 7220 6f70  , or (at your op
-000000e0: 7469 6f6e 2920 616e 7920 6c61 7465 720a  tion) any later.
-000000f0: 2320 7665 7273 696f 6e2e 0a23 0a23 2054  # version..#.# T
-00000100: 6869 7320 7072 6f67 7261 6d20 6973 2064  his program is d
-00000110: 6973 7472 6962 7574 6564 2069 6e20 7468  istributed in th
-00000120: 6520 686f 7065 2074 6861 7420 6974 2077  e hope that it w
-00000130: 696c 6c20 6265 2075 7365 6675 6c2c 2062  ill be useful, b
-00000140: 7574 0a23 2057 4954 484f 5554 2041 4e59  ut.# WITHOUT ANY
-00000150: 2057 4152 5241 4e54 593b 2077 6974 686f   WARRANTY; witho
-00000160: 7574 2065 7665 6e20 7468 6520 696d 706c  ut even the impl
-00000170: 6965 6420 7761 7272 616e 7479 206f 6620  ied warranty of 
-00000180: 4d45 5243 4841 4e54 4942 494c 4954 590a  MERCHANTIBILITY.
-00000190: 2320 6f72 2046 4954 4e45 5353 2046 4f52  # or FITNESS FOR
-000001a0: 2041 2050 4152 5449 4355 4c41 5220 5055   A PARTICULAR PU
-000001b0: 5250 4f53 452e 2020 5365 6520 7468 6520  RPOSE.  See the 
-000001c0: 474e 5520 4765 6e65 7261 6c20 5075 626c  GNU General Publ
-000001d0: 6963 204c 6963 656e 7365 0a23 2066 6f72  ic License.# for
-000001e0: 206d 6f72 6520 6465 7461 696c 732e 0a0a   more details...
-000001f0: 224d f364 756c 6f20 5472 617a 6162 696c  "M.dulo Trazabil
-00000200: 6964 6164 2064 6520 5072 6f64 7563 746f  idad de Producto
-00000210: 7320 5665 7465 7269 6e61 7269 6f73 2053  s Veterinarios S
-00000220: 454e 4153 4120 5265 736f 6c75 6369 f36e  ENASA Resoluci.n
-00000230: 2033 3639 2f32 3031 3322 0a0a 2320 496e   369/2013"..# In
-00000240: 666f 726d 6163 69f3 6e20 6164 6963 696f  formaci.n adicio
-00000250: 6e61 6c20 7920 646f 6375 6d65 6e74 6163  nal y documentac
-00000260: 69f3 6e3a 0a23 2068 7474 703a 2f2f 7777  i.n:.# http://ww
-00000270: 772e 7369 7374 656d 6173 6167 696c 6573  w.sistemasagiles
-00000280: 2e63 6f6d 2e61 722f 7472 6163 2f77 696b  .com.ar/trac/wik
-00000290: 692f 5472 617a 6162 696c 6964 6164 5072  i/TrazabilidadPr
-000002a0: 6f64 7563 746f 7356 6574 6572 696e 6172  oductosVeterinar
-000002b0: 696f 730a 0a5f 5f61 7574 686f 725f 5f20  ios..__author__ 
-000002c0: 3d20 224d 6172 6961 6e6f 2052 6569 6e67  = "Mariano Reing
-000002d0: 6172 7420 3c72 6569 6e67 6172 7440 676d  art <reingart@gm
-000002e0: 6169 6c2e 636f 6d3e 220a 5f5f 636f 7079  ail.com>".__copy
-000002f0: 7269 6768 745f 5f20 3d20 2243 6f70 7972  right__ = "Copyr
-00000300: 6967 6874 2028 4329 2032 3031 3420 4d61  ight (C) 2014 Ma
-00000310: 7269 616e 6f20 5265 696e 6761 7274 220a  riano Reingart".
-00000320: 5f5f 6c69 6365 6e73 655f 5f20 3d20 2247  __license__ = "G
-00000330: 504c 2033 2e30 2b22 0a5f 5f76 6572 7369  PL 3.0+".__versi
-00000340: 6f6e 5f5f 203d 2022 312e 3131 6422 0a0a  on__ = "1.11d"..
-00000350: 2320 6874 7470 3a2f 2f73 656e 6173 612e  # http://senasa.
-00000360: 7365 7276 6963 696f 732e 7061 6d69 2e6f  servicios.pami.o
-00000370: 7267 2e61 722f 0a0a 696d 706f 7274 206f  rg.ar/..import o
-00000380: 730a 696d 706f 7274 2073 6f63 6b65 740a  s.import socket.
-00000390: 696d 706f 7274 2073 7973 0a69 6d70 6f72  import sys.impor
-000003a0: 7420 6461 7465 7469 6d65 2c20 7469 6d65  t datetime, time
-000003b0: 0a69 6d70 6f72 7420 7472 6163 6562 6163  .import tracebac
-000003c0: 6b0a 696d 706f 7274 2070 7933 7369 6d70  k.import py3simp
-000003d0: 6c65 736f 6170 2e63 6c69 656e 740a 6672  lesoap.client.fr
-000003e0: 6f6d 2070 7933 7369 6d70 6c65 736f 6170  om py3simplesoap
-000003f0: 2e63 6c69 656e 7420 696d 706f 7274 2053  .client import S
-00000400: 6f61 7043 6c69 656e 742c 2053 6f61 7046  oapClient, SoapF
-00000410: 6175 6c74 2c20 7061 7273 655f 7072 6f78  ault, parse_prox
-00000420: 792c 205c 0a20 2020 2020 2020 2020 2020  y, \.           
-00000430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000440: 2020 2020 2073 6574 5f68 7474 705f 7772       set_http_wr
-00000450: 6170 7065 720a 6672 6f6d 2070 7933 7369  apper.from py3si
-00000460: 6d70 6c65 736f 6170 2e73 696d 706c 6578  mplesoap.simplex
-00000470: 6d6c 2069 6d70 6f72 7420 5369 6d70 6c65  ml import Simple
-00000480: 584d 4c45 6c65 6d65 6e74 0a66 726f 6d20  XMLElement.from 
-00000490: 6353 7472 696e 6749 4f20 696d 706f 7274  cStringIO import
-000004a0: 2053 7472 696e 6749 4f0a 0a23 2069 6d70   StringIO..# imp
-000004b0: 6f72 746f 2066 756e 6369 6f6e 6573 2063  orto funciones c
-000004c0: 6f6d 7061 7274 6964 6173 3a0a 6672 6f6d  ompartidas:.from
-000004d0: 202e 7574 696c 7320 696d 706f 7274 206c   .utils import l
-000004e0: 6565 722c 2065 7363 7269 6269 722c 206c  eer, escribir, l
-000004f0: 6565 725f 6462 662c 2067 7561 7264 6172  eer_dbf, guardar
-00000500: 5f64 6266 2c20 4e2c 2041 2c20 492c 206a  _dbf, N, A, I, j
-00000510: 736f 6e2c 205c 0a20 2020 2020 2020 2020  son, \.         
-00000520: 2020 2020 2020 2020 2064 6172 5f6e 6f6d           dar_nom
-00000530: 6272 655f 6361 6d70 6f5f 6462 662c 2067  bre_campo_dbf, g
-00000540: 6574 5f69 6e73 7461 6c6c 5f64 6972 2c20  et_install_dir, 
-00000550: 4261 7365 5753 2c20 5c0a 2020 2020 2020  BaseWS, \.      
-00000560: 2020 2020 2020 2020 2020 2020 696e 6963              inic
-00000570: 6961 6c69 7a61 725f 795f 6361 7074 7572  ializar_y_captur
-00000580: 6172 5f65 7863 6570 6369 6f6e 6573 0a0a  ar_excepciones..
-00000590: 484f 4d4f 203d 2054 7275 650a 5459 5045  HOMO = True.TYPE
-000005a0: 4c49 4220 3d20 4661 6c73 650a 0a57 5344  LIB = False..WSD
-000005b0: 4c20 3d20 2268 7474 7073 3a2f 2f73 6572  L = "https://ser
-000005c0: 7669 6369 6f73 2e70 616d 692e 6f72 672e  vicios.pami.org.
-000005d0: 6172 2f74 7261 7a61 656e 7665 742e 5765  ar/trazaenvet.We
-000005e0: 6253 6572 7669 6365 3f77 7364 6c22 0a4c  bService?wsdl".L
-000005f0: 4f43 4154 494f 4e20 3d20 2268 7474 7073  OCATION = "https
-00000600: 3a2f 2f73 6572 7669 6369 6f73 2e70 616d  ://servicios.pam
-00000610: 692e 6f72 672e 6172 2f74 7261 7a61 656e  i.org.ar/trazaen
-00000620: 7665 742e 5765 6253 6572 7669 6365 3f77  vet.WebService?w
-00000630: 7364 6c22 0a0a 2320 466f 726d 6174 6f20  sdl"..# Formato 
-00000640: 6465 2054 7261 6e73 6163 6369 6f6e 5365  de TransaccionSe
-00000650: 6e61 7361 4454 4f20 2853 6176 6554 7261  nasaDTO (SaveTra
-00000660: 6e73 6163 6369 6f6e 290a 5452 414e 5341  nsaccion).TRANSA
-00000670: 4343 494f 4e5f 4454 4f20 3d20 5b0a 2020  CCION_DTO = [.  
-00000680: 2020 2827 676c 6e5f 6f72 6967 656e 272c    ('gln_origen',
-00000690: 2031 332c 2041 292c 0a20 2020 2028 2767   13, A),.    ('g
-000006a0: 6c6e 5f64 6573 7469 6e6f 272c 2031 332c  ln_destino', 13,
-000006b0: 2041 292c 0a20 2020 2028 2766 5f6f 7065   A),.    ('f_ope
-000006c0: 7261 6369 6f6e 272c 2031 302c 2041 292c  racion', 10, A),
-000006d0: 0a20 2020 2028 2766 5f65 6c61 626f 7261  .    ('f_elabora
-000006e0: 6369 6f6e 272c 2031 302c 2041 292c 0a20  cion', 10, A),. 
-000006f0: 2020 2028 2766 5f76 746f 272c 2031 302c     ('f_vto', 10,
-00000700: 2041 292c 0a20 2020 2028 2769 645f 6576   A),.    ('id_ev
-00000710: 656e 746f 272c 2031 352c 204e 292c 0a20  ento', 15, N),. 
-00000720: 2020 2028 2763 6f64 5f70 726f 6475 6374     ('cod_product
-00000730: 6f27 2c20 3134 2c20 4129 2c0a 2020 2020  o', 14, A),.    
-00000740: 2827 6e5f 6361 6e74 6964 6164 272c 2033  ('n_cantidad', 3
-00000750: 302c 204e 292c 0a20 2020 2028 276e 5f73  0, N),.    ('n_s
-00000760: 6572 6965 272c 2032 302c 2041 292c 0a20  erie', 20, A),. 
-00000770: 2020 2028 276e 5f6c 6f74 6527 2c20 3530     ('n_lote', 50
-00000780: 2c20 4129 2c0a 2020 2020 2827 6e5f 6361  , A),.    ('n_ca
-00000790: 6927 2c20 3135 2c20 4129 2c0a 2020 2020  i', 15, A),.    
-000007a0: 2827 6e5f 6361 6527 2c20 3135 2c20 4129  ('n_cae', 15, A)
-000007b0: 2c0a 2020 2020 2827 6964 5f6d 6f74 6976  ,.    ('id_motiv
-000007c0: 6f5f 6465 7374 7275 6363 696f 6e27 2c20  o_destruccion', 
-000007d0: 352c 2041 292c 0a20 2020 2028 276e 5f6d  5, A),.    ('n_m
-000007e0: 616e 6966 6965 7374 6f27 2c20 3135 2c20  anifiesto', 15, 
-000007f0: 4e29 2c0a 2020 2020 2827 656e 5f74 7261  N),.    ('en_tra
-00000800: 6e73 706f 7274 6527 2c20 312c 2041 292c  nsporte', 1, A),
-00000810: 2023 2062 6f6f 6c65 616e 0a20 2020 2028   # boolean.    (
-00000820: 276e 5f72 656d 6974 6f27 2c20 3135 2c20  'n_remito', 15, 
-00000830: 4129 2c0a 2020 2020 2827 6d6f 7469 766f  A),.    ('motivo
-00000840: 5f64 6576 6f6c 7563 696f 6e27 2c20 3130  _devolucion', 10
-00000850: 302c 2041 292c 0a20 2020 2028 276f 6273  0, A),.    ('obs
-00000860: 6572 7661 6369 6f6e 6573 272c 2031 3030  ervaciones', 100
-00000870: 302c 2041 292c 0a20 2020 2028 276e 5f76  0, A),.    ('n_v
-00000880: 616c 655f 636f 6d70 7261 272c 2031 352c  ale_compra', 15,
-00000890: 2041 292c 0a20 2020 2028 2761 7065 6c6c   A),.    ('apell
-000008a0: 6964 6f4e 6f6d 6272 6573 272c 2032 3535  idoNombres', 255
-000008b0: 2c20 4129 2c0a 2020 2020 2827 6469 7265  , A),.    ('dire
-000008c0: 6363 696f 6e27 2c20 3230 302c 2041 292c  ccion', 200, A),
-000008d0: 0a20 2020 2028 276e 756d 6572 6f27 2c20  .    ('numero', 
-000008e0: 362c 204e 292c 0a20 2020 2028 276c 6f63  6, N),.    ('loc
-000008f0: 616c 6964 6164 272c 2031 352c 2041 292c  alidad', 15, A),
-00000900: 0a20 2020 2028 2770 726f 7669 6e63 6961  .    ('provincia
-00000910: 272c 2031 352c 2041 292c 0a20 2020 2028  ', 15, A),.    (
-00000920: 276e 5f70 6f73 7461 6c27 2c20 382c 2041  'n_postal', 8, A
-00000930: 292c 0a20 2020 2028 2763 7569 7427 2c20  ),.    ('cuit', 
-00000940: 3131 2c20 4129 2c0a 2020 2020 2827 636f  11, A),.    ('co
-00000950: 6469 676f 5f74 7261 6e73 6163 6369 6f6e  digo_transaccion
-00000960: 272c 2031 342c 2041 292c 0a5d 0a0a 2320  ', 14, A),.]..# 
-00000970: 466f 726d 6174 6f20 7061 7261 2054 7261  Formato para Tra
-00000980: 6e73 6163 6369 6f6e 5365 6e61 7361 2028  nsaccionSenasa (
-00000990: 6765 7454 7261 6e73 6163 6369 6f6e 6573  getTransacciones
-000009a0: 290a 5452 414e 5341 4343 494f 4e45 5320  ).TRANSACCIONES 
-000009b0: 3d20 5b0a 2020 2020 2827 6964 5f74 7261  = [.    ('id_tra
-000009c0: 6e73 6163 6369 6f6e 5f67 6c6f 6261 6c27  nsaccion_global'
-000009d0: 2c20 3135 2c20 4e29 2c0a 2020 2020 2827  , 15, N),.    ('
-000009e0: 6964 5f74 7261 6e73 6163 6369 6f6e 272c  id_transaccion',
-000009f0: 2031 352c 204e 292c 0a20 2020 2028 2766   15, N),.    ('f
-00000a00: 5f74 7261 6e73 6163 6369 6f6e 272c 2031  _transaccion', 1
-00000a10: 302c 2041 292c 0a20 2020 2028 2766 5f6f  0, A),.    ('f_o
-00000a20: 7065 7261 6369 6f6e 272c 2031 302c 2041  peracion', 10, A
-00000a30: 292c 0a20 2020 2028 2766 5f76 656e 6369  ),.    ('f_venci
-00000a40: 6d69 656e 746f 272c 2031 302c 2041 292c  miento', 10, A),
-00000a50: 0a20 2020 2028 2766 5f65 6c61 626f 7261  .    ('f_elabora
-00000a60: 6369 6f6e 272c 2031 302c 2041 292c 0a20  cion', 10, A),. 
-00000a70: 2020 2028 2764 5f65 7665 6e74 6f27 2c20     ('d_evento', 
-00000a80: 3130 302c 2041 292c 0a20 2020 2028 276e  100, A),.    ('n
-00000a90: 5f63 616e 7469 6461 6427 2c20 3330 2c20  _cantidad', 30, 
-00000aa0: 4e29 2c0a 2020 2020 2827 6964 5f75 6e69  N),.    ('id_uni
-00000ab0: 6461 6427 2c20 3135 2c20 4e29 2c0a 2020  dad', 15, N),.  
-00000ac0: 2020 2827 645f 756e 6964 6164 272c 2031    ('d_unidad', 1
-00000ad0: 3030 2c20 4129 2c0a 2020 2020 2827 636f  00, A),.    ('co
-00000ae0: 645f 7072 6f64 7563 746f 272c 2031 342c  d_producto', 14,
-00000af0: 2041 292c 0a20 2020 2028 2769 645f 756e   A),.    ('id_un
-00000b00: 6964 6164 272c 2031 352c 204e 292c 0a20  idad', 15, N),. 
-00000b10: 2020 2028 276e 5f73 6572 6965 272c 2032     ('n_serie', 2
-00000b20: 302c 2041 292c 0a20 2020 2028 276e 5f6c  0, A),.    ('n_l
-00000b30: 6f74 6527 2c20 3530 2c20 4129 2c0a 2020  ote', 50, A),.  
-00000b40: 2020 2827 6e5f 6361 6927 2c20 3135 2c20    ('n_cai', 15, 
-00000b50: 4129 2c0a 2020 2020 2827 6e5f 6361 6527  A),.    ('n_cae'
-00000b60: 2c20 3135 2c20 4129 2c0a 2020 2020 2827  , 15, A),.    ('
-00000b70: 645f 6d6f 7469 766f 5f64 6573 7472 7563  d_motivo_destruc
-00000b80: 6369 6f6e 272c 2035 302c 2041 292c 0a20  cion', 50, A),. 
-00000b90: 2020 2028 2764 5f6d 616e 6966 6965 7374     ('d_manifiest
-00000ba0: 6f27 2c20 3135 2c20 4129 2c0a 2020 2020  o', 15, A),.    
-00000bb0: 2827 656e 5f74 7261 6e73 706f 7274 6527  ('en_transporte'
-00000bc0: 2c20 312c 2041 292c 0a20 2020 2028 276e  , 1, A),.    ('n
-00000bd0: 5f72 656d 6974 6f27 2c20 3330 2c20 4129  _remito', 30, A)
-00000be0: 2c0a 2020 2020 2827 6d6f 7469 766f 5f64  ,.    ('motivo_d
-00000bf0: 6576 6f6c 7563 696f 6e27 2c20 3230 302c  evolucion', 200,
-00000c00: 2041 292c 0a20 2020 2028 276f 6273 6572   A),.    ('obser
-00000c10: 7661 6369 6f6e 6573 272c 2031 3030 302c  vaciones', 1000,
-00000c20: 2041 292c 0a20 2020 2028 276e 5f76 616c   A),.    ('n_val
-00000c30: 655f 636f 6d70 7261 272c 2031 352c 2041  e_compra', 15, A
-00000c40: 292c 0a20 2020 2028 2761 7065 6c6c 6964  ),.    ('apellid
-00000c50: 6f4e 6f6d 6272 6573 272c 2032 3535 2c20  oNombres', 255, 
-00000c60: 4129 2c0a 2020 2020 2827 6469 7265 6363  A),.    ('direcc
-00000c70: 696f 6e27 2c20 3230 302c 2041 292c 0a20  ion', 200, A),. 
-00000c80: 2020 2028 276e 756d 6572 6f27 2c20 362c     ('numero', 6,
-00000c90: 2041 292c 0a20 2020 2028 276c 6f63 616c   A),.    ('local
-00000ca0: 6964 6164 272c 2032 3530 2c20 4129 2c0a  idad', 250, A),.
-00000cb0: 2020 2020 2827 7072 6f76 696e 6369 6127      ('provincia'
-00000cc0: 2c20 3235 302c 2041 292c 0a20 2020 2028  , 250, A),.    (
-00000cd0: 276e 5f70 6f73 7461 6c27 2c20 382c 2041  'n_postal', 8, A
-00000ce0: 292c 0a20 2020 2028 2763 7569 7427 2c20  ),.    ('cuit', 
-00000cf0: 3131 2c20 4129 2c0a 2020 2020 2827 645f  11, A),.    ('d_
-00000d00: 6167 656e 7465 5f69 6e66 6f72 6d61 646f  agente_informado
-00000d10: 7227 2c20 3235 352c 2041 292c 0a20 2020  r', 255, A),.   
-00000d20: 2028 2764 5f61 6765 6e74 655f 6f72 6967   ('d_agente_orig
-00000d30: 656e 272c 2032 3535 2c20 4129 2c0a 2020  en', 255, A),.  
-00000d40: 2020 2827 645f 6167 656e 7465 5f64 6573    ('d_agente_des
-00000d50: 7469 6e6f 272c 2032 3535 2c20 4129 2c0a  tino', 255, A),.
-00000d60: 2020 2020 2827 645f 7072 6f64 7563 746f      ('d_producto
-00000d70: 272c 2032 3530 2c20 4129 2c0a 2020 2020  ', 250, A),.    
-00000d80: 2827 645f 6573 7461 646f 5f74 7261 6e73  ('d_estado_trans
-00000d90: 6163 6369 6f6e 272c 2033 302c 2041 292c  accion', 30, A),
-00000da0: 0a20 2020 2028 2764 5f74 6970 6f5f 7472  .    ('d_tipo_tr
-00000db0: 616e 7361 6363 696f 6e27 2c20 3330 2c20  ansaccion', 30, 
-00000dc0: 4129 2c0a 5d0a 0a23 2046 6f72 6d61 746f  A),.]..# Formato
-00000dd0: 2070 6172 6120 4572 726f 7265 730a 4552   para Errores.ER
-00000de0: 524f 5245 5320 3d20 5b0a 2020 2020 2827  RORES = [.    ('
-00000df0: 5f63 5f65 7272 6f72 272c 2034 2c20 4129  _c_error', 4, A)
-00000e00: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
-00000e10: 2020 2320 63f3 6469 676f 0a20 2020 2028    # c.digo.    (
-00000e20: 275f 645f 6572 726f 7227 2c20 3235 302c  '_d_error', 250,
-00000e30: 2041 292c 2020 2020 2020 2020 2020 2020   A),            
-00000e40: 2020 2023 2064 6573 6372 6970 6369 f36e     # descripci.n
-00000e50: 0a20 2020 205d 0a0a 0a63 6c61 7373 2054  .    ]...class T
-00000e60: 7261 7a61 5665 7428 4261 7365 5753 293a  razaVet(BaseWS):
-00000e70: 0a20 2020 2022 496e 7465 7266 617a 2070  .    "Interfaz p
-00000e80: 6172 6120 656c 2057 6562 5365 7276 6963  ara el WebServic
-00000e90: 6520 6465 2054 7261 7a61 6269 6c69 6461  e de Trazabilida
-00000ea0: 6420 6465 2056 6574 6572 696e 6172 696f  d de Veterinario
-00000eb0: 7320 5345 4e41 5341 220a 0a20 2020 205f  s SENASA"..    _
-00000ec0: 7075 626c 6963 5f6d 6574 686f 6473 5f20  public_methods_ 
-00000ed0: 3d20 5b27 5361 7665 5472 616e 7361 6363  = ['SaveTransacc
-00000ee0: 696f 6e27 2c20 2753 656e 6443 616e 6365  ion', 'SendCance
-00000ef0: 6c61 5472 616e 7361 6327 2c0a 2020 2020  laTransac',.    
-00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f10: 2020 2020 2753 656e 6443 6f6e 6669 726d      'SendConfirm
-00000f20: 6154 7261 6e73 6163 6327 2c20 2753 656e  aTransacc', 'Sen
-00000f30: 6441 6c65 7274 6154 7261 6e73 6163 6327  dAlertaTransacc'
-00000f40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000f50: 2020 2020 2020 2020 2020 2747 6574 5472            'GetTr
-00000f60: 616e 7361 6363 696f 6e65 7327 2c0a 2020  ansacciones',.  
-00000f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f80: 2020 2020 2020 2743 6f6e 6563 7461 7227        'Conectar'
-00000f90: 2c20 274c 6565 7245 7272 6f72 272c 2027  , 'LeerError', '
-00000fa0: 4c65 6572 5472 616e 7361 6363 696f 6e27  LeerTransaccion'
-00000fb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000fc0: 2020 2020 2020 2020 2020 2753 6574 5573            'SetUs
-00000fd0: 6572 6e61 6d65 272c 0a20 2020 2020 2020  ername',.       
-00000fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ff0: 2027 5365 7450 6172 616d 6574 726f 272c   'SetParametro',
-00001000: 2027 4765 7450 6172 616d 6574 726f 272c   'GetParametro',
-00001010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001020: 2020 2020 2020 2020 2027 4765 7443 6f64           'GetCod
-00001030: 6967 6f54 7261 6e73 6163 6369 6f6e 272c  igoTransaccion',
-00001040: 2027 4765 7452 6573 756c 7461 646f 272c   'GetResultado',
-00001050: 2027 4c6f 6164 5465 7374 584d 4c27 5d0a   'LoadTestXML'].
-00001060: 0a20 2020 205f 7075 626c 6963 5f61 7474  .    _public_att
-00001070: 7273 5f20 3d20 5b0a 2020 2020 2020 2020  rs_ = [.        
-00001080: 2755 7365 726e 616d 6527 2c20 2750 6173  'Username', 'Pas
-00001090: 7377 6f72 6427 2c0a 2020 2020 2020 2020  sword',.        
-000010a0: 2743 6f64 6967 6f54 7261 6e73 6163 6369  'CodigoTransacci
-000010b0: 6f6e 272c 2027 4572 726f 7265 7327 2c20  on', 'Errores', 
-000010c0: 2752 6573 756c 7461 646f 272c 0a20 2020  'Resultado',.   
-000010d0: 2020 2020 2027 586d 6c52 6571 7565 7374       'XmlRequest
-000010e0: 272c 2027 586d 6c52 6573 706f 6e73 6527  ', 'XmlResponse'
-000010f0: 2c0a 2020 2020 2020 2020 2756 6572 7369  ,.        'Versi
-00001100: 6f6e 272c 2027 496e 7374 616c 6c44 6972  on', 'InstallDir
-00001110: 272c 0a20 2020 2020 2020 2027 5472 6163  ',.        'Trac
-00001120: 6562 6163 6b27 2c20 2745 7863 6570 6369  eback', 'Excepci
-00001130: 6f6e 272c 0a20 2020 2020 2020 2027 4361  on',.        'Ca
-00001140: 6e74 5061 6769 6e61 7327 2c20 2748 6179  ntPaginas', 'Hay
-00001150: 4572 726f 7227 2c20 2754 7261 6e73 6163  Error', 'Transac
-00001160: 6369 6f6e 5365 6e61 7361 272c 0a20 2020  cionSenasa',.   
-00001170: 2020 2020 205d 0a0a 2020 2020 5f72 6567       ]..    _reg
-00001180: 5f70 726f 6769 645f 203d 2022 5472 617a  _progid_ = "Traz
-00001190: 6156 6574 220a 2020 2020 5f72 6567 5f63  aVet".    _reg_c
-000011a0: 6c73 6964 5f20 3d20 227b 3245 3238 4437  lsid_ = "{2E28D7
-000011b0: 3944 2d32 3342 302d 3443 3145 2d38 3542  9D-23B0-4C1E-85B
-000011c0: 392d 3634 4244 4334 3142 3846 4346 7d22  9-64BDC41B8FCF}"
-000011d0: 0a0a 2020 2020 2320 5661 7269 6162 6c65  ..    # Variable
-000011e0: 7320 676c 6f62 616c 6573 2070 6172 6120  s globales para 
-000011f0: 4261 7365 5753 3a0a 2020 2020 484f 4d4f  BaseWS:.    HOMO
-00001200: 203d 2048 4f4d 4f0a 2020 2020 5753 444c   = HOMO.    WSDL
-00001210: 203d 2057 5344 4c0a 2020 2020 5665 7273   = WSDL.    Vers
-00001220: 696f 6e20 3d20 2225 7320 2573 2025 7322  ion = "%s %s %s"
-00001230: 2025 2028 5f5f 7665 7273 696f 6e5f 5f2c   % (__version__,
-00001240: 2048 4f4d 4f20 616e 6420 2748 6f6d 6f6c   HOMO and 'Homol
-00001250: 6f67 6163 69f3 6e27 206f 7220 2727 2c0a  ogaci.n' or '',.
-00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001270: 2020 2020 2020 2020 2020 2020 7079 3373              py3s
-00001280: 696d 706c 6573 6f61 702e 636c 6965 6e74  implesoap.client
-00001290: 2e5f 5f76 6572 7369 6f6e 5f5f 290a 0a20  .__version__).. 
-000012a0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-000012b0: 7365 6c66 2c20 7265 696e 7465 6e74 6f73  self, reintentos
-000012c0: 3d31 293a 0a20 2020 2020 2020 2073 656c  =1):.        sel
-000012d0: 662e 5573 6572 6e61 6d65 203d 2073 656c  f.Username = sel
-000012e0: 662e 5061 7373 776f 7264 203d 204e 6f6e  f.Password = Non
-000012f0: 650a 2020 2020 2020 2020 7365 6c66 2e54  e.        self.T
-00001300: 7261 6e73 6163 6369 6f6e 5365 6e61 7361  ransaccionSenasa
-00001310: 203d 205b 5d0a 2020 2020 2020 2020 4261   = [].        Ba
-00001320: 7365 5753 2e5f 5f69 6e69 745f 5f28 7365  seWS.__init__(se
-00001330: 6c66 2c20 7265 696e 7465 6e74 6f73 290a  lf, reintentos).
-00001340: 0a20 2020 2064 6566 2069 6e69 6369 616c  .    def inicial
-00001350: 697a 6172 2873 656c 6629 3a0a 2020 2020  izar(self):.    
-00001360: 2020 2020 4261 7365 5753 2e69 6e69 6369      BaseWS.inici
-00001370: 616c 697a 6172 2873 656c 6629 0a20 2020  alizar(self).   
-00001380: 2020 2020 2073 656c 662e 436f 6469 676f       self.Codigo
-00001390: 5472 616e 7361 6363 696f 6e20 3d20 7365  Transaccion = se
-000013a0: 6c66 2e45 7272 6f72 6573 203d 2073 656c  lf.Errores = sel
-000013b0: 662e 5265 7375 6c74 6164 6f20 3d20 4e6f  f.Resultado = No
-000013c0: 6e65 0a20 2020 2020 2020 2073 656c 662e  ne.        self.
-000013d0: 5265 7375 6c74 6164 6f20 3d20 2727 0a20  Resultado = ''. 
-000013e0: 2020 2020 2020 2073 656c 662e 4572 726f         self.Erro
-000013f0: 7265 7320 3d20 5b5d 2020 2023 206c 6973  res = []   # lis
-00001400: 7461 2064 6520 7374 7269 6e67 7320 7061  ta de strings pa
-00001410: 7261 206c 6120 696e 7465 7266 617a 0a20  ra la interfaz. 
-00001420: 2020 2020 2020 2073 656c 662e 6572 726f         self.erro
-00001430: 7265 7320 3d20 5b5d 2020 2023 206c 6973  res = []   # lis
-00001440: 7461 2064 6520 6469 6363 696f 6e61 7269  ta de diccionari
-00001450: 6f73 2028 7573 6f20 696e 7465 726e 6f29  os (uso interno)
-00001460: 0a20 2020 2020 2020 2073 656c 662e 4361  .        self.Ca
-00001470: 6e74 5061 6769 6e61 7320 3d20 7365 6c66  ntPaginas = self
-00001480: 2e48 6179 4572 726f 7220 3d20 4e6f 6e65  .HayError = None
-00001490: 0a0a 2020 2020 6465 6620 5f5f 616e 616c  ..    def __anal
-000014a0: 697a 6172 5f65 7272 6f72 6573 2873 656c  izar_errores(sel
-000014b0: 662c 2072 6574 293a 0a20 2020 2020 2020  f, ret):.       
-000014c0: 2022 436f 6d70 7275 6562 6120 7920 6578   "Comprueba y ex
-000014d0: 7472 6165 2065 7272 6f72 6573 2073 6920  trae errores si 
-000014e0: 6578 6973 7465 6e20 656e 206c 6120 7265  existen en la re
-000014f0: 7370 7565 7374 6120 584d 4c22 0a20 2020  spuesta XML".   
-00001500: 2020 2020 2073 656c 662e 6572 726f 7265       self.errore
-00001510: 7320 3d20 7265 742e 6765 7428 2765 7272  s = ret.get('err
-00001520: 6f72 6573 272c 205b 5d29 0a20 2020 2020  ores', []).     
-00001530: 2020 2073 656c 662e 4572 726f 7265 7320     self.Errores 
-00001540: 3d20 5b22 2573 3a20 2573 2220 2520 2869  = ["%s: %s" % (i
-00001550: 745b 2763 5f65 7272 6f72 275d 2c20 6974  t['c_error'], it
-00001560: 5b27 645f 6572 726f 7227 5d29 0a20 2020  ['d_error']).   
-00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001580: 2020 2020 2066 6f72 2069 7420 696e 2072       for it in r
-00001590: 6574 2e67 6574 2827 6572 726f 7265 7327  et.get('errores'
-000015a0: 2c20 5b5d 295d 0a20 2020 2020 2020 2073  , [])].        s
-000015b0: 656c 662e 5265 7375 6c74 6164 6f20 3d20  elf.Resultado = 
-000015c0: 7265 742e 6765 7428 2772 6573 756c 7461  ret.get('resulta
-000015d0: 646f 2729 0a0a 2020 2020 6465 6620 436f  do')..    def Co
-000015e0: 6e65 6374 6172 2873 656c 662c 2063 6163  nectar(self, cac
-000015f0: 6865 3d4e 6f6e 652c 2077 7364 6c3d 4e6f  he=None, wsdl=No
-00001600: 6e65 2c20 7072 6f78 793d 2222 2c20 7772  ne, proxy="", wr
-00001610: 6170 7065 723d 4e6f 6e65 2c20 6361 6365  apper=None, cace
-00001620: 7274 3d4e 6f6e 652c 2074 696d 656f 7574  rt=None, timeout
-00001630: 3d33 3029 3a0a 2020 2020 2020 2020 2320  =30):.        # 
-00001640: 436f 6e65 6374 6f20 7573 616e 646f 2065  Conecto usando e
-00001650: 6c20 6de9 746f 646f 2065 7374 616e 6461  l m.todo estanda
-00001660: 7264 3a0a 2020 2020 2020 2020 6f6b 203d  rd:.        ok =
-00001670: 2042 6173 6557 532e 436f 6e65 6374 6172   BaseWS.Conectar
-00001680: 2873 656c 662c 2063 6163 6865 2c20 7773  (self, cache, ws
-00001690: 646c 2c20 7072 6f78 792c 2077 7261 7070  dl, proxy, wrapp
-000016a0: 6572 2c20 6361 6365 7274 2c20 7469 6d65  er, cacert, time
-000016b0: 6f75 742c 0a20 2020 2020 2020 2020 2020  out,.           
-000016c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016d0: 2020 2073 6f61 705f 7365 7276 6572 3d22     soap_server="
-000016e0: 6a65 7474 7922 290a 2020 2020 2020 2020  jetty").        
-000016f0: 6966 206f 6b3a 0a20 2020 2020 2020 2020  if ok:.         
-00001700: 2020 2023 2073 6920 656c 2061 7263 6869     # si el archi
-00001710: 766f 2065 7320 6c6f 6361 6c2c 2061 7375  vo es local, asu
-00001720: 6d6f 2071 7565 2079 6120 6573 7461 2063  mo que ya esta c
-00001730: 6f72 7265 6769 646f 3a0a 2020 2020 2020  orregido:.      
-00001740: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00001750: 662e 7773 646c 2e73 7461 7274 7377 6974  f.wsdl.startswit
-00001760: 6828 2266 696c 6522 293a 0a20 2020 2020  h("file"):.     
-00001770: 2020 2020 2020 2020 2020 2023 2063 6f72             # cor
-00001780: 7269 6a6f 2075 6269 6361 6369 f36e 2064  rijo ubicaci.n d
-00001790: 656c 2073 6572 7669 646f 7220 286c 6f63  el servidor (loc
-000017a0: 616c 686f 7374 3a35 3930 3530 2065 6e20  alhost:59050 en 
-000017b0: 656c 2057 5344 4c29 0a20 2020 2020 2020  el WSDL).       
-000017c0: 2020 2020 2020 2020 206c 6f63 6174 696f           locatio
-000017d0: 6e20 3d20 7365 6c66 2e77 7364 6c5b 3a2d  n = self.wsdl[:-
-000017e0: 355d 0a20 2020 2020 2020 2020 2020 2020  5].             
-000017f0: 2020 2077 7320 3d20 7365 6c66 2e63 6c69     ws = self.cli
-00001800: 656e 742e 7365 7276 6963 6573 5b27 4957  ent.services['IW
-00001810: 6562 5365 7276 6963 6553 656e 6173 6127  ebServiceSenasa'
-00001820: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00001830: 2020 7773 5b27 706f 7274 7327 5d5b 2749    ws['ports']['I
-00001840: 5765 6253 6572 7669 6365 5365 6e61 7361  WebServiceSenasa
-00001850: 506f 7274 275d 5b27 6c6f 6361 7469 6f6e  Port']['location
-00001860: 275d 203d 206c 6f63 6174 696f 6e0a 0a20  '] = location.. 
-00001870: 2020 2020 2020 2020 2020 2023 2045 7374             # Est
-00001880: 6162 6c65 6365 7220 6372 6564 656e 6369  ablecer credenci
-00001890: 616c 6573 2064 6520 7365 6775 7269 6461  ales de segurida
-000018a0: 643a 0a20 2020 2020 2020 2020 2020 2073  d:.            s
-000018b0: 656c 662e 636c 6965 6e74 5b27 7773 7365  elf.client['wsse
-000018c0: 3a53 6563 7572 6974 7927 5d20 3d20 7b0a  :Security'] = {.
-000018d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018e0: 2777 7373 653a 5573 6572 6e61 6d65 546f  'wsse:UsernameTo
-000018f0: 6b65 6e27 3a20 7b0a 2020 2020 2020 2020  ken': {.        
-00001900: 2020 2020 2020 2020 2020 2020 2777 7373              'wss
-00001910: 653a 5573 6572 6e61 6d65 273a 2073 656c  e:Username': sel
-00001920: 662e 5573 6572 6e61 6d65 2c0a 2020 2020  f.Username,.    
-00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001940: 2777 7373 653a 5061 7373 776f 7264 273a  'wsse:Password':
-00001950: 2073 656c 662e 5061 7373 776f 7264 2c0a   self.Password,.
-00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001970: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00001980: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00001990: 7265 7475 726e 206f 6b0a 0a20 2020 2040  return ok..    @
-000019a0: 696e 6963 6961 6c69 7a61 725f 795f 6361  inicializar_y_ca
-000019b0: 7074 7572 6172 5f65 7863 6570 6369 6f6e  pturar_excepcion
-000019c0: 6573 0a20 2020 2064 6566 2053 6176 6554  es.    def SaveT
-000019d0: 7261 6e73 6163 6369 6f6e 2873 656c 662c  ransaccion(self,
-000019e0: 2075 7375 6172 696f 2c20 7061 7373 776f   usuario, passwo
-000019f0: 7264 2c0a 2020 2020 2020 2020 2020 2020  rd,.            
-00001a00: 2020 2020 2020 2020 2020 2020 676c 6e5f              gln_
-00001a10: 6f72 6967 656e 3d4e 6f6e 652c 2067 6c6e  origen=None, gln
-00001a20: 5f64 6573 7469 6e6f 3d4e 6f6e 652c 0a20  _destino=None,. 
-00001a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a40: 2020 2020 2020 2066 5f6f 7065 7261 6369         f_operaci
-00001a50: 6f6e 3d4e 6f6e 652c 2066 5f65 6c61 626f  on=None, f_elabo
-00001a60: 7261 6369 6f6e 3d4e 6f6e 652c 2066 5f76  racion=None, f_v
-00001a70: 746f 3d4e 6f6e 652c 0a20 2020 2020 2020  to=None,.       
-00001a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a90: 2069 645f 6576 656e 746f 3d4e 6f6e 652c   id_evento=None,
-00001aa0: 2063 6f64 5f70 726f 6475 6374 6f3d 4e6f   cod_producto=No
-00001ab0: 6e65 2c20 6e5f 6361 6e74 6964 6164 3d4e  ne, n_cantidad=N
-00001ac0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00001ad0: 2020 2020 2020 2020 2020 2020 206e 5f73               n_s
-00001ae0: 6572 6965 3d4e 6f6e 652c 206e 5f6c 6f74  erie=None, n_lot
-00001af0: 653d 4e6f 6e65 2c20 6e5f 6361 693d 4e6f  e=None, n_cai=No
-00001b00: 6e65 2c20 6e5f 6361 653d 4e6f 6e65 2c0a  ne, n_cae=None,.
-00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b20: 2020 2020 2020 2020 6964 5f6d 6f74 6976          id_motiv
-00001b30: 6f5f 6465 7374 7275 6363 696f 6e3d 4e6f  o_destruccion=No
-00001b40: 6e65 2c20 6e5f 6d61 6e69 6669 6573 746f  ne, n_manifiesto
-00001b50: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-00001b60: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00001b70: 6e5f 7472 616e 7370 6f72 7465 3d4e 6f6e  n_transporte=Non
-00001b80: 652c 206e 5f72 656d 6974 6f3d 4e6f 6e65  e, n_remito=None
-00001b90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001ba0: 2020 2020 2020 2020 2020 6d6f 7469 766f            motivo
-00001bb0: 5f64 6576 6f6c 7563 696f 6e3d 4e6f 6e65  _devolucion=None
-00001bc0: 2c20 6f62 7365 7276 6163 696f 6e65 733d  , observaciones=
-00001bd0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00001be0: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
-00001bf0: 7661 6c65 5f63 6f6d 7072 613d 4e6f 6e65  vale_compra=None
-00001c00: 2c20 6170 656c 6c69 646f 4e6f 6d62 7265  , apellidoNombre
-00001c10: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-00001c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c30: 6469 7265 6363 696f 6e3d 4e6f 6e65 2c20  direccion=None, 
-00001c40: 6e75 6d65 726f 3d4e 6f6e 652c 206c 6f63  numero=None, loc
-00001c50: 616c 6964 6164 3d4e 6f6e 652c 0a20 2020  alidad=None,.   
-00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c70: 2020 2020 2070 726f 7669 6e63 6961 3d4e       provincia=N
-00001c80: 6f6e 652c 206e 5f70 6f73 7461 6c3d 4e6f  one, n_postal=No
-00001c90: 6e65 2c20 6375 6974 3d4e 6f6e 650a 2020  ne, cuit=None.  
-00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cb0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
-00001cc0: 2020 2252 6561 6c69 7a61 2065 6c20 7265    "Realiza el re
-00001cd0: 6769 7374 726f 2064 6520 756e 6120 7472  gistro de una tr
-00001ce0: 616e 7361 6363 69f3 6e20 6465 2070 726f  ansacci.n de pro
-00001cf0: 6475 6374 6f73 2066 6974 6f73 616e 6974  ductos fitosanit
-00001d00: 6172 696f 732e 2022 0a20 2020 2020 2020  arios. ".       
-00001d10: 2023 2063 7265 6f20 6c6f 7320 7061 72e1   # creo los par.
-00001d20: 6d65 7472 6f73 2070 6172 6120 6573 7461  metros para esta
-00001d30: 206c 6c61 6d61 6461 0a20 2020 2020 2020   llamada.       
-00001d40: 2070 6172 616d 7320 3d20 7b20 2027 676c   params = {  'gl
-00001d50: 6e5f 6f72 6967 656e 273a 2067 6c6e 5f6f  n_origen': gln_o
-00001d60: 7269 6765 6e2c 0a20 2020 2020 2020 2020  rigen,.         
-00001d70: 2020 2020 2020 2020 2020 2027 676c 6e5f             'gln_
-00001d80: 6465 7374 696e 6f27 3a20 676c 6e5f 6465  destino': gln_de
-00001d90: 7374 696e 6f2c 0a20 2020 2020 2020 2020  stino,.         
-00001da0: 2020 2020 2020 2020 2020 2027 665f 6f70             'f_op
-00001db0: 6572 6163 696f 6e27 3a20 665f 6f70 6572  eracion': f_oper
-00001dc0: 6163 696f 6e2c 0a20 2020 2020 2020 2020  acion,.         
-00001dd0: 2020 2020 2020 2020 2020 2027 665f 656c             'f_el
-00001de0: 6162 6f72 6163 696f 6e27 3a20 665f 656c  aboracion': f_el
-00001df0: 6162 6f72 6163 696f 6e2c 0a20 2020 2020  aboracion,.     
-00001e00: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001e10: 665f 7674 6f27 3a20 665f 7674 6f2c 0a20  f_vto': f_vto,. 
-00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e30: 2020 2027 6964 5f65 7665 6e74 6f27 3a20     'id_evento': 
-00001e40: 6964 5f65 7665 6e74 6f2c 0a20 2020 2020  id_evento,.     
-00001e50: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001e60: 636f 645f 7072 6f64 7563 746f 273a 2063  cod_producto': c
-00001e70: 6f64 5f70 726f 6475 6374 6f2c 0a20 2020  od_producto,.   
-00001e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e90: 2027 6e5f 6361 6e74 6964 6164 273a 206e   'n_cantidad': n
-00001ea0: 5f63 616e 7469 6461 642c 0a20 2020 2020  _cantidad,.     
-00001eb0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001ec0: 6e5f 7365 7269 6527 3a20 6e5f 7365 7269  n_serie': n_seri
-00001ed0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00001ee0: 2020 2020 2020 2027 6e5f 6c6f 7465 273a         'n_lote':
-00001ef0: 206e 5f6c 6f74 652c 0a20 2020 2020 2020   n_lote,.       
-00001f00: 2020 2020 2020 2020 2020 2020 2027 6e5f               'n_
-00001f10: 6361 6927 3a20 6e5f 6361 6920 6f72 204e  cai': n_cai or N
-00001f20: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00001f30: 2020 2020 2020 2020 2027 6e5f 6361 6527           'n_cae'
-00001f40: 3a20 6e5f 6361 6520 6f72 204e 6f6e 652c  : n_cae or None,
-00001f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001f60: 2020 2020 2027 6964 5f6d 6f74 6976 6f5f       'id_motivo_
-00001f70: 6465 7374 7275 6363 696f 6e27 3a20 6964  destruccion': id
+00000010: 6e0a 2320 2d2a 2d20 636f 6469 6e67 3a20  n.# -*- coding: 
+00000020: 7574 662d 3820 2d2a 2d0a 2320 5468 6973  utf-8 -*-.# This
+00000030: 2070 726f 6772 616d 2069 7320 6672 6565   program is free
+00000040: 2073 6f66 7477 6172 653b 2079 6f75 2063   software; you c
+00000050: 616e 2072 6564 6973 7472 6962 7574 6520  an redistribute 
+00000060: 6974 2061 6e64 2f6f 7220 6d6f 6469 6679  it and/or modify
+00000070: 0a23 2069 7420 756e 6465 7220 7468 6520  .# it under the 
+00000080: 7465 726d 7320 6f66 2074 6865 2047 4e55  terms of the GNU
+00000090: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
+000000a0: 4c69 6365 6e73 6520 6173 2070 7562 6c69  License as publi
+000000b0: 7368 6564 2062 7920 7468 650a 2320 4672  shed by the.# Fr
+000000c0: 6565 2053 6f66 7477 6172 6520 466f 756e  ee Software Foun
+000000d0: 6461 7469 6f6e 3b20 6569 7468 6572 2076  dation; either v
+000000e0: 6572 7369 6f6e 2033 2c20 6f72 2028 6174  ersion 3, or (at
+000000f0: 2079 6f75 7220 6f70 7469 6f6e 2920 616e   your option) an
+00000100: 7920 6c61 7465 720a 2320 7665 7273 696f  y later.# versio
+00000110: 6e2e 0a23 0a23 2054 6869 7320 7072 6f67  n..#.# This prog
+00000120: 7261 6d20 6973 2064 6973 7472 6962 7574  ram is distribut
+00000130: 6564 2069 6e20 7468 6520 686f 7065 2074  ed in the hope t
+00000140: 6861 7420 6974 2077 696c 6c20 6265 2075  hat it will be u
+00000150: 7365 6675 6c2c 2062 7574 0a23 2057 4954  seful, but.# WIT
+00000160: 484f 5554 2041 4e59 2057 4152 5241 4e54  HOUT ANY WARRANT
+00000170: 593b 2077 6974 686f 7574 2065 7665 6e20  Y; without even 
+00000180: 7468 6520 696d 706c 6965 6420 7761 7272  the implied warr
+00000190: 616e 7479 206f 6620 4d45 5243 4841 4e54  anty of MERCHANT
+000001a0: 4942 494c 4954 590a 2320 6f72 2046 4954  IBILITY.# or FIT
+000001b0: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
+000001c0: 4355 4c41 5220 5055 5250 4f53 452e 2020  CULAR PURPOSE.  
+000001d0: 5365 6520 7468 6520 474e 5520 4765 6e65  See the GNU Gene
+000001e0: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
+000001f0: 7365 0a23 2066 6f72 206d 6f72 6520 6465  se.# for more de
+00000200: 7461 696c 732e 0a0a 224d f364 756c 6f20  tails..."M.dulo 
+00000210: 5472 617a 6162 696c 6964 6164 2064 6520  Trazabilidad de 
+00000220: 5072 6f64 7563 746f 7320 5665 7465 7269  Productos Veteri
+00000230: 6e61 7269 6f73 2053 454e 4153 4120 5265  narios SENASA Re
+00000240: 736f 6c75 6369 f36e 2033 3639 2f32 3031  soluci.n 369/201
+00000250: 3322 0a0a 2320 496e 666f 726d 6163 69f3  3"..# Informaci.
+00000260: 6e20 6164 6963 696f 6e61 6c20 7920 646f  n adicional y do
+00000270: 6375 6d65 6e74 6163 69f3 6e3a 0a23 2068  cumentaci.n:.# h
+00000280: 7474 703a 2f2f 7777 772e 7369 7374 656d  ttp://www.sistem
+00000290: 6173 6167 696c 6573 2e63 6f6d 2e61 722f  asagiles.com.ar/
+000002a0: 7472 6163 2f77 696b 692f 5472 617a 6162  trac/wiki/Trazab
+000002b0: 696c 6964 6164 5072 6f64 7563 746f 7356  ilidadProductosV
+000002c0: 6574 6572 696e 6172 696f 730a 0a5f 5f61  eterinarios..__a
+000002d0: 7574 686f 725f 5f20 3d20 224d 6172 6961  uthor__ = "Maria
+000002e0: 6e6f 2052 6569 6e67 6172 7420 3c72 6569  no Reingart <rei
+000002f0: 6e67 6172 7440 676d 6169 6c2e 636f 6d3e  ngart@gmail.com>
+00000300: 220a 5f5f 636f 7079 7269 6768 745f 5f20  ".__copyright__ 
+00000310: 3d20 2243 6f70 7972 6967 6874 2028 4329  = "Copyright (C)
+00000320: 2032 3031 3420 4d61 7269 616e 6f20 5265   2014 Mariano Re
+00000330: 696e 6761 7274 220a 5f5f 6c69 6365 6e73  ingart".__licens
+00000340: 655f 5f20 3d20 2247 504c 2033 2e30 2b22  e__ = "GPL 3.0+"
+00000350: 0a5f 5f76 6572 7369 6f6e 5f5f 203d 2022  .__version__ = "
+00000360: 312e 3131 6422 0a0a 2320 6874 7470 3a2f  1.11d"..# http:/
+00000370: 2f73 656e 6173 612e 7365 7276 6963 696f  /senasa.servicio
+00000380: 732e 7061 6d69 2e6f 7267 2e61 722f 0a0a  s.pami.org.ar/..
+00000390: 696d 706f 7274 206f 730a 696d 706f 7274  import os.import
+000003a0: 2073 6f63 6b65 740a 696d 706f 7274 2073   socket.import s
+000003b0: 7973 0a69 6d70 6f72 7420 6461 7465 7469  ys.import dateti
+000003c0: 6d65 2c20 7469 6d65 0a69 6d70 6f72 7420  me, time.import 
+000003d0: 7472 6163 6562 6163 6b0a 696d 706f 7274  traceback.import
+000003e0: 2070 7933 7369 6d70 6c65 736f 6170 2e63   py3simplesoap.c
+000003f0: 6c69 656e 740a 6672 6f6d 2070 7933 7369  lient.from py3si
+00000400: 6d70 6c65 736f 6170 2e63 6c69 656e 7420  mplesoap.client 
+00000410: 696d 706f 7274 2053 6f61 7043 6c69 656e  import SoapClien
+00000420: 742c 2053 6f61 7046 6175 6c74 2c20 7061  t, SoapFault, pa
+00000430: 7273 655f 7072 6f78 792c 205c 0a20 2020  rse_proxy, \.   
+00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000450: 2020 2020 2020 2020 2020 2020 2073 6574               set
+00000460: 5f68 7474 705f 7772 6170 7065 720a 6672  _http_wrapper.fr
+00000470: 6f6d 2070 7933 7369 6d70 6c65 736f 6170  om py3simplesoap
+00000480: 2e73 696d 706c 6578 6d6c 2069 6d70 6f72  .simplexml impor
+00000490: 7420 5369 6d70 6c65 584d 4c45 6c65 6d65  t SimpleXMLEleme
+000004a0: 6e74 0a66 726f 6d20 6353 7472 696e 6749  nt.from cStringI
+000004b0: 4f20 696d 706f 7274 2053 7472 696e 6749  O import StringI
+000004c0: 4f0a 0a23 2069 6d70 6f72 746f 2066 756e  O..# importo fun
+000004d0: 6369 6f6e 6573 2063 6f6d 7061 7274 6964  ciones compartid
+000004e0: 6173 3a0a 6672 6f6d 202e 7574 696c 7320  as:.from .utils 
+000004f0: 696d 706f 7274 206c 6565 722c 2065 7363  import leer, esc
+00000500: 7269 6269 722c 206c 6565 725f 6462 662c  ribir, leer_dbf,
+00000510: 2067 7561 7264 6172 5f64 6266 2c20 4e2c   guardar_dbf, N,
+00000520: 2041 2c20 492c 206a 736f 6e2c 205c 0a20   A, I, json, \. 
+00000530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000540: 2064 6172 5f6e 6f6d 6272 655f 6361 6d70   dar_nombre_camp
+00000550: 6f5f 6462 662c 2067 6574 5f69 6e73 7461  o_dbf, get_insta
+00000560: 6c6c 5f64 6972 2c20 4261 7365 5753 2c20  ll_dir, BaseWS, 
+00000570: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
+00000580: 2020 2020 696e 6963 6961 6c69 7a61 725f      inicializar_
+00000590: 795f 6361 7074 7572 6172 5f65 7863 6570  y_capturar_excep
+000005a0: 6369 6f6e 6573 0a0a 484f 4d4f 203d 2054  ciones..HOMO = T
+000005b0: 7275 650a 5459 5045 4c49 4220 3d20 4661  rue.TYPELIB = Fa
+000005c0: 6c73 650a 0a57 5344 4c20 3d20 2268 7474  lse..WSDL = "htt
+000005d0: 7073 3a2f 2f73 6572 7669 6369 6f73 2e70  ps://servicios.p
+000005e0: 616d 692e 6f72 672e 6172 2f74 7261 7a61  ami.org.ar/traza
+000005f0: 656e 7665 742e 5765 6253 6572 7669 6365  envet.WebService
+00000600: 3f77 7364 6c22 0a4c 4f43 4154 494f 4e20  ?wsdl".LOCATION 
+00000610: 3d20 2268 7474 7073 3a2f 2f73 6572 7669  = "https://servi
+00000620: 6369 6f73 2e70 616d 692e 6f72 672e 6172  cios.pami.org.ar
+00000630: 2f74 7261 7a61 656e 7665 742e 5765 6253  /trazaenvet.WebS
+00000640: 6572 7669 6365 3f77 7364 6c22 0a0a 2320  ervice?wsdl"..# 
+00000650: 466f 726d 6174 6f20 6465 2054 7261 6e73  Formato de Trans
+00000660: 6163 6369 6f6e 5365 6e61 7361 4454 4f20  accionSenasaDTO 
+00000670: 2853 6176 6554 7261 6e73 6163 6369 6f6e  (SaveTransaccion
+00000680: 290a 5452 414e 5341 4343 494f 4e5f 4454  ).TRANSACCION_DT
+00000690: 4f20 3d20 5b0a 2020 2020 2827 676c 6e5f  O = [.    ('gln_
+000006a0: 6f72 6967 656e 272c 2031 332c 2041 292c  origen', 13, A),
+000006b0: 0a20 2020 2028 2767 6c6e 5f64 6573 7469  .    ('gln_desti
+000006c0: 6e6f 272c 2031 332c 2041 292c 0a20 2020  no', 13, A),.   
+000006d0: 2028 2766 5f6f 7065 7261 6369 6f6e 272c   ('f_operacion',
+000006e0: 2031 302c 2041 292c 0a20 2020 2028 2766   10, A),.    ('f
+000006f0: 5f65 6c61 626f 7261 6369 6f6e 272c 2031  _elaboracion', 1
+00000700: 302c 2041 292c 0a20 2020 2028 2766 5f76  0, A),.    ('f_v
+00000710: 746f 272c 2031 302c 2041 292c 0a20 2020  to', 10, A),.   
+00000720: 2028 2769 645f 6576 656e 746f 272c 2031   ('id_evento', 1
+00000730: 352c 204e 292c 0a20 2020 2028 2763 6f64  5, N),.    ('cod
+00000740: 5f70 726f 6475 6374 6f27 2c20 3134 2c20  _producto', 14, 
+00000750: 4129 2c0a 2020 2020 2827 6e5f 6361 6e74  A),.    ('n_cant
+00000760: 6964 6164 272c 2033 302c 204e 292c 0a20  idad', 30, N),. 
+00000770: 2020 2028 276e 5f73 6572 6965 272c 2032     ('n_serie', 2
+00000780: 302c 2041 292c 0a20 2020 2028 276e 5f6c  0, A),.    ('n_l
+00000790: 6f74 6527 2c20 3530 2c20 4129 2c0a 2020  ote', 50, A),.  
+000007a0: 2020 2827 6e5f 6361 6927 2c20 3135 2c20    ('n_cai', 15, 
+000007b0: 4129 2c0a 2020 2020 2827 6e5f 6361 6527  A),.    ('n_cae'
+000007c0: 2c20 3135 2c20 4129 2c0a 2020 2020 2827  , 15, A),.    ('
+000007d0: 6964 5f6d 6f74 6976 6f5f 6465 7374 7275  id_motivo_destru
+000007e0: 6363 696f 6e27 2c20 352c 2041 292c 0a20  ccion', 5, A),. 
+000007f0: 2020 2028 276e 5f6d 616e 6966 6965 7374     ('n_manifiest
+00000800: 6f27 2c20 3135 2c20 4e29 2c0a 2020 2020  o', 15, N),.    
+00000810: 2827 656e 5f74 7261 6e73 706f 7274 6527  ('en_transporte'
+00000820: 2c20 312c 2041 292c 2023 2062 6f6f 6c65  , 1, A), # boole
+00000830: 616e 0a20 2020 2028 276e 5f72 656d 6974  an.    ('n_remit
+00000840: 6f27 2c20 3135 2c20 4129 2c0a 2020 2020  o', 15, A),.    
+00000850: 2827 6d6f 7469 766f 5f64 6576 6f6c 7563  ('motivo_devoluc
+00000860: 696f 6e27 2c20 3130 302c 2041 292c 0a20  ion', 100, A),. 
+00000870: 2020 2028 276f 6273 6572 7661 6369 6f6e     ('observacion
+00000880: 6573 272c 2031 3030 302c 2041 292c 0a20  es', 1000, A),. 
+00000890: 2020 2028 276e 5f76 616c 655f 636f 6d70     ('n_vale_comp
+000008a0: 7261 272c 2031 352c 2041 292c 0a20 2020  ra', 15, A),.   
+000008b0: 2028 2761 7065 6c6c 6964 6f4e 6f6d 6272   ('apellidoNombr
+000008c0: 6573 272c 2032 3535 2c20 4129 2c0a 2020  es', 255, A),.  
+000008d0: 2020 2827 6469 7265 6363 696f 6e27 2c20    ('direccion', 
+000008e0: 3230 302c 2041 292c 0a20 2020 2028 276e  200, A),.    ('n
+000008f0: 756d 6572 6f27 2c20 362c 204e 292c 0a20  umero', 6, N),. 
+00000900: 2020 2028 276c 6f63 616c 6964 6164 272c     ('localidad',
+00000910: 2031 352c 2041 292c 0a20 2020 2028 2770   15, A),.    ('p
+00000920: 726f 7669 6e63 6961 272c 2031 352c 2041  rovincia', 15, A
+00000930: 292c 0a20 2020 2028 276e 5f70 6f73 7461  ),.    ('n_posta
+00000940: 6c27 2c20 382c 2041 292c 0a20 2020 2028  l', 8, A),.    (
+00000950: 2763 7569 7427 2c20 3131 2c20 4129 2c0a  'cuit', 11, A),.
+00000960: 2020 2020 2827 636f 6469 676f 5f74 7261      ('codigo_tra
+00000970: 6e73 6163 6369 6f6e 272c 2031 342c 2041  nsaccion', 14, A
+00000980: 292c 0a5d 0a0a 2320 466f 726d 6174 6f20  ),.]..# Formato 
+00000990: 7061 7261 2054 7261 6e73 6163 6369 6f6e  para Transaccion
+000009a0: 5365 6e61 7361 2028 6765 7454 7261 6e73  Senasa (getTrans
+000009b0: 6163 6369 6f6e 6573 290a 5452 414e 5341  acciones).TRANSA
+000009c0: 4343 494f 4e45 5320 3d20 5b0a 2020 2020  CCIONES = [.    
+000009d0: 2827 6964 5f74 7261 6e73 6163 6369 6f6e  ('id_transaccion
+000009e0: 5f67 6c6f 6261 6c27 2c20 3135 2c20 4e29  _global', 15, N)
+000009f0: 2c0a 2020 2020 2827 6964 5f74 7261 6e73  ,.    ('id_trans
+00000a00: 6163 6369 6f6e 272c 2031 352c 204e 292c  accion', 15, N),
+00000a10: 0a20 2020 2028 2766 5f74 7261 6e73 6163  .    ('f_transac
+00000a20: 6369 6f6e 272c 2031 302c 2041 292c 0a20  cion', 10, A),. 
+00000a30: 2020 2028 2766 5f6f 7065 7261 6369 6f6e     ('f_operacion
+00000a40: 272c 2031 302c 2041 292c 0a20 2020 2028  ', 10, A),.    (
+00000a50: 2766 5f76 656e 6369 6d69 656e 746f 272c  'f_vencimiento',
+00000a60: 2031 302c 2041 292c 0a20 2020 2028 2766   10, A),.    ('f
+00000a70: 5f65 6c61 626f 7261 6369 6f6e 272c 2031  _elaboracion', 1
+00000a80: 302c 2041 292c 0a20 2020 2028 2764 5f65  0, A),.    ('d_e
+00000a90: 7665 6e74 6f27 2c20 3130 302c 2041 292c  vento', 100, A),
+00000aa0: 0a20 2020 2028 276e 5f63 616e 7469 6461  .    ('n_cantida
+00000ab0: 6427 2c20 3330 2c20 4e29 2c0a 2020 2020  d', 30, N),.    
+00000ac0: 2827 6964 5f75 6e69 6461 6427 2c20 3135  ('id_unidad', 15
+00000ad0: 2c20 4e29 2c0a 2020 2020 2827 645f 756e  , N),.    ('d_un
+00000ae0: 6964 6164 272c 2031 3030 2c20 4129 2c0a  idad', 100, A),.
+00000af0: 2020 2020 2827 636f 645f 7072 6f64 7563      ('cod_produc
+00000b00: 746f 272c 2031 342c 2041 292c 0a20 2020  to', 14, A),.   
+00000b10: 2028 2769 645f 756e 6964 6164 272c 2031   ('id_unidad', 1
+00000b20: 352c 204e 292c 0a20 2020 2028 276e 5f73  5, N),.    ('n_s
+00000b30: 6572 6965 272c 2032 302c 2041 292c 0a20  erie', 20, A),. 
+00000b40: 2020 2028 276e 5f6c 6f74 6527 2c20 3530     ('n_lote', 50
+00000b50: 2c20 4129 2c0a 2020 2020 2827 6e5f 6361  , A),.    ('n_ca
+00000b60: 6927 2c20 3135 2c20 4129 2c0a 2020 2020  i', 15, A),.    
+00000b70: 2827 6e5f 6361 6527 2c20 3135 2c20 4129  ('n_cae', 15, A)
+00000b80: 2c0a 2020 2020 2827 645f 6d6f 7469 766f  ,.    ('d_motivo
+00000b90: 5f64 6573 7472 7563 6369 6f6e 272c 2035  _destruccion', 5
+00000ba0: 302c 2041 292c 0a20 2020 2028 2764 5f6d  0, A),.    ('d_m
+00000bb0: 616e 6966 6965 7374 6f27 2c20 3135 2c20  anifiesto', 15, 
+00000bc0: 4129 2c0a 2020 2020 2827 656e 5f74 7261  A),.    ('en_tra
+00000bd0: 6e73 706f 7274 6527 2c20 312c 2041 292c  nsporte', 1, A),
+00000be0: 0a20 2020 2028 276e 5f72 656d 6974 6f27  .    ('n_remito'
+00000bf0: 2c20 3330 2c20 4129 2c0a 2020 2020 2827  , 30, A),.    ('
+00000c00: 6d6f 7469 766f 5f64 6576 6f6c 7563 696f  motivo_devolucio
+00000c10: 6e27 2c20 3230 302c 2041 292c 0a20 2020  n', 200, A),.   
+00000c20: 2028 276f 6273 6572 7661 6369 6f6e 6573   ('observaciones
+00000c30: 272c 2031 3030 302c 2041 292c 0a20 2020  ', 1000, A),.   
+00000c40: 2028 276e 5f76 616c 655f 636f 6d70 7261   ('n_vale_compra
+00000c50: 272c 2031 352c 2041 292c 0a20 2020 2028  ', 15, A),.    (
+00000c60: 2761 7065 6c6c 6964 6f4e 6f6d 6272 6573  'apellidoNombres
+00000c70: 272c 2032 3535 2c20 4129 2c0a 2020 2020  ', 255, A),.    
+00000c80: 2827 6469 7265 6363 696f 6e27 2c20 3230  ('direccion', 20
+00000c90: 302c 2041 292c 0a20 2020 2028 276e 756d  0, A),.    ('num
+00000ca0: 6572 6f27 2c20 362c 2041 292c 0a20 2020  ero', 6, A),.   
+00000cb0: 2028 276c 6f63 616c 6964 6164 272c 2032   ('localidad', 2
+00000cc0: 3530 2c20 4129 2c0a 2020 2020 2827 7072  50, A),.    ('pr
+00000cd0: 6f76 696e 6369 6127 2c20 3235 302c 2041  ovincia', 250, A
+00000ce0: 292c 0a20 2020 2028 276e 5f70 6f73 7461  ),.    ('n_posta
+00000cf0: 6c27 2c20 382c 2041 292c 0a20 2020 2028  l', 8, A),.    (
+00000d00: 2763 7569 7427 2c20 3131 2c20 4129 2c0a  'cuit', 11, A),.
+00000d10: 2020 2020 2827 645f 6167 656e 7465 5f69      ('d_agente_i
+00000d20: 6e66 6f72 6d61 646f 7227 2c20 3235 352c  nformador', 255,
+00000d30: 2041 292c 0a20 2020 2028 2764 5f61 6765   A),.    ('d_age
+00000d40: 6e74 655f 6f72 6967 656e 272c 2032 3535  nte_origen', 255
+00000d50: 2c20 4129 2c0a 2020 2020 2827 645f 6167  , A),.    ('d_ag
+00000d60: 656e 7465 5f64 6573 7469 6e6f 272c 2032  ente_destino', 2
+00000d70: 3535 2c20 4129 2c0a 2020 2020 2827 645f  55, A),.    ('d_
+00000d80: 7072 6f64 7563 746f 272c 2032 3530 2c20  producto', 250, 
+00000d90: 4129 2c0a 2020 2020 2827 645f 6573 7461  A),.    ('d_esta
+00000da0: 646f 5f74 7261 6e73 6163 6369 6f6e 272c  do_transaccion',
+00000db0: 2033 302c 2041 292c 0a20 2020 2028 2764   30, A),.    ('d
+00000dc0: 5f74 6970 6f5f 7472 616e 7361 6363 696f  _tipo_transaccio
+00000dd0: 6e27 2c20 3330 2c20 4129 2c0a 5d0a 0a23  n', 30, A),.]..#
+00000de0: 2046 6f72 6d61 746f 2070 6172 6120 4572   Formato para Er
+00000df0: 726f 7265 730a 4552 524f 5245 5320 3d20  rores.ERRORES = 
+00000e00: 5b0a 2020 2020 2827 5f63 5f65 7272 6f72  [.    ('_c_error
+00000e10: 272c 2034 2c20 4129 2c20 2020 2020 2020  ', 4, A),       
+00000e20: 2020 2020 2020 2020 2020 2320 63f3 6469            # c.di
+00000e30: 676f 0a20 2020 2028 275f 645f 6572 726f  go.    ('_d_erro
+00000e40: 7227 2c20 3235 302c 2041 292c 2020 2020  r', 250, A),    
+00000e50: 2020 2020 2020 2020 2020 2023 2064 6573             # des
+00000e60: 6372 6970 6369 f36e 0a20 2020 205d 0a0a  cripci.n.    ]..
+00000e70: 0a63 6c61 7373 2054 7261 7a61 5665 7428  .class TrazaVet(
+00000e80: 4261 7365 5753 293a 0a20 2020 2022 496e  BaseWS):.    "In
+00000e90: 7465 7266 617a 2070 6172 6120 656c 2057  terfaz para el W
+00000ea0: 6562 5365 7276 6963 6520 6465 2054 7261  ebService de Tra
+00000eb0: 7a61 6269 6c69 6461 6420 6465 2056 6574  zabilidad de Vet
+00000ec0: 6572 696e 6172 696f 7320 5345 4e41 5341  erinarios SENASA
+00000ed0: 220a 0a20 2020 205f 7075 626c 6963 5f6d  "..    _public_m
+00000ee0: 6574 686f 6473 5f20 3d20 5b27 5361 7665  ethods_ = ['Save
+00000ef0: 5472 616e 7361 6363 696f 6e27 2c20 2753  Transaccion', 'S
+00000f00: 656e 6443 616e 6365 6c61 5472 616e 7361  endCancelaTransa
+00000f10: 6327 2c0a 2020 2020 2020 2020 2020 2020  c',.            
+00000f20: 2020 2020 2020 2020 2020 2020 2753 656e              'Sen
+00000f30: 6443 6f6e 6669 726d 6154 7261 6e73 6163  dConfirmaTransac
+00000f40: 6327 2c20 2753 656e 6441 6c65 7274 6154  c', 'SendAlertaT
+00000f50: 7261 6e73 6163 6327 2c0a 2020 2020 2020  ransacc',.      
+00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f70: 2020 2747 6574 5472 616e 7361 6363 696f    'GetTransaccio
+00000f80: 6e65 7327 2c0a 2020 2020 2020 2020 2020  nes',.          
+00000f90: 2020 2020 2020 2020 2020 2020 2020 2743                'C
+00000fa0: 6f6e 6563 7461 7227 2c20 274c 6565 7245  onectar', 'LeerE
+00000fb0: 7272 6f72 272c 2027 4c65 6572 5472 616e  rror', 'LeerTran
+00000fc0: 7361 6363 696f 6e27 2c0a 2020 2020 2020  saccion',.      
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fe0: 2020 2753 6574 5573 6572 6e61 6d65 272c    'SetUsername',
+00000ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001000: 2020 2020 2020 2020 2027 5365 7450 6172           'SetPar
+00001010: 616d 6574 726f 272c 2027 4765 7450 6172  ametro', 'GetPar
+00001020: 616d 6574 726f 272c 0a20 2020 2020 2020  ametro',.       
+00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001040: 2027 4765 7443 6f64 6967 6f54 7261 6e73   'GetCodigoTrans
+00001050: 6163 6369 6f6e 272c 2027 4765 7452 6573  accion', 'GetRes
+00001060: 756c 7461 646f 272c 2027 4c6f 6164 5465  ultado', 'LoadTe
+00001070: 7374 584d 4c27 5d0a 0a20 2020 205f 7075  stXML']..    _pu
+00001080: 626c 6963 5f61 7474 7273 5f20 3d20 5b0a  blic_attrs_ = [.
+00001090: 2020 2020 2020 2020 2755 7365 726e 616d          'Usernam
+000010a0: 6527 2c20 2750 6173 7377 6f72 6427 2c0a  e', 'Password',.
+000010b0: 2020 2020 2020 2020 2743 6f64 6967 6f54          'CodigoT
+000010c0: 7261 6e73 6163 6369 6f6e 272c 2027 4572  ransaccion', 'Er
+000010d0: 726f 7265 7327 2c20 2752 6573 756c 7461  rores', 'Resulta
+000010e0: 646f 272c 0a20 2020 2020 2020 2027 586d  do',.        'Xm
+000010f0: 6c52 6571 7565 7374 272c 2027 586d 6c52  lRequest', 'XmlR
+00001100: 6573 706f 6e73 6527 2c0a 2020 2020 2020  esponse',.      
+00001110: 2020 2756 6572 7369 6f6e 272c 2027 496e    'Version', 'In
+00001120: 7374 616c 6c44 6972 272c 0a20 2020 2020  stallDir',.     
+00001130: 2020 2027 5472 6163 6562 6163 6b27 2c20     'Traceback', 
+00001140: 2745 7863 6570 6369 6f6e 272c 0a20 2020  'Excepcion',.   
+00001150: 2020 2020 2027 4361 6e74 5061 6769 6e61       'CantPagina
+00001160: 7327 2c20 2748 6179 4572 726f 7227 2c20  s', 'HayError', 
+00001170: 2754 7261 6e73 6163 6369 6f6e 5365 6e61  'TransaccionSena
+00001180: 7361 272c 0a20 2020 2020 2020 205d 0a0a  sa',.        ]..
+00001190: 2020 2020 5f72 6567 5f70 726f 6769 645f      _reg_progid_
+000011a0: 203d 2022 5472 617a 6156 6574 220a 2020   = "TrazaVet".  
+000011b0: 2020 5f72 6567 5f63 6c73 6964 5f20 3d20    _reg_clsid_ = 
+000011c0: 227b 3245 3238 4437 3944 2d32 3342 302d  "{2E28D79D-23B0-
+000011d0: 3443 3145 2d38 3542 392d 3634 4244 4334  4C1E-85B9-64BDC4
+000011e0: 3142 3846 4346 7d22 0a0a 2020 2020 2320  1B8FCF}"..    # 
+000011f0: 5661 7269 6162 6c65 7320 676c 6f62 616c  Variables global
+00001200: 6573 2070 6172 6120 4261 7365 5753 3a0a  es para BaseWS:.
+00001210: 2020 2020 484f 4d4f 203d 2048 4f4d 4f0a      HOMO = HOMO.
+00001220: 2020 2020 5753 444c 203d 2057 5344 4c0a      WSDL = WSDL.
+00001230: 2020 2020 5665 7273 696f 6e20 3d20 2225      Version = "%
+00001240: 7320 2573 2025 7322 2025 2028 5f5f 7665  s %s %s" % (__ve
+00001250: 7273 696f 6e5f 5f2c 2048 4f4d 4f20 616e  rsion__, HOMO an
+00001260: 6420 2748 6f6d 6f6c 6f67 6163 69f3 6e27  d 'Homologaci.n'
+00001270: 206f 7220 2727 2c0a 2020 2020 2020 2020   or '',.        
+00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001290: 2020 2020 7079 3373 696d 706c 6573 6f61      py3simplesoa
+000012a0: 702e 636c 6965 6e74 2e5f 5f76 6572 7369  p.client.__versi
+000012b0: 6f6e 5f5f 290a 0a20 2020 2064 6566 205f  on__)..    def _
+000012c0: 5f69 6e69 745f 5f28 7365 6c66 2c20 7265  _init__(self, re
+000012d0: 696e 7465 6e74 6f73 3d31 293a 0a20 2020  intentos=1):.   
+000012e0: 2020 2020 2073 656c 662e 5573 6572 6e61       self.Userna
+000012f0: 6d65 203d 2073 656c 662e 5061 7373 776f  me = self.Passwo
+00001300: 7264 203d 204e 6f6e 650a 2020 2020 2020  rd = None.      
+00001310: 2020 7365 6c66 2e54 7261 6e73 6163 6369    self.Transacci
+00001320: 6f6e 5365 6e61 7361 203d 205b 5d0a 2020  onSenasa = [].  
+00001330: 2020 2020 2020 4261 7365 5753 2e5f 5f69        BaseWS.__i
+00001340: 6e69 745f 5f28 7365 6c66 2c20 7265 696e  nit__(self, rein
+00001350: 7465 6e74 6f73 290a 0a20 2020 2064 6566  tentos)..    def
+00001360: 2069 6e69 6369 616c 697a 6172 2873 656c   inicializar(sel
+00001370: 6629 3a0a 2020 2020 2020 2020 4261 7365  f):.        Base
+00001380: 5753 2e69 6e69 6369 616c 697a 6172 2873  WS.inicializar(s
+00001390: 656c 6629 0a20 2020 2020 2020 2073 656c  elf).        sel
+000013a0: 662e 436f 6469 676f 5472 616e 7361 6363  f.CodigoTransacc
+000013b0: 696f 6e20 3d20 7365 6c66 2e45 7272 6f72  ion = self.Error
+000013c0: 6573 203d 2073 656c 662e 5265 7375 6c74  es = self.Result
+000013d0: 6164 6f20 3d20 4e6f 6e65 0a20 2020 2020  ado = None.     
+000013e0: 2020 2073 656c 662e 5265 7375 6c74 6164     self.Resultad
+000013f0: 6f20 3d20 2727 0a20 2020 2020 2020 2073  o = ''.        s
+00001400: 656c 662e 4572 726f 7265 7320 3d20 5b5d  elf.Errores = []
+00001410: 2020 2023 206c 6973 7461 2064 6520 7374     # lista de st
+00001420: 7269 6e67 7320 7061 7261 206c 6120 696e  rings para la in
+00001430: 7465 7266 617a 0a20 2020 2020 2020 2073  terfaz.        s
+00001440: 656c 662e 6572 726f 7265 7320 3d20 5b5d  elf.errores = []
+00001450: 2020 2023 206c 6973 7461 2064 6520 6469     # lista de di
+00001460: 6363 696f 6e61 7269 6f73 2028 7573 6f20  ccionarios (uso 
+00001470: 696e 7465 726e 6f29 0a20 2020 2020 2020  interno).       
+00001480: 2073 656c 662e 4361 6e74 5061 6769 6e61   self.CantPagina
+00001490: 7320 3d20 7365 6c66 2e48 6179 4572 726f  s = self.HayErro
+000014a0: 7220 3d20 4e6f 6e65 0a0a 2020 2020 6465  r = None..    de
+000014b0: 6620 5f5f 616e 616c 697a 6172 5f65 7272  f __analizar_err
+000014c0: 6f72 6573 2873 656c 662c 2072 6574 293a  ores(self, ret):
+000014d0: 0a20 2020 2020 2020 2022 436f 6d70 7275  .        "Compru
+000014e0: 6562 6120 7920 6578 7472 6165 2065 7272  eba y extrae err
+000014f0: 6f72 6573 2073 6920 6578 6973 7465 6e20  ores si existen 
+00001500: 656e 206c 6120 7265 7370 7565 7374 6120  en la respuesta 
+00001510: 584d 4c22 0a20 2020 2020 2020 2073 656c  XML".        sel
+00001520: 662e 6572 726f 7265 7320 3d20 7265 742e  f.errores = ret.
+00001530: 6765 7428 2765 7272 6f72 6573 272c 205b  get('errores', [
+00001540: 5d29 0a20 2020 2020 2020 2073 656c 662e  ]).        self.
+00001550: 4572 726f 7265 7320 3d20 5b22 2573 3a20  Errores = ["%s: 
+00001560: 2573 2220 2520 2869 745b 2763 5f65 7272  %s" % (it['c_err
+00001570: 6f72 275d 2c20 6974 5b27 645f 6572 726f  or'], it['d_erro
+00001580: 7227 5d29 0a20 2020 2020 2020 2020 2020  r']).           
+00001590: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000015a0: 2069 7420 696e 2072 6574 2e67 6574 2827   it in ret.get('
+000015b0: 6572 726f 7265 7327 2c20 5b5d 295d 0a20  errores', [])]. 
+000015c0: 2020 2020 2020 2073 656c 662e 5265 7375         self.Resu
+000015d0: 6c74 6164 6f20 3d20 7265 742e 6765 7428  ltado = ret.get(
+000015e0: 2772 6573 756c 7461 646f 2729 0a0a 2020  'resultado')..  
+000015f0: 2020 6465 6620 436f 6e65 6374 6172 2873    def Conectar(s
+00001600: 656c 662c 2063 6163 6865 3d4e 6f6e 652c  elf, cache=None,
+00001610: 2077 7364 6c3d 4e6f 6e65 2c20 7072 6f78   wsdl=None, prox
+00001620: 793d 2222 2c20 7772 6170 7065 723d 4e6f  y="", wrapper=No
+00001630: 6e65 2c20 6361 6365 7274 3d4e 6f6e 652c  ne, cacert=None,
+00001640: 2074 696d 656f 7574 3d33 3029 3a0a 2020   timeout=30):.  
+00001650: 2020 2020 2020 2320 436f 6e65 6374 6f20        # Conecto 
+00001660: 7573 616e 646f 2065 6c20 6de9 746f 646f  usando el m.todo
+00001670: 2065 7374 616e 6461 7264 3a0a 2020 2020   estandard:.    
+00001680: 2020 2020 6f6b 203d 2042 6173 6557 532e      ok = BaseWS.
+00001690: 436f 6e65 6374 6172 2873 656c 662c 2063  Conectar(self, c
+000016a0: 6163 6865 2c20 7773 646c 2c20 7072 6f78  ache, wsdl, prox
+000016b0: 792c 2077 7261 7070 6572 2c20 6361 6365  y, wrapper, cace
+000016c0: 7274 2c20 7469 6d65 6f75 742c 0a20 2020  rt, timeout,.   
+000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016e0: 2020 2020 2020 2020 2020 2073 6f61 705f             soap_
+000016f0: 7365 7276 6572 3d22 6a65 7474 7922 290a  server="jetty").
+00001700: 2020 2020 2020 2020 6966 206f 6b3a 0a20          if ok:. 
+00001710: 2020 2020 2020 2020 2020 2023 2073 6920             # si 
+00001720: 656c 2061 7263 6869 766f 2065 7320 6c6f  el archivo es lo
+00001730: 6361 6c2c 2061 7375 6d6f 2071 7565 2079  cal, asumo que y
+00001740: 6120 6573 7461 2063 6f72 7265 6769 646f  a esta corregido
+00001750: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00001760: 206e 6f74 2073 656c 662e 7773 646c 2e73   not self.wsdl.s
+00001770: 7461 7274 7377 6974 6828 2266 696c 6522  tartswith("file"
+00001780: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00001790: 2020 2023 2063 6f72 7269 6a6f 2075 6269     # corrijo ubi
+000017a0: 6361 6369 f36e 2064 656c 2073 6572 7669  caci.n del servi
+000017b0: 646f 7220 286c 6f63 616c 686f 7374 3a35  dor (localhost:5
+000017c0: 3930 3530 2065 6e20 656c 2057 5344 4c29  9050 en el WSDL)
+000017d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000017e0: 206c 6f63 6174 696f 6e20 3d20 7365 6c66   location = self
+000017f0: 2e77 7364 6c5b 3a2d 355d 0a20 2020 2020  .wsdl[:-5].     
+00001800: 2020 2020 2020 2020 2020 2077 7320 3d20             ws = 
+00001810: 7365 6c66 2e63 6c69 656e 742e 7365 7276  self.client.serv
+00001820: 6963 6573 5b27 4957 6562 5365 7276 6963  ices['IWebServic
+00001830: 6553 656e 6173 6127 5d0a 2020 2020 2020  eSenasa'].      
+00001840: 2020 2020 2020 2020 2020 7773 5b27 706f            ws['po
+00001850: 7274 7327 5d5b 2749 5765 6253 6572 7669  rts']['IWebServi
+00001860: 6365 5365 6e61 7361 506f 7274 275d 5b27  ceSenasaPort']['
+00001870: 6c6f 6361 7469 6f6e 275d 203d 206c 6f63  location'] = loc
+00001880: 6174 696f 6e0a 0a20 2020 2020 2020 2020  ation..         
+00001890: 2020 2023 2045 7374 6162 6c65 6365 7220     # Establecer 
+000018a0: 6372 6564 656e 6369 616c 6573 2064 6520  credenciales de 
+000018b0: 7365 6775 7269 6461 643a 0a20 2020 2020  seguridad:.     
+000018c0: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+000018d0: 6e74 5b27 7773 7365 3a53 6563 7572 6974  nt['wsse:Securit
+000018e0: 7927 5d20 3d20 7b0a 2020 2020 2020 2020  y'] = {.        
+000018f0: 2020 2020 2020 2020 2777 7373 653a 5573          'wsse:Us
+00001900: 6572 6e61 6d65 546f 6b65 6e27 3a20 7b0a  ernameToken': {.
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 2020 2020 2777 7373 653a 5573 6572 6e61      'wsse:Userna
+00001930: 6d65 273a 2073 656c 662e 5573 6572 6e61  me': self.Userna
+00001940: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00001950: 2020 2020 2020 2020 2777 7373 653a 5061          'wsse:Pa
+00001960: 7373 776f 7264 273a 2073 656c 662e 5061  ssword': self.Pa
+00001970: 7373 776f 7264 2c0a 2020 2020 2020 2020  ssword,.        
+00001980: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00001990: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+000019a0: 2020 2020 2020 2020 7265 7475 726e 206f          return o
+000019b0: 6b0a 0a20 2020 2040 696e 6963 6961 6c69  k..    @iniciali
+000019c0: 7a61 725f 795f 6361 7074 7572 6172 5f65  zar_y_capturar_e
+000019d0: 7863 6570 6369 6f6e 6573 0a20 2020 2064  xcepciones.    d
+000019e0: 6566 2053 6176 6554 7261 6e73 6163 6369  ef SaveTransacci
+000019f0: 6f6e 2873 656c 662c 2075 7375 6172 696f  on(self, usuario
+00001a00: 2c20 7061 7373 776f 7264 2c0a 2020 2020  , password,.    
+00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a20: 2020 2020 676c 6e5f 6f72 6967 656e 3d4e      gln_origen=N
+00001a30: 6f6e 652c 2067 6c6e 5f64 6573 7469 6e6f  one, gln_destino
+00001a40: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+00001a50: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00001a60: 5f6f 7065 7261 6369 6f6e 3d4e 6f6e 652c  _operacion=None,
+00001a70: 2066 5f65 6c61 626f 7261 6369 6f6e 3d4e   f_elaboracion=N
+00001a80: 6f6e 652c 2066 5f76 746f 3d4e 6f6e 652c  one, f_vto=None,
+00001a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001aa0: 2020 2020 2020 2020 2069 645f 6576 656e           id_even
+00001ab0: 746f 3d4e 6f6e 652c 2063 6f64 5f70 726f  to=None, cod_pro
+00001ac0: 6475 6374 6f3d 4e6f 6e65 2c20 6e5f 6361  ducto=None, n_ca
+00001ad0: 6e74 6964 6164 3d4e 6f6e 652c 0a20 2020  ntidad=None,.   
+00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001af0: 2020 2020 206e 5f73 6572 6965 3d4e 6f6e       n_serie=Non
+00001b00: 652c 206e 5f6c 6f74 653d 4e6f 6e65 2c20  e, n_lote=None, 
+00001b10: 6e5f 6361 693d 4e6f 6e65 2c20 6e5f 6361  n_cai=None, n_ca
+00001b20: 653d 4e6f 6e65 2c0a 2020 2020 2020 2020  e=None,.        
+00001b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b40: 6964 5f6d 6f74 6976 6f5f 6465 7374 7275  id_motivo_destru
+00001b50: 6363 696f 6e3d 4e6f 6e65 2c20 6e5f 6d61  ccion=None, n_ma
+00001b60: 6e69 6669 6573 746f 3d4e 6f6e 652c 0a20  nifiesto=None,. 
+00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b80: 2020 2020 2020 2065 6e5f 7472 616e 7370         en_transp
+00001b90: 6f72 7465 3d4e 6f6e 652c 206e 5f72 656d  orte=None, n_rem
+00001ba0: 6974 6f3d 4e6f 6e65 2c0a 2020 2020 2020  ito=None,.      
+00001bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bc0: 2020 6d6f 7469 766f 5f64 6576 6f6c 7563    motivo_devoluc
+00001bd0: 696f 6e3d 4e6f 6e65 2c20 6f62 7365 7276  ion=None, observ
+00001be0: 6163 696f 6e65 733d 4e6f 6e65 2c0a 2020  aciones=None,.  
+00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c00: 2020 2020 2020 6e5f 7661 6c65 5f63 6f6d        n_vale_com
+00001c10: 7072 613d 4e6f 6e65 2c20 6170 656c 6c69  pra=None, apelli
+00001c20: 646f 4e6f 6d62 7265 733d 4e6f 6e65 2c0a  doNombres=None,.
+00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c40: 2020 2020 2020 2020 6469 7265 6363 696f          direccio
+00001c50: 6e3d 4e6f 6e65 2c20 6e75 6d65 726f 3d4e  n=None, numero=N
+00001c60: 6f6e 652c 206c 6f63 616c 6964 6164 3d4e  one, localidad=N
+00001c70: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00001c80: 2020 2020 2020 2020 2020 2020 2070 726f               pro
+00001c90: 7669 6e63 6961 3d4e 6f6e 652c 206e 5f70  vincia=None, n_p
+00001ca0: 6f73 7461 6c3d 4e6f 6e65 2c20 6375 6974  ostal=None, cuit
+00001cb0: 3d4e 6f6e 650a 2020 2020 2020 2020 2020  =None.          
+00001cc0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00001cd0: 3a0a 2020 2020 2020 2020 2252 6561 6c69  :.        "Reali
+00001ce0: 7a61 2065 6c20 7265 6769 7374 726f 2064  za el registro d
+00001cf0: 6520 756e 6120 7472 616e 7361 6363 69f3  e una transacci.
+00001d00: 6e20 6465 2070 726f 6475 6374 6f73 2066  n de productos f
+00001d10: 6974 6f73 616e 6974 6172 696f 732e 2022  itosanitarios. "
+00001d20: 0a20 2020 2020 2020 2023 2063 7265 6f20  .        # creo 
+00001d30: 6c6f 7320 7061 72e1 6d65 7472 6f73 2070  los par.metros p
+00001d40: 6172 6120 6573 7461 206c 6c61 6d61 6461  ara esta llamada
+00001d50: 0a20 2020 2020 2020 2070 6172 616d 7320  .        params 
+00001d60: 3d20 7b20 2027 676c 6e5f 6f72 6967 656e  = {  'gln_origen
+00001d70: 273a 2067 6c6e 5f6f 7269 6765 6e2c 0a20  ': gln_origen,. 
+00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d90: 2020 2027 676c 6e5f 6465 7374 696e 6f27     'gln_destino'
+00001da0: 3a20 676c 6e5f 6465 7374 696e 6f2c 0a20  : gln_destino,. 
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dc0: 2020 2027 665f 6f70 6572 6163 696f 6e27     'f_operacion'
+00001dd0: 3a20 665f 6f70 6572 6163 696f 6e2c 0a20  : f_operacion,. 
+00001de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001df0: 2020 2027 665f 656c 6162 6f72 6163 696f     'f_elaboracio
+00001e00: 6e27 3a20 665f 656c 6162 6f72 6163 696f  n': f_elaboracio
+00001e10: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+00001e20: 2020 2020 2020 2027 665f 7674 6f27 3a20         'f_vto': 
+00001e30: 665f 7674 6f2c 0a20 2020 2020 2020 2020  f_vto,.         
+00001e40: 2020 2020 2020 2020 2020 2027 6964 5f65             'id_e
+00001e50: 7665 6e74 6f27 3a20 6964 5f65 7665 6e74  vento': id_event
+00001e60: 6f2c 0a20 2020 2020 2020 2020 2020 2020  o,.             
+00001e70: 2020 2020 2020 2027 636f 645f 7072 6f64         'cod_prod
+00001e80: 7563 746f 273a 2063 6f64 5f70 726f 6475  ucto': cod_produ
+00001e90: 6374 6f2c 0a20 2020 2020 2020 2020 2020  cto,.           
+00001ea0: 2020 2020 2020 2020 2027 6e5f 6361 6e74           'n_cant
+00001eb0: 6964 6164 273a 206e 5f63 616e 7469 6461  idad': n_cantida
+00001ec0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00001ed0: 2020 2020 2020 2027 6e5f 7365 7269 6527         'n_serie'
+00001ee0: 3a20 6e5f 7365 7269 652c 0a20 2020 2020  : n_serie,.     
+00001ef0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001f00: 6e5f 6c6f 7465 273a 206e 5f6c 6f74 652c  n_lote': n_lote,
+00001f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001f20: 2020 2020 2027 6e5f 6361 6927 3a20 6e5f       'n_cai': n_
+00001f30: 6361 6920 6f72 204e 6f6e 652c 0a20 2020  cai or None,.   
+00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f50: 2027 6e5f 6361 6527 3a20 6e5f 6361 6520   'n_cae': n_cae 
+00001f60: 6f72 204e 6f6e 652c 0a20 2020 2020 2020  or None,.       
+00001f70: 2020 2020 2020 2020 2020 2020 2027 6964               'id
 00001f80: 5f6d 6f74 6976 6f5f 6465 7374 7275 6363  _motivo_destrucc
-00001f90: 696f 6e20 6f72 204e 6f6e 652c 0a20 2020  ion or None,.   
-00001fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fb0: 2027 6e5f 6d61 6e69 6669 6573 746f 273a   'n_manifiesto':
-00001fc0: 206e 5f6d 616e 6966 6965 7374 6f20 6f72   n_manifiesto or
-00001fd0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00001fe0: 2020 2020 2020 2020 2020 2027 656e 5f74             'en_t
-00001ff0: 7261 6e73 706f 7274 6527 3a20 656e 5f74  ransporte': en_t
-00002000: 7261 6e73 706f 7274 6520 6f72 204e 6f6e  ransporte or Non
-00002010: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00002020: 2020 2020 2020 2027 6e5f 7265 6d69 746f         'n_remito
-00002030: 273a 206e 5f72 656d 6974 6f20 6f72 204e  ': n_remito or N
-00002040: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00002050: 2020 2020 2020 2020 2027 6d6f 7469 766f           'motivo
-00002060: 5f64 6576 6f6c 7563 696f 6e27 3a20 6d6f  _devolucion': mo
-00002070: 7469 766f 5f64 6576 6f6c 7563 696f 6e20  tivo_devolucion 
-00002080: 6f72 204e 6f6e 652c 0a20 2020 2020 2020  or None,.       
-00002090: 2020 2020 2020 2020 2020 2020 2027 6f62               'ob
-000020a0: 7365 7276 6163 696f 6e65 7327 3a20 6f62  servaciones': ob
-000020b0: 7365 7276 6163 696f 6e65 7320 6f72 204e  servaciones or N
-000020c0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-000020d0: 2020 2020 2020 2020 2027 6e5f 7661 6c65           'n_vale
-000020e0: 5f63 6f6d 7072 6127 3a20 6e5f 7661 6c65  _compra': n_vale
-000020f0: 5f63 6f6d 7072 6120 6f72 204e 6f6e 652c  _compra or None,
-00002100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002110: 2020 2020 2027 6170 656c 6c69 646f 4e6f       'apellidoNo
-00002120: 6d62 7265 7327 3a20 6170 656c 6c69 646f  mbres': apellido
-00002130: 4e6f 6d62 7265 7320 6f72 204e 6f6e 652c  Nombres or None,
-00002140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002150: 2020 2020 2027 6469 7265 6363 696f 6e27       'direccion'
-00002160: 3a20 6469 7265 6363 696f 6e20 6f72 204e  : direccion or N
-00002170: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00002180: 2020 2020 2020 2020 2027 6e75 6d65 726f           'numero
-00002190: 273a 206e 756d 6572 6f20 6f72 204e 6f6e  ': numero or Non
-000021a0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000021b0: 2020 2020 2020 2027 6c6f 6361 6c69 6461         'localida
-000021c0: 6427 3a20 6c6f 6361 6c69 6461 6420 6f72  d': localidad or
-000021d0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-000021e0: 2020 2020 2020 2020 2020 2027 7072 6f76             'prov
-000021f0: 696e 6369 6127 3a20 7072 6f76 696e 6369  incia': provinci
-00002200: 6120 6f72 204e 6f6e 652c 0a20 2020 2020  a or None,.     
-00002210: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00002220: 6e5f 706f 7374 616c 273a 206e 5f70 6f73  n_postal': n_pos
-00002230: 7461 6c20 6f72 204e 6f6e 652c 0a20 2020  tal or None,.   
-00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002250: 2027 6375 6974 273a 2063 7569 7420 6f72   'cuit': cuit or
-00002260: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00002270: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00002280: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
-00002290: 636c 6965 6e74 2e73 6176 6554 7261 6e73  client.saveTrans
-000022a0: 6163 6369 6f6e 6573 280a 2020 2020 2020  acciones(.      
-000022b0: 2020 2020 2020 6172 6730 3d70 6172 616d        arg0=param
-000022c0: 732c 0a20 2020 2020 2020 2020 2020 2061  s,.            a
-000022d0: 7267 313d 7573 7561 7269 6f2c 0a20 2020  rg1=usuario,.   
-000022e0: 2020 2020 2020 2020 2061 7267 323d 7061           arg2=pa
-000022f0: 7373 776f 7264 2c0a 2020 2020 2020 2020  ssword,.        
-00002300: 290a 2020 2020 2020 2020 7265 7420 3d20  ).        ret = 
-00002310: 7265 735b 2772 6574 7572 6e27 5d0a 2020  res['return'].  
-00002320: 2020 2020 2020 7365 6c66 2e43 6f64 6967        self.Codig
-00002330: 6f54 7261 6e73 6163 6369 6f6e 203d 2072  oTransaccion = r
-00002340: 6574 2e67 6574 2827 636f 6469 676f 5472  et.get('codigoTr
-00002350: 616e 7361 6363 696f 6e27 290a 2020 2020  ansaccion').    
-00002360: 2020 2020 7365 6c66 2e5f 5f61 6e61 6c69      self.__anali
-00002370: 7a61 725f 6572 726f 7265 7328 7265 7429  zar_errores(ret)
-00002380: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002390: 5472 7565 0a0a 2020 2020 4069 6e69 6369  True..    @inici
-000023a0: 616c 697a 6172 5f79 5f63 6170 7475 7261  alizar_y_captura
-000023b0: 725f 6578 6365 7063 696f 6e65 730a 2020  r_excepciones.  
-000023c0: 2020 6465 6620 5365 6e64 4361 6e63 656c    def SendCancel
-000023d0: 6154 7261 6e73 6163 2873 656c 662c 2075  aTransac(self, u
-000023e0: 7375 6172 696f 2c20 7061 7373 776f 7264  suario, password
-000023f0: 2c20 636f 6469 676f 5f74 7261 6e73 6163  , codigo_transac
-00002400: 6369 6f6e 293a 0a20 2020 2020 2020 2022  cion):.        "
-00002410: 2052 6561 6c69 7a61 206c 6120 6361 6e63   Realiza la canc
-00002420: 656c 6163 69f3 6e20 6465 2075 6e61 2074  elaci.n de una t
-00002430: 7261 6e73 6163 6369 f36e 220a 2020 2020  ransacci.n".    
-00002440: 2020 2020 7265 7320 3d20 7365 6c66 2e63      res = self.c
-00002450: 6c69 656e 742e 7365 6e64 4361 6e63 656c  lient.sendCancel
-00002460: 6154 7261 6e73 6163 280a 2020 2020 2020  aTransac(.      
-00002470: 2020 2020 2020 6172 6730 3d63 6f64 6967        arg0=codig
-00002480: 6f5f 7472 616e 7361 6363 696f 6e2c 0a20  o_transaccion,. 
-00002490: 2020 2020 2020 2020 2020 2061 7267 313d             arg1=
-000024a0: 7573 7561 7269 6f2c 0a20 2020 2020 2020  usuario,.       
-000024b0: 2020 2020 2061 7267 323d 7061 7373 776f       arg2=passwo
-000024c0: 7264 2c0a 2020 2020 2020 2020 290a 2020  rd,.        ).  
-000024d0: 2020 2020 2020 7265 7420 3d20 7265 735b        ret = res[
-000024e0: 2772 6574 7572 6e27 5d0a 2020 2020 2020  'return'].      
-000024f0: 2020 7365 6c66 2e43 6f64 6967 6f54 7261    self.CodigoTra
-00002500: 6e73 6163 6369 6f6e 203d 2072 6574 2e67  nsaccion = ret.g
-00002510: 6574 2827 636f 6469 676f 5472 616e 7361  et('codigoTransa
-00002520: 6363 696f 6e27 290a 2020 2020 2020 2020  ccion').        
-00002530: 7365 6c66 2e5f 5f61 6e61 6c69 7a61 725f  self.__analizar_
-00002540: 6572 726f 7265 7328 7265 7429 0a20 2020  errores(ret).   
-00002550: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00002560: 0a0a 2020 2020 4069 6e69 6369 616c 697a  ..    @inicializ
-00002570: 6172 5f79 5f63 6170 7475 7261 725f 6578  ar_y_capturar_ex
-00002580: 6365 7063 696f 6e65 730a 2020 2020 6465  cepciones.    de
-00002590: 6620 5365 6e64 436f 6e66 6972 6d61 5472  f SendConfirmaTr
-000025a0: 616e 7361 6363 2873 656c 662c 2075 7375  ansacc(self, usu
-000025b0: 6172 696f 2c20 7061 7373 776f 7264 2c20  ario, password, 
-000025c0: 705f 6964 735f 7472 616e 7361 632c 2066  p_ids_transac, f
-000025d0: 5f6f 7065 7261 6369 6f6e 2c20 6e5f 6361  _operacion, n_ca
-000025e0: 6e74 6964 6164 3d4e 6f6e 6529 3a0a 2020  ntidad=None):.  
-000025f0: 2020 2020 2020 2243 6f6e 6669 726d 6120        "Confirma 
-00002600: 6c61 2072 6563 6570 6369 f36e 2064 6520  la recepci.n de 
-00002610: 756e 206d 6564 6963 616d 656e 746f 220a  un medicamento".
-00002620: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
-00002630: 6c66 2e63 6c69 656e 742e 7365 6e64 436f  lf.client.sendCo
-00002640: 6e66 6972 6d61 5472 616e 7361 6363 280a  nfirmaTransacc(.
-00002650: 2020 2020 2020 2020 2020 2020 6172 6730              arg0
-00002660: 3d75 7375 6172 696f 2c0a 2020 2020 2020  =usuario,.      
-00002670: 2020 2020 2020 6172 6731 3d70 6173 7377        arg1=passw
-00002680: 6f72 642c 0a20 2020 2020 2020 2020 2020  ord,.           
-00002690: 2061 7267 323d 7b27 705f 6964 735f 7472   arg2={'p_ids_tr
-000026a0: 616e 7361 6327 3a20 705f 6964 735f 7472  ansac': p_ids_tr
-000026b0: 616e 7361 632c 2027 665f 6f70 6572 6163  ansac, 'f_operac
-000026c0: 696f 6e27 3a20 665f 6f70 6572 6163 696f  ion': f_operacio
-000026d0: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-000026e0: 2020 2020 2027 6e5f 6361 6e74 6964 6164       'n_cantidad
-000026f0: 273a 206e 5f63 616e 7469 6461 642c 0a20  ': n_cantidad,. 
-00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002710: 7d2c 0a20 2020 2020 2020 2029 0a20 2020  },.        ).   
-00002720: 2020 2020 2072 6574 203d 2072 6573 5b27       ret = res['
-00002730: 7265 7475 726e 275d 0a20 2020 2020 2020  return'].       
-00002740: 2073 656c 662e 436f 6469 676f 5472 616e   self.CodigoTran
-00002750: 7361 6363 696f 6e20 3d20 7265 742e 6765  saccion = ret.ge
-00002760: 7428 2763 6f64 6967 6f54 7261 6e73 6163  t('codigoTransac
-00002770: 6369 6f6e 2729 0a20 2020 2020 2020 2073  cion').        s
-00002780: 656c 662e 5f5f 616e 616c 697a 6172 5f65  elf.__analizar_e
-00002790: 7272 6f72 6573 2872 6574 290a 2020 2020  rrores(ret).    
-000027a0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-000027b0: 0a20 2020 2040 696e 6963 6961 6c69 7a61  .    @inicializa
-000027c0: 725f 795f 6361 7074 7572 6172 5f65 7863  r_y_capturar_exc
-000027d0: 6570 6369 6f6e 6573 0a20 2020 2064 6566  epciones.    def
-000027e0: 2053 656e 6441 6c65 7274 6154 7261 6e73   SendAlertaTrans
-000027f0: 6163 6328 7365 6c66 2c20 7573 7561 7269  acc(self, usuari
-00002800: 6f2c 2070 6173 7377 6f72 642c 2070 5f69  o, password, p_i
-00002810: 6473 5f74 7261 6e73 6163 5f77 7329 3a0a  ds_transac_ws):.
-00002820: 2020 2020 2020 2020 2241 6c65 7274 6120          "Alerta 
-00002830: 756e 206d 6564 6963 616d 656e 746f 2c20  un medicamento, 
-00002840: 6163 6369 f36e 2063 6f6e 7472 6172 6961  acci.n contraria
-00002850: 2061 2093 636f 6e66 6972 6d61 7220 6c61   a .confirmar la
-00002860: 2074 7261 6e73 6163 6369 f36e 942e 220a   transacci.n..".
-00002870: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
-00002880: 6c66 2e63 6c69 656e 742e 7365 6e64 416c  lf.client.sendAl
-00002890: 6572 7461 5472 616e 7361 6363 280a 2020  ertaTransacc(.  
-000028a0: 2020 2020 2020 2020 2020 6172 6730 3d75            arg0=u
-000028b0: 7375 6172 696f 2c0a 2020 2020 2020 2020  suario,.        
-000028c0: 2020 2020 6172 6731 3d70 6173 7377 6f72      arg1=passwor
-000028d0: 642c 0a20 2020 2020 2020 2020 2020 2061  d,.            a
-000028e0: 7267 323d 705f 6964 735f 7472 616e 7361  rg2=p_ids_transa
-000028f0: 635f 7773 2c0a 2020 2020 2020 2020 290a  c_ws,.        ).
-00002900: 2020 2020 2020 2020 7265 7420 3d20 7265          ret = re
-00002910: 735b 2772 6574 7572 6e27 5d0a 2020 2020  s['return'].    
-00002920: 2020 2020 7365 6c66 2e43 6f64 6967 6f54      self.CodigoT
-00002930: 7261 6e73 6163 6369 6f6e 203d 2072 6574  ransaccion = ret
-00002940: 2e67 6574 2827 6964 5f74 7261 6e73 6163  .get('id_transac
-00002950: 5f61 736f 6369 6164 6127 290a 2020 2020  _asociada').    
-00002960: 2020 2020 7365 6c66 2e5f 5f61 6e61 6c69      self.__anali
-00002970: 7a61 725f 6572 726f 7265 7328 7265 7429  zar_errores(ret)
-00002980: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002990: 5472 7565 0a0a 2020 2020 4069 6e69 6369  True..    @inici
-000029a0: 616c 697a 6172 5f79 5f63 6170 7475 7261  alizar_y_captura
-000029b0: 725f 6578 6365 7063 696f 6e65 730a 2020  r_excepciones.  
-000029c0: 2020 6465 6620 4765 7454 7261 6e73 6163    def GetTransac
-000029d0: 6369 6f6e 6573 2873 656c 662c 2075 7375  ciones(self, usu
-000029e0: 6172 696f 2c20 7061 7373 776f 7264 2c0a  ario, password,.
-000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a00: 6964 5f74 7261 6e73 6163 6369 6f6e 3d4e  id_transaccion=N
-00002a10: 6f6e 652c 2069 645f 6576 656e 746f 3d4e  one, id_evento=N
-00002a20: 6f6e 652c 2067 6c6e 5f6f 7269 6765 6e3d  one, gln_origen=
-00002a30: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00002a40: 2020 2020 2020 6665 6368 615f 6465 7364        fecha_desd
-00002a50: 655f 743d 4e6f 6e65 2c20 6665 6368 615f  e_t=None, fecha_
-00002a60: 6861 7374 615f 743d 4e6f 6e65 2c0a 2020  hasta_t=None,.  
-00002a70: 2020 2020 2020 2020 2020 2020 2020 6665                fe
-00002a80: 6368 615f 6465 7364 655f 763d 4e6f 6e65  cha_desde_v=None
-00002a90: 2c20 6665 6368 615f 6861 7374 615f 763d  , fecha_hasta_v=
-00002aa0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00002ab0: 2020 2020 2020 676c 6e5f 696e 666f 726d        gln_inform
-00002ac0: 6164 6f72 3d4e 6f6e 652c 2069 645f 7469  ador=None, id_ti
-00002ad0: 706f 5f74 7261 6e73 6163 6369 6f6e 3d4e  po_transaccion=N
-00002ae0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00002af0: 2020 2020 2067 7469 6e5f 656c 656d 656e       gtin_elemen
-00002b00: 746f 3d4e 6f6e 652c 206e 5f6c 6f74 653d  to=None, n_lote=
-00002b10: 4e6f 6e65 2c20 6e5f 7365 7269 653d 4e6f  None, n_serie=No
-00002b20: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00002b30: 2020 2020 6e5f 7265 6d69 746f 5f66 6163      n_remito_fac
-00002b40: 7475 7261 3d4e 6f6e 652c 0a20 2020 2020  tura=None,.     
-00002b50: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
-00002b60: 2020 2020 2020 2254 7261 6520 756e 206c        "Trae un l
-00002b70: 6973 7461 646f 2064 6520 6c61 7320 7472  istado de las tr
-00002b80: 616e 7361 6363 696f 6e65 7320 7175 6520  ansacciones que 
-00002b90: 6e6f 2065 7374 e16e 2063 6f6e 6669 726d  no est.n confirm
-00002ba0: 6164 6173 220a 0a20 2020 2020 2020 2023  adas"..        #
-00002bb0: 2070 7265 7061 726f 206c 6f73 2070 6172   preparo los par
-00002bc0: 616d 6574 726f 7320 6465 2065 6e74 7261  ametros de entra
-00002bd0: 6461 206f 7063 696f 6e61 6c65 733a 0a20  da opcionales:. 
-00002be0: 2020 2020 2020 206b 7761 7267 7320 3d20         kwargs = 
-00002bf0: 7b7d 0a20 2020 2020 2020 2069 6620 6964  {}.        if id
-00002c00: 5f74 7261 6e73 6163 6369 6f6e 2069 7320  _transaccion is 
-00002c10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00002c20: 2020 2020 2020 6b77 6172 6773 5b27 6172        kwargs['ar
-00002c30: 6732 275d 203d 2069 645f 7472 616e 7361  g2'] = id_transa
-00002c40: 6363 696f 6e0a 2020 2020 2020 2020 6966  ccion.        if
-00002c50: 2069 645f 6576 656e 746f 2069 7320 6e6f   id_evento is no
-00002c60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00002c70: 2020 2020 6b77 6172 6773 5b27 6172 6733      kwargs['arg3
-00002c80: 275d 203d 2069 645f 6576 656e 746f 0a20  '] = id_evento. 
-00002c90: 2020 2020 2020 2069 6620 676c 6e5f 6f72         if gln_or
-00002ca0: 6967 656e 2069 7320 6e6f 7420 4e6f 6e65  igen is not None
-00002cb0: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
-00002cc0: 6172 6773 5b27 6172 6734 275d 203d 2067  args['arg4'] = g
-00002cd0: 6c6e 5f6f 7269 6765 6e0a 2020 2020 2020  ln_origen.      
-00002ce0: 2020 6966 2066 6563 6861 5f64 6573 6465    if fecha_desde
-00002cf0: 5f74 2069 7320 6e6f 7420 4e6f 6e65 3a0a  _t is not None:.
-00002d00: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-00002d10: 6773 5b27 6172 6735 275d 203d 2066 6563  gs['arg5'] = fec
-00002d20: 6861 5f64 6573 6465 5f74 0a20 2020 2020  ha_desde_t.     
-00002d30: 2020 2069 6620 6665 6368 615f 6861 7374     if fecha_hast
-00002d40: 615f 7420 6973 206e 6f74 204e 6f6e 653a  a_t is not None:
-00002d50: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
-00002d60: 7267 735b 2761 7267 3627 5d20 3d20 6665  rgs['arg6'] = fe
-00002d70: 6368 615f 6861 7374 615f 740a 2020 2020  cha_hasta_t.    
-00002d80: 2020 2020 6966 2066 6563 6861 5f64 6573      if fecha_des
-00002d90: 6465 5f76 2069 7320 6e6f 7420 4e6f 6e65  de_v is not None
-00002da0: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
-00002db0: 6172 6773 5b27 6172 6737 275d 203d 2066  args['arg7'] = f
-00002dc0: 6563 6861 5f64 6573 6465 5f76 0a20 2020  echa_desde_v.   
-00002dd0: 2020 2020 2069 6620 6665 6368 615f 6861       if fecha_ha
-00002de0: 7374 615f 7620 6973 206e 6f74 204e 6f6e  sta_v is not Non
-00002df0: 653a 0a20 2020 2020 2020 2020 2020 206b  e:.            k
-00002e00: 7761 7267 735b 2761 7267 3827 5d20 3d20  wargs['arg8'] = 
-00002e10: 6665 6368 615f 6861 7374 615f 760a 2020  fecha_hasta_v.  
-00002e20: 2020 2020 2020 6966 2067 6c6e 5f69 6e66        if gln_inf
-00002e30: 6f72 6d61 646f 7220 6973 206e 6f74 204e  ormador is not N
-00002e40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00002e50: 206b 7761 7267 735b 2761 7267 3927 5d20   kwargs['arg9'] 
-00002e60: 3d20 676c 6e5f 696e 666f 726d 6164 6f72  = gln_informador
-00002e70: 0a20 2020 2020 2020 2069 6620 6964 5f74  .        if id_t
-00002e80: 6970 6f5f 7472 616e 7361 6363 696f 6e20  ipo_transaccion 
-00002e90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00002ea0: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
-00002eb0: 2761 7267 3130 275d 203d 2069 645f 7469  'arg10'] = id_ti
-00002ec0: 706f 5f74 7261 6e73 6163 6369 6f6e 0a20  po_transaccion. 
-00002ed0: 2020 2020 2020 2069 6620 6774 696e 5f65         if gtin_e
-00002ee0: 6c65 6d65 6e74 6f20 6973 206e 6f74 204e  lemento is not N
-00002ef0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00002f00: 206b 7761 7267 735b 2761 7267 3131 275d   kwargs['arg11']
-00002f10: 203d 2067 7469 6e5f 656c 656d 656e 746f   = gtin_elemento
-00002f20: 0a20 2020 2020 2020 2069 6620 6e5f 6c6f  .        if n_lo
-00002f30: 7465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  te is not None:.
-00002f40: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
-00002f50: 6773 5b27 6172 6731 3227 5d20 3d20 6e5f  gs['arg12'] = n_
-00002f60: 6c6f 7465 0a20 2020 2020 2020 2069 6620  lote.        if 
-00002f70: 6e5f 7365 7269 6520 6973 206e 6f74 204e  n_serie is not N
-00002f80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00002f90: 206b 7761 7267 735b 2761 7267 3133 275d   kwargs['arg13']
-00002fa0: 203d 206e 5f73 6572 6965 0a20 2020 2020   = n_serie.     
-00002fb0: 2020 2069 6620 6e5f 7265 6d69 746f 5f66     if n_remito_f
-00002fc0: 6163 7475 7261 2069 7320 6e6f 7420 4e6f  actura is not No
-00002fd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00002fe0: 6b77 6172 6773 5b27 6172 6731 3427 5d20  kwargs['arg14'] 
-00002ff0: 3d20 6e5f 7265 6d69 746f 5f66 6163 7475  = n_remito_factu
-00003000: 7261 0a0a 2020 2020 2020 2020 2320 6c6c  ra..        # ll
-00003010: 616d 6f20 616c 2077 6562 7365 7276 6963  amo al webservic
-00003020: 650a 2020 2020 2020 2020 7265 7320 3d20  e.        res = 
-00003030: 7365 6c66 2e63 6c69 656e 742e 6765 7454  self.client.getT
-00003040: 7261 6e73 6163 6369 6f6e 6573 280a 2020  ransacciones(.  
-00003050: 2020 2020 2020 2020 2020 6172 6730 3d75            arg0=u
-00003060: 7375 6172 696f 2c0a 2020 2020 2020 2020  suario,.        
-00003070: 2020 2020 6172 6731 3d70 6173 7377 6f72      arg1=passwor
-00003080: 642c 0a20 2020 2020 2020 2020 2020 202a  d,.            *
-00003090: 2a6b 7761 7267 730a 2020 2020 2020 2020  *kwargs.        
-000030a0: 290a 2020 2020 2020 2020 7265 7420 3d20  ).        ret = 
-000030b0: 7265 735b 2772 6574 7572 6e27 5d0a 2020  res['return'].  
-000030c0: 2020 2020 2020 6966 2072 6574 3a0a 2020        if ret:.  
-000030d0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000030e0: 5f61 6e61 6c69 7a61 725f 6572 726f 7265  _analizar_errore
-000030f0: 7328 7265 7429 0a20 2020 2020 2020 2020  s(ret).         
-00003100: 2020 2073 656c 662e 4361 6e74 5061 6769     self.CantPagi
-00003110: 6e61 7320 3d20 7265 742e 6765 7428 2763  nas = ret.get('c
-00003120: 616e 7450 6167 696e 6173 2729 0a20 2020  antPaginas').   
-00003130: 2020 2020 2020 2020 2073 656c 662e 4861           self.Ha
-00003140: 7945 7272 6f72 203d 2072 6574 2e67 6574  yError = ret.get
-00003150: 2827 6861 795f 6572 726f 7227 290a 2020  ('hay_error').  
-00003160: 2020 2020 2020 2020 2020 7365 6c66 2e54            self.T
-00003170: 7261 6e73 6163 6369 6f6e 5365 6e61 7361  ransaccionSenasa
-00003180: 203d 205b 6974 2066 6f72 2069 7420 696e   = [it for it in
-00003190: 2072 6574 2e67 6574 2827 6c69 7374 272c   ret.get('list',
-000031a0: 205b 5d29 5d0a 2020 2020 2020 2020 7265   [])].        re
-000031b0: 7475 726e 2054 7275 650a 0a20 2020 2064  turn True..    d
-000031c0: 6566 2020 4c65 6572 5472 616e 7361 6363  ef  LeerTransacc
-000031d0: 696f 6e28 7365 6c66 293a 0a20 2020 2020  ion(self):.     
-000031e0: 2020 2022 5265 636f 7272 6f20 5472 616e     "Recorro Tran
-000031f0: 7361 6363 696f 6e53 656e 6173 6120 6465  saccionSenasa de
-00003200: 7675 656c 746f 2070 6f72 2047 6574 5472  vuelto por GetTr
-00003210: 616e 7361 6363 696f 6e65 7322 0a20 2020  ansacciones".   
-00003220: 2020 2020 2020 2320 7573 6172 2047 6574        # usar Get
-00003230: 5061 7261 6d65 7472 6f20 7061 7261 2063  Parametro para c
-00003240: 6f6e 7375 6c74 6172 2065 6c20 7661 6c6f  onsultar el valo
-00003250: 7220 7265 746f 726e 6164 6f20 706f 7220  r retornado por 
-00003260: 656c 2077 6562 7365 7276 6963 650a 0a20  el webservice.. 
-00003270: 2020 2020 2020 2069 6620 7365 6c66 2e54         if self.T
-00003280: 7261 6e73 6163 6369 6f6e 5365 6e61 7361  ransaccionSenasa
-00003290: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-000032a0: 6578 7472 6169 676f 2065 6c20 7072 696d  extraigo el prim
-000032b0: 6572 2069 7465 6d0a 2020 2020 2020 2020  er item.        
-000032c0: 2020 2020 7365 6c66 2e70 6172 616d 735f      self.params_
-000032d0: 6f75 7420 3d20 7365 6c66 2e54 7261 6e73  out = self.Trans
-000032e0: 6163 6369 6f6e 5365 6e61 7361 2e70 6f70  accionSenasa.pop
-000032f0: 2830 290a 2020 2020 2020 2020 2020 2020  (0).            
-00003300: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-00003310: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00003320: 2020 2020 2020 2320 6c69 6d70 696f 206c        # limpio l
-00003330: 6f73 2070 6172 e16d 6574 726f 730a 2020  os par.metros.  
-00003340: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00003350: 6172 616d 735f 6f75 7420 3d20 7b7d 0a20  arams_out = {}. 
-00003360: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003370: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
-00003380: 204c 6565 7245 7272 6f72 2873 656c 6629   LeerError(self)
-00003390: 3a0a 2020 2020 2020 2020 2252 6563 6f72  :.        "Recor
-000033a0: 726f 206c 6f73 2065 7272 6f72 6573 2064  ro los errores d
-000033b0: 6576 7565 6c74 6f73 2079 2064 6576 7565  evueltos y devue
-000033c0: 6c76 6f20 656c 2070 7269 6d65 726f 2073  lvo el primero s
-000033d0: 6920 6578 6973 7465 220a 0a20 2020 2020  i existe"..     
-000033e0: 2020 2069 6620 7365 6c66 2e45 7272 6f72     if self.Error
-000033f0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00003400: 2320 6578 7472 6169 676f 2065 6c20 7072  # extraigo el pr
-00003410: 696d 6572 2069 7465 6d0a 2020 2020 2020  imer item.      
-00003420: 2020 2020 2020 6572 203d 2073 656c 662e        er = self.
-00003430: 4572 726f 7265 732e 706f 7028 3029 0a20  Errores.pop(0). 
-00003440: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003450: 6e20 6572 0a20 2020 2020 2020 2065 6c73  n er.        els
-00003460: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00003470: 6574 7572 6e20 2222 0a0a 2020 2020 6465  eturn ""..    de
-00003480: 6620 5365 7455 7365 726e 616d 6528 7365  f SetUsername(se
-00003490: 6c66 2c20 7573 6572 6e61 6d65 293a 0a20  lf, username):. 
-000034a0: 2020 2020 2020 2022 4573 7461 626c 657a         "Establez
-000034b0: 636f 2065 6c20 6e6f 6d62 7265 2064 6520  co el nombre de 
-000034c0: 7573 7561 7269 6f22 0a20 2020 2020 2020  usuario".       
-000034d0: 2073 656c 662e 5573 6572 6e61 6d65 203d   self.Username =
-000034e0: 2075 7365 726e 616d 650a 0a20 2020 2064   username..    d
-000034f0: 6566 2053 6574 5061 7373 776f 7264 2873  ef SetPassword(s
-00003500: 656c 662c 2070 6173 7377 6f72 6429 3a0a  elf, password):.
-00003510: 2020 2020 2020 2020 2245 7374 6162 6c65          "Estable
-00003520: 7a63 6f20 6c61 2063 6f6e 7472 6173 65f1  zco la contrase.
-00003530: 6122 0a20 2020 2020 2020 2073 656c 662e  a".        self.
-00003540: 5061 7373 776f 7264 203d 2070 6173 7377  Password = passw
-00003550: 6f72 640a 0a20 2020 2064 6566 2047 6574  ord..    def Get
-00003560: 436f 6469 676f 5472 616e 7361 6363 696f  CodigoTransaccio
-00003570: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
-00003580: 2022 4465 7675 656c 766f 2065 6c20 63f3   "Devuelvo el c.
-00003590: 6469 676f 2064 6520 7472 616e 7361 6363  digo de transacc
-000035a0: 69f3 6e22 0a20 2020 2020 2020 2072 6574  i.n".        ret
-000035b0: 7572 6e20 7365 6c66 2e43 6f64 6967 6f54  urn self.CodigoT
-000035c0: 7261 6e73 6163 6369 6f6e 0a0a 2020 2020  ransaccion..    
-000035d0: 6465 6620 4765 7452 6573 756c 7461 646f  def GetResultado
-000035e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000035f0: 2244 6576 7565 6c76 6f20 656c 2072 6573  "Devuelvo el res
-00003600: 756c 7461 646f 220a 2020 2020 2020 2020  ultado".        
-00003610: 7265 7475 726e 2073 656c 662e 5265 7375  return self.Resu
-00003620: 6c74 6164 6f0a 0a0a 6465 6620 6d61 696e  ltado...def main
-00003630: 2829 3a0a 2020 2020 2246 756e 6369 f36e  ():.    "Funci.n
-00003640: 2070 7269 6e63 6970 616c 2064 6520 7072   principal de pr
-00003650: 7565 6261 7320 286f 6274 656e 6572 2043  uebas (obtener C
-00003660: 4145 2922 0a20 2020 2069 6d70 6f72 7420  AE)".    import 
-00003670: 6f73 2c20 7469 6d65 2c20 7379 730a 2020  os, time, sys.  
-00003680: 2020 676c 6f62 616c 2057 5344 4c2c 204c    global WSDL, L
-00003690: 4f43 4154 494f 4e0a 0a20 2020 2044 4542  OCATION..    DEB
-000036a0: 5547 203d 2027 2d2d 6465 6275 6727 2069  UG = '--debug' i
-000036b0: 6e20 7379 732e 6172 6776 0a0a 2020 2020  n sys.argv..    
-000036c0: 7773 203d 2054 7261 7a61 5665 7428 290a  ws = TrazaVet().
-000036d0: 0a20 2020 2077 732e 5573 6572 6e61 6d65  .    ws.Username
-000036e0: 203d 2027 7465 7374 7773 6572 7669 6365   = 'testwservice
-000036f0: 270a 2020 2020 7773 2e50 6173 7377 6f72  '.    ws.Passwor
-00003700: 6420 3d20 2774 6573 7477 7365 7276 6963  d = 'testwservic
-00003710: 6570 7377 270a 0a20 2020 2069 6620 272d  epsw'..    if '-
-00003720: 2d70 726f 6427 2069 6e20 7379 732e 6172  -prod' in sys.ar
-00003730: 6776 2061 6e64 206e 6f74 2048 4f4d 4f3a  gv and not HOMO:
-00003740: 0a20 2020 2020 2020 2057 5344 4c20 3d20  .        WSDL = 
-00003750: 2268 7474 7073 3a2f 2f73 6572 7669 6369  "https://servici
-00003760: 6f73 2e70 616d 692e 6f72 672e 6172 2f74  os.pami.org.ar/t
-00003770: 7261 7a61 7665 742e 5765 6253 6572 7669  razavet.WebServi
-00003780: 6365 3f77 7364 6c22 0a20 2020 2020 2020  ce?wsdl".       
-00003790: 2070 7269 6e74 2822 5573 616e 646f 2057   print("Usando W
-000037a0: 5344 4c3a 222c 2057 5344 4c29 0a20 2020  SDL:", WSDL).   
-000037b0: 2020 2020 2073 7973 2e61 7267 762e 706f       sys.argv.po
-000037c0: 7028 7379 732e 6172 6776 2e69 6e64 6578  p(sys.argv.index
-000037d0: 2822 2d2d 7072 6f64 2229 290a 0a20 2020  ("--prod"))..   
-000037e0: 2069 6620 272d 2d70 726f 7879 2720 696e   if '--proxy' in
-000037f0: 2073 7973 2e61 7267 7620 616e 6420 6e6f   sys.argv and no
-00003800: 7420 484f 4d4f 3a0a 2020 2020 2020 2020  t HOMO:.        
-00003810: 7072 6f78 7920 3d20 7379 732e 6172 6776  proxy = sys.argv
-00003820: 2e70 6f70 2873 7973 2e61 7267 762e 696e  .pop(sys.argv.in
-00003830: 6465 7828 222d 2d70 726f 7879 2229 202b  dex("--proxy") +
-00003840: 2031 290a 2020 2020 2020 2020 7072 696e   1).        prin
-00003850: 7428 2255 7361 6e64 6f20 7072 6f78 793a  t("Usando proxy:
-00003860: 222c 2070 726f 7879 290a 2020 2020 2020  ", proxy).      
-00003870: 2020 7379 732e 6172 6776 2e70 6f70 2873    sys.argv.pop(s
-00003880: 7973 2e61 7267 762e 696e 6465 7828 222d  ys.argv.index("-
-00003890: 2d70 726f 7879 2229 290a 2020 2020 656c  -proxy")).    el
-000038a0: 7365 3a0a 2020 2020 2020 2020 7072 6f78  se:.        prox
-000038b0: 7920 3d20 4e6f 6e65 0a0a 2020 2020 2320  y = None..    # 
-000038c0: 496e 6963 6961 6c69 7a6f 206c 6173 2076  Inicializo las v
-000038d0: 6172 6961 626c 6573 2079 2065 7374 7275  ariables y estru
-000038e0: 6374 7572 6173 2070 6172 6120 656c 2061  cturas para el a
-000038f0: 7263 6869 766f 2064 6520 696e 7465 7263  rchivo de interc
-00003900: 616d 6269 6f3a 0a20 2020 2074 7261 6e73  ambio:.    trans
-00003910: 6163 6369 6f6e 5f64 746f 203d 205b 5d0a  accion_dto = [].
-00003920: 2020 2020 7472 616e 7361 6363 696f 6e65      transaccione
-00003930: 7320 3d20 5b5d 0a20 2020 2065 7272 6f72  s = [].    error
-00003940: 6573 203d 205b 5d0a 2020 2020 666f 726d  es = [].    form
-00003950: 6174 6f73 203d 205b 2827 5472 616e 7361  atos = [('Transa
-00003960: 6363 696f 6e44 544f 272c 2054 5241 4e53  ccionDTO', TRANS
-00003970: 4143 4349 4f4e 5f44 544f 2c20 7472 616e  ACCION_DTO, tran
-00003980: 7361 6363 696f 6e5f 6474 6f29 2c0a 2020  saccion_dto),.  
-00003990: 2020 2020 2020 2020 2020 2020 2020 2827                ('
-000039a0: 5472 616e 7361 6363 696f 6e65 7327 2c20  Transacciones', 
-000039b0: 5452 414e 5341 4343 494f 4e45 532c 2074  TRANSACCIONES, t
-000039c0: 7261 6e73 6163 6369 6f6e 6573 292c 0a20  ransacciones),. 
-000039d0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-000039e0: 2745 7272 6f72 6573 272c 2045 5252 4f52  'Errores', ERROR
-000039f0: 4553 2c20 6572 726f 7265 7329 2c0a 2020  ES, errores),.  
-00003a00: 2020 2020 2020 2020 2020 2020 205d 0a0a               ]..
-00003a10: 2020 2020 6966 2027 2d2d 666f 726d 6174      if '--format
-00003a20: 6f27 2069 6e20 7379 732e 6172 6776 3a0a  o' in sys.argv:.
-00003a30: 2020 2020 2020 2020 7072 696e 7428 2246          print("F
-00003a40: 6f72 6d61 746f 3a22 290a 2020 2020 2020  ormato:").      
-00003a50: 2020 666f 7220 6d73 672c 2066 6f72 6d61    for msg, forma
-00003a60: 746f 2c20 6c69 7374 6120 696e 2066 6f72  to, lista in for
-00003a70: 6d61 746f 733a 0a20 2020 2020 2020 2020  matos:.         
-00003a80: 2020 2063 6f6d 6965 6e7a 6f20 3d20 310a     comienzo = 1.
-00003a90: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00003aa0: 7428 223d 3d3d 2025 7320 3d3d 3d22 2025  t("=== %s ===" %
-00003ab0: 206d 7367 290a 2020 2020 2020 2020 2020   msg).          
-00003ac0: 2020 7072 696e 7428 227c 7c20 252d 3235    print("|| %-25
-00003ad0: 7320 7c7c 2025 2d31 3273 207c 7c20 252d  s || %-12s || %-
-00003ae0: 3573 207c 7c20 252d 3473 207c 7c20 252d  5s || %-4s || %-
-00003af0: 3130 7320 7c7c 2220 2520 280a 2020 2020  10s ||" % (.    
-00003b00: 2020 2020 2020 2020 2020 2020 224e 6f6d              "Nom
-00003b10: 6272 6522 2c20 2254 6970 6f22 2c20 224c  bre", "Tipo", "L
-00003b20: 6f6e 672e 222c 2022 506f 7328 7478 7429  ong.", "Pos(txt)
-00003b30: 222c 2022 4361 6d70 6f28 6462 6629 2229  ", "Campo(dbf)")
-00003b40: 290a 2020 2020 2020 2020 2020 2020 636c  ).            cl
-00003b50: 6176 6573 203d 205b 5d0a 2020 2020 2020  aves = [].      
-00003b60: 2020 2020 2020 666f 7220 666d 7420 696e        for fmt in
-00003b70: 2066 6f72 6d61 746f 3a0a 2020 2020 2020   formato:.      
-00003b80: 2020 2020 2020 2020 2020 636c 6176 652c            clave,
-00003b90: 206c 6f6e 6769 7475 642c 2074 6970 6f20   longitud, tipo 
-00003ba0: 3d20 666d 745b 303a 335d 0a20 2020 2020  = fmt[0:3].     
-00003bb0: 2020 2020 2020 2020 2020 2063 6c61 7665             clave
-00003bc0: 5f64 6266 203d 2064 6172 5f6e 6f6d 6272  _dbf = dar_nombr
-00003bd0: 655f 6361 6d70 6f5f 6462 6628 636c 6176  e_campo_dbf(clav
-00003be0: 652c 2063 6c61 7665 7329 0a20 2020 2020  e, claves).     
-00003bf0: 2020 2020 2020 2020 2020 2063 6c61 7665             clave
-00003c00: 732e 6170 7065 6e64 2863 6c61 7665 5f64  s.append(clave_d
-00003c10: 6266 290a 2020 2020 2020 2020 2020 2020  bf).            
-00003c20: 2020 2020 7072 696e 7428 227c 7c20 252d      print("|| %-
-00003c30: 3235 7320 7c7c 2025 2d31 3273 207c 7c20  25s || %-12s || 
-00003c40: 2535 6420 7c7c 2020 2025 3464 2020 207c  %5d ||   %4d   |
-00003c50: 7c20 252d 3130 7320 7c7c 2220 2520 280a  | %-10s ||" % (.
-00003c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c70: 2020 2020 636c 6176 652c 2074 6970 6f2c      clave, tipo,
-00003c80: 206c 6f6e 6769 7475 642c 2063 6f6d 6965   longitud, comie
-00003c90: 6e7a 6f2c 2063 6c61 7665 5f64 6266 2929  nzo, clave_dbf))
-00003ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003cb0: 2063 6f6d 6965 6e7a 6f20 2b3d 206c 6f6e   comienzo += lon
-00003cc0: 6769 7475 640a 2020 2020 2020 2020 7379  gitud.        sy
-00003cd0: 732e 6578 6974 2830 290a 0a20 2020 2069  s.exit(0)..    i
-00003ce0: 6620 272d 2d63 6172 6761 7227 2069 6e20  f '--cargar' in 
-00003cf0: 7379 732e 6172 6776 3a0a 2020 2020 2020  sys.argv:.      
-00003d00: 2020 6966 2027 2d2d 6462 6627 2069 6e20    if '--dbf' in 
-00003d10: 7379 732e 6172 6776 3a0a 2020 2020 2020  sys.argv:.      
-00003d20: 2020 2020 2020 6c65 6572 5f64 6266 2866        leer_dbf(f
-00003d30: 6f72 6d61 746f 735b 3a31 5d2c 207b 7d29  ormatos[:1], {})
-00003d40: 0a20 2020 2020 2020 2065 6c69 6620 272d  .        elif '-
-00003d50: 2d6a 736f 6e27 2069 6e20 7379 732e 6172  -json' in sys.ar
-00003d60: 6776 3a0a 2020 2020 2020 2020 2020 2020  gv:.            
-00003d70: 666f 7220 666f 726d 6174 6f20 696e 2066  for formato in f
-00003d80: 6f72 6d61 746f 735b 3a31 5d3a 0a20 2020  ormatos[:1]:.   
-00003d90: 2020 2020 2020 2020 2020 2020 2061 7263               arc
-00003da0: 6869 766f 203d 206f 7065 6e28 666f 726d  hivo = open(form
-00003db0: 6174 6f5b 305d 2e6c 6f77 6572 2829 202b  ato[0].lower() +
-00003dc0: 2022 2e6a 736f 6e22 2c20 2272 2229 0a20   ".json", "r"). 
-00003dd0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00003de0: 203d 206a 736f 6e2e 6c6f 6164 2861 7263   = json.load(arc
-00003df0: 6869 766f 290a 2020 2020 2020 2020 2020  hivo).          
-00003e00: 2020 2020 2020 666f 726d 6174 6f5b 325d        formato[2]
-00003e10: 2e65 7874 656e 6428 6429 0a20 2020 2020  .extend(d).     
-00003e20: 2020 2020 2020 2020 2020 2061 7263 6869             archi
-00003e30: 766f 2e63 6c6f 7365 2829 0a20 2020 2020  vo.close().     
-00003e40: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00003e50: 2020 2020 2066 6f72 2066 6f72 6d61 746f       for formato
-00003e60: 2069 6e20 666f 726d 6174 6f73 5b3a 315d   in formatos[:1]
-00003e70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003e80: 2020 6172 6368 6976 6f20 3d20 6f70 656e    archivo = open
-00003e90: 2866 6f72 6d61 746f 5b30 5d2e 6c6f 7765  (formato[0].lowe
-00003ea0: 7228 2920 2b20 222e 7478 7422 2c20 2272  r() + ".txt", "r
-00003eb0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00003ec0: 2020 2066 6f72 206c 696e 6561 2069 6e20     for linea in 
-00003ed0: 6172 6368 6976 6f3a 0a20 2020 2020 2020  archivo:.       
-00003ee0: 2020 2020 2020 2020 2020 2020 2064 203d               d =
-00003ef0: 206c 6565 7228 6c69 6e65 612c 2066 6f72   leer(linea, for
-00003f00: 6d61 746f 5b31 5d29 0a20 2020 2020 2020  mato[1]).       
-00003f10: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00003f20: 6d61 746f 5b32 5d2e 6170 7065 6e64 2864  mato[2].append(d
-00003f30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003f40: 2020 6172 6368 6976 6f2e 636c 6f73 6528    archivo.close(
-00003f50: 290a 0a20 2020 2077 732e 436f 6e65 6374  )..    ws.Conect
-00003f60: 6172 2822 222c 2057 5344 4c2c 2070 726f  ar("", WSDL, pro
-00003f70: 7879 290a 0a20 2020 2069 6620 7773 2e45  xy)..    if ws.E
-00003f80: 7863 6570 6369 6f6e 3a0a 2020 2020 2020  xcepcion:.      
-00003f90: 2020 7072 696e 7428 7773 2e45 7863 6570    print(ws.Excep
-00003fa0: 6369 6f6e 290a 2020 2020 2020 2020 7072  cion).        pr
-00003fb0: 696e 7428 7773 2e54 7261 6365 6261 636b  int(ws.Traceback
-00003fc0: 290a 2020 2020 2020 2020 7379 732e 6578  ).        sys.ex
-00003fd0: 6974 282d 3129 0a0a 2020 2020 2320 4461  it(-1)..    # Da
-00003fe0: 746f 7320 6465 2070 7275 6562 6173 3a0a  tos de pruebas:.
-00003ff0: 0a20 2020 2069 6620 272d 2d74 6573 7427  .    if '--test'
-00004000: 2069 6e20 7379 732e 6172 6776 3a0a 2020   in sys.argv:.  
-00004010: 2020 2020 2020 7472 616e 7361 6363 696f        transaccio
-00004020: 6e5f 6474 6f2e 6170 7065 6e64 2864 6963  n_dto.append(dic
-00004030: 7428 0a20 2020 2020 2020 2020 2020 2067  t(.            g
-00004040: 6c6e 5f6f 7269 6765 6e3d 2239 3837 3635  ln_origen="98765
-00004050: 3433 3231 3039 3832 222c 2067 6c6e 5f64  43210982", gln_d
-00004060: 6573 7469 6e6f 3d22 3336 3932 3538 3134  estino="36925814
-00004070: 3733 3639 3322 2c0a 2020 2020 2020 2020  73693",.        
-00004080: 2020 2020 665f 6f70 6572 6163 696f 6e3d      f_operacion=
-00004090: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
-000040a0: 652e 6e6f 7728 292e 7374 7266 7469 6d65  e.now().strftime
-000040b0: 2822 2564 2f25 6d2f 2559 2229 2c0a 2020  ("%d/%m/%Y"),.  
-000040c0: 2020 2020 2020 2020 2020 665f 656c 6162            f_elab
-000040d0: 6f72 6163 696f 6e3d 6461 7465 7469 6d65  oracion=datetime
-000040e0: 2e64 6174 6574 696d 652e 6e6f 7728 292e  .datetime.now().
-000040f0: 7374 7266 7469 6d65 2822 2564 2f25 6d2f  strftime("%d/%m/
-00004100: 2559 2229 2c0a 2020 2020 2020 2020 2020  %Y"),.          
-00004110: 2020 665f 7674 6f3d 2864 6174 6574 696d    f_vto=(datetim
-00004120: 652e 6461 7465 7469 6d65 2e6e 6f77 2829  e.datetime.now()
-00004130: 2b64 6174 6574 696d 652e 7469 6d65 6465  +datetime.timede
-00004140: 6c74 6128 3330 2929 2e73 7472 6674 696d  lta(30)).strftim
-00004150: 6528 2225 642f 256d 2f25 5922 292c 0a20  e("%d/%m/%Y"),. 
-00004160: 2020 2020 2020 2020 2020 2069 645f 6576             id_ev
-00004170: 656e 746f 3d31 312c 0a20 2020 2020 2020  ento=11,.       
-00004180: 2020 2020 2063 6f64 5f70 726f 6475 6374       cod_product
-00004190: 6f3d 2238 3839 3030 3030 3030 3030 3030  o="8890000000000
-000041a0: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
-000041b0: 6e5f 6361 6e74 6964 6164 3d31 2c0a 2020  n_cantidad=1,.  
-000041c0: 2020 2020 2020 2020 2020 6e5f 7365 7269            n_seri
-000041d0: 653d 696e 7428 7469 6d65 2e74 696d 6528  e=int(time.time(
-000041e0: 292a 3130 292c 0a20 2020 2020 2020 2020  )*10),.         
-000041f0: 2020 206e 5f6c 6f74 653d 6461 7465 7469     n_lote=dateti
-00004200: 6d65 2e64 6174 6574 696d 652e 6e6f 7728  me.datetime.now(
-00004210: 292e 7374 7266 7469 6d65 2822 2559 2229  ).strftime("%Y")
-00004220: 2c0a 2020 2020 2020 2020 2020 2020 6e5f  ,.            n_
-00004230: 6361 693d 2231 3233 3435 3637 3839 3031  cai="12345678901
-00004240: 3233 3435 222c 0a20 2020 2020 2020 2020  2345",.         
-00004250: 2020 206e 5f63 6165 3d22 222c 0a20 2020     n_cae="",.   
-00004260: 2020 2020 2020 2020 2069 645f 6d6f 7469           id_moti
-00004270: 766f 5f64 6573 7472 7563 6369 6f6e 3d30  vo_destruccion=0
-00004280: 2c0a 2020 2020 2020 2020 2020 2020 6e5f  ,.            n_
-00004290: 6d61 6e69 6669 6573 746f 3d22 222c 0a20  manifiesto="",. 
-000042a0: 2020 2020 2020 2020 2020 2065 6e5f 7472             en_tr
-000042b0: 616e 7370 6f72 7465 3d22 4e22 2c0a 2020  ansporte="N",.  
-000042c0: 2020 2020 2020 2020 2020 6e5f 7265 6d69            n_remi
-000042d0: 746f 3d22 3132 3334 222c 0a20 2020 2020  to="1234",.     
-000042e0: 2020 2020 2020 206d 6f74 6976 6f5f 6465         motivo_de
-000042f0: 766f 6c75 6369 6f6e 3d22 222c 0a20 2020  volucion="",.   
-00004300: 2020 2020 2020 2020 206f 6273 6572 7661           observa
-00004310: 6369 6f6e 6573 3d22 7072 7565 6261 222c  ciones="prueba",
-00004320: 0a20 2020 2020 2020 2020 2020 206e 5f76  .            n_v
-00004330: 616c 655f 636f 6d70 7261 3d22 222c 0a20  ale_compra="",. 
-00004340: 2020 2020 2020 2020 2020 2061 7065 6c6c             apell
-00004350: 6964 6f4e 6f6d 6272 6573 3d22 4a75 616e  idoNombres="Juan
-00004360: 2050 6572 6573 222c 0a20 2020 2020 2020   Peres",.       
-00004370: 2020 2020 2064 6972 6563 6369 6f6e 3d22       direccion="
-00004380: 5361 7261 7a61 222c 206e 756d 6572 6f3d  Saraza", numero=
-00004390: 2231 3233 3422 2c0a 2020 2020 2020 2020  "1234",.        
-000043a0: 2020 2020 6c6f 6361 6c69 6461 643d 2248      localidad="H
-000043b0: 7572 6c69 6e67 6861 6d22 2c20 7072 6f76  urlingham", prov
-000043c0: 696e 6369 613d 2242 7565 6e6f 7320 4169  incia="Buenos Ai
-000043d0: 7265 7322 2c0a 2020 2020 2020 2020 2020  res",.          
-000043e0: 2020 6e5f 706f 7374 616c 3d22 3136 3838    n_postal="1688
-000043f0: 222c 0a20 2020 2020 2020 2020 2020 2063  ",.            c
-00004400: 7569 743d 2232 3032 3637 3536 3533 3933  uit="20267565393
-00004410: 222c 0a20 2020 2020 2020 2020 2020 2063  ",.            c
-00004420: 6f64 6967 6f5f 7472 616e 7361 6363 696f  odigo_transaccio
-00004430: 6e3d 4e6f 6e65 2c0a 2020 2020 2020 2020  n=None,.        
-00004440: 2929 0a0a 2020 2020 2320 4f70 6369 6f6e  ))..    # Opcion
-00004450: 6573 2070 7269 6e63 6970 616c 6573 3a0a  es principales:.
-00004460: 0a20 2020 2069 6620 272d 2d63 6f6e 6669  .    if '--confi
-00004470: 726d 6127 2069 6e20 7379 732e 6172 6776  rma' in sys.argv
-00004480: 3a0a 2020 2020 2020 2020 6966 2027 2d2d  :.        if '--
-00004490: 6c6f 6164 786d 6c27 2069 6e20 7379 732e  loadxml' in sys.
-000044a0: 6172 6776 3a0a 2020 2020 2020 2020 2020  argv:.          
-000044b0: 2020 7773 2e4c 6f61 6454 6573 7458 4d4c    ws.LoadTestXML
-000044c0: 2822 7472 617a 616d 6564 5f63 6f6e 6669  ("trazamed_confi
-000044d0: 726d 612e 786d 6c22 2920 2023 2063 6172  rma.xml")  # car
-000044e0: 676f 2072 6573 7075 6573 7461 0a20 2020  go respuesta.   
-000044f0: 2020 2020 2020 2020 206f 6b20 3d20 7773           ok = ws
-00004500: 2e53 656e 6443 6f6e 6669 726d 6154 7261  .SendConfirmaTra
-00004510: 6e73 6163 6328 7573 7561 7269 6f3d 2270  nsacc(usuario="p
-00004520: 7275 6562 6173 7773 222c 2070 6173 7377  ruebasws", passw
-00004530: 6f72 643d 2270 7275 6562 6173 7773 222c  ord="pruebasws",
-00004540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004560: 2020 2020 705f 6964 735f 7472 616e 7361      p_ids_transa
-00004570: 633d 2231 222c 2066 5f6f 7065 7261 6369  c="1", f_operaci
-00004580: 6f6e 3d22 3331 2d31 322d 3230 3133 2229  on="31-12-2013")
-00004590: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000045a0: 6e6f 7420 6f6b 3a0a 2020 2020 2020 2020  not ok:.        
-000045b0: 2020 2020 2020 2020 7261 6973 6520 5275          raise Ru
-000045c0: 6e74 696d 6545 7272 6f72 2877 732e 4578  ntimeError(ws.Ex
-000045d0: 6365 7063 696f 6e29 0a20 2020 2020 2020  cepcion).       
-000045e0: 2077 732e 5365 6e64 436f 6e66 6972 6d61   ws.SendConfirma
-000045f0: 5472 616e 7361 6363 282a 7379 732e 6172  Transacc(*sys.ar
-00004600: 6776 5b73 7973 2e61 7267 762e 696e 6465  gv[sys.argv.inde
-00004610: 7828 222d 2d63 6f6e 6669 726d 6122 292b  x("--confirma")+
-00004620: 313a 5d29 0a20 2020 2065 6c69 6620 272d  1:]).    elif '-
-00004630: 2d61 6c65 7274 6127 2069 6e20 7379 732e  -alerta' in sys.
-00004640: 6172 6776 3a0a 2020 2020 2020 2020 7773  argv:.        ws
-00004650: 2e53 656e 6441 6c65 7274 6154 7261 6e73  .SendAlertaTrans
-00004660: 6163 6328 2a73 7973 2e61 7267 765b 7379  acc(*sys.argv[sy
-00004670: 732e 6172 6776 2e69 6e64 6578 2822 2d2d  s.argv.index("--
-00004680: 616c 6572 7461 2229 2b31 3a5d 290a 2020  alerta")+1:]).  
-00004690: 2020 656c 6966 2027 2d2d 6361 6e63 656c    elif '--cancel
-000046a0: 6127 2069 6e20 7379 732e 6172 6776 3a0a  a' in sys.argv:.
-000046b0: 2020 2020 2020 2020 7773 2e53 656e 6443          ws.SendC
-000046c0: 616e 6365 6c61 5472 616e 7361 6328 2a73  ancelaTransac(*s
-000046d0: 7973 2e61 7267 765b 7379 732e 6172 6776  ys.argv[sys.argv
-000046e0: 2e69 6e64 6578 2822 2d2d 6361 6e63 656c  .index("--cancel
-000046f0: 6122 292b 313a 5d29 0a20 2020 2065 6c69  a")+1:]).    eli
-00004700: 6620 272d 2d63 6f6e 7375 6c74 6127 2069  f '--consulta' i
-00004710: 6e20 7379 732e 6172 6776 3a0a 2020 2020  n sys.argv:.    
-00004720: 2020 2020 7773 2e47 6574 5472 616e 7361      ws.GetTransa
-00004730: 6363 696f 6e65 7328 0a20 2020 2020 2020  cciones(.       
-00004740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004750: 2020 2020 202a 7379 732e 6172 6776 5b73       *sys.argv[s
-00004760: 7973 2e61 7267 762e 696e 6465 7828 222d  ys.argv.index("-
-00004770: 2d63 6f6e 7375 6c74 6122 292b 313a 5d0a  -consulta")+1:].
-00004780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004790: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000047a0: 2020 2020 2020 7072 696e 7428 2243 616e        print("Can
-000047b0: 7450 6167 696e 6173 222c 2077 732e 4361  tPaginas", ws.Ca
-000047c0: 6e74 5061 6769 6e61 7329 0a20 2020 2020  ntPaginas).     
-000047d0: 2020 2070 7269 6e74 2822 4861 7945 7272     print("HayErr
-000047e0: 6f72 222c 2077 732e 4861 7945 7272 6f72  or", ws.HayError
-000047f0: 290a 2020 2020 2020 2020 2320 7072 696e  ).        # prin
-00004800: 7428 2254 7261 6e73 6163 6369 6f6e 5365  t("TransaccionSe
-00004810: 6e61 7361 222c 2077 732e 5472 616e 7361  nasa", ws.Transa
-00004820: 6363 696f 6e53 656e 6173 6129 0a20 2020  ccionSenasa).   
-00004830: 2020 2020 2023 2070 6172 616d 6574 726f       # parametro
-00004840: 7320 636f 6d75 6e65 7320 6465 2073 616c  s comunes de sal
-00004850: 6964 6120 2863 6f6c 756d 6e61 7320 6465  ida (columnas de
-00004860: 206c 6120 7461 626c 6129 3a0a 2020 2020   la tabla):.    
-00004870: 2020 2020 636c 6176 6573 203d 205b 6b20      claves = [k 
-00004880: 666f 7220 6b2c 2076 2c20 6c20 696e 2054  for k, v, l in T
-00004890: 5241 4e53 4143 4349 4f4e 4553 5d0a 2020  RANSACCIONES].  
-000048a0: 2020 2020 2020 2320 6578 7469 656e 646f        # extiendo
-000048b0: 206c 6120 6c69 7374 6120 6465 2072 6573   la lista de res
-000048c0: 756c 7461 646f 2070 6172 6120 656c 2061  ultado para el a
-000048d0: 7263 6869 766f 2064 6520 696e 7465 7263  rchivo de interc
-000048e0: 616d 6269 6f3a 0a20 2020 2020 2020 2074  ambio:.        t
-000048f0: 7261 6e73 6163 6369 6f6e 6573 2e65 7874  ransacciones.ext
-00004900: 656e 6428 7773 2e54 7261 6e73 6163 6369  end(ws.Transacci
-00004910: 6f6e 5365 6e61 7361 290a 2020 2020 2020  onSenasa).      
-00004920: 2020 2320 656e 6361 6265 7a61 646f 2064    # encabezado d
-00004930: 6520 6c61 2074 6162 6c61 3a0a 2020 2020  e la tabla:.    
-00004940: 2020 2020 7072 696e 7428 227c 7c22 2c20      print("||", 
-00004950: 227c 7c22 2e6a 6f69 6e28 5b22 2573 2220  "||".join(["%s" 
-00004960: 2520 636c 6176 6520 666f 7220 636c 6176  % clave for clav
-00004970: 6520 696e 2063 6c61 7665 735d 292c 2022  e in claves]), "
-00004980: 7c7c 2229 0a20 2020 2020 2020 2023 2072  ||").        # r
-00004990: 6563 6f72 726f 206c 6f73 2064 6174 6f73  ecorro los datos
-000049a0: 2064 6576 7565 6c74 6f73 2028 5472 616e   devueltos (Tran
-000049b0: 7361 6363 696f 6e53 656e 6173 6129 3a0a  saccionSenasa):.
-000049c0: 2020 2020 2020 2020 7768 696c 6520 7773          while ws
-000049d0: 2e4c 6565 7254 7261 6e73 6163 6369 6f6e  .LeerTransaccion
-000049e0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000049f0: 666f 7220 636c 6176 6520 696e 2063 6c61  for clave in cla
-00004a00: 7665 733a 0a20 2020 2020 2020 2020 2020  ves:.           
-00004a10: 2020 2020 2070 7269 6e74 2822 7c7c 222c       print("||",
-00004a20: 2077 732e 4765 7450 6172 616d 6574 726f   ws.GetParametro
-00004a30: 2863 6c61 7665 2929 2020 2020 2020 2020  (clave))        
-00004a40: 2023 2069 6d70 7269 6d6f 2063 6164 6120   # imprimo cada 
-00004a50: 6669 6c61 0a20 2020 2020 2020 2020 2020  fila.           
-00004a60: 2070 7269 6e74 2822 7c7c 2229 0a20 2020   print("||").   
-00004a70: 2065 6c73 653a 0a20 2020 2020 2020 2061   else:.        a
-00004a80: 7267 7620 3d20 5b61 7267 7620 666f 7220  rgv = [argv for 
-00004a90: 6172 6776 2069 6e20 7379 732e 6172 6776  argv in sys.argv
-00004aa0: 2069 6620 6e6f 7420 6172 6776 2e73 7461   if not argv.sta
-00004ab0: 7274 7377 6974 6828 222d 2d22 295d 0a20  rtswith("--")]. 
-00004ac0: 2020 2020 2020 2069 6620 6e6f 7420 7472         if not tr
-00004ad0: 616e 7361 6363 696f 6e5f 6474 6f3a 0a20  ansaccion_dto:. 
-00004ae0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00004af0: 6e28 6172 6776 293e 3130 3a0a 2020 2020  n(argv)>10:.    
-00004b00: 2020 2020 2020 2020 2020 2020 7773 2e53              ws.S
-00004b10: 6176 6554 7261 6e73 6163 6369 6f6e 282a  aveTransaccion(*
-00004b20: 6172 6776 5b31 3a5d 290a 2020 2020 2020  argv[1:]).      
-00004b30: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00004b40: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00004b50: 7428 2245 5252 4f52 3a20 6e6f 2073 6520  t("ERROR: no se 
-00004b60: 696e 6469 6361 726f 6e20 746f 646f 7320  indicaron todos 
-00004b70: 6c6f 7320 7061 72e1 6d65 7472 6f73 2072  los par.metros r
-00004b80: 6571 7565 7269 646f 7322 290a 2020 2020  equeridos").    
-00004b90: 2020 2020 656c 6966 2074 7261 6e73 6163      elif transac
-00004ba0: 6369 6f6e 5f64 746f 3a0a 2020 2020 2020  cion_dto:.      
-00004bb0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00004bc0: 2020 2020 2020 2020 2020 2075 7375 6172             usuar
-00004bd0: 696f 2c20 7061 7373 776f 7264 203d 2061  io, password = a
-00004be0: 7267 765b 2d32 3a5d 0a20 2020 2020 2020  rgv[-2:].       
-00004bf0: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
-00004c00: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00004c10: 6e74 2822 4144 5645 5254 454e 4349 413a  nt("ADVERTENCIA:
-00004c20: 206e 6f20 7365 2069 6e64 6963 6f20 7061   no se indico pa
-00004c30: 72e1 6d65 7472 6f73 2075 7375 6172 696f  r.metros usuario
-00004c40: 2079 2070 6173 736f 776f 7264 2229 0a20   y passoword"). 
-00004c50: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00004c60: 7375 6172 696f 2c20 7061 7373 776f 7264  suario, password
-00004c70: 203d 2022 7365 6e61 7361 7773 222c 2022   = "senasaws", "
-00004c80: 436c 6176 6532 3031 3322 0a20 2020 2020  Clave2013".     
-00004c90: 2020 2020 2020 2066 6f72 2069 2c20 6474         for i, dt
-00004ca0: 6f20 696e 2065 6e75 6d65 7261 7465 2874  o in enumerate(t
-00004cb0: 7261 6e73 6163 6369 6f6e 5f64 746f 293a  ransaccion_dto):
-00004cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004cd0: 2070 7269 6e74 2822 5072 6f63 6573 616e   print("Procesan
-00004ce0: 646f 2072 6567 6973 7472 6f22 2c20 6929  do registro", i)
-00004cf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004d00: 2064 656c 2064 746f 5b27 636f 6469 676f   del dto['codigo
-00004d10: 5f74 7261 6e73 6163 6369 6f6e 275d 0a20  _transaccion']. 
-00004d20: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00004d30: 732e 5361 7665 5472 616e 7361 6363 696f  s.SaveTransaccio
-00004d40: 6e28 7573 7561 7269 6f2c 2070 6173 7377  n(usuario, passw
-00004d50: 6f72 642c 202a 2a64 746f 290a 2020 2020  ord, **dto).    
-00004d60: 2020 2020 2020 2020 2020 2020 6474 6f5b              dto[
-00004d70: 2763 6f64 6967 6f5f 7472 616e 7361 6363  'codigo_transacc
-00004d80: 696f 6e27 5d20 3d20 7773 2e43 6f64 6967  ion'] = ws.Codig
-00004d90: 6f54 7261 6e73 6163 6369 6f6e 0a20 2020  oTransaccion.   
-00004da0: 2020 2020 2020 2020 2020 2020 2065 7272               err
-00004db0: 6f72 6573 2e65 7874 656e 6428 7773 2e65  ores.extend(ws.e
-00004dc0: 7272 6f72 6573 290a 2020 2020 2020 2020  rrores).        
-00004dd0: 2020 2020 2020 2020 7072 696e 7428 227c          print("|
-00004de0: 5265 7375 6c74 6164 6f20 2535 737c 436f  Resultado %5s|Co
-00004df0: 6469 676f 5472 616e 7361 6363 696f 6e20  digoTransaccion 
-00004e00: 2531 3073 7c45 7272 6f72 6573 7c25 737c  %10s|Errores|%s|
-00004e10: 2220 2520 280a 2020 2020 2020 2020 2020  " % (.          
-00004e20: 2020 2020 2020 2020 2020 7773 2e52 6573            ws.Res
-00004e30: 756c 7461 646f 2c0a 2020 2020 2020 2020  ultado,.        
-00004e40: 2020 2020 2020 2020 2020 2020 7773 2e43              ws.C
-00004e50: 6f64 6967 6f54 7261 6e73 6163 6369 6f6e  odigoTransaccion
-00004e60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004e70: 2020 2020 2020 277c 272e 6a6f 696e 2877        '|'.join(w
-00004e80: 732e 4572 726f 7265 7320 6f72 205b 5d29  s.Errores or [])
-00004e90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004ea0: 2020 2020 2020 2929 0a20 2020 2020 2020        )).       
-00004eb0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00004ec0: 2020 2070 7269 6e74 2822 4552 524f 523a     print("ERROR:
-00004ed0: 206e 6f20 7365 2065 7370 6563 6966 6963   no se especific
-00004ee0: 6172 6f6e 2070 726f 6475 6374 6f73 2061  aron productos a
-00004ef0: 2069 6e66 6f72 6d61 7222 290a 0a20 2020   informar")..   
-00004f00: 2069 6620 6e6f 7420 7472 616e 7361 6363   if not transacc
-00004f10: 696f 6e5f 6474 6f3a 0a20 2020 2020 2020  ion_dto:.       
-00004f20: 2070 7269 6e74 2822 7c52 6573 756c 7461   print("|Resulta
-00004f30: 646f 2025 3573 7c43 6f64 6967 6f54 7261  do %5s|CodigoTra
-00004f40: 6e73 6163 6369 6f6e 2025 3130 737c 4572  nsaccion %10s|Er
-00004f50: 726f 7265 737c 2573 7c22 2025 2028 0a20  rores|%s|" % (. 
-00004f60: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00004f70: 732e 5265 7375 6c74 6164 6f2c 0a20 2020  s.Resultado,.   
-00004f80: 2020 2020 2020 2020 2020 2020 2077 732e               ws.
-00004f90: 436f 6469 676f 5472 616e 7361 6363 696f  CodigoTransaccio
-00004fa0: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-00004fb0: 2020 2027 7c27 2e6a 6f69 6e28 7773 2e45     '|'.join(ws.E
-00004fc0: 7272 6f72 6573 206f 7220 5b5d 292c 0a20  rrores or []),. 
-00004fd0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00004fe0: 290a 0a20 2020 2069 6620 7773 2e45 7863  )..    if ws.Exc
-00004ff0: 6570 6369 6f6e 3a0a 2020 2020 2020 2020  epcion:.        
-00005000: 7072 696e 7428 7773 2e54 7261 6365 6261  print(ws.Traceba
-00005010: 636b 290a 0a20 2020 2069 6620 272d 2d67  ck)..    if '--g
-00005020: 7261 6261 7227 2069 6e20 7379 732e 6172  rabar' in sys.ar
-00005030: 6776 3a0a 2020 2020 2020 2020 6966 2027  gv:.        if '
-00005040: 2d2d 6462 6627 2069 6e20 7379 732e 6172  --dbf' in sys.ar
-00005050: 6776 3a0a 2020 2020 2020 2020 2020 2020  gv:.            
-00005060: 6775 6172 6461 725f 6462 6628 666f 726d  guardar_dbf(form
-00005070: 6174 6f73 2c20 5472 7565 2c20 7b7d 290a  atos, True, {}).
-00005080: 2020 2020 2020 2020 656c 6966 2027 2d2d          elif '--
-00005090: 6a73 6f6e 2720 696e 2073 7973 2e61 7267  json' in sys.arg
-000050a0: 763a 0a20 2020 2020 2020 2020 2020 2066  v:.            f
-000050b0: 6f72 2066 6f72 6d61 746f 2069 6e20 666f  or formato in fo
-000050c0: 726d 6174 6f73 3a0a 2020 2020 2020 2020  rmatos:.        
-000050d0: 2020 2020 2020 2020 6172 6368 6976 6f20          archivo 
-000050e0: 3d20 6f70 656e 2866 6f72 6d61 746f 5b30  = open(formato[0
-000050f0: 5d2e 6c6f 7765 7228 2920 2b20 222e 6a73  ].lower() + ".js
-00005100: 6f6e 222c 2022 7722 290a 2020 2020 2020  on", "w").      
-00005110: 2020 2020 2020 2020 2020 6a73 6f6e 2e64            json.d
-00005120: 756d 7028 666f 726d 6174 6f5b 325d 2c20  ump(formato[2], 
-00005130: 6172 6368 6976 6f2c 2073 6f72 745f 6b65  archivo, sort_ke
-00005140: 7973 3d54 7275 652c 2069 6e64 656e 743d  ys=True, indent=
-00005150: 3429 0a20 2020 2020 2020 2020 2020 2020  4).             
-00005160: 2020 2061 7263 6869 766f 2e63 6c6f 7365     archivo.close
-00005170: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
-00005180: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00005190: 2066 6f72 6d61 746f 2069 6e20 666f 726d   formato in form
-000051a0: 6174 6f73 3a0a 2020 2020 2020 2020 2020  atos:.          
-000051b0: 2020 2020 2020 6172 6368 6976 6f20 3d20        archivo = 
-000051c0: 6f70 656e 2866 6f72 6d61 746f 5b30 5d2e  open(formato[0].
-000051d0: 6c6f 7765 7228 2920 2b20 222e 7478 7422  lower() + ".txt"
-000051e0: 2c20 2277 2229 0a20 2020 2020 2020 2020  , "w").         
-000051f0: 2020 2020 2020 2066 6f72 2069 7420 696e         for it in
-00005200: 2066 6f72 6d61 746f 5b32 5d3a 0a20 2020   formato[2]:.   
-00005210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005220: 2061 7263 6869 766f 2e77 7269 7465 2865   archivo.write(e
-00005230: 7363 7269 6269 7228 6974 2c20 666f 726d  scribir(it, form
-00005240: 6174 6f5b 315d 2929 0a20 2020 2020 2020  ato[1])).       
-00005250: 2020 2020 2061 7263 6869 766f 2e63 6c6f       archivo.clo
-00005260: 7365 2829 0a0a 0a23 2062 7573 636f 2065  se()...# busco e
-00005270: 6c20 6469 7265 6374 6f72 696f 2064 6520  l directorio de 
-00005280: 696e 7374 616c 6163 69f3 6e20 2867 6c6f  instalaci.n (glo
-00005290: 6261 6c20 7061 7261 2071 7565 206e 6f20  bal para que no 
-000052a0: 6361 6d62 6965 2073 6920 7573 616e 206f  cambie si usan o
-000052b0: 7472 6120 646c 6c29 0a49 4e53 5441 4c4c  tra dll).INSTALL
-000052c0: 5f44 4952 203d 2054 7261 7a61 5665 742e  _DIR = TrazaVet.
-000052d0: 496e 7374 616c 6c44 6972 203d 2067 6574  InstallDir = get
-000052e0: 5f69 6e73 7461 6c6c 5f64 6972 2829 0a0a  _install_dir()..
-000052f0: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-00005300: 275f 5f6d 6169 6e5f 5f27 3a0a 0a20 2020  '__main__':..   
-00005310: 2023 2061 6a75 7374 6f20 656c 2065 6e63   # ajusto el enc
-00005320: 6f64 696e 6720 706f 7220 6465 6665 6374  oding por defect
-00005330: 6f20 2873 6920 7365 2072 6564 6972 696a  o (si se redirij
-00005340: 6520 6c61 2073 616c 6964 6129 0a20 2020  e la salida).   
-00005350: 2069 6620 6e6f 7420 6861 7361 7474 7228   if not hasattr(
-00005360: 7379 732e 7374 646f 7574 2c20 2265 6e63  sys.stdout, "enc
-00005370: 6f64 696e 6722 2920 6f72 2073 7973 2e73  oding") or sys.s
-00005380: 7464 6f75 742e 656e 636f 6469 6e67 2069  tdout.encoding i
-00005390: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-000053a0: 696d 706f 7274 2063 6f64 6563 732c 206c  import codecs, l
-000053b0: 6f63 616c 650a 2020 2020 2020 2020 7379  ocale.        sy
-000053c0: 732e 7374 646f 7574 203d 2063 6f64 6563  s.stdout = codec
-000053d0: 732e 6765 7477 7269 7465 7228 6c6f 6361  s.getwriter(loca
-000053e0: 6c65 2e67 6574 7072 6566 6572 7265 6465  le.getpreferrede
-000053f0: 6e63 6f64 696e 6728 2929 2873 7973 2e73  ncoding())(sys.s
-00005400: 7464 6f75 742c 2272 6570 6c61 6365 2229  tdout,"replace")
-00005410: 3b0a 2020 2020 2020 2020 7379 732e 7374  ;.        sys.st
-00005420: 6465 7272 203d 2063 6f64 6563 732e 6765  derr = codecs.ge
-00005430: 7477 7269 7465 7228 6c6f 6361 6c65 2e67  twriter(locale.g
-00005440: 6574 7072 6566 6572 7265 6465 6e63 6f64  etpreferredencod
-00005450: 696e 6728 2929 2873 7973 2e73 7464 6572  ing())(sys.stder
-00005460: 722c 2272 6570 6c61 6365 2229 3b0a 0a20  r,"replace");.. 
-00005470: 2020 2069 6620 272d 2d72 6567 6973 7465     if '--registe
-00005480: 7227 2069 6e20 7379 732e 6172 6776 206f  r' in sys.argv o
-00005490: 7220 272d 2d75 6e72 6567 6973 7465 7227  r '--unregister'
-000054a0: 2069 6e20 7379 732e 6172 6776 3a0a 2020   in sys.argv:.  
-000054b0: 2020 2020 2020 696d 706f 7274 2070 7974        import pyt
-000054c0: 686f 6e63 6f6d 0a20 2020 2020 2020 2069  honcom.        i
-000054d0: 6d70 6f72 7420 7769 6e33 3263 6f6d 2e73  mport win32com.s
-000054e0: 6572 7665 722e 7265 6769 7374 6572 0a20  erver.register. 
-000054f0: 2020 2020 2020 2077 696e 3332 636f 6d2e         win32com.
-00005500: 7365 7276 6572 2e72 6567 6973 7465 722e  server.register.
-00005510: 5573 6543 6f6d 6d61 6e64 4c69 6e65 2854  UseCommandLine(T
-00005520: 7261 7a61 5665 7429 0a20 2020 2065 6c69  razaVet).    eli
-00005530: 6620 222f 4175 746f 6d61 7465 2220 696e  f "/Automate" in
-00005540: 2073 7973 2e61 7267 763a 0a20 2020 2020   sys.argv:.     
-00005550: 2020 2023 204d 5320 7365 656d 7320 746f     # MS seems to
-00005560: 206c 696b 6520 2f61 7574 6f6d 6174 6520   like /automate 
-00005570: 746f 2072 756e 2074 6865 2063 6c61 7373  to run the class
-00005580: 2066 6163 746f 7269 6573 2e0a 2020 2020   factories..    
-00005590: 2020 2020 696d 706f 7274 2077 696e 3332      import win32
-000055a0: 636f 6d2e 7365 7276 6572 2e6c 6f63 616c  com.server.local
-000055b0: 7365 7276 6572 0a20 2020 2020 2020 2023  server.        #
-000055c0: 7769 6e33 3263 6f6d 2e73 6572 7665 722e  win32com.server.
-000055d0: 6c6f 6361 6c73 6572 7665 722e 6d61 696e  localserver.main
-000055e0: 2829 0a20 2020 2020 2020 2023 2073 7461  ().        # sta
-000055f0: 7274 2074 6865 2073 6572 7665 722e 0a20  rt the server.. 
-00005600: 2020 2020 2020 2077 696e 3332 636f 6d2e         win32com.
-00005610: 7365 7276 6572 2e6c 6f63 616c 7365 7276  server.localserv
-00005620: 6572 2e73 6572 7665 285b 5472 617a 6156  er.serve([TrazaV
-00005630: 6574 2e5f 7265 675f 636c 7369 645f 5d29  et._reg_clsid_])
-00005640: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00005650: 2020 206d 6169 6e28 290a                    main().
+00001f90: 696f 6e27 3a20 6964 5f6d 6f74 6976 6f5f  ion': id_motivo_
+00001fa0: 6465 7374 7275 6363 696f 6e20 6f72 204e  destruccion or N
+00001fb0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00001fc0: 2020 2020 2020 2020 2027 6e5f 6d61 6e69           'n_mani
+00001fd0: 6669 6573 746f 273a 206e 5f6d 616e 6966  fiesto': n_manif
+00001fe0: 6965 7374 6f20 6f72 204e 6f6e 652c 0a20  iesto or None,. 
+00001ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002000: 2020 2027 656e 5f74 7261 6e73 706f 7274     'en_transport
+00002010: 6527 3a20 656e 5f74 7261 6e73 706f 7274  e': en_transport
+00002020: 6520 6f72 204e 6f6e 652c 0a20 2020 2020  e or None,.     
+00002030: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00002040: 6e5f 7265 6d69 746f 273a 206e 5f72 656d  n_remito': n_rem
+00002050: 6974 6f20 6f72 204e 6f6e 652c 0a20 2020  ito or None,.   
+00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002070: 2027 6d6f 7469 766f 5f64 6576 6f6c 7563   'motivo_devoluc
+00002080: 696f 6e27 3a20 6d6f 7469 766f 5f64 6576  ion': motivo_dev
+00002090: 6f6c 7563 696f 6e20 6f72 204e 6f6e 652c  olucion or None,
+000020a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000020b0: 2020 2020 2027 6f62 7365 7276 6163 696f       'observacio
+000020c0: 6e65 7327 3a20 6f62 7365 7276 6163 696f  nes': observacio
+000020d0: 6e65 7320 6f72 204e 6f6e 652c 0a20 2020  nes or None,.   
+000020e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020f0: 2027 6e5f 7661 6c65 5f63 6f6d 7072 6127   'n_vale_compra'
+00002100: 3a20 6e5f 7661 6c65 5f63 6f6d 7072 6120  : n_vale_compra 
+00002110: 6f72 204e 6f6e 652c 0a20 2020 2020 2020  or None,.       
+00002120: 2020 2020 2020 2020 2020 2020 2027 6170               'ap
+00002130: 656c 6c69 646f 4e6f 6d62 7265 7327 3a20  ellidoNombres': 
+00002140: 6170 656c 6c69 646f 4e6f 6d62 7265 7320  apellidoNombres 
+00002150: 6f72 204e 6f6e 652c 0a20 2020 2020 2020  or None,.       
+00002160: 2020 2020 2020 2020 2020 2020 2027 6469               'di
+00002170: 7265 6363 696f 6e27 3a20 6469 7265 6363  reccion': direcc
+00002180: 696f 6e20 6f72 204e 6f6e 652c 0a20 2020  ion or None,.   
+00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021a0: 2027 6e75 6d65 726f 273a 206e 756d 6572   'numero': numer
+000021b0: 6f20 6f72 204e 6f6e 652c 0a20 2020 2020  o or None,.     
+000021c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000021d0: 6c6f 6361 6c69 6461 6427 3a20 6c6f 6361  localidad': loca
+000021e0: 6c69 6461 6420 6f72 204e 6f6e 652c 0a20  lidad or None,. 
+000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002200: 2020 2027 7072 6f76 696e 6369 6127 3a20     'provincia': 
+00002210: 7072 6f76 696e 6369 6120 6f72 204e 6f6e  provincia or Non
+00002220: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00002230: 2020 2020 2020 2027 6e5f 706f 7374 616c         'n_postal
+00002240: 273a 206e 5f70 6f73 7461 6c20 6f72 204e  ': n_postal or N
+00002250: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00002260: 2020 2020 2020 2020 2027 6375 6974 273a           'cuit':
+00002270: 2063 7569 7420 6f72 204e 6f6e 652c 0a20   cuit or None,. 
+00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002290: 2020 207d 0a20 2020 2020 2020 2072 6573     }.        res
+000022a0: 203d 2073 656c 662e 636c 6965 6e74 2e73   = self.client.s
+000022b0: 6176 6554 7261 6e73 6163 6369 6f6e 6573  aveTransacciones
+000022c0: 280a 2020 2020 2020 2020 2020 2020 6172  (.            ar
+000022d0: 6730 3d70 6172 616d 732c 0a20 2020 2020  g0=params,.     
+000022e0: 2020 2020 2020 2061 7267 313d 7573 7561         arg1=usua
+000022f0: 7269 6f2c 0a20 2020 2020 2020 2020 2020  rio,.           
+00002300: 2061 7267 323d 7061 7373 776f 7264 2c0a   arg2=password,.
+00002310: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00002320: 2020 7265 7420 3d20 7265 735b 2772 6574    ret = res['ret
+00002330: 7572 6e27 5d0a 2020 2020 2020 2020 7365  urn'].        se
+00002340: 6c66 2e43 6f64 6967 6f54 7261 6e73 6163  lf.CodigoTransac
+00002350: 6369 6f6e 203d 2072 6574 2e67 6574 2827  cion = ret.get('
+00002360: 636f 6469 676f 5472 616e 7361 6363 696f  codigoTransaccio
+00002370: 6e27 290a 2020 2020 2020 2020 7365 6c66  n').        self
+00002380: 2e5f 5f61 6e61 6c69 7a61 725f 6572 726f  .__analizar_erro
+00002390: 7265 7328 7265 7429 0a20 2020 2020 2020  res(ret).       
+000023a0: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
+000023b0: 2020 4069 6e69 6369 616c 697a 6172 5f79    @inicializar_y
+000023c0: 5f63 6170 7475 7261 725f 6578 6365 7063  _capturar_excepc
+000023d0: 696f 6e65 730a 2020 2020 6465 6620 5365  iones.    def Se
+000023e0: 6e64 4361 6e63 656c 6154 7261 6e73 6163  ndCancelaTransac
+000023f0: 2873 656c 662c 2075 7375 6172 696f 2c20  (self, usuario, 
+00002400: 7061 7373 776f 7264 2c20 636f 6469 676f  password, codigo
+00002410: 5f74 7261 6e73 6163 6369 6f6e 293a 0a20  _transaccion):. 
+00002420: 2020 2020 2020 2022 2052 6561 6c69 7a61         " Realiza
+00002430: 206c 6120 6361 6e63 656c 6163 69f3 6e20   la cancelaci.n 
+00002440: 6465 2075 6e61 2074 7261 6e73 6163 6369  de una transacci
+00002450: f36e 220a 2020 2020 2020 2020 7265 7320  .n".        res 
+00002460: 3d20 7365 6c66 2e63 6c69 656e 742e 7365  = self.client.se
+00002470: 6e64 4361 6e63 656c 6154 7261 6e73 6163  ndCancelaTransac
+00002480: 280a 2020 2020 2020 2020 2020 2020 6172  (.            ar
+00002490: 6730 3d63 6f64 6967 6f5f 7472 616e 7361  g0=codigo_transa
+000024a0: 6363 696f 6e2c 0a20 2020 2020 2020 2020  ccion,.         
+000024b0: 2020 2061 7267 313d 7573 7561 7269 6f2c     arg1=usuario,
+000024c0: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
+000024d0: 323d 7061 7373 776f 7264 2c0a 2020 2020  2=password,.    
+000024e0: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
+000024f0: 7420 3d20 7265 735b 2772 6574 7572 6e27  t = res['return'
+00002500: 5d0a 2020 2020 2020 2020 7365 6c66 2e43  ].        self.C
+00002510: 6f64 6967 6f54 7261 6e73 6163 6369 6f6e  odigoTransaccion
+00002520: 203d 2072 6574 2e67 6574 2827 636f 6469   = ret.get('codi
+00002530: 676f 5472 616e 7361 6363 696f 6e27 290a  goTransaccion').
+00002540: 2020 2020 2020 2020 7365 6c66 2e5f 5f61          self.__a
+00002550: 6e61 6c69 7a61 725f 6572 726f 7265 7328  nalizar_errores(
+00002560: 7265 7429 0a20 2020 2020 2020 2072 6574  ret).        ret
+00002570: 7572 6e20 5472 7565 0a0a 2020 2020 4069  urn True..    @i
+00002580: 6e69 6369 616c 697a 6172 5f79 5f63 6170  nicializar_y_cap
+00002590: 7475 7261 725f 6578 6365 7063 696f 6e65  turar_excepcione
+000025a0: 730a 2020 2020 6465 6620 5365 6e64 436f  s.    def SendCo
+000025b0: 6e66 6972 6d61 5472 616e 7361 6363 2873  nfirmaTransacc(s
+000025c0: 656c 662c 2075 7375 6172 696f 2c20 7061  elf, usuario, pa
+000025d0: 7373 776f 7264 2c20 705f 6964 735f 7472  ssword, p_ids_tr
+000025e0: 616e 7361 632c 2066 5f6f 7065 7261 6369  ansac, f_operaci
+000025f0: 6f6e 2c20 6e5f 6361 6e74 6964 6164 3d4e  on, n_cantidad=N
+00002600: 6f6e 6529 3a0a 2020 2020 2020 2020 2243  one):.        "C
+00002610: 6f6e 6669 726d 6120 6c61 2072 6563 6570  onfirma la recep
+00002620: 6369 f36e 2064 6520 756e 206d 6564 6963  ci.n de un medic
+00002630: 616d 656e 746f 220a 2020 2020 2020 2020  amento".        
+00002640: 7265 7320 3d20 7365 6c66 2e63 6c69 656e  res = self.clien
+00002650: 742e 7365 6e64 436f 6e66 6972 6d61 5472  t.sendConfirmaTr
+00002660: 616e 7361 6363 280a 2020 2020 2020 2020  ansacc(.        
+00002670: 2020 2020 6172 6730 3d75 7375 6172 696f      arg0=usuario
+00002680: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
+00002690: 6731 3d70 6173 7377 6f72 642c 0a20 2020  g1=password,.   
+000026a0: 2020 2020 2020 2020 2061 7267 323d 7b27           arg2={'
+000026b0: 705f 6964 735f 7472 616e 7361 6327 3a20  p_ids_transac': 
+000026c0: 705f 6964 735f 7472 616e 7361 632c 2027  p_ids_transac, '
+000026d0: 665f 6f70 6572 6163 696f 6e27 3a20 665f  f_operacion': f_
+000026e0: 6f70 6572 6163 696f 6e2c 0a20 2020 2020  operacion,.     
+000026f0: 2020 2020 2020 2020 2020 2020 2027 6e5f               'n_
+00002700: 6361 6e74 6964 6164 273a 206e 5f63 616e  cantidad': n_can
+00002710: 7469 6461 642c 0a20 2020 2020 2020 2020  tidad,.         
+00002720: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00002730: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
+00002740: 203d 2072 6573 5b27 7265 7475 726e 275d   = res['return']
+00002750: 0a20 2020 2020 2020 2073 656c 662e 436f  .        self.Co
+00002760: 6469 676f 5472 616e 7361 6363 696f 6e20  digoTransaccion 
+00002770: 3d20 7265 742e 6765 7428 2763 6f64 6967  = ret.get('codig
+00002780: 6f54 7261 6e73 6163 6369 6f6e 2729 0a20  oTransaccion'). 
+00002790: 2020 2020 2020 2073 656c 662e 5f5f 616e         self.__an
+000027a0: 616c 697a 6172 5f65 7272 6f72 6573 2872  alizar_errores(r
+000027b0: 6574 290a 2020 2020 2020 2020 7265 7475  et).        retu
+000027c0: 726e 2054 7275 650a 0a20 2020 2040 696e  rn True..    @in
+000027d0: 6963 6961 6c69 7a61 725f 795f 6361 7074  icializar_y_capt
+000027e0: 7572 6172 5f65 7863 6570 6369 6f6e 6573  urar_excepciones
+000027f0: 0a20 2020 2064 6566 2053 656e 6441 6c65  .    def SendAle
+00002800: 7274 6154 7261 6e73 6163 6328 7365 6c66  rtaTransacc(self
+00002810: 2c20 7573 7561 7269 6f2c 2070 6173 7377  , usuario, passw
+00002820: 6f72 642c 2070 5f69 6473 5f74 7261 6e73  ord, p_ids_trans
+00002830: 6163 5f77 7329 3a0a 2020 2020 2020 2020  ac_ws):.        
+00002840: 2241 6c65 7274 6120 756e 206d 6564 6963  "Alerta un medic
+00002850: 616d 656e 746f 2c20 6163 6369 f36e 2063  amento, acci.n c
+00002860: 6f6e 7472 6172 6961 2061 2093 636f 6e66  ontraria a .conf
+00002870: 6972 6d61 7220 6c61 2074 7261 6e73 6163  irmar la transac
+00002880: 6369 f36e 942e 220a 2020 2020 2020 2020  ci.n..".        
+00002890: 7265 7320 3d20 7365 6c66 2e63 6c69 656e  res = self.clien
+000028a0: 742e 7365 6e64 416c 6572 7461 5472 616e  t.sendAlertaTran
+000028b0: 7361 6363 280a 2020 2020 2020 2020 2020  sacc(.          
+000028c0: 2020 6172 6730 3d75 7375 6172 696f 2c0a    arg0=usuario,.
+000028d0: 2020 2020 2020 2020 2020 2020 6172 6731              arg1
+000028e0: 3d70 6173 7377 6f72 642c 0a20 2020 2020  =password,.     
+000028f0: 2020 2020 2020 2061 7267 323d 705f 6964         arg2=p_id
+00002900: 735f 7472 616e 7361 635f 7773 2c0a 2020  s_transac_ws,.  
+00002910: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00002920: 7265 7420 3d20 7265 735b 2772 6574 7572  ret = res['retur
+00002930: 6e27 5d0a 2020 2020 2020 2020 7365 6c66  n'].        self
+00002940: 2e43 6f64 6967 6f54 7261 6e73 6163 6369  .CodigoTransacci
+00002950: 6f6e 203d 2072 6574 2e67 6574 2827 6964  on = ret.get('id
+00002960: 5f74 7261 6e73 6163 5f61 736f 6369 6164  _transac_asociad
+00002970: 6127 290a 2020 2020 2020 2020 7365 6c66  a').        self
+00002980: 2e5f 5f61 6e61 6c69 7a61 725f 6572 726f  .__analizar_erro
+00002990: 7265 7328 7265 7429 0a20 2020 2020 2020  res(ret).       
+000029a0: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
+000029b0: 2020 4069 6e69 6369 616c 697a 6172 5f79    @inicializar_y
+000029c0: 5f63 6170 7475 7261 725f 6578 6365 7063  _capturar_excepc
+000029d0: 696f 6e65 730a 2020 2020 6465 6620 4765  iones.    def Ge
+000029e0: 7454 7261 6e73 6163 6369 6f6e 6573 2873  tTransacciones(s
+000029f0: 656c 662c 2075 7375 6172 696f 2c20 7061  elf, usuario, pa
+00002a00: 7373 776f 7264 2c0a 2020 2020 2020 2020  ssword,.        
+00002a10: 2020 2020 2020 2020 6964 5f74 7261 6e73          id_trans
+00002a20: 6163 6369 6f6e 3d4e 6f6e 652c 2069 645f  accion=None, id_
+00002a30: 6576 656e 746f 3d4e 6f6e 652c 2067 6c6e  evento=None, gln
+00002a40: 5f6f 7269 6765 6e3d 4e6f 6e65 2c0a 2020  _origen=None,.  
+00002a50: 2020 2020 2020 2020 2020 2020 2020 6665                fe
+00002a60: 6368 615f 6465 7364 655f 743d 4e6f 6e65  cha_desde_t=None
+00002a70: 2c20 6665 6368 615f 6861 7374 615f 743d  , fecha_hasta_t=
+00002a80: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00002a90: 2020 2020 2020 6665 6368 615f 6465 7364        fecha_desd
+00002aa0: 655f 763d 4e6f 6e65 2c20 6665 6368 615f  e_v=None, fecha_
+00002ab0: 6861 7374 615f 763d 4e6f 6e65 2c0a 2020  hasta_v=None,.  
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 676c                gl
+00002ad0: 6e5f 696e 666f 726d 6164 6f72 3d4e 6f6e  n_informador=Non
+00002ae0: 652c 2069 645f 7469 706f 5f74 7261 6e73  e, id_tipo_trans
+00002af0: 6163 6369 6f6e 3d4e 6f6e 652c 0a20 2020  accion=None,.   
+00002b00: 2020 2020 2020 2020 2020 2020 2067 7469               gti
+00002b10: 6e5f 656c 656d 656e 746f 3d4e 6f6e 652c  n_elemento=None,
+00002b20: 206e 5f6c 6f74 653d 4e6f 6e65 2c20 6e5f   n_lote=None, n_
+00002b30: 7365 7269 653d 4e6f 6e65 2c0a 2020 2020  serie=None,.    
+00002b40: 2020 2020 2020 2020 2020 2020 6e5f 7265              n_re
+00002b50: 6d69 746f 5f66 6163 7475 7261 3d4e 6f6e  mito_factura=Non
+00002b60: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00002b70: 2020 2029 3a0a 2020 2020 2020 2020 2254     ):.        "T
+00002b80: 7261 6520 756e 206c 6973 7461 646f 2064  rae un listado d
+00002b90: 6520 6c61 7320 7472 616e 7361 6363 696f  e las transaccio
+00002ba0: 6e65 7320 7175 6520 6e6f 2065 7374 e16e  nes que no est.n
+00002bb0: 2063 6f6e 6669 726d 6164 6173 220a 0a20   confirmadas".. 
+00002bc0: 2020 2020 2020 2023 2070 7265 7061 726f         # preparo
+00002bd0: 206c 6f73 2070 6172 616d 6574 726f 7320   los parametros 
+00002be0: 6465 2065 6e74 7261 6461 206f 7063 696f  de entrada opcio
+00002bf0: 6e61 6c65 733a 0a20 2020 2020 2020 206b  nales:.        k
+00002c00: 7761 7267 7320 3d20 7b7d 0a20 2020 2020  wargs = {}.     
+00002c10: 2020 2069 6620 6964 5f74 7261 6e73 6163     if id_transac
+00002c20: 6369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  cion is not None
+00002c30: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
+00002c40: 6172 6773 5b27 6172 6732 275d 203d 2069  args['arg2'] = i
+00002c50: 645f 7472 616e 7361 6363 696f 6e0a 2020  d_transaccion.  
+00002c60: 2020 2020 2020 6966 2069 645f 6576 656e        if id_even
+00002c70: 746f 2069 7320 6e6f 7420 4e6f 6e65 3a0a  to is not None:.
+00002c80: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
+00002c90: 6773 5b27 6172 6733 275d 203d 2069 645f  gs['arg3'] = id_
+00002ca0: 6576 656e 746f 0a20 2020 2020 2020 2069  evento.        i
+00002cb0: 6620 676c 6e5f 6f72 6967 656e 2069 7320  f gln_origen is 
+00002cc0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00002cd0: 2020 2020 2020 6b77 6172 6773 5b27 6172        kwargs['ar
+00002ce0: 6734 275d 203d 2067 6c6e 5f6f 7269 6765  g4'] = gln_orige
+00002cf0: 6e0a 2020 2020 2020 2020 6966 2066 6563  n.        if fec
+00002d00: 6861 5f64 6573 6465 5f74 2069 7320 6e6f  ha_desde_t is no
+00002d10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00002d20: 2020 2020 6b77 6172 6773 5b27 6172 6735      kwargs['arg5
+00002d30: 275d 203d 2066 6563 6861 5f64 6573 6465  '] = fecha_desde
+00002d40: 5f74 0a20 2020 2020 2020 2069 6620 6665  _t.        if fe
+00002d50: 6368 615f 6861 7374 615f 7420 6973 206e  cha_hasta_t is n
+00002d60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00002d70: 2020 2020 206b 7761 7267 735b 2761 7267       kwargs['arg
+00002d80: 3627 5d20 3d20 6665 6368 615f 6861 7374  6'] = fecha_hast
+00002d90: 615f 740a 2020 2020 2020 2020 6966 2066  a_t.        if f
+00002da0: 6563 6861 5f64 6573 6465 5f76 2069 7320  echa_desde_v is 
+00002db0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00002dc0: 2020 2020 2020 6b77 6172 6773 5b27 6172        kwargs['ar
+00002dd0: 6737 275d 203d 2066 6563 6861 5f64 6573  g7'] = fecha_des
+00002de0: 6465 5f76 0a20 2020 2020 2020 2069 6620  de_v.        if 
+00002df0: 6665 6368 615f 6861 7374 615f 7620 6973  fecha_hasta_v is
+00002e00: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00002e10: 2020 2020 2020 206b 7761 7267 735b 2761         kwargs['a
+00002e20: 7267 3827 5d20 3d20 6665 6368 615f 6861  rg8'] = fecha_ha
+00002e30: 7374 615f 760a 2020 2020 2020 2020 6966  sta_v.        if
+00002e40: 2067 6c6e 5f69 6e66 6f72 6d61 646f 7220   gln_informador 
+00002e50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00002e60: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
+00002e70: 2761 7267 3927 5d20 3d20 676c 6e5f 696e  'arg9'] = gln_in
+00002e80: 666f 726d 6164 6f72 0a20 2020 2020 2020  formador.       
+00002e90: 2069 6620 6964 5f74 6970 6f5f 7472 616e   if id_tipo_tran
+00002ea0: 7361 6363 696f 6e20 6973 206e 6f74 204e  saccion is not N
+00002eb0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00002ec0: 206b 7761 7267 735b 2761 7267 3130 275d   kwargs['arg10']
+00002ed0: 203d 2069 645f 7469 706f 5f74 7261 6e73   = id_tipo_trans
+00002ee0: 6163 6369 6f6e 0a20 2020 2020 2020 2069  accion.        i
+00002ef0: 6620 6774 696e 5f65 6c65 6d65 6e74 6f20  f gtin_elemento 
+00002f00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00002f10: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
+00002f20: 2761 7267 3131 275d 203d 2067 7469 6e5f  'arg11'] = gtin_
+00002f30: 656c 656d 656e 746f 0a20 2020 2020 2020  elemento.       
+00002f40: 2069 6620 6e5f 6c6f 7465 2069 7320 6e6f   if n_lote is no
+00002f50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00002f60: 2020 2020 6b77 6172 6773 5b27 6172 6731      kwargs['arg1
+00002f70: 3227 5d20 3d20 6e5f 6c6f 7465 0a20 2020  2'] = n_lote.   
+00002f80: 2020 2020 2069 6620 6e5f 7365 7269 6520       if n_serie 
+00002f90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00002fa0: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
+00002fb0: 2761 7267 3133 275d 203d 206e 5f73 6572  'arg13'] = n_ser
+00002fc0: 6965 0a20 2020 2020 2020 2069 6620 6e5f  ie.        if n_
+00002fd0: 7265 6d69 746f 5f66 6163 7475 7261 2069  remito_factura i
+00002fe0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00002ff0: 2020 2020 2020 2020 6b77 6172 6773 5b27          kwargs['
+00003000: 6172 6731 3427 5d20 3d20 6e5f 7265 6d69  arg14'] = n_remi
+00003010: 746f 5f66 6163 7475 7261 0a0a 2020 2020  to_factura..    
+00003020: 2020 2020 2320 6c6c 616d 6f20 616c 2077      # llamo al w
+00003030: 6562 7365 7276 6963 650a 2020 2020 2020  ebservice.      
+00003040: 2020 7265 7320 3d20 7365 6c66 2e63 6c69    res = self.cli
+00003050: 656e 742e 6765 7454 7261 6e73 6163 6369  ent.getTransacci
+00003060: 6f6e 6573 280a 2020 2020 2020 2020 2020  ones(.          
+00003070: 2020 6172 6730 3d75 7375 6172 696f 2c0a    arg0=usuario,.
+00003080: 2020 2020 2020 2020 2020 2020 6172 6731              arg1
+00003090: 3d70 6173 7377 6f72 642c 0a20 2020 2020  =password,.     
+000030a0: 2020 2020 2020 202a 2a6b 7761 7267 730a         **kwargs.
+000030b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000030c0: 2020 7265 7420 3d20 7265 735b 2772 6574    ret = res['ret
+000030d0: 7572 6e27 5d0a 2020 2020 2020 2020 6966  urn'].        if
+000030e0: 2072 6574 3a0a 2020 2020 2020 2020 2020   ret:.          
+000030f0: 2020 7365 6c66 2e5f 5f61 6e61 6c69 7a61    self.__analiza
+00003100: 725f 6572 726f 7265 7328 7265 7429 0a20  r_errores(ret). 
+00003110: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003120: 4361 6e74 5061 6769 6e61 7320 3d20 7265  CantPaginas = re
+00003130: 742e 6765 7428 2763 616e 7450 6167 696e  t.get('cantPagin
+00003140: 6173 2729 0a20 2020 2020 2020 2020 2020  as').           
+00003150: 2073 656c 662e 4861 7945 7272 6f72 203d   self.HayError =
+00003160: 2072 6574 2e67 6574 2827 6861 795f 6572   ret.get('hay_er
+00003170: 726f 7227 290a 2020 2020 2020 2020 2020  ror').          
+00003180: 2020 7365 6c66 2e54 7261 6e73 6163 6369    self.Transacci
+00003190: 6f6e 5365 6e61 7361 203d 205b 6974 2066  onSenasa = [it f
+000031a0: 6f72 2069 7420 696e 2072 6574 2e67 6574  or it in ret.get
+000031b0: 2827 6c69 7374 272c 205b 5d29 5d0a 2020  ('list', [])].  
+000031c0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+000031d0: 650a 0a20 2020 2064 6566 2020 4c65 6572  e..    def  Leer
+000031e0: 5472 616e 7361 6363 696f 6e28 7365 6c66  Transaccion(self
+000031f0: 293a 0a20 2020 2020 2020 2022 5265 636f  ):.        "Reco
+00003200: 7272 6f20 5472 616e 7361 6363 696f 6e53  rro TransaccionS
+00003210: 656e 6173 6120 6465 7675 656c 746f 2070  enasa devuelto p
+00003220: 6f72 2047 6574 5472 616e 7361 6363 696f  or GetTransaccio
+00003230: 6e65 7322 0a20 2020 2020 2020 2020 2320  nes".         # 
+00003240: 7573 6172 2047 6574 5061 7261 6d65 7472  usar GetParametr
+00003250: 6f20 7061 7261 2063 6f6e 7375 6c74 6172  o para consultar
+00003260: 2065 6c20 7661 6c6f 7220 7265 746f 726e   el valor retorn
+00003270: 6164 6f20 706f 7220 656c 2077 6562 7365  ado por el webse
+00003280: 7276 6963 650a 0a20 2020 2020 2020 2069  rvice..        i
+00003290: 6620 7365 6c66 2e54 7261 6e73 6163 6369  f self.Transacci
+000032a0: 6f6e 5365 6e61 7361 3a0a 2020 2020 2020  onSenasa:.      
+000032b0: 2020 2020 2020 2320 6578 7472 6169 676f        # extraigo
+000032c0: 2065 6c20 7072 696d 6572 2069 7465 6d0a   el primer item.
+000032d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000032e0: 2e70 6172 616d 735f 6f75 7420 3d20 7365  .params_out = se
+000032f0: 6c66 2e54 7261 6e73 6163 6369 6f6e 5365  lf.TransaccionSe
+00003300: 6e61 7361 2e70 6f70 2830 290a 2020 2020  nasa.pop(0).    
+00003310: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00003320: 7275 650a 2020 2020 2020 2020 656c 7365  rue.        else
+00003330: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00003340: 6c69 6d70 696f 206c 6f73 2070 6172 e16d  limpio los par.m
+00003350: 6574 726f 730a 2020 2020 2020 2020 2020  etros.          
+00003360: 2020 7365 6c66 2e70 6172 616d 735f 6f75    self.params_ou
+00003370: 7420 3d20 7b7d 0a20 2020 2020 2020 2020  t = {}.         
+00003380: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00003390: 0a20 2020 2064 6566 204c 6565 7245 7272  .    def LeerErr
+000033a0: 6f72 2873 656c 6629 3a0a 2020 2020 2020  or(self):.      
+000033b0: 2020 2252 6563 6f72 726f 206c 6f73 2065    "Recorro los e
+000033c0: 7272 6f72 6573 2064 6576 7565 6c74 6f73  rrores devueltos
+000033d0: 2079 2064 6576 7565 6c76 6f20 656c 2070   y devuelvo el p
+000033e0: 7269 6d65 726f 2073 6920 6578 6973 7465  rimero si existe
+000033f0: 220a 0a20 2020 2020 2020 2069 6620 7365  "..        if se
+00003400: 6c66 2e45 7272 6f72 6573 3a0a 2020 2020  lf.Errores:.    
+00003410: 2020 2020 2020 2020 2320 6578 7472 6169          # extrai
+00003420: 676f 2065 6c20 7072 696d 6572 2069 7465  go el primer ite
+00003430: 6d0a 2020 2020 2020 2020 2020 2020 6572  m.            er
+00003440: 203d 2073 656c 662e 4572 726f 7265 732e   = self.Errores.
+00003450: 706f 7028 3029 0a20 2020 2020 2020 2020  pop(0).         
+00003460: 2020 2072 6574 7572 6e20 6572 0a20 2020     return er.   
+00003470: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00003480: 2020 2020 2020 2072 6574 7572 6e20 2222         return ""
+00003490: 0a0a 2020 2020 6465 6620 5365 7455 7365  ..    def SetUse
+000034a0: 726e 616d 6528 7365 6c66 2c20 7573 6572  rname(self, user
+000034b0: 6e61 6d65 293a 0a20 2020 2020 2020 2022  name):.        "
+000034c0: 4573 7461 626c 657a 636f 2065 6c20 6e6f  Establezco el no
+000034d0: 6d62 7265 2064 6520 7573 7561 7269 6f22  mbre de usuario"
+000034e0: 0a20 2020 2020 2020 2073 656c 662e 5573  .        self.Us
+000034f0: 6572 6e61 6d65 203d 2075 7365 726e 616d  ername = usernam
+00003500: 650a 0a20 2020 2064 6566 2053 6574 5061  e..    def SetPa
+00003510: 7373 776f 7264 2873 656c 662c 2070 6173  ssword(self, pas
+00003520: 7377 6f72 6429 3a0a 2020 2020 2020 2020  sword):.        
+00003530: 2245 7374 6162 6c65 7a63 6f20 6c61 2063  "Establezco la c
+00003540: 6f6e 7472 6173 65f1 6122 0a20 2020 2020  ontrase.a".     
+00003550: 2020 2073 656c 662e 5061 7373 776f 7264     self.Password
+00003560: 203d 2070 6173 7377 6f72 640a 0a20 2020   = password..   
+00003570: 2064 6566 2047 6574 436f 6469 676f 5472   def GetCodigoTr
+00003580: 616e 7361 6363 696f 6e28 7365 6c66 293a  ansaccion(self):
+00003590: 0a20 2020 2020 2020 2022 4465 7675 656c  .        "Devuel
+000035a0: 766f 2065 6c20 63f3 6469 676f 2064 6520  vo el c.digo de 
+000035b0: 7472 616e 7361 6363 69f3 6e22 0a20 2020  transacci.n".   
+000035c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000035d0: 2e43 6f64 6967 6f54 7261 6e73 6163 6369  .CodigoTransacci
+000035e0: 6f6e 0a0a 2020 2020 6465 6620 4765 7452  on..    def GetR
+000035f0: 6573 756c 7461 646f 2873 656c 6629 3a0a  esultado(self):.
+00003600: 2020 2020 2020 2020 2244 6576 7565 6c76          "Devuelv
+00003610: 6f20 656c 2072 6573 756c 7461 646f 220a  o el resultado".
+00003620: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00003630: 656c 662e 5265 7375 6c74 6164 6f0a 0a0a  elf.Resultado...
+00003640: 6465 6620 6d61 696e 2829 3a0a 2020 2020  def main():.    
+00003650: 2246 756e 6369 f36e 2070 7269 6e63 6970  "Funci.n princip
+00003660: 616c 2064 6520 7072 7565 6261 7320 286f  al de pruebas (o
+00003670: 6274 656e 6572 2043 4145 2922 0a20 2020  btener CAE)".   
+00003680: 2069 6d70 6f72 7420 6f73 2c20 7469 6d65   import os, time
+00003690: 2c20 7379 730a 2020 2020 676c 6f62 616c  , sys.    global
+000036a0: 2057 5344 4c2c 204c 4f43 4154 494f 4e0a   WSDL, LOCATION.
+000036b0: 0a20 2020 2044 4542 5547 203d 2027 2d2d  .    DEBUG = '--
+000036c0: 6465 6275 6727 2069 6e20 7379 732e 6172  debug' in sys.ar
+000036d0: 6776 0a0a 2020 2020 7773 203d 2054 7261  gv..    ws = Tra
+000036e0: 7a61 5665 7428 290a 0a20 2020 2077 732e  zaVet()..    ws.
+000036f0: 5573 6572 6e61 6d65 203d 2027 7465 7374  Username = 'test
+00003700: 7773 6572 7669 6365 270a 2020 2020 7773  wservice'.    ws
+00003710: 2e50 6173 7377 6f72 6420 3d20 2774 6573  .Password = 'tes
+00003720: 7477 7365 7276 6963 6570 7377 270a 0a20  twservicepsw'.. 
+00003730: 2020 2069 6620 272d 2d70 726f 6427 2069     if '--prod' i
+00003740: 6e20 7379 732e 6172 6776 2061 6e64 206e  n sys.argv and n
+00003750: 6f74 2048 4f4d 4f3a 0a20 2020 2020 2020  ot HOMO:.       
+00003760: 2057 5344 4c20 3d20 2268 7474 7073 3a2f   WSDL = "https:/
+00003770: 2f73 6572 7669 6369 6f73 2e70 616d 692e  /servicios.pami.
+00003780: 6f72 672e 6172 2f74 7261 7a61 7665 742e  org.ar/trazavet.
+00003790: 5765 6253 6572 7669 6365 3f77 7364 6c22  WebService?wsdl"
+000037a0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+000037b0: 5573 616e 646f 2057 5344 4c3a 222c 2057  Usando WSDL:", W
+000037c0: 5344 4c29 0a20 2020 2020 2020 2073 7973  SDL).        sys
+000037d0: 2e61 7267 762e 706f 7028 7379 732e 6172  .argv.pop(sys.ar
+000037e0: 6776 2e69 6e64 6578 2822 2d2d 7072 6f64  gv.index("--prod
+000037f0: 2229 290a 0a20 2020 2069 6620 272d 2d70  "))..    if '--p
+00003800: 726f 7879 2720 696e 2073 7973 2e61 7267  roxy' in sys.arg
+00003810: 7620 616e 6420 6e6f 7420 484f 4d4f 3a0a  v and not HOMO:.
+00003820: 2020 2020 2020 2020 7072 6f78 7920 3d20          proxy = 
+00003830: 7379 732e 6172 6776 2e70 6f70 2873 7973  sys.argv.pop(sys
+00003840: 2e61 7267 762e 696e 6465 7828 222d 2d70  .argv.index("--p
+00003850: 726f 7879 2229 202b 2031 290a 2020 2020  roxy") + 1).    
+00003860: 2020 2020 7072 696e 7428 2255 7361 6e64      print("Usand
+00003870: 6f20 7072 6f78 793a 222c 2070 726f 7879  o proxy:", proxy
+00003880: 290a 2020 2020 2020 2020 7379 732e 6172  ).        sys.ar
+00003890: 6776 2e70 6f70 2873 7973 2e61 7267 762e  gv.pop(sys.argv.
+000038a0: 696e 6465 7828 222d 2d70 726f 7879 2229  index("--proxy")
+000038b0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+000038c0: 2020 2020 7072 6f78 7920 3d20 4e6f 6e65      proxy = None
+000038d0: 0a0a 2020 2020 2320 496e 6963 6961 6c69  ..    # Iniciali
+000038e0: 7a6f 206c 6173 2076 6172 6961 626c 6573  zo las variables
+000038f0: 2079 2065 7374 7275 6374 7572 6173 2070   y estructuras p
+00003900: 6172 6120 656c 2061 7263 6869 766f 2064  ara el archivo d
+00003910: 6520 696e 7465 7263 616d 6269 6f3a 0a20  e intercambio:. 
+00003920: 2020 2074 7261 6e73 6163 6369 6f6e 5f64     transaccion_d
+00003930: 746f 203d 205b 5d0a 2020 2020 7472 616e  to = [].    tran
+00003940: 7361 6363 696f 6e65 7320 3d20 5b5d 0a20  sacciones = []. 
+00003950: 2020 2065 7272 6f72 6573 203d 205b 5d0a     errores = [].
+00003960: 2020 2020 666f 726d 6174 6f73 203d 205b      formatos = [
+00003970: 2827 5472 616e 7361 6363 696f 6e44 544f  ('TransaccionDTO
+00003980: 272c 2054 5241 4e53 4143 4349 4f4e 5f44  ', TRANSACCION_D
+00003990: 544f 2c20 7472 616e 7361 6363 696f 6e5f  TO, transaccion_
+000039a0: 6474 6f29 2c0a 2020 2020 2020 2020 2020  dto),.          
+000039b0: 2020 2020 2020 2827 5472 616e 7361 6363        ('Transacc
+000039c0: 696f 6e65 7327 2c20 5452 414e 5341 4343  iones', TRANSACC
+000039d0: 494f 4e45 532c 2074 7261 6e73 6163 6369  IONES, transacci
+000039e0: 6f6e 6573 292c 0a20 2020 2020 2020 2020  ones),.         
+000039f0: 2020 2020 2020 2028 2745 7272 6f72 6573         ('Errores
+00003a00: 272c 2045 5252 4f52 4553 2c20 6572 726f  ', ERRORES, erro
+00003a10: 7265 7329 2c0a 2020 2020 2020 2020 2020  res),.          
+00003a20: 2020 2020 205d 0a0a 2020 2020 6966 2027       ]..    if '
+00003a30: 2d2d 666f 726d 6174 6f27 2069 6e20 7379  --formato' in sy
+00003a40: 732e 6172 6776 3a0a 2020 2020 2020 2020  s.argv:.        
+00003a50: 7072 696e 7428 2246 6f72 6d61 746f 3a22  print("Formato:"
+00003a60: 290a 2020 2020 2020 2020 666f 7220 6d73  ).        for ms
+00003a70: 672c 2066 6f72 6d61 746f 2c20 6c69 7374  g, formato, list
+00003a80: 6120 696e 2066 6f72 6d61 746f 733a 0a20  a in formatos:. 
+00003a90: 2020 2020 2020 2020 2020 2063 6f6d 6965             comie
+00003aa0: 6e7a 6f20 3d20 310a 2020 2020 2020 2020  nzo = 1.        
+00003ab0: 2020 2020 7072 696e 7428 223d 3d3d 2025      print("=== %
+00003ac0: 7320 3d3d 3d22 2025 206d 7367 290a 2020  s ===" % msg).  
+00003ad0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00003ae0: 227c 7c20 252d 3235 7320 7c7c 2025 2d31  "|| %-25s || %-1
+00003af0: 3273 207c 7c20 252d 3573 207c 7c20 252d  2s || %-5s || %-
+00003b00: 3473 207c 7c20 252d 3130 7320 7c7c 2220  4s || %-10s ||" 
+00003b10: 2520 280a 2020 2020 2020 2020 2020 2020  % (.            
+00003b20: 2020 2020 224e 6f6d 6272 6522 2c20 2254      "Nombre", "T
+00003b30: 6970 6f22 2c20 224c 6f6e 672e 222c 2022  ipo", "Long.", "
+00003b40: 506f 7328 7478 7429 222c 2022 4361 6d70  Pos(txt)", "Camp
+00003b50: 6f28 6462 6629 2229 290a 2020 2020 2020  o(dbf)")).      
+00003b60: 2020 2020 2020 636c 6176 6573 203d 205b        claves = [
+00003b70: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+00003b80: 7220 666d 7420 696e 2066 6f72 6d61 746f  r fmt in formato
+00003b90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003ba0: 2020 636c 6176 652c 206c 6f6e 6769 7475    clave, longitu
+00003bb0: 642c 2074 6970 6f20 3d20 666d 745b 303a  d, tipo = fmt[0:
+00003bc0: 335d 0a20 2020 2020 2020 2020 2020 2020  3].             
+00003bd0: 2020 2063 6c61 7665 5f64 6266 203d 2064     clave_dbf = d
+00003be0: 6172 5f6e 6f6d 6272 655f 6361 6d70 6f5f  ar_nombre_campo_
+00003bf0: 6462 6628 636c 6176 652c 2063 6c61 7665  dbf(clave, clave
+00003c00: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+00003c10: 2020 2063 6c61 7665 732e 6170 7065 6e64     claves.append
+00003c20: 2863 6c61 7665 5f64 6266 290a 2020 2020  (clave_dbf).    
+00003c30: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00003c40: 7428 227c 7c20 252d 3235 7320 7c7c 2025  t("|| %-25s || %
+00003c50: 2d31 3273 207c 7c20 2535 6420 7c7c 2020  -12s || %5d ||  
+00003c60: 2025 3464 2020 207c 7c20 252d 3130 7320   %4d   || %-10s 
+00003c70: 7c7c 2220 2520 280a 2020 2020 2020 2020  ||" % (.        
+00003c80: 2020 2020 2020 2020 2020 2020 636c 6176              clav
+00003c90: 652c 2074 6970 6f2c 206c 6f6e 6769 7475  e, tipo, longitu
+00003ca0: 642c 2063 6f6d 6965 6e7a 6f2c 2063 6c61  d, comienzo, cla
+00003cb0: 7665 5f64 6266 2929 0a20 2020 2020 2020  ve_dbf)).       
+00003cc0: 2020 2020 2020 2020 2063 6f6d 6965 6e7a           comienz
+00003cd0: 6f20 2b3d 206c 6f6e 6769 7475 640a 2020  o += longitud.  
+00003ce0: 2020 2020 2020 7379 732e 6578 6974 2830        sys.exit(0
+00003cf0: 290a 0a20 2020 2069 6620 272d 2d63 6172  )..    if '--car
+00003d00: 6761 7227 2069 6e20 7379 732e 6172 6776  gar' in sys.argv
+00003d10: 3a0a 2020 2020 2020 2020 6966 2027 2d2d  :.        if '--
+00003d20: 6462 6627 2069 6e20 7379 732e 6172 6776  dbf' in sys.argv
+00003d30: 3a0a 2020 2020 2020 2020 2020 2020 6c65  :.            le
+00003d40: 6572 5f64 6266 2866 6f72 6d61 746f 735b  er_dbf(formatos[
+00003d50: 3a31 5d2c 207b 7d29 0a20 2020 2020 2020  :1], {}).       
+00003d60: 2065 6c69 6620 272d 2d6a 736f 6e27 2069   elif '--json' i
+00003d70: 6e20 7379 732e 6172 6776 3a0a 2020 2020  n sys.argv:.    
+00003d80: 2020 2020 2020 2020 666f 7220 666f 726d          for form
+00003d90: 6174 6f20 696e 2066 6f72 6d61 746f 735b  ato in formatos[
+00003da0: 3a31 5d3a 0a20 2020 2020 2020 2020 2020  :1]:.           
+00003db0: 2020 2020 2061 7263 6869 766f 203d 206f       archivo = o
+00003dc0: 7065 6e28 666f 726d 6174 6f5b 305d 2e6c  pen(formato[0].l
+00003dd0: 6f77 6572 2829 202b 2022 2e6a 736f 6e22  ower() + ".json"
+00003de0: 2c20 2272 2229 0a20 2020 2020 2020 2020  , "r").         
+00003df0: 2020 2020 2020 2064 203d 206a 736f 6e2e         d = json.
+00003e00: 6c6f 6164 2861 7263 6869 766f 290a 2020  load(archivo).  
+00003e10: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00003e20: 726d 6174 6f5b 325d 2e65 7874 656e 6428  rmato[2].extend(
+00003e30: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
+00003e40: 2020 2061 7263 6869 766f 2e63 6c6f 7365     archivo.close
+00003e50: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
+00003e60: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00003e70: 2066 6f72 6d61 746f 2069 6e20 666f 726d   formato in form
+00003e80: 6174 6f73 5b3a 315d 3a0a 2020 2020 2020  atos[:1]:.      
+00003e90: 2020 2020 2020 2020 2020 6172 6368 6976            archiv
+00003ea0: 6f20 3d20 6f70 656e 2866 6f72 6d61 746f  o = open(formato
+00003eb0: 5b30 5d2e 6c6f 7765 7228 2920 2b20 222e  [0].lower() + ".
+00003ec0: 7478 7422 2c20 2272 2229 0a20 2020 2020  txt", "r").     
+00003ed0: 2020 2020 2020 2020 2020 2066 6f72 206c             for l
+00003ee0: 696e 6561 2069 6e20 6172 6368 6976 6f3a  inea in archivo:
+00003ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003f00: 2020 2020 2064 203d 206c 6565 7228 6c69       d = leer(li
+00003f10: 6e65 612c 2066 6f72 6d61 746f 5b31 5d29  nea, formato[1])
+00003f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003f30: 2020 2020 2066 6f72 6d61 746f 5b32 5d2e       formato[2].
+00003f40: 6170 7065 6e64 2864 290a 2020 2020 2020  append(d).      
+00003f50: 2020 2020 2020 2020 2020 6172 6368 6976            archiv
+00003f60: 6f2e 636c 6f73 6528 290a 0a20 2020 2077  o.close()..    w
+00003f70: 732e 436f 6e65 6374 6172 2822 222c 2057  s.Conectar("", W
+00003f80: 5344 4c2c 2070 726f 7879 290a 0a20 2020  SDL, proxy)..   
+00003f90: 2069 6620 7773 2e45 7863 6570 6369 6f6e   if ws.Excepcion
+00003fa0: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+00003fb0: 7773 2e45 7863 6570 6369 6f6e 290a 2020  ws.Excepcion).  
+00003fc0: 2020 2020 2020 7072 696e 7428 7773 2e54        print(ws.T
+00003fd0: 7261 6365 6261 636b 290a 2020 2020 2020  raceback).      
+00003fe0: 2020 7379 732e 6578 6974 282d 3129 0a0a    sys.exit(-1)..
+00003ff0: 2020 2020 2320 4461 746f 7320 6465 2070      # Datos de p
+00004000: 7275 6562 6173 3a0a 0a20 2020 2069 6620  ruebas:..    if 
+00004010: 272d 2d74 6573 7427 2069 6e20 7379 732e  '--test' in sys.
+00004020: 6172 6776 3a0a 2020 2020 2020 2020 7472  argv:.        tr
+00004030: 616e 7361 6363 696f 6e5f 6474 6f2e 6170  ansaccion_dto.ap
+00004040: 7065 6e64 2864 6963 7428 0a20 2020 2020  pend(dict(.     
+00004050: 2020 2020 2020 2067 6c6e 5f6f 7269 6765         gln_orige
+00004060: 6e3d 2239 3837 3635 3433 3231 3039 3832  n="9876543210982
+00004070: 222c 2067 6c6e 5f64 6573 7469 6e6f 3d22  ", gln_destino="
+00004080: 3336 3932 3538 3134 3733 3639 3322 2c0a  3692581473693",.
+00004090: 2020 2020 2020 2020 2020 2020 665f 6f70              f_op
+000040a0: 6572 6163 696f 6e3d 6461 7465 7469 6d65  eracion=datetime
+000040b0: 2e64 6174 6574 696d 652e 6e6f 7728 292e  .datetime.now().
+000040c0: 7374 7266 7469 6d65 2822 2564 2f25 6d2f  strftime("%d/%m/
+000040d0: 2559 2229 2c0a 2020 2020 2020 2020 2020  %Y"),.          
+000040e0: 2020 665f 656c 6162 6f72 6163 696f 6e3d    f_elaboracion=
+000040f0: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
+00004100: 652e 6e6f 7728 292e 7374 7266 7469 6d65  e.now().strftime
+00004110: 2822 2564 2f25 6d2f 2559 2229 2c0a 2020  ("%d/%m/%Y"),.  
+00004120: 2020 2020 2020 2020 2020 665f 7674 6f3d            f_vto=
+00004130: 2864 6174 6574 696d 652e 6461 7465 7469  (datetime.dateti
+00004140: 6d65 2e6e 6f77 2829 2b64 6174 6574 696d  me.now()+datetim
+00004150: 652e 7469 6d65 6465 6c74 6128 3330 2929  e.timedelta(30))
+00004160: 2e73 7472 6674 696d 6528 2225 642f 256d  .strftime("%d/%m
+00004170: 2f25 5922 292c 0a20 2020 2020 2020 2020  /%Y"),.         
+00004180: 2020 2069 645f 6576 656e 746f 3d31 312c     id_evento=11,
+00004190: 0a20 2020 2020 2020 2020 2020 2063 6f64  .            cod
+000041a0: 5f70 726f 6475 6374 6f3d 2238 3839 3030  _producto="88900
+000041b0: 3030 3030 3030 3030 3122 2c0a 2020 2020  000000001",.    
+000041c0: 2020 2020 2020 2020 6e5f 6361 6e74 6964          n_cantid
+000041d0: 6164 3d31 2c0a 2020 2020 2020 2020 2020  ad=1,.          
+000041e0: 2020 6e5f 7365 7269 653d 696e 7428 7469    n_serie=int(ti
+000041f0: 6d65 2e74 696d 6528 292a 3130 292c 0a20  me.time()*10),. 
+00004200: 2020 2020 2020 2020 2020 206e 5f6c 6f74             n_lot
+00004210: 653d 6461 7465 7469 6d65 2e64 6174 6574  e=datetime.datet
+00004220: 696d 652e 6e6f 7728 292e 7374 7266 7469  ime.now().strfti
+00004230: 6d65 2822 2559 2229 2c0a 2020 2020 2020  me("%Y"),.      
+00004240: 2020 2020 2020 6e5f 6361 693d 2231 3233        n_cai="123
+00004250: 3435 3637 3839 3031 3233 3435 222c 0a20  456789012345",. 
+00004260: 2020 2020 2020 2020 2020 206e 5f63 6165             n_cae
+00004270: 3d22 222c 0a20 2020 2020 2020 2020 2020  ="",.           
+00004280: 2069 645f 6d6f 7469 766f 5f64 6573 7472   id_motivo_destr
+00004290: 7563 6369 6f6e 3d30 2c0a 2020 2020 2020  uccion=0,.      
+000042a0: 2020 2020 2020 6e5f 6d61 6e69 6669 6573        n_manifies
+000042b0: 746f 3d22 222c 0a20 2020 2020 2020 2020  to="",.         
+000042c0: 2020 2065 6e5f 7472 616e 7370 6f72 7465     en_transporte
+000042d0: 3d22 4e22 2c0a 2020 2020 2020 2020 2020  ="N",.          
+000042e0: 2020 6e5f 7265 6d69 746f 3d22 3132 3334    n_remito="1234
+000042f0: 222c 0a20 2020 2020 2020 2020 2020 206d  ",.            m
+00004300: 6f74 6976 6f5f 6465 766f 6c75 6369 6f6e  otivo_devolucion
+00004310: 3d22 222c 0a20 2020 2020 2020 2020 2020  ="",.           
+00004320: 206f 6273 6572 7661 6369 6f6e 6573 3d22   observaciones="
+00004330: 7072 7565 6261 222c 0a20 2020 2020 2020  prueba",.       
+00004340: 2020 2020 206e 5f76 616c 655f 636f 6d70       n_vale_comp
+00004350: 7261 3d22 222c 0a20 2020 2020 2020 2020  ra="",.         
+00004360: 2020 2061 7065 6c6c 6964 6f4e 6f6d 6272     apellidoNombr
+00004370: 6573 3d22 4a75 616e 2050 6572 6573 222c  es="Juan Peres",
+00004380: 0a20 2020 2020 2020 2020 2020 2064 6972  .            dir
+00004390: 6563 6369 6f6e 3d22 5361 7261 7a61 222c  eccion="Saraza",
+000043a0: 206e 756d 6572 6f3d 2231 3233 3422 2c0a   numero="1234",.
+000043b0: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
+000043c0: 6c69 6461 643d 2248 7572 6c69 6e67 6861  lidad="Hurlingha
+000043d0: 6d22 2c20 7072 6f76 696e 6369 613d 2242  m", provincia="B
+000043e0: 7565 6e6f 7320 4169 7265 7322 2c0a 2020  uenos Aires",.  
+000043f0: 2020 2020 2020 2020 2020 6e5f 706f 7374            n_post
+00004400: 616c 3d22 3136 3838 222c 0a20 2020 2020  al="1688",.     
+00004410: 2020 2020 2020 2063 7569 743d 2232 3032         cuit="202
+00004420: 3637 3536 3533 3933 222c 0a20 2020 2020  67565393",.     
+00004430: 2020 2020 2020 2063 6f64 6967 6f5f 7472         codigo_tr
+00004440: 616e 7361 6363 696f 6e3d 4e6f 6e65 2c0a  ansaccion=None,.
+00004450: 2020 2020 2020 2020 2929 0a0a 2020 2020          ))..    
+00004460: 2320 4f70 6369 6f6e 6573 2070 7269 6e63  # Opciones princ
+00004470: 6970 616c 6573 3a0a 0a20 2020 2069 6620  ipales:..    if 
+00004480: 272d 2d63 6f6e 6669 726d 6127 2069 6e20  '--confirma' in 
+00004490: 7379 732e 6172 6776 3a0a 2020 2020 2020  sys.argv:.      
+000044a0: 2020 6966 2027 2d2d 6c6f 6164 786d 6c27    if '--loadxml'
+000044b0: 2069 6e20 7379 732e 6172 6776 3a0a 2020   in sys.argv:.  
+000044c0: 2020 2020 2020 2020 2020 7773 2e4c 6f61            ws.Loa
+000044d0: 6454 6573 7458 4d4c 2822 7472 617a 616d  dTestXML("trazam
+000044e0: 6564 5f63 6f6e 6669 726d 612e 786d 6c22  ed_confirma.xml"
+000044f0: 2920 2023 2063 6172 676f 2072 6573 7075  )  # cargo respu
+00004500: 6573 7461 0a20 2020 2020 2020 2020 2020  esta.           
+00004510: 206f 6b20 3d20 7773 2e53 656e 6443 6f6e   ok = ws.SendCon
+00004520: 6669 726d 6154 7261 6e73 6163 6328 7573  firmaTransacc(us
+00004530: 7561 7269 6f3d 2270 7275 6562 6173 7773  uario="pruebasws
+00004540: 222c 2070 6173 7377 6f72 643d 2270 7275  ", password="pru
+00004550: 6562 6173 7773 222c 0a20 2020 2020 2020  ebasws",.       
+00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004570: 2020 2020 2020 2020 2020 2020 705f 6964              p_id
+00004580: 735f 7472 616e 7361 633d 2231 222c 2066  s_transac="1", f
+00004590: 5f6f 7065 7261 6369 6f6e 3d22 3331 2d31  _operacion="31-1
+000045a0: 322d 3230 3133 2229 0a20 2020 2020 2020  2-2013").       
+000045b0: 2020 2020 2069 6620 6e6f 7420 6f6b 3a0a       if not ok:.
+000045c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045d0: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
+000045e0: 6f72 2877 732e 4578 6365 7063 696f 6e29  or(ws.Excepcion)
+000045f0: 0a20 2020 2020 2020 2077 732e 5365 6e64  .        ws.Send
+00004600: 436f 6e66 6972 6d61 5472 616e 7361 6363  ConfirmaTransacc
+00004610: 282a 7379 732e 6172 6776 5b73 7973 2e61  (*sys.argv[sys.a
+00004620: 7267 762e 696e 6465 7828 222d 2d63 6f6e  rgv.index("--con
+00004630: 6669 726d 6122 292b 313a 5d29 0a20 2020  firma")+1:]).   
+00004640: 2065 6c69 6620 272d 2d61 6c65 7274 6127   elif '--alerta'
+00004650: 2069 6e20 7379 732e 6172 6776 3a0a 2020   in sys.argv:.  
+00004660: 2020 2020 2020 7773 2e53 656e 6441 6c65        ws.SendAle
+00004670: 7274 6154 7261 6e73 6163 6328 2a73 7973  rtaTransacc(*sys
+00004680: 2e61 7267 765b 7379 732e 6172 6776 2e69  .argv[sys.argv.i
+00004690: 6e64 6578 2822 2d2d 616c 6572 7461 2229  ndex("--alerta")
+000046a0: 2b31 3a5d 290a 2020 2020 656c 6966 2027  +1:]).    elif '
+000046b0: 2d2d 6361 6e63 656c 6127 2069 6e20 7379  --cancela' in sy
+000046c0: 732e 6172 6776 3a0a 2020 2020 2020 2020  s.argv:.        
+000046d0: 7773 2e53 656e 6443 616e 6365 6c61 5472  ws.SendCancelaTr
+000046e0: 616e 7361 6328 2a73 7973 2e61 7267 765b  ansac(*sys.argv[
+000046f0: 7379 732e 6172 6776 2e69 6e64 6578 2822  sys.argv.index("
+00004700: 2d2d 6361 6e63 656c 6122 292b 313a 5d29  --cancela")+1:])
+00004710: 0a20 2020 2065 6c69 6620 272d 2d63 6f6e  .    elif '--con
+00004720: 7375 6c74 6127 2069 6e20 7379 732e 6172  sulta' in sys.ar
+00004730: 6776 3a0a 2020 2020 2020 2020 7773 2e47  gv:.        ws.G
+00004740: 6574 5472 616e 7361 6363 696f 6e65 7328  etTransacciones(
+00004750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004760: 2020 2020 2020 2020 2020 2020 202a 7379               *sy
+00004770: 732e 6172 6776 5b73 7973 2e61 7267 762e  s.argv[sys.argv.
+00004780: 696e 6465 7828 222d 2d63 6f6e 7375 6c74  index("--consult
+00004790: 6122 292b 313a 5d0a 2020 2020 2020 2020  a")+1:].        
+000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047b0: 2020 2020 290a 2020 2020 2020 2020 7072      ).        pr
+000047c0: 696e 7428 2243 616e 7450 6167 696e 6173  int("CantPaginas
+000047d0: 222c 2077 732e 4361 6e74 5061 6769 6e61  ", ws.CantPagina
+000047e0: 7329 0a20 2020 2020 2020 2070 7269 6e74  s).        print
+000047f0: 2822 4861 7945 7272 6f72 222c 2077 732e  ("HayError", ws.
+00004800: 4861 7945 7272 6f72 290a 2020 2020 2020  HayError).      
+00004810: 2020 2320 7072 696e 7428 2254 7261 6e73    # print("Trans
+00004820: 6163 6369 6f6e 5365 6e61 7361 222c 2077  accionSenasa", w
+00004830: 732e 5472 616e 7361 6363 696f 6e53 656e  s.TransaccionSen
+00004840: 6173 6129 0a20 2020 2020 2020 2023 2070  asa).        # p
+00004850: 6172 616d 6574 726f 7320 636f 6d75 6e65  arametros comune
+00004860: 7320 6465 2073 616c 6964 6120 2863 6f6c  s de salida (col
+00004870: 756d 6e61 7320 6465 206c 6120 7461 626c  umnas de la tabl
+00004880: 6129 3a0a 2020 2020 2020 2020 636c 6176  a):.        clav
+00004890: 6573 203d 205b 6b20 666f 7220 6b2c 2076  es = [k for k, v
+000048a0: 2c20 6c20 696e 2054 5241 4e53 4143 4349  , l in TRANSACCI
+000048b0: 4f4e 4553 5d0a 2020 2020 2020 2020 2320  ONES].        # 
+000048c0: 6578 7469 656e 646f 206c 6120 6c69 7374  extiendo la list
+000048d0: 6120 6465 2072 6573 756c 7461 646f 2070  a de resultado p
+000048e0: 6172 6120 656c 2061 7263 6869 766f 2064  ara el archivo d
+000048f0: 6520 696e 7465 7263 616d 6269 6f3a 0a20  e intercambio:. 
+00004900: 2020 2020 2020 2074 7261 6e73 6163 6369         transacci
+00004910: 6f6e 6573 2e65 7874 656e 6428 7773 2e54  ones.extend(ws.T
+00004920: 7261 6e73 6163 6369 6f6e 5365 6e61 7361  ransaccionSenasa
+00004930: 290a 2020 2020 2020 2020 2320 656e 6361  ).        # enca
+00004940: 6265 7a61 646f 2064 6520 6c61 2074 6162  bezado de la tab
+00004950: 6c61 3a0a 2020 2020 2020 2020 7072 696e  la:.        prin
+00004960: 7428 227c 7c22 2c20 227c 7c22 2e6a 6f69  t("||", "||".joi
+00004970: 6e28 5b22 2573 2220 2520 636c 6176 6520  n(["%s" % clave 
+00004980: 666f 7220 636c 6176 6520 696e 2063 6c61  for clave in cla
+00004990: 7665 735d 292c 2022 7c7c 2229 0a20 2020  ves]), "||").   
+000049a0: 2020 2020 2023 2072 6563 6f72 726f 206c       # recorro l
+000049b0: 6f73 2064 6174 6f73 2064 6576 7565 6c74  os datos devuelt
+000049c0: 6f73 2028 5472 616e 7361 6363 696f 6e53  os (TransaccionS
+000049d0: 656e 6173 6129 3a0a 2020 2020 2020 2020  enasa):.        
+000049e0: 7768 696c 6520 7773 2e4c 6565 7254 7261  while ws.LeerTra
+000049f0: 6e73 6163 6369 6f6e 2829 3a0a 2020 2020  nsaccion():.    
+00004a00: 2020 2020 2020 2020 666f 7220 636c 6176          for clav
+00004a10: 6520 696e 2063 6c61 7665 733a 0a20 2020  e in claves:.   
+00004a20: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00004a30: 6e74 2822 7c7c 222c 2077 732e 4765 7450  nt("||", ws.GetP
+00004a40: 6172 616d 6574 726f 2863 6c61 7665 2929  arametro(clave))
+00004a50: 2020 2020 2020 2020 2023 2069 6d70 7269           # impri
+00004a60: 6d6f 2063 6164 6120 6669 6c61 0a20 2020  mo cada fila.   
+00004a70: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00004a80: 7c7c 2229 0a20 2020 2065 6c73 653a 0a20  ||").    else:. 
+00004a90: 2020 2020 2020 2061 7267 7620 3d20 5b61         argv = [a
+00004aa0: 7267 7620 666f 7220 6172 6776 2069 6e20  rgv for argv in 
+00004ab0: 7379 732e 6172 6776 2069 6620 6e6f 7420  sys.argv if not 
+00004ac0: 6172 6776 2e73 7461 7274 7377 6974 6828  argv.startswith(
+00004ad0: 222d 2d22 295d 0a20 2020 2020 2020 2069  "--")].        i
+00004ae0: 6620 6e6f 7420 7472 616e 7361 6363 696f  f not transaccio
+00004af0: 6e5f 6474 6f3a 0a20 2020 2020 2020 2020  n_dto:.         
+00004b00: 2020 2069 6620 6c65 6e28 6172 6776 293e     if len(argv)>
+00004b10: 3130 3a0a 2020 2020 2020 2020 2020 2020  10:.            
+00004b20: 2020 2020 7773 2e53 6176 6554 7261 6e73      ws.SaveTrans
+00004b30: 6163 6369 6f6e 282a 6172 6776 5b31 3a5d  accion(*argv[1:]
+00004b40: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00004b50: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00004b60: 2020 2020 7072 696e 7428 2245 5252 4f52      print("ERROR
+00004b70: 3a20 6e6f 2073 6520 696e 6469 6361 726f  : no se indicaro
+00004b80: 6e20 746f 646f 7320 6c6f 7320 7061 72e1  n todos los par.
+00004b90: 6d65 7472 6f73 2072 6571 7565 7269 646f  metros requerido
+00004ba0: 7322 290a 2020 2020 2020 2020 656c 6966  s").        elif
+00004bb0: 2074 7261 6e73 6163 6369 6f6e 5f64 746f   transaccion_dto
+00004bc0: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
+00004bd0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00004be0: 2020 2075 7375 6172 696f 2c20 7061 7373     usuario, pass
+00004bf0: 776f 7264 203d 2061 7267 765b 2d32 3a5d  word = argv[-2:]
+00004c00: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00004c10: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
+00004c20: 2020 2020 2070 7269 6e74 2822 4144 5645       print("ADVE
+00004c30: 5254 454e 4349 413a 206e 6f20 7365 2069  RTENCIA: no se i
+00004c40: 6e64 6963 6f20 7061 72e1 6d65 7472 6f73  ndico par.metros
+00004c50: 2075 7375 6172 696f 2079 2070 6173 736f   usuario y passo
+00004c60: 776f 7264 2229 0a20 2020 2020 2020 2020  word").         
+00004c70: 2020 2020 2020 2075 7375 6172 696f 2c20         usuario, 
+00004c80: 7061 7373 776f 7264 203d 2022 7365 6e61  password = "sena
+00004c90: 7361 7773 222c 2022 436c 6176 6532 3031  saws", "Clave201
+00004ca0: 3322 0a20 2020 2020 2020 2020 2020 2066  3".            f
+00004cb0: 6f72 2069 2c20 6474 6f20 696e 2065 6e75  or i, dto in enu
+00004cc0: 6d65 7261 7465 2874 7261 6e73 6163 6369  merate(transacci
+00004cd0: 6f6e 5f64 746f 293a 0a20 2020 2020 2020  on_dto):.       
+00004ce0: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00004cf0: 5072 6f63 6573 616e 646f 2072 6567 6973  Procesando regis
+00004d00: 7472 6f22 2c20 6929 0a20 2020 2020 2020  tro", i).       
+00004d10: 2020 2020 2020 2020 2064 656c 2064 746f           del dto
+00004d20: 5b27 636f 6469 676f 5f74 7261 6e73 6163  ['codigo_transac
+00004d30: 6369 6f6e 275d 0a20 2020 2020 2020 2020  cion'].         
+00004d40: 2020 2020 2020 2077 732e 5361 7665 5472         ws.SaveTr
+00004d50: 616e 7361 6363 696f 6e28 7573 7561 7269  ansaccion(usuari
+00004d60: 6f2c 2070 6173 7377 6f72 642c 202a 2a64  o, password, **d
+00004d70: 746f 290a 2020 2020 2020 2020 2020 2020  to).            
+00004d80: 2020 2020 6474 6f5b 2763 6f64 6967 6f5f      dto['codigo_
+00004d90: 7472 616e 7361 6363 696f 6e27 5d20 3d20  transaccion'] = 
+00004da0: 7773 2e43 6f64 6967 6f54 7261 6e73 6163  ws.CodigoTransac
+00004db0: 6369 6f6e 0a20 2020 2020 2020 2020 2020  cion.           
+00004dc0: 2020 2020 2065 7272 6f72 6573 2e65 7874       errores.ext
+00004dd0: 656e 6428 7773 2e65 7272 6f72 6573 290a  end(ws.errores).
+00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004df0: 7072 696e 7428 227c 5265 7375 6c74 6164  print("|Resultad
+00004e00: 6f20 2535 737c 436f 6469 676f 5472 616e  o %5s|CodigoTran
+00004e10: 7361 6363 696f 6e20 2531 3073 7c45 7272  saccion %10s|Err
+00004e20: 6f72 6573 7c25 737c 2220 2520 280a 2020  ores|%s|" % (.  
+00004e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e40: 2020 7773 2e52 6573 756c 7461 646f 2c0a    ws.Resultado,.
+00004e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e60: 2020 2020 7773 2e43 6f64 6967 6f54 7261      ws.CodigoTra
+00004e70: 6e73 6163 6369 6f6e 2c0a 2020 2020 2020  nsaccion,.      
+00004e80: 2020 2020 2020 2020 2020 2020 2020 277c                '|
+00004e90: 272e 6a6f 696e 2877 732e 4572 726f 7265  '.join(ws.Errore
+00004ea0: 7320 6f72 205b 5d29 2c0a 2020 2020 2020  s or []),.      
+00004eb0: 2020 2020 2020 2020 2020 2020 2020 2929                ))
+00004ec0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00004ed0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00004ee0: 2822 4552 524f 523a 206e 6f20 7365 2065  ("ERROR: no se e
+00004ef0: 7370 6563 6966 6963 6172 6f6e 2070 726f  specificaron pro
+00004f00: 6475 6374 6f73 2061 2069 6e66 6f72 6d61  ductos a informa
+00004f10: 7222 290a 0a20 2020 2069 6620 6e6f 7420  r")..    if not 
+00004f20: 7472 616e 7361 6363 696f 6e5f 6474 6f3a  transaccion_dto:
+00004f30: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+00004f40: 7c52 6573 756c 7461 646f 2025 3573 7c43  |Resultado %5s|C
+00004f50: 6f64 6967 6f54 7261 6e73 6163 6369 6f6e  odigoTransaccion
+00004f60: 2025 3130 737c 4572 726f 7265 737c 2573   %10s|Errores|%s
+00004f70: 7c22 2025 2028 0a20 2020 2020 2020 2020  |" % (.         
+00004f80: 2020 2020 2020 2077 732e 5265 7375 6c74         ws.Result
+00004f90: 6164 6f2c 0a20 2020 2020 2020 2020 2020  ado,.           
+00004fa0: 2020 2020 2077 732e 436f 6469 676f 5472       ws.CodigoTr
+00004fb0: 616e 7361 6363 696f 6e2c 0a20 2020 2020  ansaccion,.     
+00004fc0: 2020 2020 2020 2020 2020 2027 7c27 2e6a             '|'.j
+00004fd0: 6f69 6e28 7773 2e45 7272 6f72 6573 206f  oin(ws.Errores o
+00004fe0: 7220 5b5d 292c 0a20 2020 2020 2020 2020  r []),.         
+00004ff0: 2020 2020 2020 2029 290a 0a20 2020 2069         ))..    i
+00005000: 6620 7773 2e45 7863 6570 6369 6f6e 3a0a  f ws.Excepcion:.
+00005010: 2020 2020 2020 2020 7072 696e 7428 7773          print(ws
+00005020: 2e54 7261 6365 6261 636b 290a 0a20 2020  .Traceback)..   
+00005030: 2069 6620 272d 2d67 7261 6261 7227 2069   if '--grabar' i
+00005040: 6e20 7379 732e 6172 6776 3a0a 2020 2020  n sys.argv:.    
+00005050: 2020 2020 6966 2027 2d2d 6462 6627 2069      if '--dbf' i
+00005060: 6e20 7379 732e 6172 6776 3a0a 2020 2020  n sys.argv:.    
+00005070: 2020 2020 2020 2020 6775 6172 6461 725f          guardar_
+00005080: 6462 6628 666f 726d 6174 6f73 2c20 5472  dbf(formatos, Tr
+00005090: 7565 2c20 7b7d 290a 2020 2020 2020 2020  ue, {}).        
+000050a0: 656c 6966 2027 2d2d 6a73 6f6e 2720 696e  elif '--json' in
+000050b0: 2073 7973 2e61 7267 763a 0a20 2020 2020   sys.argv:.     
+000050c0: 2020 2020 2020 2066 6f72 2066 6f72 6d61         for forma
+000050d0: 746f 2069 6e20 666f 726d 6174 6f73 3a0a  to in formatos:.
+000050e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050f0: 6172 6368 6976 6f20 3d20 6f70 656e 2866  archivo = open(f
+00005100: 6f72 6d61 746f 5b30 5d2e 6c6f 7765 7228  ormato[0].lower(
+00005110: 2920 2b20 222e 6a73 6f6e 222c 2022 7722  ) + ".json", "w"
+00005120: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00005130: 2020 6a73 6f6e 2e64 756d 7028 666f 726d    json.dump(form
+00005140: 6174 6f5b 325d 2c20 6172 6368 6976 6f2c  ato[2], archivo,
+00005150: 2073 6f72 745f 6b65 7973 3d54 7275 652c   sort_keys=True,
+00005160: 2069 6e64 656e 743d 3429 0a20 2020 2020   indent=4).     
+00005170: 2020 2020 2020 2020 2020 2061 7263 6869             archi
+00005180: 766f 2e63 6c6f 7365 2829 0a20 2020 2020  vo.close().     
+00005190: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000051a0: 2020 2020 2066 6f72 2066 6f72 6d61 746f       for formato
+000051b0: 2069 6e20 666f 726d 6174 6f73 3a0a 2020   in formatos:.  
+000051c0: 2020 2020 2020 2020 2020 2020 2020 6172                ar
+000051d0: 6368 6976 6f20 3d20 6f70 656e 2866 6f72  chivo = open(for
+000051e0: 6d61 746f 5b30 5d2e 6c6f 7765 7228 2920  mato[0].lower() 
+000051f0: 2b20 222e 7478 7422 2c20 2277 2229 0a20  + ".txt", "w"). 
+00005200: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00005210: 6f72 2069 7420 696e 2066 6f72 6d61 746f  or it in formato
+00005220: 5b32 5d3a 0a20 2020 2020 2020 2020 2020  [2]:.           
+00005230: 2020 2020 2020 2020 2061 7263 6869 766f           archivo
+00005240: 2e77 7269 7465 2865 7363 7269 6269 7228  .write(escribir(
+00005250: 6974 2c20 666f 726d 6174 6f5b 315d 2929  it, formato[1]))
+00005260: 0a20 2020 2020 2020 2020 2020 2061 7263  .            arc
+00005270: 6869 766f 2e63 6c6f 7365 2829 0a0a 0a23  hivo.close()...#
+00005280: 2062 7573 636f 2065 6c20 6469 7265 6374   busco el direct
+00005290: 6f72 696f 2064 6520 696e 7374 616c 6163  orio de instalac
+000052a0: 69f3 6e20 2867 6c6f 6261 6c20 7061 7261  i.n (global para
+000052b0: 2071 7565 206e 6f20 6361 6d62 6965 2073   que no cambie s
+000052c0: 6920 7573 616e 206f 7472 6120 646c 6c29  i usan otra dll)
+000052d0: 0a49 4e53 5441 4c4c 5f44 4952 203d 2054  .INSTALL_DIR = T
+000052e0: 7261 7a61 5665 742e 496e 7374 616c 6c44  razaVet.InstallD
+000052f0: 6972 203d 2067 6574 5f69 6e73 7461 6c6c  ir = get_install
+00005300: 5f64 6972 2829 0a0a 0a69 6620 5f5f 6e61  _dir()...if __na
+00005310: 6d65 5f5f 203d 3d20 275f 5f6d 6169 6e5f  me__ == '__main_
+00005320: 5f27 3a0a 0a20 2020 2023 2061 6a75 7374  _':..    # ajust
+00005330: 6f20 656c 2065 6e63 6f64 696e 6720 706f  o el encoding po
+00005340: 7220 6465 6665 6374 6f20 2873 6920 7365  r defecto (si se
+00005350: 2072 6564 6972 696a 6520 6c61 2073 616c   redirije la sal
+00005360: 6964 6129 0a20 2020 2069 6620 6e6f 7420  ida).    if not 
+00005370: 6861 7361 7474 7228 7379 732e 7374 646f  hasattr(sys.stdo
+00005380: 7574 2c20 2265 6e63 6f64 696e 6722 2920  ut, "encoding") 
+00005390: 6f72 2073 7973 2e73 7464 6f75 742e 656e  or sys.stdout.en
+000053a0: 636f 6469 6e67 2069 7320 4e6f 6e65 3a0a  coding is None:.
+000053b0: 2020 2020 2020 2020 696d 706f 7274 2063          import c
+000053c0: 6f64 6563 732c 206c 6f63 616c 650a 2020  odecs, locale.  
+000053d0: 2020 2020 2020 7379 732e 7374 646f 7574        sys.stdout
+000053e0: 203d 2063 6f64 6563 732e 6765 7477 7269   = codecs.getwri
+000053f0: 7465 7228 6c6f 6361 6c65 2e67 6574 7072  ter(locale.getpr
+00005400: 6566 6572 7265 6465 6e63 6f64 696e 6728  eferredencoding(
+00005410: 2929 2873 7973 2e73 7464 6f75 742c 2272  ))(sys.stdout,"r
+00005420: 6570 6c61 6365 2229 3b0a 2020 2020 2020  eplace");.      
+00005430: 2020 7379 732e 7374 6465 7272 203d 2063    sys.stderr = c
+00005440: 6f64 6563 732e 6765 7477 7269 7465 7228  odecs.getwriter(
+00005450: 6c6f 6361 6c65 2e67 6574 7072 6566 6572  locale.getprefer
+00005460: 7265 6465 6e63 6f64 696e 6728 2929 2873  redencoding())(s
+00005470: 7973 2e73 7464 6572 722c 2272 6570 6c61  ys.stderr,"repla
+00005480: 6365 2229 3b0a 0a20 2020 2069 6620 272d  ce");..    if '-
+00005490: 2d72 6567 6973 7465 7227 2069 6e20 7379  -register' in sy
+000054a0: 732e 6172 6776 206f 7220 272d 2d75 6e72  s.argv or '--unr
+000054b0: 6567 6973 7465 7227 2069 6e20 7379 732e  egister' in sys.
+000054c0: 6172 6776 3a0a 2020 2020 2020 2020 696d  argv:.        im
+000054d0: 706f 7274 2070 7974 686f 6e63 6f6d 0a20  port pythoncom. 
+000054e0: 2020 2020 2020 2069 6d70 6f72 7420 7769         import wi
+000054f0: 6e33 3263 6f6d 2e73 6572 7665 722e 7265  n32com.server.re
+00005500: 6769 7374 6572 0a20 2020 2020 2020 2077  gister.        w
+00005510: 696e 3332 636f 6d2e 7365 7276 6572 2e72  in32com.server.r
+00005520: 6567 6973 7465 722e 5573 6543 6f6d 6d61  egister.UseComma
+00005530: 6e64 4c69 6e65 2854 7261 7a61 5665 7429  ndLine(TrazaVet)
+00005540: 0a20 2020 2065 6c69 6620 222f 4175 746f  .    elif "/Auto
+00005550: 6d61 7465 2220 696e 2073 7973 2e61 7267  mate" in sys.arg
+00005560: 763a 0a20 2020 2020 2020 2023 204d 5320  v:.        # MS 
+00005570: 7365 656d 7320 746f 206c 696b 6520 2f61  seems to like /a
+00005580: 7574 6f6d 6174 6520 746f 2072 756e 2074  utomate to run t
+00005590: 6865 2063 6c61 7373 2066 6163 746f 7269  he class factori
+000055a0: 6573 2e0a 2020 2020 2020 2020 696d 706f  es..        impo
+000055b0: 7274 2077 696e 3332 636f 6d2e 7365 7276  rt win32com.serv
+000055c0: 6572 2e6c 6f63 616c 7365 7276 6572 0a20  er.localserver. 
+000055d0: 2020 2020 2020 2023 7769 6e33 3263 6f6d         #win32com
+000055e0: 2e73 6572 7665 722e 6c6f 6361 6c73 6572  .server.localser
+000055f0: 7665 722e 6d61 696e 2829 0a20 2020 2020  ver.main().     
+00005600: 2020 2023 2073 7461 7274 2074 6865 2073     # start the s
+00005610: 6572 7665 722e 0a20 2020 2020 2020 2077  erver..        w
+00005620: 696e 3332 636f 6d2e 7365 7276 6572 2e6c  in32com.server.l
+00005630: 6f63 616c 7365 7276 6572 2e73 6572 7665  ocalserver.serve
+00005640: 285b 5472 617a 6156 6574 2e5f 7265 675f  ([TrazaVet._reg_
+00005650: 636c 7369 645f 5d29 0a20 2020 2065 6c73  clsid_]).    els
+00005660: 653a 0a20 2020 2020 2020 206d 6169 6e28  e:.        main(
+00005670: 290a                                     ).
```

### Comparing `py3afipws-0.8/py3afipws/utils.py` & `py3afipws-0.9/py3afipws/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; version 3.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/wdigdepfiel.py` & `py3afipws-0.9/py3afipws/wdigdepfiel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/ws_sr_padron.py` & `py3afipws-0.9/py3afipws/ws_sr_padron.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/wsaa.py` & `py3afipws-0.9/py3afipws/wsaa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/wsbfe.py` & `py3afipws-0.9/py3afipws/wsbfe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/wsbfev1.py` & `py3afipws-0.9/py3afipws/wsbfev1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/wscdc.py` & `py3afipws-0.9/py3afipws/wscdc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/wscoc.py` & `py3afipws-0.9/py3afipws/wscoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/wsctgv3.py` & `py3afipws-0.9/py3afipws/wsctgv3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/wsfe.py` & `py3afipws-0.9/py3afipws/wsfe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/wsfev1.py` & `py3afipws-0.9/py3afipws/wsfev1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/wsfex.py` & `py3afipws-0.9/py3afipws/wsfex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/wsfexv1.py` & `py3afipws-0.9/py3afipws/wsfexv1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/wsltv.py` & `py3afipws-0.9/py3afipws/wsltv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws/wsmtx.py` & `py3afipws-0.9/py3afipws/wsmtx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+# -*- coding: utf-8 -*-
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by the
 # Free Software Foundation; either version 3, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but
 # WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTIBILITY
```

### Comparing `py3afipws-0.8/py3afipws.egg-info/PKG-INFO` & `py3afipws-0.9/py3afipws.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: py3afipws
-Version: 0.8
+Version: 0.9
 Summary: pyafipws for python3
 Home-page: https://github.com/odoo-mastercore/pyafipws
 Author: Mastercore
 Author-email: far@mastercore.net
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: py3afipws,py3
```

### Comparing `py3afipws-0.8/py3afipws.egg-info/SOURCES.txt` & `py3afipws-0.9/py3afipws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3afipws-0.8/setup.py` & `py3afipws-0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='py3afipws',
     packages=['py3afipws'],  # this must be the same as the name above
-    version='0.8',
+    version='0.9',
     description='pyafipws for python3',
     author='Mastercore',
     author_email='far@mastercore.net',
     # use the URL to the github repo
     url='https://github.com/odoo-mastercore/pyafipws',
-    download_ur3='https://github.com/odoo-mastercore/py3afipws/tarball/0.8',
+    download_ur3='https://github.com/odoo-mastercore/py3afipws/tarball/0.9',
     keywords=['py3afipws', 'py3'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.2',
```

