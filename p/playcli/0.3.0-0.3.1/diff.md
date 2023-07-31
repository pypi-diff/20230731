# Comparing `tmp/playcli-0.3.0.tar.gz` & `tmp/playcli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playcli-0.3.0.tar", max compression
+gzip compressed data, was "playcli-0.3.1.tar", max compression
```

## Comparing `playcli-0.3.0.tar` & `playcli-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      393 2023-07-20 02:13:32.281361 playcli-0.3.0/README.md
--rw-r--r--   0        0        0      118 2023-07-18 04:16:35.684649 playcli-0.3.0/playcli/__init__.py
--rw-r--r--   0        0        0       38 2023-07-18 00:53:27.591450 playcli-0.3.0/playcli/__main__.py
--rw-r--r--   0        0        0      842 2023-07-20 02:13:32.281361 playcli-0.3.0/playcli/cli.py
--rw-r--r--   0        0        0        0 2023-07-18 00:53:27.591450 playcli-0.3.0/playcli/core/__init__.py
--rw-r--r--   0        0        0      174 2023-07-20 02:13:32.281361 playcli-0.3.0/playcli/core/commands/__init__.py
--rw-r--r--   0        0        0      186 2023-07-18 00:53:27.591450 playcli-0.3.0/playcli/core/commands/credits.py
--rw-r--r--   0        0        0      324 2023-07-20 02:13:32.281361 playcli-0.3.0/playcli/core/commands/download.py
--rw-r--r--   0        0        0     1290 2023-07-19 22:43:25.460839 playcli-0.3.0/playcli/core/commands/search.py
--rw-r--r--   0        0        0      116 2023-07-18 03:54:06.313154 playcli-0.3.0/playcli/core/platforms/__init__.py
--rw-r--r--   0        0        0     1364 2023-07-20 02:13:32.281361 playcli-0.3.0/playcli/core/platforms/elamigos.py
--rw-r--r--   0        0        0     1350 2023-07-20 02:13:32.281361 playcli-0.3.0/playcli/core/platforms/steamunlocked.py
--rw-r--r--   0        0        0      574 2023-07-20 02:13:32.282362 playcli-0.3.0/playcli/core/web.py
--rw-r--r--   0        0        0      107 2023-07-18 00:53:27.591450 playcli-0.3.0/playcli/main.py
--rw-r--r--   0        0        0      106 2023-07-20 02:13:32.282362 playcli-0.3.0/playcli/models/__init__.py
--rw-r--r--   0        0        0      501 2023-07-20 02:13:32.282362 playcli-0.3.0/playcli/models/driver.py
--rw-r--r--   0        0        0      961 2023-07-20 02:13:32.282362 playcli-0.3.0/playcli/models/platforms.py
--rw-r--r--   0        0        0     1092 2023-07-20 02:13:32.282362 playcli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 playcli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      123 2023-07-31 00:25:29.140911 playcli-0.3.1/playcli/__init__.py
+-rw-r--r--   0        0        0       41 2023-07-31 00:25:29.141912 playcli-0.3.1/playcli/__main__.py
+-rw-r--r--   0        0        0      877 2023-07-31 01:01:41.214774 playcli-0.3.1/playcli/cli.py
+-rw-r--r--   0        0        0        0 2023-07-31 00:25:29.142918 playcli-0.3.1/playcli/core/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-31 00:25:29.142918 playcli-0.3.1/playcli/core/commands/__init__.py
+-rw-r--r--   0        0        0      194 2023-07-31 01:09:24.630696 playcli-0.3.1/playcli/core/commands/credits.py
+-rw-r--r--   0        0        0      423 2023-07-31 01:09:22.911795 playcli-0.3.1/playcli/core/commands/download.py
+-rw-r--r--   0        0        0     1330 2023-07-31 00:25:29.143917 playcli-0.3.1/playcli/core/commands/search.py
+-rw-r--r--   0        0        0      118 2023-07-31 00:25:29.144917 playcli-0.3.1/playcli/core/platforms/__init__.py
+-rw-r--r--   0        0        0     1531 2023-07-31 01:09:56.271089 playcli-0.3.1/playcli/core/platforms/elamigos.py
+-rw-r--r--   0        0        0     1507 2023-07-31 01:11:31.145198 playcli-0.3.1/playcli/core/platforms/steamunlocked.py
+-rw-r--r--   0        0        0      595 2023-07-31 00:25:29.145916 playcli-0.3.1/playcli/core/web.py
+-rw-r--r--   0        0        0      116 2023-07-31 00:25:29.145916 playcli-0.3.1/playcli/main.py
+-rw-r--r--   0        0        0      122 2023-07-31 00:57:42.288924 playcli-0.3.1/playcli/models/__init__.py
+-rw-r--r--   0        0        0      709 2023-07-31 01:06:59.711490 playcli-0.3.1/playcli/models/driver.py
+-rw-r--r--   0        0        0      996 2023-07-31 01:08:48.039413 playcli-0.3.1/playcli/models/platforms.py
+-rw-r--r--   0        0        0     1140 2023-07-31 01:11:55.286224 playcli-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      417 2023-07-31 00:25:29.140911 playcli-0.3.1/README.md
+-rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 playcli-0.3.1/PKG-INFO
```

### Comparing `playcli-0.3.0/playcli/cli.py` & `playcli-0.3.1/playcli/cli.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from typing import Annotated
-
-from rich import print
-from typer import Exit, Option, Typer
-
-from playcli.core import commands as c
-from playcli.models.platforms import Platforms
-
-app: Typer = Typer(help="Download games with ease")
-
-
-@app.command(help="Code repository")
-def credits() -> None:
-    c.credits()
-
-
-@app.command(help="Search for games on multiple platforms")
-def search(
-    title: list[str],
-    page: Annotated[int, Option("--page", "-p", min=1)] = 1,
-    platform: Annotated[Platforms, Option()] = Platforms.RECURSIVE,
-) -> None:
-    c.search(" ".join(title), page, platform)
-
-
-@app.command(help="Game download links")
-def download(id: str) -> None:
-    f_ = Platforms.ALL.find(id)
-
-    if not f_:
-        print("[red]This id is invalid, or does not have a registered platform.[/]")
-
-        raise Exit(1)
-
-    c.download(*f_)
+from typing import Annotated
+
+from rich import print
+from typer import Exit, Option, Typer
+
+from playcli.core import commands as c
+from playcli.models.platforms import Platforms
+
+app: Typer = Typer(help="Download games with ease")
+
+
+@app.command(help="Code repository")
+def credits() -> None:
+    c.credits()
+
+
+@app.command(help="Search for games on multiple platforms")
+def search(
+    title: list[str],
+    page: Annotated[int, Option("--page", "-p", min=1)] = 1,
+    platform: Annotated[Platforms, Option()] = Platforms.RECURSIVE,
+) -> None:
+    c.search(" ".join(title), page, platform)
+
+
+@app.command(help="Game download links")
+def download(id: str) -> None:
+    f_ = Platforms.ALL.find(id)
+
+    if not f_:
+        print("[red]This id is invalid, or does not have a registered platform.[/]")
+
+        raise Exit(1)
+
+    c.download(*f_)
```

### Comparing `playcli-0.3.0/playcli/core/platforms/steamunlocked.py` & `playcli-0.3.1/playcli/core/platforms/steamunlocked.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-from bs4 import BeautifulSoup
-from typer import Exit
-
-from playcli.core.web import scrap
-from playcli.models.driver import Driver, GameSearch, Link
-
-
-class Steamunlocked(Driver):
-    url: str = "https://steamunlocked.net/"
-
-    E: dict[str, dict] = {
-        "game": {"link": ".btn-download"},
-        "search": {"card": ".cover-item-title > a"},
-    }
-
-    def download(self, id: str) -> list[Link]:
-        E: dict[str, str] = self.E["game"]
-
-        try:
-            parse: BeautifulSoup = scrap(self.url, [id], ex=False)
-
-            link: Link = Link(
-                target="DOWNLOAD", url=parse.select_one(E["link"])["href"]  # type: ignore
-            )
-
-            return [link]
-        except Exit:
-            return []
-
-    def search(self, q: str, page: int) -> list[GameSearch]:
-        E: dict[str, str] = self.E["search"]
-        parse: BeautifulSoup = scrap(self.url, ["page", str(page)], {"s": q})
-
-        rs: list[GameSearch] = []
-
-        for el in parse.select(E["card"]):
-            id: str = el["href"]  # type: ignore
-
-            title: str = el.text.replace("Free Download", "")
-
-            for x in [self.url, "-free-download", "/"]:
-                id = id.replace(x, "")
-
-            rs.append(
-                GameSearch(id=id, title=title.strip(), platform=self.__class__.__name__)
-            )
-
-        return rs
+from bs4 import BeautifulSoup
+from typer import Exit
+
+from playcli.core.web import scrap
+from playcli.models.driver import Driver, GameSearch, GameDownload, Link
+
+
+class Steamunlocked(Driver):
+    url: str = "https://steamunlocked.net/"
+
+    E: dict[str, dict] = {
+        "game": {"link": ".btn-download"},
+        "search": {"card": ".cover-item-title > a"},
+    }
+
+    def download(self, id_: str) -> GameDownload:
+        eh: dict[str, str] = self.E["game"]
+
+        try:
+            target: str = self.url + id_
+
+            parse: BeautifulSoup = scrap(target, ex=False)
+
+            link: Link = Link(
+                target="DOWNLOAD", url=parse.select_one(eh["link"])["href"]  # type: ignore
+            )
+
+            return GameDownload(target=target, links=[link])
+        except Exit:
+            return GameDownload()
+
+    def search(self, q: str, page: int) -> list[GameSearch]:
+        eh: dict[str, str] = self.E["search"]
+
+        parse: BeautifulSoup = scrap(self.url, ["page", str(page)], {"s": q})
+        rs: list[GameSearch] = []
+
+        for el in parse.select(eh["card"]):
+            id_: str = el["href"]  # type: ignore
+
+            title: str = el.text.replace("Free Download", "")
+
+            for x in [self.url, "-free-download", "/"]:
+                id_ = id_.replace(x, "")
+
+            rs.append(
+                GameSearch(id_=id_, title=title.strip(), platform=self.__class__.__name__)
+            )
+
+        return rs
```

### Comparing `playcli-0.3.0/playcli/core/web.py` & `playcli-0.3.1/playcli/core/web.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from bs4 import BeautifulSoup
-from requests import Response
-from requests import get as requests_get
-from rich import print
-from typer import Exit
-
-
-def scrap(
-    url: str, router: list[str] = [], params: dict = {}, ex: bool = True
-) -> BeautifulSoup:
-    res: Response = requests_get(url + "/".join(router), params=params)
-
-    if res.status_code != 200:
-        if ex:
-            print(
-                "[red]An error occurred while trying to communicate with the service.[/]"
-            )
-
-        raise Exit(code=1)
-
-    return BeautifulSoup(res.text, "html.parser")
+from bs4 import BeautifulSoup
+from requests import Response
+from requests import get as requests_get
+from rich import print
+from typer import Exit
+
+
+def scrap(
+    url: str, router: list[str] = [], params: dict = {}, ex: bool = True
+) -> BeautifulSoup:
+    res: Response = requests_get(url + "/".join(router), params=params)
+
+    if res.status_code != 200:
+        if ex:
+            print(
+                "[red]An error occurred while trying to communicate with the service.[/]"
+            )
+
+        raise Exit(code=1)
+
+    return BeautifulSoup(res.text, "html.parser")
```

### Comparing `playcli-0.3.0/playcli/models/platforms.py` & `playcli-0.3.1/playcli/models/platforms.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from enum import Enum
-
-from playcli.core import platforms as P
-from playcli.models.driver import Driver
-
-
-class Platforms(str, Enum):
-    ALL = "all"
-    RECURSIVE = "recursive"
-    ELAMIGOS = "elamigos"
-    STEAMUNLOCKED = "steamunlocked"
-
-    def __iter__(self):
-        for x in self.__class__._member_names_:
-            if x in ["ALL", "RECURSIVE"]:
-                continue
-
-            yield self.dv(x)
-
-    def find(self, id: str) -> tuple[str, Driver] | None:
-        for driver in self.__iter__():
-            platform: str = "-" + driver.__class__.__name__.lower()
-
-            if id.endswith(platform):
-                id_ = len(id) - len(platform)
-
-                return (id[:id_], driver)
-
-        return None
-
-    def dv(self, ps: str = "") -> Driver:
-        try:
-            return getattr(P, ps.capitalize() if ps else self.value.capitalize())()
-        except AttributeError:
-            raise Exception(f"The '{self.value}' has no driver")
+from enum import Enum
+
+from playcli.core import platforms as P
+from playcli.models.driver import Driver
+
+
+class Platforms(str, Enum):
+    ALL = "all"
+    RECURSIVE = "recursive"
+    ELAMIGOS = "elamigos"
+    STEAMUNLOCKED = "steamunlocked"
+
+    def __iter__(self):
+        for x in self.__class__._member_names_:
+            if x in ["ALL", "RECURSIVE"]:
+                continue
+
+            yield self.dv(x)
+
+    def find(self, id_: str) -> tuple[str, Driver] | None:
+        for driver in self.__iter__():
+            platform: str = "-" + driver.__class__.__name__.lower()
+
+            if id_.endswith(platform):
+                i_ = len(id_) - len(platform)
+
+                return id_[:i_], driver
+
+        return None
+
+    def dv(self, ps: str = "") -> Driver:
+        try:
+            return getattr(P, ps.capitalize() if ps else self.value.capitalize())()
+        except AttributeError:
+            raise Exception(f"The '{self.value}' has no driver")
```

### Comparing `playcli-0.3.0/pyproject.toml` & `playcli-0.3.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-[tool.poetry]
-name = "playcli"
-version = "0.3.0"
-description = "Browse and search games with ease"
-authors = ["Alekyo4 <alexsandergomes4742@gmail.com>"]
-license = "BeerWare"
-readme = "README.md"
-
-classifiers = [
-    "Natural Language :: Portuguese (Brazilian)",
-    "Environment :: Console",
-    "Intended Audience :: Customer Service",
-    "Programming Language :: Python :: 3",
-    "Topic :: Games/Entertainment"
-]
-
-[tool.poetry.urls]
-documentation = "https://github.com/alekyo4/playcli"
-code = "https://github.com/alekyo4/playcli"
-bug = "https://github.com/alekyo4/playcli/issues"
-
-[tool.poetry.scripts]
-playcli = "playcli.main:main"
-
-[tool.taskipy.tasks]
-format = "black . && isort ."
-test = "pytest"
-
-[tool.isort]
-profile = "black"
-line_length = 79
-
-[tool.poetry.dependencies]
-python = "^3.11"
-typer = {extras = ["all"], version = "^0.9.0"}
-beautifulsoup4 = "^4.12.2"
-requests = "^2.31.0"
-
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.4.0"
-black = "^23.7.0"
-isort = "^5.12.0"
-taskipy = "^1.11.0"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "playcli"
+version = "0.3.1"
+description = "Browse and search games with ease"
+authors = ["Alekyo4 <alexsandergomes4742@gmail.com>"]
+license = "BeerWare"
+readme = "README.md"
+
+classifiers = [
+    "Natural Language :: Portuguese (Brazilian)",
+    "Environment :: Console",
+    "Intended Audience :: Customer Service",
+    "Programming Language :: Python :: 3",
+    "Topic :: Games/Entertainment"
+]
+
+[tool.poetry.urls]
+documentation = "https://github.com/alekyo4/playcli"
+code = "https://github.com/alekyo4/playcli"
+bug = "https://github.com/alekyo4/playcli/issues"
+
+[tool.poetry.scripts]
+playcli = "playcli.main:main"
+
+[tool.taskipy.tasks]
+format = "black . && isort ."
+test = "pytest"
+
+[tool.isort]
+profile = "black"
+line_length = 79
+
+[tool.poetry.dependencies]
+python = "^3.11"
+typer = {extras = ["all"], version = "^0.9.0"}
+beautifulsoup4 = "^4.12.2"
+requests = "^2.31.0"
+
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
+black = "^23.7.0"
+isort = "^5.12.0"
+taskipy = "^1.11.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `playcli-0.3.0/PKG-INFO` & `playcli-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playcli
-Version: 0.3.0
+Version: 0.3.1
 Summary: Browse and search games with ease
 License: Beerware
 Author: Alekyo4
 Author-email: alexsandergomes4742@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Customer Service
```

