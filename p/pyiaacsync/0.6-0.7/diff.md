# Comparing `tmp/pyiaacsync-0.6.tar.gz` & `tmp/pyiaacsync-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyiaacsync-0.6.tar", last modified: Sun Jul 23 03:50:58 2023, max compression
+gzip compressed data, was "dist/pyiaacsync-0.7.tar", last modified: Mon Jul 31 12:30:46 2023, max compression
```

## Comparing `pyiaacsync-0.6.tar` & `pyiaacsync-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2023-07-23 03:50:58.000000 pyiaacsync-0.6/
--rw-r--r--   0 manasbellani   (501) wheel        (0)     5886 2023-07-23 03:50:58.000000 pyiaacsync-0.6/PKG-INFO
--rw-r--r--   0 manasbellani   (501) wheel        (0)     4775 2023-07-23 03:46:36.000000 pyiaacsync-0.6/README.md
-drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2023-07-23 03:50:58.000000 pyiaacsync-0.6/pyiaacsync/
--rw-r--r--   0 manasbellani   (501) wheel        (0)        0 2023-03-17 07:03:20.000000 pyiaacsync-0.6/pyiaacsync/__init__.py
--rw-r--r--   0 manasbellani   (501) wheel        (0)    15268 2023-07-23 02:41:02.000000 pyiaacsync-0.6/pyiaacsync/pyiaacsync.py
-drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2023-07-23 03:50:58.000000 pyiaacsync-0.6/pyiaacsync.egg-info/
--rw-r--r--   0 manasbellani   (501) wheel        (0)     5886 2023-07-23 03:50:58.000000 pyiaacsync-0.6/pyiaacsync.egg-info/PKG-INFO
--rw-r--r--   0 manasbellani   (501) wheel        (0)      235 2023-07-23 03:50:58.000000 pyiaacsync-0.6/pyiaacsync.egg-info/SOURCES.txt
--rw-r--r--   0 manasbellani   (501) wheel        (0)        1 2023-07-23 03:50:58.000000 pyiaacsync-0.6/pyiaacsync.egg-info/dependency_links.txt
--rw-r--r--   0 manasbellani   (501) wheel        (0)        7 2023-07-23 03:50:58.000000 pyiaacsync-0.6/pyiaacsync.egg-info/requires.txt
--rw-r--r--   0 manasbellani   (501) wheel        (0)       11 2023-07-23 03:50:58.000000 pyiaacsync-0.6/pyiaacsync.egg-info/top_level.txt
--rw-r--r--   0 manasbellani   (501) wheel        (0)       38 2023-07-23 03:50:58.000000 pyiaacsync-0.6/setup.cfg
--rw-r--r--   0 manasbellani   (501) wheel        (0)      864 2023-07-23 03:41:33.000000 pyiaacsync-0.6/setup.py
+drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2023-07-31 12:30:46.000000 pyiaacsync-0.7/
+-rw-r--r--   0 manasbellani   (501) wheel        (0)     6189 2023-07-31 12:30:46.000000 pyiaacsync-0.7/PKG-INFO
+-rw-r--r--   0 manasbellani   (501) wheel        (0)     5062 2023-07-23 03:54:05.000000 pyiaacsync-0.7/README.md
+drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2023-07-31 12:30:46.000000 pyiaacsync-0.7/pyiaacsync/
+-rw-r--r--   0 manasbellani   (501) wheel        (0)        0 2023-03-17 07:03:20.000000 pyiaacsync-0.7/pyiaacsync/__init__.py
+-rw-r--r--   0 manasbellani   (501) wheel        (0)    16485 2023-07-31 12:17:17.000000 pyiaacsync-0.7/pyiaacsync/pyiaacsync.py
+drwxr-xr-x   0 manasbellani   (501) wheel        (0)        0 2023-07-31 12:30:46.000000 pyiaacsync-0.7/pyiaacsync.egg-info/
+-rw-r--r--   0 manasbellani   (501) wheel        (0)     6189 2023-07-31 12:30:46.000000 pyiaacsync-0.7/pyiaacsync.egg-info/PKG-INFO
+-rw-r--r--   0 manasbellani   (501) wheel        (0)      235 2023-07-31 12:30:46.000000 pyiaacsync-0.7/pyiaacsync.egg-info/SOURCES.txt
+-rw-r--r--   0 manasbellani   (501) wheel        (0)        1 2023-07-31 12:30:46.000000 pyiaacsync-0.7/pyiaacsync.egg-info/dependency_links.txt
+-rw-r--r--   0 manasbellani   (501) wheel        (0)        7 2023-07-31 12:30:46.000000 pyiaacsync-0.7/pyiaacsync.egg-info/requires.txt
+-rw-r--r--   0 manasbellani   (501) wheel        (0)       11 2023-07-31 12:30:46.000000 pyiaacsync-0.7/pyiaacsync.egg-info/top_level.txt
+-rw-r--r--   0 manasbellani   (501) wheel        (0)       38 2023-07-31 12:30:46.000000 pyiaacsync-0.7/setup.cfg
+-rw-r--r--   0 manasbellani   (501) wheel        (0)      864 2023-07-31 12:20:26.000000 pyiaacsync-0.7/setup.py
```

### Comparing `pyiaacsync-0.6/PKG-INFO` & `pyiaacsync-0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiaacsync
-Version: 0.6
+Version: 0.7
 Summary: Deploy infrastructure as code via polling
 Home-page: https://github.com/manasmbellani/pyiaacsync
 License: UNKNOWN
 Description: # PyIAACSync
         
         ## Introduction
         infrastructure-as-code tools such as Terraform and Palumi are gaining popularity and increasingly becoming neceessary to support the principles of Site Reliability Engineering (SRE). 
