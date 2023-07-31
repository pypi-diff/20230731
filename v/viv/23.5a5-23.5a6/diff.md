# Comparing `tmp/viv-23.5a5.tar.gz` & `tmp/viv-23.5a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viv-23.5a5.tar", last modified: Fri Jun  2 19:10:02 2023, max compression
+gzip compressed data, was "viv-23.5a6.tar", last modified: Mon Jul 31 16:47:45 2023, max compression
```

## Comparing `viv-23.5a5.tar` & `viv-23.5a6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2023-06-02 13:44:22.530182 viv-23.5a5/LICENSE
--rw-r--r--   0        0        0     3666 2023-06-02 19:09:37.319887 viv-23.5a5/README.md
--rw-r--r--   0        0        0      844 2023-06-02 13:44:22.533515 viv-23.5a5/pyproject.toml
--rw-r--r--   0        0        0       48 2023-06-02 13:44:22.533515 viv-23.5a5/src/viv/__init__.py
--rw-r--r--   0        0        0       61 2023-06-02 13:44:22.536848 viv-23.5a5/src/viv/__main__.py
--rwxr-xr-x   0        0        0    48724 2023-06-02 19:09:50.793343 viv-23.5a5/src/viv/viv.py
--rw-r--r--   0        0        0     3990 1970-01-01 00:00:00.000000 viv-23.5a5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-02 13:44:22.530182 viv-23.5a6/LICENSE
+-rw-r--r--   0        0        0     3666 2023-06-02 19:09:37.319887 viv-23.5a6/README.md
+-rw-r--r--   0        0        0      821 2023-06-02 21:56:40.027575 viv-23.5a6/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-06-02 13:44:22.533515 viv-23.5a6/src/viv/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-02 13:44:22.536848 viv-23.5a6/src/viv/__main__.py
+-rwxr-xr-x   0        0        0    55937 2023-07-31 16:42:47.061951 viv-23.5a6/src/viv/viv.py
+-rw-r--r--   0        0        0     3990 1970-01-01 00:00:00.000000 viv-23.5a6/PKG-INFO
```

### Comparing `viv-23.5a5/LICENSE` & `viv-23.5a6/LICENSE`

 * *Files identical despite different names*

### Comparing `viv-23.5a5/README.md` & `viv-23.5a6/README.md`

 * *Files identical despite different names*

### Comparing `viv-23.5a5/pyproject.toml` & `viv-23.5a6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 authors = [
     { name = "Daylin Morgan", email = "daylinmorgan@gmail.com" },
 ]
 dependencies = []
 requires-python = ">= 3.8"
 readme = "README.md"
 dynamic = []
-version = "23.5a5"
+version = "23.5a6"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/daylinmorgan/viv"
 repository = "https://github.com/daylinmorgan/viv"
@@ -43,11 +43,10 @@
     "I",
 ]
 ignore = [
     "E402",
 ]
 
 [tool.mypy]
-warn_return_any = true
 check_untyped_defs = true
 disallow_untyped_defs = true
 warn_unused_configs = true
```

### Comparing `viv-23.5a5/src/viv/viv.py` & `viv-23.5a6/src/viv/viv.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from __future__ import annotations
 
 import hashlib
 import inspect
 import itertools
 import json
+import logging
 import os
 import re
 import shutil
 import site
 import subprocess
 import sys
 import tempfile
@@ -29,14 +30,15 @@
     Namespace,
     RawDescriptionHelpFormatter,
     _SubParsersAction,
 )
 from argparse import ArgumentParser as StdArgParser
 from dataclasses import dataclass
 from datetime import datetime
+from logging.handlers import RotatingFileHandler
 from pathlib import Path
 from textwrap import dedent, fill
 from types import TracebackType
 from typing import (
     Any,
     Dict,
     List,
@@ -46,30 +48,29 @@
     TextIO,
     Tuple,
     Type,
 )
 from urllib.error import HTTPError
 from urllib.request import urlopen
 
-__version__ = "23.5a5"
+__version__ = "23.5a6"
 
 
 class Spinner:
     """spinner modified from:
     https://raw.githubusercontent.com/Tagar/stuff/master/spinner.py
     """
 
     def __init__(self, message: str, delay: float = 0.1) -> None:
         self.spinner = itertools.cycle([f"{c}  " for c in "⣾⣽⣻⢿⡿⣟⣯⣷"])
         self.delay = delay
         self.busy = False
         self.spinner_visible = False
         self.message = message
-        # sys.stdout.write(message)
-        echo(message + "  ", newline=False)
+        sys.stderr.write(f"{a.prefix} {a.sep} {message} ")
 
     def write_next(self) -> None:
         with self._screen_lock:
             if not self.spinner_visible:
                 sys.stderr.write(next(self.spinner))
                 self.spinner_visible = True
                 sys.stderr.flush()
@@ -106,14 +107,69 @@
         if sys.stderr.isatty():
             self.busy = False
             self.remove_spinner(cleanup=True)
         else:
             sys.stderr.write("\r")
 
 
+def _path_ok(p: Path) -> Path:
+    p.mkdir(exist_ok=True, parents=True)
+    return p
+
+
+class Env:
+    defaults = dict(
+        viv_bin_dir=Path.home() / ".local" / "bin",
+        xdg_cache_home=Path.home() / ".cache",
+        xdg_data_home=Path.home() / ".local" / "share",
+    )
+
+    def __getattr__(self, attr: str) -> Any:
+        if (
+            not attr.startswith("_")
+            and (defined := getattr(self, f"_{attr}")) is not None
+        ):
+            return defined
+        else:
+            return os.getenv(attr.upper(), self.defaults.get(attr))
+
+    @property
+    def _viv_cache(self) -> Path:
+        return Path(os.getenv("VIV_CACHE", (Path(self.xdg_cache_home) / "viv")))
+
+    @property
+    def _viv_spec(self) -> List[str]:
+        return [i for i in os.getenv("VIV_SPEC", "").split(" ") if i]
+
+    @property
+    def _viv_log_path(self) -> Path:
+        return _path_ok(Path(self.xdg_data_home) / "viv") / "viv.log"
+
+
+class Cache:
+    def __init__(self) -> None:
+        self.base = Env().viv_cache
+
+    @property
+    def src(self) -> Path:
+        return _path_ok(self.base / "src")
+
+    @property
+    def venv(self) -> Path:
+        return _path_ok(self.base / "venvs")
+
+
+class Cfg:
+    @property
+    def src(self) -> Path:
+        p = Path(Env().xdg_data_home) / "viv" / "viv.py"
+        p.parent.mkdir(exist_ok=True, parents=True)
+        return p
+
+
 class Ansi:
     """control ouptut of ansi(VT100) control codes"""
 
     def __init__(self) -> None:
         self.bold: str = "\033[1m"
         self.dim: str = "\033[2m"
         self.underline: str = "\033[4m"
@@ -125,15 +181,15 @@
         self.end: str = "\033[0m"
 
         # for argparse help
         self.header: str = self.cyan
         self.option: str = self.yellow
         self.metavar: str = "\033[33m"  # normal yellow
 
-        if os.getenv("NO_COLOR") or not sys.stderr.isatty():
+        if Env().no_color or not sys.stderr.isatty():
             for attr in self.__dict__:
                 setattr(self, attr, "")
 
         self._ansi_escape = re.compile(
             r"""
             \x1B  # ESC
             (?:   # 7-bit C1 Fe (except CSI)
@@ -144,68 +200,138 @@
                 [ -/]*  # Intermediate bytes
                 [@-~]   # Final byte
             )
             """,
             re.VERBOSE,
         )
 
+        self.sep = f"{self.magenta}|{self.end}"
+        self.prefix = f"{self.cyan}viv{self.end}"
+
     def escape(self, txt: str) -> str:
         return self._ansi_escape.sub("", txt)
 
     def style(self, txt: str, style: str = "cyan") -> str:
         """style text with given style
         Args:
             txt: text to stylize
             style: color/style to apply to text
         Returns:
             ansi escape code stylized text
         """
         return f"{getattr(self,style)}{txt}{getattr(self,'end')}"
 
     def tagline(self) -> str:
-        """generate the viv tagline!"""
+        """generate the viv tagline"""
 
         return " ".join(
             (
                 self.style(f, "magenta") + self.style(rest, "cyan")
-                for f, rest in (("v", "iv"), ("i", "sn't"), ("v", "env!"))
+                for f, rest in (("v", "iv"), ("i", "sn't"), ("v", "env"))
             )
         )
 
     def subprocess(self, command: List[str], output: str) -> None:
         """generate output for subprocess error
 
         Args:
             output: text output from subprocess, usually from p.stdout
         """
         if not output:
             return
 
-        error("subprocess failed")
-        echo("see below for command output", style="red")
-        echo(f"cmd:\n  {' '.join(command)}", style="red")
+        log.error("subprocess failed")
+        log.error("see below for command output")
+        log.error(f"cmd:\n  {' '.join(command)}")
         new_output = [f"{self.red}->{self.end} {line}" for line in output.splitlines()]
-        echo("subprocess output:" + "\n".join(("", *new_output, "")), style="red")
-
-    def viv_preamble(self, style: str = "magenta", sep: str = "::") -> str:
-        return f"{self.cyan}viv{self.end}{self.__dict__[style]}{sep}{self.end}"
+        log.error("subprocess output:" + "\n".join(("", *new_output, "")))
 
 
 a = Ansi()
 
 
-class Template:
-    description = f"""
+class MutlilineFormatter(logging.Formatter):
+    def format(self, record: logging.LogRecord) -> str:
+        outlines = []
+        lines = (save_msg := record.msg).splitlines()
+        for line in lines:
+            record.msg = line
+            outlines.append(super().format(record))
+        record.msg = save_msg
+        record.message = (output := "\n".join(outlines))
+        return output
+
+
+class CustomFormatter(logging.Formatter):
+    def __init__(self) -> None:
+        super().__init__()
+        self.FORMATS = {
+            **{
+                level: " ".join(
+                    (
+                        a.prefix,
+                        f"{a.sep}{color}%(levelname)s{a.end}{a.sep}",
+                        "%(message)s",
+                    )
+                )
+                for level, color in {
+                    logging.DEBUG: a.dim,
+                    logging.WARNING: a.yellow,
+                    logging.ERROR: a.red,
+                    logging.CRITICAL: a.red,
+                }.items()
+            },
+            logging.INFO: f"{a.prefix} {a.sep} %(message)s",
+        }
+
+    def format(self, record: logging.LogRecord) -> str:
+        log_fmt = self.FORMATS.get(record.levelno)
+        formatter = MutlilineFormatter(log_fmt)
+        return formatter.format(record)
+
+
+class CustomFileHandler(RotatingFileHandler):
+    """Custom logging handler to strip ansi before logging to file"""
+
+    def emit(self, record: logging.LogRecord) -> None:
+        record.msg = a.escape(record.msg)
+        super().emit(record)
 
-{a.tagline()}
-to create/activate a vivenv:
-- from command line: `{a.style("viv -h","bold")}`
-- within python script: {a.style('__import__("viv").use("typer", "rich-click")','bold')}
-"""
 
+def gen_logger() -> logging.Logger:
+    logger = logging.getLogger("viv")
+    if not logger.handlers:
+        logger.setLevel(logging.DEBUG)
+
+        ch = logging.StreamHandler()
+        ch.setLevel(logging.INFO if not Env().viv_debug else logging.DEBUG)
+        ch.setFormatter(CustomFormatter())
+
+        fh = CustomFileHandler(
+            Env().viv_log_path, maxBytes=10 * 1024 * 1024, backupCount=5
+        )
+        fh.setLevel(logging.DEBUG)
+        fh.setFormatter(
+            MutlilineFormatter("%(asctime)s | %(levelname)8s | %(message)s")
+        )
+
+        logger.addHandler(ch)
+        logger.addHandler(fh)
+    return logger
+
+
+log = gen_logger()
+
+
+def err_quit(*msg: str, code: int = 1) -> None:
+    log.error("\n".join(msg))
+    sys.exit(code)
+
+
+class Template:
     _standalone_func = r"""def _viv_use(*pkgs, track_exe=False, name=""):
     import hashlib, json, os, site, shutil, sys, venv  # noqa
     from pathlib import Path  # noqa
     from datetime import datetime  # noqa
     from subprocess import run  # noqa
 
     if not {*map(type, pkgs)} == {str}:
@@ -217,191 +343,208 @@
     cache = (Path(xdg) if xdg else Path.home() / ".cache") / "viv" / "venvs"
     cache.mkdir(parents=True, exist_ok=True)
     exe = str(Path(sys.executable).resolve()) if track_exe else "N/A"
     (sha256 := hashlib.sha256()).update((str(spec := [*pkgs]) + exe).encode())
     _id = sha256.hexdigest()
     if (env := cache / (name if name else _id)) not in cache.glob("*/") or force:
         sys.stderr.write(f"generating new vivenv -> {env.name}\n")
-        venv.create(env, symlinks=True, with_pip=True, clear=True)
-        (env / "pip.conf").write_text("[global]\ndisable-pip-version-check=true")
-        run_kw = dict(zip(("stdout", "stderr"), ((None,) * 2 if verbose else (-1, 2))))
-        p = run([env / "bin" / "pip", "install", "--force-reinstall", *spec], **run_kw)
+        venv.create(env, symlinks=True, clear=True)
+        kw = dict(zip(("stdout", "stderr"), ((None,) * 2 if verbose else (-1, 2))))
+        cmd = ["pip", "--python", str(env / "bin" / "python"), "install", *spec]
+        p = run(cmd, **kw)
         if (rc := p.returncode) != 0:
             if env.is_dir():
                 shutil.rmtree(env)
             sys.stderr.write(f"pip had non zero exit ({rc})\n{p.stdout.decode()}\n")
             sys.exit(rc)
         meta.update(dict(id=_id, spec=spec, exe=exe, name=name, files=[runner]))
     else:
         meta = json.loads((env / "vivmeta.json").read_text())
-        meta.update(dict(accessed=t, files=sorted({*meta["files"],runner})))
+        meta.update(dict(accessed=t, files=sorted({*meta["files"], runner})))
 
     (env / "vivmeta.json").write_text(json.dumps(meta))
-    sys.path = [p for p in sys.path if not p != site.USER_SITE]
-    site.addsitedir(str(*(env / "lib").glob("py*/si*")))
+    site.addsitedir(sitepkgs:=str(*(env / "lib").glob("py*/si*")))
+    sys.path = [p for p in (sitepkgs,*sys.path) if p != site.USER_SITE]
     return env
 """
 
-    def noqa(self, txt: str) -> str:
+    @staticmethod
+    def description(name: str) -> str:
+        return f"""
+
+{a.tagline()}
+command line: `{a.bold}{name} --help{a.end}`
+python api: {a.style('__import__("viv").use("typer", "rich-click")','bold')}
+"""
+
+    @staticmethod
+    def noqa(txt: str) -> str:
         max_length = max(map(len, txt.splitlines()))
         return "\n".join((f"{line:{max_length}} # noqa" for line in txt.splitlines()))
 
-    def _use_str(self, spec: List[str], standalone: bool = False) -> str:
+    @staticmethod
+    def _use_str(spec: List[str], standalone: bool = False) -> str:
         spec_str = ", ".join(f'"{req}"' for req in spec)
         if standalone:
             return f"""_viv_use({fill(spec_str,width=90,subsequent_indent="    ",)})"""
         else:
             return f"""__import__("viv").use({spec_str})"""
 
