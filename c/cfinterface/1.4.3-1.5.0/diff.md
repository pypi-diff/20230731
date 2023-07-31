# Comparing `tmp/cfinterface-1.4.3.tar.gz` & `tmp/cfinterface-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfinterface-1.4.3.tar", last modified: Wed Jul 19 17:34:41 2023, max compression
+gzip compressed data, was "cfinterface-1.5.0.tar", last modified: Mon Jul 31 14:11:13 2023, max compression
```

## Comparing `cfinterface-1.4.3.tar` & `cfinterface-1.5.0.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.627362 cfinterface-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-19 17:33:13.000000 cfinterface-1.4.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-19 17:34:41.623361 cfinterface-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-19 17:33:13.000000 cfinterface-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.611360 cfinterface-1.4.3/cfinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.611360 cfinterface-1.4.3/cfinterface/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.611360 cfinterface-1.4.3/cfinterface/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.611360 cfinterface-1.4.3/cfinterface/adapters/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/adapters/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.611360 cfinterface-1.4.3/cfinterface/adapters/components/line/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/adapters/components/line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/adapters/components/line/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/adapters/components/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.611360 cfinterface-1.4.3/cfinterface/adapters/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/adapters/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/adapters/reading/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.615361 cfinterface-1.4.3/cfinterface/adapters/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/adapters/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/adapters/writing/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.615361 cfinterface-1.4.3/cfinterface/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/components/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/components/datetimefield.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/components/defaultblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/components/defaultregister.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/components/defaultsection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/components/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/components/floatfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/components/integerfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/components/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/components/literalfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/components/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/components/section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.615361 cfinterface-1.4.3/cfinterface/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/data/blockdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/data/registerdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/data/sectiondata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.615361 cfinterface-1.4.3/cfinterface/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/files/blockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/files/registerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/files/sectionfile.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.619361 cfinterface-1.4.3/cfinterface/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/reading/blockreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/reading/registerreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/reading/sectionreading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.619361 cfinterface-1.4.3/cfinterface/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/writing/blockwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/writing/registerwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-19 17:33:13.000000 cfinterface-1.4.3/cfinterface/writing/sectionwriting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.611360 cfinterface-1.4.3/cfinterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-19 17:34:41.000000 cfinterface-1.4.3/cfinterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-19 17:34:41.000000 cfinterface-1.4.3/cfinterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 17:34:41.000000 cfinterface-1.4.3/cfinterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-19 17:34:41.000000 cfinterface-1.4.3/cfinterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-19 17:34:41.000000 cfinterface-1.4.3/cfinterface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.619361 cfinterface-1.4.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 17:34:41.627362 cfinterface-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-19 17:33:13.000000 cfinterface-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.619361 cfinterface-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.619361 cfinterface-1.4.3/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.619361 cfinterface-1.4.3/tests/adapters/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/adapters/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/adapters/components/test_blockrepository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/adapters/components/test_linerepository.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/adapters/components/test_registerrepository.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/adapters/components/test_sectionrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.619361 cfinterface-1.4.3/tests/adapters/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/adapters/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/adapters/reading/test_readingrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.619361 cfinterface-1.4.3/tests/adapters/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/adapters/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/adapters/writing/test_writingrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.623361 cfinterface-1.4.3/tests/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/components/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/components/test_datetimefield.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/components/test_defaultblock.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/components/test_defaultregister.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/components/test_defaultsection.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/components/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/components/test_floatfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/components/test_integerfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/components/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/components/test_literalfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/components/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/components/test_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.623361 cfinterface-1.4.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/data/test_blockdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/data/test_registerdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/data/test_sectiondata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.623361 cfinterface-1.4.3/tests/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/files/test_blockfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/files/test_registerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/files/test_sectionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.623361 cfinterface-1.4.3/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/mocks/mock_open.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.623361 cfinterface-1.4.3/tests/reading/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/reading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/reading/test_blockreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/reading/test_registerreading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/reading/test_sectionreading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 17:34:41.623361 cfinterface-1.4.3/tests/writing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/writing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/writing/test_blockwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/writing/test_registerwriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-19 17:33:13.000000 cfinterface-1.4.3/tests/writing/test_sectionwriting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.546782 cfinterface-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 14:09:47.000000 cfinterface-1.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-31 14:11:13.546782 cfinterface-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-31 14:09:47.000000 cfinterface-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.530781 cfinterface-1.5.0/cfinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.530781 cfinterface-1.5.0/cfinterface/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.530781 cfinterface-1.5.0/cfinterface/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.530781 cfinterface-1.5.0/cfinterface/adapters/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.530781 cfinterface-1.5.0/cfinterface/adapters/components/line/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/components/line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/components/line/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/components/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.530781 cfinterface-1.5.0/cfinterface/adapters/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/reading/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.534781 cfinterface-1.5.0/cfinterface/adapters/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/adapters/writing/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.534781 cfinterface-1.5.0/cfinterface/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/datetimefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/defaultblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/defaultregister.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/defaultsection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/floatfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/integerfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/literalfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/components/section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.534781 cfinterface-1.5.0/cfinterface/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/data/blockdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/data/registerdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/data/sectiondata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.534781 cfinterface-1.5.0/cfinterface/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/files/blockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/files/registerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/files/sectionfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/cfinterface/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/reading/blockreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/reading/registerreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/reading/sectionreading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/cfinterface/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/writing/blockwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/writing/registerwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-31 14:09:47.000000 cfinterface-1.5.0/cfinterface/writing/sectionwriting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.530781 cfinterface-1.5.0/cfinterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-31 14:11:13.000000 cfinterface-1.5.0/cfinterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-31 14:11:13.000000 cfinterface-1.5.0/cfinterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:11:13.000000 cfinterface-1.5.0/cfinterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 14:11:13.000000 cfinterface-1.5.0/cfinterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-31 14:11:13.000000 cfinterface-1.5.0/cfinterface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:11:13.546782 cfinterface-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-31 14:09:47.000000 cfinterface-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/tests/adapters/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/components/test_blockrepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/components/test_linerepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/components/test_registerrepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/components/test_sectionrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/tests/adapters/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/reading/test_readingrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.538782 cfinterface-1.5.0/tests/adapters/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/adapters/writing/test_writingrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.542782 cfinterface-1.5.0/tests/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_datetimefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_defaultblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_defaultregister.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_defaultsection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_floatfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_integerfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_literalfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/components/test_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.542782 cfinterface-1.5.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/data/test_blockdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/data/test_registerdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/data/test_sectiondata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.542782 cfinterface-1.5.0/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/files/test_blockfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/files/test_registerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/files/test_sectionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.542782 cfinterface-1.5.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.542782 cfinterface-1.5.0/tests/reading/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/reading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/reading/test_blockreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/reading/test_registerreading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/reading/test_sectionreading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:11:13.546782 cfinterface-1.5.0/tests/writing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/writing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/writing/test_blockwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/writing/test_registerwriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-31 14:09:47.000000 cfinterface-1.5.0/tests/writing/test_sectionwriting.py
```

### Comparing `cfinterface-1.4.3/LICENSE.md` & `cfinterface-1.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/PKG-INFO` & `cfinterface-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfinterface
-Version: 1.4.3
+Version: 1.5.0
 Summary: Interface for handling custom formatted files
 Home-page: https://github.com/rjmalves/cfi
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfinterface-1.4.3/README.md` & `cfinterface-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/adapters/components/line/repository.py` & `cfinterface-1.5.0/cfinterface/adapters/components/line/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/adapters/components/repository.py` & `cfinterface-1.5.0/cfinterface/adapters/components/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/adapters/reading/repository.py` & `cfinterface-1.5.0/cfinterface/adapters/reading/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/adapters/writing/repository.py` & `cfinterface-1.5.0/cfinterface/adapters/writing/repository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/components/block.py` & `cfinterface-1.5.0/cfinterface/components/block.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/components/datetimefield.py` & `cfinterface-1.5.0/cfinterface/components/datetimefield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/components/defaultblock.py` & `cfinterface-1.5.0/cfinterface/components/defaultblock.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/components/defaultregister.py` & `cfinterface-1.5.0/cfinterface/components/defaultregister.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/components/defaultsection.py` & `cfinterface-1.5.0/cfinterface/components/defaultsection.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/components/field.py` & `cfinterface-1.5.0/cfinterface/components/field.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/components/floatfield.py` & `cfinterface-1.5.0/cfinterface/components/floatfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/components/integerfield.py` & `cfinterface-1.5.0/cfinterface/components/integerfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/components/line.py` & `cfinterface-1.5.0/cfinterface/components/line.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/components/literalfield.py` & `cfinterface-1.5.0/cfinterface/components/literalfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/components/register.py` & `cfinterface-1.5.0/cfinterface/components/register.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/components/section.py` & `cfinterface-1.5.0/cfinterface/components/section.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/data/blockdata.py` & `cfinterface-1.5.0/cfinterface/data/blockdata.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, Type, Generator
+from typing import TypeVar, Type, Generator, Optional, Union, List
 
 from cfinterface.components.block import Block
 
 
 class BlockData:
     """
     Class for a storing, managing and accessing data for a block file.
@@ -13,14 +13,15 @@
     def __init__(self, root: Block) -> None:
         self.__root = root
         self.__head = root
 
     def __iter__(self):
         current = self.__root
         while current:
+            print(current.data)
             yield current
             current = current.next
 
     def __len__(self) -> int:
         count = 0
         for _ in self:
             count += 1
@@ -63,14 +64,16 @@
         :param before: The existing block which will be preppended
         :type before: Block
         :param new: The new block to add to the data
         :type new: Block
         """
         if before == self.__root:
             self.__root = new
