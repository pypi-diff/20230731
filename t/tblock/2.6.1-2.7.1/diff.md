# Comparing `tmp/tblock-2.6.1.tar.gz` & `tmp/tblock-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tblock-2.6.1.tar", last modified: Mon Jan  9 22:40:01 2023, max compression
+gzip compressed data, was "tblock-2.7.1.tar", last modified: Mon Jul 31 17:08:03 2023, max compression
```

## Comparing `tblock-2.6.1.tar` & `tblock-2.7.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 twann     (1000) twann     (1000)        0 2023-01-09 22:40:01.518084 tblock-2.6.1/
--rw-r--r--   0 twann     (1000) twann     (1000)    35150 2021-10-04 15:07:31.000000 tblock-2.6.1/LICENSE
--rw-r--r--   0 twann     (1000) twann     (1000)       59 2022-12-25 17:24:05.000000 tblock-2.6.1/MANIFEST.in
--rw-r--r--   0 twann     (1000) twann     (1000)     5896 2023-01-09 22:40:01.518084 tblock-2.6.1/PKG-INFO
--rw-r--r--   0 twann     (1000) twann     (1000)     5259 2023-01-09 19:51:20.000000 tblock-2.6.1/README.md
--rw-r--r--   0 twann     (1000) twann     (1000)       84 2023-01-09 20:18:50.000000 tblock-2.6.1/pyproject.toml
--rw-r--r--   0 twann     (1000) twann     (1000)       17 2023-01-09 20:18:50.000000 tblock-2.6.1/requirements.txt
--rw-r--r--   0 twann     (1000) twann     (1000)      204 2023-01-09 22:40:01.518084 tblock-2.6.1/setup.cfg
--rwxr-xr-x   0 twann     (1000) twann     (1000)     2963 2023-01-09 20:18:50.000000 tblock-2.6.1/setup.py
-drwxr-xr-x   0 twann     (1000) twann     (1000)        0 2023-01-09 22:40:01.518084 tblock-2.6.1/tblock/
--rw-r--r--   0 twann     (1000) twann     (1000)     2340 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/__init__.py
--rw-r--r--   0 twann     (1000) twann     (1000)     1015 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/__main__.py
-drwxr-xr-x   0 twann     (1000) twann     (1000)        0 2023-01-09 22:40:01.518084 tblock-2.6.1/tblock/argumentor/
--rw-r--r--   0 twann     (1000) twann     (1000)    35240 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/argumentor/__init__.py
--rw-r--r--   0 twann     (1000) twann     (1000)     1166 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/argumentor/exceptions.py
--rw-r--r--   0 twann     (1000) twann     (1000)    29536 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/cli.py
--rw-r--r--   0 twann     (1000) twann     (1000)    11041 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/compat.py
--rw-r--r--   0 twann     (1000) twann     (1000)     6168 2023-01-09 22:33:56.000000 tblock-2.6.1/tblock/config.py
--rw-r--r--   0 twann     (1000) twann     (1000)     4004 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/const.py
-drwxr-xr-x   0 twann     (1000) twann     (1000)        0 2023-01-09 22:40:01.518084 tblock-2.6.1/tblock/converter/
--rw-r--r--   0 twann     (1000) twann     (1000)    21008 2023-01-09 21:59:04.000000 tblock-2.6.1/tblock/converter/__init__.py
--rw-r--r--   0 twann     (1000) twann     (1000)     1036 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/converter/__main__.py
--rw-r--r--   0 twann     (1000) twann     (1000)     9884 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/converter/syntaxtools.py
-drwxr-xr-x   0 twann     (1000) twann     (1000)        0 2023-01-09 22:40:01.518084 tblock-2.6.1/tblock/daemon/
--rw-r--r--   0 twann     (1000) twann     (1000)     9787 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/daemon/__init__.py
--rw-r--r--   0 twann     (1000) twann     (1000)     1030 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/daemon/__main__.py
--rw-r--r--   0 twann     (1000) twann     (1000)     2009 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/exceptions.py
--rw-r--r--   0 twann     (1000) twann     (1000)    71613 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/filters.py
--rw-r--r--   0 twann     (1000) twann     (1000)    14669 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/hosts.py
--rw-r--r--   0 twann     (1000) twann     (1000)    22770 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/rules.py
--rw-r--r--   0 twann     (1000) twann     (1000)     6018 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/style.py
--rw-r--r--   0 twann     (1000) twann     (1000)     9375 2023-01-09 20:18:50.000000 tblock-2.6.1/tblock/utils.py
-drwxr-xr-x   0 twann     (1000) twann     (1000)        0 2023-01-09 22:40:01.518084 tblock-2.6.1/tblock.egg-info/
--rw-r--r--   0 twann     (1000) twann     (1000)     5896 2023-01-09 22:40:01.000000 tblock-2.6.1/tblock.egg-info/PKG-INFO
--rw-r--r--   0 twann     (1000) twann     (1000)      769 2023-01-09 22:40:01.000000 tblock-2.6.1/tblock.egg-info/SOURCES.txt
--rw-r--r--   0 twann     (1000) twann     (1000)        1 2023-01-09 22:40:01.000000 tblock-2.6.1/tblock.egg-info/dependency_links.txt
--rw-r--r--   0 twann     (1000) twann     (1000)      109 2023-01-09 22:40:01.000000 tblock-2.6.1/tblock.egg-info/entry_points.txt
--rw-r--r--   0 twann     (1000) twann     (1000)       18 2023-01-09 22:40:01.000000 tblock-2.6.1/tblock.egg-info/requires.txt
--rw-r--r--   0 twann     (1000) twann     (1000)        7 2023-01-09 22:40:01.000000 tblock-2.6.1/tblock.egg-info/top_level.txt
-drwxr-xr-x   0 twann     (1000) twann     (1000)        0 2023-01-09 22:40:01.518084 tblock-2.6.1/test/
--rw-r--r--   0 twann     (1000) twann     (1000)     3051 2023-01-09 20:18:50.000000 tblock-2.6.1/test/test_config.py
--rw-r--r--   0 twann     (1000) twann     (1000)    28109 2023-01-09 20:18:50.000000 tblock-2.6.1/test/test_filters.py
--rw-r--r--   0 twann     (1000) twann     (1000)     8118 2023-01-09 20:18:50.000000 tblock-2.6.1/test/test_hosts.py
--rw-r--r--   0 twann     (1000) twann     (1000)    35974 2023-01-09 20:18:50.000000 tblock-2.6.1/test/test_rules.py
--rw-r--r--   0 twann     (1000) twann     (1000)     8098 2023-01-09 20:18:50.000000 tblock-2.6.1/test/test_utils.py
+drwxr-xr-x   0 twann     (1000) twann     (1000)        0 2023-07-31 17:08:03.683426 tblock-2.7.1/
+-rw-r--r--   0 twann     (1000) twann     (1000)    35150 2021-10-04 15:07:31.000000 tblock-2.7.1/LICENSE
+-rw-r--r--   0 twann     (1000) twann     (1000)       59 2022-12-25 17:24:05.000000 tblock-2.7.1/MANIFEST.in
+-rw-r--r--   0 twann     (1000) twann     (1000)     5022 2023-07-31 17:08:03.683426 tblock-2.7.1/PKG-INFO
+-rw-r--r--   0 twann     (1000) twann     (1000)     4385 2023-06-08 23:46:32.000000 tblock-2.7.1/README.md
+-rw-r--r--   0 twann     (1000) twann     (1000)       84 2023-06-02 21:16:05.000000 tblock-2.7.1/pyproject.toml
+-rw-r--r--   0 twann     (1000) twann     (1000)       23 2023-06-09 00:55:48.000000 tblock-2.7.1/requirements.txt
+-rw-r--r--   0 twann     (1000) twann     (1000)      219 2023-07-31 17:08:03.683426 tblock-2.7.1/setup.cfg
+-rwxr-xr-x   0 twann     (1000) twann     (1000)     2963 2023-06-02 21:16:05.000000 tblock-2.7.1/setup.py
+drwxr-xr-x   0 twann     (1000) twann     (1000)        0 2023-07-31 17:08:03.680092 tblock-2.7.1/tblock/
+-rw-r--r--   0 twann     (1000) twann     (1000)     2410 2023-06-07 22:11:07.000000 tblock-2.7.1/tblock/__init__.py
+-rw-r--r--   0 twann     (1000) twann     (1000)     1015 2023-06-02 21:16:05.000000 tblock-2.7.1/tblock/__main__.py
+drwxr-xr-x   0 twann     (1000) twann     (1000)        0 2023-07-31 17:08:03.683426 tblock-2.7.1/tblock/argumentor/
+-rw-r--r--   0 twann     (1000) twann     (1000)    38913 2023-06-07 22:06:26.000000 tblock-2.7.1/tblock/argumentor/__init__.py
+-rw-r--r--   0 twann     (1000) twann     (1000)     1167 2023-06-02 21:16:05.000000 tblock-2.7.1/tblock/argumentor/exceptions.py
+-rw-r--r--   0 twann     (1000) twann     (1000)    30228 2023-06-07 22:11:07.000000 tblock-2.7.1/tblock/cli.py
+-rw-r--r--   0 twann     (1000) twann     (1000)    11436 2023-06-07 22:11:07.000000 tblock-2.7.1/tblock/compat.py
+-rw-r--r--   0 twann     (1000) twann     (1000)     5964 2023-07-31 17:07:59.000000 tblock-2.7.1/tblock/config.py
+-rw-r--r--   0 twann     (1000) twann     (1000)     4535 2023-06-08 23:21:51.000000 tblock-2.7.1/tblock/const.py
+drwxr-xr-x   0 twann     (1000) twann     (1000)        0 2023-07-31 17:08:03.683426 tblock-2.7.1/tblock/converter/
+-rw-r--r--   0 twann     (1000) twann     (1000)    22271 2023-06-07 22:11:07.000000 tblock-2.7.1/tblock/converter/__init__.py
+-rw-r--r--   0 twann     (1000) twann     (1000)     1036 2023-06-02 21:16:05.000000 tblock-2.7.1/tblock/converter/__main__.py
+-rw-r--r--   0 twann     (1000) twann     (1000)     9884 2023-06-02 21:16:05.000000 tblock-2.7.1/tblock/converter/syntaxtools.py
+drwxr-xr-x   0 twann     (1000) twann     (1000)        0 2023-07-31 17:08:03.683426 tblock-2.7.1/tblock/daemon/
+-rw-r--r--   0 twann     (1000) twann     (1000)     9146 2023-06-04 00:05:04.000000 tblock-2.7.1/tblock/daemon/__init__.py
+-rw-r--r--   0 twann     (1000) twann     (1000)     1030 2023-06-02 21:16:05.000000 tblock-2.7.1/tblock/daemon/__main__.py
+-rw-r--r--   0 twann     (1000) twann     (1000)     2009 2023-06-02 21:16:05.000000 tblock-2.7.1/tblock/exceptions.py
+-rw-r--r--   0 twann     (1000) twann     (1000)    70416 2023-06-08 23:19:03.000000 tblock-2.7.1/tblock/filters.py
+-rw-r--r--   0 twann     (1000) twann     (1000)    15167 2023-06-04 10:53:46.000000 tblock-2.7.1/tblock/hosts.py
+-rw-r--r--   0 twann     (1000) twann     (1000)    23004 2023-06-07 22:11:07.000000 tblock-2.7.1/tblock/rules.py
+-rw-r--r--   0 twann     (1000) twann     (1000)     6197 2023-06-07 22:12:57.000000 tblock-2.7.1/tblock/style.py
+-rw-r--r--   0 twann     (1000) twann     (1000)     9507 2023-06-02 23:34:02.000000 tblock-2.7.1/tblock/utils.py
+drwxr-xr-x   0 twann     (1000) twann     (1000)        0 2023-07-31 17:08:03.680092 tblock-2.7.1/tblock.egg-info/
+-rw-r--r--   0 twann     (1000) twann     (1000)     5022 2023-07-31 17:08:03.000000 tblock-2.7.1/tblock.egg-info/PKG-INFO
+-rw-r--r--   0 twann     (1000) twann     (1000)      769 2023-07-31 17:08:03.000000 tblock-2.7.1/tblock.egg-info/SOURCES.txt
+-rw-r--r--   0 twann     (1000) twann     (1000)        1 2023-07-31 17:08:03.000000 tblock-2.7.1/tblock.egg-info/dependency_links.txt
+-rw-r--r--   0 twann     (1000) twann     (1000)      109 2023-07-31 17:08:03.000000 tblock-2.7.1/tblock.egg-info/entry_points.txt
+-rw-r--r--   0 twann     (1000) twann     (1000)       23 2023-07-31 17:08:03.000000 tblock-2.7.1/tblock.egg-info/requires.txt
+-rw-r--r--   0 twann     (1000) twann     (1000)        7 2023-07-31 17:08:03.000000 tblock-2.7.1/tblock.egg-info/top_level.txt
+drwxr-xr-x   0 twann     (1000) twann     (1000)        0 2023-07-31 17:08:03.683426 tblock-2.7.1/test/
+-rw-r--r--   0 twann     (1000) twann     (1000)     3051 2023-06-02 21:16:05.000000 tblock-2.7.1/test/test_config.py
+-rw-r--r--   0 twann     (1000) twann     (1000)    21651 2023-06-07 22:11:07.000000 tblock-2.7.1/test/test_filters.py
+-rw-r--r--   0 twann     (1000) twann     (1000)     8118 2023-06-02 21:16:05.000000 tblock-2.7.1/test/test_hosts.py
+-rw-r--r--   0 twann     (1000) twann     (1000)    35974 2023-06-02 21:16:05.000000 tblock-2.7.1/test/test_rules.py
+-rw-r--r--   0 twann     (1000) twann     (1000)     8098 2023-06-02 21:16:05.000000 tblock-2.7.1/test/test_utils.py
```

### Comparing `tblock-2.6.1/LICENSE` & `tblock-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tblock-2.6.1/PKG-INFO` & `tblock-2.7.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tblock
-Version: 2.6.1
+Version: 2.7.1
 Summary: An anti-capitalist ad-blocker that uses the hosts file
 Home-page: https://tblock.codeberg.page/
 Author: Twann
 Author-email: tw4nn@disroot.org
 License: GPLv3
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,36 +13,30 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-<img align="center" src="https://codeberg.org/tblock/tblock/raw/branch/main/assets/icons/tblock.svg" alt="TBlock logo" width="220px">
+<img align="center" src="https://codeberg.org/tblock/tblock-gui/raw/commit/2456e9651103baef81f3a6c25cce97bf9d0252ee/assets/banner.png">
 </p>
 <p align="center">
 <h1 align="center">TBlock</h1>
 </p>
 <p align="center">
-<a href="https://github.com/humanetech-community/awesome-humane-tech"><img src="https://codeberg.org/tblock/tblock/raw/branch/main/assets/icons/humane-tech-badge.svg" alt="Awesome Humane Tech"></a>
+<a href="https://github.com/humanetech-community/awesome-humane-tech"><img src="https://codeberg.org/tblock/tblock/raw/branch/main/extra/icons/humane-tech-badge.svg" alt="Awesome Humane Tech"></a>
 <a href="https://framagit.org/twann/tblock/-/pipelines"><img src="https://framagit.org/twann/tblock/badges/main/pipeline.svg" alt="Pipeline status"></a>
 <a href="https://nogithub.codeberg.page"><img src="https://nogithub.codeberg.page/badge.svg" alt="Please don't upload to GitHub"></a>
 </p>
 
 ## Description
 
 TBlock is a free and open-source system-wide ad-blocker that is compatible with most filter list formats.
 
