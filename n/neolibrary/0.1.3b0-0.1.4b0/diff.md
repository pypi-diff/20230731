# Comparing `tmp/neolibrary-0.1.3b0.tar.gz` & `tmp/neolibrary-0.1.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neolibrary-0.1.3b0.tar", max compression
+gzip compressed data, was "neolibrary-0.1.4b0.tar", max compression
```

## Comparing `neolibrary-0.1.3b0.tar` & `neolibrary-0.1.4b0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/LICENSE
--rw-r--r--   0        0        0      448 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/README.md
--rw-r--r--   0        0        0      445 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/src/neolibrary/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/src/neolibrary/monitoring/__init__.py
--rw-r--r--   0        0        0      770 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/src/neolibrary/monitoring/config/config.py
--rw-r--r--   0        0        0     3711 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/src/neolibrary/monitoring/logger.py
--rw-r--r--   0        0        0      714 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/src/neolibrary/utils.py
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 neolibrary-0.1.3b0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/LICENSE
+-rw-r--r--   0        0        0      448 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/README.md
+-rw-r--r--   0        0        0      445 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/src/neolibrary/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/src/neolibrary/monitoring/__init__.py
+-rw-r--r--   0        0        0      770 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/src/neolibrary/monitoring/config/config.py
+-rw-r--r--   0        0        0     3518 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/src/neolibrary/monitoring/logger.py
+-rw-r--r--   0        0        0      714 2023-07-31 11:54:51.266891 neolibrary-0.1.4b0/src/neolibrary/utils.py
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 neolibrary-0.1.4b0/PKG-INFO
```

### Comparing `neolibrary-0.1.3b0/LICENSE` & `neolibrary-0.1.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `neolibrary-0.1.3b0/src/neolibrary/monitoring/config/config.py` & `neolibrary-0.1.4b0/src/neolibrary/monitoring/config/config.py`

 * *Files identical despite different names*

### Comparing `neolibrary-0.1.3b0/src/neolibrary/monitoring/logger.py` & `neolibrary-0.1.4b0/src/neolibrary/monitoring/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,28 +34,33 @@
         super().__init__(name, level)
         self.init_logger()
         self.name = name
         self.PATH = config.ROOT + "/logs/" + name + ".log"
         logging.addLevelName(config.SUCCESS, "SUCCESS")
         logging.addLevelName(config.FAIL, "FAIL")
         logging.addLevelName(config.PIPE, "PIPE")
+        logging.root.setLevel(level)
         self.formatter = ColoredFormatter(
             config.LOGFORMAT,
             log_colors=config.LOG_COLORS,
         )
         self.e_formatter = ColoredFormatter(
             config.LOGFORMAT_ERROR,
             log_colors=config.LOG_COLORS,
         )
         self.stream = logging.StreamHandler()
         self.file_handler = logging.FileHandler(self.PATH)
         self.file_handler.setLevel(level_e)
         self.stream.setFormatter(self.formatter)
         self.file_handler.setFormatter(self.e_formatter)
-        logging.root.setLevel(level)
+        self.setLevel(config.LOG_LEVEL)
+        if self.hasHandlers():
+            self.handlers.clear()
+        self.addHandler(self.stream)
+        self.addHandler(self.file_handler)
 
     def success(self, message: str, *args: Any, **kws: Any) -> NoReturn:
         """
         Log 'message % args' with severity 'SUCCESS'.
 
         Args:
             message (str): Message to log.
@@ -94,28 +99,14 @@
 
         Returns:
             None: NoReturn
         """
         if self.isEnabledFor(config.PIPE):
             self._log(config.PIPE, message, args, **kws)
 
-    def get_logger(self) -> Any:
-        """
-        Get the logger
-
-        Returns:
-            logging.Logger: A logger.
-        """
-        log = logging.getLogger(self.name)
-        log.setLevel(config.LOG_LEVEL)
-        if log.hasHandlers():
-            log.handlers.clear()
-        log.addHandler(self.stream)
-        log.addHandler(self.file_handler)
-        return log
 
     def init_logger(self):
         """ 
         Initialize the logger by setting up the folder structure if it doesn't exist.
         """
         if not os.path.exists(config.ROOT + "/logs"):
             os.makedirs(config.ROOT + "/logs")
```

### Comparing `neolibrary-0.1.3b0/src/neolibrary/utils.py` & `neolibrary-0.1.4b0/src/neolibrary/utils.py`

 * *Files identical despite different names*

### Comparing `neolibrary-0.1.3b0/PKG-INFO` & `neolibrary-0.1.4b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neolibrary
-Version: 0.1.3b0
+Version: 0.1.4b0
 Summary: The general utils library for neomedsys development
 License: Apache-2.0 license
 Author: Martin Soria Røvang
 Author-email: martinrovang@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