+        else:
+            before.previous.next = new
         new.previous = before.previous
         before.previous = new
         new.next = before
 
     def add_after(self, after: Block, new: Block):
         """
         Adds a new block to the data after another
@@ -79,14 +82,16 @@
         :param after: The existing block which will be appended
         :type after: Block
         :param new: The new block to add to the data
         :type new: Block
         """
         if after == self.__head:
             self.__head = new
+        else:
+            after.next.previous = new
         new.next = after.next
         after.next = new
         new.previous = after
 
     def remove(self, b: Block):
         """
         Removes an existing block in the chain.
@@ -108,14 +113,44 @@
         :yield: Blocks filtered by type T
         :rtype: Generator[T, None, None]
         """
         for b in self:
             if isinstance(b, t):
                 yield b
 
+    def get_blocks_of_type(
+        self, t: Type[T], **kwargs
+    ) -> Optional[Union[T, List[T]]]:
+        """
+        A block or block list that only returns
+        blocks of type T that meet
+        given filter requirements passed as kwargs.
+
+        :param t: The block type that is desired
+        :type t: Type[T]
+        :return: Blocks filtered by type T and optional properties
+        :rtype: T | list[T] | None
+        """
+
+        def __meets(r) -> bool:
+            conditions: List[bool] = []
+            for k, v in kwargs.items():
+                if v is not None:
+                    conditions.append(getattr(r, k) == v)
+            return all(conditions)
+
+        all_blocks_of_type = [b for b in self.of_type(t)]
+        filtered_blocks = [r for r in all_blocks_of_type if __meets(r)]
+        if len(filtered_blocks) == 0:
+            return None
+        elif len(filtered_blocks) == 1:
+            return filtered_blocks[0]
+        else:
+            return filtered_blocks
+
     @property
     def first(self) -> Block:
         return self.__root
 
     @property
     def last(self) -> Block:
         return self.__head
