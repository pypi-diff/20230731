# Comparing `tmp/jupyterlab_vim-0.17.0.tar.gz` & `tmp/jupyterlab_vim-4.0.0.tar.gz`

## Comparing `jupyterlab_vim-0.17.0.tar` & `jupyterlab_vim-4.0.0.tar`

### file list

```diff
@@ -1,37 +1,36 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/.eslintignore
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/.prettierignore
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/.prettierrc
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/.yarnrc.yml
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/CHANGELOG.md
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/RELEASE.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/Untitled.ipynb
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/install.json
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/installing.md
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/modify-keybinds.md
--rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/tsconfig.json
--rw-r--r--   0        0        0   211305 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/yarn.lock
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/_version.py
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/package.json
--rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig
--rw-r--r--   0        0        0     9952 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json
--rw-r--r--   0        0        0   130333 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/252.e0500116419ca3a355d1.js
--rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/353.184fc74aa8db790efd40.js
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/747.a573445024188eae7034.js
--rw-r--r--   0        0        0     7518 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/remoteEntry.6d29f029f239ba56d940.js
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/style.js
--rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     9952 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/schema/plugin.json
--rw-r--r--   0        0        0    10125 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/src/codemirrorCommands.ts
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/src/index.ts
--rw-r--r--   0        0        0     8183 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/src/labCommands.ts
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/style/index.js
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/LICENSE
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/README.md
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/pyproject.toml
--rw-r--r--   0        0        0     8706 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/.eslintignore
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/.prettierrc
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/.yarnrc.yml
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/RELEASE.md
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/install.json
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/installing.md
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/modify-keybinds.md
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/tsconfig.json
+-rw-r--r--   0        0        0   212877 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/yarn.lock
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/_version.py
+-rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/package.json
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig
+-rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json
+-rw-r--r--   0        0        0   130333 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/252.e0500116419ca3a355d1.js
+-rw-r--r--   0        0        0    10172 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/353.8b609c372dc07b2baac6.js
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/747.a573445024188eae7034.js
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/remoteEntry.a73b7957e55f8d1b9f75.js
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/style.js
+-rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/schema/plugin.json
+-rw-r--r--   0        0        0    11763 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/src/codemirrorCommands.ts
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/src/index.ts
+-rw-r--r--   0        0        0     8187 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/src/labCommands.ts
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/style/index.js
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/LICENSE
+-rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/README.md
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.0/PKG-INFO
```

### Comparing `jupyterlab_vim-0.17.0/RELEASE.md` & `jupyterlab_vim-4.0.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-0.17.0/modify-keybinds.md` & `jupyterlab_vim-4.0.0/modify-keybinds.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-0.17.0/package.json` & `jupyterlab_vim-4.0.0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768105158730158%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/fileeditor': '^4.0.3'}",*

 * * "'devDependencies'": "{'@jupyterlab/codeeditor': '^4.0.3'}",*

 * * "'version'": "'4.0.0'"}*

```diff
@@ -7,28 +7,30 @@
     },
     "dependencies": {
         "@codemirror/state": "^6.2.1",
         "@codemirror/view": "^6.15.3",
         "@jupyterlab/application": "^4.0.3",
         "@jupyterlab/cells": "^4.0.3",
         "@jupyterlab/codemirror": "^4.0.3",
+        "@jupyterlab/fileeditor": "^4.0.3",
         "@jupyterlab/notebook": "^4.0.3",
         "@jupyterlab/settingregistry": "^4.0.3",
         "@lumino/commands": "^2.0.1",
         "@lumino/coreutils": "^2.0.0",
         "@lumino/disposable": "^2.1.2",
         "@lumino/domutils": "^2.0.0",
         "@replit/codemirror-vim": "^6.0.14",
         "react": "^18.2.0"
     },
     "description": "Code cell vim bindings",
     "devDependencies": {
         "@codemirror/language": "^6.8.0",
         "@codemirror/search": "^6.5.0",
         "@jupyterlab/builder": "^4.0.0",
+        "@jupyterlab/codeeditor": "^4.0.3",
         "@types/codemirror": "^0.0.87",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@typescript-eslint/eslint-plugin": "^6.1.0",
         "@typescript-eslint/parser": "^6.1.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
@@ -185,9 +187,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.17.0"
+    "version": "4.0.0"
 }
```

### Comparing `jupyterlab_vim-0.17.0/tsconfig.json` & `jupyterlab_vim-4.0.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-0.17.0/yarn.lock` & `jupyterlab_vim-4.0.0/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     "@codemirror/language": ^6.8.0
     "@codemirror/search": ^6.5.0
     "@codemirror/state": ^6.2.1
     "@codemirror/view": ^6.15.3
     "@jupyterlab/application": ^4.0.3
     "@jupyterlab/builder": ^4.0.0
     "@jupyterlab/cells": ^4.0.3
+    "@jupyterlab/codeeditor": ^4.0.3
     "@jupyterlab/codemirror": ^4.0.3
+    "@jupyterlab/fileeditor": ^4.0.3
     "@jupyterlab/notebook": ^4.0.3
     "@jupyterlab/settingregistry": ^4.0.3
     "@lumino/commands": ^2.0.1
     "@lumino/coreutils": ^2.0.0
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.0
     "@replit/codemirror-vim": ^6.0.14
@@ -848,14 +850,39 @@
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
   checksum: 30c2447cfe76fb2d1c3d1c88136b842f8d0f46451d4082ecc1a26496e35f5309a956468af18b2b0ac42a72c9bd14a1ddd050d434c6d9740b468956a6bb989086
   languageName: node
   linkType: hard
 
+"@jupyterlab/fileeditor@npm:^4.0.3":
+  version: 4.0.3
+  resolution: "@jupyterlab/fileeditor@npm:4.0.3"
+  dependencies:
+    "@jupyterlab/apputils": ^4.1.3
+    "@jupyterlab/codeeditor": ^4.0.3
+    "@jupyterlab/codemirror": ^4.0.3
+    "@jupyterlab/coreutils": ^6.0.3
+    "@jupyterlab/docregistry": ^4.0.3
+    "@jupyterlab/documentsearch": ^4.0.3
+    "@jupyterlab/lsp": ^4.0.3
+    "@jupyterlab/statusbar": ^4.0.3
+    "@jupyterlab/toc": ^6.0.3
+    "@jupyterlab/translation": ^4.0.3
+    "@jupyterlab/ui-components": ^4.0.3
+    "@lumino/commands": ^2.1.1
+    "@lumino/coreutils": ^2.1.1
+    "@lumino/messaging": ^2.0.0
+    "@lumino/widgets": ^2.1.1
+    react: ^18.2.0
+    regexp-match-indices: ^1.0.2
+  checksum: 9ff129ffa6b91752d3c4f0d36357532a29bec56a4a91d2d3a182e7cba2d3a5ba9b67317bb66356bbd201ca75af30bf5b0985f4629ef4acc4c2842cc7bca72ff6
+  languageName: node
+  linkType: hard
+
 "@jupyterlab/lsp@npm:^4.0.3":
   version: 4.0.3
   resolution: "@jupyterlab/lsp@npm:4.0.3"
   dependencies:
     "@jupyterlab/apputils": ^4.1.3
     "@jupyterlab/codeeditor": ^4.0.3
     "@jupyterlab/coreutils": ^6.0.3
@@ -4784,14 +4811,32 @@
   dependencies:
     indent-string: ^5.0.0
     strip-indent: ^4.0.0
   checksum: 6944e7b1d8f3fd28c2515f5c605b9f7f0ea0f4edddf41890bbbdd4d9ee35abb7540c3b278f03ff827bd278bb6ff4a5bd8692ca406b748c5c1c3ce7355e9fbf8f
   languageName: node
   linkType: hard
 
+"regexp-match-indices@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "regexp-match-indices@npm:1.0.2"
+  dependencies:
+    regexp-tree: ^0.1.11
+  checksum: 8cc779f6cf8f404ead828d09970a7d4bd66bd78d43ab9eb2b5e65f2ef2ba1ed53536f5b5fa839fb90b350365fb44b6a851c7f16289afc3f37789c113ab2a7916
+  languageName: node
+  linkType: hard
+
+"regexp-tree@npm:^0.1.11":
+  version: 0.1.27
+  resolution: "regexp-tree@npm:0.1.27"
+  bin:
+    regexp-tree: bin/regexp-tree
+  checksum: 129aebb34dae22d6694ab2ac328be3f99105143737528ab072ef624d599afecbcfae1f5c96a166fa9e5f64fa1ecf30b411c4691e7924c3e11bbaf1712c260c54
+  languageName: node
+  linkType: hard
+
 "require-from-string@npm:^2.0.2":
   version: 2.0.2
   resolution: "require-from-string@npm:2.0.2"
   checksum: a03ef6895445f33a4015300c426699bc66b2b044ba7b670aa238610381b56d3f07c686251740d575e22f4c87531ba662d06937508f0f3c0f1ddc04db3130560b
   languageName: node
   linkType: hard
```

### Comparing `jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/package.json` & `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9716021825396824%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/fileeditor': '^4.0.3'}",*

 * * "'devDependencies'": "{'@jupyterlab/codeeditor': '^4.0.3'}",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'version'": "'4.0.0'"}*