-    def standalone(self, spec: List[str]) -> str:
+    @classmethod
+    def standalone(cls, spec: List[str]) -> str:
         func_use = "\n".join(
-            (self._standalone_func, self.noqa(self._use_str(spec, standalone=True)))
+            (cls._standalone_func, cls.noqa(cls._use_str(spec, standalone=True)))
         )
         return f"""
 # AUTOGENERATED by viv (v{__version__})
 # see `python3 <(curl -fsSL viv.dayl.in/viv.py) --help`
 {func_use}
 """
 
-    def _rel_import(self, local_source: Optional[Path]) -> str:
+    @staticmethod
+    def _rel_import(local_source: Optional[Path]) -> str:
         if not local_source:
             raise ValueError("local source must exist")
 
         path_to_viv = path_to_viv = str(
             local_source.resolve().absolute().parent.parent
         ).replace(str(Path.home()), "~")
         return (
             """__import__("sys").path.append(__import__("os")"""
             f""".path.expanduser("{path_to_viv}"))  # noqa"""
         )
 
-    def _absolute_import(self, local_source: Optional[Path]) -> str:
+    @staticmethod
+    def _absolute_import(local_source: Optional[Path]) -> str:
         if not local_source:
             raise ValueError("local source must exist")
 
         path_to_viv = local_source.resolve().absolute().parent.parent
         return f"""__import__("sys").path.append("{path_to_viv}")  # noqa"""
 
+    @classmethod
     def frozen_import(
-        self, path: str, local_source: Optional[Path], spec: List[str]
+        cls, path: str, local_source: Optional[Path], spec: List[str]
     ) -> str:
         if path == "abs":
-            imports = self._absolute_import(local_source)
+            imports = cls._absolute_import(local_source)
         elif path == "rel":
-            imports = self._rel_import(local_source)
+            imports = cls._rel_import(local_source)
         else:
             imports = ""
         return f"""\
 {imports}
-{self.noqa(self._use_str(spec))}
+{cls.noqa(cls._use_str(spec))}
 """
 
+    @classmethod
     def shim(
-        self,
+        cls,
         path: str,
         local_source: Optional[Path],
         standalone: bool,
         spec: List[str],
         bin: str,
     ) -> str:
         if standalone:
-            imports = self._standalone_func
+            imports = cls._standalone_func
         elif path == "abs":
-            imports = self._absolute_import(local_source)
+            imports = cls._absolute_import(local_source)
         elif path == "rel":
-            imports = self._rel_import(local_source)
+            imports = cls._rel_import(local_source)
         else:
             imports = ""
         return f"""\
-#!/usr/bin/env python
+#!/usr/bin/env python3
 # AUTOGENERATED by viv (v{__version__})
 # see `python3 <(curl -fsSL viv.dayl.in/viv.py) --help`
 
 {imports}
 import subprocess
 import sys
 
 if __name__ == "__main__":
-    vivenv = {self.noqa(self._use_str(spec, standalone))}
+    vivenv = {cls.noqa(cls._use_str(spec, standalone))}
     sys.exit(subprocess.run([vivenv / "bin" / "{bin}", *sys.argv[1:]]).returncode)
 """
 
+    @staticmethod
     def update(
-        self, src: Optional[Path], cli: Path, local_version: str, next_version: str
+        src: Optional[Path], cli: Path, local_version: str, next_version: str
     ) -> str:
         return f"""
   Update source at {a.green}{src}{a.end}
   Symlink {a.bold}{src}{a.end} to {a.bold}{cli}{a.end}
   Version {a.bold}{local_version}{a.end} -> {a.bold}{next_version}{a.end}
 
 """
 
-    def install(self, src: Path, cli: Path) -> str:
+    @staticmethod
+    def install(src: Path, cli: Path) -> str:
         return f"""
   Install viv.py to {a.green}{src}{a.end}
   Symlink {a.bold}{src}{a.end} to {a.bold}{cli}{a.end}
 
 """
 
+    @staticmethod
     def show(
-        self, cli: Optional[Path | str], running: Path, local: Optional[Path | str]
+        cli: Optional[Path | str], running: Path, local: Optional[Path | str]
     ) -> str:
         return (
             "\n".join(
                 f"  {a.bold}{k}{a.end}: {v}"
                 for k, v in (
                     ("Version", __version__),
                     ("CLI", cli),
                     ("Running Source", running),
                     ("Local Source", local),
+                    ("Cache", Cache().base),
                 )
             )
             + "\n"
         )
 
 
-t = Template()
-
-
 # TODO: convert the below functions into a proper file/stream logging interface
 def echo(
     msg: str, style: str = "magenta", newline: bool = True, fd: TextIO = sys.stderr
 ) -> None:
     """output general message to stdout"""
-    output = f"{a.viv_preamble(style)} {msg}"
-    if newline:
-        output += "\n"
+    output = f"{a.prefix} {a.sep} {msg}\n"
     fd.write(output)
 
 
-def error(msg: str, code: int = 0) -> None:
+def error(*msg: str, exit: bool = True, code: int = 1) -> None:
     """output error message and if code provided exit"""
-    echo(f"{a.red}error:{a.end} {msg}", style="red")
-    if code:
+    prefix = f"{a.prefix} {a.sep}{a.red}ERROR{a.end}{a.sep} "
+    sys.stderr.write("\n".join((f"{prefix}{line}" for line in msg)) + "\n")
+    if exit:
         sys.exit(code)
 
 
-def warn(msg: str) -> None:
-    """output warning message to stdout"""
-    echo(f"{a.yellow}warn:{a.end} {msg}", style="yellow")
-
-
-def confirm(question: str, context: str = "") -> bool:
+def confirm(question: str, context: str = "", yes: bool = False) -> bool:
     sys.stderr.write(context)
+    # TODO: update this
     sys.stderr.write(
-        a.viv_preamble(sep="?? ") + question + a.style(" (Y)es/(n)o ", "yellow")
+        f"{a.prefix} {a.sep}{a.magenta}?{a.end}{a.sep}"
+        f" {question} {a.yellow}(Y)es/(n)o{a.end} "
     )
+    if yes:
+        sys.stderr.write(f"{a.green}[FORCED YES]{a.end}\n")
+        return True
+
     while True:
         ans = input().strip().lower()
         if ans in ("y", "yes"):
             return True
         elif ans in ("n", "no"):
             return False
-        sys.stdout.write("Please select (Y)es or (n)o. ")
-    sys.stdout.write("\n")
+        sys.stderr.write("Please select (Y)es or (n)o. ")
+    sys.stderr.write("\n")
 
 
 class CustomHelpFormatter(RawDescriptionHelpFormatter, HelpFormatter):
     """formatter to remove extra metavar on short opts"""
 
     def _get_invocation_length(self, invocation: str) -> int:
         return len(a.escape(invocation))
@@ -526,16 +669,15 @@
 
         self.formatter_class = lambda prog: CustomHelpFormatter(
             prog,
             max_help_position=35,
         )
 
     def error(self, message: str) -> NoReturn:
