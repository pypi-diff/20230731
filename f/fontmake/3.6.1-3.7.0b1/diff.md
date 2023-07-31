# Comparing `tmp/fontmake-3.6.1.zip` & `tmp/fontmake-3.7.0b1.zip`

## zipinfo {}

```diff
@@ -1,727 +1,728 @@
-Zip file size: 468112 bytes, number of entries: 725
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/Lib/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/.github/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/
--rw-r--r--  2.0 unx      466 b- defN 23-Jul-20 10:51 fontmake-3.6.1/requirements.txt
--rw-r--r--  2.0 unx      226 b- defN 23-Jul-20 10:52 fontmake-3.6.1/setup.cfg
--rwxr-xr-x  2.0 unx     1298 b- defN 23-Jul-20 10:51 fontmake-3.6.1/build_pyz.sh
--rw-r--r--  2.0 unx     7301 b- defN 23-Jul-20 10:52 fontmake-3.6.1/PKG-INFO
--rw-r--r--  2.0 unx     3193 b- defN 23-Jul-20 10:51 fontmake-3.6.1/TROUBLESHOOTING.md
--rw-r--r--  2.0 unx     1453 b- defN 23-Jul-20 10:51 fontmake-3.6.1/.gitignore
--rw-r--r--  2.0 unx      191 b- defN 23-Jul-20 10:51 fontmake-3.6.1/test_requirements.txt
--rw-r--r--  2.0 unx      142 b- defN 23-Jul-20 10:51 fontmake-3.6.1/MANIFEST.in
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-20 10:51 fontmake-3.6.1/LICENSE
--rw-r--r--  2.0 unx    19601 b- defN 23-Jul-20 10:51 fontmake-3.6.1/USAGE.md
--rw-r--r--  2.0 unx     6285 b- defN 23-Jul-20 10:51 fontmake-3.6.1/README.md
--rw-r--r--  2.0 unx     2924 b- defN 23-Jul-20 10:51 fontmake-3.6.1/setup.py
--rw-r--r--  2.0 unx      163 b- defN 23-Jul-20 10:51 fontmake-3.6.1/pyproject.toml
--rw-r--r--  2.0 unx      806 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tox.ini
--rw-r--r--  2.0 unx      792 b- defN 23-Jul-20 10:51 fontmake-3.6.1/.coveragerc
--rw-r--r--  2.0 unx     1450 b- defN 23-Jul-20 10:51 fontmake-3.6.1/CONTRIBUTING.md
--rw-r--r--  2.0 unx       77 b- defN 23-Jul-20 10:51 fontmake-3.6.1/.codecov.yml
--rw-r--r--  2.0 unx      227 b- defN 23-Jul-20 10:51 fontmake-3.6.1/.editorconfig
--rw-r--r--  2.0 unx      322 b- defN 23-Jul-20 10:51 fontmake-3.6.1/.gitattributes
--rw-r--r--  2.0 unx      168 b- defN 23-Jul-20 10:51 fontmake-3.6.1/.pyup.yml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/Lib/fontmake/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/Lib/fontmake.egg-info/
--rw-r--r--  2.0 unx     3049 b- defN 23-Jul-20 10:51 fontmake-3.6.1/Lib/fontmake/compatibility.py
--rw-r--r--  2.0 unx    32133 b- defN 23-Jul-20 10:51 fontmake-3.6.1/Lib/fontmake/instantiator.py
--rw-r--r--  2.0 unx     1439 b- defN 23-Jul-20 10:51 fontmake-3.6.1/Lib/fontmake/errors.py
--rw-r--r--  2.0 unx     3288 b- defN 23-Jul-20 10:51 fontmake-3.6.1/Lib/fontmake/ttfautohint.py
--rw-r--r--  2.0 unx    58334 b- defN 23-Jul-20 10:51 fontmake-3.6.1/Lib/fontmake/font_project.py
--rw-r--r--  2.0 unx      160 b- defN 23-Jul-20 10:51 fontmake-3.6.1/Lib/fontmake/_version.py
--rw-r--r--  2.0 unx      108 b- defN 23-Jul-20 10:51 fontmake-3.6.1/Lib/fontmake/__init__.py
--rw-r--r--  2.0 unx    25640 b- defN 23-Jul-20 10:51 fontmake-3.6.1/Lib/fontmake/__main__.py
--rw-r--r--  2.0 unx     7301 b- defN 23-Jul-20 10:52 fontmake-3.6.1/Lib/fontmake.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-20 10:52 fontmake-3.6.1/Lib/fontmake.egg-info/top_level.txt
--rw-r--r--  2.0 unx    42241 b- defN 23-Jul-20 10:52 fontmake-3.6.1/Lib/fontmake.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      402 b- defN 23-Jul-20 10:52 fontmake-3.6.1/Lib/fontmake.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-20 10:52 fontmake-3.6.1/Lib/fontmake.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-20 10:52 fontmake-3.6.1/Lib/fontmake.egg-info/entry_points.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/.github/workflows/
--rw-r--r--  2.0 unx     4279 b- defN 23-Jul-20 10:51 fontmake-3.6.1/.github/workflows/ci.yml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/
--rw-r--r--  2.0 unx      133 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/conftest.py
--rw-r--r--  2.0 unx    25699 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/test_instantiator.py
--rw-r--r--  2.0 unx    33198 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/test_main.py
--rw-r--r--  2.0 unx     1668 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/test_compatibility.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/SwapGlyphNames/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceTest/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/InterpolateLayoutTest/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/AutohintingTest/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/IncompatibleSans/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/
--rw-r--r--  2.0 unx     6386 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/TestSubset.glyphs
--rw-r--r--  2.0 unx     6381 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/TestSubset2.glyphs
--rw-r--r--  2.0 unx    30579 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/GlyphsUnitTestSans.glyphs
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/
--rw-r--r--  2.0 unx     2035 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/
--rw-r--r--  2.0 unx      275 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/layercontents.plist
--rw-r--r--  2.0 unx      887 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/metainfo.plist
--rw-r--r--  2.0 unx      360 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/lib.plist
--rw-r--r--  2.0 unx     1455 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif
--rw-r--r--  2.0 unx      412 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1659 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx     1261 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif
--rw-r--r--  2.0 unx     1265 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/
--rw-r--r--  2.0 unx      275 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/layercontents.plist
--rw-r--r--  2.0 unx      890 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/metainfo.plist
--rw-r--r--  2.0 unx      360 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/lib.plist
--rw-r--r--  2.0 unx     1439 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif
--rw-r--r--  2.0 unx      412 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1642 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx     1263 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif
--rw-r--r--  2.0 unx     1263 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/layercontents.plist
--rw-r--r--  2.0 unx      471 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/groups.plist
--rw-r--r--  2.0 unx      714 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/kerning.plist
--rw-r--r--  2.0 unx      790 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/metainfo.plist
--rw-r--r--  2.0 unx      443 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/lib.plist
--rw-r--r--  2.0 unx      382 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.glif
--rw-r--r--  2.0 unx      522 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif
--rw-r--r--  2.0 unx      393 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.swap.glif
--rw-r--r--  2.0 unx      581 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif
--rw-r--r--  2.0 unx      436 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.glif
--rw-r--r--  2.0 unx      543 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      156 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      646 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/layercontents.plist
--rw-r--r--  2.0 unx      790 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/metainfo.plist
--rw-r--r--  2.0 unx      410 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/lib.plist
--rw-r--r--  2.0 unx      898 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif
--rw-r--r--  2.0 unx      487 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      539 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif
--rw-r--r--  2.0 unx      205 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.alt.glif
--rw-r--r--  2.0 unx      784 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif
--rw-r--r--  2.0 unx      221 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/
--rw-r--r--  2.0 unx    22772 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist
--rw-r--r--  2.0 unx       83 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/order.plist
--rw-r--r--  2.0 unx     1308 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph
--rw-r--r--  2.0 unx      454 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_dieresis.glyph
--rw-r--r--  2.0 unx     1580 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph
--rw-r--r--  2.0 unx      764 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph
--rw-r--r--  2.0 unx      902 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph
--rw-r--r--  2.0 unx     1889 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph
--rw-r--r--  2.0 unx     1026 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph
--rw-r--r--  2.0 unx      445 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/adieresis.glyph
--rw-r--r--  2.0 unx     5010 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph
--rw-r--r--  2.0 unx     6165 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph
--rw-r--r--  2.0 unx     2295 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/
--rw-r--r--  2.0 unx      983 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest.designspace
--rw-r--r--  2.0 unx     3057 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufoz
--rw-r--r--  2.0 unx      852 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace
--rw-r--r--  2.0 unx      614 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace
--rw-r--r--  2.0 unx      621 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace
--rw-r--r--  2.0 unx     1340 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace
--rw-r--r--  2.0 unx      916 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace
--rw-r--r--  2.0 unx     2253 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufoz
--rw-r--r--  2.0 unx      745 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/layercontents.plist
--rw-r--r--  2.0 unx      357 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/groups.plist
--rw-r--r--  2.0 unx      878 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/metainfo.plist
--rw-r--r--  2.0 unx      240 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/lib.plist
--rw-r--r--  2.0 unx      343 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/l.glif
--rw-r--r--  2.0 unx      237 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/contents.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/layercontents.plist
--rw-r--r--  2.0 unx      548 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/metainfo.plist
--rw-r--r--  2.0 unx      345 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/l.glif
--rw-r--r--  2.0 unx      237 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/contents.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/
--rw-r--r--  2.0 unx      830 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/
--rw-r--r--  2.0 unx      283 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/layercontents.plist
--rw-r--r--  2.0 unx      897 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/metainfo.plist
--rw-r--r--  2.0 unx     1030 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist
--rw-r--r--  2.0 unx      243 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      770 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif
--rw-r--r--  2.0 unx      247 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/layerinfo.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/
--rw-r--r--  2.0 unx      283 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/layercontents.plist
--rw-r--r--  2.0 unx      900 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/metainfo.plist
--rw-r--r--  2.0 unx     1030 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist
--rw-r--r--  2.0 unx      243 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      786 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif
--rw-r--r--  2.0 unx      247 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/layerinfo.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/
--rw-r--r--  2.0 unx      983 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace
--rw-r--r--  2.0 unx     1135 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/layercontents.plist
--rw-r--r--  2.0 unx      887 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/metainfo.plist
--rw-r--r--  2.0 unx      303 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/lib.plist
--rw-r--r--  2.0 unx      343 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/l.glif
--rw-r--r--  2.0 unx      288 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      479 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/asas.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/layercontents.plist
--rw-r--r--  2.0 unx      886 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/metainfo.plist
--rw-r--r--  2.0 unx      303 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/lib.plist
--rw-r--r--  2.0 unx      345 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/l.glif
--rw-r--r--  2.0 unx      288 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      425 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/asas.glif
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GSUB.txt
--rw-r--r--  2.0 unx      716 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist
--rw-r--r--  2.0 unx       73 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GDEF.txt
--rw-r--r--  2.0 unx      249 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 1000 GPOS.txt
--rw-r--r--  2.0 unx     6904 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 0 GPOS.txt
--rw-r--r--  2.0 unx   125360 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/AutohintingTest/Padyakke.glyphs
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/
--rw-r--r--  2.0 unx      762 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/
--rw-r--r--  2.0 unx      101 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/features.fea
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1158 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/metainfo.plist
--rw-r--r--  2.0 unx     2113 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist
--rw-r--r--  2.0 unx      694 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx      215 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      560 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      429 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      154 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx     1196 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1160 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/metainfo.plist
--rw-r--r--  2.0 unx     2107 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist
--rw-r--r--  2.0 unx      652 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx      217 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      652 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      429 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      154 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      893 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/
--rw-r--r--  2.0 unx     1059 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/family.fea
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/
--rw-r--r--  2.0 unx       20 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/features.fea
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/layercontents.plist
--rw-r--r--  2.0 unx      899 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/metainfo.plist
--rw-r--r--  2.0 unx      183 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/contents.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/layercontents.plist
--rw-r--r--  2.0 unx      897 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/metainfo.plist
--rw-r--r--  2.0 unx      183 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/contents.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/
--rw-r--r--  2.0 unx     8462 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSans_missing.designspace
--rw-r--r--  2.0 unx     7111 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSans.designspace
--rw-r--r--  2.0 unx     1394 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSans-width-only.designspace
--rw-r--r--  2.0 unx     2611 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace
--rw-r--r--  2.0 unx     1412 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSans-weight-only.designspace
--rw-r--r--  2.0 unx     1067 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace
--rw-r--r--  2.0 unx     1074 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/LICENSE
--rw-r--r--  2.0 unx     7834 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSans_no_default.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
--rw-r--r--  2.0 unx       37 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/features.fea
--rw-r--r--  2.0 unx      383 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx      366 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/groups.plist
--rw-r--r--  2.0 unx     4852 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist
--rw-r--r--  2.0 unx     1873 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx    18291 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist
--rw-r--r--  2.0 unx     1965 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      252 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx      228 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
--rw-r--r--  2.0 unx     2537 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
--rw-r--r--  2.0 unx      341 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
--rw-r--r--  2.0 unx      181 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
--rw-r--r--  2.0 unx      237 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
--rw-r--r--  2.0 unx      228 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
--rw-r--r--  2.0 unx     2459 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
--rw-r--r--  2.0 unx      344 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
--rw-r--r--  2.0 unx      857 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif
--rw-r--r--  2.0 unx      325 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblleft.glif
--rw-r--r--  2.0 unx      549 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif
--rw-r--r--  2.0 unx     1459 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif
--rw-r--r--  2.0 unx     1388 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif
--rw-r--r--  2.0 unx     1751 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx     1134 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx     1970 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      230 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/colon.glif
--rw-r--r--  2.0 unx      801 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif
--rw-r--r--  2.0 unx      924 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif
--rw-r--r--  2.0 unx      752 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif
--rw-r--r--  2.0 unx      703 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      954 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx     1416 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      349 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dot.glif
--rw-r--r--  2.0 unx      518 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif
--rw-r--r--  2.0 unx     1785 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      943 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif
--rw-r--r--  2.0 unx      743 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx      749 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif
--rw-r--r--  2.0 unx      740 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif
--rw-r--r--  2.0 unx     1158 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      521 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif
--rw-r--r--  2.0 unx     2687 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      370 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dieresis.glif
--rw-r--r--  2.0 unx      747 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif
--rw-r--r--  2.0 unx      378 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx      154 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      235 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblbase.glif
--rw-r--r--  2.0 unx      542 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblright.glif
--rw-r--r--  2.0 unx      354 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_acute.glif
--rw-r--r--  2.0 unx      514 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif
--rw-r--r--  2.0 unx     1130 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif
--rw-r--r--  2.0 unx      233 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/semicolon.glif
--rw-r--r--  2.0 unx      802 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif
--rw-r--r--  2.0 unx      360 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_dieresis.glif
--rw-r--r--  2.0 unx      518 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif
--rw-r--r--  2.0 unx      875 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif
--rw-r--r--  2.0 unx     1320 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx     1056 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif
--rw-r--r--  2.0 unx      750 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif
--rw-r--r--  2.0 unx     2358 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/acute.glif
--rw-r--r--  2.0 unx      371 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      352 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/period.glif
--rw-r--r--  2.0 unx     1357 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx      193 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotesinglbase.glif
--rw-r--r--  2.0 unx      517 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif
--rw-r--r--  2.0 unx      181 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
--rw-r--r--  2.0 unx      236 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/
--rw-r--r--  2.0 unx       68 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      615 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1386 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx    16617 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx      228 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     2353 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif
--rw-r--r--  2.0 unx      343 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx      268 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/contents.plist
--rw-r--r--  2.0 unx     3181 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif
--rw-r--r--  2.0 unx      341 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/layerinfo.plist
--rw-r--r--  2.0 unx      950 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif
--rw-r--r--  2.0 unx     2307 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx      923 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx     1806 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      422 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     2646 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      371 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      983 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx      228 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/contents.plist
--rw-r--r--  2.0 unx      344 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/layerinfo.plist
--rw-r--r--  2.0 unx     1938 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/
--rw-r--r--  2.0 unx       42 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      383 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx      366 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/groups.plist
--rw-r--r--  2.0 unx     4580 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist
--rw-r--r--  2.0 unx     1885 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx     7840 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx     1988 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      252 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx      858 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif
--rw-r--r--  2.0 unx      325 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblleft.glif
--rw-r--r--  2.0 unx      546 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif
--rw-r--r--  2.0 unx     1829 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif
--rw-r--r--  2.0 unx     1359 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif
--rw-r--r--  2.0 unx     1774 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx     1128 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx     2285 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/colon.glif
--rw-r--r--  2.0 unx      800 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif
--rw-r--r--  2.0 unx      915 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif
--rw-r--r--  2.0 unx      744 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif
--rw-r--r--  2.0 unx      701 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      747 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx     1785 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      351 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dot.glif
--rw-r--r--  2.0 unx      491 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowright.glif
--rw-r--r--  2.0 unx     1799 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      936 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif
--rw-r--r--  2.0 unx      741 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx      741 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif
--rw-r--r--  2.0 unx      740 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif
--rw-r--r--  2.0 unx     1137 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      521 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif
--rw-r--r--  2.0 unx     2687 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      384 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dieresis.glif
--rw-r--r--  2.0 unx      748 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif
--rw-r--r--  2.0 unx      379 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx      154 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      608 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif
--rw-r--r--  2.0 unx      542 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblright.glif
--rw-r--r--  2.0 unx      340 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_acute.glif
--rw-r--r--  2.0 unx      491 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowdown.glif
--rw-r--r--  2.0 unx     1204 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif
--rw-r--r--  2.0 unx      245 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/semicolon.glif
--rw-r--r--  2.0 unx      825 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif
--rw-r--r--  2.0 unx      346 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_dieresis.glif
--rw-r--r--  2.0 unx      490 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowleft.glif
--rw-r--r--  2.0 unx      872 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif
--rw-r--r--  2.0 unx     1319 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx      936 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif
--rw-r--r--  2.0 unx      743 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif
--rw-r--r--  2.0 unx     2367 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/acute.glif
--rw-r--r--  2.0 unx      371 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      350 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/period.glif
--rw-r--r--  2.0 unx     1382 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx      566 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif
--rw-r--r--  2.0 unx      490 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowup.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/
--rw-r--r--  2.0 unx       68 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/features.fea
--rw-r--r--  2.0 unx      383 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx     5462 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist
--rw-r--r--  2.0 unx     1384 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx    16223 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist
--rw-r--r--  2.0 unx      228 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     2396 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif
--rw-r--r--  2.0 unx      343 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     2148 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx      911 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx     1824 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      376 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      371 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx     1162 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/
--rw-r--r--  2.0 unx       36 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/features.fea
--rw-r--r--  2.0 unx      383 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx      366 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/groups.plist
--rw-r--r--  2.0 unx      301 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/kerning.plist
--rw-r--r--  2.0 unx     1870 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx    12341 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist
--rw-r--r--  2.0 unx     1986 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      298 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     2005 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx      861 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif
--rw-r--r--  2.0 unx      325 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblleft.glif
--rw-r--r--  2.0 unx      549 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif
--rw-r--r--  2.0 unx     1495 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif
--rw-r--r--  2.0 unx     1387 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif
--rw-r--r--  2.0 unx     1747 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx     1150 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx     2369 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      242 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/colon.glif
--rw-r--r--  2.0 unx      803 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif
--rw-r--r--  2.0 unx      919 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif
--rw-r--r--  2.0 unx      750 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif
--rw-r--r--  2.0 unx      701 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      750 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx     1418 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      351 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dot.glif
--rw-r--r--  2.0 unx      495 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowright.glif
--rw-r--r--  2.0 unx     2203 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx     1037 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif
--rw-r--r--  2.0 unx      742 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx      745 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif
--rw-r--r--  2.0 unx      742 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif
--rw-r--r--  2.0 unx     1154 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      522 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif
--rw-r--r--  2.0 unx     2687 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      370 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dieresis.glif
--rw-r--r--  2.0 unx      750 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif
--rw-r--r--  2.0 unx      380 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx      154 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      259 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblbase.glif
--rw-r--r--  2.0 unx      545 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblright.glif
--rw-r--r--  2.0 unx      354 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_acute.glif
--rw-r--r--  2.0 unx      491 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowdown.glif
--rw-r--r--  2.0 unx     1140 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif
--rw-r--r--  2.0 unx      245 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/semicolon.glif
--rw-r--r--  2.0 unx      806 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif
--rw-r--r--  2.0 unx      360 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_dieresis.glif
--rw-r--r--  2.0 unx      493 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowleft.glif
--rw-r--r--  2.0 unx      875 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif
--rw-r--r--  2.0 unx      947 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx      940 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif
--rw-r--r--  2.0 unx      748 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif
--rw-r--r--  2.0 unx     2376 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/acute.glif
--rw-r--r--  2.0 unx      371 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      350 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/period.glif
--rw-r--r--  2.0 unx      988 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx      205 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotesinglbase.glif
--rw-r--r--  2.0 unx      492 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowup.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
--rw-r--r--  2.0 unx       68 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      811 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx      491 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/groups.plist
--rw-r--r--  2.0 unx      517 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist
--rw-r--r--  2.0 unx     1888 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx    18792 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx     3998 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      298 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     3358 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
--rw-r--r--  2.0 unx      244 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     2452 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif
--rw-r--r--  2.0 unx      422 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.closed.glif
--rw-r--r--  2.0 unx      751 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif
--rw-r--r--  2.0 unx     2111 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif
--rw-r--r--  2.0 unx      482 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
--rw-r--r--  2.0 unx     3498 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
--rw-r--r--  2.0 unx      247 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
--rw-r--r--  2.0 unx     1471 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif
--rw-r--r--  2.0 unx      853 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif
--rw-r--r--  2.0 unx      330 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
--rw-r--r--  2.0 unx      828 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
--rw-r--r--  2.0 unx     2706 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
--rw-r--r--  2.0 unx      371 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
--rw-r--r--  2.0 unx     2825 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
--rw-r--r--  2.0 unx      252 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
--rw-r--r--  2.0 unx      853 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif
--rw-r--r--  2.0 unx      325 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblleft.glif
--rw-r--r--  2.0 unx      546 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif
--rw-r--r--  2.0 unx     1462 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif
--rw-r--r--  2.0 unx     1372 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif
--rw-r--r--  2.0 unx     1728 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif
--rw-r--r--  2.0 unx     1136 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif
--rw-r--r--  2.0 unx     1966 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      230 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/colon.glif
--rw-r--r--  2.0 unx      798 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif
--rw-r--r--  2.0 unx      914 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif
--rw-r--r--  2.0 unx      739 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif
--rw-r--r--  2.0 unx      701 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      743 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif
--rw-r--r--  2.0 unx     1402 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif
--rw-r--r--  2.0 unx      349 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dot.glif
--rw-r--r--  2.0 unx      627 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif
--rw-r--r--  2.0 unx     1799 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif
--rw-r--r--  2.0 unx      929 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif
--rw-r--r--  2.0 unx      739 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx      736 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif
--rw-r--r--  2.0 unx      737 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif
--rw-r--r--  2.0 unx     1105 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      515 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif
--rw-r--r--  2.0 unx     2687 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      369 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dieresis.glif
--rw-r--r--  2.0 unx     1120 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif
--rw-r--r--  2.0 unx      377 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Q_.glif
--rw-r--r--  2.0 unx      154 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/space.glif
--rw-r--r--  2.0 unx      235 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblbase.glif
--rw-r--r--  2.0 unx      538 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblright.glif
--rw-r--r--  2.0 unx      352 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_acute.glif
--rw-r--r--  2.0 unx      628 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif
--rw-r--r--  2.0 unx     1146 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif
--rw-r--r--  2.0 unx      233 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/semicolon.glif
--rw-r--r--  2.0 unx      797 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif
--rw-r--r--  2.0 unx      358 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_dieresis.glif
--rw-r--r--  2.0 unx      690 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif
--rw-r--r--  2.0 unx      870 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif
--rw-r--r--  2.0 unx      942 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx      929 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif
--rw-r--r--  2.0 unx      741 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif
--rw-r--r--  2.0 unx     2453 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/acute.glif
--rw-r--r--  2.0 unx      371 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      350 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/period.glif
--rw-r--r--  2.0 unx      975 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif
--rw-r--r--  2.0 unx      193 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotesinglbase.glif
--rw-r--r--  2.0 unx      626 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif
--rw-r--r--  2.0 unx      238 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
--rw-r--r--  2.0 unx      183 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
--rw-r--r--  2.0 unx     1176 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
--rw-r--r--  2.0 unx     3543 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
--rw-r--r--  2.0 unx      298 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
--rw-r--r--  2.0 unx     3534 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
--rw-r--r--  2.0 unx      247 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/
--rw-r--r--  2.0 unx     5741 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace
--rw-r--r--  2.0 unx     5180 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace
--rw-r--r--  2.0 unx     5197 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace
--rw-r--r--  2.0 unx     1074 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/LICENSE
--rw-r--r--  2.0 unx     7158 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
--rw-r--r--  2.0 unx       37 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/features.fea
--rw-r--r--  2.0 unx      361 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1829 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx    16116 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist
--rw-r--r--  2.0 unx     1818 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx      240 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx      228 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
--rw-r--r--  2.0 unx     2537 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
--rw-r--r--  2.0 unx      341 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
--rw-r--r--  2.0 unx      181 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
--rw-r--r--  2.0 unx      237 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
--rw-r--r--  2.0 unx      228 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
--rw-r--r--  2.0 unx     2459 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
--rw-r--r--  2.0 unx      344 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
--rw-r--r--  2.0 unx     1831 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      654 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      691 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx     1065 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1222 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx     2188 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      181 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
--rw-r--r--  2.0 unx      236 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/
--rw-r--r--  2.0 unx       37 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/features.fea
--rw-r--r--  2.0 unx      271 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1834 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx    16116 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist
--rw-r--r--  2.0 unx      232 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1578 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/
--rw-r--r--  2.0 unx       42 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      361 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1841 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx     6839 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx     1849 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx      240 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     2099 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      652 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      689 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx     1057 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1221 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx     2197 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/
--rw-r--r--  2.0 unx       68 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      271 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1849 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx    16556 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx      232 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1228 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/
--rw-r--r--  2.0 unx       36 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/features.fea
--rw-r--r--  2.0 unx      361 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1826 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/metainfo.plist
--rw-r--r--  2.0 unx    10710 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist
--rw-r--r--  2.0 unx     1847 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      288 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     1865 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
--rw-r--r--  2.0 unx      240 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx     2192 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      652 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      690 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx     1062 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      879 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx     2206 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-20 10:52 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
--rw-r--r--  2.0 unx       68 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/features.fea
--rw-r--r--  2.0 unx      749 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist
--rw-r--r--  2.0 unx     1844 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/metainfo.plist
--rw-r--r--  2.0 unx    16556 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist
--rw-r--r--  2.0 unx     3539 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
--rw-r--r--  2.0 unx      288 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
--rw-r--r--  2.0 unx     2617 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
--rw-r--r--  2.0 unx      238 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
--rw-r--r--  2.0 unx      232 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
--rw-r--r--  2.0 unx     3007 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
--rw-r--r--  2.0 unx      241 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
--rw-r--r--  2.0 unx      274 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
--rw-r--r--  2.0 unx      732 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
--rw-r--r--  2.0 unx     2474 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
--rw-r--r--  2.0 unx     2492 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
--rw-r--r--  2.0 unx      246 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
--rw-r--r--  2.0 unx      240 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
--rw-r--r--  2.0 unx     1827 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
--rw-r--r--  2.0 unx      652 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
--rw-r--r--  2.0 unx      687 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif
--rw-r--r--  2.0 unx     1028 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
--rw-r--r--  2.0 unx      473 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx      874 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx     2247 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif
--rw-r--r--  2.0 unx      353 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
--rw-r--r--  2.0 unx      238 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
--rw-r--r--  2.0 unx      183 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
--rw-r--r--  2.0 unx     1176 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
--rw-r--r--  2.0 unx     3060 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
--rw-r--r--  2.0 unx      288 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
--rw-r--r--  2.0 unx     3051 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
--rw-r--r--  2.0 unx      241 b- defN 23-Jul-20 10:51 fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
-725 files, 1204720 bytes uncompressed, 296466 bytes compressed:  75.4%
+Zip file size: 474488 bytes, number of entries: 726
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/.github/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/
+-rw-r--r--  2.0 unx      910 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/requirements.txt
+-rw-r--r--  2.0 unx      226 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/setup.cfg
+-rwxr-xr-x  2.0 unx     1298 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/build_pyz.sh
+-rw-r--r--  2.0 unx     7349 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/PKG-INFO
+-rw-r--r--  2.0 unx     3193 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/TROUBLESHOOTING.md
+-rw-r--r--  2.0 unx     1453 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/.gitignore
+-rw-r--r--  2.0 unx      191 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/test_requirements.txt
+-rw-r--r--  2.0 unx      142 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/MANIFEST.in
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/LICENSE
+-rw-r--r--  2.0 unx    19601 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/USAGE.md
+-rw-r--r--  2.0 unx     6285 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/README.md
+-rw-r--r--  2.0 unx     3917 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/setup.py
+-rw-r--r--  2.0 unx      163 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/pyproject.toml
+-rw-r--r--  2.0 unx      806 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tox.ini
+-rw-r--r--  2.0 unx      792 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/.coveragerc
+-rw-r--r--  2.0 unx     1450 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/CONTRIBUTING.md
+-rw-r--r--  2.0 unx       77 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/.codecov.yml
+-rw-r--r--  2.0 unx      227 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/.editorconfig
+-rw-r--r--  2.0 unx      322 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/.gitattributes
+-rw-r--r--  2.0 unx      168 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/.pyup.yml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake.egg-info/
+-rw-r--r--  2.0 unx     3049 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake/compatibility.py
+-rw-r--r--  2.0 unx    32133 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake/instantiator.py
+-rw-r--r--  2.0 unx     1439 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake/errors.py
+-rw-r--r--  2.0 unx     3288 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake/ttfautohint.py
+-rw-r--r--  2.0 unx    61003 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake/font_project.py
+-rw-r--r--  2.0 unx      162 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake/_version.py
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake/__init__.py
+-rw-r--r--  2.0 unx    27227 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake/__main__.py
+-rw-r--r--  2.0 unx     7349 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake.egg-info/top_level.txt
+-rw-r--r--  2.0 unx    42266 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      768 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/Lib/fontmake.egg-info/entry_points.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/.github/workflows/
+-rw-r--r--  2.0 unx     4056 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/.github/workflows/ci.yml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/
+-rw-r--r--  2.0 unx      133 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/conftest.py
+-rw-r--r--  2.0 unx    25699 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/test_instantiator.py
+-rw-r--r--  2.0 unx    37281 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/test_main.py
+-rw-r--r--  2.0 unx     1668 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/test_compatibility.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/AutohintingTest/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/
+-rw-r--r--  2.0 unx     6386 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/TestSubset.glyphs
+-rw-r--r--  2.0 unx      150 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphData.xml
+-rw-r--r--  2.0 unx     6381 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/TestSubset2.glyphs
+-rw-r--r--  2.0 unx    31198 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans.glyphs
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/
+-rw-r--r--  2.0 unx     2035 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/
+-rw-r--r--  2.0 unx      275 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      887 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      360 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/lib.plist
+-rw-r--r--  2.0 unx     1455 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif
+-rw-r--r--  2.0 unx      412 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     1659 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx     1261 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif
+-rw-r--r--  2.0 unx     1265 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/
+-rw-r--r--  2.0 unx      275 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      890 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      360 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/lib.plist
+-rw-r--r--  2.0 unx     1439 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif
+-rw-r--r--  2.0 unx      412 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     1642 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx     1263 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif
+-rw-r--r--  2.0 unx     1263 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/
+-rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      471 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/groups.plist
+-rw-r--r--  2.0 unx      714 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/kerning.plist
+-rw-r--r--  2.0 unx      790 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      443 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/lib.plist
+-rw-r--r--  2.0 unx      382 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.glif
+-rw-r--r--  2.0 unx      522 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif
+-rw-r--r--  2.0 unx      393 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.swap.glif
+-rw-r--r--  2.0 unx      581 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif
+-rw-r--r--  2.0 unx      436 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.glif
+-rw-r--r--  2.0 unx      543 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      156 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      646 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/
+-rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      790 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      410 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/lib.plist
+-rw-r--r--  2.0 unx      898 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif
+-rw-r--r--  2.0 unx      487 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      539 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif
+-rw-r--r--  2.0 unx      205 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.alt.glif
+-rw-r--r--  2.0 unx      784 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif
+-rw-r--r--  2.0 unx      221 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/
+-rw-r--r--  2.0 unx    22772 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist
+-rw-r--r--  2.0 unx       83 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/order.plist
+-rw-r--r--  2.0 unx     1308 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph
+-rw-r--r--  2.0 unx      454 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_dieresis.glyph
+-rw-r--r--  2.0 unx     1580 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph
+-rw-r--r--  2.0 unx      764 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph
+-rw-r--r--  2.0 unx      902 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph
+-rw-r--r--  2.0 unx     1889 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph
+-rw-r--r--  2.0 unx     1026 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph
+-rw-r--r--  2.0 unx      445 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/adieresis.glyph
+-rw-r--r--  2.0 unx     5010 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph
+-rw-r--r--  2.0 unx     6165 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph
+-rw-r--r--  2.0 unx     2295 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufo/
+-rw-r--r--  2.0 unx      983 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest.designspace
+-rw-r--r--  2.0 unx     3057 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufoz
+-rw-r--r--  2.0 unx      852 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace
+-rw-r--r--  2.0 unx      614 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace
+-rw-r--r--  2.0 unx      621 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace
+-rw-r--r--  2.0 unx     1340 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace
+-rw-r--r--  2.0 unx      916 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace
+-rw-r--r--  2.0 unx     2253 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufoz
+-rw-r--r--  2.0 unx      745 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/
+-rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      357 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/groups.plist
+-rw-r--r--  2.0 unx      878 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      240 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/lib.plist
+-rw-r--r--  2.0 unx      343 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/l.glif
+-rw-r--r--  2.0 unx      237 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/contents.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/
+-rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      548 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      345 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/l.glif
+-rw-r--r--  2.0 unx      237 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/contents.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/
+-rw-r--r--  2.0 unx      830 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/
+-rw-r--r--  2.0 unx      283 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      897 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     1030 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist
+-rw-r--r--  2.0 unx      243 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      770 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif
+-rw-r--r--  2.0 unx      247 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/
+-rw-r--r--  2.0 unx      283 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      900 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     1030 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist
+-rw-r--r--  2.0 unx      243 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      786 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif
+-rw-r--r--  2.0 unx      247 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/
+-rw-r--r--  2.0 unx      983 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace
+-rw-r--r--  2.0 unx     1135 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/
+-rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      887 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      303 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/lib.plist
+-rw-r--r--  2.0 unx      343 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/l.glif
+-rw-r--r--  2.0 unx      288 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      479 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/asas.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/
+-rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      886 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      303 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/lib.plist
+-rw-r--r--  2.0 unx      345 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/l.glif
+-rw-r--r--  2.0 unx      288 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      425 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/asas.glif
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GSUB.txt
+-rw-r--r--  2.0 unx      716 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist
+-rw-r--r--  2.0 unx       73 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GDEF.txt
+-rw-r--r--  2.0 unx      249 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 1000 GPOS.txt
+-rw-r--r--  2.0 unx     6904 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs
+-rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 0 GPOS.txt
+-rw-r--r--  2.0 unx   125360 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/AutohintingTest/Padyakke.glyphs
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/
+-rw-r--r--  2.0 unx      762 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/
+-rw-r--r--  2.0 unx      101 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/features.fea
+-rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1158 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     2113 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist
+-rw-r--r--  2.0 unx      694 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx      215 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx      560 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      429 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      154 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx     1196 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/
+-rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1160 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     2107 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist
+-rw-r--r--  2.0 unx      652 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx      217 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx      652 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      429 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      154 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      893 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/family.fea
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/features.fea
+-rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      899 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      183 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/contents.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/
+-rw-r--r--  2.0 unx      287 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      897 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      183 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/contents.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/
+-rw-r--r--  2.0 unx     8462 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans_missing.designspace
+-rw-r--r--  2.0 unx     7111 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans.designspace
+-rw-r--r--  2.0 unx     1394 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans-width-only.designspace
+-rw-r--r--  2.0 unx     2611 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace
+-rw-r--r--  2.0 unx     1412 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans-weight-only.designspace
+-rw-r--r--  2.0 unx     1067 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace
+-rw-r--r--  2.0 unx     1074 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/LICENSE
+-rw-r--r--  2.0 unx     7834 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans_no_default.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
+-rw-r--r--  2.0 unx       37 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/features.fea
+-rw-r--r--  2.0 unx      383 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      366 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/groups.plist
+-rw-r--r--  2.0 unx     4852 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist
+-rw-r--r--  2.0 unx     1873 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx    18291 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist
+-rw-r--r--  2.0 unx     1965 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      252 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx      228 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
+-rw-r--r--  2.0 unx     2537 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
+-rw-r--r--  2.0 unx      341 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
+-rw-r--r--  2.0 unx      181 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
+-rw-r--r--  2.0 unx      237 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
+-rw-r--r--  2.0 unx      228 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
+-rw-r--r--  2.0 unx     2459 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
+-rw-r--r--  2.0 unx      344 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
+-rw-r--r--  2.0 unx      857 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif
+-rw-r--r--  2.0 unx      325 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblleft.glif
+-rw-r--r--  2.0 unx      549 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif
+-rw-r--r--  2.0 unx     1459 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif
+-rw-r--r--  2.0 unx     1388 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif
+-rw-r--r--  2.0 unx     1751 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx     1134 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx     1970 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      230 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/colon.glif
+-rw-r--r--  2.0 unx      801 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif
+-rw-r--r--  2.0 unx      924 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif
+-rw-r--r--  2.0 unx      752 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif
+-rw-r--r--  2.0 unx      703 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx      954 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx     1416 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx      349 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dot.glif
+-rw-r--r--  2.0 unx      518 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif
+-rw-r--r--  2.0 unx     1785 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      943 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif
+-rw-r--r--  2.0 unx      743 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx      749 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif
+-rw-r--r--  2.0 unx      740 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif
+-rw-r--r--  2.0 unx     1158 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      521 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif
+-rw-r--r--  2.0 unx     2687 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      370 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dieresis.glif
+-rw-r--r--  2.0 unx      747 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif
+-rw-r--r--  2.0 unx      378 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      235 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblbase.glif
+-rw-r--r--  2.0 unx      542 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif
+-rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblright.glif
+-rw-r--r--  2.0 unx      354 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_acute.glif
+-rw-r--r--  2.0 unx      514 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif
+-rw-r--r--  2.0 unx     1130 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif
+-rw-r--r--  2.0 unx      233 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/semicolon.glif
+-rw-r--r--  2.0 unx      802 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif
+-rw-r--r--  2.0 unx      360 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_dieresis.glif
+-rw-r--r--  2.0 unx      518 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif
+-rw-r--r--  2.0 unx      875 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif
+-rw-r--r--  2.0 unx     1320 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx     1056 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif
+-rw-r--r--  2.0 unx      750 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif
+-rw-r--r--  2.0 unx     2358 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/acute.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      352 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/period.glif
+-rw-r--r--  2.0 unx     1357 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx      193 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--  2.0 unx      517 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif
+-rw-r--r--  2.0 unx      181 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
+-rw-r--r--  2.0 unx      236 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/
+-rw-r--r--  2.0 unx       68 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      615 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1386 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx    16617 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx      228 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx     2353 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif
+-rw-r--r--  2.0 unx      343 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx      268 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/contents.plist
+-rw-r--r--  2.0 unx     3181 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif
+-rw-r--r--  2.0 unx      341 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/layerinfo.plist
+-rw-r--r--  2.0 unx      950 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif
+-rw-r--r--  2.0 unx     2307 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx      923 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx     1806 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      422 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     2646 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      983 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx      228 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/contents.plist
+-rw-r--r--  2.0 unx      344 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/layerinfo.plist
+-rw-r--r--  2.0 unx     1938 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/
+-rw-r--r--  2.0 unx       42 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      383 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      366 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/groups.plist
+-rw-r--r--  2.0 unx     4580 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist
+-rw-r--r--  2.0 unx     1885 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     7840 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx     1988 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      252 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx      858 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif
+-rw-r--r--  2.0 unx      325 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblleft.glif
+-rw-r--r--  2.0 unx      546 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif
+-rw-r--r--  2.0 unx     1829 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif
+-rw-r--r--  2.0 unx     1359 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif
+-rw-r--r--  2.0 unx     1774 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx     1128 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx     2285 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      242 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/colon.glif
+-rw-r--r--  2.0 unx      800 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif
+-rw-r--r--  2.0 unx      915 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif
+-rw-r--r--  2.0 unx      744 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif
+-rw-r--r--  2.0 unx      701 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx      747 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx     1785 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx      351 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dot.glif
+-rw-r--r--  2.0 unx      491 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowright.glif
+-rw-r--r--  2.0 unx     1799 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      936 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif
+-rw-r--r--  2.0 unx      741 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx      741 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif
+-rw-r--r--  2.0 unx      740 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif
+-rw-r--r--  2.0 unx     1137 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      521 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif
+-rw-r--r--  2.0 unx     2687 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      384 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dieresis.glif
+-rw-r--r--  2.0 unx      748 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif
+-rw-r--r--  2.0 unx      379 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      608 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif
+-rw-r--r--  2.0 unx      542 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif
+-rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblright.glif
+-rw-r--r--  2.0 unx      340 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_acute.glif
+-rw-r--r--  2.0 unx      491 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowdown.glif
+-rw-r--r--  2.0 unx     1204 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif
+-rw-r--r--  2.0 unx      245 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/semicolon.glif
+-rw-r--r--  2.0 unx      825 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif
+-rw-r--r--  2.0 unx      346 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_dieresis.glif
+-rw-r--r--  2.0 unx      490 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowleft.glif
+-rw-r--r--  2.0 unx      872 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif
+-rw-r--r--  2.0 unx     1319 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx      936 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif
+-rw-r--r--  2.0 unx      743 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif
+-rw-r--r--  2.0 unx     2367 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/acute.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      350 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/period.glif
+-rw-r--r--  2.0 unx     1382 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx      566 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--  2.0 unx      490 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowup.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/
+-rw-r--r--  2.0 unx       68 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/features.fea
+-rw-r--r--  2.0 unx      383 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     5462 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist
+-rw-r--r--  2.0 unx     1384 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx    16223 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist
+-rw-r--r--  2.0 unx      228 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx     2396 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif
+-rw-r--r--  2.0 unx      343 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     2148 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx      911 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx     1824 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      376 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      371 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx     1162 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/
+-rw-r--r--  2.0 unx       36 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/features.fea
+-rw-r--r--  2.0 unx      383 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      366 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/groups.plist
+-rw-r--r--  2.0 unx      301 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/kerning.plist
+-rw-r--r--  2.0 unx     1870 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx    12341 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist
+-rw-r--r--  2.0 unx     1986 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      298 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx     2005 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
+-rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx      861 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif
+-rw-r--r--  2.0 unx      325 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblleft.glif
+-rw-r--r--  2.0 unx      549 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif
+-rw-r--r--  2.0 unx     1495 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif
+-rw-r--r--  2.0 unx     1387 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif
+-rw-r--r--  2.0 unx     1747 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx     1150 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx     2369 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      242 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/colon.glif
+-rw-r--r--  2.0 unx      803 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif
+-rw-r--r--  2.0 unx      919 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif
+-rw-r--r--  2.0 unx      750 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif
+-rw-r--r--  2.0 unx      701 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx      750 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx     1418 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx      351 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dot.glif
+-rw-r--r--  2.0 unx      495 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowright.glif
+-rw-r--r--  2.0 unx     2203 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx     1037 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif
+-rw-r--r--  2.0 unx      742 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx      745 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif
+-rw-r--r--  2.0 unx      742 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif
+-rw-r--r--  2.0 unx     1154 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      522 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif
+-rw-r--r--  2.0 unx     2687 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      370 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dieresis.glif
+-rw-r--r--  2.0 unx      750 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif
+-rw-r--r--  2.0 unx      380 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      259 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblbase.glif
+-rw-r--r--  2.0 unx      545 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif
+-rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblright.glif
+-rw-r--r--  2.0 unx      354 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_acute.glif
+-rw-r--r--  2.0 unx      491 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowdown.glif
+-rw-r--r--  2.0 unx     1140 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif
+-rw-r--r--  2.0 unx      245 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/semicolon.glif
+-rw-r--r--  2.0 unx      806 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif
+-rw-r--r--  2.0 unx      360 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_dieresis.glif
+-rw-r--r--  2.0 unx      493 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowleft.glif
+-rw-r--r--  2.0 unx      875 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif
+-rw-r--r--  2.0 unx      947 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx      940 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif
+-rw-r--r--  2.0 unx      748 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif
+-rw-r--r--  2.0 unx     2376 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/acute.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      350 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/period.glif
+-rw-r--r--  2.0 unx      988 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx      205 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--  2.0 unx      492 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowup.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
+-rw-r--r--  2.0 unx       68 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      811 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx      491 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/groups.plist
+-rw-r--r--  2.0 unx      517 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist
+-rw-r--r--  2.0 unx     1888 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx    18792 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx     3998 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      298 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx     3358 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
+-rw-r--r--  2.0 unx      244 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     2452 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif
+-rw-r--r--  2.0 unx      422 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.closed.glif
+-rw-r--r--  2.0 unx      751 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif
+-rw-r--r--  2.0 unx     2111 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif
+-rw-r--r--  2.0 unx      482 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
+-rw-r--r--  2.0 unx     3498 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
+-rw-r--r--  2.0 unx      247 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
+-rw-r--r--  2.0 unx     1471 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif
+-rw-r--r--  2.0 unx      853 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif
+-rw-r--r--  2.0 unx      330 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
+-rw-r--r--  2.0 unx      828 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
+-rw-r--r--  2.0 unx     2706 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
+-rw-r--r--  2.0 unx     2825 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
+-rw-r--r--  2.0 unx      252 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
+-rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
+-rw-r--r--  2.0 unx      853 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif
+-rw-r--r--  2.0 unx      325 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblleft.glif
+-rw-r--r--  2.0 unx      546 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif
+-rw-r--r--  2.0 unx     1462 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif
+-rw-r--r--  2.0 unx     1372 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif
+-rw-r--r--  2.0 unx     1728 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif
+-rw-r--r--  2.0 unx     1136 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif
+-rw-r--r--  2.0 unx     1966 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      230 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/colon.glif
+-rw-r--r--  2.0 unx      798 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif
+-rw-r--r--  2.0 unx      914 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif
+-rw-r--r--  2.0 unx      739 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif
+-rw-r--r--  2.0 unx      701 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx      743 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif
+-rw-r--r--  2.0 unx     1402 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif
+-rw-r--r--  2.0 unx      349 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dot.glif
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif
+-rw-r--r--  2.0 unx     1799 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif
+-rw-r--r--  2.0 unx      929 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif
+-rw-r--r--  2.0 unx      739 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx      736 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif
+-rw-r--r--  2.0 unx      737 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif
+-rw-r--r--  2.0 unx     1105 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      515 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif
+-rw-r--r--  2.0 unx     2687 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      369 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dieresis.glif
+-rw-r--r--  2.0 unx     1120 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif
+-rw-r--r--  2.0 unx      377 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Q_.glif
+-rw-r--r--  2.0 unx      154 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/space.glif
+-rw-r--r--  2.0 unx      235 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblbase.glif
+-rw-r--r--  2.0 unx      538 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif
+-rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblright.glif
+-rw-r--r--  2.0 unx      352 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_acute.glif
+-rw-r--r--  2.0 unx      628 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif
+-rw-r--r--  2.0 unx     1146 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif
+-rw-r--r--  2.0 unx      233 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/semicolon.glif
+-rw-r--r--  2.0 unx      797 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif
+-rw-r--r--  2.0 unx      358 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_dieresis.glif
+-rw-r--r--  2.0 unx      690 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif
+-rw-r--r--  2.0 unx      870 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif
+-rw-r--r--  2.0 unx      942 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx      929 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif
+-rw-r--r--  2.0 unx      741 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif
+-rw-r--r--  2.0 unx     2453 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/acute.glif
+-rw-r--r--  2.0 unx      371 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      350 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/period.glif
+-rw-r--r--  2.0 unx      975 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif
+-rw-r--r--  2.0 unx      193 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotesinglbase.glif
+-rw-r--r--  2.0 unx      626 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif
+-rw-r--r--  2.0 unx      238 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
+-rw-r--r--  2.0 unx      183 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
+-rw-r--r--  2.0 unx     1176 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
+-rw-r--r--  2.0 unx     3543 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
+-rw-r--r--  2.0 unx      298 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
+-rw-r--r--  2.0 unx     3534 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
+-rw-r--r--  2.0 unx      247 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/
+-rw-r--r--  2.0 unx     5741 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace
+-rw-r--r--  2.0 unx     5180 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace
+-rw-r--r--  2.0 unx     5197 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace
+-rw-r--r--  2.0 unx     1074 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/LICENSE
+-rw-r--r--  2.0 unx     7158 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
+-rw-r--r--  2.0 unx       37 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/features.fea
+-rw-r--r--  2.0 unx      361 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1829 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx    16116 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist
+-rw-r--r--  2.0 unx     1818 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      240 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx      228 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
+-rw-r--r--  2.0 unx     2537 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
+-rw-r--r--  2.0 unx      341 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
+-rw-r--r--  2.0 unx      181 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
+-rw-r--r--  2.0 unx      237 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
+-rw-r--r--  2.0 unx      228 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
+-rw-r--r--  2.0 unx     2459 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
+-rw-r--r--  2.0 unx      344 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
+-rw-r--r--  2.0 unx     1831 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      654 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx      691 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     1222 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx     2188 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      181 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
+-rw-r--r--  2.0 unx      236 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/
+-rw-r--r--  2.0 unx       37 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/features.fea
+-rw-r--r--  2.0 unx      271 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1834 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx    16116 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist
+-rw-r--r--  2.0 unx      232 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     1578 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/
+-rw-r--r--  2.0 unx       42 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      361 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1841 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx     6839 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx     1849 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx      240 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     2099 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      652 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx      689 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx     1057 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     1221 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx     2197 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/
+-rw-r--r--  2.0 unx       68 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      271 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1849 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx    16556 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx      232 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     1228 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/
+-rw-r--r--  2.0 unx       36 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/features.fea
+-rw-r--r--  2.0 unx      361 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1826 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/metainfo.plist
+-rw-r--r--  2.0 unx    10710 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist
+-rw-r--r--  2.0 unx     1847 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      288 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
+-rw-r--r--  2.0 unx      240 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx     2192 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      652 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx      690 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx     1062 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      879 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx     2206 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
+-rw-r--r--  2.0 unx       68 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/features.fea
+-rw-r--r--  2.0 unx      749 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     1844 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/metainfo.plist
+-rw-r--r--  2.0 unx    16556 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist
+-rw-r--r--  2.0 unx     3539 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
+-rw-r--r--  2.0 unx      288 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
+-rw-r--r--  2.0 unx     2617 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
+-rw-r--r--  2.0 unx      238 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
+-rw-r--r--  2.0 unx      232 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
+-rw-r--r--  2.0 unx     3007 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
+-rw-r--r--  2.0 unx      241 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
+-rw-r--r--  2.0 unx      274 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
+-rw-r--r--  2.0 unx      732 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
+-rw-r--r--  2.0 unx     2474 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
+-rw-r--r--  2.0 unx     2492 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
+-rw-r--r--  2.0 unx      246 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
+-rw-r--r--  2.0 unx      240 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
+-rw-r--r--  2.0 unx     1827 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
+-rw-r--r--  2.0 unx      652 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
+-rw-r--r--  2.0 unx      687 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif
+-rw-r--r--  2.0 unx     1028 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
+-rw-r--r--  2.0 unx      473 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx      874 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx     2247 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif
+-rw-r--r--  2.0 unx      353 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
+-rw-r--r--  2.0 unx      238 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
+-rw-r--r--  2.0 unx      183 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
+-rw-r--r--  2.0 unx     1176 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
+-rw-r--r--  2.0 unx     3060 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
+-rw-r--r--  2.0 unx      288 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
+-rw-r--r--  2.0 unx     3051 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
+-rw-r--r--  2.0 unx      241 b- defN 23-Jul-31 17:08 fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
+726 files, 1215531 bytes uncompressed, 299784 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -1,2176 +1,2179 @@
-Filename: fontmake-3.6.1/
+Filename: fontmake-3.7.0b1/
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/
+Filename: fontmake-3.7.0b1/Lib/
 Comment: 
 
-Filename: fontmake-3.6.1/.github/
+Filename: fontmake-3.7.0b1/.github/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/
+Filename: fontmake-3.7.0b1/tests/
 Comment: 
 
-Filename: fontmake-3.6.1/requirements.txt
+Filename: fontmake-3.7.0b1/requirements.txt
 Comment: 
 
-Filename: fontmake-3.6.1/setup.cfg
+Filename: fontmake-3.7.0b1/setup.cfg
 Comment: 
 
-Filename: fontmake-3.6.1/build_pyz.sh
+Filename: fontmake-3.7.0b1/build_pyz.sh
 Comment: 
 
-Filename: fontmake-3.6.1/PKG-INFO
+Filename: fontmake-3.7.0b1/PKG-INFO
 Comment: 
 
-Filename: fontmake-3.6.1/TROUBLESHOOTING.md
+Filename: fontmake-3.7.0b1/TROUBLESHOOTING.md
 Comment: 
 
-Filename: fontmake-3.6.1/.gitignore
+Filename: fontmake-3.7.0b1/.gitignore
 Comment: 
 
-Filename: fontmake-3.6.1/test_requirements.txt
+Filename: fontmake-3.7.0b1/test_requirements.txt
 Comment: 
 
-Filename: fontmake-3.6.1/MANIFEST.in
+Filename: fontmake-3.7.0b1/MANIFEST.in
 Comment: 
 
-Filename: fontmake-3.6.1/LICENSE
+Filename: fontmake-3.7.0b1/LICENSE
 Comment: 
 
-Filename: fontmake-3.6.1/USAGE.md
+Filename: fontmake-3.7.0b1/USAGE.md
 Comment: 
 
-Filename: fontmake-3.6.1/README.md
+Filename: fontmake-3.7.0b1/README.md
 Comment: 
 
-Filename: fontmake-3.6.1/setup.py
+Filename: fontmake-3.7.0b1/setup.py
 Comment: 
 
-Filename: fontmake-3.6.1/pyproject.toml
+Filename: fontmake-3.7.0b1/pyproject.toml
 Comment: 
 
-Filename: fontmake-3.6.1/tox.ini
+Filename: fontmake-3.7.0b1/tox.ini
 Comment: 
 
-Filename: fontmake-3.6.1/.coveragerc
+Filename: fontmake-3.7.0b1/.coveragerc
 Comment: 
 
-Filename: fontmake-3.6.1/CONTRIBUTING.md
+Filename: fontmake-3.7.0b1/CONTRIBUTING.md
 Comment: 
 
-Filename: fontmake-3.6.1/.codecov.yml
+Filename: fontmake-3.7.0b1/.codecov.yml
 Comment: 
 
-Filename: fontmake-3.6.1/.editorconfig
+Filename: fontmake-3.7.0b1/.editorconfig
 Comment: 
 
-Filename: fontmake-3.6.1/.gitattributes
+Filename: fontmake-3.7.0b1/.gitattributes
 Comment: 
 
-Filename: fontmake-3.6.1/.pyup.yml
+Filename: fontmake-3.7.0b1/.pyup.yml
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake/
+Filename: fontmake-3.7.0b1/Lib/fontmake/
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake.egg-info/
+Filename: fontmake-3.7.0b1/Lib/fontmake.egg-info/
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake/compatibility.py
+Filename: fontmake-3.7.0b1/Lib/fontmake/compatibility.py
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake/instantiator.py
+Filename: fontmake-3.7.0b1/Lib/fontmake/instantiator.py
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake/errors.py
+Filename: fontmake-3.7.0b1/Lib/fontmake/errors.py
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake/ttfautohint.py
+Filename: fontmake-3.7.0b1/Lib/fontmake/ttfautohint.py
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake/font_project.py
+Filename: fontmake-3.7.0b1/Lib/fontmake/font_project.py
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake/_version.py
+Filename: fontmake-3.7.0b1/Lib/fontmake/_version.py
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake/__init__.py
+Filename: fontmake-3.7.0b1/Lib/fontmake/__init__.py
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake/__main__.py
+Filename: fontmake-3.7.0b1/Lib/fontmake/__main__.py
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake.egg-info/PKG-INFO
+Filename: fontmake-3.7.0b1/Lib/fontmake.egg-info/PKG-INFO
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake.egg-info/top_level.txt
+Filename: fontmake-3.7.0b1/Lib/fontmake.egg-info/top_level.txt
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake.egg-info/SOURCES.txt
+Filename: fontmake-3.7.0b1/Lib/fontmake.egg-info/SOURCES.txt
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake.egg-info/requires.txt
+Filename: fontmake-3.7.0b1/Lib/fontmake.egg-info/requires.txt
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake.egg-info/dependency_links.txt
+Filename: fontmake-3.7.0b1/Lib/fontmake.egg-info/dependency_links.txt
 Comment: 
 
-Filename: fontmake-3.6.1/Lib/fontmake.egg-info/entry_points.txt
+Filename: fontmake-3.7.0b1/Lib/fontmake.egg-info/entry_points.txt
 Comment: 
 
-Filename: fontmake-3.6.1/.github/workflows/
+Filename: fontmake-3.7.0b1/.github/workflows/
 Comment: 
 
-Filename: fontmake-3.6.1/.github/workflows/ci.yml
+Filename: fontmake-3.7.0b1/.github/workflows/ci.yml
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/
+Filename: fontmake-3.7.0b1/tests/data/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/conftest.py
+Filename: fontmake-3.7.0b1/tests/conftest.py
 Comment: 
 
-Filename: fontmake-3.6.1/tests/test_instantiator.py
+Filename: fontmake-3.7.0b1/tests/test_instantiator.py
 Comment: 
 
-Filename: fontmake-3.6.1/tests/test_main.py
+Filename: fontmake-3.7.0b1/tests/test_main.py
 Comment: 
 
-Filename: fontmake-3.6.1/tests/test_compatibility.py
+Filename: fontmake-3.7.0b1/tests/test_compatibility.py
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InterpolateLayoutTest/
+Filename: fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/AutohintingTest/
+Filename: fontmake-3.7.0b1/tests/data/AutohintingTest/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/TestSubset.glyphs
+Filename: fontmake-3.7.0b1/tests/data/TestSubset.glyphs
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/TestSubset2.glyphs
+Filename: fontmake-3.7.0b1/tests/data/GlyphData.xml
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans.glyphs
+Filename: fontmake-3.7.0b1/tests/data/TestSubset2.glyphs
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans.glyphs
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont.designspace
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/groups.plist
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/kerning.plist
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.glif
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.swap.glif
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/aaa.swap.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.glif
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/space.glif
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.alt.glif
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.alt.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.glif
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/adieresis.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/order.plist
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/order.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_dieresis.glyph
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_dieresis.glyph
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/adieresis.glyph
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/adieresis.glyph
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/
+Filename: fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest.designspace
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufoz
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufoz
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufoz
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufoz
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/groups.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/l.glif
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/l.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/l.glif
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/l.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/
+Filename: fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/l.glif
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/l.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/asas.glif
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/glyphs/asas.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/l.glif
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/l.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/asas.glif
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GSUB.txt
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/glyphs/asas.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist
+Filename: fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GSUB.txt
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GDEF.txt
+Filename: fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 1000 GPOS.txt
+Filename: fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest GDEF.txt
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs
+Filename: fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 1000 GPOS.txt
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 0 GPOS.txt
+Filename: fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/AutohintingTest/Padyakke.glyphs
+Filename: fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest 0 GPOS.txt
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/
+Filename: fontmake-3.7.0b1/tests/data/AutohintingTest/Padyakke.glyphs
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans.designspace
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/features.fea
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/C_.glif
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/space.glif
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/C_.glif
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/space.glif
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/
+Filename: fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/family.fea
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/family.fea
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/features.fea
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/
+Filename: fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSans_missing.designspace
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSans.designspace
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans_missing.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSans-width-only.designspace
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans-width-only.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSans-weight-only.designspace
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans-weight-only.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/LICENSE
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSans_no_default.designspace
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/LICENSE
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans_no_default.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/features.fea
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/groups.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblleft.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblleft.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/colon.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/colon.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dot.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dot.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dieresis.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/dieresis.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Q_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/space.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblbase.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblbase.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblright.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_acute.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotedblright.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_acute.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/semicolon.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/semicolon.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_dieresis.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_dieresis.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/acute.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/acute.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/period.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/period.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotesinglbase.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/quotesinglbase.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/features.fea
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/features.fea
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/groups.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblleft.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblleft.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/colon.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/colon.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dot.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowright.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dot.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowright.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dieresis.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/dieresis.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Q_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/space.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblright.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_acute.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblright.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowdown.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_acute.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowdown.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/semicolon.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/semicolon.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_dieresis.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowleft.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_dieresis.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowleft.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/acute.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/acute.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/period.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/period.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowup.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/arrowup.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/features.fea
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/features.fea
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/groups.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/kerning.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblleft.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblleft.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/colon.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/colon.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dot.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowright.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dot.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowright.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dieresis.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/dieresis.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Q_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/space.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblbase.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblbase.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblright.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_acute.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotedblright.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowdown.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_acute.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowdown.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/semicolon.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/semicolon.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_dieresis.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowleft.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_dieresis.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowleft.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/acute.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/acute.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/period.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/period.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotesinglbase.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowup.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/quotesinglbase.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/arrowup.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/features.fea
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/groups.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/groups.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblleft.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblleft.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/colon.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/colon.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dot.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dot.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dieresis.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/dieresis.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Q_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/space.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Q_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblbase.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/space.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblbase.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblright.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_acute.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotedblright.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_acute.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/semicolon.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/semicolon.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_dieresis.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_dieresis.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/acute.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/acute.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/period.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/period.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotesinglbase.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/quotesinglbase.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/LICENSE
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/LICENSE
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/features.fea
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_0.00_weight_0.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_695.65_weight_166.38/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/features.fea
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/features.fea
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/features.fea
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/features.fea
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/features.fea
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/features.fea
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/metainfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/metainfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/layerinfo.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/contents.plist
 Comment: 
 
-Filename: fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif
+Comment: 
+
+Filename: fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/layerinfo.plist
 Comment: 
 
 Zip file comment:
```

