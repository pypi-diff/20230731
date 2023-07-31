# Comparing `tmp/dataclass_binder-0.3.2.tar.gz` & `tmp/dataclass_binder-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_binder-0.3.2.tar", max compression
+gzip compressed data, was "dataclass_binder-0.3.3.tar", max compression
```

## Comparing `dataclass_binder-0.3.2.tar` & `dataclass_binder-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-07-27 01:34:05.108884 dataclass_binder-0.3.2/LICENSE
--rw-r--r--   0        0        0    18141 2023-07-27 01:34:05.108884 dataclass_binder-0.3.2/README.md
--rw-r--r--   0        0        0     2550 2023-07-27 01:34:28.332758 dataclass_binder-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      172 2023-07-27 01:34:05.108884 dataclass_binder-0.3.2/src/dataclass_binder/__init__.py
--rw-r--r--   0        0        0    35105 2023-07-27 01:34:05.108884 dataclass_binder-0.3.2/src/dataclass_binder/_impl.py
--rw-r--r--   0        0        0        0 2023-07-27 01:34:05.108884 dataclass_binder-0.3.2/src/dataclass_binder/py.typed
--rw-r--r--   0        0        0    19536 1970-01-01 00:00:00.000000 dataclass_binder-0.3.2/setup.py
--rw-r--r--   0        0        0    19057 1970-01-01 00:00:00.000000 dataclass_binder-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-31 13:46:28.774212 dataclass_binder-0.3.3/LICENSE
+-rw-r--r--   0        0        0    19287 2023-07-31 13:46:28.774212 dataclass_binder-0.3.3/README.md
+-rw-r--r--   0        0        0     2550 2023-07-31 13:46:50.474477 dataclass_binder-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-07-31 13:46:28.774212 dataclass_binder-0.3.3/src/dataclass_binder/__init__.py
+-rw-r--r--   0        0        0    36974 2023-07-31 13:46:28.774212 dataclass_binder-0.3.3/src/dataclass_binder/_impl.py
+-rw-r--r--   0        0        0        0 2023-07-31 13:46:28.774212 dataclass_binder-0.3.3/src/dataclass_binder/py.typed
+-rw-r--r--   0        0        0    20725 1970-01-01 00:00:00.000000 dataclass_binder-0.3.3/setup.py
+-rw-r--r--   0        0        0    20203 1970-01-01 00:00:00.000000 dataclass_binder-0.3.3/PKG-INFO
```

### Comparing `dataclass_binder-0.3.2/LICENSE` & `dataclass_binder-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclass_binder-0.3.2/README.md` & `dataclass_binder-0.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -449,14 +449,51 @@
 
 # TCP port on which to accept connections.
 # Default:
 # port = 12345
 port = 8080
 ```
 
+### Generating a Compact Configuration File
+
+If you want to generate a fully populated configuration, you can use the `format_toml()` method.
+Compared to the template formatting, this leaves out optional parts for which no data has been provided.
+
+For example, when the following dataclass defines your configuration:
+
+```py
+@dataclass
+class Config:
+    path: str
+    """Path of input file."""
+
+    verbose: bool = False
+    """Be extra verbose in logging."""
+
+    options: dict[str, Any] = field(default_factory=dict)
+    """Various named options that are passed on to tool XYZ."""
+```
+
+This code generates a populated configuration file:
+
+```py
+config = Config(path="./data")
+
+with open("config.toml", "w") as out:
+    for line in Binder(config).format_toml():
+        print(line, file=out)
+```
+
+With the contents of `config.toml` containing only the `path` field:
+
+```toml
+# Path of input file.
+path = './data'
+```
+
 ### Troubleshooting
 
 Finally, a troubleshooting tip: instead of the full `Binder(Config).parse_toml()`, first try to execute only `Binder(Config)`.
 If that fails, the problem is in the dataclass definitions.
 If that succeeds, but the `parse_toml()` call fails, the problem is that the TOML file does not match the format defined in the dataclasses.
 
 
@@ -531,9 +568,13 @@
 
 - Generate template in depth-first order ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))
 - Fix binder creation and formatting for recursive dataclasses ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))
 
 ### 0.3.2 - 2023-07-27:
 
 - Document fields with a `default_factory` as optional in template ([#35](https://github.com/ProtixIT/dataclass-binder/pull/35))
-- Omit values that are formatted equally to the default ([#36](https://github.com/ProtixIT/dataclass-binder/pull/36))
-- Require optional fields to have `None` as their default ([#37](https://github.com/ProtixIT/dataclass-binder/pull/37))
+- Omit values from template that are formatted equally to the default ([#36](https://github.com/ProtixIT/dataclass-binder/pull/36))
+- Require fields with `None` in their annotation to have `None` as their default ([#37](https://github.com/ProtixIT/dataclass-binder/pull/37))
+
+### 0.3.3 - 2023-07-31:
+
+- Add `Binder.format_toml()` method to generate more compact TOML that excludes unused optional parts ([#38](https://github.com/ProtixIT/dataclass-binder/pull/38))
```

### Comparing `dataclass_binder-0.3.2/pyproject.toml` & `dataclass_binder-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-binder"
-version = "0.3.2"
+version = "0.3.3"
 description = "Library to bind TOML data to Python dataclasses in a type-safe way."
 authors = [
     "Maarten ter Huurne <maarten.terhuurne@protix.eu>",
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ProtixIT/dataclass-binder"
```

### Comparing `dataclass_binder-0.3.2/src/dataclass_binder/_impl.py` & `dataclass_binder-0.3.3/src/dataclass_binder/_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -426,34 +426,51 @@
             )
 
         if instance is None:
             return self._dataclass(**parsed)
         else:
             return replace(instance, **parsed)  # type: ignore[type-var]
 
+    def format_toml(self) -> Iterator[str]:
+        """
+        Yield lines of TOML text for populating the dataclass or object that we are binding to.
+
+        If we are binding to an object, non-default values from that object will be output.
+
+        If we are binding to a class, example values for mandatory fields will be derived from the field types;
+        these example values can be syntactically incorrect placeholders.
+        """
+
+        return self._format_toml_root(template=False)
+
     def format_toml_template(self) -> Iterator[str]:
         """
         Yield lines of TOML text as a template for populating the dataclass or object that we are binding to.
 
         A template in this case means it is suitable as a starting point for a user to fill in;
         the template is not guaranteed to be parseable as-is.
 
         If we are binding to an object, values from that object will be used to populate the template.
         If we are binding to a class, example values will be derived from the field types.
         """
 
+        return self._format_toml_root(template=True)
+
+    def _format_toml_root(self, *, template: bool) -> Iterator[str]:
         table = Table(self, "", self._instance, None)
-        lines = table.format_table(set())
+        lines = table.format_table(set(), template=template)
         for line in lines:
             if line:
                 yield line
                 break
         yield from lines
 
