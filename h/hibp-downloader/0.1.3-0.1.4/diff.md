# Comparing `tmp/hibp_downloader-0.1.3.tar.gz` & `tmp/hibp_downloader-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hibp_downloader-0.1.3.tar", max compression
+gzip compressed data, was "hibp_downloader-0.1.4.tar", max compression
```

## Comparing `hibp_downloader-0.1.3.tar` & `hibp_downloader-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0     1565 2023-07-26 04:14:23.983439 hibp_downloader-0.1.3/LICENSE
--rw-r--r--   0        0        0     2572 2023-07-31 00:24:18.561251 hibp_downloader-0.1.3/README.md
--rw-r--r--   0        0        0     2937 2023-07-31 02:11:13.366700 hibp_downloader-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1570 2023-07-31 02:11:13.371700 hibp_downloader-0.1.3/src/hibp_downloader/__init__.py
--rw-r--r--   0        0        0    10970 2023-07-31 02:07:51.377302 hibp_downloader-0.1.3/src/hibp_downloader/commands/hibp_download.py
--rw-r--r--   0        0        0     3813 2023-07-30 11:12:13.966653 hibp_downloader-0.1.3/src/hibp_downloader/commands/hibp_generate.py
--rw-r--r--   0        0        0      568 2023-07-26 04:18:19.902342 hibp_downloader-0.1.3/src/hibp_downloader/exceptions.py
--rw-r--r--   0        0        0     4267 2023-07-31 01:58:30.039646 hibp_downloader-0.1.3/src/hibp_downloader/lib/app.py
--rw-r--r--   0        0        0     3818 2023-07-31 02:08:03.814450 hibp_downloader-0.1.3/src/hibp_downloader/lib/filedata.py
--rw-r--r--   0        0        0      657 2023-07-29 09:39:32.590020 hibp_downloader-0.1.3/src/hibp_downloader/lib/generators.py
--rw-r--r--   0        0        0     1858 2023-07-30 07:01:44.988273 hibp_downloader-0.1.3/src/hibp_downloader/lib/http.py
--rw-r--r--   0        0        0     3281 2023-07-30 13:34:36.552050 hibp_downloader-0.1.3/src/hibp_downloader/lib/logger.py
--rw-r--r--   0        0        0     1285 2023-07-30 06:49:39.677165 hibp_downloader-0.1.3/src/hibp_downloader/main.py
--rw-r--r--   0        0        0      214 2023-07-30 03:31:02.403390 hibp_downloader-0.1.3/src/hibp_downloader/models/__init__.py
--rw-r--r--   0        0        0      395 2023-07-30 13:34:36.556051 hibp_downloader-0.1.3/src/hibp_downloader/models/app_context.py
--rw-r--r--   0        0        0       87 2023-07-29 11:47:32.763631 hibp_downloader-0.1.3/src/hibp_downloader/models/hash_type.py
--rw-r--r--   0        0        0     1829 2023-07-30 13:34:36.559051 hibp_downloader-0.1.3/src/hibp_downloader/models/prefix_metadata.py
--rw-r--r--   0        0        0     5456 2023-07-30 13:34:36.562051 hibp_downloader-0.1.3/src/hibp_downloader/models/stats.py
--rw-r--r--   0        0        0        0 2023-07-26 00:51:50.083564 hibp_downloader-0.1.3/src/hibp_downloader/py.typed
--rw-r--r--   0        0        0     3818 1970-01-01 00:00:00.000000 hibp_downloader-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1565 2023-07-26 04:14:23.983439 hibp_downloader-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3350 2023-07-31 12:58:13.391147 hibp_downloader-0.1.4/README.md
+-rw-r--r--   0        0        0     3639 2023-07-31 12:56:50.702165 hibp_downloader-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1771 2023-07-31 12:56:50.707166 hibp_downloader-0.1.4/src/hibp_downloader/__init__.py
+-rw-r--r--   0        0        0    10970 2023-07-31 02:13:39.644436 hibp_downloader-0.1.4/src/hibp_downloader/commands/hibp_download.py
+-rw-r--r--   0        0        0     3813 2023-07-30 11:12:13.966653 hibp_downloader-0.1.4/src/hibp_downloader/commands/hibp_generate.py
+-rw-r--r--   0        0        0     3533 2023-07-31 12:56:50.711166 hibp_downloader-0.1.4/src/hibp_downloader/commands/hibp_query.py
+-rw-r--r--   0        0        0      568 2023-07-26 04:18:19.902342 hibp_downloader-0.1.4/src/hibp_downloader/exceptions.py
+-rw-r--r--   0        0        0     4511 2023-07-31 12:56:50.716166 hibp_downloader-0.1.4/src/hibp_downloader/lib/app.py
+-rw-r--r--   0        0        0     3818 2023-07-31 12:56:50.721166 hibp_downloader-0.1.4/src/hibp_downloader/lib/filedata.py
+-rw-r--r--   0        0        0      657 2023-07-29 09:39:32.590020 hibp_downloader-0.1.4/src/hibp_downloader/lib/generators.py
+-rw-r--r--   0        0        0      243 2023-07-31 12:56:50.724166 hibp_downloader-0.1.4/src/hibp_downloader/lib/hashing.py
+-rw-r--r--   0        0        0     1858 2023-07-30 07:01:44.988273 hibp_downloader-0.1.4/src/hibp_downloader/lib/http.py
+-rw-r--r--   0        0        0     3281 2023-07-30 13:34:36.552050 hibp_downloader-0.1.4/src/hibp_downloader/lib/logger.py
+-rw-r--r--   0        0        0     5304 2023-07-31 12:56:50.727166 hibp_downloader-0.1.4/src/hibp_downloader/lib/md4.py
+-rw-r--r--   0        0        0     1285 2023-07-30 06:49:39.677165 hibp_downloader-0.1.4/src/hibp_downloader/main.py
+-rw-r--r--   0        0        0      214 2023-07-30 03:31:02.403390 hibp_downloader-0.1.4/src/hibp_downloader/models/__init__.py
+-rw-r--r--   0        0        0      395 2023-07-30 13:34:36.556051 hibp_downloader-0.1.4/src/hibp_downloader/models/app_context.py
+-rw-r--r--   0        0        0       87 2023-07-29 11:47:32.763631 hibp_downloader-0.1.4/src/hibp_downloader/models/hash_type.py
+-rw-r--r--   0        0        0     1829 2023-07-30 13:34:36.559051 hibp_downloader-0.1.4/src/hibp_downloader/models/prefix_metadata.py
+-rw-r--r--   0        0        0     5456 2023-07-30 13:34:36.562051 hibp_downloader-0.1.4/src/hibp_downloader/models/stats.py
+-rw-r--r--   0        0        0        0 2023-07-26 00:51:50.083564 hibp_downloader-0.1.4/src/hibp_downloader/py.typed
+-rw-r--r--   0        0        0     4597 1970-01-01 00:00:00.000000 hibp_downloader-0.1.4/PKG-INFO
```

### Comparing `hibp_downloader-0.1.3/LICENSE` & `hibp_downloader-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.3/README.md` & `hibp_downloader-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 # hibp-downloader
 
