# Comparing `tmp/investigraph-0.3.0.tar.gz` & `tmp/investigraph-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investigraph-0.3.0.tar", max compression
+gzip compressed data, was "investigraph-0.3.1.tar", max compression
```

## Comparing `investigraph-0.3.0.tar` & `investigraph-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,28 @@
--rw-r--r--   0        0        0     1077 2023-05-31 13:25:47.750897 investigraph-0.3.0/LICENSE
--rw-r--r--   0        0        0     3633 2023-07-19 19:26:21.972231 investigraph-0.3.0/README.md
--rw-r--r--   0        0        0      228 2023-07-28 15:45:34.272516 investigraph-0.3.0/investigraph/__init__.py
--rw-r--r--   0        0        0     2225 2023-07-28 05:54:17.625205 investigraph-0.3.0/investigraph/cache.py
--rw-r--r--   0        0        0     4851 2023-07-28 18:13:46.585000 investigraph-0.3.0/investigraph/cli.py
--rw-r--r--   0        0        0       88 2023-06-14 09:53:12.989488 investigraph-0.3.0/investigraph/exceptions.py
--rw-r--r--   0        0        0     2418 2023-07-19 19:27:06.088877 investigraph-0.3.0/investigraph/inspect.py
--rw-r--r--   0        0        0        0 2023-06-14 09:53:12.989488 investigraph-0.3.0/investigraph/logic/__init__.py
--rw-r--r--   0        0        0     2373 2023-07-27 10:36:14.954671 investigraph-0.3.0/investigraph/logic/aggregate.py
--rw-r--r--   0        0        0     1380 2023-07-21 12:12:19.753244 investigraph-0.3.0/investigraph/logic/extract.py
--rw-r--r--   0        0        0     1731 2023-07-27 10:36:14.954671 investigraph-0.3.0/investigraph/logic/load.py
--rw-r--r--   0        0        0     1581 2023-07-26 18:56:04.099112 investigraph-0.3.0/investigraph/logic/requests.py
--rw-r--r--   0        0        0      759 2023-07-28 05:14:21.814503 investigraph-0.3.0/investigraph/logic/transform.py
--rw-r--r--   0        0        0      513 2023-07-28 15:45:19.824525 investigraph-0.3.0/investigraph/model/__init__.py
--rw-r--r--   0        0        0     3438 2023-07-28 05:08:46.387588 investigraph-0.3.0/investigraph/model/block.py
--rw-r--r--   0        0        0     2634 2023-07-28 15:41:17.176859 investigraph-0.3.0/investigraph/model/config.py
--rw-r--r--   0        0        0     3402 2023-07-28 06:38:23.841941 investigraph-0.3.0/investigraph/model/context.py
--rw-r--r--   0        0        0     4528 2023-07-28 18:18:16.765300 investigraph-0.3.0/investigraph/model/dataset.py
--rw-r--r--   0        0        0     2301 2023-07-28 06:38:23.841941 investigraph-0.3.0/investigraph/model/flow.py
--rw-r--r--   0        0        0     1319 2023-07-28 05:01:47.270488 investigraph-0.3.0/investigraph/model/mapping.py
--rw-r--r--   0        0        0     1620 2023-07-28 17:57:21.112182 investigraph-0.3.0/investigraph/model/mixins.py
--rw-r--r--   0        0        0     3589 2023-07-28 06:38:23.841941 investigraph-0.3.0/investigraph/model/resolver.py
--rw-r--r--   0        0        0     2238 2023-07-27 10:36:14.954671 investigraph-0.3.0/investigraph/model/source.py
--rw-r--r--   0        0        0     2494 2023-07-28 06:38:23.761940 investigraph-0.3.0/investigraph/model/stage.py
--rw-r--r--   0        0        0     4769 2023-07-28 05:17:15.986769 investigraph-0.3.0/investigraph/pipeline.py
--rw-r--r--   0        0        0     1387 2023-07-28 18:48:09.415365 investigraph-0.3.0/investigraph/settings.py
--rw-r--r--   0        0        0      570 2023-07-28 18:23:23.585653 investigraph-0.3.0/investigraph/types.py
--rw-r--r--   0        0        0     5066 2023-07-28 17:34:38.618717 investigraph-0.3.0/investigraph/util.py
--rw-r--r--   0        0        0     1753 2023-07-28 18:48:09.415365 investigraph-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5564 1970-01-01 00:00:00.000000 investigraph-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 13:25:47.750897 investigraph-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3633 2023-07-19 19:26:21.972231 investigraph-0.3.1/README.md
+-rw-r--r--   0        0        0      228 2023-07-28 15:45:34.272516 investigraph-0.3.1/investigraph/__init__.py
+-rw-r--r--   0        0        0     2225 2023-07-28 05:54:17.625205 investigraph-0.3.1/investigraph/cache.py
+-rw-r--r--   0        0        0     4774 2023-07-31 13:02:58.874979 investigraph-0.3.1/investigraph/cli.py
+-rw-r--r--   0        0        0       88 2023-06-14 09:53:12.989488 investigraph-0.3.1/investigraph/exceptions.py
+-rw-r--r--   0        0        0     2418 2023-07-19 19:27:06.088877 investigraph-0.3.1/investigraph/inspect.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:53:12.989488 investigraph-0.3.1/investigraph/logic/__init__.py
+-rw-r--r--   0        0        0     3359 2023-07-31 12:14:28.200457 investigraph-0.3.1/investigraph/logic/aggregate.py
+-rw-r--r--   0        0        0     1380 2023-07-21 12:12:19.753244 investigraph-0.3.1/investigraph/logic/extract.py
+-rw-r--r--   0        0        0     1731 2023-07-29 10:22:50.721817 investigraph-0.3.1/investigraph/logic/load.py
+-rw-r--r--   0        0        0     1581 2023-07-26 18:56:04.099112 investigraph-0.3.1/investigraph/logic/requests.py
+-rw-r--r--   0        0        0      759 2023-07-28 05:14:21.814503 investigraph-0.3.1/investigraph/logic/transform.py
+-rw-r--r--   0        0        0      498 2023-07-31 12:14:28.200457 investigraph-0.3.1/investigraph/model/__init__.py
+-rw-r--r--   0        0        0     3438 2023-07-28 05:08:46.387588 investigraph-0.3.1/investigraph/model/block.py
+-rw-r--r--   0        0        0     2939 2023-07-31 12:14:28.200457 investigraph-0.3.1/investigraph/model/config.py
+-rw-r--r--   0        0        0     2985 2023-07-31 12:14:28.200457 investigraph-0.3.1/investigraph/model/context.py
+-rw-r--r--   0        0        0     3318 2023-07-31 12:14:28.200457 investigraph-0.3.1/investigraph/model/flow.py
+-rw-r--r--   0        0        0     1319 2023-07-28 05:01:47.270488 investigraph-0.3.1/investigraph/model/mapping.py
+-rw-r--r--   0        0        0     3600 2023-07-31 12:14:28.200457 investigraph-0.3.1/investigraph/model/resolver.py
+-rw-r--r--   0        0        0     2248 2023-07-31 12:15:22.783873 investigraph-0.3.1/investigraph/model/source.py
+-rw-r--r--   0        0        0     2139 2023-07-31 12:14:28.200457 investigraph-0.3.1/investigraph/model/stage.py
+-rw-r--r--   0        0        0     5095 2023-07-31 12:14:28.200457 investigraph-0.3.1/investigraph/pipeline.py
+-rw-r--r--   0        0        0     1674 2023-07-31 13:13:12.748151 investigraph-0.3.1/investigraph/settings.py
+-rw-r--r--   0        0        0      564 2023-07-31 12:14:28.200457 investigraph-0.3.1/investigraph/types.py
+-rw-r--r--   0        0        0     5066 2023-07-28 17:34:38.618717 investigraph-0.3.1/investigraph/util.py
+-rw-r--r--   0        0        0     1701 2023-07-31 13:13:12.748151 investigraph-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5516 1970-01-01 00:00:00.000000 investigraph-0.3.1/PKG-INFO
```

### Comparing `investigraph-0.3.0/LICENSE` & `investigraph-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `investigraph-0.3.0/README.md` & `investigraph-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `investigraph-0.3.0/investigraph/cache.py` & `investigraph-0.3.1/investigraph/cache.py`

 * *Files identical despite different names*

### Comparing `investigraph-0.3.0/investigraph/cli.py` & `investigraph-0.3.1/investigraph/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import shutil
 import sys
 from pathlib import Path
