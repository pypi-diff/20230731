# Comparing `tmp/pretext-1.7.4.tar.gz` & `tmp/pretext-1.7.4.dev20230729.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.7.4.tar", max compression
+gzip compressed data, was "pretext-1.7.4.dev20230729.tar", max compression
```

## Comparing `pretext-1.7.4.tar` & `pretext-1.7.4.dev20230729.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    35148 2023-07-31 01:55:30.316036 pretext-1.7.4/LICENSE
--rw-r--r--   0        0        0     9757 2023-07-31 01:55:30.316036 pretext-1.7.4/README.md
--rw-r--r--   0        0        0     1500 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/__main__.py
--rw-r--r--   0        0        0    11608 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/build.py
--rw-r--r--   0        0        0    27783 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/cli.py
--rw-r--r--   0        0        0     6149 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/codechat.py
--rw-r--r--   0        0        0     5943 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      675 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/constants.py
--rw-r--r--   0        0        0      350 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/core/__init__.py
--rw-r--r--   0        0        0   172498 2023-07-31 01:56:02.169029 pretext-1.7.4/pretext/core/pretext.py
--rw-r--r--   0        0        0     1484 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/core/resources.py
--rw-r--r--   0        0        0  1045100 2023-07-31 01:56:02.169029 pretext-1.7.4/pretext/core/resources.zip
--rw-r--r--   0        0        0    16741 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/generate.py
--rw-r--r--   0        0        0    29656 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/project/__init__.py
--rw-r--r--   0        0        0    30392 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/project/refactor.py
--rw-r--r--   0        0        0     2620 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/project/xml.py
--rw-r--r--   0        0        0      739 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/templates/__init__.py
--rw-r--r--   0        0        0     2480 2023-07-31 01:56:02.237031 pretext-1.7.4/pretext/templates/resources/.devcontainer.json
--rw-r--r--   0        0        0     1676 2023-07-31 01:56:02.237031 pretext-1.7.4/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-07-31 01:56:02.237031 pretext-1.7.4/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   158949 2023-07-31 01:56:02.237031 pretext-1.7.4/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     6455 2023-07-31 01:56:02.225031 pretext-1.7.4/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   172278 2023-07-31 01:56:02.221031 pretext-1.7.4/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     3496 2023-07-31 01:56:02.237031 pretext-1.7.4/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-07-31 01:56:02.237031 pretext-1.7.4/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-07-31 01:56:02.237031 pretext-1.7.4/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     7231 2023-07-31 01:56:02.229031 pretext-1.7.4/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0      109 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/types.py
--rw-r--r--   0        0        0    25401 2023-07-31 01:55:30.316036 pretext-1.7.4/pretext/utils.py
--rw-r--r--   0        0        0     3341 2023-07-31 01:55:30.316036 pretext-1.7.4/pyproject.toml
--rw-r--r--   0        0        0    10879 1970-01-01 00:00:00.000000 pretext-1.7.4/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-29 06:14:20.414995 pretext-1.7.4.dev20230729/LICENSE
+-rw-r--r--   0        0        0     9757 2023-07-29 06:14:20.414995 pretext-1.7.4.dev20230729/README.md
+-rw-r--r--   0        0        0     1500 2023-07-29 06:15:01.909596 pretext-1.7.4.dev20230729/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-29 06:14:20.418995 pretext-1.7.4.dev20230729/pretext/__main__.py
+-rw-r--r--   0        0        0    11608 2023-07-29 06:14:20.418995 pretext-1.7.4.dev20230729/pretext/build.py
+-rw-r--r--   0        0        0    27783 2023-07-29 06:14:20.418995 pretext-1.7.4.dev20230729/pretext/cli.py
+-rw-r--r--   0        0        0     6149 2023-07-29 06:14:20.418995 pretext-1.7.4.dev20230729/pretext/codechat.py
+-rw-r--r--   0        0        0     5943 2023-07-29 06:14:20.418995 pretext-1.7.4.dev20230729/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      675 2023-07-29 06:14:20.418995 pretext-1.7.4.dev20230729/pretext/constants.py
+-rw-r--r--   0        0        0      350 2023-07-29 06:14:20.418995 pretext-1.7.4.dev20230729/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172498 2023-07-29 06:15:07.341922 pretext-1.7.4.dev20230729/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1484 2023-07-29 06:14:20.418995 pretext-1.7.4.dev20230729/pretext/core/resources.py
+-rw-r--r--   0        0        0  1045100 2023-07-29 06:15:07.341922 pretext-1.7.4.dev20230729/pretext/core/resources.zip
+-rw-r--r--   0        0        0    16741 2023-07-29 06:14:20.418995 pretext-1.7.4.dev20230729/pretext/generate.py
+-rw-r--r--   0        0        0    29656 2023-07-29 06:14:20.418995 pretext-1.7.4.dev20230729/pretext/project/__init__.py
+-rw-r--r--   0        0        0    30392 2023-07-29 06:14:20.418995 pretext-1.7.4.dev20230729/pretext/project/refactor.py
+-rw-r--r--   0        0        0     2620 2023-07-29 06:14:20.418995 pretext-1.7.4.dev20230729/pretext/project/xml.py
+-rw-r--r--   0        0        0      739 2023-07-29 06:14:20.418995 pretext-1.7.4.dev20230729/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     2480 2023-07-29 06:15:07.421927 pretext-1.7.4.dev20230729/pretext/templates/resources/.devcontainer.json
+-rw-r--r--   0        0        0     1676 2023-07-29 06:15:07.421927 pretext-1.7.4.dev20230729/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-07-29 06:15:07.421927 pretext-1.7.4.dev20230729/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   158949 2023-07-29 06:15:07.417927 pretext-1.7.4.dev20230729/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     6455 2023-07-29 06:15:07.405926 pretext-1.7.4.dev20230729/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   172278 2023-07-29 06:15:07.401926 pretext-1.7.4.dev20230729/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     3496 2023-07-29 06:15:07.421927 pretext-1.7.4.dev20230729/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-07-29 06:15:07.421927 pretext-1.7.4.dev20230729/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-07-29 06:15:07.421927 pretext-1.7.4.dev20230729/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     7231 2023-07-29 06:15:07.405926 pretext-1.7.4.dev20230729/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0      109 2023-07-29 06:14:20.418995 pretext-1.7.4.dev20230729/pretext/types.py
+-rw-r--r--   0        0        0    25401 2023-07-29 06:14:20.418995 pretext-1.7.4.dev20230729/pretext/utils.py
+-rw-r--r--   0        0        0     3333 2023-07-29 06:15:01.909596 pretext-1.7.4.dev20230729/pyproject.toml
+-rw-r--r--   0        0        0    10848 1970-01-01 00:00:00.000000 pretext-1.7.4.dev20230729/PKG-INFO
```

### Comparing `pretext-1.7.4/LICENSE` & `pretext-1.7.4.dev20230729/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/README.md` & `pretext-1.7.4.dev20230729/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/__init__.py` & `pretext-1.7.4.dev20230729/pretext/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 from single_version import get_version
 
 log = logging.getLogger("ptxlogger")
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = "9bce7e55911fb14e3e6e362bfa78bd6431c38597"
+CORE_COMMIT = '9bce7e55911fb14e3e6e362bfa78bd6431c38597'
 
 
 def activate() -> None:
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-1.7.4/pretext/build.py` & `pretext-1.7.4.dev20230729/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/cli.py` & `pretext-1.7.4.dev20230729/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/codechat.py` & `pretext-1.7.4.dev20230729/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/config/xml_overlay.py` & `pretext-1.7.4.dev20230729/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/constants.py` & `pretext-1.7.4.dev20230729/pretext/constants.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/core/pretext.py` & `pretext-1.7.4.dev20230729/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/core/resources.py` & `pretext-1.7.4.dev20230729/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/core/resources.zip` & `pretext-1.7.4.dev20230729/pretext/core/resources.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,144 +1,144 @@
 Zip file size: 1045100 bytes, number of entries: 142
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:56 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:56 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:56 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:56 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:56 xsl/
--rw-r--r--  2.0 unx    30908 b- defN 23-Jul-31 01:56 pretext/pretext
--rw-r--r--  2.0 unx     1955 b- defN 23-Jul-31 01:56 pretext/module-test.py
--rw-r--r--  2.0 unx     2566 b- defN 23-Jul-31 01:56 pretext/pretext.cfg
--rw-r--r--  2.0 unx   172498 b- defN 23-Jul-31 01:56 pretext/pretext.py
--rw-r--r--  2.0 unx     1367 b- defN 23-Jul-31 01:56 pretext/README.md
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-31 01:56 pretext/__init__.py
--rw-r--r--  2.0 unx    36045 b- defN 23-Jul-31 01:56 pretext/braille_format.py
--rw-r--r--  2.0 unx   125135 b- defN 23-Jul-31 01:56 schema/pretext.xsd
--rw-r--r--  2.0 unx      326 b- defN 23-Jul-31 01:56 schema/xml.xsd
--rw-r--r--  2.0 unx    58086 b- defN 23-Jul-31 01:56 schema/pretext.rnc
--rw-r--r--  2.0 unx    17587 b- defN 23-Jul-31 01:56 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx    25870 b- defN 23-Jul-31 01:56 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    18421 b- defN 23-Jul-31 01:56 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx     1180 b- defN 23-Jul-31 01:56 schema/README.md
--rw-r--r--  2.0 unx   134043 b- defN 23-Jul-31 01:56 schema/pretext.xml
--rw-r--r--  2.0 unx     3135 b- defN 23-Jul-31 01:56 schema/build.sh
--rw-r--r--  2.0 unx    34210 b- defN 23-Jul-31 01:56 schema/pretext-dev.rng
--rw-r--r--  2.0 unx   101829 b- defN 23-Jul-31 01:56 schema/pretext.rng
--rw-r--r--  2.0 unx     1276 b- defN 23-Jul-31 01:56 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx     2608 b- defN 23-Jul-31 01:56 css/colors_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-31 01:56 css/colors_blue_red.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jul-31 01:56 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-31 01:56 css/colors_green_plum.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jul-31 01:56 css/style_soundwriting.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Jul-31 01:56 css/colors_red_blue.css
--rw-r--r--  2.0 unx     7761 b- defN 23-Jul-31 01:56 css/style_default.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jul-31 01:56 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jul-31 01:56 css/colors_martiansands.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jul-31 01:56 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-31 01:56 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jul-31 01:56 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-31 01:56 css/colors_orange_navy.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jul-31 01:56 css/setcolors.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jul-31 01:56 css/update_css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jul-31 01:56 css/README.md
--rw-r--r--  2.0 unx     4308 b- defN 23-Jul-31 01:56 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-31 01:56 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jul-31 01:56 css/pretext.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jul-31 01:56 css/mathbook-content.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jul-31 01:56 css/mathbook-3.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Jul-31 01:56 css/epub.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-31 01:56 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx      691 b- defN 23-Jul-31 01:56 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jul-31 01:56 css/colors_green_blue.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jul-31 01:56 css/pretext_add_on.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jul-31 01:56 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jul-31 01:56 css/kindle.css
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:56 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:56 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:56 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:56 xsl/utilities/
--rw-r--r--  2.0 unx     2248 b- defN 23-Jul-31 01:56 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jul-31 01:56 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jul-31 01:56 xsl/entities.ent
--rw-r--r--  2.0 unx    17293 b- defN 23-Jul-31 01:56 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jul-31 01:56 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jul-31 01:56 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-Jul-31 01:56 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Jul-31 01:56 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx   231265 b- defN 23-Jul-31 01:56 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   611284 b- defN 23-Jul-31 01:56 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jul-31 01:56 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jul-31 01:56 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jul-31 01:56 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jul-31 01:56 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jul-31 01:56 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx    94587 b- defN 23-Jul-31 01:56 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Jul-31 01:56 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jul-31 01:56 xsl/README.md
--rw-r--r--  2.0 unx    10708 b- defN 23-Jul-31 01:56 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jul-31 01:56 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jul-31 01:56 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Jul-31 01:56 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-Jul-31 01:56 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Jul-31 01:56 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx   544154 b- defN 23-Jul-31 01:56 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jul-31 01:56 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx   548615 b- defN 23-Jul-31 01:56 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jul-31 01:56 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jul-31 01:56 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx   116581 b- defN 23-Jul-31 01:56 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jul-31 01:56 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jul-31 01:56 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jul-31 01:56 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jul-31 01:56 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jul-31 01:56 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-Jul-31 01:56 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jul-31 01:56 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx   110949 b- defN 23-Jul-31 01:56 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Jul-31 01:56 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-Jul-31 01:56 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jul-31 01:56 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Jul-31 01:56 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jul-31 01:56 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jul-31 01:56 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-Jul-31 01:56 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx    30257 b- defN 23-Jul-31 01:56 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-Jul-31 01:56 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx      513 b- defN 23-Jul-31 01:56 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4299 b- defN 23-Jul-31 01:56 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx     1810 b- defN 23-Jul-31 01:56 xsl/utilities/README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:56 xsl/support/play-button/
--rw-r--r--  2.0 unx      486 b- defN 23-Jul-31 01:56 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5879 b- defN 23-Jul-31 01:56 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-Jul-31 01:56 xsl/support/README.md
--rw-r--r--  2.0 unx     5065 b- defN 23-Jul-31 01:56 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx    10306 b- defN 23-Jul-31 01:56 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Jul-31 01:56 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5800 b- defN 23-Jul-31 01:56 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     6621 b- defN 23-Jul-31 01:56 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx      722 b- defN 23-Jul-31 01:56 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     2657 b- defN 23-Jul-31 01:56 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx    16534 b- defN 23-Jul-31 01:56 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    16349 b- defN 23-Jul-31 01:56 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    15866 b- defN 23-Jul-31 01:56 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16312 b- defN 23-Jul-31 01:56 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    15582 b- defN 23-Jul-31 01:56 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17056 b- defN 23-Jul-31 01:56 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16085 b- defN 23-Jul-31 01:56 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    19185 b- defN 23-Jul-31 01:56 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    17081 b- defN 23-Jul-31 01:56 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx     2286 b- defN 23-Jul-31 01:56 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx     4760 b- defN 23-Jul-31 01:56 xsl/localizations/README.md
--rw-r--r--  2.0 unx    19326 b- defN 23-Jul-31 01:56 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    17231 b- defN 23-Jul-31 01:56 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16500 b- defN 23-Jul-31 01:56 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17301 b- defN 23-Jul-31 01:56 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    20481 b- defN 23-Jul-31 01:56 xsl/localizations/ku-CKB.xml
--rw-r--r--  2.0 unx    16252 b- defN 23-Jul-31 01:56 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    16837 b- defN 23-Jul-31 01:56 xsl/localizations/af-ZA.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:56 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-Jul-31 01:56 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-Jul-31 01:56 script/mbx
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 01:56 script/mjsre/update-sre
--rw-r--r--  2.0 unx      116 b- defN 23-Jul-31 01:56 script/mjsre/package.json
--rw-r--r--  2.0 unx      481 b- defN 23-Jul-31 01:56 script/mjsre/README.md
--rw-r--r--  2.0 unx     9251 b- defN 23-Jul-31 01:56 script/mjsre/mj-sre-page.js
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:15 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:15 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:15 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:15 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:15 xsl/
+-rw-r--r--  2.0 unx    30908 b- defN 23-Jul-29 06:15 pretext/pretext
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jul-29 06:15 pretext/module-test.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jul-29 06:15 pretext/pretext.cfg
+-rw-r--r--  2.0 unx   172498 b- defN 23-Jul-29 06:15 pretext/pretext.py
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jul-29 06:15 pretext/README.md
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-29 06:15 pretext/__init__.py
+-rw-r--r--  2.0 unx    36045 b- defN 23-Jul-29 06:15 pretext/braille_format.py
+-rw-r--r--  2.0 unx   125135 b- defN 23-Jul-29 06:15 schema/pretext.xsd
+-rw-r--r--  2.0 unx      326 b- defN 23-Jul-29 06:15 schema/xml.xsd
+-rw-r--r--  2.0 unx    58086 b- defN 23-Jul-29 06:15 schema/pretext.rnc
+-rw-r--r--  2.0 unx    17587 b- defN 23-Jul-29 06:15 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx    25870 b- defN 23-Jul-29 06:15 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx    18421 b- defN 23-Jul-29 06:15 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jul-29 06:15 schema/README.md
+-rw-r--r--  2.0 unx   134043 b- defN 23-Jul-29 06:15 schema/pretext.xml
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jul-29 06:15 schema/build.sh
+-rw-r--r--  2.0 unx    34210 b- defN 23-Jul-29 06:15 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx   101829 b- defN 23-Jul-29 06:15 schema/pretext.rng
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jul-29 06:15 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-Jul-29 06:15 css/colors_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-29 06:15 css/colors_blue_red.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Jul-29 06:15 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-29 06:15 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Jul-29 06:15 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Jul-29 06:15 css/colors_red_blue.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-Jul-29 06:15 css/style_default.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jul-29 06:15 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jul-29 06:15 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jul-29 06:15 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-29 06:15 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jul-29 06:15 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-29 06:15 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Jul-29 06:15 css/setcolors.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Jul-29 06:15 css/update_css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jul-29 06:15 css/README.md
+-rw-r--r--  2.0 unx     4308 b- defN 23-Jul-29 06:15 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-29 06:15 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Jul-29 06:15 css/pretext.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Jul-29 06:15 css/mathbook-content.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Jul-29 06:15 css/mathbook-3.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jul-29 06:15 css/epub.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-29 06:15 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx      691 b- defN 23-Jul-29 06:15 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jul-29 06:15 css/colors_green_blue.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Jul-29 06:15 css/pretext_add_on.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Jul-29 06:15 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Jul-29 06:15 css/kindle.css
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:15 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:15 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:15 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:15 xsl/utilities/
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jul-29 06:15 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Jul-29 06:15 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Jul-29 06:15 xsl/entities.ent
+-rw-r--r--  2.0 unx    17293 b- defN 23-Jul-29 06:15 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jul-29 06:15 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Jul-29 06:15 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-Jul-29 06:15 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-Jul-29 06:15 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx   231265 b- defN 23-Jul-29 06:15 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   611284 b- defN 23-Jul-29 06:15 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jul-29 06:15 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jul-29 06:15 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-Jul-29 06:15 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jul-29 06:15 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jul-29 06:15 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx    94587 b- defN 23-Jul-29 06:15 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Jul-29 06:15 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jul-29 06:15 xsl/README.md
+-rw-r--r--  2.0 unx    10708 b- defN 23-Jul-29 06:15 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Jul-29 06:15 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Jul-29 06:15 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Jul-29 06:15 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-Jul-29 06:15 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-Jul-29 06:15 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx   544154 b- defN 23-Jul-29 06:15 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Jul-29 06:15 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx   548615 b- defN 23-Jul-29 06:15 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jul-29 06:15 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jul-29 06:15 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx   116581 b- defN 23-Jul-29 06:15 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Jul-29 06:15 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Jul-29 06:15 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Jul-29 06:15 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jul-29 06:15 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Jul-29 06:15 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-Jul-29 06:15 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Jul-29 06:15 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx   110949 b- defN 23-Jul-29 06:15 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 23-Jul-29 06:15 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-Jul-29 06:15 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jul-29 06:15 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Jul-29 06:15 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Jul-29 06:15 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Jul-29 06:15 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-Jul-29 06:15 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jul-29 06:15 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-Jul-29 06:15 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx      513 b- defN 23-Jul-29 06:15 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jul-29 06:15 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jul-29 06:15 xsl/utilities/README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:15 xsl/support/play-button/
+-rw-r--r--  2.0 unx      486 b- defN 23-Jul-29 06:15 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5879 b- defN 23-Jul-29 06:15 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-Jul-29 06:15 xsl/support/README.md
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jul-29 06:15 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx    10306 b- defN 23-Jul-29 06:15 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Jul-29 06:15 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jul-29 06:15 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     6621 b- defN 23-Jul-29 06:15 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx      722 b- defN 23-Jul-29 06:15 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jul-29 06:15 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx    16534 b- defN 23-Jul-29 06:15 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    16349 b- defN 23-Jul-29 06:15 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    15866 b- defN 23-Jul-29 06:15 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16312 b- defN 23-Jul-29 06:15 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    15582 b- defN 23-Jul-29 06:15 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17056 b- defN 23-Jul-29 06:15 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    16085 b- defN 23-Jul-29 06:15 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    19185 b- defN 23-Jul-29 06:15 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    17081 b- defN 23-Jul-29 06:15 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx     2286 b- defN 23-Jul-29 06:15 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx     4760 b- defN 23-Jul-29 06:15 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    19326 b- defN 23-Jul-29 06:15 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    17231 b- defN 23-Jul-29 06:15 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16500 b- defN 23-Jul-29 06:15 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17301 b- defN 23-Jul-29 06:15 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    20481 b- defN 23-Jul-29 06:15 xsl/localizations/ku-CKB.xml
+-rw-r--r--  2.0 unx    16252 b- defN 23-Jul-29 06:15 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    16837 b- defN 23-Jul-29 06:15 xsl/localizations/af-ZA.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:15 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-Jul-29 06:15 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-Jul-29 06:15 script/mbx
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 06:15 script/mjsre/update-sre
+-rw-r--r--  2.0 unx      116 b- defN 23-Jul-29 06:15 script/mjsre/package.json
+-rw-r--r--  2.0 unx      481 b- defN 23-Jul-29 06:15 script/mjsre/README.md
+-rw-r--r--  2.0 unx     9251 b- defN 23-Jul-29 06:15 script/mjsre/mj-sre-page.js
 142 files, 4848159 bytes uncompressed, 1027526 bytes compressed:  78.8%