-        error(message)
-        echo(f"see `{self.prog} --help` for more info", style="red")
+        error(message, f"see `{self.prog} --help` for more info")
         sys.exit(2)
 
 
 def run(
     command: List[str],
     spinmsg: str = "",
     clean_up_path: Optional[Path] = None,
@@ -609,30 +751,31 @@
     files: List[str]
     exe: str
     created: str = ""
     accessed: str = ""
 
     @classmethod
     def load(cls, name: str) -> "Meta":
-        if not (c.venvcache / name / "vivmeta.json").exists():
-            warn(f"possibly corrupted vivenv: {name}")
+        if not (Cache().venv / name / "vivmeta.json").exists():
+            log.warning(f"possibly corrupted vivenv: {name}")
             # add empty values for corrupted vivenvs so it will still load
             return cls(name=name, spec=[""], files=[""], exe="", id="")
         else:
-            meta = json.loads((c.venvcache / name / "vivmeta.json").read_text())
+            meta = json.loads((Cache().venv / name / "vivmeta.json").read_text())
 
         return cls(**meta)
 
     def write(self, p: Path | None = None) -> None:
         if not p:
-            p = (c.venvcache) / self.name / "vivmeta.json"
+            p = (Cache().venv) / self.name / "vivmeta.json"
 
         p.write_text(json.dumps(self.__dict__))
 
     def addfile(self, f: Path) -> None:
+        log.debug(f"associating {f} with {self.name}")
         self.accessed = str(datetime.today())
         self.files = sorted({*self.files, str(f.absolute().resolve())})
 
 
 class ViVenv:
     def __init__(
         self,
@@ -644,19 +787,19 @@
         skip_load: bool = False,
         metadata: Meta | None = None,
     ) -> None:
         self.loaded = False
         spec = self._validate_spec(spec)
         id = id if id else get_hash(spec, track_exe)
 
-        self.name = name if name else id
-        self.path = path if path else c.venvcache / self.name
+        self.name = name if name else id[:8]
+        self.set_path(path)
 
         if not metadata:
-            if self.name in (d.name for d in c.venvcache.iterdir()):
+            if self.name in (d.name for d in Cache().venv.iterdir()):
                 self.loaded = True
                 self.meta = Meta.load(self.name)
             else:
                 self.meta = Meta(
                     spec=spec,
                     name=self.name,
                     id=id,
@@ -672,56 +815,69 @@
         Args:
             name: used as lookup in the vivenv cache
         """
         vivenv = cls(name=name, metadata=Meta.load(name))
 
         return vivenv
 
+    def set_path(self, path: Path | None = None) -> None:
+        self.path = path if path else Cache().venv / self.name
+        self.python = str((self.path / "bin" / "python").absolute())
+        self.pip = ("pip", "--python", self.python)
+
     def _validate_spec(self, spec: List[str]) -> List[str]:
         """ensure spec is at least of sequence of strings
 
         Args:
             spec: sequence of package specifications
         """
         if not set(map(type, spec)) == {str}:
-            error("unexepected input in package spec")
-            error(f"check your packages definitions: {spec}", code=1)
+            err_quit(
+                "unexepected input in package spec",
+                f"check your packages definitions: {spec}",
+            )
 
         return sorted(spec)
 
     def create(self, quiet: bool = False) -> None:
-        if not quiet:
-            echo(f"new unique vivenv -> {self.name}")
+        log.info(f"new unique vivenv: {a.bold}{self.name}{a.end}")
+        log.debug(f"creating new venv at {self.path}")
         with Spinner("creating vivenv"):
-            venv.create(self.path, with_pip=True, clear=True, symlinks=True)
-
-            # add config to ignore pip version
-            (self.path / "pip.conf").write_text(
-                "[global]\ndisable-pip-version-check = true"
+            venv.create(
+                self.path,
+                clear=True,
+                symlinks=True,
             )
 
         self.meta.created = str(datetime.today())
 
     def install_pkgs(self) -> None:
         cmd: List[str] = [
-            str(self.path / "bin" / "pip"),
+            *self.pip,
             "install",
             "--force-reinstall",
         ] + self.meta.spec
 
         run(
             cmd,
             spinmsg="installing packages in vivenv",
             clean_up_path=self.path,
-            verbose=bool(os.getenv("VIV_VERBOSE")),
+            verbose=bool(Env().viv_verbose),
         )
 
     def touch(self) -> None:
         self.meta.accessed = str(datetime.today())
 
+    def activate(self) -> None:
+        # also add sys.path here so that it comes first
+        log.debug(f"activating {self.name}")
+        path_to_add = str(*(self.path / "lib").glob("python*/site-packages"))
+        sys.path = [p for p in (path_to_add, *sys.path) if p != site.USER_SITE]
+        site.addsitedir(path_to_add)
+
     def show(self) -> None:
         _id = (
             self.meta.id[:8]
             if self.meta.id == self.name
             else (self.name[:5] + "..." if len(self.name) > 8 else self.name)
         )
 
@@ -733,29 +889,28 @@
     def _tree_leaves(self, items: List[str], indent: str = "") -> str:
         tree_chars = ["├"] * (len(items) - 1) + ["╰"]
         return "\n".join(
             (f"{indent}{a.yellow}{c}─{a.end} {i}" for c, i in zip(tree_chars, items))
         )
 
     def tree(self) -> None:
-        _id = self.meta.id if self.meta.id == self.name else self.name
-        # TODO: generarlize and loop this or make a template..
         items = [
             f"{a.magenta}{k}{a.end}: {v}"
             for k, v in {
                 **{
+                    "id": self.meta.id,
                     "spec": ", ".join(self.meta.spec),
                     "created": self.meta.created,
                     "accessed": self.meta.accessed,
                 },
                 **({"exe": self.meta.exe} if self.meta.exe != "N/A" else {}),
                 **({"files": ""} if self.meta.files else {}),
             }.items()
         ]
-        rows = [f"\n{a.bold}{a.cyan}{_id}{a.end}", self._tree_leaves(items)]
+        rows = [f"\n{a.bold}{a.cyan}{self.name}{a.end}", self._tree_leaves(items)]
         if self.meta.files:
             rows += (self._tree_leaves(self.meta.files, indent="   "),)
 
         sys.stdout.write("\n".join(rows) + "\n")
 
 
 def get_caller_path() -> Path:
@@ -773,48 +928,43 @@
 
     Args:
         packages: package specifications with optional version specifiers
         track_exe: if true make env python exe specific
         name: use as vivenv name, if not provided id is used
     """
 
-    vivenv = ViVenv(list(packages), track_exe=track_exe, name=name)
-    if not vivenv.loaded or os.getenv("VIV_FORCE"):
+    vivenv = ViVenv([*list(packages), *Env().viv_spec], track_exe=track_exe, name=name)
+    if not vivenv.loaded or Env().viv_force:
         vivenv.create()
         vivenv.install_pkgs()
-
     vivenv.meta.addfile(get_caller_path())
     vivenv.meta.write()
 
-    modify_sys_path(vivenv.path)
-    return vivenv.path
-
+    vivenv.activate()
 
-def modify_sys_path(new_path: Path) -> None:
-    sys.path = [p for p in sys.path if p is not site.USER_SITE]
-    site.addsitedir(str(*(new_path / "lib").glob("python*/site-packages")))
+    return vivenv.path
 
 
 def get_venvs() -> Dict[str, ViVenv]:
     vivenvs = {}
-    for p in c.venvcache.iterdir():
+    for p in Cache().venv.iterdir():
         vivenv = ViVenv.load(p.name)
         vivenvs[vivenv.name] = vivenv
     return vivenvs
 
 
 def combined_spec(reqs: List[str], requirements: Path) -> List[str]:
     if requirements:
         with requirements.open("r") as f:
             reqs += f.readlines()
     return reqs
 
 
-def resolve_deps(args: Namespace) -> List[str]:
-    spec = combined_spec(args.reqs, args.requirements)
+def resolve_deps(reqs: List[str], requirements: Path) -> List[str]:
+    spec = combined_spec(reqs, requirements)
 
     cmd = [
         "pip",
         "install",
         "--dry-run",
         "--quiet",
         "--ignore-installed",
@@ -827,105 +977,90 @@
         f"{pkg['metadata']['name']}=={pkg['metadata']['version']}"
         for pkg in report["install"]
     ]
 
     return resolved_spec
 
 
-def fetch_source(reference: str) -> str:
+def fetch_script(url: str) -> str:
     try:
-        r = urlopen(
-            "https://raw.githubusercontent.com/daylinmorgan/viv/"
-            + reference
-            + "/src/viv/viv.py"
-        )
-    except HTTPError as e:
-        error(
-            "Issue updating viv see below:"
-            + a.style("->  ", "red").join(["\n"] + repr(e).splitlines())
-        )
-        if "404" in repr(e):
-            echo("Please check your reference is valid.", style="red")
-        sys.exit(1)
+        r = urlopen(url)
+    except (HTTPError, ValueError) as e:
+        err_quit(
+            "Failed to fetch from remote url:",
+            f"  {a.bold}{url}{a.end}",
+            "see below:" + a.style("->  ", "red").join(["\n"] + repr(e).splitlines()),
+        )
+
+    return r.read().decode("utf-8")
 
-    src = r.read()
-    (hash := hashlib.sha256()).update(src)
+
+def fetch_source(reference: str) -> str:
+    src = fetch_script(
+        "https://raw.githubusercontent.com/daylinmorgan/viv/"
+        + reference
+        + "/src/viv/viv.py"
+    )
+
+    (hash := hashlib.sha256()).update(src.encode())
     sha256 = hash.hexdigest()
 
-    cached_src_file = c.srccache / f"{sha256}.py"
+    cached_src_file = Cache().src / f"{sha256}.py"
 
     if not cached_src_file.is_file():
-        with cached_src_file.open("w") as f:
-            f.write(src.decode())
+        cached_src_file.write_text(src)
 
     return sha256
 
 
 def make_executable(path: Path) -> None:
     """apply an executable bit for all users with read access"""
     mode = os.stat(path).st_mode
     mode |= (mode & 0o444) >> 2  # copy R bits to X
     os.chmod(path, mode)
 
 
-class Config:
-    """viv config manager"""
-
-    def __init__(self) -> None:
-        self._cache = Path(os.getenv("XDG_CACHE_HOME", Path.home() / ".cache")) / "viv"
-
-    def _ensure(self, p: Path) -> Path:
-        p.mkdir(parents=True, exist_ok=True)
-        return p
-
-    @property
-    def venvcache(self) -> Path:
-        return self._ensure(self._cache / "venvs")
-
-    @property
-    def srccache(self) -> Path:
-        return self._ensure(self._cache / "src")
-
-    @property
-    def binparent(self) -> Path:
-        return self._ensure(
-            Path(os.getenv("VIV_BIN_DIR", Path.home() / ".local" / "bin"))
-        )
-
-    @property
-    def srcdefault(self) -> Path:
-        parent = (
-            Path(os.getenv("XDG_DATA_HOME", Path.home() / ".local" / "share")) / "viv"
+def uses_viv(txt: str) -> bool:
+    return bool(
+        re.search(
+            """
+            \s*__import__\(\s*["']viv["']\s*\).use\(.*
+            |
+            from\ viv\ import\ use
+            |
+            import\ viv 
+        """,
+            txt,
+            re.VERBOSE,
         )
-        return self._ensure(parent) / "viv.py"
-
-
-c = Config()
+    )
 
 
 class Viv:
     def __init__(self) -> None:
+        self.t = Template()
         self.vivenvs = get_venvs()
         self._get_sources()
         self.name = "viv" if self.local else "python3 <(curl -fsSL viv.dayl.in/viv.py)"
 
     def _get_sources(self) -> None:
         self.local_source: Optional[Path] = None
         self.running_source = Path(__file__).resolve()
         self.local = not str(self.running_source).startswith("/proc/")
         if self.local:
             self.local_source = self.running_source
             self.local_version = __version__
         else:
             try:
                 _local_viv = __import__("viv")
-                self.local_source = (
-                    Path(_local_viv.__file__) if _local_viv.__file__ else None
-                )
-                self.local_version = _local_viv.__version__
+                if _local_viv.__file__:
+                    self.local_source = Path(_local_viv.__file__)
+                    self.local_version = _local_viv.__version__
+                else:
+                    self.local_version = "Not Found"
             except ImportError:
                 self.local_version = "Not Found"
 
         if self.local_source:
             self.git = (self.local_source.parent.parent.parent / ".git").is_dir()
         else:
             self.git = False
@@ -941,296 +1076,398 @@
                 matches.append(v)
             elif v.name.startswith(name_id):
                 matches.append(v)
 
         if len(matches) == 1:
             return matches[0]
         elif len(matches) > 1:
-            echo(f"matches {','.join((match.name for match in matches))}", style="red")
-            error("too many matches maybe try a longer name?", code=1)
+            err_quit(
+                "matches: " + ",".join((match.name for match in matches)),
+                "too many matches maybe try a longer name?",
+            )
         else:
-            error(f"no matches found for {name_id}", code=1)
+            err_quit(f"no matches found for {name_id}")
 
-    def remove(self, args: Namespace) -> None:
+    def remove(self, vivenvs: List[str]) -> None:
         """\
         remove a vivenv
 
         To remove all viv venvs:
         `viv rm $(viv l -q)`
         """
 
-        for name in args.vivenv:
+        for name in vivenvs:
             vivenv = self._match_vivenv(name)
             if vivenv.path.is_dir():
-                echo(f"removing {vivenv.name}")
+                log.info(f"removing {vivenv.name}")
                 shutil.rmtree(vivenv.path)
             else:
-                error(
+                err_quit(
                     f"cowardly exiting because I didn't find vivenv: {name}",
-                    code=1,
                 )
 
-    def freeze(self, args: Namespace) -> None:
+    def freeze(
+        self,
+        reqs: List[str],
+        requirements: Path,
+        keep: bool,
+        standalone: bool,
+        path: str,
+    ) -> None:
         """create import statement from package spec"""
 
-        spec = resolve_deps(args)
-        if args.keep:
+        spec = resolve_deps(reqs, requirements)
+        if keep:
             # re-create env again since path's are hard-coded
             vivenv = ViVenv(spec)
 
-            if not vivenv.loaded or os.getenv("VIV_FORCE"):
+            if not vivenv.loaded or Env().viv_force:
                 vivenv.create()
                 vivenv.install_pkgs()
                 vivenv.meta.write()
             else:
-                echo("re-using existing vivenv")
+                log.info("re-using existing vivenv")
 
             vivenv.touch()
             vivenv.meta.write()
 
-        echo("see below for import statements\n")
+        log.info("see below for import statements\n")
 
-        if args.standalone:
-            sys.stdout.write(t.standalone(spec))
+        if standalone:
+            sys.stdout.write(self.t.standalone(spec))
             return
 
-        if args.path and not self.local_source:
-            error("No local viv found to import from", code=1)
+        if path and not self.local_source:
+            err_quit("No local viv found to import from")
 
-        sys.stdout.write(t.frozen_import(args.path, self.local_source, spec))
+        sys.stdout.write(self.t.frozen_import(path, self.local_source, spec))
 
-    def list(self, args: Namespace) -> None:
+    def list(self, quiet: bool, full: bool, use_json: bool) -> None:
         """list all vivenvs"""
 
-        if args.quiet:
+        if quiet:
             sys.stdout.write("\n".join(self.vivenvs) + "\n")
         elif len(self.vivenvs) == 0:
-            echo("no vivenvs setup")
-        elif args.full:
+            log.info("no vivenvs setup")
+        elif full:
             for _, vivenv in self.vivenvs.items():
                 vivenv.tree()
-        elif args.json:
+        elif use_json:
             sys.stdout.write(
                 json.dumps({k: v.meta.__dict__ for k, v in self.vivenvs.items()})
             )
         else:
             for _, vivenv in self.vivenvs.items():
                 vivenv.show()
 
-    def exe(self, args: Namespace) -> None:
+    def exe(self, vivenv_id: str, cmd: str, rest: List[str]) -> None:
         """\
         run binary/script in existing vivenv
 
         examples:
-            viv exe <vivenv> pip -- list
             viv exe <vivenv> python -- script.py
+            viv exe <vivenv> python -- -m http.server
         """
 
-        vivenv = self._match_vivenv(args.vivenv)
-        bin = vivenv.path / "bin" / args.cmd
+        vivenv = self._match_vivenv(vivenv_id)
+        bin = vivenv.path / "bin" / cmd
 
         if not bin.exists():
-            error(f"{args.cmd} does not exist in {vivenv.name}", code=1)
+            err_quit(f"{cmd} does not exist in {vivenv.name}")
 
-        cmd = [bin, *args.rest]
+        full_cmd = [str(bin), *rest]
 
-        run(cmd, verbose=True)
+        run(full_cmd, verbose=True)
 
-    def info(self, args: Namespace) -> None:
+    def info(self, vivenv_id: str, path: bool, use_json: bool) -> None:
         """get metadata about a vivenv"""
-        vivenv = self._match_vivenv(args.vivenv)
+        vivenv = self._match_vivenv(vivenv_id)
         metadata_file = vivenv.path / "vivmeta.json"
 
         if not metadata_file.is_file():
-            error(f"Unable to find metadata for vivenv: {args.vivenv}", code=1)
-        if args.json:
+            err_quit(f"Unable to find metadata for vivenv: {vivenv_id}")
+
+        if use_json:
             sys.stdout.write(json.dumps(vivenv.meta.__dict__))
+        elif path:
+            sys.stdout.write(f"{vivenv.path.absolute()}\n")
         else:
             vivenv.tree()
 
-    def _install_local_src(self, sha256: str, src: Path, cli: Path) -> None:
-        echo("updating local source copy of viv")
-        shutil.copy(c.srccache / f"{sha256}.py", src)
+    def _install_local_src(self, sha256: str, src: Path, cli: Path, yes: bool) -> None:
+        log.info("updating local source copy of viv")
+        shutil.copy(Cache().src / f"{sha256}.py", src)
         make_executable(src)
-        echo("symlinking cli")
+        log.info("symlinking cli")
 
         if cli.is_file():
-            echo(f"Existing file at {a.style(str(cli),'bold')}")
-            if confirm("Would you like to overwrite it?"):
+            log.info(f"Existing file at {a.style(str(cli),'bold')}")
+            if confirm("Would you like to overwrite it?", yes=yes):
                 cli.unlink()
                 cli.symlink_to(src)
         else:
             cli.symlink_to(src)
 
-        echo("Remember to include the following line in your shell rc file:")
+        log.info("Remember to include the following line in your shell rc file:")
         sys.stderr.write(
             '  export PYTHONPATH="$PYTHONPATH:$HOME/'
             f'{src.relative_to(Path.home()).parent}"\n'
         )
 
     def _get_new_version(self, ref: str) -> Tuple[str, str]:
-        sys.path.append(str(c.srccache))
+        sys.path.append(str(Cache().src))
         return (sha256 := fetch_source(ref)), __import__(sha256).__version__
 
-    def manage(self, args: Namespace) -> None:
+    def manage(self) -> None:
         """manage viv itself"""
 
-        if args.subcmd == "show":
-            if args.pythonpath:
-                if self.local and self.local_source:
-                    sys.stdout.write(str(self.local_source.parent) + "\n")
-                else:
-                    error("expected to find a local installation", code=1)
+    def manage_show(
+        self,
+        pythonpath: bool = False,
+    ) -> None:
+        """manage viv itself"""
+        if pythonpath:
+            if self.local and self.local_source:
+                sys.stdout.write(str(self.local_source.parent) + "\n")
             else:
-                echo("Current:")
-                sys.stderr.write(
-                    t.show(
-                        cli=shutil.which("viv"),
-                        running=self.running_source,
-                        local=self.local_source,
-                    )
+                err_quit("expected to find a local installation")
+        else:
+            echo("Current:")
+            sys.stderr.write(
+                self.t.show(
+                    cli=shutil.which("viv"),
+                    running=self.running_source,
+                    local=self.local_source,
                 )
+            )
 
-        elif args.subcmd == "update":
-            sha256, next_version = self._get_new_version(args.ref)
+    def manage_update(
+        self,
+        ref: str,
+        src: Path,
+        cli: Path,
+        yes: bool,
+    ) -> None:
+        sha256, next_version = self._get_new_version(ref)
 
-            if self.local_version == next_version:
-                echo(f"no change between {args.ref} and local version")
-                sys.exit(0)
-
-            if confirm(
-                "Would you like to perform the above installation steps?",
-                t.update(self.local_source, args.cli, self.local_version, next_version),
-            ):
-                self._install_local_src(
-                    sha256,
-                    Path(
-                        args.src if not self.local_source else self.local_source,
-                    ),
-                    args.cli,
-                )
+        if self.local_version == next_version:
+            log.info(f"no change between {ref} and local version")
+            sys.exit(0)
 
-        elif args.subcmd == "install":
-            sha256, downloaded_version = self._get_new_version(args.ref)
+        if confirm(
+            "Would you like to perform the above installation steps?",
+            self.t.update(self.local_source, cli, self.local_version, next_version),
+            yes=yes,
+        ):
+            self._install_local_src(
+                sha256,
+                Path(
+                    src if not self.local_source else self.local_source,
+                ),
+                cli,
+                yes,
+            )
 
-            echo(f"Downloaded version: {downloaded_version}")
+    def manage_install(
+        self,
+        ref: str,
+        src: Path,
+        cli: Path,
+        yes: bool,
+    ) -> None:
+        sha256, downloaded_version = self._get_new_version(ref)
 
-            # TODO: see if file is actually where
-            # we are about to install and give more instructions
+        log.info(f"Downloaded version: {downloaded_version}")
 
-            if confirm(
-                "Would you like to perform the above installation steps?",
-                t.install(args.src, args.cli),
-            ):
-                self._install_local_src(sha256, args.src, args.cli)
+        # TODO: see if file is actually where
+        # we are about to install and give more instructions
 
-        elif args.subcmd == "purge":
-            to_remove = []
-            if c._cache.is_dir():
-                to_remove.append(c._cache)
-            if args.src.is_file():
-                to_remove.append(
-                    args.src.parent if args.src == c.srcdefault else args.src
-                )
-            if self.local_source and self.local_source.is_file():
-                if self.local_source.parent.name == "viv":
-                    to_remove.append(self.local_source.parent)
-                else:
-                    to_remove.append(self.local_source)
+        if confirm(
+            "Would you like to perform the above installation steps?",
+            self.t.install(src, cli),
+            yes=yes,
+        ):
+            self._install_local_src(sha256, src, cli, yes)
 
-            if args.cli.is_file():
-                to_remove.append(args.cli)
+    def manage_purge(
+        self,
+        ref: str,
+        src: Path,
+        cli: Path,
+        yes: bool,
+    ) -> None:
+        to_remove = []
+        if Cache().base.is_dir():
+            to_remove.append(Cache().base)
+        if src.is_file():
+            to_remove.append(src.parent if src == (Cfg().src) else src)
+        if self.local_source and self.local_source.is_file():
+            if self.local_source.parent.name == "viv":
+                to_remove.append(self.local_source.parent)
+            else:
+                to_remove.append(self.local_source)
 
-            to_remove = list(set(to_remove))
-            if confirm(
-                "Remove the above files/directories?",
-                "\n".join(f"  - {a.red}{p}{a.end}" for p in to_remove) + "\n",
-            ):
-                for p in to_remove:
-                    if p.is_dir():
-                        shutil.rmtree(p)
-                    else:
-                        p.unlink()
-
-                echo(
-                    "to re-install use: "
-                    "`python3 <(curl -fsSL viv.dayl.in/viv.py) manage install`"
-                )
+        if cli.is_file():
+            to_remove.append(cli)
 
-    def _pick_bin(self, args: Namespace) -> Tuple[str, str]:
-        default = re.split(r"[=><~!*]+", args.reqs[0])[0]
-        return default, (default if not args.bin else args.bin)
+        to_remove = list(set(to_remove))
+        if confirm(
+            "Remove the above files/directories?",
+            "\n".join(f"  - {a.red}{p}{a.end}" for p in to_remove) + "\n",
+            yes=yes,
+        ):
+            for p in to_remove:
+                if p.is_dir():
+                    shutil.rmtree(p)
+                else:
+                    p.unlink()
+
+            log.info(
+                "to re-install use: "
+                "`python3 <(curl -fsSL viv.dayl.in/viv.py) manage install`"
+            )
 
-    def shim(self, args: Namespace) -> None:
+    def _pick_bin(self, reqs: List[str], bin: str) -> Tuple[str, str]:
+        default = re.split(r"[=><~!*]+", reqs[0])[0]
+        return default, (default if not bin else bin)
+
+    def shim(
+        self,
+        reqs: List[str],
+        requirements: Path,
+        bin: str,
+        output: Path,
+        freeze: bool,
+        yes: bool,
+        path: str,
+        standalone: bool,
+    ) -> None:
         """\
         generate viv-powered cli apps
 
         examples:
           viv shim black
           viv shim yartsu -o ~/bin/yartsu --standalone
         """
-        default_bin, bin = self._pick_bin(args)
-        output = (
-            c.binparent / default_bin if not args.output else args.output.absolute()
-        )
+        default_bin, bin = self._pick_bin(reqs, bin)
+        output = Env().viv_bin_dir / default_bin if not output else output.absolute()
 
         if output.is_file():
-            error(f"{output} already exists...exiting", code=1)
+            err_quit(f"{output} already exists...exiting")
 
-        if args.freeze:
-            spec = resolve_deps(args)
+        if freeze:
+            spec = resolve_deps(reqs, requirements)
         else:
-            spec = combined_spec(args.reqs, args.requirements)
+            spec = combined_spec(reqs, requirements)
 
         if confirm(
-            f"Write shim for {a.style(bin,'bold')} to {a.style(output,'green')}?"
+            f"Write shim for {a.bold}{bin}{a.end} to {a.green}{output}{a.end}?",
+            yes=yes,
         ):
             with output.open("w") as f:
-                f.write(
-                    t.shim(args.path, self.local_source, args.standalone, spec, bin)
-                )
+                f.write(self.t.shim(path, self.local_source, standalone, spec, bin))
 
             make_executable(output)
 
-    def run(self, args: Namespace) -> None:
+    def run(
+        self,
+        reqs: List[str],
+        requirements: Path,
+        script: str,
+        keep: bool,
+        rest: List[str],
+        bin: str,
+    ) -> None:
         """\
-        run an app with an on-demand venv
+        run an app/script with an on-demand venv
 
         examples:
           viv r pycowsay -- "viv isn't venv\!"
           viv r rich -b python -- -m rich
+          viv r -s <remote python script>
         """
 
-        _, bin = self._pick_bin(args)
-        spec = combined_spec(args.reqs, args.requirements)
-        vivenv = ViVenv(spec)
-
-        # TODO: respect a VIV_RUN_MODE env variable as the same as keep i.e.
-        # ephemeral (default), semi-ephemeral (persist inside /tmp), or
-        # persist (use c.cache)
-
-        if not vivenv.loaded or os.getenv("VIV_FORCE"):
-            if not args.keep:
-                with tempfile.TemporaryDirectory(prefix="viv-") as tmpdir:
-                    vivenv.path = Path(tmpdir)
-                    vivenv.create()
-                    vivenv.install_pkgs()
+        spec = combined_spec(reqs, requirements)
+
+        if script:
+            env = os.environ
+            name = script.split("/")[-1]
+
+            # TODO: reduce boilerplate and dry out
+            with tempfile.TemporaryDirectory(prefix="viv-") as tmpdir:
+                tmppath = Path(tmpdir)
+                scriptpath = tmppath / name
+                if not self.local_source:
+                    (tmppath / "viv.py").write_text(
+                        # TODO: use latest tag once ready
+                        fetch_script(
+                            "https://raw.githubusercontent.com/daylinmorgan/viv/dev/src/viv/viv.py"
+                        )
+                    )
+
+                if Path(script).is_file():
+                    script_text = Path(script).read_text()
+                else:
+                    script_text = fetch_script(script)
+
+                viv_used = uses_viv(script_text)
+                scriptpath.write_text(script_text)
+
+                if not keep:
+                    env.update({"VIV_CACHE": tmpdir})
+                    os.environ["VIV_CACHE"] = tmpdir
+
+                if viv_used:
+                    env.update({"VIV_SPEC": " ".join(f"'{req}'" for req in spec)})
+
                     sys.exit(
                         subprocess.run(
-                            [vivenv.path / "bin" / bin, *args.rest]
+                            [sys.executable, scriptpath, *rest], env=env
                         ).returncode
                     )
-            else:
-                vivenv.create()
-                vivenv.install_pkgs()
+                else:
+                    vivenv = ViVenv(spec)
+                    if not vivenv.loaded or Env().viv_force:
+                        vivenv.create()
+                        vivenv.install_pkgs()
 
-        vivenv.touch()
-        vivenv.meta.write()
+                    vivenv.touch()
+                    vivenv.meta.write()
 
-        sys.exit(subprocess.run([vivenv.path / "bin" / bin, *args.rest]).returncode)
+                    sys.exit(
+                        subprocess.run([vivenv.python, scriptpath, *rest]).returncode
+                    )
+
+        else:
+            _, bin = self._pick_bin(reqs, bin)
+            vivenv = ViVenv(spec)
+
+            # TODO: respect a VIV_RUN_MODE env variable as the same as keep i.e.
+            # ephemeral (default), semi-ephemeral (persist inside /tmp), or
+            # persist (use c.cache)
+
+            if not vivenv.loaded or Env().viv_force:
+                if not keep:
+                    with tempfile.TemporaryDirectory(prefix="viv-") as tmpdir:
+                        vivenv.set_path(Path(tmpdir))
+                        vivenv.create()
+                        vivenv.install_pkgs()
+                        sys.exit(
+                            subprocess.run(
+                                [vivenv.path / "bin" / bin, *rest]
+                            ).returncode
+                        )
+                else:
+                    vivenv.create()
+                    vivenv.install_pkgs()
+
+            vivenv.touch()
+            vivenv.meta.write()
+
+            sys.exit(subprocess.run([vivenv.path / "bin" / bin, *rest]).returncode)
 
 
 class Arg:
     def __init__(self, *args: str, **kwargs: Any) -> None:
         self.args = args
         self.kwargs = kwargs
 
@@ -1262,22 +1499,38 @@
                 "-o",
                 "--output",
                 help="path/to/output file",
                 type=Path,
                 metavar="<path>",
             ),
         ],
-        ("remove",): [Arg("vivenv", help="name/hash of vivenv", nargs="*")],
-        ("exe", "info"): [Arg("vivenv", help="name/hash of vivenv")],
+        ("info",): [
+            Arg(
+                "-p",
+                "--path",
+                help="print the absolute path to the vivenv",
+                action="store_true",
+            ),
+        ],
+        ("remove",): [
+            Arg("vivenvs", help="name/hash of vivenv", nargs="*", metavar="vivenv")
+        ],
+        ("run",): [
+            Arg("-s", "--script", help="remote script to run", metavar="<script>")
+        ],
+        ("exe", "info"): [
+            Arg("vivenv_id", help="name/hash of vivenv", metavar="vivenv")
+        ],
         ("list", "info"): [
             Arg(
                 "--json",
                 help="name:metadata json for vivenvs ",
                 action="store_true",
                 default=False,
+                dest="use_json",
             )
         ],
         ("freeze", "shim"): [
             Arg(
                 "-p",
                 "--path",
                 help="generate line to add viv to sys.path",
@@ -1287,26 +1540,29 @@
                 "-s",
                 "--standalone",
                 help="generate standalone activation function",
                 action="store_true",
             ),
         ],
         ("run", "freeze", "shim"): [
-            Arg(
-                "-k",
-                "--keep",
-                help="preserve environment",
-                action="store_true",
-            ),
             Arg("reqs", help="requirements specifiers", nargs="*"),
             Arg(
                 "-r",
                 "--requirements",
                 help="path/to/requirements.txt file",
                 metavar="<path>",
+                type=Path,
+            ),
+        ],
+        ("run", "freeze"): [
+            Arg(
+                "-k",
+                "--keep",
+                help="preserve environment",
+                action="store_true",
             ),
         ],
         ("run", "shim"): [
             Arg("-b", "--bin", help="console_script/script to invoke", metavar="<bin>"),
         ],
         ("manage|purge", "manage|update", "manage|install"): [
             Arg(
@@ -1316,34 +1572,37 @@
                 default="latest",
                 metavar="<ref>",
             ),
             Arg(
                 "-s",
                 "--src",
                 help="path/to/source_file",
-                default=c.srcdefault,
+                default=Cfg().src,
                 metavar="<src>",
             ),
             Arg(
                 "-c",
                 "--cli",
                 help="path/to/cli (symlink to src)",
                 default=Path.home() / ".local" / "bin" / "viv",
                 metavar="<cli>",
             ),
         ],
-        "manage|show": [
+        ("shim", "manage|purge", "manage|update", "manage|install"): [
+            Arg("-y", "--yes", help="respond yes to all prompts", action="store_true")
+        ],
+        ("manage|show",): [
             Arg(
                 "-p",
                 "--pythonpath",
                 help="show the path/to/install",
                 action="store_true",
             )
         ],
-        ("exe"): [
+        ("exe",): [
             Arg(
                 "cmd",
                 help="command to to execute",
             )
         ],
     }
     (
@@ -1371,78 +1630,84 @@
                 )
             }
         }
     )
 
     def __init__(self, viv: Viv) -> None:
         self.viv = viv
-        self.parser = ArgumentParser(prog=viv.name, description=t.description)
+        self.parser = ArgumentParser(
+            prog=viv.name, description=viv.t.description(viv.name)
+        )
         self._cmd_arg_group_map()
-        self._make_parsers()
+        self.parsers = self._make_parsers()
         self._add_args()
 
     def _cmd_arg_group_map(self) -> None:
         self.cmd_arg_group_map: Dict[str, List[Sequence[str] | str]] = {}
         for grp in self.args:
             if isinstance(grp, str):
                 self.cmd_arg_group_map.setdefault(grp, []).append(grp)
             else:
                 for cmd in grp:
                     self.cmd_arg_group_map.setdefault(cmd, []).append(grp)
 
-    def _make_parsers(self) -> None:
-        self.parsers = {**{grp: ArgumentParser(add_help=False) for grp in self.args}}
+    def _make_parsers(self) -> Dict[Sequence[str] | str, ArgumentParser]:
+        return {**{grp: ArgumentParser(add_help=False) for grp in self.args}}
 
     def _add_args(self) -> None:
         for grp, args in self.args.items():
             for arg in args:
                 self.parsers[grp].add_argument(*arg.args, **arg.kwargs)
 
     def _validate_args(self, args: Namespace) -> None:
-        if args.func.__name__ in ("freeze", "shim", "run"):
+        if args.func.__name__ in ("freeze", "shim"):
             if not args.reqs:
-                error("must specify a requirement", code=1)
+                error("must specify a requirement")
         if args.func.__name__ in ("freeze", "shim"):
             if not self.viv.local_source and not (args.standalone or args.path):
-                warn(
+                log.warning(
                     "failed to find local copy of `viv` "
                     "make sure to add it to your PYTHONPATH "
                     "or consider using --path/--standalone"
                 )
 
+            # TODO: move this since this is code logic not flag logic
             if args.path and not self.viv.local_source:
-                error("No local viv found to import from", code=1)
+                error("No local viv found to import from")
 
             if args.path and args.standalone:
-                error("-p/--path and -s/--standalone are mutually exclusive", code=1)
+                error("-p/--path and -s/--standalone are mutually exclusive")
 
-        if args.func.__name__ == "manage":
-            if args.subcmd == "install" and self.viv.local_source:
-                error(f"found existing viv installation at {self.viv.local_source}")
-                echo(
-                    "use "
-                    + a.style("viv manage update", "bold")
-                    + " to modify current installation.",
-                    style="red",
+        if args.func.__name__ == "manage_install" and self.viv.local_source:
+            error(
+                f"found existing viv installation at {self.viv.local_source}",
+                "use "
+                + a.style("viv manage update", "bold")
+                + " to modify current installation.",
+            )
+
+        if args.func.__name__ == "manage_update":
+            if not self.viv.local_source:
+                error(
+                    a.style("viv manage update", "bold")
+                    + " should be used with an exisiting installation",
                 )
-                sys.exit(1)
-            if args.subcmd == "update":
-                if not self.viv.local_source:
-                    error(
-                        a.style("viv manage update", "bold")
-                        + " should be used with an exisiting installation",
-                        1,
-                    )
 
-                if self.viv.git:
-                    error(
-                        a.style("viv manage update", "bold")
-                        + " shouldn't be used with a git-based installation",
-                        1,
-                    )
+            if self.viv.git:
+                error(
+                    a.style("viv manage update", "bold")
+                    + " shouldn't be used with a git-based installation",
+                )
+        if args.func.__name__ == "run":
+            if not (args.reqs or args.script):
+                error("must specify a requirement or --script")
+
+        if args.func.__name__ == "info":
+            if args.use_json and args.path:
+                error("--json and -p/--path are mutually exclusive")
 
     def _get_subcmd_parser(
         self,
         subparsers: _SubParsersAction[ArgumentParser],
         name: str,
         attr: Optional[str] = None,
         **kwargs: Any,
@@ -1487,34 +1752,37 @@
                     subcmd_cmd_p.add_parser(
                         subcmd,
                         parents=[
                             self.parsers[k]
                             for k in self.cmd_arg_group_map[f"{cmd}|{subcmd}"]
                         ],
                         **kwargs,
-                    ).set_defaults(func=getattr(self.viv, cmd), subcmd=subcmd)
+                        # ).set_defaults(func=getattr(self.viv, cmd), subcmd=subcmd)
+                    ).set_defaults(func=getattr(self.viv, f"{cmd}_{subcmd}"))
 
             else:
                 self._get_subcmd_parser(
                     cmd_p,
                     cmd,
                     parents=[self.parsers.get(k) for k in self.cmd_arg_group_map[cmd]],
                 )
 
         if "--" in sys.argv:
             i = sys.argv.index("--")
             args = self.parser.parse_args(sys.argv[1:i])
             args.rest = sys.argv[i + 1 :]
         else:
             args = self.parser.parse_args()
-            args.rest = []
+            if args.func.__name__ in ("run", "exe"):
+                args.rest = []
 
         self._validate_args(args)
-        args.func(
-            args,
+        func = args.__dict__.pop("func")
+        func(
+            **vars(args),
         )
 
 
 def main() -> None:
     viv = Viv()
     Cli(viv).run()
```

### Comparing `viv-23.5a5/PKG-INFO` & `viv-23.5a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viv
-Version: 23.5a5
+Version: 23.5a6
 Summary: viv isn't venv
 License: MIT
 Author-email: Daylin Morgan <daylinmorgan@gmail.com>
 Requires-Python: >= 3.8
 Project-URL: homepage, https://github.com/daylinmorgan/viv
 Project-URL: repository, https://github.com/daylinmorgan/viv
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viv Version: 23.5a5 Summary: viv isn't venv
+Metadata-Version: 2.1 Name: viv Version: 23.5a6 Summary: viv isn't venv
 License: MIT Author-email: Daylin Morgan
 gmail.com> Requires-Python: >= 3.8 Project-URL: homepage, https://github.com/
 daylinmorgan/viv Project-URL: repository, https://github.com/daylinmorgan/viv
 Description-Content-Type: text/markdown
                                     [Logo]
                          ****** viv isn't venv ******
                                [cli screenshot]
```

