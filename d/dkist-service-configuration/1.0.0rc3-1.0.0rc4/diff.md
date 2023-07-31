# Comparing `tmp/dkist-service-configuration-1.0.0rc3.tar.gz` & `tmp/dkist-service-configuration-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-service-configuration-1.0.0rc3.tar", last modified: Wed Jul 26 22:19:55 2023, max compression
+gzip compressed data, was "dkist-service-configuration-1.0.0rc4.tar", last modified: Thu Jul 27 19:47:27 2023, max compression
```

## Comparing `dkist-service-configuration-1.0.0rc3.tar` & `dkist-service-configuration-1.0.0rc4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 22:19:55.312128 dkist-service-configuration-1.0.0rc3/
--rw-rw-rw-   0 root         (0) root         (0)     1757 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-26 22:19:55.312128 dkist-service-configuration-1.0.0rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1394 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 22:19:55.308128 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1688 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 22:19:55.312128 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/tests/test_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1333 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/tests/test_settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 22:19:55.312128 dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-26 22:19:55.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-07-26 22:19:55.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 22:19:55.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-26 22:19:55.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-26 22:19:55.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-07-26 22:19:55.312128 dkist-service-configuration-1.0.0rc3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-27 19:47:27.546760 dkist-service-configuration-1.0.0rc4/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-27 19:47:27.546760 dkist-service-configuration-1.0.0rc4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1394 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-27 19:47:27.546760 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-27 19:47:27.546760 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/tests/test_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration/tests/test_settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-27 19:47:27.546760 dkist-service-configuration-1.0.0rc4/dkist_service_configuration.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-27 19:47:27.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-07-27 19:47:27.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-27 19:47:27.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-27 19:47:27.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-27 19:47:27.000000 dkist-service-configuration-1.0.0rc4/dkist_service_configuration.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-07-27 19:47:27.546760 dkist-service-configuration-1.0.0rc4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-27 19:47:12.000000 dkist-service-configuration-1.0.0rc4/setup.py
```

### Comparing `dkist-service-configuration-1.0.0rc3/.gitignore` & `dkist-service-configuration-1.0.0rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc3/.pre-commit-config.yaml` & `dkist-service-configuration-1.0.0rc4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc3/LICENSE` & `dkist-service-configuration-1.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc3/PKG-INFO` & `dkist-service-configuration-1.0.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-service-configuration
-Version: 1.0.0rc3
+Version: 1.0.0rc4
 Summary: Configuration support for DKIST services
 Home-page: https://bitbucket.org/dkistdc/dkist_service_configuration/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-service-configuration-1.0.0rc3/README.rst` & `dkist-service-configuration-1.0.0rc4/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc3/bitbucket-pipelines.yml` & `dkist-service-configuration-1.0.0rc4/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc3/dkist_service_configuration/logging.py` & `dkist-service-configuration-1.0.0rc4/dkist_service_configuration/logging.py`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc3/dkist_service_configuration/settings.py` & `dkist-service-configuration-1.0.0rc4/dkist_service_configuration/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,16 @@
                 return True
         return False
 
     def log_configurations(self):
         for field_name in self.__fields__:  # __fields__ -> model_fields in pydantic 2.x
             if self._is_secret(field_name=field_name):
                 logger.info(f"{field_name}: <CENSORED>")
-            logger.info(f"{field_name}: {getattr(self, field_name)}")
+            else:
+                logger.info(f"{field_name}: {getattr(self, field_name)}")
 
 
 class MeshService(BaseModel):
     """Model of the metadata for a node in the service mesh"""
 
     host: str = Field(..., alias="mesh_address")
     port: int = Field(..., alias="mesh_port")
```

### Comparing `dkist-service-configuration-1.0.0rc3/dkist_service_configuration/tests/test_settings.py` & `dkist-service-configuration-1.0.0rc4/dkist_service_configuration/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/PKG-INFO` & `dkist-service-configuration-1.0.0rc4/dkist_service_configuration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-service-configuration
-Version: 1.0.0rc3
+Version: 1.0.0rc4
 Summary: Configuration support for DKIST services
 Home-page: https://bitbucket.org/dkistdc/dkist_service_configuration/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/SOURCES.txt` & `dkist-service-configuration-1.0.0rc4/dkist_service_configuration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc3/setup.cfg` & `dkist-service-configuration-1.0.0rc4/setup.cfg`

 * *Files identical despite different names*