## Comparing `fontmake-3.6.1/build_pyz.sh` & `fontmake-3.7.0b1/build_pyz.sh`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/PKG-INFO` & `fontmake-3.7.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fontmake
-Version: 3.6.1
+Version: 3.7.0b1
 Summary: Compile fonts from sources (UFO, Glyphs) to binary (OpenType, TrueType).
 Home-page: https://github.com/googlei18n/fontmake
 License: Apache Software License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,14 +18,16 @@
 Classifier: Topic :: Text Processing :: Fonts
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pathops
 Provides-Extra: lxml
 Provides-Extra: mutatormath
 Provides-Extra: autohint
+Provides-Extra: json
+Provides-Extra: repacker
 Provides-Extra: all
 License-File: LICENSE
 
 ![GitHub Actions Build Status][] ![Python Versions][] [![PyPI
 Version][]][1]
 
 # fontmake
```

## Comparing `fontmake-3.6.1/TROUBLESHOOTING.md` & `fontmake-3.7.0b1/TROUBLESHOOTING.md`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/.gitignore` & `fontmake-3.7.0b1/.gitignore`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/LICENSE` & `fontmake-3.7.0b1/LICENSE`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/USAGE.md` & `fontmake-3.7.0b1/USAGE.md`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/README.md` & `fontmake-3.7.0b1/README.md`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/setup.py` & `fontmake-3.7.0b1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,26 +23,66 @@
 
 needs_wheel = {"bdist_wheel"}.intersection(sys.argv)
 wheel = ["wheel"] if needs_wheel else []
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
+
+dep_versions = {
+    "attrs": ">=19",
+    "fontMath": ">=0.9.3",
+    "fonttools": ">=4.41.1",
+    "glyphsLib": ">=6.2.5",
+    "ufo2ft": ">=2.33.2",
+    "ufoLib2": ">=0.16.0",
+}
+
+dep_extras = {
+    "fonttools": {
+        "implementation_name == 'cpython'": "ufo,lxml,unicode",
+        "implementation_name != 'cpython'": "ufo,unicode",
+    },
+    "ufo2ft": "compreffor",
+}
+
 extras_require = {
     "pathops": ["skia-pathops>=0.3.0"],
     # this is now default; kept here for backward compatibility
-    "lxml": [
-        # "lxml>=4.2.4",
-    ],
-    "mutatormath": ["MutatorMath>=2.1.2"],
+    "lxml": [],
+    # MutatorMath is no longer supported but a dummy extras is kept below
+    # to avoid fontmake installation failing if requested
+    "mutatormath": [],
     "autohint": ["ttfautohint-py>=0.5.0"],
+    # For reading/writing ufoLib2's .ufo.json files (cattrs + orjson)
+    "json": [f"ufoLib2[json]{dep_versions['ufoLib2']}"],
+    # For compiling GPOS/GSUB using the harfbuzz repacker
+    "repacker": [
+        f"fonttools[{extras},repacker]{dep_versions['fonttools']}; {marker}"
+        for marker, extras in dep_extras["fonttools"].items()
+    ],
 }
 # use a special 'all' key as shorthand to includes all the extra dependencies
 extras_require["all"] = sum(extras_require.values(), [])
 
+install_requires = [
+    f"{name}{version}"
+    for name, version in dep_versions.items()
+    if name not in dep_extras
+]
+for name, extras in dep_extras.items():
+    if isinstance(extras, dict):
+        for marker, ext in extras.items():
+            install_requires.append(f"{name}[{ext}]{dep_versions[name]}; {marker}")
+    elif isinstance(extras, str):
+        install_requires.append(f"{name}[{extras}]{dep_versions[name]}")
+    else:
+        raise TypeError(type(extras))
+
+
 setup(
     name="fontmake",
     use_scm_version={"write_to": "Lib/fontmake/_version.py"},
     description=(
         "Compile fonts from sources (UFO, Glyphs) to binary (OpenType, TrueType)."
     ),
     long_description=long_description,
@@ -50,23 +90,15 @@
     url="https://github.com/googlei18n/fontmake",
     license="Apache Software License 2.0",
     packages=find_packages("Lib"),
     package_dir={"": "Lib"},
     entry_points={"console_scripts": ["fontmake = fontmake.__main__:main"]},
     setup_requires=wheel + ["setuptools_scm"],
     python_requires=">=3.8",
-    install_requires=[
-        "fonttools[ufo,lxml,unicode]>=4.40.0 ; implementation_name == 'cpython'",
-        "fonttools[ufo,unicode]>=4.40.0 ; implementation_name != 'cpython'",
-        "glyphsLib>=6.2.5",
-        "ufo2ft[compreffor]>=2.32.0",
-        "fontMath>=0.9.3",
-        "ufoLib2>=0.14.0",
-        "attrs>=19",
-    ],
+    install_requires=install_requires,
     extras_require=extras_require,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
```

