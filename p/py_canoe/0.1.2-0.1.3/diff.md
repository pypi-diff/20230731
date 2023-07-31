# Comparing `tmp/py_canoe-0.1.2.tar.gz` & `tmp/py_canoe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_canoe-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_canoe-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_canoe-0.1.2.tar` & `py_canoe-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     3699 2023-06-21 03:21:26.026953 py_canoe-0.1.2/.gitignore
--rw-r--r--   0        0        0     5330 2023-06-21 02:44:58.263085 py_canoe-0.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1095 2023-06-21 02:44:58.263085 py_canoe-0.1.2/LICENSE
--rw-r--r--   0        0        0     1919 2023-06-21 02:44:58.263085 py_canoe-0.1.2/README.md
--rw-r--r--   0        0        0      147 2023-06-21 02:44:58.263085 py_canoe-0.1.2/_config.yml
--rw-r--r--   0        0        0     1852 2023-06-21 02:44:58.273095 py_canoe-0.1.2/docs/index.md
--rw-r--r--   0        0        0      507 2023-06-21 02:44:58.273095 py_canoe-0.1.2/mkdocs.yml
--rw-r--r--   0        0        0      668 2023-06-21 02:44:58.273095 py_canoe-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       60 2023-06-21 02:44:58.273095 py_canoe-0.1.2/requirements.txt
--rwxr-xr-x   0        0        0      635 2023-06-29 17:56:00.911096 py_canoe-0.1.2/scripts/deploy_docs_to_github.bat
--rwxr-xr-x   0        0        0     1526 2023-06-29 17:56:00.911096 py_canoe-0.1.2/scripts/install_dependencies.bat
--rwxr-xr-x   0        0        0      589 2023-06-21 02:44:58.273095 py_canoe-0.1.2/scripts/run_pytests.bat
--rwxr-xr-x   0        0        0      608 2023-06-21 02:44:58.273095 py_canoe-0.1.2/scripts/upload_package_to_pypi.bat
--rw-r--r--   0        0        0        0 2023-06-29 17:34:50.054974 py_canoe-0.1.2/src/__int__.py
--rw-r--r--   0        0        0    47414 2023-07-01 18:10:39.507550 py_canoe-0.1.2/src/py_canoe.py
--rw-r--r--   0        0        0       31 2023-06-21 02:44:58.283091 py_canoe-0.1.2/tests/__int__.py
--rw-r--r--   0        0        0     2192 2023-06-21 02:44:58.283091 py_canoe-0.1.2/tests/demo_cfg/CANdb/easy.dbc
--rw-r--r--   0        0        0  1106768 2023-06-21 02:44:58.293092 py_canoe-0.1.2/tests/demo_cfg/CDD/UDS-ExampleEcu-5.0.2.cdd
--rw-r--r--   0        0        0    11560 2023-06-29 17:34:50.054974 py_canoe-0.1.2/tests/demo_cfg/Logs/demo_log.blf
--rw-r--r--   0        0        0     3708 2023-06-21 02:44:58.293092 py_canoe-0.1.2/tests/demo_cfg/Nodes/SimDiagECU.can
--rw-r--r--   0        0        0      928 2023-06-21 02:44:58.293092 py_canoe-0.1.2/tests/demo_cfg/Nodes/system_events.can
--rw-r--r--   0        0        0      256 2023-06-21 02:44:58.293092 py_canoe-0.1.2/tests/demo_cfg/Nodes/system_variables.can
--rw-r--r--   0        0        0     5436 2023-06-21 02:44:58.303089 py_canoe-0.1.2/tests/demo_cfg/Panels/sys_var_demo_panel.xvp
--rw-r--r--   0        0        0   203010 2023-06-29 17:34:50.064968 py_canoe-0.1.2/tests/demo_cfg/demo.cfg
--rw-r--r--   0        0        0   194788 2023-06-29 17:34:50.064968 py_canoe-0.1.2/tests/demo_cfg/demo_offline.cfg
--rw-r--r--   0        0        0     3925 2023-07-01 18:13:10.224114 py_canoe-0.1.2/tests/test_canoe.py
--rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 py_canoe-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3697 2023-07-31 18:39:54.265699 py_canoe-0.1.3/.gitignore
+-rw-r--r--   0        0        0     5330 2023-06-21 02:44:58.263085 py_canoe-0.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1095 2023-06-21 02:44:58.263085 py_canoe-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1919 2023-06-21 02:44:58.263085 py_canoe-0.1.3/README.md
+-rw-r--r--   0        0        0      147 2023-06-21 02:44:58.263085 py_canoe-0.1.3/_config.yml
+-rw-r--r--   0        0        0     1852 2023-06-21 02:44:58.273095 py_canoe-0.1.3/docs/index.md
+-rw-r--r--   0        0        0      507 2023-06-21 02:44:58.273095 py_canoe-0.1.3/mkdocs.yml
+-rw-r--r--   0        0        0      668 2023-06-21 02:44:58.273095 py_canoe-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-06-21 02:44:58.273095 py_canoe-0.1.3/requirements.txt
+-rwxr-xr-x   0        0        0      635 2023-06-29 17:56:00.911096 py_canoe-0.1.3/scripts/deploy_docs_to_github.bat
+-rwxr-xr-x   0        0        0     1526 2023-06-29 17:56:00.911096 py_canoe-0.1.3/scripts/install_dependencies.bat
+-rwxr-xr-x   0        0        0      589 2023-06-21 02:44:58.273095 py_canoe-0.1.3/scripts/run_pytests.bat
+-rwxr-xr-x   0        0        0      608 2023-06-21 02:44:58.273095 py_canoe-0.1.3/scripts/upload_package_to_pypi.bat
+-rw-r--r--   0        0        0        0 2023-06-29 17:34:50.054974 py_canoe-0.1.3/src/__int__.py
+-rw-r--r--   0        0        0    49533 2023-07-31 18:54:18.872443 py_canoe-0.1.3/src/py_canoe.py
+-rw-r--r--   0        0        0       31 2023-06-21 02:44:58.283091 py_canoe-0.1.3/tests/__int__.py
+-rw-r--r--   0        0        0     2192 2023-06-21 02:44:58.283091 py_canoe-0.1.3/tests/demo_cfg/CANdb/easy.dbc
+-rw-r--r--   0        0        0  1106768 2023-06-21 02:44:58.293092 py_canoe-0.1.3/tests/demo_cfg/CDD/UDS-ExampleEcu-5.0.2.cdd
+-rw-r--r--   0        0        0    11560 2023-06-29 17:34:50.054974 py_canoe-0.1.3/tests/demo_cfg/Logs/demo_log.blf
+-rw-r--r--   0        0        0     3708 2023-06-21 02:44:58.293092 py_canoe-0.1.3/tests/demo_cfg/Nodes/SimDiagECU.can
+-rw-r--r--   0        0        0      928 2023-06-21 02:44:58.293092 py_canoe-0.1.3/tests/demo_cfg/Nodes/system_events.can
+-rw-r--r--   0        0        0      256 2023-06-21 02:44:58.293092 py_canoe-0.1.3/tests/demo_cfg/Nodes/system_variables.can
+-rw-r--r--   0        0        0     5436 2023-06-21 02:44:58.303089 py_canoe-0.1.3/tests/demo_cfg/Panels/sys_var_demo_panel.xvp
+-rw-r--r--   0        0        0   203010 2023-07-31 18:36:47.204695 py_canoe-0.1.3/tests/demo_cfg/demo.cfg
+-rw-r--r--   0        0        0   194788 2023-06-29 17:34:50.064968 py_canoe-0.1.3/tests/demo_cfg/demo_offline.cfg
+-rw-r--r--   0        0        0     4275 2023-07-31 18:45:55.657606 py_canoe-0.1.3/tests/test_canoe.py
+-rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 py_canoe-0.1.3/PKG-INFO
```

### Comparing `py_canoe-0.1.2/.gitignore` & `py_canoe-0.1.3/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -167,13 +167,14 @@
 ### Python Patch ###
 # Poetry local configuration file - https://python-poetry.org/docs/configuration/#local-configuration
 poetry.toml
 
 
 # End of https://www.toptal.com/developers/gitignore/api/python
 
