# Comparing `tmp/jupyterlab_vim-0.16.0.tar.gz` & `tmp/jupyterlab_vim-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_vim-0.16.0.tar", last modified: Sun Mar 12 23:21:50 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab_vim-0.16.0.tar` & `jupyterlab_vim-0.17.0.tar`

### file list

```diff
@@ -1,39 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:50.554575 jupyterlab_vim-0.16.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-12 23:20:09.000000 jupyterlab_vim-0.16.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-12 23:20:09.000000 jupyterlab_vim-0.16.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-03-12 23:21:50.554575 jupyterlab_vim-0.16.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-03-12 23:20:09.000000 jupyterlab_vim-0.16.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-12 23:20:09.000000 jupyterlab_vim-0.16.0/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:50.550575 jupyterlab_vim-0.16.0/jupyterlab_vim/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-12 23:20:09.000000 jupyterlab_vim-0.16.0/jupyterlab_vim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-12 23:20:09.000000 jupyterlab_vim-0.16.0/jupyterlab_vim/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:50.554575 jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-03-12 23:21:50.000000 jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:50.550575 jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:50.550575 jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/@axlair/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:50.554575 jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-12 23:21:49.000000 jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-03-12 23:21:49.000000 jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:50.554575 jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-03-12 23:21:50.000000 jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/static/830.29023cea9c147059457e.js
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-03-12 23:21:50.000000 jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/static/remoteEntry.383e80b88deea45d9495.js
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-12 23:21:49.000000 jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/static/style.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:50.554575 jupyterlab_vim-0.16.0/jupyterlab_vim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-03-12 23:21:50.000000 jupyterlab_vim-0.16.0/jupyterlab_vim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-12 23:21:50.000000 jupyterlab_vim-0.16.0/jupyterlab_vim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 23:21:50.000000 jupyterlab_vim-0.16.0/jupyterlab_vim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 23:21:06.000000 jupyterlab_vim-0.16.0/jupyterlab_vim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-12 23:21:50.000000 jupyterlab_vim-0.16.0/jupyterlab_vim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-12 23:20:15.000000 jupyterlab_vim-0.16.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-12 23:20:09.000000 jupyterlab_vim-0.16.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 23:21:50.554575 jupyterlab_vim-0.16.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-03-12 23:20:09.000000 jupyterlab_vim-0.16.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:50.554575 jupyterlab_vim-0.16.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-03-12 23:20:09.000000 jupyterlab_vim-0.16.0/src/codemirrorCommands.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-03-12 23:20:09.000000 jupyterlab_vim-0.16.0/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-03-12 23:20:09.000000 jupyterlab_vim-0.16.0/src/labCommands.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 23:21:50.554575 jupyterlab_vim-0.16.0/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 23:20:09.000000 jupyterlab_vim-0.16.0/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 23:20:09.000000 jupyterlab_vim-0.16.0/style/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-12 23:20:09.000000 jupyterlab_vim-0.16.0/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)   191574 2023-03-12 23:20:09.000000 jupyterlab_vim-0.16.0/yarn.lock
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/.eslintignore
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/.prettierrc
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/.yarnrc.yml
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/RELEASE.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/Untitled.ipynb
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/install.json
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/installing.md
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/modify-keybinds.md
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/tsconfig.json
+-rw-r--r--   0        0        0   211305 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/yarn.lock
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/_version.py
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/package.json
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig
+-rw-r--r--   0        0        0     9952 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json
+-rw-r--r--   0        0        0   130333 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/252.e0500116419ca3a355d1.js
+-rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/353.184fc74aa8db790efd40.js
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/747.a573445024188eae7034.js
+-rw-r--r--   0        0        0     7518 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/remoteEntry.6d29f029f239ba56d940.js
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/style.js
+-rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     9952 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/schema/plugin.json
+-rw-r--r--   0        0        0    10125 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/src/codemirrorCommands.ts
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/src/index.ts
+-rw-r--r--   0        0        0     8183 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/src/labCommands.ts
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/style/index.js
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/LICENSE
+-rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/README.md
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/pyproject.toml
+-rw-r--r--   0        0        0     8706 2020-02-02 00:00:00.000000 jupyterlab_vim-0.17.0/PKG-INFO
```

### Comparing `jupyterlab_vim-0.16.0/LICENSE` & `jupyterlab_vim-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-0.16.0/PKG-INFO` & `jupyterlab_vim-0.17.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,94 +1,69 @@
-Metadata-Version: 2.1
-Name: jupyterlab_vim
-Version: 0.16.0
-Summary: Code cell vim bindings
-Home-page: https://github.com/jupyterlab-contrib/jupyterlab-vim
-Author: Jupyterlab-vim contributors
-License: MIT
-Keywords: Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # jupyterlab-vim
 
-> Community fork of <https://github.com/jwkvam/jupyterlab-vim> updated for jupyterlab 2 and 3
+> Community fork of <https://github.com/jwkvam/jupyterlab-vim> updated for jupyterlab 2, 3 and 4
 