## Comparing `fontmake-3.6.1/tox.ini` & `fontmake-3.7.0b1/tox.ini`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/.coveragerc` & `fontmake-3.7.0b1/.coveragerc`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/CONTRIBUTING.md` & `fontmake-3.7.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/Lib/fontmake/compatibility.py` & `fontmake-3.7.0b1/Lib/fontmake/compatibility.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/Lib/fontmake/instantiator.py` & `fontmake-3.7.0b1/Lib/fontmake/instantiator.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/Lib/fontmake/errors.py` & `fontmake-3.7.0b1/Lib/fontmake/errors.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/Lib/fontmake/ttfautohint.py` & `fontmake-3.7.0b1/Lib/fontmake/ttfautohint.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/Lib/fontmake/font_project.py` & `fontmake-3.7.0b1/Lib/fontmake/font_project.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,32 +10,33 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+import enum
 import glob
 import logging
 import math
 import os
 import shutil
 import tempfile
 from collections import OrderedDict
-from contextlib import contextmanager
 from functools import partial
 from pathlib import Path
 from re import fullmatch
 
 import attr
 import ufo2ft
 import ufo2ft.errors
 import ufoLib2
 from fontTools import designspaceLib
 from fontTools.designspaceLib.split import splitInterpolable
+from fontTools.misc.cliTools import makeOutputFileName
 from fontTools.misc.loggingTools import Timer
 from fontTools.misc.plistlib import load as readPlist
 from fontTools.ttLib import TTFont
 from fontTools.varLib.interpolate_layout import interpolate_layout
 from ufo2ft import CFFOptimization
 from ufo2ft.featureCompiler import parseLayoutFeatures
 from ufo2ft.featureWriters import FEATURE_WRITERS_KEY, loadFeatureWriters
