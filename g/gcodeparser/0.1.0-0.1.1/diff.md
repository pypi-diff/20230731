# Comparing `tmp/gcodeparser-0.1.0.tar.gz` & `tmp/gcodeparser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gcodeparser-0.1.0.tar", last modified: Fri Jan  6 11:01:36 2023, max compression
+gzip compressed data, was "gcodeparser-0.1.1.tar", last modified: Mon Jul 31 09:56:28 2023, max compression
```

## Comparing `gcodeparser-0.1.0.tar` & `gcodeparser-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-01-06 11:01:36.720306 gcodeparser-0.1.0/
--rw-rw-rw-   0        0        0     6000 2023-01-06 11:01:36.719306 gcodeparser-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4389 2021-06-24 09:42:35.000000 gcodeparser-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-01-06 11:01:36.702307 gcodeparser-0.1.0/gcodeparser/
--rw-rw-rw-   0        0        0      107 2023-01-06 11:01:28.000000 gcodeparser-0.1.0/gcodeparser/__init__.py
--rw-rw-rw-   0        0        0      116 2021-02-08 10:48:08.000000 gcodeparser-0.1.0/gcodeparser/commands.py
--rw-rw-rw-   0        0        0     3804 2023-01-06 10:50:30.000000 gcodeparser-0.1.0/gcodeparser/gcode_parser.py
-drwxrwxrwx   0        0        0        0 2023-01-06 11:01:36.709307 gcodeparser-0.1.0/gcodeparser.egg-info/
--rw-rw-rw-   0        0        0     6000 2023-01-06 11:01:36.000000 gcodeparser-0.1.0/gcodeparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-01-06 11:01:36.000000 gcodeparser-0.1.0/gcodeparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-06 11:01:36.000000 gcodeparser-0.1.0/gcodeparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-01-06 11:01:36.000000 gcodeparser-0.1.0/gcodeparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-06 11:01:36.720306 gcodeparser-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-01-06 11:01:28.000000 gcodeparser-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-06 11:01:36.717306 gcodeparser-0.1.0/test/
--rw-rw-rw-   0        0        0        0 2021-03-03 10:57:25.000000 gcodeparser-0.1.0/test/__init__.py
--rw-rw-rw-   0        0        0      689 2021-03-03 14:41:57.000000 gcodeparser-0.1.0/test/test_element_type.py
--rw-rw-rw-   0        0        0     1147 2021-06-18 09:51:49.000000 gcodeparser-0.1.0/test/test_gcode_line.py
--rw-rw-rw-   0        0        0     3316 2021-03-03 14:47:41.000000 gcodeparser-0.1.0/test/test_get_lines.py
--rw-rw-rw-   0        0        0     1558 2023-01-06 10:54:40.000000 gcodeparser-0.1.0/test/test_split_params.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:56:28.751952 gcodeparser-0.1.1/
+-rw-rw-rw-   0        0        0     1082 2023-07-31 09:32:37.000000 gcodeparser-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4813 2023-07-31 09:56:28.750953 gcodeparser-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4389 2023-07-31 09:32:37.000000 gcodeparser-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 09:56:28.738697 gcodeparser-0.1.1/gcodeparser/
+-rw-rw-rw-   0        0        0      107 2023-07-31 09:55:49.000000 gcodeparser-0.1.1/gcodeparser/__init__.py
+-rw-rw-rw-   0        0        0      116 2023-07-31 09:32:37.000000 gcodeparser-0.1.1/gcodeparser/commands.py
+-rw-rw-rw-   0        0        0     4016 2023-07-31 09:49:34.000000 gcodeparser-0.1.1/gcodeparser/gcode_parser.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:56:28.743710 gcodeparser-0.1.1/gcodeparser.egg-info/
+-rw-rw-rw-   0        0        0     4813 2023-07-31 09:56:28.000000 gcodeparser-0.1.1/gcodeparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-07-31 09:56:28.000000 gcodeparser-0.1.1/gcodeparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 09:56:28.000000 gcodeparser-0.1.1/gcodeparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-31 09:56:28.000000 gcodeparser-0.1.1/gcodeparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 09:56:28.751952 gcodeparser-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-07-31 09:55:49.000000 gcodeparser-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:56:28.749952 gcodeparser-0.1.1/test/
+-rw-rw-rw-   0        0        0        0 2023-07-31 09:32:37.000000 gcodeparser-0.1.1/test/__init__.py
+-rw-rw-rw-   0        0        0      724 2023-07-31 09:32:37.000000 gcodeparser-0.1.1/test/test_element_type.py
+-rw-rw-rw-   0        0        0     1587 2023-07-31 09:50:25.000000 gcodeparser-0.1.1/test/test_gcode_line.py
+-rw-rw-rw-   0        0        0     3439 2023-07-31 09:32:37.000000 gcodeparser-0.1.1/test/test_get_lines.py
+-rw-rw-rw-   0        0        0     1611 2023-07-31 09:32:37.000000 gcodeparser-0.1.1/test/test_split_params.py
```

### Comparing `gcodeparser-0.1.0/PKG-INFO` & `gcodeparser-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,159 +1,145 @@
-Metadata-Version: 2.1
-Name: gcodeparser
-Version: 0.1.0
-Summary: Python gcode parser
-Home-page: https://github.com/AndyEveritt/GcodeParser
-Author: Andy Everitt
-Author-email: andreweveritt@e3d-online.com
-License: UNKNOWN
-Description: # GcodeParser
-        
-        A simple gcode parser that takes a string of text and returns a list where each gcode command is seperated into a python object.
-        
-        The structure of the python object is:
-        
-        `G1 X10 Y-2.5 ; this is a comment`
-        
-        ```python
-        GcodeLine(
-          command = ('G', 1),
-          params = {'X': 10, 'Y': -2.5},
-          comment = 'this is a comment',
-        )
-        ```
-        
-        # Install
-        
-        ```
-        pip install gcodeparser
-        ```
-        
-        Alternatively:
-        
-        ```
-        pip install -e "git+https://github.com/AndyEveritt/GcodeParser.git@master#egg=gcodeparser"
-        ```
-        
-        # Usage
-        
-        ```python
-        from gcodeparser import GcodeParser
-        
-        # open gcode file and store contents as variable
-        with open('my_gcode.gcode', 'r') as f:
-          gcode = f.read()
-        
-        GcodeParser(gcode).lines    # get parsed gcode lines
-        ```
-        
-        ## Include Comments
-        
-        `GcodeParser` takes a second argument called `include_comments` which defaults to `False`. If this is set to `True` then any line from the gcode file which only contains a comment will also be included in the output.
-        
-        ```py
-        gcode = (
-          'G1 X1 ; this comment is always included\n',
-          '; this comment will only be included if `include_comments=True`',
-        )
-        
-        GcodeParser(gcode, include_comments=True).lines
-        ```
-        
-        If `include_comments` is `True` then the comment line will be in the form of:
-        
-        ```python
-        GcodeLine(
-          command = (';', None),
-          params = {},
-          comment = 'this comment will only be included if `include_comments=True`',
-        )
-        ```
-        
-        ## Converting a File
-        
-        ```python
-        from gcodeparser import GcodeParser
-        
-        with open('3DBenchy.gcode', 'r') as f:
-            gcode = f.read()
-        parsed_gcode = GcodeParser(gcode)
-        parsed_gcode.lines
-        ```
-        
-        _output:_
-        
-        ```py
-        [GcodeLine(command=('G', 10), params={'P': 0, 'R': 0, 'S': 0}, comment='sets the standby temperature'),
-         GcodeLine(command=('G', 29), params={'S': 1}, comment=''),
-         GcodeLine(command=('T', 0), params={}, comment=''),
-         GcodeLine(command=('G', 21), params={}, comment='set units to millimeters'),
-         GcodeLine(command=('G', 90), params={}, comment='use absolute coordinates'),
-         GcodeLine(command=('M', 83), params={}, comment='use relative distances for extrusion'),
-         GcodeLine(command=('G', 1), params={'E': -0.6, 'F': 3600.0}, comment=''),
-         GcodeLine(command=('G', 1), params={'Z': 0.45, 'F': 7800.0}, comment=''),
-         GcodeLine(command=('G', 1), params={'Z': 2.35}, comment=''),
-         GcodeLine(command=('G', 1), params={'X': 119.575, 'Y': 89.986}, comment=''),
-         GcodeLine(command=('G', 1), params={'Z': 0.45}, comment=''),
-         GcodeLine(command=('G', 1), params={'E': 0.6, 'F': 3600.0}, comment=''),
-         GcodeLine(command=('G', 1), params={'F': 1800.0}, comment=''),
-         GcodeLine(command=('G', 1), params={'X': 120.774, 'Y': 88.783, 'E': 0.17459}, comment=''),
-         GcodeLine(command=('G', 1), params={'X': 121.692, 'Y': 88.145, 'E': 0.11492}, comment=''),
-         GcodeLine(command=('G', 1), params={'X': 122.7, 'Y': 87.638, 'E': 0.11596}, comment=''),
-         GcodeLine(command=('G', 1), params={'X': 123.742, 'Y': 87.285, 'E': 0.11317}, comment=''),
-         ...
-        ]
-        ```
-        
-        ## Convert Command Tuple to String
-        
-        The `GcodeLine`class has a property `command_str` which will return the command tuple as a string. ie `('G', 91)` -> `"G91"`.
-        
-        ## Changing back to Gcode String
-        
-        The `GcodeLine` class has a property `gcode_str` which will return the equivalent gcode string.
-        
-        > This was called `to_gcode()` in version 0.0.6 and before.
-        
-        ## Parameters
-        
-        The `GcodeLine` class has a several helper methods to get and manipulate gcode parameters.
-        
-        For an example `GcodeLine` `line`:
-        
-        ### Retrieving Params
-        
-        To retrieve a param, use the method `get_param(param: str, return_type=None, default=None)` which
-        returns the value of the param if it exists, otherwise it will the `default` value.
-        If `return_type` is set, the return value will be type cast.
-        
-        ```python
-        line.get_param('X')
-        ```
-        
-        ### Updating Params
-        
-        To update a param, use the method `update_param(param: str, value: int | float)`
-        
-        ```python
-        line.update_param('X', 10)
-        ```
-        
-        If the param does not exist, it will return `None` else it will return the updated value.
-        
-        ### Deleting Params
-        
-        To delete a param, use the method `delete_param(param: str)`
-        
-        ```python
-        line.delete_param('X')
-        ```
-        
-        ## Converting to DataFrames
-        
-        If for whatever reason you want to convert your list of `GcodeLine` objects into a pandas dataframe, simply use `pd.DataFrame(GcodeParser(gcode).lines)`
-        
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+# GcodeParser
+
+A simple gcode parser that takes a string of text and returns a list where each gcode command is seperated into a python object.
+
+The structure of the python object is:
+
+`G1 X10 Y-2.5 ; this is a comment`
+
+```python
+GcodeLine(
+  command = ('G', 1),
+  params = {'X': 10, 'Y': -2.5},
+  comment = 'this is a comment',
+)
+```
+
+# Install
+
+```
+pip install gcodeparser
+```
+
+Alternatively:
+
+```
+pip install -e "git+https://github.com/AndyEveritt/GcodeParser.git@master#egg=gcodeparser"
+```
+
+# Usage
+
+```python
+from gcodeparser import GcodeParser
+
+# open gcode file and store contents as variable
+with open('my_gcode.gcode', 'r') as f:
+  gcode = f.read()
+
+GcodeParser(gcode).lines    # get parsed gcode lines
+```
+
+## Include Comments
+
+`GcodeParser` takes a second argument called `include_comments` which defaults to `False`. If this is set to `True` then any line from the gcode file which only contains a comment will also be included in the output.
+
+```py
+gcode = (
+  'G1 X1 ; this comment is always included\n',
+  '; this comment will only be included if `include_comments=True`',
+)
+
+GcodeParser(gcode, include_comments=True).lines
+```
+
+If `include_comments` is `True` then the comment line will be in the form of:
+
+```python
+GcodeLine(
+  command = (';', None),
+  params = {},
+  comment = 'this comment will only be included if `include_comments=True`',
+)
+```
+
+## Converting a File
+
+```python
+from gcodeparser import GcodeParser
+
+with open('3DBenchy.gcode', 'r') as f:
+    gcode = f.read()
+parsed_gcode = GcodeParser(gcode)
+parsed_gcode.lines
+```
+
+_output:_
+
+```py
+[GcodeLine(command=('G', 10), params={'P': 0, 'R': 0, 'S': 0}, comment='sets the standby temperature'),
+ GcodeLine(command=('G', 29), params={'S': 1}, comment=''),
+ GcodeLine(command=('T', 0), params={}, comment=''),
+ GcodeLine(command=('G', 21), params={}, comment='set units to millimeters'),
+ GcodeLine(command=('G', 90), params={}, comment='use absolute coordinates'),
+ GcodeLine(command=('M', 83), params={}, comment='use relative distances for extrusion'),
+ GcodeLine(command=('G', 1), params={'E': -0.6, 'F': 3600.0}, comment=''),
+ GcodeLine(command=('G', 1), params={'Z': 0.45, 'F': 7800.0}, comment=''),
+ GcodeLine(command=('G', 1), params={'Z': 2.35}, comment=''),
+ GcodeLine(command=('G', 1), params={'X': 119.575, 'Y': 89.986}, comment=''),
+ GcodeLine(command=('G', 1), params={'Z': 0.45}, comment=''),
+ GcodeLine(command=('G', 1), params={'E': 0.6, 'F': 3600.0}, comment=''),
+ GcodeLine(command=('G', 1), params={'F': 1800.0}, comment=''),
+ GcodeLine(command=('G', 1), params={'X': 120.774, 'Y': 88.783, 'E': 0.17459}, comment=''),
+ GcodeLine(command=('G', 1), params={'X': 121.692, 'Y': 88.145, 'E': 0.11492}, comment=''),
+ GcodeLine(command=('G', 1), params={'X': 122.7, 'Y': 87.638, 'E': 0.11596}, comment=''),
+ GcodeLine(command=('G', 1), params={'X': 123.742, 'Y': 87.285, 'E': 0.11317}, comment=''),
+ ...
+]
+```
+
+## Convert Command Tuple to String
+
+The `GcodeLine`class has a property `command_str` which will return the command tuple as a string. ie `('G', 91)` -> `"G91"`.
+
+## Changing back to Gcode String
+
+The `GcodeLine` class has a property `gcode_str` which will return the equivalent gcode string.
+
+> This was called `to_gcode()` in version 0.0.6 and before.
+
+## Parameters
+
+The `GcodeLine` class has a several helper methods to get and manipulate gcode parameters.
+
+For an example `GcodeLine` `line`:
+
+### Retrieving Params
+
+To retrieve a param, use the method `get_param(param: str, return_type=None, default=None)` which
+returns the value of the param if it exists, otherwise it will the `default` value.
+If `return_type` is set, the return value will be type cast.
+
+```python
+line.get_param('X')
+```
+
+### Updating Params
+
+To update a param, use the method `update_param(param: str, value: int | float)`
+
+```python
+line.update_param('X', 10)
+```
+
+If the param does not exist, it will return `None` else it will return the updated value.
+
+### Deleting Params
+
+To delete a param, use the method `delete_param(param: str)`
+
+```python
+line.delete_param('X')
+```
+
+## Converting to DataFrames
+
+If for whatever reason you want to convert your list of `GcodeLine` objects into a pandas dataframe, simply use `pd.DataFrame(GcodeParser(gcode).lines)`
```

### Comparing `gcodeparser-0.1.0/README.md` & `gcodeparser-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: gcodeparser
+Version: 0.1.1
+Summary: Python gcode parser
+Home-page: https://github.com/AndyEveritt/GcodeParser
+Author: Andy Everitt
+Author-email: andreweveritt@e3d-online.com
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # GcodeParser
 
 A simple gcode parser that takes a string of text and returns a list where each gcode command is seperated into a python object.
 
 The structure of the python object is:
 
 `G1 X10 Y-2.5 ; this is a comment`