```

### Comparing `pretext-1.7.4/pretext/generate.py` & `pretext-1.7.4.dev20230729/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/project/__init__.py` & `pretext-1.7.4.dev20230729/pretext/project/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/project/refactor.py` & `pretext-1.7.4.dev20230729/pretext/project/refactor.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/project/xml.py` & `pretext-1.7.4.dev20230729/pretext/project/xml.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/templates/__init__.py` & `pretext-1.7.4.dev20230729/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/templates/resources/.devcontainer.json` & `pretext-1.7.4.dev20230729/pretext/templates/resources/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/templates/resources/.gitignore` & `pretext-1.7.4.dev20230729/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/templates/resources/article.zip` & `pretext-1.7.4.dev20230729/pretext/templates/resources/article.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 158949 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:55 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:55 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:55 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-31 01:56 .gitignore
--rw-r--r--  2.0 unx       86 b- defN 23-Jul-31 01:55 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-31 01:56 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Jul-31 01:56 codechat_config.yaml
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-31 01:55 publication/publication.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jul-31 01:55 source/section-2.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-Jul-31 01:55 source/section-1.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jul-31 01:55 source/main.ptx
--rw-r--r--  2.0 unx   154806 b- defN 23-Jul-31 01:55 assets/frog.jpg
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:14 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:14 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:14 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-29 06:15 .gitignore
+-rw-r--r--  2.0 unx       86 b- defN 23-Jul-29 06:14 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-29 06:15 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Jul-29 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx      242 b- defN 23-Jul-29 06:14 publication/publication.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Jul-29 06:14 source/section-2.ptx
+-rw-r--r--  2.0 unx      449 b- defN 23-Jul-29 06:14 source/section-1.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Jul-29 06:14 source/main.ptx
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jul-29 06:14 assets/frog.jpg
 12 files, 162919 bytes uncompressed, 157669 bytes compressed:  3.2%
