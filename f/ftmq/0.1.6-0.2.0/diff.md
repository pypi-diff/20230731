# Comparing `tmp/ftmq-0.1.6.tar.gz` & `tmp/ftmq-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftmq-0.1.6.tar", max compression
+gzip compressed data, was "ftmq-0.2.0.tar", max compression
```

## Comparing `ftmq-0.1.6.tar` & `ftmq-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.1.6/LICENSE
--rw-r--r--   0        0        0     4376 2023-06-20 10:59:09.516461 ftmq-0.1.6/README.md
--rw-r--r--   0        0        0       22 2023-07-28 05:24:37.608824 ftmq-0.1.6/ftmq/__init__.py
--rw-r--r--   0        0        0     2714 2023-06-20 10:59:09.516461 ftmq-0.1.6/ftmq/cli.py
--rw-r--r--   0        0        0      287 2023-07-27 16:03:41.306274 ftmq-0.1.6/ftmq/enums.py
--rw-r--r--   0        0        0       43 2023-02-17 15:30:40.666516 ftmq-0.1.6/ftmq/exceptions.py
--rw-r--r--   0        0        0     4982 2023-07-28 04:09:12.400103 ftmq-0.1.6/ftmq/filters.py
--rw-r--r--   0        0        0     2151 2023-07-26 18:11:21.346315 ftmq-0.1.6/ftmq/io.py
--rw-r--r--   0        0        0     1784 2023-06-14 17:04:10.502390 ftmq-0.1.6/ftmq/query.py
--rw-r--r--   0        0        0      564 2023-07-28 05:20:05.583374 ftmq-0.1.6/ftmq/types.py
--rw-r--r--   0        0        0      973 2023-07-28 04:58:52.872628 ftmq-0.1.6/ftmq/util.py
--rw-r--r--   0        0        0     1415 2023-07-28 05:24:37.608824 ftmq-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5652 1970-01-01 00:00:00.000000 ftmq-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5162 2023-07-30 16:07:06.752065 ftmq-0.2.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-31 12:06:31.470588 ftmq-0.2.0/ftmq/__init__.py
+-rw-r--r--   0        0        0     3583 2023-07-31 11:55:19.470970 ftmq-0.2.0/ftmq/cli.py
+-rw-r--r--   0        0        0     1148 2023-07-28 20:08:27.942739 ftmq-0.2.0/ftmq/enums.py
+-rw-r--r--   0        0        0       43 2023-02-17 15:30:40.666516 ftmq-0.2.0/ftmq/exceptions.py
+-rw-r--r--   0        0        0     4998 2023-07-31 11:53:34.994545 ftmq-0.2.0/ftmq/filters.py
+-rw-r--r--   0        0        0     2868 2023-07-31 11:55:19.474970 ftmq-0.2.0/ftmq/io.py
+-rw-r--r--   0        0        0      175 2023-07-30 15:52:21.016040 ftmq-0.2.0/ftmq/model/__init__.py
+-rw-r--r--   0        0        0     2368 2023-07-30 15:33:11.604008 ftmq-0.2.0/ftmq/model/coverage.py
+-rw-r--r--   0        0        0     3899 2023-07-29 08:53:06.255213 ftmq-0.2.0/ftmq/model/dataset.py
+-rw-r--r--   0        0        0     2311 2023-07-31 11:41:09.826459 ftmq-0.2.0/ftmq/model/mixins.py
+-rw-r--r--   0        0        0     1784 2023-06-14 17:04:10.502390 ftmq-0.2.0/ftmq/query.py
+-rw-r--r--   0        0        0      896 2023-07-29 07:48:44.982562 ftmq-0.2.0/ftmq/types.py
+-rw-r--r--   0        0        0      698 2023-07-28 13:56:13.237817 ftmq-0.2.0/ftmq/util.py
+-rw-r--r--   0        0        0     1448 2023-07-31 12:06:31.470588 ftmq-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6514 1970-01-01 00:00:00.000000 ftmq-0.2.0/PKG-INFO
```

### Comparing `ftmq-0.1.6/LICENSE` & `ftmq-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.6/README.md` & `ftmq-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -84,14 +84,43 @@
 
     ftmq apply -i ./entities.ftm.json -d <aditional_dataset>
 
 Overwrite datasets:
 
     ftmq apply -i ./entities.ftm.json -d <aditional_dataset> --replace-dataset
 
+### Coverage / Statistics
+
+Often in ftm scripting, we are iterating through all the proxies (e.g. during aggregation). Why not use this to collect statistics on the way? There is a context manager for this, which turns into the `Coverage` model:
+
+Print coverage to stdout (and filtered entities to nowhere):
+
+    cat entities.ftm.json | ftmq -s Event -o /dev/null --coverage-uri -
+
+Within code:
+
+```python
+from ftmq.coverage import Coverage
+
+fragments = [...]
+buffer = {}
+
+coverage = Coverage({"frequency": "unknown"})
+with coverage as cx:
+    for proxy in fragments:
+        if proxy.id in buffer:
+            buffer[proxy.id].merge(proxy)
+        else:
+            buffer[proxy.id] = proxy
+            # here collect stats:
+            cx.collect(proxy)
+
+stats = coverage.dict()
+```
+
 ### ftmstore (database read)
 
 **NOT IMPLEMENTED YET**
 
 The same cli logic applies:
 
     ftmq store iterate -d ec_meetings -s Event --date__gte=2019 --date__lte=2020