```

### Comparing `gcodeparser-0.1.0/gcodeparser/gcode_parser.py` & `gcodeparser-0.1.1/gcodeparser/gcode_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,15 +49,23 @@
         if self.get_param(param) is None:
             return
         self.params.pop(param)
 
     @property
     def gcode_str(self):
         command = self.command_str
-        params = " ".join(f"{param}{self.get_param(param)}" for param in self.params.keys())
+
+        def param_value(param):
+            value = self.get_param(param)
+            is_flag_parameter = value is True
+            if is_flag_parameter:
+                return ""
+            return value
+
+        params = " ".join(f"{param}{param_value(param)}" for param in self.params.keys())
         comment = f"; {self.comment}" if self.comment != '' else ""
         if command == ';':
             return comment
         return f"{command} {params} {comment}".strip()
 
 
 class GcodeParser:
```

### Comparing `gcodeparser-0.1.0/gcodeparser.egg-info/PKG-INFO` & `gcodeparser-0.1.1/gcodeparser.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,159 +1,158 @@
 Metadata-Version: 2.1
 Name: gcodeparser
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python gcode parser
 Home-page: https://github.com/AndyEveritt/GcodeParser
 Author: Andy Everitt
 Author-email: andreweveritt@e3d-online.com
-License: UNKNOWN
-Description: # GcodeParser
-        
-        A simple gcode parser that takes a string of text and returns a list where each gcode command is seperated into a python object.
-        
-        The structure of the python object is:
-        
-        `G1 X10 Y-2.5 ; this is a comment`
-        
-        ```python
-        GcodeLine(
-          command = ('G', 1),
-          params = {'X': 10, 'Y': -2.5},
-          comment = 'this is a comment',
-        )
-        ```
-        
-        # Install
-        
-        ```
-        pip install gcodeparser
-        ```
-        
-        Alternatively:
-        
-        ```
-        pip install -e "git+https://github.com/AndyEveritt/GcodeParser.git@master#egg=gcodeparser"
-        ```
-        
-        # Usage
-        
-        ```python
-        from gcodeparser import GcodeParser
-        
-        # open gcode file and store contents as variable
-        with open('my_gcode.gcode', 'r') as f:
-          gcode = f.read()
-        
-        GcodeParser(gcode).lines    # get parsed gcode lines
-        ```
-        
-        ## Include Comments
-        
-        `GcodeParser` takes a second argument called `include_comments` which defaults to `False`. If this is set to `True` then any line from the gcode file which only contains a comment will also be included in the output.
-        
-        ```py
-        gcode = (
-          'G1 X1 ; this comment is always included\n',
-          '; this comment will only be included if `include_comments=True`',
-        )
-        
-        GcodeParser(gcode, include_comments=True).lines
-        ```
-        
-        If `include_comments` is `True` then the comment line will be in the form of:
-        
-        ```python
-        GcodeLine(
-          command = (';', None),
-          params = {},
-          comment = 'this comment will only be included if `include_comments=True`',
-        )
-        ```
-        
-        ## Converting a File
-        
-        ```python
-        from gcodeparser import GcodeParser
-        
-        with open('3DBenchy.gcode', 'r') as f:
-            gcode = f.read()
-        parsed_gcode = GcodeParser(gcode)
-        parsed_gcode.lines
-        ```
-        
-        _output:_
-        
-        ```py
-        [GcodeLine(command=('G', 10), params={'P': 0, 'R': 0, 'S': 0}, comment='sets the standby temperature'),
-         GcodeLine(command=('G', 29), params={'S': 1}, comment=''),
-         GcodeLine(command=('T', 0), params={}, comment=''),
-         GcodeLine(command=('G', 21), params={}, comment='set units to millimeters'),
-         GcodeLine(command=('G', 90), params={}, comment='use absolute coordinates'),
-         GcodeLine(command=('M', 83), params={}, comment='use relative distances for extrusion'),
-         GcodeLine(command=('G', 1), params={'E': -0.6, 'F': 3600.0}, comment=''),
-         GcodeLine(command=('G', 1), params={'Z': 0.45, 'F': 7800.0}, comment=''),
-         GcodeLine(command=('G', 1), params={'Z': 2.35}, comment=''),
-         GcodeLine(command=('G', 1), params={'X': 119.575, 'Y': 89.986}, comment=''),
-         GcodeLine(command=('G', 1), params={'Z': 0.45}, comment=''),
-         GcodeLine(command=('G', 1), params={'E': 0.6, 'F': 3600.0}, comment=''),
-         GcodeLine(command=('G', 1), params={'F': 1800.0}, comment=''),
-         GcodeLine(command=('G', 1), params={'X': 120.774, 'Y': 88.783, 'E': 0.17459}, comment=''),
-         GcodeLine(command=('G', 1), params={'X': 121.692, 'Y': 88.145, 'E': 0.11492}, comment=''),
-         GcodeLine(command=('G', 1), params={'X': 122.7, 'Y': 87.638, 'E': 0.11596}, comment=''),
-         GcodeLine(command=('G', 1), params={'X': 123.742, 'Y': 87.285, 'E': 0.11317}, comment=''),
-         ...
-        ]
-        ```
-        
-        ## Convert Command Tuple to String
-        
-        The `GcodeLine`class has a property `command_str` which will return the command tuple as a string. ie `('G', 91)` -> `"G91"`.
-        
-        ## Changing back to Gcode String
-        
-        The `GcodeLine` class has a property `gcode_str` which will return the equivalent gcode string.
-        
-        > This was called `to_gcode()` in version 0.0.6 and before.
-        
-        ## Parameters
-        
-        The `GcodeLine` class has a several helper methods to get and manipulate gcode parameters.
-        
-        For an example `GcodeLine` `line`:
-        
-        ### Retrieving Params
-        
-        To retrieve a param, use the method `get_param(param: str, return_type=None, default=None)` which
-        returns the value of the param if it exists, otherwise it will the `default` value.
-        If `return_type` is set, the return value will be type cast.
-        
-        ```python
-        line.get_param('X')
-        ```
-        
-        ### Updating Params
-        
-        To update a param, use the method `update_param(param: str, value: int | float)`
-        
-        ```python
-        line.update_param('X', 10)
-        ```
-        
-        If the param does not exist, it will return `None` else it will return the updated value.
-        
-        ### Deleting Params
-        
-        To delete a param, use the method `delete_param(param: str)`
-        
-        ```python
-        line.delete_param('X')
-        ```
-        
-        ## Converting to DataFrames
-        
-        If for whatever reason you want to convert your list of `GcodeLine` objects into a pandas dataframe, simply use `pd.DataFrame(GcodeParser(gcode).lines)`
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# GcodeParser
+
+A simple gcode parser that takes a string of text and returns a list where each gcode command is seperated into a python object.
+
+The structure of the python object is:
+
+`G1 X10 Y-2.5 ; this is a comment`
+
+```python
+GcodeLine(
+  command = ('G', 1),
+  params = {'X': 10, 'Y': -2.5},
+  comment = 'this is a comment',
+)
+```
+
+# Install
+
+```
+pip install gcodeparser
+```
+
+Alternatively:
+
+```
+pip install -e "git+https://github.com/AndyEveritt/GcodeParser.git@master#egg=gcodeparser"
+```
+
+# Usage
+
+```python
+from gcodeparser import GcodeParser
+
+# open gcode file and store contents as variable
+with open('my_gcode.gcode', 'r') as f:
+  gcode = f.read()
+
+GcodeParser(gcode).lines    # get parsed gcode lines
+```
+
+## Include Comments
+
+`GcodeParser` takes a second argument called `include_comments` which defaults to `False`. If this is set to `True` then any line from the gcode file which only contains a comment will also be included in the output.
+
+```py
+gcode = (
+  'G1 X1 ; this comment is always included\n',
+  '; this comment will only be included if `include_comments=True`',
+)
+
+GcodeParser(gcode, include_comments=True).lines
+```
+
+If `include_comments` is `True` then the comment line will be in the form of:
+
+```python
+GcodeLine(
+  command = (';', None),
+  params = {},
+  comment = 'this comment will only be included if `include_comments=True`',
+)
+```
+
+## Converting a File
+
+```python
+from gcodeparser import GcodeParser
+
+with open('3DBenchy.gcode', 'r') as f:
+    gcode = f.read()
+parsed_gcode = GcodeParser(gcode)
+parsed_gcode.lines
+```
+
+_output:_
+
+```py
+[GcodeLine(command=('G', 10), params={'P': 0, 'R': 0, 'S': 0}, comment='sets the standby temperature'),
+ GcodeLine(command=('G', 29), params={'S': 1}, comment=''),
+ GcodeLine(command=('T', 0), params={}, comment=''),
+ GcodeLine(command=('G', 21), params={}, comment='set units to millimeters'),
+ GcodeLine(command=('G', 90), params={}, comment='use absolute coordinates'),
+ GcodeLine(command=('M', 83), params={}, comment='use relative distances for extrusion'),
+ GcodeLine(command=('G', 1), params={'E': -0.6, 'F': 3600.0}, comment=''),
+ GcodeLine(command=('G', 1), params={'Z': 0.45, 'F': 7800.0}, comment=''),
+ GcodeLine(command=('G', 1), params={'Z': 2.35}, comment=''),
+ GcodeLine(command=('G', 1), params={'X': 119.575, 'Y': 89.986}, comment=''),
+ GcodeLine(command=('G', 1), params={'Z': 0.45}, comment=''),
+ GcodeLine(command=('G', 1), params={'E': 0.6, 'F': 3600.0}, comment=''),
+ GcodeLine(command=('G', 1), params={'F': 1800.0}, comment=''),
+ GcodeLine(command=('G', 1), params={'X': 120.774, 'Y': 88.783, 'E': 0.17459}, comment=''),
+ GcodeLine(command=('G', 1), params={'X': 121.692, 'Y': 88.145, 'E': 0.11492}, comment=''),
+ GcodeLine(command=('G', 1), params={'X': 122.7, 'Y': 87.638, 'E': 0.11596}, comment=''),
+ GcodeLine(command=('G', 1), params={'X': 123.742, 'Y': 87.285, 'E': 0.11317}, comment=''),
+ ...
+]
+```
+
+## Convert Command Tuple to String
+
+The `GcodeLine`class has a property `command_str` which will return the command tuple as a string. ie `('G', 91)` -> `"G91"`.
+
+## Changing back to Gcode String
+
+The `GcodeLine` class has a property `gcode_str` which will return the equivalent gcode string.
+
+> This was called `to_gcode()` in version 0.0.6 and before.
+
+## Parameters
+
+The `GcodeLine` class has a several helper methods to get and manipulate gcode parameters.
+
+For an example `GcodeLine` `line`:
+
+### Retrieving Params
+
+To retrieve a param, use the method `get_param(param: str, return_type=None, default=None)` which
+returns the value of the param if it exists, otherwise it will the `default` value.
+If `return_type` is set, the return value will be type cast.
+
+```python
+line.get_param('X')
+```
+
+### Updating Params
+
+To update a param, use the method `update_param(param: str, value: int | float)`
+
+```python
+line.update_param('X', 10)
+```
+
+If the param does not exist, it will return `None` else it will return the updated value.
+
+### Deleting Params
+
+To delete a param, use the method `delete_param(param: str)`
+
+```python
+line.delete_param('X')
+```
+
+## Converting to DataFrames
+
+If for whatever reason you want to convert your list of `GcodeLine` objects into a pandas dataframe, simply use `pd.DataFrame(GcodeParser(gcode).lines)`
```

### Comparing `gcodeparser-0.1.0/setup.py` & `gcodeparser-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="gcodeparser",
-    version="0.1.0",
+    version="0.1.1",
     include_package_data=True,
     packages=find_packages(),
 
     install_requires=[
     ],
 
     author="Andy Everitt",