```

### Comparing `pretext-1.7.4/pretext/templates/resources/book.zip` & `pretext-1.7.4.dev20230729/pretext/templates/resources/book.zip`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 6455 bytes, number of entries: 8
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:55 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:55 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-31 01:56 .gitignore
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-31 01:55 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-31 01:56 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Jul-31 01:56 codechat_config.yaml
--rw-r--r--  2.0 unx     6114 b- defN 23-Jul-31 01:55 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-Jul-31 01:55 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:14 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:14 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-29 06:15 .gitignore
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-29 06:14 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-29 06:15 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Jul-29 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jul-29 06:14 publication/publication.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-Jul-29 06:14 source/main.ptx
 8 files, 13887 bytes uncompressed, 5603 bytes compressed:  59.7%
```

### Comparing `pretext-1.7.4/pretext/templates/resources/demo.zip` & `pretext-1.7.4.dev20230729/pretext/templates/resources/demo.zip`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,35 +1,35 @@
 Zip file size: 172278 bytes, number of entries: 33
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:55 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:55 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:55 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-31 01:56 .gitignore
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-31 01:55 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-Jul-31 01:56 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Jul-31 01:56 codechat_config.yaml
--rw-r--r--  2.0 unx     6092 b- defN 23-Jul-31 01:55 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:55 source/images/
--rw-r--r--  2.0 unx     1515 b- defN 23-Jul-31 01:55 source/ex-first.ptx
--rw-r--r--  2.0 unx     2295 b- defN 23-Jul-31 01:55 source/ch-generate.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Jul-31 01:55 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-Jul-31 01:55 source/sec-features.ptx
--rw-r--r--  2.0 unx      777 b- defN 23-Jul-31 01:55 source/ww.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jul-31 01:55 source/ch-empty.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jul-31 01:55 source/frontmatter.ptx
--rw-r--r--  2.0 unx     2428 b- defN 23-Jul-31 01:55 source/main.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jul-31 01:55 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jul-31 01:55 source/backmatter.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jul-31 01:55 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jul-31 01:55 source/ch-features.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Jul-31 01:55 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jul-31 01:55 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jul-31 01:55 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jul-31 01:55 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jul-31 01:55 source/docinfo.ptx
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-31 01:55 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx      835 b- defN 23-Jul-31 01:55 source/images/cflag.asy
--rw-r--r--  2.0 unx       93 b- defN 23-Jul-31 01:55 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Jul-31 01:55 source/images/tikz.tex
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:55 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jul-31 01:55 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jul-31 01:55 assets/jsxgraph/infinity.js
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:14 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:14 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:14 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-29 06:15 .gitignore
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-29 06:14 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-29 06:15 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Jul-29 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     6092 b- defN 23-Jul-29 06:14 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:14 source/images/
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jul-29 06:14 source/ex-first.ptx
+-rw-r--r--  2.0 unx     2295 b- defN 23-Jul-29 06:14 source/ch-generate.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jul-29 06:14 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-Jul-29 06:14 source/sec-features.ptx
+-rw-r--r--  2.0 unx      777 b- defN 23-Jul-29 06:14 source/ww.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Jul-29 06:14 source/ch-empty.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Jul-29 06:14 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     2428 b- defN 23-Jul-29 06:14 source/main.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Jul-29 06:14 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Jul-29 06:14 source/backmatter.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Jul-29 06:14 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-Jul-29 06:14 source/ch-features.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Jul-29 06:14 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Jul-29 06:14 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Jul-29 06:14 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Jul-29 06:14 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jul-29 06:14 source/docinfo.ptx
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-29 06:14 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx      835 b- defN 23-Jul-29 06:14 source/images/cflag.asy
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-29 06:14 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Jul-29 06:14 source/images/tikz.tex
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:14 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jul-29 06:14 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jul-29 06:14 assets/jsxgraph/infinity.js
 33 files, 188129 bytes uncompressed, 168462 bytes compressed:  10.5%