-from typing import Optional
+from typing import Annotated, Optional
 
 import orjson
 import typer
+from ftmq.io import smart_write
+from ftmq.model import Catalog
 from prefect.settings import PREFECT_HOME
 from rich import print
-from smart_open import open
-from typing_extensions import Annotated
 
 from investigraph.inspect import inspect_config, inspect_extract, inspect_transform
 from investigraph.model.block import get_block
-from investigraph.model.dataset import Catalog
 from investigraph.model.flow import FlowOptions
 from investigraph.pipeline import run
 from investigraph.settings import DATASETS_BLOCK, DATASETS_REPO
 
 cli = typer.Typer()
 
 
@@ -113,15 +112,15 @@
 def cli_catalog(
     path: Annotated[Path, typer.Argument()],
     uri: Annotated[str, typer.Option("-o")] = "-",
     flatten: Annotated[Optional[bool], typer.Option(...)] = False,
 ):
     """
     Build a catalog from datasets metadata and write it to anywhere from stdout
-    (default) to any uri `smart_open` can handle, e.g.:
+    (default) to any uri `fsspec` can handle, e.g.:
 
         investigraph build-catalog catalog.yml -u s3://mybucket/catalog.json
     """
     catalog = Catalog.from_path(path)
     if uri != "-":
         catalog.uri = uri
     if flatten:
