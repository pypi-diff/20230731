# Comparing `tmp/sprit-0.1.3.tar.gz` & `tmp/sprit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprit-0.1.3.tar", last modified: Mon Jul 31 16:38:51 2023, max compression
+gzip compressed data, was "sprit-0.1.4.tar", last modified: Mon Jul 31 17:08:38 2023, max compression
```

## Comparing `sprit-0.1.3.tar` & `sprit-0.1.4.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:38:51.176011 sprit-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-31 16:38:34.000000 sprit-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-31 16:38:51.176011 sprit-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-31 16:38:34.000000 sprit-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-31 16:38:34.000000 sprit-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 16:38:51.176011 sprit-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-31 16:38:34.000000 sprit-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:38:51.148011 sprit-0.1.3/sprit/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:38:51.152011 sprit-0.1.3/sprit/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    44172 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/rs3dv7_metadata.inv
--rw-r--r--   0 runner    (1001) docker     (123)   536638 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/sprit_icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/sprit_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/sprit_icon.xcf
--rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/sprit_icon_alpha.ico
--rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/sprit_icon_thickly.xcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:38:51.152011 sprit-0.1.3/sprit/resources/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:38:51.164011 sprit-0.1.3/sprit/resources/themes/forest-dark/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/border-accent-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/border-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/border-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/border-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/border-invalid.png
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/card.png
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-tri-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-tri-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-tri-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-unsel-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-unsel-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-unsel-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/check-unsel-pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/combo-button-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/combo-button-focus.png
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/combo-button-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/down.png
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/empty.png
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/hor-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/hor-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/hor-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/notebook.png
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/off-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/off-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/off-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/on-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/on-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/on-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-tri-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-tri-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-tri-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-unsel-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-unsel-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-unsel-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/radio-unsel-pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/rect-accent-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/rect-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/rect-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/rect-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/right.png
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/scale-hor.png
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/scale-vert.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/sizegrip.png
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/spin-button-down-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/spin-button-down-focus.png
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/spin-button-up.png
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/tab-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/tab-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/tab-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/thumb-hor-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/thumb-hor-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/thumb-hor-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/thumb-vert-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/thumb-vert-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/thumb-vert-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/tree-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/tree-pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/up.png
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/vert-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/vert-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark/vert-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-dark.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:38:51.176011 sprit-0.1.3/sprit/resources/themes/forest-light/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/border-accent-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/border-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/border-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/border-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/border-invalid.png
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/card.png
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-tri-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-tri-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-tri-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-unsel-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-unsel-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-unsel-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/check-unsel-pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/combo-button-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/combo-button-focus.png
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/combo-button-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/down-focus.png
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/down.png
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/empty.png
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/hor-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/hor-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/hor-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/notebook.png
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/off-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/off-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/off-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/on-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/on-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/on-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-tri-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-tri-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-tri-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-unsel-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-unsel-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-unsel-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/radio-unsel-pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/rect-accent-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/rect-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/rect-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/rect-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/right-focus.png
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/right.png
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/scale-hor.png
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/scale-vert.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/sizegrip.png
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/spin-button-down-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/spin-button-down-focus.png
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/spin-button-up.png
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/tab-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/tab-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/tab-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/thumb-hor-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/thumb-hor-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/thumb-hor-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/thumb-vert-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/thumb-vert-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/thumb-vert-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/tree-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/tree-pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/up.png
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/vert-accent.png
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/vert-basic.png
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light/vert-hover.png
--rw-r--r--   0 runner    (1001) docker     (123)    19157 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/themes/forest-light.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/resources/todo.md
--rw-r--r--   0 runner    (1001) docker     (123)   195150 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/sprit.py
--rw-r--r--   0 runner    (1001) docker     (123)   139243 2023-07-31 16:38:34.000000 sprit-0.1.3/sprit/sprit_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:38:51.148011 sprit-0.1.3/sprit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-31 16:38:51.000000 sprit-0.1.3/sprit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-07-31 16:38:51.000000 sprit-0.1.3/sprit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:38:51.000000 sprit-0.1.3/sprit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-31 16:38:51.000000 sprit-0.1.3/sprit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 16:38:51.000000 sprit-0.1.3/sprit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:08:38.143322 sprit-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-31 17:08:19.000000 sprit-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-31 17:08:38.143322 sprit-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-31 17:08:19.000000 sprit-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-31 17:08:19.000000 sprit-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 17:08:38.143322 sprit-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-31 17:08:19.000000 sprit-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:08:38.119321 sprit-0.1.4/sprit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:08:38.123321 sprit-0.1.4/sprit/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    44172 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/rs3dv7_metadata.inv
+-rw-r--r--   0 runner    (1001) docker     (123)   536638 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/sprit_icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/sprit_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/sprit_icon.xcf
+-rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/sprit_icon_alpha.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/sprit_icon_thickly.xcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:08:38.123321 sprit-0.1.4/sprit/resources/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:08:38.135322 sprit-0.1.4/sprit/resources/themes/forest-dark/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/border-accent-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/border-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/border-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/border-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/border-invalid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/card.png
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/check-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/check-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/check-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/check-tri-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/check-tri-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/check-tri-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/check-unsel-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/check-unsel-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/check-unsel-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/check-unsel-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/combo-button-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/combo-button-focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/combo-button-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/empty.png
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/hor-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/hor-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/hor-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/notebook.png
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/off-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/off-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/off-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/on-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/on-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/on-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/radio-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/radio-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/radio-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/radio-tri-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/radio-tri-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/radio-tri-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/radio-unsel-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/radio-unsel-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/radio-unsel-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/radio-unsel-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/rect-accent-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/rect-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/rect-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/rect-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/scale-hor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/scale-vert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/sizegrip.png
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/spin-button-down-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/spin-button-down-focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/spin-button-up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/tab-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/tab-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/tab-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/thumb-hor-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/thumb-hor-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/thumb-hor-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/thumb-vert-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/thumb-vert-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/thumb-vert-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/tree-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/tree-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/vert-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/vert-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark/vert-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-dark.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:08:38.143322 sprit-0.1.4/sprit/resources/themes/forest-light/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/border-accent-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/border-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/border-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/border-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/border-invalid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/card.png
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/check-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/check-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/check-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/check-tri-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/check-tri-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/check-tri-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/check-unsel-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/check-unsel-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/check-unsel-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/check-unsel-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/combo-button-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/combo-button-focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/combo-button-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/down-focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/empty.png
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/hor-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/hor-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/hor-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/notebook.png
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/off-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/off-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/off-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/on-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/on-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/on-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/radio-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/radio-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/radio-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/radio-tri-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/radio-tri-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/radio-tri-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/radio-unsel-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/radio-unsel-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/radio-unsel-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/radio-unsel-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/rect-accent-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/rect-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/rect-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/rect-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/right-focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/scale-hor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/scale-vert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/sizegrip.png
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/spin-button-down-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/spin-button-down-focus.png
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/spin-button-up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/tab-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/tab-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/tab-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/thumb-hor-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/thumb-hor-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/thumb-hor-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/thumb-vert-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/thumb-vert-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/thumb-vert-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/tree-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/tree-pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/vert-accent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/vert-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light/vert-hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19157 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/themes/forest-light.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/resources/todo.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195456 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/sprit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139243 2023-07-31 17:08:19.000000 sprit-0.1.4/sprit/sprit_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:08:38.123321 sprit-0.1.4/sprit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-31 17:08:38.000000 sprit-0.1.4/sprit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-07-31 17:08:38.000000 sprit-0.1.4/sprit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:08:38.000000 sprit-0.1.4/sprit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-31 17:08:38.000000 sprit-0.1.4/sprit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 17:08:38.000000 sprit-0.1.4/sprit.egg-info/top_level.txt
```

### Comparing `sprit-0.1.3/LICENSE` & `sprit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/PKG-INFO` & `sprit-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprit
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for processing and analyzing HVSR (Horizontal to Vertical Spectral Ratio) data
 Author: Riley Balikian
 Author-email: balikian@illinois.edu
 License: MIT License
         
         Copyright (c) 2023 RJbalikian
```

### Comparing `sprit-0.1.3/README.md` & `sprit-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/pyproject.toml` & `sprit-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprit"
 dynamic = ["readme"]
 license = {file = "LICENSE"}