```

### Comparing `pretext-1.7.4/pretext/templates/resources/hello.zip` & `pretext-1.7.4.dev20230729/pretext/templates/resources/hello.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 3496 bytes, number of entries: 8
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:55 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:55 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-31 01:56 .gitignore
--rw-r--r--  2.0 unx       69 b- defN 23-Jul-31 01:55 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-Jul-31 01:55 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Jul-31 01:56 codechat_config.yaml
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-31 01:55 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-Jul-31 01:55 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:14 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:14 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-29 06:15 .gitignore
+-rw-r--r--  2.0 unx       69 b- defN 23-Jul-29 06:14 README.md
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jul-29 06:14 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Jul-29 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx      242 b- defN 23-Jul-29 06:14 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-Jul-29 06:14 source/main.ptx
 8 files, 5898 bytes uncompressed, 2644 bytes compressed:  55.2%
```

### Comparing `pretext-1.7.4/pretext/templates/resources/project.ptx` & `pretext-1.7.4.dev20230729/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pretext/templates/resources/slideshow.zip` & `pretext-1.7.4.dev20230729/pretext/templates/resources/slideshow.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 7231 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:55 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:55 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 01:55 xsl/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-31 01:56 .gitignore
--rw-r--r--  2.0 unx      784 b- defN 23-Jul-31 01:55 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Jul-31 01:56 codechat_config.yaml
--rw-r--r--  2.0 unx     2097 b- defN 23-Jul-31 01:55 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-Jul-31 01:55 source/main.ptx
--rw-r--r--  2.0 unx      190 b- defN 23-Jul-31 01:55 xsl/slides.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:14 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:14 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-29 06:14 xsl/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jul-29 06:15 .gitignore
+-rw-r--r--  2.0 unx      784 b- defN 23-Jul-29 06:14 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Jul-29 06:15 codechat_config.yaml
+-rw-r--r--  2.0 unx     2097 b- defN 23-Jul-29 06:14 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-Jul-29 06:14 source/main.ptx
+-rw-r--r--  2.0 unx      190 b- defN 23-Jul-29 06:14 xsl/slides.xsl
 9 files, 18485 bytes uncompressed, 6285 bytes compressed:  66.0%