```diff
@@ -7,28 +7,30 @@
     },
     "dependencies": {
         "@codemirror/state": "^6.2.1",
         "@codemirror/view": "^6.15.3",
         "@jupyterlab/application": "^4.0.3",
         "@jupyterlab/cells": "^4.0.3",
         "@jupyterlab/codemirror": "^4.0.3",
+        "@jupyterlab/fileeditor": "^4.0.3",
         "@jupyterlab/notebook": "^4.0.3",
         "@jupyterlab/settingregistry": "^4.0.3",
         "@lumino/commands": "^2.0.1",
         "@lumino/coreutils": "^2.0.0",
         "@lumino/disposable": "^2.1.2",
         "@lumino/domutils": "^2.0.0",
         "@replit/codemirror-vim": "^6.0.14",
         "react": "^18.2.0"
     },
     "description": "Code cell vim bindings",
     "devDependencies": {
         "@codemirror/language": "^6.8.0",
         "@codemirror/search": "^6.5.0",
         "@jupyterlab/builder": "^4.0.0",
+        "@jupyterlab/codeeditor": "^4.0.3",
         "@types/codemirror": "^0.0.87",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@typescript-eslint/eslint-plugin": "^6.1.0",
         "@typescript-eslint/parser": "^6.1.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
@@ -113,19 +115,14 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.{json,}",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab-contrib/jupyterlab-vim",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.6d29f029f239ba56d940.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "jupyterlab_vim/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "extension",
         "jupyter",
@@ -190,9 +187,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.17.0"
+    "version": "4.0.0"
 }
```

### Comparing `jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig` & `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/package.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9716021825396824%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/fileeditor': '^4.0.3'}",*

 * * "'devDependencies'": "{'@jupyterlab/codeeditor': '^4.0.3'}",*

 * * "'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.a73b7957e55f8d1b9f75.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'4.0.0'"}*

```diff
@@ -7,28 +7,30 @@
     },
     "dependencies": {
         "@codemirror/state": "^6.2.1",
         "@codemirror/view": "^6.15.3",
         "@jupyterlab/application": "^4.0.3",
         "@jupyterlab/cells": "^4.0.3",
         "@jupyterlab/codemirror": "^4.0.3",
+        "@jupyterlab/fileeditor": "^4.0.3",
         "@jupyterlab/notebook": "^4.0.3",
         "@jupyterlab/settingregistry": "^4.0.3",
         "@lumino/commands": "^2.0.1",
         "@lumino/coreutils": "^2.0.0",
         "@lumino/disposable": "^2.1.2",
         "@lumino/domutils": "^2.0.0",
         "@replit/codemirror-vim": "^6.0.14",
         "react": "^18.2.0"
     },
     "description": "Code cell vim bindings",
     "devDependencies": {
         "@codemirror/language": "^6.8.0",
         "@codemirror/search": "^6.5.0",
         "@jupyterlab/builder": "^4.0.0",
+        "@jupyterlab/codeeditor": "^4.0.3",
         "@types/codemirror": "^0.0.87",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@typescript-eslint/eslint-plugin": "^6.1.0",
         "@typescript-eslint/parser": "^6.1.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
@@ -113,14 +115,19 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.{json,}",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab-contrib/jupyterlab-vim",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.a73b7957e55f8d1b9f75.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "jupyterlab_vim/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "extension",
         "jupyter",
@@ -185,9 +192,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.17.0"
+    "version": "4.0.0"
 }
```