-version="0.1.3"
+version="0.1.4"
 description = "A package for processing and analyzing HVSR (Horizontal to Vertical Spectral Ratio) data"
 keywords = ["HVSR", "seismic", "horizontal to vertical spectral ratio", "obspy", 'geology', 'geophysics', 'geotechnical']
 requires-python = ">=3.9"
 dependencies =  ["obspy", "scipy", "matplotlib", "pandas", "numpy", "pyqt5", "tkcalendar"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Intended Audience :: Science/Research",
```

### Comparing `sprit-0.1.3/sprit/__init__.py` & `sprit-0.1.4/sprit/__init__.py`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/rs3dv7_metadata.inv` & `sprit-0.1.4/sprit/resources/rs3dv7_metadata.inv`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/sprit_icon.ico` & `sprit-0.1.4/sprit/resources/sprit_icon.ico`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/sprit_icon.png` & `sprit-0.1.4/sprit/resources/sprit_icon.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/sprit_icon.xcf` & `sprit-0.1.4/sprit/resources/sprit_icon.xcf`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/sprit_icon_alpha.ico` & `sprit-0.1.4/sprit/resources/sprit_icon_alpha.ico`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/sprit_icon_thickly.xcf` & `sprit-0.1.4/sprit/resources/sprit_icon_thickly.xcf`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/LICENSE` & `sprit-0.1.4/sprit/resources/themes/LICENSE`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/README.md` & `sprit-0.1.4/sprit/resources/themes/README.md`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/example.py` & `sprit-0.1.4/sprit/resources/themes/example.py`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-dark/off-accent.png` & `sprit-0.1.4/sprit/resources/themes/forest-dark/off-accent.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-dark/off-basic.png` & `sprit-0.1.4/sprit/resources/themes/forest-dark/off-basic.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-dark/off-hover.png` & `sprit-0.1.4/sprit/resources/themes/forest-dark/off-hover.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-dark/on-accent.png` & `sprit-0.1.4/sprit/resources/themes/forest-dark/on-accent.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-dark/on-basic.png` & `sprit-0.1.4/sprit/resources/themes/forest-dark/on-basic.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-dark/on-hover.png` & `sprit-0.1.4/sprit/resources/themes/forest-dark/on-hover.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-dark/radio-accent.png` & `sprit-0.1.4/sprit/resources/themes/forest-dark/radio-accent.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-dark/radio-basic.png` & `sprit-0.1.4/sprit/resources/themes/forest-dark/radio-basic.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-dark/radio-hover.png` & `sprit-0.1.4/sprit/resources/themes/forest-dark/radio-hover.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-dark/radio-unsel-accent.png` & `sprit-0.1.4/sprit/resources/themes/forest-dark/radio-unsel-accent.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-dark/radio-unsel-basic.png` & `sprit-0.1.4/sprit/resources/themes/forest-dark/radio-unsel-basic.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-dark/radio-unsel-hover.png` & `sprit-0.1.4/sprit/resources/themes/forest-dark/radio-unsel-hover.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-dark.tcl` & `sprit-0.1.4/sprit/resources/themes/forest-dark.tcl`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light/check-accent.png` & `sprit-0.1.4/sprit/resources/themes/forest-light/check-accent.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light/check-hover.png` & `sprit-0.1.4/sprit/resources/themes/forest-light/check-hover.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light/off-accent.png` & `sprit-0.1.4/sprit/resources/themes/forest-light/off-accent.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light/off-basic.png` & `sprit-0.1.4/sprit/resources/themes/forest-light/off-basic.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light/off-hover.png` & `sprit-0.1.4/sprit/resources/themes/forest-light/off-hover.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light/on-accent.png` & `sprit-0.1.4/sprit/resources/themes/forest-light/on-accent.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light/on-basic.png` & `sprit-0.1.4/sprit/resources/themes/forest-light/on-basic.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light/on-hover.png` & `sprit-0.1.4/sprit/resources/themes/forest-light/on-hover.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light/radio-accent.png` & `sprit-0.1.4/sprit/resources/themes/forest-light/radio-accent.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light/radio-hover.png` & `sprit-0.1.4/sprit/resources/themes/forest-light/radio-hover.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light/radio-tri-accent.png` & `sprit-0.1.4/sprit/resources/themes/forest-light/radio-tri-accent.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light/radio-tri-hover.png` & `sprit-0.1.4/sprit/resources/themes/forest-light/radio-tri-hover.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light/radio-unsel-accent.png` & `sprit-0.1.4/sprit/resources/themes/forest-light/radio-unsel-accent.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light/radio-unsel-hover.png` & `sprit-0.1.4/sprit/resources/themes/forest-light/radio-unsel-hover.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light/radio-unsel-pressed.png` & `sprit-0.1.4/sprit/resources/themes/forest-light/radio-unsel-pressed.png`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/resources/themes/forest-light.tcl` & `sprit-0.1.4/sprit/resources/themes/forest-light.tcl`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit/sprit.py` & `sprit-0.1.4/sprit/sprit.py`

 * *Files 0% similar despite different names*

```diff
@@ -11871,327 +11871,346 @@
 0002e5e0: 650a 2020 2020 2020 2020 2020 2020 2d20  e.            - 
 0002e5f0: 4669 6775 7265 2077 6974 6820 3320 636f  Figure with 3 co
 0002e600: 6d70 6f6e 656e 7473 0a20 2020 2022 2222  mponents.    """
 0002e610: 0a20 2020 2023 7072 696e 7420 7374 6174  .    #print stat
 0002e620: 656d 656e 740a 2020 2020 2343 6865 636b  ement.    #Check
 0002e630: 2069 6620 7265 7375 6c74 7320 6172 6520   if results are 
 0002e640: 676f 6f64 0a20 2020 2023 4375 7276 6520  good.    #Curve 
-0002e650: 7061 7373 3f0a 2020 2020 6375 7276 6550  pass?.    curveP
-0002e660: 6173 7320 3d20 2868 7673 725f 7265 7375  ass = (hvsr_resu
-0002e670: 6c74 735b 2742 6573 7420 5065 616b 275d  lts['Best Peak']
-0002e680: 5b27 5061 7373 204c 6973 7427 5d5b 2757  ['Pass List']['W
-0002e690: 696e 646f 7720 4c65 6e67 7468 2046 7265  indow Length Fre
-0002e6a0: 712e 275d 202b 0a20 2020 2020 2020 2020  q.'] +.         
+0002e650: 7061 7373 3f0a 2020 2020 6375 7276 5465  pass?.    curvTe
+0002e660: 7374 7350 6173 7365 6420 3d20 2868 7673  stsPassed = (hvs
+0002e670: 725f 7265 7375 6c74 735b 2742 6573 7420  r_results['Best 
+0002e680: 5065 616b 275d 5b27 5061 7373 204c 6973  Peak']['Pass Lis
+0002e690: 7427 5d5b 2757 696e 646f 7720 4c65 6e67  t']['Window Leng
+0002e6a0: 7468 2046 7265 712e 275d 202b 0a20 2020  th Freq.'] +.   
 0002e6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e6c0: 6876 7372 5f72 6573 756c 7473 5b27 4265  hvsr_results['Be
-0002e6d0: 7374 2050 6561 6b27 5d5b 2750 6173 7320  st Peak']['Pass 
-0002e6e0: 4c69 7374 275d 5b27 5369 676e 6966 6963  List']['Signific
-0002e6f0: 616e 7420 4379 636c 6573 275d 2b0a 2020  ant Cycles']+.  
-0002e700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e710: 2020 2020 2020 2068 7673 725f 7265 7375         hvsr_resu
-0002e720: 6c74 735b 2742 6573 7420 5065 616b 275d  lts['Best Peak']
-0002e730: 5b27 5061 7373 204c 6973 7427 5d5b 274c  ['Pass List']['L
-0002e740: 6f77 2043 7572 7665 2053 7444 6576 2e20  ow Curve StDev. 
-0002e750: 6f76 6572 2074 696d 6527 5d29 203e 2032  over time']) > 2
-0002e760: 0a20 2020 200a 2020 2020 2350 6561 6b20  .    .    #Peak 
-0002e770: 5061 7373 3f0a 2020 2020 7065 616b 5061  Pass?.    peakPa
-0002e780: 7373 203d 2028 2068 7673 725f 7265 7375  ss = ( hvsr_resu
-0002e790: 6c74 735b 2742 6573 7420 5065 616b 275d  lts['Best Peak']
-0002e7a0: 5b27 5061 7373 204c 6973 7427 5d5b 2750  ['Pass List']['P
-0002e7b0: 6561 6b20 4672 6571 2e20 436c 6172 6974  eak Freq. Clarit
-0002e7c0: 7920 4265 6c6f 7727 5d20 2b0a 2020 2020  y Below'] +.    
-0002e7d0: 2020 2020 2020 2020 2020 2020 6876 7372              hvsr
-0002e7e0: 5f72 6573 756c 7473 5b27 4265 7374 2050  _results['Best P
-0002e7f0: 6561 6b27 5d5b 2750 6173 7320 4c69 7374  eak']['Pass List
-0002e800: 275d 5b27 5065 616b 2046 7265 712e 2043  ']['Peak Freq. C
-0002e810: 6c61 7269 7479 2041 626f 7665 275d 2b0a  larity Above']+.
-0002e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002e830: 6876 7372 5f72 6573 756c 7473 5b27 4265  hvsr_results['Be
-0002e840: 7374 2050 6561 6b27 5d5b 2750 6173 7320  st Peak']['Pass 
-0002e850: 4c69 7374 275d 5b27 5065 616b 2041 6d70  List']['Peak Amp
-0002e860: 2e20 436c 6172 6974 7927 5d2b 0a20 2020  . Clarity']+.   
-0002e870: 2020 2020 2020 2020 2020 2020 2068 7673               hvs
-0002e880: 725f 7265 7375 6c74 735b 2742 6573 7420  r_results['Best 
-0002e890: 5065 616b 275d 5b27 5061 7373 204c 6973  Peak']['Pass Lis
-0002e8a0: 7427 5d5b 2746 7265 712e 2053 7461 6269  t']['Freq. Stabi
-0002e8b0: 6c69 7479 275d 2b0a 2020 2020 2020 2020  lity']+.        
-0002e8c0: 2020 2020 2020 2020 6876 7372 5f72 6573          hvsr_res
-0002e8d0: 756c 7473 5b27 4265 7374 2050 6561 6b27  ults['Best Peak'
-0002e8e0: 5d5b 2750 6173 7320 4c69 7374 275d 5b27  ]['Pass List']['
-0002e8f0: 5065 616b 2053 7461 6269 6c69 7479 2028  Peak Stability (
-0002e900: 6672 6571 2e20 7374 6429 275d 2b0a 2020  freq. std)']+.  
-0002e910: 2020 2020 2020 2020 2020 2020 2020 6876                hv
-0002e920: 7372 5f72 6573 756c 7473 5b27 4265 7374  sr_results['Best
-0002e930: 2050 6561 6b27 5d5b 2750 6173 7320 4c69   Peak']['Pass Li
-0002e940: 7374 275d 5b27 5065 616b 2053 7461 6269  st']['Peak Stabi
-0002e950: 6c69 7479 2028 616d 702e 2073 7464 2927  lity (amp. std)'
-0002e960: 5d29 203e 3d20 350a 2020 2020 2020 2020  ]) >= 5.        
-0002e970: 0a20 2020 200a 2020 2020 6966 2066 6f72  .    .    if for
-0002e980: 6d61 743d 3d27 7072 696e 7427 3a0a 2020  mat=='print':.  
-0002e990: 2020 2020 2020 2350 7269 6e74 2072 6573        #Print res
-0002e9a0: 756c 7473 0a20 2020 2020 2020 2070 7269  ults.        pri
-0002e9b0: 6e74 2827 5369 7465 3a27 2c68 7673 725f  nt('Site:',hvsr_
-0002e9c0: 7265 7375 6c74 735b 2769 6e70 7574 5f70  results['input_p
-0002e9d0: 6172 616d 7327 5d5b 2773 6974 6527 5d29  arams']['site'])
-0002e9e0: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
-0002e9f0: 4163 7175 6973 6974 696f 6e20 4461 7465  Acquisition Date
-0002ea00: 3a27 2c20 6876 7372 5f72 6573 756c 7473  :', hvsr_results
-0002ea10: 5b27 696e 7075 745f 7061 7261 6d73 275d  ['input_params']
-0002ea20: 5b27 6163 715f 6461 7465 275d 290a 2020  ['acq_date']).  
-0002ea30: 2020 2020 2020 7072 696e 7428 2753 6974        print('Sit
-0002ea40: 6520 4c6f 6361 7469 6f6e 3a27 2c20 6876  e Location:', hv
-0002ea50: 7372 5f72 6573 756c 7473 5b27 696e 7075  sr_results['inpu
-0002ea60: 745f 7061 7261 6d73 275d 5b27 6c6f 6e67  t_params']['long
-0002ea70: 6974 7564 6527 5d2c 2068 7673 725f 7265  itude'], hvsr_re
-0002ea80: 7375 6c74 735b 2769 6e70 7574 5f70 6172  sults['input_par
-0002ea90: 616d 7327 5d5b 276c 6174 6974 7564 6527  ams']['latitude'
-0002eaa0: 5d29 0a20 2020 2020 2020 2070 7269 6e74  ]).        print
-0002eab0: 2827 456c 6576 6174 696f 6e3a 272c 6876  ('Elevation:',hv
-0002eac0: 7372 5f72 6573 756c 7473 5b27 696e 7075  sr_results['inpu
-0002ead0: 745f 7061 7261 6d73 275d 5b27 656c 6576  t_params']['elev
-0002eae0: 6174 696f 6e27 5d29 0a20 2020 2020 2020  ation']).       
-0002eaf0: 2070 7269 6e74 2829 0a20 2020 2020 2020   print().       
-0002eb00: 2070 7269 6e74 2827 7b30 3a2e 3366 7d20   print('{0:.3f} 
-0002eb10: 487a 2050 6561 6b20 4672 6571 7565 6e63  Hz Peak Frequenc
-0002eb20: 7927 2e66 6f72 6d61 7428 6876 7372 5f72  y'.format(hvsr_r
-0002eb30: 6573 756c 7473 5b27 4265 7374 2050 6561  esults['Best Pea
-0002eb40: 6b27 5d5b 2766 3027 5d29 2920 2020 2020  k']['f0']))     
-0002eb50: 2020 200a 2020 2020 2020 2020 6966 2063     .        if c
-0002eb60: 7572 7665 5061 7373 2061 6e64 2070 6561  urvePass and pea
-0002eb70: 6b50 6173 733a 0a20 2020 2020 2020 2020  kPass:.         
-0002eb80: 2020 2070 7269 6e74 2827 e29c 9420 4375     print('... Cu
-0002eb90: 7276 6520 6174 207b 303a 2e33 667d 2048  rve at {0:.3f} H
-0002eba0: 7a20 7061 7373 6564 2071 7561 6c69 7479  z passed quality
-0002ebb0: 2063 6865 636b 7321 203a 4427 2e66 6f72   checks! :D'.for
-0002ebc0: 6d61 7428 6876 7372 5f72 6573 756c 7473  mat(hvsr_results
-0002ebd0: 5b27 4265 7374 2050 6561 6b27 5d5b 2766  ['Best Peak']['f
-0002ebe0: 3027 5d29 290a 2020 2020 2020 2020 656c  0'])).        el
-0002ebf0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0002ec00: 7072 696e 7428 27e2 9c98 2050 6561 6b20  print('... Peak 
-0002ec10: 6174 207b 303a 2e33 667d 2048 7a20 6469  at {0:.3f} Hz di
-0002ec20: 6420 4e4f 5420 7061 7373 2071 7561 6c69  d NOT pass quali
-0002ec30: 7479 2063 6865 636b 7320 3a28 272e 666f  ty checks :('.fo
-0002ec40: 726d 6174 2868 7673 725f 7265 7375 6c74  rmat(hvsr_result
-0002ec50: 735b 2742 6573 7420 5065 616b 275d 5b27  s['Best Peak']['
-0002ec60: 6630 275d 2929 2020 2020 2020 2020 2020  f0']))          
-0002ec70: 2020 0a0a 2020 2020 2020 2020 2350 7269    ..        #Pri
-0002ec80: 6e74 2069 6e64 6976 6964 7561 6c20 7265  nt individual re
-0002ec90: 7375 6c74 730a 2020 2020 2020 2020 7072  sults.        pr
-0002eca0: 696e 7428 275c 7443 7572 7665 2054 6573  int('\tCurve Tes
-0002ecb0: 7473 3a27 290a 2020 2020 2020 2020 7072  ts:').        pr
-0002ecc0: 696e 7428 275c 745c 7427 2c20 6876 7372  int('\t\t', hvsr
-0002ecd0: 5f72 6573 756c 7473 5b27 4265 7374 2050  _results['Best P
-0002ece0: 6561 6b27 5d5b 2752 6570 6f72 7427 5d5b  eak']['Report'][
-0002ecf0: 274c 7727 5d5b 2d31 5d2c 2027 4c65 6e67  'Lw'][-1], 'Leng
-0002ed00: 7468 206f 6620 7072 6f63 6573 7369 6e67  th of processing
-0002ed10: 2077 696e 646f 7773 3a27 2c20 6876 7372   windows:', hvsr
-0002ed20: 5f72 6573 756c 7473 5b27 4265 7374 2050  _results['Best P
-0002ed30: 6561 6b27 5d5b 2752 6570 6f72 7427 5d5b  eak']['Report'][
-0002ed40: 274c 7727 5d29 0a20 2020 2020 2020 2070  'Lw']).        p
-0002ed50: 7269 6e74 2827 5c74 5c74 272c 2068 7673  rint('\t\t', hvs
-0002ed60: 725f 7265 7375 6c74 735b 2742 6573 7420  r_results['Best 
-0002ed70: 5065 616b 275d 5b27 5265 706f 7274 275d  Peak']['Report']
-0002ed80: 5b27 4e63 275d 5b2d 315d 2c20 274e 756d  ['Nc'][-1], 'Num
-0002ed90: 6265 7220 6f66 2073 6967 6e69 6669 6361  ber of significa
-0002eda0: 6e74 2063 7963 6c65 733a 272c 2068 7673  nt cycles:', hvs
-0002edb0: 725f 7265 7375 6c74 735b 2742 6573 7420  r_results['Best 
-0002edc0: 5065 616b 275d 5b27 5265 706f 7274 275d  Peak']['Report']
-0002edd0: 5b27 4e63 275d 290a 2020 2020 2020 2020  ['Nc']).        
-0002ede0: 7072 696e 7428 275c 745c 7427 2c20 6876  print('\t\t', hv
-0002edf0: 7372 5f72 6573 756c 7473 5b27 4265 7374  sr_results['Best
-0002ee00: 2050 6561 6b27 5d5b 2752 6570 6f72 7427   Peak']['Report'
-0002ee10: 5d5b 27cf 835f 4128 6629 275d 5b2d 315d  ]['.._A(f)'][-1]
-0002ee20: 2c20 274c 6f77 2053 7444 6576 2e20 6f66  , 'Low StDev. of
-0002ee30: 2048 2f56 2043 7572 7665 206f 7665 7220   H/V Curve over 
-0002ee40: 7469 6d65 3a27 2c20 6876 7372 5f72 6573  time:', hvsr_res
-0002ee50: 756c 7473 5b27 4265 7374 2050 6561 6b27  ults['Best Peak'
-0002ee60: 5d5b 2752 6570 6f72 7427 5d5b 27cf 835f  ]['Report']['.._
-0002ee70: 4128 6629 275d 290a 0a0a 2020 2020 2020  A(f)'])...      
-0002ee80: 2020 7072 696e 7428 275c 7450 6561 6b20    print('\tPeak 
-0002ee90: 5465 7374 733a 2729 0a20 2020 2020 2020  Tests:').       
-0002eea0: 2070 7269 6e74 2827 5c74 5c74 272c 2068   print('\t\t', h
-0002eeb0: 7673 725f 7265 7375 6c74 735b 2742 6573  vsr_results['Bes
-0002eec0: 7420 5065 616b 275d 5b27 5265 706f 7274  t Peak']['Report
-0002eed0: 275d 5b27 4128 662d 2927 5d5b 2d31 5d2c  ']['A(f-)'][-1],
-0002eee0: 2027 436c 6172 6974 7920 4265 6c6f 7720   'Clarity Below 
-0002eef0: 5065 616b 2046 7265 7175 656e 6379 3a27  Peak Frequency:'
-0002ef00: 2c20 6876 7372 5f72 6573 756c 7473 5b27  , hvsr_results['
-0002ef10: 4265 7374 2050 6561 6b27 5d5b 2752 6570  Best Peak']['Rep
-0002ef20: 6f72 7427 5d5b 2741 2866 2d29 275d 290a  ort']['A(f-)']).
-0002ef30: 2020 2020 2020 2020 7072 696e 7428 275c          print('\
-0002ef40: 745c 7427 2c20 6876 7372 5f72 6573 756c  t\t', hvsr_resul
-0002ef50: 7473 5b27 4265 7374 2050 6561 6b27 5d5b  ts['Best Peak'][
-0002ef60: 2752 6570 6f72 7427 5d5b 2741 2866 2b29  'Report']['A(f+)
-0002ef70: 275d 5b2d 315d 2c20 2743 6c61 7269 7479  '][-1], 'Clarity
-0002ef80: 2041 626f 7665 2050 6561 6b20 4672 6571   Above Peak Freq
-0002ef90: 7565 6e63 793a 272c 6876 7372 5f72 6573  uency:',hvsr_res
-0002efa0: 756c 7473 5b27 4265 7374 2050 6561 6b27  ults['Best Peak'
-0002efb0: 5d5b 2752 6570 6f72 7427 5d5b 2741 2866  ]['Report']['A(f
-0002efc0: 2b29 275d 290a 2020 2020 2020 2020 7072  +)']).        pr
-0002efd0: 696e 7428 275c 745c 7427 2c20 6876 7372  int('\t\t', hvsr
-0002efe0: 5f72 6573 756c 7473 5b27 4265 7374 2050  _results['Best P
-0002eff0: 6561 6b27 5d5b 2752 6570 6f72 7427 5d5b  eak']['Report'][
-0002f000: 2741 3027 5d5b 2d31 5d2c 2027 436c 6172  'A0'][-1], 'Clar
-0002f010: 6974 7920 6f66 2050 6561 6b20 416d 706c  ity of Peak Ampl
-0002f020: 6974 7564 653a 272c 6876 7372 5f72 6573  itude:',hvsr_res
-0002f030: 756c 7473 5b27 4265 7374 2050 6561 6b27  ults['Best Peak'
-0002f040: 5d5b 2752 6570 6f72 7427 5d5b 2741 3027  ]['Report']['A0'
-0002f050: 5d29 0a20 2020 2020 2020 2069 6620 6876  ]).        if hv
-0002f060: 7372 5f72 6573 756c 7473 5b27 4265 7374  sr_results['Best
-0002f070: 2050 6561 6b27 5d5b 2750 6173 7320 4c69   Peak']['Pass Li
-0002f080: 7374 275d 5b27 4672 6571 2e20 5374 6162  st']['Freq. Stab
-0002f090: 696c 6974 7927 5d3a 0a20 2020 2020 2020  ility']:.       
-0002f0a0: 2020 2020 2072 6573 203d 2027 e29c 9427       res = '...'
-0002f0b0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0002f0c0: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-0002f0d0: 2027 e29c 9827 0a20 2020 2020 2020 2070   '...'.        p
-0002f0e0: 7269 6e74 2827 5c74 5c74 272c 2072 6573  rint('\t\t', res
-0002f0f0: 2c20 2753 7461 6269 6c69 7479 206f 6620  , 'Stability of 
-0002f100: 5065 616b 2046 7265 712e 204f 7665 7220  Peak Freq. Over 
-0002f110: 7469 6d65 3a27 2c20 6876 7372 5f72 6573  time:', hvsr_res
-0002f120: 756c 7473 5b27 4265 7374 2050 6561 6b27  ults['Best Peak'
-0002f130: 5d5b 2752 6570 6f72 7427 5d5b 2750 2d27  ]['Report']['P-'
-0002f140: 5d5b 3a35 5d20 2b20 2720 616e 6420 2720  ][:5] + ' and ' 
-0002f150: 2b20 6876 7372 5f72 6573 756c 7473 5b27  + hvsr_results['
-0002f160: 4265 7374 2050 6561 6b27 5d5b 2752 6570  Best Peak']['Rep
-0002f170: 6f72 7427 5d5b 2750 2b27 5d5b 3a2d 315d  ort']['P+'][:-1]
-0002f180: 2c20 7265 7329 0a20 2020 2020 2020 2070  , res).        p
-0002f190: 7269 6e74 2827 5c74 5c74 272c 2068 7673  rint('\t\t', hvs
-0002f1a0: 725f 7265 7375 6c74 735b 2742 6573 7420  r_results['Best 
-0002f1b0: 5065 616b 275d 5b27 5265 706f 7274 275d  Peak']['Report']
-0002f1c0: 5b27 5366 275d 5b2d 315d 2c20 2753 7461  ['Sf'][-1], 'Sta
-0002f1d0: 6269 6c69 7479 206f 6620 5065 616b 2028  bility of Peak (
-0002f1e0: 4672 6571 2e20 5374 4465 7629 3a27 2c20  Freq. StDev):', 
-0002f1f0: 6876 7372 5f72 6573 756c 7473 5b27 4265  hvsr_results['Be
-0002f200: 7374 2050 6561 6b27 5d5b 2752 6570 6f72  st Peak']['Repor
-0002f210: 7427 5d5b 2753 6627 5d29 0a20 2020 2020  t']['Sf']).     
+0002e6c0: 2020 2020 2020 6876 7372 5f72 6573 756c        hvsr_resul
+0002e6d0: 7473 5b27 4265 7374 2050 6561 6b27 5d5b  ts['Best Peak'][
+0002e6e0: 2750 6173 7320 4c69 7374 275d 5b27 5369  'Pass List']['Si
+0002e6f0: 676e 6966 6963 616e 7420 4379 636c 6573  gnificant Cycles
+0002e700: 275d 2b0a 2020 2020 2020 2020 2020 2020  ']+.            
+0002e710: 2020 2020 2020 2020 2020 2020 2068 7673               hvs
+0002e720: 725f 7265 7375 6c74 735b 2742 6573 7420  r_results['Best 
+0002e730: 5065 616b 275d 5b27 5061 7373 204c 6973  Peak']['Pass Lis
+0002e740: 7427 5d5b 274c 6f77 2043 7572 7665 2053  t']['Low Curve S
+0002e750: 7444 6576 2e20 6f76 6572 2074 696d 6527  tDev. over time'
+0002e760: 5d29 0a20 2020 2063 7572 7665 5061 7373  ]).    curvePass
+0002e770: 203d 2063 7572 7654 6573 7473 5061 7373   = curvTestsPass
+0002e780: 6564 203e 2032 0a20 2020 200a 2020 2020  ed > 2.    .    
+0002e790: 2350 6561 6b20 5061 7373 3f0a 2020 2020  #Peak Pass?.    
+0002e7a0: 7065 616b 5465 7374 7350 6173 7365 6420  peakTestsPassed 
+0002e7b0: 3d20 2820 6876 7372 5f72 6573 756c 7473  = ( hvsr_results
+0002e7c0: 5b27 4265 7374 2050 6561 6b27 5d5b 2750  ['Best Peak']['P
+0002e7d0: 6173 7320 4c69 7374 275d 5b27 5065 616b  ass List']['Peak
+0002e7e0: 2046 7265 712e 2043 6c61 7269 7479 2042   Freq. Clarity B
+0002e7f0: 656c 6f77 275d 202b 0a20 2020 2020 2020  elow'] +.       
+0002e800: 2020 2020 2020 2020 2068 7673 725f 7265           hvsr_re
+0002e810: 7375 6c74 735b 2742 6573 7420 5065 616b  sults['Best Peak
+0002e820: 275d 5b27 5061 7373 204c 6973 7427 5d5b  ']['Pass List'][
+0002e830: 2750 6561 6b20 4672 6571 2e20 436c 6172  'Peak Freq. Clar
+0002e840: 6974 7920 4162 6f76 6527 5d2b 0a20 2020  ity Above']+.   
+0002e850: 2020 2020 2020 2020 2020 2020 2068 7673               hvs
+0002e860: 725f 7265 7375 6c74 735b 2742 6573 7420  r_results['Best 
+0002e870: 5065 616b 275d 5b27 5061 7373 204c 6973  Peak']['Pass Lis
+0002e880: 7427 5d5b 2750 6561 6b20 416d 702e 2043  t']['Peak Amp. C
+0002e890: 6c61 7269 7479 275d 2b0a 2020 2020 2020  larity']+.      
+0002e8a0: 2020 2020 2020 2020 2020 6876 7372 5f72            hvsr_r
+0002e8b0: 6573 756c 7473 5b27 4265 7374 2050 6561  esults['Best Pea
+0002e8c0: 6b27 5d5b 2750 6173 7320 4c69 7374 275d  k']['Pass List']
+0002e8d0: 5b27 4672 6571 2e20 5374 6162 696c 6974  ['Freq. Stabilit
+0002e8e0: 7927 5d2b 0a20 2020 2020 2020 2020 2020  y']+.           
+0002e8f0: 2020 2020 2068 7673 725f 7265 7375 6c74       hvsr_result
+0002e900: 735b 2742 6573 7420 5065 616b 275d 5b27  s['Best Peak']['
+0002e910: 5061 7373 204c 6973 7427 5d5b 2750 6561  Pass List']['Pea
+0002e920: 6b20 5374 6162 696c 6974 7920 2866 7265  k Stability (fre
+0002e930: 712e 2073 7464 2927 5d2b 0a20 2020 2020  q. std)']+.     
+0002e940: 2020 2020 2020 2020 2020 2068 7673 725f             hvsr_
+0002e950: 7265 7375 6c74 735b 2742 6573 7420 5065  results['Best Pe
+0002e960: 616b 275d 5b27 5061 7373 204c 6973 7427  ak']['Pass List'
+0002e970: 5d5b 2750 6561 6b20 5374 6162 696c 6974  ]['Peak Stabilit
+0002e980: 7920 2861 6d70 2e20 7374 6429 275d 290a  y (amp. std)']).
+0002e990: 2020 2020 7065 616b 5061 7373 203d 2070      peakPass = p
+0002e9a0: 6561 6b54 6573 7473 5061 7373 6564 203e  eakTestsPassed >
+0002e9b0: 3d20 350a 2020 2020 2020 2020 0a20 2020  = 5.        .   
+0002e9c0: 200a 2020 2020 6966 2066 6f72 6d61 743d   .    if format=
+0002e9d0: 3d27 7072 696e 7427 3a0a 2020 2020 2020  ='print':.      
+0002e9e0: 2020 2350 7269 6e74 2072 6573 756c 7473    #Print results
+0002e9f0: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
+0002ea00: 5369 7465 3a27 2c68 7673 725f 7265 7375  Site:',hvsr_resu
+0002ea10: 6c74 735b 2769 6e70 7574 5f70 6172 616d  lts['input_param
+0002ea20: 7327 5d5b 2773 6974 6527 5d29 0a20 2020  s']['site']).   
+0002ea30: 2020 2020 2070 7269 6e74 2827 4163 7175       print('Acqu
+0002ea40: 6973 6974 696f 6e20 4461 7465 3a27 2c20  isition Date:', 
+0002ea50: 6876 7372 5f72 6573 756c 7473 5b27 696e  hvsr_results['in
+0002ea60: 7075 745f 7061 7261 6d73 275d 5b27 6163  put_params']['ac
+0002ea70: 715f 6461 7465 275d 290a 2020 2020 2020  q_date']).      
+0002ea80: 2020 7072 696e 7428 2753 6974 6520 4c6f    print('Site Lo
+0002ea90: 6361 7469 6f6e 3a27 2c20 6876 7372 5f72  cation:', hvsr_r
+0002eaa0: 6573 756c 7473 5b27 696e 7075 745f 7061  esults['input_pa
+0002eab0: 7261 6d73 275d 5b27 6c6f 6e67 6974 7564  rams']['longitud
+0002eac0: 6527 5d2c 2068 7673 725f 7265 7375 6c74  e'], hvsr_result
+0002ead0: 735b 2769 6e70 7574 5f70 6172 616d 7327  s['input_params'
+0002eae0: 5d5b 276c 6174 6974 7564 6527 5d29 0a20  ]['latitude']). 
+0002eaf0: 2020 2020 2020 2070 7269 6e74 2827 456c         print('El
+0002eb00: 6576 6174 696f 6e3a 272c 6876 7372 5f72  evation:',hvsr_r
+0002eb10: 6573 756c 7473 5b27 696e 7075 745f 7061  esults['input_pa
+0002eb20: 7261 6d73 275d 5b27 656c 6576 6174 696f  rams']['elevatio
+0002eb30: 6e27 5d29 0a20 2020 2020 2020 2070 7269  n']).        pri
+0002eb40: 6e74 2829 0a20 2020 2020 2020 2070 7269  nt().        pri
+0002eb50: 6e74 2827 7b30 3a2e 3366 7d20 487a 2050  nt('{0:.3f} Hz P
+0002eb60: 6561 6b20 4672 6571 7565 6e63 7927 2e66  eak Frequency'.f
+0002eb70: 6f72 6d61 7428 6876 7372 5f72 6573 756c  ormat(hvsr_resul
+0002eb80: 7473 5b27 4265 7374 2050 6561 6b27 5d5b  ts['Best Peak'][
+0002eb90: 2766 3027 5d29 2920 2020 2020 2020 200a  'f0']))        .
+0002eba0: 2020 2020 2020 2020 6966 2063 7572 7665          if curve
+0002ebb0: 5061 7373 2061 6e64 2070 6561 6b50 6173  Pass and peakPas
+0002ebc0: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
+0002ebd0: 7269 6e74 2827 e29c 9420 4375 7276 6520  rint('... Curve 
+0002ebe0: 6174 207b 303a 2e33 667d 2048 7a20 7061  at {0:.3f} Hz pa
+0002ebf0: 7373 6564 2071 7561 6c69 7479 2063 6865  ssed quality che
+0002ec00: 636b 7321 203a 4427 2e66 6f72 6d61 7428  cks! :D'.format(
+0002ec10: 6876 7372 5f72 6573 756c 7473 5b27 4265  hvsr_results['Be
+0002ec20: 7374 2050 6561 6b27 5d5b 2766 3027 5d29  st Peak']['f0'])
+0002ec30: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0002ec40: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0002ec50: 7428 27e2 9c98 2050 6561 6b20 6174 207b  t('... Peak at {
+0002ec60: 303a 2e33 667d 2048 7a20 6469 6420 4e4f  0:.3f} Hz did NO
+0002ec70: 5420 7061 7373 2071 7561 6c69 7479 2063  T pass quality c
+0002ec80: 6865 636b 7320 3a28 272e 666f 726d 6174  hecks :('.format
+0002ec90: 2868 7673 725f 7265 7375 6c74 735b 2742  (hvsr_results['B
+0002eca0: 6573 7420 5065 616b 275d 5b27 6630 275d  est Peak']['f0']
+0002ecb0: 2929 2020 2020 2020 2020 2020 2020 0a0a  ))            ..
+0002ecc0: 2020 2020 2020 2020 2350 7269 6e74 2069          #Print i
+0002ecd0: 6e64 6976 6964 7561 6c20 7265 7375 6c74  ndividual result
+0002ece0: 730a 2020 2020 2020 2020 7072 696e 7428  s.        print(
+0002ecf0: 275c 7443 7572 7665 2054 6573 7473 3a20  '\tCurve Tests: 
+0002ed00: 7b7d 2f33 2070 6173 7365 6427 2e66 6f72  {}/3 passed'.for
+0002ed10: 6d61 7428 6375 7276 5465 7374 7350 6173  mat(curvTestsPas
+0002ed20: 7365 6429 290a 2020 2020 2020 2020 7072  sed)).        pr
+0002ed30: 696e 7428 275c 745c 7427 2c20 6876 7372  int('\t\t', hvsr
+0002ed40: 5f72 6573 756c 7473 5b27 4265 7374 2050  _results['Best P
+0002ed50: 6561 6b27 5d5b 2752 6570 6f72 7427 5d5b  eak']['Report'][
+0002ed60: 274c 7727 5d5b 2d31 5d2c 2027 4c65 6e67  'Lw'][-1], 'Leng
+0002ed70: 7468 206f 6620 7072 6f63 6573 7369 6e67  th of processing
+0002ed80: 2077 696e 646f 7773 3a27 2c20 6876 7372   windows:', hvsr
+0002ed90: 5f72 6573 756c 7473 5b27 4265 7374 2050  _results['Best P
+0002eda0: 6561 6b27 5d5b 2752 6570 6f72 7427 5d5b  eak']['Report'][
+0002edb0: 274c 7727 5d29 0a20 2020 2020 2020 2070  'Lw']).        p
+0002edc0: 7269 6e74 2827 5c74 5c74 272c 2068 7673  rint('\t\t', hvs
+0002edd0: 725f 7265 7375 6c74 735b 2742 6573 7420  r_results['Best 
+0002ede0: 5065 616b 275d 5b27 5265 706f 7274 275d  Peak']['Report']
+0002edf0: 5b27 4e63 275d 5b2d 315d 2c20 274e 756d  ['Nc'][-1], 'Num
+0002ee00: 6265 7220 6f66 2073 6967 6e69 6669 6361  ber of significa
+0002ee10: 6e74 2063 7963 6c65 733a 272c 2068 7673  nt cycles:', hvs
+0002ee20: 725f 7265 7375 6c74 735b 2742 6573 7420  r_results['Best 
+0002ee30: 5065 616b 275d 5b27 5265 706f 7274 275d  Peak']['Report']
+0002ee40: 5b27 4e63 275d 290a 2020 2020 2020 2020  ['Nc']).        
+0002ee50: 7072 696e 7428 275c 745c 7427 2c20 6876  print('\t\t', hv
+0002ee60: 7372 5f72 6573 756c 7473 5b27 4265 7374  sr_results['Best
+0002ee70: 2050 6561 6b27 5d5b 2752 6570 6f72 7427   Peak']['Report'
+0002ee80: 5d5b 27cf 835f 4128 6629 275d 5b2d 315d  ]['.._A(f)'][-1]
+0002ee90: 2c20 274c 6f77 2053 7444 6576 2e20 6f66  , 'Low StDev. of
+0002eea0: 2048 2f56 2043 7572 7665 206f 7665 7220   H/V Curve over 
+0002eeb0: 7469 6d65 3a27 2c20 6876 7372 5f72 6573  time:', hvsr_res
+0002eec0: 756c 7473 5b27 4265 7374 2050 6561 6b27  ults['Best Peak'
+0002eed0: 5d5b 2752 6570 6f72 7427 5d5b 27cf 835f  ]['Report']['.._
+0002eee0: 4128 6629 275d 290a 0a0a 2020 2020 2020  A(f)'])...      
+0002eef0: 2020 7072 696e 7428 275c 7450 6561 6b20    print('\tPeak 
+0002ef00: 5465 7374 733a 207b 7d2f 3620 7061 7373  Tests: {}/6 pass
+0002ef10: 6564 272e 666f 726d 6174 2870 6561 6b54  ed'.format(peakT
+0002ef20: 6573 7473 5061 7373 6564 2929 0a20 2020  estsPassed)).   
+0002ef30: 2020 2020 2070 7269 6e74 2827 5c74 5c74       print('\t\t
+0002ef40: 272c 2068 7673 725f 7265 7375 6c74 735b  ', hvsr_results[
+0002ef50: 2742 6573 7420 5065 616b 275d 5b27 5265  'Best Peak']['Re
+0002ef60: 706f 7274 275d 5b27 4128 662d 2927 5d5b  port']['A(f-)'][
+0002ef70: 2d31 5d2c 2027 436c 6172 6974 7920 4265  -1], 'Clarity Be
+0002ef80: 6c6f 7720 5065 616b 2046 7265 7175 656e  low Peak Frequen
+0002ef90: 6379 3a27 2c20 6876 7372 5f72 6573 756c  cy:', hvsr_resul
+0002efa0: 7473 5b27 4265 7374 2050 6561 6b27 5d5b  ts['Best Peak'][
+0002efb0: 2752 6570 6f72 7427 5d5b 2741 2866 2d29  'Report']['A(f-)
+0002efc0: 275d 290a 2020 2020 2020 2020 7072 696e  ']).        prin
+0002efd0: 7428 275c 745c 7427 2c20 6876 7372 5f72  t('\t\t', hvsr_r
+0002efe0: 6573 756c 7473 5b27 4265 7374 2050 6561  esults['Best Pea
+0002eff0: 6b27 5d5b 2752 6570 6f72 7427 5d5b 2741  k']['Report']['A
+0002f000: 2866 2b29 275d 5b2d 315d 2c20 2743 6c61  (f+)'][-1], 'Cla
+0002f010: 7269 7479 2041 626f 7665 2050 6561 6b20  rity Above Peak 
+0002f020: 4672 6571 7565 6e63 793a 272c 6876 7372  Frequency:',hvsr
+0002f030: 5f72 6573 756c 7473 5b27 4265 7374 2050  _results['Best P
+0002f040: 6561 6b27 5d5b 2752 6570 6f72 7427 5d5b  eak']['Report'][
+0002f050: 2741 2866 2b29 275d 290a 2020 2020 2020  'A(f+)']).      
+0002f060: 2020 7072 696e 7428 275c 745c 7427 2c20    print('\t\t', 
+0002f070: 6876 7372 5f72 6573 756c 7473 5b27 4265  hvsr_results['Be
+0002f080: 7374 2050 6561 6b27 5d5b 2752 6570 6f72  st Peak']['Repor
+0002f090: 7427 5d5b 2741 3027 5d5b 2d31 5d2c 2027  t']['A0'][-1], '
+0002f0a0: 436c 6172 6974 7920 6f66 2050 6561 6b20  Clarity of Peak 
+0002f0b0: 416d 706c 6974 7564 653a 272c 6876 7372  Amplitude:',hvsr
+0002f0c0: 5f72 6573 756c 7473 5b27 4265 7374 2050  _results['Best P
+0002f0d0: 6561 6b27 5d5b 2752 6570 6f72 7427 5d5b  eak']['Report'][
+0002f0e0: 2741 3027 5d29 0a20 2020 2020 2020 2069  'A0']).        i
+0002f0f0: 6620 6876 7372 5f72 6573 756c 7473 5b27  f hvsr_results['
+0002f100: 4265 7374 2050 6561 6b27 5d5b 2750 6173  Best Peak']['Pas
+0002f110: 7320 4c69 7374 275d 5b27 4672 6571 2e20  s List']['Freq. 
+0002f120: 5374 6162 696c 6974 7927 5d3a 0a20 2020  Stability']:.   
+0002f130: 2020 2020 2020 2020 2072 6573 203d 2027           res = '
+0002f140: e29c 9427 0a20 2020 2020 2020 2065 6c73  ...'.        els
+0002f150: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002f160: 6573 203d 2027 e29c 9827 0a20 2020 2020  es = '...'.     
+0002f170: 2020 2070 7269 6e74 2827 5c74 5c74 272c     print('\t\t',
+0002f180: 2072 6573 2c20 2753 7461 6269 6c69 7479   res, 'Stability
+0002f190: 206f 6620 5065 616b 2046 7265 712e 204f   of Peak Freq. O
+0002f1a0: 7665 7220 7469 6d65 3a27 2c20 6876 7372  ver time:', hvsr
+0002f1b0: 5f72 6573 756c 7473 5b27 4265 7374 2050  _results['Best P
+0002f1c0: 6561 6b27 5d5b 2752 6570 6f72 7427 5d5b  eak']['Report'][
+0002f1d0: 2750 2d27 5d5b 3a35 5d20 2b20 2720 616e  'P-'][:5] + ' an
+0002f1e0: 6420 2720 2b20 6876 7372 5f72 6573 756c  d ' + hvsr_resul
+0002f1f0: 7473 5b27 4265 7374 2050 6561 6b27 5d5b  ts['Best Peak'][
+0002f200: 2752 6570 6f72 7427 5d5b 2750 2b27 5d5b  'Report']['P+'][
+0002f210: 3a2d 315d 2c20 7265 7329 0a20 2020 2020  :-1], res).     
 0002f220: 2020 2070 7269 6e74 2827 5c74 5c74 272c     print('\t\t',
 0002f230: 2068 7673 725f 7265 7375 6c74 735b 2742   hvsr_results['B
 0002f240: 6573 7420 5065 616b 275d 5b27 5265 706f  est Peak']['Repo
-0002f250: 7274 275d 5b27 5361 275d 5b2d 315d 2c20  rt']['Sa'][-1], 
+0002f250: 7274 275d 5b27 5366 275d 5b2d 315d 2c20  rt']['Sf'][-1], 
 0002f260: 2753 7461 6269 6c69 7479 206f 6620 5065  'Stability of Pe
-0002f270: 616b 2028 416d 702e 2053 7444 6576 293a  ak (Amp. StDev):
-0002f280: 272c 2068 7673 725f 7265 7375 6c74 735b  ', hvsr_results[
-0002f290: 2742 6573 7420 5065 616b 275d 5b27 5265  'Best Peak']['Re
-0002f2a0: 706f 7274 275d 5b27 5361 275d 290a 0a20  port']['Sa']).. 
-0002f2b0: 2020 2065 6c69 6620 666f 726d 6174 3d3d     elif format==
-0002f2c0: 2763 7376 273a 0a20 2020 2020 2020 2069  'csv':.        i
-0002f2d0: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
-0002f2e0: 7064 0a20 2020 2020 2020 2070 6443 6f6c  pd.        pdCol
-0002f2f0: 7320 3d20 5b27 5369 7465 204e 616d 6527  s = ['Site Name'
-0002f300: 2c20 2741 6371 7573 6974 696f 6e20 4461  , 'Acqusition Da
-0002f310: 7465 272c 2027 4c6f 6e67 6974 7564 6527  te', 'Longitude'
-0002f320: 2c20 274c 6174 6974 6964 6527 2c20 2745  , 'Latitide', 'E
-0002f330: 6c65 7661 7469 6f6e 272c 2027 5065 616b  levation', 'Peak
-0002f340: 2046 7265 7175 656e 6379 272c 200a 2020   Frequency', .  
-0002f350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002f360: 2757 696e 646f 7720 4c65 6e67 7468 2046  'Window Length F
-0002f370: 7265 712e 272c 2753 6967 6e69 6669 6361  req.','Significa
-0002f380: 6e74 2043 7963 6c65 7327 2c27 4c6f 7720  nt Cycles','Low 
-0002f390: 4375 7276 6520 5374 4465 762e 206f 7665  Curve StDev. ove
-0002f3a0: 7220 7469 6d65 272c 0a20 2020 2020 2020  r time',.       
-0002f3b0: 2020 2020 2020 2020 2020 2027 5065 616b             'Peak
-0002f3c0: 2046 7265 712e 2043 6c61 7269 7479 2042   Freq. Clarity B
-0002f3d0: 656c 6f77 272c 2750 6561 6b20 4672 6571  elow','Peak Freq
-0002f3e0: 2e20 436c 6172 6974 7920 4162 6f76 6527  . Clarity Above'
-0002f3f0: 2c27 5065 616b 2041 6d70 2e20 436c 6172  ,'Peak Amp. Clar
-0002f400: 6974 7927 2c27 4672 6571 2e20 5374 6162  ity','Freq. Stab
-0002f410: 696c 6974 7927 2c20 2750 6561 6b20 5374  ility', 'Peak St
-0002f420: 6162 696c 6974 7920 2866 7265 712e 2073  ability (freq. s
-0002f430: 7464 2927 2c27 5065 616b 2053 7461 6269  td)','Peak Stabi
-0002f440: 6c69 7479 2028 616d 702e 2073 7464 2927  lity (amp. std)'
-0002f450: 2c20 2750 6561 6b20 5061 7373 6573 275d  , 'Peak Passes']
-0002f460: 0a20 2020 2020 2020 2064 203d 2068 7673  .        d = hvs
-0002f470: 725f 7265 7375 6c74 730a 2020 2020 2020  r_results.      
-0002f480: 2020 6372 6974 6572 6961 4c69 7374 203d    criteriaList =
-0002f490: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
-0002f4a0: 7020 696e 2068 7673 725f 7265 7375 6c74  p in hvsr_result
-0002f4b0: 735b 2742 6573 7420 5065 616b 275d 5b22  s['Best Peak']["
-0002f4c0: 5061 7373 204c 6973 7422 5d3a 0a20 2020  Pass List"]:.   
-0002f4d0: 2020 2020 2020 2020 2063 7269 7465 7269           criteri
-0002f4e0: 614c 6973 742e 6170 7065 6e64 2868 7673  aList.append(hvs
-0002f4f0: 725f 7265 7375 6c74 735b 2742 6573 7420  r_results['Best 
-0002f500: 5065 616b 275d 5b22 5061 7373 204c 6973  Peak']["Pass Lis
-0002f510: 7422 5d5b 705d 290a 2020 2020 2020 2020  t"][p]).        
-0002f520: 6372 6974 6572 6961 4c69 7374 2e61 7070  criteriaList.app
-0002f530: 656e 6428 6876 7372 5f72 6573 756c 7473  end(hvsr_results
-0002f540: 5b27 4265 7374 2050 6561 6b27 5d5b 2250  ['Best Peak']["P
-0002f550: 6561 6b20 5061 7373 6573 225d 290a 2020  eak Passes"]).  
-0002f560: 2020 2020 2020 6466 4c69 7374 203d 205b        dfList = [
-0002f570: 5b64 5b27 696e 7075 745f 7061 7261 6d73  [d['input_params
-0002f580: 275d 5b27 7369 7465 275d 2c20 645b 2769  ']['site'], d['i
-0002f590: 6e70 7574 5f70 6172 616d 7327 5d5b 2761  nput_params']['a
-0002f5a0: 6371 5f64 6174 6527 5d2c 2064 5b27 696e  cq_date'], d['in
-0002f5b0: 7075 745f 7061 7261 6d73 275d 5b27 6c6f  put_params']['lo
-0002f5c0: 6e67 6974 7564 6527 5d2c 2064 5b27 696e  ngitude'], d['in
-0002f5d0: 7075 745f 7061 7261 6d73 275d 5b27 6c61  put_params']['la
-0002f5e0: 7469 7475 6465 275d 2c20 645b 2769 6e70  titude'], d['inp
-0002f5f0: 7574 5f70 6172 616d 7327 5d5b 2765 6c65  ut_params']['ele
-0002f600: 7661 7469 6f6e 275d 2c20 726f 756e 6428  vation'], round(
-0002f610: 645b 2742 6573 7420 5065 616b 275d 5b27  d['Best Peak']['
-0002f620: 6630 275d 2c20 3329 5d5d 0a20 2020 2020  f0'], 3)]].     
-0002f630: 2020 2064 664c 6973 745b 305d 2e65 7874     dfList[0].ext
-0002f640: 656e 6428 6372 6974 6572 6961 4c69 7374  end(criteriaList
-0002f650: 290a 2020 2020 2020 2020 6f75 7444 4620  ).        outDF 
-0002f660: 3d20 7064 2e44 6174 6146 7261 6d65 2864  = pd.DataFrame(d
-0002f670: 664c 6973 742c 2063 6f6c 756d 6e73 3d70  fList, columns=p
-0002f680: 6443 6f6c 7329 0a20 2020 2020 2020 2069  dCols).        i
-0002f690: 6620 6578 706f 7274 3d3d 2727 3a0a 2020  f export=='':.  
-0002f6a0: 2020 2020 2020 2020 2020 696e 4669 6c65            inFile
-0002f6b0: 203d 2070 6174 686c 6962 2e50 6174 6828   = pathlib.Path(
-0002f6c0: 6876 7372 5f72 6573 756c 7473 5b27 696e  hvsr_results['in
-0002f6d0: 7075 745f 7061 7261 6d73 275d 5b27 2064  put_params'][' d
-0002f6e0: 6174 6170 6174 6827 5d29 0a20 2020 2020  atapath']).     
-0002f6f0: 2020 2020 2020 2069 6620 696e 4669 6c65         if inFile
-0002f700: 2e69 735f 6469 7228 293a 0a20 2020 2020  .is_dir():.     
-0002f710: 2020 2020 2020 2020 2020 2069 6e46 696c             inFil
-0002f720: 6520 3d20 696e 4669 6c65 2e61 735f 706f  e = inFile.as_po
-0002f730: 7369 7828 290a 2020 2020 2020 2020 2020  six().          
-0002f740: 2020 2020 2020 6966 2069 6e46 696c 655b        if inFile[
-0002f750: 2d31 5d3d 3d27 2f27 3a0a 2020 2020 2020  -1]=='/':.      
-0002f760: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-0002f770: 7373 0a20 2020 2020 2020 2020 2020 2020  ss.             
-0002f780: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0002f790: 2020 2020 2020 2020 2020 2020 2069 6e46               inF
-0002f7a0: 696c 6520 3d20 696e 4669 6c65 202b 2027  ile = inFile + '
-0002f7b0: 2f27 0a20 2020 2020 2020 2020 2020 2020  /'.             
-0002f7c0: 2020 2066 6e61 6d65 203d 2068 7673 725f     fname = hvsr_
-0002f7d0: 7265 7375 6c74 735b 2769 6e70 7574 5f70  results['input_p
-0002f7e0: 6172 616d 7327 5d5b 2773 6974 6527 5d2b  arams']['site']+
-0002f7f0: 275f 272b 7374 7228 6876 7372 5f72 6573  '_'+str(hvsr_res
-0002f800: 756c 7473 5b27 696e 7075 745f 7061 7261  ults['input_para
-0002f810: 6d73 275d 5b27 6163 715f 6461 7465 275d  ms']['acq_date']
-0002f820: 292b 275f 272b 7374 7228 6876 7372 5f72  )+'_'+str(hvsr_r
-0002f830: 6573 756c 7473 5b27 696e 7075 745f 7061  esults['input_pa
-0002f840: 7261 6d73 275d 5b27 7374 6172 7474 696d  rams']['starttim
-0002f850: 6527 5d2e 7469 6d65 295b 3a35 5d2b 272d  e'].time)[:5]+'-
-0002f860: 272b 7374 7228 6876 7372 5f72 6573 756c  '+str(hvsr_resul
-0002f870: 7473 5b27 696e 7075 745f 7061 7261 6d73  ts['input_params
-0002f880: 275d 5b27 656e 6474 696d 6527 5d2e 7469  ']['endtime'].ti
-0002f890: 6d65 295b 3a35 5d0a 2020 2020 2020 2020  me)[:5].        
-0002f8a0: 2020 2020 2020 2020 696e 4669 6c65 203d          inFile =
-0002f8b0: 2069 6e46 696c 6520 2b20 666e 616d 6520   inFile + fname 
-0002f8c0: 2b27 2e63 7376 270a 2020 2020 2020 2020  +'.csv'.        
-0002f8d0: 2020 2020 656c 6966 2069 6e46 696c 652e      elif inFile.
-0002f8e0: 6973 5f66 696c 6528 293a 0a20 2020 2020  is_file():.     
-0002f8f0: 2020 2020 2020 2020 2020 2065 7870 6f72             expor
-0002f900: 7420 3d20 696e 4669 6c65 2e77 6974 685f  t = inFile.with_
-0002f910: 7375 6666 6978 2827 2e63 7376 2729 0a20  suffix('.csv'). 
-0002f920: 2020 2020 2020 206f 7574 4446 2e74 6f5f         outDF.to_
-0002f930: 6373 7628 6578 706f 7274 2c20 696e 6465  csv(export, inde
-0002f940: 785f 6c61 6265 6c3d 2749 4427 290a 2020  x_label='ID').  
-0002f950: 2020 2020 2020 7265 7475 726e 206f 7574        return out
-0002f960: 4446 0a20 2020 2065 6c69 6620 666f 726d  DF.    elif form
-0002f970: 6174 3d3d 2770 6c6f 7427 3a0a 2020 2020  at=='plot':.    
-0002f980: 2020 2020 6876 7372 5f72 6573 756c 7473      hvsr_results
-0002f990: 5b27 4856 5f50 6c6f 7427 5d3d 6876 706c  ['HV_Plot']=hvpl
-0002f9a0: 6f74 2868 7673 725f 7265 7375 6c74 732c  ot(hvsr_results,
-0002f9b0: 2070 6c6f 745f 7479 7065 3d70 6c6f 745f   plot_type=plot_
-0002f9c0: 7479 7065 290a 2020 2020 2020 2020 6966  type).        if
-0002f9d0: 2072 6574 7572 6e5f 7265 7375 6c74 733a   return_results:
-0002f9e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0002f9f0: 7572 6e20 6876 7372 5f72 6573 756c 7473  urn hvsr_results
-0002fa00: 0a0a 2020 2020 6966 2065 7870 6f72 743a  ..    if export:
-0002fa10: 0a20 2020 2020 2020 2070 6173 730a 2020  .        pass.  
-0002fa20: 2020 2020 2020 2363 6f64 6520 746f 2077        #code to w
-0002fa30: 7269 7465 2074 6f20 6f75 7470 7574 2066  rite to output f
-0002fa40: 696c 650a 2020 2020 7265 7475 726e       ile.    return
+0002f270: 616b 2028 4672 6571 2e20 5374 4465 7629  ak (Freq. StDev)
+0002f280: 3a27 2c20 6876 7372 5f72 6573 756c 7473  :', hvsr_results
+0002f290: 5b27 4265 7374 2050 6561 6b27 5d5b 2752  ['Best Peak']['R
+0002f2a0: 6570 6f72 7427 5d5b 2753 6627 5d29 0a20  eport']['Sf']). 
+0002f2b0: 2020 2020 2020 2070 7269 6e74 2827 5c74         print('\t
+0002f2c0: 5c74 272c 2068 7673 725f 7265 7375 6c74  \t', hvsr_result
+0002f2d0: 735b 2742 6573 7420 5065 616b 275d 5b27  s['Best Peak']['
+0002f2e0: 5265 706f 7274 275d 5b27 5361 275d 5b2d  Report']['Sa'][-
+0002f2f0: 315d 2c20 2753 7461 6269 6c69 7479 206f  1], 'Stability o
+0002f300: 6620 5065 616b 2028 416d 702e 2053 7444  f Peak (Amp. StD
+0002f310: 6576 293a 272c 2068 7673 725f 7265 7375  ev):', hvsr_resu
+0002f320: 6c74 735b 2742 6573 7420 5065 616b 275d  lts['Best Peak']
+0002f330: 5b27 5265 706f 7274 275d 5b27 5361 275d  ['Report']['Sa']
+0002f340: 290a 0a20 2020 2065 6c69 6620 666f 726d  )..    elif form
+0002f350: 6174 3d3d 2763 7376 273a 0a20 2020 2020  at=='csv':.     
+0002f360: 2020 2069 6d70 6f72 7420 7061 6e64 6173     import pandas
+0002f370: 2061 7320 7064 0a20 2020 2020 2020 2070   as pd.        p
+0002f380: 6443 6f6c 7320 3d20 5b27 5369 7465 204e  dCols = ['Site N
+0002f390: 616d 6527 2c20 2741 6371 7573 6974 696f  ame', 'Acqusitio
+0002f3a0: 6e20 4461 7465 272c 2027 4c6f 6e67 6974  n Date', 'Longit
+0002f3b0: 7564 6527 2c20 274c 6174 6974 6964 6527  ude', 'Latitide'
+0002f3c0: 2c20 2745 6c65 7661 7469 6f6e 272c 2027  , 'Elevation', '
+0002f3d0: 5065 616b 2046 7265 7175 656e 6379 272c  Peak Frequency',
+0002f3e0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+0002f3f0: 2020 2020 2757 696e 646f 7720 4c65 6e67      'Window Leng
+0002f400: 7468 2046 7265 712e 272c 2753 6967 6e69  th Freq.','Signi
+0002f410: 6669 6361 6e74 2043 7963 6c65 7327 2c27  ficant Cycles','
+0002f420: 4c6f 7720 4375 7276 6520 5374 4465 762e  Low Curve StDev.
+0002f430: 206f 7665 7220 7469 6d65 272c 0a20 2020   over time',.   
+0002f440: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0002f450: 5065 616b 2046 7265 712e 2043 6c61 7269  Peak Freq. Clari
+0002f460: 7479 2042 656c 6f77 272c 2750 6561 6b20  ty Below','Peak 
+0002f470: 4672 6571 2e20 436c 6172 6974 7920 4162  Freq. Clarity Ab
+0002f480: 6f76 6527 2c27 5065 616b 2041 6d70 2e20  ove','Peak Amp. 
+0002f490: 436c 6172 6974 7927 2c27 4672 6571 2e20  Clarity','Freq. 
+0002f4a0: 5374 6162 696c 6974 7927 2c20 2750 6561  Stability', 'Pea
+0002f4b0: 6b20 5374 6162 696c 6974 7920 2866 7265  k Stability (fre
+0002f4c0: 712e 2073 7464 2927 2c27 5065 616b 2053  q. std)','Peak S
+0002f4d0: 7461 6269 6c69 7479 2028 616d 702e 2073  tability (amp. s
+0002f4e0: 7464 2927 2c20 2750 6561 6b20 5061 7373  td)', 'Peak Pass
+0002f4f0: 6573 275d 0a20 2020 2020 2020 2064 203d  es'].        d =
+0002f500: 2068 7673 725f 7265 7375 6c74 730a 2020   hvsr_results.  
+0002f510: 2020 2020 2020 6372 6974 6572 6961 4c69        criteriaLi
+0002f520: 7374 203d 205b 5d0a 2020 2020 2020 2020  st = [].        
+0002f530: 666f 7220 7020 696e 2068 7673 725f 7265  for p in hvsr_re
+0002f540: 7375 6c74 735b 2742 6573 7420 5065 616b  sults['Best Peak
+0002f550: 275d 5b22 5061 7373 204c 6973 7422 5d3a  ']["Pass List"]:
+0002f560: 0a20 2020 2020 2020 2020 2020 2063 7269  .            cri
+0002f570: 7465 7269 614c 6973 742e 6170 7065 6e64  teriaList.append
+0002f580: 2868 7673 725f 7265 7375 6c74 735b 2742  (hvsr_results['B
+0002f590: 6573 7420 5065 616b 275d 5b22 5061 7373  est Peak']["Pass
+0002f5a0: 204c 6973 7422 5d5b 705d 290a 2020 2020   List"][p]).    
+0002f5b0: 2020 2020 6372 6974 6572 6961 4c69 7374      criteriaList
+0002f5c0: 2e61 7070 656e 6428 6876 7372 5f72 6573  .append(hvsr_res
+0002f5d0: 756c 7473 5b27 4265 7374 2050 6561 6b27  ults['Best Peak'
+0002f5e0: 5d5b 2250 6561 6b20 5061 7373 6573 225d  ]["Peak Passes"]
+0002f5f0: 290a 2020 2020 2020 2020 6466 4c69 7374  ).        dfList
+0002f600: 203d 205b 5b64 5b27 696e 7075 745f 7061   = [[d['input_pa
+0002f610: 7261 6d73 275d 5b27 7369 7465 275d 2c20  rams']['site'], 
+0002f620: 645b 2769 6e70 7574 5f70 6172 616d 7327  d['input_params'
+0002f630: 5d5b 2761 6371 5f64 6174 6527 5d2c 2064  ]['acq_date'], d
+0002f640: 5b27 696e 7075 745f 7061 7261 6d73 275d  ['input_params']
+0002f650: 5b27 6c6f 6e67 6974 7564 6527 5d2c 2064  ['longitude'], d
+0002f660: 5b27 696e 7075 745f 7061 7261 6d73 275d  ['input_params']
+0002f670: 5b27 6c61 7469 7475 6465 275d 2c20 645b  ['latitude'], d[
+0002f680: 2769 6e70 7574 5f70 6172 616d 7327 5d5b  'input_params'][
+0002f690: 2765 6c65 7661 7469 6f6e 275d 2c20 726f  'elevation'], ro
+0002f6a0: 756e 6428 645b 2742 6573 7420 5065 616b  und(d['Best Peak
+0002f6b0: 275d 5b27 6630 275d 2c20 3329 5d5d 0a20  ']['f0'], 3)]]. 
+0002f6c0: 2020 2020 2020 2064 664c 6973 745b 305d         dfList[0]
+0002f6d0: 2e65 7874 656e 6428 6372 6974 6572 6961  .extend(criteria
+0002f6e0: 4c69 7374 290a 2020 2020 2020 2020 6f75  List).        ou
+0002f6f0: 7444 4620 3d20 7064 2e44 6174 6146 7261  tDF = pd.DataFra
+0002f700: 6d65 2864 664c 6973 742c 2063 6f6c 756d  me(dfList, colum
+0002f710: 6e73 3d70 6443 6f6c 7329 0a20 2020 2020  ns=pdCols).     
+0002f720: 2020 2069 6620 6578 706f 7274 2069 7320     if export is 
+0002f730: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002f740: 2020 7061 7373 0a20 2020 2020 2020 2065    pass.        e
+0002f750: 6c69 6620 6578 706f 7274 3d3d 2727 3a0a  lif export=='':.
+0002f760: 2020 2020 2020 2020 2020 2020 696e 4669              inFi
+0002f770: 6c65 203d 2070 6174 686c 6962 2e50 6174  le = pathlib.Pat
+0002f780: 6828 6876 7372 5f72 6573 756c 7473 5b27  h(hvsr_results['
+0002f790: 696e 7075 745f 7061 7261 6d73 275d 5b27  input_params']['
+0002f7a0: 2064 6174 6170 6174 6827 5d29 0a20 2020   datapath']).   
+0002f7b0: 2020 2020 2020 2020 2069 6620 696e 4669           if inFi
+0002f7c0: 6c65 2e69 735f 6469 7228 293a 0a20 2020  le.is_dir():.   
+0002f7d0: 2020 2020 2020 2020 2020 2020 2069 6e46               inF
+0002f7e0: 696c 6520 3d20 696e 4669 6c65 2e61 735f  ile = inFile.as_
+0002f7f0: 706f 7369 7828 290a 2020 2020 2020 2020  posix().        
+0002f800: 2020 2020 2020 2020 6966 2069 6e46 696c          if inFil
+0002f810: 655b 2d31 5d3d 3d27 2f27 3a0a 2020 2020  e[-1]=='/':.    
+0002f820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002f830: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
+0002f840: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0002f850: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0002f860: 6e46 696c 6520 3d20 696e 4669 6c65 202b  nFile = inFile +
+0002f870: 2027 2f27 0a20 2020 2020 2020 2020 2020   '/'.           
+0002f880: 2020 2020 2066 6e61 6d65 203d 2068 7673       fname = hvs
+0002f890: 725f 7265 7375 6c74 735b 2769 6e70 7574  r_results['input
+0002f8a0: 5f70 6172 616d 7327 5d5b 2773 6974 6527  _params']['site'
+0002f8b0: 5d2b 275f 272b 7374 7228 6876 7372 5f72  ]+'_'+str(hvsr_r
+0002f8c0: 6573 756c 7473 5b27 696e 7075 745f 7061  esults['input_pa
+0002f8d0: 7261 6d73 275d 5b27 6163 715f 6461 7465  rams']['acq_date
+0002f8e0: 275d 292b 275f 272b 7374 7228 6876 7372  '])+'_'+str(hvsr
+0002f8f0: 5f72 6573 756c 7473 5b27 696e 7075 745f  _results['input_
+0002f900: 7061 7261 6d73 275d 5b27 7374 6172 7474  params']['startt
+0002f910: 696d 6527 5d2e 7469 6d65 295b 3a35 5d2b  ime'].time)[:5]+
+0002f920: 272d 272b 7374 7228 6876 7372 5f72 6573  '-'+str(hvsr_res
+0002f930: 756c 7473 5b27 696e 7075 745f 7061 7261  ults['input_para
+0002f940: 6d73 275d 5b27 656e 6474 696d 6527 5d2e  ms']['endtime'].
+0002f950: 7469 6d65 295b 3a35 5d0a 2020 2020 2020  time)[:5].      
+0002f960: 2020 2020 2020 2020 2020 696e 4669 6c65            inFile
+0002f970: 203d 2069 6e46 696c 6520 2b20 666e 616d   = inFile + fnam
+0002f980: 6520 2b27 2e63 7376 270a 2020 2020 2020  e +'.csv'.      
+0002f990: 2020 2020 2020 656c 6966 2069 6e46 696c        elif inFil
+0002f9a0: 652e 6973 5f66 696c 6528 293a 0a20 2020  e.is_file():.   
+0002f9b0: 2020 2020 2020 2020 2020 2020 2065 7870               exp
+0002f9c0: 6f72 7420 3d20 696e 4669 6c65 2e77 6974  ort = inFile.wit
+0002f9d0: 685f 7375 6666 6978 2827 2e63 7376 2729  h_suffix('.csv')
+0002f9e0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+0002f9f0: 4446 2e74 6f5f 6373 7628 6578 706f 7274  DF.to_csv(export
+0002fa00: 2c20 696e 6465 785f 6c61 6265 6c3d 2749  , index_label='I
+0002fa10: 4427 290a 2020 2020 2020 2020 656c 7365  D').        else
+0002fa20: 3a0a 2020 2020 2020 2020 2020 2020 6f75  :.            ou
+0002fa30: 7444 462e 746f 5f63 7376 2865 7870 6f72  tDF.to_csv(expor
+0002fa40: 742c 2069 6e64 6578 5f6c 6162 656c 3d27  t, index_label='
+0002fa50: 4944 2729 0a20 2020 2020 2020 2068 7673  ID').        hvs
+0002fa60: 725f 7265 7375 6c74 735b 2743 5356 5f52  r_results['CSV_R
+0002fa70: 6570 6f72 7427 5d20 3d20 6f75 7444 460a  eport'] = outDF.
+0002fa80: 2020 2020 2020 2020 7265 7475 726e 206f          return o
+0002fa90: 7574 4446 0a20 2020 2065 6c69 6620 666f  utDF.    elif fo
+0002faa0: 726d 6174 3d3d 2770 6c6f 7427 3a0a 2020  rmat=='plot':.  
+0002fab0: 2020 2020 2020 6876 7372 5f72 6573 756c        hvsr_resul
+0002fac0: 7473 5b27 4856 5f50 6c6f 7427 5d3d 6876  ts['HV_Plot']=hv
+0002fad0: 706c 6f74 2868 7673 725f 7265 7375 6c74  plot(hvsr_result
+0002fae0: 732c 2070 6c6f 745f 7479 7065 3d70 6c6f  s, plot_type=plo
+0002faf0: 745f 7479 7065 290a 2020 2020 2020 2020  t_type).        
+0002fb00: 6966 2072 6574 7572 6e5f 7265 7375 6c74  if return_result
+0002fb10: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+0002fb20: 6574 7572 6e20 6876 7372 5f72 6573 756c  eturn hvsr_resul
+0002fb30: 7473 0a0a 2020 2020 6966 2065 7870 6f72  ts..    if expor
+0002fb40: 743a 0a20 2020 2020 2020 2070 6173 730a  t:.        pass.
+0002fb50: 2020 2020 2020 2020 2363 6f64 6520 746f          #code to
+0002fb60: 2077 7269 7465 2074 6f20 6f75 7470 7574   write to output
+0002fb70: 2066 696c 650a 2020 2020 7265 7475 726e   file.    return
```

### Comparing `sprit-0.1.3/sprit/sprit_gui.py` & `sprit-0.1.4/sprit/sprit_gui.py`

 * *Files identical despite different names*

### Comparing `sprit-0.1.3/sprit.egg-info/PKG-INFO` & `sprit-0.1.4/sprit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprit
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for processing and analyzing HVSR (Horizontal to Vertical Spectral Ratio) data
 Author: Riley Balikian
 Author-email: balikian@illinois.edu
 License: MIT License
         
         Copyright (c) 2023 RJbalikian
```

### Comparing `sprit-0.1.3/sprit.egg-info/SOURCES.txt` & `sprit-0.1.4/sprit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