```

### Comparing `cfinterface-1.4.3/cfinterface/data/registerdata.py` & `cfinterface-1.5.0/cfinterface/data/registerdata.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, Type, Generator
+from typing import TypeVar, Type, Generator, Optional, Union, List
 
 from cfinterface.components.register import Register
 
 
 class RegisterData:
     """
     Class for a storing, managing and accessing data for a register file.
@@ -63,14 +63,16 @@
         :param before: The existing register which will be preppended
         :type before: Register
         :param new: The new register to add to the data
         :type new: Register
         """
         if before == self.__root:
             self.__root = new
+        else:
+            before.previous.next = new
         new.previous = before.previous
         before.previous = new
         new.next = before
 
     def add_after(self, after: Register, new: Register):
         """
         Adds a new register to the data after another
@@ -79,14 +81,16 @@
         :param after: The existing register which will be appended
         :type after: Register
         :param new: The new register to add to the data
         :type new: Register
         """
         if after == self.__head:
             self.__head = new
+        else:
+            after.next.previous = new
         new.next = after.next
         after.next = new
         new.previous = after
 
     def remove(self, r: Register):
         """
         Removes an existing register in the chain.
@@ -108,14 +112,44 @@
         :yield: Registers filtered by type T
         :rtype: Generator[T, None, None]
         """
         for r in self:
             if isinstance(r, t):
                 yield r
 