```

### Comparing `pretext-1.7.4/pretext/utils.py` & `pretext-1.7.4.dev20230729/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.4/pyproject.toml` & `pretext-1.7.4.dev20230729/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "1.7.4"
+version = "1.7.4.dev20230729"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
@@ -29,16 +29,15 @@
 [tool.poetry.dependencies]
 python = "^3.8.5"
 lxml = "^4.8"
 requests = "^2"
 watchdog = "^3"
 GitPython = "^3"
 click = "^8"
-pdfCropMargins = "~1.0.9"
-PyPDF2 = "~2.5"
+pdfCropMargins = "^2"
 click-log = "^0.4"
 ghp-import = "^2"
 single-version = "^1"
 playwright = "^1"
 pydantic-xml = "^1"
 qrcode = "^7"
```

### Comparing `pretext-1.7.4/PKG-INFO` & `pretext-1.7.4.dev20230729/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.7.4
+Version: 1.7.4.dev20230729
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3,<4)
-Requires-Dist: PyPDF2 (>=2.5,<2.6)
 Requires-Dist: click (>=8,<9)
 Requires-Dist: click-log (>=0.4,<0.5)
 Requires-Dist: ghp-import (>=2,<3)
 Requires-Dist: lxml (>=4.8,<5.0)
-Requires-Dist: pdfCropMargins (>=1.0.9,<1.1.0)
+Requires-Dist: pdfCropMargins (>=2,<3)
 Requires-Dist: playwright (>=1,<2)
 Requires-Dist: pydantic-xml (>=1,<2)
 Requires-Dist: qrcode (>=7,<8)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: single-version (>=1,<2)
 Requires-Dist: watchdog (>=3,<4)
 Project-URL: Repository, https://github.com/PreTeXtBook/pretext-cli
```