-    def _format_toml_table(self, instance: T | None, defer: Callable[[Table[Any]], None]) -> Iterator[str]:
+    def _format_toml_table(
+        self, instance: T | None, defer: Callable[[Table[Any]], None], *, template: bool
+    ) -> Iterator[str]:
         dataclass = self._dataclass
         field_types = self._class_info.field_types
         docstrings = self._class_info.field_docstrings
 
         for field in fields(dataclass):  # type: ignore[arg-type]
             if not field.init:
                 continue
@@ -490,49 +507,58 @@
                                 f"{key_fmt}.{''.join(_iter_format_key(nested_key))}": nested_value
                                 for nested_key, nested_value in value.items()
                             }
                         for nested_key_fmt, nested_value in nested_map.items():
                             defer(Table(value_type, nested_key_fmt, nested_value, docstring))
                         continue
                     if value_type is object:  # Any
-                        defer(Table(None, key_fmt, value, docstring, optional))
+                        if template or value or default:
+                            defer(Table(None, key_fmt, value, docstring, optional))
                         continue
                 elif issubclass(origin, Sequence):
                     (value_type,) = get_args(field_type)
                     binder = value_type if isinstance(value_type, Binder) else None
                     if binder is not None or (
                         value_type is object  # Any
                         and (value is None or all(isinstance(item, Mapping) or is_dataclass(item) for item in value))
                     ):
                         nested_key_fmt = f"[{key_fmt}]"
                         for nested_value in [None] if value is None else value:
                             defer(Table(binder, nested_key_fmt, nested_value, docstring, optional))
                         continue
 
-            yield ""
+            default_fmt = None if default is MISSING or default is None else format_toml_pair(key, default)
 
-            comments = [docstring]
-            if not optional or default is None:
-                fmt_default = None
-                comments.append("Optional." if default is None else "Mandatory.")
+            if value is not None:
+                value_fmt: str | None = format_toml_pair(key, value)
+                if value_fmt == default_fmt:
+                    value_fmt = None
+            elif optional:
+                value_fmt = None
             else:
-                fmt_default = format_toml_pair(key, default)
-                comments.append(f"Default:\n{fmt_default}")
-            yield from _format_comments(*comments)
-
-            if value is None:
-                if not optional or default is None:
-                    comment = "# " if default is None else ""
-                    key_fmt = "".join(_iter_format_key(key))
-                    value_fmt = _format_value_for_type(field_type)
-                    yield f"{comment}{key_fmt} = {value_fmt}"
-            else:
-                fmt_value = format_toml_pair(key, value)
-                if fmt_value != fmt_default:
-                    yield fmt_value
+                # Make up an example value.
+                value_fmt = f"{key_fmt} = {_format_value_for_type(field_type)}"
+
+            if template or value_fmt is not None:
+                comments = [docstring]
+                if template:
+                    if not optional:
+                        comments.append("Mandatory.")
+                    elif default_fmt is not None:
+                        comments.append(f"Default:\n{default_fmt}")
+                    elif value_fmt is not None:
+                        # We don't need an example value in the comment if we're outputting a value line.
+                        comments.append("Optional.")
+                    else:
+                        # We have no value; we do have a default but it's unformattable.
+                        comments.append(f"Optional.\n{key_fmt} = {_format_value_for_type(field_type)}")
+                yield from _format_comments(*comments, leading_newline=True)
+
+            if value_fmt is not None:
+                yield value_fmt
 
     if TYPE_CHECKING:
         # These definitions exist to support the deprecated `Binder[DC]` syntax in mypy.
 
         @classmethod
         def bind(cls, data: Mapping[str, Any]) -> T:
             ...
@@ -570,55 +596,63 @@
     def class_docstring(self) -> str | None:
         binder = self.binder
         return None if binder is None else binder._class_info.class_docstring
 
     def prefix_context(self, context: str) -> Table[T]:
         return replace(self, key_fmt=f"{context}.{self.key_fmt}" if context else self.key_fmt)
 
-    def format_table(self, inside: Set[type]) -> Iterator[str]:
+    def format_table(self, inside: Set[type], *, template: bool) -> Iterator[str]:
         """
         The `inside` parameter keeps track of which dataclasses we are currently outputting,
         to prevent infinite recursion.
         """
 
         child_tables: list[Table[Any]] = []
         context = self.key_fmt
         value = self.value
 
+        if template:
+            defer = child_tables.append
+        else:
+
+            def defer(table: Table) -> None:
+                if table.value is not None or not table.optional:
+                    child_tables.append(table)
+
         if (binder := self.binder) is None:
             match value:
                 case Mapping() as mapping:
                     content = [format_toml_pair(k, v) for k, v in mapping.items()]
                 case dc if is_dataclass(dc):
                     content = [format_toml_pair(k, v) for k, v in asdict(dc).items()]  # type: ignore[arg-type]
                 case _:
                     content = []
         elif value is None and binder._dataclass in inside:
             content = None
         else:
             inside |= {binder._dataclass}
-            content = list(binder._format_toml_table(value, child_tables.append))
+            content = list(binder._format_toml_table(value, defer=defer, template=template))
             if not content:
                 content = None
 
         if content is not None:
             if context:
-                yield from self.format_header()
+                yield from self.format_header(template=template)
 
             yield from content
 
         for table in child_tables:
-            yield from table.prefix_context(context).format_table(inside)
+            yield from table.prefix_context(context).format_table(inside, template=template)
 
-    def format_header(self) -> Iterator[str]:
+    def format_header(self, *, template: bool) -> Iterator[str]:
         yield ""
         yield from _format_comments(
             self.class_docstring,
             self.field_docstring,
-            "Optional table." if self.optional else None,
+            "Optional table." if template and self.optional else None,
         )
         yield f"[{self.key_fmt}]"
 
 
 def format_toml_pair(key: str, value: object) -> str:
     """Format a key/value pair as TOML text."""
     suffix, data = _to_toml_pair(value)
@@ -708,48 +742,52 @@
     yield from _iter_format_value(value)
 
 
 def _iter_format_key(key: str) -> Iterator[str]:
     if _TOML_BARE_KEY.match(key):
         yield key
     else:
-        yield from _iter_format_value(key)
+        yield from _iter_format_string(key)
+
+
+def _iter_format_string(value: str) -> Iterator[str]:
+    # Ideally we could assume that every tool along the way defaults to UTF-8 and just output that,
+    # but I don't think we live in that world yet, so escape non-ASCII characters.
+    if value.isprintable() and value.isascii() and "'" not in value:
+        # Use a literal string if possible.
+        yield "'"
+        yield value
+        yield "'"
+    else:
+        # Use basic string otherwise.
+        yield '"'
+        for ch in value:
+            if ch.isascii():
+                try:
+                    yield _TOML_ESCAPES[ch]
+                except KeyError:
+                    if ch.isprintable():
+                        yield ch
+                    else:
+                        yield f"\\u{ord(ch):04X}"
+            elif ord(ch) < 0x10000:
+                yield f"\\u{ord(ch):04X}"
+            else:
+                yield f"\\U{ord(ch):08X}"
+        yield '"'
 
 
 def _iter_format_value(value: object) -> Iterator[str]:
     match value:
         case bool():
             yield str(value).lower()
         case int() | float():
             yield str(value)
         case str():