-![Extension status](https://img.shields.io/badge/status-ready-success "ready to be used")
+![Extension status](https://img.shields.io/badge/status-ready-success 'ready to be used')
 [![Github Actions Status](https://github.com/jupyterlab-contrib/jupyterlab-vim/workflows/Build/badge.svg)](https://github.com/jupyterlab-contrib/jupyterlab-vim/actions?query=workflow%3ABuild)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyterlab-contrib/jupyterlab-vim/master?urlpath=lab)
 [![npm version](https://img.shields.io/npm/v/@axlair/jupyterlab_vim)](https://www.npmjs.com/package/@axlair/jupyterlab_vim)
 [![npm downloads](https://img.shields.io/npm/dw/@axlair/jupyterlab_vim.svg)](https://www.npmjs.com/package/@axlair/jupyterlab_vim)
 [![PyPI](https://img.shields.io/pypi/v/jupyterlab-vim)](https://pypi.org/project/jupyterlab-vim)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/jupyterlab_vim.svg)](https://anaconda.org/conda-forge/jupyterlab_vim)
 
 Notebook cell vim bindings
 
 ![jlabvim](https://user-images.githubusercontent.com/86304/38079432-b7596fd8-32f3-11e8-9ebd-4b9e7823f5f9.gif)
 
-
 ## Modes
 
 Like vim, Jupyterlab has a distinction between edit mode and command mode. Jupyterlab Command mode is when the cursor is not in a specific cell, and edit mode when typing in a cell.
 
 This extension combines the Jupyterlab (Edit and Command) modes with the standard vim modes (Normal, Insert, Visual). So the set of modes now looks like:
 
 1. Jupyterlab Command Mode
 2. Jupyterlab Edit Mode
-    - Insert
-    - Normal
-    - Visual
+   - Insert
+   - Normal
+   - Visual
 
 ## Install
 
 ```bash
 pip install jupyterlab-vim
 ```
-or  with conda/mamba:
+
+or with conda/mamba:
+
 ```bash
 mamba install -c conda-forge jupyterlab_vim
 ```
-For Jupyterlab<3 see [installing.md](installing.md).
 
+For Jupyterlab<3 see [installing.md](installing.md).
 
 ## Key Bindings
+
 To learn how to modify key bindings see the [modify-keybinds.md](modify-keybinds.md) file.
 
 **Please note that all keys are lowercase unless `Shift` is explicitly indicated.**
 For example, `Y, Y` is two lowercase `y`s, `Shift-Y, Y` is one uppercase `Y` followed by a lowercase `y`.
 
 Shortcuts this extension introduces:
 
 ### Vim Ex commands
 
 | Command  | Action                     |
-| -------  | ------                     |
+| -------- | -------------------------- |
 | :w[rite] | Save Notebook              |
 | :q[uit]  | Enter Jupyter command mode |
 
 ### Vim command bindings
 
 | Chord           | Action                    |
-| -----           | -------                   |
+| --------------- | ------------------------- |
 | Ctrl-O, U       | Undo Cell Action          |
 | -               | Split Cell at Cursor      |
 | Ctrl-O, -       | Split Cell at Cursor      |
 | Ctrl-O, D       | Cut Cell                  |
 | Ctrl-O, Y       | Copy Cell                 |
 | Ctrl-O, P       | Paste Cell                |
 | Ctrl-Shift-J    | Extend Marked Cells Below |
@@ -107,49 +82,46 @@
 | Command/Ctrl-2  | Markdown Cell Mode        |
 | Command/Ctrl-3  | Raw Cell Mode             |
 | Shift-Escape    | Leave Vim Mode            |
 | Escape, Ctrl-\[ | Exit Vim Insert Mode      |
 
 ### Jupyter command bindings
 
-| Chord   | Action            |
-| -----   | ------            |
-| G, G    | Select First Cell |
-| Shift-G | Select Last Cell  |
-| D, D    | Delete Cell       |
-| Y, Y    | Yank (Copy) Cell  |
-| P       | Paste Cell        |
-| Shift-P | Paste Cell Above  |
-| O       | Insert Cell       |
-| Shift-O | Insert Cell Above |
-| U       | Undo Cell Action  |
-| Ctrl-E  | Move Cells Down   |
-| Ctrl-Y  | Move Cells Up     |
-| Z, Z    | Center Cell       |
-| Z, C    | Hide Code Cell |
-| Z, O    | Show Code Cell |
+| Chord   | Action              |
+| ------- | ------------------- |
+| G, G    | Select First Cell   |
+| Shift-G | Select Last Cell    |
+| D, D    | Delete Cell         |
+| Y, Y    | Yank (Copy) Cell    |
+| P       | Paste Cell          |
+| Shift-P | Paste Cell Above    |
+| O       | Insert Cell         |
+| Shift-O | Insert Cell Above   |
+| U       | Undo Cell Action    |
+| Ctrl-E  | Move Cells Down     |
+| Ctrl-Y  | Move Cells Up       |
+| Z, Z    | Center Cell         |
+| Z, C    | Hide Code Cell      |
+| Z, O    | Show Code Cell      |
 | Z, M    | Hide All Code Cells |
-| Z, R    | Show All Code Cells  |
+| Z, R    | Show All Code Cells |
 
 ## Special Thanks
 
-
 From @jwkvam:
 
 > I want to acknowledge [Alisue](https://github.com/lambdalisue) and his excellent work creating [vim bindings](https://github.com/lambdalisue/jupyter-vim-binding) for Jupyter notebooks.
 > I hope this extension can meet the high bar his work set.
 
 @jkwvam is the original author of this extension - the original version can be seen [here](https://github.com/jwkvam/jupyterlab-vim). When that version was not updated it was updated first by @axelfahy and then moved to this community organization.
 
 ## Contributing
 
 Contributions and feedback are most welcome!
 
-[![](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/images/0)](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/links/0)[![](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/images/1)](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/links/1)[![](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/images/2)](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/links/2)[![](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/images/3)](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/links/3)[![](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/images/4)](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/links/4)[![](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/images/5)](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/links/5)[![](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/images/6)](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/links/6)[![](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/images/7)](https://sourcerer.io/fame/jwkvam/jwkvam/jupyterlab-vim/links/7)
-
 ### Development install
 
 Note: You will need NodeJS to build the extension package. To install with `conda` do:
 
 ```
 conda install -c conda-forge nodejs
 ```
@@ -158,15 +130,14 @@
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
 # Change directory to the jupyterlab_vim directory
 # Install package in development mode
-pip install jupyter_packaging
 pip install -e .
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Rebuild extension Typescript source after making changes
 jlpm run build
 ```
```

### Comparing `jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json` & `jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 11% similar despite different names*

```diff
@@ -7,678 +7,616 @@
 00000060: 6469 7469 6f6e 616c 5072 6f70 6572 7469  ditionalProperti
 00000070: 6573 223a 2066 616c 7365 2c0a 2020 226a  es": false,.  "j
 00000080: 7570 7974 6572 2e6c 6162 2e73 686f 7274  upyter.lab.short
 00000090: 6375 7473 223a 205b 0a20 2020 207b 0a20  cuts": [.    {. 
 000000a0: 2020 2020 2022 636f 6d6d 616e 6422 3a20       "command": 
 000000b0: 226e 6f74 6562 6f6f 6b3a 656e 7465 722d  "notebook:enter-
 000000c0: 636f 6d6d 616e 642d 6d6f 6465 222c 0a20  command-mode",. 
-000000d0: 2020 2020 2022 6b65 7973 223a 205b 0a20       "keys": [. 
-000000e0: 2020 2020 2020 2022 4573 6361 7065 220a         "Escape".
-000000f0: 2020 2020 2020 5d2c 0a20 2020 2020 2022        ],.      "
-00000100: 7365 6c65 6374 6f72 223a 2022 2e6a 702d  selector": ".jp-
-00000110: 4e6f 7465 626f 6f6b 2e6a 702d 6d6f 642d  Notebook.jp-mod-
-00000120: 6564 6974 4d6f 6465 222c 0a20 2020 2020  editMode",.     
-00000130: 2022 6469 7361 626c 6564 223a 2074 7275   "disabled": tru
-00000140: 650a 2020 2020 7d2c 0a20 2020 207b 0a20  e.    },.    {. 
-00000150: 2020 2020 2022 7365 6c65 6374 6f72 223a       "selector":
-00000160: 2022 2e6a 702d 4e6f 7465 626f 6f6b 5061   ".jp-NotebookPa
-00000170: 6e65 6c5b 6461 7461 2d6a 702d 7669 6d2d  nel[data-jp-vim-
-00000180: 6d6f 6465 3d27 7472 7565 275d 202e 6a70  mode='true'] .jp
-00000190: 2d4e 6f74 6562 6f6f 6b2e 6a70 2d6d 6f64  -Notebook.jp-mod
-000001a0: 2d65 6469 744d 6f64 6522 2c0a 2020 2020  -editMode",.    
-000001b0: 2020 226b 6579 7322 3a20 5b0a 2020 2020    "keys": [.    
-000001c0: 2020 2020 2243 7472 6c20 4f22 2c0a 2020      "Ctrl O",.  
-000001d0: 2020 2020 2020 2255 220a 2020 2020 2020        "U".      
-000001e0: 5d2c 0a20 2020 2020 2022 636f 6d6d 616e  ],.      "comman
-000001f0: 6422 3a20 226e 6f74 6562 6f6f 6b3a 756e  d": "notebook:un
-00000200: 646f 2d63 656c 6c2d 6163 7469 6f6e 220a  do-cell-action".
-00000210: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
-00000220: 2020 2022 7365 6c65 6374 6f72 223a 2022     "selector": "
-00000230: 2e6a 702d 4e6f 7465 626f 6f6b 5061 6e65  .jp-NotebookPane
-00000240: 6c5b 6461 7461 2d6a 702d 7669 6d2d 6d6f  l[data-jp-vim-mo
-00000250: 6465 3d27 7472 7565 275d 202e 6a70 2d4e  de='true'] .jp-N
-00000260: 6f74 6562 6f6f 6b50 616e 656c 5b64 6174  otebookPanel[dat
-00000270: 612d 6a70 2d76 696d 2d6d 6f64 653d 2774  a-jp-vim-mode='t
-00000280: 7275 6527 5d20 2e6a 702d 4e6f 7465 626f  rue'] .jp-Notebo
-00000290: 6f6b 2e6a 702d 6d6f 642d 6564 6974 4d6f  ok.jp-mod-editMo
-000002a0: 6465 222c 0a20 2020 2020 2022 6b65 7973  de",.      "keys
-000002b0: 223a 205b 0a20 2020 2020 2020 2022 4374  ": [.        "Ct
-000002c0: 726c 204f 222c 0a20 2020 2020 2020 2022  rl O",.        "
-000002d0: 2d22 0a20 2020 2020 205d 2c0a 2020 2020  -".      ],.    
-000002e0: 2020 2263 6f6d 6d61 6e64 223a 2022 6e6f    "command": "no
-000002f0: 7465 626f 6f6b 3a73 706c 6974 2d63 656c  tebook:split-cel
-00000300: 6c2d 6174 2d63 7572 736f 7222 0a20 2020  l-at-cursor".   
-00000310: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
-00000320: 2273 656c 6563 746f 7222 3a20 222e 6a70  "selector": ".jp
-00000330: 2d4e 6f74 6562 6f6f 6b50 616e 656c 5b64  -NotebookPanel[d
-00000340: 6174 612d 6a70 2d76 696d 2d6d 6f64 653d  ata-jp-vim-mode=
-00000350: 2774 7275 6527 5d20 2e6a 702d 4e6f 7465  'true'] .jp-Note
-00000360: 626f 6f6b 2e6a 702d 6d6f 642d 6564 6974  book.jp-mod-edit
-00000370: 4d6f 6465 222c 0a20 2020 2020 2022 6b65  Mode",.      "ke
-00000380: 7973 223a 205b 0a20 2020 2020 2020 2022  ys": [.        "
-00000390: 4374 726c 204f 222c 0a20 2020 2020 2020  Ctrl O",.       
-000003a0: 2022 4422 0a20 2020 2020 205d 2c0a 2020   "D".      ],.  
-000003b0: 2020 2020 2263 6f6d 6d61 6e64 223a 2022      "command": "
-000003c0: 7669 6d3a 6375 742d 6365 6c6c 2d61 6e64  vim:cut-cell-and
-000003d0: 2d65 6469 7422 0a20 2020 207d 2c0a 2020  -edit".    },.  
-000003e0: 2020 7b0a 2020 2020 2020 2273 656c 6563    {.      "selec
-000003f0: 746f 7222 3a20 222e 6a70 2d4e 6f74 6562  tor": ".jp-Noteb
-00000400: 6f6f 6b50 616e 656c 5b64 6174 612d 6a70  ookPanel[data-jp
-00000410: 2d76 696d 2d6d 6f64 653d 2774 7275 6527  -vim-mode='true'
-00000420: 5d20 2e6a 702d 4e6f 7465 626f 6f6b 2e6a  ] .jp-Notebook.j
-00000430: 702d 6d6f 642d 6564 6974 4d6f 6465 222c  p-mod-editMode",
-00000440: 0a20 2020 2020 2022 6b65 7973 223a 205b  .      "keys": [
-00000450: 0a20 2020 2020 2020 2022 4374 726c 204f  .        "Ctrl O
-00000460: 222c 0a20 2020 2020 2020 2022 5922 0a20  ",.        "Y". 
-00000470: 2020 2020 205d 2c0a 2020 2020 2020 2263       ],.      "c
-00000480: 6f6d 6d61 6e64 223a 2022 7669 6d3a 636f  ommand": "vim:co
-00000490: 7079 2d63 656c 6c2d 616e 642d 6564 6974  py-cell-and-edit
-000004a0: 220a 2020 2020 7d2c 0a20 2020 207b 0a20  ".    },.    {. 
-000004b0: 2020 2020 2022 7365 6c65 6374 6f72 223a       "selector":
-000004c0: 2022 2e6a 702d 4e6f 7465 626f 6f6b 5061   ".jp-NotebookPa
-000004d0: 6e65 6c5b 6461 7461 2d6a 702d 7669 6d2d  nel[data-jp-vim-
-000004e0: 6d6f 6465 3d27 7472 7565 275d 202e 6a70  mode='true'] .jp
-000004f0: 2d4e 6f74 6562 6f6f 6b2e 6a70 2d6d 6f64  -Notebook.jp-mod
-00000500: 2d65 6469 744d 6f64 6522 2c0a 2020 2020  -editMode",.    
-00000510: 2020 226b 6579 7322 3a20 5b0a 2020 2020    "keys": [.    
-00000520: 2020 2020 2243 7472 6c20 4f22 2c0a 2020      "Ctrl O",.  
-00000530: 2020 2020 2020 2250 220a 2020 2020 2020        "P".      
-00000540: 5d2c 0a20 2020 2020 2022 636f 6d6d 616e  ],.      "comman
-00000550: 6422 3a20 2276 696d 3a70 6173 7465 2d63  d": "vim:paste-c
-00000560: 656c 6c2d 616e 642d 6564 6974 220a 2020  ell-and-edit".  
-00000570: 2020 7d2c 0a20 2020 207b 0a20 2020 2020    },.    {.     
-00000580: 2022 7365 6c65 6374 6f72 223a 2022 2e6a   "selector": ".j
-00000590: 702d 4e6f 7465 626f 6f6b 5061 6e65 6c5b  p-NotebookPanel[
-000005a0: 6461 7461 2d6a 702d 7669 6d2d 6d6f 6465  data-jp-vim-mode
-000005b0: 3d27 7472 7565 275d 202e 6a70 2d4e 6f74  ='true'] .jp-Not
-000005c0: 6562 6f6f 6b2e 6a70 2d6d 6f64 2d65 6469  ebook.jp-mod-edi
-000005d0: 744d 6f64 6522 2c0a 2020 2020 2020 226b  tMode",.      "k
-000005e0: 6579 7322 3a20 5b0a 2020 2020 2020 2020  eys": [.        
-000005f0: 2243 7472 6c20 5368 6966 7420 4a22 0a20  "Ctrl Shift J". 
-00000600: 2020 2020 205d 2c0a 2020 2020 2020 2263       ],.      "c
-00000610: 6f6d 6d61 6e64 223a 2022 6e6f 7465 626f  ommand": "notebo
-00000620: 6f6b 3a65 7874 656e 642d 6d61 726b 6564  ok:extend-marked
-00000630: 2d63 656c 6c73 2d62 656c 6f77 220a 2020  -cells-below".  
-00000640: 2020 7d2c 0a20 2020 207b 0a20 2020 2020    },.    {.     
-00000650: 2022 7365 6c65 6374 6f72 223a 2022 2e6a   "selector": ".j
-00000660: 702d 4e6f 7465 626f 6f6b 5061 6e65 6c5b  p-NotebookPanel[
-00000670: 6461 7461 2d6a 702d 7669 6d2d 6d6f 6465  data-jp-vim-mode
-00000680: 3d27 7472 7565 275d 202e 6a70 2d4e 6f74  ='true'] .jp-Not
-00000690: 6562 6f6f 6b3a 666f 6375 7322 2c0a 2020  ebook:focus",.  
-000006a0: 2020 2020 226b 6579 7322 3a20 5b0a 2020      "keys": [.  
-000006b0: 2020 2020 2020 2243 7472 6c20 5368 6966        "Ctrl Shif
-000006c0: 7420 4a22 0a20 2020 2020 205d 2c0a 2020  t J".      ],.  
-000006d0: 2020 2020 2263 6f6d 6d61 6e64 223a 2022      "command": "
-000006e0: 6e6f 7465 626f 6f6b 3a65 7874 656e 642d  notebook:extend-
-000006f0: 6d61 726b 6564 2d63 656c 6c73 2d62 656c  marked-cells-bel
-00000700: 6f77 220a 2020 2020 7d2c 0a20 2020 207b  ow".    },.    {
-00000710: 0a20 2020 2020 2022 7365 6c65 6374 6f72  .      "selector
-00000720: 223a 2022 2e6a 702d 4e6f 7465 626f 6f6b  ": ".jp-Notebook
-00000730: 5061 6e65 6c5b 6461 7461 2d6a 702d 7669  Panel[data-jp-vi
-00000740: 6d2d 6d6f 6465 3d27 7472 7565 275d 202e  m-mode='true'] .
-00000750: 6a70 2d4e 6f74 6562 6f6f 6b2e 6a70 2d6d  jp-Notebook.jp-m
-00000760: 6f64 2d65 6469 744d 6f64 6522 2c0a 2020  od-editMode",.  
-00000770: 2020 2020 226b 6579 7322 3a20 5b0a 2020      "keys": [.  
-00000780: 2020 2020 2020 2243 7472 6c20 5368 6966        "Ctrl Shif
-00000790: 7420 4b22 0a20 2020 2020 205d 2c0a 2020  t K".      ],.  
-000007a0: 2020 2020 2263 6f6d 6d61 6e64 223a 2022      "command": "
-000007b0: 6e6f 7465 626f 6f6b 3a65 7874 656e 642d  notebook:extend-
-000007c0: 6d61 726b 6564 2d63 656c 6c73 2d61 626f  marked-cells-abo
-000007d0: 7665 220a 2020 2020 7d2c 0a20 2020 207b  ve".    },.    {
-000007e0: 0a20 2020 2020 2022 7365 6c65 6374 6f72  .      "selector
-000007f0: 223a 2022 2e6a 702d 4e6f 7465 626f 6f6b  ": ".jp-Notebook
-00000800: 5061 6e65 6c5b 6461 7461 2d6a 702d 7669  Panel[data-jp-vi
-00000810: 6d2d 6d6f 6465 3d27 7472 7565 275d 202e  m-mode='true'] .
-00000820: 6a70 2d4e 6f74 6562 6f6f 6b3a 666f 6375  jp-Notebook:focu
-00000830: 7322 2c0a 2020 2020 2020 226b 6579 7322  s",.      "keys"
-00000840: 3a20 5b0a 2020 2020 2020 2020 2243 7472  : [.        "Ctr
-00000850: 6c20 5368 6966 7420 4b22 0a20 2020 2020  l Shift K".     
-00000860: 205d 2c0a 2020 2020 2020 2263 6f6d 6d61   ],.      "comma
-00000870: 6e64 223a 2022 6e6f 7465 626f 6f6b 3a65  nd": "notebook:e
-00000880: 7874 656e 642d 6d61 726b 6564 2d63 656c  xtend-marked-cel
-00000890: 6c73 2d61 626f 7665 220a 2020 2020 7d2c  ls-above".    },
-000008a0: 0a20 2020 207b 0a20 2020 2020 2022 7365  .    {.      "se
-000008b0: 6c65 6374 6f72 223a 2022 2e6a 702d 4e6f  lector": ".jp-No
-000008c0: 7465 626f 6f6b 5061 6e65 6c5b 6461 7461  tebookPanel[data
-000008d0: 2d6a 702d 7669 6d2d 6d6f 6465 3d27 7472  -jp-vim-mode='tr
-000008e0: 7565 275d 202e 6a70 2d4e 6f74 6562 6f6f  ue'] .jp-Noteboo
-000008f0: 6b2e 6a70 2d6d 6f64 2d65 6469 744d 6f64  k.jp-mod-editMod
-00000900: 6522 2c0a 2020 2020 2020 226b 6579 7322  e",.      "keys"
-00000910: 3a20 5b0a 2020 2020 2020 2020 2243 7472  : [.        "Ctr
-00000920: 6c20 4f22 2c0a 2020 2020 2020 2020 2253  l O",.        "S
-00000930: 6869 6674 204f 220a 2020 2020 2020 5d2c  hift O".      ],
-00000940: 0a20 2020 2020 2022 636f 6d6d 616e 6422  .      "command"
-00000950: 3a20 226e 6f74 6562 6f6f 6b3a 696e 7365  : "notebook:inse
-00000960: 7274 2d63 656c 6c2d 6162 6f76 6522 0a20  rt-cell-above". 
-00000970: 2020 207d 2c0a 2020 2020 7b0a 2020 2020     },.    {.    
-00000980: 2020 2273 656c 6563 746f 7222 3a20 222e    "selector": ".
-00000990: 6a70 2d4e 6f74 6562 6f6f 6b50 616e 656c  jp-NotebookPanel
-000009a0: 5b64 6174 612d 6a70 2d76 696d 2d6d 6f64  [data-jp-vim-mod
-000009b0: 653d 2774 7275 6527 5d20 2e6a 702d 4e6f  e='true'] .jp-No
-000009c0: 7465 626f 6f6b 2e6a 702d 6d6f 642d 6564  tebook.jp-mod-ed
-000009d0: 6974 4d6f 6465 222c 0a20 2020 2020 2022  itMode",.      "
-000009e0: 6b65 7973 223a 205b 0a20 2020 2020 2020  keys": [.       
-000009f0: 2022 4374 726c 204f 222c 0a20 2020 2020   "Ctrl O",.     
-00000a00: 2020 2022 4374 726c 204f 220a 2020 2020     "Ctrl O".    
-00000a10: 2020 5d2c 0a20 2020 2020 2022 636f 6d6d    ],.      "comm
-00000a20: 616e 6422 3a20 226e 6f74 6562 6f6f 6b3a  and": "notebook:
-00000a30: 696e 7365 7274 2d63 656c 6c2d 6162 6f76  insert-cell-abov
-00000a40: 6522 0a20 2020 207d 2c0a 2020 2020 7b0a  e".    },.    {.
-00000a50: 2020 2020 2020 2273 656c 6563 746f 7222        "selector"
-00000a60: 3a20 222e 6a70 2d4e 6f74 6562 6f6f 6b50  : ".jp-NotebookP
-00000a70: 616e 656c 5b64 6174 612d 6a70 2d76 696d  anel[data-jp-vim
-00000a80: 2d6d 6f64 653d 2774 7275 6527 5d20 2e6a  -mode='true'] .j
-00000a90: 702d 4e6f 7465 626f 6f6b 2e6a 702d 6d6f  p-Notebook.jp-mo
-00000aa0: 642d 6564 6974 4d6f 6465 222c 0a20 2020  d-editMode",.   
-00000ab0: 2020 2022 6b65 7973 223a 205b 0a20 2020     "keys": [.   
-00000ac0: 2020 2020 2022 4374 726c 204f 222c 0a20       "Ctrl O",. 
-00000ad0: 2020 2020 2020 2022 4f22 0a20 2020 2020         "O".     
-00000ae0: 205d 2c0a 2020 2020 2020 2263 6f6d 6d61   ],.      "comma
-00000af0: 6e64 223a 2022 6e6f 7465 626f 6f6b 3a69  nd": "notebook:i
-00000b00: 6e73 6572 742d 6365 6c6c 2d62 656c 6f77  nsert-cell-below
-00000b10: 220a 2020 2020 7d2c 0a20 2020 207b 0a20  ".    },.    {. 
-00000b20: 2020 2020 2022 7365 6c65 6374 6f72 223a       "selector":
-00000b30: 2022 2e6a 702d 4e6f 7465 626f 6f6b 5061   ".jp-NotebookPa
-00000b40: 6e65 6c5b 6461 7461 2d6a 702d 7669 6d2d  nel[data-jp-vim-
-00000b50: 6d6f 6465 3d27 7472 7565 275d 202e 6a70  mode='true'] .jp
-00000b60: 2d4e 6f74 6562 6f6f 6b2e 6a70 2d6d 6f64  -Notebook.jp-mod
-00000b70: 2d65 6469 744d 6f64 6522 2c0a 2020 2020  -editMode",.    
-00000b80: 2020 226b 6579 7322 3a20 5b0a 2020 2020    "keys": [.    
-00000b90: 2020 2020 2243 7472 6c20 4a22 0a20 2020      "Ctrl J".   
-00000ba0: 2020 205d 2c0a 2020 2020 2020 2263 6f6d     ],.      "com
-00000bb0: 6d61 6e64 223a 2022 7669 6d3a 7365 6c65  mand": "vim:sele
-00000bc0: 6374 2d62 656c 6f77 2d65 7865 6375 7465  ct-below-execute
-00000bd0: 2d6d 6172 6b64 6f77 6e22 0a20 2020 207d  -markdown".    }
-00000be0: 2c0a 2020 2020 7b0a 2020 2020 2020 2273  ,.    {.      "s
-00000bf0: 656c 6563 746f 7222 3a20 222e 6a70 2d4e  elector": ".jp-N
-00000c00: 6f74 6562 6f6f 6b50 616e 656c 5b64 6174  otebookPanel[dat
-00000c10: 612d 6a70 2d76 696d 2d6d 6f64 653d 2774  a-jp-vim-mode='t
-00000c20: 7275 6527 5d20 2e6a 702d 4e6f 7465 626f  rue'] .jp-Notebo
-00000c30: 6f6b 2e6a 702d 6d6f 642d 6564 6974 4d6f  ok.jp-mod-editMo
-00000c40: 6465 222c 0a20 2020 2020 2022 6b65 7973  de",.      "keys
-00000c50: 223a 205b 0a20 2020 2020 2020 2022 4374  ": [.        "Ct
-00000c60: 726c 204b 220a 2020 2020 2020 5d2c 0a20  rl K".      ],. 
-00000c70: 2020 2020 2022 636f 6d6d 616e 6422 3a20       "command": 
-00000c80: 2276 696d 3a73 656c 6563 742d 6162 6f76  "vim:select-abov
-00000c90: 652d 6578 6563 7574 652d 6d61 726b 646f  e-execute-markdo
-00000ca0: 776e 220a 2020 2020 7d2c 0a20 2020 207b  wn".    },.    {
-00000cb0: 0a20 2020 2020 2022 7365 6c65 6374 6f72  .      "selector
-00000cc0: 223a 2022 2e6a 702d 4e6f 7465 626f 6f6b  ": ".jp-Notebook
-00000cd0: 5061 6e65 6c5b 6461 7461 2d6a 702d 7669  Panel[data-jp-vi
-00000ce0: 6d2d 6d6f 6465 3d27 7472 7565 275d 202e  m-mode='true'] .
-00000cf0: 6a70 2d4e 6f74 6562 6f6f 6b2e 6a70 2d6d  jp-Notebook.jp-m
-00000d00: 6f64 2d65 6469 744d 6f64 6522 2c0a 2020  od-editMode",.  
-00000d10: 2020 2020 226b 6579 7322 3a20 5b0a 2020      "keys": [.  
-00000d20: 2020 2020 2020 2245 7363 6170 6522 0a20        "Escape". 
-00000d30: 2020 2020 205d 2c0a 2020 2020 2020 2263       ],.      "c
-00000d40: 6f6d 6d61 6e64 223a 2022 7669 6d3a 6c65  ommand": "vim:le
-00000d50: 6176 652d 696e 7365 7274 2d6d 6f64 6522  ave-insert-mode"
-00000d60: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
-00000d70: 2020 2020 2273 656c 6563 746f 7222 3a20      "selector": 
-00000d80: 222e 6a70 2d4e 6f74 6562 6f6f 6b50 616e  ".jp-NotebookPan
-00000d90: 656c 5b64 6174 612d 6a70 2d76 696d 2d6d  el[data-jp-vim-m
-00000da0: 6f64 653d 2774 7275 6527 5d20 2e6a 702d  ode='true'] .jp-
-00000db0: 4e6f 7465 626f 6f6b 2e6a 702d 6d6f 642d  Notebook.jp-mod-
-00000dc0: 6564 6974 4d6f 6465 222c 0a20 2020 2020  editMode",.     
-00000dd0: 2022 6b65 7973 223a 205b 0a20 2020 2020   "keys": [.     
-00000de0: 2020 2022 4374 726c 205b 220a 2020 2020     "Ctrl [".    
-00000df0: 2020 5d2c 0a20 2020 2020 2022 636f 6d6d    ],.      "comm
-00000e00: 616e 6422 3a20 2276 696d 3a6c 6561 7665  and": "vim:leave
-00000e10: 2d69 6e73 6572 742d 6d6f 6465 220a 2020  -insert-mode".  
-00000e20: 2020 7d2c 0a20 2020 207b 0a20 2020 2020    },.    {.     
-00000e30: 2022 7365 6c65 6374 6f72 223a 2022 2e6a   "selector": ".j
-00000e40: 702d 4e6f 7465 626f 6f6b 5061 6e65 6c5b  p-NotebookPanel[
-00000e50: 6461 7461 2d6a 702d 7669 6d2d 6d6f 6465  data-jp-vim-mode
-00000e60: 3d27 7472 7565 275d 202e 6a70 2d4e 6f74  ='true'] .jp-Not
-00000e70: 6562 6f6f 6b3a 666f 6375 7322 2c0a 2020  ebook:focus",.  
-00000e80: 2020 2020 226b 6579 7322 3a20 5b0a 2020      "keys": [.  
-00000e90: 2020 2020 2020 2243 7472 6c20 4922 0a20        "Ctrl I". 
-00000ea0: 2020 2020 205d 2c0a 2020 2020 2020 2263       ],.      "c
-00000eb0: 6f6d 6d61 6e64 223a 2022 7669 6d3a 656e  ommand": "vim:en
-00000ec0: 7465 722d 696e 7365 7274 2d6d 6f64 6522  ter-insert-mode"
-00000ed0: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
-00000ee0: 2020 2020 2273 656c 6563 746f 7222 3a20      "selector": 
-00000ef0: 222e 6a70 2d4e 6f74 6562 6f6f 6b50 616e  ".jp-NotebookPan
-00000f00: 656c 5b64 6174 612d 6a70 2d76 696d 2d6d  el[data-jp-vim-m
-00000f10: 6f64 653d 2774 7275 6527 5d20 2e6a 702d  ode='true'] .jp-
-00000f20: 4e6f 7465 626f 6f6b 2e6a 702d 6d6f 642d  Notebook.jp-mod-
-00000f30: 6564 6974 4d6f 6465 222c 0a20 2020 2020  editMode",.     
-00000f40: 2022 6b65 7973 223a 205b 0a20 2020 2020   "keys": [.     
-00000f50: 2020 2022 4374 726c 2045 6e74 6572 220a     "Ctrl Enter".
-00000f60: 2020 2020 2020 5d2c 0a20 2020 2020 2022        ],.      "
-00000f70: 636f 6d6d 616e 6422 3a20 2276 696d 3a72  command": "vim:r
-00000f80: 756e 2d63 656c 6c2d 616e 642d 6564 6974  un-cell-and-edit
-00000f90: 220a 2020 2020 7d2c 0a20 2020 207b 0a20  ".    },.    {. 
-00000fa0: 2020 2020 2022 7365 6c65 6374 6f72 223a       "selector":
-00000fb0: 2022 2e6a 702d 4e6f 7465 626f 6f6b 5061   ".jp-NotebookPa
-00000fc0: 6e65 6c5b 6461 7461 2d6a 702d 7669 6d2d  nel[data-jp-vim-
-00000fd0: 6d6f 6465 3d27 7472 7565 275d 202e 6a70  mode='true'] .jp
-00000fe0: 2d4e 6f74 6562 6f6f 6b2e 6a70 2d6d 6f64  -Notebook.jp-mod
-00000ff0: 2d65 6469 744d 6f64 6522 2c0a 2020 2020  -editMode",.    
-00001000: 2020 226b 6579 7322 3a20 5b0a 2020 2020    "keys": [.    
-00001010: 2020 2020 2253 6869 6674 2045 6e74 6572      "Shift Enter
-00001020: 220a 2020 2020 2020 5d2c 0a20 2020 2020  ".      ],.     
-00001030: 2022 636f 6d6d 616e 6422 3a20 2276 696d   "command": "vim
-00001040: 3a72 756e 2d73 656c 6563 742d 6e65 7874  :run-select-next
-00001050: 2d65 6469 7422 0a20 2020 207d 2c0a 2020  -edit".    },.  
-00001060: 2020 7b0a 2020 2020 2020 2273 656c 6563    {.      "selec
-00001070: 746f 7222 3a20 222e 6a70 2d4e 6f74 6562  tor": ".jp-Noteb
-00001080: 6f6f 6b50 616e 656c 5b64 6174 612d 6a70  ookPanel[data-jp
-00001090: 2d76 696d 2d6d 6f64 653d 2774 7275 6527  -vim-mode='true'
-000010a0: 5d20 2e6a 702d 4e6f 7465 626f 6f6b 2e6a  ] .jp-Notebook.j
-000010b0: 702d 6d6f 642d 6564 6974 4d6f 6465 222c  p-mod-editMode",
-000010c0: 0a20 2020 2020 2022 6b65 7973 223a 205b  .      "keys": [
-000010d0: 0a20 2020 2020 2020 2022 5368 6966 7420  .        "Shift 
-000010e0: 4573 6361 7065 220a 2020 2020 2020 5d2c  Escape".      ],
-000010f0: 0a20 2020 2020 2022 636f 6d6d 616e 6422  .      "command"
-00001100: 3a20 226e 6f74 6562 6f6f 6b3a 656e 7465  : "notebook:ente
-00001110: 722d 636f 6d6d 616e 642d 6d6f 6465 220a  r-command-mode".
-00001120: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
-00001130: 2020 2022 7365 6c65 6374 6f72 223a 2022     "selector": "
-00001140: 2e6a 702d 4e6f 7465 626f 6f6b 5061 6e65  .jp-NotebookPane
-00001150: 6c5b 6461 7461 2d6a 702d 7669 6d2d 6d6f  l[data-jp-vim-mo
-00001160: 6465 3d27 7472 7565 275d 202e 6a70 2d4e  de='true'] .jp-N
-00001170: 6f74 6562 6f6f 6b3a 666f 6375 7322 2c0a  otebook:focus",.
-00001180: 2020 2020 2020 226b 6579 7322 3a20 5b0a        "keys": [.
-00001190: 2020 2020 2020 2020 2253 6869 6674 204d          "Shift M
-000011a0: 220a 2020 2020 2020 5d2c 0a20 2020 2020  ".      ],.     
-000011b0: 2022 636f 6d6d 616e 6422 3a20 2276 696d   "command": "vim
-000011c0: 3a6d 6572 6765 2d61 6e64 2d65 6469 7422  :merge-and-edit"
-000011d0: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
-000011e0: 2020 2020 2273 656c 6563 746f 7222 3a20      "selector": 
-000011f0: 222e 6a70 2d4e 6f74 6562 6f6f 6b50 616e  ".jp-NotebookPan
-00001200: 656c 5b64 6174 612d 6a70 2d76 696d 2d6d  el[data-jp-vim-m
-00001210: 6f64 653d 2774 7275 6527 5d20 2e6a 702d  ode='true'] .jp-
-00001220: 4e6f 7465 626f 6f6b 2e6a 702d 6d6f 642d  Notebook.jp-mod-
-00001230: 6564 6974 4d6f 6465 222c 0a20 2020 2020  editMode",.     
-00001240: 2022 6b65 7973 223a 205b 0a20 2020 2020   "keys": [.     
-00001250: 2020 2022 4163 6365 6c20 3122 0a20 2020     "Accel 1".   
-00001260: 2020 205d 2c0a 2020 2020 2020 2263 6f6d     ],.      "com
-00001270: 6d61 6e64 223a 2022 6e6f 7465 626f 6f6b  mand": "notebook
-00001280: 3a63 6861 6e67 652d 6365 6c6c 2d74 6f2d  :change-cell-to-
-00001290: 636f 6465 220a 2020 2020 7d2c 0a20 2020  code".    },.   
-000012a0: 207b 0a20 2020 2020 2022 7365 6c65 6374   {.      "select
-000012b0: 6f72 223a 2022 2e6a 702d 4e6f 7465 626f  or": ".jp-Notebo
-000012c0: 6f6b 5061 6e65 6c5b 6461 7461 2d6a 702d  okPanel[data-jp-
-000012d0: 7669 6d2d 6d6f 6465 3d27 7472 7565 275d  vim-mode='true']
-000012e0: 202e 6a70 2d4e 6f74 6562 6f6f 6b2e 6a70   .jp-Notebook.jp
-000012f0: 2d6d 6f64 2d65 6469 744d 6f64 6522 2c0a  -mod-editMode",.
-00001300: 2020 2020 2020 226b 6579 7322 3a20 5b0a        "keys": [.
-00001310: 2020 2020 2020 2020 2241 6363 656c 2032          "Accel 2
-00001320: 220a 2020 2020 2020 5d2c 0a20 2020 2020  ".      ],.     
-00001330: 2022 636f 6d6d 616e 6422 3a20 226e 6f74   "command": "not
-00001340: 6562 6f6f 6b3a 6368 616e 6765 2d63 656c  ebook:change-cel
-00001350: 6c2d 746f 2d6d 6172 6b64 6f77 6e22 0a20  l-to-markdown". 
-00001360: 2020 207d 2c0a 2020 2020 7b0a 2020 2020     },.    {.    
-00001370: 2020 2273 656c 6563 746f 7222 3a20 222e    "selector": ".
-00001380: 6a70 2d4e 6f74 6562 6f6f 6b50 616e 656c  jp-NotebookPanel
-00001390: 5b64 6174 612d 6a70 2d76 696d 2d6d 6f64  [data-jp-vim-mod
-000013a0: 653d 2774 7275 6527 5d20 2e6a 702d 4e6f  e='true'] .jp-No
-000013b0: 7465 626f 6f6b 2e6a 702d 6d6f 642d 6564  tebook.jp-mod-ed
-000013c0: 6974 4d6f 6465 222c 0a20 2020 2020 2022  itMode",.      "
-000013d0: 6b65 7973 223a 205b 0a20 2020 2020 2020  keys": [.       
-000013e0: 2022 4163 6365 6c20 3322 0a20 2020 2020   "Accel 3".     
-000013f0: 205d 2c0a 2020 2020 2020 2263 6f6d 6d61   ],.      "comma
-00001400: 6e64 223a 2022 6e6f 7465 626f 6f6b 3a63  nd": "notebook:c
-00001410: 6861 6e67 652d 6365 6c6c 2d74 6f2d 7261  hange-cell-to-ra
-00001420: 7722 0a20 2020 207d 2c0a 2020 2020 7b0a  w".    },.    {.
-00001430: 2020 2020 2020 2273 656c 6563 746f 7222        "selector"
-00001440: 3a20 222e 6a70 2d4e 6f74 6562 6f6f 6b50  : ".jp-NotebookP
-00001450: 616e 656c 5b64 6174 612d 6a70 2d76 696d  anel[data-jp-vim
-00001460: 2d6d 6f64 653d 2774 7275 6527 5d20 2e6a  -mode='true'] .j
-00001470: 702d 4e6f 7465 626f 6f6b 2e6a 702d 6d6f  p-Notebook.jp-mo
-00001480: 642d 6564 6974 4d6f 6465 222c 0a20 2020  d-editMode",.   
-00001490: 2020 2022 6b65 7973 223a 205b 0a20 2020     "keys": [.   
-000014a0: 2020 2020 2022 4374 726c 204f 222c 0a20       "Ctrl O",. 
-000014b0: 2020 2020 2020 2022 4722 0a20 2020 2020         "G".     
-000014c0: 205d 2c0a 2020 2020 2020 2263 6f6d 6d61   ],.      "comma
-000014d0: 6e64 223a 2022 7669 6d3a 7365 6c65 6374  nd": "vim:select
-000014e0: 2d66 6972 7374 2d63 656c 6c22 0a20 2020  -first-cell".   
-000014f0: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
-00001500: 2273 656c 6563 746f 7222 3a20 222e 6a70  "selector": ".jp
-00001510: 2d4e 6f74 6562 6f6f 6b50 616e 656c 5b64  -NotebookPanel[d
-00001520: 6174 612d 6a70 2d76 696d 2d6d 6f64 653d  ata-jp-vim-mode=
-00001530: 2774 7275 6527 5d20 2e6a 702d 4e6f 7465  'true'] .jp-Note
-00001540: 626f 6f6b 2e6a 702d 6d6f 642d 6564 6974  book.jp-mod-edit
-00001550: 4d6f 6465 222c 0a20 2020 2020 2022 6b65  Mode",.      "ke
-00001560: 7973 223a 205b 0a20 2020 2020 2020 2022  ys": [.        "
-00001570: 4374 726c 204f 222c 0a20 2020 2020 2020  Ctrl O",.       
-00001580: 2022 4374 726c 2047 220a 2020 2020 2020   "Ctrl G".      
-00001590: 5d2c 0a20 2020 2020 2022 636f 6d6d 616e  ],.      "comman
-000015a0: 6422 3a20 2276 696d 3a73 656c 6563 742d  d": "vim:select-
-000015b0: 6c61 7374 2d63 656c 6c22 0a20 2020 207d  last-cell".    }
-000015c0: 2c0a 2020 2020 7b0a 2020 2020 2020 2273  ,.    {.      "s
-000015d0: 656c 6563 746f 7222 3a20 222e 6a70 2d4e  elector": ".jp-N
-000015e0: 6f74 6562 6f6f 6b50 616e 656c 5b64 6174  otebookPanel[dat
-000015f0: 612d 6a70 2d76 696d 2d6d 6f64 653d 2774  a-jp-vim-mode='t
-00001600: 7275 6527 5d20 2e6a 702d 4e6f 7465 626f  rue'] .jp-Notebo
-00001610: 6f6b 3a66 6f63 7573 222c 0a20 2020 2020  ok:focus",.     
-00001620: 2022 6b65 7973 223a 205b 0a20 2020 2020   "keys": [.     
-00001630: 2020 2022 4722 2c0a 2020 2020 2020 2020     "G",.        
-00001640: 2247 220a 2020 2020 2020 5d2c 0a20 2020  "G".      ],.   
-00001650: 2020 2022 636f 6d6d 616e 6422 3a20 2276     "command": "v
-00001660: 696d 3a73 656c 6563 742d 6669 7273 742d  im:select-first-
-00001670: 6365 6c6c 220a 2020 2020 7d2c 0a20 2020  cell".    },.   
-00001680: 207b 0a20 2020 2020 2022 7365 6c65 6374   {.      "select
-00001690: 6f72 223a 2022 2e6a 702d 4e6f 7465 626f  or": ".jp-Notebo
-000016a0: 6f6b 5061 6e65 6c5b 6461 7461 2d6a 702d  okPanel[data-jp-
-000016b0: 7669 6d2d 6d6f 6465 3d27 7472 7565 275d  vim-mode='true']
-000016c0: 202e 6a70 2d4e 6f74 6562 6f6f 6b3a 666f   .jp-Notebook:fo
-000016d0: 6375 7322 2c0a 2020 2020 2020 226b 6579  cus",.      "key
-000016e0: 7322 3a20 5b0a 2020 2020 2020 2020 2253  s": [.        "S
-000016f0: 6869 6674 2047 220a 2020 2020 2020 5d2c  hift G".      ],
-00001700: 0a20 2020 2020 2022 636f 6d6d 616e 6422  .      "command"
-00001710: 3a20 2276 696d 3a73 656c 6563 742d 6c61  : "vim:select-la
-00001720: 7374 2d63 656c 6c22 0a20 2020 207d 2c0a  st-cell".    },.
-00001730: 2020 2020 7b0a 2020 2020 2020 2273 656c      {.      "sel
-00001740: 6563 746f 7222 3a20 222e 6a70 2d4e 6f74  ector": ".jp-Not
-00001750: 6562 6f6f 6b50 616e 656c 5b64 6174 612d  ebookPanel[data-
-00001760: 6a70 2d76 696d 2d6d 6f64 653d 2774 7275  jp-vim-mode='tru
-00001770: 6527 5d20 2e6a 702d 4e6f 7465 626f 6f6b  e'] .jp-Notebook
-00001780: 3a66 6f63 7573 222c 0a20 2020 2020 2022  :focus",.      "
-00001790: 6b65 7973 223a 205b 0a20 2020 2020 2020  keys": [.       
-000017a0: 2022 5922 2c0a 2020 2020 2020 2020 2259   "Y",.        "Y
-000017b0: 220a 2020 2020 2020 5d2c 0a20 2020 2020  ".      ],.     
-000017c0: 2022 636f 6d6d 616e 6422 3a20 226e 6f74   "command": "not
-000017d0: 6562 6f6f 6b3a 636f 7079 2d63 656c 6c22  ebook:copy-cell"
-000017e0: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
-000017f0: 2020 2020 2263 6f6d 6d61 6e64 223a 2022      "command": "
-00001800: 6e6f 7465 626f 6f6b 3a63 7574 2d63 656c  notebook:cut-cel
-00001810: 6c22 2c0a 2020 2020 2020 226b 6579 7322  l",.      "keys"
-00001820: 3a20 5b0a 2020 2020 2020 2020 2244 222c  : [.        "D",
-00001830: 0a20 2020 2020 2020 2022 4422 0a20 2020  .        "D".   
-00001840: 2020 205d 2c0a 2020 2020 2020 2273 656c     ],.      "sel
-00001850: 6563 746f 7222 3a20 222e 6a70 2d4e 6f74  ector": ".jp-Not
-00001860: 6562 6f6f 6b50 616e 656c 5b64 6174 612d  ebookPanel[data-
-00001870: 6a70 2d76 696d 2d6d 6f64 653d 2774 7275  jp-vim-mode='tru
-00001880: 6527 5d20 2e6a 702d 4e6f 7465 626f 6f6b  e'] .jp-Notebook
-00001890: 3a66 6f63 7573 220a 2020 2020 7d2c 0a20  :focus".    },. 
-000018a0: 2020 207b 0a20 2020 2020 2022 7365 6c65     {.      "sele
-000018b0: 6374 6f72 223a 2022 2e6a 702d 4e6f 7465  ctor": ".jp-Note
-000018c0: 626f 6f6b 5061 6e65 6c5b 6461 7461 2d6a  bookPanel[data-j
-000018d0: 702d 7669 6d2d 6d6f 6465 3d27 7472 7565  p-vim-mode='true
-000018e0: 275d 202e 6a70 2d4e 6f74 6562 6f6f 6b3a  '] .jp-Notebook:
-000018f0: 666f 6375 7322 2c0a 2020 2020 2020 226b  focus",.      "k
-00001900: 6579 7322 3a20 5b0a 2020 2020 2020 2020  eys": [.        
-00001910: 2253 6869 6674 2050 220a 2020 2020 2020  "Shift P".      
-00001920: 5d2c 0a20 2020 2020 2022 636f 6d6d 616e  ],.      "comman
-00001930: 6422 3a20 226e 6f74 6562 6f6f 6b3a 7061  d": "notebook:pa
-00001940: 7374 652d 6365 6c6c 2d61 626f 7665 220a  ste-cell-above".
-00001950: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
-00001960: 2020 2022 7365 6c65 6374 6f72 223a 2022     "selector": "
-00001970: 2e6a 702d 4e6f 7465 626f 6f6b 5061 6e65  .jp-NotebookPane
-00001980: 6c5b 6461 7461 2d6a 702d 7669 6d2d 6d6f  l[data-jp-vim-mo
-00001990: 6465 3d27 7472 7565 275d 202e 6a70 2d4e  de='true'] .jp-N
-000019a0: 6f74 6562 6f6f 6b3a 666f 6375 7322 2c0a  otebook:focus",.
-000019b0: 2020 2020 2020 226b 6579 7322 3a20 5b0a        "keys": [.
-000019c0: 2020 2020 2020 2020 2250 220a 2020 2020          "P".    
-000019d0: 2020 5d2c 0a20 2020 2020 2022 636f 6d6d    ],.      "comm
-000019e0: 616e 6422 3a20 226e 6f74 6562 6f6f 6b3a  and": "notebook:
-000019f0: 7061 7374 652d 6365 6c6c 2d62 656c 6f77  paste-cell-below
-00001a00: 220a 2020 2020 7d2c 0a20 2020 207b 0a20  ".    },.    {. 
-00001a10: 2020 2020 2022 7365 6c65 6374 6f72 223a       "selector":
-00001a20: 2022 2e6a 702d 4e6f 7465 626f 6f6b 5061   ".jp-NotebookPa
-00001a30: 6e65 6c5b 6461 7461 2d6a 702d 7669 6d2d  nel[data-jp-vim-
-00001a40: 6d6f 6465 3d27 7472 7565 275d 202e 6a70  mode='true'] .jp
-00001a50: 2d4e 6f74 6562 6f6f 6b3a 666f 6375 7322  -Notebook:focus"
-00001a60: 2c0a 2020 2020 2020 226b 6579 7322 3a20  ,.      "keys": 
-00001a70: 5b0a 2020 2020 2020 2020 224f 220a 2020  [.        "O".  
-00001a80: 2020 2020 5d2c 0a20 2020 2020 2022 636f      ],.      "co
-00001a90: 6d6d 616e 6422 3a20 226e 6f74 6562 6f6f  mmand": "noteboo
-00001aa0: 6b3a 696e 7365 7274 2d63 656c 6c2d 6265  k:insert-cell-be
-00001ab0: 6c6f 7722 0a20 2020 207d 2c0a 2020 2020  low".    },.    
-00001ac0: 7b0a 2020 2020 2020 2273 656c 6563 746f  {.      "selecto
-00001ad0: 7222 3a20 222e 6a70 2d4e 6f74 6562 6f6f  r": ".jp-Noteboo
-00001ae0: 6b50 616e 656c 5b64 6174 612d 6a70 2d76  kPanel[data-jp-v
-00001af0: 696d 2d6d 6f64 653d 2774 7275 6527 5d20  im-mode='true'] 
-00001b00: 2e6a 702d 4e6f 7465 626f 6f6b 3a66 6f63  .jp-Notebook:foc
-00001b10: 7573 222c 0a20 2020 2020 2022 6b65 7973  us",.      "keys
-00001b20: 223a 205b 0a20 2020 2020 2020 2022 5368  ": [.        "Sh
-00001b30: 6966 7420 4f22 0a20 2020 2020 205d 2c0a  ift O".      ],.
-00001b40: 2020 2020 2020 2263 6f6d 6d61 6e64 223a        "command":
-00001b50: 2022 6e6f 7465 626f 6f6b 3a69 6e73 6572   "notebook:inser
-00001b60: 742d 6365 6c6c 2d61 626f 7665 220a 2020  t-cell-above".  
-00001b70: 2020 7d2c 0a20 2020 207b 0a20 2020 2020    },.    {.     
-00001b80: 2022 7365 6c65 6374 6f72 223a 2022 2e6a   "selector": ".j
-00001b90: 702d 4e6f 7465 626f 6f6b 5061 6e65 6c5b  p-NotebookPanel[
-00001ba0: 6461 7461 2d6a 702d 7669 6d2d 6d6f 6465  data-jp-vim-mode
-00001bb0: 3d27 7472 7565 275d 202e 6a70 2d4e 6f74  ='true'] .jp-Not
-00001bc0: 6562 6f6f 6b3a 666f 6375 7322 2c0a 2020  ebook:focus",.  
-00001bd0: 2020 2020 226b 6579 7322 3a20 5b0a 2020      "keys": [.  
-00001be0: 2020 2020 2020 2255 220a 2020 2020 2020        "U".      
-00001bf0: 5d2c 0a20 2020 2020 2022 636f 6d6d 616e  ],.      "comman
-00001c00: 6422 3a20 226e 6f74 6562 6f6f 6b3a 756e  d": "notebook:un
-00001c10: 646f 2d63 656c 6c2d 6163 7469 6f6e 220a  do-cell-action".
-00001c20: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
-00001c30: 2020 2022 7365 6c65 6374 6f72 223a 2022     "selector": "
-00001c40: 2e6a 702d 4e6f 7465 626f 6f6b 5061 6e65  .jp-NotebookPane
-00001c50: 6c5b 6461 7461 2d6a 702d 7669 6d2d 6d6f  l[data-jp-vim-mo
-00001c60: 6465 3d27 7472 7565 275d 202e 6a70 2d4e  de='true'] .jp-N
-00001c70: 6f74 6562 6f6f 6b3a 666f 6375 7322 2c0a  otebook:focus",.
-00001c80: 2020 2020 2020 226b 6579 7322 3a20 5b0a        "keys": [.
-00001c90: 2020 2020 2020 2020 2243 7472 6c20 4522          "Ctrl E"
-00001ca0: 0a20 2020 2020 205d 2c0a 2020 2020 2020  .      ],.      
-00001cb0: 2263 6f6d 6d61 6e64 223a 2022 6e6f 7465  "command": "note
-00001cc0: 626f 6f6b 3a6d 6f76 652d 6365 6c6c 2d64  book:move-cell-d
-00001cd0: 6f77 6e22 0a20 2020 207d 2c0a 2020 2020  own".    },.    
-00001ce0: 7b0a 2020 2020 2020 2273 656c 6563 746f  {.      "selecto
-00001cf0: 7222 3a20 222e 6a70 2d4e 6f74 6562 6f6f  r": ".jp-Noteboo
-00001d00: 6b50 616e 656c 5b64 6174 612d 6a70 2d76  kPanel[data-jp-v
-00001d10: 696d 2d6d 6f64 653d 2774 7275 6527 5d20  im-mode='true'] 
-00001d20: 2e6a 702d 4e6f 7465 626f 6f6b 3a66 6f63  .jp-Notebook:foc
-00001d30: 7573 222c 0a20 2020 2020 2022 6b65 7973  us",.      "keys
-00001d40: 223a 205b 0a20 2020 2020 2020 2022 4374  ": [.        "Ct
-00001d50: 726c 2059 220a 2020 2020 2020 5d2c 0a20  rl Y".      ],. 
-00001d60: 2020 2020 2022 636f 6d6d 616e 6422 3a20       "command": 
-00001d70: 226e 6f74 6562 6f6f 6b3a 6d6f 7665 2d63  "notebook:move-c
-00001d80: 656c 6c2d 7570 220a 2020 2020 7d2c 0a20  ell-up".    },. 
-00001d90: 2020 207b 0a20 2020 2020 2022 7365 6c65     {.      "sele
-00001da0: 6374 6f72 223a 2022 2e6a 702d 4e6f 7465  ctor": ".jp-Note
-00001db0: 626f 6f6b 5061 6e65 6c5b 6461 7461 2d6a  bookPanel[data-j
-00001dc0: 702d 7669 6d2d 6d6f 6465 3d27 7472 7565  p-vim-mode='true
-00001dd0: 275d 202e 6a70 2d4e 6f74 6562 6f6f 6b3a  '] .jp-Notebook:
-00001de0: 666f 6375 7322 2c0a 2020 2020 2020 226b  focus",.      "k
-00001df0: 6579 7322 3a20 5b0a 2020 2020 2020 2020  eys": [.        
-00001e00: 225a 222c 0a20 2020 2020 2020 2022 5a22  "Z",.        "Z"
-00001e10: 0a20 2020 2020 205d 2c0a 2020 2020 2020  .      ],.      
-00001e20: 2263 6f6d 6d61 6e64 223a 2022 7669 6d3a  "command": "vim:
-00001e30: 6365 6e74 6572 2d63 656c 6c22 0a20 2020  center-cell".   
-00001e40: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
-00001e50: 2273 656c 6563 746f 7222 3a20 222e 6a70  "selector": ".jp
-00001e60: 2d4e 6f74 6562 6f6f 6b50 616e 656c 5b64  -NotebookPanel[d
-00001e70: 6174 612d 6a70 2d76 696d 2d6d 6f64 653d  ata-jp-vim-mode=
-00001e80: 2774 7275 6527 5d20 2e6a 702d 4e6f 7465  'true'] .jp-Note
-00001e90: 626f 6f6b 3a66 6f63 7573 222c 0a20 2020  book:focus",.   
-00001ea0: 2020 2022 6b65 7973 223a 205b 0a20 2020     "keys": [.   
-00001eb0: 2020 2020 2022 5a22 2c0a 2020 2020 2020       "Z",.      
-00001ec0: 2020 2243 220a 2020 2020 2020 5d2c 0a20    "C".      ],. 
-00001ed0: 2020 2020 2022 636f 6d6d 616e 6422 3a20       "command": 
-00001ee0: 226e 6f74 6562 6f6f 6b3a 6869 6465 2d63  "notebook:hide-c
-00001ef0: 656c 6c2d 636f 6465 220a 2020 2020 7d2c  ell-code".    },
-00001f00: 0a20 2020 207b 0a20 2020 2020 2022 7365  .    {.      "se
-00001f10: 6c65 6374 6f72 223a 2022 2e6a 702d 4e6f  lector": ".jp-No
-00001f20: 7465 626f 6f6b 5061 6e65 6c5b 6461 7461  tebookPanel[data
-00001f30: 2d6a 702d 7669 6d2d 6d6f 6465 3d27 7472  -jp-vim-mode='tr
-00001f40: 7565 275d 202e 6a70 2d4e 6f74 6562 6f6f  ue'] .jp-Noteboo
-00001f50: 6b3a 666f 6375 7322 2c0a 2020 2020 2020  k:focus",.      
-00001f60: 226b 6579 7322 3a20 5b0a 2020 2020 2020  "keys": [.      
-00001f70: 2020 225a 222c 0a20 2020 2020 2020 2022    "Z",.        "
-00001f80: 4f22 0a20 2020 2020 205d 2c0a 2020 2020  O".      ],.    
-00001f90: 2020 2263 6f6d 6d61 6e64 223a 2022 6e6f    "command": "no
-00001fa0: 7465 626f 6f6b 3a73 686f 772d 6365 6c6c  tebook:show-cell
-00001fb0: 2d63 6f64 6522 0a20 2020 207d 2c0a 2020  -code".    },.  
-00001fc0: 2020 7b0a 2020 2020 2020 2273 656c 6563    {.      "selec
-00001fd0: 746f 7222 3a20 222e 6a70 2d4e 6f74 6562  tor": ".jp-Noteb
-00001fe0: 6f6f 6b50 616e 656c 5b64 6174 612d 6a70  ookPanel[data-jp
-00001ff0: 2d76 696d 2d6d 6f64 653d 2774 7275 6527  -vim-mode='true'
-00002000: 5d20 2e6a 702d 4e6f 7465 626f 6f6b 3a66  ] .jp-Notebook:f
-00002010: 6f63 7573 222c 0a20 2020 2020 2022 6b65  ocus",.      "ke
-00002020: 7973 223a 205b 0a20 2020 2020 2020 2022  ys": [.        "
-00002030: 5a22 2c0a 2020 2020 2020 2020 224d 220a  Z",.        "M".
-00002040: 2020 2020 2020 5d2c 0a20 2020 2020 2022        ],.      "
-00002050: 636f 6d6d 616e 6422 3a20 226e 6f74 6562  command": "noteb
-00002060: 6f6f 6b3a 6869 6465 2d61 6c6c 2d63 656c  ook:hide-all-cel
-00002070: 6c2d 636f 6465 220a 2020 2020 7d2c 0a20  l-code".    },. 
-00002080: 2020 207b 0a20 2020 2020 2022 7365 6c65     {.      "sele
-00002090: 6374 6f72 223a 2022 2e6a 702d 4e6f 7465  ctor": ".jp-Note
-000020a0: 626f 6f6b 5061 6e65 6c5b 6461 7461 2d6a  bookPanel[data-j
-000020b0: 702d 7669 6d2d 6d6f 6465 3d27 7472 7565  p-vim-mode='true
-000020c0: 275d 202e 6a70 2d4e 6f74 6562 6f6f 6b3a  '] .jp-Notebook:
-000020d0: 666f 6375 7322 2c0a 2020 2020 2020 226b  focus",.      "k
-000020e0: 6579 7322 3a20 5b0a 2020 2020 2020 2020  eys": [.        
-000020f0: 225a 222c 0a20 2020 2020 2020 2022 5222  "Z",.        "R"
-00002100: 0a20 2020 2020 205d 2c0a 2020 2020 2020  .      ],.      
-00002110: 2263 6f6d 6d61 6e64 223a 2022 6e6f 7465  "command": "note
-00002120: 626f 6f6b 3a73 686f 772d 616c 6c2d 6365  book:show-all-ce
-00002130: 6c6c 2d63 6f64 6522 0a20 2020 207d 2c0a  ll-code".    },.
-00002140: 2020 2020 7b0a 2020 2020 2020 2273 656c      {.      "sel
-00002150: 6563 746f 7222 3a20 222e 6a70 2d4e 6f74  ector": ".jp-Not
-00002160: 6562 6f6f 6b50 616e 656c 5b64 6174 612d  ebookPanel[data-
-00002170: 6a70 2d76 696d 2d6d 6f64 653d 2774 7275  jp-vim-mode='tru
-00002180: 6527 5d20 2e6a 702d 4e6f 7465 626f 6f6b  e'] .jp-Notebook
-00002190: 2e6a 702d 6d6f 642d 6564 6974 4d6f 6465  .jp-mod-editMode
-000021a0: 222c 0a20 2020 2020 2022 6b65 7973 223a  ",.      "keys":
-000021b0: 205b 0a20 2020 2020 2020 2022 4374 726c   [.        "Ctrl
-000021c0: 204f 222c 0a20 2020 2020 2020 2022 5a22   O",.        "Z"
-000021d0: 2c0a 2020 2020 2020 2020 225a 220a 2020  ,.        "Z".  
-000021e0: 2020 2020 5d2c 0a20 2020 2020 2022 636f      ],.      "co
-000021f0: 6d6d 616e 6422 3a20 2276 696d 3a63 656e  mmand": "vim:cen
-00002200: 7465 722d 6365 6c6c 220a 2020 2020 7d2c  ter-cell".    },
-00002210: 0a20 2020 207b 0a20 2020 2020 2022 7365  .    {.      "se
-00002220: 6c65 6374 6f72 223a 2022 2e6a 702d 4e6f  lector": ".jp-No
-00002230: 7465 626f 6f6b 5061 6e65 6c5b 6461 7461  tebookPanel[data
-00002240: 2d6a 702d 7669 6d2d 6d6f 6465 3d27 7472  -jp-vim-mode='tr
-00002250: 7565 275d 202e 6a70 2d4e 6f74 6562 6f6f  ue'] .jp-Noteboo
-00002260: 6b2e 6a70 2d6d 6f64 2d65 6469 744d 6f64  k.jp-mod-editMod
-00002270: 6520 2e6a 702d 496e 7075 7441 7265 612d  e .jp-InputArea-
-00002280: 6564 6974 6f72 3a6e 6f74 282e 6a70 2d6d  editor:not(.jp-m
-00002290: 6f64 2d68 6173 2d70 7269 6d61 7279 2d73  od-has-primary-s
-000022a0: 656c 6563 7469 6f6e 2922 2c0a 2020 2020  election)",.    
-000022b0: 2020 226b 6579 7322 3a20 5b0a 2020 2020    "keys": [.    
-000022c0: 2020 2020 2243 7472 6c20 4722 0a20 2020      "Ctrl G".   
-000022d0: 2020 205d 2c0a 2020 2020 2020 2263 6f6d     ],.      "com
-000022e0: 6d61 6e64 223a 2022 746f 6f6c 7469 703a  mand": "tooltip:
-000022f0: 6c61 756e 6368 2d6e 6f74 6562 6f6f 6b22  launch-notebook"
-00002300: 0a20 2020 207d 0a20 205d 2c0a 2020 226a  .    }.  ],.  "j
-00002310: 7570 7974 6572 2e6c 6162 2e6d 656e 7573  upyter.lab.menus
-00002320: 223a 207b 0a20 2020 2022 6d61 696e 223a  ": {.    "main":
-00002330: 205b 0a20 2020 2020 207b 0a20 2020 2020   [.      {.     
-00002340: 2020 2022 6964 223a 2022 6a70 2d6d 6169     "id": "jp-mai
-00002350: 6e6d 656e 752d 7365 7474 696e 6773 222c  nmenu-settings",
-00002360: 0a20 2020 2020 2020 2022 6974 656d 7322  .        "items"
-00002370: 3a20 5b0a 2020 2020 2020 2020 2020 7b0a  : [.          {.
-00002380: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00002390: 6522 3a20 2273 6570 6172 6174 6f72 222c  e": "separator",
-000023a0: 0a20 2020 2020 2020 2020 2020 2022 7261  .            "ra
-000023b0: 6e6b 223a 2033 380a 2020 2020 2020 2020  nk": 38.        
-000023c0: 2020 7d2c 0a20 2020 2020 2020 2020 207b    },.          {
-000023d0: 0a20 2020 2020 2020 2020 2020 2022 636f  .            "co
-000023e0: 6d6d 616e 6422 3a20 226a 7570 7974 6572  mmand": "jupyter
-000023f0: 6c61 622d 7669 6d3a 746f 6767 6c65 222c  lab-vim:toggle",
-00002400: 0a20 2020 2020 2020 2020 2020 2022 7261  .            "ra
-00002410: 6e6b 223a 2033 380a 2020 2020 2020 2020  nk": 38.        
-00002420: 2020 7d2c 0a20 2020 2020 2020 2020 207b    },.          {
-00002430: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
-00002440: 7065 223a 2022 7365 7061 7261 746f 7222  pe": "separator"
-00002450: 2c0a 2020 2020 2020 2020 2020 2020 2272  ,.            "r
-00002460: 616e 6b22 3a20 3338 0a20 2020 2020 2020  ank": 38.       
-00002470: 2020 207d 0a20 2020 2020 2020 205d 0a20     }.        ]. 
-00002480: 2020 2020 207d 0a20 2020 205d 0a20 207d       }.    ].  }
-00002490: 2c0a 2020 2270 726f 7065 7274 6965 7322  ,.  "properties"
-000024a0: 3a20 7b0a 2020 2020 2265 6e61 626c 6564  : {.    "enabled
-000024b0: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
-000024c0: 223a 2022 626f 6f6c 6561 6e22 2c0a 2020  ": "boolean",.  
-000024d0: 2020 2020 2274 6974 6c65 223a 2022 456e      "title": "En
-000024e0: 6162 6c65 6422 2c0a 2020 2020 2020 2264  abled",.      "d
-000024f0: 6573 6372 6970 7469 6f6e 223a 2022 456e  escription": "En
-00002500: 6162 6c65 2f64 6973 6162 6c65 206e 6f74  able/disable not
-00002510: 6562 6f6f 6b20 7669 6d20 286d 6179 2072  ebook vim (may r
-00002520: 6571 7569 7265 2061 2070 6167 6520 7265  equire a page re
-00002530: 6672 6573 6829 222c 0a20 2020 2020 2022  fresh)",.      "
-00002540: 6465 6661 756c 7422 3a20 7472 7565 0a20  default": true. 
-00002550: 2020 207d 2c0a 2020 2020 2265 7874 7261     },.    "extra
-00002560: 4b65 7962 696e 6469 6e67 7322 3a20 7b0a  Keybindings": {.
-00002570: 2020 2020 2020 2274 7970 6522 3a20 2261        "type": "a
-00002580: 7272 6179 222c 0a20 2020 2020 2022 7469  rray",.      "ti
-00002590: 746c 6522 3a20 2245 7874 7261 2056 696d  tle": "Extra Vim
-000025a0: 204b 6579 6269 6e64 696e 6773 222c 0a20   Keybindings",. 
-000025b0: 2020 2020 2022 6974 656d 7322 3a20 7b0a       "items": {.
-000025c0: 2020 2020 2020 2020 2224 7265 6622 3a20          "$ref": 
-000025d0: 2223 2f64 6566 696e 6974 696f 6e73 2f73  "#/definitions/s
-000025e0: 686f 7274 6375 7422 0a20 2020 2020 207d  hortcut".      }
-000025f0: 2c0a 2020 2020 2020 2264 6566 6175 6c74  ,.      "default
-00002600: 223a 205b 5d0a 2020 2020 7d0a 2020 7d2c  ": [].    }.  },
-00002610: 0a20 2022 6465 6669 6e69 7469 6f6e 7322  .  "definitions"
-00002620: 3a20 7b0a 2020 2020 2273 686f 7274 6375  : {.    "shortcu
-00002630: 7422 3a20 7b0a 2020 2020 2020 2270 726f  t": {.      "pro
-00002640: 7065 7274 6965 7322 3a20 7b0a 2020 2020  perties": {.    
-00002650: 2020 2020 2263 6f6d 6d61 6e64 223a 207b      "command": {
-00002660: 0a20 2020 2020 2020 2020 2022 7469 746c  .          "titl
-00002670: 6522 3a20 224b 6579 6269 6e64 696e 6722  e": "Keybinding"
-00002680: 2c0a 2020 2020 2020 2020 2020 2264 6573  ,.          "des
-00002690: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
-000026a0: 6e65 7720 7669 6d20 6b65 7962 696e 6469  new vim keybindi
-000026b0: 6e67 2c20 6f72 2027 6c65 6674 2068 616e  ng, or 'left han
-000026c0: 6420 7369 6465 2720 6f66 2074 6865 206b  d side' of the k
-000026d0: 6579 6269 6e64 696e 672c 2065 2e67 2e20  eybinding, e.g. 
-000026e0: 604d 6022 2c0a 2020 2020 2020 2020 2020  `M`",.          
-000026f0: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
-00002700: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
-00002710: 2020 2020 226b 6579 7322 3a20 7b0a 2020      "keys": {.  
-00002720: 2020 2020 2020 2020 2274 6974 6c65 223a          "title":
-00002730: 2022 5468 6520 6b65 7920 7365 7175 656e   "The key sequen
-00002740: 6365 2074 6f20 6578 6563 7574 6522 2c0a  ce to execute",.
-00002750: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00002760: 6970 7469 6f6e 223a 2022 5468 6520 2772  iption": "The 'r
-00002770: 6967 6874 2068 616e 6420 7369 6465 2720  ight hand side' 
-00002780: 6f66 2074 6865 206b 6579 6269 6e64 696e  of the keybindin
-00002790: 6720 746f 2062 6520 6578 6563 7574 6564  g to be executed
-000027a0: 2c20 652e 672e 2060 3a6e 6f68 3c63 723e  , e.g. `:noh<cr>
-000027b0: 6022 2c0a 2020 2020 2020 2020 2020 2274  `",.          "t
-000027c0: 7970 6522 3a20 2273 7472 696e 6722 0a20  ype": "string". 
-000027d0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-000027e0: 2020 2263 6f6e 7465 7874 223a 207b 0a20    "context": {. 
-000027f0: 2020 2020 2020 2020 2022 7469 746c 6522           "title"
-00002800: 3a20 224d 6f64 6522 2c0a 2020 2020 2020  : "Mode",.      
-00002810: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00002820: 223a 2022 5669 6d20 6d6f 6465 2069 6e20  ": "Vim mode in 
-00002830: 7768 6963 6820 7468 6520 6b65 7962 696e  which the keybin
-00002840: 6469 6e67 2061 7070 6c69 6573 222c 0a20  ding applies",. 
-00002850: 2020 2020 2020 2020 2022 656e 756d 223a           "enum":
-00002860: 205b 0a20 2020 2020 2020 2020 2020 2022   [.            "
-00002870: 6e6f 726d 616c 222c 0a20 2020 2020 2020  normal",.       
-00002880: 2020 2020 2022 696e 7365 7274 222c 0a20       "insert",. 
-00002890: 2020 2020 2020 2020 2020 2022 7669 7375             "visu
-000028a0: 616c 220a 2020 2020 2020 2020 2020 5d2c  al".          ],
-000028b0: 0a20 2020 2020 2020 2020 2022 6465 6661  .          "defa
-000028c0: 756c 7422 3a20 226e 6f72 6d61 6c22 0a20  ult": "normal". 
-000028d0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-000028e0: 2020 226d 6170 666e 223a 207b 0a20 2020    "mapfn": {.   
-000028f0: 2020 2020 2020 2022 7469 746c 6522 3a20         "title": 
-00002900: 224d 6170 2066 756e 6374 696f 6e22 2c0a  "Map function",.
-00002910: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00002920: 6970 7469 6f6e 223a 2022 5669 6d20 6d61  iption": "Vim ma
-00002930: 7020 6675 6e63 7469 6f6e 2074 6f20 7573  p function to us
-00002940: 6522 2c0a 2020 2020 2020 2020 2020 2265  e",.          "e
-00002950: 6e75 6d22 3a20 5b0a 2020 2020 2020 2020  num": [.        
-00002960: 2020 2020 226d 6170 222c 0a20 2020 2020      "map",.     
-00002970: 2020 2020 2020 2022 6e6f 7265 6d61 7022         "noremap"
-00002980: 0a20 2020 2020 2020 2020 205d 2c0a 2020  .          ],.  
-00002990: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
-000029a0: 223a 2022 6d61 7022 0a20 2020 2020 2020  ": "map".       
-000029b0: 207d 2c0a 2020 2020 2020 2020 2265 6e61   },.        "ena
-000029c0: 626c 6564 223a 207b 0a20 2020 2020 2020  bled": {.       
-000029d0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-000029e0: 3a20 2257 6865 7468 6572 2074 6869 7320  : "Whether this 
-000029f0: 6b65 7962 696e 6469 6e67 2069 7320 656e  keybinding is en
-00002a00: 6162 6c65 6420 6f72 206e 6f74 2e22 2c0a  abled or not.",.
-00002a10: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00002a20: 3a20 2262 6f6f 6c65 616e 222c 0a20 2020  : "boolean",.   
-00002a30: 2020 2020 2020 2022 6465 6661 756c 7422         "default"
-00002a40: 3a20 7472 7565 0a20 2020 2020 2020 207d  : true.        }
-00002a50: 0a20 2020 2020 207d 2c0a 2020 2020 2020  .      },.      
-00002a60: 2272 6571 7569 7265 6422 3a20 5b0a 2020  "required": [.  
-00002a70: 2020 2020 2020 2263 6f6d 6d61 6e64 222c        "command",
-00002a80: 0a20 2020 2020 2020 2022 6b65 7973 220a  .        "keys".
-00002a90: 2020 2020 2020 5d2c 0a20 2020 2020 2022        ],.      "
-00002aa0: 7479 7065 223a 2022 6f62 6a65 6374 220a  type": "object".
-00002ab0: 2020 2020 7d0a 2020 7d0a 7d0a                }.  }.}.
+000000d0: 2020 2020 2022 6b65 7973 223a 205b 2245       "keys": ["E
+000000e0: 7363 6170 6522 5d2c 0a20 2020 2020 2022  scape"],.      "
+000000f0: 7365 6c65 6374 6f72 223a 2022 2e6a 702d  selector": ".jp-
+00000100: 4e6f 7465 626f 6f6b 2e6a 702d 6d6f 642d  Notebook.jp-mod-
+00000110: 6564 6974 4d6f 6465 222c 0a20 2020 2020  editMode",.     
+00000120: 2022 6469 7361 626c 6564 223a 2074 7275   "disabled": tru
+00000130: 650a 2020 2020 7d2c 0a20 2020 207b 0a20  e.    },.    {. 
+00000140: 2020 2020 2022 7365 6c65 6374 6f72 223a       "selector":
+00000150: 2022 2e6a 702d 4e6f 7465 626f 6f6b 5061   ".jp-NotebookPa
+00000160: 6e65 6c5b 6461 7461 2d6a 702d 7669 6d2d  nel[data-jp-vim-
+00000170: 6d6f 6465 3d27 7472 7565 275d 202e 6a70  mode='true'] .jp
+00000180: 2d4e 6f74 6562 6f6f 6b2e 6a70 2d6d 6f64  -Notebook.jp-mod
+00000190: 2d65 6469 744d 6f64 6522 2c0a 2020 2020  -editMode",.    
+000001a0: 2020 226b 6579 7322 3a20 5b22 4374 726c    "keys": ["Ctrl
+000001b0: 204f 222c 2022 5522 5d2c 0a20 2020 2020   O", "U"],.     
+000001c0: 2022 636f 6d6d 616e 6422 3a20 226e 6f74   "command": "not
+000001d0: 6562 6f6f 6b3a 756e 646f 2d63 656c 6c2d  ebook:undo-cell-
+000001e0: 6163 7469 6f6e 220a 2020 2020 7d2c 0a20  action".    },. 
+000001f0: 2020 207b 0a20 2020 2020 2022 7365 6c65     {.      "sele
+00000200: 6374 6f72 223a 2022 2e6a 702d 4e6f 7465  ctor": ".jp-Note
+00000210: 626f 6f6b 5061 6e65 6c5b 6461 7461 2d6a  bookPanel[data-j
+00000220: 702d 7669 6d2d 6d6f 6465 3d27 7472 7565  p-vim-mode='true
+00000230: 275d 202e 6a70 2d4e 6f74 6562 6f6f 6b50  '] .jp-NotebookP
+00000240: 616e 656c 5b64 6174 612d 6a70 2d76 696d  anel[data-jp-vim
+00000250: 2d6d 6f64 653d 2774 7275 6527 5d20 2e6a  -mode='true'] .j
+00000260: 702d 4e6f 7465 626f 6f6b 2e6a 702d 6d6f  p-Notebook.jp-mo
+00000270: 642d 6564 6974 4d6f 6465 222c 0a20 2020  d-editMode",.   
+00000280: 2020 2022 6b65 7973 223a 205b 2243 7472     "keys": ["Ctr
+00000290: 6c20 4f22 2c20 222d 225d 2c0a 2020 2020  l O", "-"],.    
+000002a0: 2020 2263 6f6d 6d61 6e64 223a 2022 6e6f    "command": "no
+000002b0: 7465 626f 6f6b 3a73 706c 6974 2d63 656c  tebook:split-cel
+000002c0: 6c2d 6174 2d63 7572 736f 7222 0a20 2020  l-at-cursor".   
+000002d0: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
+000002e0: 2273 656c 6563 746f 7222 3a20 222e 6a70  "selector": ".jp
+000002f0: 2d4e 6f74 6562 6f6f 6b50 616e 656c 5b64  -NotebookPanel[d
+00000300: 6174 612d 6a70 2d76 696d 2d6d 6f64 653d  ata-jp-vim-mode=
+00000310: 2774 7275 6527 5d20 2e6a 702d 4e6f 7465  'true'] .jp-Note
+00000320: 626f 6f6b 2e6a 702d 6d6f 642d 6564 6974  book.jp-mod-edit
+00000330: 4d6f 6465 222c 0a20 2020 2020 2022 6b65  Mode",.      "ke
+00000340: 7973 223a 205b 2243 7472 6c20 4f22 2c20  ys": ["Ctrl O", 
+00000350: 2244 225d 2c0a 2020 2020 2020 2263 6f6d  "D"],.      "com
+00000360: 6d61 6e64 223a 2022 7669 6d3a 6375 742d  mand": "vim:cut-
+00000370: 6365 6c6c 2d61 6e64 2d65 6469 7422 0a20  cell-and-edit". 
+00000380: 2020 207d 2c0a 2020 2020 7b0a 2020 2020     },.    {.    
+00000390: 2020 2273 656c 6563 746f 7222 3a20 222e    "selector": ".
+000003a0: 6a70 2d4e 6f74 6562 6f6f 6b50 616e 656c  jp-NotebookPanel
+000003b0: 5b64 6174 612d 6a70 2d76 696d 2d6d 6f64  [data-jp-vim-mod
+000003c0: 653d 2774 7275 6527 5d20 2e6a 702d 4e6f  e='true'] .jp-No
+000003d0: 7465 626f 6f6b 2e6a 702d 6d6f 642d 6564  tebook.jp-mod-ed
+000003e0: 6974 4d6f 6465 222c 0a20 2020 2020 2022  itMode",.      "
+000003f0: 6b65 7973 223a 205b 2243 7472 6c20 4f22  keys": ["Ctrl O"
+00000400: 2c20 2259 225d 2c0a 2020 2020 2020 2263  , "Y"],.      "c
+00000410: 6f6d 6d61 6e64 223a 2022 7669 6d3a 636f  ommand": "vim:co
+00000420: 7079 2d63 656c 6c2d 616e 642d 6564 6974  py-cell-and-edit
+00000430: 220a 2020 2020 7d2c 0a20 2020 207b 0a20  ".    },.    {. 
+00000440: 2020 2020 2022 7365 6c65 6374 6f72 223a       "selector":
+00000450: 2022 2e6a 702d 4e6f 7465 626f 6f6b 5061   ".jp-NotebookPa
+00000460: 6e65 6c5b 6461 7461 2d6a 702d 7669 6d2d  nel[data-jp-vim-
+00000470: 6d6f 6465 3d27 7472 7565 275d 202e 6a70  mode='true'] .jp
+00000480: 2d4e 6f74 6562 6f6f 6b2e 6a70 2d6d 6f64  -Notebook.jp-mod
+00000490: 2d65 6469 744d 6f64 6522 2c0a 2020 2020  -editMode",.    
+000004a0: 2020 226b 6579 7322 3a20 5b22 4374 726c    "keys": ["Ctrl
+000004b0: 204f 222c 2022 5022 5d2c 0a20 2020 2020   O", "P"],.     
+000004c0: 2022 636f 6d6d 616e 6422 3a20 2276 696d   "command": "vim
+000004d0: 3a70 6173 7465 2d63 656c 6c2d 616e 642d  :paste-cell-and-
+000004e0: 6564 6974 220a 2020 2020 7d2c 0a20 2020  edit".    },.   
+000004f0: 207b 0a20 2020 2020 2022 7365 6c65 6374   {.      "select
+00000500: 6f72 223a 2022 2e6a 702d 4e6f 7465 626f  or": ".jp-Notebo
+00000510: 6f6b 5061 6e65 6c5b 6461 7461 2d6a 702d  okPanel[data-jp-
+00000520: 7669 6d2d 6d6f 6465 3d27 7472 7565 275d  vim-mode='true']
+00000530: 202e 6a70 2d4e 6f74 6562 6f6f 6b2e 6a70   .jp-Notebook.jp
+00000540: 2d6d 6f64 2d65 6469 744d 6f64 6522 2c0a  -mod-editMode",.
+00000550: 2020 2020 2020 226b 6579 7322 3a20 5b22        "keys": ["
+00000560: 4374 726c 2053 6869 6674 204a 225d 2c0a  Ctrl Shift J"],.
+00000570: 2020 2020 2020 2263 6f6d 6d61 6e64 223a        "command":
+00000580: 2022 6e6f 7465 626f 6f6b 3a65 7874 656e   "notebook:exten
+00000590: 642d 6d61 726b 6564 2d63 656c 6c73 2d62  d-marked-cells-b
+000005a0: 656c 6f77 220a 2020 2020 7d2c 0a20 2020  elow".    },.   
+000005b0: 207b 0a20 2020 2020 2022 7365 6c65 6374   {.      "select
+000005c0: 6f72 223a 2022 2e6a 702d 4e6f 7465 626f  or": ".jp-Notebo
+000005d0: 6f6b 5061 6e65 6c5b 6461 7461 2d6a 702d  okPanel[data-jp-
+000005e0: 7669 6d2d 6d6f 6465 3d27 7472 7565 275d  vim-mode='true']
+000005f0: 202e 6a70 2d4e 6f74 6562 6f6f 6b3a 666f   .jp-Notebook:fo
+00000600: 6375 7322 2c0a 2020 2020 2020 226b 6579  cus",.      "key
+00000610: 7322 3a20 5b22 4374 726c 2053 6869 6674  s": ["Ctrl Shift
+00000620: 204a 225d 2c0a 2020 2020 2020 2263 6f6d   J"],.      "com
+00000630: 6d61 6e64 223a 2022 6e6f 7465 626f 6f6b  mand": "notebook
+00000640: 3a65 7874 656e 642d 6d61 726b 6564 2d63  :extend-marked-c
+00000650: 656c 6c73 2d62 656c 6f77 220a 2020 2020  ells-below".    
+00000660: 7d2c 0a20 2020 207b 0a20 2020 2020 2022  },.    {.      "
+00000670: 7365 6c65 6374 6f72 223a 2022 2e6a 702d  selector": ".jp-
+00000680: 4e6f 7465 626f 6f6b 5061 6e65 6c5b 6461  NotebookPanel[da
+00000690: 7461 2d6a 702d 7669 6d2d 6d6f 6465 3d27  ta-jp-vim-mode='
+000006a0: 7472 7565 275d 202e 6a70 2d4e 6f74 6562  true'] .jp-Noteb
+000006b0: 6f6f 6b2e 6a70 2d6d 6f64 2d65 6469 744d  ook.jp-mod-editM
+000006c0: 6f64 6522 2c0a 2020 2020 2020 226b 6579  ode",.      "key
+000006d0: 7322 3a20 5b22 4374 726c 2053 6869 6674  s": ["Ctrl Shift
+000006e0: 204b 225d 2c0a 2020 2020 2020 2263 6f6d   K"],.      "com
+000006f0: 6d61 6e64 223a 2022 6e6f 7465 626f 6f6b  mand": "notebook
+00000700: 3a65 7874 656e 642d 6d61 726b 6564 2d63  :extend-marked-c
+00000710: 656c 6c73 2d61 626f 7665 220a 2020 2020  ells-above".    
+00000720: 7d2c 0a20 2020 207b 0a20 2020 2020 2022  },.    {.      "
+00000730: 7365 6c65 6374 6f72 223a 2022 2e6a 702d  selector": ".jp-
+00000740: 4e6f 7465 626f 6f6b 5061 6e65 6c5b 6461  NotebookPanel[da
+00000750: 7461 2d6a 702d 7669 6d2d 6d6f 6465 3d27  ta-jp-vim-mode='
+00000760: 7472 7565 275d 202e 6a70 2d4e 6f74 6562  true'] .jp-Noteb
+00000770: 6f6f 6b3a 666f 6375 7322 2c0a 2020 2020  ook:focus",.    
+00000780: 2020 226b 6579 7322 3a20 5b22 4374 726c    "keys": ["Ctrl
+00000790: 2053 6869 6674 204b 225d 2c0a 2020 2020   Shift K"],.    
+000007a0: 2020 2263 6f6d 6d61 6e64 223a 2022 6e6f    "command": "no
+000007b0: 7465 626f 6f6b 3a65 7874 656e 642d 6d61  tebook:extend-ma
+000007c0: 726b 6564 2d63 656c 6c73 2d61 626f 7665  rked-cells-above
+000007d0: 220a 2020 2020 7d2c 0a20 2020 207b 0a20  ".    },.    {. 
+000007e0: 2020 2020 2022 7365 6c65 6374 6f72 223a       "selector":
+000007f0: 2022 2e6a 702d 4e6f 7465 626f 6f6b 5061   ".jp-NotebookPa
+00000800: 6e65 6c5b 6461 7461 2d6a 702d 7669 6d2d  nel[data-jp-vim-
+00000810: 6d6f 6465 3d27 7472 7565 275d 202e 6a70  mode='true'] .jp
+00000820: 2d4e 6f74 6562 6f6f 6b2e 6a70 2d6d 6f64  -Notebook.jp-mod
+00000830: 2d65 6469 744d 6f64 6522 2c0a 2020 2020  -editMode",.    
+00000840: 2020 226b 6579 7322 3a20 5b22 4374 726c    "keys": ["Ctrl
+00000850: 204f 222c 2022 5368 6966 7420 4f22 5d2c   O", "Shift O"],
+00000860: 0a20 2020 2020 2022 636f 6d6d 616e 6422  .      "command"
+00000870: 3a20 226e 6f74 6562 6f6f 6b3a 696e 7365  : "notebook:inse
+00000880: 7274 2d63 656c 6c2d 6162 6f76 6522 0a20  rt-cell-above". 
+00000890: 2020 207d 2c0a 2020 2020 7b0a 2020 2020     },.    {.    
+000008a0: 2020 2273 656c 6563 746f 7222 3a20 222e    "selector": ".
+000008b0: 6a70 2d4e 6f74 6562 6f6f 6b50 616e 656c  jp-NotebookPanel
+000008c0: 5b64 6174 612d 6a70 2d76 696d 2d6d 6f64  [data-jp-vim-mod
+000008d0: 653d 2774 7275 6527 5d20 2e6a 702d 4e6f  e='true'] .jp-No
+000008e0: 7465 626f 6f6b 2e6a 702d 6d6f 642d 6564  tebook.jp-mod-ed
+000008f0: 6974 4d6f 6465 222c 0a20 2020 2020 2022  itMode",.      "
+00000900: 6b65 7973 223a 205b 2243 7472 6c20 4f22  keys": ["Ctrl O"
+00000910: 2c20 2243 7472 6c20 4f22 5d2c 0a20 2020  , "Ctrl O"],.   
+00000920: 2020 2022 636f 6d6d 616e 6422 3a20 226e     "command": "n
+00000930: 6f74 6562 6f6f 6b3a 696e 7365 7274 2d63  otebook:insert-c
+00000940: 656c 6c2d 6162 6f76 6522 0a20 2020 207d  ell-above".    }
+00000950: 2c0a 2020 2020 7b0a 2020 2020 2020 2273  ,.    {.      "s
+00000960: 656c 6563 746f 7222 3a20 222e 6a70 2d4e  elector": ".jp-N
+00000970: 6f74 6562 6f6f 6b50 616e 656c 5b64 6174  otebookPanel[dat
+00000980: 612d 6a70 2d76 696d 2d6d 6f64 653d 2774  a-jp-vim-mode='t
+00000990: 7275 6527 5d20 2e6a 702d 4e6f 7465 626f  rue'] .jp-Notebo
+000009a0: 6f6b 2e6a 702d 6d6f 642d 6564 6974 4d6f  ok.jp-mod-editMo
+000009b0: 6465 222c 0a20 2020 2020 2022 6b65 7973  de",.      "keys
+000009c0: 223a 205b 2243 7472 6c20 4f22 2c20 224f  ": ["Ctrl O", "O
+000009d0: 225d 2c0a 2020 2020 2020 2263 6f6d 6d61  "],.      "comma
+000009e0: 6e64 223a 2022 6e6f 7465 626f 6f6b 3a69  nd": "notebook:i
+000009f0: 6e73 6572 742d 6365 6c6c 2d62 656c 6f77  nsert-cell-below
+00000a00: 220a 2020 2020 7d2c 0a20 2020 207b 0a20  ".    },.    {. 
+00000a10: 2020 2020 2022 7365 6c65 6374 6f72 223a       "selector":
+00000a20: 2022 2e6a 702d 4e6f 7465 626f 6f6b 5061   ".jp-NotebookPa
+00000a30: 6e65 6c5b 6461 7461 2d6a 702d 7669 6d2d  nel[data-jp-vim-
+00000a40: 6d6f 6465 3d27 7472 7565 275d 202e 6a70  mode='true'] .jp
+00000a50: 2d4e 6f74 6562 6f6f 6b2e 6a70 2d6d 6f64  -Notebook.jp-mod
+00000a60: 2d65 6469 744d 6f64 6522 2c0a 2020 2020  -editMode",.    
+00000a70: 2020 226b 6579 7322 3a20 5b22 4374 726c    "keys": ["Ctrl
+00000a80: 204a 225d 2c0a 2020 2020 2020 2263 6f6d   J"],.      "com
+00000a90: 6d61 6e64 223a 2022 7669 6d3a 7365 6c65  mand": "vim:sele
+00000aa0: 6374 2d62 656c 6f77 2d65 7865 6375 7465  ct-below-execute
+00000ab0: 2d6d 6172 6b64 6f77 6e22 0a20 2020 207d  -markdown".    }
+00000ac0: 2c0a 2020 2020 7b0a 2020 2020 2020 2273  ,.    {.      "s
+00000ad0: 656c 6563 746f 7222 3a20 222e 6a70 2d4e  elector": ".jp-N
+00000ae0: 6f74 6562 6f6f 6b50 616e 656c 5b64 6174  otebookPanel[dat
+00000af0: 612d 6a70 2d76 696d 2d6d 6f64 653d 2774  a-jp-vim-mode='t
+00000b00: 7275 6527 5d20 2e6a 702d 4e6f 7465 626f  rue'] .jp-Notebo
+00000b10: 6f6b 2e6a 702d 6d6f 642d 6564 6974 4d6f  ok.jp-mod-editMo
+00000b20: 6465 222c 0a20 2020 2020 2022 6b65 7973  de",.      "keys
+00000b30: 223a 205b 2243 7472 6c20 4b22 5d2c 0a20  ": ["Ctrl K"],. 
+00000b40: 2020 2020 2022 636f 6d6d 616e 6422 3a20       "command": 
+00000b50: 2276 696d 3a73 656c 6563 742d 6162 6f76  "vim:select-abov
+00000b60: 652d 6578 6563 7574 652d 6d61 726b 646f  e-execute-markdo
+00000b70: 776e 220a 2020 2020 7d2c 0a20 2020 207b  wn".    },.    {
+00000b80: 0a20 2020 2020 2022 7365 6c65 6374 6f72  .      "selector
+00000b90: 223a 2022 2e6a 702d 4e6f 7465 626f 6f6b  ": ".jp-Notebook
+00000ba0: 5061 6e65 6c5b 6461 7461 2d6a 702d 7669  Panel[data-jp-vi
+00000bb0: 6d2d 6d6f 6465 3d27 7472 7565 275d 202e  m-mode='true'] .
+00000bc0: 6a70 2d4e 6f74 6562 6f6f 6b2e 6a70 2d6d  jp-Notebook.jp-m
+00000bd0: 6f64 2d65 6469 744d 6f64 6522 2c0a 2020  od-editMode",.  
+00000be0: 2020 2020 226b 6579 7322 3a20 5b22 4573      "keys": ["Es
+00000bf0: 6361 7065 225d 2c0a 2020 2020 2020 2263  cape"],.      "c
+00000c00: 6f6d 6d61 6e64 223a 2022 7669 6d3a 6c65  ommand": "vim:le
+00000c10: 6176 652d 696e 7365 7274 2d6d 6f64 6522  ave-insert-mode"
+00000c20: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
+00000c30: 2020 2020 2273 656c 6563 746f 7222 3a20      "selector": 
+00000c40: 222e 6a70 2d4e 6f74 6562 6f6f 6b50 616e  ".jp-NotebookPan
+00000c50: 656c 5b64 6174 612d 6a70 2d76 696d 2d6d  el[data-jp-vim-m
+00000c60: 6f64 653d 2774 7275 6527 5d20 2e6a 702d  ode='true'] .jp-
+00000c70: 4e6f 7465 626f 6f6b 2e6a 702d 6d6f 642d  Notebook.jp-mod-
+00000c80: 6564 6974 4d6f 6465 222c 0a20 2020 2020  editMode",.     
+00000c90: 2022 6b65 7973 223a 205b 2243 7472 6c20   "keys": ["Ctrl 
+00000ca0: 5b22 5d2c 0a20 2020 2020 2022 636f 6d6d  ["],.      "comm
+00000cb0: 616e 6422 3a20 2276 696d 3a6c 6561 7665  and": "vim:leave
+00000cc0: 2d69 6e73 6572 742d 6d6f 6465 220a 2020  -insert-mode".  
+00000cd0: 2020 7d2c 0a20 2020 207b 0a20 2020 2020    },.    {.     
+00000ce0: 2022 7365 6c65 6374 6f72 223a 2022 2e6a   "selector": ".j
+00000cf0: 702d 4e6f 7465 626f 6f6b 5061 6e65 6c5b  p-NotebookPanel[
+00000d00: 6461 7461 2d6a 702d 7669 6d2d 6d6f 6465  data-jp-vim-mode
+00000d10: 3d27 7472 7565 275d 202e 6a70 2d4e 6f74  ='true'] .jp-Not
+00000d20: 6562 6f6f 6b3a 666f 6375 7322 2c0a 2020  ebook:focus",.  
+00000d30: 2020 2020 226b 6579 7322 3a20 5b22 4374      "keys": ["Ct
+00000d40: 726c 2049 225d 2c0a 2020 2020 2020 2263  rl I"],.      "c
+00000d50: 6f6d 6d61 6e64 223a 2022 7669 6d3a 656e  ommand": "vim:en
+00000d60: 7465 722d 696e 7365 7274 2d6d 6f64 6522  ter-insert-mode"
+00000d70: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
+00000d80: 2020 2020 2273 656c 6563 746f 7222 3a20      "selector": 
+00000d90: 222e 6a70 2d4e 6f74 6562 6f6f 6b50 616e  ".jp-NotebookPan
+00000da0: 656c 5b64 6174 612d 6a70 2d76 696d 2d6d  el[data-jp-vim-m
+00000db0: 6f64 653d 2774 7275 6527 5d20 2e6a 702d  ode='true'] .jp-
+00000dc0: 4e6f 7465 626f 6f6b 2e6a 702d 6d6f 642d  Notebook.jp-mod-
+00000dd0: 6564 6974 4d6f 6465 222c 0a20 2020 2020  editMode",.     
+00000de0: 2022 6b65 7973 223a 205b 2243 7472 6c20   "keys": ["Ctrl 
+00000df0: 456e 7465 7222 5d2c 0a20 2020 2020 2022  Enter"],.      "
+00000e00: 636f 6d6d 616e 6422 3a20 2276 696d 3a72  command": "vim:r
+00000e10: 756e 2d63 656c 6c2d 616e 642d 6564 6974  un-cell-and-edit
+00000e20: 220a 2020 2020 7d2c 0a20 2020 207b 0a20  ".    },.    {. 
+00000e30: 2020 2020 2022 7365 6c65 6374 6f72 223a       "selector":
+00000e40: 2022 2e6a 702d 4e6f 7465 626f 6f6b 5061   ".jp-NotebookPa
+00000e50: 6e65 6c5b 6461 7461 2d6a 702d 7669 6d2d  nel[data-jp-vim-
+00000e60: 6d6f 6465 3d27 7472 7565 275d 202e 6a70  mode='true'] .jp
+00000e70: 2d4e 6f74 6562 6f6f 6b2e 6a70 2d6d 6f64  -Notebook.jp-mod
+00000e80: 2d65 6469 744d 6f64 6522 2c0a 2020 2020  -editMode",.    
+00000e90: 2020 226b 6579 7322 3a20 5b22 5368 6966    "keys": ["Shif
+00000ea0: 7420 456e 7465 7222 5d2c 0a20 2020 2020  t Enter"],.     
+00000eb0: 2022 636f 6d6d 616e 6422 3a20 2276 696d   "command": "vim
+00000ec0: 3a72 756e 2d73 656c 6563 742d 6e65 7874  :run-select-next
+00000ed0: 2d65 6469 7422 0a20 2020 207d 2c0a 2020  -edit".    },.  
+00000ee0: 2020 7b0a 2020 2020 2020 2273 656c 6563    {.      "selec
+00000ef0: 746f 7222 3a20 222e 6a70 2d4e 6f74 6562  tor": ".jp-Noteb
+00000f00: 6f6f 6b50 616e 656c 5b64 6174 612d 6a70  ookPanel[data-jp
+00000f10: 2d76 696d 2d6d 6f64 653d 2774 7275 6527  -vim-mode='true'
+00000f20: 5d20 2e6a 702d 4e6f 7465 626f 6f6b 2e6a  ] .jp-Notebook.j
+00000f30: 702d 6d6f 642d 6564 6974 4d6f 6465 222c  p-mod-editMode",
+00000f40: 0a20 2020 2020 2022 6b65 7973 223a 205b  .      "keys": [
+00000f50: 2253 6869 6674 2045 7363 6170 6522 5d2c  "Shift Escape"],
+00000f60: 0a20 2020 2020 2022 636f 6d6d 616e 6422  .      "command"
+00000f70: 3a20 226e 6f74 6562 6f6f 6b3a 656e 7465  : "notebook:ente
+00000f80: 722d 636f 6d6d 616e 642d 6d6f 6465 220a  r-command-mode".
+00000f90: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
+00000fa0: 2020 2022 7365 6c65 6374 6f72 223a 2022     "selector": "
+00000fb0: 2e6a 702d 4e6f 7465 626f 6f6b 5061 6e65  .jp-NotebookPane
+00000fc0: 6c5b 6461 7461 2d6a 702d 7669 6d2d 6d6f  l[data-jp-vim-mo
+00000fd0: 6465 3d27 7472 7565 275d 202e 6a70 2d4e  de='true'] .jp-N
+00000fe0: 6f74 6562 6f6f 6b3a 666f 6375 7322 2c0a  otebook:focus",.
+00000ff0: 2020 2020 2020 226b 6579 7322 3a20 5b22        "keys": ["
+00001000: 5368 6966 7420 4d22 5d2c 0a20 2020 2020  Shift M"],.     
+00001010: 2022 636f 6d6d 616e 6422 3a20 2276 696d   "command": "vim
+00001020: 3a6d 6572 6765 2d61 6e64 2d65 6469 7422  :merge-and-edit"
+00001030: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
+00001040: 2020 2020 2273 656c 6563 746f 7222 3a20      "selector": 
+00001050: 222e 6a70 2d4e 6f74 6562 6f6f 6b50 616e  ".jp-NotebookPan
+00001060: 656c 5b64 6174 612d 6a70 2d76 696d 2d6d  el[data-jp-vim-m
+00001070: 6f64 653d 2774 7275 6527 5d20 2e6a 702d  ode='true'] .jp-
+00001080: 4e6f 7465 626f 6f6b 2e6a 702d 6d6f 642d  Notebook.jp-mod-
+00001090: 6564 6974 4d6f 6465 222c 0a20 2020 2020  editMode",.     
+000010a0: 2022 6b65 7973 223a 205b 2241 6363 656c   "keys": ["Accel
+000010b0: 2031 225d 2c0a 2020 2020 2020 2263 6f6d   1"],.      "com
+000010c0: 6d61 6e64 223a 2022 6e6f 7465 626f 6f6b  mand": "notebook
+000010d0: 3a63 6861 6e67 652d 6365 6c6c 2d74 6f2d  :change-cell-to-
+000010e0: 636f 6465 220a 2020 2020 7d2c 0a20 2020  code".    },.   
+000010f0: 207b 0a20 2020 2020 2022 7365 6c65 6374   {.      "select
+00001100: 6f72 223a 2022 2e6a 702d 4e6f 7465 626f  or": ".jp-Notebo
+00001110: 6f6b 5061 6e65 6c5b 6461 7461 2d6a 702d  okPanel[data-jp-
+00001120: 7669 6d2d 6d6f 6465 3d27 7472 7565 275d  vim-mode='true']
+00001130: 202e 6a70 2d4e 6f74 6562 6f6f 6b2e 6a70   .jp-Notebook.jp
+00001140: 2d6d 6f64 2d65 6469 744d 6f64 6522 2c0a  -mod-editMode",.
+00001150: 2020 2020 2020 226b 6579 7322 3a20 5b22        "keys": ["
+00001160: 4163 6365 6c20 3222 5d2c 0a20 2020 2020  Accel 2"],.     
+00001170: 2022 636f 6d6d 616e 6422 3a20 226e 6f74   "command": "not
+00001180: 6562 6f6f 6b3a 6368 616e 6765 2d63 656c  ebook:change-cel
+00001190: 6c2d 746f 2d6d 6172 6b64 6f77 6e22 0a20  l-to-markdown". 
+000011a0: 2020 207d 2c0a 2020 2020 7b0a 2020 2020     },.    {.    
+000011b0: 2020 2273 656c 6563 746f 7222 3a20 222e    "selector": ".
+000011c0: 6a70 2d4e 6f74 6562 6f6f 6b50 616e 656c  jp-NotebookPanel
+000011d0: 5b64 6174 612d 6a70 2d76 696d 2d6d 6f64  [data-jp-vim-mod
+000011e0: 653d 2774 7275 6527 5d20 2e6a 702d 4e6f  e='true'] .jp-No
+000011f0: 7465 626f 6f6b 2e6a 702d 6d6f 642d 6564  tebook.jp-mod-ed
+00001200: 6974 4d6f 6465 222c 0a20 2020 2020 2022  itMode",.      "
+00001210: 6b65 7973 223a 205b 2241 6363 656c 2033  keys": ["Accel 3
+00001220: 225d 2c0a 2020 2020 2020 2263 6f6d 6d61  "],.      "comma
+00001230: 6e64 223a 2022 6e6f 7465 626f 6f6b 3a63  nd": "notebook:c
+00001240: 6861 6e67 652d 6365 6c6c 2d74 6f2d 7261  hange-cell-to-ra
+00001250: 7722 0a20 2020 207d 2c0a 2020 2020 7b0a  w".    },.    {.
+00001260: 2020 2020 2020 2273 656c 6563 746f 7222        "selector"
+00001270: 3a20 222e 6a70 2d4e 6f74 6562 6f6f 6b50  : ".jp-NotebookP
+00001280: 616e 656c 5b64 6174 612d 6a70 2d76 696d  anel[data-jp-vim
+00001290: 2d6d 6f64 653d 2774 7275 6527 5d20 2e6a  -mode='true'] .j
+000012a0: 702d 4e6f 7465 626f 6f6b 2e6a 702d 6d6f  p-Notebook.jp-mo
+000012b0: 642d 6564 6974 4d6f 6465 222c 0a20 2020  d-editMode",.   
+000012c0: 2020 2022 6b65 7973 223a 205b 2243 7472     "keys": ["Ctr
+000012d0: 6c20 4f22 2c20 2247 225d 2c0a 2020 2020  l O", "G"],.    
+000012e0: 2020 2263 6f6d 6d61 6e64 223a 2022 7669    "command": "vi
+000012f0: 6d3a 7365 6c65 6374 2d66 6972 7374 2d63  m:select-first-c
+00001300: 656c 6c22 0a20 2020 207d 2c0a 2020 2020  ell".    },.    
+00001310: 7b0a 2020 2020 2020 2273 656c 6563 746f  {.      "selecto
+00001320: 7222 3a20 222e 6a70 2d4e 6f74 6562 6f6f  r": ".jp-Noteboo
+00001330: 6b50 616e 656c 5b64 6174 612d 6a70 2d76  kPanel[data-jp-v
+00001340: 696d 2d6d 6f64 653d 2774 7275 6527 5d20  im-mode='true'] 
+00001350: 2e6a 702d 4e6f 7465 626f 6f6b 2e6a 702d  .jp-Notebook.jp-
+00001360: 6d6f 642d 6564 6974 4d6f 6465 222c 0a20  mod-editMode",. 
+00001370: 2020 2020 2022 6b65 7973 223a 205b 2243       "keys": ["C
+00001380: 7472 6c20 4f22 2c20 2243 7472 6c20 4722  trl O", "Ctrl G"
+00001390: 5d2c 0a20 2020 2020 2022 636f 6d6d 616e  ],.      "comman
+000013a0: 6422 3a20 2276 696d 3a73 656c 6563 742d  d": "vim:select-
+000013b0: 6c61 7374 2d63 656c 6c22 0a20 2020 207d  last-cell".    }
+000013c0: 2c0a 2020 2020 7b0a 2020 2020 2020 2273  ,.    {.      "s
+000013d0: 656c 6563 746f 7222 3a20 222e 6a70 2d4e  elector": ".jp-N
+000013e0: 6f74 6562 6f6f 6b50 616e 656c 5b64 6174  otebookPanel[dat
+000013f0: 612d 6a70 2d76 696d 2d6d 6f64 653d 2774  a-jp-vim-mode='t
+00001400: 7275 6527 5d20 2e6a 702d 4e6f 7465 626f  rue'] .jp-Notebo
+00001410: 6f6b 3a66 6f63 7573 222c 0a20 2020 2020  ok:focus",.     
+00001420: 2022 6b65 7973 223a 205b 2247 222c 2022   "keys": ["G", "
+00001430: 4722 5d2c 0a20 2020 2020 2022 636f 6d6d  G"],.      "comm
+00001440: 616e 6422 3a20 2276 696d 3a73 656c 6563  and": "vim:selec
+00001450: 742d 6669 7273 742d 6365 6c6c 220a 2020  t-first-cell".  
+00001460: 2020 7d2c 0a20 2020 207b 0a20 2020 2020    },.    {.     
+00001470: 2022 7365 6c65 6374 6f72 223a 2022 2e6a   "selector": ".j
+00001480: 702d 4e6f 7465 626f 6f6b 5061 6e65 6c5b  p-NotebookPanel[
+00001490: 6461 7461 2d6a 702d 7669 6d2d 6d6f 6465  data-jp-vim-mode
+000014a0: 3d27 7472 7565 275d 202e 6a70 2d4e 6f74  ='true'] .jp-Not
+000014b0: 6562 6f6f 6b3a 666f 6375 7322 2c0a 2020  ebook:focus",.  
+000014c0: 2020 2020 226b 6579 7322 3a20 5b22 5368      "keys": ["Sh
+000014d0: 6966 7420 4722 5d2c 0a20 2020 2020 2022  ift G"],.      "
+000014e0: 636f 6d6d 616e 6422 3a20 2276 696d 3a73  command": "vim:s
+000014f0: 656c 6563 742d 6c61 7374 2d63 656c 6c22  elect-last-cell"
+00001500: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
+00001510: 2020 2020 2273 656c 6563 746f 7222 3a20      "selector": 
+00001520: 222e 6a70 2d4e 6f74 6562 6f6f 6b50 616e  ".jp-NotebookPan
+00001530: 656c 5b64 6174 612d 6a70 2d76 696d 2d6d  el[data-jp-vim-m
+00001540: 6f64 653d 2774 7275 6527 5d20 2e6a 702d  ode='true'] .jp-
+00001550: 4e6f 7465 626f 6f6b 3a66 6f63 7573 222c  Notebook:focus",
+00001560: 0a20 2020 2020 2022 6b65 7973 223a 205b  .      "keys": [
+00001570: 2259 222c 2022 5922 5d2c 0a20 2020 2020  "Y", "Y"],.     
+00001580: 2022 636f 6d6d 616e 6422 3a20 226e 6f74   "command": "not
+00001590: 6562 6f6f 6b3a 636f 7079 2d63 656c 6c22  ebook:copy-cell"
+000015a0: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
+000015b0: 2020 2020 2263 6f6d 6d61 6e64 223a 2022      "command": "
+000015c0: 6e6f 7465 626f 6f6b 3a63 7574 2d63 656c  notebook:cut-cel
+000015d0: 6c22 2c0a 2020 2020 2020 226b 6579 7322  l",.      "keys"
+000015e0: 3a20 5b22 4422 2c20 2244 225d 2c0a 2020  : ["D", "D"],.  
+000015f0: 2020 2020 2273 656c 6563 746f 7222 3a20      "selector": 
+00001600: 222e 6a70 2d4e 6f74 6562 6f6f 6b50 616e  ".jp-NotebookPan
+00001610: 656c 5b64 6174 612d 6a70 2d76 696d 2d6d  el[data-jp-vim-m
+00001620: 6f64 653d 2774 7275 6527 5d20 2e6a 702d  ode='true'] .jp-
+00001630: 4e6f 7465 626f 6f6b 3a66 6f63 7573 220a  Notebook:focus".
+00001640: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
+00001650: 2020 2022 7365 6c65 6374 6f72 223a 2022     "selector": "
+00001660: 2e6a 702d 4e6f 7465 626f 6f6b 5061 6e65  .jp-NotebookPane
+00001670: 6c5b 6461 7461 2d6a 702d 7669 6d2d 6d6f  l[data-jp-vim-mo
+00001680: 6465 3d27 7472 7565 275d 202e 6a70 2d4e  de='true'] .jp-N
+00001690: 6f74 6562 6f6f 6b3a 666f 6375 7322 2c0a  otebook:focus",.
+000016a0: 2020 2020 2020 226b 6579 7322 3a20 5b22        "keys": ["
+000016b0: 5368 6966 7420 5022 5d2c 0a20 2020 2020  Shift P"],.     
+000016c0: 2022 636f 6d6d 616e 6422 3a20 226e 6f74   "command": "not
+000016d0: 6562 6f6f 6b3a 7061 7374 652d 6365 6c6c  ebook:paste-cell
+000016e0: 2d61 626f 7665 220a 2020 2020 7d2c 0a20  -above".    },. 
+000016f0: 2020 207b 0a20 2020 2020 2022 7365 6c65     {.      "sele
+00001700: 6374 6f72 223a 2022 2e6a 702d 4e6f 7465  ctor": ".jp-Note
+00001710: 626f 6f6b 5061 6e65 6c5b 6461 7461 2d6a  bookPanel[data-j
+00001720: 702d 7669 6d2d 6d6f 6465 3d27 7472 7565  p-vim-mode='true
+00001730: 275d 202e 6a70 2d4e 6f74 6562 6f6f 6b3a  '] .jp-Notebook:
+00001740: 666f 6375 7322 2c0a 2020 2020 2020 226b  focus",.      "k
+00001750: 6579 7322 3a20 5b22 5022 5d2c 0a20 2020  eys": ["P"],.   
+00001760: 2020 2022 636f 6d6d 616e 6422 3a20 226e     "command": "n
+00001770: 6f74 6562 6f6f 6b3a 7061 7374 652d 6365  otebook:paste-ce
+00001780: 6c6c 2d62 656c 6f77 220a 2020 2020 7d2c  ll-below".    },
+00001790: 0a20 2020 207b 0a20 2020 2020 2022 7365  .    {.      "se
+000017a0: 6c65 6374 6f72 223a 2022 2e6a 702d 4e6f  lector": ".jp-No
+000017b0: 7465 626f 6f6b 5061 6e65 6c5b 6461 7461  tebookPanel[data
+000017c0: 2d6a 702d 7669 6d2d 6d6f 6465 3d27 7472  -jp-vim-mode='tr
+000017d0: 7565 275d 202e 6a70 2d4e 6f74 6562 6f6f  ue'] .jp-Noteboo
+000017e0: 6b3a 666f 6375 7322 2c0a 2020 2020 2020  k:focus",.      
+000017f0: 226b 6579 7322 3a20 5b22 4f22 5d2c 0a20  "keys": ["O"],. 
+00001800: 2020 2020 2022 636f 6d6d 616e 6422 3a20       "command": 
+00001810: 226e 6f74 6562 6f6f 6b3a 696e 7365 7274  "notebook:insert
+00001820: 2d63 656c 6c2d 6265 6c6f 7722 0a20 2020  -cell-below".   
+00001830: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
+00001840: 2273 656c 6563 746f 7222 3a20 222e 6a70  "selector": ".jp
+00001850: 2d4e 6f74 6562 6f6f 6b50 616e 656c 5b64  -NotebookPanel[d
+00001860: 6174 612d 6a70 2d76 696d 2d6d 6f64 653d  ata-jp-vim-mode=
+00001870: 2774 7275 6527 5d20 2e6a 702d 4e6f 7465  'true'] .jp-Note
+00001880: 626f 6f6b 3a66 6f63 7573 222c 0a20 2020  book:focus",.   
+00001890: 2020 2022 6b65 7973 223a 205b 2253 6869     "keys": ["Shi
+000018a0: 6674 204f 225d 2c0a 2020 2020 2020 2263  ft O"],.      "c
+000018b0: 6f6d 6d61 6e64 223a 2022 6e6f 7465 626f  ommand": "notebo
+000018c0: 6f6b 3a69 6e73 6572 742d 6365 6c6c 2d61  ok:insert-cell-a
+000018d0: 626f 7665 220a 2020 2020 7d2c 0a20 2020  bove".    },.   
+000018e0: 207b 0a20 2020 2020 2022 7365 6c65 6374   {.      "select
+000018f0: 6f72 223a 2022 2e6a 702d 4e6f 7465 626f  or": ".jp-Notebo
+00001900: 6f6b 5061 6e65 6c5b 6461 7461 2d6a 702d  okPanel[data-jp-
+00001910: 7669 6d2d 6d6f 6465 3d27 7472 7565 275d  vim-mode='true']
+00001920: 202e 6a70 2d4e 6f74 6562 6f6f 6b3a 666f   .jp-Notebook:fo
+00001930: 6375 7322 2c0a 2020 2020 2020 226b 6579  cus",.      "key
+00001940: 7322 3a20 5b22 5522 5d2c 0a20 2020 2020  s": ["U"],.     
+00001950: 2022 636f 6d6d 616e 6422 3a20 226e 6f74   "command": "not
+00001960: 6562 6f6f 6b3a 756e 646f 2d63 656c 6c2d  ebook:undo-cell-
+00001970: 6163 7469 6f6e 220a 2020 2020 7d2c 0a20  action".    },. 
+00001980: 2020 207b 0a20 2020 2020 2022 7365 6c65     {.      "sele
+00001990: 6374 6f72 223a 2022 2e6a 702d 4e6f 7465  ctor": ".jp-Note
+000019a0: 626f 6f6b 5061 6e65 6c5b 6461 7461 2d6a  bookPanel[data-j
+000019b0: 702d 7669 6d2d 6d6f 6465 3d27 7472 7565  p-vim-mode='true
+000019c0: 275d 202e 6a70 2d4e 6f74 6562 6f6f 6b3a  '] .jp-Notebook:
+000019d0: 666f 6375 7322 2c0a 2020 2020 2020 226b  focus",.      "k
+000019e0: 6579 7322 3a20 5b22 4374 726c 2045 225d  eys": ["Ctrl E"]
+000019f0: 2c0a 2020 2020 2020 2263 6f6d 6d61 6e64  ,.      "command
+00001a00: 223a 2022 6e6f 7465 626f 6f6b 3a6d 6f76  ": "notebook:mov
+00001a10: 652d 6365 6c6c 2d64 6f77 6e22 0a20 2020  e-cell-down".   
+00001a20: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
+00001a30: 2273 656c 6563 746f 7222 3a20 222e 6a70  "selector": ".jp
+00001a40: 2d4e 6f74 6562 6f6f 6b50 616e 656c 5b64  -NotebookPanel[d
+00001a50: 6174 612d 6a70 2d76 696d 2d6d 6f64 653d  ata-jp-vim-mode=
+00001a60: 2774 7275 6527 5d20 2e6a 702d 4e6f 7465  'true'] .jp-Note
+00001a70: 626f 6f6b 3a66 6f63 7573 222c 0a20 2020  book:focus",.   
+00001a80: 2020 2022 6b65 7973 223a 205b 2243 7472     "keys": ["Ctr
+00001a90: 6c20 5922 5d2c 0a20 2020 2020 2022 636f  l Y"],.      "co
+00001aa0: 6d6d 616e 6422 3a20 226e 6f74 6562 6f6f  mmand": "noteboo
+00001ab0: 6b3a 6d6f 7665 2d63 656c 6c2d 7570 220a  k:move-cell-up".
+00001ac0: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
+00001ad0: 2020 2022 7365 6c65 6374 6f72 223a 2022     "selector": "
+00001ae0: 2e6a 702d 4e6f 7465 626f 6f6b 5061 6e65  .jp-NotebookPane
+00001af0: 6c5b 6461 7461 2d6a 702d 7669 6d2d 6d6f  l[data-jp-vim-mo
+00001b00: 6465 3d27 7472 7565 275d 202e 6a70 2d4e  de='true'] .jp-N
+00001b10: 6f74 6562 6f6f 6b3a 666f 6375 7322 2c0a  otebook:focus",.
+00001b20: 2020 2020 2020 226b 6579 7322 3a20 5b22        "keys": ["
+00001b30: 5a22 2c20 225a 225d 2c0a 2020 2020 2020  Z", "Z"],.      
+00001b40: 2263 6f6d 6d61 6e64 223a 2022 7669 6d3a  "command": "vim:
+00001b50: 6365 6e74 6572 2d63 656c 6c22 0a20 2020  center-cell".   
+00001b60: 207d 2c0a 2020 2020 7b0a 2020 2020 2020   },.    {.      
+00001b70: 2273 656c 6563 746f 7222 3a20 222e 6a70  "selector": ".jp
+00001b80: 2d4e 6f74 6562 6f6f 6b50 616e 656c 5b64  -NotebookPanel[d
+00001b90: 6174 612d 6a70 2d76 696d 2d6d 6f64 653d  ata-jp-vim-mode=
+00001ba0: 2774 7275 6527 5d20 2e6a 702d 4e6f 7465  'true'] .jp-Note
+00001bb0: 626f 6f6b 3a66 6f63 7573 222c 0a20 2020  book:focus",.   
+00001bc0: 2020 2022 6b65 7973 223a 205b 225a 222c     "keys": ["Z",
+00001bd0: 2022 4322 5d2c 0a20 2020 2020 2022 636f   "C"],.      "co
+00001be0: 6d6d 616e 6422 3a20 226e 6f74 6562 6f6f  mmand": "noteboo
+00001bf0: 6b3a 6869 6465 2d63 656c 6c2d 636f 6465  k:hide-cell-code
+00001c00: 220a 2020 2020 7d2c 0a20 2020 207b 0a20  ".    },.    {. 
+00001c10: 2020 2020 2022 7365 6c65 6374 6f72 223a       "selector":
+00001c20: 2022 2e6a 702d 4e6f 7465 626f 6f6b 5061   ".jp-NotebookPa
+00001c30: 6e65 6c5b 6461 7461 2d6a 702d 7669 6d2d  nel[data-jp-vim-
+00001c40: 6d6f 6465 3d27 7472 7565 275d 202e 6a70  mode='true'] .jp
+00001c50: 2d4e 6f74 6562 6f6f 6b3a 666f 6375 7322  -Notebook:focus"
+00001c60: 2c0a 2020 2020 2020 226b 6579 7322 3a20  ,.      "keys": 
+00001c70: 5b22 5a22 2c20 224f 225d 2c0a 2020 2020  ["Z", "O"],.    
+00001c80: 2020 2263 6f6d 6d61 6e64 223a 2022 6e6f    "command": "no
+00001c90: 7465 626f 6f6b 3a73 686f 772d 6365 6c6c  tebook:show-cell
+00001ca0: 2d63 6f64 6522 0a20 2020 207d 2c0a 2020  -code".    },.  
+00001cb0: 2020 7b0a 2020 2020 2020 2273 656c 6563    {.      "selec
+00001cc0: 746f 7222 3a20 222e 6a70 2d4e 6f74 6562  tor": ".jp-Noteb
+00001cd0: 6f6f 6b50 616e 656c 5b64 6174 612d 6a70  ookPanel[data-jp
+00001ce0: 2d76 696d 2d6d 6f64 653d 2774 7275 6527  -vim-mode='true'
+00001cf0: 5d20 2e6a 702d 4e6f 7465 626f 6f6b 3a66  ] .jp-Notebook:f
+00001d00: 6f63 7573 222c 0a20 2020 2020 2022 6b65  ocus",.      "ke
+00001d10: 7973 223a 205b 225a 222c 2022 4d22 5d2c  ys": ["Z", "M"],
+00001d20: 0a20 2020 2020 2022 636f 6d6d 616e 6422  .      "command"
+00001d30: 3a20 226e 6f74 6562 6f6f 6b3a 6869 6465  : "notebook:hide
+00001d40: 2d61 6c6c 2d63 656c 6c2d 636f 6465 220a  -all-cell-code".
+00001d50: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
+00001d60: 2020 2022 7365 6c65 6374 6f72 223a 2022     "selector": "
+00001d70: 2e6a 702d 4e6f 7465 626f 6f6b 5061 6e65  .jp-NotebookPane
+00001d80: 6c5b 6461 7461 2d6a 702d 7669 6d2d 6d6f  l[data-jp-vim-mo
+00001d90: 6465 3d27 7472 7565 275d 202e 6a70 2d4e  de='true'] .jp-N
+00001da0: 6f74 6562 6f6f 6b3a 666f 6375 7322 2c0a  otebook:focus",.
+00001db0: 2020 2020 2020 226b 6579 7322 3a20 5b22        "keys": ["
+00001dc0: 5a22 2c20 2252 225d 2c0a 2020 2020 2020  Z", "R"],.      
+00001dd0: 2263 6f6d 6d61 6e64 223a 2022 6e6f 7465  "command": "note
+00001de0: 626f 6f6b 3a73 686f 772d 616c 6c2d 6365  book:show-all-ce
+00001df0: 6c6c 2d63 6f64 6522 0a20 2020 207d 2c0a  ll-code".    },.
+00001e00: 2020 2020 7b0a 2020 2020 2020 2273 656c      {.      "sel
+00001e10: 6563 746f 7222 3a20 222e 6a70 2d4e 6f74  ector": ".jp-Not
+00001e20: 6562 6f6f 6b50 616e 656c 5b64 6174 612d  ebookPanel[data-
+00001e30: 6a70 2d76 696d 2d6d 6f64 653d 2774 7275  jp-vim-mode='tru
+00001e40: 6527 5d20 2e6a 702d 4e6f 7465 626f 6f6b  e'] .jp-Notebook
+00001e50: 2e6a 702d 6d6f 642d 6564 6974 4d6f 6465  .jp-mod-editMode
+00001e60: 222c 0a20 2020 2020 2022 6b65 7973 223a  ",.      "keys":
+00001e70: 205b 2243 7472 6c20 4f22 2c20 225a 222c   ["Ctrl O", "Z",
+00001e80: 2022 5a22 5d2c 0a20 2020 2020 2022 636f   "Z"],.      "co
+00001e90: 6d6d 616e 6422 3a20 2276 696d 3a63 656e  mmand": "vim:cen
+00001ea0: 7465 722d 6365 6c6c 220a 2020 2020 7d2c  ter-cell".    },
+00001eb0: 0a20 2020 207b 0a20 2020 2020 2022 7365  .    {.      "se
+00001ec0: 6c65 6374 6f72 223a 2022 2e6a 702d 4e6f  lector": ".jp-No
+00001ed0: 7465 626f 6f6b 5061 6e65 6c5b 6461 7461  tebookPanel[data
+00001ee0: 2d6a 702d 7669 6d2d 6d6f 6465 3d27 7472  -jp-vim-mode='tr
+00001ef0: 7565 275d 202e 6a70 2d4e 6f74 6562 6f6f  ue'] .jp-Noteboo
+00001f00: 6b2e 6a70 2d6d 6f64 2d65 6469 744d 6f64  k.jp-mod-editMod
+00001f10: 6520 2e6a 702d 496e 7075 7441 7265 612d  e .jp-InputArea-
+00001f20: 6564 6974 6f72 3a6e 6f74 282e 6a70 2d6d  editor:not(.jp-m
+00001f30: 6f64 2d68 6173 2d70 7269 6d61 7279 2d73  od-has-primary-s
+00001f40: 656c 6563 7469 6f6e 2922 2c0a 2020 2020  election)",.    
+00001f50: 2020 226b 6579 7322 3a20 5b22 4374 726c    "keys": ["Ctrl
+00001f60: 2047 225d 2c0a 2020 2020 2020 2263 6f6d   G"],.      "com
+00001f70: 6d61 6e64 223a 2022 746f 6f6c 7469 703a  mand": "tooltip:
+00001f80: 6c61 756e 6368 2d6e 6f74 6562 6f6f 6b22  launch-notebook"
+00001f90: 0a20 2020 207d 0a20 205d 2c0a 2020 226a  .    }.  ],.  "j
+00001fa0: 7570 7974 6572 2e6c 6162 2e6d 656e 7573  upyter.lab.menus
+00001fb0: 223a 207b 0a20 2020 2022 6d61 696e 223a  ": {.    "main":
+00001fc0: 205b 0a20 2020 2020 207b 0a20 2020 2020   [.      {.     
+00001fd0: 2020 2022 6964 223a 2022 6a70 2d6d 6169     "id": "jp-mai
+00001fe0: 6e6d 656e 752d 7365 7474 696e 6773 222c  nmenu-settings",
+00001ff0: 0a20 2020 2020 2020 2022 6974 656d 7322  .        "items"
+00002000: 3a20 5b0a 2020 2020 2020 2020 2020 7b0a  : [.          {.
+00002010: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00002020: 6522 3a20 2273 6570 6172 6174 6f72 222c  e": "separator",
+00002030: 0a20 2020 2020 2020 2020 2020 2022 7261  .            "ra
+00002040: 6e6b 223a 2033 380a 2020 2020 2020 2020  nk": 38.        
+00002050: 2020 7d2c 0a20 2020 2020 2020 2020 207b    },.          {
+00002060: 0a20 2020 2020 2020 2020 2020 2022 636f  .            "co
+00002070: 6d6d 616e 6422 3a20 226a 7570 7974 6572  mmand": "jupyter
+00002080: 6c61 622d 7669 6d3a 746f 6767 6c65 222c  lab-vim:toggle",
+00002090: 0a20 2020 2020 2020 2020 2020 2022 7261  .            "ra
+000020a0: 6e6b 223a 2033 380a 2020 2020 2020 2020  nk": 38.        
+000020b0: 2020 7d2c 0a20 2020 2020 2020 2020 207b    },.          {
+000020c0: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
+000020d0: 7065 223a 2022 7365 7061 7261 746f 7222  pe": "separator"
+000020e0: 2c0a 2020 2020 2020 2020 2020 2020 2272  ,.            "r
+000020f0: 616e 6b22 3a20 3338 0a20 2020 2020 2020  ank": 38.       
+00002100: 2020 207d 0a20 2020 2020 2020 205d 0a20     }.        ]. 
+00002110: 2020 2020 207d 0a20 2020 205d 0a20 207d       }.    ].  }
+00002120: 2c0a 2020 2270 726f 7065 7274 6965 7322  ,.  "properties"
+00002130: 3a20 7b0a 2020 2020 2265 6e61 626c 6564  : {.    "enabled
+00002140: 223a 207b 0a20 2020 2020 2022 7479 7065  ": {.      "type
+00002150: 223a 2022 626f 6f6c 6561 6e22 2c0a 2020  ": "boolean",.  
+00002160: 2020 2020 2274 6974 6c65 223a 2022 456e      "title": "En
+00002170: 6162 6c65 6422 2c0a 2020 2020 2020 2264  abled",.      "d
+00002180: 6573 6372 6970 7469 6f6e 223a 2022 456e  escription": "En
+00002190: 6162 6c65 2f64 6973 6162 6c65 206e 6f74  able/disable not
+000021a0: 6562 6f6f 6b20 7669 6d20 286d 6179 2072  ebook vim (may r
+000021b0: 6571 7569 7265 2061 2070 6167 6520 7265  equire a page re
+000021c0: 6672 6573 6829 222c 0a20 2020 2020 2022  fresh)",.      "
+000021d0: 6465 6661 756c 7422 3a20 7472 7565 0a20  default": true. 
+000021e0: 2020 207d 2c0a 2020 2020 2265 7874 7261     },.    "extra
+000021f0: 4b65 7962 696e 6469 6e67 7322 3a20 7b0a  Keybindings": {.
+00002200: 2020 2020 2020 2274 7970 6522 3a20 2261        "type": "a
+00002210: 7272 6179 222c 0a20 2020 2020 2022 7469  rray",.      "ti
+00002220: 746c 6522 3a20 2245 7874 7261 2056 696d  tle": "Extra Vim
+00002230: 204b 6579 6269 6e64 696e 6773 222c 0a20   Keybindings",. 
+00002240: 2020 2020 2022 6974 656d 7322 3a20 7b0a       "items": {.
+00002250: 2020 2020 2020 2020 2224 7265 6622 3a20          "$ref": 
+00002260: 2223 2f64 6566 696e 6974 696f 6e73 2f73  "#/definitions/s
+00002270: 686f 7274 6375 7422 0a20 2020 2020 207d  hortcut".      }
+00002280: 2c0a 2020 2020 2020 2264 6566 6175 6c74  ,.      "default
+00002290: 223a 205b 5d0a 2020 2020 7d0a 2020 7d2c  ": [].    }.  },
+000022a0: 0a20 2022 6465 6669 6e69 7469 6f6e 7322  .  "definitions"
+000022b0: 3a20 7b0a 2020 2020 2273 686f 7274 6375  : {.    "shortcu
+000022c0: 7422 3a20 7b0a 2020 2020 2020 2270 726f  t": {.      "pro
+000022d0: 7065 7274 6965 7322 3a20 7b0a 2020 2020  perties": {.    
+000022e0: 2020 2020 2263 6f6d 6d61 6e64 223a 207b      "command": {
+000022f0: 0a20 2020 2020 2020 2020 2022 7469 746c  .          "titl
+00002300: 6522 3a20 224b 6579 6269 6e64 696e 6722  e": "Keybinding"
+00002310: 2c0a 2020 2020 2020 2020 2020 2264 6573  ,.          "des
+00002320: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
+00002330: 6e65 7720 7669 6d20 6b65 7962 696e 6469  new vim keybindi
+00002340: 6e67 2c20 6f72 2027 6c65 6674 2068 616e  ng, or 'left han
+00002350: 6420 7369 6465 2720 6f66 2074 6865 206b  d side' of the k
+00002360: 6579 6269 6e64 696e 672c 2065 2e67 2e20  eybinding, e.g. 
+00002370: 604d 6022 2c0a 2020 2020 2020 2020 2020  `M`",.          
+00002380: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
+00002390: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+000023a0: 2020 2020 226b 6579 7322 3a20 7b0a 2020      "keys": {.  
+000023b0: 2020 2020 2020 2020 2274 6974 6c65 223a          "title":
+000023c0: 2022 5468 6520 6b65 7920 7365 7175 656e   "The key sequen
+000023d0: 6365 2074 6f20 6578 6563 7574 6522 2c0a  ce to execute",.
+000023e0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+000023f0: 6970 7469 6f6e 223a 2022 5468 6520 2772  iption": "The 'r
+00002400: 6967 6874 2068 616e 6420 7369 6465 2720  ight hand side' 
+00002410: 6f66 2074 6865 206b 6579 6269 6e64 696e  of the keybindin
+00002420: 6720 746f 2062 6520 6578 6563 7574 6564  g to be executed
+00002430: 2c20 652e 672e 2060 3a6e 6f68 3c63 723e  , e.g. `:noh<cr>
+00002440: 6022 2c0a 2020 2020 2020 2020 2020 2274  `",.          "t
+00002450: 7970 6522 3a20 2273 7472 696e 6722 0a20  ype": "string". 
+00002460: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00002470: 2020 2263 6f6e 7465 7874 223a 207b 0a20    "context": {. 
+00002480: 2020 2020 2020 2020 2022 7469 746c 6522           "title"
+00002490: 3a20 224d 6f64 6522 2c0a 2020 2020 2020  : "Mode",.      
+000024a0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+000024b0: 223a 2022 5669 6d20 6d6f 6465 2069 6e20  ": "Vim mode in 
+000024c0: 7768 6963 6820 7468 6520 6b65 7962 696e  which the keybin
+000024d0: 6469 6e67 2061 7070 6c69 6573 222c 0a20  ding applies",. 
+000024e0: 2020 2020 2020 2020 2022 656e 756d 223a           "enum":
+000024f0: 205b 226e 6f72 6d61 6c22 2c20 2269 6e73   ["normal", "ins
+00002500: 6572 7422 2c20 2276 6973 7561 6c22 5d2c  ert", "visual"],
+00002510: 0a20 2020 2020 2020 2020 2022 6465 6661  .          "defa
+00002520: 756c 7422 3a20 226e 6f72 6d61 6c22 0a20  ult": "normal". 
+00002530: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00002540: 2020 226d 6170 666e 223a 207b 0a20 2020    "mapfn": {.   
+00002550: 2020 2020 2020 2022 7469 746c 6522 3a20         "title": 
+00002560: 224d 6170 2066 756e 6374 696f 6e22 2c0a  "Map function",.
+00002570: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00002580: 6970 7469 6f6e 223a 2022 5669 6d20 6d61  iption": "Vim ma
+00002590: 7020 6675 6e63 7469 6f6e 2074 6f20 7573  p function to us
+000025a0: 6522 2c0a 2020 2020 2020 2020 2020 2265  e",.          "e
+000025b0: 6e75 6d22 3a20 5b22 6d61 7022 2c20 226e  num": ["map", "n
+000025c0: 6f72 656d 6170 225d 2c0a 2020 2020 2020  oremap"],.      
+000025d0: 2020 2020 2264 6566 6175 6c74 223a 2022      "default": "
+000025e0: 6d61 7022 0a20 2020 2020 2020 207d 2c0a  map".        },.
+000025f0: 2020 2020 2020 2020 2265 6e61 626c 6564          "enabled
+00002600: 223a 207b 0a20 2020 2020 2020 2020 2022  ": {.          "
+00002610: 6465 7363 7269 7074 696f 6e22 3a20 2257  description": "W
+00002620: 6865 7468 6572 2074 6869 7320 6b65 7962  hether this keyb
+00002630: 696e 6469 6e67 2069 7320 656e 6162 6c65  inding is enable
+00002640: 6420 6f72 206e 6f74 2e22 2c0a 2020 2020  d or not.",.    
+00002650: 2020 2020 2020 2274 7970 6522 3a20 2262        "type": "b
+00002660: 6f6f 6c65 616e 222c 0a20 2020 2020 2020  oolean",.       
+00002670: 2020 2022 6465 6661 756c 7422 3a20 7472     "default": tr
+00002680: 7565 0a20 2020 2020 2020 207d 0a20 2020  ue.        }.   
+00002690: 2020 207d 2c0a 2020 2020 2020 2272 6571     },.      "req
+000026a0: 7569 7265 6422 3a20 5b22 636f 6d6d 616e  uired": ["comman
+000026b0: 6422 2c20 226b 6579 7322 5d2c 0a20 2020  d", "keys"],.   
+000026c0: 2020 2022 7479 7065 223a 2022 6f62 6a65     "type": "obje
+000026d0: 6374 220a 2020 2020 7d0a 2020 7d0a 7d0a  ct".    }.  }.}.
```

### Comparing `jupyterlab_vim-0.16.0/jupyterlab_vim/labextension/static/830.29023cea9c147059457e.js` & `jupyterlab_vim-0.17.0/jupyterlab_vim/labextension/static/353.184fc74aa8db790efd40.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,367 +1,391 @@
+"use strict";
 (self.webpackChunk_axlair_jupyterlab_vim = self.webpackChunk_axlair_jupyterlab_vim || []).push([
-    [830], {
-        830: (e, t, n) => {
-            "use strict";
-            n.r(t), n.d(t, {
-                default: () => u
+    [353], {
+        353: (e, t, o) => {
+            o.r(t), o.d(t, {
+                default: () => v
             });
-            var o = n(767),
-                l = n(346),
-                i = n(598);
-            const a = !!navigator.platform.match(/Mac/i);
-            class c {
+            var n = o(861),
+                l = o(408),
+                i = o(663),
+                a = o(829),
+                c = o(211),
+                d = o(204);
+            class s {
                 constructor({
                     commands: e,
-                    cm: t,
-                    enabled: n,
+                    enabled: t,
                     userKeybindings: o
                 }) {
-                    this._commands = e, this._cm = t, this.enabled = n, this.lastActiveCell = null, this.userKeybindings = null != o ? o : []
+                    this._commands = e, this.enabled = t, this.lastActiveCell = null, this.userKeybindings = null != o ? o : []
                 }
                 onActiveCellChanged(e, t) {
-                    this.modifyCell(t)
+                    this.modifyCell(t).catch(console.error)
                 }
-                modifyCell(e) {
+                async modifyCell(e) {
                     if (!e) return;
-                    this.lastActiveCell = e;
+                    this.lastActiveCell = e, await e.ready;
                     const t = e.editor;
+                    if (e.isDisposed) return void console.warn("Cell was already disposed, cannot setup vim mode");
+                    if (!t) throw Error("Cell editor not available");
+                    const o = t.editor;
                     if (this.enabled) {
-                        t.setOption("keyMap", "vim");
-                        const n = t.getOption("extraKeys") || {};
-                        n.Esc = this._cm.prototype.leaveInsertMode, a || (n["Ctrl-C"] = !1), this._cm.prototype.save = () => {
-                            this._commands.execute("docmanager:save")
-                        }, t.setOption("extraKeys", n);
-                        const o = this._cm.Vim;
-                        ["normal", "visual", "insert"].forEach((e => o.mapclear(e))), this.userKeybindings.forEach((({
+                        if (!t.getOption("vim")) {
+                            t.setOption("vim", !0);
+                            const e = (0, a.getCM)(o);
+                            t.hasFocus = () => !(!e.state.dialog || !e.state.dialog.contains(document.activeElement)) || o.hasFocus
+                        }
+                        const n = (0, a.getCM)(o),
+                            l = a.Vim;
+                        ["normal", "visual", "insert"].forEach((e => l.mapclear(e))), this.userKeybindings.forEach((({
                             command: e,
                             keys: t,
-                            context: n,
-                            mapfn: l,
+                            context: o,
+                            mapfn: n,
                             enabled: i
                         }) => {
-                            i && ("map" === l ? o.map(e, t, n) : o.noremap(e, t, n))
-                        })), o.defineEx("quit", "q", (e => {
-                            this._commands.execute("notebook:enter-command-mode")
-                        })), this._cm.Vim.handleKey(t.editor, "<Esc>");
-                        const l = (t, n, o, i) => {
-                            const a = n;
-                            let c = a.ch;
-                            const d = e;
-                            switch (null == i ? void 0 : i.lastMotion) {
+                            i && ("map" === n ? l.map(e, t, o) : l.noremap(e, t, o))
+                        })), a.Vim.handleKey(n, "<Esc>");
+                        const i = (t, n, l, c) => {
+                            const d = n;
+                            let s = d.ch;
+                            const r = e;
+                            switch (null == c ? void 0 : c.lastMotion) {
                                 case t.moveByLines:
                                 case t.moveByDisplayLines:
                                 case t.moveByScroll:
                                 case t.moveToColumn:
                                 case t.moveToEol:
-                                case l:
-                                    c = i.lastHPos;
+                                case i:
+                                    s = c.lastHPos;
                                     break;
                                 default:
-                                    i.lastHPos = c
+                                    c.lastHPos = s
                             }
-                            const s = o.repeat + (o.repeatOffset || 0);
-                            let m = o.forward ? a.line + s : a.line - s;
-                            const r = t.firstLine(),
-                                u = t.lastLine(),
-                                C = t.findPosV(a, o.forward ? s : -s, "line", i.lastHSPos);
-                            if ((o.forward ? C.line > m : C.line < m) && (m = C.line, c = C.ch), !(m < r || m > u)) return o.toFirstChar && (c = function(e) {
+                            const m = l.repeat + (l.repeatOffset || 0);
+                            let u = l.forward ? d.line + m : d.line - m;
+                            const C = t.firstLine(),
+                                v = t.lastLine(),
+                                b = t.findPosV(d, l.forward ? m : -m, "line", c.lastHSPos);
+                            if ((l.forward ? b.line > u : b.line < u) && (u = b.line, s = b.ch), !(u < C || u > v)) return l.toFirstChar && (s = function(e) {
                                 if (!e) return 0;
                                 const t = e.search(/\S/);
                                 return -1 === t ? e.length : t
-                            }(t.getLine(m)), i.lastHPos = c), i.lastHSPos = t.charCoords(this._cm.Pos(m, c), "div").left, this._cm.Pos(m, c);
-                            if (null !== d && "markdown" === d.model.type && (o.handleArrow || (d.rendered = !0)), o.forward)
-                                if (o.handleArrow) {
+                            }(t.getLine(u)), c.lastHPos = s), c.lastHSPos = t.charCoords(new a.CodeMirror.Pos(u, s), "div").left, new a.CodeMirror.Pos(u, s);
+                            if (null !== r && "markdown" === r.model.type && (l.handleArrow || (r.rendered = !0)), l.forward)
+                                if (l.handleArrow) {
                                     const e = t.getCursor(),
-                                        n = t.doc.getLine(u).length;
-                                    e.line === u && e.ch === n || (t.setCursor({
-                                        line: u,
-                                        ch: n
-                                    }), this._commands.execute("notebook:move-cursor-down"))
+                                        n = o.state.doc.line(v + 1).length;
+                                    e.line === v && e.ch === n || (t.setCursor(v, n), this._commands.execute("notebook:move-cursor-down"))
                                 } else this._commands.execute("notebook:move-cursor-down");
-                            else if (o.handleArrow) {
+                            else if (l.handleArrow) {
                                 const e = t.getCursor();
-                                0 === e.line && 0 === e.ch || (t.setCursor({
-                                    line: 0,
-                                    ch: 0
-                                }), this._commands.execute("notebook:move-cursor-up"))
+                                0 === e.line && 0 === e.ch || (t.setCursor(0, 0), this._commands.execute("notebook:move-cursor-up"))
                             } else this._commands.execute("notebook:move-cursor-up")
                         };
-                        o.defineMotion("moveByLinesOrCell", l), o.mapCommand("<Up>", "motion", "moveByLinesOrCell", {
+                        l.defineMotion("moveByLinesOrCell", i), l.mapCommand("<Up>", "motion", "moveByLinesOrCell", {
                             forward: !1,
                             linewise: !0,
                             handleArrow: !0
                         }, {
                             context: "normal"
-                        }), o.mapCommand("<Down>", "motion", "moveByLinesOrCell", {
+                        }), l.mapCommand("<Down>", "motion", "moveByLinesOrCell", {
                             forward: !0,
                             linewise: !0,
                             handleArrow: !0
                         }, {
                             context: "normal"
-                        }), o.mapCommand("k", "motion", "moveByLinesOrCell", {
+                        }), l.mapCommand("k", "motion", "moveByLinesOrCell", {
                             forward: !1,
                             linewise: !0
                         }, {
                             context: "normal"
-                        }), o.mapCommand("j", "motion", "moveByLinesOrCell", {
+                        }), l.mapCommand("j", "motion", "moveByLinesOrCell", {
                             forward: !0,
                             linewise: !0
                         }, {
                             context: "normal"
-                        }), o.defineAction("moveCellDown", ((e, t) => {
+                        }), l.defineAction("moveCellDown", ((e, t) => {
                             this._commands.execute("notebook:move-cell-down")
-                        })), o.defineAction("moveCellUp", ((e, t) => {
+                        })), l.defineAction("moveCellUp", ((e, t) => {
                             this._commands.execute("notebook:move-cell-up")
-                        })), o.mapCommand("<C-e>", "action", "moveCellDown", {}, {
+                        })), l.mapCommand("<C-e>", "action", "moveCellDown", {}, {
                             extra: "normal"
-                        }), o.mapCommand("<C-y>", "action", "moveCellUp", {}, {
+                        }), l.mapCommand("<C-y>", "action", "moveCellUp", {}, {
                             extra: "normal"
-                        }), o.defineAction("splitCell", ((e, t) => {
+                        }), l.defineAction("splitCell", ((e, t) => {
                             this._commands.execute("notebook:split-cell-at-cursor")
-                        })), o.mapCommand("-", "action", "splitCell", {}, {
+                        })), l.mapCommand("-", "action", "splitCell", {}, {
                             extra: "normal"
                         })
-                    } else "vim" === t.getOption("keyMap") && t.setOption("keyMap", "default")
+                    } else t.getOption("vim") && t.setOption("vim", !1)
                 }
             }
-            var d = n(520);
-            const s = "@axlair/jupyterlab_vim",
-                m = "jupyterlab-vim:toggle";
-            let r = !1;
-            const u = {
-                id: s,
+            var r = o(593);
+            const m = "@axlair/jupyterlab_vim",
+                u = "jupyterlab-vim:toggle";
+            let C = !1;
+            const v = {
+                id: m,
                 autoStart: !0,
-                activate: async function(e, t, n, l) {
-                    e.commands.addCommand(m, {
+                activate: async function(e, t, o, i) {
+                    const v = d.Prec.highest(c.EditorView.theme({
+                        ".cm-fat-cursor": {
+                            position: "absolute",
+                            background: "var(--jp-vim-cursor-color)",
+                            border: "none",
+                            whiteSpace: "pre"
+                        },
+                        "&:not(.cm-focused) .cm-fat-cursor": {
+                            background: "none",
+                            outline: "solid 1px var(--jp-vim-cursor-color)",
+                            color: "transparent !important"
+                        }
+                    }));
+                    o.addExtension({
+                        name: "vim",
+                        factory: e => l.EditorExtensionRegistry.createConditionalExtension([v, (0, a.vim)({
+                            status: !1
+                        })])
+                    }), e.commands.addCommand(u, {
                         label: "Enable Notebook Vim mode",
                         execute: () => {
-                            l && l.set(`${s}:plugin`, "enabled", !r)
+                            i && i.set(`${m}:plugin`, "enabled", !C)
                         },
-                        isToggled: () => r
+                        isToggled: () => C
                     });
-                    const i = (await l.get(`${s}:plugin`, "extraKeybindings")).composite,
-                        a = n.CodeMirror;
-                    let u = null,
-                        C = null,
-                        v = !1;
-                    async function b(o) {
-                        const i = (await l.get(`${s}:plugin`, "extraKeybindings")).composite;
-                        r = !0 === o.get("enabled").composite, e.commands.notifyCommandChanged(m), u && (u.enabled = r, u.userKeybindings = i), r ? (null == C || C.dispose(), v || (v = !0, await e.restored, await n.ensureVimKeymap())) : C = e.commands.addKeyBinding({
+                    const b = (await i.get(`${m}:plugin`, "extraKeybindings")).composite;
+                    let f = null,
+                        p = null,
+                        w = !1;
+                    async function x(o) {
+                        const n = (await i.get(`${m}:plugin`, "extraKeybindings")).composite;
+                        C = !0 === o.get("enabled").composite, e.commands.notifyCommandChanged(u), f && (f.enabled = C, f.userKeybindings = n), C ? (null == p || p.dispose(), w || (w = !0, await e.restored)) : p = e.commands.addKeyBinding({
                             command: "notebook:enter-command-mode",
                             keys: ["Escape"],
                             selector: ".jp-Notebook.jp-mod-editMode"
                         }), t.forEach((e => {
-                            e.node.dataset.jpVimMode = `${r}`
-                        })), null == u || u.modifyCell(u.lastActiveCell), t.widgetAdded.connect(((e, t) => {
-                            t.node.dataset.jpVimMode = `${r}`
+                            e.node.dataset.jpVimMode = `${C}`
+                        })), null == f || f.modifyCell(f.lastActiveCell), t.widgetAdded.connect(((e, t) => {
+                            t.node.dataset.jpVimMode = `${C}`
                         }))
                     }
-                    return u = new c({
+                    return a.Vim.defineEx("write", "w", (() => {
+                            e.commands.execute("docmanager:save")
+                        })), a.Vim.defineEx("quit", "q", (() => {
+                            setTimeout((() => {
+                                e.commands.execute("notebook:enter-command-mode")
+                            }))
+                        })), f = new s({
                             commands: e.commands,
-                            cm: a,
-                            enabled: r,
-                            userKeybindings: i
-                        }), t.activeCellChanged.connect(u.onActiveCellChanged, u),
-                        function(e, t, n) {
+                            enabled: C,
+                            userKeybindings: b
+                        }), t.activeCellChanged.connect(f.onActiveCellChanged, f),
+                        function(e, t) {
                             const {
-                                commands: l,
-                                shell: i
+                                commands: o,
+                                shell: l
                             } = e;
 
-                            function a(e) {
-                                const n = t.currentWidget;
-                                return !1 !== e.activate && n && i.activateById(n.id), n
+                            function i(e) {
+                                const o = t.currentWidget;
+                                return !1 !== e.activate && o && l.currentWidget !== o && l.activateById(o.id), o
                             }
 
                             function c() {
                                 return null !== t.currentWidget && t.currentWidget === e.shell.currentWidget
                             }
-                            l.addCommand("vim:run-select-next-edit", {
+                            o.addCommand("vim:run-select-next-edit", {
                                 label: "Run Cell and Edit Next Cell",
                                 execute: e => {
-                                    const t = a(e);
+                                    const t = i(e);
                                     if (t) {
                                         const {
                                             context: e,
-                                            content: n
+                                            content: o
                                         } = t;
-                                        o.NotebookActions.runAndAdvance(n, e.sessionContext), t.content.mode = "edit"
+                                        n.NotebookActions.runAndAdvance(o, e.sessionContext), t.content.mode = "edit"
                                     }
                                 },
                                 isEnabled: c
-                            }), l.addCommand("vim:run-cell-and-edit", {
+                            }), o.addCommand("vim:run-cell-and-edit", {
                                 label: "Run Cell and Edit Cell",
                                 execute: e => {
-                                    const t = a(e);
+                                    const t = i(e);
                                     if (t) {
                                         const {
                                             context: e,
-                                            content: n
+                                            content: o
                                         } = t;
-                                        o.NotebookActions.run(n, e.sessionContext), t.content.mode = "edit"
+                                        n.NotebookActions.run(o, e.sessionContext), t.content.mode = "edit"
                                     }
                                 },
                                 isEnabled: c
-                            }), l.addCommand("vim:cut-cell-and-edit", {
+                            }), o.addCommand("vim:cut-cell-and-edit", {
                                 label: "Cut Cell(s) and Edit Cell",
                                 execute: e => {
-                                    const t = a(e);
+                                    const t = i(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
-                                        o.NotebookActions.cut(e), e.mode = "edit"
+                                        n.NotebookActions.cut(e), e.mode = "edit"
                                     }
                                 },
                                 isEnabled: c
-                            }), l.addCommand("vim:copy-cell-and-edit", {
+                            }), o.addCommand("vim:copy-cell-and-edit", {
                                 label: "Copy Cell(s) and Edit Cell",
                                 execute: e => {
-                                    const t = a(e);
+                                    const t = i(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
-                                        o.NotebookActions.copy(e), e.mode = "edit"
+                                        n.NotebookActions.copy(e), e.mode = "edit"
                                     }
                                 },
                                 isEnabled: c
-                            }), l.addCommand("vim:paste-cell-and-edit", {
+                            }), o.addCommand("vim:paste-cell-and-edit", {
                                 label: "Paste Cell(s) and Edit Cell",
                                 execute: e => {
-                                    const t = a(e);
+                                    const t = i(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
-                                        o.NotebookActions.paste(e, "below"), e.mode = "edit"
+                                        n.NotebookActions.paste(e, "below"), e.mode = "edit"
                                     }
                                 },
                                 isEnabled: c
-                            }), l.addCommand("vim:merge-and-edit", {
+                            }), o.addCommand("vim:merge-and-edit", {
                                 label: "Merge and Edit Cell",
                                 execute: e => {
-                                    const t = a(e);
+                                    const t = i(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
-                                        o.NotebookActions.mergeCells(e), t.content.mode = "edit"
+                                        n.NotebookActions.mergeCells(e), t.content.mode = "edit"
                                     }
                                 },
                                 isEnabled: c
-                            }), l.addCommand("vim:enter-insert-mode", {
+                            }), o.addCommand("vim:enter-insert-mode", {
                                 label: "Enter Insert Mode",
                                 execute: e => {
-                                    const t = a(e);
+                                    const t = i(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
                                         if (null !== e.activeCell) {
                                             const o = e.activeCell.editor;
-                                            t.content.mode = "edit", n.Vim.handleKey(o.editor, "i")
+                                            t.content.mode = "edit";
+                                            const n = (0, a.getCM)(o.editor);
+                                            if (!n) return void console.error("CodeMirror vim wrapper not found");
+                                            a.Vim.handleKey(n, "i")
                                         }
                                     }
                                 },
                                 isEnabled: c
-                            }), l.addCommand("vim:leave-insert-mode", {
+                            }), o.addCommand("vim:leave-insert-mode", {
                                 label: "Leave Insert Mode",
                                 execute: e => {
-                                    const t = a(e);
+                                    const t = i(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
                                         if (null !== e.activeCell) {
-                                            const t = e.activeCell.editor;
-                                            n.Vim.handleKey(t.editor, "<Esc>")
+                                            const t = e.activeCell.editor,
+                                                o = (0, a.getCM)(t.editor);
+                                            if (!o) return void console.error("CodeMirror vim wrapper not found");
+                                            a.Vim.handleKey(o, "<Esc>")
                                         }
                                     }
                                 },
                                 isEnabled: c
-                            }), l.addCommand("vim:leave-current-mode", {
+                            }), o.addCommand("vim:leave-current-mode", {
                                 label: 'Move Insert to Normal to Jupyter Command Mode"',
                                 execute: e => {
-                                    const t = a(e);
+                                    const t = i(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
                                         if (null !== e.activeCell) {
-                                            const t = e.activeCell.editor;
-                                            t.editor.state.vim.insertMode || t.editor.state.vim.visualMode ? n.Vim.handleKey(t.editor, "<Esc>") : l.execute("notebook:enter-command-mode")
+                                            const t = e.activeCell.editor,
+                                                n = (0, a.getCM)(t.editor);
+                                            if (!n) return void console.error("CodeMirror vim wrapper not found");
+                                            const l = n.state.vim;
+                                            l.insertMode || l.visualMode ? a.Vim.handleKey(n, "<Esc>") : o.execute("notebook:enter-command-mode")
                                         }
                                     }
                                 },
                                 isEnabled: c
-                            }), l.addCommand("vim:select-below-execute-markdown", {
+                            }), o.addCommand("vim:select-below-execute-markdown", {
                                 label: "Execute Markdown and Select Cell Below",
                                 execute: e => {
-                                    const t = a(e);
+                                    const t = i(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
-                                        return null !== e.activeCell && "markdown" === e.activeCell.model.type && (t.content.activeCell.rendered = !0), o.NotebookActions.selectBelow(t.content)
+                                        return null !== e.activeCell && "markdown" === e.activeCell.model.type && (t.content.activeCell.rendered = !0), n.NotebookActions.selectBelow(t.content)
                                     }
                                 },
                                 isEnabled: c
-                            }), l.addCommand("vim:select-above-execute-markdown", {
+                            }), o.addCommand("vim:select-above-execute-markdown", {
                                 label: "Execute Markdown and Select Cell Below",
                                 execute: e => {
-                                    const t = a(e);
+                                    const t = i(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
-                                        return null !== e.activeCell && "markdown" === e.activeCell.model.type && (t.content.activeCell.rendered = !0), o.NotebookActions.selectAbove(t.content)
+                                        return null !== e.activeCell && "markdown" === e.activeCell.model.type && (t.content.activeCell.rendered = !0), n.NotebookActions.selectAbove(t.content)
                                     }
                                 },
                                 isEnabled: c
-                            }), l.addCommand("vim:select-first-cell", {
+                            }), o.addCommand("vim:select-first-cell", {
                                 label: "Select First Cell",
                                 execute: e => {
-                                    const t = a(e);
+                                    const t = i(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
-                                        e.activeCellIndex = 0, e.deselectAll(), null !== e.activeCell && d.ElementExt.scrollIntoViewIfNeeded(e.node, e.activeCell.node)
+                                        e.activeCellIndex = 0, e.deselectAll(), null !== e.activeCell && r.ElementExt.scrollIntoViewIfNeeded(e.node, e.activeCell.node)
                                     }
                                 },
                                 isEnabled: c
-                            }), l.addCommand("vim:select-last-cell", {
+                            }), o.addCommand("vim:select-last-cell", {
                                 label: "Select Last Cell",
                                 execute: e => {
-                                    const t = a(e);
+                                    const t = i(e);
                                     if (t) {
                                         const {
                                             content: e
                                         } = t;
-                                        e.activeCellIndex = t.content.widgets.length - 1, e.deselectAll(), null !== e.activeCell && d.ElementExt.scrollIntoViewIfNeeded(e.node, e.activeCell.node)
+                                        e.activeCellIndex = t.content.widgets.length - 1, e.deselectAll(), null !== e.activeCell && r.ElementExt.scrollIntoViewIfNeeded(e.node, e.activeCell.node)
                                     }
                                 },
                                 isEnabled: c
-                            }), l.addCommand("vim:center-cell", {
+                            }), o.addCommand("vim:center-cell", {
                                 label: "Center Cell",
                                 execute: e => {
-                                    const t = a(e);
-                                    if (t && null !== t.content.activeCell) {
-                                        const e = t.content.activeCell.inputArea.node.getBoundingClientRect();
-                                        t.content.scrollToPosition(e.bottom, 0)
-                                    }
+                                    const t = i(e);
+                                    t && null !== t.content.activeCell && t.content.scrollToCell(t.content.activeCell, "center")
                                 },
                                 isEnabled: c
                             })
-                        }(e, t, a), l.load(`${s}:plugin`).then((e => {
-                            b(e), e.changed.connect(b)
+                        }(e, t), i.load(`${m}:plugin`).then((e => {
+                            x(e), e.changed.connect(x)
                         }), (e => {
-                            console.error(`Could not load settings, so did not active ${s}: ${e}`)
+                            console.error(`Could not load settings, so did not active ${m}: ${e}`)
                         })), Promise.resolve()
                 },
-                requires: [o.INotebookTracker, l.ICodeMirror, i.ISettingRegistry]
+                requires: [n.INotebookTracker, l.IEditorExtensionRegistry, i.ISettingRegistry]
             }
         }
     }
 ]);
```

### Comparing `jupyterlab_vim-0.16.0/src/codemirrorCommands.ts` & `jupyterlab_vim-0.17.0/src/codemirrorCommands.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,93 @@
 import { Cell, ICellModel, MarkdownCell } from '@jupyterlab/cells';
 import { CodeMirrorEditor } from '@jupyterlab/codemirror';
 import { INotebookTracker } from '@jupyterlab/notebook';
 import { CommandRegistry } from '@lumino/commands';
+import { Vim, getCM, CodeMirror } from '@replit/codemirror-vim';
 
-/**
- * A boolean indicating whether the platform is Mac.
- */
-const IS_MAC = !!navigator.platform.match(/Mac/i);
+// It may be worth contributing types for these upstream
+interface IVimCodeMirror extends CodeMirror {
+  moveByLines: undefined;
+  moveByDisplayLines: undefined;
+  moveByScroll: undefined;
+  moveToColumn: undefined;
+  moveToEol: undefined;
+}
 
 export interface IKeybinding {
   command: string;
   keys: string;
   context: string;
   mapfn: string;
   enabled: boolean;
 }
 
 export interface IOptions {
   commands: CommandRegistry;
-  cm: CodeMirrorEditor;
   enabled: boolean;
   userKeybindings: IKeybinding[];
 }
 
 export class VimCellManager {
-  constructor({ commands, cm, enabled, userKeybindings }: IOptions) {
+  constructor({ commands, enabled, userKeybindings }: IOptions) {
     this._commands = commands;
-    this._cm = cm;
     this.enabled = enabled;
     this.lastActiveCell = null;
     this.userKeybindings = userKeybindings ?? [];
   }
 
   onActiveCellChanged(
     tracker: INotebookTracker,
     activeCell: Cell<ICellModel> | null
   ): void {
-    this.modifyCell(activeCell);
+    this.modifyCell(activeCell).catch(console.error);
   }
 
-  modifyCell(activeCell: Cell<ICellModel> | null): void {
+  async modifyCell(activeCell: Cell<ICellModel> | null): Promise<void> {
     if (!activeCell) {
       return;
     }
     this.lastActiveCell = activeCell;
-    const editor = activeCell.editor as CodeMirrorEditor;
-
-    if (this.enabled) {
-      editor.setOption('keyMap', 'vim');
-      const extraKeys = editor.getOption('extraKeys') || {};
+    await activeCell.ready;
+    const editor = activeCell.editor as CodeMirrorEditor | null;
 
-      // TODO: does can this be any codemirror?
-      extraKeys['Esc'] = (this._cm as any).prototype.leaveInsertMode;
-      if (!IS_MAC) {
-        extraKeys['Ctrl-C'] = false;
-      }
+    if (activeCell.isDisposed) {
+      console.warn('Cell was already disposed, cannot setup vim mode');
+      return;
+    }
 
-      (this._cm as any).prototype.save = (): void => {
-        this._commands.execute('docmanager:save');
-      };
+    if (!editor) {
+      throw Error('Cell editor not available');
+    }
 
-      editor.setOption('extraKeys', extraKeys);
+    const view = editor.editor;
 
-      const lcm = this._cm as any;
-      const lvim = lcm.Vim as any;
+    if (this.enabled) {
+      if (!editor.getOption('vim')) {
+        // this erases state, we do not want to call it if not needed.
+        editor.setOption('vim', true);
+
+        // On each key press the notebook (`Notebook.handleEvent`) invokes
+        // a handler ensuring focus (`Notebook._ensureFocus`); the logic does
+        // not work well for the `ex commands` panel which is always interpreted
+        // as blurred because it exists outside of the CodeMirror6 state; here
+        // we override `hasFocus` handler to ensure it is taken into account.
+        const cm = getCM(view)!;
+        editor.hasFocus = () => {
+          if (
+            cm.state.dialog &&
+            cm.state.dialog.contains(document.activeElement)
+          ) {
+            return true;
+          }
+          return view.hasFocus;
+        };
+      }
+      const lcm = getCM(view);
+      const lvim = Vim;
 
       // Clear existing user keybindings, then re-register in case they changed in the user settings
       ['normal', 'visual', 'insert'].forEach(ctx => lvim.mapclear(ctx));
       this.userKeybindings.forEach(
         ({
           command,
           keys,
@@ -81,25 +101,21 @@
             } else {
               lvim.noremap(command, keys, context);
             }
           }
         }
       );
 
-      lvim.defineEx('quit', 'q', (cm: any) => {
-        this._commands.execute('notebook:enter-command-mode');
-      });
-
-      (this._cm as any).Vim.handleKey(editor.editor, '<Esc>');
+      Vim.handleKey(lcm, '<Esc>');
 
       // Define a function to use as Vim motion
       // This replaces the codemirror moveByLines function to
       // for jumping between notebook cells.
       const moveByLinesOrCell = (
-        cm: any,
+        cm: IVimCodeMirror,
         head: any,
         motionArgs: any,
         vim: any
       ): any => {
         const cur = head;
         let endCh = cur.ch;
         const currentCell = activeCell;
@@ -165,32 +181,33 @@
             if (!motionArgs.handleArrow) {
               this._commands.execute('notebook:move-cursor-down');
             } else {
               // This block preventing double cell hop when you use arrow keys for navigation
               //    also arrow key navigation works properly when current cursor position
               //    at the beginning of line for up move, and at the end for down move
               const cursor = cm.getCursor();
-              const last_char = cm.doc.getLine(last).length;
+              // CM6 is 1-based
+              const last_char = view.state.doc.line(last + 1).length;
               if (cursor.line !== last || cursor.ch !== last_char) {
-                cm.setCursor({ line: last, ch: last_char });
+                cm.setCursor(last, last_char);
                 this._commands.execute('notebook:move-cursor-down');
               }
             }
             // key = 'j';
           } else {
             // ns.notebook.select_prev();
             if (!motionArgs.handleArrow) {
               this._commands.execute('notebook:move-cursor-up');
             } else {
               // This block preventing double cell hop when you use arrow keys for navigation
               //    also arrow key navigation works properly when current cursor position
               //    at the beginning of line for up move, and at the end for down move
               const cursor = cm.getCursor();
               if (cursor.line !== 0 || cursor.ch !== 0) {
-                cm.setCursor({ line: 0, ch: 0 });
+                cm.setCursor(0, 0);
                 this._commands.execute('notebook:move-cursor-up');
               }
             }
             // key = 'k';
           }
           return;
         }
@@ -207,18 +224,18 @@
 
         if (motionArgs.toFirstChar) {
           endCh = findFirstNonWhiteSpaceCharacter(cm.getLine(line));
           vim.lastHPos = endCh;
         }
 
         vim.lastHSPos = cm.charCoords(
-          (this._cm as any).Pos(line, endCh),
+          new CodeMirror.Pos(line, endCh),
           'div'
         ).left;
-        return (this._cm as any).Pos(line, endCh);
+        return new CodeMirror.Pos(line, endCh);
       };
       lvim.defineMotion('moveByLinesOrCell', moveByLinesOrCell);
 
       lvim.mapCommand(
         '<Up>',
         'motion',
         'moveByLinesOrCell',
@@ -261,18 +278,17 @@
         { extra: 'normal' }
       );
       lvim.mapCommand('<C-y>', 'action', 'moveCellUp', {}, { extra: 'normal' });
       lvim.defineAction('splitCell', (cm: any, actionArgs: any) => {
         this._commands.execute('notebook:split-cell-at-cursor');
       });
       lvim.mapCommand('-', 'action', 'splitCell', {}, { extra: 'normal' });
-    } else if (editor.getOption('keyMap') === 'vim') {
-      editor.setOption('keyMap', 'default');
+    } else if (editor.getOption('vim')) {
+      editor.setOption('vim', false);
     }
   }
 
   private _commands: CommandRegistry;
-  private _cm: CodeMirrorEditor;
   public lastActiveCell: Cell<ICellModel> | null;
   public enabled: boolean;
   public userKeybindings: IKeybinding[];
 }
```

### Comparing `jupyterlab_vim-0.16.0/src/index.ts` & `jupyterlab_vim-0.17.0/src/index.ts`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
 import { INotebookTracker } from '@jupyterlab/notebook';
 
-import { ICodeMirror, CodeMirrorEditor } from '@jupyterlab/codemirror';
+import {
+  IEditorExtensionRegistry,
+  EditorExtensionRegistry
+} from '@jupyterlab/codemirror';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { IDisposable } from '@lumino/disposable';
+import { vim, Vim } from '@replit/codemirror-vim';
+import { EditorView } from '@codemirror/view';
+import { Prec } from '@codemirror/state';
 
 import { VimCellManager, IKeybinding } from './codemirrorCommands';
 import { addJLabCommands } from './labCommands';
 
 const PLUGIN_NAME = '@axlair/jupyterlab_vim';
 const TOGGLE_ID = 'jupyterlab-vim:toggle';
 let enabled = false;
@@ -19,80 +25,115 @@
 /**
  * Initialization data for the jupyterlab_vim extension.
  */
 const extension: JupyterFrontEndPlugin<void> = {
   id: PLUGIN_NAME,
   autoStart: true,
   activate: activateCellVim,
-  requires: [INotebookTracker, ICodeMirror, ISettingRegistry]
+  requires: [INotebookTracker, IEditorExtensionRegistry, ISettingRegistry]
 };
 
 async function activateCellVim(
   app: JupyterFrontEnd,
   tracker: INotebookTracker,
-  jlabCodeMirror: ICodeMirror,
+  editorExtensionRegistry: IEditorExtensionRegistry,
   settingRegistry: ISettingRegistry
 ): Promise<void> {
-  // await app.restored;
+  const theme = Prec.highest(
+    EditorView.theme({
+      '.cm-fat-cursor': {
+        position: 'absolute',
+        background: 'var(--jp-vim-cursor-color)',
+        border: 'none',
+        whiteSpace: 'pre'
+      },
+      '&:not(.cm-focused) .cm-fat-cursor': {
+        background: 'none',
+        outline: 'solid 1px var(--jp-vim-cursor-color)',
+        color: 'transparent !important'
+      }
+    })
+  );
+
+  editorExtensionRegistry.addExtension({
+    name: 'vim',
+    factory: options => {
+      return EditorExtensionRegistry.createConditionalExtension([
+        theme,
+        vim({
+          status: false
+        })
+      ]);
+    }
+  });
+
   app.commands.addCommand(TOGGLE_ID, {
     label: 'Enable Notebook Vim mode',
     execute: () => {
       if (settingRegistry) {
         void settingRegistry.set(`${PLUGIN_NAME}:plugin`, 'enabled', !enabled);
       }
     },
     isToggled: () => enabled
   });
 
-  const userKeybindings = ((
+  const userKeybindings = (
     await settingRegistry.get(`${PLUGIN_NAME}:plugin`, 'extraKeybindings')
-  ).composite as unknown) as Array<IKeybinding>;
+  ).composite as unknown as Array<IKeybinding>;
 
-  // eslint-disable-next-line prettier/prettier
-  const globalCodeMirror = jlabCodeMirror.CodeMirror as unknown as CodeMirrorEditor;
   let cellManager: VimCellManager | null = null;
   let escBinding: IDisposable | null = null;
   let hasEverBeenEnabled = false;
 
+  Vim.defineEx('write', 'w', () => {
+    app.commands.execute('docmanager:save');
+  });
+
+  Vim.defineEx('quit', 'q', () => {
+    // In JupyterLab 4.0 needs to be executed after vim panel has closed, here
+    // achived by moving it to end of execution stack with `setTimeout()`.
+    setTimeout(() => {
+      app.commands.execute('notebook:enter-command-mode');
+    });
+  });
+
   cellManager = new VimCellManager({
     commands: app.commands,
-    cm: globalCodeMirror,
     enabled,
     userKeybindings
   });
   // it's ok to connect here because we will never reach the vim section unless
   // ensureVimKeyMap has been called due to the checks for enabled.
   // we need to have now in order to keep track of the last active cell
   // so that we can modify it when vim is turned on or off.
   tracker.activeCellChanged.connect(
     cellManager.onActiveCellChanged,
     cellManager
   );
 
-  addJLabCommands(app, tracker, globalCodeMirror);
+  addJLabCommands(app, tracker);
 
   async function updateSettings(
     settings: ISettingRegistry.ISettings
   ): Promise<void> {
-    const userKeybindings = ((
+    const userKeybindings = (
       await settingRegistry.get(`${PLUGIN_NAME}:plugin`, 'extraKeybindings')
-    ).composite as unknown) as Array<IKeybinding>;
+    ).composite as unknown as Array<IKeybinding>;
 
     enabled = settings.get('enabled').composite === true;
     app.commands.notifyCommandChanged(TOGGLE_ID);
     if (cellManager) {
       cellManager.enabled = enabled;
       cellManager.userKeybindings = userKeybindings;
     }
     if (enabled) {
       escBinding?.dispose();
       if (!hasEverBeenEnabled) {
         hasEverBeenEnabled = true;
         await app.restored;
-        await jlabCodeMirror.ensureVimKeymap();
       }
     } else {
       escBinding = app.commands.addKeyBinding({
         command: 'notebook:enter-command-mode',
         keys: ['Escape'],
         selector: '.jp-Notebook.jp-mod-editMode'
       });
```

### Comparing `jupyterlab_vim-0.16.0/src/labCommands.ts` & `jupyterlab_vim-0.17.0/src/labCommands.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import { JupyterFrontEnd } from '@jupyterlab/application';
 import { MarkdownCell } from '@jupyterlab/cells';
+import { Vim, getCM } from '@replit/codemirror-vim';
 import { CodeMirrorEditor } from '@jupyterlab/codemirror';
 import {
   INotebookTracker,
   NotebookActions,
   NotebookPanel
 } from '@jupyterlab/notebook';
 import { ReadonlyPartialJSONObject } from '@lumino/coreutils';
 
 import { IDisposable } from '@lumino/disposable';
 import { ElementExt } from '@lumino/domutils';
 
 export function addJLabCommands(
   app: JupyterFrontEnd,
-  tracker: INotebookTracker,
-  CodeMirror: CodeMirrorEditor
+  tracker: INotebookTracker
 ): Array<IDisposable> {
   const { commands, shell } = app;
   function getCurrent(args: ReadonlyPartialJSONObject): NotebookPanel | null {
     const widget = tracker.currentWidget;
     const activate = args['activate'] !== false;
 
-    if (activate && widget) {
+    // Should we expose `activeWidget` in `IShell`?
+    // when `activateById` is called the Notebook handler focuses current editor
+    // which leads to bluring the panel for inputing ex commands and may render
+    // the use of ex commands impossible if called needlesly.
+    if (activate && widget && shell.currentWidget !== widget) {
       shell.activateById(widget.id);
     }
 
     return widget;
   }
   function isEnabled(): boolean {
     return (
@@ -118,30 +122,40 @@
         const current = getCurrent(args);
 
         if (current) {
           const { content } = current;
           if (content.activeCell !== null) {
             const editor = content.activeCell.editor as CodeMirrorEditor;
             current.content.mode = 'edit';
-            (CodeMirror as any).Vim.handleKey(editor.editor, 'i');
+            const cm = getCM(editor.editor);
+            if (!cm) {
+              console.error('CodeMirror vim wrapper not found');
+              return;
+            }
+            Vim.handleKey(cm, 'i');
           }
         }
       },
       isEnabled
     }),
     commands.addCommand('vim:leave-insert-mode', {
       label: 'Leave Insert Mode',
       execute: args => {
         const current = getCurrent(args);
 
         if (current) {
           const { content } = current;
           if (content.activeCell !== null) {
             const editor = content.activeCell.editor as CodeMirrorEditor;
-            (CodeMirror as any).Vim.handleKey(editor.editor, '<Esc>');
+            const cm = getCM(editor.editor);
+            if (!cm) {
+              console.error('CodeMirror vim wrapper not found');
+              return;
+            }
+            Vim.handleKey(cm, '<Esc>');
           }
         }
       },
       isEnabled
     }),
     commands.addCommand('vim:leave-current-mode', {
       label: 'Move Insert to Normal to Jupyter Command Mode"',
@@ -149,20 +163,24 @@
         const current = getCurrent(args);
 
         if (current) {
           const { content } = current;
           if (content.activeCell !== null) {
             const editor = content.activeCell.editor as CodeMirrorEditor;
 
+            const cm = getCM(editor.editor);
+            if (!cm) {
+              console.error('CodeMirror vim wrapper not found');
+              return;
+            }
+            const vim = cm.state.vim;
+
             // Get the current editor state
-            if (
-              editor.editor.state.vim.insertMode ||
-              editor.editor.state.vim.visualMode
-            ) {
-              (CodeMirror as any).Vim.handleKey(editor.editor, '<Esc>');
+            if (vim.insertMode || vim.visualMode) {
+              Vim.handleKey(cm, '<Esc>');
             } else {
               commands.execute('notebook:enter-command-mode');
             }
           }
         }
       },
       isEnabled
@@ -243,16 +261,15 @@
     }),
     commands.addCommand('vim:center-cell', {
       label: 'Center Cell',
       execute: args => {
         const current = getCurrent(args);
 
         if (current && current.content.activeCell !== null) {
-          const er = current.content.activeCell.inputArea.node.getBoundingClientRect();
-          current.content.scrollToPosition(er.bottom, 0);
+          current.content.scrollToCell(current.content.activeCell, 'center');
         }
       },
       isEnabled
     })
   ];
   return addedCommands;
 }
```

### Comparing `jupyterlab_vim-0.16.0/tsconfig.json` & `jupyterlab_vim-0.17.0/tsconfig.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9802631578947368%*

 * *Differences: {"'compilerOptions'": "{'target': 'ES2018', delete: ['types']}"}*

```diff
@@ -13,14 +13,13 @@
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "es2017",
-        "types": []
+        "target": "ES2018"
     },
     "include": [
         "src/*"
     ]
 }
```