@@ -69,55 +70,53 @@
     ["ttf-interpolatable", "otf-interpolatable", "variable", "variable-cff2"]
 )
 
 AUTOHINTING_PARAMETERS = (
     GLYPHS_PREFIX + "customParameter.InstanceDescriptorAsGSInstance.TTFAutohint options"
 )
 
+# tempLib keys for fontmake's internal use only, won't be saved to disk
+INSTANCE_LOCATION_KEY = "com.github.googlefonts.fontmake.instance_location"
+INSTANCE_FILENAME_KEY = "com.github.googlefonts.fontmake.instance_filename"
+
+
+UFO_STRUCTURE_EXTENSIONS = {
+    "package": ".ufo",
+    "zip": ".ufoz",
+    "json": ".ufo.json",
+}
+
+
+class CurveConversion(enum.Enum):
+    # convert all cubic Bezier curves to quadratic splines: glyf format 0
+    ALL_CUBIC_TO_QUAD = "cu2qu"
+    # convert cubic curves to quadratic when more economical: glyf format 1
+    MIXED_CUBIC_TO_QUAD = "mixed"
+    # skip conversion, treat original curves as quadratic: glyf format 0
+    KEEP_QUAD = "keep-quad"
+    # skip conversion, treat original curves as cubic or mixed: glyf format 1
+    KEEP_CUBIC = "keep-cubic"
+
+    @classmethod
+    def default(cls):
+        return cls.ALL_CUBIC_TO_QUAD
+
+    @property
+    def convertCubics(self):
+        return self in (
+            CurveConversion.ALL_CUBIC_TO_QUAD,
+            CurveConversion.MIXED_CUBIC_TO_QUAD,
+        )
 