-            # Ideally we could assume that every tool along the way defaults to UTF-8 and just output that,
-            # but I don't think we live in that world yet, so escape non-ASCII characters.
-            if value.isprintable() and value.isascii() and "'" not in value:
-                # Use a literal string if possible.
-                yield "'"
-                yield value
-                yield "'"
-            else:
-                # Use basic string otherwise.
-                yield '"'
-                for ch in value:
-                    if ch.isascii():
-                        try:
-                            yield _TOML_ESCAPES[ch]
-                        except KeyError:
-                            if ch.isprintable():
-                                yield ch
-                            else:
-                                yield f"\\u{ord(ch):04X}"
-                    elif ord(ch) < 0x10000:
-                        yield f"\\u{ord(ch):04X}"
-                    else:
-                        yield f"\\U{ord(ch):08X}"
-                yield '"'
+            yield from _iter_format_string(value)
         case date() | time():
             yield value.isoformat()
         case Mapping():
             first = True
             yield "{"
             for key, elem in value.items():
                 if first:
@@ -768,18 +806,30 @@
                     yield ", "
                 yield from _iter_format_value(elem)
             yield "]"
         case _:
             raise TypeError(type(value).__name__)
 
 
-def _format_comments(*comments: str | None) -> Iterator[str]:
+def _format_comments(*comments: str | None, leading_newline: bool = False) -> Iterator[str]:
+    """
+    Yield lines containing a formatted version of the given comments.
+
+    Comments that are None will be ignored.
+    If `leading_newline` is True, an empty ine will be output before any comment lines,
+    but only if the output is non-empty.
+    """
+
     separator = False
     for comment in comments:
         if comment:
+            if leading_newline:
+                yield ""
+                leading_newline = False
+
             contains_empty = False
             for line in comment.split("\n"):
                 if separator:
                     yield "#"
                     separator = False
                 yield f"# {line}".rstrip()
                 contains_empty |= not line
