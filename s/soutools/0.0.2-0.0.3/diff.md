# Comparing `tmp/soutools-0.0.2.tar.gz` & `tmp/soutools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soutools-0.0.2.tar", last modified: Tue Jul 25 03:15:15 2023, max compression
+gzip compressed data, was "soutools-0.0.3.tar", last modified: Mon Jul 31 20:46:38 2023, max compression
```

## Comparing `soutools-0.0.2.tar` & `soutools-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 03:15:15.142420 soutools-0.0.2/
--rw-rw-rw-   0        0        0     3670 2023-07-12 21:52:49.000000 soutools-0.0.2/.gitignore
--rw-rw-rw-   0        0        0     1089 2023-07-12 21:56:03.000000 soutools-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       78 2023-07-25 03:15:15.141424 soutools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4734 2023-07-18 03:33:41.000000 soutools-0.0.2/README.md
--rw-rw-rw-   0        0        0      308 2023-07-25 03:13:59.000000 soutools-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      246 2023-07-25 02:52:40.000000 soutools-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 03:15:15.142420 soutools-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-25 03:15:15.008787 soutools-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 03:15:15.095558 soutools-0.0.2/src/soutools/
--rw-rw-rw-   0        0        0        0 2023-07-12 22:01:06.000000 soutools-0.0.2/src/soutools/__init__.py
--rw-rw-rw-   0        0        0     2915 2023-07-25 01:47:05.000000 soutools-0.0.2/src/soutools/controller.py
--rw-rw-rw-   0        0        0     5268 2023-07-25 00:37:59.000000 soutools-0.0.2/src/soutools/helpers.py
--rw-rw-rw-   0        0        0     2345 2023-07-24 14:56:11.000000 soutools-0.0.2/src/soutools/main.py
--rw-rw-rw-   0        0        0     1506 2023-07-24 14:56:11.000000 soutools-0.0.2/src/soutools/menu.py
--rw-rw-rw-   0        0        0     7654 2023-07-25 02:53:54.000000 soutools-0.0.2/src/soutools/model.py
--rw-rw-rw-   0        0        0     3839 2023-07-25 00:38:00.000000 soutools-0.0.2/src/soutools/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-25 03:15:15.129455 soutools-0.0.2/src/soutools.egg-info/
--rw-rw-rw-   0        0        0       78 2023-07-25 03:15:14.000000 soutools-0.0.2/src/soutools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-07-25 03:15:14.000000 soutools-0.0.2/src/soutools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 03:15:14.000000 soutools-0.0.2/src/soutools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-25 03:15:14.000000 soutools-0.0.2/src/soutools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      232 2023-07-25 03:15:14.000000 soutools-0.0.2/src/soutools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-25 03:15:14.000000 soutools-0.0.2/src/soutools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 03:15:15.136437 soutools-0.0.2/tests/
--rw-rw-rw-   0        0        0        0 2023-07-12 22:10:13.000000 soutools-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0     1776 2023-07-14 17:45:04.000000 soutools-0.0.2/tests/test_settings.py
+drwxrwxrwx   0        0        0        0 2023-07-31 20:46:38.117119 soutools-0.0.3/
+-rw-rw-rw-   0        0        0     3670 2023-07-12 21:52:49.000000 soutools-0.0.3/.gitignore
+-rw-rw-rw-   0        0        0     1089 2023-07-12 21:56:03.000000 soutools-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       78 2023-07-31 20:46:38.116137 soutools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4734 2023-07-18 03:33:41.000000 soutools-0.0.3/README.md
+-rw-rw-rw-   0        0        0      308 2023-07-31 20:42:11.000000 soutools-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      246 2023-07-25 02:52:40.000000 soutools-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 20:46:38.117119 soutools-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 20:46:38.016190 soutools-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 20:46:38.074175 soutools-0.0.3/src/soutools/
+-rw-rw-rw-   0        0        0        0 2023-07-12 22:01:06.000000 soutools-0.0.3/src/soutools/__init__.py
+-rw-rw-rw-   0        0        0     3412 2023-07-31 20:41:44.000000 soutools-0.0.3/src/soutools/controller.py
+-rw-rw-rw-   0        0        0     5268 2023-07-25 00:37:59.000000 soutools-0.0.3/src/soutools/helpers.py
+-rw-rw-rw-   0        0        0     2345 2023-07-24 14:56:11.000000 soutools-0.0.3/src/soutools/main.py
+-rw-rw-rw-   0        0        0     1506 2023-07-24 14:56:11.000000 soutools-0.0.3/src/soutools/menu.py
+-rw-rw-rw-   0        0        0     7697 2023-07-31 20:41:45.000000 soutools-0.0.3/src/soutools/model.py
+-rw-rw-rw-   0        0        0     3839 2023-07-25 00:38:00.000000 soutools-0.0.3/src/soutools/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-31 20:46:38.103432 soutools-0.0.3/src/soutools.egg-info/
+-rw-rw-rw-   0        0        0       78 2023-07-31 20:46:37.000000 soutools-0.0.3/src/soutools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-07-31 20:46:38.000000 soutools-0.0.3/src/soutools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 20:46:37.000000 soutools-0.0.3/src/soutools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-31 20:46:37.000000 soutools-0.0.3/src/soutools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      232 2023-07-31 20:46:37.000000 soutools-0.0.3/src/soutools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 20:46:37.000000 soutools-0.0.3/src/soutools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 20:46:38.110264 soutools-0.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-12 22:10:13.000000 soutools-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     1776 2023-07-14 17:45:04.000000 soutools-0.0.3/tests/test_settings.py
```

### Comparing `soutools-0.0.2/.gitignore` & `soutools-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `soutools-0.0.2/LICENSE` & `soutools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `soutools-0.0.2/README.md` & `soutools-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `soutools-0.0.2/src/soutools/controller.py` & `soutools-0.0.3/src/soutools/controller.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 def view_organization():
     logger.debug('The "view_organization" function called')
     logger.debug('Checking if organization name is set')
     if not org_name:
         print('\nYou have not selected an organization yet\n')
         logger.debug('Notified user that organization name is not set')
     else:
-        blue_highlight = helpers.colorme(org_name, 'blue')
-        print(f'\nThe "{blue_highlight}" organization is currently selected\n')
+        highlight_orgname = helpers.colorme(org_name, 'blue')
+        highlight_orgid = helpers.colorme(org_id, 'blue')
+        print(f'\nThe "{highlight_orgname}" organization with ID {highlight_orgid} is currently selected\n')
         logger.debug(f'Notified user that organization name is set to {org_name}')
     input('Press [ENTER] to continue...')
 
 
 def wireless_options():
     menu_title = helpers.menu_title
     wireless_menu = menu.Menu(
@@ -61,17 +62,27 @@
 def wireless_report_with_ssid_number():
     logger.debug('The "wireless_with_ssid_x_report" function called')
     dashboard.find_ssid_number()
     input('Press [ENTER] to continue...')
 
 
 def update_radius_settings():
+    make_changes = 'n'
     logger.debug('The "update_radius_settings" function called')
-    dashboard.update_radius_servers()
-    input('Press [ENTER] to continue...')
+    warning = helpers.colorme('WARNING', 'red')
+    highlight_orgname = helpers.colorme(org_name, 'blue')
+    print(f'{warning} - You are about to make changes to the {highlight_orgname} organizaiton')
+    make_changes = input('Are you sure you want to continue [Y/N] ').upper()
+    if 'Y' in make_changes:
+        print()
+        dashboard.update_radius_servers()
+        input('Press [ENTER] to continue...')
+    else:
+        wireless_options()
+    
 
 
 def quit():
     helpers.clear_screen()
     sys.exit()
```

