# Comparing `tmp/sprit-0.1.2.tar.gz` & `tmp/sprit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprit-0.1.2.tar", last modified: Fri Jul 28 21:52:36 2023, max compression
+gzip compressed data, was "sprit-0.1.3.tar", last modified: Mon Jul 31 16:38:51 2023, max compression
```

## Comparing `sprit-0.1.2.tar` & `sprit-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:36.681313 sprit-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-28 21:52:24.000000 sprit-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-28 21:52:36.681313 sprit-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-28 21:52:24.000000 sprit-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-28 21:52:24.000000 sprit-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 21:52:36.681313 sprit-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-28 21:52:24.000000 sprit-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:36.677313 sprit-0.1.2/sprit/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:36.681313 sprit-0.1.2/sprit/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    44172 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/rs3dv7_metadata.inv
--rw-r--r--   0 runner    (1001) docker     (123)   536638 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/sprit_icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/sprit_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/sprit_icon.xcf
--rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/sprit_icon_alpha.ico
--rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/sprit_icon_thickly.xcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:36.681313 sprit-0.1.2/sprit/resources/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/themes/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/resources/todo.md
--rw-r--r--   0 runner    (1001) docker     (123)   195150 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/sprit.py
--rw-r--r--   0 runner    (1001) docker     (123)   139236 2023-07-28 21:52:24.000000 sprit-0.1.2/sprit/sprit_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 21:52:36.677313 sprit-0.1.2/sprit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-28 21:52:36.000000 sprit-0.1.2/sprit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-28 21:52:36.000000 sprit-0.1.2/sprit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 21:52:36.000000 sprit-0.1.2/sprit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 21:52:36.000000 sprit-0.1.2/sprit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 21:52:36.000000 sprit-0.1.2/sprit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:38:51.176011 sprit-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-31 16:38:34.000000 sprit-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-31 16:38:51.176011 sprit-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-31 16:38:34.000000 sprit-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-31 16:38:34.000000 sprit-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 16:38:51.176011 sprit-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-31 16:38:34.000000 sprit-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:38:51.148011 sprit-0.1.3/sprit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:38:51.152011 sprit-0.1.3/sprit/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    44172 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/rs3dv7_metadata.inv
+-rw-r--r--   0 runner    (1001) docker     (123)   536638 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/sprit_icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/sprit_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/sprit_icon.xcf
+-rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/sprit_icon_alpha.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/sprit_icon_thickly.xcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:38:51.152011 sprit-0.1.3/sprit/resources/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:38:51.164011 sprit-0.1.3/sprit/resources/themes/forest-dark/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/border-accent-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/border-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/border-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/border-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/border-invalid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/card.png
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-tri-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-tri-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-tri-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-unsel-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-unsel-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-unsel-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-unsel-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/combo-button-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/combo-button-focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/combo-button-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/empty.png
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/hor-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/hor-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/hor-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/notebook.png
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/off-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/off-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/off-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/on-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/on-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/on-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-tri-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-tri-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-tri-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-unsel-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-unsel-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-unsel-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-unsel-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/rect-accent-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/rect-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/rect-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/rect-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/scale-hor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/scale-vert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/sizegrip.png
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/spin-button-down-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/spin-button-down-focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/spin-button-up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/tab-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/tab-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/tab-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/thumb-hor-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/thumb-hor-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/thumb-hor-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/thumb-vert-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/thumb-vert-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/thumb-vert-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/tree-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/tree-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/vert-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/vert-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/vert-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:38:51.176011 sprit-0.1.3/sprit/resources/themes/forest-light/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/border-accent-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/border-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/border-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/border-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/border-invalid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/card.png
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-tri-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-tri-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-tri-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-unsel-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-unsel-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-unsel-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-unsel-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/combo-button-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/combo-button-focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/combo-button-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/down-focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/empty.png
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/hor-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/hor-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/hor-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/notebook.png
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/off-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/off-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/off-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/on-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/on-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/on-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-tri-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-tri-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-tri-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-unsel-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-unsel-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-unsel-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-unsel-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/rect-accent-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/rect-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/rect-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/rect-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/right-focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/scale-hor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/scale-vert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/sizegrip.png
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/spin-button-down-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/spin-button-down-focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/spin-button-up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/tab-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/tab-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/tab-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/thumb-hor-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/thumb-hor-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/thumb-hor-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/thumb-vert-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/thumb-vert-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/thumb-vert-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/tree-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/tree-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/vert-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/vert-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/vert-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19157 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/todo.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195150 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/sprit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139243 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/sprit_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:38:51.148011 sprit-0.1.3/sprit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-31 16:38:51.000000 sprit-0.1.3/sprit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-07-31 16:38:51.000000 sprit-0.1.3/sprit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:38:51.000000 sprit-0.1.3/sprit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-31 16:38:51.000000 sprit-0.1.3/sprit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 16:38:51.000000 sprit-0.1.3/sprit.egg-info/top_level.txt
```

### Comparing `sprit-0.1.2/LICENSE` & `sprit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sprit-0.1.2/PKG-INFO` & `sprit-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for processing and analyzing HVSR (Horizontal to Vertical Spectral Ratio) data
 Author: Riley Balikian
 Author-email: balikian@illinois.edu
 License: MIT License
         
         Copyright (c) 2023 RJbalikian