```

### Comparing `dataclass_binder-0.3.2/setup.py` & `dataclass_binder-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'dataclass-binder',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'Library to bind TOML data to Python dataclasses in a type-safe way.',
-    'long_description': '# Dataclass Binder\n\nLibrary to bind TOML data to Python dataclasses in a type-safe way.\n\n\n## Features\n\nCurrently it has the following properties that might set it apart from other data binding libraries:\n\n- requires Python 3.10+\n- relies only on dataclasses from the Python standard library\n- detailed error messages which mention location, expected data and actual data\n- strict parsing which considers unknown keys to be errors\n- support for durations (`timedelta`)\n- support for immutable (frozen) dataclasses\n- can bind data from files, I/O streams or pre-parsed dictionaries\n- can generate configuration templates from dataclass definitions\n\nThis library was originally designed for parsing configuration files.\nAs TOML\'s data model is very similar to JSON\'s, adding support for JSON in the future would be an option and would make the library useful for binding HTTP API requests.\n\n\n## Maturity\n\nThis library is fully type-checked, has unit tests which provide 100% branch coverage and is used in production, so it should be reliable.\n\nThe API might still change in incompatible ways until the 1.0 release.\nIn particular the following aspects are subject to change:\n\n- use of key suffixes for `timedelta`: this mechanism doesn\'t work for arrays\n- the handling of separators in keys: currently `-` in TOML is mapped to `_` in Python and `_` is forbidden in TOML; most applications seem to accept both `-` and `_` in TOML instead\n\n\n## Why Dataclasses?\n\nA typical TOML, JSON or YAML parser returns the parse results as a nested dictionary.\nYou might wonder why you would want to use a data binding library rather than just getting the values directly from that dictionary.\n\nLet\'s take the following example code for a service that connects to a database using a connection URL configured in a TOML file:\n\n```py\nimport tomllib  # or \'tomli\' on Python <3.11\n\n\ndef read_config() -> dict:\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n    return config\n\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    print("connect to database:", url)\n\nconfig = read_config()\n...\nhandle_request(config)\n```\n\nIf the configuration is missing a `database-url` key or its value is not a string, this service would start up without complaints and then fail when the first requests comes in.\nIt would be better to instead check the configuration on startup, so let\'s add code for that:\n\n```py\ndef read_config():\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n\n    url = config["database-url"]\n    if not isinstance(url, str):\n        raise TypeError(\n            f"Value for \'database-url\' has type \'{type(url).__name__}\', expected \'str\'"\n        )\n\n    return config\n```\n\nImagine you have 20 different configurable options: you\'d need this code 20 times.\n\nNow let\'s assume that you use a type checker like `mypy`.\nInside `read_config()`, the type checker will know that `url` is a `str`, but if you fetch the same value elsewhere in the code, that information is lost:\n\n```py\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    reveal_type(url)\n    print("connect to database:", url)\n```\n\nWhen you run `mypy` on this code, it will output \'Revealed type is "Any"\'.\nFalling back to `Any` means type checking will not be able to find type mismatches and autocomplete in an IDE will not work well either.\n\nDeclaring the desired type in a dataclass solves both these issues:\n- the type can be verified at runtime before instantiating the dataclass\n- tooling knows the type when you read the value from the dataclass\n\nHaving the dataclass as a central and formal place for defining the configuration format is also an advantage.\nFor example, it enables automatic generation of a documented configuration file template.\n\n\n## Usage\n\nThe `dataclass_binder` module contains the `Binder` class which makes it easy to bind TOML data, such as a configuration file, to Python [dataclasses](https://docs.python.org/3/library/dataclasses.html).\n\nThe binding is a two-step process:\n- instantiate the `Binder` class by passing your top-level dataclass as an argument\n- call the `parse_toml()` method, providing the path of the configuration file as its argument\n\nPut together, the code looks like this:\n\n```py\nimport logging\nimport sys\nfrom pathlib import Path\n\nfrom dataclass_binder import Binder\n\n\nlogger = logging.getLogger(__name__)\n\nif __name__ == "__main__":\n    config_file = Path("config.toml")\n    try:\n        config = Binder(Config).parse_toml(config_file)\n    except Exception as ex:\n        logger.critical("Error reading configuration file \'%s\': %s", config_file, ex)\n        sys.exit(1)\n```\n\n### Binding a Pre-parsed Dictionary\n\nIf you don\'t want to bind the contents of a full file, there is also the option to bind a pre-parsed dictionary instead.\nFor this, you can use the `bind()` method on the `Binder` object.\n\nFor example, the following service is configured by one table within a larger TOML configuration file:\n\n```py\nimport tomllib  # or \'tomli\' on Python <3.11\nfrom dataclass_binder import Binder\n\n\nwith open("config.toml", "rb") as f:\n    config = tomllib.load(f)\nservice_config = Binder(ServiceConfig).bind(config["service"])\n```\n\nTo keep these examples short, from now on `import` statements will only be included the first time a particular imported name is used.\n\n### Basic Types\n\nDataclass fields correspond to TOML keys. In the dataclass, underscores are used as word separators, while dashes are used in the TOML file. Let\'s configure a service that listens on a TCP port for requests and stores its data in a database, using the following TOML fragment:\n\n```toml\ndatabase-url = \'postgresql://user:password@host/db\'\nport = 8080\n```\n\nThis configuration can be bound to the following dataclass:\n\n```py\nfrom dataclasses import dataclass\n\n@dataclass\nclass Config:\n    database_url: str\n    port: int\n    verbose: bool\n```\n\nThe `float` type can be used to bind floating point numbers.\nSupport for `Decimal` is not there at the moment but would be relatively easy to add, as `tomllib`/`tomli` has an option for that.\n\n### Defaults\n\nFields can be made optional by assigning a default value. Using `None` as a default value is allowed too:\n\n```py\n@dataclass\nclass Config:\n    verbose: bool = False\n    webhook_url: str | None = None\n```\n\nIf you want to mix fields with and without defaults in any order, mark the fields as keyword-only:\n\n```py\n@dataclass(kw_only=True)\nclass Config:\n    database_url: str\n    verbose: bool = False\n    port: int\n```\n\n### Dates and Times\n\nTOML handles dates and timestamps as first-class values.\nDate, time and date+time TOML values are bound to `datetime.date`, `datetime.time` and `datetime.datetime` Python objects respectively.\n\nThere is also support for time intervals using `datetime.timedelta`:\n\n```py\nfrom datetime import timedelta\n\n@dataclass\nclass Config:\n    retry_after: timedelta\n    delete_after: timedelta\n```\n\nIntervals shorter than a day can be specified using a TOML time value.\nLonger intervals are supported by adding an `-hours`, `-days`, or `-weeks` suffix.\nOther supported suffixes are `-minutes`, `-seconds`, `-milliseconds` and `-microseconds`, but these are there for completeness sake and less likely to be useful.\nHere is an example TOML fragment corresponding to the dataclass above:\n\n```toml\nretry-after = 00:02:30\ndelete-after-days = 30\n```\n\n### Collections\n\nLists and dictionaries can be used to bind TOML arrays and tables.\nIf you want to make a `list` or `dict` optional, you need to provide a default value via the `default_factory` mechanism as usual, see the [dataclasses documentation](https://docs.python.org/3/library/dataclasses.html#mutable-default-values) for details.\n\n```py\nfrom dataclasses import dataclass, field\n\n@dataclass\nclass Config:\n    tags: list[str] = field(default_factory=list)\n    limits: dict[str, int]\n```\n\nThe dataclass above can be used to bind the following TOML fragment:\n\n```toml\ntags = ["production", "development"]\nlimits = {ram-gb = 1, disk-gb = 100}\n```\n\nAn alternative to `default_factory` is to use a homogeneous (single element type) tuple:\n\n```py\n@dataclass\nclass Config:\n    tags: tuple[str, ...] = ()\n    limits: dict[str, int]\n```\n\nHeterogeneous tuples are supported too: for example `tuple[str, bool]` binds a TOML array that must always have a string as its first element and a Boolean as its second and last element.\nIt is generally clearer though to define a separate dataclass when you need more than one value to configure something:\n\n```py\n@dataclass\nclass Webhook:\n    url: str\n    token: str\n\n@dataclass\nclass Config:\n    webhooks: tuple[Webhook, ...] = ()\n```\n\nThe extra keys (`url` and `token` in this example) provide the clarity:\n\n```toml\nwebhooks = [\n    {url = "https://host1/notify", token = "12345"},\n    {url = "https://host2/hook", token = "frperg"}\n]\n```\n\nTOML\'s array-of-tables syntax can make this configuration a bit easier on the eyes:\n\n```toml\n[[webhooks]]\nurl = "https://host1/notify"\ntoken = "12345"\n\n[[webhooks]]\nurl = "https://host2/hook"\ntoken = "frperg"\n```\n\nAlways define additional dataclasses at the module level in your Python code: if the class is for example defined inside a function, the `Binder` constructor will not be able to find it.\n\n### Untyped Data\n\nSometimes the full structure of the data you want to bind is either too complex or too much in flux to be worth fully annotating.\nIn such a situation, you can use `typing.Any` as the annotation to simply capture the output of Python\'s TOML parser without type-checking it.\n\nIn the following example, a service uses the Python standard library logging implementation, configured using the [configuration dictionary schema](https://docs.python.org/3/library/logging.config.html#logging-config-dictschema):\n\n```py\nimport logging.config\nfrom dataclasses import dataclass\nfrom typing import Any\n\nfrom dataclass_binder import Binder\n\n\n@dataclass\nclass Config:\n    database_url: str\n    logging: Any\n\n\ndef run(url: str) -> None:\n    logging.info("Service starting")\n\n\nif __name__ == "__main__":\n    config = Binder[Config].parse_toml("service.toml")\n    logging.config.dictConfig(config.logging)\n    run(config.database_url)\n```\n\nThe `service.toml` configuration file for this service could look like this:\n\n```toml\ndatabase-url = \'postgresql://user:password@host/db\'\n\n[logging]\nversion = 1\n\n[logging.root]\nlevel = \'INFO\'\nhandlers = [\'file\']\n\n[logging.handlers.file]\nclass = \'logging.handlers.RotatingFileHandler\'\nfilename = \'service.log\'\nformatter = \'simple\'\n\n[logging.formatters.simple]\nformat = \'%(asctime)s %(name)s %(levelname)s %(message)s\'\n```\n\n### Plugins\n\nTo select plugins to activate, you can bind Python classes or modules using `type[BaseClass]` and `types.ModuleType` annotations respectively:\n\n```py\nfrom dataclasses import dataclass, field\nfrom types import ModuleType\n\nfrom supertool.plugins import PostProcessor\n\n\n@dataclass\nclass PluginConfig:\n    postprocessors = tuple[type[PostProcessor], ...] = ()\n    modules: dict[str, ModuleType] = field(default_factory=dict)\n```\n\nIn the TOML, you specify Python classes or modules using their fully qualified names:\n\n```toml\npostprocessors = ["supertool_addons.reporters.JSONReport"]\nmodules = {lint = "supertool_addons.linter"}\n```\n\nThere is no mechanism yet to add configuration to be used by the plugins.\n\n### Immutable\n\nIf you prefer immutable configuration objects, you can achieve that using the `frozen` argument of the `dataclass` decorator and using abstract collection types in the annotations. For example, the following dataclass will be instantiated with a `tuple` object for `tags` and an immutable dictionary view for `limits`:\n\n```py\nfrom collections.abc import Mapping, Sequence\n\n\n@dataclass(frozen=True)\nclass Config:\n    tags: Sequence[str] = ()\n    limits: Mapping[str, int]\n```\n\n### Layered Binding\n\n`Binder` can be instantiated from a dataclass object rather than the dataclass itself.\nThe dataclass object will provide new default values when binding data to it.\nThis can be used to implement a layered configuration parsing mechanism, where there is a default configuration that can be customized using a system-wide configuration file and/or a per-user configuration file:\n\n```py\nconfig = Config()\nif system_config_path.exists():\n    config = Binder(config).parse_toml(system_config_path)\nif user_config_path.exists():\n    config = Binder(config).parse_toml(user_config_path)\n```\n\nLater layers can override individual fields in nested dataclasses, allowing fine-grained configuration merging, but collections are replaced whole instead of merged.\n\n### Generating a Configuration Template\n\nTo provide users with a starting point for configuring your application/service, you can automatically generate a configuration template from the information in the dataclass.\n\nFor example, when the following dataclass defines your configuration:\n\n```py\n@dataclass\nclass Config:\n    database_url: str\n    """The URL of the database to connect to."""\n\n    port: int = 12345\n    """TCP port on which to accept connections."""\n```\n\nYou can generate a template configuration file using:\n\n```py\nfrom dataclass_binder import Binder\n\n\nfor line in Binder(Config).format_toml_template():\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'???\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\n```\n\nIt is also possible to provide placeholder values by passing a dataclass instance rather than the dataclass itself to `format_toml_template()`:\n\n```py\nTEMPLATE = Config(\n    database_url="postgresql://<username>:<password>@<hostname>/<database name>",\n    port=8080,\n)\n\nfor line in Binder(TEMPLATE).format_toml_template():\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'postgresql://<username>:<password>@<hostname>/<database name>\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\nport = 8080\n```\n\n### Troubleshooting\n\nFinally, a troubleshooting tip: instead of the full `Binder(Config).parse_toml()`, first try to execute only `Binder(Config)`.\nIf that fails, the problem is in the dataclass definitions.\nIf that succeeds, but the `parse_toml()` call fails, the problem is that the TOML file does not match the format defined in the dataclasses.\n\n\n## Development Environment\n\n[Poetry](https://python-poetry.org/) is used to set up a virtual environment with all the dependencies and development tools that you need:\n\n    $ cd dataclass-binder\n    $ poetry install\n\nYou can activate a shell which contains the development tools in its search path:\n\n    $ poetry shell\n\nWe recommend setting up pre-commit hooks for Git in the `dataclass-binder` work area.\nThese hooks automatically run a few simple checks and cleanups when you create a new commit.\nAfter you first set up your virtual environment with Poetry, run this command to install the pre-commit hooks:\n\n    $ pre-commit install\n\n\n## Release Procedure\n\n- Verify that CI passes on the branch that you want to release (typically `main`)\n- Create a release on the GitHub web interface; name the tag `v<major>.<minor>.<patchlevel>`\n- After publishing the release on GitHub, the package will be built and published on PyPI automatically via Actions\n\n\n## Deprecations\n\n### Binder Specialization\n\nPrior to version 0.2.0, the `Binder` class was specialized using a type argument (`Binder[Config]`) rather than instantiation (`Binder(config)`). The old syntax is still supported for now, but the backwards compatibility might be removed in a minor release prior to 1.0 if it becomes a maintenance burden, so please update your code.\n\n### Template Formatting\n\nIn version 0.3.0, the function `format_template()` has been replaced by the method `Binder.format_toml_template()`. The old function is still available for now.\n\n## Changelog\n\n### 0.1.0 - 2023-02-21:\n\n- First open source release; thanks to my employer [Protix](https://protix.eu/) for making this possible\n\n### 0.1.1 - 2023-02-22:\n\n- Relax `Binder.bind()` argument type to `Mapping` ([#3](https://github.com/ProtixIT/dataclass-binder/issues/3))\n\n### 0.1.2 - 2023-03-03:\n\n- Fix `get()` and `[]` on object bound to read-only mapping ([#6](https://github.com/ProtixIT/dataclass-binder/issues/6))\n\n### 0.1.3 - 2023-03-05:\n\n- Ignore dataclass fields with `init=False` ([#2](https://github.com/ProtixIT/dataclass-binder/issues/2))\n\n### 0.2.0 - 2023-06-26:\n\n- Instantiate `Binder` instead of specializing it ([#14](https://github.com/ProtixIT/dataclass-binder/pull/14))\n- Support `typing.Any` as a field annotation ([#10](https://github.com/ProtixIT/dataclass-binder/issues/10))\n- Fix crash in `format_template()` on optional fields with non-string annotations ([#16](https://github.com/ProtixIT/dataclass-binder/pull/16))\n\n### 0.3.0 - 2023-07-13:\n\n- Replace `format_template()` function by `Binder.format_toml_template()` method ([#23](https://github.com/ProtixIT/dataclass-binder/pull/23))\n- Format nested dataclasses as TOML tables ([#25](https://github.com/ProtixIT/dataclass-binder/pull/25))\n- Format untyped mappings and sequences as TOML tables ([#27](https://github.com/ProtixIT/dataclass-binder/pull/27))\n- Fix formatting of `init=False` field in nested dataclasses ([#22](https://github.com/ProtixIT/dataclass-binder/pull/22))\n- Fix annotation evaluation on inherited dataclasses ([#21](https://github.com/ProtixIT/dataclass-binder/pull/21))\n\n### 0.3.1 - 2023-07-17:\n\n- Generate template in depth-first order ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))\n- Fix binder creation and formatting for recursive dataclasses ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))\n\n### 0.3.2 - 2023-07-27:\n\n- Document fields with a `default_factory` as optional in template ([#35](https://github.com/ProtixIT/dataclass-binder/pull/35))\n- Omit values that are formatted equally to the default ([#36](https://github.com/ProtixIT/dataclass-binder/pull/36))\n- Require optional fields to have `None` as their default ([#37](https://github.com/ProtixIT/dataclass-binder/pull/37))\n',
+    'long_description': '# Dataclass Binder\n\nLibrary to bind TOML data to Python dataclasses in a type-safe way.\n\n\n## Features\n\nCurrently it has the following properties that might set it apart from other data binding libraries:\n\n- requires Python 3.10+\n- relies only on dataclasses from the Python standard library\n- detailed error messages which mention location, expected data and actual data\n- strict parsing which considers unknown keys to be errors\n- support for durations (`timedelta`)\n- support for immutable (frozen) dataclasses\n- can bind data from files, I/O streams or pre-parsed dictionaries\n- can generate configuration templates from dataclass definitions\n\nThis library was originally designed for parsing configuration files.\nAs TOML\'s data model is very similar to JSON\'s, adding support for JSON in the future would be an option and would make the library useful for binding HTTP API requests.\n\n\n## Maturity\n\nThis library is fully type-checked, has unit tests which provide 100% branch coverage and is used in production, so it should be reliable.\n\nThe API might still change in incompatible ways until the 1.0 release.\nIn particular the following aspects are subject to change:\n\n- use of key suffixes for `timedelta`: this mechanism doesn\'t work for arrays\n- the handling of separators in keys: currently `-` in TOML is mapped to `_` in Python and `_` is forbidden in TOML; most applications seem to accept both `-` and `_` in TOML instead\n\n\n## Why Dataclasses?\n\nA typical TOML, JSON or YAML parser returns the parse results as a nested dictionary.\nYou might wonder why you would want to use a data binding library rather than just getting the values directly from that dictionary.\n\nLet\'s take the following example code for a service that connects to a database using a connection URL configured in a TOML file:\n\n```py\nimport tomllib  # or \'tomli\' on Python <3.11\n\n\ndef read_config() -> dict:\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n    return config\n\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    print("connect to database:", url)\n\nconfig = read_config()\n...\nhandle_request(config)\n```\n\nIf the configuration is missing a `database-url` key or its value is not a string, this service would start up without complaints and then fail when the first requests comes in.\nIt would be better to instead check the configuration on startup, so let\'s add code for that:\n\n```py\ndef read_config():\n    with open("config.toml", "rb") as f:\n        config = tomllib.load(f)\n\n    url = config["database-url"]\n    if not isinstance(url, str):\n        raise TypeError(\n            f"Value for \'database-url\' has type \'{type(url).__name__}\', expected \'str\'"\n        )\n\n    return config\n```\n\nImagine you have 20 different configurable options: you\'d need this code 20 times.\n\nNow let\'s assume that you use a type checker like `mypy`.\nInside `read_config()`, the type checker will know that `url` is a `str`, but if you fetch the same value elsewhere in the code, that information is lost:\n\n```py\ndef handle_request(config: dict) -> None:\n    url = config["database-url"]\n    reveal_type(url)\n    print("connect to database:", url)\n```\n\nWhen you run `mypy` on this code, it will output \'Revealed type is "Any"\'.\nFalling back to `Any` means type checking will not be able to find type mismatches and autocomplete in an IDE will not work well either.\n\nDeclaring the desired type in a dataclass solves both these issues:\n- the type can be verified at runtime before instantiating the dataclass\n- tooling knows the type when you read the value from the dataclass\n\nHaving the dataclass as a central and formal place for defining the configuration format is also an advantage.\nFor example, it enables automatic generation of a documented configuration file template.\n\n\n## Usage\n\nThe `dataclass_binder` module contains the `Binder` class which makes it easy to bind TOML data, such as a configuration file, to Python [dataclasses](https://docs.python.org/3/library/dataclasses.html).\n\nThe binding is a two-step process:\n- instantiate the `Binder` class by passing your top-level dataclass as an argument\n- call the `parse_toml()` method, providing the path of the configuration file as its argument\n\nPut together, the code looks like this:\n\n```py\nimport logging\nimport sys\nfrom pathlib import Path\n\nfrom dataclass_binder import Binder\n\n\nlogger = logging.getLogger(__name__)\n\nif __name__ == "__main__":\n    config_file = Path("config.toml")\n    try:\n        config = Binder(Config).parse_toml(config_file)\n    except Exception as ex:\n        logger.critical("Error reading configuration file \'%s\': %s", config_file, ex)\n        sys.exit(1)\n```\n\n### Binding a Pre-parsed Dictionary\n\nIf you don\'t want to bind the contents of a full file, there is also the option to bind a pre-parsed dictionary instead.\nFor this, you can use the `bind()` method on the `Binder` object.\n\nFor example, the following service is configured by one table within a larger TOML configuration file:\n\n```py\nimport tomllib  # or \'tomli\' on Python <3.11\nfrom dataclass_binder import Binder\n\n\nwith open("config.toml", "rb") as f:\n    config = tomllib.load(f)\nservice_config = Binder(ServiceConfig).bind(config["service"])\n```\n\nTo keep these examples short, from now on `import` statements will only be included the first time a particular imported name is used.\n\n### Basic Types\n\nDataclass fields correspond to TOML keys. In the dataclass, underscores are used as word separators, while dashes are used in the TOML file. Let\'s configure a service that listens on a TCP port for requests and stores its data in a database, using the following TOML fragment:\n\n```toml\ndatabase-url = \'postgresql://user:password@host/db\'\nport = 8080\n```\n\nThis configuration can be bound to the following dataclass:\n\n```py\nfrom dataclasses import dataclass\n\n@dataclass\nclass Config:\n    database_url: str\n    port: int\n    verbose: bool\n```\n\nThe `float` type can be used to bind floating point numbers.\nSupport for `Decimal` is not there at the moment but would be relatively easy to add, as `tomllib`/`tomli` has an option for that.\n\n### Defaults\n\nFields can be made optional by assigning a default value. Using `None` as a default value is allowed too:\n\n```py\n@dataclass\nclass Config:\n    verbose: bool = False\n    webhook_url: str | None = None\n```\n\nIf you want to mix fields with and without defaults in any order, mark the fields as keyword-only:\n\n```py\n@dataclass(kw_only=True)\nclass Config:\n    database_url: str\n    verbose: bool = False\n    port: int\n```\n\n### Dates and Times\n\nTOML handles dates and timestamps as first-class values.\nDate, time and date+time TOML values are bound to `datetime.date`, `datetime.time` and `datetime.datetime` Python objects respectively.\n\nThere is also support for time intervals using `datetime.timedelta`:\n\n```py\nfrom datetime import timedelta\n\n@dataclass\nclass Config:\n    retry_after: timedelta\n    delete_after: timedelta\n```\n\nIntervals shorter than a day can be specified using a TOML time value.\nLonger intervals are supported by adding an `-hours`, `-days`, or `-weeks` suffix.\nOther supported suffixes are `-minutes`, `-seconds`, `-milliseconds` and `-microseconds`, but these are there for completeness sake and less likely to be useful.\nHere is an example TOML fragment corresponding to the dataclass above:\n\n```toml\nretry-after = 00:02:30\ndelete-after-days = 30\n```\n\n### Collections\n\nLists and dictionaries can be used to bind TOML arrays and tables.\nIf you want to make a `list` or `dict` optional, you need to provide a default value via the `default_factory` mechanism as usual, see the [dataclasses documentation](https://docs.python.org/3/library/dataclasses.html#mutable-default-values) for details.\n\n```py\nfrom dataclasses import dataclass, field\n\n@dataclass\nclass Config:\n    tags: list[str] = field(default_factory=list)\n    limits: dict[str, int]\n```\n\nThe dataclass above can be used to bind the following TOML fragment:\n\n```toml\ntags = ["production", "development"]\nlimits = {ram-gb = 1, disk-gb = 100}\n```\n\nAn alternative to `default_factory` is to use a homogeneous (single element type) tuple:\n\n```py\n@dataclass\nclass Config:\n    tags: tuple[str, ...] = ()\n    limits: dict[str, int]\n```\n\nHeterogeneous tuples are supported too: for example `tuple[str, bool]` binds a TOML array that must always have a string as its first element and a Boolean as its second and last element.\nIt is generally clearer though to define a separate dataclass when you need more than one value to configure something:\n\n```py\n@dataclass\nclass Webhook:\n    url: str\n    token: str\n\n@dataclass\nclass Config:\n    webhooks: tuple[Webhook, ...] = ()\n```\n\nThe extra keys (`url` and `token` in this example) provide the clarity:\n\n```toml\nwebhooks = [\n    {url = "https://host1/notify", token = "12345"},\n    {url = "https://host2/hook", token = "frperg"}\n]\n```\n\nTOML\'s array-of-tables syntax can make this configuration a bit easier on the eyes:\n\n```toml\n[[webhooks]]\nurl = "https://host1/notify"\ntoken = "12345"\n\n[[webhooks]]\nurl = "https://host2/hook"\ntoken = "frperg"\n```\n\nAlways define additional dataclasses at the module level in your Python code: if the class is for example defined inside a function, the `Binder` constructor will not be able to find it.\n\n### Untyped Data\n\nSometimes the full structure of the data you want to bind is either too complex or too much in flux to be worth fully annotating.\nIn such a situation, you can use `typing.Any` as the annotation to simply capture the output of Python\'s TOML parser without type-checking it.\n\nIn the following example, a service uses the Python standard library logging implementation, configured using the [configuration dictionary schema](https://docs.python.org/3/library/logging.config.html#logging-config-dictschema):\n\n```py\nimport logging.config\nfrom dataclasses import dataclass\nfrom typing import Any\n\nfrom dataclass_binder import Binder\n\n\n@dataclass\nclass Config:\n    database_url: str\n    logging: Any\n\n\ndef run(url: str) -> None:\n    logging.info("Service starting")\n\n\nif __name__ == "__main__":\n    config = Binder[Config].parse_toml("service.toml")\n    logging.config.dictConfig(config.logging)\n    run(config.database_url)\n```\n\nThe `service.toml` configuration file for this service could look like this:\n\n```toml\ndatabase-url = \'postgresql://user:password@host/db\'\n\n[logging]\nversion = 1\n\n[logging.root]\nlevel = \'INFO\'\nhandlers = [\'file\']\n\n[logging.handlers.file]\nclass = \'logging.handlers.RotatingFileHandler\'\nfilename = \'service.log\'\nformatter = \'simple\'\n\n[logging.formatters.simple]\nformat = \'%(asctime)s %(name)s %(levelname)s %(message)s\'\n```\n\n### Plugins\n\nTo select plugins to activate, you can bind Python classes or modules using `type[BaseClass]` and `types.ModuleType` annotations respectively:\n\n```py\nfrom dataclasses import dataclass, field\nfrom types import ModuleType\n\nfrom supertool.plugins import PostProcessor\n\n\n@dataclass\nclass PluginConfig:\n    postprocessors = tuple[type[PostProcessor], ...] = ()\n    modules: dict[str, ModuleType] = field(default_factory=dict)\n```\n\nIn the TOML, you specify Python classes or modules using their fully qualified names:\n\n```toml\npostprocessors = ["supertool_addons.reporters.JSONReport"]\nmodules = {lint = "supertool_addons.linter"}\n```\n\nThere is no mechanism yet to add configuration to be used by the plugins.\n\n### Immutable\n\nIf you prefer immutable configuration objects, you can achieve that using the `frozen` argument of the `dataclass` decorator and using abstract collection types in the annotations. For example, the following dataclass will be instantiated with a `tuple` object for `tags` and an immutable dictionary view for `limits`:\n\n```py\nfrom collections.abc import Mapping, Sequence\n\n\n@dataclass(frozen=True)\nclass Config:\n    tags: Sequence[str] = ()\n    limits: Mapping[str, int]\n```\n\n### Layered Binding\n\n`Binder` can be instantiated from a dataclass object rather than the dataclass itself.\nThe dataclass object will provide new default values when binding data to it.\nThis can be used to implement a layered configuration parsing mechanism, where there is a default configuration that can be customized using a system-wide configuration file and/or a per-user configuration file:\n\n```py\nconfig = Config()\nif system_config_path.exists():\n    config = Binder(config).parse_toml(system_config_path)\nif user_config_path.exists():\n    config = Binder(config).parse_toml(user_config_path)\n```\n\nLater layers can override individual fields in nested dataclasses, allowing fine-grained configuration merging, but collections are replaced whole instead of merged.\n\n### Generating a Configuration Template\n\nTo provide users with a starting point for configuring your application/service, you can automatically generate a configuration template from the information in the dataclass.\n\nFor example, when the following dataclass defines your configuration:\n\n```py\n@dataclass\nclass Config:\n    database_url: str\n    """The URL of the database to connect to."""\n\n    port: int = 12345\n    """TCP port on which to accept connections."""\n```\n\nYou can generate a template configuration file using:\n\n```py\nfrom dataclass_binder import Binder\n\n\nfor line in Binder(Config).format_toml_template():\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'???\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\n```\n\nIt is also possible to provide placeholder values by passing a dataclass instance rather than the dataclass itself to `format_toml_template()`:\n\n```py\nTEMPLATE = Config(\n    database_url="postgresql://<username>:<password>@<hostname>/<database name>",\n    port=8080,\n)\n\nfor line in Binder(TEMPLATE).format_toml_template():\n    print(line)\n```\n\nWhich will print:\n\n```toml\n# The URL of the database to connect to.\n# Mandatory.\ndatabase-url = \'postgresql://<username>:<password>@<hostname>/<database name>\'\n\n# TCP port on which to accept connections.\n# Default:\n# port = 12345\nport = 8080\n```\n\n### Generating a Compact Configuration File\n\nIf you want to generate a fully populated configuration, you can use the `format_toml()` method.\nCompared to the template formatting, this leaves out optional parts for which no data has been provided.\n\nFor example, when the following dataclass defines your configuration:\n\n```py\n@dataclass\nclass Config:\n    path: str\n    """Path of input file."""\n\n    verbose: bool = False\n    """Be extra verbose in logging."""\n\n    options: dict[str, Any] = field(default_factory=dict)\n    """Various named options that are passed on to tool XYZ."""\n```\n\nThis code generates a populated configuration file:\n\n```py\nconfig = Config(path="./data")\n\nwith open("config.toml", "w") as out:\n    for line in Binder(config).format_toml():\n        print(line, file=out)\n```\n\nWith the contents of `config.toml` containing only the `path` field:\n\n```toml\n# Path of input file.\npath = \'./data\'\n```\n\n### Troubleshooting\n\nFinally, a troubleshooting tip: instead of the full `Binder(Config).parse_toml()`, first try to execute only `Binder(Config)`.\nIf that fails, the problem is in the dataclass definitions.\nIf that succeeds, but the `parse_toml()` call fails, the problem is that the TOML file does not match the format defined in the dataclasses.\n\n\n## Development Environment\n\n[Poetry](https://python-poetry.org/) is used to set up a virtual environment with all the dependencies and development tools that you need:\n\n    $ cd dataclass-binder\n    $ poetry install\n\nYou can activate a shell which contains the development tools in its search path:\n\n    $ poetry shell\n\nWe recommend setting up pre-commit hooks for Git in the `dataclass-binder` work area.\nThese hooks automatically run a few simple checks and cleanups when you create a new commit.\nAfter you first set up your virtual environment with Poetry, run this command to install the pre-commit hooks:\n\n    $ pre-commit install\n\n\n## Release Procedure\n\n- Verify that CI passes on the branch that you want to release (typically `main`)\n- Create a release on the GitHub web interface; name the tag `v<major>.<minor>.<patchlevel>`\n- After publishing the release on GitHub, the package will be built and published on PyPI automatically via Actions\n\n\n## Deprecations\n\n### Binder Specialization\n\nPrior to version 0.2.0, the `Binder` class was specialized using a type argument (`Binder[Config]`) rather than instantiation (`Binder(config)`). The old syntax is still supported for now, but the backwards compatibility might be removed in a minor release prior to 1.0 if it becomes a maintenance burden, so please update your code.\n\n### Template Formatting\n\nIn version 0.3.0, the function `format_template()` has been replaced by the method `Binder.format_toml_template()`. The old function is still available for now.\n\n## Changelog\n\n### 0.1.0 - 2023-02-21:\n\n- First open source release; thanks to my employer [Protix](https://protix.eu/) for making this possible\n\n### 0.1.1 - 2023-02-22:\n\n- Relax `Binder.bind()` argument type to `Mapping` ([#3](https://github.com/ProtixIT/dataclass-binder/issues/3))\n\n### 0.1.2 - 2023-03-03:\n\n- Fix `get()` and `[]` on object bound to read-only mapping ([#6](https://github.com/ProtixIT/dataclass-binder/issues/6))\n\n### 0.1.3 - 2023-03-05:\n\n- Ignore dataclass fields with `init=False` ([#2](https://github.com/ProtixIT/dataclass-binder/issues/2))\n\n### 0.2.0 - 2023-06-26:\n\n- Instantiate `Binder` instead of specializing it ([#14](https://github.com/ProtixIT/dataclass-binder/pull/14))\n- Support `typing.Any` as a field annotation ([#10](https://github.com/ProtixIT/dataclass-binder/issues/10))\n- Fix crash in `format_template()` on optional fields with non-string annotations ([#16](https://github.com/ProtixIT/dataclass-binder/pull/16))\n\n### 0.3.0 - 2023-07-13:\n\n- Replace `format_template()` function by `Binder.format_toml_template()` method ([#23](https://github.com/ProtixIT/dataclass-binder/pull/23))\n- Format nested dataclasses as TOML tables ([#25](https://github.com/ProtixIT/dataclass-binder/pull/25))\n- Format untyped mappings and sequences as TOML tables ([#27](https://github.com/ProtixIT/dataclass-binder/pull/27))\n- Fix formatting of `init=False` field in nested dataclasses ([#22](https://github.com/ProtixIT/dataclass-binder/pull/22))\n- Fix annotation evaluation on inherited dataclasses ([#21](https://github.com/ProtixIT/dataclass-binder/pull/21))\n\n### 0.3.1 - 2023-07-17:\n\n- Generate template in depth-first order ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))\n- Fix binder creation and formatting for recursive dataclasses ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))\n\n### 0.3.2 - 2023-07-27:\n\n- Document fields with a `default_factory` as optional in template ([#35](https://github.com/ProtixIT/dataclass-binder/pull/35))\n- Omit values from template that are formatted equally to the default ([#36](https://github.com/ProtixIT/dataclass-binder/pull/36))\n- Require fields with `None` in their annotation to have `None` as their default ([#37](https://github.com/ProtixIT/dataclass-binder/pull/37))\n\n### 0.3.3 - 2023-07-31:\n\n- Add `Binder.format_toml()` method to generate more compact TOML that excludes unused optional parts ([#38](https://github.com/ProtixIT/dataclass-binder/pull/38))\n',
     'author': 'Maarten ter Huurne',
     'author_email': 'maarten.terhuurne@protix.eu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ProtixIT/dataclass-binder',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `dataclass_binder-0.3.2/PKG-INFO` & `dataclass_binder-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-binder
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library to bind TOML data to Python dataclasses in a type-safe way.
 Home-page: https://github.com/ProtixIT/dataclass-binder
 License: MIT
 Keywords: dataclass,toml,bind,binding
 Author: Maarten ter Huurne
 Author-email: maarten.terhuurne@protix.eu
 Requires-Python: >=3.10,<4.0
@@ -470,14 +470,51 @@
 
 # TCP port on which to accept connections.
 # Default:
 # port = 12345
 port = 8080
 ```
 
