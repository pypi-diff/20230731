# Comparing `tmp/termynal-0.6.0.tar.gz` & `tmp/termynal-0.7.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termynal-0.6.0.tar", max compression
+gzip compressed data, was "termynal-0.7.0a0.tar", max compression
```

## Comparing `termynal-0.6.0.tar` & `termynal-0.7.0a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1092 2023-07-30 06:47:20.978323 termynal-0.6.0/LICENSE
--rw-r--r--   0        0        0     1758 2023-07-30 06:47:20.978323 termynal-0.6.0/README.md
--rw-r--r--   0        0        0     2461 2023-07-30 06:47:20.978323 termynal-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-30 06:47:20.978323 termynal-0.6.0/termynal/__init__.py
--rw-r--r--   0        0        0     2303 2023-07-30 06:47:20.978323 termynal-0.6.0/termynal/assets/termynal.css
--rw-r--r--   0        0        0     9704 2023-07-30 06:47:20.978323 termynal-0.6.0/termynal/assets/termynal.js
--rw-r--r--   0        0        0     5643 2023-07-30 06:47:20.978323 termynal-0.6.0/termynal/markdown.py
--rw-r--r--   0        0        0     1121 2023-07-30 06:47:20.978323 termynal-0.6.0/termynal/plugin.py
--rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 termynal-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-31 06:04:19.854718 termynal-0.7.0a0/LICENSE
+-rw-r--r--   0        0        0     1758 2023-07-31 06:04:19.854718 termynal-0.7.0a0/README.md
+-rw-r--r--   0        0        0     2465 2023-07-31 06:04:19.854718 termynal-0.7.0a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 06:04:19.854718 termynal-0.7.0a0/termynal/__init__.py
+-rw-r--r--   0        0        0     2379 2023-07-31 06:04:19.854718 termynal-0.7.0a0/termynal/assets/termynal.css
+-rw-r--r--   0        0        0     9704 2023-07-31 06:04:19.854718 termynal-0.7.0a0/termynal/assets/termynal.js
+-rw-r--r--   0        0        0     6496 2023-07-31 06:04:19.854718 termynal-0.7.0a0/termynal/markdown.py
+-rw-r--r--   0        0        0     1121 2023-07-31 06:04:19.854718 termynal-0.7.0a0/termynal/plugin.py
+-rw-r--r--   0        0        0     2425 1970-01-01 00:00:00.000000 termynal-0.7.0a0/PKG-INFO
```

### Comparing `termynal-0.6.0/LICENSE` & `termynal-0.7.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `termynal-0.6.0/README.md` & `termynal-0.7.0a0/README.md`

 * *Files identical despite different names*

### Comparing `termynal-0.6.0/pyproject.toml` & `termynal-0.7.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.6.0"
+version = "0.7.0a0"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "termynal"
-version = "0.6.0"
+version = "0.7.0a0"
 description = ""
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/termynal"
 homepage = "https://pypi.org/project/termynal"
 keywords = []
```

### Comparing `termynal-0.6.0/termynal/assets/termynal.css` & `termynal-0.7.0a0/termynal/assets/termynal.css`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,18 @@
     color: var(--color-text-subtle);
     top: 5px;
     left: 0;
     width: 100%;
     text-align: center;
 }
 
+[data-termynal][data-ty-title]:after {
+    content: attr(data-ty-title);
+}
+
 a[data-terminal-control] {
     text-align: right;
     display: block;
     color: #aebbff;
 }
 
 [data-ty] {
```

### Comparing `termynal-0.6.0/termynal/assets/termynal.js` & `termynal-0.7.0a0/termynal/assets/termynal.js`

 * *Files identical despite different names*

### Comparing `termynal-0.6.0/termynal/markdown.py` & `termynal-0.7.0a0/termynal/markdown.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,65 @@
 import re
-from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Tuple
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Tuple
 
 from markdown.extensions import Extension
 from markdown.preprocessors import Preprocessor
 
 if TYPE_CHECKING:  # pragma:no cover
     from markdown import core
 
 
+def make_regex_prompts(prompt_literal_start: Iterable[str]) -> re.Pattern[str]:
+    prompt_literal_start = [re.escape(p).strip() for p in prompt_literal_start]
+    prompt_to_replace = {
+        ">": "&gt;",
+        "<": "&lt;",
+    }
+    for i, prompt in enumerate(prompt_literal_start):
+        if prompt in prompt_to_replace:
+            prompt_literal_start[i] = prompt_to_replace[prompt]
+    prompt_literal_start_re = "|".join(f"{p} " for p in prompt_literal_start)
+    return re.compile(f"^({prompt_literal_start_re})")
+
+
 class Termynal:
     progress_literal_start = "---&gt; 100%"
     custom_literal_start = "# "
 
     def __init__(
         self,
-        prompt_literal_start: Iterable[str] = ("$ ",),
-        promt_in_multiline: bool = False,
+        title: Optional[str] = None,
+        prompt_literal_start: Iterable[str] = ("$",),
+        prompt_in_multiline: bool = False,
     ):