-@contextmanager
-def temporarily_disabling_axis_maps(designspace_path):
-    """Context manager to prevent MutatorMath from warping designspace locations.
-
-    MutatorMath assumes that the masters and instances' locations are in
-    user-space coordinates -- whereas they actually are in internal design-space
-    coordinates, and thus they do not need any 'bending'. To work around this we
-    we create a temporary designspace document without the axis maps, and with the
-    min/default/max triplet mapped "forward" from user-space coordinates (input)
-    to internal designspace coordinates (output).
-
-    Args:
-        designspace_path: A path to a designspace document.
-
-    Yields:
-        A temporary path string to the thus modified designspace document.
-        After the context is exited, it removes the temporary file.
-
-    Related issues:
-        https://github.com/LettError/designSpaceDocument/issues/16
-        https://github.com/fonttools/fonttools/pull/1395
-    """
-    try:
-        designspace = designspaceLib.DesignSpaceDocument.fromfile(designspace_path)
-    except Exception as e:
-        raise FontmakeError("Reading Designspace failed", designspace_path) from e
-
-    for axis in designspace.axes:
-        axis.minimum = axis.map_forward(axis.minimum)
-        axis.default = axis.map_forward(axis.default)
-        axis.maximum = axis.map_forward(axis.maximum)
-        del axis.map[:]
-
-    fd, temp_designspace_path = tempfile.mkstemp()
-    os.close(fd)
-    try:
-        designspace.write(temp_designspace_path)
-        yield temp_designspace_path
-    finally:
-        os.remove(temp_designspace_path)
+    @property
+    def allQuadratic(self):
+        return self in (
+            CurveConversion.ALL_CUBIC_TO_QUAD,
+            CurveConversion.KEEP_QUAD,
+        )
 
 
 def needs_subsetting(ufo):
     if KEEP_GLYPHS_OLD_KEY in ufo.lib or KEEP_GLYPHS_NEW_KEY in ufo.lib:
         return True
     if REMOVE_GLYPHS_OLD_KEY in ufo.lib or REMOVE_GLYPHS_NEW_KEY in ufo.lib:
         return True
@@ -156,26 +155,50 @@
         logger.debug(
             "ufoLib UFO validation is %s", "enabled" if validate_ufo else "disabled"
         )
         self.validate_ufo = validate_ufo
 
     def open_ufo(self, path):
         try:
+            path = Path(path)
+            if path.suffix == ".json":
+                with open(path, "rb") as f:
+                    # pylint: disable=no-member
+                    return ufoLib2.Font.json_load(f)  # type: ignore
             return ufoLib2.Font.open(path, validate=self.validate_ufo)
         except Exception as e:
             raise FontmakeError("Reading UFO source failed", path) from e
 
-    def save_ufo_as(self, font, path, ufo_structure="package"):
+    @staticmethod
+    def _fix_ufo_path(path, ufo_structure):
+        """Normalizes UFO path and updates extension suffix to match its structure"""
+        return os.path.normpath(
+            Path(path).with_suffix(UFO_STRUCTURE_EXTENSIONS[ufo_structure])
+        )
+
+    def save_ufo_as(self, font, path, ufo_structure="package", indent_json=False):
         try:
-            font.save(
-                path,
-                overwrite=True,
-                validate=self.validate_ufo,
-                structure=ufo_structure,
-            )
+            path = _ensure_parent_dir(path)
+            if ufo_structure == "json":
+                with open(path, "wb") as f:
+                    # pylint: disable=no-member
+                    font.json_dump(
+                        f,
+                        # orjson only supports either 2 or none
+                        indent=2 if indent_json else None,
+                        # makes output deterministic
+                        sort_keys=True,
+                    )  # type: ignore
+            else:
+                font.save(
+                    path,
+                    overwrite=True,
+                    validate=self.validate_ufo,
+                    structure=ufo_structure,
+                )
         except Exception as e:
             raise FontmakeError("Writing UFO source failed", path) from e
 
     @timer()
     def build_master_ufos(
         self,
         glyphs_path,
@@ -183,22 +206,23 @@
         master_dir=None,
         instance_dir=None,
         family_name=None,
         mti_source=None,
         write_skipexportglyphs=True,
         generate_GDEF=True,
         ufo_structure="package",
+        indent_json=False,
+        glyph_data=None,
+        save_ufos=True,
     ):
-        """Build UFOs and MutatorMath designspace from Glyphs source."""
+        """Build UFOs and designspace from Glyphs source."""
         import glyphsLib
 
         if master_dir is None:
             master_dir = self._output_dir("ufo")
-        if not os.path.isdir(master_dir):
-            os.mkdir(master_dir)
         if instance_dir is None:
             instance_dir = self._output_dir("ufo", is_instance=True)
 
         if designspace_path is not None:
             designspace_dir = os.path.dirname(designspace_path)
         else:
             designspace_dir = master_dir
@@ -225,39 +249,52 @@
             family_name=family_name,
             instance_dir=instance_dir,
             write_skipexportglyphs=write_skipexportglyphs,
             ufo_module=ufoLib2,
             generate_GDEF=generate_GDEF,
             store_editor_state=False,
             minimal=True,
+            glyph_data=glyph_data,
         )
 
         masters = {}
         # multiple sources can have the same font/filename (but different layer),
         # we want to save a font only once
         for source in designspace.sources:
-            if source.path in masters:
-                assert source.font is masters[source.path]
-                continue
-            ufo_path = os.path.join(master_dir, source.filename)
-            # no need to also set the relative 'filename' attribute as that
-            # will be auto-updated on writing the designspace document
+            ufo_path = self._fix_ufo_path(
+                os.path.join(master_dir, source.filename), ufo_structure
+            )
             source.path = ufo_path
+            # relative 'filename' would be auto-updated upon writing the designspace
+            # but we may not always write one out, thus we keep it up-to-date
+            source.filename = os.path.relpath(ufo_path, designspace_dir)
+            if ufo_path in masters:
+                assert source.font is masters[ufo_path]
+                continue
             masters[ufo_path] = source.font
 
-        if designspace_path is None:
-            designspace_path = os.path.join(master_dir, designspace.filename)
-        designspace.write(designspace_path)
         if mti_source:
             self.add_mti_features_to_master_ufos(mti_source, masters)
 
-        for ufo_path, ufo in masters.items():
-            self.save_ufo_as(ufo, ufo_path, ufo_structure)
+        save_ds = designspace_path is not None or save_ufos
+        if designspace_path is None:
+            designspace_path = os.path.join(master_dir, designspace.filename)
+
+        if save_ds:
+            logger.info("Saving %s", designspace_path)
+            designspace.write(_ensure_parent_dir(designspace_path))
+        else:
+            designspace.path = designspace_path
+
+        if save_ufos:
+            for ufo_path, ufo in masters.items():
+                logger.info("Saving %s", ufo_path)
+                self.save_ufo_as(ufo, ufo_path, ufo_structure, indent_json)
 
-        return designspace_path
+        return designspace
 
     @timer()
     def add_mti_features_to_master_ufos(self, mti_source, masters):
         mti_dir = os.path.dirname(mti_source)
         with open(mti_source, "rb") as mti_file:
             mti_paths = readPlist(mti_file)
         for master_path, master in masters.items():
@@ -278,52 +315,39 @@
         """Build OpenType binaries with CFF outlines."""
         self.save_otfs(ufos, **kwargs)
 
     def build_ttfs(self, ufos, **kwargs):
         """Build OpenType binaries with TrueType outlines."""
         self.save_otfs(ufos, ttf=True, **kwargs)
 
-    def _load_designspace_sources(self, designspace):
-        if isinstance(designspace, (str, os.PathLike)):
-            ds_path = os.fspath(designspace)
-        else:
-            # reload designspace from its path so we have a new copy
-            # that can be modified in-place.
-            ds_path = designspace.path
-        if ds_path is not None:
-            try:
-                designspace = designspaceLib.DesignSpaceDocument.fromfile(ds_path)
-            except Exception as e:
-                raise FontmakeError("Reading Designspace failed", ds_path) from e
-
-        designspace.loadSourceFonts(opener=self.open_ufo)
-
-        return designspace
-
     def _build_interpolatable_masters(
         self,
         designspace,
         ttf,
         use_production_names=None,
         reverse_direction=True,
+        ttf_curves=CurveConversion.ALL_CUBIC_TO_QUAD,
         conversion_error=None,
         feature_writers=None,
         cff_round_tolerance=None,
         debug_feature_file=None,
         fea_include_dir=None,
         flatten_components=False,
         filters=None,
         auto_use_my_metrics=True,
         **kwargs,
     ):
         if ttf:
+            ttf_curves = CurveConversion(ttf_curves)
             return ufo2ft.compileInterpolatableTTFsFromDS(
                 designspace,
                 useProductionNames=use_production_names,
                 reverseDirection=reverse_direction,
+                convertCubics=ttf_curves.convertCubics,
+                allQuadratic=ttf_curves.allQuadratic,
                 cubicConversionError=conversion_error,
                 featureWriters=feature_writers,
                 debugFeatureFile=debug_feature_file,
                 feaIncludeDir=fea_include_dir,
                 filters=filters,
                 flattenComponents=flatten_components,
                 autoUseMyMetrics=auto_use_my_metrics,
@@ -360,14 +384,15 @@
         output_path=None,
         output_dir=None,
         ttf=True,
         optimize_gvar=True,
         optimize_cff=CFFOptimization.SPECIALIZE,
         use_production_names=None,
         reverse_direction=True,
+        ttf_curves=CurveConversion.ALL_CUBIC_TO_QUAD,
         conversion_error=None,
         feature_writers=None,
         cff_round_tolerance=None,
         debug_feature_file=None,
         fea_include_dir=None,
         flatten_components=False,
         filters=None,
@@ -417,18 +442,21 @@
                 vf_name_to_output_path[vf.name] = output_path
 
         logger.info(
             "Building variable fonts " + ", ".join(vf_name_to_output_path.values())
         )
 
         if ttf:
+            ttf_curves = CurveConversion(ttf_curves)
             fonts = ufo2ft.compileVariableTTFs(
                 designspace,
                 featureWriters=feature_writers,
                 useProductionNames=use_production_names,
+                convertCubics=ttf_curves.convertCubics,
+                allQuadratic=ttf_curves.allQuadratic,
                 cubicConversionError=conversion_error,
                 reverseDirection=reverse_direction,
                 optimizeGvar=optimize_gvar,
                 flattenComponents=flatten_components,
                 debugFeatureFile=debug_feature_file,
                 feaIncludeDir=fea_include_dir,
                 filters=filters,
@@ -448,27 +476,31 @@
                 optimizeCFF=optimize_cff,
                 filters=filters,
                 inplace=True,
                 variableFontNames=list(vf_name_to_output_path),
             )
 
         for name, font in fonts.items():
-            font.save(vf_name_to_output_path[name])
+            output_path = vf_name_to_output_path[name]
+            logger.info("Saving %s", output_path)
+            font.save(_ensure_parent_dir(output_path))
 
     def _iter_compile(self, ufos, ttf=False, debugFeatureFile=None, **kwargs):
         # generator function that calls ufo2ft compiler for each ufo and
         # yields ttFont instances
         options = dict(kwargs)
         if ttf:
             for key in ("optimizeCFF", "roundTolerance", "subroutinizer", "cffVersion"):
                 options.pop(key, None)
             compile_func, fmt = ufo2ft.compileTTF, "TTF"
         else:
             for key in (
+                "convertCubics",
                 "cubicConversionError",
+                "allQuadratic",
                 "reverseDirection",
                 "flattenComponents",
                 "autoUseMyMetrics",
                 "dropImpliedOnCurves",
             ):
                 options.pop(key, None)
             compile_func, fmt = ufo2ft.compileOTF, "OTF"
@@ -497,14 +529,15 @@
         use_production_names=None,
         subroutinize=None,  # deprecated
         optimize_cff=CFFOptimization.NONE,
         cff_round_tolerance=None,
         remove_overlaps=True,
         overlaps_backend=None,
         reverse_direction=True,
+        ttf_curves=CurveConversion.ALL_CUBIC_TO_QUAD,
         conversion_error=None,
         feature_writers=None,
         interpolate_layout_from=None,
         interpolate_layout_dir=None,
         output_path=None,
         output_dir=None,
         debug_feature_file=None,
@@ -544,14 +577,16 @@
                 between only round floats which are close to their integral
                 part within the tolerated range. Ignored if ttf=True.
             remove_overlaps: If True, remove overlaps in glyph shapes.
             overlaps_backend: name of the library to remove overlaps. Can be
                 either "booleanOperations" (default) or "pathops".
             reverse_direction: If True, reverse contour directions when
                 compiling TrueType outlines.
+            ttf_curves: Choose between "cu2qu" (default), "mixed", "keep-quad" or
+                "keep-cubic". NOTE: cubics in TTF use glyf v1 which is still draft!
             conversion_error: Error to allow when converting cubic CFF contours
                 to quadratic TrueType contours.
             feature_writers: list of ufo2ft-compatible feature writer classes
                 or pre-initialized objects that are passed on to ufo2ft
                 feature compiler to generate automatic feature code. The
                 default value (None) means that ufo2ft will use its built-in
                 default feature writers (for kern, mark, mkmk, etc.). An empty
@@ -578,14 +613,16 @@
                 in the middle of two off-curve points (TrueType only; default: False).
         """  # noqa: B950
         assert not (output_path and output_dir), "mutually exclusive args"
 
         if output_path is not None and len(ufos) > 1:
             raise ValueError("output_path requires a single input")
 
+        ttf_curves = CurveConversion(ttf_curves)
+
         if subroutinize is not None:
             import warnings
 
             warnings.warn(
                 "the 'subroutinize' argument is deprecated, use 'optimize_cff'",
                 UserWarning,
                 stacklevel=2,
@@ -617,33 +654,39 @@
             ttf,
             removeOverlaps=remove_overlaps,
             overlapsBackend=overlaps_backend,
             optimizeCFF=optimize_cff,
             roundTolerance=cff_round_tolerance,
             useProductionNames=use_production_names,
             reverseDirection=reverse_direction,
+            convertCubics=ttf_curves.convertCubics,
+            allQuadratic=ttf_curves.allQuadratic,
             cubicConversionError=conversion_error,
             featureWriters=feature_writers,
             debugFeatureFile=debug_feature_file,
             feaIncludeDir=fea_include_dir,
             cffVersion=cff_version,
             subroutinizer=subroutinizer,
             flattenComponents=flatten_components,
             filters=filters,
             autoUseMyMetrics=auto_use_my_metrics,
             dropImpliedOnCurves=drop_implied_oncurves,
             inplace=True,  # avoid extra copy
         )
 
+        if interpolate_layout_from is not None:
+            master_locations = self._designspace_full_source_locations(
+                interpolate_layout_from
+            )
         for font, ufo in zip(fonts, ufos):
-            if interpolate_layout_from is not None:
-                master_locations, instance_locations = self._designspace_locations(
-                    interpolate_layout_from
-                )
-                loc = instance_locations[_normpath(ufo.path)]
+            if (
+                interpolate_layout_from is not None
+                and INSTANCE_LOCATION_KEY in ufo.tempLib
+            ):
+                loc = ufo.tempLib[INSTANCE_LOCATION_KEY]
                 gpos_src = interpolate_layout(
                     interpolate_layout_from, loc, finder, mapped=True
                 )
                 font["GPOS"] = gpos_src["GPOS"]
                 gsub_src = TTFont(finder(self._closest_location(master_locations, loc)))
                 if "GDEF" in gsub_src:
                     font["GDEF"] = gsub_src["GDEF"]
@@ -674,15 +717,15 @@
                 otf_path = self._output_path(
                     ufo, ext, is_instance, output_dir=output_dir
                 )
             else:
                 otf_path = output_path
 
             logger.info("Saving %s", otf_path)
-            font.save(otf_path)
+            font.save(_ensure_parent_dir(otf_path))
 
             # 'subset' is an Optional[bool], can be None, True or False.
             # When False, we never subset; when True, we always do; when
             # None (default), we check the presence of custom parameters
             if subset is False:
                 pass
             elif subset is True or needs_subsetting(ufo):
@@ -695,15 +738,19 @@
                 hinted_otf_path = output_path
             else:
                 hinted_otf_path = self._output_path(
                     ufo, ext, is_instance, autohinted=True, output_dir=output_dir
                 )
             try:
                 logger.info("Autohinting %s", hinted_otf_path)
-                ttfautohint(otf_path, hinted_otf_path, args=autohint_thisfont)
+                ttfautohint(
+                    otf_path,
+                    _ensure_parent_dir(hinted_otf_path),
+                    args=autohint_thisfont,
+                )
             except TTFAError:
                 # copy unhinted font to destination before re-raising error
                 shutil.copyfile(otf_path, hinted_otf_path)
                 raise
             finally:
                 # must clean up temp file
                 os.remove(otf_path)
@@ -717,15 +764,15 @@
                 ext,
                 is_instance=False,
                 interpolatable=True,
                 output_dir=output_dir,
                 suffix=source.layerName,
             )
             logger.info("Saving %s", otf_path)
-            source.font.save(otf_path)
+            source.font.save(_ensure_parent_dir(otf_path))
             source.path = otf_path
             source.layerName = None
         for instance in designspace.instances:
             instance.path = instance.filename = None
 
         if output_dir is None:
             output_dir = self._output_dir(ext, interpolatable=True)
@@ -812,14 +859,18 @@
         designspace_path=None,
         master_dir=None,
         instance_dir=None,
         family_name=None,
         mti_source=None,
         write_skipexportglyphs=True,
         generate_GDEF=True,
+        glyph_data=None,
+        output=(),
+        output_dir=None,
+        interpolate=False,
         **kwargs,
     ):
         """Run toolchain from Glyphs source.
 
         Args:
             glyphs_path: Path to source file.
             designspace_path: Output path of generated designspace document.
@@ -829,49 +880,101 @@
             instance_dir: Directory where to save UFO instances (default:
                 "instance_ufo").
             family_name: If provided, uses this family name in the output.
             mti_source: Path to property list file containing a dictionary
                 mapping UFO masters to dictionaries mapping layout table
                 tags to MTI source paths which should be compiled into
                 those tables.
+            glyph_data: A list of GlyphData XML file paths.
             kwargs: Arguments passed along to run_from_designspace.
         """
+        # only save *master* UFOs when explicitly requested: i.e. outputs contain
+        # 'ufo' and the -i/--interpolate option was not passed (that's for *instances*)
+        # or a --master-dir was set
+        save_ufos = "ufo" in output and (not interpolate or master_dir is not None)
+        # take --output-dir to mean same as --master-dir when -o ufo and not -i
+        if (
+            set(output) == {"ufo"}
+            and not interpolate
+            and master_dir is None
+            and output_dir is not None
+        ):
+            master_dir = output_dir
 
         logger.info("Building master UFOs and designspace from Glyphs source")
-        designspace_path = self.build_master_ufos(
+        designspace = self.build_master_ufos(
             glyphs_path,
             designspace_path=designspace_path,
             master_dir=master_dir,
             instance_dir=instance_dir,
             family_name=family_name,
             mti_source=mti_source,
             write_skipexportglyphs=write_skipexportglyphs,
             generate_GDEF=generate_GDEF,
             ufo_structure=kwargs.get("ufo_structure"),
+            indent_json=kwargs.get("indent_json"),
+            glyph_data=glyph_data,
+            save_ufos=save_ufos,
         )
         # 'include' statements in features.fea should be resolved relative to
         # the input .glyphs path, like Glyphs.app would do, and not relative
         # to the UFOs that are generated by glyphsLib.
         fea_include_dir = os.path.dirname(glyphs_path)
         try:
             self.run_from_designspace(
-                designspace_path, fea_include_dir=fea_include_dir, **kwargs
+                designspace,
+                output=output,
+                fea_include_dir=fea_include_dir,
+                output_dir=output_dir,
+                interpolate=interpolate,
+                **kwargs,
             )
         except FontmakeError as e:
             e.source_trail.append(glyphs_path)
             raise
 
+    def _instance_ufo_path(
+        self, instance, designspace_path, output_dir=None, ufo_structure="package"
+    ):
+        """Return an instance path, optionally overriding output dir or extension"""
+        # prefer absolute instance.path over relative instance.filename
+        instance_path = instance.path
+        if instance_path is not None:
+            instance_dir = Path(instance_path).parent
+        elif instance.filename is not None:
+            instance_path = Path(designspace_path).parent / instance.filename
+            instance_dir = instance_path.parent
+        else:
+            # if neither is set, make one up from UFO family/style names
+            instance_path = self._font_name(instance.font)
+            instance_dir = None
+
+        # let --output-dir override the instance UFO directory
+        if output_dir is not None:
+            instance_dir = output_dir
+
+        # fall back to 'instance_ufo/' if we can't find a suitable directory
+        if instance_dir is None:
+            instance_dir = self._output_dir("ufo", is_instance=True)
+
+        instance_path = Path(instance_dir) / Path(instance_path).name
+        return self._fix_ufo_path(instance_path, ufo_structure)
+
     def interpolate_instance_ufos(
         self,
         designspace,
         include=None,
         round_instances=False,
         expand_features_to_instances=False,
         fea_include_dir=None,
         ufo_structure="package",
+        indent_json=False,
+        save_ufos=True,
+        output_path=None,
+        output_dir=None,
     ):
         """Interpolate master UFOs with Instantiator and return instance UFOs.
 
         Args:
             designspace: a DesignSpaceDocument object containing sources and
                 instances.
             include (str): optional regular expression pattern to match the
@@ -888,20 +991,17 @@
         Raises:
             FontmakeError: instances could not be prepared for interpolation or
                 interpolation failed.
             ValueError: an instance descriptor did not have a filename attribute set.
         """
         from glyphsLib.interpolation import apply_instance_data_to_ufo
 
-        logger.info("Interpolating master UFOs from designspace")
-        try:
-            designspace = designspaceLib.DesignSpaceDocument.fromfile(designspace.path)
-        except Exception as e:
-            raise FontmakeError("Reading Designspace failed", designspace.path) from e
+        assert not (output_path and output_dir), "mutually exclusive args"
 
+        logger.info("Interpolating master UFOs from designspace")
         for _location, subDoc in splitInterpolable(designspace):
             try:
                 generator = instantiator.Instantiator.from_designspace(
                     subDoc, round_geometry=round_instances
                 )
             except instantiator.InstantiatorError as e:
                 raise FontmakeError(
@@ -936,143 +1036,85 @@
                             instance.styleName
                         ),
                         designspace.path,
                     ) from e
 
                 apply_instance_data_to_ufo(instance.font, instance, subDoc)
 
-                # TODO: Making filenames up on the spot is complicated, ideally don't save
-                # anything if filename is not set, but make something up when "ufo" is in
-                # output formats, but also consider output_path.
-                if instance.filename is None:
-                    raise ValueError(
-                        "It is currently required that instances have filenames set."
+                if save_ufos:
+                    if output_path is not None:
+                        # we don't know in advance how many instances we will generate
+                        # (depends on splitInterpolable and include filter); if we
+                        # overwrite or stop in the middle of the build it'd be worse,
+                        # so we make the output_path unique using #1, #2, etc. suffix
+                        instance_path = makeOutputFileName(
+                            output_path,
+                            extension=UFO_STRUCTURE_EXTENSIONS[ufo_structure],
+                        )
+                    else:
+                        instance_path = self._instance_ufo_path(
+                            instance, designspace.path, output_dir, ufo_structure
+                        )
+                    logger.info("Saving %s", instance_path)
+                    self.save_ufo_as(
+                        instance.font, instance_path, ufo_structure, indent_json
                     )
-                ufo_path = os.path.join(
-                    os.path.dirname(designspace.path), instance.filename
-                )
-                os.makedirs(os.path.dirname(ufo_path), exist_ok=True)
-                self.save_ufo_as(instance.font, ufo_path, ufo_structure)
+                elif instance.filename is not None:
+                    # saving a UFO sets its path attribute; when saving the binary font
+                    # compiled from this UFO, self._output_path() uses the ufo.path to
+                    # make up the output path. Since we aren't saving the UFO in this
+                    # case, the ufo.path is not set (it's a read-only attribute).
+                    # Therefore we resort to this temporary lib key to pass down the DS
+                    # instance filename to self._output_path() method and make sure the
+                    # font is named correctly whether or not the UFO is saved to disk.
+                    instance.font.tempLib[INSTANCE_FILENAME_KEY] = instance.filename
+
+                # --interpolate-binary-layout needs to know the location of each
+                # instance UFO; the previous code relied on matching instance.path and
+                # ufo.path, but we no longer necessarily save the UFO thus the ufo.path
+                # may not be set. Instead store the location directly in the ufo.tempLib
+                instance.font.tempLib[INSTANCE_LOCATION_KEY] = instance.location
 
                 yield instance.font
 
-    def interpolate_instance_ufos_mutatormath(
-        self,
-        designspace,
-        include=None,
-        round_instances=False,
-        expand_features_to_instances=False,
-        fea_include_dir=None,
-    ):
-        """Interpolate master UFOs with MutatorMath and return instance UFOs.
-
-        Args:
-            designspace: a DesignSpaceDocument object containing sources and
-                instances.
-            include (str): optional regular expression pattern to match the
-                DS instance 'name' attribute and only interpolate the matching
-                instances.
-            round_instances (bool): round instances' coordinates to integer.
-            expand_features_to_instances: parses the master feature file, expands all
-                include()s and writes the resulting full feature file to all instance
-                UFOs. Use this if you share feature files among masters in external
-                files. Otherwise, the relative include paths can break as instances
-                may end up elsewhere. Only done on interpolation.
-        Returns:
-            list of defcon.Font objects corresponding to the UFO instances.
-        Raises:
-            FontmakeError: if any of the sources defines a custom 'layer', for
-                this is not supported by MutatorMath.
-            ValueError: "expand_features_to_instances" is True but no source in the
-                designspace document is designated with '<features copy="1"/>'.
-        """
-        from glyphsLib.interpolation import apply_instance_data
-        from mutatorMath.ufo.document import DesignSpaceDocumentReader
-
-        if any(source.layerName is not None for source in designspace.sources):
-            raise FontmakeError(
-                "MutatorMath doesn't support DesignSpace sources with 'layer' "
-                "attribute",
-                None,
-            )
-
-        with temporarily_disabling_axis_maps(designspace.path) as temp_designspace_path:
-            builder = DesignSpaceDocumentReader(
-                temp_designspace_path,
-                ufoVersion=3,
-                roundGeometry=round_instances,
-                verbose=True,
-            )
-            logger.info("Interpolating master UFOs from designspace")
-            if include is not None:
-                instances = self._search_instances(designspace, pattern=include)
-                for instance_name in instances:
-                    builder.readInstance(("name", instance_name))
-                filenames = set(instances.values())
-            else:
-                builder.readInstances()
-                filenames = None  # will include all instances
-
-        logger.info("Applying instance data from designspace")
-        instance_ufos = apply_instance_data(designspace, include_filenames=filenames)
-
-        if expand_features_to_instances:
-            logger.debug("Expanding features to instance UFOs")
-            master_source = next(
-                (s for s in designspace.sources if s.copyFeatures), None
-            )
-            if not master_source:
-                raise ValueError("No source is designated as the master for features.")
-            else:
-                master_source_font = builder.sources[master_source.name][0]
-                master_source_features = parseLayoutFeatures(
-                    master_source_font, includeDir=fea_include_dir
-                ).asFea()
-                for instance_ufo in instance_ufos:
-                    instance_ufo.features.text = master_source_features
-                    instance_ufo.save()
-
-        return instance_ufos
-
     def run_from_designspace(
         self,
-        designspace_path,
+        designspace,
         output=(),
         interpolate=False,
         variable_fonts: str = ".*",
         masters_as_instances=False,
         interpolate_binary_layout=False,
         round_instances=False,
         feature_writers=None,
         filters=None,
         expand_features_to_instances=False,
-        use_mutatormath=False,
         check_compatibility=None,
         **kwargs,
     ):
         """Run toolchain from a DesignSpace document to produce either static
         instance fonts (ttf or otf), interpolatable or variable fonts.
 
         Args:
-            designspace_path: Path to designspace document.
+            designspace: Path to designspace or DesignSpaceDocument object.
             interpolate: If True output all instance fonts, otherwise just
                 masters. If the value is a string, only build instance(s) that
                 match given name. The string is compiled into a regular
                 expression and matched against the "name" attribute of
                 designspace instances using `re.fullmatch`.
             variable_fonts: if True output all variable fonts, otherwise if the
                 value is a string, only build variable fonts that match the
                 given filename. As above, the string is compiled into a regular
                 expression and matched against the "filename" attribute of
                 designspace variable fonts using `re.fullmatch`.
             masters_as_instances: If True, output master fonts as instances.
             interpolate_binary_layout: Interpolate layout tables from compiled
                 master binaries.
-            round_instances: apply integer rounding when interpolating with
-                MutatorMath.
+            round_instances: apply integer rounding when interpolating static
+                instance UFOs.
             kwargs: Arguments passed along to run_from_ufos.
 
         Raises:
             TypeError: "variable" or "interpolatable" outputs are incompatible
                 with arguments "interpolate", "masters_as_instances", and
                 "interpolate_binary_layout".
         """
@@ -1087,20 +1129,33 @@
             ):
                 if locals()[argname]:
                     raise TypeError(
                         '"%s" argument incompatible with output %r'
                         % (argname, ", ".join(sorted(interp_outputs)))
                     )
 
-        try:
-            designspace = designspaceLib.DesignSpaceDocument.fromfile(designspace_path)
-        except Exception as e:
-            raise FontmakeError("Reading Designspace failed", designspace_path) from e
+        if isinstance(designspace, (str, os.PathLike)):
+            designspace_path = os.fspath(designspace)
+            try:
+                designspace = designspaceLib.DesignSpaceDocument.fromfile(
+                    designspace_path
+                )
+            except Exception as e:
+                raise FontmakeError(
+                    "Reading Designspace failed", designspace_path
+                ) from e
+        elif isinstance(designspace, designspaceLib.DesignSpaceDocument):
+            # get our own DS copy so we can modify in-place
+            designspace = designspace.deepcopyExceptFonts()
+        else:
+            raise TypeError(
+                f"expected path or DesignSpaceDocument, found {type(designspace.__name__)}"
+            )
 
-        designspace = self._load_designspace_sources(designspace)
+        designspace.loadSourceFonts(opener=self.open_ufo)
 
         # if no --feature-writers option was passed, check in the designspace's
         # <lib> element if user supplied a custom featureWriters configuration;
         # if so, use that for all the UFOs built from this designspace
         if feature_writers is None and FEATURE_WRITERS_KEY in designspace.lib:
             feature_writers = loadFeatureWriters(designspace)
 
@@ -1134,15 +1189,14 @@
                     outputs=static_outputs,
                     interpolate=interpolate,
                     masters_as_instances=masters_as_instances,
                     interpolate_binary_layout=interpolate_binary_layout,
                     round_instances=round_instances,
                     feature_writers=feature_writers,
                     expand_features_to_instances=expand_features_to_instances,
-                    use_mutatormath=use_mutatormath,
                     filters=filters,
                     **kwargs,
                 )
             if interp_outputs:
                 self._run_from_designspace_interpolatable(
                     designspace,
                     outputs=interp_outputs,
@@ -1169,44 +1223,48 @@
         interpolate=False,
         masters_as_instances=False,
         interpolate_binary_layout=False,
         round_instances=False,
         feature_writers=None,
         expand_features_to_instances=False,
         fea_include_dir=None,
-        use_mutatormath=False,
         ufo_structure="package",
+        indent_json=False,
+        output_path=None,
+        output_dir=None,
         **kwargs,
     ):
+        save_ufos = "ufo" in outputs
         ufos = []
         if not interpolate or masters_as_instances:
-            ufos.extend(s.path for s in designspace.sources if s.path)
+            unique_srcs = {id(s.font): s.font for s in designspace.sources}
+            ufos.extend(unique_srcs.values())
         if interpolate:
             pattern = interpolate if isinstance(interpolate, str) else None
-            if use_mutatormath:
-                ufos.extend(
-                    self.interpolate_instance_ufos_mutatormath(
-                        designspace,
-                        include=pattern,
-                        round_instances=round_instances,
-                        expand_features_to_instances=expand_features_to_instances,
-                        fea_include_dir=fea_include_dir,
-                    )
-                )
-            else:
-                ufos.extend(
-                    self.interpolate_instance_ufos(
-                        designspace,
-                        include=pattern,
-                        round_instances=round_instances,
-                        expand_features_to_instances=expand_features_to_instances,
-                        fea_include_dir=fea_include_dir,
-                        ufo_structure=ufo_structure,
-                    )
+            # use --output-{path,dir} options for instance UFOs if 'ufo' is the only -o
+            ufo_output_path = ufo_output_dir = None
+            if set(outputs) == {"ufo"}:
+                if output_path is not None:
+                    ufo_output_path = output_path
+                if output_dir is not None:
+                    ufo_output_dir = output_dir
+            ufos.extend(
+                self.interpolate_instance_ufos(
+                    designspace,
+                    include=pattern,
+                    round_instances=round_instances,
+                    expand_features_to_instances=expand_features_to_instances,
+                    fea_include_dir=fea_include_dir,
+                    ufo_structure=ufo_structure,
+                    indent_json=indent_json,
+                    save_ufos=save_ufos,
+                    output_path=ufo_output_path,
+                    output_dir=ufo_output_dir,
                 )
+            )
 
         if interpolate_binary_layout is False:
             interpolate_layout_from = interpolate_layout_dir = None
         else:
             interpolate_layout_from = designspace
             # Unload UFO fonts, we will reload them as binary
             for s in interpolate_layout_from.sources:
@@ -1220,14 +1278,16 @@
             ufos,
             output=outputs,
             is_instance=(interpolate or masters_as_instances),
             interpolate_layout_from=interpolate_layout_from,
             interpolate_layout_dir=interpolate_layout_dir,
             feature_writers=feature_writers,
             fea_include_dir=fea_include_dir,
+            output_path=output_path,
+            output_dir=output_dir,
             **kwargs,
         )
 
     def _run_from_designspace_interpolatable(
         self,
         designspace,
         outputs,
@@ -1278,39 +1338,35 @@
             return
 
         if "otf" in output and "otf-cff2" in output:
             raise ValueError("'otf' and 'otf-cff2' outputs are mutually exclusive")
 
         # the `ufos` parameter can be a list of UFO objects
         # or it can be a path (string) with a glob syntax
-        ufo_paths = []
         if isinstance(ufos, str):
-            ufo_paths = glob.glob(ufos)
-            ufos = [self.open_ufo(x) for x in ufo_paths]
+            ufos = [self.open_ufo(x) for x in glob.glob(ufos)]
         elif isinstance(ufos, list):
             # ufos can be either paths or open Font objects, so normalize them
             ufos = [self.open_ufo(x) if isinstance(x, str) else x for x in ufos]
-            ufo_paths = [x.path for x in ufos]
         else:
             raise TypeError(
-                "UFOs parameter is neither a defcon.Font object, a path or a glob, "
+                "UFOs parameter is neither a ufoLib2.Font object, a path or a glob, "
                 f"nor a list of any of these: {ufos:r}."
             )
 
-        need_reload = False
         cff_version = 1 if "otf" in output else 2 if "otf-cff2" in output else None
+
+        # if building both OTF & TTF we must tell ufo2ft to compile with inplace=False
+        inplace = not (cff_version is not None and "ttf" in output)
+
         if cff_version is not None:
-            self.build_otfs(ufos, cff_version=cff_version, **kwargs)
-            need_reload = True
+            self.build_otfs(ufos, cff_version=cff_version, inplace=inplace, **kwargs)
 
         if "ttf" in output:
-            if need_reload:
-                ufos = [self.open_ufo(path) for path in ufo_paths]
-            self.build_ttfs(ufos, **kwargs)
-            need_reload = True
+            self.build_ttfs(ufos, inplace=inplace, **kwargs)
 
     @staticmethod
     def _search_instances(designspace, pattern):
         instances = OrderedDict()
         for instance in designspace.instances:
             # is 'name' optional? 'filename' certainly must not be
             if fullmatch(pattern, instance.name):
@@ -1378,44 +1434,47 @@
         output_dir=None,
         suffix=None,
     ):
         """Generate output path for a font file with given extension."""
 
         if isinstance(ufo_or_font_name, str):
             font_name = ufo_or_font_name
-        elif ufo_or_font_name.path:
-            font_name = os.path.splitext(
-                os.path.basename(os.path.normpath(ufo_or_font_name.path))
-            )[0]
         else:
-            font_name = self._font_name(ufo_or_font_name)
+            ufo = ufo_or_font_name
+            if ufo.path:
+                font_name = os.path.splitext(
+                    os.path.basename(os.path.normpath(ufo.path))
+                )[0]
+            elif INSTANCE_FILENAME_KEY in ufo.tempLib:
+                font_name = Path(ufo.tempLib[INSTANCE_FILENAME_KEY]).stem
+            else:
+                font_name = self._font_name(ufo)
 
         if output_dir is None:
             output_dir = self._output_dir(
                 ext, is_instance, interpolatable, autohinted, is_variable
             )
-        if not os.path.exists(output_dir):
-            os.makedirs(output_dir)
 
         if suffix:
             return os.path.join(output_dir, f"{font_name}-{suffix}.{ext}")
         else:
             return os.path.join(output_dir, f"{font_name}.{ext}")
 
-    def _designspace_locations(self, designspace):
-        """Map font filenames to their locations in a designspace."""
+    def _designspace_full_source_locations(self, designspace):
+        """Map "full" sources' paths to their locations in a designspace.
 
-        maps = []
-        for elements in (designspace.sources, designspace.instances):
-            location_map = {}
-            for element in elements:
-                path = _normpath(element.path)
-                location_map[path] = element.location
-            maps.append(location_map)
-        return maps
+        'Sparse layer' sources only contributing glyph outlines but no
+        info/kerning/features are ignored.
+        """
+        location_map = {}
+        default_source = designspace.findDefault()
+        for source in designspace.sources:
+            if source is default_source or source.layerName is not None:
+                location_map[_normpath(source.path)] = source.location
+        return location_map
 
     def _closest_location(self, location_map, target):
         """Return path of font whose location is closest to target."""
 
         def dist(a, b):
             return math.sqrt(sum((a[k] - b[k]) ** 2 for k in a.keys()))
 
@@ -1438,7 +1497,12 @@
     """
     fname = os.path.splitext(os.path.basename(source))[0] + "." + ext
     return os.path.join(directory, fname)
 
 
 def _normpath(fname):
     return os.path.normcase(os.path.normpath(fname))
+
+
+def _ensure_parent_dir(path):
+    Path(path).parent.mkdir(parents=True, exist_ok=True)
+    return path
```

## Comparing `fontmake-3.6.1/Lib/fontmake/__main__.py` & `fontmake-3.7.0b1/Lib/fontmake/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import os
 import sys
-from argparse import ArgumentParser, FileType
+from argparse import SUPPRESS, ArgumentParser, FileType
 from collections import namedtuple
 from contextlib import contextmanager
 from textwrap import dedent
 
 from fontTools.misc.loggingTools import configLogger
 from ufo2ft import CFFOptimization
 from ufo2ft.featureWriters import loadFeatureWriterFromString
 from ufo2ft.filters import loadFilterFromString
 
 from fontmake import __version__
 from fontmake.errors import FontmakeError
-from fontmake.font_project import INTERPOLATABLE_OUTPUTS, FontProject
+from fontmake.font_project import INTERPOLATABLE_OUTPUTS, CurveConversion, FontProject
 
 
 def _loadPlugins(parser, specs, from_string_func, parser_error_message):
     plugins = []
     seen_ellipsis = False
     for s in specs:
         if s == "None":
@@ -128,27 +128,29 @@
             if glyphs_path:
                 parser.error("Only one *.glyphs source file is allowed")
             glyphs_path = filename
         elif filename.endswith(".designspace"):
             if designspace_path:
                 parser.error("Only one *.designspace source file is allowed")
             designspace_path = filename
-        elif (
-            os.path.normpath(filename).endswith(".ufo") and os.path.isdir(filename)
-        ) or (filename.endswith(".ufoz") and os.path.isfile(filename)):
+        elif filename.endswith((".ufo", ".ufoz", ".ufo.json")):
             ufo_paths.append(filename)
         else:
             parser.error(f"Unknown input file extension: {filename!r}")
 
     count = sum(bool(p) for p in (glyphs_path, ufo_paths, designspace_path))
     if count == 0:
         parser.error("No input files specified")
     elif count > 1:
         parser.error(f"Expected 1, got {count} different types of inputs files")
 
+    for filename in [glyphs_path] + [designspace_path] + ufo_paths:
+        if filename is not None and not os.path.exists(filename):
+            parser.error(f"{filename} not found")
+
     format_name = (
         "Glyphs" if glyphs_path else "designspace" if designspace_path else "UFO"
     ) + " source"
 
     return _ParsedInputs(
         glyphs_path,
         ufo_paths,
@@ -228,14 +230,25 @@
     positionalInputs.add_argument(
         "posargs",
         nargs="*",
         metavar="INPUTS",
         help="Either one *.designspace or *.glyphs file, or one or more *.ufo",
     )
 
+    otherInputGroup = parser.add_argument_group(title="Other input arguments")
+    otherInputGroup.add_argument(
+        "--glyph-data",
+        action="append",
+        default=None,
+        metavar="GLYPHDATA",
+        help="Custom GlyphData XML file with glyph info (production name, "
+        "script, category, subCategory, etc.). Can be used more than once "
+        "(for Glyphs sources only).",
+    )
+
     outputGroup = parser.add_argument_group(title="Output arguments")
     outputGroup.add_argument(
         "-o",
         "--output",
         nargs="+",
         default=("otf", "ttf"),
         metavar="FORMAT",
@@ -273,15 +286,15 @@
         const=True,
         metavar="INSTANCE_NAME",
         help="Interpolate masters and generate all the instances defined. "
         "To only interpolate a specific instance (or instances) that "
         'match a given "name" attribute, you can pass as argument '
         "the full instance name or a regular expression. "
         'E.g.: -i "Noto Sans Bold"; or -i ".* UI Condensed". '
-        "(for Glyphs or MutatorMath sources only). ",
+        "(for Glyphs or DesignSpace sources only). ",
     )
     outputGroup.add_argument(
         "--variable-fonts",
         nargs="?",
         default=".*",
         const=True,
         metavar="VARIABLE_FONT_FILENAME",
@@ -293,22 +306,16 @@
             that match a given "filename" attribute, you can pass as argument
             the full filename or a regular expression. E.g.: --variable-fonts
             "MyFontVF_WeightOnly.ttf"; or --variable-fonts
             "MyFontVFItalic_.*.ttf".
         """
         ),
     )
-    outputGroup.add_argument(
-        "--use-mutatormath",
-        action="store_true",
-        help=(
-            "Use MutatorMath to generate instances (supports extrapolation and "
-            "anisotropic locations)."
-        ),
-    )
+    # no longer show option in --help but keep to produce nice error message
+    outputGroup.add_argument("--use-mutatormath", action="store_true", help=SUPPRESS)
     outputGroup.add_argument(
         "-M",
         "--masters-as-instances",
         action="store_true",
         help="Output masters as instances",
     )
     outputGroup.add_argument(
@@ -389,22 +396,35 @@
     )
     outputGroup.add_argument(
         "--no-generate-GDEF",
         dest="generate_GDEF",
         action="store_false",
         help="Do not auto-generate a GDEF table, but keep an existing one intact.",
     )
-    outputGroup.add_argument(
+
+    ufoStructureGroup = outputGroup.add_mutually_exclusive_group(required=False)
+    # kept for backward compat
+    ufoStructureGroup.add_argument(
         "--save-ufo-as-zip",
-        dest="ufo_structure",
-        action="store_const",
-        const="zip",
+        dest="save_ufo_as_zip",
+        action="store_true",
+        help="Deprecated. Use --ufo-structure=zip instead.",
+    )
+    ufoStructureGroup.add_argument(
+        "--ufo-structure",
         default="package",
-        help="Save UFOs as .ufoz format. Only valid when generating UFO masters "
-        "from glyphs source or interpolating UFO instances.",
+        choices=("package", "zip", "json"),
+        help="Select UFO format structure. Choose between: %(choices)s "
+        "(default: %(default)s). NOTE: json export is unofficial/experimental.",
+    )
+    outputGroup.add_argument(
+        "--indent-json",
+        action="store_true",
+        help="Whether to format the JSON files created with --ufo-structure=json "
+        "as multiple lines with 2-space indentation. Default: single line, no indent.",
     )
 
     contourGroup = parser.add_argument_group(title="Handling of contours")
     contourGroup.add_argument(
         "--keep-overlaps",
         dest="remove_overlaps",
         action="store_false",
@@ -423,14 +443,25 @@
         "--keep-direction",
         dest="reverse_direction",
         action="store_false",
         help="Do not reverse contour direction when output is ttf or "
         "ttf-interpolatable",
     )
     contourGroup.add_argument(
+        "--ttf-curves",
+        dest="ttf_curves",
+        default=CurveConversion.default().value,
+        choices=[e.value for e in CurveConversion],
+        help="Controls conversion of cubic Bézier curves to TrueType quadratic splines."
+        " By default ('cu2qu'), all cubics are converted to quadratic (glyf v0). With"
+        " 'mixed', cubics are converted to quadratic only when more economical."
+        " If 'keep-quad' or 'keep-cubic', cu2qu is skipped altogether and curves are"
+        " compiled unchanged. NOTE: cubics in TTF use glyf v1 which is still draft!",
+    )
+    contourGroup.add_argument(
         "-e",
         "--conversion-error",
         type=float,
         default=None,
         metavar="ERROR",
         help="Maximum approximation error for cubic to quadratic conversion "
         "measured in EM",
@@ -521,15 +552,15 @@
     layoutGroup.add_argument(
         "--interpolate-binary-layout",
         nargs="?",
         default=False,
         const=True,
         metavar="MASTER_DIR",
         help="Interpolate layout tables from compiled master binaries. "
-        "Requires Glyphs or MutatorMath source.",
+        "Requires Glyphs or DesignSpace source.",
     )
     layoutGroup.add_argument(
         "--feature-writer",
         metavar="CLASS",
         action="append",
         dest="feature_writer_specs",
         help="string specifying a feature writer class to load, either "
@@ -605,60 +636,59 @@
         choices=("DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"),
         help="Configure the logger verbosity level. Choose between: "
         "%(choices)s. Default: INFO",
     )
 
     args = vars(parser.parse_args(args))
 
+    use_mutatormath = args.pop("use_mutatormath")
+    if use_mutatormath:
+        parser.error(
+            "MutatorMath is no longer supported by fontmake. "
+            "Try to use ufoProcessor: https://github.com/LettError/ufoProcessor"
+        )
+
     level = args.pop("verbose")
     _configure_logging(level, timing=args.pop("timing"))
 
     specs = args.pop("feature_writer_specs")
     if specs is not None:
         args["feature_writers"] = _loadFeatureWriters(parser, specs)
 
     specs = args.pop("filter_specs")
     if specs is not None:
         args["filters"] = _loadFilters(parser, specs)
 
+    if args.pop("save_ufo_as_zip"):
+        args["ufo_structure"] = "zip"
+
     inputs = parse_mutually_exclusive_inputs(parser, args)
 
     if INTERPOLATABLE_OUTPUTS.intersection(args["output"]):
         if not (inputs.glyphs_path or inputs.designspace_path):
             parser.error("Glyphs or designspace source required for variable font")
         exclude_args(
             parser,
             args,
             [
                 "interpolate",
                 "masters_as_instances",
                 "interpolate_binary_layout",
-                "use_mutatormath",
             ],
             "variable output",
         )
     else:
         exclude_args(
             parser,
             args,
             ["variable_fonts", "optimize_gvar"],
             "static output",
             positive=False,
         )
 
-    if args.get("use_mutatormath"):
-        for module in ("defcon", "mutatorMath"):
-            try:
-                __import__(module)
-            except ImportError:
-                parser.error(
-                    f"{module} module not found; reinstall fontmake with the "
-                    "[mutatormath] extra"
-                )
-
     PRINT_TRACEBACK = level == "DEBUG"
     try:
         project = FontProject(validate_ufo=args.pop("validate_ufo"))
 
         if inputs.glyphs_path:
             # we don't support customizing include directory for .glyphs input
             # for Glyphs.app does not either.
@@ -673,14 +703,15 @@
             args,
             [
                 "family_name",
                 "mti_source",
                 "designspace_path",
                 "master_dir",
                 "instance_dir",
+                "glyph_data",
             ],
             inputs.format_name,
         )
         exclude_args(
             parser, args, ["write_skipexportglyphs"], inputs.format_name, positive=False
         )
         if inputs.designspace_path:
@@ -689,23 +720,23 @@
 
         exclude_args(
             parser,
             args,
             [
                 "interpolate",
                 "variable_fonts",
-                "use_mutatormath",
                 "interpolate_binary_layout",
                 "round_instances",
                 "expand_features_to_instances",
                 "check_compatibility",
             ],
             inputs.format_name,
         )
         args.pop("ufo_structure", None)  # unused for UFO output
+        args.pop("indent_json", None)
         project.run_from_ufos(
             inputs.ufo_paths, is_instance=args.pop("masters_as_instances"), **args
         )
     except FontmakeError as e:
         if PRINT_TRACEBACK:
             logging.exception(e)
             sys.exit(1)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `fontmake-3.6.1/Lib/fontmake.egg-info/PKG-INFO` & `fontmake-3.7.0b1/Lib/fontmake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fontmake
-Version: 3.6.1
+Version: 3.7.0b1
 Summary: Compile fonts from sources (UFO, Glyphs) to binary (OpenType, TrueType).
 Home-page: https://github.com/googlei18n/fontmake
 License: Apache Software License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,14 +18,16 @@
 Classifier: Topic :: Text Processing :: Fonts
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pathops
 Provides-Extra: lxml
 Provides-Extra: mutatormath
 Provides-Extra: autohint
+Provides-Extra: json
+Provides-Extra: repacker
 Provides-Extra: all
 License-File: LICENSE
 
 ![GitHub Actions Build Status][] ![Python Versions][] [![PyPI
 Version][]][1]
 
 # fontmake
```

## Comparing `fontmake-3.6.1/Lib/fontmake.egg-info/SOURCES.txt` & `fontmake-3.7.0b1/Lib/fontmake.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 Lib/fontmake.egg-info/entry_points.txt
 Lib/fontmake.egg-info/requires.txt
 Lib/fontmake.egg-info/top_level.txt
 tests/conftest.py
 tests/test_compatibility.py
 tests/test_instantiator.py
 tests/test_main.py
+tests/data/GlyphData.xml
 tests/data/GlyphsUnitTestSans.glyphs
 tests/data/TestSubset.glyphs
 tests/data/TestSubset2.glyphs
 tests/data/AutohintingTest/Padyakke.glyphs
 tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace
 tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace
 tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist
```

## Comparing `fontmake-3.6.1/.github/workflows/ci.yml` & `fontmake-3.7.0b1/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -92,31 +92,26 @@
         if egrep -q "$PRERELEASE_TAG_PATTERN" <<< "$TAG_NAME"; then
           echo "Tag contains a pre-release suffix"
           echo "IS_PRERELEASE=true" >> "$GITHUB_ENV"
         else
           echo "Tag does not contain pre-release suffix"
           echo "IS_PRERELEASE=false" >> "$GITHUB_ENV"
         fi
-    - name: Create GitHub release
-      id: create_release
-      uses: actions/create-release@v1
-      env:
-        # This token is provided by Actions, you do not need to create your own token
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-      with:
-        tag_name: ${{ github.ref }}
-        release_name: ${{ github.ref }}
-        body_path: "${{ runner.temp }}/release_notes.md"
-        draft: false
-        prerelease: ${{ env.IS_PRERELEASE }}
     - name: Build and publish
       env:
         TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
         TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
       run: |
         if [ "$IS_PRERELEASE" == true ]; then
           echo "DEBUG: This is a pre-release"
         else
           echo "DEBUG: This is a final release"
         fi
         python setup.py sdist bdist_wheel
         twine upload dist/*
+    - name: Create GitHub release
+      id: create_release
+      uses: ncipollo/release-action@v1
+      with:
+        bodyFile: "${{ runner.temp }}/release_notes.md"
+        draft: false
+        prerelease: ${{ env.IS_PRERELEASE }}
```

## Comparing `fontmake-3.6.1/tests/test_instantiator.py` & `fontmake-3.7.0b1/tests/test_instantiator.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/test_main.py` & `fontmake-3.7.0b1/tests/test_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,65 +67,14 @@
         "MutatorMathTest-Sans Light Condensed.ttf",
         "MutatorMathTest-Serif Light Condensed.otf",
         "MutatorMathTest-Sans Light Condensed.otf",
         "MutatorMathTest-Serif Light Condensed.ttf",
     }
 
 
-def test_interpolation_mutatormath(data_dir, tmp_path):
-    shutil.copytree(data_dir / "DesignspaceTest", tmp_path / "sources")
-
-    fontmake.__main__.main(
-        [
-            "-m",
-            str(tmp_path / "sources" / "DesignspaceTest.designspace"),
-            "-i",
-            "--use-mutatormath",
-            "--output-dir",
-            str(tmp_path),
-        ]
-    )
-
-    assert {p.name for p in tmp_path.glob("*.*")} == {
-        "MyFont-Regular.ttf",
-        "MyFont-Regular.otf",
-    }
-
-    test_output_ttf = fontTools.ttLib.TTFont(tmp_path / "MyFont-Regular.ttf")
-    assert test_output_ttf["OS/2"].usWeightClass == 400
-    glyph = test_output_ttf["glyf"]["l"]
-    assert glyph.xMin == 50
-    assert glyph.xMax == 170
-
-    test_output_otf = fontTools.ttLib.TTFont(tmp_path / "MyFont-Regular.otf")
-    assert test_output_otf["OS/2"].usWeightClass == 400
-    glyph_set = test_output_otf.getGlyphSet()
-    charstrings = list(test_output_otf["CFF "].cff.values())[0].CharStrings
-    glyph = charstrings["l"]
-    x_min, _, x_max, _ = glyph.calcBounds(glyph_set)
-    assert x_min == 50
-    assert x_max == 170
-
-
-def test_interpolation_mutatormath_source_layer(data_dir, tmp_path):
-    shutil.copytree(data_dir / "MutatorSans", tmp_path / "layertest")
-
-    with pytest.raises(SystemExit, match="sources with 'layer'"):
-        fontmake.__main__.main(
-            [
-                "-m",
-                str(tmp_path / "layertest" / "MutatorSans.designspace"),
-                "-i",
-                "--use-mutatormath",
-                "--output-dir",
-                str(tmp_path),
-            ]
-        )
-
-
 def test_interpolation_and_masters_as_instances(data_dir, tmp_path):
     shutil.copytree(data_dir / "DesignspaceTest", tmp_path / "sources")
 
     fontmake.__main__.main(
         [
             "-m",
             str(tmp_path / "sources" / "DesignspaceTest.designspace"),
@@ -410,23 +359,21 @@
     fontmake.__main__.main(
         [
             "-m",
             str(tmp_path / "sources" / "DesignspaceTestSharedFeatures.designspace"),
             "-i",
             "--expand-features-to-instances",
             "-o",
-            "ttf",
+            "ufo",
             "--output-dir",
             str(tmp_path),
         ]
     )
 
-    test_feature_file = (
-        tmp_path / "sources/instance_ufo/DesignspaceTest-Light.ufo/features.fea"
-    )
+    test_feature_file = tmp_path / "DesignspaceTest-Light.ufo/features.fea"
     assert test_feature_file.read_text() == "# test"
 
 
 def test_shared_features_ufo(data_dir, tmp_path):
     shutil.copytree(data_dir / "DesignspaceTestSharedFeatures", tmp_path / "sources")
 
     fontmake.__main__.main(
@@ -690,14 +637,63 @@
     with open(debug_feature_path, "r") as debug_feature_file:
         features = debug_feature_file.read()
 
     assert "### GlyphsUnitTestSans-Regular" in features
     assert "### GlyphsUnitTestSans-Black" in features
 
 
+def test_glyph_data(data_dir, tmp_path):
+    shutil.copyfile(
+        data_dir / "GlyphsUnitTestSans.glyphs", tmp_path / "GlyphsUnitTestSans.glyphs"
+    )
+    shutil.copyfile(data_dir / "GlyphData.xml", tmp_path / "GlyphData.xml")
+
+    args = [
+        "-g",
+        str(tmp_path / "GlyphsUnitTestSans.glyphs"),
+        "--master-dir",
+        str(tmp_path / "master_ufos"),
+        "--instance-dir",
+        str(tmp_path / "instance_ufos"),
+        "-o",
+        "ufo",
+    ]
+    fontmake.__main__.main(args)
+
+    for path in (tmp_path / "master_ufos").glob("*.ufo"):
+        with ufoLib2.Font.open(path) as ufo:
+            assert "public.openTypeCategories" in ufo.lib
+            assert ufo.lib["public.openTypeCategories"].get("fatha-ar") == "mark"
+
+            fatha = ufo["fatha-ar"]
+            assert fatha.width == 0
+            assert "com.schriftgestaltung.Glyphs.originalWidth" in fatha.lib
+
+    shutil.rmtree(tmp_path / "master_ufos")
+
+    fontmake.__main__.main(
+        args
+        + [
+            "--glyph-data",
+            str(tmp_path / "GlyphData.xml"),
+        ]
+    )
+
+    for path in (tmp_path / "master_ufos").glob("*.ufo"):
+        with ufoLib2.Font.open(path) as ufo:
+            assert "public.openTypeCategories" in ufo.lib
+            assert ufo.lib["public.openTypeCategories"].get("fatha-ar") is None
+
+            fatha = ufo["fatha-ar"]
+            assert fatha.width != 0
+            assert "com.schriftgestaltung.Glyphs.originalWidth" not in fatha.lib
+            assert fatha.lib.get("com.schriftgestaltung.Glyphs.category") == "Letter"
+            assert fatha.lib.get("com.schriftgestaltung.Glyphs.subCategory") is None
+
+
 def test_ufo_to_static_otf_cff2(data_dir, tmp_path):
     fontmake.__main__.main(
         [
             "-u",
             str(data_dir / "DesignspaceTest" / "MyFont-Light.ufo"),
             "-o",
             "otf-cff2",
@@ -1047,19 +1043,20 @@
                 data_dir / "MutatorSansLite" / "MutatorSans_v5_several_vfs.designspace"
             ),
             "-o",
             "variable",
             "--variable-fonts",
             "MutatorSansVariable_Width",
             "--output-path",
-            str(tmp_path / "MySingleVF.ttf"),
+            str(tmp_path / "output" / "MySingleVF.ttf"),
         ]
     )
 
-    assert (tmp_path / "MySingleVF.ttf").exists()
+    # 'output' subfolder was created automatically
+    assert (tmp_path / "output" / "MySingleVF.ttf").exists()
 
 
 def test_main_designspace_v5_dont_interpolate_discrete_axis(data_dir, tmp_path):
     fontmake.__main__.main(
         [
             "-m",
             str(
@@ -1117,7 +1114,128 @@
     )
 
     assert re.search(
         r"^DEBUG:fontmake.timer:Took [\.0-9]+s to run 'save_otfs'\r?$",
         result.stderr.decode(),
         flags=re.MULTILINE,
     )
+
+
+@pytest.fixture(params=["package", "zip", "json"])
+def ufo_structure(request):
+    if request.param == "json":
+        # skip if ufoLib2's extra dep is not installed
+        pytest.importorskip("cattrs")
+    return request.param
+
+
+@pytest.mark.parametrize("interpolate", [False, True])
+def test_main_export_custom_ufo_structure(
+    data_dir, tmp_path, ufo_structure, interpolate
+):
+    args = [
+        str(data_dir / "GlyphsUnitTestSans.glyphs"),
+        "-o",
+        "ufo",
+        "--output-dir",
+        str(tmp_path),
+        "--ufo-structure",
+        ufo_structure,
+    ]
+    if interpolate:
+        args.append("-i")
+    else:
+        # strictly not needed, added just to make Windows happy about relative
+        # instance.filename when designspace is written to a different mount point
+        args.extend(["--instance-dir", str(tmp_path)])
+
+    fontmake.__main__.main(args)
+
+    ext = {"package": ".ufo", "zip": ".ufoz", "json": ".ufo.json"}[ufo_structure]
+
+    for style in ["Light", "Regular", "Bold"]:
+        assert (tmp_path / f"GlyphsUnitTestSans-{style}").with_suffix(ext).exists()
+
+    if interpolate:
+        for style in ["Thin", "ExtraLight", "Medium", "Black", "Web"]:
+            assert (tmp_path / f"GlyphsUnitTestSans-{style}").with_suffix(ext).exists()
+
+
+@pytest.mark.parametrize("ufo_structure", ["zip", "json"])
+def test_main_build_from_custom_ufo_structure(data_dir, tmp_path, ufo_structure):
+    pytest.importorskip("cattrs")
+
+    # export designspace pointing to {json,zip}-flavored source UFOs
+    fontmake.__main__.main(
+        [
+            str(data_dir / "GlyphsUnitTestSans.glyphs"),
+            "-o",
+            "ufo",
+            "--output-dir",
+            str(tmp_path / "master_ufos"),
+            "--ufo-structure",
+            ufo_structure,
+            # makes Windows happy about relative instance.filename across drives
+            "--instance-dir",
+            str(tmp_path / "instance_ufos"),
+        ]
+    )
+
+    # interpolate one static TTF instance from this designspace
+    fontmake.__main__.main(
+        [
+            str(tmp_path / "master_ufos" / "GlyphsUnitTestSans.designspace"),
+            "-o",
+            "ttf",
+            "-i",
+            "Glyphs Unit Test Sans Extra Light",
+            "--output-path",
+            str(tmp_path / "instance_ttfs" / "GlyphsUnitTestSans-ExtraLight.ttf"),
+        ]
+    )
+
+    assert len(list((tmp_path / "instance_ttfs").glob("*.ttf"))) == 1
+    assert (tmp_path / "instance_ttfs" / "GlyphsUnitTestSans-ExtraLight.ttf").exists()
+
+    # build one {json,zip} UFO => OTF
+    ext = {"json": ".ufo.json", "zip": ".ufoz"}[ufo_structure]
+    fontmake.__main__.main(
+        [
+            str(tmp_path / "master_ufos" / f"GlyphsUnitTestSans-Regular{ext}"),
+            "-o",
+            "otf",
+            "--output-path",
+            str(tmp_path / "master_otfs" / "GlyphsUnitTestSans-Regular.otf"),
+        ]
+    )
+
+    assert len(list((tmp_path / "master_otfs").glob("*.otf"))) == 1
+    assert (tmp_path / "master_otfs" / "GlyphsUnitTestSans-Regular.otf").exists()
+
+
+@pytest.mark.parametrize("indent_json", [False, True])
+def test_main_export_ufo_json_with_indentation(data_dir, tmp_path, indent_json):
+    pytest.importorskip("cattrs")
+
+    fontmake.__main__.main(
+        [
+            str(data_dir / "GlyphsUnitTestSans.glyphs"),
+            "-o",
+            "ufo",
+            "--output-dir",
+            str(tmp_path / "master_ufos"),
+            "--ufo-structure",
+            "json",
+            # makes Windows happy about relative instance.filename across drives
+            "--instance-dir",
+            str(tmp_path / "instance_ufos"),
+        ]
+        + (["--indent-json"] if indent_json else [])
+    )
+
+    regular_ufo = tmp_path / "master_ufos" / "GlyphsUnitTestSans-Regular.ufo.json"
+    assert (regular_ufo).exists()
+
+    if indent_json:
+        assert regular_ufo.read_text().startswith('{\n  "features"')
+    else:
+        assert regular_ufo.read_text().startswith('{"features"')
```

## Comparing `fontmake-3.6.1/tests/test_compatibility.py` & `fontmake-3.7.0b1/tests/test_compatibility.py`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/TestSubset.glyphs` & `fontmake-3.7.0b1/tests/data/TestSubset.glyphs`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/TestSubset2.glyphs` & `fontmake-3.7.0b1/tests/data/TestSubset2.glyphs`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/GlyphsUnitTestSans.glyphs` & `fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans.glyphs`

 * *Files 1% similar despite different names*

```diff
@@ -1367,14 +1367,66 @@
 }
 );
 leftKerningGroup = A.sc;
 rightKerningGroup = A.sc;
 rightMetricsKey = "=|";
 },
 {
+glyphname = "fatha-ar";
+lastChange = "2023-07-18 21:25:18 +0000";
+layers = (
+{
+layerId = "C4872ECA-A3A9-40AB-960A-1DB2202F16DE";
+paths = (
+{
+closed = 1;
+nodes = (
+"363 466 LINE",
+"363 486 LINE",
+"100 417 LINE",
+"100 397 LINE"
+);
+}
+);
+width = 463;
+},
+{
+layerId = "3E7589AA-8194-470F-8E2F-13C1C581BE24";
+paths = (
+{
+closed = 1;
+nodes = (
+"363 446 LINE",
+"363 486 LINE",
+"100 417 LINE",
+"100 377 LINE"
+);
+}
+);
+width = 463;
+},
+{
+layerId = "BFFFD157-90D3-4B85-B99D-9A2F366F03CA";
+paths = (
+{
+closed = 1;
+nodes = (
+"363 426 LINE",
+"363 486 LINE",
+"100 417 LINE",
+"100 357 LINE"
+);
+}
+);
+width = 463;
+}
+);
+unicode = 064E;
+},
+{
 glyphname = dieresis;
 lastChange = "2015-12-31 14:44:23 +0000";
 layers = (
 {
 anchors = (
 {
 name = _top;
```

## Comparing `fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont.designspace` & `fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif` & `fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.alt.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif` & `fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif` & `fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif` & `fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Black.ufo/glyphs/Q_.ss01.alt.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif` & `fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.alt.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif` & `fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif` & `fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif` & `fontmake-3.7.0b1/tests/data/DesignspaceRuleOrder/MyFont_Hair.ufo/glyphs/Q_.ss01.alt.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/kerning.plist` & `fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/kerning.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif` & `fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/y.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif` & `fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/a.swap.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist` & `fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif` & `fontmake-3.7.0b1/tests/data/SwapGlyphNames/A.ufo/glyphs/x.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif` & `fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif` & `fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/dieresiscomb.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif` & `fontmake-3.7.0b1/tests/data/SwapGlyphNames/B.ufo/glyphs/a.alt.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph` & `fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.sc.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph` & `fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/n.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph` & `fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/h.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph` & `fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/m.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph` & `fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/A_.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph` & `fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/dieresis.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph` & `fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.shoulder.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph` & `fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/a.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph` & `fontmake-3.7.0b1/tests/data/GlyphsUnitTestSans3.glyphspackage/glyphs/_part.stem.glyph`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest.designspace` & `fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufoz` & `fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufoz`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace` & `fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-instance-attrs.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace` & `fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-slnt.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace` & `fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-opsz.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace` & `fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-lib.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace` & `fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-wght-wdth.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufoz` & `fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufoz`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace` & `fontmake-3.7.0b1/tests/data/DesignspaceTest/DesignspaceTest-bare.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Light.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/DesignspaceTest/MyFont-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace` & `fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/StrictMathGlyph.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif` & `fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareOne.ufo/glyphs/test.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif` & `fontmake-3.7.0b1/tests/data/InstantiatorStrictMathGlyph/SquareTwo.ufo/glyphs/test.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace` & `fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/DesignspaceTest.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace` & `fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/Designspace-MastersAsInstances.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Light.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/DesignspaceBrokenTest/MyFont-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist` & `fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs` & `fontmake-3.7.0b1/tests/data/InterpolateLayoutTest/InterpolateLayoutTest.glyphs`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/AutohintingTest/Padyakke.glyphs` & `fontmake-3.7.0b1/tests/data/AutohintingTest/Padyakke.glyphs`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans.designspace` & `fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif` & `fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif` & `fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif` & `fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Bold.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif` & `fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif` & `fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif` & `fontmake-3.7.0b1/tests/data/IncompatibleSans/IncompatibleSans-Regular.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace` & `fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTestSharedFeatures.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Regular.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/DesignspaceTestSharedFeatures/DesignspaceTest-Light.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSans_missing.designspace` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans_missing.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSans.designspace` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSans-width-only.designspace` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans-width-only.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans-with-openNodes.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSans-weight-only.designspace` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans-weight-only.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans-non-default-layer.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/LICENSE` & `fontmake-3.7.0b1/tests/data/MutatorSans/LICENSE`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSans_no_default.designspace` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSans_no_default.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/kerning.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowright.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowdown.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowleft.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightWide.ufo/glyphs/arrowup.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/layercontents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.reference.interpolation/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateCondensed.ufo/glyphs.interpolation/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/kerning.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotedblbase.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldCondensed.ufo/glyphs/quotesinglbase.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/kerning.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansIntermediateWide.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansBoldWide.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/layercontents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/kerning.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/W_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/W_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/T_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/R_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/O_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/G_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/D_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/X_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/M_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Z_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/F_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/C_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowright.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/B_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/U_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/N_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/V_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/comma.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/contents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/Y_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/L_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowdown.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/P_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowleft.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/K_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/H_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs/arrowup.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSans/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSans_v5_several_vfs_discrete_axis.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSans_v5_implicit_one_vf.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/LICENSE` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/LICENSE`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorFamily_v5_discrete_axis.designspace`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_720.00_weight_645.00/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs.master_width_500.00_weight_500.00/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSerifLightCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansBoldWide.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/layercontents.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/lib.plist`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.background/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbar/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.middle/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.narrow.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/I_J_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs/S_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.crossbars/E_.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.closed.glif`

 * *Files identical despite different names*

## Comparing `fontmake-3.6.1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif` & `fontmake-3.7.0b1/tests/data/MutatorSansLite/MutatorSansLightCondensed.ufo/glyphs.support.S_.wide/S_.glif`

 * *Files identical despite different names*