+    def get_registers_of_type(
+        self, t: Type[T], **kwargs
+    ) -> Optional[Union[T, List[T]]]:
+        """
+        A register or register list that only returns
+        registers of type T that meet
+        given filter requirements passed as kwargs.
+
+        :param t: The register type that is desired
+        :type t: Type[T]
+        :return: Registers filtered by type T and optional properties
+        :rtype: T | list[T] | None
+        """
+
+        def __meets(r) -> bool:
+            conditions: List[bool] = []
+            for k, v in kwargs.items():
+                if v is not None:
+                    conditions.append(getattr(r, k) == v)
+            return all(conditions)
+
+        all_registers_of_type = [b for b in self.of_type(t)]
+        filtered_registers = [r for r in all_registers_of_type if __meets(r)]
+        if len(filtered_registers) == 0:
+            return None
+        elif len(filtered_registers) == 1:
+            return filtered_registers[0]
+        else:
+            return filtered_registers
+
     @property
     def first(self) -> Register:
         return self.__root
 
     @property
     def last(self) -> Register:
         return self.__head
```

### Comparing `cfinterface-1.4.3/cfinterface/data/sectiondata.py` & `cfinterface-1.5.0/cfinterface/data/sectiondata.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, Type, Generator
+from typing import TypeVar, Type, Generator, Optional, Union, List
 
 from cfinterface.components.section import Section
 
 
 class SectionData:
     """
     Class for a storing, managing and accessing data for a section file.
@@ -63,14 +63,16 @@
         :param before: The existing section which will be preppended
         :type before: Section
         :param new: The new section to add to the data
         :type new: Section
         """
         if before == self.__root:
             self.__root = new
+        else:
+            before.previous.next = new
         new.previous = before.previous
         before.previous = new
         new.next = before
 
     def add_after(self, after: Section, new: Section):
         """
         Adds a new section to the data after another
@@ -79,14 +81,16 @@
         :param after: The existing section which will be appended
         :type after: Section
         :param new: The new section to add to the data
         :type new: Section
         """
         if after == self.__head:
             self.__head = new
+        else:
+            after.next.previous = new
         new.next = after.next
         after.next = new
         new.previous = after
 
     def remove(self, s: Section):
         """
         Removes an existing section in the chain.
@@ -108,14 +112,44 @@
         :yield: Sections filtered by type T
         :rtype: Generator[T, None, None]
         """
         for s in self:
             if isinstance(s, t):
                 yield s
 
+    def get_sections_of_type(
+        self, t: Type[T], **kwargs
+    ) -> Optional[Union[T, List[T]]]:
+        """
+        A section or section list that only returns
+        sections of type T that meet
+        given filter requirements passed as kwargs.
+
+        :param t: The section type that is desired
+        :type t: Type[T]
+        :return: Sections filtered by type T and optional properties
+        :rtype: T | list[T] | None
+        """
+
+        def __meets(r) -> bool:
+            conditions: List[bool] = []
+            for k, v in kwargs.items():
+                if v is not None:
+                    conditions.append(getattr(r, k) == v)
+            return all(conditions)
+
+        all_sections_of_type = [b for b in self.of_type(t)]
+        filtered_sections = [r for r in all_sections_of_type if __meets(r)]
+        if len(filtered_sections) == 0:
+            return None
+        elif len(filtered_sections) == 1:
+            return filtered_sections[0]
+        else:
+            return filtered_sections
+
     @property
     def first(self) -> Section:
         return self.__root
 
     @property
     def last(self) -> Section:
         return self.__head