-        self.prompt_literal_start = "|".join(re.escape(p) for p in prompt_literal_start)
-        self.regex_prompts = re.compile(f"^({self.prompt_literal_start})")
-        self.promt_in_multiline = promt_in_multiline
+        self.title = title
+        self.regex_prompts = make_regex_prompts(prompt_literal_start)
+        self.prompt_in_multiline = prompt_in_multiline
 
     def convert(self, code: str) -> str:
         code_lines: List[str] = []
-        code_lines.append('<div class="termy" data-termynal>')
+        if self.title is not None:
+            code_lines.append(
+                f'<div class="termy" data-termynal data-ty-title="{self.title}">',
+            )
+        else:
+            code_lines.append('<div class="termy">')
         multiline = False
         used_prompt = None
         for line in code.split("\n"):
             if match := self.regex_prompts.match(line):
                 used_prompt = match.group()
                 code_lines.append(
                     f'<span data-ty="input" data-ty-prompt="{used_prompt.strip()}">'
                     f"{line.rsplit(used_prompt)[1]}</span>",
                 )
                 multiline = bool(line.endswith("\\"))
             elif multiline:
                 used_prompt = used_prompt or ""
-                if not self.promt_in_multiline:
+                if not self.prompt_in_multiline:
                     used_prompt = ""
                 code_lines.append(
                     f'<span data-ty="input" data-ty-prompt="{used_prompt.strip()}">'
                     f"{line}</span>",
                 )
                 multiline = bool(line.endswith("\\"))
 
@@ -58,16 +77,17 @@
 
 class TermynalPreprocessor(Preprocessor):
     rexep = re.compile("(<code.*>)((.|\n)*?)(</code>)")
     comment = "<!-- termynal -->"
     language_class = 'class="language-console"'
 
     def __init__(self, config: Dict[str, Any], md: "core.Markdown"):
+        self.title = config.get("title", None)
         self.prompt_literal_start = config.get("prompt_literal_start", ("$ ",))
-        self.promt_in_multiline = config.get("promt_in_multiline", False)
+        self.prompt_in_multiline = config.get("prompt_in_multiline", False)
 
         super(TermynalPreprocessor, self).__init__(md=md)
 
     def run(self, lines: List[str]) -> List[str]:
         content_by_placeholder = {}
         for i in range(self.md.htmlStash.html_counter):
             placeholder = self.md.htmlStash.get_placeholder(i)
@@ -87,16 +107,17 @@
 
     def _get_lines(
         self,
         lines: List[str],
         content_by_placeholder: Dict[str, Tuple[str, int]],
     ) -> Dict[str, str]:  # pylint:disable=too-many-nested-blocks
         termynal_obj = Termynal(
+            title=self.title,
             prompt_literal_start=self.prompt_literal_start,
-            promt_in_multiline=self.promt_in_multiline,
+            prompt_in_multiline=self.prompt_in_multiline,
         )
         lines_by_placeholder = {}
         is_termynal_code = False
         for line in lines:
             if line in content_by_placeholder:
                 (content, i) = content_by_placeholder[line]
 
@@ -126,22 +147,26 @@
 
         return lines_by_placeholder
 
 
 class TermynalExtension(Extension):
     def __init__(self, *args: Any, **kwargs: Any):
         self.config = {
+            "title": [
+                "bash",
+                "Default: 'bash'",
+            ],
             "prompt_literal_start": [
                 [
-                    "$ ",
+                    "$",
                 ],
                 "A list of prompt characters start to consider as console - "
-                "Default: ['$ ',]",
+                "Default: ['$']",
             ],
-            "promt_in_multiline": [
+            "prompt_in_multiline": [
                 False,
                 "Default: False",
             ],
         }
 
         super(TermynalExtension, self).__init__(*args, **kwargs)
```

### Comparing `termynal-0.6.0/termynal/plugin.py` & `termynal-0.7.0a0/termynal/plugin.py`

 * *Files identical despite different names*

### Comparing `termynal-0.6.0/PKG-INFO` & `termynal-0.7.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termynal
-Version: 0.6.0
+Version: 0.7.0a0
 Summary: 
 Home-page: https://pypi.org/project/termynal
 License: MIT
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