-# pycharm and vscode ettings
+# pycharm and vscode
 .idea/
 .vscode/
 # CANoe Files
 *.cbf
 *.stcfg
+.vs/
```

### Comparing `py_canoe-0.1.2/CODE_OF_CONDUCT.md` & `py_canoe-0.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/LICENSE` & `py_canoe-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/README.md` & `py_canoe-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/docs/index.md` & `py_canoe-0.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/pyproject.toml` & `py_canoe-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/scripts/deploy_docs_to_github.bat` & `py_canoe-0.1.3/scripts/deploy_docs_to_github.bat`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/scripts/install_dependencies.bat` & `py_canoe-0.1.3/scripts/install_dependencies.bat`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/scripts/run_pytests.bat` & `py_canoe-0.1.3/scripts/run_pytests.bat`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/scripts/upload_package_to_pypi.bat` & `py_canoe-0.1.3/scripts/upload_package_to_pypi.bat`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/src/py_canoe.py` & `py_canoe-0.1.3/src/py_canoe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Python package for controlling Vector CANoe tool"""
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 # Import Python Libraries here
 import os
 import sys
 import logging
 import pythoncom
 import win32com.client
@@ -802,14 +802,54 @@
                         'patch': self.__canoe_objects['Application'].Version.Patch}
         self.log.info('> CANoe Application.Version <'.center(100, '='))
         for k, v in version_info.items():
             self.log.info(f'{k:<10}: {v}')
         self.log.info(''.center(100, '='))
         return version_info
 
+    def define_system_namespace(self, sys_namespace: str):
+        """define_system_namespace Create a namespace for variables
+        Args:
+            sys_namespace (str): The name of the system namespace. Ex- "sys_var_demo"
+        Examples:
+            >>> # The following example gets system variable value
+            >>> canoe_inst = CANoe()
+            >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
+            >>> canoe_inst.define_system_namespace('sys_demo')
+        """
+        namespace_already_available = False
+        for n in self.__canoe_objects['Namespaces']:
+            if n.Name == sys_namespace:
+                namespace_already_available = True
+        if namespace_already_available:
+            self.log.info(f'namespace ({sys_namespace}) already available.')
+        else:
+            self.__canoe_objects['Namespaces'].Add(sys_namespace)
+            self.log.info(f'namespace ({sys_namespace}) created.')
+
+    def define_system_variable(self, sys_var_name: str, value: Union[int, float, str]):
+        """define_system_variable Create a system variable with an initial value
+        Args:
+            sys_var_name (str): The name of the system variable. Ex- "sys_var_demo::speed"
+            value (Union[int, float, str]): variable value.
+        Examples:
+            >>> # The following example gets system variable value
+            >>> canoe_inst = CANoe()
+            >>> canoe_inst.open(r'D:\_kms_local\vector_canoe\py_canoe\demo_cfg\demo.cfg')
+            >>> canoe_inst.define_system_variable('sys_demo::speed', 1)
+        """
+        namespace = '::'.join(sys_var_name.split('::')[:-1])
+        variable_name = sys_var_name.split('::')[-1]
+        try:
+            namespace_object = self.__canoe_objects['Namespaces'](namespace)
+            namespace_object.Variables.Add(variable_name, value)
+            self.log.info(f'system variable({sys_var_name}) created with value set to {value}.')
+        except Exception as e:
+            self.log.info(f'failed to create system variable({sys_var_name}). {e}')
+
     def get_system_variable_value(self, sys_var_name: str) -> Union[int, float, str]:
         r"""get_system_variable_value Returns a system variable value.
 
         Args:
             sys_var_name (str): The name of the system variable. Ex- "sys_var_demo::speed"
 
         Returns:
```

### Comparing `py_canoe-0.1.2/tests/demo_cfg/CANdb/easy.dbc` & `py_canoe-0.1.3/tests/demo_cfg/CANdb/easy.dbc`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/tests/demo_cfg/CDD/UDS-ExampleEcu-5.0.2.cdd` & `py_canoe-0.1.3/tests/demo_cfg/CDD/UDS-ExampleEcu-5.0.2.cdd`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/tests/demo_cfg/Logs/demo_log.blf` & `py_canoe-0.1.3/tests/demo_cfg/Logs/demo_log.blf`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/tests/demo_cfg/Nodes/SimDiagECU.can` & `py_canoe-0.1.3/tests/demo_cfg/Nodes/SimDiagECU.can`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/tests/demo_cfg/Nodes/system_events.can` & `py_canoe-0.1.3/tests/demo_cfg/Nodes/system_events.can`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/tests/demo_cfg/Panels/sys_var_demo_panel.xvp` & `py_canoe-0.1.3/tests/demo_cfg/Panels/sys_var_demo_panel.xvp`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/tests/demo_cfg/demo.cfg` & `py_canoe-0.1.3/tests/demo_cfg/demo.cfg`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/tests/demo_cfg/demo_offline.cfg` & `py_canoe-0.1.3/tests/demo_cfg/demo_offline.cfg`

 * *Files identical despite different names*

### Comparing `py_canoe-0.1.2/tests/test_canoe.py` & `py_canoe-0.1.3/tests/test_canoe.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,22 @@
     assert canoe_inst.start_measurement()
     wait(1)
     canoe_inst.set_system_variable_value('demo::level_two_1::sys_var2', 20)
     wait(1)
     sys_var_val = canoe_inst.get_system_variable_value('demo::level_two_1::sys_var2')
     assert canoe_inst.stop_measurement()
     assert sys_var_val == 20
+    canoe_inst.define_system_namespace('sys_demo')
+    canoe_inst.define_system_variable('sys_demo::demo', 1)
+    canoe_inst.save_configuration()
+    assert canoe_inst.start_measurement()
+    wait(1)
+    sys_var_val = canoe_inst.get_system_variable_value('sys_demo::demo')
+    assert sys_var_val == 1
+    assert canoe_inst.stop_measurement()
     wait(2)
 
 def test_canoe_open_close_methods():
     canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
     wait(1)
     canoe_inst.open(fr'{file_path}\demo_cfg\demo.cfg')
     wait(1)
```

### Comparing `py_canoe-0.1.2/PKG-INFO` & `py_canoe-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_canoe
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package for controlling Vector CANoe tool
 Author-email: chaitu-ycr <chaitu.ycr@gmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
```