+### Generating a Compact Configuration File
+
+If you want to generate a fully populated configuration, you can use the `format_toml()` method.
+Compared to the template formatting, this leaves out optional parts for which no data has been provided.
+
+For example, when the following dataclass defines your configuration:
+
+```py
+@dataclass
+class Config:
+    path: str
+    """Path of input file."""
+
+    verbose: bool = False
+    """Be extra verbose in logging."""
+
+    options: dict[str, Any] = field(default_factory=dict)
+    """Various named options that are passed on to tool XYZ."""
+```
+
+This code generates a populated configuration file:
+
+```py
+config = Config(path="./data")
+
+with open("config.toml", "w") as out:
+    for line in Binder(config).format_toml():
+        print(line, file=out)
+```
+
+With the contents of `config.toml` containing only the `path` field:
+
+```toml
+# Path of input file.
+path = './data'
+```
+
 ### Troubleshooting
 
 Finally, a troubleshooting tip: instead of the full `Binder(Config).parse_toml()`, first try to execute only `Binder(Config)`.
 If that fails, the problem is in the dataclass definitions.
 If that succeeds, but the `parse_toml()` call fails, the problem is that the TOML file does not match the format defined in the dataclasses.
 
 
@@ -552,10 +589,14 @@
 
 - Generate template in depth-first order ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))
 - Fix binder creation and formatting for recursive dataclasses ([#28](https://github.com/ProtixIT/dataclass-binder/pull/28))
 
 ### 0.3.2 - 2023-07-27:
 
 - Document fields with a `default_factory` as optional in template ([#35](https://github.com/ProtixIT/dataclass-binder/pull/35))
-- Omit values that are formatted equally to the default ([#36](https://github.com/ProtixIT/dataclass-binder/pull/36))
-- Require optional fields to have `None` as their default ([#37](https://github.com/ProtixIT/dataclass-binder/pull/37))
+- Omit values from template that are formatted equally to the default ([#36](https://github.com/ProtixIT/dataclass-binder/pull/36))
+- Require fields with `None` in their annotation to have `None` as their default ([#37](https://github.com/ProtixIT/dataclass-binder/pull/37))
+
+### 0.3.3 - 2023-07-31:
+
+- Add `Binder.format_toml()` method to generate more compact TOML that excludes unused optional parts ([#38](https://github.com/ProtixIT/dataclass-binder/pull/38))
```