```

### Comparing `cfinterface-1.4.3/cfinterface/files/blockfile.py` & `cfinterface-1.5.0/cfinterface/files/blockfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,28 @@
         :type to: str | IO
         """
         writer = BlockWriting(self.__data, self.__storage)
         writer.write(to, self.__encoding, *args, **kwargs)
 
     @property
     def data(self) -> BlockData:
+        """
+        Exposes the :class:`BlockData` object, which gives access
+        to the methods:
+
+        - `preppend()`
+        - `append()`
+        - `add_before()`
+        - `add_after()`
+        - `get_blocks_of_type()`
+
+
+        :return: The data internal object
+        :rtype: :class:`BlockData`
+        """
         return self.__data
 
     @classmethod
     def set_version(cls, v: str):
         """
         Sets the file's version to be read. Different file versions
         may contain different blocks. The version to be set is considered
```

### Comparing `cfinterface-1.4.3/cfinterface/files/registerfile.py` & `cfinterface-1.5.0/cfinterface/files/registerfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,28 @@
         :type to: str | IO
         """
         writer = RegisterWriting(self.__data, self.__storage, *args, **kwargs)
         writer.write(to, self.__encoding, *args, **kwargs)
 
     @property
     def data(self) -> RegisterData:
+        """
+        Exposes the :class:`RegisterData` object, which gives access
+        to the methods:
+
+        - `preppend()`
+        - `append()`
+        - `add_before()`
+        - `add_after()`
+        - `get_blocks_of_type()`
+
+
+        :return: The data internal object
+        :rtype: :class:`RegisterData`
+        """
         return self.__data
 
     @classmethod
     def set_version(cls, v: str):
         """
         Sets the file's version to be read. Different file versions
         may contain different registers. The version to be set is considered
```

### Comparing `cfinterface-1.4.3/cfinterface/files/sectionfile.py` & `cfinterface-1.5.0/cfinterface/files/sectionfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,14 +53,28 @@
         :type to: str | IO
         """
         writer = SectionWriting(self.__data, self.__storage)
         writer.write(to, self.__encoding, *args, **kwargs)
 
     @property
     def data(self) -> SectionData:
+        """
+        Exposes the :class:`SectionData` object, which gives access
+        to the methods:
+
+        - `preppend()`
+        - `append()`
+        - `add_before()`
+        - `add_after()`
+        - `get_blocks_of_type()`
+
+
+        :return: The data internal object
+        :rtype: :class:`SectionData`
+        """
         return self.__data
 
     @classmethod
     def set_version(cls, v: str):
         """
         Sets the file's version to be read. Different file versions
         may contain different sections. The version to be set is considered
```

### Comparing `cfinterface-1.4.3/cfinterface/reading/blockreading.py` & `cfinterface-1.5.0/cfinterface/reading/blockreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/reading/registerreading.py` & `cfinterface-1.5.0/cfinterface/reading/registerreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/reading/sectionreading.py` & `cfinterface-1.5.0/cfinterface/reading/sectionreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/writing/blockwriting.py` & `cfinterface-1.5.0/cfinterface/writing/blockwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/writing/registerwriting.py` & `cfinterface-1.5.0/cfinterface/writing/registerwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface/writing/sectionwriting.py` & `cfinterface-1.5.0/cfinterface/writing/sectionwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/cfinterface.egg-info/PKG-INFO` & `cfinterface-1.5.0/cfinterface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfinterface
-Version: 1.4.3
+Version: 1.5.0
 Summary: Interface for handling custom formatted files
 Home-page: https://github.com/rjmalves/cfi
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cfinterface-1.4.3/cfinterface.egg-info/SOURCES.txt` & `cfinterface-1.5.0/cfinterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/setup.py` & `cfinterface-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/adapters/components/test_linerepository.py` & `cfinterface-1.5.0/tests/adapters/components/test_linerepository.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/components/test_block.py` & `cfinterface-1.5.0/tests/components/test_block.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/components/test_datetimefield.py` & `cfinterface-1.5.0/tests/components/test_datetimefield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/components/test_defaultblock.py` & `cfinterface-1.5.0/tests/components/test_defaultblock.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/components/test_defaultregister.py` & `cfinterface-1.5.0/tests/components/test_defaultregister.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/components/test_defaultsection.py` & `cfinterface-1.5.0/tests/components/test_defaultsection.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/components/test_floatfield.py` & `cfinterface-1.5.0/tests/components/test_floatfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/components/test_integerfield.py` & `cfinterface-1.5.0/tests/components/test_integerfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/components/test_line.py` & `cfinterface-1.5.0/tests/components/test_line.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/components/test_literalfield.py` & `cfinterface-1.5.0/tests/components/test_literalfield.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/components/test_register.py` & `cfinterface-1.5.0/tests/components/test_register.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/components/test_section.py` & `cfinterface-1.5.0/tests/components/test_section.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/data/test_blockdata.py` & `cfinterface-1.5.0/tests/data/test_blockdata.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, self.__class__):
             return False
         else:
             return o.data == self.data
 
