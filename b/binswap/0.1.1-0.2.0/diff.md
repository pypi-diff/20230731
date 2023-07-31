# Comparing `tmp/binswap-0.1.1.tar.gz` & `tmp/binswap-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binswap-0.1.1.tar", last modified: Thu Jul 20 12:44:15 2023, max compression
+gzip compressed data, was "binswap-0.2.0.tar", last modified: Mon Jul 31 06:15:28 2023, max compression
```

## Comparing `binswap-0.1.1.tar` & `binswap-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 12:44:15.902073 binswap-0.1.1/
--rw-rw-rw-   0        0        0     1066 2023-07-20 10:10:11.000000 binswap-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      526 2023-07-20 12:44:15.902073 binswap-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-07-20 10:05:21.000000 binswap-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 12:44:15.870828 binswap-0.1.1/binswap/
--rw-rw-rw-   0        0        0        0 2023-07-20 09:46:34.000000 binswap-0.1.1/binswap/__init__.py
--rw-rw-rw-   0        0        0     4870 2023-07-20 10:05:30.000000 binswap-0.1.1/binswap/main.py
-drwxrwxrwx   0        0        0        0 2023-07-20 12:44:15.886450 binswap-0.1.1/binswap.egg-info/
--rw-rw-rw-   0        0        0      526 2023-07-20 12:44:15.000000 binswap-0.1.1/binswap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-07-20 12:44:15.000000 binswap-0.1.1/binswap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 12:44:15.000000 binswap-0.1.1/binswap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-20 12:44:15.000000 binswap-0.1.1/binswap.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-20 12:44:15.000000 binswap-0.1.1/binswap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-20 12:44:15.000000 binswap-0.1.1/binswap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 12:44:15.902073 binswap-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-07-20 12:44:01.000000 binswap-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:15:28.434574 binswap-0.2.0/
+-rw-rw-rw-   0        0        0      504 2023-07-31 06:15:28.434574 binswap-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-07-20 13:06:11.000000 binswap-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 06:15:28.387698 binswap-0.2.0/binswap/
+-rw-rw-rw-   0        0        0        0 2023-07-20 09:46:34.000000 binswap-0.2.0/binswap/__init__.py
+-rw-rw-rw-   0        0        0     5728 2023-07-31 05:51:37.000000 binswap-0.2.0/binswap/main.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:15:28.434574 binswap-0.2.0/binswap.egg-info/
+-rw-rw-rw-   0        0        0      504 2023-07-31 06:15:28.000000 binswap-0.2.0/binswap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-07-31 06:15:28.000000 binswap-0.2.0/binswap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 06:15:28.000000 binswap-0.2.0/binswap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-31 06:15:28.000000 binswap-0.2.0/binswap.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 06:15:28.000000 binswap-0.2.0/binswap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 06:15:28.000000 binswap-0.2.0/binswap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 06:15:28.434574 binswap-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-07-31 05:59:01.000000 binswap-0.2.0/setup.py
```

### Comparing `binswap-0.1.1/binswap/main.py` & `binswap-0.2.0/binswap/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,37 +57,66 @@
                     )
                     self.process.kill()
             os._exit(0)
 
     @staticmethod
     def _terminate_process(process: subprocess.Popen) -> None:
         if platform.system() == "Windows":
-            subprocess.run(["taskkill", "/F", "/PID", str(process.pid)])
+            subprocess.run(["taskkill", "/F", "/T", "/PID", str(process.pid)])
         else:
             process.terminate()
-            process.wait()
 
     @staticmethod
     def _create_subprocess(binary_path: str) -> subprocess.Popen:
         if platform.system() == "Windows":
-            return subprocess.Popen(
-                ["python", binary_path], creationflags=subprocess.CREATE_NEW_CONSOLE
-            )
+            interpreter = _get_script_interpreter(binary_path)
+
+            if interpreter:
+                return subprocess.Popen(
+                    [interpreter, binary_path],
+                    creationflags=subprocess.CREATE_NEW_CONSOLE,
+                )
+            elif os.path.isfile(binary_path) and binary_path.lower().endswith(".exe"):
+                return subprocess.Popen(
+                    [binary_path], creationflags=subprocess.CREATE_NEW_CONSOLE
+                )
+            else:
+                logger.error(f"Unsupported file type for Windows: {binary_path}")
         else:
-            return subprocess.Popen(["python", binary_path])
+            return subprocess.Popen([binary_path])
+
+
+def count_dir_files(directory: Path) -> int:
+    return sum(1 for _ in directory.iterdir() if _.is_file())
+
+
+def _get_script_interpreter(script_path: str) -> str:
+    interpreter_mapping = {
+        "py": "python",
+        "js": "node",
+        "rb": "ruby",
+        "php": "php",
+        "sh": "bash",
+        "pl": "perl",
+        "lua": "lua",
+    }
+
+    script_extension = script_path.lower().split(".")[-1]
+    return interpreter_mapping.get(script_extension, "")
 
 
 def init_file_monitoring(binary_path: str, monitored_directory: str) -> None:
     """
-    Monitor directory for changes and auto relaunch bin.
+    Monitor dir for changes and auto relaunch executable (.exe) or script files.
 
     Args:
-        binary_path (str): Path to the actual binary.
+        binary_path (str): Path to the executable or script file.
         monitored_directory (str): Directory to be monitored.
 
+    Example:
         init_file_monitoring("/path/to/binary", "/path/to/directory")
     """
     event_handler = FileChangeHandler(binary_path)
     observer = Observer()
 
     try:
         observer.schedule(event_handler, str(monitored_directory), recursive=False)
@@ -106,18 +135,14 @@
     except Exception as e:
         logger.error(f"An error occurred: {e}")
     finally:
         observer.stop()
         observer.join()
 
 
-def count_dir_files(directory: Path) -> int:
-    return sum(1 for _ in directory.iterdir() if _.is_file())
-
-
 def main():
     parser = argparse.ArgumentParser(
         description="Monitor directory and automatically relaunch binary."
     )
     parser.add_argument(
         "--bin", type=Path, required=True, help="Path to the actual binary."
     )
```