```

### Comparing `gcodeparser-0.1.0/test/test_get_lines.py` & `gcodeparser-0.1.1/test/test_get_lines.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-from gcodeparser.gcode_parser import (
-    GcodeLine,
-    GcodeParser,
-    get_lines,
-    element_type,
-    split_params,
-)
-from gcodeparser.commands import Commands
-
-
-def test_no_params():
-    line = GcodeLine(
-        command=('G', 21),
-        params={},
-        comment='',
-    )
-    assert get_lines('G21')[0] == line
-
-
-def test_params():
-    line = GcodeLine(
-        command=('G', 1),
-        params={'X': 10, 'Y': 20},
-        comment='',
-    )
-    assert get_lines('G1 X10 Y20')[0] == line
-
-
-def test_2_commands_line():
-    line1 = GcodeLine(
-        command=('G', 91),
-        params={},
-        comment='',
-    )
-    line2 = GcodeLine(
-        command=('G', 1),
-        params={'X': 10, 'Y': 20},
-        comment='',
-    )
-    lines = get_lines('G91 G1 X10 Y20')
-    assert lines[0] == line1
-    assert lines[1] == line2
-
-
-def test_string_params():
-    line = GcodeLine(
-        command=('M', 550),
-        params={'P': '"hostname"'},
-        comment='',
-    )
-    assert get_lines('M550 P"hostname"')[0] == line
-
-
-def test_ip_address_params():
-    line = GcodeLine(
-        command=('M', 552),
-        params={'P': '192.168.0.1', 'S': 1},
-        comment='',
-    )
-    assert get_lines('M552 P192.168.0.1 S1')[0] == line
-
-
-def test_inline_comment():
-    line = GcodeLine(
-        command=('G', 1),
-        params={'X': 10, 'Y': 20},
-        comment='this is a comment',
-    )
-    assert get_lines('G1 X10 Y20 ; this is a comment')[0] == line
-    assert get_lines('G1 X10 Y20 ;      this is a comment')[0] == line
-    assert get_lines('G1 X10 Y20 \t;     \t this is a comment')[0] == line
-    assert get_lines('G1 X10 Y20 \t;     \t this is a comment')[0] == line
-
-
-def test_inline_comment2():
-    line = GcodeLine(
-        command=('G', 1),
-        params={'X': 10, 'Y': 20},
-        comment='this is a comment ; with a dummy comment for bants',
-    )
-    assert get_lines('G1 X10 Y20 ; this is a comment ; with a dummy comment for bants')[0] == line
-
-
-def test_include_comment_true():
-    line = GcodeLine(
-        command=(';', None),
-        params={},
-        comment='this is a comment',
-    )
-    assert get_lines('; this is a comment', include_comments=True)[0] == line
-
-
-def test_include_comment_false():
-    assert len(get_lines('; this is a comment', include_comments=False)) == 0
-
-
-def test_multi_line():
-    lines = [
-        GcodeLine(
-            command=('G', 91),
-            params={},
-            comment='',
-        ), GcodeLine(
-            command=('G', 1),
-            params={'X': -10, 'Y': 20},
-            comment='inline comment',
-        ), GcodeLine(
-            command=('G', 1),
-            params={'Z': 0.5},
-            comment='',
-        ), GcodeLine(
-            command=('T', 1),
-            params={},
-            comment='',
-        ), GcodeLine(
-            command=('M', 350),
-            params={'T': 100},
-            comment='',
-        )]
-    assert get_lines('G91\nG1 X-10 Y20 ; inline comment\nG1 Z0.5\nT1\nM350 T100') == lines
-    assert get_lines('G91G1 X-10 Y20;inline comment\nG1 Z0.5\nT1M350 T100') == lines
-    assert get_lines(' \tG91\n\tG1\t  X-10 Y20 \t ;\t inline comment\nG1 Z0.5\nT1\nM350 T100') == lines
-    assert get_lines('G91\nG1 X-10 Y20 ; inline comment\n; comment to be excluded\nG1 Z0.5\nT1\nM350 T100', include_comments=False) == lines
+from gcodeparser.gcode_parser import (
+    GcodeLine,
+    GcodeParser,
+    get_lines,
+    element_type,
+    split_params,
+)
+from gcodeparser.commands import Commands
+
+
+def test_no_params():
+    line = GcodeLine(
+        command=('G', 21),
+        params={},
+        comment='',
+    )
+    assert get_lines('G21')[0] == line
+
+
+def test_params():
+    line = GcodeLine(
+        command=('G', 1),
+        params={'X': 10, 'Y': 20},
+        comment='',
+    )
+    assert get_lines('G1 X10 Y20')[0] == line
+
+
+def test_2_commands_line():
+    line1 = GcodeLine(
+        command=('G', 91),
+        params={},
+        comment='',
+    )
+    line2 = GcodeLine(
+        command=('G', 1),
+        params={'X': 10, 'Y': 20},
+        comment='',
+    )
+    lines = get_lines('G91 G1 X10 Y20')
+    assert lines[0] == line1
+    assert lines[1] == line2
+
+
+def test_string_params():
+    line = GcodeLine(
+        command=('M', 550),
+        params={'P': '"hostname"'},
+        comment='',
+    )
+    assert get_lines('M550 P"hostname"')[0] == line
+
+
+def test_ip_address_params():
+    line = GcodeLine(
+        command=('M', 552),
+        params={'P': '192.168.0.1', 'S': 1},
+        comment='',
+    )
+    assert get_lines('M552 P192.168.0.1 S1')[0] == line
+
+
+def test_inline_comment():
+    line = GcodeLine(
+        command=('G', 1),
+        params={'X': 10, 'Y': 20},
+        comment='this is a comment',
+    )
+    assert get_lines('G1 X10 Y20 ; this is a comment')[0] == line
+    assert get_lines('G1 X10 Y20 ;      this is a comment')[0] == line
+    assert get_lines('G1 X10 Y20 \t;     \t this is a comment')[0] == line
+    assert get_lines('G1 X10 Y20 \t;     \t this is a comment')[0] == line
+
+
+def test_inline_comment2():
+    line = GcodeLine(
+        command=('G', 1),
+        params={'X': 10, 'Y': 20},
+        comment='this is a comment ; with a dummy comment for bants',
+    )
+    assert get_lines('G1 X10 Y20 ; this is a comment ; with a dummy comment for bants')[0] == line
+
+
+def test_include_comment_true():
+    line = GcodeLine(
+        command=(';', None),
+        params={},
+        comment='this is a comment',
+    )
+    assert get_lines('; this is a comment', include_comments=True)[0] == line
+
+
+def test_include_comment_false():
+    assert len(get_lines('; this is a comment', include_comments=False)) == 0
+
+
+def test_multi_line():
+    lines = [
+        GcodeLine(
+            command=('G', 91),
+            params={},
+            comment='',
+        ), GcodeLine(
+            command=('G', 1),
+            params={'X': -10, 'Y': 20},
+            comment='inline comment',
+        ), GcodeLine(
+            command=('G', 1),
+            params={'Z': 0.5},
+            comment='',
+        ), GcodeLine(
+            command=('T', 1),
+            params={},
+            comment='',
+        ), GcodeLine(
+            command=('M', 350),
+            params={'T': 100},
+            comment='',
+        )]
+    assert get_lines('G91\nG1 X-10 Y20 ; inline comment\nG1 Z0.5\nT1\nM350 T100') == lines
+    assert get_lines('G91G1 X-10 Y20;inline comment\nG1 Z0.5\nT1M350 T100') == lines
+    assert get_lines(' \tG91\n\tG1\t  X-10 Y20 \t ;\t inline comment\nG1 Z0.5\nT1\nM350 T100') == lines
+    assert get_lines('G91\nG1 X-10 Y20 ; inline comment\n; comment to be excluded\nG1 Z0.5\nT1\nM350 T100', include_comments=False) == lines
```

