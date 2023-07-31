# Comparing `tmp/browserist-1.5.0.tar.gz` & `tmp/browserist-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserist-1.5.0.tar", last modified: Sun Jun 18 10:20:39 2023, max compression
+gzip compressed data, was "browserist-1.5.1.tar", last modified: Mon Jul 31 01:28:07 2023, max compression
```

## Comparing `browserist-1.5.0.tar` & `browserist-1.5.1.tar`

### file list

```diff
@@ -1,314 +1,330 @@
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.443834 browserist-1.5.0/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2198 2023-06-18 10:14:23.000000 browserist-1.5.0/INSTALLATION.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    11343 2023-01-25 13:58:31.000000 browserist-1.5.0/LICENSE.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      217 2023-04-02 09:20:52.000000 browserist-1.5.0/MANIFEST.in
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    24782 2023-06-18 10:20:39.444338 browserist-1.5.0/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    10257 2023-06-18 10:14:23.000000 browserist-1.5.0/README.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      141 2023-02-03 11:49:45.000000 browserist-1.5.0/pyproject.toml
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1811 2023-06-18 10:20:39.445045 browserist-1.5.0/setup.cfg
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.352210 browserist-1.5.0/src/
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.356525 browserist-1.5.0/src/browserist/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1016 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.357872 browserist-1.5.0/src/browserist/browser/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     4622 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/browser/__main__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.360703 browserist-1.5.0/src/browserist/browser/check_if/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/check_if/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3312 2023-06-15 14:37:23.000000 browserist-1.5.0/src/browserist/browser/check_if/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      447 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/check_if/contains_any_text.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      590 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/check_if/contains_text.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      400 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/check_if/does_exist.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      506 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/check_if/is_clickable.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      299 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/check_if/is_disabled.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      427 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/check_if/is_displayed.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      423 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/check_if/is_enabled.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      504 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/check_if/is_image_loaded.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      999 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/check_if/is_in_viewport.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      425 2023-06-15 14:37:23.000000 browserist-1.5.0/src/browserist/browser/check_if/is_selected.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.361720 browserist-1.5.0/src/browserist/browser/click/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/click/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1017 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/click/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      721 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/browser/click/button.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1094 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/click/button_if_contains_text.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.362851 browserist-1.5.0/src/browserist/browser/combo/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/combo/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1815 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/combo/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1619 2023-02-01 06:40:37.000000 browserist-1.5.0/src/browserist/browser/combo/cookie_banner.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3071 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/combo/log_in.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1440 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/combo/search.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.364247 browserist-1.5.0/src/browserist/browser/get/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3275 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/__main__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.365505 browserist-1.5.0/src/browserist/browser/get/attribute/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/attribute/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1414 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/attribute/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      505 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/attribute/value.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      542 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/attribute/values.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      639 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/dimensions.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      732 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/element.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      749 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/elements.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      416 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/elements_by_tag.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      199 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/page_title.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      681 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/text.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      491 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/texts.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.367622 browserist-1.5.0/src/browserist/browser/get/url/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/url/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2690 2023-03-17 10:25:47.000000 browserist-1.5.0/src/browserist/browser/get/url/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      207 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/url/current.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      270 2023-03-17 10:25:47.000000 browserist-1.5.0/src/browserist/browser/get/url/current_domain.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      683 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/url/from_image.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      342 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/url/from_images.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      685 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/url/from_link.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      342 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/get/url/from_links.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.368498 browserist-1.5.0/src/browserist/browser/iframe/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/iframe/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      858 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/iframe/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      533 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/iframe/switch_to.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      224 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/iframe/switch_to_original_page.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.369387 browserist-1.5.0/src/browserist/browser/input/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/input/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1622 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/input/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      495 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/input/clear.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      461 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/input/select.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      588 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/input/value.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.369969 browserist-1.5.0/src/browserist/browser/mouse/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/mouse/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      593 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/mouse/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      642 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/mouse/hover.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.370652 browserist-1.5.0/src/browserist/browser/open/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/open/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1229 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/open/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      253 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/open/url.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      986 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/open/url_if_not_current.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.371815 browserist-1.5.0/src/browserist/browser/prompt/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/browser/prompt/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1085 2023-06-15 14:37:23.000000 browserist-1.5.0/src/browserist/browser/prompt/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      474 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/browser/prompt/input_value.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      647 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/browser/prompt/proceed_yes_or_no.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.373188 browserist-1.5.0/src/browserist/browser/screenshot/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/screenshot/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3403 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/screenshot/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1116 2023-03-17 10:25:47.000000 browserist-1.5.0/src/browserist/browser/screenshot/complete_page.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      992 2023-03-17 10:25:47.000000 browserist-1.5.0/src/browserist/browser/screenshot/element.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      796 2023-03-17 10:25:47.000000 browserist-1.5.0/src/browserist/browser/screenshot/visible_portion.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.376853 browserist-1.5.0/src/browserist/browser/scroll/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     4040 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      373 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/by.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.378783 browserist-1.5.0/src/browserist/browser/scroll/check_if/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/check_if/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      872 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/check_if/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      725 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/check_if/is_end_of_page.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      245 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/check_if/is_top_of_page.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      238 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/down_by.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.380468 browserist-1.5.0/src/browserist/browser/scroll/get/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/get/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      825 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/get/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      347 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/get/position.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      545 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/get/total_height.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      681 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/into_view.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      483 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/into_view_if_not_visible.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      239 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/left_by.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.383669 browserist-1.5.0/src/browserist/browser/scroll/page/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/page/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1559 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/page/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      384 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/page/down.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1354 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/page/to_end.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      251 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/page/to_top.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      385 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/page/up.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      239 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/right_by.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      382 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/to_position.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      237 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/scroll/up_by.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.385181 browserist-1.5.0/src/browserist/browser/tool/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/tool/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1472 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/tool/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      454 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/tool/count_elements.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      347 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/tool/execute_script.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      216 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/tool/is_input_valid.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.385688 browserist-1.5.0/src/browserist/browser/viewport/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/viewport/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      561 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/viewport/__main__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.387674 browserist-1.5.0/src/browserist/browser/viewport/get/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/viewport/get/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1061 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/viewport/get/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      248 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/viewport/get/height.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      330 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/viewport/get/size.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      246 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/viewport/get/width.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.389034 browserist-1.5.0/src/browserist/browser/viewport/set/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/viewport/set/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1312 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/viewport/set/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      982 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/viewport/set/size.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      318 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/viewport/set/size_by_device.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.390558 browserist-1.5.0/src/browserist/browser/wait/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1513 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/browser/wait/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1651 2023-06-18 10:12:35.000000 browserist-1.5.0/src/browserist/browser/wait/for_element.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      158 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/browser/wait/random_seconds.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       80 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/browser/wait/seconds.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.396038 browserist-1.5.0/src/browserist/browser/wait/until/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2791 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      467 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/contains_any_text.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      446 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/element_disappears.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      829 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/images_have_loaded.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      438 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/is_clickable.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1215 2023-06-18 10:12:35.000000 browserist-1.5.0/src/browserist/browser/wait/until/number_of_window_handles_is.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.397545 browserist-1.5.0/src/browserist/browser/wait/until/page_title/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/page_title/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1658 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/page_title/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      542 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/page_title/changes.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1200 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/browser/wait/until/page_title/contains.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1156 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/browser/wait/until/page_title/equals.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.399106 browserist-1.5.0/src/browserist/browser/wait/until/text/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/text/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1570 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/text/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      722 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/text/changes.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      789 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/text/contains.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      742 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/text/equals.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.401096 browserist-1.5.0/src/browserist/browser/wait/until/url/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/url/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1622 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/url/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      593 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/wait/until/url/changes.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1121 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/browser/wait/until/url/contains.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1137 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/browser/wait/until/url/equals.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.402502 browserist-1.5.0/src/browserist/browser/window/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2857 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      479 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/close.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      210 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/fullscreen.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.403557 browserist-1.5.0/src/browserist/browser/window/get/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/get/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1456 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/get/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      234 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/get/height.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      327 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/get/position.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      320 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/get/size.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      232 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/get/width.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.404378 browserist-1.5.0/src/browserist/browser/window/handle/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/handle/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1617 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/handle/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      449 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/handle/all.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      403 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/handle/count.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      227 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/handle/current.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      206 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/maximize.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      206 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/minimize.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.404978 browserist-1.5.0/src/browserist/browser/window/open/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/open/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1599 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/open/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1307 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/open/new_tab_or_window.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.406069 browserist-1.5.0/src/browserist/browser/window/set/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/set/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      793 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/set/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      235 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/set/position.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      245 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/set/size.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      573 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/browser/window/switch_to.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.407135 browserist-1.5.0/src/browserist/constant/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      117 2023-02-01 06:40:45.000000 browserist-1.5.0/src/browserist/constant/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       97 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/constant/directory.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       60 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/constant/interval.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       48 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/constant/screenshot.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      249 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/constant/timeout.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.409059 browserist-1.5.0/src/browserist/exception/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/exception/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1392 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/exception/element.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      273 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/exception/file_png.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      723 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/exception/headless.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      437 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/exception/retry.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      250 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/exception/scroll.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1821 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/exception/timeout.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      254 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/exception/url.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1762 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/exception/window_handle.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      262 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/exception/xpath.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.410715 browserist-1.5.0/src/browserist/factory/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      129 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/factory/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      646 2023-04-10 10:57:16.000000 browserist-1.5.0/src/browserist/factory/chromium.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1170 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/factory/get.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      944 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/factory/internet_explorer.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      887 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/factory/safari.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      717 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/factory/set.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.416252 browserist-1.5.0/src/browserist/helper/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      309 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/helper/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      416 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/helper/date_time.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1220 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/helper/directory.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      460 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/helper/file.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1418 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/helper/image.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       83 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/helper/operating_system.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      117 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/helper/regex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      468 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/helper/terminal.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      590 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/helper/timeout.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1591 2023-03-17 10:25:47.000000 browserist-1.5.0/src/browserist/helper/url.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      272 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/helper/viewport.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      626 2023-03-20 06:14:36.000000 browserist-1.5.0/src/browserist/helper/window_handle.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      934 2023-02-01 06:40:45.000000 browserist-1.5.0/src/browserist/helper/xpath.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.417206 browserist-1.5.0/src/browserist/helper_iteration/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       41 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/helper_iteration/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2796 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/helper_iteration/retry.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.418057 browserist-1.5.0/src/browserist/helper_screenshot/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      976 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/helper_screenshot/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3489 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/helper_screenshot/complete_page.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1422 2023-03-17 10:25:47.000000 browserist-1.5.0/src/browserist/helper_screenshot/controller.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1420 2023-03-17 10:25:47.000000 browserist-1.5.0/src/browserist/helper_screenshot/file.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.419729 browserist-1.5.0/src/browserist/model/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.420899 browserist-1.5.0/src/browserist/model/browser/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      636 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/browser/README.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/browser/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.421709 browserist-1.5.0/src/browserist/model/browser/base/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/browser/base/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     4381 2023-06-18 10:12:35.000000 browserist-1.5.0/src/browserist/model/browser/base/driver.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      459 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/browser/base/page_load_strategy.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1854 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/browser/base/settings.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.422433 browserist-1.5.0/src/browserist/model/browser/base/timeout/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/browser/base/timeout/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      684 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/browser/base/timeout/settings.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      261 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/browser/base/timeout/strategy.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      283 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/browser/base/type.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1092 2023-06-18 10:12:35.000000 browserist-1.5.0/src/browserist/model/browser/chrome.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1512 2023-06-18 10:12:35.000000 browserist-1.5.0/src/browserist/model/browser/edge.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.423124 browserist-1.5.0/src/browserist/model/browser/extension/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/browser/extension/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      601 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/browser/extension/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      439 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/browser/extension/internet_explorer.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      407 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/browser/extension/safari.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1299 2023-06-18 10:12:35.000000 browserist-1.5.0/src/browserist/model/browser/firefox.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1117 2023-06-18 10:12:35.000000 browserist-1.5.0/src/browserist/model/browser/internet_explorer.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1105 2023-06-18 10:12:35.000000 browserist-1.5.0/src/browserist/model/browser/opera.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1125 2023-06-18 10:12:35.000000 browserist-1.5.0/src/browserist/model/browser/safari.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.424146 browserist-1.5.0/src/browserist/model/combo_settings/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/combo_settings/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1184 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/combo_settings/cookie_banner.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      289 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/combo_settings/login_credentials.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2770 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/combo_settings/login_form.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1105 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/combo_settings/search.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      987 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/driver_methods.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3215 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/screenshot.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.424949 browserist-1.5.0/src/browserist/model/type/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/type/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      507 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/model/type/callable.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      823 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/type/file_png.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      789 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/type/path.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      773 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/type/url.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      811 2023-02-01 06:40:45.000000 browserist-1.5.0/src/browserist/model/type/xpath.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.426047 browserist-1.5.0/src/browserist/model/viewport/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/viewport/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.433392 browserist-1.5.0/src/browserist/model/viewport/collection/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/viewport/collection/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1080 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/model/viewport/collection/apple.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      271 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/model/viewport/collection/google.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      234 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/model/viewport/collection/microsoft.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      333 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/model/viewport/collection/samsung.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      285 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/viewport/common_devices.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      208 2023-02-03 11:49:45.000000 browserist-1.5.0/src/browserist/model/viewport/device.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.438709 browserist-1.5.0/src/browserist/model/window/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/window/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3231 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/window/controller.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      261 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/window/handle.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      212 2023-01-25 13:58:31.000000 browserist-1.5.0/src/browserist/model/window/tab_or_window.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-01-25 15:16:10.000000 browserist-1.5.0/src/browserist/py.typed
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       80 2023-06-18 10:14:41.000000 browserist-1.5.0/src/browserist/version.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-18 10:20:39.357461 browserist-1.5.0/src/browserist.egg-info/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    24782 2023-06-18 10:20:39.000000 browserist-1.5.0/src/browserist.egg-info/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    11230 2023-06-18 10:20:39.000000 browserist-1.5.0/src/browserist.egg-info/SOURCES.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-06-18 10:20:39.000000 browserist-1.5.0/src/browserist.egg-info/dependency_links.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-25 15:10:37.000000 browserist-1.5.0/src/browserist.egg-info/not-zip-safe
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      169 2023-06-18 10:20:39.000000 browserist-1.5.0/src/browserist.egg-info/requires.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       11 2023-06-18 10:20:39.000000 browserist-1.5.0/src/browserist.egg-info/top_level.txt
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.518000 browserist-1.5.1/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2368 2023-07-31 01:21:47.000000 browserist-1.5.1/INSTALLATION.md
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)    11343 2022-04-27 16:24:39.000000 browserist-1.5.1/LICENSE.md
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      217 2023-07-28 09:43:17.000000 browserist-1.5.1/MANIFEST.in
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)    18731 2023-07-31 01:28:07.518394 browserist-1.5.1/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     4036 2023-07-31 01:21:47.000000 browserist-1.5.1/README.md
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      141 2023-07-10 16:42:59.000000 browserist-1.5.1/pyproject.toml
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1812 2023-07-31 01:28:07.520987 browserist-1.5.1/setup.cfg
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.040766 browserist-1.5.1/src/
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.164626 browserist-1.5.1/src/browserist/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1016 2022-12-28 11:41:43.000000 browserist-1.5.1/src/browserist/__init__.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.194832 browserist-1.5.1/src/browserist/browser/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     4940 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/__main__.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.229884 browserist-1.5.1/src/browserist/browser/check_if/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/check_if/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     5058 2023-07-28 14:41:31.000000 browserist-1.5.1/src/browserist/browser/check_if/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      447 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/check_if/contains_any_text.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      590 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/check_if/contains_text.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      400 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/check_if/does_exist.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      506 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/check_if/is_clickable.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      299 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/check_if/is_disabled.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      427 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/check_if/is_displayed.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      423 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/check_if/is_enabled.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      504 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/check_if/is_image_loaded.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      999 2022-09-05 16:59:39.000000 browserist-1.5.1/src/browserist/browser/check_if/is_in_viewport.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      425 2023-07-28 09:43:17.000000 browserist-1.5.1/src/browserist/browser/check_if/is_selected.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.242621 browserist-1.5.1/src/browserist/browser/click/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/click/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1764 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/click/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      721 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/browser/click/button.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1094 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/click/button_if_contains_text.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.260376 browserist-1.5.1/src/browserist/browser/combo/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/combo/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     3026 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/combo/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1619 2022-12-15 05:40:55.000000 browserist-1.5.1/src/browserist/browser/combo/cookie_banner.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     3071 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/combo/log_in.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1440 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/combo/search.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.282723 browserist-1.5.1/src/browserist/browser/get/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/get/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     4845 2023-07-31 01:02:22.000000 browserist-1.5.1/src/browserist/browser/get/__main__.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.292023 browserist-1.5.1/src/browserist/browser/get/attribute/
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.296879 browserist-1.5.1/src/browserist/browser/get/attribute/.pytest_cache/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       37 2022-06-13 18:03:21.000000 browserist-1.5.1/src/browserist/browser/get/attribute/.pytest_cache/.gitignore
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      191 2022-06-13 18:03:21.000000 browserist-1.5.1/src/browserist/browser/get/attribute/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      302 2022-06-13 18:03:21.000000 browserist-1.5.1/src/browserist/browser/get/attribute/.pytest_cache/README.md
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.054126 browserist-1.5.1/src/browserist/browser/get/attribute/.pytest_cache/v/
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.303157 browserist-1.5.1/src/browserist/browser/get/attribute/.pytest_cache/v/cache/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        2 2022-06-13 18:03:21.000000 browserist-1.5.1/src/browserist/browser/get/attribute/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        2 2022-06-13 18:03:21.000000 browserist-1.5.1/src/browserist/browser/get/attribute/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/get/attribute/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2126 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/get/attribute/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      505 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/get/attribute/value.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      542 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/get/attribute/values.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      639 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/get/dimensions.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      732 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/get/element.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      749 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/get/elements.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      416 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/get/elements_by_tag.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      199 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/get/page_title.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      681 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/get/text.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      491 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/get/texts.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.322227 browserist-1.5.1/src/browserist/browser/get/url/
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.327411 browserist-1.5.1/src/browserist/browser/get/url/.pytest_cache/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       37 2022-06-13 22:10:16.000000 browserist-1.5.1/src/browserist/browser/get/url/.pytest_cache/.gitignore
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      191 2022-06-13 22:10:16.000000 browserist-1.5.1/src/browserist/browser/get/url/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      302 2022-06-13 22:10:16.000000 browserist-1.5.1/src/browserist/browser/get/url/.pytest_cache/README.md
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.070796 browserist-1.5.1/src/browserist/browser/get/url/.pytest_cache/v/
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.332120 browserist-1.5.1/src/browserist/browser/get/url/.pytest_cache/v/cache/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        2 2022-06-13 22:10:16.000000 browserist-1.5.1/src/browserist/browser/get/url/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        2 2022-06-13 22:10:16.000000 browserist-1.5.1/src/browserist/browser/get/url/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/get/url/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     4171 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/get/url/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      207 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/get/url/current.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      270 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/browser/get/url/current_domain.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      683 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/get/url/from_image.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      342 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/get/url/from_images.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      685 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/get/url/from_link.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      342 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/get/url/from_links.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.345074 browserist-1.5.1/src/browserist/browser/iframe/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/iframe/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1084 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/iframe/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      533 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/iframe/switch_to.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      224 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/iframe/switch_to_original_page.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.362551 browserist-1.5.1/src/browserist/browser/input/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/input/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2472 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/input/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      495 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/input/clear.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      461 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/input/select.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      588 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/input/value.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.372501 browserist-1.5.1/src/browserist/browser/mouse/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/mouse/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      818 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/mouse/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      642 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/mouse/hover.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.407116 browserist-1.5.1/src/browserist/browser/open/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/open/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1671 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/open/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      253 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/open/url.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      986 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/open/url_if_not_current.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.423855 browserist-1.5.1/src/browserist/browser/prompt/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/browser/prompt/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1588 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/prompt/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      474 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/browser/prompt/input_value.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      647 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/browser/prompt/proceed_yes_or_no.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.462283 browserist-1.5.1/src/browserist/browser/screenshot/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-07-15 15:31:49.000000 browserist-1.5.1/src/browserist/browser/screenshot/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     4914 2023-07-28 14:41:31.000000 browserist-1.5.1/src/browserist/browser/screenshot/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1116 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/browser/screenshot/complete_page.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      992 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/browser/screenshot/element.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      796 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/browser/screenshot/visible_portion.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.564903 browserist-1.5.1/src/browserist/browser/scroll/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/scroll/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     5798 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/scroll/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      373 2022-08-15 08:27:18.000000 browserist-1.5.1/src/browserist/browser/scroll/by.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.611453 browserist-1.5.1/src/browserist/browser/scroll/check_if/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-07-01 04:59:43.000000 browserist-1.5.1/src/browserist/browser/scroll/check_if/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1122 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/scroll/check_if/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      725 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/scroll/check_if/is_end_of_page.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      245 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/scroll/check_if/is_top_of_page.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      238 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/scroll/down_by.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.660902 browserist-1.5.1/src/browserist/browser/scroll/get/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-07-01 04:59:43.000000 browserist-1.5.1/src/browserist/browser/scroll/get/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1055 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/scroll/get/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      347 2022-08-15 08:27:18.000000 browserist-1.5.1/src/browserist/browser/scroll/get/position.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      545 2022-08-15 08:27:18.000000 browserist-1.5.1/src/browserist/browser/scroll/get/total_height.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      681 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/scroll/into_view.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      483 2022-09-05 16:59:39.000000 browserist-1.5.1/src/browserist/browser/scroll/into_view_if_not_visible.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      239 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/scroll/left_by.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.689461 browserist-1.5.1/src/browserist/browser/scroll/page/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-07-01 04:59:43.000000 browserist-1.5.1/src/browserist/browser/scroll/page/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1875 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/scroll/page/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      384 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/scroll/page/down.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1354 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/scroll/page/to_end.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      251 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/scroll/page/to_top.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      385 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/scroll/page/up.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      239 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/scroll/right_by.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      382 2022-08-15 08:27:18.000000 browserist-1.5.1/src/browserist/browser/scroll/to_position.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      237 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/scroll/up_by.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.697327 browserist-1.5.1/src/browserist/browser/tool/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/tool/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2833 2023-07-31 01:20:26.000000 browserist-1.5.1/src/browserist/browser/tool/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      454 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/tool/count_elements.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      347 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/tool/execute_script.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      216 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/tool/is_input_valid.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.701811 browserist-1.5.1/src/browserist/browser/viewport/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/viewport/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      561 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/viewport/__main__.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.709776 browserist-1.5.1/src/browserist/browser/viewport/get/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/viewport/get/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1377 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/viewport/get/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      248 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/viewport/get/height.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      330 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/viewport/get/size.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      246 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/viewport/get/width.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.718400 browserist-1.5.1/src/browserist/browser/viewport/set/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/viewport/set/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1839 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/viewport/set/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      982 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/viewport/set/size.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      318 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/viewport/set/size_by_device.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.753327 browserist-1.5.1/src/browserist/browser/wait/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/wait/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2338 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/wait/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1651 2023-07-28 09:43:17.000000 browserist-1.5.1/src/browserist/browser/wait/for_element.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      158 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/browser/wait/random_seconds.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       80 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/browser/wait/seconds.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.803680 browserist-1.5.1/src/browserist/browser/wait/until/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-28 05:34:12.000000 browserist-1.5.1/src/browserist/browser/wait/until/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     4598 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/wait/until/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      467 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/wait/until/contains_any_text.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      446 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/wait/until/element_disappears.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      829 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/wait/until/images_have_loaded.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      438 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/wait/until/is_clickable.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1215 2023-07-28 09:43:17.000000 browserist-1.5.1/src/browserist/browser/wait/until/number_of_window_handles_is.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.826570 browserist-1.5.1/src/browserist/browser/wait/until/page_title/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-28 05:34:12.000000 browserist-1.5.1/src/browserist/browser/wait/until/page_title/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2500 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/wait/until/page_title/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      542 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/wait/until/page_title/changes.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1200 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/browser/wait/until/page_title/contains.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1156 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/browser/wait/until/page_title/equals.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.853819 browserist-1.5.1/src/browserist/browser/wait/until/text/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-28 05:34:12.000000 browserist-1.5.1/src/browserist/browser/wait/until/text/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2666 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/wait/until/text/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      722 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/wait/until/text/changes.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      789 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/wait/until/text/contains.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      742 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/wait/until/text/equals.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.923735 browserist-1.5.1/src/browserist/browser/wait/until/url/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-28 05:34:12.000000 browserist-1.5.1/src/browserist/browser/wait/until/url/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     3452 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/wait/until/url/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      593 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/wait/until/url/changes.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1121 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/browser/wait/until/url/contains.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1137 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/browser/wait/until/url/equals.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.937536 browserist-1.5.1/src/browserist/browser/window/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/window/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     3657 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/window/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      479 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/window/close.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      210 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/window/fullscreen.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.946175 browserist-1.5.1/src/browserist/browser/window/get/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/window/get/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2017 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/window/get/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      234 2022-08-15 08:26:38.000000 browserist-1.5.1/src/browserist/browser/window/get/height.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      327 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/window/get/position.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      320 2022-08-15 08:26:38.000000 browserist-1.5.1/src/browserist/browser/window/get/size.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      232 2022-08-15 08:26:38.000000 browserist-1.5.1/src/browserist/browser/window/get/width.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.095134 browserist-1.5.1/src/browserist/browser/window/handle/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/window/handle/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1929 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/window/handle/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      449 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/window/handle/all.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      403 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/browser/window/handle/count.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      227 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/window/handle/current.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      206 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/window/maximize.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      206 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/window/minimize.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.110303 browserist-1.5.1/src/browserist/browser/window/open/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/window/open/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2895 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/browser/window/open/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1307 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/window/open/new_tab_or_window.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.128500 browserist-1.5.1/src/browserist/browser/window/set/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/browser/window/set/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1365 2023-07-29 16:01:46.000000 browserist-1.5.1/src/browserist/browser/window/set/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      235 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/window/set/position.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      245 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/window/set/size.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      573 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/browser/window/switch_to.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.139980 browserist-1.5.1/src/browserist/constant/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      117 2022-10-26 03:09:24.000000 browserist-1.5.1/src/browserist/constant/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       97 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/constant/directory.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       60 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/constant/interval.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       48 2022-07-21 01:25:19.000000 browserist-1.5.1/src/browserist/constant/screenshot.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      249 2022-08-09 18:35:35.000000 browserist-1.5.1/src/browserist/constant/timeout.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.153846 browserist-1.5.1/src/browserist/exception/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/exception/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1392 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/exception/element.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      273 2022-09-23 20:59:14.000000 browserist-1.5.1/src/browserist/exception/file_png.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      723 2022-06-28 05:34:12.000000 browserist-1.5.1/src/browserist/exception/headless.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      437 2022-06-28 05:34:12.000000 browserist-1.5.1/src/browserist/exception/retry.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      250 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/exception/scroll.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1821 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/exception/timeout.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      254 2022-06-28 05:34:12.000000 browserist-1.5.1/src/browserist/exception/url.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1762 2022-06-28 05:34:12.000000 browserist-1.5.1/src/browserist/exception/window_handle.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      262 2022-06-28 05:34:12.000000 browserist-1.5.1/src/browserist/exception/xpath.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.161894 browserist-1.5.1/src/browserist/factory/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      129 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/factory/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      646 2023-07-28 09:43:17.000000 browserist-1.5.1/src/browserist/factory/chromium.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1170 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/factory/get.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      944 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/factory/internet_explorer.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      887 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/factory/safari.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      717 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/factory/set.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.180040 browserist-1.5.1/src/browserist/helper/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      309 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/helper/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      416 2022-07-21 01:25:19.000000 browserist-1.5.1/src/browserist/helper/date_time.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1220 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/helper/directory.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      460 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/helper/file.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1418 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/helper/image.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       83 2022-08-06 22:42:23.000000 browserist-1.5.1/src/browserist/helper/operating_system.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      117 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/helper/regex.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      468 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/helper/terminal.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      590 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/helper/timeout.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1595 2023-07-29 15:52:42.000000 browserist-1.5.1/src/browserist/helper/url.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      272 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/helper/viewport.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      626 2023-07-28 09:43:17.000000 browserist-1.5.1/src/browserist/helper/window_handle.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      934 2022-10-26 03:09:24.000000 browserist-1.5.1/src/browserist/helper/xpath.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.184337 browserist-1.5.1/src/browserist/helper_iteration/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       41 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/helper_iteration/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2796 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/helper_iteration/retry.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.189683 browserist-1.5.1/src/browserist/helper_screenshot/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      976 2022-08-21 23:07:08.000000 browserist-1.5.1/src/browserist/helper_screenshot/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     3489 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/helper_screenshot/complete_page.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1422 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/helper_screenshot/controller.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1420 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/helper_screenshot/file.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.193032 browserist-1.5.1/src/browserist/model/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/model/__init__.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.204548 browserist-1.5.1/src/browserist/model/browser/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      636 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/model/browser/README.md
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/model/browser/__init__.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.214347 browserist-1.5.1/src/browserist/model/browser/base/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/model/browser/base/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     4381 2023-07-28 09:43:17.000000 browserist-1.5.1/src/browserist/model/browser/base/driver.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      459 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/model/browser/base/page_load_strategy.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1854 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/model/browser/base/settings.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.389943 browserist-1.5.1/src/browserist/model/browser/base/timeout/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/model/browser/base/timeout/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      684 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/model/browser/base/timeout/settings.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      261 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/model/browser/base/timeout/strategy.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      283 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/model/browser/base/type.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1092 2023-07-28 09:43:17.000000 browserist-1.5.1/src/browserist/model/browser/chrome.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1512 2023-07-28 09:43:17.000000 browserist-1.5.1/src/browserist/model/browser/edge.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.436115 browserist-1.5.1/src/browserist/model/browser/extension/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/model/browser/extension/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      601 2022-06-28 05:34:12.000000 browserist-1.5.1/src/browserist/model/browser/extension/__main__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      439 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/model/browser/extension/internet_explorer.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      407 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/model/browser/extension/safari.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1299 2023-07-28 09:43:17.000000 browserist-1.5.1/src/browserist/model/browser/firefox.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1117 2023-07-28 09:43:17.000000 browserist-1.5.1/src/browserist/model/browser/internet_explorer.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1105 2023-07-28 09:43:17.000000 browserist-1.5.1/src/browserist/model/browser/opera.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1125 2023-07-28 09:43:17.000000 browserist-1.5.1/src/browserist/model/browser/safari.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.454370 browserist-1.5.1/src/browserist/model/combo_settings/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/model/combo_settings/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1184 2022-12-11 22:32:17.000000 browserist-1.5.1/src/browserist/model/combo_settings/cookie_banner.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      289 2022-06-28 05:34:12.000000 browserist-1.5.1/src/browserist/model/combo_settings/login_credentials.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2770 2022-09-25 17:29:04.000000 browserist-1.5.1/src/browserist/model/combo_settings/login_form.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1105 2022-09-25 17:29:06.000000 browserist-1.5.1/src/browserist/model/combo_settings/search.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      987 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/model/driver_methods.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     3215 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/model/screenshot.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.492151 browserist-1.5.1/src/browserist/model/type/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-28 05:34:12.000000 browserist-1.5.1/src/browserist/model/type/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      507 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/model/type/callable.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      823 2022-09-23 21:13:58.000000 browserist-1.5.1/src/browserist/model/type/file_png.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      789 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/model/type/path.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      773 2022-06-28 05:34:12.000000 browserist-1.5.1/src/browserist/model/type/url.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      811 2022-10-26 03:09:24.000000 browserist-1.5.1/src/browserist/model/type/xpath.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.499013 browserist-1.5.1/src/browserist/model/viewport/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/model/viewport/__init__.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.508900 browserist-1.5.1/src/browserist/model/viewport/collection/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/model/viewport/collection/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1498 2023-07-31 00:31:29.000000 browserist-1.5.1/src/browserist/model/viewport/collection/apple.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      711 2023-07-31 00:31:29.000000 browserist-1.5.1/src/browserist/model/viewport/collection/google.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      683 2023-07-31 00:31:29.000000 browserist-1.5.1/src/browserist/model/viewport/collection/microsoft.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      781 2023-07-31 00:31:29.000000 browserist-1.5.1/src/browserist/model/viewport/collection/samsung.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      285 2022-10-24 03:28:03.000000 browserist-1.5.1/src/browserist/model/viewport/common_devices.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      208 2023-07-10 16:42:59.000000 browserist-1.5.1/src/browserist/model/viewport/device.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:07.515754 browserist-1.5.1/src/browserist/model/window/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       24 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/model/window/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     3231 2022-08-14 22:18:20.000000 browserist-1.5.1/src/browserist/model/window/controller.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      261 2022-06-28 05:34:12.000000 browserist-1.5.1/src/browserist/model/window/handle.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      212 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/model/window/tab_or_window.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        0 2022-06-10 19:03:49.000000 browserist-1.5.1/src/browserist/py.typed
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       80 2023-07-31 01:22:08.000000 browserist-1.5.1/src/browserist/version.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-07-31 01:28:06.188539 browserist-1.5.1/src/browserist.egg-info/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)    18731 2023-07-31 01:28:05.000000 browserist-1.5.1/src/browserist.egg-info/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)    11844 2023-07-31 01:28:06.000000 browserist-1.5.1/src/browserist.egg-info/SOURCES.txt
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        1 2023-07-31 01:28:05.000000 browserist-1.5.1/src/browserist.egg-info/dependency_links.txt
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        1 2022-05-07 22:12:45.000000 browserist-1.5.1/src/browserist.egg-info/not-zip-safe
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      169 2023-07-31 01:28:05.000000 browserist-1.5.1/src/browserist.egg-info/requires.txt
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       11 2023-07-31 01:28:05.000000 browserist-1.5.1/src/browserist.egg-info/top_level.txt
```

### Comparing `browserist-1.5.0/INSTALLATION.md` & `browserist-1.5.1/INSTALLATION.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.0&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
 ![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![Apache 2.0 license](https://img.shields.io/static/v1?label=license&message=Apache%202.0&color=blue)](https://github.com/jakob-bagterp/browserist/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1JL65T099J)](https://codecov.io/gh/jakob-bagterp/browserist)
+[![CodeQL](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml)
 [![Downloads](https://static.pepy.tech/badge/browserist)](https://pepy.tech/project/browserist)
 
 # 👩‍💻 How to Install Browserist 👨‍💻
 ## Prerequisites
 * Python 3.10 or higher
 * [Selenium](https://www.selenium.dev)
```

### Comparing `browserist-1.5.0/LICENSE.md` & `browserist-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/PKG-INFO` & `browserist-1.5.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserist
-Version: 1.5.0
+Version: 1.5.1
 Summary: Extension for the Selenium web driver that makes browser automation even easier
 Home-page: https://github.com/jakob-bagterp/browserist
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
 License: Apache-2.0
@@ -22,206 +22,111 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.0&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
 ![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![Apache 2.0 license](https://img.shields.io/static/v1?label=license&message=Apache%202.0&color=blue)](https://github.com/jakob-bagterp/browserist/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1JL65T099J)](https://codecov.io/gh/jakob-bagterp/browserist)
+[![CodeQL](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml)
 [![Downloads](https://static.pepy.tech/badge/browserist)](https://pepy.tech/project/browserist)
 
-# 👩‍💻 Browserist Extension for Selenium 👨‍💻
+# 👩‍💻 Browserist – Python Extension for Selenium 👨‍💻
 > **browserist**
 > 1. The belief that web browsers account for differences in websites or web applications in all of their ability and that a particular web browser is superior to others.
 > 2. Discrimination or prejudice based on web browser.
 
-Despite the [urban definition](https://www.urbandictionary.com/define.php?term=browserist), Browserist is a Python extension of the Selenium web driver that makes it even easier to use different browsers for testing and automation.
+Despite the [urban definition](https://www.urbandictionary.com/define.php?term=browserist), Browserist is a Python extension of the [Selenium web driver](https://www.selenium.dev/) that makes it even easier to use different browsers for testing and automation.
 
 Main features of Browserist:
 
 * Improves stability and speed
-* Simple syntax
-* Hassle-free setup that works across browsers: Chrome, Firefox, Edge, Safari, Opera, Internet Explorer
-* Extended library of browser automation functions and tools without elaborate code
-* Supports IntelliSense type hints and other capabilites of Python 3.10 that makes development more efficient
+* Simple syntax and less code
+* Hassle-free setup across browsers: Chrome, Firefox, Edge, Safari, Opera, Internet Explorer
+* Extensive framework of functions that makes browser automation easy
+* Supports IntelliSense and type hints that makes development more efficient
 
 ## How to Install
-Ready to try? [Learn how to install](https://github.com/jakob-bagterp/browserist/blob/master/INSTALLATION.md).
+Ready to try? With [PyPI](https://pypi.org/project/browserist/):
 
-## Getting Started
-The default browser is Chrome (except Edge for Windows). Simply type:
+```shell
+pip3 install browserist
+```
 
-```python
-from browserist import Browser
+Or with [Homebrew](https://brew.sh):
 
-browser = Browser()
-browser.open.url("http://example.com/")
-browser.quit()
+```shell
+brew tap jakob-bagterp/browserist
+brew install browserist
 ```
 
-Or use the built-in context manager so the browser automatically closes when done or if an error occurs:
+Find more installation details [here](https://jakob-bagterp.github.io/browserist/getting-started/installation/).
+
+## Getting Started
+You're now ready to go:
 
 ```python
 from browserist import Browser
 
 with Browser() as browser:
-    browser.open.url("http://example.com/")
-```
-
-### Browser Types
-If you want to use other browser types, e.g. Firefox, Edge, etc., define this in the settings:
-
-```python
-from browserist import Browser, BrowserSettings, BrowserType
-
-settings = BrowserSettings(type = BrowserType.FIREFOX)
-with Browser(settings) as browser:
-    browser.open.url("http://example.com/")
+    browser.open.url("https://example.com")
+    browser.wait.seconds(5)
 ```
 
-#### Supported Browsers
-| Name              | Type                            |
-| ----------------- | ------------------------------- |
-| Chrome            | `BrowserType.CHROME`            |
-| Edge              | `BrowserType.EDGE`              |
-| Firefox           | `BrowserType.FIREFOX`           |
-| Internet Explorer | `BrowserType.INTERNET_EXPLORER` |
-| Opera             | `BrowserType.OPERA`             |
-| Safari            | `BrowserType.SAFARI`            |
-
-### Navigation
-Similar to Selenium, use simple commands to automate the browser:
-
-| Action  | How                 | Description                        |
-| ------- | ------------------- | ---------------------------------- |
-| Forward | `browser.forward()` | Press the browser's back button    |
-| Back    | `browser.back()`    | Press the browser's forward button |
-| Refresh | `browser.refresh()` | Refresh the current page           |
-| Quit    | `browser.quit()`    | Close the browser                  |
-
 ## Improved Stability and Less Code
-Browserist improves stability with less code. As a browsers need time to render a page, especially single-page applications, Selenium is often used with explicit timeouts:
+Browserist improves stability with less code compared to standard use of Selenium. As a browsers need time to render a page, especially single-page applications, Selenium is often used with explicit timeouts:
 
 ```python
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 
 driver = webdriver.Chrome()
 
-driver.get("http://example.com/")
+driver.get("https://example.com")
 driver.implicitly_wait(3)
 search_box = driver.find_element(By.XPATH, "//xpath/to/input")
 search_button = driver.find_element(By.XPATH, "//xpath/to/button")
 search_box.send_keys("Lorem ipsum")
 search_button.click()
 driver.quit()
 ```
 
 Browserist does the same with less and cleaner code, yet also with increased stability and without explicit/implicit waits:
 
 ```python
 from browserist import Browser
 
 with Browser() as browser:
-    browser.open.url("http://example.com/")
+    browser.open.url("https://example.com")
     browser.input.value("//xpath/to/input", "Lorem ipsum")
     browser.click.button("//xpath/to/button")
 ```
 
-As you can't click a button that's not ready in the DOM, Browserist simply checks if elements are ready before interacting with them:
-
-| Timing:      | Too short ->  |     Just right     |  <- Too long   |
-| :----------- | :-----------: | :----------------: | :------------: |
-| Example:     | time.sleep(1) | wait.for_element() | time.sleep(10) |
-| Consequence: | _Code breaks_ | _Stable and fast_  |     _Slow_     |
-
-## Settings
-If you want a headless browser with Selenium, you typically would use different settings from browser to browser. Browserist solves this problem so that settings for Chrome, Firefox, Edge, etc. are standardised. For example, you can easily scale test runs across different browsers in a lightweight, headless configuration:
-
-```python
-from browserist import Browser, BrowserSettings, BrowserType
-
-chrome = BrowserSettings(type = BrowserType.CHROME, headless = True, disable_images = True)
-edge = BrowserSettings(type = BrowserType.EDGE, headless = True, disable_images = True)
-firefox = BrowserSettings(type = BrowserType.FIREFOX, headless = True, disable_images = True)
-
-for settings in [chrome, edge, firefox]:
-    with Browser(settings) as browser:
-        browser.open.url("http://example.com/")
-```
-
-Use `BrowserSettings` with the following options:
-
-| Setting              | Option                                    | Default                              | Description                                                                                                      |
-| -------------------- | ----------------------------------------- | ------------------------------------ | ---------------------------------------------------------------------------------------------------------------- |
-| `type`               | `BrowserType`                             | `BrowserType.CHROME`                 | Set browser type, e.g. Chrome, Edge, Firefox, etc.                                                               |
-| `headless`           | `True` or `False`                         | `False`                              | Run the browser in headless mode. May not be supported by all browsers.                                          |
-| `disable_images`     | `True` or `False`                         | `False`                              | Neither request nor render images, which typically improves loading speed. May not be supported by all browsers. |
-| `page_load_strategy` | `PageLoadStrategy`                        | `PageLoadStrategy.NORMAL`            | Set page load strategy.                                                                                          |
-| `path_to_executable` | Path to file                              | System default                       | If the browser executable isn't in a default folder, select which file to use.                                   |
-| `screenshot_dir`     | Path to directory                         | System default                       | Set where to save sreenshots. Default is the directory of Browserist.                                            |
-| `timeout`            | `TimeoutSettings`                         | `TimeoutStrategy.STOP` and 5 seconds | Set timeout strategy and time.                                                                                   |
-| `viewport`           | `DeviceViewportSize` or `(width, height)` | Browser default                      | Emulate viewport size as device or set custom value in pixels.                                                   |
-
-### Timeout Strategy
-What happens if a function times out: Should the browser stop or continue its operation?
-
-Define a general strategy and timeout in seconds:
-
-* Default is `5` seconds per function (note that a function-specific timeout overrides this)
-* The strategy can be `TimeoutStrategy.STOP` (default) or `TimeoutStrategy.CONTINUE`
-
-```python
-from browserist import Browser, BrowserSettings, TimeoutSettings, TimeoutStrategy
-
-timeout_settings = TimeoutSettings(strategy = TimeoutStrategy.CONTINUE, seconds = 10)
-settings = BrowserSettings(timeout = timeout_settings)
-
-with Browser(settings) as browser:
-    browser.open.url("http://example.com/")
-```
-
-#### Strategy Options
-| Option                     | Description                                                         |
-| -------------------------- | ------------------------------------------------------------------- |
-| `TimeoutStrategy.STOP`     | Default. Fail fast upon timeout and raise errors.                   |
-| `TimeoutStrategy.CONTINUE` | Continue despite timeouts and most errors (syntax errors excluded). |
-
-### Emulate Viewport of Common Devices
-You can set the viewport to emulate common device sizes or to a custom size. Note that it's recommended to run emulations in headless mode since an open browser may have minimum or maximum dimensions, either limited by the browser window or the monitor. Example:
-
-```python
-from browserist import Browser, BrowserSettings, common_devices
-
-settings = BrowserSettings(headless = True)
-
-with Browser(settings) as browser:
-    browser.viewport.set.size_by_device(common_devices.Apple.IPHONE_SE)
-    browser.open.url("http://example.com/")
-    browser.viewport.set.size(768, 1024)
-```
+## Documentation
+Find tutorials, code examples, list of all methods and much more [here](https://jakob-bagterp.github.io/browserist).
 
 # Thank You for Supporting
 ## Donate
-This module is free to use. And if you like it, feel free to [buy me a coffee](https://github.com/sponsors/jakob-bagterp).
+This module is free to use. And if you like it, feel free to [sponsor the project](https://github.com/sponsors/jakob-bagterp).
 
 ## Contribute
 If you have suggestions or changes to the module, feel free to add to the code and create a [pull request](https://github.com/jakob-bagterp/browserist/pulls).
 
 ## Report Bugs
 Report bugs and issues [here](https://github.com/jakob-bagterp/browserist/issues).
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.0&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
 ![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![Apache 2.0 license](https://img.shields.io/static/v1?label=license&message=Apache%202.0&color=blue)](https://github.com/jakob-bagterp/browserist/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1JL65T099J)](https://codecov.io/gh/jakob-bagterp/browserist)
+[![CodeQL](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml)
 [![Downloads](https://static.pepy.tech/badge/browserist)](https://pepy.tech/project/browserist)
 
 # 👩‍💻 How to Install Browserist 👨‍💻
 ## Prerequisites
 * Python 3.10 or higher
 * [Selenium](https://www.selenium.dev)
```

### Comparing `browserist-1.5.0/setup.cfg` & `browserist-1.5.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -29,34 +29,34 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
 setup_requires = 
-	lxml==4.9.2
-	pillow==9.5.0
+	lxml==4.9.3
+	pillow==10.0.0
 	selenium==4.10.0
 install_requires = 
 	chromedriver
-	lxml==4.9.2
-	pillow==9.5.0
+	lxml==4.9.3
+	pillow==10.0.0
 	selenium==4.10.0
 zip_safe = no
 include_package_data = True
 
 [options.extras_require]
 testing = 
 	coverage==7.2.7
 	flake8==6.0.0
-	keyring==23.13.1
-	mypy==1.3.0
-	pytest==7.3.2
+	keyring==24.2.0
+	mypy==1.4.1
+	pytest==7.4.0
 	pytest-cov==4.1.0
-	tox==4.6.0
+	tox==4.6.4
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 browserist = py.typed
```

### Comparing `browserist-1.5.0/src/browserist/__init__.py` & `browserist-1.5.1/src/browserist/__init__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/__main__.py` & `browserist-1.5.1/src/browserist/browser/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,26 @@
 class Browser:
     """Main class of Browserist that sets the Selenium web driver and contains all helper functions."""
 
     __slots__ = ["_browser_driver", "driver", "ie", "safari",
                  "check_if", "click", "combo", "get", "iframe", "input", "mouse", "open", "prompt", "screenshot", "scroll", "select", "tool", "viewport", "wait", "window"]
 
     def __init__(self, settings: BrowserSettings | None = None) -> None:
-        """Initiates the browser driver whether the settings call for Chrome, Firefox, etc."""
+        """Initiates the browser driver whether the settings call for Chrome, Edge, Firefox, etc.
+
+        Example:
+            ```python title=""
+            from browserist import Browser, BrowserSettings
+
+            settings = BrowserSettings(browser_type=BrowserType.FIREFOX)
+
+            with Browser(settings) as browser:
+                browser.open.url("https://example.com")
+            ```
+        """
 
         if settings is None:
             settings = BrowserSettings()  # Use default settings if no custom settings are given.
 
         self._browser_driver: BrowserDriver = factory.get.browser_driver(settings)
         self.driver: object = self._browser_driver.get_webdriver()
```

### Comparing `browserist-1.5.0/src/browserist/browser/check_if/contains_text.py` & `browserist-1.5.1/src/browserist/browser/check_if/contains_text.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/check_if/is_in_viewport.py` & `browserist-1.5.1/src/browserist/browser/check_if/is_in_viewport.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/click/button.py` & `browserist-1.5.1/src/browserist/browser/click/button.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/click/button_if_contains_text.py` & `browserist-1.5.1/src/browserist/browser/click/button_if_contains_text.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/combo/cookie_banner.py` & `browserist-1.5.1/src/browserist/browser/combo/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/combo/log_in.py` & `browserist-1.5.1/src/browserist/browser/combo/log_in.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/combo/search.py` & `browserist-1.5.1/src/browserist/browser/combo/search.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/get/attribute/values.py` & `browserist-1.5.1/src/browserist/browser/get/attribute/values.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/get/dimensions.py` & `browserist-1.5.1/src/browserist/browser/get/dimensions.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/get/element.py` & `browserist-1.5.1/src/browserist/browser/get/element.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/get/elements.py` & `browserist-1.5.1/src/browserist/browser/get/elements.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/get/text.py` & `browserist-1.5.1/src/browserist/browser/get/text.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/get/url/__main__.py` & `browserist-1.5.1/src/browserist/browser/get/url/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,49 +9,91 @@
 
 
 class GetUrlDriverMethods(DriverMethods):
     def __init__(self, browser_driver: BrowserDriver) -> None:
         super().__init__(browser_driver)
 
     def current(self) -> str:  # type: ignore
-        """Get URL of the current page."""
+        """Get URL of the current page, e.g. `https://example.com`.
+
+        Returns:
+            str: URL of the current page, e.g. `https://example.com`.
+        """
 
         if self._timeout_should_continue():
             return get_current_url(self._browser_driver)
 
     def current_domain(self) -> str:  # type: ignore
-        """Get domain of the current page, e.g. www.example.com."""
+        """Get domain of the current page, e.g. `example.com`.
+
+        Returns:
+            str: Domain of the current page, e.g. `example.com`.
+        """
 
         if self._timeout_should_continue():
             return get_current_domain(self._browser_driver)
 
     def from_image(self, xpath: str, timeout: float | None = None) -> str:  # type: ignore
-        """Get URL source from image, e.g. <img> tag.
+        """Get URL source from image, i.e. `<img>` tag.
+
+        Note:
+            This method assumes that the image isn't empty and therefore will retry to get the URL (for better support of single-page apps with extended loading time).
 
-        This method assumes that the image shouldn't be empty and therefore will retry to get the URL (for better support of single-page apps with extended loading time)."""
+        Args:
+            xpath (str): XPath of the image. Should target an `<img>` tag.
+            timeout (float | None, optional): In seconds. Timeout to wait for element. If `None`, the global timeout setting is used (default 5 seconds).
+
+        Returns:
+            str: URL source of the image.
+        """
 
         if self._timeout_should_continue():
             timeout = self._mediate_timeout(timeout)
             return get_url_from_image(self._browser_driver, xpath, timeout)
 
     def from_images(self, xpath: str, timeout: float | None = None) -> list[str]:  # type: ignore
-        """Get array of URLs from images, e.g. <img> tags. Assumes that the XPath targets multiple images."""
+        """Get list of URLs from images, i.e. `<img>` tags. Assumes that the XPath targets multiple images.
+
+        Args:
+            xpath (str): XPath of the images. Should target `<img>` tags.
+            timeout (float | None, optional): In seconds. Timeout to wait for element. If `None`, the global timeout setting is used (default 5 seconds).
+
+        Returns:
+            list[str]: List of image URLs.
+        """
 
         if self._timeout_should_continue():
             timeout = self._mediate_timeout(timeout)
             return get_url_from_images(self._browser_driver, xpath, timeout)
 
     def from_link(self, xpath: str, timeout: float | None = None) -> str:  # type: ignore
-        """Get URL from link, e.g. <a> tag or button.
+        """Get URL from link or button, i.e. `<a>` tag.
+
+        Note:
+            This method assumes that the link isn't empty and therefore will retry to get the URL (for better support of single-page apps with extended loading time).
 
-        This method assumes that the link shouldn't be empty and therefore will retry to get the URL (for better support of single-page apps with extended loading time)."""
+        Args:
+            xpath (str): XPath of the link. Should target an `<a>` tag.
+            timeout (float | None, optional): In seconds. Timeout to wait for element. If `None`, the global timeout setting is used (default 5 seconds).
+
+        Returns:
+            str: URL of the link.
+        """
 
         if self._timeout_should_continue():
             timeout = self._mediate_timeout(timeout)
             return get_url_from_link(self._browser_driver, xpath, timeout)
 
     def from_links(self, xpath: str, timeout: float | None = None) -> list[str]:  # type: ignore
-        """Get array of URLs from links, e.g. <a> tags or buttons. Assumes that the XPath targets multiple links."""
+        """Get array of URLs from links or buttons, i.e. `<a>` tags. Assumes that the XPath targets multiple links.
+
+        Args:
+            xpath (str): XPath of the links. Should target `<a>` tags.
+            timeout (float | None, optional): In seconds. Timeout to wait for element. If `None`, the global timeout setting is used (default 5 seconds).
+
+        Returns:
+            list[str]: List of link URLs.
+        """
 
         if self._timeout_should_continue():
             timeout = self._mediate_timeout(timeout)
             return get_url_from_links(self._browser_driver, xpath, timeout)
```

### Comparing `browserist-1.5.0/src/browserist/browser/get/url/from_image.py` & `browserist-1.5.1/src/browserist/browser/get/url/from_image.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/get/url/from_link.py` & `browserist-1.5.1/src/browserist/browser/get/url/from_link.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/iframe/__main__.py` & `browserist-1.5.1/src/browserist/browser/iframe/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,18 +5,23 @@
 
 
 class IframeDriverMethods(DriverMethods):
     def __init__(self, browser_driver: BrowserDriver) -> None:
         super().__init__(browser_driver)
 
     def switch_to(self, xpath: str, timeout: float | None = None) -> None:
-        """Switch to iframe."""
+        """Switch to iframe.
+
+        Args:
+            xpath (str): XPath of the iframe.
+            timeout (float | None, optional): In seconds. Timeout to wait for element. If `None`, the global timeout setting is used (default 5 seconds).
+        """
 
         if self._timeout_should_continue():
             timeout = self._mediate_timeout(timeout)
             switch_to_iframe(self._browser_driver, xpath, timeout)
 
     def switch_to_original_page(self) -> None:
-        """After switch to iframe, use this to go back to the original page."""
+        """After switch to iframe, use this to come back to the original page."""
 
         if self._timeout_should_continue():
             switch_to_original_page(self._browser_driver)
```

### Comparing `browserist-1.5.0/src/browserist/browser/iframe/switch_to.py` & `browserist-1.5.1/src/browserist/browser/iframe/switch_to.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/input/value.py` & `browserist-1.5.1/src/browserist/browser/input/value.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/mouse/__main__.py` & `browserist-1.5.1/src/browserist/model/driver_methods.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,26 @@
-from ...model.browser.base.driver import BrowserDriver
-from ...model.driver_methods import DriverMethods
-from .hover import mouse_hover
+from .. import helper
+from .browser.base.driver import BrowserDriver
 
 
-class MouseDriverMethods(DriverMethods):
+class DriverMethods:
+    """Super class with initializer that can be extended in sub classes for web driver methods."""
+
+    __slots__ = ["_browser_driver"]
+
     def __init__(self, browser_driver: BrowserDriver) -> None:
-        super().__init__(browser_driver)
+        self._browser_driver: BrowserDriver = browser_driver
+
+    def _timeout_should_continue(self) -> bool:
+        """Controller for timeout strategy for each relevant browser method."""
+
+        return helper.timeout.should_continue(self._browser_driver.settings)
+
+    def _mediate_timeout(self, timeout: float | None) -> float:
+        """Mediate whether timeout seconds should use a global or a local setting."""
+
+        return helper.timeout.mediate_timeout(self._browser_driver.settings, timeout)
 
-    def hover(self, xpath: str, timeout: float | None = None) -> None:
-        """Simulate moving the mouse cursor over the middle of an element."""
+    def _set_is_timed_out(self) -> None:
+        """Sets global timeout to true."""
 
-        if self._timeout_should_continue():
-            timeout = self._mediate_timeout(timeout)
-            mouse_hover(self._browser_driver, xpath, timeout)
+        self._browser_driver.settings = helper.timeout.set_is_timed_out(self._browser_driver.settings)
```

### Comparing `browserist-1.5.0/src/browserist/browser/mouse/hover.py` & `browserist-1.5.1/src/browserist/browser/mouse/hover.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/open/url_if_not_current.py` & `browserist-1.5.1/src/browserist/browser/open/url_if_not_current.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/prompt/__main__.py` & `browserist-1.5.1/src/browserist/browser/mouse/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from ...model.browser.base.driver import BrowserDriver
 from ...model.driver_methods import DriverMethods
-from .input_value import prompt_and_input_value
-from .proceed_yes_or_no import prompt_proceed_yes_or_no
+from .hover import mouse_hover
 
 
-class PromptDriverMethods(DriverMethods):
+class MouseDriverMethods(DriverMethods):
     def __init__(self, browser_driver: BrowserDriver) -> None:
         super().__init__(browser_driver)
 
-    def input_value(self, xpath: str, prompt_message: str, validate_input_regex: str | None = None, timeout: float | None = None) -> None:
-        """Prompt user for value through the terminal and insert this value into form field. Optional to validate input by regex."""
+    def hover(self, xpath: str, timeout: float | None = None) -> None:
+        """Simulate moving the mouse cursor over the middle of an element.
 
-        if self._timeout_should_continue():
-            timeout = self._mediate_timeout(timeout)
-            prompt_and_input_value(self._browser_driver, xpath, prompt_message, validate_input_regex, timeout)
-
-    def proceed_yes_or_no(self) -> bool:
-        """Prompt user whether to proceed or not through the terminal."""
+        Args:
+            xpath (str): XPath of the element.
+            timeout (float | None, optional): In seconds. Timeout to wait for element. If `None`, the global timeout setting is used (default 5 seconds).
+        """
 
         if self._timeout_should_continue():
-            return prompt_proceed_yes_or_no()
-        else:
-            return False
+            timeout = self._mediate_timeout(timeout)
+            mouse_hover(self._browser_driver, xpath, timeout)
```

### Comparing `browserist-1.5.0/src/browserist/browser/prompt/proceed_yes_or_no.py` & `browserist-1.5.1/src/browserist/browser/prompt/proceed_yes_or_no.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/screenshot/complete_page.py` & `browserist-1.5.1/src/browserist/browser/screenshot/complete_page.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/screenshot/element.py` & `browserist-1.5.1/src/browserist/browser/screenshot/element.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/screenshot/visible_portion.py` & `browserist-1.5.1/src/browserist/browser/screenshot/visible_portion.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/scroll/check_if/__main__.py` & `browserist-1.5.1/src/browserist/browser/scroll/check_if/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,17 +5,25 @@
 
 
 class ScrollCheckIfDriverMethods(DriverMethods):
     def __init__(self, browser_driver: BrowserDriver) -> None:
         super().__init__(browser_driver)
 
     def is_end_of_page(self) -> bool:  # type: ignore
-        """Check if current scroll position is at the end of the page."""
+        """Check if current scroll position is at the end of the page.
+
+        Returns:
+            bool: `True` if current scroll position is at the end of the page, `False` otherwise.
+        """
 
         if self._timeout_should_continue():
             return check_if_scroll_is_end_of_page(self._browser_driver)
 
     def is_top_of_page(self) -> bool:  # type: ignore
-        """Check if current scroll position is at the top of the page."""
+        """Check if current scroll position is at the top of the page.
+
+        Returns:
+            bool: `True` if current scroll position is at the top of the page, `False` otherwise.
+        """
 
         if self._timeout_should_continue():
             return check_if_scroll_is_top_of_page(self._browser_driver)
```

### Comparing `browserist-1.5.0/src/browserist/browser/scroll/check_if/is_end_of_page.py` & `browserist-1.5.1/src/browserist/browser/scroll/check_if/is_end_of_page.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/scroll/get/total_height.py` & `browserist-1.5.1/src/browserist/browser/scroll/get/total_height.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/scroll/into_view.py` & `browserist-1.5.1/src/browserist/browser/scroll/into_view.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/scroll/page/__main__.py` & `browserist-1.5.1/src/browserist/browser/scroll/page/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,29 +7,45 @@
 
 
 class ScrollPageDriverMethods(DriverMethods):
     def __init__(self, browser_driver: BrowserDriver) -> None:
         super().__init__(browser_driver)
 
     def down(self, delay_seconds: float = 1) -> None:
-        """If possible, scroll page down. Add custom delay in seconds to ensure the view is updated after scroll."""
+        """If possible, scroll page down.
+
+        Args:
+            delay_seconds (float, optional): Option to add custom delay in seconds to ensure the view is updated after scroll.
+        """
 
         if self._timeout_should_continue():
             scroll_page_down(self._browser_driver, delay_seconds)
 
     def to_end(self, delay_seconds: float = 1) -> None:
-        """If possible, scroll to end of page. Add custom delay in seconds to ensure the view is updated after scroll."""
+        """If possible, scroll to end of page.
+
+        Args:
+            delay_seconds (float, optional): Option to add custom delay in seconds to ensure the view is updated after scroll.
+        """
 
         if self._timeout_should_continue():
             scroll_to_end_of_page(self._browser_driver, delay_seconds)
 
     def to_top(self, delay_seconds: float = 1) -> None:
-        """If possible, scroll to top of page. Add custom delay in seconds to ensure the view is updated after scroll."""
+        """If possible, scroll to top of page.
+
+        Args:
+            delay_seconds (float, optional): Option to add custom delay in seconds to ensure the view is updated after scroll.
+        """
 
         if self._timeout_should_continue():
             scroll_to_top_of_page(self._browser_driver, delay_seconds)
 
     def up(self, delay_seconds: float = 1) -> None:
-        """If possible, scroll page up. Add custom delay in seconds to ensure the view is updated after scroll."""
+        """If possible, scroll page up.
+
+        Args:
+            delay_seconds (float, optional): Option to add custom delay in seconds to ensure the view is updated after scroll.
+        """
 
         if self._timeout_should_continue():
             scroll_page_up(self._browser_driver, delay_seconds)
```

### Comparing `browserist-1.5.0/src/browserist/browser/scroll/page/to_end.py` & `browserist-1.5.1/src/browserist/browser/scroll/page/to_end.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/viewport/__main__.py` & `browserist-1.5.1/src/browserist/browser/viewport/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/viewport/get/__main__.py` & `browserist-1.5.1/src/browserist/browser/viewport/get/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,25 +6,40 @@
 
 
 class ViewportGetDriverMethods(DriverMethods):
     def __init__(self, browser_driver: BrowserDriver) -> None:
         super().__init__(browser_driver)
 
     def height(self) -> int:  # type: ignore
-        """Get height of the viewport in pixels."""
+        """Get height of the viewport in pixels.
+
+        Returns:
+            int: Height of the viewport in pixels.
+        """
 
         if self._timeout_should_continue():
             return get_viewport_height(self._browser_driver)
 
     def size(self) -> tuple[int, int]:  # type: ignore
-        """Get width and height of the viewport in pixels. Usage:
+        """Get width and height of the viewport in pixels.
+
+        Returns:
+            tuple[int, int]: Width and height of the viewport in pixels.
 
-        width, height = browser.viewport.get.size()"""
+        Example:
+            ```python title=""
+            width, height = browser.viewport.get.size()
+            ```
+        """
 
         if self._timeout_should_continue():
             return get_viewport_size(self._browser_driver)
 
     def width(self) -> int:  # type: ignore
-        """Get width of the viewport in pixels."""
+        """Get width of the viewport in pixels.
+
+        Returns:
+            int: Width of the viewport in pixels.
+        """
 
         if self._timeout_should_continue():
             return get_viewport_width(self._browser_driver)
```

### Comparing `browserist-1.5.0/src/browserist/browser/viewport/set/__main__.py` & `browserist-1.5.1/src/browserist/browser/viewport/set/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,39 @@
 class ViewportSetDriverMethods(DriverMethods):
     def __init__(self, browser_driver: BrowserDriver) -> None:
         super().__init__(browser_driver)
 
     def size(self, width: int, height: int) -> None:
         """Attempt to set custom viewport size in pixels.
 
-        Note that it's recommended to run emulations in headless mode since an open browser may have minimum or maximum dimensions, either limited by the browser window or the monitor."""
+        Note:
+            It's recommended to run emulations in headless mode since an open browser may have minimum or maximum dimensions, either limited by the browser window or the monitor.
+
+        Args:
+            width (int): Viewport width in pixels.
+            height (int): Viewport height in pixels.
+        """
 
         if self._timeout_should_continue():
             return set_viewport_size(self._browser_driver, width, height)
 
     def size_by_device(self, device: DeviceViewportSize) -> None:
         """Attempt to set the viewport size by device types, e.g. iPhone, iPad, or other common devices.
 
-        Note that it's recommended to run emulations in headless mode since an open browser may have minimum or maximum dimensions, either limited by the browser window or the monitor."""
+        Note:
+            It's recommended to run emulations in headless mode since an open browser may have minimum or maximum dimensions, either limited by the browser window or the monitor.
+
+        Args:
+            device (DeviceViewportSize): Device type to emulate.
+
+        Example:
+            ```python title=""
+            from browserist import Browser, DeviceViewportSize
+
+            browser = Browser()
+            custom_device = DeviceViewportSize(width=375, height=812)
+            browser.viewport.set.size_by_device(custom_device)
+            ```
+        """
 
         if self._timeout_should_continue():
             return set_viewport_size_by_device(self._browser_driver, device)
```

### Comparing `browserist-1.5.0/src/browserist/browser/viewport/set/size.py` & `browserist-1.5.1/src/browserist/browser/viewport/set/size.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/wait/__main__.py` & `browserist-1.5.1/src/browserist/browser/wait/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,24 +12,47 @@
     def __init__(self, browser_driver: BrowserDriver) -> None:
         super().__init__(browser_driver)
         self.until: WaitUntilDriverMethods = WaitUntilDriverMethods(browser_driver)
 
     def for_element(self, xpath: str, timeout: float | None = None) -> None:
         """Wait until element is ready in the DOM and/or on the screen.
 
-        Especially useful for single-page app elements handled/modified by JavaScript, but also standard HTML that doesn't load immediately, this helper function ensures that DOM elements are ready before processing."""
+        Args:
+            xpath (str): XPath of the element.
+            timeout (float | None, optional): In seconds. Timeout to wait for element. If `None`, the global timeout setting is used (default 5 seconds).
+
+        Example:
+            Useful for single-page app elements handled by JavaScript, but also standard HTML that doesn't load immediately. This helper function ensures that DOM elements are ready before processing. The example waits for any H1 headline to be ready:
+
+            ```python title=""
+            from browserist import Browser
+
+            browser = Browser()
+            browser.open.url("https://example.com")
+            browser.wait.for_element("//h1")
+            ```
+        """
 
         if self._timeout_should_continue():
             timeout = self._mediate_timeout(timeout)
             wait_for_element(self._browser_driver, xpath, timeout)
 
     def random_seconds(self, min_seconds: float = 1, max_seconds: float = 5) -> None:
-        """Randomize sleep timing to make actions look less like a bot."""
+        """Sleep for a random amount of time to make actions look less like a bot. The waiting time will be somewhere between the speficied minimum and maximum seconds.
+
+        Args:
+            min_seconds (float, optional): Minimum seconds to wait.
+            max_seconds (float, optional): Maximum seconds to wait.
+        """
 
         if self._timeout_should_continue():
             wait_random_seconds(min_seconds, max_seconds)
 
     def seconds(self, seconds: float) -> None:
-        """Sleep for a fixed amount of time."""
+        """Sleep for a fixed amount of time.
+
+        Args:
+            seconds (float): Seconds to wait.
+        """
 
         if self._timeout_should_continue():
             wait_seconds(seconds)
```

### Comparing `browserist-1.5.0/src/browserist/browser/wait/for_element.py` & `browserist-1.5.1/src/browserist/browser/wait/for_element.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/wait/until/images_have_loaded.py` & `browserist-1.5.1/src/browserist/browser/wait/until/images_have_loaded.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/wait/until/number_of_window_handles_is.py` & `browserist-1.5.1/src/browserist/browser/wait/until/number_of_window_handles_is.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/wait/until/page_title/__main__.py` & `browserist-1.5.1/src/browserist/browser/wait/until/page_title/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,26 +6,41 @@
 
 
 class WaitUntilPageTitleDriverMethods(DriverMethods):
     def __init__(self, browser_driver: BrowserDriver) -> None:
         super().__init__(browser_driver)
 
     def changes(self, baseline_text: str, timeout: float | None = None) -> None:
-        """Wait until the page title changes from a baseline text, e.g. after a page reload or change. The text is evaluated as an exact match."""
+        """Wait until the page title changes compared to a baseline text, e.g. after a page reload or update.
+
+        Args:
+            baseline_text (str): Baseline text to compare current page title against. It's evaluated as any change.
+            timeout (float | None, optional): In seconds. Timeout to wait for page title to change. If `None`, the global timeout setting is used (default 5 seconds).
+        """
 
         if self._timeout_should_continue():
             timeout = self._mediate_timeout(timeout)
             wait_until_page_title_changes(self._browser_driver, baseline_text, timeout)
 
     def contains(self, page_title_fragment: str, timeout: float | None = None) -> None:
-        """Wait until the page title has changed, e.g. after a redirect or update. The input can contain both a fragment or the full page title."""
+        """Wait until the page title contains a specified text fragment, e.g. after a redirect or update.
+
+        Args:
+            page_title_fragment (str): The input can contain both a fragment or the full page title.
+            timeout (float | None, optional): In seconds. Timeout to wait for page title to contain text fragment. If `None`, the global timeout setting is used (default 5 seconds).
+        """
 
         if self._timeout_should_continue():
             timeout = self._mediate_timeout(timeout)
             wait_until_page_title_contains(self._browser_driver, page_title_fragment, timeout)
 
     def equals(self, page_title: str, timeout: float | None = None) -> None:
-        """Wait until the page title has changed, e.g. after a redirect or update. The input has to match the exact page title."""
+        """Wait until the page title has changed to a specific text, e.g. after a redirect or update.
+
+        Args:
+            page_title (str): Full page title to compare the new current page title against. Evaluated as an exact match.
+            timeout (float | None, optional): In seconds. Timeout to wait for page title to match specified text. If `None`, the global timeout setting is used (default 5 seconds).
+        """
 
         if self._timeout_should_continue():
             timeout = self._mediate_timeout(timeout)
             wait_until_page_title_equals(self._browser_driver, page_title, timeout)
```

### Comparing `browserist-1.5.0/src/browserist/browser/wait/until/page_title/changes.py` & `browserist-1.5.1/src/browserist/browser/wait/until/page_title/changes.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/wait/until/page_title/contains.py` & `browserist-1.5.1/src/browserist/browser/wait/until/page_title/contains.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/wait/until/page_title/equals.py` & `browserist-1.5.1/src/browserist/browser/wait/until/page_title/equals.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/wait/until/text/__main__.py` & `browserist-1.5.1/src/browserist/browser/click/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-from .....model.browser.base.driver import BrowserDriver
-from .....model.driver_methods import DriverMethods
-from .changes import wait_until_text_changes
-from .contains import wait_until_text_contains
-from .equals import wait_until_text_equals
+from ...model.browser.base.driver import BrowserDriver
+from ...model.driver_methods import DriverMethods
+from .button import click_button
+from .button_if_contains_text import click_button_if_contains_text
 
 
-class WaitUntilTextDriverMethods(DriverMethods):
+class ClickDriverMethods(DriverMethods):
     def __init__(self, browser_driver: BrowserDriver) -> None:
         super().__init__(browser_driver)
 
-    def changes(self, xpath: str, baseline_text: str, timeout: float | None = None) -> None:
-        """Wait until the text of an element changes from a baseline text, e.g. after a form action. The text is evaluated as an exact match."""
+    def button(self, xpath: str, timeout: float | None = None) -> None:
+        """Click button.
 
-        if self._timeout_should_continue():
-            timeout = self._mediate_timeout(timeout)
-            wait_until_text_changes(self._browser_driver, xpath, baseline_text, timeout)
-
-    def contains(self, xpath: str, regex: str, timeout: float | None = None) -> None:
-        """Wait until the text of an element has changed, e.g. after a form action."""
+        Args:
+            xpath (str): XPath of the button element.
+            timeout (float | None, optional): In seconds. Timeout to wait for element. If `None`, the global timeout setting is used (default 5 seconds).
+        """
 
         if self._timeout_should_continue():
             timeout = self._mediate_timeout(timeout)
-            wait_until_text_contains(self._browser_driver, xpath, regex, timeout)
+            click_button(self._browser_driver, xpath, timeout)
+
+    def button_if_contains_text(self, xpath: str, regex: str, ignore_case: bool = True, timeout: float | None = None) -> None:
+        """Click button if it contains certain text.
 
-    def equals(self, xpath: str, regex: str, timeout: float | None = None) -> None:
-        """Wait until the text of an element has changed, e.g. after a form action. The text is evaluated as an exact match."""
+        Args:
+            xpath (str): XPath of the button element.
+            regex (str): Regular expression or text to search for. The condition works for both ordinary text (e.g. `"Submit"`) or regular expression (e.g. `r"colou?r"`). Note it's a search for text, not a strict text match.
+            ignore_case (bool, optional): Ignore case when searching for text.
+            timeout (float | None, optional): In seconds. Timeout to wait for element. If `None`, the global timeout setting is used (default 5 seconds).
+        """
 
         if self._timeout_should_continue():
             timeout = self._mediate_timeout(timeout)
-            wait_until_text_equals(self._browser_driver, xpath, regex, timeout)
+            click_button_if_contains_text(self._browser_driver, xpath, regex, ignore_case, timeout)
```

### Comparing `browserist-1.5.0/src/browserist/browser/wait/until/text/changes.py` & `browserist-1.5.1/src/browserist/browser/wait/until/text/changes.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/wait/until/text/contains.py` & `browserist-1.5.1/src/browserist/browser/wait/until/text/contains.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/wait/until/text/equals.py` & `browserist-1.5.1/src/browserist/browser/wait/until/text/equals.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/wait/until/url/changes.py` & `browserist-1.5.1/src/browserist/browser/wait/until/url/changes.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/wait/until/url/contains.py` & `browserist-1.5.1/src/browserist/browser/wait/until/url/contains.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/wait/until/url/equals.py` & `browserist-1.5.1/src/browserist/browser/wait/until/url/equals.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/window/__main__.py` & `browserist-1.5.1/src/browserist/browser/window/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,36 +26,62 @@
     def close(self) -> None:
         """Close current tab or window."""
 
         if self._timeout_should_continue():
             window_close(self._browser_driver, self._controller)
 
     def fullscreen(self) -> None:
-        """Fills the entire screen, similar to pressing F11 in most browsers."""
+        """Fills the entire screen. Similar to pressing F11 in most browsers."""
 
         if self._timeout_should_continue():
             window_fullscreen(self._browser_driver)
 
     def maximize(self) -> None:
-        """Enlarges the window. For most operating systems, the window will fill the screen, without blocking the operating system's own menus and toolbars."""
+        """Enlarge the browser window to maximum allowed size.
+
+        Note:
+            For most operating systems, the window will fill the screen, without blocking the operating system's own menus and toolbars. Obviously, the size of the browser window also depends on the device and its screen resolution.
+        """
 
         if self._timeout_should_continue():
             window_maximize(self._browser_driver)
 
     def minimize(self) -> None:
-        """Minimizes the window of current browsing context. The exact behavior of this command is specific to individual window managers. Minimize Window typically hides the window in the system tray."""
+        """Minimizes the window of current browsing context.
+
+        Note:
+            The exact behavior of this command is specific to individual window managers. Minimize Window typically hides the window in the system tray.
+        """
 
         if self._timeout_should_continue():
             window_minimize(self._browser_driver)
 
     def switch_to(self, window_handle: str) -> None:
-        """Switch to window/tab by handle ID or name."""
+        """Switch to window/tab by handle ID or name.
+
+        Args:
+            window_handle (str): Handle ID or name of window/tab to switch to.
+
+        Example:
+            ```python title=""
+            from browserist import Browser
+
+            with Browser() as browser:
+                browser.window.open.new_tab("https://example.com", "tab_1")
+                browser.window.open.new_tab("https://www.google.com", "tab_2")
+                browser.window.switch_to("tab_1")
+            ```
+        """
 
         if self._timeout_should_continue():
             switch_to_window(self._browser_driver, self._controller, window_handle)
 
     def switch_to_original_window(self) -> None:
-        """Switch to initial window/tab."""
+        """Switch to initial window/tab.
+
+        Note:
+            Browserist automatically remembers the handle ID of the initial window/tab when the browser is first opened.
+        """
 
         if self._timeout_should_continue():
             original_window_handle_id = self._controller.get_handle_id_by_name(self._controller._original_window_name)
             switch_to_window(self._browser_driver, self._controller, original_window_handle_id)
```

### Comparing `browserist-1.5.0/src/browserist/browser/window/handle/__main__.py` & `browserist-1.5.1/src/browserist/browser/window/handle/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,27 +12,39 @@
     def __init__(self, browser_driver: BrowserDriver, controller: WindowHandleController) -> None:
         super().__init__(browser_driver)
         self._controller = controller
 
     def all(self, selenium: bool = False) -> list[str]:  # type: ignore
         """Get list of IDs of all open tabs or windows.
 
-        selenium: Set to "True" if you want the Selenium handle IDs rather than from the internal window handle controller."""
+        Args:
+            selenium (bool, optional): Set to `True` if you want the Selenium handle IDs rather than from Browserist's internal window handle controller.
+
+        Returns:
+            list[str]: List of IDs of all open tabs or windows.
+        """
 
         if self._timeout_should_continue():
             return get_all_window_handles(self._browser_driver, self._controller, selenium)
 
     def count(self, selenium: bool = False) -> int:  # type: ignore
         """Count number of open tabs or windows.
 
-        selenium: Set to "True" if you want the number of Selenium handle IDs rather than from the internal window handle controller."""
+        Args:
+            selenium (bool, optional): Set to `True` if you want the Selenium handle IDs rather than from Browserist's internal window handle controller.
+
+        Returns:
+            int: Number of open tabs or windows.
+        """
 
         if self._timeout_should_continue():
             return count_window_handles(self._browser_driver, self._controller, selenium)
 
     def current(self) -> str:  # type: ignore
         """Get the ID of the current tab or window.
 
-        Example: CDwindow-69663F4BF867CC38F6AF46D55BFC1A8A"""
+        Returns:
+            str: ID of the current tab or window. e.g. `CDwindow-69663F4BF867CC38F6AF46D55BFC1A8A`.
+        """
 
         if self._timeout_should_continue():
             return get_current_window_handle(self._browser_driver)
```

### Comparing `browserist-1.5.0/src/browserist/browser/window/open/new_tab_or_window.py` & `browserist-1.5.1/src/browserist/browser/window/open/new_tab_or_window.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/browser/window/set/__main__.py` & `browserist-1.5.1/src/browserist/browser/scroll/get/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 from ....model.browser.base.driver import BrowserDriver
 from ....model.driver_methods import DriverMethods
-from .position import set_window_position
-from .size import set_window_size
+from .position import get_scroll_position
+from .total_height import get_total_scroll_height
 
 
-class WindowSetDriverMethods(DriverMethods):
+class ScrollGetDriverMethods(DriverMethods):
     def __init__(self, browser_driver: BrowserDriver) -> None:
         super().__init__(browser_driver)
 
-    def position(self, x: int, y: int) -> None:
-        """Moves the window to the chosen coordinate of the screen in pixels."""
+    def position(self) -> tuple[int, int]:  # type: ignore
+        """Get scroll position of the X and Y axis.
+
+        Returns:
+            tuple[int, int]: Scroll position of the X and Y axis. In pixels.
+
+        Example:
+            ```python title=""
+            x, y = browser.scroll.get.position()
+            ```
+        """
 
         if self._timeout_should_continue():
-            set_window_position(self._browser_driver, x, y)
+            return get_scroll_position(self._browser_driver)
+
+    def total_height(self) -> int:  # type: ignore
+        """Get total scroll height.
 
-    def size(self, width: int, height: int) -> None:
-        """Restores the window and sets the window size."""
+        Returns:
+            int: Total scroll height.
+        """
 
         if self._timeout_should_continue():
-            set_window_size(self._browser_driver, width, height)
+            return get_total_scroll_height(self._browser_driver)
```

### Comparing `browserist-1.5.0/src/browserist/browser/window/switch_to.py` & `browserist-1.5.1/src/browserist/browser/window/switch_to.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/exception/element.py` & `browserist-1.5.1/src/browserist/exception/element.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/exception/headless.py` & `browserist-1.5.1/src/browserist/exception/headless.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/exception/timeout.py` & `browserist-1.5.1/src/browserist/exception/timeout.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/exception/window_handle.py` & `browserist-1.5.1/src/browserist/exception/window_handle.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/factory/chromium.py` & `browserist-1.5.1/src/browserist/factory/chromium.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/factory/get.py` & `browserist-1.5.1/src/browserist/factory/get.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/factory/internet_explorer.py` & `browserist-1.5.1/src/browserist/factory/internet_explorer.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/factory/safari.py` & `browserist-1.5.1/src/browserist/factory/safari.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/factory/set.py` & `browserist-1.5.1/src/browserist/factory/set.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/helper/directory.py` & `browserist-1.5.1/src/browserist/helper/directory.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/helper/image.py` & `browserist-1.5.1/src/browserist/helper/image.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/helper/timeout.py` & `browserist-1.5.1/src/browserist/helper/timeout.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/helper/url.py` & `browserist-1.5.1/src/browserist/helper/url.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from urllib.parse import urlparse
 
 from ..model.type.url import URL
 
 
 def ensure_trailing_slash(url: str) -> str:
-    """When comparing URLs, e.g. "http://example.com/" and "http://example.com", use this method to normalise the comparison."""
+    """When comparing URLs, e.g. "https://example.com" and "https://example.com/", use this method to normalise the comparison."""
 
-    if "?" in url:  # If the URL contains a parameter (e.g. https://example.com/search?page=1), ignore trailing slash.
+    if "?" in url:  # If the URL contains a parameter (e.g. "https://example.com/search?page=1"), ignore trailing slash.
         return url
     return url if url[-1] == "/" else f"{url}/"
 
 
 def is_https(url: str) -> bool:
     return url.startswith("https:")
```

### Comparing `browserist-1.5.0/src/browserist/helper/window_handle.py` & `browserist-1.5.1/src/browserist/helper/window_handle.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/helper/xpath.py` & `browserist-1.5.1/src/browserist/helper/xpath.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/helper_iteration/retry.py` & `browserist-1.5.1/src/browserist/helper_iteration/retry.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/helper_screenshot/__init__.py` & `browserist-1.5.1/src/browserist/helper_screenshot/__init__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/helper_screenshot/complete_page.py` & `browserist-1.5.1/src/browserist/helper_screenshot/complete_page.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/helper_screenshot/controller.py` & `browserist-1.5.1/src/browserist/helper_screenshot/controller.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/helper_screenshot/file.py` & `browserist-1.5.1/src/browserist/helper_screenshot/file.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/browser/README.md` & `browserist-1.5.1/src/browserist/model/browser/README.md`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/browser/base/driver.py` & `browserist-1.5.1/src/browserist/model/browser/base/driver.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/browser/base/settings.py` & `browserist-1.5.1/src/browserist/model/browser/base/settings.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/browser/base/timeout/settings.py` & `browserist-1.5.1/src/browserist/model/browser/base/timeout/settings.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/browser/chrome.py` & `browserist-1.5.1/src/browserist/model/browser/chrome.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/browser/edge.py` & `browserist-1.5.1/src/browserist/model/browser/edge.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/browser/extension/__main__.py` & `browserist-1.5.1/src/browserist/model/browser/extension/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/browser/firefox.py` & `browserist-1.5.1/src/browserist/model/browser/firefox.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/browser/internet_explorer.py` & `browserist-1.5.1/src/browserist/model/browser/internet_explorer.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/browser/opera.py` & `browserist-1.5.1/src/browserist/model/browser/opera.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/browser/safari.py` & `browserist-1.5.1/src/browserist/model/browser/safari.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/combo_settings/cookie_banner.py` & `browserist-1.5.1/src/browserist/model/combo_settings/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/combo_settings/login_form.py` & `browserist-1.5.1/src/browserist/model/combo_settings/login_form.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/combo_settings/search.py` & `browserist-1.5.1/src/browserist/model/combo_settings/search.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/screenshot.py` & `browserist-1.5.1/src/browserist/model/screenshot.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/type/file_png.py` & `browserist-1.5.1/src/browserist/model/type/file_png.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/type/path.py` & `browserist-1.5.1/src/browserist/model/type/path.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/type/url.py` & `browserist-1.5.1/src/browserist/model/type/url.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/type/xpath.py` & `browserist-1.5.1/src/browserist/model/type/xpath.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist/model/window/controller.py` & `browserist-1.5.1/src/browserist/model/window/controller.py`

 * *Files identical despite different names*

### Comparing `browserist-1.5.0/src/browserist.egg-info/PKG-INFO` & `browserist-1.5.1/src/browserist.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserist
-Version: 1.5.0
+Version: 1.5.1
 Summary: Extension for the Selenium web driver that makes browser automation even easier
 Home-page: https://github.com/jakob-bagterp/browserist
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
 License: Apache-2.0
@@ -22,206 +22,111 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.0&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
 ![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![Apache 2.0 license](https://img.shields.io/static/v1?label=license&message=Apache%202.0&color=blue)](https://github.com/jakob-bagterp/browserist/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1JL65T099J)](https://codecov.io/gh/jakob-bagterp/browserist)
+[![CodeQL](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml)
 [![Downloads](https://static.pepy.tech/badge/browserist)](https://pepy.tech/project/browserist)
 
-# 👩‍💻 Browserist Extension for Selenium 👨‍💻
+# 👩‍💻 Browserist – Python Extension for Selenium 👨‍💻
 > **browserist**
 > 1. The belief that web browsers account for differences in websites or web applications in all of their ability and that a particular web browser is superior to others.
 > 2. Discrimination or prejudice based on web browser.
 
-Despite the [urban definition](https://www.urbandictionary.com/define.php?term=browserist), Browserist is a Python extension of the Selenium web driver that makes it even easier to use different browsers for testing and automation.
+Despite the [urban definition](https://www.urbandictionary.com/define.php?term=browserist), Browserist is a Python extension of the [Selenium web driver](https://www.selenium.dev/) that makes it even easier to use different browsers for testing and automation.
 
 Main features of Browserist:
 
 * Improves stability and speed
-* Simple syntax
-* Hassle-free setup that works across browsers: Chrome, Firefox, Edge, Safari, Opera, Internet Explorer
-* Extended library of browser automation functions and tools without elaborate code
-* Supports IntelliSense type hints and other capabilites of Python 3.10 that makes development more efficient
+* Simple syntax and less code
+* Hassle-free setup across browsers: Chrome, Firefox, Edge, Safari, Opera, Internet Explorer
+* Extensive framework of functions that makes browser automation easy
+* Supports IntelliSense and type hints that makes development more efficient
 
 ## How to Install
-Ready to try? [Learn how to install](https://github.com/jakob-bagterp/browserist/blob/master/INSTALLATION.md).
+Ready to try? With [PyPI](https://pypi.org/project/browserist/):
 
-## Getting Started
-The default browser is Chrome (except Edge for Windows). Simply type:
+```shell
+pip3 install browserist
+```
 
-```python
-from browserist import Browser
+Or with [Homebrew](https://brew.sh):
 
-browser = Browser()
-browser.open.url("http://example.com/")
-browser.quit()
+```shell
+brew tap jakob-bagterp/browserist
+brew install browserist
 ```
 
-Or use the built-in context manager so the browser automatically closes when done or if an error occurs:
+Find more installation details [here](https://jakob-bagterp.github.io/browserist/getting-started/installation/).
+
+## Getting Started
+You're now ready to go:
 
 ```python
 from browserist import Browser
 
 with Browser() as browser:
-    browser.open.url("http://example.com/")
-```
-
-### Browser Types
-If you want to use other browser types, e.g. Firefox, Edge, etc., define this in the settings:
-
-```python
-from browserist import Browser, BrowserSettings, BrowserType
-
-settings = BrowserSettings(type = BrowserType.FIREFOX)
-with Browser(settings) as browser:
-    browser.open.url("http://example.com/")
+    browser.open.url("https://example.com")
+    browser.wait.seconds(5)
 ```
 
-#### Supported Browsers
-| Name              | Type                            |
-| ----------------- | ------------------------------- |
-| Chrome            | `BrowserType.CHROME`            |
-| Edge              | `BrowserType.EDGE`              |
-| Firefox           | `BrowserType.FIREFOX`           |
-| Internet Explorer | `BrowserType.INTERNET_EXPLORER` |
-| Opera             | `BrowserType.OPERA`             |
-| Safari            | `BrowserType.SAFARI`            |
-
-### Navigation
-Similar to Selenium, use simple commands to automate the browser:
-
-| Action  | How                 | Description                        |
-| ------- | ------------------- | ---------------------------------- |
-| Forward | `browser.forward()` | Press the browser's back button    |
-| Back    | `browser.back()`    | Press the browser's forward button |
-| Refresh | `browser.refresh()` | Refresh the current page           |
-| Quit    | `browser.quit()`    | Close the browser                  |
-
 ## Improved Stability and Less Code
-Browserist improves stability with less code. As a browsers need time to render a page, especially single-page applications, Selenium is often used with explicit timeouts:
+Browserist improves stability with less code compared to standard use of Selenium. As a browsers need time to render a page, especially single-page applications, Selenium is often used with explicit timeouts:
 
 ```python
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 
 driver = webdriver.Chrome()
 
-driver.get("http://example.com/")
+driver.get("https://example.com")
 driver.implicitly_wait(3)
 search_box = driver.find_element(By.XPATH, "//xpath/to/input")
 search_button = driver.find_element(By.XPATH, "//xpath/to/button")
 search_box.send_keys("Lorem ipsum")
 search_button.click()
 driver.quit()
 ```
 
 Browserist does the same with less and cleaner code, yet also with increased stability and without explicit/implicit waits:
 
 ```python
 from browserist import Browser
 
 with Browser() as browser:
-    browser.open.url("http://example.com/")
+    browser.open.url("https://example.com")
     browser.input.value("//xpath/to/input", "Lorem ipsum")
     browser.click.button("//xpath/to/button")
 ```
 
-As you can't click a button that's not ready in the DOM, Browserist simply checks if elements are ready before interacting with them:
-
-| Timing:      | Too short ->  |     Just right     |  <- Too long   |
-| :----------- | :-----------: | :----------------: | :------------: |
-| Example:     | time.sleep(1) | wait.for_element() | time.sleep(10) |
-| Consequence: | _Code breaks_ | _Stable and fast_  |     _Slow_     |
-
-## Settings
-If you want a headless browser with Selenium, you typically would use different settings from browser to browser. Browserist solves this problem so that settings for Chrome, Firefox, Edge, etc. are standardised. For example, you can easily scale test runs across different browsers in a lightweight, headless configuration:
-
-```python
-from browserist import Browser, BrowserSettings, BrowserType
-
-chrome = BrowserSettings(type = BrowserType.CHROME, headless = True, disable_images = True)
-edge = BrowserSettings(type = BrowserType.EDGE, headless = True, disable_images = True)
-firefox = BrowserSettings(type = BrowserType.FIREFOX, headless = True, disable_images = True)
-
-for settings in [chrome, edge, firefox]:
-    with Browser(settings) as browser:
-        browser.open.url("http://example.com/")
-```
-
-Use `BrowserSettings` with the following options:
-
-| Setting              | Option                                    | Default                              | Description                                                                                                      |
-| -------------------- | ----------------------------------------- | ------------------------------------ | ---------------------------------------------------------------------------------------------------------------- |
-| `type`               | `BrowserType`                             | `BrowserType.CHROME`                 | Set browser type, e.g. Chrome, Edge, Firefox, etc.                                                               |
-| `headless`           | `True` or `False`                         | `False`                              | Run the browser in headless mode. May not be supported by all browsers.                                          |
-| `disable_images`     | `True` or `False`                         | `False`                              | Neither request nor render images, which typically improves loading speed. May not be supported by all browsers. |
-| `page_load_strategy` | `PageLoadStrategy`                        | `PageLoadStrategy.NORMAL`            | Set page load strategy.                                                                                          |
-| `path_to_executable` | Path to file                              | System default                       | If the browser executable isn't in a default folder, select which file to use.                                   |
-| `screenshot_dir`     | Path to directory                         | System default                       | Set where to save sreenshots. Default is the directory of Browserist.                                            |
-| `timeout`            | `TimeoutSettings`                         | `TimeoutStrategy.STOP` and 5 seconds | Set timeout strategy and time.                                                                                   |
-| `viewport`           | `DeviceViewportSize` or `(width, height)` | Browser default                      | Emulate viewport size as device or set custom value in pixels.                                                   |
-
-### Timeout Strategy
-What happens if a function times out: Should the browser stop or continue its operation?
-
-Define a general strategy and timeout in seconds:
-
-* Default is `5` seconds per function (note that a function-specific timeout overrides this)
-* The strategy can be `TimeoutStrategy.STOP` (default) or `TimeoutStrategy.CONTINUE`
-
-```python
-from browserist import Browser, BrowserSettings, TimeoutSettings, TimeoutStrategy
-
-timeout_settings = TimeoutSettings(strategy = TimeoutStrategy.CONTINUE, seconds = 10)
-settings = BrowserSettings(timeout = timeout_settings)
-
-with Browser(settings) as browser:
-    browser.open.url("http://example.com/")
-```
-
-#### Strategy Options
-| Option                     | Description                                                         |
-| -------------------------- | ------------------------------------------------------------------- |
-| `TimeoutStrategy.STOP`     | Default. Fail fast upon timeout and raise errors.                   |
-| `TimeoutStrategy.CONTINUE` | Continue despite timeouts and most errors (syntax errors excluded). |
-
-### Emulate Viewport of Common Devices
-You can set the viewport to emulate common device sizes or to a custom size. Note that it's recommended to run emulations in headless mode since an open browser may have minimum or maximum dimensions, either limited by the browser window or the monitor. Example:
-
-```python
-from browserist import Browser, BrowserSettings, common_devices
-
-settings = BrowserSettings(headless = True)
-
-with Browser(settings) as browser:
-    browser.viewport.set.size_by_device(common_devices.Apple.IPHONE_SE)
-    browser.open.url("http://example.com/")
-    browser.viewport.set.size(768, 1024)
-```
+## Documentation
+Find tutorials, code examples, list of all methods and much more [here](https://jakob-bagterp.github.io/browserist).
 
 # Thank You for Supporting
 ## Donate
-This module is free to use. And if you like it, feel free to [buy me a coffee](https://github.com/sponsors/jakob-bagterp).
+This module is free to use. And if you like it, feel free to [sponsor the project](https://github.com/sponsors/jakob-bagterp).
 
 ## Contribute
 If you have suggestions or changes to the module, feel free to add to the code and create a [pull request](https://github.com/jakob-bagterp/browserist/pulls).
 
 ## Report Bugs
 Report bugs and issues [here](https://github.com/jakob-bagterp/browserist/issues).
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.0&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.5.1&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
 ![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![Apache 2.0 license](https://img.shields.io/static/v1?label=license&message=Apache%202.0&color=blue)](https://github.com/jakob-bagterp/browserist/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1JL65T099J)](https://codecov.io/gh/jakob-bagterp/browserist)
+[![CodeQL](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml)
 [![Downloads](https://static.pepy.tech/badge/browserist)](https://pepy.tech/project/browserist)
 
 # 👩‍💻 How to Install Browserist 👨‍💻
 ## Prerequisites
 * Python 3.10 or higher
 * [Selenium](https://www.selenium.dev)
```

### Comparing `browserist-1.5.0/src/browserist.egg-info/SOURCES.txt` & `browserist-1.5.1/src/browserist.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,22 +45,32 @@
 src/browserist/browser/get/page_title.py
 src/browserist/browser/get/text.py
 src/browserist/browser/get/texts.py
 src/browserist/browser/get/attribute/__init__.py
 src/browserist/browser/get/attribute/__main__.py
 src/browserist/browser/get/attribute/value.py
 src/browserist/browser/get/attribute/values.py
+src/browserist/browser/get/attribute/.pytest_cache/.gitignore
+src/browserist/browser/get/attribute/.pytest_cache/CACHEDIR.TAG
+src/browserist/browser/get/attribute/.pytest_cache/README.md
+src/browserist/browser/get/attribute/.pytest_cache/v/cache/nodeids
+src/browserist/browser/get/attribute/.pytest_cache/v/cache/stepwise
 src/browserist/browser/get/url/__init__.py
 src/browserist/browser/get/url/__main__.py
 src/browserist/browser/get/url/current.py
 src/browserist/browser/get/url/current_domain.py
 src/browserist/browser/get/url/from_image.py
 src/browserist/browser/get/url/from_images.py
 src/browserist/browser/get/url/from_link.py
 src/browserist/browser/get/url/from_links.py
+src/browserist/browser/get/url/.pytest_cache/.gitignore
+src/browserist/browser/get/url/.pytest_cache/CACHEDIR.TAG
+src/browserist/browser/get/url/.pytest_cache/README.md
+src/browserist/browser/get/url/.pytest_cache/v/cache/nodeids
+src/browserist/browser/get/url/.pytest_cache/v/cache/stepwise
 src/browserist/browser/iframe/__init__.py
 src/browserist/browser/iframe/__main__.py
 src/browserist/browser/iframe/switch_to.py
 src/browserist/browser/iframe/switch_to_original_page.py
 src/browserist/browser/input/__init__.py
 src/browserist/browser/input/__main__.py
 src/browserist/browser/input/clear.py
```