-## Features
-
-- Blocks ads and trackers system-wide
-- Compatible with most filter list formats
-- Has an online repository to help you find and subscribe to popular blocklists in an easy way
-- Has a built-in filter list converter
-- Has a built-in daemon that regularly updates the filter lists and prevents your hosts file from being modified by other programs and users
+To view the repository for the graphical user interface, [click here](https://codeberg.org/tblock/tblock-gui).
 
 ## Installation
 
 You can easily install TBlock with:
 
 ```sh
 pipx install tblock
@@ -54,40 +48,40 @@
 
 After installing, you need to setup TBlock in order to enable protection against ads and trackers:
 
 ```sh
 tblock --init
 ```
 
-You can learn more by reading [the documentation](https://tblock.codeberg.page/docs/).
+You can learn more by reading [the documentation](https://docs.tblock.me/).
+
+## Demo
+
+[![asciicast](https://asciinema.org/a/589465.svg)](https://asciinema.org/a/589465)
 
 ## Roadmap
 
 Here is a list of the upcoming changes in TBlock code. Suggestions are, of course, welcome.
 
-- [ ] ~~Mark filter lists that are included in another list as `subscribed` when the user subscribes to the list~~
-- [x] ~~Allow virtual filter lists to exist (would act as a "group", like `base-devel` does on Arch Linux)~~*
-- [ ] Implement a GUI for TBlock
+- [x] Implement [a GUI for TBlock](https://codeberg.org/tblock/tblock-gui)
 - [ ] Rewrite the entire code, make a clearer public API and publish release 3.0.0
 
-> *This feature is now available [as profiles](https://tblock.codeberg.page/docs/profiles.html).
-
 ## Contributing
 
-Everyone ([?](https://codeberg.org/tblock/tblock/src/branch/main/CONTRIBUTING.md#limitations)) is welcome to contribute to TBlock in different ways. Bug reports can be made directly from the [Gitea issue tracker](https://codeberg.org/tblock/tblock/issues), by sending an email to the team or in [our Matrix room](https://matrix.to/#/#tblock:envs.net). 
+Everyone is welcome to contribute to TBlock in different ways. Bug reports can be made directly from the [Gitea issue tracker](https://codeberg.org/tblock/tblock/issues), by sending an email to the team or in [our Matrix room](https://matrix.to/#/#tblock:envs.net). 
 
 If you want to suggest a modification in the code, you can [open a pull request](https://codeberg.org/tblock/tblock/pulls) or send your patch using email or Matrix.
 
 If you want to be a beta-tester, you can install the latest beta version from our [release page](https://codeberg.org/tblock/tblock/releases) and contact us to give a feedback.
 
 You can find more information on how to contribute [here](https://codeberg.org/tblock/tblock/src/branch/main/CONTRIBUTING.md).
 
 ## Support
 
-The best way to support is to [contribute](#contributing). If you want, you can also [make a donation](https://tblock.codeberg.page/donate).
+The best way to support is to [contribute](#contributing). If you want, you can also [make a donation](https://tblock.me/donate).
 
 ## Authors and acknowledgment
 
 TBlock is currently mainained by [Twann](https://codeberg.org/twann), who is also its creator.
 A big thank you to all the people [who contribute(d) to the project](https://codeberg.org/tblock/tblock/src/branch/main/CONTRIBUTORS.md).
 
 ## Credits
@@ -101,27 +95,18 @@
 | [urllib3](https://urllib3.readthedocs.io/) | Andrey Petrov | MIT |
 | [argumentor](https://codeberg.org/twann/python-argumentor) | Twann | LGPLv3 |
 
 It is also worth mentioning [pacman](https://archlinux.org/pacman/), from which TBlock's command-line design is highly inspired.
 
 ## Contact
 
-- [Blog](https://fediverse.blog/~/TBlock)
 - [Mastodon](https://fosstodon.org/@tblock)
 - [Matrix](https://matrix.to/#/#tblock:matrix.org)
-- [Telegram](https://t.me/tblock)
 - [XMPP](xmpp:tblockproject@chat.disroot.org?join)
 
-## Screenshots
-
-<p align="center">
-    <img src="https://codeberg.org/tblock/tblock/raw/branch/main/assets/screenshots/screenshot2.png">
-    <img src="https://codeberg.org/tblock/tblock/raw/branch/main/assets/screenshots/screenshot1.png">
-</p>
-
 ## License
 
 [![GPLv3](https://www.gnu.org/graphics/gplv3-with-text-136x68.png)](https://www.gnu.org/licenses/gpl-3.0)
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

#### html2text {}

```diff
@@ -1,72 +1,62 @@
-Metadata-Version: 2.1 Name: tblock Version: 2.6.1 Summary: An anti-capitalist
+Metadata-Version: 2.1 Name: tblock Version: 2.7.1 Summary: An anti-capitalist
 ad-blocker that uses the hosts file Home-page: https://tblock.codeberg.page/
 Author: Twann Author-email: tw4nn@disroot.org License: GPLv3 Classifier:
 Environment :: Console Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE
-                                 [TBlock logo]
+              [https://codeberg.org/tblock/tblock-gui/raw/commit/
+          2456e9651103baef81f3a6c25cce97bf9d0252ee/assets/banner.png]
                              ****** TBlock ******
     [Awesome_Humane_Tech] [Pipeline_status] [Please_don't_upload_to_GitHub]
 ## Description TBlock is a free and open-source system-wide ad-blocker that is
-compatible with most filter list formats. ## Features - Blocks ads and trackers
-system-wide - Compatible with most filter list formats - Has an online
-repository to help you find and subscribe to popular blocklists in an easy way
-- Has a built-in filter list converter - Has a built-in daemon that regularly
-updates the filter lists and prevents your hosts file from being modified by
-other programs and users ## Installation You can easily install TBlock with:
-```sh pipx install tblock ``` More installation methods â such as Windows
-installer and packages for Linux distributions â can be found [on the
-website](https://tblock.codeberg.page/install). ## Usage After installing, you
-need to setup TBlock in order to enable protection against ads and trackers:
-```sh tblock --init ``` You can learn more by reading [the documentation]
-(https://tblock.codeberg.page/docs/). ## Roadmap Here is a list of the upcoming
-changes in TBlock code. Suggestions are, of course, welcome. - [ ] ~~Mark
-filter lists that are included in another list as `subscribed` when the user
-subscribes to the list~~ - [x] ~~Allow virtual filter lists to exist (would act
-as a "group", like `base-devel` does on Arch Linux)~~* - [ ] Implement a GUI
-for TBlock - [ ] Rewrite the entire code, make a clearer public API and publish
-release 3.0.0 > *This feature is now available [as profiles](https://
-tblock.codeberg.page/docs/profiles.html). ## Contributing Everyone ([?](https:/
-/codeberg.org/tblock/tblock/src/branch/main/CONTRIBUTING.md#limitations)) is
-welcome to contribute to TBlock in different ways. Bug reports can be made
-directly from the [Gitea issue tracker](https://codeberg.org/tblock/tblock/
-issues), by sending an email to the team or in [our Matrix room](https://
-matrix.to/#/#tblock:envs.net). If you want to suggest a modification in the
-code, you can [open a pull request](https://codeberg.org/tblock/tblock/pulls)
-or send your patch using email or Matrix. If you want to be a beta-tester, you
-can install the latest beta version from our [release page](https://
-codeberg.org/tblock/tblock/releases) and contact us to give a feedback. You can
-find more information on how to contribute [here](https://codeberg.org/tblock/
-tblock/src/branch/main/CONTRIBUTING.md). ## Support The best way to support is
-to [contribute](#contributing). If you want, you can also [make a donation]
-(https://tblock.codeberg.page/donate). ## Authors and acknowledgment TBlock is
-currently mainained by [Twann](https://codeberg.org/twann), who is also its
-creator. A big thank you to all the people [who contribute(d) to the project]
-(https://codeberg.org/tblock/tblock/src/branch/main/CONTRIBUTORS.md). ##
-Credits Here is a list of all libraries used in the project: | Name | Author |
-License | | --- | --- | --- | | [colorama](https://github.com/tartley/colorama)
-| Jonathan Hartley | BSD | | [requests](https://requests.readthedocs.io/) |
-Kenneth Reitz | Apache 2.0 | | [urllib3](https://urllib3.readthedocs.io/) |
-Andrey Petrov | MIT | | [argumentor](https://codeberg.org/twann/python-
-argumentor) | Twann | LGPLv3 | It is also worth mentioning [pacman](https://
-archlinux.org/pacman/), from which TBlock's command-line design is highly
-inspired. ## Contact - [Blog](https://fediverse.blog/~/TBlock) - [Mastodon]
-(https://fosstodon.org/@tblock) - [Matrix](https://matrix.to/#/#tblock:
-matrix.org) - [Telegram](https://t.me/tblock) - [XMPP](xmpp:
-tblockproject@chat.disroot.org?join) ## Screenshots
-    [https://codeberg.org/tblock/tblock/raw/branch/main/assets/screenshots/
- screenshot2.png] [https://codeberg.org/tblock/tblock/raw/branch/main/assets/
-                         screenshots/screenshot1.png]
-## License [![GPLv3](https://www.gnu.org/graphics/gplv3-with-text-136x68.png)]
-(https://www.gnu.org/licenses/gpl-3.0) This program is free software: you can
-redistribute it and/or modify it under the terms of the GNU General Public
-License as published by the Free Software Foundation, either version 3 of the
-License, or (at your option) any later version. This program is distributed in
-the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the
-implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See
-the GNU General Public License for more details. You should have received a
-copy of the GNU General Public License along with this program. If not, see
+compatible with most filter list formats. To view the repository for the
+graphical user interface, [click here](https://codeberg.org/tblock/tblock-gui).
+## Installation You can easily install TBlock with: ```sh pipx install tblock
+``` More installation methods â such as Windows installer and packages for
+Linux distributions â can be found [on the website](https://
+tblock.codeberg.page/install). ## Usage After installing, you need to setup
+TBlock in order to enable protection against ads and trackers: ```sh tblock --
+init ``` You can learn more by reading [the documentation](https://
+docs.tblock.me/). ## Demo [![asciicast](https://asciinema.org/a/589465.svg)]
+(https://asciinema.org/a/589465) ## Roadmap Here is a list of the upcoming
+changes in TBlock code. Suggestions are, of course, welcome. - [x] Implement [a
+GUI for TBlock](https://codeberg.org/tblock/tblock-gui) - [ ] Rewrite the
+entire code, make a clearer public API and publish release 3.0.0 ##
+Contributing Everyone is welcome to contribute to TBlock in different ways. Bug
+reports can be made directly from the [Gitea issue tracker](https://
+codeberg.org/tblock/tblock/issues), by sending an email to the team or in [our
+Matrix room](https://matrix.to/#/#tblock:envs.net). If you want to suggest a
+modification in the code, you can [open a pull request](https://codeberg.org/
+tblock/tblock/pulls) or send your patch using email or Matrix. If you want to
+be a beta-tester, you can install the latest beta version from our [release
+page](https://codeberg.org/tblock/tblock/releases) and contact us to give a
+feedback. You can find more information on how to contribute [here](https://
+codeberg.org/tblock/tblock/src/branch/main/CONTRIBUTING.md). ## Support The
+best way to support is to [contribute](#contributing). If you want, you can
+also [make a donation](https://tblock.me/donate). ## Authors and acknowledgment
+TBlock is currently mainained by [Twann](https://codeberg.org/twann), who is
+also its creator. A big thank you to all the people [who contribute(d) to the
+project](https://codeberg.org/tblock/tblock/src/branch/main/CONTRIBUTORS.md).
+## Credits Here is a list of all libraries used in the project: | Name | Author
+| License | | --- | --- | --- | | [colorama](https://github.com/tartley/
+colorama) | Jonathan Hartley | BSD | | [requests](https://
+requests.readthedocs.io/) | Kenneth Reitz | Apache 2.0 | | [urllib3](https://
+urllib3.readthedocs.io/) | Andrey Petrov | MIT | | [argumentor](https://
+codeberg.org/twann/python-argumentor) | Twann | LGPLv3 | It is also worth
+mentioning [pacman](https://archlinux.org/pacman/), from which TBlock's
+command-line design is highly inspired. ## Contact - [Mastodon](https://
+fosstodon.org/@tblock) - [Matrix](https://matrix.to/#/#tblock:matrix.org) -
+[XMPP](xmpp:tblockproject@chat.disroot.org?join) ## License [![GPLv3](https://
+www.gnu.org/graphics/gplv3-with-text-136x68.png)](https://www.gnu.org/licenses/
+gpl-3.0) This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by the Free
+Software Foundation, either version 3 of the License, or (at your option) any
+later version. This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
+or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for
+more details. You should have received a copy of the GNU General Public License
+along with this program. If not, see
 www.gnu.org/licenses/>.
```

### Comparing `tblock-2.6.1/README.md` & `tblock-2.7.1/tblock.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,42 @@
+Metadata-Version: 2.1
+Name: tblock
+Version: 2.7.1
+Summary: An anti-capitalist ad-blocker that uses the hosts file
+Home-page: https://tblock.codeberg.page/
+Author: Twann
+Author-email: tw4nn@disroot.org
+License: GPLv3
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
-<img align="center" src="https://codeberg.org/tblock/tblock/raw/branch/main/assets/icons/tblock.svg" alt="TBlock logo" width="220px">
+<img align="center" src="https://codeberg.org/tblock/tblock-gui/raw/commit/2456e9651103baef81f3a6c25cce97bf9d0252ee/assets/banner.png">
 </p>
 <p align="center">
 <h1 align="center">TBlock</h1>
 </p>
 <p align="center">
-<a href="https://github.com/humanetech-community/awesome-humane-tech"><img src="https://codeberg.org/tblock/tblock/raw/branch/main/assets/icons/humane-tech-badge.svg" alt="Awesome Humane Tech"></a>
+<a href="https://github.com/humanetech-community/awesome-humane-tech"><img src="https://codeberg.org/tblock/tblock/raw/branch/main/extra/icons/humane-tech-badge.svg" alt="Awesome Humane Tech"></a>
 <a href="https://framagit.org/twann/tblock/-/pipelines"><img src="https://framagit.org/twann/tblock/badges/main/pipeline.svg" alt="Pipeline status"></a>
 <a href="https://nogithub.codeberg.page"><img src="https://nogithub.codeberg.page/badge.svg" alt="Please don't upload to GitHub"></a>
 </p>
 
 ## Description
 
 TBlock is a free and open-source system-wide ad-blocker that is compatible with most filter list formats.
 
-## Features
-
-- Blocks ads and trackers system-wide
-- Compatible with most filter list formats
-- Has an online repository to help you find and subscribe to popular blocklists in an easy way
-- Has a built-in filter list converter
-- Has a built-in daemon that regularly updates the filter lists and prevents your hosts file from being modified by other programs and users
+To view the repository for the graphical user interface, [click here](https://codeberg.org/tblock/tblock-gui).
 
 ## Installation
 
 You can easily install TBlock with:
 
 ```sh
 pipx install tblock
@@ -36,40 +48,40 @@
 
 After installing, you need to setup TBlock in order to enable protection against ads and trackers:
 
 ```sh
 tblock --init
 ```
 
-You can learn more by reading [the documentation](https://tblock.codeberg.page/docs/).
+You can learn more by reading [the documentation](https://docs.tblock.me/).
+
+## Demo
+
+[![asciicast](https://asciinema.org/a/589465.svg)](https://asciinema.org/a/589465)
 
 ## Roadmap
 
 Here is a list of the upcoming changes in TBlock code. Suggestions are, of course, welcome.
 
-- [ ] ~~Mark filter lists that are included in another list as `subscribed` when the user subscribes to the list~~
-- [x] ~~Allow virtual filter lists to exist (would act as a "group", like `base-devel` does on Arch Linux)~~*
-- [ ] Implement a GUI for TBlock
+- [x] Implement [a GUI for TBlock](https://codeberg.org/tblock/tblock-gui)
 - [ ] Rewrite the entire code, make a clearer public API and publish release 3.0.0
 
-> *This feature is now available [as profiles](https://tblock.codeberg.page/docs/profiles.html).
-
 ## Contributing
 
-Everyone ([?](https://codeberg.org/tblock/tblock/src/branch/main/CONTRIBUTING.md#limitations)) is welcome to contribute to TBlock in different ways. Bug reports can be made directly from the [Gitea issue tracker](https://codeberg.org/tblock/tblock/issues), by sending an email to the team or in [our Matrix room](https://matrix.to/#/#tblock:envs.net). 
+Everyone is welcome to contribute to TBlock in different ways. Bug reports can be made directly from the [Gitea issue tracker](https://codeberg.org/tblock/tblock/issues), by sending an email to the team or in [our Matrix room](https://matrix.to/#/#tblock:envs.net). 
 
 If you want to suggest a modification in the code, you can [open a pull request](https://codeberg.org/tblock/tblock/pulls) or send your patch using email or Matrix.
 
 If you want to be a beta-tester, you can install the latest beta version from our [release page](https://codeberg.org/tblock/tblock/releases) and contact us to give a feedback.
 
 You can find more information on how to contribute [here](https://codeberg.org/tblock/tblock/src/branch/main/CONTRIBUTING.md).
 
 ## Support
 
-The best way to support is to [contribute](#contributing). If you want, you can also [make a donation](https://tblock.codeberg.page/donate).
+The best way to support is to [contribute](#contributing). If you want, you can also [make a donation](https://tblock.me/donate).
 
 ## Authors and acknowledgment
 
 TBlock is currently mainained by [Twann](https://codeberg.org/twann), who is also its creator.
 A big thank you to all the people [who contribute(d) to the project](https://codeberg.org/tblock/tblock/src/branch/main/CONTRIBUTORS.md).
 
 ## Credits
@@ -83,27 +95,18 @@
 | [urllib3](https://urllib3.readthedocs.io/) | Andrey Petrov | MIT |
 | [argumentor](https://codeberg.org/twann/python-argumentor) | Twann | LGPLv3 |
 
 It is also worth mentioning [pacman](https://archlinux.org/pacman/), from which TBlock's command-line design is highly inspired.
 
 ## Contact
 
-- [Blog](https://fediverse.blog/~/TBlock)
 - [Mastodon](https://fosstodon.org/@tblock)
 - [Matrix](https://matrix.to/#/#tblock:matrix.org)
-- [Telegram](https://t.me/tblock)
 - [XMPP](xmpp:tblockproject@chat.disroot.org?join)
 
-## Screenshots
-
-<p align="center">
-    <img src="https://codeberg.org/tblock/tblock/raw/branch/main/assets/screenshots/screenshot2.png">
-    <img src="https://codeberg.org/tblock/tblock/raw/branch/main/assets/screenshots/screenshot1.png">
-</p>
-
 ## License
 
 [![GPLv3](https://www.gnu.org/graphics/gplv3-with-text-136x68.png)](https://www.gnu.org/licenses/gpl-3.0)
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

#### html2text {}

```diff
@@ -1,63 +1,62 @@
-                                 [TBlock logo]
+Metadata-Version: 2.1 Name: tblock Version: 2.7.1 Summary: An anti-capitalist
+ad-blocker that uses the hosts file Home-page: https://tblock.codeberg.page/
+Author: Twann Author-email: tw4nn@disroot.org License: GPLv3 Classifier:
+Environment :: Console Classifier: License :: OSI Approved :: GNU General
+Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent Description-Content-Type: text/
+markdown License-File: LICENSE
+              [https://codeberg.org/tblock/tblock-gui/raw/commit/
+          2456e9651103baef81f3a6c25cce97bf9d0252ee/assets/banner.png]
                              ****** TBlock ******
     [Awesome_Humane_Tech] [Pipeline_status] [Please_don't_upload_to_GitHub]
 ## Description TBlock is a free and open-source system-wide ad-blocker that is
-compatible with most filter list formats. ## Features - Blocks ads and trackers
-system-wide - Compatible with most filter list formats - Has an online
-repository to help you find and subscribe to popular blocklists in an easy way
-- Has a built-in filter list converter - Has a built-in daemon that regularly
-updates the filter lists and prevents your hosts file from being modified by
-other programs and users ## Installation You can easily install TBlock with:
-```sh pipx install tblock ``` More installation methods â such as Windows
-installer and packages for Linux distributions â can be found [on the
-website](https://tblock.codeberg.page/install). ## Usage After installing, you
-need to setup TBlock in order to enable protection against ads and trackers:
-```sh tblock --init ``` You can learn more by reading [the documentation]
-(https://tblock.codeberg.page/docs/). ## Roadmap Here is a list of the upcoming
-changes in TBlock code. Suggestions are, of course, welcome. - [ ] ~~Mark
-filter lists that are included in another list as `subscribed` when the user
-subscribes to the list~~ - [x] ~~Allow virtual filter lists to exist (would act
-as a "group", like `base-devel` does on Arch Linux)~~* - [ ] Implement a GUI
-for TBlock - [ ] Rewrite the entire code, make a clearer public API and publish
-release 3.0.0 > *This feature is now available [as profiles](https://
-tblock.codeberg.page/docs/profiles.html). ## Contributing Everyone ([?](https:/
-/codeberg.org/tblock/tblock/src/branch/main/CONTRIBUTING.md#limitations)) is
-welcome to contribute to TBlock in different ways. Bug reports can be made
-directly from the [Gitea issue tracker](https://codeberg.org/tblock/tblock/
-issues), by sending an email to the team or in [our Matrix room](https://
-matrix.to/#/#tblock:envs.net). If you want to suggest a modification in the
-code, you can [open a pull request](https://codeberg.org/tblock/tblock/pulls)
-or send your patch using email or Matrix. If you want to be a beta-tester, you
-can install the latest beta version from our [release page](https://
-codeberg.org/tblock/tblock/releases) and contact us to give a feedback. You can
-find more information on how to contribute [here](https://codeberg.org/tblock/
-tblock/src/branch/main/CONTRIBUTING.md). ## Support The best way to support is
-to [contribute](#contributing). If you want, you can also [make a donation]
-(https://tblock.codeberg.page/donate). ## Authors and acknowledgment TBlock is
-currently mainained by [Twann](https://codeberg.org/twann), who is also its
-creator. A big thank you to all the people [who contribute(d) to the project]
-(https://codeberg.org/tblock/tblock/src/branch/main/CONTRIBUTORS.md). ##
-Credits Here is a list of all libraries used in the project: | Name | Author |
-License | | --- | --- | --- | | [colorama](https://github.com/tartley/colorama)
-| Jonathan Hartley | BSD | | [requests](https://requests.readthedocs.io/) |
-Kenneth Reitz | Apache 2.0 | | [urllib3](https://urllib3.readthedocs.io/) |
-Andrey Petrov | MIT | | [argumentor](https://codeberg.org/twann/python-
-argumentor) | Twann | LGPLv3 | It is also worth mentioning [pacman](https://
-archlinux.org/pacman/), from which TBlock's command-line design is highly
-inspired. ## Contact - [Blog](https://fediverse.blog/~/TBlock) - [Mastodon]
-(https://fosstodon.org/@tblock) - [Matrix](https://matrix.to/#/#tblock:
-matrix.org) - [Telegram](https://t.me/tblock) - [XMPP](xmpp:
-tblockproject@chat.disroot.org?join) ## Screenshots
-    [https://codeberg.org/tblock/tblock/raw/branch/main/assets/screenshots/
- screenshot2.png] [https://codeberg.org/tblock/tblock/raw/branch/main/assets/
-                         screenshots/screenshot1.png]
-## License [![GPLv3](https://www.gnu.org/graphics/gplv3-with-text-136x68.png)]
-(https://www.gnu.org/licenses/gpl-3.0) This program is free software: you can
-redistribute it and/or modify it under the terms of the GNU General Public
-License as published by the Free Software Foundation, either version 3 of the
-License, or (at your option) any later version. This program is distributed in
-the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the
-implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See
-the GNU General Public License for more details. You should have received a
-copy of the GNU General Public License along with this program. If not, see
+compatible with most filter list formats. To view the repository for the
+graphical user interface, [click here](https://codeberg.org/tblock/tblock-gui).
+## Installation You can easily install TBlock with: ```sh pipx install tblock
+``` More installation methods â such as Windows installer and packages for
+Linux distributions â can be found [on the website](https://
+tblock.codeberg.page/install). ## Usage After installing, you need to setup
+TBlock in order to enable protection against ads and trackers: ```sh tblock --
+init ``` You can learn more by reading [the documentation](https://
+docs.tblock.me/). ## Demo [![asciicast](https://asciinema.org/a/589465.svg)]
+(https://asciinema.org/a/589465) ## Roadmap Here is a list of the upcoming
+changes in TBlock code. Suggestions are, of course, welcome. - [x] Implement [a
+GUI for TBlock](https://codeberg.org/tblock/tblock-gui) - [ ] Rewrite the
+entire code, make a clearer public API and publish release 3.0.0 ##
+Contributing Everyone is welcome to contribute to TBlock in different ways. Bug
+reports can be made directly from the [Gitea issue tracker](https://
+codeberg.org/tblock/tblock/issues), by sending an email to the team or in [our
+Matrix room](https://matrix.to/#/#tblock:envs.net). If you want to suggest a
+modification in the code, you can [open a pull request](https://codeberg.org/
+tblock/tblock/pulls) or send your patch using email or Matrix. If you want to
+be a beta-tester, you can install the latest beta version from our [release
+page](https://codeberg.org/tblock/tblock/releases) and contact us to give a
+feedback. You can find more information on how to contribute [here](https://
+codeberg.org/tblock/tblock/src/branch/main/CONTRIBUTING.md). ## Support The
+best way to support is to [contribute](#contributing). If you want, you can
+also [make a donation](https://tblock.me/donate). ## Authors and acknowledgment
+TBlock is currently mainained by [Twann](https://codeberg.org/twann), who is
+also its creator. A big thank you to all the people [who contribute(d) to the
+project](https://codeberg.org/tblock/tblock/src/branch/main/CONTRIBUTORS.md).
+## Credits Here is a list of all libraries used in the project: | Name | Author
+| License | | --- | --- | --- | | [colorama](https://github.com/tartley/
+colorama) | Jonathan Hartley | BSD | | [requests](https://
+requests.readthedocs.io/) | Kenneth Reitz | Apache 2.0 | | [urllib3](https://
+urllib3.readthedocs.io/) | Andrey Petrov | MIT | | [argumentor](https://
+codeberg.org/twann/python-argumentor) | Twann | LGPLv3 | It is also worth
+mentioning [pacman](https://archlinux.org/pacman/), from which TBlock's
+command-line design is highly inspired. ## Contact - [Mastodon](https://
+fosstodon.org/@tblock) - [Matrix](https://matrix.to/#/#tblock:matrix.org) -
+[XMPP](xmpp:tblockproject@chat.disroot.org?join) ## License [![GPLv3](https://
+www.gnu.org/graphics/gplv3-with-text-136x68.png)](https://www.gnu.org/licenses/
+gpl-3.0) This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by the Free
+Software Foundation, either version 3 of the License, or (at your option) any
+later version. This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
+or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for
+more details. You should have received a copy of the GNU General Public License
+along with this program. If not, see
 www.gnu.org/licenses/>.
```

### Comparing `tblock-2.6.1/setup.py` & `tblock-2.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
```

### Comparing `tblock-2.6.1/tblock/__init__.py` & `tblock-2.7.1/tblock/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -25,18 +25,18 @@
 from .config import hosts_are_safe, Path
 from .filters import (
     subscribe,
     subscribe_custom,
     update,
     update_all,
     rename_custom,
+    change_permissions,
     sync_filter_list_repo,
     get_all_filter_lists,
     unsubscribe,
-    change_permissions,
     Filter,
     purge_cache,
     get_active_filter_lists_count,
     get_search_results_filter_lists,
 )
 from .rules import (
     allow_domains,
@@ -64,14 +64,16 @@
 # Simplify rule policies
 ALLOW = RulePolicy.ALLOW
 BLOCK = RulePolicy.BLOCK
 REDIRECT = RulePolicy.REDIRECT
 del RulePolicy
 
 # Simplify config variables
-DEFAULT_PERMISSIONS = Var.DEFAULT_PERMISSIONS
-DEFAULT_PERMISSIONS_CUSTOM = Var.DEFAULT_PERMISSIONS_CUSTOM
 DEFAULT_IP = Var.DEFAULT_IP
 REPO_MIRRORS = Var.REPO_MIRRORS
 ALLOW_IPV6 = Var.ALLOW_IPV6
 DEFAULT_IPV6 = Var.DEFAULT_IPV6
 del Var
+
+# This doesn't do anything, it is just kept here for compatibility purposes
+DEFAULT_PERMISSIONS = FilterPermissions("AB")
+DEFAULT_PERMISSIONS_CUSTOM = FilterPermissions("AB")
```

### Comparing `tblock-2.6.1/tblock/__main__.py` & `tblock-2.7.1/tblock/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
```

### Comparing `tblock-2.6.1/tblock/argumentor/__init__.py` & `tblock-2.7.1/tblock/argumentor/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 # argumentor - A simple, copylefted, lightweight library to work with command-line arguments in Python
 # Licensed under LGPLv3
 # Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
 
 import sys
 import re
-from .exceptions import ExecNameError, OperationExistsError, OptionExistsError, ArgumentValueError, GroupExistsError, \
-    GroupNotExistsError, InvalidOptionError, InvalidOperationError
+from .exceptions import (
+    ExecNameError,
+    OperationExistsError,
+    OptionExistsError,
+    ArgumentValueError,
+    GroupExistsError,
+    GroupNotExistsError,
+    InvalidOptionError,
+    InvalidOperationError,
+)
 
-__version__ = '1.0.0'
+__version__ = "1.1.0"
 
 
 class Arguments:
-
-    def __init__(self, arguments: list = None, exec_name: str = None, help_page: str = None,
-                 one_operation_required: bool = True, allow_short_args_together: bool = True,
-                 show_operation_groups_on_help_page: bool = True, show_option_groups_on_help_page: bool = True,
-                 copyright_header: str = None, more_info_footer: str = None) -> None:
+    def __init__(
+        self,
+        arguments: list = None,
+        exec_name: str = None,
+        help_page: str = None,
+        one_operation_required: bool = True,
+        allow_short_args_together: bool = True,
+        show_operation_groups_on_help_page: bool = True,
+        show_option_groups_on_help_page: bool = True,
+        copyright_header: str = None,
+        more_info_footer: str = None,
+    ) -> None:
         """
         Argumentor parser object
         :param arguments: Optional. Arguments to parse. If not set, sys.argv[1:] will be used
         :param exec_name: Optional. The name of the executable running. If not set, sys.argv[0] will be used
         :param help_page: Optional. Specify a custom help page as self.help_page. If None, argumentor will generate one
         :param one_operation_required: Defaults to True. If no operation is specified, the script will return an error
         :param allow_short_args_together: Defaults to True. Allow short arguments to be combined
@@ -34,33 +49,37 @@
             self.arguments = sys.argv[1:]
         else:
             self.arguments = arguments
 
         if len(sys.argv) >= 1 and exec_name is None:
             self.exec_name = sys.argv[0]
         elif exec_name is None:
-            raise ExecNameError('cannot find executable name')
+            raise ExecNameError("cannot find executable name")
         else:
             self.exec_name = exec_name
 
-        self.one_operation_required = one_operation_required            # One operation is required
-        self.allow_short_args_together = allow_short_args_together      # Allow short args to be combined
-
-        self.operations = {}                                            # Available operations
-        self.short_operations = {}                                      # Available short operations
-        self.operation_groups = {}                                      # Existing operation groups
-        self.options = {}                                               # Available options
-        self.short_options = {}                                         # Available short options
-        self.option_groups = {}                                         # Existing option groups
+        self.one_operation_required = (
+            one_operation_required  # One operation is required
+        )
+        self.allow_short_args_together = (
+            allow_short_args_together  # Allow short args to be combined
+        )
+
+        self.operations = {}  # Available operations
+        self.short_operations = {}  # Available short operations
+        self.operation_groups = {}  # Existing operation groups
+        self.options = {}  # Available options
+        self.short_options = {}  # Available short options
+        self.option_groups = {}  # Existing option groups
 
-        self.active_operation = None                                    # The operation that is running
-        self.isolate_unmatched = True                                   # Invalid args are stored as operation value
+        self.active_operation = None  # The operation that is running
+        self.isolate_unmatched = True  # Invalid args are stored as operation value
 
-        self.output_operations = {}                                     # Operations result after parsing
-        self.output_options = {}                                        # Options result after parsing
+        self.output_operations = {}  # Operations result after parsing
+        self.output_options = {}  # Options result after parsing
 
         self.show_operation_groups_on_help_page = show_operation_groups_on_help_page
         self.show_option_groups_on_help_page = show_option_groups_on_help_page
         self.copyright_header = copyright_header
         self.more_info_footer = more_info_footer
 
         if help_page:
@@ -70,170 +89,202 @@
             self.help_page = self.__generate_help_page()
             self.generate_help_page = True
 
     def __generate_help_page(self) -> str:
         """
         :return: str: The help page
         """
-        output = ''
+        output = ""
         if self.copyright_header is not None:
-            output += f'{self.copyright_header}\n'
+            output += f"{self.copyright_header}\n"
 
         if self.operations is not None and self.options is None:
-            output += f'usage: {self.exec_name} [operation] [arg(s)]\n\n'
+            output += f"usage: {self.exec_name} [operation] [arg(s)]\n\n"
         elif self.operations is None and self.options is not None:
-            output += f'usage: {self.exec_name} [option(s)] [arg(s)]\n\n'
+            output += f"usage: {self.exec_name} [option(s)] [arg(s)]\n\n"
         elif self.operations is not None and self.options is not None:
-            output += f'usage: {self.exec_name} [operation] [option(s)] [arg(s)]\n\n'
+            output += f"usage: {self.exec_name} [operation] [option(s)] [arg(s)]\n\n"
         else:
-            output += f'usage: {self.exec_name} [arg(s)]\n\n'
+            output += f"usage: {self.exec_name} [arg(s)]\n\n"
 
         if self.operations != {}:
-            output += '<operations>\n'
+            output += "<operations>\n"
 
             for operation in self.operations:
-                if self.operations[operation]['group'] is None:
-                    line = ''
-                    if self.operations[operation]['short_operation'] is not None:
-                        line += f'  {self.operations[operation]["short_operation"]}'
-                    line += f'  {operation}'
-                    if self.operations[operation]['description'] is not None:
-                        if len(line) > 15:
-                            line += f'\t\t\t{self.operations[operation]["description"]}\n'
+                if self.operations[operation]["group"] is None:
+                    line = ""
+                    if not self.operations[operation]["hidden"]:
+                        if self.operations[operation]["short_operation"] is not None:
+                            line += f'  {self.operations[operation]["short_operation"]}'
+                        line += f"  {operation}"
+                        if self.operations[operation]["description"] is not None:
+                            if len(line) > 15:
+                                line += f'\t\t\t{self.operations[operation]["description"]}\n'
+                            else:
+                                line += f'\t\t\t\t{self.operations[operation]["description"]}\n'
                         else:
-                            line += f'\t\t\t\t{self.operations[operation]["description"]}\n'
-                    else:
-                        line += '\n'
-                    output += line
+                            line += "\n"
+                        output += line
             for group in self.operation_groups.keys():
                 if self.show_operation_groups_on_help_page:
                     if self.operation_groups[group]["name"]:
                         output += f'* {self.operation_groups[group]["name"]}\n'
                     else:
-                        output += f'* {group}\n'
+                        output += f"* {group}\n"
                 for operation in self.__get_operations_from_group(group):
-                    line = ''
-                    if self.operations[operation]['short_operation'] is not None:
-                        line += f'  {self.operations[operation]["short_operation"]}'
-                    line += f'  {operation}'
-                    if self.operations[operation]['description'] is not None:
-                        if len(line) > 15:
-                            line += f'\t\t\t{self.operations[operation]["description"]}\n'
+                    line = ""
+                    if not self.operations[operation]["hidden"]:
+                        if self.operations[operation]["short_operation"] is not None:
+                            line += f'  {self.operations[operation]["short_operation"]}'
+                        line += f"  {operation}"
+                        if self.operations[operation]["description"] is not None:
+                            if len(line) > 15:
+                                line += f'\t\t\t{self.operations[operation]["description"]}\n'
+                            else:
+                                line += f'\t\t\t\t{self.operations[operation]["description"]}\n'
                         else:
-                            line += f'\t\t\t\t{self.operations[operation]["description"]}\n'
-                    else:
-                        line += '\n'
-                    output += line
+                            line += "\n"
+                        output += line
 
         if self.options != {}:
-            output += '\n<options>\n'
+            output += "\n<options>\n"
 
             for option in self.options:
-                if self.options[option]['group'] is None:
-                    line = ''
-                    if self.options[option]['short_option'] is not None:
-                        line += f'  {self.options[option]["short_option"]}'
-                    line += f'  {option}'
-                    if self.options[option]['description'] is not None:
-                        if len(line) > 15:
-                            line += f'\t\t\t{self.options[option]["description"]}\n'
+                if self.options[option]["group"] is None:
+                    line = ""
+                    if not self.options[option]["hidden"]:
+                        if self.options[option]["short_option"] is not None:
+                            line += f'  {self.options[option]["short_option"]}'
+                        line += f"  {option}"
+                        if self.options[option]["description"] is not None:
+                            if len(line) > 15:
+                                line += f'\t\t\t{self.options[option]["description"]}\n'
+                            else:
+                                line += (
+                                    f'\t\t\t\t{self.options[option]["description"]}\n'
+                                )
                         else:
-                            line += f'\t\t\t\t{self.options[option]["description"]}\n'
-                    else:
-                        line += '\n'
-                    output += line
+                            line += "\n"
+                        output += line
             for group in self.option_groups.keys():
                 if self.show_option_groups_on_help_page:
                     if self.option_groups[group]["name"]:
                         output += f'* {self.option_groups[group]["name"]}\n'
                     else:
-                        output += f'* {group}\n'
+                        output += f"* {group}\n"
                 for option in self.__get_options_from_group(group):
-                    line = ''
-                    if self.options[option]['short_option'] is not None:
-                        line += f'  {self.options[option]["short_option"]}'
-                    line += f'  {option}'
-                    if self.options[option]['description'] is not None:
-                        if len(line) > 15:
-                            line += f'\t\t\t{self.options[option]["description"]}\n'
+                    line = ""
+                    if not self.options[option]["hidden"]:
+                        if self.options[option]["short_option"] is not None:
+                            line += f'  {self.options[option]["short_option"]}'
+                        line += f"  {option}"
+                        if self.options[option]["description"] is not None:
+                            if len(line) > 15:
+                                line += f'\t\t\t{self.options[option]["description"]}\n'
+                            else:
+                                line += (
+                                    f'\t\t\t\t{self.options[option]["description"]}\n'
+                                )
                         else:
-                            line += f'\t\t\t\t{self.options[option]["description"]}\n'
-                    else:
-                        line += '\n'
-                    output += line
+                            line += "\n"
+                        output += line
 
         if self.more_info_footer is not None:
-            output += f'\n{self.more_info_footer}'
+            output += f"\n{self.more_info_footer}"
         return output
 
     def __get_operations_from_group(self, group: str) -> list:
         if group not in self.operation_groups:
             raise GroupNotExistsError(f'operation group "{group}" does not exist')
         else:
-            return self.operation_groups[group]['operations']
+            return self.operation_groups[group]["operations"]
 
     def __get_options_from_group(self, group: str) -> list:
         if group not in self.option_groups:
             raise GroupNotExistsError(f'option group "{group}" does not exist')
         else:
-            return self.option_groups[group]['options']
+            return self.option_groups[group]["options"]
 
-    def add_operation(self, operation: str, value_type, description: str = None,
-                      short_operation: str = None, required: bool = False, group: str = None,
-                      default_value=None) -> None:
+    def add_operation(
+        self,
+        operation: str,
+        value_type,
+        description: str = None,
+        short_operation: str = None,
+        required: bool = False,
+        group: str = None,
+        hidden: bool = False,
+        default_value=None,
+    ) -> None:
         """
         Add an operation to the list of supported arguments
         :param operation: The operation (ex. '--help')
         :param value_type: The type of the value to catch (bool, str, int, list).
         :param description: Optional. The description of what the operation does
         :param short_operation: Optional. The short version of the operation (ex. '-h')
         :param required: Defaults to False. Choose if the operation is required or not
         :param group: Optional. Specify an operation group
+        :param hidden: Hide operation from help page
         :param default_value. Specify the default value to use if the argument is not passed. Defaults to None
         (or False for bool).
 
         :return:
         """
         if operation in self.operations.keys():
             raise OperationExistsError(f'operation "{operation}" already exists')
         elif operation in self.options.keys():
             raise OptionExistsError(f'option "{operation}" already exists')
-        elif short_operation is not None and short_operation in self.short_operations.keys():
-            raise OperationExistsError(f'short operation "{short_operation}" already exists')
-        elif short_operation is not None and short_operation in self.short_options.keys():
+        elif (
+            short_operation is not None
+            and short_operation in self.short_operations.keys()
+        ):
+            raise OperationExistsError(
+                f'short operation "{short_operation}" already exists'
+            )
+        elif (
+            short_operation is not None and short_operation in self.short_options.keys()
+        ):
             raise OptionExistsError(f'short option "{short_operation}" already exists')
         elif value_type not in [bool, str, int, list]:
             raise ArgumentValueError(f'value type "{value_type}" is not supported')
         elif group is not None and group not in self.operation_groups:
             raise GroupNotExistsError(f'operation group "{group}" does not exist')
-        elif short_operation is not None and len(short_operation) > 1 and not re.match(r'-[A-z\d]', short_operation):
+        elif (
+            short_operation is not None
+            and len(short_operation) > 1
+            and not re.match(r"-[A-z\d]", short_operation)
+        ):
             raise InvalidOperationError(
-                f'short operation can only be one-character long when no dash, not "{short_operation}"')
+                f'short operation can only be one-character long when no dash, not "{short_operation}"'
+            )
         elif short_operation is not None and len(short_operation) > 2:
             raise InvalidOperationError(
-                f'short operation can contain a dash and a character maximum, not "{short_operation}"')
+                f'short operation can contain a dash and a character maximum, not "{short_operation}"'
+            )
         elif short_operation == operation:
-            raise InvalidOperationError('short operation is equal to long operation')
+            raise InvalidOperationError("short operation is equal to long operation")
         else:
             if default_value is None and value_type == bool:
                 default_value = False
             elif default_value is not None and type(default_value) != value_type:
                 raise ArgumentValueError(
-                    f'default value for operation {operation} is from '
-                    f'type "{type(default_value)}" instead of "{value_type}"')
+                    f"default value for operation {operation} is from "
+                    f'type "{type(default_value)}" instead of "{value_type}"'
+                )
             self.operations[operation] = {
-                'value_type': value_type,
-                'description': description,
-                'required': required,
-                'group': group,
-                'short_operation': short_operation,
-                'default_value': default_value
+                "value_type": value_type,
+                "description": description,
+                "required": required,
+                "group": group,
+                "short_operation": short_operation,
+                "default_value": default_value,
+                "hidden": hidden,
             }
             if group is not None:
-                self.operation_groups[group]['operations'].append(operation)
+                self.operation_groups[group]["operations"].append(operation)
             if short_operation is not None:
                 self.short_operations[short_operation] = operation
             if self.generate_help_page:
                 self.help_page = self.__generate_help_page()
 
     def add_operation_group(self, group_name: str, name: str = None) -> None:
         """
@@ -242,109 +293,151 @@
         :param name: Optional. Specify a different name to show on the help page.
         :return:
         """
 
         if group_name in self.operation_groups:
             raise GroupExistsError(f'operation group "{group_name}" already exists')
         else:
-            self.operation_groups[group_name] = {'operations': [], 'name': name}
+            self.operation_groups[group_name] = {"operations": [], "name": name}
 
-    def add_option(self, option: str, value_type, description: str = None,
-                   short_option: str = None, required: bool = False, available_with_operations: list = None,
-                   required_by_operations: list = None, available_with_groups: list = None,
-                   required_by_groups: list = None, group: str = None, inherit_from_group: bool = True,
-                   default_value=None) -> None:
+    def add_option(
+        self,
+        option: str,
+        value_type,
+        description: str = None,
+        short_option: str = None,
+        required: bool = False,
+        available_with_operations: list = None,
+        required_by_operations: list = None,
+        available_with_groups: list = None,
+        required_by_groups: list = None,
+        group: str = None,
+        inherit_from_group: bool = True,
+        hidden: bool = False,
+        default_value=None,
+    ) -> None:
         """
         Add an option to the list of supported arguments
         :param option: The option (ex. '--force')
         :param value_type: The type of the value to catch (bool, str, int, list).
         :param description: Optional. The description of what the operation does
         :param short_option: Optional. The short version of the operation (ex. '-f')
         :param required: Defaults to False. Choose if the operation is required or not
         :param available_with_operations: Optional. Option will only be available with operation in the list
         :param required_by_operations: Optional. Every operation in the list will fail without this option
         :param available_with_groups: Optional. Option will only be available with operation in the specified groups
         :param required_by_groups: Optional. Every operation in the specified groups will fail without this option
         :param group: Optional. Specify an option group
         :param inherit_from_group: Defaults to True. Inherit requirements and availability from group.
+        :param hidden: Hide option from help page
         :param default_value. Specify the default value to use if the argument is not passed. Defaults to None
         (or False for bool).
 
         :return:
         """
         if option in self.options.keys():
             raise OptionExistsError(f'option "{option}" already exists')
         elif option in self.operations.keys():
             raise OperationExistsError(f'operation "{option}" already exists')
         elif short_option is not None and short_option in self.short_options.keys():
             raise OptionExistsError(f'short option "{option}" already exists')
         elif short_option is not None and short_option in self.short_operations.keys():
-            raise OperationExistsError(f'short operation "{short_option}" already exists')
+            raise OperationExistsError(
+                f'short operation "{short_option}" already exists'
+            )
         elif value_type not in [bool, str, int, list]:
             raise ArgumentValueError(f'value type "{value_type}" is not supported')
         elif group is not None and group not in self.option_groups.keys():
             raise GroupNotExistsError(f'option group "{group}" does not exist')
-        elif not re.match(r'--[A-z\d\-]*', option):
-            raise InvalidOptionError(f'option should start with two dashes: "--", not "{short_option}"')
+        elif not re.match(r"--[A-z\d\-]*", option):
+            raise InvalidOptionError(
+                f'option should start with two dashes: "--", not "{short_option}"'
+            )
         elif short_option is not None and len(short_option) != 2:
-            raise InvalidOptionError(f'short option must be two-characters long, not "{short_option}"')
-        elif short_option is not None and not re.match(r'-[A-z\d]', short_option):
             raise InvalidOptionError(
-                f'short option must start with a dash and finish with a character, not "{short_option}"')
+                f'short option must be two-characters long, not "{short_option}"'
+            )
+        elif short_option is not None and not re.match(r"-[A-z\d]", short_option):
+            raise InvalidOptionError(
+                f'short option must start with a dash and finish with a character, not "{short_option}"'
+            )
         else:
             if default_value is None and value_type == bool:
                 default_value = False
             elif default_value is not None and type(default_value) != value_type:
                 raise ArgumentValueError(
-                    f'default value for operation {option} is '
-                    f'from type "{type(default_value)}" instead of "{value_type}"')
+                    f"default value for operation {option} is "
+                    f'from type "{type(default_value)}" instead of "{value_type}"'
+                )
             if group is not None and inherit_from_group:
                 self.options[option] = {
-                    'value_type': value_type,
-                    'description': description,
-                    'required': required,
-                    'group': group,
-                    'available_with_operations': self.option_groups[group]['available_with_operations'],
-                    'required_by_operations': self.option_groups[group]['required_by_operations'],
-                    'available_with_groups': self.option_groups[group]['available_with_groups'],
-                    'required_by_groups': self.option_groups[group]['required_by_groups'],
-                    'short_option': short_option,
-                    'default_value': default_value
+                    "value_type": value_type,
+                    "description": description,
+                    "required": required,
+                    "group": group,
+                    "available_with_operations": self.option_groups[group][
+                        "available_with_operations"
+                    ],
+                    "required_by_operations": self.option_groups[group][
+                        "required_by_operations"
+                    ],
+                    "available_with_groups": self.option_groups[group][
+                        "available_with_groups"
+                    ],
+                    "required_by_groups": self.option_groups[group][
+                        "required_by_groups"
+                    ],
+                    "short_option": short_option,
+                    "default_value": default_value,
+                    "hidden": hidden,
                 }
                 if available_with_operations is not None:
-                    self.options[option]['available_with_operations'] = available_with_operations
+                    self.options[option][
+                        "available_with_operations"
+                    ] = available_with_operations
                 if required_by_operations is not None:
-                    self.options[option]['required_by_operations'] = required_by_operations
+                    self.options[option][
+                        "required_by_operations"
+                    ] = required_by_operations
                 if available_with_groups is not None:
-                    self.options[option]['available_with_groups'] = available_with_groups
+                    self.options[option][
+                        "available_with_groups"
+                    ] = available_with_groups
                 if required_by_groups is not None:
-                    self.options[option]['required_by_groups'] = required_by_groups
+                    self.options[option]["required_by_groups"] = required_by_groups
             else:
                 self.options[option] = {
-                    'value_type': value_type,
-                    'description': description,
-                    'required': required,
-                    'group': group,
-                    'available_with_operations': available_with_operations,
-                    'required_by_operations': required_by_operations,
-                    'available_with_groups': available_with_groups,
-                    'required_by_groups': required_by_groups,
-                    'short_option': short_option,
-                    'default_value': default_value
+                    "value_type": value_type,
+                    "description": description,
+                    "required": required,
+                    "group": group,
+                    "available_with_operations": available_with_operations,
+                    "required_by_operations": required_by_operations,
+                    "available_with_groups": available_with_groups,
+                    "required_by_groups": required_by_groups,
+                    "short_option": short_option,
+                    "default_value": default_value,
+                    "hidden": hidden,
                 }
             if group is not None:
-                self.option_groups[group]['options'].append(option)
+                self.option_groups[group]["options"].append(option)
             if short_option is not None:
                 self.short_options[short_option] = option
             if self.generate_help_page:
                 self.help_page = self.__generate_help_page()
 
-    def add_option_group(self, group_name: str, name: str = None, available_with_operations: list = None,
-                         required_by_operations: list = None, available_with_groups: list = None,
-                         required_by_groups: list = None) -> None:
+    def add_option_group(
+        self,
+        group_name: str,
+        name: str = None,
+        available_with_operations: list = None,
+        required_by_operations: list = None,
+        available_with_groups: list = None,
+        required_by_groups: list = None,
+    ) -> None:
         """
         Create an option group
         :param group_name: The name of the groups
         :param name: Optional. Specify a different name to show on the help page.
         :param available_with_operations: Optional. Options will only be available with operation in the list
         :param required_by_operations: Optional. Every operation in the list will fail without these options
         :param available_with_groups: Optional. Options will only be available with operation in the specified groups
@@ -352,123 +445,163 @@
         :return:
         """
 
         if group_name in self.option_groups.keys():
             raise GroupExistsError(f'option group "{group_name}" already exists')
         else:
             self.option_groups[group_name] = {
-                'available_with_operations': available_with_operations,
-                'required_by_operations': required_by_operations,
-                'available_with_groups': available_with_groups,
-                'required_by_groups': required_by_groups,
-                'options': [],
-                'name': name
+                "available_with_operations": available_with_operations,
+                "required_by_operations": required_by_operations,
+                "available_with_groups": available_with_groups,
+                "required_by_groups": required_by_groups,
+                "options": [],
+                "name": name,
             }
 
-    def __match_operation(self, operation_title: str, real_operation: str, real_argument: str) -> None:
-
+    def __match_operation(
+        self, operation_title: str, real_operation: str, real_argument: str
+    ) -> None:
         if self.active_operation is None:
-
             self.active_operation = operation_title
 
             if len(real_argument.split("=")) == 2:
-                if self.operations[operation_title]['value_type'] == int:
+                if self.operations[operation_title]["value_type"] == int:
                     try:
-                        self.output_operations[operation_title] = int(real_argument.split("=")[1])
+                        self.output_operations[operation_title] = int(
+                            real_argument.split("=")[1]
+                        )
                         self.isolate_unmatched = False
                     except ValueError:
-                        print(f'Error: operation "{real_operation}" requires an integer')
+                        print(
+                            f'Error: operation "{real_operation}" requires an integer'
+                        )
                         raise SystemExit(1)
-                elif self.operations[operation_title]['value_type'] == str:
+                elif self.operations[operation_title]["value_type"] == str:
                     if real_argument.split("=")[1]:
-                        self.output_operations[operation_title] = str(real_argument.split("=")[1])
+                        self.output_operations[operation_title] = str(
+                            real_argument.split("=")[1]
+                        )
                         self.isolate_unmatched = False
                     else:
-                        print(f'Error: operation "{real_operation}" requires at least one argument')
+                        print(
+                            f'Error: operation "{real_operation}" requires at least one argument'
+                        )
                         raise SystemExit(1)
                 else:
-                    print(f'Error: operation "{real_operation}" does not support the "=" operator')
+                    print(
+                        f'Error: operation "{real_operation}" does not support the "=" operator'
+                    )
                     raise SystemExit(1)
-            elif self.operations[operation_title]['value_type'] == bool:
+            elif self.operations[operation_title]["value_type"] == bool:
                 self.output_operations[operation_title] = True
             elif len(self.arguments) - self.arguments.index(real_argument) > 1:
-                if self.operations[operation_title]['value_type'] == int:
+                if self.operations[operation_title]["value_type"] == int:
                     self.output_operations[operation_title] = None
                     self.isolate_unmatched = True
-                elif self.operations[operation_title]['value_type'] == str:
+                elif self.operations[operation_title]["value_type"] == str:
                     self.output_operations[operation_title] = None
                     self.isolate_unmatched = True
-                elif self.operations[operation_title]['value_type'] == list:
+                elif self.operations[operation_title]["value_type"] == list:
                     self.output_operations[operation_title] = []
                     self.isolate_unmatched = True
                 else:
-                    raise ArgumentValueError(f'invalid value type: "{self.operations[operation_title]["value_type"]}"')
+                    raise ArgumentValueError(
+                        f'invalid value type: "{self.operations[operation_title]["value_type"]}"'
+                    )
             else:
-                print(f'Error: operation "{real_operation}" requires at least one argument')
+                print(
+                    f'Error: operation "{real_operation}" requires at least one argument'
+                )
                 raise SystemExit(1)
         else:
-
-            print('Error: only one operation at the same time is supported')
+            print("Error: only one operation at the same time is supported")
             raise SystemExit(1)
 
-    def __match_option(self, option_title: str, real_option: str, real_argument: str) -> None:
-
-        if self.active_operation is not None and self.options[option_title]['available_with_operations'] is not None \
-                and self.active_operation not in self.options[option_title]['available_with_operations']:
-            print(f'Error: option "{real_option}" is not available with operation "{self.active_operation}"')
+    def __match_option(
+        self, option_title: str, real_option: str, real_argument: str
+    ) -> None:
+        if (
+            self.active_operation is not None
+            and self.options[option_title]["available_with_operations"] is not None
+            and self.active_operation
+            not in self.options[option_title]["available_with_operations"]
+        ):
+            print(
+                f'Error: option "{real_option}" is not available with operation "{self.active_operation}"'
+            )
             raise SystemExit(1)
 
-        elif self.active_operation is not None and self.options[option_title]['available_with_groups'] is not None \
-                and self.operations[self.active_operation]['group'] not in \
-                self.options[option_title]['available_with_groups']:
-            print(f'Error: option "{real_option}" is not available with operation "{self.active_operation}"')
+        elif (
+            self.active_operation is not None
+            and self.options[option_title]["available_with_groups"] is not None
+            and self.operations[self.active_operation]["group"]
+            not in self.options[option_title]["available_with_groups"]
+        ):
+            print(
+                f'Error: option "{real_option}" is not available with operation "{self.active_operation}"'
+            )
             raise SystemExit(1)
 
         else:
-
             if len(real_argument.split("=")) == 2:
-                if self.options[option_title]['value_type'] == int:
+                if self.options[option_title]["value_type"] == int:
                     try:
-                        self.output_options[option_title] = int(real_argument.split("=")[1])
+                        self.output_options[option_title] = int(
+                            real_argument.split("=")[1]
+                        )
                     except ValueError:
                         print(f'Error: option "{real_option}" requires an integer')
                         raise SystemExit(1)
-                elif self.options[option_title]['value_type'] == str:
+                elif self.options[option_title]["value_type"] == str:
                     if real_argument.split("=")[1]:
-                        self.output_options[option_title] = str(real_argument.split("=")[1])
+                        self.output_options[option_title] = str(
+                            real_argument.split("=")[1]
+                        )
                     else:
-                        print(f'Error: option "{real_option}" requires at least one argument')
+                        print(
+                            f'Error: option "{real_option}" requires at least one argument'
+                        )
                         raise SystemExit(1)
                 else:
-                    print(f'Error: option "{real_option}" does not support the "=" operator')
+                    print(
+                        f'Error: option "{real_option}" does not support the "=" operator'
+                    )
                     raise SystemExit(1)
-            elif self.options[option_title]['value_type'] == bool:
+            elif self.options[option_title]["value_type"] == bool:
                 self.output_options[option_title] = True
             elif len(self.arguments) - self.arguments.index(real_argument) > 1:
-                if self.options[option_title]['value_type'] == int:
+                if self.options[option_title]["value_type"] == int:
                     try:
-                        self.output_options[option_title] = int(self.arguments[self.arguments.index(real_argument) + 1])
+                        self.output_options[option_title] = int(
+                            self.arguments[self.arguments.index(real_argument) + 1]
+                        )
                     except ValueError:
                         print(f'Error: option "{real_option}" requires an integer')
                         raise SystemExit(1)
                     else:
                         self.arguments.pop(self.arguments.index(real_argument) + 1)
-                elif self.options[option_title]['value_type'] == str:
-                    self.output_options[option_title] = str(self.arguments[self.arguments.index(real_argument) + 1])
+                elif self.options[option_title]["value_type"] == str:
+                    self.output_options[option_title] = str(
+                        self.arguments[self.arguments.index(real_argument) + 1]
+                    )
                     self.arguments.pop(self.arguments.index(real_argument) + 1)
-                elif self.options[option_title]['value_type'] == list:
+                elif self.options[option_title]["value_type"] == list:
                     self.output_options[option_title] = []
-                    for value in self.arguments[self.arguments.index(real_argument) + 1:]:
-                        if re.match(r'-[A-z\d_.\-]*', value):
+                    for value in self.arguments[
+                        self.arguments.index(real_argument) + 1 :
+                    ]:
+                        if re.match(r"-[A-z\d_.\-]*", value):
                             break
                         else:
                             self.output_options[option_title].append(value)
                             self.arguments.remove(value)
                 else:
-                    raise ArgumentValueError(f'invalid value type: "{self.options[option_title]["value_type"]}"')
+                    raise ArgumentValueError(
+                        f'invalid value type: "{self.options[option_title]["value_type"]}"'
+                    )
             else:
                 print(f'Error: option "{real_option}" requires at least one argument')
                 raise SystemExit(1)
 
     def parse(self) -> [dict, dict]:
         """
         Parse all arguments and return matches
@@ -476,183 +609,245 @@
         """
 
         # Empty the output arguments to avoid problems if this function is used multiple times
         self.output_operations = {}
         self.output_options = {}
 
         for argument in self.arguments:
-
             if argument in self.operations.keys():
-
                 self.__match_operation(
                     operation_title=argument,
                     real_operation=argument,
-                    real_argument=argument
+                    real_argument=argument,
                 )
 
             elif argument in self.options.keys():
-
                 self.__match_option(
-                    option_title=argument,
-                    real_option=argument,
-                    real_argument=argument
+                    option_title=argument, real_option=argument, real_argument=argument
                 )
 
             elif argument in self.short_operations.keys():
-
                 self.__match_operation(
                     operation_title=self.short_operations[argument],
                     real_operation=argument,
-                    real_argument=argument
+                    real_argument=argument,
                 )
 
             elif argument in self.short_options.keys():
-
                 self.__match_option(
                     option_title=self.short_options[argument],
                     real_option=argument,
-                    real_argument=argument
+                    real_argument=argument,
                 )
 
-            elif len(argument.split("=")) == 2 and argument.split("=")[0] in self.operations.keys():
-
+            elif (
+                len(argument.split("=")) == 2
+                and argument.split("=")[0] in self.operations.keys()
+            ):
                 self.__match_operation(
                     operation_title=argument.split("=")[0],
                     real_operation=argument.split("=")[0],
-                    real_argument=argument
+                    real_argument=argument,
                 )
 
-            elif len(argument.split("=")) == 2 and argument.split("=")[0] in self.options.keys():
-
+            elif (
+                len(argument.split("=")) == 2
+                and argument.split("=")[0] in self.options.keys()
+            ):
                 self.__match_option(
                     option_title=argument.split("=")[0],
                     real_option=argument.split("=")[0],
-                    real_argument=argument
+                    real_argument=argument,
                 )
 
-            elif self.allow_short_args_together and len(argument) > 1 and \
-                    (argument[0:1] in self.short_operations.keys() or argument[0:2] in self.short_operations.keys()):
-
-                for character in argument.replace('-', ''):
-
-                    if character in self.short_operations.keys() or f'-{character}' in self.short_operations.keys():
-                        short_argument = character if character in self.short_operations.keys() else f'-{character}'
+            elif (
+                self.allow_short_args_together
+                and len(argument) > 1
+                and (
+                    argument[0:1] in self.short_operations.keys()
+                    or argument[0:2] in self.short_operations.keys()
+                )
+            ):
+                for character in argument.replace("-", ""):
+                    if (
+                        character in self.short_operations.keys()
+                        or f"-{character}" in self.short_operations.keys()
+                    ):
+                        short_argument = (
+                            character
+                            if character in self.short_operations.keys()
+                            else f"-{character}"
+                        )
 
                         self.__match_operation(
                             operation_title=self.short_operations[short_argument],
                             real_operation=short_argument,
-                            real_argument=argument
+                            real_argument=argument,
                         )
 
-                    elif character in self.short_options.keys() or f'-{character}' in self.short_options.keys():
-                        short_argument = character if character in self.short_options.keys() else f'-{character}'
+                    elif (
+                        character in self.short_options.keys()
+                        or f"-{character}" in self.short_options.keys()
+                    ):
+                        short_argument = (
+                            character
+                            if character in self.short_options.keys()
+                            else f"-{character}"
+                        )
 
                         self.__match_option(
                             option_title=self.short_options[short_argument],
                             real_option=short_argument,
-                            real_argument=argument
+                            real_argument=argument,
                         )
 
                     else:
                         print(f'Error: invalid argument "{character}" in "{argument}"')
                         raise SystemExit(1)
 
-            elif self.allow_short_args_together and len(argument) > 1 and argument[0:2] in self.short_options.keys():
-
-                for character in argument.replace('-', ''):
-
-                    if character in self.short_options.keys() or f'-{character}' in self.short_options.keys():
-                        short_argument = character if character in self.short_options.keys() else f'-{character}'
+            elif (
+                self.allow_short_args_together
+                and len(argument) > 1
+                and argument[0:2] in self.short_options.keys()
+            ):
+                for character in argument.replace("-", ""):
+                    if (
+                        character in self.short_options.keys()
+                        or f"-{character}" in self.short_options.keys()
+                    ):
+                        short_argument = (
+                            character
+                            if character in self.short_options.keys()
+                            else f"-{character}"
+                        )
 
                         self.__match_option(
                             option_title=self.short_options[short_argument],
                             real_option=short_argument,
-                            real_argument=argument
+                            real_argument=argument,
                         )
 
-                    elif character in self.short_operations.keys() or f'-{character}' in self.short_operations.keys():
-                        print('Error: operation must be specified before any other arguments')
+                    elif (
+                        character in self.short_operations.keys()
+                        or f"-{character}" in self.short_operations.keys()
+                    ):
+                        print(
+                            "Error: operation must be specified before any other arguments"
+                        )
                         raise SystemExit(1)
 
                     else:
                         print(f'Error: invalid argument "{character}" in "{argument}"')
                         raise SystemExit(1)
 
-            elif self.isolate_unmatched and self.active_operation is not None and \
-                    not re.match(r'-[A-z\d_.\-]*', argument) \
-                    and self.operations[self.active_operation]['value_type'] == list:
-
+            elif (
+                self.isolate_unmatched
+                and self.active_operation is not None
+                and not re.match(r"-[A-z\d_.\-]*", argument)
+                and self.operations[self.active_operation]["value_type"] == list
+            ):
                 self.output_operations[self.active_operation].append(argument)
 
-            elif self.isolate_unmatched and self.active_operation is not None and \
-                    not re.match(r'-[A-z\d_.\-]*', argument) \
-                    and self.operations[self.active_operation]['value_type'] == str and \
-                    self.output_operations[self.active_operation] is None:
-
+            elif (
+                self.isolate_unmatched
+                and self.active_operation is not None
+                and not re.match(r"-[A-z\d_.\-]*", argument)
+                and self.operations[self.active_operation]["value_type"] == str
+                and self.output_operations[self.active_operation] is None
+            ):
                 self.output_operations[self.active_operation] = argument
 
-            elif self.isolate_unmatched and self.active_operation is not None and \
-                    not re.match(r'-[A-z\d_.\-]*', argument) \
-                    and self.operations[self.active_operation]['value_type'] == int and \
-                    self.output_operations[self.active_operation] is None:
-
+            elif (
+                self.isolate_unmatched
+                and self.active_operation is not None
+                and not re.match(r"-[A-z\d_.\-]*", argument)
+                and self.operations[self.active_operation]["value_type"] == int
+                and self.output_operations[self.active_operation] is None
+            ):
                 try:
                     self.output_operations[self.active_operation] = int(argument)
                 except ValueError:
                     print(f'Error: operation "{argument}" requires an integer')
                     raise SystemExit(1)
 
             else:
-
                 print(f'Error: invalid argument "{argument}"')
                 raise SystemExit(1)
 
         # Check if all active operations that require a list, a str or an int have at least one value
         for active_operation in self.output_operations.keys():
-            if self.operations[active_operation]['value_type'] == list and \
-                    self.output_operations[active_operation] == []:
-                print(f'Error: operation "{active_operation}" requires at least one argument')
+            if (
+                self.operations[active_operation]["value_type"] == list
+                and self.output_operations[active_operation] == []
+            ):
+                print(
+                    f'Error: operation "{active_operation}" requires at least one argument'
+                )
                 raise SystemExit(1)
-            elif self.operations[active_operation]['value_type'] in (str, int) and \
-                    self.output_operations[active_operation] is None:
-                print(f'Error: operation "{active_operation}" requires at least one argument')
+            elif (
+                self.operations[active_operation]["value_type"] in (str, int)
+                and self.output_operations[active_operation] is None
+            ):
+                print(
+                    f'Error: operation "{active_operation}" requires at least one argument'
+                )
                 raise SystemExit(1)
 
         # Check if all required operations are active
         for operation in self.operations:
-            if self.operations[operation]['required'] and operation not in self.output_operations.keys():
+            if (
+                self.operations[operation]["required"]
+                and operation not in self.output_operations.keys()
+            ):
                 print(f'Error: operation "{operation}" is required')
                 raise SystemExit(1)
 
         # Check if all required options (by an operation or by the program) are available
         for option in self.options:
-            if self.options[option]['required'] and option not in self.output_options.keys():
+            if (
+                self.options[option]["required"]
+                and option not in self.output_options.keys()
+            ):
                 print(f'Error: option "{option}" is required')
                 raise SystemExit(1)
-            if self.options[option]['required_by_operations'] is not None and option not in self.output_options:
-                for required in self.options[option]['required_by_operations']:
+            if (
+                self.options[option]["required_by_operations"] is not None
+                and option not in self.output_options
+            ):
+                for required in self.options[option]["required_by_operations"]:
                     if required in self.output_operations.keys():
-                        print(f'Error: operation "{required}" requires the option "{option}"')
+                        print(
+                            f'Error: operation "{required}" requires the option "{option}"'
+                        )
                         raise SystemExit(1)
-            if self.options[option]['required_by_groups'] is not None and option not in self.output_options:
-                for required_group in self.options[option]['required_by_groups']:
+            if (
+                self.options[option]["required_by_groups"] is not None
+                and option not in self.output_options
+            ):
+                for required_group in self.options[option]["required_by_groups"]:
                     for operation in self.operations:
-                        if self.operations[operation]['group'] == required_group and \
-                                operation in self.output_operations:
-                            print(f'Error: operation "{operation}" requires the option "{option}"')
+                        if (
+                            self.operations[operation]["group"] == required_group
+                            and operation in self.output_operations
+                        ):
+                            print(
+                                f'Error: operation "{operation}" requires the option "{option}"'
+                            )
                             raise SystemExit(1)
 
         # Check if at least one operation is specified
         if self.output_operations == {} and self.one_operation_required:
-            print('Error: one operation is required')
+            print("Error: one operation is required")
             raise SystemExit(1)
 
         # Set all the unused arguments to False or None
         for operation in self.operations:
             if operation not in self.output_operations:
-                self.output_operations[operation] = self.operations[operation]['default_value']
+                self.output_operations[operation] = self.operations[operation][
+                    "default_value"
+                ]
 
         for option in self.options:
             if option not in self.output_options:
-                self.output_options[option] = self.options[option]['default_value']
+                self.output_options[option] = self.options[option]["default_value"]
 
         return self.output_operations, self.output_options
```

### Comparing `tblock-2.6.1/tblock/argumentor/exceptions.py` & `tblock-2.7.1/tblock/argumentor/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # argumentor - A simple, copylefted, lightweight library to work with command-line arguments in Python
 # Licensed under LGPLv3
 # Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
 
+
 class ExecNameError(IOError):
     def __init__(self, *args):
         super(ExecNameError, self).__init__(*args)
 
 
 class OperationExistsError(IOError):
     def __init__(self, *args):
```

### Comparing `tblock-2.6.1/tblock/cli.py` & `tblock-2.7.1/tblock/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -22,25 +22,23 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # Standard modules
 import sqlite3
 import sys
 
 # Local modules
-from .config import Var, log_message, create_dirs, VERSION, Path
+from .config import log_message, create_dirs, VERSION, Path
 from .filters import (
     subscribe,
     subscribe_custom,
     update_all,
-    change_permissions,
     unsubscribe,
     rename_custom,
     sync_filter_list_repo,
     show_info,
-    FilterPermissions,
     list_filter_lists,
     search_filter_lists,
     purge_cache,
     query_domain_to_filter_list,
     init_tblock,
 )
 from .hosts import update_hosts, restore_hosts, gen_hosts, enable_protection
@@ -92,54 +90,99 @@
 
     :param args: The command-line arguments
     """
     parser = Arguments(
         arguments=args,
         exec_name="tblock",
         copyright_header="TBlock - An anti-capitalist ad-blocker that uses the hosts file\n"
-        "Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>\n",
+        "Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>\n",
         more_info_footer="For more information, see tblock(1).",
     )
 
     # Add operation groups
     parser.add_operation_group("General", "General")
+    parser.add_operation_group("Hosts", "Hosts")
     parser.add_operation_group("Rules", "Rules")
     parser.add_operation_group("Filter lists", "Filter lists")
-    parser.add_operation_group("Hosts", "Hosts")
     parser.add_operation_group("Search", "Search")
 
     # Add option groups
     parser.add_option_group("General", "General")
     parser.add_option_group("Rules", "Rules")
     parser.add_option_group("Filter lists", "Filter lists")
     parser.add_option_group("Search", "Search")
 
     # Add "General" operations
     parser.add_operation(
+        operation="--init",
+        short_operation="-1",
+        value_type=bool,
+        description="Setup TBlock for the first time",
+        group="General",
+    )
+    parser.add_operation(
         operation="--help",
         short_operation="-h",
         value_type=bool,
         description="Show this help page",
         group="General",
     )
     parser.add_operation(
+        operation="--gen-hosts",
+        short_operation="-G",
+        value_type=bool,
+        description="Generate hosts file template",
+        group="General",
+    )
+    parser.add_operation(
         operation="--status",
         short_operation="-s",
         value_type=bool,
         description="Show status information",
         group="General",
     )
     parser.add_operation(
         operation="--version",
         short_operation="-v",
         value_type=bool,
         description="Show version and license information",
         group="General",
     )
 
+    # Add "Hosts" operations
+    parser.add_operation(
+        operation="--build",
+        short_operation="-B",
+        value_type=bool,
+        description="Rebuild hosts file",
+        group="Hosts",
+    )
+    parser.add_operation(
+        operation="--disable",
+        short_operation="-D",
+        value_type=bool,
+        description="Disable TBlock",
+        group="Hosts",
+    )
+    parser.add_operation(
+        operation="--enable",
+        short_operation="-E",
+        value_type=bool,
+        description="Enable TBlock",
+        group="Hosts",
+    )
+    parser.add_operation(
+        operation="--update-hosts",
+        short_operation="-H",
+        value_type=bool,
+        description="Rebuild hosts file (deprecated)",
+        group="Hosts",
+        hidden=True,
+    )
+
     # Add "Rules" operations
     parser.add_operation(
         operation="--allow",
         short_operation="-a",
         value_type=list,
         description="Allow specified domain(s)",
         group="Rules",
@@ -164,21 +207,14 @@
         value_type=list,
         description="Delete rule(s) for specified domain(s)",
         group="Rules",
     )
 
     # Add "Filter lists" operations
     parser.add_operation(
-        operation="--init",
-        short_operation="-1",
-        value_type=bool,
-        description="Setup TBlock for the first time",
-        group="Filter lists",
-    )
-    parser.add_operation(
         operation="--sync",
         short_operation="-Y",
         value_type=bool,
         description="Sync the filter list repository",
         group="Filter lists",
     )
     parser.add_operation(
@@ -213,63 +249,36 @@
         operation="--update",
         short_operation="-U",
         value_type=bool,
         description="Update all filter lists",
         group="Filter lists",
     )
     parser.add_operation(
-        operation="--mod",
-        short_operation="-M",
+        operation="--info",
+        short_operation="-I",
         value_type=list,
-        description="Change permissions of specified filter list(s)",
+        description="Get information about specified filter list(s)",
         group="Filter lists",
     )
+    # Only kept for compatibility purposes
     parser.add_operation(
-        operation="--info",
-        short_operation="-I",
+        operation="--mod",
+        short_operation="-M",
         value_type=list,
-        description="Get information about specified filter list(s)",
+        description="Change permissions of specified filter list(s) (deprecated)",
         group="Filter lists",
+        hidden=True,
     )
     parser.add_operation(
         operation="--purge-cache",
         short_operation="-P",
         value_type=bool,
-        description="Remove cached filter lists",
+        description="Remove cached filter lists (deprecated)",
         group="Filter lists",
-    )
-
-    # Add "Hosts" operations
-    parser.add_operation(
-        operation="--disable",
-        short_operation="-D",
-        value_type=bool,
-        description="Restore default hosts file",
-        group="Hosts",
-    )
-    parser.add_operation(
-        operation="--enable",
-        short_operation="-E",
-        value_type=bool,
-        description="Enable protection without rebuild hosts file",
-        group="Hosts",
-    )
-    parser.add_operation(
-        operation="--update-hosts",
-        short_operation="-H",
-        value_type=bool,
-        description="Rebuild hosts file",
-        group="Hosts",
-    )
-    parser.add_operation(
-        operation="--gen-hosts",
-        short_operation="-G",
-        value_type=bool,
-        description="Generate hosts file template",
-        group="Hosts",
+        hidden=True,
     )
 
     # Add "Search" operations
     parser.add_operation(
         operation="--list-rules",
         short_operation="-l",
         value_type=bool,
@@ -322,35 +331,17 @@
         short_option="-i",
         value_type=str,
         description="Specify the redirection IP address (with --redirect)",
         group="Rules",
         available_with_operations=["--redirect"],
         required_by_operations=["--redirect"],
     )
-    parser.add_option(
-        option="--rebuild-hosts",
-        short_option="-o",
-        value_type=bool,
-        description="Re-build the whole hosts file after saving rules",
-        group="Rules",
-        available_with_groups=["Rules"],
-    )
 
     # Add "Filter lists" options
     parser.add_option(
-        option="--permissions",
-        short_option="-p",
-        value_type=str,
-        description="Specify the permissions to give to filter lists",
-        group="Filter lists",
-        available_with_operations=["--subscribe", "--add-custom", "--mod"],
-        required_by_operations=["--mod"],
-        default_value=Var.DEFAULT_PERMISSIONS.compacted,
-    )
-    parser.add_option(
         option="--with-sync",
         short_option="-y",
         value_type=bool,
         description="Also sync filter list repository",
         group="Filter lists",
         available_with_operations=[
             "--subscribe",
@@ -394,14 +385,25 @@
             "--sync",
             "--subscribe",
             "--remove",
             "--update",
             "--update-all",
         ],
     )
+    # Only kept for compatibility purposes
+    parser.add_option(
+        option="--permissions",
+        short_option="-p",
+        value_type=str,
+        description="Specify the permissions to give to filter lists (deprecated)",
+        group="Filter lists",
+        available_with_operations=["--subscribe", "--add-custom", "--mod"],
+        hidden=True,
+    )
+
     # Add "Search" options
     parser.add_option(
         option="--user",
         short_option="-e",
         value_type=bool,
         description="List user rules only",
         group="Search",
@@ -465,15 +467,15 @@
 
     :param args: The command-line arguments
     """
     parser = Arguments(
         arguments=args,
         exec_name="tblockc",
         copyright_header="TBlockc - TBlock's built-in filter converter\n"
-        "Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>\n",
+        "Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>\n",
         more_info_footer="For more information, see tblockc(1).",
     )
 
     # Add operations
     parser.add_operation(
         operation="--help",
         short_operation="-h",
@@ -574,15 +576,15 @@
 
     :param args: The command-line arguments
     """
 
     parser = Arguments(
         arguments=args,
         exec_name="tblockd",
-        copyright_header="TBlockD - TBlock's built-in daemon\nCopyright (C) 2021-2022 Twann <tw4nn@disroot.org>\n",
+        copyright_header="TBlockD - TBlock's built-in daemon\nCopyright (C) 2021-2023 Twann <tw4nn@disroot.org>\n",
         more_info_footer="For more information, see tblockd(1).",
     )
 
     parser.add_operation(
         operation="--daemon",
         short_operation="-d",
         value_type=bool,
@@ -647,59 +649,69 @@
             f"TBlock v{VERSION} - An anti-capitalist ad-blocker that uses the hosts file\n\n{LICENSE_TEXT}"
         )
     elif operations["--allow"]:
         allow_domains(
             domains=operations["--allow"],
             force=options["--force"],
             quiet=options["--quiet"],
-            also_update_hosts=options["--rebuild-hosts"],
+            do_not_prompt=options["--no-prompt"],
         )
     elif operations["--block"]:
         block_domains(
             domains=operations["--block"],
             force=options["--force"],
             quiet=options["--quiet"],
-            also_update_hosts=options["--rebuild-hosts"],
+            do_not_prompt=options["--no-prompt"],
         )
     elif operations["--redirect"]:
         redirect_domains(
             domains=operations["--redirect"],
             ip=options["--ip"],
             force=options["--force"],
             quiet=options["--quiet"],
-            also_update_hosts=options["--rebuild-hosts"],
+            do_not_prompt=options["--no-prompt"],
         )
     elif operations["--delete-rule"]:
         delete_rules(
             domains=operations["--delete-rule"],
             quiet=options["--quiet"],
-            also_update_hosts=options["--rebuild-hosts"],
+            do_not_prompt=options["--no-prompt"],
         )
     elif operations["--init"]:
         init_tblock()
     elif operations["--sync"]:
         sync_filter_list_repo(force=options["--force"], quiet=options["--quiet"])
     elif operations["--subscribe"]:
+        if options["--permissions"]:
+            print(
+                Fore.YELLOW
+                + "Warning: option --permissions is deprecated and no longer does anything since permissions do not exist anymore."
+                + Style.RESET_ALL
+            )
         subscribe(
             filter_lists=operations["--subscribe"],
             do_not_prompt=options["--no-prompt"],
             quiet=options["--quiet"],
             sync_repo=options["--with-sync"],
             full_update=options["--with-update"],
-            permissions=FilterPermissions(options["--permissions"]),
             force=options["--force"],
         )
     elif operations["--add-custom"]:
+        if options["--permissions"]:
+            print(
+                Fore.YELLOW
+                + "Warning: option --permissions is deprecated and no longer does anything since permissions do not exist anymore."
+                + Style.RESET_ALL
+            )
         subscribe_custom(
             filter_lists=operations["--add-custom"],
             do_not_prompt=options["--no-prompt"],
             quiet=options["--quiet"],
             sync_repo=options["--with-sync"],
             full_update=options["--with-update"],
-            permissions=FilterPermissions(options["--permissions"]),
             force=options["--force"],
             custom_syntax=options["--custom-syntax"],
         )
     elif operations["--rename"]:
         rename_custom(
             filter_lists=operations["--rename"],
             do_not_prompt=options["--no-prompt"],
@@ -721,41 +733,51 @@
         update_all(
             do_not_prompt=options["--no-prompt"],
             quiet=options["--quiet"],
             sync_repo=options["--with-sync"],
             force=options["--force"],
         )
     elif operations["--mod"]:
-        change_permissions(
-            filter_lists=operations["--mod"],
-            permissions=FilterPermissions(options["--permissions"]),
-            do_not_prompt=options["--no-prompt"],
-            quiet=options["--quiet"],
-            sync_repo=options["--with-sync"],
-            force=options["--force"],
+        print(
+            Fore.YELLOW
+            + "Warning: operation --mod is deprecated and no longer does anything since permissions do not exist anymore."
+            + Style.RESET_ALL
         )
     elif operations["--info"]:
         show_info(filter_lists=operations["--info"], quiet=options["--quiet"])
     elif operations["--purge-cache"]:
+        print(
+            Fore.YELLOW
+            + "Warning: operation --purge-cache is deprecated. Please use your shell instead."
+            + Style.RESET_ALL
+        )
         purge_cache(do_not_prompt=options["--no-prompt"], quiet=options["--quiet"])
     elif operations["--disable"]:
         restore_hosts(quiet=options["--quiet"], do_not_prompt=options["--no-prompt"])
     elif operations["--enable"]:
         enable_protection(
             quiet=options["--quiet"], do_not_prompt=options["--no-prompt"]
         )
+    elif operations["--build"]:
+        update_hosts(quiet=options["--quiet"], do_not_prompt=options["--no-prompt"])
     elif operations["--update-hosts"]:
+        print(
+            Fore.YELLOW
+            + "Warning: operation --update-hosts is deprecated. Please use --build instead."
+            + Style.RESET_ALL
+        )
         update_hosts(quiet=options["--quiet"], do_not_prompt=options["--no-prompt"])
     elif operations["--gen-hosts"]:
         gen_hosts()
     elif operations["--list-rules"]:
         list_rules(
             from_filter_lists=options["--from-filters"],
             user_only=options["--user"],
             standard_only=options["--standard"],
+            quiet=options["--quiet"],
         )
     elif operations["--list"]:
         list_filter_lists(
             custom_only=options["--custom"],
             on_repo_only=options["--on-repo"],
             subscribing_only=options["--subscribing"],
             not_subscribing_only=options["--not-subscribing"],
```

### Comparing `tblock-2.6.1/tblock/compat.py` & `tblock-2.7.1/tblock/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -120,14 +120,22 @@
                     (x[0], x[1], x[2]),
                 )
         conn.cursor().execute(
             "DELETE FROM rules WHERE filter_id=?", (USER_RULE_PRIORITY,)
         )
 
 
+def update_database_from_2_6_1(quiet: bool = False) -> None:
+    """
+    :param quiet: Optional. Do not display an output (false by default)
+    """
+    with sqlite3.connect(Path.DATABASE) as conn:
+        conn.cursor().execute("ALTER TABLE filters DROP COLUMN permissions;")
+
+
 def update_database_from_2_3_0(quiet: bool = False) -> None:
     """
     :param quiet: Optional. Do not display an output (false by default)
     """
     with sqlite3.connect(Path.DATABASE) as conn:
         conn.cursor().execute(
             "UPDATE filters SET syntax=? WHERE syntax=?", ("tblock_legacy", "tblock")
@@ -280,9 +288,11 @@
                         )
                         conn.commit()
                         conn.close()
                         if db_version < "2.4.0":
                             update_database_from_2_3_0(quiet=quiet)
                         if db_version < "2.5.0":
                             update_database_from_2_4_1(quiet=quiet)
+                        if db_version < "2.7.0":
+                            update_database_from_2_6_1(quiet=quiet)
             else:
                 update_database_from_1_3_2(quiet=quiet)
```

### Comparing `tblock-2.6.1/tblock/config.py` & `tblock-2.7.1/tblock/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -28,19 +28,19 @@
 import configparser
 import sqlite3
 
 # Local modules
 from .const import FilterPermissions
 
 
-VERSION = "2.6.1"
+VERSION = "2.7.1"
+REPO_COMPATIBLE_VERSION = "2.4.0"
 
 
 class Path:
-
     TERMUX_ROOT = "/data/data/com.termux/files/usr/"
 
     # The script is running on Termux
     if os.path.isdir(TERMUX_ROOT):
         PREFIX = os.path.join(TERMUX_ROOT, "lib", "tblock")
         HOSTS = os.path.join("/", "system", "etc", "hosts")
         TMP_DIR = os.path.join(TERMUX_ROOT, "tmp", "tblock")
@@ -86,42 +86,38 @@
 def load_config(config_file: str) -> configparser.ConfigParser:
     config = configparser.ConfigParser()
     config.read(config_file)
     return config
 
 
 class Var:
-
     __config = load_config(Path.CONFIG)
 
     try:
-        DEFAULT_PERMISSIONS = FilterPermissions(__config.get("policy", "regular"))
-    except (configparser.NoSectionError, configparser.NoOptionError, ValueError):
-        DEFAULT_PERMISSIONS = FilterPermissions("AB")
-    try:
-        DEFAULT_PERMISSIONS_CUSTOM = FilterPermissions(__config.get("policy", "custom"))
-    except (configparser.NoSectionError, configparser.NoOptionError, ValueError):
-        DEFAULT_PERMISSIONS_CUSTOM = FilterPermissions("AB")
-    try:
         DEFAULT_IP = __config.get("hosts", "default_ip")
     except (configparser.NoSectionError, configparser.NoOptionError, ValueError):
         DEFAULT_IP = "0.0.0.0"
     try:
         DEFAULT_IPV6 = __config.get("hosts", "default_ipv6")
     except (configparser.NoSectionError, configparser.NoOptionError, ValueError):
         DEFAULT_IPV6 = "::1"
     try:
         ALLOW_IPV6 = __config.getboolean("hosts", "allow_ipv6")
     except (configparser.NoSectionError, configparser.NoOptionError, ValueError):
         ALLOW_IPV6 = False
+
     REPO_MIRRORS = [
+        "https://update.tblock.me/2.4.0/index.json",
         "https://tblock.codeberg.page/repo/2.4.0/index.json",
         "https://codeberg.org/tblock/repo/raw/branch/pages/2.4.0/index.json",
-        "https://framagit.org/twann/repo/-/raw/pages/2.4.0/index.json",
         "https://git.disroot.org/tblock/repo/raw/branch/pages/2.4.0/index.json",
+        "https://mirror.tblock.me/index/2.4.0/index.json",
+        "https://download.tblock.me/index/2.4.0/index.json",
+        "https://tblock.b-cdn.net/index/2.4.0/index.json",
+        "https://framagit.org/twann/repo/-/raw/pages/2.4.0/index.json",
     ]
 
 
 def hosts_are_safe() -> bool:
     """
     Check if the hosts file's saved sha512sum is the same as the active hosts file's sha512sum.
     This can be useful to prevent hosts hijack
```

### Comparing `tblock-2.6.1/tblock/const.py` & `tblock-2.7.1/tblock/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -97,40 +97,52 @@
     )
     TBLOCK = re.compile(
         r'^([a-z\d\-.]*\.[a-z]*|(\[allow]|\[block]|\[redirect "[\d.:a-f]*"])|#.*)$'
     )
 
 
 class Profile:
+    """
+    This contains the different profiles that are available during the setup wizard
+    """
 
-    NONE = ()
-    LIGHT = ("peter-lowe", "stevenblack-hosts", "tblock-base")
-    BALANCED = (
-        "adguard-cname",
-        "adguard-dns",
-        "adguard-tracking-servers",
-        "cpbl-filters",
-        "peter-lowe",
-        "stevenblack-hosts",
-        "tblock-base",
-        "tblock-security",
-    )
-    AGGRESSIVE = (
-        "adguard-cname",
-        "adguard-dns",
-        "adguard-tracking-servers",
-        "cpbl-filters",
-        "ddgtrackerradar",
-        "divested",
-        "mpvs-hosts",
-        "peter-lowe",
-        "stevenblack-hosts",
-        "tblock-base",
+    # pylint: disable=too-few-public-methods
+
+    NONE = []
+    LIGHT = NONE + ["peter-lowe", "stevenblack-hosts", "tblock-allow", "tblock-base"]
+    BALANCED = LIGHT + ["adguard-cname", "adguard-dns", "cpbl-filters"]
+    AGGRESSIVE = BALANCED + ["ddgtrackerradar", "divested", "mpvs-hosts"]
+
+
+class Components:
+    """
+    This contains the different additional components that one can choose to block during the setup wizard
+    """
+
+    # pylint: disable=too-few-public-methods
+
+    SECURITY = [
+        "blocklistproject-phishing",
+        "blocklistproject-ramsomware",
+        "blocklistproject-malware",
+        "spam404",
         "tblock-security",
-    )
+        "urlhaus",
+    ]
+    PORNOGRAPHY = ["blocklistproject-porn"]
+    FAKE_NEWS = ["fakenews"]
+    DRUGS = ["blocklistproject-drugs"]
+    GAMBLING = ["blocklistproject-gambling"]
+    PIRACY = ["blocklistproject-piracy"]
+    HATE = [
+        "antifa-blocklist",
+        "antifa-blocklist-alttech",
+        "antifa-blocklist-populistic",
+    ]
+    CRYPTO = ["blocklistproject-crypto"]
 
 
 # Code name to use to tell TBlock that a rule is a user-defined rule
 USER_RULE_PRIORITY = "!user"
 
 RULE_COMMENTS = "C"
```

### Comparing `tblock-2.6.1/tblock/converter/__init__.py` & `tblock-2.7.1/tblock/converter/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -25,19 +25,17 @@
 import io
 import sqlite3
 
 # Local modules
 from .syntaxtools import detect_syntax, is_valid_rule, get_rule
 from ..style import loading_icon, Icon, Font
 from ..const import (
-    USER_RULE_PRIORITY,
     RulePolicy,
     TBlockSyntaxStatus,
     FilterSyntax,
-    FilterPermissions,
     RULE_COMMENTS,
 )
 from ..utils import contains_wildcards
 from ..exceptions import FilterSyntaxError
 from ..config import Path
 
 
@@ -79,158 +77,162 @@
                 raise FilterSyntaxError("is a directory: {0}".format(self.file))
         else:
             if syntax not in ALL_SYNTAX:
                 raise FilterSyntaxError("invalid input syntax: {0}".format(syntax))
             else:
                 self.syntax = syntax
 
-    def insert_rules_to_database(
-        self, filter_id: str, permissions: FilterPermissions
-    ) -> None:
+    def insert_rules_to_database(self, filter_id: str, permissions=None) -> None:
+        # This function is WAY too long
+        # TODO: make a cleaner and shorter function
         try:
             with io.open(self.file, "rt") as f:
-                data = f.readlines()
+                all_rules_count = sum(1 for _ in f)
         except UnicodeDecodeError:
             raise FilterSyntaxError("unable to decode file: {0}".format(self.file))
         except PermissionError:
             raise FilterSyntaxError("unable to access file: {0}".format(self.file))
         except FileNotFoundError:
             raise FilterSyntaxError("file not found: {0}".format(self.file))
 
         if not self.quiet and self.syntax == FilterSyntax.TBLOCK_LEGACY:
             print(
                 f" {Icon.WARNING} TBlock filter format v1 is deprecated. In future versions, only v2 will be supported."
             )
 
         count = 0
         percent = 0
-        all_rules_count = len(data)
 
         connection = sqlite3.connect(Path.DATABASE)
         cursor = connection.cursor()
 
         # TBlock syntax support
         tblock_begin = False
         tblock_policy = None
         tblock_ip = None
+        invalid_rules = 0
 
         user_rules = []
         rules_connection = sqlite3.connect(Path.RULES_DATABASE)
         rules_cursor = rules_connection.cursor()
         u = rules_cursor.execute("SELECT domain FROM r ORDER BY domain ASC;").fetchall()
         for x in u:
             user_rules.append(x[0])
         rules_connection.close()
 
-        for line in data:
+        if not self.quiet:
+            print(
+                " {0} Adding rules ({1}): 0%".format(
+                    loading_icon(count), all_rules_count
+                ),
+                end="\r",
+            )
 
-            count += 1
-            percent = int(count * 100 / len(data))
-            if not self.quiet:
-                print(
-                    " {0} Inserting rules into database ({1}): {2}%".format(
-                        loading_icon(count), all_rules_count, percent
-                    ),
-                    end="\r",
-                )
+        with io.open(self.file, "rt", encoding="utf-8") as f:
+            while True:
+                line = f.readline()
+                if not line:
+                    break
+                count += 1
+
+                if count % 25000 == 0:
+                    percent = int(count * 100 / all_rules_count)
+                    if not self.quiet:
+                        print(
+                            " {0} Adding rules ({1}): {2}%".format(
+                                loading_icon(count / 25000), all_rules_count, percent
+                            ),
+                            end="\r",
+                        )
 
-            if is_valid_rule(line.split("\n")[0], self.syntax):
-                if self.syntax == FilterSyntax.TBLOCK_LEGACY:
-                    rule = get_rule(
-                        line.split("\n")[0],
-                        self.syntax,
-                        allow_comments=False,
-                        tblock_begin=tblock_begin,
-                        tblock_policy=tblock_policy,
-                        tblock_ip=tblock_ip,
-                        allow_allow=permissions.ALLOW,
-                        allow_block=permissions.BLOCK,
-                        allow_redirect=permissions.REDIRECT,
-                    )
-                elif self.syntax == FilterSyntax.TBLOCK:
-                    rule = get_rule(
-                        line.split("\n")[0],
-                        self.syntax,
-                        allow_comments=False,
-                        tblock_policy=tblock_policy,
-                        tblock_ip=tblock_ip,
-                        allow_allow=permissions.ALLOW,
-                        allow_block=permissions.BLOCK,
-                        allow_redirect=permissions.REDIRECT,
-                    )
-                else:
-                    rule = get_rule(
-                        line.split("\n")[0],
-                        self.syntax,
-                        allow_comments=False,
-                        allow_allow=permissions.ALLOW,
-                        allow_block=permissions.BLOCK,
-                        allow_redirect=permissions.REDIRECT,
-                    )
-
-                if rule:
-                    # Change the IP address if rule is a redirecting rule
-                    if rule[1] == RulePolicy.REDIRECT:
-                        ip = rule[2].compressed
+                if is_valid_rule(line.split("\n")[0], self.syntax):
+                    if self.syntax == FilterSyntax.TBLOCK_LEGACY:
+                        rule = get_rule(
+                            line.split("\n")[0],
+                            self.syntax,
+                            allow_comments=False,
+                            tblock_begin=tblock_begin,
+                            tblock_policy=tblock_policy,
+                            tblock_ip=tblock_ip,
+                            allow_allow=True,
+                            allow_block=True,
+                            allow_redirect=False,
+                        )
+                    elif self.syntax == FilterSyntax.TBLOCK:
+                        rule = get_rule(
+                            line.split("\n")[0],
+                            self.syntax,
+                            allow_comments=False,
+                            tblock_policy=tblock_policy,
+                            tblock_ip=tblock_ip,
+                            allow_allow=True,
+                            allow_block=True,
+                            allow_redirect=False,
+                        )
                     else:
-                        ip = None
+                        rule = get_rule(
+                            line.split("\n")[0],
+                            self.syntax,
+                            allow_comments=False,
+                            allow_allow=True,
+                            allow_block=True,
+                            allow_redirect=False,
+                        )
 
-                    # TBlock syntax support
-                    if self.syntax in (FilterSyntax.TBLOCK_LEGACY, FilterSyntax.TBLOCK):
-                        if rule[0] == TBlockSyntaxStatus.CURRENT_STATUS:
-                            tblock_begin = rule[1]
-                            continue
-                        elif rule[0] == TBlockSyntaxStatus.CURRENT_POLICY:
-                            tblock_policy = rule[1]
-                            if tblock_policy == RulePolicy.REDIRECT:
-                                tblock_ip = rule[2]
-                            continue
-
-                    domain = rule[0]
-                    policy = rule[1]
-
-                    query = cursor.execute(
-                        "SELECT domain, policy FROM rules WHERE domain=?", (domain,)
-                    ).fetchone()
-                    # Check whether the rule already exists in the database
-                    if domain not in user_rules:
-                        # Check if the rule exists and if the rule is not a user rule
-                        if query:
-                            # Check if the local rule has a higher priority (block < redirect < allow)
-                            if (
-                                query[1] == policy == RulePolicy.BLOCK
-                                or policy == RulePolicy.REDIRECT
-                                and policy != RulePolicy.ALLOW
-                                or policy == RulePolicy.ALLOW
-                            ):
-                                cursor.execute(
-                                    "UPDATE rules SET policy=?, filter_id=?, ip=? WHERE domain=?;",
-                                    (policy, filter_id, ip, domain),
-                                )
-                        else:
+                    if rule:
+                        # TBlock syntax support
+                        if self.syntax in (
+                            FilterSyntax.TBLOCK_LEGACY,
+                            FilterSyntax.TBLOCK,
+                        ):
+                            if rule[0] == TBlockSyntaxStatus.CURRENT_STATUS:
+                                tblock_begin = rule[1]
+                                continue
+                            elif rule[0] == TBlockSyntaxStatus.CURRENT_POLICY:
+                                tblock_policy = rule[1]
+                                continue
+
+                        domain = rule[0]
+                        policy = rule[1]
+
+                        # Check whether the rule already exists in the database
+                        if domain not in user_rules:
+                            # Check if the rule exists and if the rule is not a user rule
                             cursor.execute(
-                                "INSERT INTO rules (domain, policy, filter_id, ip) VALUES (?, ?, ?, ?);",
-                                (domain, policy, filter_id, ip),
+                                "INSERT INTO rules (domain, policy, filter_id) VALUES (?, ?, ?) "
+                                "ON CONFLICT(domain) "
+                                "DO UPDATE SET policy=?, filter_id=? WHERE policy NOT IN (?, ?);",
+                                (
+                                    domain,
+                                    policy,
+                                    filter_id,
+                                    policy,
+                                    filter_id,
+                                    "A",
+                                    policy,
+                                ),
                             )
-                    # This will remove rules that are duplicate of user rules
-                    elif query:
-                        cursor.execute("DELETE FROM rules WHERE domain=?;", (domain,))
+                    else:
+                        invalid_rules += 1
+                else:
+                    invalid_rules += 1
         if not self.quiet:
+            percent = int(count * 100 / all_rules_count)
             print(
-                " {0} Inserting rules into database ({1}): {2}%".format(
+                " {0} Adding rules ({1}): {2}%".format(
                     Icon.SUCCESS, all_rules_count, percent
                 )
             )
             print(
                 " {0} Skipped {1} invalid rules or lines ({2}%)".format(
                     Icon.INFORMATION,
-                    str(len(data) - connection.total_changes),
+                    str(invalid_rules),
                     str(
                         round(
-                            ((len(data) - connection.total_changes) * 100 / len(data)),
+                            (invalid_rules * 100 / all_rules_count),
                             1,
                         )
                     ),
                 )
             )
 
         connection.commit()
@@ -241,17 +243,19 @@
         output_file: str,
         output_syntax: str,
         allow_comments: bool = False,
         redirect_to_zero: bool = False,
         dnsmasq_server: bool = False,
         optimize: bool = False,
     ) -> None:
+        # This function is also WAY too long
+        # TODO: make a cleaner and shorter function
         try:
             with io.open(self.file, "rt") as f:
-                data = f.readlines()
+                all_rules_count = sum(1 for _ in f)
         except UnicodeDecodeError:
             raise FilterSyntaxError("unable to decode file: {0}".format(self.file))
         except PermissionError:
             raise FilterSyntaxError("unable to access file: {0}".format(self.file))
         except FileNotFoundError:
             raise FilterSyntaxError("file not found: {0}".format(self.file))
 
@@ -270,207 +274,226 @@
         tblock_begin = False
         tblock_policy = None
         tblock_ip = None
 
         output_tblock_policy = None
         output_tblock_ip = None
         count = 0
-        rules_count = len(data)
 
         with open(output_file, "wt") as w:
             if output_syntax == FilterSyntax.ADBLOCKPLUS:
                 w.write("[Adblock Plus 2.0]\n\n")
             elif output_syntax == FilterSyntax.TBLOCK_LEGACY:
                 w.write("@BEGIN_RULES\n\n")
 
-            for line in data:
-
-                if is_valid_rule(line.split("\n")[0], self.syntax):
-                    if self.syntax == FilterSyntax.TBLOCK_LEGACY:
-                        rule = get_rule(
-                            line.split("\n")[0],
-                            self.syntax,
-                            allow_comments=allow_comments,
-                            tblock_begin=tblock_begin,
-                            tblock_policy=tblock_policy,
-                            tblock_ip=tblock_ip,
-                        )
-                    elif self.syntax == FilterSyntax.TBLOCK:
-                        rule = get_rule(
-                            line.split("\n")[0],
-                            self.syntax,
-                            allow_comments=allow_comments,
-                            tblock_policy=tblock_policy,
-                            tblock_ip=tblock_ip,
-                        )
-                    else:
-                        rule = get_rule(
-                            line.split("\n")[0],
-                            self.syntax,
-                            allow_comments=allow_comments,
-                        )
+            print(
+                " {0} Converting filter list ({1}): 0%".format(
+                    loading_icon(count), all_rules_count
+                ),
+                end="\r",
+            )
 
-                    if rule:
-                        # Change the IP address if rule is a redirecting rule
-                        if rule[1] == RulePolicy.REDIRECT:
-                            ip = rule[2].compressed
+            with io.open(self.file, "rt", encoding="utf-8") as f:
+                while True:
+                    line = f.readline()
+                    if not line:
+                        break
+                    if is_valid_rule(line.split("\n")[0], self.syntax):
+                        if self.syntax == FilterSyntax.TBLOCK_LEGACY:
+                            rule = get_rule(
+                                line.split("\n")[0],
+                                self.syntax,
+                                allow_comments=allow_comments,
+                                tblock_begin=tblock_begin,
+                                tblock_policy=tblock_policy,
+                                tblock_ip=tblock_ip,
+                            )
+                        elif self.syntax == FilterSyntax.TBLOCK:
+                            rule = get_rule(
+                                line.split("\n")[0],
+                                self.syntax,
+                                allow_comments=allow_comments,
+                                tblock_policy=tblock_policy,
+                                tblock_ip=tblock_ip,
+                            )
                         else:
-                            ip = None
-
-                        # TBlock syntax support
-                        if self.syntax in (
-                            FilterSyntax.TBLOCK_LEGACY,
-                            FilterSyntax.TBLOCK,
-                        ):
-                            if rule[0] == TBlockSyntaxStatus.CURRENT_STATUS:
-                                tblock_begin = rule[1]
-                                continue
-                            elif rule[0] == TBlockSyntaxStatus.CURRENT_POLICY:
-                                tblock_policy = rule[1]
-                                if tblock_policy == RulePolicy.REDIRECT:
-                                    tblock_ip = rule[2]
-                                continue
-
-                        count += 1
-                        percent = int(count * 100 / rules_count)
-                        if not self.quiet:
-                            print(
-                                " {0} Converting filter list ({1}): {2}%".format(
-                                    loading_icon(count), rules_count, percent
-                                ),
-                                end="\r",
+                            rule = get_rule(
+                                line.split("\n")[0],
+                                self.syntax,
+                                allow_comments=allow_comments,
                             )
 
-                        if output_syntax == FilterSyntax.ADBLOCKPLUS:
-                            if rule[1] == RulePolicy.ALLOW:
-                                w.write(f"@@||{rule[0]}^\n")
-                            elif rule[1] == RulePolicy.BLOCK:
-                                w.write(f"||{rule[0]}^\n")
-                            elif rule[1] == RULE_COMMENTS and allow_comments:
-                                w.write(f"!{rule[0]}\n")
-
-                        elif output_syntax == FilterSyntax.HOSTS:
-                            if rule[1] == RulePolicy.BLOCK and not contains_wildcards(
-                                rule[0]
-                            ):
-                                if redirect_to_zero:
-                                    w.write(f"0.0.0.0\t\t{rule[0]}\n")
-                                else:
-                                    w.write(f"127.0.0.1\t\t{rule[0]}\n")
-                            elif rule[
-                                1
-                            ] == RulePolicy.REDIRECT and not contains_wildcards(
-                                rule[0]
-                            ):
-                                w.write(f"{ip}\t{rule[0]}\n")
-                            elif rule[1] == RULE_COMMENTS and allow_comments:
-                                w.write(f"#{rule[0]}\n")
-
-                        elif output_syntax == FilterSyntax.LIST:
-                            if rule[1] == RulePolicy.BLOCK and not contains_wildcards(
-                                rule[0]
-                            ):
-                                w.write(f"{rule[0]}\n")
-                            elif rule[1] == RULE_COMMENTS and allow_comments:
-                                w.write(f"#{rule[0]}\n")
-
-                        elif output_syntax == FilterSyntax.DNSMASQ:
-                            if rule[1] == RulePolicy.BLOCK and not contains_wildcards(
-                                rule[0]
-                            ):
-                                if dnsmasq_server:
-                                    w.write(f"server=/{rule[0]}/\n")
-                                elif redirect_to_zero:
-                                    w.write(f"address=/{rule[0]}/0.0.0.0/\n")
-                                else:
-                                    w.write(f"address=/{rule[0]}/127.0.0.1/\n")
-                            elif rule[
-                                1
-                            ] == RulePolicy.REDIRECT and not contains_wildcards(
-                                rule[0]
-                            ):
-                                w.write(f"address=/{rule[0]}/{ip}/\n")
-                            elif rule[1] == RULE_COMMENTS and allow_comments:
-                                w.write(f"#{rule[0]}\n")
-
-                        elif output_syntax == FilterSyntax.TBLOCK:
-                            if (
-                                not rule[1] == output_tblock_policy
-                                or not ip == output_tblock_ip
+                        if rule:
+                            # Change the IP address if rule is a redirecting rule
+                            if rule[1] == RulePolicy.REDIRECT:
+                                ip = rule[2].compressed
+                            else:
+                                ip = None
+
+                            # TBlock syntax support
+                            if self.syntax in (
+                                FilterSyntax.TBLOCK_LEGACY,
+                                FilterSyntax.TBLOCK,
                             ):
+                                if rule[0] == TBlockSyntaxStatus.CURRENT_STATUS:
+                                    tblock_begin = rule[1]
+                                    continue
+                                elif rule[0] == TBlockSyntaxStatus.CURRENT_POLICY:
+                                    tblock_policy = rule[1]
+                                    if tblock_policy == RulePolicy.REDIRECT:
+                                        tblock_ip = rule[2]
+                                    continue
+
+                            count += 1
+
+                            if count % 25000 == 0:
+                                percent = int(count * 100 / all_rules_count)
+                                if not self.quiet:
+                                    print(
+                                        " {0} Converting filter list ({1}): {2}%".format(
+                                            loading_icon(count / 25000),
+                                            all_rules_count,
+                                            percent,
+                                        ),
+                                        end="\r",
+                                    )
+
+                            if output_syntax == FilterSyntax.ADBLOCKPLUS:
                                 if rule[1] == RulePolicy.ALLOW:
-                                    w.write("\n[allow]\n")
-                                elif rule[
+                                    w.write(f"@@||{rule[0]}^\n")
+                                elif rule[1] == RulePolicy.BLOCK:
+                                    w.write(f"||{rule[0]}^\n")
+                                elif rule[1] == RULE_COMMENTS and allow_comments:
+                                    w.write(f"!{rule[0]}\n")
+
+                            elif output_syntax == FilterSyntax.HOSTS:
+                                if rule[
                                     1
                                 ] == RulePolicy.BLOCK and not contains_wildcards(
                                     rule[0]
                                 ):
-                                    w.write("\n[block]\n")
+                                    if redirect_to_zero:
+                                        w.write(f"0.0.0.0\t\t{rule[0]}\n")
+                                    else:
+                                        w.write(f"127.0.0.1\t\t{rule[0]}\n")
                                 elif rule[
                                     1
                                 ] == RulePolicy.REDIRECT and not contains_wildcards(
                                     rule[0]
                                 ):
-                                    w.write(f'\n[redirect "{ip}"]\n')
-                                if rule[1] != RULE_COMMENTS:
-                                    output_tblock_policy = rule[1]
-                                    output_tblock_ip = ip
-                            if not rule[1] == RULE_COMMENTS:
-                                w.write(f"{rule[0]}\n")
-                            elif allow_comments:
-                                w.write(f"#{rule[0]}\n")
-
-                        elif output_syntax == FilterSyntax.TBLOCK_LEGACY:
-                            if (
-                                not rule[1] == output_tblock_policy
-                                or not ip == output_tblock_ip
-                            ):
-                                if rule[1] == RulePolicy.ALLOW:
-                                    w.write("\n!allow\n")
-                                elif rule[
+                                    w.write(f"{ip}\t{rule[0]}\n")
+                                elif rule[1] == RULE_COMMENTS and allow_comments:
+                                    w.write(f"#{rule[0]}\n")
+
+                            elif output_syntax == FilterSyntax.LIST:
+                                if rule[
+                                    1
+                                ] == RulePolicy.BLOCK and not contains_wildcards(
+                                    rule[0]
+                                ):
+                                    w.write(f"{rule[0]}\n")
+                                elif rule[1] == RULE_COMMENTS and allow_comments:
+                                    w.write(f"#{rule[0]}\n")
+
+                            elif output_syntax == FilterSyntax.DNSMASQ:
+                                if rule[
                                     1
                                 ] == RulePolicy.BLOCK and not contains_wildcards(
                                     rule[0]
                                 ):
-                                    w.write("\n!block\n")
+                                    if dnsmasq_server:
+                                        w.write(f"server=/{rule[0]}/\n")
+                                    elif redirect_to_zero:
+                                        w.write(f"address=/{rule[0]}/0.0.0.0/\n")
+                                    else:
+                                        w.write(f"address=/{rule[0]}/127.0.0.1/\n")
                                 elif rule[
                                     1
                                 ] == RulePolicy.REDIRECT and not contains_wildcards(
                                     rule[0]
                                 ):
-                                    w.write(f"\n!redirect {ip}\n")
-                                if rule[1] != RULE_COMMENTS:
-                                    output_tblock_policy = rule[1]
-                                    output_tblock_ip = ip
-                            if not rule[1] == RULE_COMMENTS:
-                                w.write(f"{rule[0]}\n")
-                            elif allow_comments:
-                                w.write(f"#{rule[0]}\n")
-
-                        else:
-                            raise FilterSyntaxError(
-                                "invalid output syntax: {0}".format(output_syntax)
-                            )
-                elif line == "\n" and not optimize:
-                    w.write("\n")
+                                    w.write(f"address=/{rule[0]}/{ip}/\n")
+                                elif rule[1] == RULE_COMMENTS and allow_comments:
+                                    w.write(f"#{rule[0]}\n")
+
+                            elif output_syntax == FilterSyntax.TBLOCK:
+                                if (
+                                    not rule[1] == output_tblock_policy
+                                    or not ip == output_tblock_ip
+                                ):
+                                    if rule[1] == RulePolicy.ALLOW:
+                                        w.write("\n[allow]\n")
+                                    elif rule[
+                                        1
+                                    ] == RulePolicy.BLOCK and not contains_wildcards(
+                                        rule[0]
+                                    ):
+                                        w.write("\n[block]\n")
+                                    elif rule[
+                                        1
+                                    ] == RulePolicy.REDIRECT and not contains_wildcards(
+                                        rule[0]
+                                    ):
+                                        w.write(f'\n[redirect "{ip}"]\n')
+                                    if rule[1] != RULE_COMMENTS:
+                                        output_tblock_policy = rule[1]
+                                        output_tblock_ip = ip
+                                if not rule[1] == RULE_COMMENTS:
+                                    w.write(f"{rule[0]}\n")
+                                elif allow_comments:
+                                    w.write(f"#{rule[0]}\n")
+
+                            elif output_syntax == FilterSyntax.TBLOCK_LEGACY:
+                                if (
+                                    not rule[1] == output_tblock_policy
+                                    or not ip == output_tblock_ip
+                                ):
+                                    if rule[1] == RulePolicy.ALLOW:
+                                        w.write("\n!allow\n")
+                                    elif rule[
+                                        1
+                                    ] == RulePolicy.BLOCK and not contains_wildcards(
+                                        rule[0]
+                                    ):
+                                        w.write("\n!block\n")
+                                    elif rule[
+                                        1
+                                    ] == RulePolicy.REDIRECT and not contains_wildcards(
+                                        rule[0]
+                                    ):
+                                        w.write(f"\n!redirect {ip}\n")
+                                    if rule[1] != RULE_COMMENTS:
+                                        output_tblock_policy = rule[1]
+                                        output_tblock_ip = ip
+                                if not rule[1] == RULE_COMMENTS:
+                                    w.write(f"{rule[0]}\n")
+                                elif allow_comments:
+                                    w.write(f"#{rule[0]}\n")
+
+                            else:
+                                raise FilterSyntaxError(
+                                    "invalid output syntax: {0}".format(output_syntax)
+                                )
+                    elif line == "\n" and not optimize:
+                        w.write("\n")
 
             if output_syntax == FilterSyntax.TBLOCK_LEGACY:
                 w.write("\n\n@END_RULES")
 
         if not self.quiet:
             print(
                 " {0} Converting filter list ({1}): 100%".format(
-                    Icon.SUCCESS, rules_count
+                    Icon.SUCCESS, all_rules_count
                 )
             )
             print(
                 " {0} Skipped {1} rules ({2}%)".format(
                     Icon.INFORMATION,
-                    rules_count - count,
-                    round((rules_count - count) * 100 / rules_count, 1),
+                    all_rules_count - count,
+                    round((all_rules_count - count) * 100 / all_rules_count, 1),
                 )
             )
 
 
 def convert(
     input_file: str,
     output_file: str,
```

### Comparing `tblock-2.6.1/tblock/converter/__main__.py` & `tblock-2.7.1/tblock/converter/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
```

### Comparing `tblock-2.6.1/tblock/converter/syntaxtools.py` & `tblock-2.7.1/tblock/converter/syntaxtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
```

### Comparing `tblock-2.6.1/tblock/daemon/__init__.py` & `tblock-2.7.1/tblock/daemon/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -93,28 +93,24 @@
                 )
     else:
         if not no_pid:
             with open(Path.DAEMON_PID, "wt") as w:
                 w.write(str(os.getpid()))
         try:
             frequency = daemon_config.getint("daemon", "frequency")
-            # Prevent the frequency from being set to a value lower than one hour
-            if frequency < 3:
+            # Prevent the frequency from being set to a value lower than 12 hour
+            if frequency < 12:
                 frequency = 12
         except (configparser.NoSectionError, configparser.NoOptionError, ValueError):
-            frequency = 12
+            frequency = 48
         try:
             sync_repo = daemon_config.getboolean("daemon", "sync_repo")
         except (configparser.NoSectionError, configparser.NoOptionError, ValueError):
             sync_repo = True
         try:
-            anti_hijack = daemon_config.getboolean("daemon", "anti_hijack")
-        except (configparser.NoSectionError, configparser.NoOptionError, ValueError):
-            anti_hijack = True
-        try:
             force = daemon_config.getboolean("daemon", "force")
         except (configparser.NoSectionError, configparser.NoOptionError, ValueError):
             force = False
 
         with sqlite3.connect(Path.DATABASE) as conn:
             cur = conn.cursor()
             last_update = cur.execute(
@@ -130,31 +126,24 @@
                 os.getpid()
             )
         )
         updater(
             sync_repo=sync_repo,
             frequency=frequency,
             do_not_remove_pid=no_pid,
-            anti_hijack=anti_hijack,
             force=force,
             quiet=quiet,
             last_update=last_update,
         )
 
 
-def launch_anti_hijack(quiet: bool = False):
-    if not hosts_are_safe() and not hosts_are_default():
-        print(f"{Font.BOLD}==> Hosts file hijack detected{Font.DEFAULT}")
-        update_hosts(do_not_prompt=True)
-        log_message(
-            "[tblockd] WARN:  hosts hijack was detected; hosts file was updated"
-        )
-
-
 def time_left(last_update: int, frequency: int) -> int:
+    # This has to be redesigned to use datetime directly
+    # But it seems to work though
+    # TODO: change this shit
     if last_update and last_update + frequency > int(
         datetime.datetime.now().strftime("%Y%m%d%H")
     ):
         return (last_update + frequency) - int(
             datetime.datetime.now().strftime("%Y%m%d%H")
         )
     else:
@@ -179,35 +168,31 @@
             )
 
 
 def updater(
     sync_repo: bool = False,
     frequency: int = 12,
     do_not_remove_pid: bool = False,
-    anti_hijack: bool = True,
     last_update: int = 0,
     force: bool = False,
     quiet: bool = False,
 ) -> None:
     process = SignalHandler()
     while not process.stopped:
-
         hours_left = time_left(last_update=last_update, frequency=frequency)
         if hours_left:
             if not quiet:
                 print(
                     f"{Font.BOLD}==> Update was already done, waiting {hours_left} hour(s)...{Font.DEFAULT}"
                 )
             x = 1
             while hours_left:
                 hours_left = time_left(last_update=last_update, frequency=frequency)
                 if process.stopped:
                     break
-                elif x % 60 and anti_hijack:
-                    launch_anti_hijack(quiet)
                 time.sleep(1)
                 x += 1
 
         if process.stopped:
             if not do_not_remove_pid:
                 os.remove(Path.DAEMON_PID)
             log_message(
@@ -258,14 +243,15 @@
                 pass
             except FileNotFoundError as err:
                 log_message(
                     "[tblockd] ERROR:  PID: {0}; caught FileNotFoundError: {1}".format(
                         os.getpid(), err.__str__()
                     )
                 )
+            del f
 
         save_update_time()
 
         # Unlock the database
         unlock_db()
 
         log_message(
@@ -275,16 +261,14 @@
             print(
                 f"{Font.BOLD}==> Waiting {frequency} hour(s) until next update...{Font.DEFAULT}"
             )
         x = 1
         while x <= frequency * 3600:
             if process.stopped:
                 break
-            elif x % 60 and anti_hijack:
-                launch_anti_hijack(quiet)
             time.sleep(1)
             x += 1
     else:
         if not do_not_remove_pid:
             os.remove(Path.DAEMON_PID)
         log_message(
             "[tblockd] INFO:  caught {0}; PID: {1}; stopping now".format(
```

### Comparing `tblock-2.6.1/tblock/daemon/__main__.py` & `tblock-2.7.1/tblock/daemon/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
```

### Comparing `tblock-2.6.1/tblock/exceptions.py` & `tblock-2.7.1/tblock/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
```

### Comparing `tblock-2.6.1/tblock/filters.py` & `tblock-2.7.1/tblock/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -26,27 +26,37 @@
 import io
 import os.path
 import sqlite3
 import json
 import hashlib
 import lzma
 import gzip
+import warnings
+import shutil
 from colorama import Fore, Style
 
 # Local modules
-from .const import FilterPermissions, WARNS, RulePolicy, USER_RULE_PRIORITY, Profile
+from .const import (
+    WARNS,
+    RulePolicy,
+    USER_RULE_PRIORITY,
+    Profile,
+    Components,
+    FilterPermissions,
+)
 from .style import Icon, Font, loading_icon
 from .config import Path, Var
 from .utils import (
     fetch_file,
     prompt_user,
     is_url,
     check_root_access,
     lock_db,
     unlock_db,
+    get_user_response,
 )
 from .exceptions import FilterError, RepoError, FilterSyntaxError
 from .converter import detect_syntax, FilterParser, ALL_SYNTAX
 from .hosts import update_hosts
 from .rules import Rule, __remove_allowed_matches
 
 # To avoid confusion when updating the filter list repository
@@ -68,15 +78,15 @@
         self.quiet = quiet
 
         # Fetch filter list data from the database
         with sqlite3.connect(Path.DATABASE) as conn:
             data = (
                 conn.cursor()
                 .execute(
-                    "SELECT source, metadata, subscribing, on_repo, permissions, mirrors, syntax, rules_count "
+                    "SELECT source, metadata, subscribing, on_repo, mirrors, syntax, rules_count "
                     "FROM filters WHERE id=?;",
                     (self.id,),
                 )
                 .fetchone()
             )
 
         self.exists = bool(data)
@@ -99,25 +109,32 @@
             self.source_exists = True
         else:
             self.source_exists = False
 
         self.metadata = json.loads(data[1]) if self.exists else {}
         self.subscribing = bool(data[2]) if self.exists else False
         self.on_repo = bool(data[3]) if self.exists else False
-        self.permissions = FilterPermissions(data[4]) if self.exists else None
-        self.mirrors = json.loads(data[5]) if (self.exists and data[5]) else {}
-        self.syntax = data[6] if self.exists else None
-        self.rules_count = data[7] if self.exists else 0
+        self.mirrors = json.loads(data[4]) if (self.exists and data[4]) else {}
+        self.syntax = data[5] if self.exists else None
+        self.rules_count = data[6] if self.exists and data[6] else 0
         self.tmp_file = os.path.join(
             Path.TMP_DIR, self.id.replace(":", "_").replace("/", "_").replace("?", "_")
         )
         self.cache_file = os.path.join(
             Path.CACHE, self.id.replace(":", "_").replace("/", "_").replace("?", "_")
         )
 
+    @property
+    def permissions(self) -> FilterPermissions:
+        warnings.warn(
+            "This property is no longer useful, since permissions do not exist anymore.",
+            DeprecationWarning,
+        )
+        return FilterPermissions("AB") if self.exists else None
+
     def retrieve_mirror(self, mirror: str, compression: str = None) -> bool:
         """
         Retrieve a mirror of a filter list when the main location is unreachable
 
         :param mirror: The mirror to retrieve
         :param compression: Optional. Specify the compression algorithm for the mirror (xz/gzip)
 
@@ -272,19 +289,19 @@
             )
         elif (
             self.cache_is_up_to_date()
             and self.get_rules_count() == self.rules_count
             and not force
         ):
             if not self.quiet:
-                print(f" {Icon.SUCCESS} " + "Filter list is up-to-date")
+                print(f" {Icon.INFORMATION} " + "Nothing to update")
         else:
-
             # Remove rules from this filter lists
-            self.delete_all_rules()
+            if self.rules_count != 0:
+                self.delete_all_rules()
 
             if self.syntax is None:
                 with io.open(self.tmp_file, "rt") as f:
                     lines = f.readlines()
                     if not self.quiet:
                         __msg = "Detecting filter list syntax"
                         print(f" {loading_icon(1)} {__msg}", end="\r")
@@ -292,23 +309,21 @@
                     with sqlite3.connect(Path.DATABASE) as conn:
                         conn.cursor().execute(
                             "UPDATE filters SET syntax=? WHERE id=?",
                             (self.syntax, self.id),
                         )
                     if not self.quiet:
                         print(f" {Icon.SUCCESS} {__msg}")
-
-            if not self.quiet:
-                print(
-                    f" {Icon.INFORMATION} "
-                    + "Filter list syntax is: {0}".format(self.syntax)
-                )
+                        print(
+                            f" {Icon.INFORMATION} "
+                            + "Filter list syntax is: {0}".format(self.syntax)
+                        )
 
             parser = FilterParser(self.tmp_file, self.syntax, self.quiet)
-            parser.insert_rules_to_database(self.id, self.permissions)
+            parser.insert_rules_to_database(self.id)
 
             # Move downloaded filter list to cache and insert its hash into the database
             with open(self.tmp_file, "rb") as f:
                 content = f.read()
             shasum = hashlib.sha512(content).hexdigest()
             with sqlite3.connect(Path.DATABASE) as conn:
                 try:
@@ -318,81 +333,85 @@
                     )
                 except sqlite3.IntegrityError:
                     conn.cursor().execute(
                         "UPDATE cache SET sha512=? WHERE key=?;", (shasum, self.id)
                     )
                 conn.commit()
 
-            with open(self.tmp_file, "rt") as f:
-                with open(self.cache_file, "wt") as w:
-                    w.write(f.read())
+            shutil.copy(self.tmp_file, self.cache_file)
 
             # Store initial rule count
             with sqlite3.connect(Path.DATABASE) as conn:
-
                 conn.cursor().execute(
                     "UPDATE filters SET rules_count=? WHERE id=?",
                     (self.get_rules_count(), self.id),
                 )
                 conn.commit()
 
             # Delete temporary file
             os.remove(self.tmp_file)
 
     def delete_all_rules(self) -> None:
         """
         Delete all rules that are set by the filter list
         """
-        __msg = "Cleaning rules cache:"
+        __msg = "Deleting previous rules:"
         if not self.quiet:
-            print(f" {Icon.LOADING_1} {__msg} 0", end="\r")
+            print(f" {loading_icon(1)} {__msg} 0", end="\r")
         with sqlite3.connect(Path.DATABASE) as conn:
             conn.cursor().execute('DELETE FROM "rules" WHERE filter_id=?;', (self.id,))
             conn.cursor().execute(
                 "UPDATE filters SET rules_count=? WHERE id=?;", (None, self.id)
             )
             conn.commit()
             total_changes = conn.total_changes - 1
         if not self.quiet:
             print(f" {Icon.SUCCESS} {__msg} {total_changes}")
 
-    def subscribe(
-        self, permissions: FilterPermissions = Var.DEFAULT_PERMISSIONS
-    ) -> None:
+    def subscribe(self, permissions=None) -> None:
         """
         Mark the filter list as "subscribed" in the database
 
-        :param permissions: Optional. Permissions to grant to filter list. Defaults to `tblock.DEFAULT_PERMISSIONS`
+        :param permissions: Deprecated parameter only kept for compatibility purposes
         """
         if not os.path.isfile(self.tmp_file):
             raise FilterError(
                 "filter list needs to be downloaded before updating its rule"
             )
         elif self.subscribing:
             if not self.quiet:
                 print(f" {Icon.WARNING} Already subscribing to filter list: {self.id}")
         else:
-            __msg = "Marking filter list as subscribed in database"
+            __msg = f"Subscribing to: {self.id}"
             if not self.quiet:
                 print(f" {loading_icon(1)} {__msg}", end="\r")
             with sqlite3.connect(Path.DATABASE) as conn:
                 conn.cursor().execute(
-                    "UPDATE filters SET subscribing=?, permissions=? WHERE id=?",
-                    (int(True), permissions.compacted, self.id),
+                    "UPDATE filters SET subscribing=? WHERE id=?",
+                    (int(True), self.id),
                 )
-                self.permissions = permissions
                 self.subscribing = True
             if not self.quiet:
                 if self.on_repo:
-                    if self.metadata["warning"] > 0:
-                        print(
-                            f" {Icon.WARNING} Warning: filter list {WARNS[self.metadata['warning']]}"
-                        )
+                    if (
+                        "deprecated" in self.metadata.keys()
+                        and self.metadata["deprecated"]
+                    ):
+                        print(f" {Icon.WARNING} Warning: {self.id} is deprecated")
                 print(f" {Icon.SUCCESS} {__msg}")
 
+    def change_permissions(self, permissions=None) -> None:
+        """
+        Deprecated method only kept for compatibility purposes
+        """
+        warnings.warn(
+            "This method is no longer useful, since permissions do not exist anymore.",
+            DeprecationWarning,
+        )
+
     def add_custom(self, custom_syntax: str = None) -> None:
         """
         Add custom filter lists to database
 
         :param custom_syntax: Optional. Specify the syntax of the custom filter list
 
         Note:
@@ -421,23 +440,22 @@
                 self.source = os.path.realpath(self.source)
 
             __msg = "Inserting filter list into database:"
             if not self.quiet:
                 print(f" {loading_icon(1)} {__msg} {self.id}", end="\r")
             with sqlite3.connect(Path.DATABASE) as conn:
                 conn.cursor().execute(
-                    "INSERT INTO filters (id, source, metadata, subscribing, on_repo, permissions, mirrors, syntax)"
-                    "VALUES (?, ?, ?, ?, ?, ?, ?, ?);",
+                    "INSERT INTO filters (id, source, metadata, subscribing, on_repo, mirrors, syntax)"
+                    "VALUES (?, ?, ?, ?, ?, ?, ?);",
                     (
                         self.id,
                         self.source,
                         json.dumps({}),
                         int(False),
                         int(False),
-                        None,
                         json.dumps({}),
                         custom_syntax,
                     ),
                 )
             self.exists = True
             self.syntax = custom_syntax
             if not self.quiet:
@@ -449,15 +467,15 @@
         """
         if not self.subscribing and self.on_repo:
             if not self.quiet:
                 print(" {Icon.WARNING} " + "Not subscribing to filter list")
         else:
             self.delete_all_rules()
             if self.on_repo:
-                __msg = "Marking filter list as unsubscribed in database"
+                __msg = f"Removing: {self.id}"
                 if not self.quiet:
                     print(f" {loading_icon(1)} {__msg}", end="\r")
                 with sqlite3.connect(Path.DATABASE) as conn:
                     conn.cursor().execute(
                         "UPDATE filters SET subscribing=? WHERE id=?",
                         (int(False), self.id),
                     )
@@ -473,38 +491,14 @@
                 with sqlite3.connect(Path.DATABASE) as conn:
                     conn.cursor().execute("DELETE FROM filters WHERE id=?", (self.id,))
                 self.__init__(self.id, quiet=self.quiet, custom_source=self.source)
                 if not self.quiet:
                     print(f" {Icon.SUCCESS} {__msg}")
             # self.delete_cache()
 
-    def change_permissions(
-        self, permissions: FilterPermissions = Var.DEFAULT_PERMISSIONS
-    ) -> None:
-        """
-        Change the permissions of a filter list
-
-        :param permissions: Optional. Permissions to grant to filter list. Defaults to `tblock.DEFAULT_PERMISSIONS`
-        """
-        if not self.subscribing:
-            if not self.quiet:
-                print(f" {Icon.WARNING} Not subscribing to filter list")
-        else:
-            __msg = "Changing permissions of filter list: {0}".format(self.id)
-            if not self.quiet:
-                print(f" {loading_icon(1)} {__msg}", end="\r")
-            with sqlite3.connect(Path.DATABASE) as conn:
-                conn.cursor().execute(
-                    "UPDATE filters SET permissions=? WHERE id=?",
-                    (permissions.compacted, self.id),
-                )
-                self.permissions = permissions
-            if not self.quiet:
-                print(f" {Icon.SUCCESS} {__msg}")
-
     def rename_custom(self, filter_id: str) -> None:
         """
         Change the ID of a custom filter list
 
         :param filter_id: The new ID to use
         """
         if self.on_repo:
@@ -545,14 +539,16 @@
     Check every filter list of a list and returns True if all filter lists exist or are custom
 
     :param filter_lists: The list of filter lists to check
     :param custom_sources: Optional. If custom, list containing sources, ordered in the same order as filter lists
 
     :return: bool. True if all filter lists exist or are custom. Otherwise, raise a FilterError
     """
+    if custom_sources is not None and len(filter_lists) != len(custom_sources):
+        raise FilterError("one filter list ID should be provided for each source")
     for filter_id in filter_lists:
         # Define filter list object
         if custom_sources:
             filter_object = Filter(
                 filter_id, custom_sources[filter_lists.index(filter_id)]
             )
         else:
@@ -704,27 +700,29 @@
 
 def subscribe(
     filter_lists: list,
     do_not_prompt: bool = False,
     quiet: bool = False,
     sync_repo: bool = False,
     full_update: bool = False,
-    permissions: FilterPermissions = Var.DEFAULT_PERMISSIONS,
     force: bool = False,
+    rebuild_hosts: bool = True,
+    permissions=None,
 ) -> None:
     """
     Subscribe to a given list of filter lists
 
     :param filter_lists: The filter lists IDs
     :param do_not_prompt: Optional. Do not prompt before subscribing (false by default)
     :param quiet: Optional. Do not display an output (false by default)
     :param sync_repo: Optional. Also sync the filter lists repository before subscribing (false by default)
     :param full_update: Optional. Also update all filter lists before subscribing (false by default)
-    :param permissions: Optional. Permissions to grant to filter list. Defaults to `.DEFAULT_PERMISSIONS`
     :param force: Optional. Force updating, even if filter list or the filter list repository is up-to-date
+    :param rebuild_hosts: Optional. Rebuild the hosts file after the operation is done (true by default)
+    :param permissions: Deprecated parameter only kept for compatibility purposes
     """
 
     # Check root access
     if not check_root_access():
         raise PermissionError("you need to run as root to perform this operation")
 
     # Lock database
@@ -744,30 +742,31 @@
                 if full_update:
                     update_all(
                         do_not_prompt=True,
                         quiet=quiet,
                         sync_repo=False,
                         force=force,
                         blacklist=filter_lists,
-                        also_update_hosts=False,
+                        rebuild_hosts=False,
                         lock_database=False,
                     )
                 # Then, retrieve them
                 __retrieve_filter_lists(filter_lists, quiet)
                 # Mark filter lists as subscribed in the database and update them
                 for filter_id in filter_lists:
                     if not quiet:
                         print(
                             f"{Font.BOLD}==> Subscribing to filter list: {filter_id}{Font.DEFAULT}"
                         )
                     filter_object = Filter(filter_id, quiet)
-                    filter_object.subscribe(permissions=permissions)
+                    filter_object.subscribe()
                     filter_object.update(force=force)
                 __remove_allowed_matches(quiet)
-                update_hosts(quiet=quiet)
+                if rebuild_hosts:
+                    update_hosts(quiet=quiet)
 
     else:
         # This condition is required because in the following situation:
         # if the user wants to subscribe to a filter list available in the new index but not in the local database
         # That way, TBlock syncs the repository before and no error is triggered.
         # This is mainly useful right after the installation, if the user runs: "tblock -Sy tblock-base"
         if do_not_prompt or prompt_user(
@@ -778,122 +777,74 @@
                 if full_update:
                     update_all(
                         do_not_prompt=True,
                         quiet=quiet,
                         sync_repo=False,
                         force=force,
                         blacklist=filter_lists,
-                        also_update_hosts=False,
+                        rebuild_hosts=False,
                         lock_database=False,
                     )
                 # Then, retrieve them
                 __retrieve_filter_lists(filter_lists, quiet)
                 # Mark filter lists as subscribed in the database and update them
                 for filter_id in filter_lists:
                     if not quiet:
                         print(
                             f"{Font.BOLD}==> Subscribing to filter list: {filter_id}{Font.DEFAULT}"
                         )
                     filter_object = Filter(filter_id, quiet)
-                    filter_object.subscribe(permissions=permissions)
+                    filter_object.subscribe()
                     filter_object.update(force=force)
                 __remove_allowed_matches(quiet)
-                update_hosts(quiet=quiet)
+                if rebuild_hosts:
+                    update_hosts(quiet=quiet)
 
     # Unlock the database
     unlock_db()
 
 
 def change_permissions(
     filter_lists: list,
-    permissions: FilterPermissions,
+    permissions,
     do_not_prompt: bool = False,
     quiet: bool = False,
     sync_repo: bool = False,
     full_update: bool = False,
     force: bool = False,
+    rebuild_hosts: bool = True,
 ) -> None:
     """
-    Change the permissions of a given list of filter lists
-
-    :param filter_lists: The filter lists IDs
-    :param permissions: Optional. Permissions to grant to filter list. Defaults to `tblock.DEFAULT_PERMISSIONS`
-    :param do_not_prompt: Optional. Do not prompt before subscribing (false by default)
-    :param quiet: Optional. Do not display an output (false by default)
-    :param sync_repo: Optional. Also sync the filter lists repository before subscribing (false by default)
-    :param full_update: Optional. Also update all filter lists before subscribing (false by default)
-    :param force: Optional. Force updating, even if filter list or the filter list repository is up-to-date
+    Deprecated function only kept for compatibility purposes
     """
-
-    # Check root access
-    if not check_root_access():
-        raise PermissionError("you need to run as root to perform this operation")
-
-    # Lock the database
-    lock_db()
-
-    # Check all filter lists
-    if __check_filter_lists_validity_subscribed(filter_lists):
-        # Prompt the user before continuing
-        if do_not_prompt or prompt_user(
-            "You are about to change the permissions of the following filters:",
-            filter_lists,
-        ):
-            # Sync the upstream filter lists repository if needed
-            if sync_repo:
-                sync_filter_list_repo(force=force, quiet=quiet, lock_database=False)
-
-            if full_update:
-                update_all(
-                    do_not_prompt=True,
-                    quiet=quiet,
-                    sync_repo=False,
-                    force=force,
-                    blacklist=filter_lists,
-                    also_update_hosts=False,
-                    lock_database=False,
-                )
-            # Change filter lists permissions
-            for filter_id in filter_lists:
-                filter_object = Filter(filter_id, quiet)
-                filter_object.change_permissions(permissions=permissions)
-            # Then, retrieve them
-            __retrieve_filter_lists(filter_lists, quiet)
-            # Mark filter lists as subscribed in the database and update them
-            for filter_id in filter_lists:
-                if not quiet:
-                    print(
-                        f"{Font.BOLD}==> Updating filter list: {filter_id}{Font.DEFAULT}"
-                    )
-                filter_object = Filter(filter_id, quiet)
-                filter_object.update(force=True)
-            __remove_allowed_matches(quiet)
-            update_hosts(quiet=quiet)
-
-    # Unlock the database
-    unlock_db()
+    warnings.warn(
+        "This function is no longer useful, since permissions do not exist anymore.",
+        DeprecationWarning,
+    )
 
 
 def rename_custom(
     filter_lists: list,
     do_not_prompt: bool = False,
     quiet: bool = False,
     sync_repo: bool = False,
     full_update: bool = False,
     force: bool = False,
+    rebuild_hosts: bool = True,
 ) -> None:
     """
     Change the ID of a given list of custom filter lists
 
     :param filter_lists: The filter lists IDs, followed by new IDs, like: `["old_id1", "new_id1", "old_id2", "new_id2"]`
     :param do_not_prompt: Optional. Do not prompt before subscribing (false by default)
     :param quiet: Optional. Do not display an output (false by default)
     :param sync_repo: Optional. Also sync the filter lists repository before subscribing (false by default)
     :param full_update: Optional. Also update all filter lists before subscribing (false by default)
     :param force: Optional. Force updating, even if filter list or the filter list repository is up-to-date
+    :param rebuild_hosts: Optional. Rebuild the hosts file after the operation is done (true by default)
     """
 
     # Check root access
     if not check_root_access():
         raise PermissionError("you need to run as root to perform this operation")
 
     # Lock the database
@@ -923,53 +874,55 @@
 
             if full_update:
                 update_all(
                     do_not_prompt=True,
                     quiet=quiet,
                     sync_repo=False,
                     force=force,
-                    also_update_hosts=False,
+                    rebuild_hosts=False,
                     lock_database=False,
                 )
             # Change filter lists ID
             if not quiet:
                 print(f"{Font.BOLD}==> Renaming filter lists{Font.DEFAULT}")
             for filter_id in filter_lists:
                 filter_object = Filter(filter_id, quiet)
                 filter_object.rename_custom(new_ids[filter_lists.index(filter_id)])
-            if full_update:
+            if full_update and rebuild_hosts:
                 # If only the name of the filter changed, no need to update
                 update_hosts(quiet=quiet)
 
     # Unlock the database
     unlock_db()
 
 
 def subscribe_custom(
     filter_lists: list,
     do_not_prompt: bool = False,
     quiet: bool = False,
     sync_repo: bool = False,
     full_update: bool = False,
-    permissions: FilterPermissions = Var.DEFAULT_PERMISSIONS_CUSTOM,
     force: bool = False,
     custom_syntax: str = None,
+    rebuild_hosts: bool = True,
+    permissions=None,
 ) -> None:
     """
     Subscribe to a given list of filter lists
 
     :param filter_lists: The filter lists IDs, followed by custom sources, like:
         `["custom_1", "https://example.org/1.txt", "custom_2", "ftp://ftp.example.com/2.txt"]`
     :param do_not_prompt: Optional. Do not prompt before subscribing (false by default)
     :param quiet: Optional. Do not display an output (false by default)
     :param sync_repo: Optional. Also sync the filter lists repository before subscribing (false by default)
     :param full_update: Optional. Also update all filter lists before subscribing (false by default)
-    :param permissions: Optional. Permissions to grant to filter list. Defaults to `tblock.DEFAULT_PERMISSIONS_CUSTOM`
     :param force: Optional. Force updating, even if filter list or the filter list repository is up-to-date
     :param custom_syntax: Optional. Specify the syntax of the custom filter list
+    :param rebuild_hosts: Optional. Rebuild the hosts file after the operation is done (true by default)
+    :param permissions: Deprecated parameter only kept for compatibility purposes
     """
 
     # Check root access
     if not check_root_access():
         raise PermissionError("you need to run as root to perform this operation")
 
     # Lock the database
@@ -1001,15 +954,15 @@
 
             if full_update:
                 update_all(
                     do_not_prompt=True,
                     quiet=quiet,
                     sync_repo=False,
                     force=force,
-                    also_update_hosts=False,
+                    rebuild_hosts=False,
                     lock_database=False,
                 )
             # Add them to the database
             if not quiet:
                 print(
                     f"{Font.BOLD}==> Adding custom filter lists to database{Font.DEFAULT}"
                 )
@@ -1025,40 +978,43 @@
             # Mark filter lists as subscribed in the database and update them
             for filter_id in filter_lists:
                 if not quiet:
                     print(
                         f"{Font.BOLD}==> Subscribing to filter list: {filter_id}{Font.DEFAULT}"
                     )
                 filter_object = Filter(filter_id, quiet)
-                filter_object.subscribe(permissions=permissions)
+                filter_object.subscribe()
                 filter_object.update(force=force)
             __remove_allowed_matches(quiet)
-            update_hosts(quiet=quiet)
+            if rebuild_hosts:
+                update_hosts(quiet=quiet)
 
     # Unlock the database
     unlock_db()
 
 
 def unsubscribe(
     filter_lists: list,
     do_not_prompt: bool = False,
     force: bool = False,
     quiet: bool = False,
     sync_repo: bool = False,
     full_update: bool = False,
+    rebuild_hosts: bool = True,
 ) -> None:
     """
     Unsubscribe from a given list of filter lists
 
     :param filter_lists: The filter lists IDs
     :param do_not_prompt: Optional. Do not prompt before subscribing (false by default)
     :param force: Optional. Force updating, even if filter list or the filter list repository is up-to-date
     :param quiet: Optional. Do not display an output (false by default)
     :param sync_repo: Optional. Also sync the filter lists repository before subscribing (false by default)
     :param full_update: Optional. Also update all filter lists before subscribing (false by default)
+    :param rebuild_hosts: Optional. Rebuild the hosts file after the operation is done (true by default)
     """
 
     # Check root access
     if not check_root_access():
         raise PermissionError("you need to run as root to perform this operation")
 
     # Lock the database
@@ -1084,44 +1040,47 @@
                 filter_object.delete_cache()
             if full_update:
                 update_all(
                     do_not_prompt=True,
                     quiet=quiet,
                     sync_repo=False,
                     force=force,
-                    also_update_hosts=False,
+                    rebuild_hosts=False,
                     lock_database=False,
                 )
                 update_hosts(quiet=quiet)
             else:
                 __remove_allowed_matches(quiet)
-                update_hosts(quiet=quiet)
+                if rebuild_hosts:
+                    update_hosts(quiet=quiet)
                 print(
                     f" {Icon.WARNING} Always remember to update all filter lists after this operation"
                 )
 
     # Unlock the database
     unlock_db()
 
 
 def update(
     filter_lists: list,
     do_not_prompt: bool = False,
     force: bool = False,
     quiet: bool = False,
     sync_repo: bool = False,
+    rebuild_hosts: bool = True,
 ) -> None:
     """
     Update a given list of filter lists
 
     :param filter_lists: The filter lists IDs
     :param do_not_prompt: Optional. Do not prompt before subscribing (false by default)
     :param force: Optional. Force updating, even if filter list or the filter list repository is up-to-date
     :param quiet: Optional. Do not display an output (false by default)
     :param sync_repo: Optional. Also sync the filter lists repository before subscribing (false by default)
+    :param rebuild_hosts: Optional. Rebuild the hosts file after the operation is done (true by default)
     """
 
     # Check root access
     if not check_root_access():
         raise PermissionError("you need to run as root to perform this operation")
 
     # Lock the database
@@ -1143,38 +1102,39 @@
                 if not quiet:
                     print(
                         f"{Font.BOLD}==> Updating filter list: {filter_id}{Font.DEFAULT}"
                     )
                 filter_object = Filter(filter_id, quiet)
                 filter_object.update(force=force)
             __remove_allowed_matches(quiet)
-            update_hosts(quiet=quiet)
+            if rebuild_hosts:
+                update_hosts(quiet=quiet)
 
     # Unlock the database
     unlock_db()
 
 
 def update_all(
     do_not_prompt: bool = False,
     force: bool = False,
     quiet: bool = False,
     sync_repo: bool = False,
     blacklist: list = None,
-    also_update_hosts: bool = True,
+    rebuild_hosts: bool = True,
     lock_database: bool = True,
 ) -> None:
     """
     Update all subscribed filter lists
 
     :param do_not_prompt: Optional. Do not prompt before subscribing (false by default)
     :param force: Optional. Force updating, even if filter list or the filter list repository is up-to-date
     :param quiet: Optional. Do not display an output (false by default)
     :param sync_repo: Optional. Also sync the filter lists repository before subscribing (false by default)
     :param blacklist: Optional. Filter list IDs to ignore
-    :param also_update_hosts: Optional. Update hosts file after updating filter lists (true by default)
+    :param rebuild_hosts: Optional. Update hosts file after updating filter lists (true by default)
     :param lock_database: Optional. Lock the database to avoid conflict with other running instances (true by default)
     """
 
     # Check root access
     if not check_root_access():
         raise PermissionError("you need to run as root to perform this operation")
 
@@ -1199,15 +1159,15 @@
                 if not quiet:
                     print(
                         f"{Font.BOLD}==> Updating filter list: {filter_id}{Font.DEFAULT}"
                     )
                 filter_object = Filter(filter_id, quiet)
                 filter_object.update(force=force)
             __remove_allowed_matches(quiet)
-            if also_update_hosts:
+            if rebuild_hosts:
                 update_hosts(quiet=quiet)
 
     # Unlock the database
     if lock_database:
         unlock_db()
 
 
@@ -1238,18 +1198,15 @@
             print(f"{Font.BOLD}Source          : {Font.DEFAULT}{filter_object.source}")
             if filter_object.subscribing:
                 print(f"{Font.BOLD}Subscribing     : {Font.DEFAULT}yes")
                 print(
                     f"{Font.BOLD}Syntax          : {Font.DEFAULT}{filter_object.syntax}"
                 )
                 print(
-                    f"{Font.BOLD}Rules           : {Font.DEFAULT}{filter_object.get_rules_count()}"
-                )
-                print(
-                    f"{Font.BOLD}Permissions     : {Font.DEFAULT}{filter_object.permissions.compacted}"
+                    f"{Font.BOLD}Active rules    : {Font.DEFAULT}{filter_object.rules_count}"
                 )
             elif filter_object.on_repo:
                 print(f"{Font.BOLD}Subscribing     : {Font.DEFAULT}no")
                 print(
                     f"{Font.BOLD}Syntax          : {Font.DEFAULT}{filter_object.syntax}"
                 )
             if filter_object.on_repo:
@@ -1270,14 +1227,20 @@
                     )
                 try:
                     print(
                         f"{Font.BOLD}Status          : {Font.DEFAULT}{WARNS[filter_object.metadata['warning']]}"
                     )
                 except KeyError:
                     pass
+                if (
+                    "deprecated" in filter_object.metadata.keys()
+                    and filter_object.metadata["deprecated"]
+                ):
+                    print(f"{Font.BOLD}Deprecated      : {Font.DEFAULT}yes")
+
                 tag_list = ""
                 try:
                     for tag in filter_object.metadata["tags"]:
                         tag_list += tag + " "
                 except KeyError:
                     pass
                 print(f"{Font.BOLD}Tags            : {Font.DEFAULT}{tag_list}")
@@ -1628,14 +1591,15 @@
             metadata = {
                 "title": None,
                 "description": None,
                 "homepage": None,
                 "license": [],
                 "tags": [],
                 "warning": 0,
+                "deprecated": False,
             }
             syntax = None
             mirrors = {}
 
             filter_obj = Filter(_filter_list)
 
             all_filter_lists_in_new_index.append(filter_obj.id)
@@ -1660,14 +1624,16 @@
             if "mirrors" in data["filters"][_filter_list].keys():
                 for m in data["filters"][_filter_list]["mirrors"]:
                     mirrors[m[0]] = {"compression": m[1]}
             if "tags" in data["filters"][_filter_list].keys():
                 metadata["tags"] = data["filters"][_filter_list]["tags"]
             if "warning" in data["filters"][_filter_list].keys():
                 metadata["warning"] = int(data["filters"][_filter_list]["warning"])
+            if "deprecated" in data["filters"][_filter_list].keys():
+                metadata["deprecated"] = data["filters"][_filter_list]["deprecated"]
 
             if filter_obj.exists and filter_obj.on_repo:
                 try:
                     cursor.execute(
                         "UPDATE filters SET source=?, metadata=?, mirrors=?, syntax=? WHERE id=?;",
                         (
                             source,
@@ -1755,57 +1721,70 @@
 
         # Unlock the database
         if lock_database:
             unlock_db()
 
 
 def setup_profile(profile: tuple, quiet: bool = False) -> None:
-    # Check root access
-    if not check_root_access():
-        raise PermissionError("you need to run as root to perform this operation")
-    # Lock the database
     subscribe(list(profile), do_not_prompt=True, quiet=quiet, sync_repo=True)
 
 
 def init_tblock() -> None:
     # Check root access
     if not check_root_access():
         raise PermissionError("you need to run as root to perform this operation")
 
     print(
         f"\n{Font.BOLD}> Welcome to TBlock!{Font.DEFAULT}\n\n\n"
-        ":: Please choose the profile that suits your needs the best:"
+        ":: Please select the level that suits your needs the best:"
         "\n\n [0] None: lets you configure everything yourself\n"
         " [1] Light: light protection, some ads and trackers won't be blocked\n"
         " [2] Balanced: perfect solution for regular users\n"
         " [3] Aggressive: powerful, yet it may break some web pages\n"
     )
     choice = None
-    while type(choice) != tuple:
+    while choice is None:
         answer = input("Your choice [default=2]: ")
         if answer == "0":
             choice = Profile.NONE
         elif answer == "1":
             choice = Profile.LIGHT
         elif answer == "2" or answer == "":
             choice = Profile.BALANCED
         elif answer == "3":
             choice = Profile.AGGRESSIVE
         else:
             choice = None
     else:
+        if get_user_response("Block malicious websites?"):
+            choice += Components.SECURITY
+        if get_user_response("Block pornographic websites?"):
+            choice += Components.PORNOGRAPHY
+        if get_user_response("Block websites that spread fake news?"):
+            choice += Components.FAKE_NEWS
+        if get_user_response("Block websites related to addictive substances?"):
+            choice += Components.DRUGS
+        if get_user_response("Block gambling websites?"):
+            choice += Components.GAMBLING
+        if get_user_response("Block illegal websites (piracy)?"):
+            choice += Components.PIRACY
+        if get_user_response("Block cryptocurrency services?"):
+            choice += Components.CRYPTO
+        if get_user_response("Block hate speech and far-right content?"):
+            # fuck nazis 0w0
+            choice += Components.HATE
         print("\n")
         try:
-            setup_profile(choice)
+            setup_profile(tuple(choice))
         except KeyboardInterrupt:
             raise KeyboardInterrupt()
         print(
             f"\n{Font.BOLD}> Wonderful! TBlock is now protecting you!{Font.DEFAULT}\n\n"
             f"To disable it, simply run:\n    $ {Fore.GREEN}tblock{Style.RESET_ALL} -D"
             f"\nAnd then, to enable it again:\n    $ {Fore.GREEN}tblock{Style.RESET_ALL} -E\n"
             f"It is also highly recommended to read the documentation: "
-            f"https://tblock.codeberg.page/docs/"
+            f"https://docs.tblock.me"
         )
         print(
             f"\n{Font.BOLD}> The setup is now finished{Font.DEFAULT}.\nHit ENTER to exit the program."
         )
         input()
```

### Comparing `tblock-2.6.1/tblock/hosts.py` & `tblock-2.7.1/tblock/hosts.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -18,14 +18,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # Standard modules
+import shutil
 import hashlib
 import os
 import re
 import sqlite3
 
 # Local modules
 from .config import Path, Var, hosts_are_default
@@ -60,15 +61,14 @@
 def enable_protection(quiet: bool = False, do_not_prompt: bool = True) -> None:
     if not check_root_access():
         raise PermissionError("you need to run as root to perform this operation")
 
     if do_not_prompt or prompt_user(
         "You are about to replace your default hosts file with the one built by TBlock"
     ):
-
         if not quiet:
             print(f"{Font.BOLD}==> Applying built hosts file")
 
         if hosts_are_default():
             if os.path.isfile(Path.BUILT_HOSTS_BACKUP):
                 if not quiet:
                     print(f" {loading_icon(1)} Checking checksum", end="\r")
@@ -77,60 +77,58 @@
                         conn.cursor()
                         .execute(
                             "SELECT value FROM system WHERE variable='hosts_shasum';",
                         )
                         .fetchone()[0]
                     )
                 with open(os.path.join(Path.BUILT_HOSTS_BACKUP), "rb") as f:
-                    content = f.read()
-                    shasum = hashlib.sha512(content).hexdigest()
-                if s == shasum:
+                    shasum = hashlib.sha512()
+                    for line in f:
+                        shasum.update(line)
+                if s == shasum.hexdigest():
                     if not quiet:
                         print(f" {Icon.SUCCESS} Checking checksum")
                     __msg = "Saving default hosts file"
                     if not quiet:
                         print(f" {loading_icon(1)} {__msg}", end="\r")
-                    with open(Path.HOSTS, "rt") as f:
-                        default_hosts = f.read()
-                    with open(Path.HOSTS_BACKUP, "wt") as w:
-                        w.write(default_hosts)
+                    shutil.copy(Path.HOSTS, Path.HOSTS_BACKUP)
                     if not quiet:
                         print(f" {Icon.SUCCESS} {__msg}")
-                        print(f" {loading_icon(1)} Applying built hosts file", end="\r")
-                    with open(Path.HOSTS, "wb") as f:
-                        f.write(content)
+                        print(
+                            f" {loading_icon(1)} Applying previously built hosts file",
+                            end="\r",
+                        )
+                    shutil.copy(Path.BUILT_HOSTS_BACKUP, Path.HOSTS)
                     os.remove(Path.BUILT_HOSTS_BACKUP)
                     if not quiet:
-                        print(f" {Icon.SUCCESS} Applying built hosts file")
+                        print(f" {Icon.SUCCESS} Applying previously built hosts file")
                         print(f" {Icon.INFORMATION} " + "Protection is now enabled")
                 else:
                     if not quiet:
                         print(f" {Icon.ERROR} Checking checksum")
                         print(
-                            f" {Icon.INFORMATION} Run tblock -H to build the hosts file"
+                            f" {Icon.INFORMATION} Run tblock -B to build the hosts file"
                         )
                         raise SystemExit(1)
             elif not quiet:
                 print(f" {Icon.WARNING} TBlock has never built the hosts file")
-                print(f" {Icon.INFORMATION} Run tblock -H to build the hosts file")
+                print(f" {Icon.INFORMATION} Run tblock -B to build the hosts file")
         elif not quiet:
             print(f" {Icon.WARNING} Protection is already active")
-            print(f" {Icon.INFORMATION} Run tblock -H to rebuild the hosts file")
+            print(f" {Icon.INFORMATION} Run tblock -B to rebuild the hosts file")
 
 
 def update_hosts(quiet: bool = False, do_not_prompt: bool = True) -> None:
-
     # Check root access
     if not check_root_access():
         raise PermissionError("you need to run as root to perform this operation")
 
-    if do_not_prompt or prompt_user("You are about to update your hosts file"):
-
+    if do_not_prompt or prompt_user("You are about to build a whole new hosts file"):
         if not quiet:
-            print(f"{Font.BOLD}==> Updating hosts file")
+            print(f"{Font.BOLD}==> Building hosts file")
 
         # Backup hosts if tblock is not yet active
         if hosts_are_default():
             enabling_protection = True
             __msg = "Saving default hosts file"
             if not quiet:
                 print(f" {loading_icon(1)} {__msg}", end="\r")
@@ -153,115 +151,126 @@
             rules = cursor.execute(
                 "SELECT domain, policy, ip FROM r WHERE policy != ? ORDER BY domain ASC;",
                 (RulePolicy.ALLOW,),
             )
 
             db2 = sqlite3.connect(Path.DATABASE)
             cursor2 = db2.cursor()
-            total_rules += cursor2.execute("SELECT COUNT() FROM rules;").fetchone()[0]
+            total_rules2 = cursor2.execute("SELECT COUNT() FROM rules;").fetchone()[0]
             rules2 = cursor2.execute(
                 "SELECT domain, policy, ip FROM rules WHERE policy != ? ORDER BY domain ASC;",
                 (RulePolicy.ALLOW,),
             )
             count = 0
             invalid = False
-            __msg = "Retrieving rules:"
             w.write(
                 f"# This file is generated by TBlock\n"
                 f"# Do not edit it manually, otherwise your changes will be overwritten"
                 f"\n\n# ----- DEFAULT HOSTS -----\n{default_hosts}\n\n# ----- CUSTOM RULES -----\n"
             )
         with open(os.path.join(Path.TMP_DIR, "hosts.txt"), "at") as w:
             content = ""
+            __msg = "Processing user rules:"
+            if not quiet:
+                print(
+                    f" {loading_icon(count)} {__msg} {count}/{total_rules} (0%)",
+                    end="\r",
+                )
             for row in rules:
                 count += 1
-                percent = int(count * 100 / total_rules)
-                if not quiet:
-                    print(
-                        f" {loading_icon(count)} {__msg} {count}/{total_rules} ({percent}%)",
-                        end="\r",
-                    )
                 if not invalid:
                     if row[1] == RulePolicy.BLOCK:
                         content += f"{Var.DEFAULT_IP}\t\t{row[0]}\n"
                         if Var.ALLOW_IPV6:
                             content += f"{Var.DEFAULT_IPV6}\t\t\t{row[0]}\n"
                     elif row[1] == RulePolicy.REDIRECT:
                         content += f"{row[2]}\t\t{row[0]}\n"
                 if count % 100000 == 0:
+                    percent = int(count * 100 / total_rules)
+                    if not quiet:
+                        print(
+                            f" {loading_icon(count / 100000)} {__msg} {count}/{total_rules} ({percent}%)",
+                            end="\r",
+                        )
                     w.write(content)
                     content = ""
+            if not quiet:
+                print(f" {Icon.SUCCESS} {__msg} {total_rules}/{total_rules} (100%)")
             content += "\n\n# ----- TBLOCK RULES -----\n"
             db.close()
             w.write(content)
             content = ""
+            __msg = "Processing rules:"
+            if not quiet:
+                print(
+                    f" {loading_icon(count)} {__msg} {count}/{total_rules2} (0%)",
+                    end="\r",
+                )
             for row in rules2:
                 count += 1
-                percent = int(count * 100 / total_rules)
-                if not quiet:
-                    print(
-                        f" {loading_icon(count)} {__msg} {count}/{total_rules} ({percent}%)",
-                        end="\r",
-                    )
                 if not invalid:
                     if row[1] == RulePolicy.BLOCK:
                         content += f"{Var.DEFAULT_IP}\t\t{row[0]}\n"
                         if Var.ALLOW_IPV6:
                             content += f"{Var.DEFAULT_IPV6}\t\t\t{row[0]}\n"
                     elif row[1] == RulePolicy.REDIRECT:
                         content += f"{row[2]}\t\t{row[0]}\n"
                 if count % 100000 == 0:
+                    percent = int(count * 100 / total_rules2)
+                    if not quiet:
+                        print(
+                            f" {loading_icon(count / 100000)} {__msg} {count}/{total_rules2} ({percent}%)",
+                            end="\r",
+                        )
                     w.write(content)
                     content = ""
             db2.close()
             w.write(content)
         if not quiet:
-            print(f" {Icon.SUCCESS} {__msg} {total_rules}/{total_rules} (100%)")
+            print(f" {Icon.SUCCESS} {__msg} {total_rules2}/{total_rules2} (100%)")
 
         # Write changes into hosts file
         __msg = "Writing new hosts file"
         if not quiet:
             print(f" {loading_icon(1)} {__msg}", end="\r")
         with open(os.path.join(Path.TMP_DIR, "hosts.txt"), "rb") as f:
-            content = f.read()
-            shasum = hashlib.sha512(content).hexdigest()
+            shasum = hashlib.sha512()
+            for line in f:
+                shasum.update(line)
         with sqlite3.connect(Path.DATABASE) as conn:
             conn.cursor().execute(
-                "UPDATE system SET value=? WHERE variable='hosts_shasum';", (shasum,)
+                "UPDATE system SET value=? WHERE variable='hosts_shasum';",
+                (shasum.hexdigest(),),
             )
-        with open(Path.HOSTS, "wb") as w:
-            w.write(content)
+        shutil.copy(os.path.join(Path.TMP_DIR, "hosts.txt"), Path.HOSTS)
         if not quiet:
             print(f" {Icon.SUCCESS} {__msg}")
         if not quiet and enabling_protection:
             print(f" {Icon.INFORMATION} " + "Protection is now enabled")
 
 
 def restore_hosts(quiet: bool = False, do_not_prompt: bool = True) -> None:
-
     # Check root access
     if not check_root_access():
         raise PermissionError("you need to run as root to perform this operation")
 
     if not hosts_are_default():
         if do_not_prompt or prompt_user("You are about to update your hosts file"):
-            __msg = "Restoring default hosts file"
+            __msg = "Restoring stock hosts file"
             if not quiet:
                 print(f"{Font.BOLD}==> {__msg}")
-                print(f" {loading_icon(1)} Saving built hosts file", end="\r")
-            with open(Path.HOSTS, "rt") as f:
-                with open(Path.BUILT_HOSTS_BACKUP, "wt") as w:
-                    w.write(f.read())
+                print(
+                    f" {loading_icon(1)} Backing up previously built hosts file",
+                    end="\r",
+                )
+            shutil.copy(Path.HOSTS, Path.BUILT_HOSTS_BACKUP)
             if not quiet:
-                print(f" {Icon.SUCCESS} Saving built hosts file")
+                print(f" {Icon.SUCCESS} Backing up previously built hosts file")
                 print(f" {loading_icon(1)} {__msg}", end="\r")
-            with open(Path.HOSTS_BACKUP, "rt") as f:
-                content = f.read()
-            with open(Path.HOSTS, "wt") as w:
-                w.write(content)
+            shutil.copy(Path.HOSTS_BACKUP, Path.HOSTS)
             os.remove(Path.HOSTS_BACKUP)
             if not quiet:
                 print(f" {Icon.SUCCESS} {__msg}")
                 print(f" {Icon.WARNING} " + "Protection is now disabled")
     else:
         raise HostsError("default hosts file already restored")
```

### Comparing `tblock-2.6.1/tblock/rules.py` & `tblock-2.7.1/tblock/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -126,22 +126,20 @@
             raise RuleError("Invalid domain rule: {0}".format(self.domain))
         else:
             if (
                 policy == RulePolicy.ALLOW
                 or policy == RulePolicy.BLOCK
                 or policy == RulePolicy.REDIRECT
             ):
-
                 if policy != RulePolicy.REDIRECT or is_valid_ip(ip):
                     __msg = "Adding rule for domain: {0}".format(self.domain)
                     if not quiet:
                         print(f" {loading_icon(1)} {__msg}", end="\r")
 
                     if policy == RulePolicy.ALLOW or not self.wildcard_exists():
-
                         if policy == RulePolicy.REDIRECT:
                             ip_address = ipaddress.ip_address(ip)
                             if self.exists and self.filter_id == USER_RULE_PRIORITY:
                                 with sqlite3.connect(Path.RULES_DATABASE) as conn:
                                     conn.cursor().execute(
                                         "UPDATE r SET policy=?, ip=? WHERE domain=?;",
                                         (policy, ip_address.compressed, self.domain),
@@ -528,15 +526,18 @@
         if data2 is not None:
             for rule in data2:
                 output.append(rule[0])
         return output
 
 
 def list_rules(
-    from_filter_lists: list = None, user_only: bool = False, standard_only: bool = False
+    from_filter_lists: list = None,
+    user_only: bool = False,
+    standard_only: bool = False,
+    quiet: bool = False,
 ) -> None:
     """
     List rules stored in the database
 
     :param from_filter_lists: List only rules that are set by specified filter lists
     :param user_only: List only user rules
     :param standard_only: List only rules that are set by filter lists (that are not set by the user)
@@ -574,28 +575,34 @@
                 )
             with sqlite3.connect(Path.DATABASE) as conn:
                 data2 = conn.cursor().execute(
                     'SELECT "domain", "policy", "ip" FROM "rules" ORDER BY domain ASC;'
                 )
 
         for rule in data:
-            if rule[1] == RulePolicy.ALLOW:
-                print("ALLOW    " + rule[0])
-            elif rule[1] == RulePolicy.BLOCK:
-                print("BLOCK    " + rule[0])
-            elif rule[1] == RulePolicy.REDIRECT:
-                print("REDIRECT " + rule[0] + " -> " + rule[2])
-        if data2 is not None:
-            for rule in data2:
+            if quiet:
+                print(rule[0])
+            else:
                 if rule[1] == RulePolicy.ALLOW:
                     print("ALLOW    " + rule[0])
                 elif rule[1] == RulePolicy.BLOCK:
                     print("BLOCK    " + rule[0])
                 elif rule[1] == RulePolicy.REDIRECT:
                     print("REDIRECT " + rule[0] + " -> " + rule[2])
+        if data2 is not None:
+            for rule in data2:
+                if quiet:
+                    print(rule[0])
+                else:
+                    if rule[1] == RulePolicy.ALLOW:
+                        print("ALLOW    " + rule[0])
+                    elif rule[1] == RulePolicy.BLOCK:
+                        print("BLOCK    " + rule[0])
+                    elif rule[1] == RulePolicy.REDIRECT:
+                        print("REDIRECT " + rule[0] + " -> " + rule[2])
 
 
 def get_rules_count() -> int:
     with sqlite3.connect(Path.DATABASE) as db:
         count = db.cursor().execute("SELECT COUNT() FROM rules;").fetchone()[0]
     with sqlite3.connect(Path.RULES_DATABASE) as db:
         return count + db.cursor().execute("SELECT COUNT() FROM r;").fetchone()[0]
```

### Comparing `tblock-2.6.1/tblock/style.py` & `tblock-2.7.1/tblock/style.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -122,18 +122,25 @@
 def show_status(quiet: bool = False) -> None:
     if not os.path.isfile(Path.DATABASE):
         raise FileNotFoundError(
             "database does not exist yet. "
             "Please run 'tblock -Y' with admin privileges to create it"
         )
     with sqlite3.connect(Path.DATABASE) as db:
-        total_rules = db.cursor().execute("SELECT COUNT() FROM rules;").fetchone()[0]
+        total_rules = (
+            db.cursor()
+            .execute(
+                "SELECT SUM(rules_count) FROM filters "
+                "WHERE rules_count IS NOT NULL and rules_count!=0 AND subscribing=1;"
+            )
+            .fetchone()[0]
+        )
         total_filter_lists = (
             db.cursor()
-            .execute("SELECT COUNT() FROM filters WHERE subscribing=1;")
+            .execute("SELECT COUNT(id) FROM filters WHERE subscribing=1;")
             .fetchone()[0]
         )
     if not quiet:
         print(
             f"{Font.BOLD}{Fore.LIGHTMAGENTA_EX}\n"
             f"       xxxxxxxxxxxx          TBlock v{VERSION}\n"
             f"    xxxxxxxxxxxxxxxxxx       {Font.DEFAULT}{Fore.RESET}-------------{Font.BOLD}{Fore.LIGHTMAGENTA_EX}\n"
```

### Comparing `tblock-2.6.1/tblock/utils.py` & `tblock-2.7.1/tblock/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -66,20 +66,24 @@
                 pid = int(r.read())
             if pid == os.getpid():
                 os.remove(Path.DB_LOCK)
         except FileNotFoundError:
             pass
 
 
-def _get_user_consent() -> bool:
-    answer = input(":: Are you sure to continue ? [y/n] ")
-    while "n" != answer.lower() != "y" and answer != "":
-        answer = input(":: Are you sure to continue ? [y/n] ")
+def get_user_response(message, strict: bool = True) -> bool:
+    answer = input(message + " [y/n] ")
+    while ("n" != answer.lower() != "y") and (answer != "" or strict):
+        answer = input(message + " [y/n] ")
     else:
-        return answer.lower() == "y" or answer == ""
+        return answer.lower() == "y" or (answer == "" and not strict)
+
+
+def _get_user_consent() -> bool:
+    return get_user_response(":: Are you sure to continue ?", strict=False)
 
 
 def is_valid_ip(ip: str) -> bool:
     try:
         ipaddress.ip_address(ip)
     except ValueError:
         return False
```

### Comparing `tblock-2.6.1/tblock.egg-info/SOURCES.txt` & `tblock-2.7.1/tblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tblock-2.6.1/test/test_config.py` & `tblock-2.7.1/test/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
```

### Comparing `tblock-2.6.1/test/test_filters.py` & `tblock-2.7.1/test/test_filters.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -45,62 +45,62 @@
 tblock.config.Path.LOGS = os.path.join(__root__, "var", "log", "tblock.log")
 tblock.config.Path.TMP_DIR = os.path.join(__root__, "tmp", "tblock")
 
 tblock.config.Var.REPO_MIRRORS = ["http://127.0.0.1:12345/index.json"]
 
 
 class TestFilterClass(unittest.TestCase):
-
     def test_method_init(self):
         _create_env()
         f = tblock.Filter("test", quiet=True)
         self.assertTupleEqual(
-            (f.id, f.exists, f.source, f.source_exists, f.metadata, f.subscribing, f.on_repo, f.permissions,
-             f.mirrors, f.syntax, f.rules_count),
-            ("test", False, None, False, {}, False, False, None, {}, None, 0)
+            (
+                f.id,
+                f.exists,
+                f.source,
+                f.source_exists,
+                f.metadata,
+                f.subscribing,
+                f.on_repo,
+                f.mirrors,
+                f.syntax,
+                f.rules_count,
+            ),
+            ("test", False, None, False, {}, False, False, {}, None, 0),
         )
 
     def test_method_retrieve_mirror(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         get = f.retrieve_mirror("http://127.0.0.1:12345/test-list.txt", None)
-        self.assertTupleEqual(
-            (get, os.path.isfile(f.tmp_file)),
-            (True, True)
-        )
+        self.assertTupleEqual((get, os.path.isfile(f.tmp_file)), (True, True))
 
     def test_method_retrieve_mirror_xz(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         get = f.retrieve_mirror("http://127.0.0.1:12345/test-list.txt.xz", "xz")
-        self.assertTupleEqual(
-            (get, os.path.isfile(f.tmp_file)),
-            (True, True)
-        )
+        self.assertTupleEqual((get, os.path.isfile(f.tmp_file)), (True, True))
 
     def test_method_retrieve_mirror_gzip(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         get = f.retrieve_mirror("http://127.0.0.1:12345/test-list.txt.gz", "gzip")
-        self.assertTupleEqual(
-            (get, os.path.isfile(f.tmp_file)),
-            (True, True)
-        )
+        self.assertTupleEqual((get, os.path.isfile(f.tmp_file)), (True, True))
 
     def test_method_cache_exists_false(self):
         _create_env()
         f = tblock.Filter("test-list", quiet=True)
         self.assertFalse(f.cache_exists())
 
     def test_method_cache_exists_true(self):
@@ -128,150 +128,123 @@
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         tblock.subscribe(["test-list"], quiet=True, do_not_prompt=True)
         f = tblock.Filter("test-list")
-        self.assertEqual(
-            f.get_rules_count(),
-            6
-        )
+        self.assertEqual(f.get_rules_count(), 6)
 
     def test_method_get_rules_count_0(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         f.retrieve()
         f.subscribe()
-        self.assertEqual(
-            f.get_rules_count(),
-            0
-        )
+        self.assertEqual(f.get_rules_count(), 0)
 
     def test_method_get_rules_count_none(self):
         _create_env()
         f = tblock.Filter("test-list")
-        self.assertRaises(
-            tblock.exceptions.FilterError,
-            f.get_rules_count
-        )
+        self.assertRaises(tblock.exceptions.FilterError, f.get_rules_count)
 
     def test_method_delete_cache(self):
         _create_env()
         f = tblock.Filter("test-list", quiet=True)
         open(f.cache_file, "wt").close()
         f.delete_cache()
-        self.assertFalse(
-            os.path.isfile(f.cache_file)
-        )
+        self.assertFalse(os.path.isfile(f.cache_file))
 
     def test_method_delete_cache_none(self):
         _create_env()
         f = tblock.Filter("test-list", quiet=True)
         f.delete_cache()
-        self.assertFalse(
-            os.path.isfile(f.cache_file)
-        )
+        self.assertFalse(os.path.isfile(f.cache_file))
 
     def test_method_retrieve(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         f.retrieve()
-        self.assertTrue(
-            os.path.isfile(f.tmp_file)
-        )
+        self.assertTrue(os.path.isfile(f.tmp_file))
 
     def test_method_retrieve_unknown(self):
         _create_env()
         f = tblock.Filter("test-list", quiet=True)
-        self.assertRaises(
-            tblock.exceptions.FilterError,
-            f.retrieve
-        )
+        self.assertRaises(tblock.exceptions.FilterError, f.retrieve)
 
     def test_method_retrieve_fallback_mirror(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         f.source = "http://127.0.0.1:12345/null"
         f.mirrors = {"http://127.0.0.1:12345/test-list.txt": {"compressions": None}}
         f.retrieve()
-        self.assertTrue(
-            os.path.isfile(f.tmp_file)
-        )
+        self.assertTrue(os.path.isfile(f.tmp_file))
 
     def test_method_retrieve_fallback_mirror_xz(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         f.source = "http://127.0.0.1:12345/null"
         f.mirrors = {"http://127.0.0.1:12345/test-list.txt.xz": {"compressions": "xz"}}
         f.retrieve()
-        self.assertTrue(
-            os.path.isfile(f.tmp_file)
-        )
+        self.assertTrue(os.path.isfile(f.tmp_file))
 
     def test_method_retrieve_fallback_mirror_gzip(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         f.source = "http://127.0.0.1:12345/null"
-        f.mirrors = {"http://127.0.0.1:12345/test-list.txt.gz": {"compressions": "gzip"}}
+        f.mirrors = {
+            "http://127.0.0.1:12345/test-list.txt.gz": {"compressions": "gzip"}
+        }
         f.retrieve()
-        self.assertTrue(
-            os.path.isfile(f.tmp_file)
-        )
+        self.assertTrue(os.path.isfile(f.tmp_file))
 
     def test_method_retrieve_mirror_fallback_local_cache(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         f.retrieve()
         f.subscribe()
         f.update()
         f.source = "http://127.0.0.1:12345/null"
         f.mirrors = {}
         f.retrieve()
-        self.assertTrue(
-            os.path.isfile(f.tmp_file)
-        )
+        self.assertTrue(os.path.isfile(f.tmp_file))
 
     def test_method_retrieve_mirror_fail(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         f.source = "http://127.0.0.1:12345/null"
         f.mirrors = {}
-        self.assertRaises(
-            tblock.exceptions.FilterError,
-            f.retrieve
-        )
+        self.assertRaises(tblock.exceptions.FilterError, f.retrieve)
 
     def test_method_update(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
@@ -281,191 +254,81 @@
         f.update()
         r1 = tblock.Rule("example.org")
         r2 = tblock.Rule("block.example.com")
         r3 = tblock.Rule("allow.example.org")
         r4 = tblock.Rule("redirect.example.com")
         self.assertTupleEqual(
             (r1.filter_id, r2.filter_id, r3.exists, r4.exists),
-            ("test-list", "test-list", True, False)
-        )
-
-    def test_method_update_allow(self):
-        _create_env()
-        try:
-            tblock.sync_filter_list_repo(quiet=True)
-        except tblock.exceptions.RepoError:
-            self.skipTest("server not running")
-        f = tblock.Filter("test-list", quiet=True)
-        f.retrieve()
-        f.subscribe(permissions=tblock.FilterPermissions("A"))
-        f.update()
-        r1 = tblock.Rule("example.org")
-        r2 = tblock.Rule("block.example.com")
-        r3 = tblock.Rule("allow.example.org")
-        r4 = tblock.Rule("redirect.example.com")
-        self.assertTupleEqual(
-            (r1.exists, r2.exists, r3.filter_id, r4.exists),
-            (False, False, "test-list", False)
-        )
-
-    def test_method_update_block(self):
-        _create_env()
-        try:
-            tblock.sync_filter_list_repo(quiet=True)
-        except tblock.exceptions.RepoError:
-            self.skipTest("server not running")
-        f = tblock.Filter("test-list", quiet=True)
-        f.retrieve()
-        f.subscribe(permissions=tblock.FilterPermissions("B"))
-        f.update()
-        r1 = tblock.Rule("example.org")
-        r2 = tblock.Rule("block.example.com")
-        r3 = tblock.Rule("allow.example.org")
-        r4 = tblock.Rule("redirect.example.com")
-        self.assertTupleEqual(
-            (r1.filter_id, r2.filter_id, r3.exists, r4.exists),
-            ("test-list", "test-list", False, False)
-        )
-
-    def test_method_update_allow_redirect(self):
-        _create_env()
-        try:
-            tblock.sync_filter_list_repo(quiet=True)
-        except tblock.exceptions.RepoError:
-            self.skipTest("server not running")
-        f = tblock.Filter("test-list", quiet=True)
-        f.retrieve()
-        f.subscribe(permissions=tblock.FilterPermissions("AR"))
-        f.update()
-        r1 = tblock.Rule("example.org")
-        r2 = tblock.Rule("block.example.com")
-        r3 = tblock.Rule("allow.example.org")
-        r4 = tblock.Rule("redirect.example.com")
-        self.assertTupleEqual(
-            (r1.exists, r2.exists, r3.filter_id, r4.filter_id),
-            (False, False, "test-list", "test-list")
-        )
-
-    def test_method_update_block_redirect(self):
-        _create_env()
-        try:
-            tblock.sync_filter_list_repo(quiet=True)
-        except tblock.exceptions.RepoError:
-            self.skipTest("server not running")
-        f = tblock.Filter("test-list", quiet=True)
-        f.retrieve()
-        f.subscribe(permissions=tblock.FilterPermissions("BR"))
-        f.update()
-        r1 = tblock.Rule("example.org")
-        r2 = tblock.Rule("block.example.com")
-        r3 = tblock.Rule("allow.example.org")
-        r4 = tblock.Rule("redirect.example.com")
-        self.assertTupleEqual(
-            (r1.filter_id, r2.filter_id, r3.exists, r4.filter_id),
-            ("test-list", "test-list", False, "test-list")
-        )
-
-    def test_method_update_redirect(self):
-        _create_env()
-        try:
-            tblock.sync_filter_list_repo(quiet=True)
-        except tblock.exceptions.RepoError:
-            self.skipTest("server not running")
-        f = tblock.Filter("test-list", quiet=True)
-        f.retrieve()
-        f.subscribe(permissions=tblock.FilterPermissions("R"))
-        f.update()
-        r1 = tblock.Rule("example.org")
-        r2 = tblock.Rule("block.example.com")
-        r3 = tblock.Rule("allow.example.org")
-        r4 = tblock.Rule("redirect.example.com")
-        self.assertTupleEqual(
-            (r1.exists, r2.exists, r3.exists, r4.filter_id),
-            (False, False, False, "test-list")
-        )
-
-    def test_method_update_allow_block_redirect(self):
-        _create_env()
-        try:
-            tblock.sync_filter_list_repo(quiet=True)
-        except tblock.exceptions.RepoError:
-            self.skipTest("server not running")
-        f = tblock.Filter("test-list", quiet=True)
-        f.retrieve()
-        f.subscribe(permissions=tblock.FilterPermissions("ABR"))
-        f.update()
-        r1 = tblock.Rule("example.org")
-        r2 = tblock.Rule("block.example.com")
-        r3 = tblock.Rule("allow.example.org")
-        r4 = tblock.Rule("redirect.example.com")
-        self.assertTupleEqual(
-            (r1.filter_id, r2.filter_id, r3.filter_id, r4.filter_id),
-            ("test-list", "test-list", "test-list", "test-list")
+            ("test-list", "test-list", True, False),
         )
 
-    def test_method_update_allow_block_none(self):
+    def test_method_update_then_overwrite(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
-        except tblock.exceptions.RepoError:
+        except tblock.exceptions.RepoError as err:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         f.retrieve()
-        f.subscribe(permissions=tblock.FilterPermissions(""))
+        f.subscribe()
         f.update()
-        r1 = tblock.Rule("example.org")
-        r2 = tblock.Rule("block.example.com")
-        r3 = tblock.Rule("allow.example.org")
-        r4 = tblock.Rule("redirect.example.com")
-        self.assertTupleEqual(
-            (r1.exists, r2.exists, r3.exists, r4.exists),
-            (False, False, False, False)
-        )
+        f2 = tblock.Filter("test-list-2", quiet=True)
+        f2.retrieve()
+        f2.subscribe()
+        f2.update()
+        r1 = tblock.Rule("allow.example.org")
+        r2 = tblock.Rule("example.org")
+        r3 = tblock.Rule("allow.example.com")
+        r4 = tblock.Rule("block.example.org")
+        # Check that allowing rules are not being overwritten by allowing rules from other filter lists
+        assert r1.filter_id == "test-list"
+        assert r1.policy == "A"
+        # Check that blocking rules are being overwritten by allowing rules from other filter lists
+        assert r2.filter_id == "test-list-2"
+        assert r2.policy == "A"
+        # Check that allowing rules are not being overwritten by blocking rules from other filter lists
+        assert r3.filter_id == "test-list"
+        assert r3.policy == "A"
+        # Check that blocking rules are not being overwritten by blocking rules from other filter lists
+        assert r4.filter_id == "test-list"
+        assert r4.policy == "B"
 
     def test_method_update_not_subscribing_not_retrieved(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
-        self.assertRaises(
-            tblock.exceptions.FilterError,
-            f.update
-        )
+        self.assertRaises(tblock.exceptions.FilterError, f.update)
 
     def test_method_update_not_subscribing(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         f.retrieve()
-        self.assertRaises(
-            tblock.exceptions.FilterError,
-            f.update
-        )
+        self.assertRaises(tblock.exceptions.FilterError, f.update)
 
     def test_method_update_up_to_date(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         f.retrieve()
         f.subscribe()
         f.update()
         f.retrieve()
         status = f.cache_is_up_to_date()
         f.update()
-        self.assertTrue(
-            (os.path.isfile(f.tmp_file), status)
-        )
+        self.assertTrue((os.path.isfile(f.tmp_file), status))
 
     def test_method_delete_all_rules(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
@@ -473,332 +336,278 @@
         f.retrieve()
         f.subscribe()
         f.update()
         rb = tblock.Rule("example.org").filter_id
         f.delete_all_rules()
         self.assertTupleEqual(
             (rb, tblock.Rule("example.org").exists, f.get_rules_count()),
-            ("test-list", False, 0)
+            ("test-list", False, 0),
         )
 
     def test_method_delete_all_rules_not_subscribing(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         f.delete_all_rules()
-        self.assertFalse(
-            f.subscribing
-        )
+        self.assertFalse(f.subscribing)
 
     def test_method_subscribe(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         f.retrieve()
         f.subscribe()
-        self.assertTupleEqual(
-            (f.subscribing, f.get_rules_count()),
-            (True, 0)
-        )
+        self.assertTupleEqual((f.subscribing, f.get_rules_count()), (True, 0))
 
     def test_method_subscribe_not_retrieved(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
-        self.assertRaises(
-            tblock.exceptions.FilterError,
-            f.subscribe
-        )
+        self.assertRaises(tblock.exceptions.FilterError, f.subscribe)
 
     def test_method_subscribe_non_existing(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("null", quiet=True)
-        self.assertRaises(
-            tblock.exceptions.FilterError,
-            f.subscribe
-        )
-
-    def test_method_subscribe_perm_allow(self):
-        _create_env()
-        try:
-            tblock.sync_filter_list_repo(quiet=True)
-        except tblock.exceptions.RepoError:
-            self.skipTest("server not running")
-        f = tblock.Filter("test-list", quiet=True)
-        f.retrieve()
-        f.subscribe(permissions=tblock.FilterPermissions("A"))
-        self.assertTupleEqual(
-            (f.subscribing, f.permissions.compacted),
-            (True, tblock.FilterPermissions("A").compacted)
-        )
+        self.assertRaises(tblock.exceptions.FilterError, f.subscribe)
 
     def test_method_add_custom(self):
         _create_env()
-        f = tblock.Filter("test-list-local", quiet=True,
-                          custom_source=os.path.join(os.path.dirname(__file__), "srv", "test-list.txt"))
+        f = tblock.Filter(
+            "test-list-local",
+            quiet=True,
+            custom_source=os.path.join(
+                os.path.dirname(__file__), "srv", "test-list.txt"
+            ),
+        )
         f.add_custom()
         self.assertTupleEqual(
-            (f.exists, f.on_repo, f.subscribing),
-            (True, False, False)
+            (f.exists, f.on_repo, f.subscribing), (True, False, False)
         )
 
     def test_method_add_custom_user_id_priority(self):
         _create_env()
-        f = tblock.Filter(tblock.USER_RULE_PRIORITY, quiet=True,
-                          custom_source=os.path.join(os.path.dirname(__file__), "srv", "test-list.txt"))
-        self.assertRaises(
-            tblock.exceptions.FilterError,
-            f.add_custom
+        f = tblock.Filter(
+            tblock.USER_RULE_PRIORITY,
+            quiet=True,
+            custom_source=os.path.join(
+                os.path.dirname(__file__), "srv", "test-list.txt"
+            ),
         )
+        self.assertRaises(tblock.exceptions.FilterError, f.add_custom)
 
     def test_method_add_custom_file_not_found(self):
         _create_env()
-        f = tblock.Filter("test-list-local", quiet=True,
-                          custom_source=os.path.join(os.path.dirname(__file__), "srv", "null"))
+        f = tblock.Filter(
+            "test-list-local",
+            quiet=True,
+            custom_source=os.path.join(os.path.dirname(__file__), "srv", "null"),
+        )
         f.add_custom()
         self.assertTupleEqual(
-            (f.exists, f.on_repo, f.subscribing),
-            (True, False, False)
+            (f.exists, f.on_repo, f.subscribing), (True, False, False)
         )
 
     def test_method_add_custom_conflict_id(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
-        f = tblock.Filter("test-list", quiet=True,
-                          custom_source=os.path.join(os.path.dirname(__file__), "srv", "test-list.txt"))
-        self.assertRaises(
-            tblock.exceptions.FilterError,
-            f.add_custom
+        f = tblock.Filter(
+            "test-list",
+            quiet=True,
+            custom_source=os.path.join(
+                os.path.dirname(__file__), "srv", "test-list.txt"
+            ),
         )
+        self.assertRaises(tblock.exceptions.FilterError, f.add_custom)
 
     def test_method_add_custom_conflict_source(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
-        f = tblock.Filter("test-list-local", quiet=True,
-                          custom_source=tblock.Filter("test-list").source)
-        self.assertRaises(
-            tblock.exceptions.FilterError,
-            f.add_custom
+        f = tblock.Filter(
+            "test-list-local",
+            quiet=True,
+            custom_source=tblock.Filter("test-list").source,
         )
+        self.assertRaises(tblock.exceptions.FilterError, f.add_custom)
 
     def test_method_add_custom_no_source(self):
         _create_env()
         f = tblock.Filter("test-list-local", quiet=True)
-        self.assertRaises(
-            tblock.exceptions.FilterError,
-            f.add_custom
-        )
+        self.assertRaises(tblock.exceptions.FilterError, f.add_custom)
 
     def test_method_unsubscribe(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         f.retrieve()
         f.subscribe()
         f.update()
         f.unsubscribe()
         rb = tblock.Rule("example.org")
         self.assertTupleEqual(
-            (f.subscribing, f.on_repo, rb.exists),
-            (False, True, False)
+            (f.subscribing, f.on_repo, rb.exists), (False, True, False)
         )
 
     def test_method_unsubscribe_custom(self):
         _create_env()
-        f = tblock.Filter("test-list-local", quiet=True,
-                          custom_source=os.path.join(os.path.dirname(__file__), "srv", "test-list.txt"))
+        f = tblock.Filter(
+            "test-list-local",
+            quiet=True,
+            custom_source=os.path.join(
+                os.path.dirname(__file__), "srv", "test-list.txt"
+            ),
+        )
         f.add_custom()
         f.retrieve()
         f.subscribe()
         f.update()
         f.unsubscribe()
         rb = tblock.Rule("example.org")
         self.assertTupleEqual(
             (f.subscribing, f.on_repo, rb.exists, f.exists),
-            (False, False, False, False)
+            (False, False, False, False),
         )
 
     def test_method_unsubscribe_not_subscribing(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         f.unsubscribe()
-        self.assertTupleEqual(
-            (f.subscribing, f.on_repo),
-            (False, True)
-        )
+        self.assertTupleEqual((f.subscribing, f.on_repo), (False, True))
 
     def test_method_unsubscribe_custom_not_subscribing(self):
         _create_env()
-        f = tblock.Filter("test-list-local", quiet=True,
-                          custom_source=os.path.join(os.path.dirname(__file__), "srv", "test-list.txt"))
+        f = tblock.Filter(
+            "test-list-local",
+            quiet=True,
+            custom_source=os.path.join(
+                os.path.dirname(__file__), "srv", "test-list.txt"
+            ),
+        )
         f.add_custom()
         f.unsubscribe()
         self.assertTupleEqual(
-            (f.subscribing, f.on_repo, f.exists),
-            (False, False, False)
+            (f.subscribing, f.on_repo, f.exists), (False, False, False)
         )
 
     def test_method_unsubscribe_custom_non_existing(self):
         _create_env()
         f = tblock.Filter("test-list", quiet=True)
         f.unsubscribe()
         self.assertTupleEqual(
-            (f.subscribing, f.on_repo, f.exists),
-            (False, False, False)
-        )
-
-    def test_method_change_permissions(self):
-        _create_env()
-        try:
-            tblock.sync_filter_list_repo(quiet=True)
-        except tblock.exceptions.RepoError:
-            self.skipTest("server not running")
-        f = tblock.Filter("test-list", quiet=True)
-        f.retrieve()
-        f.subscribe()
-        f.update()
-        f.change_permissions(tblock.FilterPermissions("A"))
-        rb = tblock.Rule("example.org")
-        self.assertTupleEqual(
-            (f.permissions.compacted, rb.exists, rb.policy, rb.filter_id),
-            (tblock.FilterPermissions("A").compacted, True, tblock.BLOCK, f.id),
-        )
-
-    def test_method_change_permissions_custom(self):
-        _create_env()
-        f = tblock.Filter("test-list-local", quiet=True,
-                          custom_source=os.path.join(os.path.dirname(__file__), "srv", "test-list.txt"))
-        f.add_custom()
-        f.retrieve()
-        f.subscribe()
-        f.update()
-        f.change_permissions(tblock.FilterPermissions("A"))
-        rb = tblock.Rule("example.org")
-        self.assertTupleEqual(
-            (f.permissions.compacted, rb.exists, rb.policy, rb.filter_id),
-            (tblock.FilterPermissions("A").compacted, True, tblock.BLOCK, f.id),
-        )
-
-    def test_method_change_permissions_not_subscribing(self):
-        _create_env()
-        try:
-            tblock.sync_filter_list_repo(quiet=True)
-        except tblock.exceptions.RepoError:
-            self.skipTest("server not running")
-        f = tblock.Filter("test-list", quiet=True)
-        op = f.permissions
-        f.change_permissions(tblock.FilterPermissions("A"))
-        self.assertEqual(
-            f.permissions.compacted,
-            op.compacted
-        )
-
-    def test_method_change_permissions_non_existing(self):
-        _create_env()
-        f = tblock.Filter("test-list", quiet=True)
-        f.change_permissions(tblock.FilterPermissions("A"))
-        self.assertIsNone(
-            f.permissions
+            (f.subscribing, f.on_repo, f.exists), (False, False, False)
         )
 
     def test_method_rename(self):
         _create_env()
-        f = tblock.Filter("test-list-local", quiet=True,
-                          custom_source=os.path.join(os.path.dirname(__file__), "srv", "test-list.txt"))
+        f = tblock.Filter(
+            "test-list-local",
+            quiet=True,
+            custom_source=os.path.join(
+                os.path.dirname(__file__), "srv", "test-list.txt"
+            ),
+        )
         f.add_custom()
         f.retrieve()
         f.subscribe()
         f.update()
         f.rename_custom("test-list-renamed")
         self.assertTupleEqual(
             (tblock.Rule("example.org").filter_id, f.id),
-            ("test-list-renamed", "test-list-renamed")
+            ("test-list-renamed", "test-list-renamed"),
         )
 
     def test_method_rename_conflict_id(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
-        f = tblock.Filter("test-list-local", quiet=True,
-                          custom_source=os.path.join(os.path.dirname(__file__), "srv", "test-list.txt"))
+        f = tblock.Filter(
+            "test-list-local",
+            quiet=True,
+            custom_source=os.path.join(
+                os.path.dirname(__file__), "srv", "test-list.txt"
+            ),
+        )
         f.add_custom()
         f.retrieve()
         f.subscribe()
         f.update()
-        self.assertRaises(
-            tblock.exceptions.FilterError,
-            f.rename_custom, "test-list"
-        )
+        self.assertRaises(tblock.exceptions.FilterError, f.rename_custom, "test-list")
 
     def test_method_rename_same_id(self):
         _create_env()
-        f = tblock.Filter("test-list-local", quiet=True,
-                          custom_source=os.path.join(os.path.dirname(__file__), "srv", "test-list.txt"))
+        f = tblock.Filter(
+            "test-list-local",
+            quiet=True,
+            custom_source=os.path.join(
+                os.path.dirname(__file__), "srv", "test-list.txt"
+            ),
+        )
         f.add_custom()
         f.retrieve()
         f.subscribe()
         f.update()
         self.assertRaises(
-            tblock.exceptions.FilterError,
-            f.rename_custom, "test-list-local"
+            tblock.exceptions.FilterError, f.rename_custom, "test-list-local"
         )
 
     def test_method_rename_not_custom(self):
         _create_env()
         try:
             tblock.sync_filter_list_repo(quiet=True)
         except tblock.exceptions.RepoError:
             self.skipTest("server not running")
         f = tblock.Filter("test-list", quiet=True)
         f.retrieve()
         f.subscribe()
         f.update()
         f.rename_custom("test-list-local")
-        self.assertEqual(
-            f.id,
-            "test-list"
-        )
+        self.assertEqual(f.id, "test-list")
 
     def test_method_rename_user_id_priority(self):
         _create_env()
-        f = tblock.Filter("test-list-local", quiet=True,
-                          custom_source=os.path.join(os.path.dirname(__file__), "srv", "test-list.txt"))
+        f = tblock.Filter(
+            "test-list-local",
+            quiet=True,
+            custom_source=os.path.join(
+                os.path.dirname(__file__), "srv", "test-list.txt"
+            ),
+        )
         f.add_custom()
         f.retrieve()
         f.subscribe()
         f.update()
         self.assertRaises(
             tblock.exceptions.FilterError,
-            f.rename_custom, filter_id=tblock.USER_RULE_PRIORITY
+            f.rename_custom,
+            filter_id=tblock.USER_RULE_PRIORITY,
         )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `tblock-2.6.1/test/test_hosts.py` & `tblock-2.7.1/test/test_hosts.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
```

### Comparing `tblock-2.6.1/test/test_rules.py` & `tblock-2.7.1/test/test_rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
```

### Comparing `tblock-2.6.1/test/test_utils.py` & `tblock-2.7.1/test/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   _____ ____  _            _
 #  |_   _| __ )| | ___   ___| | __
 #    | | |  _ \| |/ _ \ / __| |/ /
 #    | | | |_) | | (_) | (__|   <
 #    |_| |____/|_|\___/ \___|_|\_\
 #
 # An anti-capitalist ad-blocker that uses the hosts file
-# Copyright (C) 2021-2022 Twann <tw4nn@disroot.org>
+# Copyright (C) 2021-2023 Twann <tw4nn@disroot.org>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
```