```

### Comparing `ftmq-0.1.6/ftmq/cli.py` & `ftmq-0.2.0/ftmq/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import click
+import orjson
 from click_default_group import DefaultGroup
 
-from ftmq.io import apply_datasets, smart_read_proxies, smart_write_proxies
-
-from .query import Query
-from .util import parse_unknown_cli_filters
+from ftmq.io import (
+    apply_datasets,
+    smart_read,
+    smart_read_proxies,
+    smart_write,
+    smart_write_proxies,
+)
+from ftmq.model.coverage import Collector
+from ftmq.query import Query
+from ftmq.util import parse_unknown_cli_filters
 
 
 @click.group(cls=DefaultGroup, default="q", default_if_no_args=True)
 def cli():
     pass
 
 
@@ -27,23 +34,29 @@
 @click.option("-s", "--schema", multiple=True, help="Schema(s) to filter for")
 @click.option(
     "--schema-include-descendants", is_flag=True, default=False, show_default=True
 )
 @click.option(
     "--schema-include-matchable", is_flag=True, default=False, show_default=True
 )
+@click.option(
+    "--coverage-uri",
+    default=None,
+    help="If specified, print coverage information to this uri",
+)
 @click.argument("properties", nargs=-1)
 def q(
     input_uri: str | None = "-",
     output_uri: str | None = "-",
     dataset: tuple[str] | None = (),
     schema: tuple[str] | None = (),
     schema_include_descendants: bool | None = False,
     schema_include_matchable: bool | None = False,
     properties: tuple[str] | None = (),
+    coverage_uri: str | None = None,
 ):
     """
     Apply ftmq filter to a json stream of ftm entities.
     """
     q = Query()
     for value in dataset:
         q = q.where(dataset=value)
@@ -53,14 +66,18 @@
             include_descendants=schema_include_descendants,
             include_matchable=schema_include_matchable,
         )
     for prop, value, op in parse_unknown_cli_filters(properties):
         q = q.where(prop=prop, value=value, operator=op)
 
     proxies = q.apply_iter(smart_read_proxies(input_uri))
+    if coverage_uri:
+        coverage = Collector.apply(proxies)
+        coverage = orjson.dumps(coverage.dict(), option=orjson.OPT_APPEND_NEWLINE)
+        smart_write(coverage_uri, coverage)
     smart_write_proxies(output_uri, proxies, serialize=True)
 
 
 @cli.command("apply")
 @click.option(
     "-i", "--input-uri", default="-", show_default=True, help="input file or uri"
 )