### Comparing `soutools-0.0.2/src/soutools/helpers.py` & `soutools-0.0.3/src/soutools/helpers.py`

 * *Files identical despite different names*

### Comparing `soutools-0.0.2/src/soutools/main.py` & `soutools-0.0.3/src/soutools/main.py`

 * *Files identical despite different names*

### Comparing `soutools-0.0.2/src/soutools/menu.py` & `soutools-0.0.3/src/soutools/menu.py`

 * *Files identical despite different names*

### Comparing `soutools-0.0.2/src/soutools/model.py` & `soutools-0.0.3/src/soutools/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,16 @@
         logger.debug('The "select_organization" function called from the model')
         organizations = None
         try:
             logger.debug('Trying to get organizations from the Meraki dashboard')
             organizations = self.dashboard.organizations.getOrganizations()
             logger.debug(f'organizations is equal to {organizations}')
         except meraki.exceptions.APIError:
-        
             sys.exit('Check network settings and verify API Key')
+        organizations.sort(key=lambda x: x["name"])
         counter = 1
         print('  Organizations to choose from:\n')
         for organization in organizations:
             name = helpers.colorme(f"{str(counter)} - {organization['name']}", 'green')
             print(f'    {name}')
             counter += 1
         selected = helpers.validate_integer_in_range(counter)
```

### Comparing `soutools-0.0.2/src/soutools/settings.py` & `soutools-0.0.3/src/soutools/settings.py`

 * *Files identical despite different names*

### Comparing `soutools-0.0.2/tests/test_settings.py` & `soutools-0.0.3/tests/test_settings.py`

 * *Files identical despite different names*