@@ -132,16 +131,15 @@
         }
     else:
         data = catalog.dict()
     data = orjson.dumps(data, option=orjson.OPT_APPEND_NEWLINE)
     if uri == "-":
         sys.stdout.write(data.decode())
     else:
-        with open(uri, "wb") as fh:
-            fh.write(data)
+        smart_write(uri, data)
 
 
 @cli.command("reset")
 def cli_reset(yes: Annotated[str, typer.Option(prompt="Are you sure? [yes/no]")]):
     """
     Reset all prefect data in `PREFECT_HOME`
     """
```

### Comparing `investigraph-0.3.0/investigraph/inspect.py` & `investigraph-0.3.1/investigraph/inspect.py`

 * *Files identical despite different names*

### Comparing `investigraph-0.3.0/investigraph/logic/extract.py` & `investigraph-0.3.1/investigraph/logic/extract.py`

 * *Files identical despite different names*

### Comparing `investigraph-0.3.0/investigraph/logic/load.py` & `investigraph-0.3.1/investigraph/logic/load.py`

 * *Files identical despite different names*

### Comparing `investigraph-0.3.0/investigraph/logic/requests.py` & `investigraph-0.3.1/investigraph/logic/requests.py`

 * *Files identical despite different names*

### Comparing `investigraph-0.3.0/investigraph/logic/transform.py` & `investigraph-0.3.1/investigraph/logic/transform.py`

 * *Files identical despite different names*

### Comparing `investigraph-0.3.0/investigraph/model/block.py` & `investigraph-0.3.1/investigraph/model/block.py`

 * *Files identical despite different names*

### Comparing `investigraph-0.3.0/investigraph/model/config.py` & `investigraph-0.3.1/investigraph/model/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 import logging
 from pathlib import Path
 
 import yaml
+from ftmq.model import Dataset
+from ftmq.model.mixins import RemoteMixin, YamlMixin
 from pydantic import BaseModel
 from runpandarun.util import absolute_path
 
 from investigraph.exceptions import ImproperlyConfigured
 from investigraph.model.block import get_block
-from investigraph.model.dataset import Dataset
-from investigraph.model.mixins import RemoteMixin, YamlMixin
-from investigraph.model.stage import ExtractStage, LoadStage, TransformStage
+from investigraph.model.stage import (
+    AggregateStage,
+    ExtractStage,
+    LoadStage,
+    TransformStage,
+)
 from investigraph.settings import DATASETS_BLOCK
 from investigraph.util import PathLike, is_module
 
 log = logging.getLogger(__name__)
 
 
 class Config(BaseModel, YamlMixin, RemoteMixin):
     dataset: Dataset
     base_path: Path | None = Path()
     extract: ExtractStage | None = ExtractStage()
     transform: TransformStage | None = TransformStage()
     load: LoadStage | None = LoadStage()