+    @property
+    def my_data(self):
+        return self.data
+
 
 def test_blockdata_eq():
     bd1 = BlockData(DummyBlock(data=-1))
     bd2 = BlockData(DummyBlock(data=-1))
     assert bd1 == bd2
 
 
@@ -49,33 +53,75 @@
     bd = BlockData(DummyBlock(data=-1))
     b1 = DummyBlock(data=1)
     bd.append(b1)
     b2 = DummyBlock(data=2)
     bd.add_before(b1, b2)
     assert b1.previous == b2
     assert b2.next == b1
+    assert bd.last == b1
+    assert len(bd) == 3
+
+
+def test_blockdata_add_before_root():
+    b1 = DummyBlock(data=-1)
+    bd = BlockData(b1)
+    b2 = DummyBlock(data=2)
+    bd.add_before(b1, b2)
+    assert b1.previous == b2
+    assert b2.next == b1
+    assert bd.last == b1
+    assert len(bd) == 2
 
 
 def test_blockdata_add_after():
     bd = BlockData(DummyBlock(data=-1))
     b1 = DummyBlock(data=1)
     bd.append(b1)
     b2 = DummyBlock(data=2)
     bd.add_after(b1, b2)
     assert b1.next == b2
     assert b2.previous == b1
+    assert bd.last == b2
+    assert len(bd) == 3
+
+
+def test_blockdata_add_after_head():
+    b1 = DummyBlock(data=-1)
+    bd = BlockData(b1)
+    b2 = DummyBlock(data=2)
+    bd.add_after(b1, b2)
+    assert b1.next == b2
+    assert b2.previous == b1
+    assert bd.last == b2
+    assert len(bd) == 2
 
 
 def test_blockdata_remove():
     bd = BlockData(DummyBlock(data=-1))
     b1 = DummyBlock(data=1)
     bd.append(b1)
     assert len(bd) == 2
     bd.remove(b1)
     assert len(bd) == 1
 
 
 def test_blockdata_of_type():
     bd = BlockData(DummyBlock())
-    bd.append(Block())
+    bd.append(DummyBlock())
     assert len(bd) == 2
-    assert len([b for b in bd.of_type(DummyBlock)]) == 1
+    assert len([b for b in bd.of_type(DummyBlock)]) == 2
+
+
+def test_blockdata_get_blocks_of_type_no_filter():
+    b1 = DummyBlock(data=10)
+    bd = BlockData(b1)
+    bd.append(Block())
+    assert bd.get_blocks_of_type(DummyBlock) == b1
+
+
+def test_blockdata_get_blocks_of_type_filter():
+    b1 = DummyBlock(data=10)
+    bd = BlockData(b1)
+    bd.append(DummyBlock())
+    bd.append(DummyBlock(data=11))
+    assert len(bd.get_blocks_of_type(DummyBlock)) == 3
+    assert bd.get_blocks_of_type(DummyBlock, my_data=10) == b1
```

### Comparing `cfinterface-1.4.3/tests/data/test_registerdata.py` & `cfinterface-1.5.0/tests/data/test_registerdata.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 
 class DummyRegister(Register):
     IDENTIFIER = "reg"
     IDENTIFIER_DIGITS = 4
     LINE = Line([LiteralField(13, 4)])
 
