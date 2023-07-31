# Comparing `tmp/termynal-0.7.0a0.tar.gz` & `tmp/termynal-0.7.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termynal-0.7.0a0.tar", max compression
+gzip compressed data, was "termynal-0.7.0a1.tar", max compression
```

## Comparing `termynal-0.7.0a0.tar` & `termynal-0.7.0a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1092 2023-07-31 06:04:19.854718 termynal-0.7.0a0/LICENSE
--rw-r--r--   0        0        0     1758 2023-07-31 06:04:19.854718 termynal-0.7.0a0/README.md
--rw-r--r--   0        0        0     2465 2023-07-31 06:04:19.854718 termynal-0.7.0a0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-31 06:04:19.854718 termynal-0.7.0a0/termynal/__init__.py
--rw-r--r--   0        0        0     2379 2023-07-31 06:04:19.854718 termynal-0.7.0a0/termynal/assets/termynal.css
--rw-r--r--   0        0        0     9704 2023-07-31 06:04:19.854718 termynal-0.7.0a0/termynal/assets/termynal.js
--rw-r--r--   0        0        0     6496 2023-07-31 06:04:19.854718 termynal-0.7.0a0/termynal/markdown.py
--rw-r--r--   0        0        0     1121 2023-07-31 06:04:19.854718 termynal-0.7.0a0/termynal/plugin.py
--rw-r--r--   0        0        0     2425 1970-01-01 00:00:00.000000 termynal-0.7.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-31 06:23:26.184987 termynal-0.7.0a1/LICENSE
+-rw-r--r--   0        0        0     1493 2023-07-31 06:23:26.184987 termynal-0.7.0a1/README.md
+-rw-r--r--   0        0        0     2465 2023-07-31 06:23:26.184987 termynal-0.7.0a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 06:23:26.184987 termynal-0.7.0a1/termynal/__init__.py
+-rw-r--r--   0        0        0     2379 2023-07-31 06:23:26.184987 termynal-0.7.0a1/termynal/assets/termynal.css
+-rw-r--r--   0        0        0     9704 2023-07-31 06:23:26.184987 termynal-0.7.0a1/termynal/assets/termynal.js
+-rw-r--r--   0        0        0     6498 2023-07-31 06:23:26.184987 termynal-0.7.0a1/termynal/markdown.py
+-rw-r--r--   0        0        0     1121 2023-07-31 06:23:26.184987 termynal-0.7.0a1/termynal/plugin.py
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 termynal-0.7.0a1/PKG-INFO
```

### Comparing `termynal-0.7.0a0/LICENSE` & `termynal-0.7.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `termynal-0.7.0a0/README.md` & `termynal-0.7.0a1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -17,59 +17,25 @@
 
 ```
 $ pip install termynal
 ---> 100%
 Installed
 ```
 
-[Example](https://daxartio.github.io/termynal/)
+[Examples](https://daxartio.github.io/termynal/)
 
 ## Usage
 
 Use `<!-- termynal -->` before code block
 
 ````
 <!-- termynal -->
 
 ```
-// code
-```
-````
-
-or `console` in code block
-
-````
-```console
-// code
-```
-````
-
-progress, prompt `---> 100%`
-
-````
-```console
-$ show progress
----> 100%
-Done!
-```
-````
-
-command, start with `$`
-
-````
-```console
-$ command
-```
-````
-
-comment, start with `#`
-
-````
-```console
-# comment
+$ python script.py
 ```
 ````
 
 ### Mkdocs integration
 
 Declare the plugin:
 
@@ -83,16 +49,16 @@
 Optionally, pass options to the processor:
 
 ```yaml
 [...]
 markdown_extensions:
   - termynal:
       prompt_literal_start:
-        - "$ "
-        - "&gt; "
+        - "$"
+        - ">"
 [...]
 ```
 
 This config allows you to use another prompt:
 
 ````markdown
 <!-- termynal -->
```

### Comparing `termynal-0.7.0a0/pyproject.toml` & `termynal-0.7.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.7.0a0"
+version = "0.7.0a1"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "termynal"
-version = "0.7.0a0"
+version = "0.7.0a1"
 description = ""
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/termynal"
 homepage = "https://pypi.org/project/termynal"
 keywords = []
```

### Comparing `termynal-0.7.0a0/termynal/assets/termynal.css` & `termynal-0.7.0a1/termynal/assets/termynal.css`

 * *Files identical despite different names*

### Comparing `termynal-0.7.0a0/termynal/assets/termynal.js` & `termynal-0.7.0a1/termynal/assets/termynal.js`

 * *Files identical despite different names*

### Comparing `termynal-0.7.0a0/termynal/markdown.py` & `termynal-0.7.0a1/termynal/markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from markdown.extensions import Extension
 from markdown.preprocessors import Preprocessor
 
 if TYPE_CHECKING:  # pragma:no cover
     from markdown import core
 
 
-def make_regex_prompts(prompt_literal_start: Iterable[str]) -> re.Pattern[str]:
+def make_regex_prompts(prompt_literal_start: Iterable[str]) -> "re.Pattern[str]":
     prompt_literal_start = [re.escape(p).strip() for p in prompt_literal_start]
     prompt_to_replace = {
         ">": "&gt;",
         "<": "&lt;",
     }
     for i, prompt in enumerate(prompt_literal_start):
         if prompt in prompt_to_replace:
```

### Comparing `termynal-0.7.0a0/termynal/plugin.py` & `termynal-0.7.0a1/termynal/plugin.py`

 * *Files identical despite different names*

### Comparing `termynal-0.7.0a0/PKG-INFO` & `termynal-0.7.0a1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termynal
-Version: 0.7.0a0
+Version: 0.7.0a1
 Summary: 
 Home-page: https://pypi.org/project/termynal
 License: MIT
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -37,59 +37,25 @@
 
 ```
 $ pip install termynal
 ---> 100%
 Installed
 ```
 
-[Example](https://daxartio.github.io/termynal/)
+[Examples](https://daxartio.github.io/termynal/)
 
 ## Usage
 
 Use `<!-- termynal -->` before code block
 
 ````
 <!-- termynal -->
 
 ```
-// code
-```
-````
-
-or `console` in code block
-
-````
-```console
-// code
-```
-````
-
-progress, prompt `---> 100%`
-
-````
-```console
-$ show progress
----> 100%
-Done!
-```
-````
-
-command, start with `$`
-
-````
-```console
-$ command
-```
-````
-
-comment, start with `#`
-
-````
-```console
-# comment
+$ python script.py
 ```
 ````
 
 ### Mkdocs integration
 
 Declare the plugin:
 
@@ -103,16 +69,16 @@
 Optionally, pass options to the processor:
 
 ```yaml
 [...]
 markdown_extensions:
   - termynal:
       prompt_literal_start:
-        - "$ "
-        - "&gt; "
+        - "$"
+        - ">"
 [...]
 ```
 
 This config allows you to use another prompt:
 
 ````markdown
 <!-- termynal -->
```