+    aggregate: bool | AggregateStage | None = AggregateStage()
 
     class Config:
         arbitrary_types_allowed = True
 
     def __init__(self, **data):
         if "dataset" not in data:
             data["dataset"] = data
@@ -50,14 +56,19 @@
             config.transform.handler = str(
                 absolute_path(config.transform.handler, config.base_path)
             )
         if not is_module(config.load.handler):
             config.load.handler = str(
                 absolute_path(config.load.handler, config.base_path)
             )
+        if config.aggregate:
+            if not is_module(config.aggregate.handler):
+                config.aggregate.handler = str(
+                    absolute_path(config.aggregate.handler, config.base_path)
+                )
 
         return config
 
 
 def get_config(
     dataset: str | None = None, block: str | None = None, path: PathLike | None = None
 ) -> Config:
```

### Comparing `investigraph-0.3.0/investigraph/model/context.py` & `investigraph-0.3.1/investigraph/model/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 from datetime import datetime
 from typing import Iterable
 
 import orjson
 from followthemoney.util import make_entity_id
+from ftmq.io import smart_write
 from nomenklatura.entity import CE
-from nomenklatura.util import datetime_iso
 from prefect import get_run_logger
 from prefect.logging.loggers import PrefectLogAdapter
 from pydantic import BaseModel
-from smart_open import open
 
 from investigraph.cache import Cache, get_cache
+from investigraph.logic.aggregate import AggregatorResult
 from investigraph.model.config import Config
 from investigraph.model.source import Source
-from investigraph.settings import DATA_ROOT
 from investigraph.types import CEGenerator
-from investigraph.util import ensure_path, join_slug, make_proxy
+from investigraph.util import join_slug, make_proxy
 
 
 class Context(BaseModel):
     dataset: str
     prefix: str
     config: Config
     source: Source
 
-    class Config:
-        arbitrary_types_allowed = True
-
     def __hash__(self) -> int:
-        return hash((self.dataset, self.source.uri))
+        return hash(repr(self.dict()))
 
     @property
     def cache(self) -> Cache:
         return get_cache()
 
     @property
     def log(self) -> PrefectLogAdapter:
@@ -44,20 +40,22 @@
         return self.config.load.handle(self, *args, **kwargs)
 
     def load_entities(self, *args, **kwargs) -> str:
         kwargs["uri"] = kwargs.pop("uri", self.config.load.entities_uri)
         kwargs["parts"] = False
         return self.config.load.handle(self, *args, **kwargs)
 
+    def aggregate(self, *args, **kwargs) -> AggregatorResult:
+        return self.config.aggregate.handle(*args, **kwargs)
+
     def export_metadata(self) -> None:
         data = self.config.dataset
-        data.updated_at = data.updated_at or datetime_iso(datetime.utcnow())
+        data.updated_at = data.updated_at or datetime.utcnow()
         data = orjson.dumps(data.dict())
-        with open(self.config.load.index_uri, "wb") as fh:
-            fh.write(data)
+        smart_write(self.config.load.index_uri, data)
 
     def make_proxy(self, *args, **kwargs) -> CE:
         return make_proxy(*args, dataset=self.dataset, **kwargs)
 
     def make(self, *args, **kwargs) -> CE:
         # align with zavod api for easy migration
         return self.make_proxy(*args, **kwargs)
@@ -88,21 +86,13 @@
 
     def emit(self, proxy: CE) -> None:
         # mimic zavod
         self.proxies.append(proxy)
 
 
 def init_context(config: Config, source: Source) -> Context:
-    path = ensure_path(DATA_ROOT / config.dataset.name)
-    if config.load.index_uri is None:
-        config.load.index_uri = (path / "index.json").as_uri()
-    if config.load.fragments_uri is None:
-        config.load.fragments_uri = (path / "fragments.json").as_uri()
-    if config.load.entities_uri is None:
-        config.load.entities_uri = (path / "entities.ftm.json").as_uri()
-
     return Context(
         dataset=config.dataset.name,
         prefix=config.dataset.prefix,
         config=config,
         source=source,
     )
```

### Comparing `investigraph-0.3.0/investigraph/model/mapping.py` & `investigraph-0.3.1/investigraph/model/mapping.py`

 * *Files identical despite different names*

### Comparing `investigraph-0.3.0/investigraph/model/resolver.py` & `investigraph-0.3.1/investigraph/model/resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 resolver for `.source.Source`
 """
 
 from io import BytesIO
 
+from ftmq.io import smart_open as open
 from normality import slugify
 from pantomime import types
 from pydantic import BaseModel
-from smart_open import open
 
 from investigraph.exceptions import ImproperlyConfigured
 from investigraph.logic import requests
 from investigraph.model.source import Source, SourceHead
 from investigraph.types import BytesGenerator
 from investigraph.util import checksum
```

### Comparing `investigraph-0.3.0/investigraph/model/source.py` & `investigraph-0.3.1/investigraph/model/source.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import mimetypes
 from datetime import datetime
+from urllib.parse import urlparse
 
 import requests
 from dateparser import parse as parse_date
 from normality import slugify
 from pantomime import normalize_mimetype, types
 from pydantic import BaseModel
 from runpandarun import Playbook
 from runpandarun.util import PathLike, absolute_path
-from smart_open import parse_uri
 
 from investigraph.util import slugified_dict
 
 
 class SourceHead(BaseModel):
     etag: str | None = None
     last_modified: datetime | None = None
@@ -40,15 +40,15 @@
     mimetype: str | None = None
     pandas: Playbook | None = Playbook()
     stream: bool | None = None
 
     def __init__(self, **data):
         data["uri"] = str(data["uri"])
         data["name"] = data.get("name", slugify(data["uri"]))
-        data["scheme"] = data.get("scheme", parse_uri(data["uri"]).scheme)
+        data["scheme"] = data.get("scheme", urlparse(data["uri"]).scheme or "file")
         if "mimetype" not in data:
             mtype, _ = mimetypes.guess_type(data["uri"])
             data["mimetype"] = normalize_mimetype(mtype)
         data["stream"] = data.get("stream", data["mimetype"] == types.CSV)
         super().__init__(**data)
 
     def ensure_uri(self, base: PathLike) -> None:
```

### Comparing `investigraph-0.3.0/investigraph/model/stage.py` & `investigraph-0.3.1/investigraph/model/stage.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from typing import TYPE_CHECKING, Callable
 
 from banal import ensure_list, keys_values
 from pydantic import BaseModel
 from runpandarun import Playbook
 
-from investigraph.logic.load import TProxies
 from investigraph.model.mapping import QueryMapping
 from investigraph.settings import (
     CHUNK_SIZE,
+    DEFAULT_AGGREGATOR,
     DEFAULT_EXTRACTOR,
     DEFAULT_LOADER,
     DEFAULT_TRANSFORMER,
+    FTM_STORE_URI,
 )
 from investigraph.types import TaskResult
 from investigraph.util import get_func, pydantic_merge
 
 if TYPE_CHECKING:
     from investigraph.model.context import Context
 
@@ -32,15 +33,15 @@
         super().__init__(**data)
 
     def get_handler(self) -> Callable:
         return get_func(self.handler)
 
     def handle(self, ctx: "Context", *args, **kwargs) -> TaskResult:
         handler = self.get_handler()
-        yield from handler(ctx, *args, **kwargs)
+        return handler(ctx, *args, **kwargs)
 
 
 class ExtractStage(Stage):
     _default_handler = DEFAULT_EXTRACTOR
 
     fetch: bool | None = True
     sources: list[Source] | None = []
@@ -64,23 +65,18 @@
 
 class LoadStage(Stage):
     _default_handler = DEFAULT_LOADER
 
     index_uri: str | None = None
     fragments_uri: str | None = None
     entities_uri: str | None = None
-    aggregate: bool | None = True
 
-    @property
-    def target(self) -> str:
-        if self.entities_uri is not None:
-            if self.entities_uri.startswith("postg"):
-                return "postgres"
-        return "json"
 
-    def handle(self, ctx: "Context", proxies: TProxies, *args, **kwargs) -> str:
-        handler = self.get_handler()
-        if self.target == "postgres":
-            # write directly to entities instead of fragments
-            # as aggregation is happening within postgres store on write
-            kwargs["uri"] = kwargs.pop("uri", self.entities_uri)
-        return handler(ctx, proxies, *args, **kwargs)
+class AggregateStage(Stage):
+    _default_handler = DEFAULT_AGGREGATOR
+
+    db_uri: str | None = FTM_STORE_URI
+
+    def __init__(self, **data):
+        if data.pop("handler", None) == "db":
+            data["handler"] = "investigraph.logic.aggregate.in_db"
+        super().__init__(**data)
```

### Comparing `investigraph-0.3.0/investigraph/pipeline.py` & `investigraph-0.3.1/investigraph/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 The main entrypoint for the prefect flow
 """
 