+    @property
+    def my_data(self):
+        return self.data[0]
+
 
 def test_registerdata_eq():
     rd1 = RegisterData(DummyRegister(data=-1))
     rd2 = RegisterData(DummyRegister(data=-1))
     assert rd1 == rd2
 
 
@@ -46,33 +50,75 @@
     rd = RegisterData(DummyRegister(data=-1))
     r1 = DummyRegister(data=1)
     rd.append(r1)
     r2 = DummyRegister(data=2)
     rd.add_before(r1, r2)
     assert r1.previous == r2
     assert r2.next == r1
+    assert rd.last == r1
+    assert len(rd) == 3
+
+
+def test_registerdata_add_before_root():
+    r1 = DummyRegister(data=-1)
+    rd = RegisterData(r1)
+    r2 = DummyRegister(data=2)
+    rd.add_before(r1, r2)
+    assert r1.previous == r2
+    assert r2.next == r1
+    assert rd.last == r1
+    assert len(rd) == 2
 
 
 def test_registerdata_add_after():
     rd = RegisterData(DummyRegister(data=-1))
     r1 = DummyRegister(data=1)
     rd.append(r1)
     r2 = DummyRegister(data=2)
     rd.add_after(r1, r2)
     assert r1.next == r2
     assert r2.previous == r1
+    assert rd.last == r2
+    assert len(rd) == 3
+
+
+def test_registerdata_add_after_head():
+    r1 = DummyRegister(data=-1)
+    rd = RegisterData(r1)
+    r2 = DummyRegister(data=2)
+    rd.add_after(r1, r2)
+    assert r1.next == r2
+    assert r2.previous == r1
+    assert rd.last == r2
+    assert len(rd) == 2
 
 
 def test_registerdata_remove():
     rd = RegisterData(DummyRegister(data=-1))
     r1 = DummyRegister(data=1)
     rd.append(r1)
     assert len(rd) == 2
     rd.remove(r1)
     assert len(rd) == 1
 
 
 def test_registerdata_of_type():
     rd = RegisterData(DummyRegister())
-    rd.append(Register())
+    rd.append(DummyRegister())
     assert len(rd) == 2
-    assert len([b for b in rd.of_type(DummyRegister)]) == 1
+    assert len([b for b in rd.of_type(DummyRegister)]) == 2
+
+
+def test_RegisterData_get_registers_of_type_no_filter():
+    r1 = DummyRegister(data=[10])
+    rd = RegisterData(r1)
+    rd.append(Register())
+    assert rd.get_registers_of_type(DummyRegister) == r1
+
+
+def test_RegisterData_get_registers_of_type_filter():
+    r1 = DummyRegister(data=[10])
+    rd = RegisterData(r1)
+    rd.append(DummyRegister())
+    rd.append(DummyRegister(data=[11]))
+    assert len(rd.get_registers_of_type(DummyRegister)) == 3
+    assert rd.get_registers_of_type(DummyRegister, my_data=10) == r1
```

### Comparing `cfinterface-1.4.3/tests/data/test_sectiondata.py` & `cfinterface-1.5.0/tests/data/test_sectiondata.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,74 +5,120 @@
 class DummySection(Section):
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, self.__class__):
             return False
         else:
             return o.data == self.data
 
+    @property
+    def my_data(self):
+        return self.data
 
-def test_blockdata_eq():
+
+def test_sectiondata_eq():
     sd1 = SectionData(DummySection(data=-1))
     sd2 = SectionData(DummySection(data=-1))
     assert sd1 == sd2
 
 
-def test_blockdata_not_eq():
+def test_sectiondata_not_eq():
     sd1 = SectionData(DummySection(data=-1))
     sd2 = SectionData(DummySection(data=+1))
     assert sd1 != sd2
 
 
-def test_blockdata_append():
+def test_sectiondata_append():
     sd = SectionData(DummySection(data=-1))
     n_sections = 10
     for i in range(n_sections):
         sd.append(DummySection(data=i))
     assert len(sd) == n_sections + 1
     assert sd.first.data == -1
     assert sd.last.data == n_sections - 1
 
 