@@ -58,14 +58,16 @@
         ```
         ...
             random_args = {}
             ## uncomment line below to demonstrate how the random arguments can work
             #random_args = {'message': 'hello world'}
         ```
         
+        *Note*: An additional example has been added in folder called `example-fileasset-with-update` where the `fileassetwupd.py` is a python file which additionally includes the `update` method in the `FileAssetWithUpdate` class. The commands listed below also apply to files in this folder.
+        
         ### Actions
         
         #### init
         The first steps is to execute `init` which will create a new state file `out-teststate.yaml`:
         ```
         python3 example.py -a init
         ```
```

### Comparing `pyiaacsync-0.6/README.md` & `pyiaacsync-0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 ```
 ...
     random_args = {}
     ## uncomment line below to demonstrate how the random arguments can work
     #random_args = {'message': 'hello world'}
 ```
 
+*Note*: An additional example has been added in folder called `example-fileasset-with-update` where the `fileassetwupd.py` is a python file which additionally includes the `update` method in the `FileAssetWithUpdate` class. The commands listed below also apply to files in this folder.
+
 ### Actions
 
 #### init
 The first steps is to execute `init` which will create a new state file `out-teststate.yaml`:
 ```
 python3 example.py -a init
 ```
```

### Comparing `pyiaacsync-0.6/pyiaacsync/pyiaacsync.py` & `pyiaacsync-0.7/pyiaacsync/pyiaacsync.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,34 +37,37 @@
 
 class IaacSync:
     """Class used for deploying and syncing IAAC assets defined in an IAAC Sync folder (`iaac_sync_folder`) (e.g. a folder managed via git 
     for version control) that contains various configs describing how to create assets using the `asset` functions
     """
     def __init__(self, iaac_sync_folder, state_file, asset, conf_file_extensions=CONFIG_FILE_EXTENSIONS, 
             init=False, init_force=False, init_state_file=None, delete_all_only=False, validate_configs_only=False,
-            **args):
+            delete_if_asset_not_updated=True, **args):
         """Function to sync spec configs defined in IAAC Sync folder 
 
         Args:
             iaac_sync_folder (str): The IAAC Sync folder path which contains the spec for asset to create
             state_file (str): The path of the state which will be used for syncing the assets
             asset (object): A class that represents the asset to sync. The asset is an class which defines the validate, check, 
                 create, delete methods
             conf_file_extensions (list, optional): List of extensions in iaac_sync_folder. Defaults to CONFIG_FILE_EXTENSIONS.
             init (bool, optional): Initialize the state file only. Defaults to False.
             init_state_file (str, optional): An optional initial state file to use when performing initialize. Defaults to None.
             init_force (bool, optional): Force initialization even if init file exists. Defaults to False.
             delete_all_only (bool, optional): Delete all the assets that have been created and clean the state file. Defaults to `False`.
             validate_configs_only (bool, optional): Whether to only validate the configs (not execute any syncing). Defaults to False.
+            delete_if_asset_not_updated (bool, optional): If True, then asset is not updated successful, then delete the asset to be 
+                re-created. Otherwise, create the asset again
             args (dict): Any additional optional args which would get passed to the methods defined in the asset class
         """
         self.iaac_sync_folder = iaac_sync_folder
         self.state_file = state_file
         self.asset = asset
         self.conf_file_extensions = conf_file_extensions