+from datetime import datetime
 from typing import Any, Generator
 
+from ftmq.model import Coverage
 from prefect import flow, task
 from prefect.task_runners import ConcurrentTaskRunner
 from prefect_dask import DaskTaskRunner
 from prefect_ray import RayTaskRunner
 
 from investigraph import __version__, settings
-from investigraph.logic.aggregate import in_memory
-from investigraph.model import Context, Flow, FlowOptions, Resolver
-from investigraph.model.context import init_context
+from investigraph.model.context import Context, init_context
+from investigraph.model.flow import Flow, FlowOptions
+from investigraph.model.resolver import Resolver
 from investigraph.util import data_checksum
 
 
 def get_runner_from_env() -> ConcurrentTaskRunner | DaskTaskRunner | RayTaskRunner:
     if settings.TASK_RUNNER == "dask":
         return DaskTaskRunner()
     if settings.TASK_RUNNER == "ray":
@@ -31,30 +33,29 @@
 @task(
     retries=settings.TASK_RETRIES,
     retry_delay_seconds=settings.TASK_RETRY_DELAY,
     cache_key_fn=get_task_cache_key,
     cache_expiration=settings.TASK_CACHE_EXPIRATION,
     refresh_cache=not settings.TASK_CACHE,
 )
-def aggregate(ctx: Context, results: list[str], ckey: str):
-    fragments, proxies = in_memory(ctx, *results)
-    ctx.log.info("AGGREGATED %d fragments to %d proxies", fragments, proxies)
-    out = ctx.config.load.entities_uri
-    ctx.log.info("OUTPUT: %s", out)
-    return out
+def aggregate(ctx: Context, results: list[str], ckey: str) -> Coverage:
+    fragments, coverage = ctx.aggregate(ctx, results)
+    ctx.log.info("AGGREGATED %d fragments to %d proxies", fragments, coverage.entities)
+    ctx.log.info("OUTPUT: %s", ctx.config.load.entities_uri)
+    return coverage
 
 
 @task(
     retries=settings.TASK_RETRIES,
     retry_delay_seconds=settings.TASK_RETRY_DELAY,
     cache_key_fn=get_task_cache_key,
     cache_expiration=settings.TASK_CACHE_EXPIRATION,
     refresh_cache=not settings.TASK_CACHE,
 )
-def load(ctx: Context, ckey: str):
+def load(ctx: Context, ckey: str) -> str:
     proxies = ctx.cache.get(ckey)
     out = ctx.load_fragments(proxies, ckey=ckey)
     ctx.log.info("LOADED %d proxies", len(proxies))
     ctx.log.info("OUTPUT: %s", out)
     return out
 
 
@@ -106,15 +107,15 @@
 
 @flow(
     name="investigraph-pipeline",
     version=__version__,
     flow_run_name="{ctx.dataset}-{ctx.source.name}",
     task_runner=get_runner_from_env(),
 )
-def run_pipeline(ctx: Context):
+def run_pipeline(ctx: Context) -> list[Any]:
     res = None
     if ctx.config.extract.fetch:
         res = Resolver(source=ctx.source)
         if res.source.is_http:
             res._resolve_http()
         ckey = res.get_cache_key()
     else:
@@ -131,25 +132,28 @@
 
 @flow(
     name="investigraph",
     version=__version__,
     flow_run_name="{options.flow_name}",
     task_runner=get_runner_from_env(),
 )
-def run(options: FlowOptions) -> str:
+def run(options: FlowOptions) -> Flow:
     flow = Flow.from_options(options)
     results = []
     for ix, source in enumerate(flow.config.extract.sources):
         ctx = init_context(config=flow.config, source=source)
         if ix == 0:  # only on first time
             ctx.export_metadata()
             ctx.log.info("INDEX: %s" % ctx.config.load.index_uri)
-        results.append(run_pipeline(ctx))
-
-    results = [r.result() for result in results for r in result]
+        results.extend(run_pipeline(ctx))
 
-    if flow.should_aggregate:
-        results = [aggregate(ctx, results, data_checksum(results))]
-
-    for uri in results:
-        ctx.log.info(f"LOADED proxies to `{uri}`")
-    return results
+    if flow.config.aggregate:
+        fragments = [r.result() for r in results]
+        res = aggregate.submit(ctx, fragments, data_checksum(fragments))
+        ctx.config.dataset.coverage = res.result()
+        ctx.export_metadata()
+        ctx.log.info("INDEX (updated with coverage): %s" % ctx.config.load.index_uri)
+
+    flow.end = datetime.utcnow()
+    fragment_uris = [r.result() for r in results]
+    flow.fragment_uris = filter(lambda x: x is not None, fragment_uris)
+    return flow
```

### Comparing `investigraph-0.3.0/investigraph/settings.py` & `investigraph-0.3.1/investigraph/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import os
-from datetime import datetime, timedelta
+from datetime import timedelta
 from pathlib import Path
 from typing import Any
 
 from banal import as_bool
+from ftmstore import settings as ftmstore_settings
+from prefect.settings import PREFECT_API_DATABASE_CONNECTION_URL
 
 
 def get_env(env: str, default: Any | None = None) -> Any | None:
     return os.environ.get(env, default)
 
 
-VERSION = "0.3.0"
-RUN_TIME = datetime.utcnow().replace(microsecond=0)
+VERSION = "0.3.1"
 
 DEBUG = as_bool(get_env("DEBUG", 1))
 DATA_ROOT = Path(get_env("DATA_ROOT", Path.cwd() / "data")).absolute()
 DATASETS_REPO = "https://github.com/investigativedata/investigraph-datasets.git"
 DATASETS_BLOCK = get_env("DATASETS_BLOCK")
 
 DEFAULT_EXTRACTOR = get_env("DEFAULT_EXTRACTOR", "investigraph.logic.extract:handle")
 DEFAULT_TRANSFORMER = get_env(
     "DEFAULT_TRANSFORMER", "investigraph.logic.transform:map_ftm"
 )
 DEFAULT_LOADER = get_env("DEFAULT_LOADER", "investigraph.logic.load:load_proxies")
+DEFAULT_AGGREGATOR = get_env(
+    "DEFAULT_AGGREGATOR", "investigraph.logic.aggregate:in_memory"
+)
 
 REDIS_URL = get_env("REDIS_URL", "redis://localhost:6379")
 REDIS_PREFIX = get_env("REDIS_PREFIX", f"investigraph:{VERSION}")
 
 TASK_CACHE = as_bool(get_env("TASK_CACHE", 1))
 TASK_RETRIES = int(get_env("TASK_RETRIES", 3))
 TASK_RETRY_DELAY = int(get_env("TASK_RETRY_DELAY", 5))
@@ -34,7 +38,10 @@
 TASK_CACHE_EXPIRATION = (
     timedelta(TASK_CACHE_EXPIRATION) if TASK_CACHE_EXPIRATION is not None else None
 )
 
 TASK_RUNNER = get_env("PREFECT_TASK_RUNNER", "").lower()
 
 CHUNK_SIZE = int(get_env("CHUNK_SIZE", 1000))