-def test_blockdata_preppend():
+def test_sectiondata_preppend():
     sd = SectionData(DummySection(data=-1))
     n_sections = 10
     for i in range(n_sections):
         sd.preppend(DummySection(data=i))
     assert len(sd) == n_sections + 1
     assert sd.first.data == n_sections - 1
     assert sd.last.data == -1
 
 
-def test_blockdata_add_before():
+def test_sectiondata_add_before():
     sd = SectionData(DummySection(data=-1))
     s1 = DummySection(data=1)
     sd.append(s1)
     s2 = DummySection(data=2)
     sd.add_before(s1, s2)
     assert s1.previous == s2
     assert s2.next == s1
+    assert sd.last == s1
+    assert len(sd) == 3
+
+
+def test_sectiondata_add_before_root():
+    s1 = DummySection(data=1)
+    sd = SectionData(s1)
+    s2 = DummySection(data=2)
+    sd.add_before(s1, s2)
+    assert s1.previous == s2
+    assert s2.next == s1
+    assert sd.last == s1
+    assert len(sd) == 2
 
 
-def test_blockdata_add_after():
+def test_sectiondata_add_after():
     sd = SectionData(DummySection(data=-1))
     s1 = DummySection(data=1)
     sd.append(s1)
     s2 = DummySection(data=2)
     sd.add_after(s1, s2)
     assert s1.next == s2
     assert s2.previous == s1
+    assert sd.last == s2
+    assert len(sd) == 3
+
+
+def test_sectiondata_add_after_head():
+    s1 = DummySection(data=-1)
+    sd = SectionData(s1)
+    s2 = DummySection(data=2)
+    sd.add_after(s1, s2)
+    assert s1.next == s2
+    assert s2.previous == s1
+    assert sd.last == s2
+    assert len(sd) == 2
 
 
-def test_blockdata_remove():
+def test_sectiondata_remove():
     sd = SectionData(DummySection(data=-1))
     s1 = DummySection(data=1)
     sd.append(s1)
     assert len(sd) == 2
     sd.remove(s1)
     assert len(sd) == 1
 
 
-def test_blockdata_of_type():
+def test_sectiondata_of_type():
     sd = SectionData(DummySection())
     sd.append(Section())
     assert len(sd) == 2
     assert len([b for b in sd.of_type(DummySection)]) == 1
+
+
+def test_sectiondata_get_sections_of_type_no_filter():
+    b1 = DummySection(data=10)
+    bd = SectionData(b1)
+    bd.append(Section())
+    assert bd.get_sections_of_type(DummySection) == b1
+
+
+def test_sectiondata_get_sections_of_type_filter():
+    b1 = DummySection(data=10)
+    bd = SectionData(b1)
+    bd.append(DummySection())
+    bd.append(DummySection(data=11))
+    assert len(bd.get_sections_of_type(DummySection)) == 3
+    assert bd.get_sections_of_type(DummySection, my_data=10) == b1
```

### Comparing `cfinterface-1.4.3/tests/files/test_blockfile.py` & `cfinterface-1.5.0/tests/files/test_blockfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/files/test_registerfile.py` & `cfinterface-1.5.0/tests/files/test_registerfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/files/test_sectionfile.py` & `cfinterface-1.5.0/tests/files/test_sectionfile.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/mocks/mock_open.py` & `cfinterface-1.5.0/tests/mocks/mock_open.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/reading/test_blockreading.py` & `cfinterface-1.5.0/tests/reading/test_blockreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/reading/test_registerreading.py` & `cfinterface-1.5.0/tests/reading/test_registerreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/reading/test_sectionreading.py` & `cfinterface-1.5.0/tests/reading/test_sectionreading.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/writing/test_blockwriting.py` & `cfinterface-1.5.0/tests/writing/test_blockwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/writing/test_registerwriting.py` & `cfinterface-1.5.0/tests/writing/test_registerwriting.py`

 * *Files identical despite different names*

### Comparing `cfinterface-1.4.3/tests/writing/test_sectionwriting.py` & `cfinterface-1.5.0/tests/writing/test_sectionwriting.py`

 * *Files identical despite different names*