```

### Comparing `sprit-0.1.2/README.md` & `sprit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sprit-0.1.2/pyproject.toml` & `sprit-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprit"
 dynamic = ["readme"]
 license = {file = "LICENSE"}
-version="0.1.2"
+version="0.1.3"
 description = "A package for processing and analyzing HVSR (Horizontal to Vertical Spectral Ratio) data"
 keywords = ["HVSR", "seismic", "horizontal to vertical spectral ratio", "obspy", 'geology', 'geophysics', 'geotechnical']
 requires-python = ">=3.9"
 dependencies =  ["obspy", "scipy", "matplotlib", "pandas", "numpy", "pyqt5", "tkcalendar"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Intended Audience :: Science/Research",
```

### Comparing `sprit-0.1.2/sprit/__init__.py` & `sprit-0.1.3/sprit/__init__.py`

 * *Files identical despite different names*

### Comparing `sprit-0.1.2/sprit/resources/rs3dv7_metadata.inv` & `sprit-0.1.3/sprit/resources/rs3dv7_metadata.inv`

 * *Files identical despite different names*

### Comparing `sprit-0.1.2/sprit/resources/sprit_icon.ico` & `sprit-0.1.3/sprit/resources/sprit_icon.ico`

 * *Files identical despite different names*

### Comparing `sprit-0.1.2/sprit/resources/sprit_icon.png` & `sprit-0.1.3/sprit/resources/sprit_icon.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.2/sprit/resources/sprit_icon.xcf` & `sprit-0.1.3/sprit/resources/sprit_icon.xcf`

 * *Files identical despite different names*

### Comparing `sprit-0.1.2/sprit/resources/sprit_icon_alpha.ico` & `sprit-0.1.3/sprit/resources/sprit_icon_alpha.ico`

 * *Files identical despite different names*

### Comparing `sprit-0.1.2/sprit/resources/sprit_icon_thickly.xcf` & `sprit-0.1.3/sprit/resources/sprit_icon_thickly.xcf`

 * *Files identical despite different names*

### Comparing `sprit-0.1.2/sprit/resources/themes/example.py` & `sprit-0.1.3/sprit/resources/themes/example.py`

 * *Files identical despite different names*

### Comparing `sprit-0.1.2/sprit/sprit.py` & `sprit-0.1.3/sprit/sprit.py`

 * *Files identical despite different names*

### Comparing `sprit-0.1.2/sprit/sprit_gui.py` & `sprit-0.1.3/sprit/sprit_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         # Set the theme
         self.darkthemepath = pathlib.Path(pkg_resources.resource_filename(__name__, "/resources/themes/forest-dark.tcl"))
         self.lightthemepath = pathlib.Path(pkg_resources.resource_filename(__name__, "/resources/themes/forest-light.tcl"))
         
         # Create the style object
         self.style = ttk.Style(master)
-        root.tk.call('source', self.lightthemepath)
+        self.master.tk.call('source', self.lightthemepath)
         #self.style.theme_use('default')
         self.style.theme_use('forest-light')
 
         self.create_menubar()
         self.create_tabs()
 
         self.master.rowconfigure(0, weight=1)
```

### Comparing `sprit-0.1.2/sprit.egg-info/PKG-INFO` & `sprit-0.1.3/sprit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for processing and analyzing HVSR (Horizontal to Vertical Spectral Ratio) data
 Author: Riley Balikian
 Author-email: balikian@illinois.edu
 License: MIT License
         
         Copyright (c) 2023 RJbalikian
```