-[![PyPi](https://img.shields.io/pypi/v/hibp-downloader.svg)](https://pypi.python.org/pypi/hibp-downloader/)
-[![Python Versions](https://img.shields.io/pypi/pyversions/hibp-downloader.svg)](https://github.com/threatpatrols/hibp-downloader/)
+[![pypi](https://img.shields.io/pypi/v/hibp-downloader.svg)](https://pypi.python.org/pypi/hibp-downloader/)
+[![python](https://img.shields.io/pypi/pyversions/hibp-downloader.svg)](https://github.com/threatpatrols/hibp-downloader/)
 [![build tests](https://github.com/threatpatrols/hibp-downloader/actions/workflows/build-tests.yml/badge.svg)](https://github.com/threatpatrols/hibp-downloader/actions/workflows/build-tests.yml)
-[![License](https://img.shields.io/github/license/threatpatrols/hibp-downloader.svg)](https://github.com/threatpatrols/hibp-downloader)
+[![docs](https://img.shields.io/readthedocs/hibp-downloader)](https://hibp-downloader.readthedocs.io)
+[![license](https://img.shields.io/github/license/threatpatrols/hibp-downloader.svg)](https://github.com/threatpatrols/hibp-downloader)
 
-This is a Python implementation of [PwnedPasswordsDownloader](https://github.com/HaveIBeenPwned/PwnedPasswordsDownloader)
-that is more download efficient and provides additional useful functionality
- - Automatically **only** download prefix-chunks that have changed since the last download
- - Ability to start, stop and re-start without loss of data already collected
- - Ability to start and stop at named hash positions
- - Per prefix file metadata in JSON format for easy data reuse
+This is a CLI tool to efficiently download a local copy of the pwned password hash data from the very awesome
+[HIBP](https://haveibeenpwned.com/Passwords) pwned passwords [api-endpoint](https://api.pwnedpasswords.com) using 
+multiprocessing, async-processes, local-caching, content-etags and http2-connection pooling to make things as fast 
+as (seems) Pythonly possible.
+
+## Features
+
+ - Only download hash-prefix content blocks when the hash-prefix block content has changed.
+ - Start, stop and re-start the data-collection process without loss of data already collected.
+ - Ability to query clear text values and return results from the pwned password data set.
+ - Generate a single text file with pwned password hash values in-order, similar to [PwnedPasswordsDownloader](https://github.com/HaveIBeenPwned/PwnedPasswordsDownloader) from the HIBP team.
+ - Per prefix file metadata in JSON format for easy data reuse.
 
 ## Install
 ```commandline
 pip install --upgrade hibp-downloader
 ```
 
 ## Usage
-![screenshot-help.png](https://raw.githubusercontent.com/threatpatrols/hibp-downloader/main/docs/assets/screenshot-help.png)
+![screenshot-help.png](https://raw.githubusercontent.com/threatpatrols/hibp-downloader/main/docs/content/assets/screenshot-help.png)
 
-## Runtime Logs
-Sample download activity log
+## Performance
+Sample download activity log; host with 12 cores on 45Mbit/s DSL connection. 
 ```text
 2023-07-31T03:22:45+1000 | INFO | hibp-downloader | prefix=e585f source=[lc:265201 et:0 rc:722148 ro:3 xx:0] runtime_rate=[11.2MBit/s 86req/s ~71005H/s] runtime=2.33hr download=11748.0MB
 2023-07-31T03:22:48+1000 | INFO | hibp-downloader | prefix=e5877 source=[lc:265201 et:0 rc:722268 ro:3 xx:0] runtime_rate=[11.2MBit/s 86req/s ~70998H/s] runtime=2.33hr download=11750.0MB
 2023-07-31T03:22:50+1000 | INFO | hibp-downloader | prefix=f5837 source=[lc:265201 et:0 rc:722388 ro:3 xx:0] runtime_rate=[11.2MBit/s 86req/s ~70992H/s] runtime=2.33hr download=11751.9MB
 ```
- - 86 requests per second to api.pwnedpasswords.com
+
+ - 86 requests per second to `api.pwnedpasswords.com`
  - 265,201 prefix files from (`lc`) local-cache; 722,388 from (`rc`) remote-cache; 3 from (`ro`) remote-origin; 0 failed (`xx`) download
  - estimated ~70k hash values downloaded per second
- - 11.5GB (11,751MB) downloaded in 2.3 hours
+ - 11.5GB (11,751MB) downloaded in 2.3 hours (full dataset is ~3.5 hours)
 
-## Source
- - https://github.com/threatpatrols/hibp-downloader
+## Project
 
-## Issues
- - https://github.com/threatpatrols/hibp-downloader/issues
+ - Github - [github.com/threatpatrols/hibp-downloader](https://github.com/threatpatrols/hibp-downloader)
+ - PyPI - [pypi.org/project/hibp-downloader/](https://pypi.org/project/hibp-downloader/)
+ - ReadTheDocs - [hibp-downloader.readthedocs.io](https://hibp-downloader.readthedocs.io)
 
 ## Copyright
- - Copyright &copy; 2023 Threat Patrols Pty Ltd &lt;contact@threatpatrols.com&gt;
- - Copyright &copy; 2023 Nicholas de Jong &lt;contact@nicholasdejong.com&gt;
+ - Copyright &copy; 2023 [Threat Patrols Pty Ltd](https://www.threatpatrols.com)
+ - Copyright &copy; 2023 [Nicholas de Jong](https://www.nicholasdejong.com)
 
 All rights reserved.
 
 ## License
  * BSD-3-Clause - see LICENSE file for details.
```

### Comparing `hibp_downloader-0.1.3/pyproject.toml` & `hibp_downloader-0.1.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hibp-downloader"
-version = "0.1.3"
+version = "0.1.4"
 description = "Efficiently download HIBP new pwned password data by hash-prefix for a local-copy"
 authors = ["Nicholas de Jong <contact@threatpatrols.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [{ include = "hibp_downloader", from = "src" }]
 classifiers = [
     "Environment :: Console",
@@ -24,29 +24,39 @@
 Repository = "https://gitlab.com/threatpatrols/hibp-downloader"
 
 [tool.poetry.scripts]
 hibp-downloader = "hibp_downloader.main:entrypoint"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-"httpx[http2]" = "^0.24.1"      # https://pypi.org/project/httpx/#history
-"typer[all]" = "0.9.0"          # https://pypi.org/project/typer/#history
-shellingham = "1.5.0.post1"     # https://pypi.org/project/shellingham/#history
-aiofiles = "23.1.0"             # https://pypi.org/project/aiofiles/#history
+"httpx[http2]" = "^0.24"        # https://pypi.org/project/httpx/#history
+"typer[all]" = "^0.9"           # https://pypi.org/project/typer/#history
+shellingham = "^1.5"            # https://pypi.org/project/shellingham/#history
+aiofiles = "^23.0"              # https://pypi.org/project/aiofiles/#history
 
 [tool.poetry.dev-dependencies]
-black = "^23.7.0"               # https://pypi.org/project/black/#history
-flake8 = "^6.1.0"               # https://pypi.org/project/flake8/#history
-isort = "^5.12.0"               # https://pypi.org/project/isort/#history
-mypy = "^1.4.1"                 # https://pypi.org/project/mypy/#history
-pycln = "^2.1.7"                # https://pypi.org/project/pycln/#history
-pytest = "^7.4.0"               # https://pypi.org/project/pytest/#history
+black = "^23.7"                 # https://pypi.org/project/black/#history
+flake8 = "^6.1"                 # https://pypi.org/project/flake8/#history
+isort = "^5.12"                 # https://pypi.org/project/isort/#history
+mypy = "^1.4"                   # https://pypi.org/project/mypy/#history
+pycln = "^2.1"                  # https://pypi.org/project/pycln/#history
+pytest = "^7.4"                 # https://pypi.org/project/pytest/#history
 safety = "^2.4.0b1"             # https://pypi.org/project/safety/#history
-pyinstrument = "^4.5.1"         # https://pypi.org/project/pyinstrument/#history
-types-aiofiles = "23.1.0.5"     # https://pypi.org/project/types-aiofiles/#history
+pyinstrument = "^4.5"           # https://pypi.org/project/pyinstrument/#history
+types-aiofiles = "23.1"         # https://pypi.org/project/types-aiofiles/#history
+# NB: pip installs in .readthedocs.yml need to be kept up-to-date manually
+novella = "^0.2"                # https://pypi.org/project/novella/#history
+pydoc-markdown = "^4.8"         # https://pypi.org/project/pydoc-markdown/#history
+mkdocs-material = "^9.1"        # https://pypi.org/project/mkdocs-material/#history
+
+[tool.poetry.plugins."slap.plugins.check"]
+changelog = "slap.ext.checks.changelog:ChangelogValidationCheckPlugin"
+general = "slap.ext.checks.general:GeneralChecksPlugin"
+poetry = "slap.ext.checks.poetry:PoetryChecksPlugin"
+release = "slap.ext.checks.release:ReleaseChecksPlugin"
 
 [tool.slap]
 typed = true
 release.branch = "dev"
 
 [tool.slap.test]
 check = "slap check"
@@ -55,15 +65,17 @@
 isort = "isort --check-only src/ tests/"
 # mypy = "dmypy run src/"
 pycln  = "pycln src/ tests/ --check"
 safety = "pip freeze | safety check --stdin --short-report --output text"
 pytest = "pytest tests/ -vv"
 
 [tool.slap.run]
-format = "black src/ tests/ && isort src/ tests/ "
+format = "black src/ tests/ && isort src/ tests/"
+docs-build = "cd docs && novella --base-url hibp-downloader/"
+docs-server = "cd docs && novella --serve"
 
 [tool.mypy]
 explicit_package_bases = true
 ignore_missing_imports = true
 mypy_path = ["src"]
 namespace_packages = true
 pretty = true
```

### Comparing `hibp_downloader-0.1.3/src/hibp_downloader/__init__.py` & `hibp_downloader-0.1.4/src/hibp_downloader/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from os import cpu_count, getenv
 from sys import argv
 
 from .lib.logger import logger_get
 from .models import AppContext
 
 __title__ = "HIBP Downloader"
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __logger_name__ = "hibp-downloader"
 __pwnedpasswords_api_url__ = "https://api.pwnedpasswords.com"
 __local_cache_ttl_default__ = 86400
 __multiprocessing_processes_default__ = cpu_count()
 __multiprocessing_prefixes_chunk_size__ = cpu_count() * 2
 __approx_gzip_bytes_per_hash__ = 20.674
 __logging_info_event_modulus__ = 5
@@ -20,19 +20,24 @@
 # tools (eg zcat, zgrep) are more readily available than brotli enabled tools when examining the data-store files
 __encoding_type__ = "gzip"  # values: [ gzip | br | None ]
 
 __logger_level__ = "info"
 if "--debug" in argv or getenv("HIBPDL_DEBUG", "").lower().startswith(("true", "yes", "enable")):
     __logger_level__ = "debug"
 
+if "--quiet" in argv or getenv("HIBPDL_QUIET", "").lower().startswith(("true", "yes", "enable")):
+    __logger_level__ = "fatal"
+
 __app_profiler__ = False
 if "--profiler" in argv or getenv("HIBPDL_PROFILER", "").lower().startswith(("true", "yes", "enable")):
     __app_profiler__ = True
 
 __help_epilog_footer__ = f"""
-{__title__}: v{__version__}
+{__title__} v{__version__}
+
+Docs: [hibp-downloader.readthedocs.io](https://hibp-downloader.readthedocs.io)
 
-Project: [https://github.com/threatpatrols/hibp-downloader](https://github.com/threatpatrols/hibp-downloader)
+Project: [github.com/threatpatrols/hibp-downloader](https://github.com/threatpatrols/hibp-downloader)
 """
 
 logger_get(name=__logger_name__, loglevel=__logger_level__)
 app_context = AppContext(debug=True if __logger_level__ == "debug" else False, profiler=__app_profiler__)
```

### Comparing `hibp_downloader-0.1.3/src/hibp_downloader/commands/hibp_download.py` & `hibp_downloader-0.1.4/src/hibp_downloader/commands/hibp_download.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.3/src/hibp_downloader/commands/hibp_generate.py` & `hibp_downloader-0.1.4/src/hibp_downloader/commands/hibp_generate.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.3/src/hibp_downloader/exceptions.py` & `hibp_downloader-0.1.4/src/hibp_downloader/exceptions.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.3/src/hibp_downloader/lib/app.py` & `hibp_downloader-0.1.4/src/hibp_downloader/lib/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 import importlib
 import os
 import sys
-import textwrap
 
 import typer
 from typing_extensions import Annotated
 
 from .. import __help_epilog_footer__, __logger_name__, __title__, __version__, app_context
 from ..exceptions import HibpDownloaderException
 from ..lib.logger import logger_get
 
 logger = logger_get(name=__logger_name__)
 app = typer.Typer(
     add_completion=app_context.add_completion,
     no_args_is_help=app_context.no_args_is_help,
     rich_markup_mode="rich",
-    epilog=textwrap.dedent(
-        """
-        Environment variables prefixed with HIBPDL_ that match their command-line equivalent may be used; for
-        example use [bold]HIBPDL_DATA_PATH[/bold] to set the --data-path command option.
-           
-           
-           
-    """
-        + __help_epilog_footer__,
+    epilog=(
+        "Environment variables prefixed with HIBPDL_ that match their command-line equivalent may be used; for "
+        "example use [bold]HIBPDL_DATA_PATH[/bold] to set the --data-path command option."
+        "\n\n---\n"
+        f"{__help_epilog_footer__}"
     ),
 )
 
 
 def invoke_app():
     try:
         load_commands()
@@ -58,29 +53,41 @@
     profiler: Annotated[
         bool,
         typer.Option(
             hidden=True, help="Enable the application performance profiler", envvar="HIBPDL_PROFILER", show_envvar=False
         ),
     ] = False,
     debug: Annotated[
-        bool, typer.Option(help="Enable debug logging to stderr", envvar="HIBPDL_DEBUG", show_envvar=False)
+        bool, typer.Option(help="Set logging to debug-level messages", envvar="HIBPDL_DEBUG", show_envvar=False)
+    ] = False,
+    quiet: Annotated[
+        bool,
+        typer.Option(
+            help="Set logging to fatal-level messages; overrides --debug option",
+            envvar="HIBPDL_QUIET",
+            show_envvar=False,
+        ),
     ] = False,
 ):
     """
-    [bold]hibp-downloader[/bold] - Efficiently download new data for a local-copy of the pwned password hashes from https://api.pwnedpasswords.com
+    [bold]hibp-downloader[/bold] - Efficiently download new pwned password hashes from api.pwnedpasswords.com fast.
     """
 
     # return early if --help is all we need
     if "--help" in sys.argv:
         return
 
     # debug is captured at __init__; referenced here for happy linters
     if debug:
         ...
 
+    # quiet is captured at __init__; referenced here for happy linters
+    if quiet:
+        ...
+
     # profiler is captured at __init__; referenced here for happy linters
     if profiler:
         ...
 
     # command context
     app_context.command = ctx.invoked_subcommand
     app_context.data_path = data_path
```

### Comparing `hibp_downloader-0.1.3/src/hibp_downloader/lib/filedata.py` & `hibp_downloader-0.1.4/src/hibp_downloader/lib/filedata.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         data = gzip.decompress(data)
     else:
         raise HibpDownloaderException(f"Unsupported decompression_type {decompression_type}")
 
     if prepend_prefix is False:
         return data.decode("utf8")
 
-    data_lines = [f"{prefix.lower()}{x.lower()}" for x in data.decode("utf8").replace("\r", "").split("\n")]
+    data_lines = [f"{prefix.upper()}{x.upper()}" for x in data.decode("utf8").replace("\r", "").split("\n")]
     return "\n".join(data_lines)
 
 
 async def load_metadata(metadata_path: str, prefix: str) -> PrefixMetadata:
     filename = os.path.join(metadata_path, prefix[0:2], prefix[2:4], f"{prefix}.meta")
 
     content = None
```

### Comparing `hibp_downloader-0.1.3/src/hibp_downloader/lib/generators.py` & `hibp_downloader-0.1.4/src/hibp_downloader/lib/generators.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.3/src/hibp_downloader/lib/http.py` & `hibp_downloader-0.1.4/src/hibp_downloader/lib/http.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.3/src/hibp_downloader/lib/logger.py` & `hibp_downloader-0.1.4/src/hibp_downloader/lib/logger.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.3/src/hibp_downloader/main.py` & `hibp_downloader-0.1.4/src/hibp_downloader/main.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.3/src/hibp_downloader/models/prefix_metadata.py` & `hibp_downloader-0.1.4/src/hibp_downloader/models/prefix_metadata.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.3/src/hibp_downloader/models/stats.py` & `hibp_downloader-0.1.4/src/hibp_downloader/models/stats.py`

 * *Files identical despite different names*

### Comparing `hibp_downloader-0.1.3/PKG-INFO` & `hibp_downloader-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,84 @@
 Metadata-Version: 2.1
 Name: hibp-downloader
-Version: 0.1.3
+Version: 0.1.4
 Summary: Efficiently download HIBP new pwned password data by hash-prefix for a local-copy
 License: BSD-3-Clause
 Keywords: hibp-downloader,hibp,haveibeenpwned,haveibeenpwned-downloader,sha1,ntlm
 Author: Nicholas de Jong
 Author-email: contact@threatpatrols.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiofiles (==23.1.0)
-Requires-Dist: httpx[http2] (>=0.24.1,<0.25.0)
-Requires-Dist: shellingham (==1.5.0.post1)
-Requires-Dist: typer[all] (==0.9.0)
+Requires-Dist: aiofiles (>=23.0,<24.0)
+Requires-Dist: httpx[http2] (>=0.24,<0.25)
+Requires-Dist: shellingham (>=1.5,<2.0)
+Requires-Dist: typer[all] (>=0.9,<0.10)
 Project-URL: Bug Tracker, https://github.com/threatpatrols/hibp-downloader/issues
 Project-URL: Documentation, https://github.com/threatpatrols/hibp-downloader
 Project-URL: Homepage, https://gitlab.com/threatpatrols/hibp-downloader
 Project-URL: Repository, https://gitlab.com/threatpatrols/hibp-downloader
 Description-Content-Type: text/markdown
 
 # hibp-downloader
 
-[![PyPi](https://img.shields.io/pypi/v/hibp-downloader.svg)](https://pypi.python.org/pypi/hibp-downloader/)
-[![Python Versions](https://img.shields.io/pypi/pyversions/hibp-downloader.svg)](https://github.com/threatpatrols/hibp-downloader/)
+[![pypi](https://img.shields.io/pypi/v/hibp-downloader.svg)](https://pypi.python.org/pypi/hibp-downloader/)
+[![python](https://img.shields.io/pypi/pyversions/hibp-downloader.svg)](https://github.com/threatpatrols/hibp-downloader/)
 [![build tests](https://github.com/threatpatrols/hibp-downloader/actions/workflows/build-tests.yml/badge.svg)](https://github.com/threatpatrols/hibp-downloader/actions/workflows/build-tests.yml)
-[![License](https://img.shields.io/github/license/threatpatrols/hibp-downloader.svg)](https://github.com/threatpatrols/hibp-downloader)
+[![docs](https://img.shields.io/readthedocs/hibp-downloader)](https://hibp-downloader.readthedocs.io)
+[![license](https://img.shields.io/github/license/threatpatrols/hibp-downloader.svg)](https://github.com/threatpatrols/hibp-downloader)
 
-This is a Python implementation of [PwnedPasswordsDownloader](https://github.com/HaveIBeenPwned/PwnedPasswordsDownloader)
-that is more download efficient and provides additional useful functionality
- - Automatically **only** download prefix-chunks that have changed since the last download
- - Ability to start, stop and re-start without loss of data already collected
- - Ability to start and stop at named hash positions
- - Per prefix file metadata in JSON format for easy data reuse
+This is a CLI tool to efficiently download a local copy of the pwned password hash data from the very awesome
+[HIBP](https://haveibeenpwned.com/Passwords) pwned passwords [api-endpoint](https://api.pwnedpasswords.com) using 
+multiprocessing, async-processes, local-caching, content-etags and http2-connection pooling to make things as fast 
+as (seems) Pythonly possible.
+
+## Features
+
+ - Only download hash-prefix content blocks when the hash-prefix block content has changed.
+ - Start, stop and re-start the data-collection process without loss of data already collected.
+ - Ability to query clear text values and return results from the pwned password data set.
+ - Generate a single text file with pwned password hash values in-order, similar to [PwnedPasswordsDownloader](https://github.com/HaveIBeenPwned/PwnedPasswordsDownloader) from the HIBP team.
+ - Per prefix file metadata in JSON format for easy data reuse.
 
 ## Install
 ```commandline
 pip install --upgrade hibp-downloader
 ```
 
 ## Usage
-![screenshot-help.png](https://raw.githubusercontent.com/threatpatrols/hibp-downloader/main/docs/assets/screenshot-help.png)
+![screenshot-help.png](https://raw.githubusercontent.com/threatpatrols/hibp-downloader/main/docs/content/assets/screenshot-help.png)
 
-## Runtime Logs
-Sample download activity log
+## Performance
+Sample download activity log; host with 12 cores on 45Mbit/s DSL connection. 
 ```text
 2023-07-31T03:22:45+1000 | INFO | hibp-downloader | prefix=e585f source=[lc:265201 et:0 rc:722148 ro:3 xx:0] runtime_rate=[11.2MBit/s 86req/s ~71005H/s] runtime=2.33hr download=11748.0MB
 2023-07-31T03:22:48+1000 | INFO | hibp-downloader | prefix=e5877 source=[lc:265201 et:0 rc:722268 ro:3 xx:0] runtime_rate=[11.2MBit/s 86req/s ~70998H/s] runtime=2.33hr download=11750.0MB
 2023-07-31T03:22:50+1000 | INFO | hibp-downloader | prefix=f5837 source=[lc:265201 et:0 rc:722388 ro:3 xx:0] runtime_rate=[11.2MBit/s 86req/s ~70992H/s] runtime=2.33hr download=11751.9MB
 ```
- - 86 requests per second to api.pwnedpasswords.com
+
+ - 86 requests per second to `api.pwnedpasswords.com`
  - 265,201 prefix files from (`lc`) local-cache; 722,388 from (`rc`) remote-cache; 3 from (`ro`) remote-origin; 0 failed (`xx`) download
  - estimated ~70k hash values downloaded per second
- - 11.5GB (11,751MB) downloaded in 2.3 hours
+ - 11.5GB (11,751MB) downloaded in 2.3 hours (full dataset is ~3.5 hours)
 
-## Source
- - https://github.com/threatpatrols/hibp-downloader
+## Project
 
-## Issues
- - https://github.com/threatpatrols/hibp-downloader/issues
+ - Github - [github.com/threatpatrols/hibp-downloader](https://github.com/threatpatrols/hibp-downloader)
+ - PyPI - [pypi.org/project/hibp-downloader/](https://pypi.org/project/hibp-downloader/)
+ - ReadTheDocs - [hibp-downloader.readthedocs.io](https://hibp-downloader.readthedocs.io)
 
 ## Copyright
- - Copyright &copy; 2023 Threat Patrols Pty Ltd &lt;contact@threatpatrols.com&gt;
- - Copyright &copy; 2023 Nicholas de Jong &lt;contact@nicholasdejong.com&gt;
+ - Copyright &copy; 2023 [Threat Patrols Pty Ltd](https://www.threatpatrols.com)
+ - Copyright &copy; 2023 [Nicholas de Jong](https://www.nicholasdejong.com)
 
 All rights reserved.
 
 ## License
  * BSD-3-Clause - see LICENSE file for details.
```