### Comparing `jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json` & `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9716145833333334%*

 * *Differences: {"'jupyter.lab.shortcuts'": "{insert: [(1, OrderedDict([('command', 'vim:enter-normal-mode'), "*

 * *                            "('keys', ['Escape']), ('selector', '.jp-FileEditor')])), (2, "*

 * *                            "OrderedDict([('command', 'documentsearch:end'), ('keys', ['Escape']), "*

 * *                            "('selector', '.jp-mod-searchable .jp-FileEditor .cm-vimMode')])), (3, "*

 * *                            "OrderedDict([('command', 'documentsearch:end'), ('keys', ['Escape']), "*

 * *                      […]*

```diff
@@ -73,14 +73,49 @@
             "disabled": true,
             "keys": [
                 "Escape"
             ],
             "selector": ".jp-Notebook.jp-mod-editMode"
         },
         {
+            "command": "vim:enter-normal-mode",
+            "keys": [
+                "Escape"
+            ],
+            "selector": ".jp-FileEditor"
+        },
+        {
+            "command": "documentsearch:end",
+            "keys": [
+                "Escape"
+            ],
+            "selector": ".jp-mod-searchable .jp-FileEditor .cm-vimMode"
+        },
+        {
+            "command": "documentsearch:end",
+            "keys": [
+                "Escape"
+            ],
+            "selector": ".jp-mod-searchable .jp-Notebook .cm-vimMode"
+        },
+        {
+            "command": "documentsearch:end",
+            "keys": [
+                "Escape"
+            ],
+            "selector": ".jp-mod-search-active .jp-FileEditor .cm-vimMode"
+        },
+        {
+            "command": "documentsearch:end",
+            "keys": [
+                "Escape"
+            ],
+            "selector": ".jp-mod-search-active .jp-Notebook .cm-vimMode"
+        },
+        {
             "command": "notebook:undo-cell-action",
             "keys": [
                 "Ctrl O",
                 "U"
             ],
             "selector": ".jp-NotebookPanel[data-jp-vim-mode='true'] .jp-Notebook.jp-mod-editMode"
         },
@@ -404,18 +439,24 @@
             ],
             "selector": ".jp-NotebookPanel[data-jp-vim-mode='true'] .jp-Notebook.jp-mod-editMode .jp-InputArea-editor:not(.jp-mod-has-primary-selection)"
         }
     ],
     "properties": {
         "enabled": {
             "default": true,
-            "description": "Enable/disable notebook vim (may require a page refresh)",
+            "description": "Enable/disable vim extension (may require a page refresh)",
             "title": "Enabled",
             "type": "boolean"
         },
+        "enabledInEditors": {
+            "default": true,
+            "description": "Enable/disable vim in text editors (may require a page refresh)",
+            "title": "Enabled in Text Editor",
+            "type": "boolean"
+        },
         "extraKeybindings": {
             "default": [],
             "items": {
                 "$ref": "#/definitions/shortcut"
             },
             "title": "Extra Vim Keybindings",
             "type": "array"
```

### Comparing `jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/252.e0500116419ca3a355d1.js` & `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/252.e0500116419ca3a355d1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/353.184fc74aa8db790efd40.js` & `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/353.8b609c372dc07b2baac6.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,391 +1,437 @@
 "use strict";
 (self.webpackChunk_axlair_jupyterlab_vim = self.webpackChunk_axlair_jupyterlab_vim || []).push([
     [353], {
         353: (e, t, o) => {
             o.r(t), o.d(t, {
-                default: () => v
+                default: () => p
             });
             var n = o(861),
+                i = o(785),
                 l = o(408),
-                i = o(663),
+                d = o(663),
                 a = o(829),
                 c = o(211),
-                d = o(204);
-            class s {
+                s = o(204);
+            class r {
                 constructor({
-                    commands: e,
-                    enabled: t,
-                    userKeybindings: o
+                    enabled: e,
+                    userKeybindings: t
                 }) {
-                    this._commands = e, this.enabled = t, this.lastActiveCell = null, this.userKeybindings = null != o ? o : []
+                    this._lastActiveEditor = null, this.enabled = e, this.userKeybindings = null != t ? t : []
                 }
-                onActiveCellChanged(e, t) {
-                    this.modifyCell(t).catch(console.error)
+                async onActiveEditorChanged(e, t) {
+                    t && (await t.content.ready, this.modifyEditor(t.content.editor))
                 }
-                async modifyCell(e) {
-                    if (!e) return;
-                    this.lastActiveCell = e, await e.ready;
-                    const t = e.editor;
-                    if (e.isDisposed) return void console.warn("Cell was already disposed, cannot setup vim mode");
-                    if (!t) throw Error("Cell editor not available");
+                updateLastActive() {
+                    this.modifyEditor(this._lastActiveEditor)
+                }
+                modifyEditor(e) {
+                    const t = e;
+                    if (!t) throw Error("Editor not available");
+                    this._lastActiveEditor = t;
                     const o = t.editor;
                     if (this.enabled) {
                         if (!t.getOption("vim")) {
                             t.setOption("vim", !0);
                             const e = (0, a.getCM)(o);
                             t.hasFocus = () => !(!e.state.dialog || !e.state.dialog.contains(document.activeElement)) || o.hasFocus
                         }
-                        const n = (0, a.getCM)(o),
-                            l = a.Vim;
-                        ["normal", "visual", "insert"].forEach((e => l.mapclear(e))), this.userKeybindings.forEach((({
+                        a.Vim.defineAction("undo", ((t, o) => {
+                            for (let t = 0; t < o.repeat; t++) e.undo()
+                        })), a.Vim.defineAction("redo", ((t, o) => {
+                            for (let t = 0; t < o.repeat; t++) e.redo()
+                        }));
+                        const n = (0, a.getCM)(o);
+                        return ["normal", "visual", "insert"].forEach((e => a.Vim.mapclear(e))), this.userKeybindings.forEach((({
                             command: e,
                             keys: t,
                             context: o,
                             mapfn: n,
                             enabled: i
                         }) => {
-                            i && ("map" === n ? l.map(e, t, o) : l.noremap(e, t, o))
-                        })), a.Vim.handleKey(n, "<Esc>");
-                        const i = (t, n, l, c) => {
-                            const d = n;
-                            let s = d.ch;
-                            const r = e;
-                            switch (null == c ? void 0 : c.lastMotion) {
-                                case t.moveByLines:
-                                case t.moveByDisplayLines:
-                                case t.moveByScroll:
-                                case t.moveToColumn:
-                                case t.moveToEol:
-                                case i:
-                                    s = c.lastHPos;
-                                    break;
-                                default:
-                                    c.lastHPos = s
-                            }
-                            const m = l.repeat + (l.repeatOffset || 0);
-                            let u = l.forward ? d.line + m : d.line - m;
-                            const C = t.firstLine(),
-                                v = t.lastLine(),
-                                b = t.findPosV(d, l.forward ? m : -m, "line", c.lastHSPos);
-                            if ((l.forward ? b.line > u : b.line < u) && (u = b.line, s = b.ch), !(u < C || u > v)) return l.toFirstChar && (s = function(e) {
-                                if (!e) return 0;
-                                const t = e.search(/\S/);
-                                return -1 === t ? e.length : t
-                            }(t.getLine(u)), c.lastHPos = s), c.lastHSPos = t.charCoords(new a.CodeMirror.Pos(u, s), "div").left, new a.CodeMirror.Pos(u, s);
-                            if (null !== r && "markdown" === r.model.type && (l.handleArrow || (r.rendered = !0)), l.forward)
-                                if (l.handleArrow) {
-                                    const e = t.getCursor(),
-                                        n = o.state.doc.line(v + 1).length;
-                                    e.line === v && e.ch === n || (t.setCursor(v, n), this._commands.execute("notebook:move-cursor-down"))
-                                } else this._commands.execute("notebook:move-cursor-down");
-                            else if (l.handleArrow) {
-                                const e = t.getCursor();
-                                0 === e.line && 0 === e.ch || (t.setCursor(0, 0), this._commands.execute("notebook:move-cursor-up"))
-                            } else this._commands.execute("notebook:move-cursor-up")
-                        };
-                        l.defineMotion("moveByLinesOrCell", i), l.mapCommand("<Up>", "motion", "moveByLinesOrCell", {
-                            forward: !1,
-                            linewise: !0,
-                            handleArrow: !0
-                        }, {
-                            context: "normal"
-                        }), l.mapCommand("<Down>", "motion", "moveByLinesOrCell", {
-                            forward: !0,
-                            linewise: !0,
-                            handleArrow: !0
-                        }, {
-                            context: "normal"
-                        }), l.mapCommand("k", "motion", "moveByLinesOrCell", {
-                            forward: !1,
-                            linewise: !0
-                        }, {
-                            context: "normal"
-                        }), l.mapCommand("j", "motion", "moveByLinesOrCell", {
-                            forward: !0,
-                            linewise: !0
-                        }, {
-                            context: "normal"
-                        }), l.defineAction("moveCellDown", ((e, t) => {
-                            this._commands.execute("notebook:move-cell-down")
-                        })), l.defineAction("moveCellUp", ((e, t) => {
-                            this._commands.execute("notebook:move-cell-up")
-                        })), l.mapCommand("<C-e>", "action", "moveCellDown", {}, {
-                            extra: "normal"
-                        }), l.mapCommand("<C-y>", "action", "moveCellUp", {}, {
-                            extra: "normal"
-                        }), l.defineAction("splitCell", ((e, t) => {
-                            this._commands.execute("notebook:split-cell-at-cursor")
-                        })), l.mapCommand("-", "action", "splitCell", {}, {
-                            extra: "normal"
-                        })
-                    } else t.getOption("vim") && t.setOption("vim", !1)
+                            i && ("map" === n ? a.Vim.map(e, t, o) : a.Vim.noremap(e, t, o))
+                        })), a.Vim.handleKey(n, "<Esc>"), !0
+                    }
+                    return !!t.getOption("vim") && (t.setOption("vim", !1), !1)
+                }
+            }
+            class m extends r {
+                constructor({
+                    commands: e,
+                    enabled: t,
+                    userKeybindings: o
+                }) {
+                    super({
+                        userKeybindings: o,
+                        enabled: t
+                    }), this._lastActiveCell = null, this._commands = e
+                }
+                onActiveCellChanged(e, t) {
+                    this.modifyCell(t).catch(console.error)
+                }
+                updateLastActive() {
+                    this.modifyCell(this._lastActiveCell)
+                }
+                async modifyCell(e) {
+                    e && (this._lastActiveCell = e, await e.ready, e.isDisposed ? console.warn("Cell was already disposed, cannot setup vim mode") : this.modifyEditor(e.editor) && this._modifyEdgeNavigation(e))
+                }
+                _modifyEdgeNavigation(e) {
+                    const t = (o, n, i, l) => {
+                        const d = n;
+                        let c = d.ch;
+                        const s = e;
+                        switch (null == l ? void 0 : l.lastMotion) {
+                            case o.moveByLines:
+                            case o.moveByDisplayLines:
+                            case o.moveByScroll:
+                            case o.moveToColumn:
+                            case o.moveToEol:
+                            case t:
+                                c = l.lastHPos;
+                                break;
+                            default:
+                                l.lastHPos = c
+                        }
+                        const r = i.repeat + (i.repeatOffset || 0);
+                        let m = i.forward ? d.line + r : d.line - r;
+                        const u = o.firstLine(),
+                            C = o.lastLine(),
+                            v = o.findPosV(d, i.forward ? r : -r, "line", l.lastHSPos);
+                        if ((i.forward ? v.line > m : v.line < m) && (m = v.line, c = v.ch), !(m < u || m > C)) return i.toFirstChar && (c = function(e) {
+                            if (!e) return 0;
+                            const t = e.search(/\S/);
+                            return -1 === t ? e.length : t
+                        }(o.getLine(m)), l.lastHPos = c), l.lastHSPos = o.charCoords(new a.CodeMirror.Pos(m, c), "div").left, new a.CodeMirror.Pos(m, c);
+                        if (null !== s && "markdown" === s.model.type && (i.handleArrow || (s.rendered = !0)), i.forward)
+                            if (i.handleArrow) {
+                                const e = o.getCursor(),
+                                    t = o.cm6.state.doc.line(C + 1).length;
+                                e.line === C && e.ch === t || (o.setCursor(C, t), this._commands.execute("notebook:move-cursor-down"))
+                            } else this._commands.execute("notebook:move-cursor-down");
+                        else if (i.handleArrow) {
+                            const e = o.getCursor();
+                            0 === e.line && 0 === e.ch || (o.setCursor(0, 0), this._commands.execute("notebook:move-cursor-up"))
+                        } else this._commands.execute("notebook:move-cursor-up")
+                    };
+                    a.Vim.defineMotion("moveByLinesOrCell", t), a.Vim.mapCommand("<Up>", "motion", "moveByLinesOrCell", {
+                        forward: !1,
+                        linewise: !0,
+                        handleArrow: !0
+                    }, {
+                        context: "normal"
+                    }), a.Vim.mapCommand("<Down>", "motion", "moveByLinesOrCell", {
+                        forward: !0,
+                        linewise: !0,
+                        handleArrow: !0
+                    }, {
+                        context: "normal"
+                    }), a.Vim.mapCommand("k", "motion", "moveByLinesOrCell", {
+                        forward: !1,
+                        linewise: !0
+                    }, {
+                        context: "normal"
+                    }), a.Vim.mapCommand("j", "motion", "moveByLinesOrCell", {
+                        forward: !0,
+                        linewise: !0
+                    }, {
+                        context: "normal"
+                    }), a.Vim.defineAction("moveCellDown", ((e, t) => {
+                        this._commands.execute("notebook:move-cell-down")
+                    })), a.Vim.defineAction("moveCellUp", ((e, t) => {
+                        this._commands.execute("notebook:move-cell-up")
+                    })), a.Vim.mapCommand("<C-e>", "action", "moveCellDown", {}, {
+                        extra: "normal"
+                    }), a.Vim.mapCommand("<C-y>", "action", "moveCellUp", {}, {
+                        extra: "normal"
+                    }), a.Vim.defineAction("splitCell", ((e, t) => {
+                        this._commands.execute("notebook:split-cell-at-cursor")
+                    })), a.Vim.mapCommand("-", "action", "splitCell", {}, {
+                        extra: "normal"
+                    })
                 }
             }
-            var r = o(593);
-            const m = "@axlair/jupyterlab_vim",
-                u = "jupyterlab-vim:toggle";
-            let C = !1;
-            const v = {
-                id: m,
+            var u = o(593);
+            const C = "@axlair/jupyterlab_vim",
+                v = "jupyterlab-vim:toggle";
+            let b = !1,
+                f = !0;
+            const p = {
+                id: C,
                 autoStart: !0,
-                activate: async function(e, t, o, i) {
-                    const v = d.Prec.highest(c.EditorView.theme({
+                activate: async function(e, t, o, i, d) {
+                    const p = s.Prec.highest(c.EditorView.theme({
                         ".cm-fat-cursor": {
                             position: "absolute",
                             background: "var(--jp-vim-cursor-color)",
                             border: "none",
                             whiteSpace: "pre"
                         },
                         "&:not(.cm-focused) .cm-fat-cursor": {
                             background: "none",
                             outline: "solid 1px var(--jp-vim-cursor-color)",
                             color: "transparent !important"
                         }
                     }));
                     o.addExtension({
                         name: "vim",
-                        factory: e => l.EditorExtensionRegistry.createConditionalExtension([v, (0, a.vim)({
+                        factory: e => l.EditorExtensionRegistry.createConditionalExtension([p, (0, a.vim)({
                             status: !1
                         })])
-                    }), e.commands.addCommand(u, {
-                        label: "Enable Notebook Vim mode",
+                    }), e.commands.addCommand(v, {
+                        label: "Enable Vim Mode",
                         execute: () => {
-                            i && i.set(`${m}:plugin`, "enabled", !C)
+                            i && i.set(`${C}:plugin`, "enabled", !b)
                         },
-                        isToggled: () => C
+                        isToggled: () => b
+                    }), e.commands.addCommand("vim:enter-normal-mode", {
+                        label: "Enter Normal Vim Mode",
+                        execute: () => {
+                            const o = e.shell.currentWidget;
+                            o ? d.currentWidget === o ? w.modifyEditor(d.currentWidget.content.editor) : t.currentWidget === o ? h.modifyCell(t.currentWidget.content.activeCell) : console.warn("Current widget is not vim-enabled") : console.warn("Current widget not found")
+                        },
+                        isEnabled: () => b
                     });
-                    const b = (await i.get(`${m}:plugin`, "extraKeybindings")).composite;
-                    let f = null,
-                        p = null,
-                        w = !1;
+                    const g = (await i.get(`${C}:plugin`, "extraKeybindings")).composite,
+                        h = new m({
+                            commands: e.commands,
+                            enabled: b,
+                            userKeybindings: g
+                        }),
+                        w = new r({
+                            enabled: b && f,
+                            userKeybindings: g
+                        });
+                    let E = null,
+                        y = !1;
                     async function x(o) {
-                        const n = (await i.get(`${m}:plugin`, "extraKeybindings")).composite;
-                        C = !0 === o.get("enabled").composite, e.commands.notifyCommandChanged(u), f && (f.enabled = C, f.userKeybindings = n), C ? (null == p || p.dispose(), w || (w = !0, await e.restored)) : p = e.commands.addKeyBinding({
+                        const n = (await i.get(`${C}:plugin`, "extraKeybindings")).composite;
+                        b = !0 === o.get("enabled").composite, f = !0 === o.get("enabledInEditors").composite, e.commands.notifyCommandChanged(v), h.enabled = b, h.userKeybindings = n, w.enabled = b && f, w.userKeybindings = n, b ? (null == E || E.dispose(), y || (y = !0, await e.restored)) : E = e.commands.addKeyBinding({
                             command: "notebook:enter-command-mode",
                             keys: ["Escape"],
                             selector: ".jp-Notebook.jp-mod-editMode"
                         }), t.forEach((e => {
-                            e.node.dataset.jpVimMode = `${C}`
-                        })), null == f || f.modifyCell(f.lastActiveCell), t.widgetAdded.connect(((e, t) => {
-                            t.node.dataset.jpVimMode = `${C}`
+                            e.node.dataset.jpVimMode = `${b}`
+                        })), d.forEach((e => {
+                            e.node.dataset.jpVimMode = `${b&&f}`
+                        })), null == w || w.updateLastActive(), null == h || h.updateLastActive(), t.widgetAdded.connect(((e, t) => {
+                            t.node.dataset.jpVimMode = `${b}`
+                        })), d.widgetAdded.connect(((e, t) => {
+                            t.node.dataset.jpVimMode = `${b&&f}`
                         }))
                     }
                     return a.Vim.defineEx("write", "w", (() => {
                             e.commands.execute("docmanager:save")
                         })), a.Vim.defineEx("quit", "q", (() => {
                             setTimeout((() => {
                                 e.commands.execute("notebook:enter-command-mode")
                             }))
-                        })), f = new s({
-                            commands: e.commands,
-                            enabled: C,
-                            userKeybindings: b
-                        }), t.activeCellChanged.connect(f.onActiveCellChanged, f),
+                        })), t.activeCellChanged.connect(h.onActiveCellChanged, h), d.currentChanged.connect(w.onActiveEditorChanged, w),
                         function(e, t) {
                             const {
                                 commands: o,
-                                shell: l
+                                shell: i
                             } = e;
 
-                            function i(e) {
+                            function l(e) {
                                 const o = t.currentWidget;
-                                return !1 !== e.activate && o && l.currentWidget !== o && l.activateById(o.id), o
+                                return !1 !== e.activate && o && i.currentWidget !== o && i.activateById(o.id), o
                             }
 
-                            function c() {
+                            function d() {
                                 return null !== t.currentWidget && t.currentWidget === e.shell.currentWidget
                             }
                             o.addCommand("vim:run-select-next-edit", {
                                 label: "Run Cell and Edit Next Cell",
                                 execute: e => {
-                                    const t = i(e);
+                                    const t = l(e);
                                     if (t) {
                                         const {
                                             context: e,
                                             content: o
                                         } = t;
                                         n.NotebookActions.runAndAdvance(o, e.sessionContext), t.content.mode = "edit"
                                     }
                                 },
-                                isEnabled: c
+                                isEnabled: d
                             }), o.addCommand("vim:run-cell-and-edit", {
                                 label: "Run Cell and Edit Cell",
                                 execute: e => {
-                                    const t = i(e);
+                                    const t = l(e);
                                     if (t) {
                                         const {
                                             context: e,
                                             content: o
                                         } = t;
                                         n.NotebookActions.run(o, e.sessionContext), t.content.mode = "edit"
                                     }
                                 },
-                                isEnabled: c
+                                isEnabled: d
                             }), o.addCommand("vim:cut-cell-and-edit", {
                                 label: "Cut Cell(s) and Edit Cell",
                                 execute: e => {
-                                    const t = i(e);
+                                    const t = l(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
                                         n.NotebookActions.cut(e), e.mode = "edit"
                                     }
                                 },
-                                isEnabled: c
+                                isEnabled: d
                             }), o.addCommand("vim:copy-cell-and-edit", {
                                 label: "Copy Cell(s) and Edit Cell",
                                 execute: e => {
-                                    const t = i(e);
+                                    const t = l(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
                                         n.NotebookActions.copy(e), e.mode = "edit"
                                     }
                                 },
-                                isEnabled: c
+                                isEnabled: d
                             }), o.addCommand("vim:paste-cell-and-edit", {
                                 label: "Paste Cell(s) and Edit Cell",
                                 execute: e => {
-                                    const t = i(e);
+                                    const t = l(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
                                         n.NotebookActions.paste(e, "below"), e.mode = "edit"
                                     }
                                 },
-                                isEnabled: c
+                                isEnabled: d
                             }), o.addCommand("vim:merge-and-edit", {
                                 label: "Merge and Edit Cell",
                                 execute: e => {
-                                    const t = i(e);
+                                    const t = l(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
                                         n.NotebookActions.mergeCells(e), t.content.mode = "edit"
                                     }
                                 },
-                                isEnabled: c
+                                isEnabled: d
                             }), o.addCommand("vim:enter-insert-mode", {
                                 label: "Enter Insert Mode",
                                 execute: e => {
-                                    const t = i(e);
+                                    const t = l(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
                                         if (null !== e.activeCell) {
                                             const o = e.activeCell.editor;
                                             t.content.mode = "edit";
                                             const n = (0, a.getCM)(o.editor);
                                             if (!n) return void console.error("CodeMirror vim wrapper not found");
                                             a.Vim.handleKey(n, "i")
                                         }
                                     }
                                 },
-                                isEnabled: c
+                                isEnabled: d
                             }), o.addCommand("vim:leave-insert-mode", {
                                 label: "Leave Insert Mode",
                                 execute: e => {
-                                    const t = i(e);
+                                    const t = l(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
                                         if (null !== e.activeCell) {
                                             const t = e.activeCell.editor,
                                                 o = (0, a.getCM)(t.editor);
                                             if (!o) return void console.error("CodeMirror vim wrapper not found");
                                             a.Vim.handleKey(o, "<Esc>")
                                         }
                                     }
                                 },
-                                isEnabled: c
+                                isEnabled: d
                             }), o.addCommand("vim:leave-current-mode", {
                                 label: 'Move Insert to Normal to Jupyter Command Mode"',
                                 execute: e => {
-                                    const t = i(e);
+                                    const t = l(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
                                         if (null !== e.activeCell) {
                                             const t = e.activeCell.editor,
                                                 n = (0, a.getCM)(t.editor);
                                             if (!n) return void console.error("CodeMirror vim wrapper not found");
-                                            const l = n.state.vim;
-                                            l.insertMode || l.visualMode ? a.Vim.handleKey(n, "<Esc>") : o.execute("notebook:enter-command-mode")
+                                            const i = n.state.vim;
+                                            i.insertMode || i.visualMode ? a.Vim.handleKey(n, "<Esc>") : o.execute("notebook:enter-command-mode")
                                         }
                                     }
                                 },
-                                isEnabled: c
+                                isEnabled: d
                             }), o.addCommand("vim:select-below-execute-markdown", {
                                 label: "Execute Markdown and Select Cell Below",
                                 execute: e => {
-                                    const t = i(e);
+                                    const t = l(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
                                         return null !== e.activeCell && "markdown" === e.activeCell.model.type && (t.content.activeCell.rendered = !0), n.NotebookActions.selectBelow(t.content)
                                     }
                                 },
-                                isEnabled: c
+                                isEnabled: d
                             }), o.addCommand("vim:select-above-execute-markdown", {
                                 label: "Execute Markdown and Select Cell Below",
                                 execute: e => {
-                                    const t = i(e);
+                                    const t = l(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
                                         return null !== e.activeCell && "markdown" === e.activeCell.model.type && (t.content.activeCell.rendered = !0), n.NotebookActions.selectAbove(t.content)
                                     }
                                 },
-                                isEnabled: c
+                                isEnabled: d
                             }), o.addCommand("vim:select-first-cell", {
                                 label: "Select First Cell",
                                 execute: e => {
-                                    const t = i(e);
+                                    const t = l(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
-                                        e.activeCellIndex = 0, e.deselectAll(), null !== e.activeCell && r.ElementExt.scrollIntoViewIfNeeded(e.node, e.activeCell.node)
+                                        e.activeCellIndex = 0, e.deselectAll(), null !== e.activeCell && u.ElementExt.scrollIntoViewIfNeeded(e.node, e.activeCell.node)
                                     }
                                 },
-                                isEnabled: c
+                                isEnabled: d
                             }), o.addCommand("vim:select-last-cell", {
                                 label: "Select Last Cell",
                                 execute: e => {
-                                    const t = i(e);
+                                    const t = l(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
-                                        e.activeCellIndex = t.content.widgets.length - 1, e.deselectAll(), null !== e.activeCell && r.ElementExt.scrollIntoViewIfNeeded(e.node, e.activeCell.node)
+                                        e.activeCellIndex = t.content.widgets.length - 1, e.deselectAll(), null !== e.activeCell && u.ElementExt.scrollIntoViewIfNeeded(e.node, e.activeCell.node)
                                     }
                                 },
-                                isEnabled: c
+                                isEnabled: d
                             }), o.addCommand("vim:center-cell", {
                                 label: "Center Cell",
                                 execute: e => {
-                                    const t = i(e);
+                                    const t = l(e);
                                     t && null !== t.content.activeCell && t.content.scrollToCell(t.content.activeCell, "center")
                                 },
-                                isEnabled: c
+                                isEnabled: d
                             })
-                        }(e, t), i.load(`${m}:plugin`).then((e => {
+                        }(e, t), i.load(`${C}:plugin`).then((e => {
                             x(e), e.changed.connect(x)
                         }), (e => {
-                            console.error(`Could not load settings, so did not active ${m}: ${e}`)
+                            console.error(`Could not load settings, so did not active ${C}: ${e}`)
                         })), Promise.resolve()
                 },
-                requires: [n.INotebookTracker, l.IEditorExtensionRegistry, i.ISettingRegistry]
+                requires: [n.INotebookTracker, l.IEditorExtensionRegistry, d.ISettingRegistry],
+                optional: [i.IEditorTracker]
             }
         }
     }
 ]);
```

### Comparing `jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/747.a573445024188eae7034.js` & `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/747.a573445024188eae7034.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/remoteEntry.6d29f029f239ba56d940.js` & `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/remoteEntry.a73b7957e55f8d1b9f75.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, i, l, u, d, s, f, c, p, h, v, m, b, g, y = {
+    var e, r, t, a, o, n, i, l, u, d, f, s, c, p, h, v, m, b, g, y = {
             130: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(598), t.e(353)]).then((() => () => t(353))),
                         "./extension": () => Promise.all([t.e(598), t.e(353)]).then((() => () => t(353))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -44,21 +44,21 @@
     }, j.d = (e, r) => {
         for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         252: "e0500116419ca3a355d1",
-        353: "184fc74aa8db790efd40",
+        353: "8b609c372dc07b2baac6",
         598: "ad606b2bbb9816d73182",
         747: "a573445024188eae7034",
         818: "53acaa7ded124a9243cd"
     } [e] + ".js?v=" + {
         252: "e0500116419ca3a355d1",
-        353: "184fc74aa8db790efd40",
+        353: "8b609c372dc07b2baac6",
         598: "ad606b2bbb9816d73182",
         747: "a573445024188eae7034",
         818: "53acaa7ded124a9243cd"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
@@ -67,31 +67,31 @@
         }
     }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@axlair/jupyterlab_vim:", j.l = (t, a, o, n) => {
         if (e[t]) e[t].push(a);
         else {
             var i, l;
             if (void 0 !== o)
                 for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
-                    var s = u[d];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        i = s;
+                    var f = u[d];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        i = f;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [a];
-            var f = (r, a) => {
+            var s = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(a))), r) return r(a)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -113,15 +113,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@axlair/jupyterlab_vim", "0.17.0", (() => Promise.all([j.e(598), j.e(353)]).then((() => () => j(353))))), l("@replit/codemirror-vim", "6.0.14", (() => Promise.all([j.e(252), j.e(598), j.e(818)]).then((() => () => j(252)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@axlair/jupyterlab_vim", "4.0.0", (() => Promise.all([j.e(598), j.e(353)]).then((() => () => j(353))))), l("@replit/codemirror-vim", "6.0.14", (() => Promise.all([j.e(252), j.e(598), j.e(818)]).then((() => () => j(252)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -171,33 +171,33 @@
     }, n = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 o = a < 0;
             o && (a = -a - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var d, s, f = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !u || ("u" == f ? l > a && !o : "" == f != o);
-                if ("u" == s) {
-                    if (!u || "u" != f) return !1
+                var d, f, s = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !u || ("u" == s ? l > a && !o : "" == s != o);
+                if ("u" == f) {
+                    if (!u || "u" != s) return !1
                 } else if (u)
-                    if (f == s)
+                    if (s == f)
                         if (l <= a) {
                             if (d != e[l]) return !1
                         } else {
                             if (o ? d > e[l] : d < e[l]) return !1;
                             d != e[l] && (u = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != s && "n" != s) {
                     if (o || l <= a) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= a || s < f != o) return !1;
+                    if (l <= a || f < s != o) return !1;
                     u = !1
-                } else "s" != f && "n" != f && (u = !1, l--)
+                } else "s" != s && "n" != s && (u = !1, l--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? n(h, r) : !p())
@@ -208,38 +208,39 @@
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", d = (e, r, t, a) => {
         var o = l(e, t);
-        return n(a, o) || f(u(e, t, o, a)), c(e[t][o])
-    }, s = (e, r, t) => {
+        return n(a, o) || s(u(e, t, o, a)), c(e[t][o])
+    }, f = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !n(t, r) || e && !a(e, r) ? e : r), 0)) && o[r]
-    }, f = e => {
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, o) {
         var n = j.I(r);
         return n && n.then ? n.then(e.bind(e, r, j.S[r], t, a, o)) : e(r, j.S[r], t, a, o)
     })(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), v = p(((e, r, t, a, o) => {
-        var n = r && j.o(r, t) && s(r, t, a);
+        var n = r && j.o(r, t) && f(r, t, a);
         return n ? c(n) : o()
     })), m = {}, b = {
         204: () => h("default", "@codemirror/state", [1, 6, 2, 0]),
         211: () => h("default", "@codemirror/view", [1, 6, 9, 6]),
         408: () => h("default", "@jupyterlab/codemirror", [1, 4, 0, 3]),
         593: () => h("default", "@lumino/domutils", [1, 2, 0, 0]),
         663: () => h("default", "@jupyterlab/settingregistry", [1, 4, 0, 3]),
+        785: () => h("default", "@jupyterlab/fileeditor", [1, 4, 0, 3]),
         829: () => v("default", "@replit/codemirror-vim", [1, 6, 0, 14], (() => Promise.all([j.e(252), j.e(818)]).then((() => () => j(252))))),
         861: () => h("default", "@jupyterlab/notebook", [1, 4, 0, 3]),
         373: () => h("default", "@codemirror/language", [1, 6, 0, 0]),
         851: () => h("default", "@lezer/common", [1, 1, 0, 0])
     }, g = {
-        353: [408, 593, 663, 829, 861],
+        353: [408, 593, 663, 785, 829, 861],
         598: [204, 211],
         818: [373, 851]
     }, j.f.consumes = (e, r) => {
         j.o(g, e) && g[e].forEach((e => {
             if (j.o(m, e)) return r.push(m[e]);
             var t = r => {
                     m[e] = 0, j.m[e] = t => {
```

### Comparing `jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/third-party-licenses.json` & `jupyterlab_vim-4.0.0/jupyterlab_vim/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-0.17.0/schema/plugin.json` & `jupyterlab_vim-4.0.0/schema/plugin.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9716145833333334%*

 * *Differences: {"'jupyter.lab.shortcuts'": "{insert: [(1, OrderedDict([('command', 'vim:enter-normal-mode'), "*

 * *                            "('keys', ['Escape']), ('selector', '.jp-FileEditor')])), (2, "*

 * *                            "OrderedDict([('command', 'documentsearch:end'), ('keys', ['Escape']), "*

 * *                            "('selector', '.jp-mod-searchable .jp-FileEditor .cm-vimMode')])), (3, "*

 * *                            "OrderedDict([('command', 'documentsearch:end'), ('keys', ['Escape']), "*

 * *                      […]*

```diff
@@ -73,14 +73,49 @@
             "disabled": true,
             "keys": [
                 "Escape"
             ],
             "selector": ".jp-Notebook.jp-mod-editMode"
         },
         {
+            "command": "vim:enter-normal-mode",
+            "keys": [
+                "Escape"
+            ],
+            "selector": ".jp-FileEditor"
+        },
+        {
+            "command": "documentsearch:end",
+            "keys": [
+                "Escape"
+            ],
+            "selector": ".jp-mod-searchable .jp-FileEditor .cm-vimMode"
+        },
+        {
+            "command": "documentsearch:end",
+            "keys": [
+                "Escape"
+            ],
+            "selector": ".jp-mod-searchable .jp-Notebook .cm-vimMode"
+        },
+        {
+            "command": "documentsearch:end",
+            "keys": [
+                "Escape"
+            ],
+            "selector": ".jp-mod-search-active .jp-FileEditor .cm-vimMode"
+        },
+        {
+            "command": "documentsearch:end",
+            "keys": [
+                "Escape"
+            ],
+            "selector": ".jp-mod-search-active .jp-Notebook .cm-vimMode"
+        },
+        {
             "command": "notebook:undo-cell-action",
             "keys": [
                 "Ctrl O",
                 "U"
             ],
             "selector": ".jp-NotebookPanel[data-jp-vim-mode='true'] .jp-Notebook.jp-mod-editMode"
         },
@@ -404,18 +439,24 @@
             ],
             "selector": ".jp-NotebookPanel[data-jp-vim-mode='true'] .jp-Notebook.jp-mod-editMode .jp-InputArea-editor:not(.jp-mod-has-primary-selection)"
         }
     ],
     "properties": {
         "enabled": {
             "default": true,
-            "description": "Enable/disable notebook vim (may require a page refresh)",
+            "description": "Enable/disable vim extension (may require a page refresh)",
             "title": "Enabled",
             "type": "boolean"
         },
+        "enabledInEditors": {
+            "default": true,
+            "description": "Enable/disable vim in text editors (may require a page refresh)",
+            "title": "Enabled in Text Editor",
+            "type": "boolean"
+        },
         "extraKeybindings": {
             "default": [],
             "items": {
                 "$ref": "#/definitions/shortcut"
             },
             "title": "Extra Vim Keybindings",
             "type": "array"
```

### Comparing `jupyterlab_vim-0.17.0/src/codemirrorCommands.ts` & `jupyterlab_vim-4.0.0/src/codemirrorCommands.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import { Cell, ICellModel, MarkdownCell } from '@jupyterlab/cells';
 import { CodeMirrorEditor } from '@jupyterlab/codemirror';
 import { INotebookTracker } from '@jupyterlab/notebook';
+import { IEditorTracker, FileEditor } from '@jupyterlab/fileeditor';
+import { IDocumentWidget } from '@jupyterlab/docregistry';
+import type { CodeEditor } from '@jupyterlab/codeeditor';
 import { CommandRegistry } from '@lumino/commands';
 import { Vim, getCM, CodeMirror } from '@replit/codemirror-vim';
 
 // It may be worth contributing types for these upstream
 interface IVimCodeMirror extends CodeMirror {
   moveByLines: undefined;
   moveByDisplayLines: undefined;
@@ -17,278 +20,339 @@
   command: string;
   keys: string;
   context: string;
   mapfn: string;
   enabled: boolean;
 }
 
-export interface IOptions {
-  commands: CommandRegistry;
-  enabled: boolean;
-  userKeybindings: IKeybinding[];
+export namespace VimEditorManager {
+  export interface IOptions {
+    enabled: boolean;
+    userKeybindings: IKeybinding[];
+  }
 }
 
-export class VimCellManager {
-  constructor({ commands, enabled, userKeybindings }: IOptions) {
-    this._commands = commands;
-    this.enabled = enabled;
-    this.lastActiveCell = null;
-    this.userKeybindings = userKeybindings ?? [];
+export namespace VimCellManager {
+  export interface IOptions extends VimEditorManager.IOptions {
+    commands: CommandRegistry;
   }
+}
 
-  onActiveCellChanged(
-    tracker: INotebookTracker,
-    activeCell: Cell<ICellModel> | null
-  ): void {
-    this.modifyCell(activeCell).catch(console.error);
+interface IUndoOptions {
+  repeat: number;
+  repeatIsExplicit: boolean;
+  registerName: unknown;
+}
+
+export class VimEditorManager {
+  constructor({ enabled, userKeybindings }: VimEditorManager.IOptions) {
+    this.enabled = enabled;
+    this.userKeybindings = userKeybindings ?? [];
   }
 
-  async modifyCell(activeCell: Cell<ICellModel> | null): Promise<void> {
-    if (!activeCell) {
+  async onActiveEditorChanged(
+    tracker: IEditorTracker,
+    activeEditor: IDocumentWidget<FileEditor> | null
+  ): Promise<void> {
+    if (!activeEditor) {
       return;
     }
-    this.lastActiveCell = activeCell;
-    await activeCell.ready;
-    const editor = activeCell.editor as CodeMirrorEditor | null;
+    await activeEditor.content.ready;
+    this.modifyEditor(activeEditor.content.editor);
+  }
 
-    if (activeCell.isDisposed) {
-      console.warn('Cell was already disposed, cannot setup vim mode');
-      return;
-    }
+  updateLastActive() {
+    this.modifyEditor(this._lastActiveEditor);
+  }
 
-    if (!editor) {
-      throw Error('Cell editor not available');
+  modifyEditor(editor: CodeEditor.IEditor | null): boolean {
+    // JupyterLab 4.0 only supports CodeMirror editors
+    const mirrorEditor = editor as CodeMirrorEditor | null;
+
+    if (!mirrorEditor) {
+      throw Error('Editor not available');
     }
+    this._lastActiveEditor = mirrorEditor;
 
-    const view = editor.editor;
+    const view = mirrorEditor.editor;
 
     if (this.enabled) {
-      if (!editor.getOption('vim')) {
+      if (!mirrorEditor.getOption('vim')) {
         // this erases state, we do not want to call it if not needed.
-        editor.setOption('vim', true);
+        mirrorEditor.setOption('vim', true);
 
         // On each key press the notebook (`Notebook.handleEvent`) invokes
         // a handler ensuring focus (`Notebook._ensureFocus`); the logic does
         // not work well for the `ex commands` panel which is always interpreted
         // as blurred because it exists outside of the CodeMirror6 state; here
         // we override `hasFocus` handler to ensure it is taken into account.
         const cm = getCM(view)!;
-        editor.hasFocus = () => {
+        mirrorEditor.hasFocus = () => {
           if (
             cm.state.dialog &&
             cm.state.dialog.contains(document.activeElement)
           ) {
             return true;
           }
           return view.hasFocus;
         };
       }
+
+      // Override vim-mode undo/redo to make it work with JupyterLab RTC-aware
+      // history; it needs to happen on every change of the editor.
+      Vim.defineAction('undo', (cm: CodeMirror, options: IUndoOptions) => {
+        for (let i = 0; i < options.repeat; i++) {
+          editor!.undo();
+        }
+      });
+      Vim.defineAction('redo', (cm: CodeMirror, options: IUndoOptions) => {
+        for (let i = 0; i < options.repeat; i++) {
+          editor!.redo();
+        }
+      });
+
       const lcm = getCM(view);
-      const lvim = Vim;
 
       // Clear existing user keybindings, then re-register in case they changed in the user settings
-      ['normal', 'visual', 'insert'].forEach(ctx => lvim.mapclear(ctx));
+      ['normal', 'visual', 'insert'].forEach(ctx => Vim.mapclear(ctx));
       this.userKeybindings.forEach(
         ({
           command,
           keys,
           context,
           mapfn,
           enabled: keybindEnabled
         }: IKeybinding) => {
           if (keybindEnabled) {
             if (mapfn === 'map') {
-              lvim.map(command, keys, context);
+              Vim.map(command, keys, context);
             } else {
-              lvim.noremap(command, keys, context);
+              Vim.noremap(command, keys, context);
             }
           }
         }
       );
 
       Vim.handleKey(lcm, '<Esc>');
 
-      // Define a function to use as Vim motion
-      // This replaces the codemirror moveByLines function to
-      // for jumping between notebook cells.
-      const moveByLinesOrCell = (
-        cm: IVimCodeMirror,
-        head: any,
-        motionArgs: any,
-        vim: any
-      ): any => {
-        const cur = head;
-        let endCh = cur.ch;
-        const currentCell = activeCell;
-        // TODO: these references will be undefined
-        // Depending what our last motion was, we may want to do different
-        // things. If our last motion was moving vertically, we want to
-        // preserve the HPos from our last horizontal move.  If our last motion
-        // was going to the end of a line, moving vertically we should go to
-        // the end of the line, etc.
-        switch (vim?.lastMotion) {
-          case cm.moveByLines:
-          case cm.moveByDisplayLines:
-          case cm.moveByScroll:
-          case cm.moveToColumn:
-          case cm.moveToEol:
-          // JUPYTER PATCH: add our custom method to the motion cases
-          // eslint-disable-next-line no-fallthrough
-          case moveByLinesOrCell:
-            endCh = vim.lastHPos;
-            break;
-          default:
-            vim.lastHPos = endCh;
-        }
-        const repeat = motionArgs.repeat + (motionArgs.repeatOffset || 0);
-        let line = motionArgs.forward ? cur.line + repeat : cur.line - repeat;
-        const first = cm.firstLine();
-        const last = cm.lastLine();
-        const posV = cm.findPosV(
-          cur,
-          motionArgs.forward ? repeat : -repeat,
-          'line',
-          vim.lastHSPos
-        );
-        const hasMarkedText = motionArgs.forward
-          ? posV.line > line
-          : posV.line < line;
-        if (hasMarkedText) {
-          line = posV.line;
-          endCh = posV.ch;
-        }
+      return true;
+    } else if (mirrorEditor.getOption('vim')) {
+      mirrorEditor.setOption('vim', false);
+      return false;
+    }
+    return false;
+  }
 
-        // JUPYTER PATCH BEGIN
-        // here we insert the jumps to the next cells
+  private _lastActiveEditor: CodeEditor.IEditor | null = null;
+  public enabled: boolean;
+  public userKeybindings: IKeybinding[];
+}
 
-        if (line < first || line > last) {
-          // var currentCell = ns.notebook.get_selected_cell();
-          // var currentCell = tracker.activeCell;
-          // var key = '';
-          // `currentCell !== null should not be needed since `activeCell`
-          // is already check against null (row 61). Added to avoid warning.
-          if (currentCell !== null && currentCell.model.type === 'markdown') {
-            if (!motionArgs.handleArrow) {
-              // markdown cells tends to improperly handle arrow keys movement,
-              //  on the way up the cell is rendered, but down movement is ignored
-              //  when use arrows the cell will remain unrendered (need to shift+enter)
-              //  However, this is the same as Jupyter default behaviour
-              (currentCell as MarkdownCell).rendered = true;
-            }
-            // currentCell.execute();
+export class VimCellManager extends VimEditorManager {
+  constructor({ commands, enabled, userKeybindings }: VimCellManager.IOptions) {
+    super({ userKeybindings, enabled });
+    this._commands = commands;
+  }
+
+  onActiveCellChanged(
+    tracker: INotebookTracker,
+    activeCell: Cell<ICellModel> | null
+  ): void {
+    this.modifyCell(activeCell).catch(console.error);
+  }
+
+  updateLastActive() {
+    this.modifyCell(this._lastActiveCell);
+  }
+
+  async modifyCell(activeCell: Cell<ICellModel> | null): Promise<void> {
+    if (!activeCell) {
+      return;
+    }
+    this._lastActiveCell = activeCell;
+    await activeCell.ready;
+
+    if (activeCell.isDisposed) {
+      console.warn('Cell was already disposed, cannot setup vim mode');
+      return;
+    }
+    const wasEnabled = this.modifyEditor(activeCell.editor);
+    if (wasEnabled) {
+      this._modifyEdgeNavigation(activeCell);
+    }
+  }
+
+  private _modifyEdgeNavigation(activeCell: Cell<ICellModel>) {
+    // Define a function to use as Vim motion
+    // This replaces the codemirror moveByLines function to
+    // for jumping between notebook cells.
+    const moveByLinesOrCell = (
+      cm: IVimCodeMirror,
+      head: any,
+      motionArgs: any,
+      vim: any
+    ): any => {
+      const cur = head;
+      let endCh = cur.ch;
+      const currentCell = activeCell;
+      // TODO: these references will be undefined
+      // Depending what our last motion was, we may want to do different
+      // things. If our last motion was moving vertically, we want to
+      // preserve the HPos from our last horizontal move.  If our last motion
+      // was going to the end of a line, moving vertically we should go to
+      // the end of the line, etc.
+      switch (vim?.lastMotion) {
+        case cm.moveByLines:
+        case cm.moveByDisplayLines:
+        case cm.moveByScroll:
+        case cm.moveToColumn:
+        case cm.moveToEol:
+        // JUPYTER PATCH: add our custom method to the motion cases
+        // eslint-disable-next-line no-fallthrough
+        case moveByLinesOrCell:
+          endCh = vim.lastHPos;
+          break;
+        default:
+          vim.lastHPos = endCh;
+      }
+      const repeat = motionArgs.repeat + (motionArgs.repeatOffset || 0);
+      let line = motionArgs.forward ? cur.line + repeat : cur.line - repeat;
+      const first = cm.firstLine();
+      const last = cm.lastLine();
+      const posV = cm.findPosV(
+        cur,
+        motionArgs.forward ? repeat : -repeat,
+        'line',
+        vim.lastHSPos
+      );
+      const hasMarkedText = motionArgs.forward
+        ? posV.line > line
+        : posV.line < line;
+      if (hasMarkedText) {
+        line = posV.line;
+        endCh = posV.ch;
+      }
+
+      // JUPYTER PATCH BEGIN
+      // here we insert the jumps to the next cells
+
+      if (line < first || line > last) {
+        // var currentCell = ns.notebook.get_selected_cell();
+        // var currentCell = tracker.activeCell;
+        // var key = '';
+        // `currentCell !== null should not be needed since `activeCell`
+        // is already check against null (row 61). Added to avoid warning.
+        if (currentCell !== null && currentCell.model.type === 'markdown') {
+          if (!motionArgs.handleArrow) {
+            // markdown cells tends to improperly handle arrow keys movement,
+            //  on the way up the cell is rendered, but down movement is ignored
+            //  when use arrows the cell will remain unrendered (need to shift+enter)
+            //  However, this is the same as Jupyter default behaviour
+            (currentCell as MarkdownCell).rendered = true;
           }
-          if (motionArgs.forward) {
-            // ns.notebook.select_next();
-            if (!motionArgs.handleArrow) {
+          // currentCell.execute();
+        }
+        if (motionArgs.forward) {
+          // ns.notebook.select_next();
+          if (!motionArgs.handleArrow) {
+            this._commands.execute('notebook:move-cursor-down');
+          } else {
+            // This block preventing double cell hop when you use arrow keys for navigation
+            //    also arrow key navigation works properly when current cursor position
+            //    at the beginning of line for up move, and at the end for down move
+            const cursor = cm.getCursor();
+            // CM6 is 1-based
+            const last_char = cm.cm6.state.doc.line(last + 1).length;
+            if (cursor.line !== last || cursor.ch !== last_char) {
+              cm.setCursor(last, last_char);
               this._commands.execute('notebook:move-cursor-down');
-            } else {
-              // This block preventing double cell hop when you use arrow keys for navigation
-              //    also arrow key navigation works properly when current cursor position
-              //    at the beginning of line for up move, and at the end for down move
-              const cursor = cm.getCursor();
-              // CM6 is 1-based
-              const last_char = view.state.doc.line(last + 1).length;
-              if (cursor.line !== last || cursor.ch !== last_char) {
-                cm.setCursor(last, last_char);
-                this._commands.execute('notebook:move-cursor-down');
-              }
             }
-            // key = 'j';
+          }
+          // key = 'j';
+        } else {
+          // ns.notebook.select_prev();
+          if (!motionArgs.handleArrow) {
+            this._commands.execute('notebook:move-cursor-up');
           } else {
-            // ns.notebook.select_prev();
-            if (!motionArgs.handleArrow) {
+            // This block preventing double cell hop when you use arrow keys for navigation
+            //    also arrow key navigation works properly when current cursor position
+            //    at the beginning of line for up move, and at the end for down move
+            const cursor = cm.getCursor();
+            if (cursor.line !== 0 || cursor.ch !== 0) {
+              cm.setCursor(0, 0);
               this._commands.execute('notebook:move-cursor-up');
-            } else {
-              // This block preventing double cell hop when you use arrow keys for navigation
-              //    also arrow key navigation works properly when current cursor position
-              //    at the beginning of line for up move, and at the end for down move
-              const cursor = cm.getCursor();
-              if (cursor.line !== 0 || cursor.ch !== 0) {
-                cm.setCursor(0, 0);
-                this._commands.execute('notebook:move-cursor-up');
-              }
             }
-            // key = 'k';
-          }
-          return;
-        }
-        // JUPYTER PATCH END
-
-        // function taken from https://github.com/codemirror/CodeMirror/blob/9d0f9d19de70abe817e8b8e161034fbd3f907030/keymap/vim.js#L3328
-        function findFirstNonWhiteSpaceCharacter(text: any): number {
-          if (!text) {
-            return 0;
           }
-          const firstNonWS = text.search(/\S/);
-          return firstNonWS === -1 ? text.length : firstNonWS;
+          // key = 'k';
         }
+        return;
+      }
+      // JUPYTER PATCH END
 
-        if (motionArgs.toFirstChar) {
-          endCh = findFirstNonWhiteSpaceCharacter(cm.getLine(line));
-          vim.lastHPos = endCh;
+      // function taken from https://github.com/codemirror/CodeMirror/blob/9d0f9d19de70abe817e8b8e161034fbd3f907030/keymap/vim.js#L3328
+      function findFirstNonWhiteSpaceCharacter(text: any): number {
+        if (!text) {
+          return 0;
         }
+        const firstNonWS = text.search(/\S/);
+        return firstNonWS === -1 ? text.length : firstNonWS;
+      }
 
-        vim.lastHSPos = cm.charCoords(
-          new CodeMirror.Pos(line, endCh),
-          'div'
-        ).left;
-        return new CodeMirror.Pos(line, endCh);
-      };
-      lvim.defineMotion('moveByLinesOrCell', moveByLinesOrCell);
-
-      lvim.mapCommand(
-        '<Up>',
-        'motion',
-        'moveByLinesOrCell',
-        { forward: false, linewise: true, handleArrow: true },
-        { context: 'normal' }
-      );
-      lvim.mapCommand(
-        '<Down>',
-        'motion',
-        'moveByLinesOrCell',
-        { forward: true, linewise: true, handleArrow: true },
-        { context: 'normal' }
-      );
-      lvim.mapCommand(
-        'k',
-        'motion',
-        'moveByLinesOrCell',
-        { forward: false, linewise: true },
-        { context: 'normal' }
-      );
-      lvim.mapCommand(
-        'j',
-        'motion',
-        'moveByLinesOrCell',
-        { forward: true, linewise: true },
-        { context: 'normal' }
-      );
+      if (motionArgs.toFirstChar) {
+        endCh = findFirstNonWhiteSpaceCharacter(cm.getLine(line));
+        vim.lastHPos = endCh;
+      }
 
-      lvim.defineAction('moveCellDown', (cm: any, actionArgs: any) => {
-        this._commands.execute('notebook:move-cell-down');
-      });
-      lvim.defineAction('moveCellUp', (cm: any, actionArgs: any) => {
-        this._commands.execute('notebook:move-cell-up');
-      });
-      lvim.mapCommand(
-        '<C-e>',
-        'action',
-        'moveCellDown',
-        {},
-        { extra: 'normal' }
-      );
-      lvim.mapCommand('<C-y>', 'action', 'moveCellUp', {}, { extra: 'normal' });
-      lvim.defineAction('splitCell', (cm: any, actionArgs: any) => {
-        this._commands.execute('notebook:split-cell-at-cursor');
-      });
-      lvim.mapCommand('-', 'action', 'splitCell', {}, { extra: 'normal' });
-    } else if (editor.getOption('vim')) {
-      editor.setOption('vim', false);
-    }
+      vim.lastHSPos = cm.charCoords(
+        new CodeMirror.Pos(line, endCh),
+        'div'
+      ).left;
+      return new CodeMirror.Pos(line, endCh);
+    };
+    Vim.defineMotion('moveByLinesOrCell', moveByLinesOrCell);
+
+    Vim.mapCommand(
+      '<Up>',
+      'motion',
+      'moveByLinesOrCell',
+      { forward: false, linewise: true, handleArrow: true },
+      { context: 'normal' }
+    );
+    Vim.mapCommand(
+      '<Down>',
+      'motion',
+      'moveByLinesOrCell',
+      { forward: true, linewise: true, handleArrow: true },
+      { context: 'normal' }
+    );
+    Vim.mapCommand(
+      'k',
+      'motion',
+      'moveByLinesOrCell',
+      { forward: false, linewise: true },
+      { context: 'normal' }
+    );
+    Vim.mapCommand(
+      'j',
+      'motion',
+      'moveByLinesOrCell',
+      { forward: true, linewise: true },
+      { context: 'normal' }
+    );
+
+    Vim.defineAction('moveCellDown', (cm: any, actionArgs: any) => {
+      this._commands.execute('notebook:move-cell-down');
+    });
+    Vim.defineAction('moveCellUp', (cm: any, actionArgs: any) => {
+      this._commands.execute('notebook:move-cell-up');
+    });
+    Vim.mapCommand('<C-e>', 'action', 'moveCellDown', {}, { extra: 'normal' });
+    Vim.mapCommand('<C-y>', 'action', 'moveCellUp', {}, { extra: 'normal' });
+    Vim.defineAction('splitCell', (cm: any, actionArgs: any) => {
+      this._commands.execute('notebook:split-cell-at-cursor');
+    });
+    Vim.mapCommand('-', 'action', 'splitCell', {}, { extra: 'normal' });
   }
 
   private _commands: CommandRegistry;
-  public lastActiveCell: Cell<ICellModel> | null;
-  public enabled: boolean;
-  public userKeybindings: IKeybinding[];
+  private _lastActiveCell: Cell<ICellModel> | null = null;
 }
```

### Comparing `jupyterlab_vim-0.17.0/src/index.ts` & `jupyterlab_vim-4.0.0/src/index.ts`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
 import { INotebookTracker } from '@jupyterlab/notebook';
+import { IEditorTracker } from '@jupyterlab/fileeditor';
 
 import {
   IEditorExtensionRegistry,
   EditorExtensionRegistry
 } from '@jupyterlab/codemirror';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { IDisposable } from '@lumino/disposable';
 import { vim, Vim } from '@replit/codemirror-vim';
 import { EditorView } from '@codemirror/view';
 import { Prec } from '@codemirror/state';
 
-import { VimCellManager, IKeybinding } from './codemirrorCommands';
-import { addJLabCommands } from './labCommands';
+import {
+  VimEditorManager,
+  VimCellManager,
+  IKeybinding
+} from './codemirrorCommands';
+import { addNotebookCommands } from './labCommands';
 
 const PLUGIN_NAME = '@axlair/jupyterlab_vim';
 const TOGGLE_ID = 'jupyterlab-vim:toggle';
 let enabled = false;
+let enabledInEditors = true;
 
 /**
  * Initialization data for the jupyterlab_vim extension.
  */
 const extension: JupyterFrontEndPlugin<void> = {
   id: PLUGIN_NAME,
   autoStart: true,
   activate: activateCellVim,
-  requires: [INotebookTracker, IEditorExtensionRegistry, ISettingRegistry]
+  requires: [INotebookTracker, IEditorExtensionRegistry, ISettingRegistry],
+  optional: [IEditorTracker]
 };
 
 async function activateCellVim(
   app: JupyterFrontEnd,
-  tracker: INotebookTracker,
+  notebookTracker: INotebookTracker,
   editorExtensionRegistry: IEditorExtensionRegistry,
-  settingRegistry: ISettingRegistry
+  settingRegistry: ISettingRegistry,
+  editorTracker: IEditorTracker
 ): Promise<void> {
   const theme = Prec.highest(
     EditorView.theme({
       '.cm-fat-cursor': {
         position: 'absolute',
         background: 'var(--jp-vim-cursor-color)',
         border: 'none',
@@ -63,28 +71,56 @@
           status: false
         })
       ]);
     }
   });
 
   app.commands.addCommand(TOGGLE_ID, {
-    label: 'Enable Notebook Vim mode',
+    label: 'Enable Vim Mode',
     execute: () => {
       if (settingRegistry) {
         void settingRegistry.set(`${PLUGIN_NAME}:plugin`, 'enabled', !enabled);
       }
     },
     isToggled: () => enabled
   });
 
+  app.commands.addCommand('vim:enter-normal-mode', {
+    label: 'Enter Normal Vim Mode',
+    execute: () => {
+      const current = app.shell.currentWidget;
+      if (!current) {
+        console.warn('Current widget not found');
+      } else if (editorTracker.currentWidget === current) {
+        editorManager.modifyEditor(editorTracker.currentWidget.content.editor);
+      } else if (notebookTracker.currentWidget === current) {
+        cellManager.modifyCell(
+          notebookTracker.currentWidget.content.activeCell
+        );
+      } else {
+        console.warn('Current widget is not vim-enabled');
+      }
+    },
+    isEnabled: () => enabled
+  });
+
   const userKeybindings = (
     await settingRegistry.get(`${PLUGIN_NAME}:plugin`, 'extraKeybindings')
   ).composite as unknown as Array<IKeybinding>;
 
-  let cellManager: VimCellManager | null = null;
+  const cellManager = new VimCellManager({
+    commands: app.commands,
+    enabled,
+    userKeybindings
+  });
+  const editorManager = new VimEditorManager({
+    enabled: enabled && enabledInEditors,
+    userKeybindings
+  });
+
   let escBinding: IDisposable | null = null;
   let hasEverBeenEnabled = false;
 
   Vim.defineEx('write', 'w', () => {
     app.commands.execute('docmanager:save');
   });
 
@@ -92,66 +128,76 @@
     // In JupyterLab 4.0 needs to be executed after vim panel has closed, here
     // achived by moving it to end of execution stack with `setTimeout()`.
     setTimeout(() => {
       app.commands.execute('notebook:enter-command-mode');
     });
   });
 
-  cellManager = new VimCellManager({
-    commands: app.commands,
-    enabled,
-    userKeybindings
-  });
   // it's ok to connect here because we will never reach the vim section unless
   // ensureVimKeyMap has been called due to the checks for enabled.
   // we need to have now in order to keep track of the last active cell
   // so that we can modify it when vim is turned on or off.
-  tracker.activeCellChanged.connect(
+  notebookTracker.activeCellChanged.connect(
     cellManager.onActiveCellChanged,
     cellManager
   );
+  editorTracker.currentChanged.connect(
+    editorManager.onActiveEditorChanged,
+    editorManager
+  );
 
-  addJLabCommands(app, tracker);
+  addNotebookCommands(app, notebookTracker);
 
   async function updateSettings(
     settings: ISettingRegistry.ISettings
   ): Promise<void> {
     const userKeybindings = (
       await settingRegistry.get(`${PLUGIN_NAME}:plugin`, 'extraKeybindings')
     ).composite as unknown as Array<IKeybinding>;
 
     enabled = settings.get('enabled').composite === true;
+    enabledInEditors = settings.get('enabledInEditors').composite === true;
     app.commands.notifyCommandChanged(TOGGLE_ID);
-    if (cellManager) {
-      cellManager.enabled = enabled;
-      cellManager.userKeybindings = userKeybindings;
-    }
+
+    cellManager.enabled = enabled;
+    cellManager.userKeybindings = userKeybindings;
+
+    editorManager.enabled = enabled && enabledInEditors;
+    editorManager.userKeybindings = userKeybindings;
+
     if (enabled) {
       escBinding?.dispose();
       if (!hasEverBeenEnabled) {
         hasEverBeenEnabled = true;
         await app.restored;
       }
     } else {
       escBinding = app.commands.addKeyBinding({
         command: 'notebook:enter-command-mode',
         keys: ['Escape'],
         selector: '.jp-Notebook.jp-mod-editMode'
       });
     }
 
-    tracker.forEach(notebook => {
+    notebookTracker.forEach(notebook => {
       notebook.node.dataset.jpVimMode = `${enabled}`;
     });
-    cellManager?.modifyCell(cellManager.lastActiveCell);
+    editorTracker.forEach(document => {
+      document.node.dataset.jpVimMode = `${enabled && enabledInEditors}`;
+    });
+    editorManager?.updateLastActive();
+    cellManager?.updateLastActive();
 
     // make sure our css selector is added to new notebooks
-    tracker.widgetAdded.connect((sender, notebook) => {
+    notebookTracker.widgetAdded.connect((sender, notebook) => {
       notebook.node.dataset.jpVimMode = `${enabled}`;
     });
+    editorTracker.widgetAdded.connect((sender, document) => {
+      document.node.dataset.jpVimMode = `${enabled && enabledInEditors}`;
+    });
   }
 
   settingRegistry.load(`${PLUGIN_NAME}:plugin`).then(
     (settings: ISettingRegistry.ISettings) => {
       updateSettings(settings);
       settings.changed.connect(updateSettings);
     },
```

### Comparing `jupyterlab_vim-0.17.0/src/labCommands.ts` & `jupyterlab_vim-4.0.0/src/labCommands.ts`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   NotebookPanel
 } from '@jupyterlab/notebook';
 import { ReadonlyPartialJSONObject } from '@lumino/coreutils';
 
 import { IDisposable } from '@lumino/disposable';
 import { ElementExt } from '@lumino/domutils';
 
-export function addJLabCommands(
+export function addNotebookCommands(
   app: JupyterFrontEnd,
   tracker: INotebookTracker
 ): Array<IDisposable> {
   const { commands, shell } = app;
   function getCurrent(args: ReadonlyPartialJSONObject): NotebookPanel | null {
     const widget = tracker.currentWidget;
     const activate = args['activate'] !== false;
```

### Comparing `jupyterlab_vim-0.17.0/.gitignore` & `jupyterlab_vim-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-0.17.0/LICENSE` & `jupyterlab_vim-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-0.17.0/README.md` & `jupyterlab_vim-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-0.17.0/pyproject.toml` & `jupyterlab_vim-4.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-0.17.0/PKG-INFO` & `jupyterlab_vim-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_vim
-Version: 0.17.0
+Version: 4.0.0
 Summary: Code cell vim bindings
 Project-URL: Homepage, https://github.com/jupyterlab-contrib/jupyterlab-vim
 Project-URL: Bug Tracker, https://github.com/jupyterlab-contrib/jupyterlab-vim/issues
 Project-URL: Repository, https://github.com/jupyterlab-contrib/jupyterlab-vim.git
 Author: Axel Fahy
 License: MIT License
```