+
+FTM_STORE_URI = get_env("FTM_STORE_URI", PREFECT_API_DATABASE_CONNECTION_URL.value())
+ftmstore_settings.DATABASE_URI = FTM_STORE_URI
```

### Comparing `investigraph-0.3.0/investigraph/types.py` & `investigraph-0.3.1/investigraph/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Generator, TypeAlias
 
+from ftmq.types import PathLike
 from nomenklatura.entity import CE
-from runpandarun.util import PathLike
 
 # a string-keyed dict
 Record: TypeAlias = dict[str, Any]
 SDict: TypeAlias = Record  # FIXME backwards compatibility
 RecordGenerator: TypeAlias = Generator[Record, None, None]
 
 # composite entity generator
```

### Comparing `investigraph-0.3.0/investigraph/util.py` & `investigraph-0.3.1/investigraph/util.py`

 * *Files identical despite different names*

### Comparing `investigraph-0.3.0/pyproject.toml` & `investigraph-0.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "investigraph"
-version = "0.3.0"
+version = "0.3.1"
 description = "etl pipeline for investigations with follow the money data"
 authors = ["Simon Wörpel <simon@investigativedata.org>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://investigraph.dev"
 repository = "https://github.com/investigativedata/investigraph-etl"
 documentation = "https://docs.investigraph.dev"
@@ -35,30 +35,29 @@
 nomenklatura = "<3"
 pandas = "^2.0.3"
 pantomime = "^0.6.1"
 prefect = "^2.11.1"
 prefect-dask = "^0.2.4"
 redis = "^4.6.0"
 requests = "^2.31.0"
-smart-open = {extras = ["all"], version = "^6.3.0"}
 sqlalchemy = "^2.0.19"
 tabulate = "^0.9.0"
 typer = "^0.9.0"
-ftmq = ">=0.1.5"
+ftmq = ">=0.2.0"
 prefect-ray = "^0.2.5"
 ray = "^2.5.1"
 pydantic = "<2"
 runpandarun = ">=0.2.5"
 cryptography = ">=41.0.2"
 xlrd = "^2.0.1"
 normality = "^2.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest-env = "^0.8.2"
-moto = "4.1.13"
+moto = "4.1.14"
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
 pre-commit = "^3.3.3"
 flake8 = "^6.0.0"
```

### Comparing `investigraph-0.3.0/PKG-INFO` & `investigraph-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investigraph
-Version: 0.3.0
+Version: 0.3.1
 Summary: etl pipeline for investigations with follow the money data
 Home-page: https://investigraph.dev
 License: MIT
 Author: Simon Wörpel
 Author-email: simon@investigativedata.org
 Requires-Python: >=3.10,<3.13
 Classifier: Intended Audience :: Developers
@@ -17,29 +17,28 @@
 Requires-Dist: banal (>=1.0.6,<2.0.0)
 Requires-Dist: cachelib (>=0.10.2,<0.11.0)
 Requires-Dist: cryptography (>=41.0.2)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: fakeredis (>=2.17.0,<3.0.0)
 Requires-Dist: followthemoney (>=3.4.0,<4.0.0)
 Requires-Dist: followthemoney-store (>=3.0.5,<4.0.0)
-Requires-Dist: ftmq (>=0.1.5)
+Requires-Dist: ftmq (>=0.2.0)
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0)
 Requires-Dist: nomenklatura (<3)
 Requires-Dist: normality (>=2.4.0,<3.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pantomime (>=0.6.1,<0.7.0)
 Requires-Dist: prefect (>=2.11.1,<3.0.0)
 Requires-Dist: prefect-dask (>=0.2.4,<0.3.0)
 Requires-Dist: prefect-ray (>=0.2.5,<0.3.0)
 Requires-Dist: pydantic (<2)
 Requires-Dist: ray (>=2.5.1,<3.0.0)
 Requires-Dist: redis (>=4.6.0,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: runpandarun (>=0.2.5)
-Requires-Dist: smart-open[all] (>=6.3.0,<7.0.0)
 Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/investigativedata/investigraph-etl/issues
 Project-URL: Documentation, https://docs.investigraph.dev
 Project-URL: Repository, https://github.com/investigativedata/investigraph-etl
```

