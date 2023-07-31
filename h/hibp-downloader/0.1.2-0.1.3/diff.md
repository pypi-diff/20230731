# Comparing `tmp/hibp_downloader-0.1.2.tar.gz` & `tmp/hibp_downloader-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hibp_downloader-0.1.2.tar", max compression
+gzip compressed data, was "hibp_downloader-0.1.3.tar", max compression
```

## Comparing `hibp_downloader-0.1.2.tar` & `hibp_downloader-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1565 2023-07-26 04:14:23.983439 hibp_downloader-0.1.2/LICENSE
--rw-r--r--   0        0        0     2597 2023-07-30 15:00:09.957823 hibp_downloader-0.1.2/README.md
--rw-r--r--   0        0        0     2937 2023-07-30 15:00:09.963823 hibp_downloader-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1548 2023-07-30 15:00:09.975823 hibp_downloader-0.1.2/src/hibp_downloader/__init__.py
--rw-r--r--   0        0        0    10806 2023-07-30 11:09:59.800056 hibp_downloader-0.1.2/src/hibp_downloader/commands/hibp_download.py
--rw-r--r--   0        0        0     3813 2023-07-30 11:12:13.966653 hibp_downloader-0.1.2/src/hibp_downloader/commands/hibp_generate.py
--rw-r--r--   0        0        0      568 2023-07-26 04:18:19.902342 hibp_downloader-0.1.2/src/hibp_downloader/exceptions.py
--rw-r--r--   0        0        0     4268 2023-07-30 12:12:56.451940 hibp_downloader-0.1.2/src/hibp_downloader/lib/app.py
--rw-r--r--   0        0        0     3741 2023-07-30 13:34:36.549050 hibp_downloader-0.1.2/src/hibp_downloader/lib/filedata.py
--rw-r--r--   0        0        0      657 2023-07-29 09:39:32.590020 hibp_downloader-0.1.2/src/hibp_downloader/lib/generators.py
--rw-r--r--   0        0        0     1858 2023-07-30 07:01:44.988273 hibp_downloader-0.1.2/src/hibp_downloader/lib/http.py
--rw-r--r--   0        0        0     3281 2023-07-30 13:34:36.552050 hibp_downloader-0.1.2/src/hibp_downloader/lib/logger.py
--rw-r--r--   0        0        0     1285 2023-07-30 06:49:39.677165 hibp_downloader-0.1.2/src/hibp_downloader/main.py
--rw-r--r--   0        0        0      214 2023-07-30 03:31:02.403390 hibp_downloader-0.1.2/src/hibp_downloader/models/__init__.py
--rw-r--r--   0        0        0      395 2023-07-30 13:34:36.556051 hibp_downloader-0.1.2/src/hibp_downloader/models/app_context.py
--rw-r--r--   0        0        0       87 2023-07-29 11:47:32.763631 hibp_downloader-0.1.2/src/hibp_downloader/models/hash_type.py
--rw-r--r--   0        0        0     1829 2023-07-30 13:34:36.559051 hibp_downloader-0.1.2/src/hibp_downloader/models/prefix_metadata.py
--rw-r--r--   0        0        0     5456 2023-07-30 13:34:36.562051 hibp_downloader-0.1.2/src/hibp_downloader/models/stats.py
--rw-r--r--   0        0        0        0 2023-07-26 00:51:50.083564 hibp_downloader-0.1.2/src/hibp_downloader/py.typed
--rw-r--r--   0        0        0     3843 1970-01-01 00:00:00.000000 hibp_downloader-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1565 2023-07-26 04:14:23.983439 hibp_downloader-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2572 2023-07-31 00:24:18.561251 hibp_downloader-0.1.3/README.md
+-rw-r--r--   0        0        0     2937 2023-07-31 02:11:13.366700 hibp_downloader-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1570 2023-07-31 02:11:13.371700 hibp_downloader-0.1.3/src/hibp_downloader/__init__.py
+-rw-r--r--   0        0        0    10970 2023-07-31 02:07:51.377302 hibp_downloader-0.1.3/src/hibp_downloader/commands/hibp_download.py
+-rw-r--r--   0        0        0     3813 2023-07-30 11:12:13.966653 hibp_downloader-0.1.3/src/hibp_downloader/commands/hibp_generate.py
+-rw-r--r--   0        0        0      568 2023-07-26 04:18:19.902342 hibp_downloader-0.1.3/src/hibp_downloader/exceptions.py
+-rw-r--r--   0        0        0     4267 2023-07-31 01:58:30.039646 hibp_downloader-0.1.3/src/hibp_downloader/lib/app.py
+-rw-r--r--   0        0        0     3818 2023-07-31 02:08:03.814450 hibp_downloader-0.1.3/src/hibp_downloader/lib/filedata.py
+-rw-r--r--   0        0        0      657 2023-07-29 09:39:32.590020 hibp_downloader-0.1.3/src/hibp_downloader/lib/generators.py
+-rw-r--r--   0        0        0     1858 2023-07-30 07:01:44.988273 hibp_downloader-0.1.3/src/hibp_downloader/lib/http.py
+-rw-r--r--   0        0        0     3281 2023-07-30 13:34:36.552050 hibp_downloader-0.1.3/src/hibp_downloader/lib/logger.py
+-rw-r--r--   0        0        0     1285 2023-07-30 06:49:39.677165 hibp_downloader-0.1.3/src/hibp_downloader/main.py
+-rw-r--r--   0        0        0      214 2023-07-30 03:31:02.403390 hibp_downloader-0.1.3/src/hibp_downloader/models/__init__.py
+-rw-r--r--   0        0        0      395 2023-07-30 13:34:36.556051 hibp_downloader-0.1.3/src/hibp_downloader/models/app_context.py
+-rw-r--r--   0        0        0       87 2023-07-29 11:47:32.763631 hibp_downloader-0.1.3/src/hibp_downloader/models/hash_type.py
+-rw-r--r--   0        0        0     1829 2023-07-30 13:34:36.559051 hibp_downloader-0.1.3/src/hibp_downloader/models/prefix_metadata.py
+-rw-r--r--   0        0        0     5456 2023-07-30 13:34:36.562051 hibp_downloader-0.1.3/src/hibp_downloader/models/stats.py
+-rw-r--r--   0        0        0        0 2023-07-26 00:51:50.083564 hibp_downloader-0.1.3/src/hibp_downloader/py.typed
+-rw-r--r--   0        0        0     3818 1970-01-01 00:00:00.000000 hibp_downloader-0.1.3/PKG-INFO
```

### Comparing `hibp_downloader-0.1.2/LICENSE` & `hibp_downloader-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.2/README.md` & `hibp_downloader-0.1.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 # hibp-downloader
 
 [![PyPi](https://img.shields.io/pypi/v/hibp-downloader.svg)](https://pypi.python.org/pypi/hibp-downloader/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/hibp-downloader.svg)](https://github.com/threatpatrols/hibp-downloader/)
 [![build tests](https://github.com/threatpatrols/hibp-downloader/actions/workflows/build-tests.yml/badge.svg)](https://github.com/threatpatrols/hibp-downloader/actions/workflows/build-tests.yml)
 [![License](https://img.shields.io/github/license/threatpatrols/hibp-downloader.svg)](https://github.com/threatpatrols/hibp-downloader)
 
-This is a Python implementation of the original [PwnedPasswordsDownloader](https://github.com/HaveIBeenPwned/PwnedPasswordsDownloader)
-that provides some additional useful functionality 
- - Automatically only download prefix-chunks that have changed since the last download
+This is a Python implementation of [PwnedPasswordsDownloader](https://github.com/HaveIBeenPwned/PwnedPasswordsDownloader)
+that is more download efficient and provides additional useful functionality
+ - Automatically **only** download prefix-chunks that have changed since the last download
  - Ability to start, stop and re-start without loss of data already collected
- - Ability to name the `--first-hash` and `--last-hash` positions
- - Metadata file per prefix file in JSON format for easy data reuse
+ - Ability to start and stop at named hash positions
+ - Per prefix file metadata in JSON format for easy data reuse
 
 ## Install
 ```commandline
 pip install --upgrade hibp-downloader
 ```
 
 ## Usage
 ![screenshot-help.png](https://raw.githubusercontent.com/threatpatrols/hibp-downloader/main/docs/assets/screenshot-help.png)
 
 ## Runtime Logs
-Sample download activity logs 
+Sample download activity log
 ```text
-2023-07-30T21:42:06+1000 | INFO | hibp-downloader | prefix=65747 source=[lc:207328 et:0 rc:56672 ro:0 xx:0] runtime_rate=[10.3MBit/s 79req/s ~65602H/s] runtime=0.2hr download=922.5MB
-2023-07-30T21:42:07+1000 | INFO | hibp-downloader | prefix=29da7 source=[lc:207328 et:0 rc:56792 ro:0 xx:0] runtime_rate=[10.4MBit/s 79req/s ~65646H/s] runtime=0.2hr download=924.5MB
-2023-07-30T21:42:09+1000 | INFO | hibp-downloader | prefix=43c7f source=[lc:207328 et:0 rc:56912 ro:0 xx:0] runtime_rate=[10.3MBit/s 79req/s ~65617H/s] runtime=0.2hr download=926.5MB
+2023-07-31T03:22:45+1000 | INFO | hibp-downloader | prefix=e585f source=[lc:265201 et:0 rc:722148 ro:3 xx:0] runtime_rate=[11.2MBit/s 86req/s ~71005H/s] runtime=2.33hr download=11748.0MB
+2023-07-31T03:22:48+1000 | INFO | hibp-downloader | prefix=e5877 source=[lc:265201 et:0 rc:722268 ro:3 xx:0] runtime_rate=[11.2MBit/s 86req/s ~70998H/s] runtime=2.33hr download=11750.0MB
+2023-07-31T03:22:50+1000 | INFO | hibp-downloader | prefix=f5837 source=[lc:265201 et:0 rc:722388 ro:3 xx:0] runtime_rate=[11.2MBit/s 86req/s ~70992H/s] runtime=2.33hr download=11751.9MB
 ```
- - 79 requests per second to api.pwnedpasswords.com
- - 207,328 prefix files from (`lc`) local-cache
- - 56,912 prefix files from (`rc`) remote-cache
- - 0 files from (`ro`) remote-origin, 0 files failed (`xx`) download
- - estimated 65,617 hash values downloaded per second
- - 926MB downloaded in ~12 minutes (0.20 hour)
+ - 86 requests per second to api.pwnedpasswords.com
+ - 265,201 prefix files from (`lc`) local-cache; 722,388 from (`rc`) remote-cache; 3 from (`ro`) remote-origin; 0 failed (`xx`) download
+ - estimated ~70k hash values downloaded per second
+ - 11.5GB (11,751MB) downloaded in 2.3 hours
 
+## Source
+ - https://github.com/threatpatrols/hibp-downloader
 
 ## Issues
  - https://github.com/threatpatrols/hibp-downloader/issues
 
-## Source
- - https://github.com/threatpatrols/hibp-downloader
-
 ## Copyright
  - Copyright &copy; 2023 Threat Patrols Pty Ltd &lt;contact@threatpatrols.com&gt;
  - Copyright &copy; 2023 Nicholas de Jong &lt;contact@nicholasdejong.com&gt;
 
 All rights reserved.
 
 ## License
```

### Comparing `hibp_downloader-0.1.2/pyproject.toml` & `hibp_downloader-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hibp-downloader"
-version = "0.1.2"
+version = "0.1.3"
 description = "Efficiently download HIBP new pwned password data by hash-prefix for a local-copy"
 authors = ["Nicholas de Jong <contact@threatpatrols.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [{ include = "hibp_downloader", from = "src" }]
 classifiers = [
     "Environment :: Console",
@@ -31,21 +31,21 @@
 "httpx[http2]" = "^0.24.1"      # https://pypi.org/project/httpx/#history
 "typer[all]" = "0.9.0"          # https://pypi.org/project/typer/#history
 shellingham = "1.5.0.post1"     # https://pypi.org/project/shellingham/#history
 aiofiles = "23.1.0"             # https://pypi.org/project/aiofiles/#history
 
 [tool.poetry.dev-dependencies]
 black = "^23.7.0"               # https://pypi.org/project/black/#history
-flake8 = "^6.0.0"               # https://pypi.org/project/flake8/#history
+flake8 = "^6.1.0"               # https://pypi.org/project/flake8/#history
 isort = "^5.12.0"               # https://pypi.org/project/isort/#history
 mypy = "^1.4.1"                 # https://pypi.org/project/mypy/#history
 pycln = "^2.1.7"                # https://pypi.org/project/pycln/#history
 pytest = "^7.4.0"               # https://pypi.org/project/pytest/#history
 safety = "^2.4.0b1"             # https://pypi.org/project/safety/#history
-pyinstrument = "^4.4.0"         # https://pypi.org/project/pyinstrument/#history
+pyinstrument = "^4.5.1"         # https://pypi.org/project/pyinstrument/#history
 types-aiofiles = "23.1.0.5"     # https://pypi.org/project/types-aiofiles/#history
 
 [tool.slap]
 typed = true
 release.branch = "dev"
 
 [tool.slap.test]
```

### Comparing `hibp_downloader-0.1.2/src/hibp_downloader/__init__.py` & `hibp_downloader-0.1.3/src/hibp_downloader/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from os import cpu_count, getenv
 from sys import argv
 
 from .lib.logger import logger_get
 from .models import AppContext
 
 __title__ = "HIBP Downloader"
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __logger_name__ = "hibp-downloader"
 __pwnedpasswords_api_url__ = "https://api.pwnedpasswords.com"
 __local_cache_ttl_default__ = 86400
 __multiprocessing_processes_default__ = cpu_count()
 __multiprocessing_prefixes_chunk_size__ = cpu_count() * 2
 __approx_gzip_bytes_per_hash__ = 20.674
 __logging_info_event_modulus__ = 5
@@ -24,13 +24,15 @@
 if "--debug" in argv or getenv("HIBPDL_DEBUG", "").lower().startswith(("true", "yes", "enable")):
     __logger_level__ = "debug"
 
 __app_profiler__ = False
 if "--profiler" in argv or getenv("HIBPDL_PROFILER", "").lower().startswith(("true", "yes", "enable")):
     __app_profiler__ = True
 
-__help_epilog_footer__ = """
-        Project: [https://github.com/threatpatrols/hibp-downloader](https://github.com/threatpatrols/hibp-downloader)
+__help_epilog_footer__ = f"""
+{__title__}: v{__version__}
+
+Project: [https://github.com/threatpatrols/hibp-downloader](https://github.com/threatpatrols/hibp-downloader)
 """
 
 logger_get(name=__logger_name__, loglevel=__logger_level__)
 app_context = AppContext(debug=True if __logger_level__ == "debug" else False, profiler=__app_profiler__)
```

### Comparing `hibp_downloader-0.1.2/src/hibp_downloader/commands/hibp_download.py` & `hibp_downloader-0.1.3/src/hibp_downloader/commands/hibp_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,38 +99,38 @@
     logger.info(f"data-path {app_context.data_path!r}")
     logger.info(f"metadata-path {app_context.metadata_path!r}")
 
     if force:
         ignore_etag = True
         local_cache_ttl = 0
 
-    encoding_type = __encoding_type__
-    prefix_chunks = iterable_chunker(
-        iterable=hex_sequence(hex_first=first_hash[0:5], hex_last=last_hash[0:5]), size=chunk_size
-    )
-
     results_queue_process = Process(target=results_queue_processor, args=(results_queue,))
     results_queue_process.start()
 
     with Pool(
         processes=processes, initializer=results_queue_initialize, initargs=(results_queue,)
     ) as multiprocessing_pool:
+        prefix_chunks = iterable_chunker(
+            iterable=hex_sequence(hex_first=first_hash[0:5], hex_last=last_hash[0:5]), size=chunk_size
+        )
+
         multiprocessing_pool.starmap(
             pwnedpasswords_get_and_store_asyncio_run,
             zip(
                 prefix_chunks,
                 repeat(hash_type),
                 repeat(os.path.join(app_context.data_path, hash_type.value)),  # data_path
                 repeat(os.path.join(app_context.metadata_path, hash_type.value)),  # metadata_path
-                repeat(encoding_type),
+                repeat(__encoding_type__),  # encoding_type: read comments in __init__ before wanting Brotli
                 repeat(ignore_etag),
                 repeat(local_cache_ttl),
                 repeat(logger),
             ),
         )
+
         multiprocessing_pool.close()
         multiprocessing_pool.join()
         results_queue.put(results_queue_exit_sentinel)
 
     results_queue_process.join()
 
 
@@ -259,14 +259,16 @@
 
 def results_queue_processor(q: Queue):
     running_stats = QueueRunningStats()
 
     while True:
         metadata_items = q.get()
         if metadata_items == results_queue_exit_sentinel:
+            running_stats.end_trigger()
+            logger.info(f"Finished in {round(running_stats.run_time/60,1)}min")
             break
 
         if metadata_items:
             running_stats.add_item_stats(item=QueueItemStatsCompute(metadata_items).stats)
 
         if running_stats.queue_item_count % __logging_info_event_modulus__ == 0:
             logger.info(
@@ -275,15 +277,15 @@
                 f"et:{running_stats.local_source_etag_match_count_sum} "
                 f"rc:{running_stats.remote_source_remote_cache_count_sum} "
                 f"ro:{running_stats.remote_source_origin_source_count_sum} "
                 f"xx:{running_stats.unknown_source_status_count_sum}] "
                 f"runtime_rate=[{to_mbytes(running_stats.bytes_received_rate_total * 8, 1)}MBit/s "
                 f"{int(running_stats.request_rate_total)}req/s "
                 f"~{int(running_stats.bytes_received_rate_total / __approx_gzip_bytes_per_hash__)}H/s] "
-                f"runtime={round(running_stats.run_time/3600,2)}hr "
+                f"runtime={round(running_stats.run_time/60,1)}min "
                 f"download={to_mbytes(running_stats.bytes_received_sum, 1)}MB"
             )
 
 
 def to_mbytes(value, rounding=None):
     if value is not None:
         return round(value / 1024 / 1024, rounding) if rounding else value / 1024 / 1024
```

### Comparing `hibp_downloader-0.1.2/src/hibp_downloader/commands/hibp_generate.py` & `hibp_downloader-0.1.3/src/hibp_downloader/commands/hibp_generate.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.2/src/hibp_downloader/exceptions.py` & `hibp_downloader-0.1.3/src/hibp_downloader/exceptions.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.2/src/hibp_downloader/lib/app.py` & `hibp_downloader-0.1.3/src/hibp_downloader/lib/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     # command context
     app_context.command = ctx.invoked_subcommand
     app_context.data_path = data_path
     app_context.metadata_path = metadata_path if metadata_path else data_path
 
     # start
-    logger.info(f"{__title__} [v{__version__}]")
+    logger.info(f"{__title__}: v{__version__}")
 
 
 def load_commands():
     loader_paths = [os.path.join(os.path.dirname(__file__), "..", "commands")]
 
     for loader_path in loader_paths:
         loader_path = os.path.realpath(loader_path)
```

### Comparing `hibp_downloader-0.1.2/src/hibp_downloader/lib/filedata.py` & `hibp_downloader-0.1.3/src/hibp_downloader/lib/filedata.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,18 +86,21 @@
     filename = os.path.join(metadata_path, prefix[0:2], prefix[2:4], f"{prefix}.meta")
 
     content = None
     if await aiofiles.os.path.isfile(filename):
         async with aiofiles.open(filename, "r") as f:
             content = await f.read()
 
-    if content is None:
+    if not content:
         return PrefixMetadata(prefix=prefix)
 
-    prefix_metadata = PrefixMetadata(**json.loads(content))
+    try:
+        prefix_metadata = PrefixMetadata(**json.loads(content))
+    except ValueError:
+        return PrefixMetadata(prefix=prefix)
 
     if isinstance(prefix_metadata.server_timestamp, str):
         prefix_metadata.server_timestamp = datetime.fromisoformat(prefix_metadata.server_timestamp)
     if isinstance(prefix_metadata.last_modified, str):
         prefix_metadata.last_modified = datetime.fromisoformat(prefix_metadata.last_modified)
 
     return prefix_metadata
```

### Comparing `hibp_downloader-0.1.2/src/hibp_downloader/lib/generators.py` & `hibp_downloader-0.1.3/src/hibp_downloader/lib/generators.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.2/src/hibp_downloader/lib/http.py` & `hibp_downloader-0.1.3/src/hibp_downloader/lib/http.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.2/src/hibp_downloader/lib/logger.py` & `hibp_downloader-0.1.3/src/hibp_downloader/lib/logger.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.2/src/hibp_downloader/main.py` & `hibp_downloader-0.1.3/src/hibp_downloader/main.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.2/src/hibp_downloader/models/prefix_metadata.py` & `hibp_downloader-0.1.3/src/hibp_downloader/models/prefix_metadata.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.2/src/hibp_downloader/models/stats.py` & `hibp_downloader-0.1.3/src/hibp_downloader/models/stats.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.2/PKG-INFO` & `hibp_downloader-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hibp-downloader
-Version: 0.1.2
+Version: 0.1.3
 Summary: Efficiently download HIBP new pwned password data by hash-prefix for a local-copy
 License: BSD-3-Clause
 Keywords: hibp-downloader,hibp,haveibeenpwned,haveibeenpwned-downloader,sha1,ntlm
 Author: Nicholas de Jong
 Author-email: contact@threatpatrols.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -28,50 +28,47 @@
 # hibp-downloader
 
 [![PyPi](https://img.shields.io/pypi/v/hibp-downloader.svg)](https://pypi.python.org/pypi/hibp-downloader/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/hibp-downloader.svg)](https://github.com/threatpatrols/hibp-downloader/)
 [![build tests](https://github.com/threatpatrols/hibp-downloader/actions/workflows/build-tests.yml/badge.svg)](https://github.com/threatpatrols/hibp-downloader/actions/workflows/build-tests.yml)
 [![License](https://img.shields.io/github/license/threatpatrols/hibp-downloader.svg)](https://github.com/threatpatrols/hibp-downloader)
 
-This is a Python implementation of the original [PwnedPasswordsDownloader](https://github.com/HaveIBeenPwned/PwnedPasswordsDownloader)
-that provides some additional useful functionality 
- - Automatically only download prefix-chunks that have changed since the last download
+This is a Python implementation of [PwnedPasswordsDownloader](https://github.com/HaveIBeenPwned/PwnedPasswordsDownloader)
+that is more download efficient and provides additional useful functionality
+ - Automatically **only** download prefix-chunks that have changed since the last download
  - Ability to start, stop and re-start without loss of data already collected
- - Ability to name the `--first-hash` and `--last-hash` positions
- - Metadata file per prefix file in JSON format for easy data reuse
+ - Ability to start and stop at named hash positions
+ - Per prefix file metadata in JSON format for easy data reuse
 
 ## Install
 ```commandline
 pip install --upgrade hibp-downloader
 ```
 
 ## Usage
 ![screenshot-help.png](https://raw.githubusercontent.com/threatpatrols/hibp-downloader/main/docs/assets/screenshot-help.png)
 
 ## Runtime Logs
-Sample download activity logs 
+Sample download activity log
 ```text
-2023-07-30T21:42:06+1000 | INFO | hibp-downloader | prefix=65747 source=[lc:207328 et:0 rc:56672 ro:0 xx:0] runtime_rate=[10.3MBit/s 79req/s ~65602H/s] runtime=0.2hr download=922.5MB
-2023-07-30T21:42:07+1000 | INFO | hibp-downloader | prefix=29da7 source=[lc:207328 et:0 rc:56792 ro:0 xx:0] runtime_rate=[10.4MBit/s 79req/s ~65646H/s] runtime=0.2hr download=924.5MB
-2023-07-30T21:42:09+1000 | INFO | hibp-downloader | prefix=43c7f source=[lc:207328 et:0 rc:56912 ro:0 xx:0] runtime_rate=[10.3MBit/s 79req/s ~65617H/s] runtime=0.2hr download=926.5MB
+2023-07-31T03:22:45+1000 | INFO | hibp-downloader | prefix=e585f source=[lc:265201 et:0 rc:722148 ro:3 xx:0] runtime_rate=[11.2MBit/s 86req/s ~71005H/s] runtime=2.33hr download=11748.0MB
+2023-07-31T03:22:48+1000 | INFO | hibp-downloader | prefix=e5877 source=[lc:265201 et:0 rc:722268 ro:3 xx:0] runtime_rate=[11.2MBit/s 86req/s ~70998H/s] runtime=2.33hr download=11750.0MB
+2023-07-31T03:22:50+1000 | INFO | hibp-downloader | prefix=f5837 source=[lc:265201 et:0 rc:722388 ro:3 xx:0] runtime_rate=[11.2MBit/s 86req/s ~70992H/s] runtime=2.33hr download=11751.9MB
 ```
- - 79 requests per second to api.pwnedpasswords.com
- - 207,328 prefix files from (`lc`) local-cache
- - 56,912 prefix files from (`rc`) remote-cache
- - 0 files from (`ro`) remote-origin, 0 files failed (`xx`) download
- - estimated 65,617 hash values downloaded per second
- - 926MB downloaded in ~12 minutes (0.20 hour)
+ - 86 requests per second to api.pwnedpasswords.com
+ - 265,201 prefix files from (`lc`) local-cache; 722,388 from (`rc`) remote-cache; 3 from (`ro`) remote-origin; 0 failed (`xx`) download
+ - estimated ~70k hash values downloaded per second
+ - 11.5GB (11,751MB) downloaded in 2.3 hours
 
+## Source
+ - https://github.com/threatpatrols/hibp-downloader
 
 ## Issues
  - https://github.com/threatpatrols/hibp-downloader/issues
 
-## Source
- - https://github.com/threatpatrols/hibp-downloader
-
 ## Copyright
  - Copyright &copy; 2023 Threat Patrols Pty Ltd &lt;contact@threatpatrols.com&gt;
  - Copyright &copy; 2023 Nicholas de Jong &lt;contact@nicholasdejong.com&gt;
 
 All rights reserved.
 
 ## License
```