+        self.delete_if_asset_not_updated = delete_if_asset_not_updated
         self.state = {}
         if init:
             self.init_state(init_state_file, init_force)
         elif delete_all_only:
             self.__delete_assets(**args)
         elif validate_configs_only:
             self.__validate_configs(**args)
@@ -235,15 +238,25 @@
                                             if hasattr(self.asset, 'update') and callable(self.asset.update):
                                                 if self.asset.update(asset_id, config, **args):
                                                     # Call the update function, and ensure that the same asset ID is returned
                                                     # if asset ID not returned then there was an error
                                                     self.state[config_path]['hash'] = config_hash
                                                     self.state[config_path]['asset_id'] = asset_id
                                                 else:
-                                                    raise AssetNotUpdatedException(f"Asset with config in file {config_path} could not be updated")
+                                                    if self.delete_if_asset_not_updated:
+                                                        if self.asset.delete(asset_id, **args):
+                                                            # Asset ID deleted
+                                                            asset_id = ''
+                                                            if config_path in self.state:
+                                                                # Update the state file that asset has been deleted
+                                                                del self.state[config_path]
+                                                        else:
+                                                            raise AssetNotDeletedException(f"Asset with config in file {config_path} could not be deleted")
+                                                    else:
+                                                        raise AssetNotUpdatedException(f"Asset with config in file {config_path} could not be updated")
 
                                             else:
                                                 if self.asset.delete(asset_id, **args):
                                                     # Asset ID deleted
                                                     asset_id = ''
                                                     if config_path in self.state:
                                                         # Update the state file that asset has been deleted
```

### Comparing `pyiaacsync-0.6/pyiaacsync.egg-info/PKG-INFO` & `pyiaacsync-0.7/pyiaacsync.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiaacsync
-Version: 0.6
+Version: 0.7
 Summary: Deploy infrastructure as code via polling
 Home-page: https://github.com/manasmbellani/pyiaacsync
 License: UNKNOWN
 Description: # PyIAACSync
         
         ## Introduction
         infrastructure-as-code tools such as Terraform and Palumi are gaining popularity and increasingly becoming neceessary to support the principles of Site Reliability Engineering (SRE). 
@@ -58,14 +58,16 @@
         ```
         ...
             random_args = {}
             ## uncomment line below to demonstrate how the random arguments can work
             #random_args = {'message': 'hello world'}
         ```
         
+        *Note*: An additional example has been added in folder called `example-fileasset-with-update` where the `fileassetwupd.py` is a python file which additionally includes the `update` method in the `FileAssetWithUpdate` class. The commands listed below also apply to files in this folder.
+        
         ### Actions
         
         #### init
         The first steps is to execute `init` which will create a new state file `out-teststate.yaml`:
         ```
         python3 example.py -a init
         ```
```

### Comparing `pyiaacsync-0.6/setup.py` & `pyiaacsync-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Read the description from the markdown file
 with open('README.md', 'r') as f:
     description = f.read()
 
 setup(
     name="pyiaacsync",
-    version="0.6",
+    version="0.7",
     packages=find_packages(),
     install_requires=requirements,
     description=project_description,
     long_description=description,
     long_description_content_type="text/markdown",
     url=get_git_remote_url()
 )
```