@@ -79,7 +96,21 @@
     Uplevel an entity stream to nomenklatura entities and apply dataset(s) property
     """
 
     proxies = smart_read_proxies(input_uri)
     if dataset:
         proxies = apply_datasets(proxies, *dataset, replace=replace_dataset)
     smart_write_proxies(output_uri, proxies, serialize=True)
+
+
+@cli.command("io")
+@click.option(
+    "-i", "--input-uri", default="-", show_default=True, help="input file or uri"
+)
+@click.option(
+    "-o", "--output-uri", default="-", show_default=True, help="output file or uri"
+)
+def io(input_uri: str | None = "-", output_uri: str | None = "-"):
+    """
+    Generic cli wrapper around ftmq.io.smart_open
+    """
+    smart_write(output_uri, smart_read(input_uri))
```

### Comparing `ftmq-0.1.6/ftmq/filters.py` & `ftmq-0.2.0/ftmq/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from banal import as_bool, ensure_list
 from followthemoney import model
 from followthemoney.property import Property
 from followthemoney.schema import Schema
 from nomenklatura.dataset import Dataset
 from nomenklatura.entity import CE
 
-from .enums import Operators, Properties, Schemata
-from .exceptions import ValidationError
-from .types import Value
-from .util import StrEnum, make_dataset
+from ftmq.enums import Operators, Properties, Schemata, StrEnum
+from ftmq.exceptions import ValidationError
+from ftmq.types import Value
+from ftmq.util import make_dataset
 
 
 class BaseFilter:
     instance: Dataset | Schema | Property | None = None
     options: StrEnum = None
 
     def __init__(self, value: str | Dataset | Schema | Property | None):
```

### Comparing `ftmq-0.1.6/ftmq/query.py` & `ftmq-0.2.0/ftmq/query.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.6/ftmq/util.py` & `ftmq-0.2.0/ftmq/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,12 @@
-from enum import Enum
-from typing import Any, Generator, Iterable
+from typing import Generator
 
 from nomenklatura.dataset import DataCatalog, Dataset
 
 
-def StrEnum(name: str, values: Iterable[Any]) -> Enum:
-    # mimic py3.11 enum.StrEnum
-    class _StrEnum(str, Enum):
-        def __str__(self):
-            return self.value
-
-    return _StrEnum(name, {str(v): str(v) for v in values})
-
-
 def make_dataset(name: str) -> Dataset:
     catalog = DataCatalog(
         Dataset, {"datasets": [{"name": name, "title": name.title()}]}
     )
     return catalog.get(name)
```

### Comparing `ftmq-0.1.6/pyproject.toml` & `ftmq-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftmq"
-version = "0.1.6"
+version = "0.2.0"
 description = "followthemoney query dsl and io helpers"
 authors = ["Simon Wörpel <simon.woerpel@pm.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/investigativedata/ftmq"
 repository = "https://github.com/investigativedata/ftmq"
 documentation = "https://github.com/investigativedata/ftmq"
@@ -27,31 +27,34 @@
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 banal = "^1.0.6"
 followthemoney = "^3.4.0"
 nomenklatura = "2.14.1"
 orjson = "^3.9.1"
 PyICU = "^2.11"
-smart-open = {version = "6.3.0", extras = ["all"]}
 click = "^8.1.3"
 click-default-group = "^1.2.2"
 cryptography = ">=41.0.2"
 certifi = ">=2023.07.22"
 scipy = ">=1.10.0"
+pydantic = "<2"
+fsspec = "^2023.6.0"
+s3fs = "^2023.6.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
 pre-commit = "^3.3.3"
 flake8 = "^6.0.0"
 moto = "^4.1.11"
 ipdb = "^0.13.13"
 bump2version = "^1.0.1"
 cloudpickle = "^2.2.1"
+absolufy-imports = "^0.3.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ftmq-0.1.6/PKG-INFO` & `ftmq-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftmq
-Version: 0.1.6
+Version: 0.2.0
 Summary: followthemoney query dsl and io helpers
 Home-page: https://github.com/investigativedata/ftmq
 License: MIT
 Author: Simon Wörpel
 Author-email: simon.woerpel@pm.me
 Requires-Python: >=3.10,<3.13
 Classifier: Intended Audience :: Developers
@@ -17,18 +17,20 @@
 Requires-Dist: PyICU (>=2.11,<3.0)
 Requires-Dist: banal (>=1.0.6,<2.0.0)
 Requires-Dist: certifi (>=2023.07.22)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: cryptography (>=41.0.2)
 Requires-Dist: followthemoney (>=3.4.0,<4.0.0)
+Requires-Dist: fsspec (>=2023.6.0,<2024.0.0)
 Requires-Dist: nomenklatura (==2.14.1)
 Requires-Dist: orjson (>=3.9.1,<4.0.0)
+Requires-Dist: pydantic (<2)
+Requires-Dist: s3fs (>=2023.6.0,<2024.0.0)
 Requires-Dist: scipy (>=1.10.0)
-Requires-Dist: smart-open[all] (==6.3.0)
 Project-URL: Bug Tracker, https://github.com/investigativedata/ftmq/issues
 Project-URL: Documentation, https://github.com/investigativedata/ftmq
 Project-URL: Repository, https://github.com/investigativedata/ftmq
 Description-Content-Type: text/markdown
 
 [![ftmq on pypi](https://img.shields.io/pypi/v/ftmq)](https://pypi.org/project/ftmq/) [![Python test and package](https://github.com/investigativedata/ftmq/actions/workflows/python.yml/badge.svg)](https://github.com/investigativedata/ftmq/actions/workflows/python.yml) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit) [![Coverage Status](https://coveralls.io/repos/github/investigativedata/ftmq/badge.svg?branch=main)](https://coveralls.io/github/investigativedata/ftmq?branch=main) [![MIT License](https://img.shields.io/pypi/l/ftmq)](./LICENSE)
 
@@ -116,14 +118,43 @@
 
     ftmq apply -i ./entities.ftm.json -d <aditional_dataset>
 
 Overwrite datasets:
 
     ftmq apply -i ./entities.ftm.json -d <aditional_dataset> --replace-dataset
 
+### Coverage / Statistics
+
+Often in ftm scripting, we are iterating through all the proxies (e.g. during aggregation). Why not use this to collect statistics on the way? There is a context manager for this, which turns into the `Coverage` model:
+
+Print coverage to stdout (and filtered entities to nowhere):
+
+    cat entities.ftm.json | ftmq -s Event -o /dev/null --coverage-uri -
+
+Within code:
+
+```python
+from ftmq.coverage import Coverage
+
+fragments = [...]
+buffer = {}
+
+coverage = Coverage({"frequency": "unknown"})
+with coverage as cx:
+    for proxy in fragments:
+        if proxy.id in buffer:
+            buffer[proxy.id].merge(proxy)
+        else:
+            buffer[proxy.id] = proxy
+            # here collect stats:
+            cx.collect(proxy)
+
+stats = coverage.dict()
+```
+
 ### ftmstore (database read)
 
 **NOT IMPLEMENTED YET**
 
 The same cli logic applies:
 
     ftmq store iterate -d ec_meetings -s Event --date__gte=2019 --date__lte=2020
```

