# Comparing `tmp/createrepo_c-0.21.1.tar.gz` & `tmp/createrepo_c-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "createrepo_c-0.21.1.tar", last modified: Tue Apr  4 10:37:51 2023, max compression
+gzip compressed data, was "createrepo_c-1.0.0.tar", last modified: Mon Jul 31 05:41:20 2023, max compression
```

## Comparing `createrepo_c-0.21.1.tar` & `createrepo_c-1.0.0.tar`

### file list

```diff
@@ -1,506 +1,510 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.885487 createrepo_c-0.21.1/
--rw-rw-r--   0 root         (0) root         (0)      499 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/AUTHORS
--rw-rw-r--   0 root         (0) root         (0)     5791 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)    18092 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/COPYING
--rw-rw-r--   0 root         (0) root         (0)      198 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      812 2023-04-04 10:37:51.885487 createrepo_c-0.21.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    11433 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/README.md
--rw-rw-r--   0 root         (0) root         (0)       55 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/VERSION.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.841485 createrepo_c-0.21.1/doc/
--rw-rw-r--   0 root         (0) root         (0)      637 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/doc/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)   114986 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/doc/Doxyfile.in.in
--rw-rw-r--   0 root         (0) root         (0)     8725 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/doc/createrepo_c.8
--rw-rw-r--   0 root         (0) root         (0)     1523 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/doc/logo.png
--rw-rw-r--   0 root         (0) root         (0)    80453 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/doc/logo.xcf
--rw-rw-r--   0 root         (0) root         (0)     3476 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/doc/mergerepo_c.8
--rw-rw-r--   0 root         (0) root         (0)     2164 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/doc/modifyrepo_c.8
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.841485 createrepo_c-0.21.1/doc/python/
--rw-rw-r--   0 root         (0) root         (0)      255 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/doc/python/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)     8128 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/doc/python/conf.py
--rw-rw-r--   0 root         (0) root         (0)      307 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/doc/python/index.rst
--rw-rw-r--   0 root         (0) root         (0)      550 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/doc/python/lib.rst
--rw-rw-r--   0 root         (0) root         (0)     1772 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/doc/sqliterepo_c.8
--rw-rw-r--   0 root         (0) root         (0)      140 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       30 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-04 10:37:51.885487 createrepo_c-0.21.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2000 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.849485 createrepo_c-0.21.1/src/
--rw-rw-r--   0 root         (0) root         (0)     4658 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)     8242 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/checksum.c
--rw-rw-r--   0 root         (0) root         (0)     3660 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/checksum.h
--rw-rw-r--   0 root         (0) root         (0)     4014 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/cleanup.h
--rw-rw-r--   0 root         (0) root         (0)    29168 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/cmd_parser.c
--rw-rw-r--   0 root         (0) root         (0)     9165 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/cmd_parser.h
--rw-rw-r--   0 root         (0) root         (0)    54854 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/compression_wrapper.c
--rw-rw-r--   0 root         (0) root         (0)     8210 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/compression_wrapper.h
--rw-rw-r--   0 root         (0) root         (0)     1138 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/constants.h
--rw-rw-r--   0 root         (0) root         (0)   107815 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/createrepo_c.c
--rw-rw-r--   0 root         (0) root         (0)     1654 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/createrepo_c.h
--rw-rw-r--   0 root         (0) root         (0)      353 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/createrepo_c.pc.cmake
--rw-rw-r--   0 root         (0) root         (0)     9307 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/createrepo_shared.c
--rw-rw-r--   0 root         (0) root         (0)     4332 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/createrepo_shared.h
--rw-rw-r--   0 root         (0) root         (0)    27661 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/deltarpms.c
--rw-rw-r--   0 root         (0) root         (0)     3729 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/deltarpms.h.in
--rw-rw-r--   0 root         (0) root         (0)    27993 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/dumper_thread.c
--rw-rw-r--   0 root         (0) root         (0)     6181 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/dumper_thread.h
--rw-rw-r--   0 root         (0) root         (0)     3441 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/error.c
--rw-rw-r--   0 root         (0) root         (0)     3975 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/error.h
--rw-rw-r--   0 root         (0) root         (0)    15382 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/helpers.c
--rw-rw-r--   0 root         (0) root         (0)     2751 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/helpers.h
--rw-rw-r--   0 root         (0) root         (0)    11353 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/koji.c
--rw-rw-r--   0 root         (0) root         (0)     3679 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/koji.h
--rw-rw-r--   0 root         (0) root         (0)    22428 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/load_metadata.c
--rw-rw-r--   0 root         (0) root         (0)     5524 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/load_metadata.h
--rw-rw-r--   0 root         (0) root         (0)    13006 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/locate_metadata.c
--rw-rw-r--   0 root         (0) root         (0)     5817 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/locate_metadata.h
--rw-rw-r--   0 root         (0) root         (0)    86385 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/mergerepo_c.c
--rw-rw-r--   0 root         (0) root         (0)     2555 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/mergerepo_c.h
--rw-rw-r--   0 root         (0) root         (0)     1827 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/metadata_internal.h
--rw-rw-r--   0 root         (0) root         (0)    43763 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/misc.c
--rw-rw-r--   0 root         (0) root         (0)    20340 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/misc.h
--rw-rw-r--   0 root         (0) root         (0)    11612 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/modifyrepo_c.c
--rw-rw-r--   0 root         (0) root         (0)    18830 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/modifyrepo_shared.c
--rw-rw-r--   0 root         (0) root         (0)     2240 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/modifyrepo_shared.h
--rw-rw-r--   0 root         (0) root         (0)     8081 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/package.c
--rw-rw-r--   0 root         (0) root         (0)     7680 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/package.h
--rw-rw-r--   0 root         (0) root         (0)     1303 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/package_internal.h
--rw-rw-r--   0 root         (0) root         (0)    26867 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/parsehdr.c
--rw-rw-r--   0 root         (0) root         (0)     2020 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/parsehdr.h
--rw-rw-r--   0 root         (0) root         (0)     8518 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/parsepkg.c
--rw-rw-r--   0 root         (0) root         (0)     5467 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/parsepkg.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.853486 createrepo_c-0.21.1/src/python/
--rw-rw-r--   0 root         (0) root         (0)     2730 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)     1473 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/checksum-py.c
--rw-rw-r--   0 root         (0) root         (0)     1298 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/checksum-py.h
--rw-rw-r--   0 root         (0) root         (0)     6450 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/compression_wrapper-py.c
--rw-rw-r--   0 root         (0) root         (0)     1622 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/compression_wrapper-py.h
--rw-rw-r--   0 root         (0) root         (0)     6696 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/contentstat-py.c
--rw-rw-r--   0 root         (0) root         (0)     1104 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/contentstat-py.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.853486 createrepo_c-0.21.1/src/python/createrepo_c/
--rw-rw-r--   0 root         (0) root         (0)    14523 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/createrepo_c/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.857486 createrepo_c-0.21.1/src/python/createrepo_c.egg-info/
--rw-r--r--   0 root         (0) root         (0)      812 2023-04-04 10:37:51.000000 createrepo_c-0.21.1/src/python/createrepo_c.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20454 2023-04-04 10:37:51.000000 createrepo_c-0.21.1/src/python/createrepo_c.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 10:37:51.000000 createrepo_c-0.21.1/src/python/createrepo_c.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-04-04 10:37:51.000000 createrepo_c-0.21.1/src/python/createrepo_c.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-04 10:37:51.000000 createrepo_c-0.21.1/src/python/createrepo_c.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)    12022 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/createrepo_cmodule.c
--rw-rw-r--   0 root         (0) root         (0)     2517 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/exception-py.c
--rw-rw-r--   0 root         (0) root         (0)     1307 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/exception-py.h
--rw-rw-r--   0 root         (0) root         (0)    10077 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/load_metadata-py.c
--rw-rw-r--   0 root         (0) root         (0)     1043 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/load_metadata-py.h
--rw-rw-r--   0 root         (0) root         (0)     7280 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/locate_metadata-py.c
--rw-rw-r--   0 root         (0) root         (0)     1143 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/locate_metadata-py.h
--rw-rw-r--   0 root         (0) root         (0)     2573 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/misc-py.c
--rw-rw-r--   0 root         (0) root         (0)     1495 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/misc-py.h
--rw-rw-r--   0 root         (0) root         (0)    19845 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/package-py.c
--rw-rw-r--   0 root         (0) root         (0)     1242 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/package-py.h
--rw-rw-r--   0 root         (0) root         (0)     4047 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/parsepkg-py.c
--rw-rw-r--   0 root         (0) root         (0)     1444 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/parsepkg-py.h
--rw-rw-r--   0 root         (0) root         (0)    13961 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/repomd-py.c
--rw-rw-r--   0 root         (0) root         (0)     1069 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/repomd-py.h
--rw-rw-r--   0 root         (0) root         (0)    13661 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/repomdrecord-py.c
--rw-rw-r--   0 root         (0) root         (0)     1168 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/repomdrecord-py.h
--rw-rw-r--   0 root         (0) root         (0)     5675 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/sqlite-py.c
--rw-rw-r--   0 root         (0) root         (0)     1023 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/sqlite-py.h
--rw-rw-r--   0 root         (0) root         (0)     7571 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/typeconversion.c
--rw-rw-r--   0 root         (0) root         (0)     1849 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/typeconversion.h
--rw-rw-r--   0 root         (0) root         (0)    10308 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/updatecollection-py.c
--rw-rw-r--   0 root         (0) root         (0)     1216 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/updatecollection-py.h
--rw-rw-r--   0 root         (0) root         (0)     7595 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/updatecollectionmodule-py.c
--rw-rw-r--   0 root         (0) root         (0)     1270 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/updatecollectionmodule-py.h
--rw-rw-r--   0 root         (0) root         (0)     8365 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/updatecollectionpackage-py.c
--rw-rw-r--   0 root         (0) root         (0)     1279 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/updatecollectionpackage-py.h
--rw-rw-r--   0 root         (0) root         (0)     7867 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/updateinfo-py.c
--rw-rw-r--   0 root         (0) root         (0)     1097 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/updateinfo-py.h
--rw-rw-r--   0 root         (0) root         (0)    15281 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/updaterecord-py.c
--rw-rw-r--   0 root         (0) root         (0)     1168 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/updaterecord-py.h
--rw-rw-r--   0 root         (0) root         (0)     6257 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/updatereference-py.c
--rw-rw-r--   0 root         (0) root         (0)     1195 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/updatereference-py.h
--rw-rw-r--   0 root         (0) root         (0)     4938 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/xml_dump-py.c
--rw-rw-r--   0 root         (0) root         (0)     2121 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/xml_dump-py.h
--rw-rw-r--   0 root         (0) root         (0)     7503 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/xml_file-py.c
--rw-rw-r--   0 root         (0) root         (0)     1030 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/xml_file-py.h
--rw-rw-r--   0 root         (0) root         (0)    27454 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/xml_parser-py.c
--rw-rw-r--   0 root         (0) root         (0)     3318 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/python/xml_parser-py.h
--rw-rw-r--   0 root         (0) root         (0)    36323 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/repomd.c
--rw-rw-r--   0 root         (0) root         (0)    11634 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/repomd.h
--rw-rw-r--   0 root         (0) root         (0)     1359 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/repomd_internal.h
--rw-rw-r--   0 root         (0) root         (0)    48112 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/sqlite.c
--rw-rw-r--   0 root         (0) root         (0)     5768 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/sqlite.h
--rw-rw-r--   0 root         (0) root         (0)    34362 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/sqliterepo_c.c
--rw-rw-r--   0 root         (0) root         (0)     5190 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/threads.c
--rw-rw-r--   0 root         (0) root         (0)     5854 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/threads.h
--rw-rw-r--   0 root         (0) root         (0)     9476 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/updateinfo.c
--rw-rw-r--   0 root         (0) root         (0)     5407 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/updateinfo.h
--rw-rw-r--   0 root         (0) root         (0)     1312 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/version.h.in
--rw-rw-r--   0 root         (0) root         (0)    10941 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_dump.c
--rw-rw-r--   0 root         (0) root         (0)     7158 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_dump.h
--rw-rw-r--   0 root         (0) root         (0)     4453 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_dump_deltapackage.c
--rw-rw-r--   0 root         (0) root         (0)     3830 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_dump_filelists.c
--rw-rw-r--   0 root         (0) root         (0)     3198 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_dump_internal.h
--rw-rw-r--   0 root         (0) root         (0)     4333 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_dump_other.c
--rw-rw-r--   0 root         (0) root         (0)    12584 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_dump_primary.c
--rw-rw-r--   0 root         (0) root         (0)     8647 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_dump_repomd.c
--rw-rw-r--   0 root         (0) root         (0)     9345 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_dump_updateinfo.c
--rw-rw-r--   0 root         (0) root         (0)    15876 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_file.c
--rw-rw-r--   0 root         (0) root         (0)    10285 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_file.h
--rw-rw-r--   0 root         (0) root         (0)     9169 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_parser.c
--rw-rw-r--   0 root         (0) root         (0)    13838 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_parser.h
--rw-rw-r--   0 root         (0) root         (0)    14997 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_parser_filelists.c
--rw-rw-r--   0 root         (0) root         (0)     9269 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_parser_internal.h
--rw-rw-r--   0 root         (0) root         (0)    17381 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_parser_main_metadata_together.c
--rw-rw-r--   0 root         (0) root         (0)    13200 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_parser_other.c
--rw-rw-r--   0 root         (0) root         (0)    27752 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_parser_primary.c
--rw-rw-r--   0 root         (0) root         (0)    14399 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_parser_repomd.c
--rw-rw-r--   0 root         (0) root         (0)    20016 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/src/xml_parser_updateinfo.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.857486 createrepo_c-0.21.1/tests/
--rw-rw-r--   0 root         (0) root         (0)     2887 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.865486 createrepo_c-0.21.1/tests/createrepo/
--rw-rw-r--   0 root         (0) root         (0)     4658 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)     8242 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/checksum.c
--rw-rw-r--   0 root         (0) root         (0)     3660 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/checksum.h
--rw-rw-r--   0 root         (0) root         (0)     4014 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/cleanup.h
--rw-rw-r--   0 root         (0) root         (0)    29168 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/cmd_parser.c
--rw-rw-r--   0 root         (0) root         (0)     9165 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/cmd_parser.h
--rw-rw-r--   0 root         (0) root         (0)    54854 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/compression_wrapper.c
--rw-rw-r--   0 root         (0) root         (0)     8210 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/compression_wrapper.h
--rw-rw-r--   0 root         (0) root         (0)     1138 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/constants.h
--rw-rw-r--   0 root         (0) root         (0)   107815 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/createrepo_c.c
--rw-rw-r--   0 root         (0) root         (0)     1654 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/createrepo_c.h
--rw-rw-r--   0 root         (0) root         (0)      353 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/createrepo_c.pc.cmake
--rw-rw-r--   0 root         (0) root         (0)     9307 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/createrepo_shared.c
--rw-rw-r--   0 root         (0) root         (0)     4332 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/createrepo_shared.h
--rw-rw-r--   0 root         (0) root         (0)    27661 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/deltarpms.c
--rw-rw-r--   0 root         (0) root         (0)     3729 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/deltarpms.h.in
--rw-rw-r--   0 root         (0) root         (0)    27993 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/dumper_thread.c
--rw-rw-r--   0 root         (0) root         (0)     6181 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/dumper_thread.h
--rw-rw-r--   0 root         (0) root         (0)     3441 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/error.c
--rw-rw-r--   0 root         (0) root         (0)     3975 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/error.h
--rw-rw-r--   0 root         (0) root         (0)    15382 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/helpers.c
--rw-rw-r--   0 root         (0) root         (0)     2751 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/helpers.h
--rw-rw-r--   0 root         (0) root         (0)    11353 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/koji.c
--rw-rw-r--   0 root         (0) root         (0)     3679 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/koji.h
--rw-rw-r--   0 root         (0) root         (0)    22428 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/load_metadata.c
--rw-rw-r--   0 root         (0) root         (0)     5524 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/load_metadata.h
--rw-rw-r--   0 root         (0) root         (0)    13006 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/locate_metadata.c
--rw-rw-r--   0 root         (0) root         (0)     5817 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/locate_metadata.h
--rw-rw-r--   0 root         (0) root         (0)    86385 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/mergerepo_c.c
--rw-rw-r--   0 root         (0) root         (0)     2555 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/mergerepo_c.h
--rw-rw-r--   0 root         (0) root         (0)     1827 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/metadata_internal.h
--rw-rw-r--   0 root         (0) root         (0)    43763 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/misc.c
--rw-rw-r--   0 root         (0) root         (0)    20340 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/misc.h
--rw-rw-r--   0 root         (0) root         (0)    11612 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/modifyrepo_c.c
--rw-rw-r--   0 root         (0) root         (0)    18830 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/modifyrepo_shared.c
--rw-rw-r--   0 root         (0) root         (0)     2240 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/modifyrepo_shared.h
--rw-rw-r--   0 root         (0) root         (0)     8081 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/package.c
--rw-rw-r--   0 root         (0) root         (0)     7680 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/package.h
--rw-rw-r--   0 root         (0) root         (0)     1303 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/package_internal.h
--rw-rw-r--   0 root         (0) root         (0)    26867 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/parsehdr.c
--rw-rw-r--   0 root         (0) root         (0)     2020 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/parsehdr.h
--rw-rw-r--   0 root         (0) root         (0)     8518 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/parsepkg.c
--rw-rw-r--   0 root         (0) root         (0)     5467 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/parsepkg.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.869486 createrepo_c-0.21.1/tests/createrepo/python/
--rw-rw-r--   0 root         (0) root         (0)     2730 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)     1473 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/checksum-py.c
--rw-rw-r--   0 root         (0) root         (0)     1298 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/checksum-py.h
--rw-rw-r--   0 root         (0) root         (0)     6450 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/compression_wrapper-py.c
--rw-rw-r--   0 root         (0) root         (0)     1622 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/compression_wrapper-py.h
--rw-rw-r--   0 root         (0) root         (0)     6696 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/contentstat-py.c
--rw-rw-r--   0 root         (0) root         (0)     1104 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/contentstat-py.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.869486 createrepo_c-0.21.1/tests/createrepo/python/createrepo_c/
--rw-rw-r--   0 root         (0) root         (0)    14523 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/createrepo_c/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.869486 createrepo_c-0.21.1/tests/createrepo/python/createrepo_c.egg-info/
--rw-r--r--   0 root         (0) root         (0)      812 2023-04-04 10:37:51.000000 createrepo_c-0.21.1/tests/createrepo/python/createrepo_c.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20454 2023-04-04 10:37:51.000000 createrepo_c-0.21.1/tests/createrepo/python/createrepo_c.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 10:37:51.000000 createrepo_c-0.21.1/tests/createrepo/python/createrepo_c.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-04-04 10:37:51.000000 createrepo_c-0.21.1/tests/createrepo/python/createrepo_c.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-04 10:37:51.000000 createrepo_c-0.21.1/tests/createrepo/python/createrepo_c.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)    12022 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/createrepo_cmodule.c
--rw-rw-r--   0 root         (0) root         (0)     2517 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/exception-py.c
--rw-rw-r--   0 root         (0) root         (0)     1307 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/exception-py.h
--rw-rw-r--   0 root         (0) root         (0)    10077 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/load_metadata-py.c
--rw-rw-r--   0 root         (0) root         (0)     1043 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/load_metadata-py.h
--rw-rw-r--   0 root         (0) root         (0)     7280 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/locate_metadata-py.c
--rw-rw-r--   0 root         (0) root         (0)     1143 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/locate_metadata-py.h
--rw-rw-r--   0 root         (0) root         (0)     2573 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/misc-py.c
--rw-rw-r--   0 root         (0) root         (0)     1495 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/misc-py.h
--rw-rw-r--   0 root         (0) root         (0)    19845 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/package-py.c
--rw-rw-r--   0 root         (0) root         (0)     1242 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/package-py.h
--rw-rw-r--   0 root         (0) root         (0)     4047 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/parsepkg-py.c
--rw-rw-r--   0 root         (0) root         (0)     1444 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/parsepkg-py.h
--rw-rw-r--   0 root         (0) root         (0)    13961 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/repomd-py.c
--rw-rw-r--   0 root         (0) root         (0)     1069 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/repomd-py.h
--rw-rw-r--   0 root         (0) root         (0)    13661 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/repomdrecord-py.c
--rw-rw-r--   0 root         (0) root         (0)     1168 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/repomdrecord-py.h
--rw-rw-r--   0 root         (0) root         (0)     5675 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/sqlite-py.c
--rw-rw-r--   0 root         (0) root         (0)     1023 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/sqlite-py.h
--rw-rw-r--   0 root         (0) root         (0)     7571 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/typeconversion.c
--rw-rw-r--   0 root         (0) root         (0)     1849 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/typeconversion.h
--rw-rw-r--   0 root         (0) root         (0)    10308 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/updatecollection-py.c
--rw-rw-r--   0 root         (0) root         (0)     1216 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/updatecollection-py.h
--rw-rw-r--   0 root         (0) root         (0)     7595 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/updatecollectionmodule-py.c
--rw-rw-r--   0 root         (0) root         (0)     1270 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/updatecollectionmodule-py.h
--rw-rw-r--   0 root         (0) root         (0)     8365 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/updatecollectionpackage-py.c
--rw-rw-r--   0 root         (0) root         (0)     1279 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/updatecollectionpackage-py.h
--rw-rw-r--   0 root         (0) root         (0)     7867 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/updateinfo-py.c
--rw-rw-r--   0 root         (0) root         (0)     1097 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/updateinfo-py.h
--rw-rw-r--   0 root         (0) root         (0)    15281 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/updaterecord-py.c
--rw-rw-r--   0 root         (0) root         (0)     1168 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/updaterecord-py.h
--rw-rw-r--   0 root         (0) root         (0)     6257 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/updatereference-py.c
--rw-rw-r--   0 root         (0) root         (0)     1195 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/updatereference-py.h
--rw-rw-r--   0 root         (0) root         (0)     4938 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/xml_dump-py.c
--rw-rw-r--   0 root         (0) root         (0)     2121 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/xml_dump-py.h
--rw-rw-r--   0 root         (0) root         (0)     7503 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/xml_file-py.c
--rw-rw-r--   0 root         (0) root         (0)     1030 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/xml_file-py.h
--rw-rw-r--   0 root         (0) root         (0)    27454 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/xml_parser-py.c
--rw-rw-r--   0 root         (0) root         (0)     3318 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/python/xml_parser-py.h
--rw-rw-r--   0 root         (0) root         (0)    36323 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/repomd.c
--rw-rw-r--   0 root         (0) root         (0)    11634 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/repomd.h
--rw-rw-r--   0 root         (0) root         (0)     1359 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/repomd_internal.h
--rw-rw-r--   0 root         (0) root         (0)    48112 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/sqlite.c
--rw-rw-r--   0 root         (0) root         (0)     5768 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/sqlite.h
--rw-rw-r--   0 root         (0) root         (0)    34362 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/sqliterepo_c.c
--rw-rw-r--   0 root         (0) root         (0)     5190 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/threads.c
--rw-rw-r--   0 root         (0) root         (0)     5854 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/threads.h
--rw-rw-r--   0 root         (0) root         (0)     9476 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/updateinfo.c
--rw-rw-r--   0 root         (0) root         (0)     5407 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/updateinfo.h
--rw-rw-r--   0 root         (0) root         (0)     1312 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/version.h.in
--rw-rw-r--   0 root         (0) root         (0)    10941 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_dump.c
--rw-rw-r--   0 root         (0) root         (0)     7158 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_dump.h
--rw-rw-r--   0 root         (0) root         (0)     4453 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_dump_deltapackage.c
--rw-rw-r--   0 root         (0) root         (0)     3830 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_dump_filelists.c
--rw-rw-r--   0 root         (0) root         (0)     3198 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_dump_internal.h
--rw-rw-r--   0 root         (0) root         (0)     4333 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_dump_other.c
--rw-rw-r--   0 root         (0) root         (0)    12584 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_dump_primary.c
--rw-rw-r--   0 root         (0) root         (0)     8647 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_dump_repomd.c
--rw-rw-r--   0 root         (0) root         (0)     9345 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_dump_updateinfo.c
--rw-rw-r--   0 root         (0) root         (0)    15876 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_file.c
--rw-rw-r--   0 root         (0) root         (0)    10285 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_file.h
--rw-rw-r--   0 root         (0) root         (0)     9169 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_parser.c
--rw-rw-r--   0 root         (0) root         (0)    13838 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_parser.h
--rw-rw-r--   0 root         (0) root         (0)    14997 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_parser_filelists.c
--rw-rw-r--   0 root         (0) root         (0)     9269 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_parser_internal.h
--rw-rw-r--   0 root         (0) root         (0)    17381 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_parser_main_metadata_together.c
--rw-rw-r--   0 root         (0) root         (0)    13200 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_parser_other.c
--rw-rw-r--   0 root         (0) root         (0)    27752 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_parser_primary.c
--rw-rw-r--   0 root         (0) root         (0)    14399 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_parser_repomd.c
--rw-rw-r--   0 root         (0) root         (0)    20016 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/createrepo/xml_parser_updateinfo.c
--rw-rw-r--   0 root         (0) root         (0)    11645 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/fixtures.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.869486 createrepo_c-0.21.1/tests/python/
--rw-rw-r--   0 root         (0) root         (0)       25 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.873486 createrepo_c-0.21.1/tests/python/tests/
--rw-rw-r--   0 root         (0) root         (0)      167 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/CMakeLists.txt
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7555 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/fixtures.py
--rwxrwxr-x   0 root         (0) root         (0)      199 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/run_unittests.sh.in
--rw-rw-r--   0 root         (0) root         (0)     1212 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_checksum.py
--rw-rw-r--   0 root         (0) root         (0)     3242 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_compression_wrapper.py
--rw-rw-r--   0 root         (0) root         (0)     2514 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_contentstat.py
--rw-rw-r--   0 root         (0) root         (0)     4166 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_crfile.py
--rw-rw-r--   0 root         (0) root         (0)     3414 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_load_metadata.py
--rw-rw-r--   0 root         (0) root         (0)     4235 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_locate_metadata.py
--rw-rw-r--   0 root         (0) root         (0)     3249 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_misc.py
--rw-rw-r--   0 root         (0) root         (0)    10847 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_package.py
--rw-rw-r--   0 root         (0) root         (0)     2435 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_parsepkg.py
--rw-rw-r--   0 root         (0) root         (0)     4875 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_repomd.py
--rw-rw-r--   0 root         (0) root         (0)     7982 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_repomdrecord.py
--rw-rw-r--   0 root         (0) root         (0)    10544 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_sqlite.py
--rw-rw-r--   0 root         (0) root         (0)     3063 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_updatecollection.py
--rw-rw-r--   0 root         (0) root         (0)      938 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_updatecollectionmodule.py
--rw-rw-r--   0 root         (0) root         (0)     1760 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_updatecollectionpackage.py
--rw-rw-r--   0 root         (0) root         (0)    13055 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_updateinfo.py
--rw-rw-r--   0 root         (0) root         (0)     6315 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_updaterecord.py
--rw-rw-r--   0 root         (0) root         (0)      710 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_updatereference.py
--rw-rw-r--   0 root         (0) root         (0)      317 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_version.py
--rw-rw-r--   0 root         (0) root         (0)    14610 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_xml_file.py
--rw-rw-r--   0 root         (0) root         (0)    56795 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/python/tests/test_xml_parser.py
--rwxrwxr-x   0 root         (0) root         (0)      688 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/run_tests.sh.in
--rw-rw-r--   0 root         (0) root         (0)     5518 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/test_checksum.c
--rw-rw-r--   0 root         (0) root         (0)    26799 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/test_compression_wrapper.c
--rw-rw-r--   0 root         (0) root         (0)    14197 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/test_koji.c
--rw-rw-r--   0 root         (0) root         (0)     8097 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/test_load_metadata.c
--rw-rw-r--   0 root         (0) root         (0)    10143 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/test_locate_metadata.c
--rw-rw-r--   0 root         (0) root         (0)    43237 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/test_misc.c
--rw-rw-r--   0 root         (0) root         (0)     4643 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/test_modifyrepo_shared.c
--rw-rw-r--   0 root         (0) root         (0)     6301 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/test_sqlite.c
--rw-rw-r--   0 root         (0) root         (0)     3948 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/test_xml_dump.c
--rw-rw-r--   0 root         (0) root         (0)    15120 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/test_xml_dump_primary.c
--rw-rw-r--   0 root         (0) root         (0)     4565 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/test_xml_file.c
--rw-rw-r--   0 root         (0) root         (0)    16817 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/test_xml_parser_filelists.c
--rw-rw-r--   0 root         (0) root         (0)    11176 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/test_xml_parser_main_metadata_together.c
--rw-rw-r--   0 root         (0) root         (0)     4156 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/test_xml_parser_repomd.c
--rw-rw-r--   0 root         (0) root         (0)    10261 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/test_xml_parser_updateinfo.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.841485 createrepo_c-0.21.1/tests/testdata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.873486 createrepo_c-0.21.1/tests/testdata/compressed_files/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/00_plain.foo0
--rw-rw-r--   0 root         (0) root         (0)       33 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/00_plain.foo1
--rw-rw-r--   0 root         (0) root         (0)       14 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/00_plain.foo2
--rw-rw-r--   0 root         (0) root         (0)       32 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/00_plain.foo3
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/00_plain.foo4
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/00_plain.txt
--rw-rw-r--   0 root         (0) root         (0)       14 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/00_plain.txt.bz2
--rw-rw-r--   0 root         (0) root         (0)       33 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/00_plain.txt.gz
--rw-rw-r--   0 root         (0) root         (0)       32 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/00_plain.txt.xz
--rw-rw-r--   0 root         (0) root         (0)       95 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/00_plain.txt.zck
--rw-rw-r--   0 root         (0) root         (0)       56 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/01_plain.foo0
--rw-rw-r--   0 root         (0) root         (0)       64 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/01_plain.foo1
--rw-rw-r--   0 root         (0) root         (0)       69 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/01_plain.foo2
--rw-rw-r--   0 root         (0) root         (0)       96 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/01_plain.foo3
--rw-rw-r--   0 root         (0) root         (0)      169 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/01_plain.foo4
--rw-rw-r--   0 root         (0) root         (0)       56 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/01_plain.txt
--rw-rw-r--   0 root         (0) root         (0)       69 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/01_plain.txt.bz2
--rw-rw-r--   0 root         (0) root         (0)       64 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/01_plain.txt.gz
--rw-rw-r--   0 root         (0) root         (0)       96 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/01_plain.txt.xz
--rw-rw-r--   0 root         (0) root         (0)      158 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/compressed_files/01_plain.txt.zck
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.873486 createrepo_c-0.21.1/tests/testdata/comps_files/
--rw-rw-r--   0 root         (0) root         (0)      638 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/comps_files/comps_00.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.877487 createrepo_c-0.21.1/tests/testdata/modified_repo_files/
--rw-rw-r--   0 root         (0) root         (0)      633 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/bad_file_type-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      570 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/error_00-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      802 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/error_00-other.xml
--rw-rw-r--   0 root         (0) root         (0)     3174 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/error_00-primary.xml
--rw-rw-r--   0 root         (0) root         (0)    68135 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/long_primary.xml
--rw-rw-r--   0 root         (0) root         (0)     1528 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/missing_type-repomd.xml
--rw-rw-r--   0 root         (0) root         (0)      764 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/multiple_warnings_00-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      985 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/multiple_warnings_00-other.xml
--rw-rw-r--   0 root         (0) root         (0)     3588 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/multiple_warnings_00-primary.xml
--rw-rw-r--   0 root         (0) root         (0)      510 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/no_pkgid-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      767 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/no_pkgid-other.xml
--rw-rw-r--   0 root         (0) root         (0)      405 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/repo_01_ampersand-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      551 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/repo_01_ampersand-other.xml
--rw-rw-r--   0 root         (0) root         (0)     2239 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/repo_01_ampersand-primary.xml
--rw-rw-r--   0 root         (0) root         (0)      598 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/repo_02_different_order_filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      608 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_00-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      840 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_00-other.xml
--rw-rw-r--   0 root         (0) root         (0)     3277 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_00-primary.xml
--rw-rw-r--   0 root         (0) root         (0)      606 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_01-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      838 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_01-other.xml
--rw-rw-r--   0 root         (0) root         (0)     3353 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_01-primary.xml
--rw-rw-r--   0 root         (0) root         (0)      657 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_02-filelists.xml
--rw-rw-r--   0 root         (0) root         (0)      889 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_02-other.xml
--rw-rw-r--   0 root         (0) root         (0)     3342 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_02-primary.xml
--rw-rw-r--   0 root         (0) root         (0)     1277 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/modified_repo_files/updateinfo_ampersand.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.877487 createrepo_c-0.21.1/tests/testdata/other_metadata/
--rw-rw-r--   0 root         (0) root         (0)      894 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/other_metadata/0402e012013246e7e2f2f638c8a6046efdfd71ae1cbeff9c391d9c1ae5d7d431-comps-f19.xml.bz2
--rw-rw-r--   0 root         (0) root         (0)     2364 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/other_metadata/36c4f2d6dda3b015b4a7da59552c7c76eff99a59979178513cb51341f6eead44-comps-f19.xml
--rw-rw-r--   0 root         (0) root         (0)      760 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/other_metadata/71d988ca33b31a18b0d775478d6f59b40583c794ae76393284850ee97bfba4dc-comps-f19.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      804 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/other_metadata/c941e2c77a27cdca324c0e0bc3190e134fddddb36a03fb5517e55d156b955205-comps-f19.xml.xz
--rw-rw-r--   0 root         (0) root         (0)     2364 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/other_metadata/comps-f19.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.877487 createrepo_c-0.21.1/tests/testdata/packages/
--rw-rw-r--   0 root         (0) root         (0)     3101 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/packages/Archer-3.4.5-6.x86_64.rpm
--rw-rw-r--   0 root         (0) root         (0)     3096 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/packages/Rimmer-1.0.2-2.x86_64.rpm
--rw-rw-r--   0 root         (0) root         (0)     1717 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/packages/balicek-iso88591-1.1.1-1.x86_64.rpm
--rw-rw-r--   0 root         (0) root         (0)     1741 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/packages/balicek-iso88592-1.1.1-1.x86_64.rpm
--rw-rw-r--   0 root         (0) root         (0)     1789 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/packages/balicek-utf8-1.1.1-1.x86_64.rpm
--rw-rw-r--   0 root         (0) root         (0)     1488 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/packages/empty-0-0.src.rpm
--rw-rw-r--   0 root         (0) root         (0)     1401 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/packages/empty-0-0.x86_64.rpm
--rw-rw-r--   0 root         (0) root         (0)     2237 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/packages/fake_bash-1.1.1-1.x86_64.rpm
--rw-rw-r--   0 root         (0) root         (0)     2845 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/packages/super_kernel-6.0.1-2.x86_64.rpm
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.841485 createrepo_c-0.21.1/tests/testdata/repo_00/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.877487 createrepo_c-0.21.1/tests/testdata/repo_00/repodata/
--rw-rw-r--   0 root         (0) root         (0)      134 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_00/repodata/1cb61ea996355add02b1426ed4c1780ea75ce0c04c5d1107c025c3fbd7d8bcae-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      262 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_00/repodata/2e7db4492173b6c437fd1299dc335e63d09f24cbdadeac5175a61b787c2f7a44-filelists.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      123 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_00/repodata/95a4415d859d7120efb6b3cf964c07bebbff9a5275ca673e6e74a97bcbfb2a5f-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      263 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_00/repodata/a939c4765106655c3f7a13fb41d0f239824efa66bcd6c1e6c044a854012bda75-other.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      269 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_00/repodata/e0ac03cd77e95e724dbf90ded0dba664e233315a8940051dd8882c56b9878595-primary.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      123 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_00/repodata/ef3e20691954c3d1318ec3071a982da339f4ed76967ded668b795c9e070aaab6-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     3381 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_00/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.841485 createrepo_c-0.21.1/tests/testdata/repo_01/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.877487 createrepo_c-0.21.1/tests/testdata/repo_01/repodata/
--rw-rw-r--   0 root         (0) root         (0)      783 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_01/repodata/6c662d665c24de9a0f62c17d8fa50622307739d7376f0d19097ca96c6d7f5e3e-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      332 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_01/repodata/b752a73d9efd4006d740f943db5fb7c2dd77a8324bd99da92e86bd55a2c126ef-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      273 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_01/repodata/c7db035d0e6f1b2e883a7fa3229e2d2be70c05a8b8d2b57dbb5f9c1a67483b6c-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1497 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_01/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.841485 createrepo_c-0.21.1/tests/testdata/repo_02/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.881487 createrepo_c-0.21.1/tests/testdata/repo_02/repodata/
--rw-rw-r--   0 root         (0) root         (0)      341 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_02/repodata/3b7e6ecd01af9cb674aff6458186911d7081bb5676d5562a21a963afc8a8bcc7-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      403 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_02/repodata/ab5d3edeea50f9b4ec5ee13e4d25c147e318e3a433dbabc94d3461f58ac28255-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      973 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_02/repodata/bcde64b04916a2a72fdc257d61bc922c70b3d58e953499180585f7a360ce86cf-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1497 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_02/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.841485 createrepo_c-0.21.1/tests/testdata/repo_03/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.881487 createrepo_c-0.21.1/tests/testdata/repo_03/repodata/
--rw-rw-r--   0 root         (0) root         (0)      134 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_03/repodata/1cb61ea996355add02b1426ed4c1780ea75ce0c04c5d1107c025c3fbd7d8bcae-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      262 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_03/repodata/2e7db4492173b6c437fd1299dc335e63d09f24cbdadeac5175a61b787c2f7a44-filelists.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      123 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_03/repodata/95a4415d859d7120efb6b3cf964c07bebbff9a5275ca673e6e74a97bcbfb2a5f-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1044 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_03/repodata/a850093e240506c728d6ce26a6fc51d6a7fe10730c67988d13afa7dd82df82d5-modules.yaml.xz
--rw-rw-r--   0 root         (0) root         (0)      263 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_03/repodata/a939c4765106655c3f7a13fb41d0f239824efa66bcd6c1e6c044a854012bda75-other.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      269 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_03/repodata/e0ac03cd77e95e724dbf90ded0dba664e233315a8940051dd8882c56b9878595-primary.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      123 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_03/repodata/ef3e20691954c3d1318ec3071a982da339f4ed76967ded668b795c9e070aaab6-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     3838 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_03/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.841485 createrepo_c-0.21.1/tests/testdata/repo_04/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.881487 createrepo_c-0.21.1/tests/testdata/repo_04/repodata/
--rw-rw-r--   0 root         (0) root         (0)      987 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_04/repodata/6a5f64dd82a126a161657764fe8f4b4092c0a3b61b9a34bde2af89dc1df112a1-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      397 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_04/repodata/6d0101044d9b4683e4ddc76491b3eb2228cddaace9e1d148c5eb138de9f71c17-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      429 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_04/repodata/d1c632d489f1c72b68b5c0d5de38ed1cb5c7a521380a88bed86771d39fb19538-filelists-ext.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      336 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_04/repodata/d7b8b1b6caa124aa17e4c6a1867e50e6893791ade0ebe212ab6f536695b5ce84-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     2012 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_04/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.841485 createrepo_c-0.21.1/tests/testdata/repo_koji_01/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.881487 createrepo_c-0.21.1/tests/testdata/repo_koji_01/repodata/
--rw-rw-r--   0 root         (0) root         (0)      816 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_koji_01/repodata/5d039d9ec332d158c69d083f04ac88a187c6b68444472b802eaf0249aec83294-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1007 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_koji_01/repodata/b153f86915d1dacbb89b244da26e50adb204195262fd3562290de26725daa21d-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      487 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_koji_01/repodata/c0e88e9a81f76341e91cd06f8ded80d4c289bdb4977e7624068802654b6da506-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1549 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_koji_01/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.841485 createrepo_c-0.21.1/tests/testdata/repo_koji_02/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.881487 createrepo_c-0.21.1/tests/testdata/repo_koji_02/repodata/
--rw-rw-r--   0 root         (0) root         (0)      338 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_koji_02/repodata/118e790330a62cfb167ce670478b25f4bfc58d7fc671096e4fd294fe40cee201-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      913 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_koji_02/repodata/ee9261d1d2916d841cf24bb01743198ec63ed596f410784602eca2350e430e17-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      687 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_koji_02/repodata/feb0b5fdcb0ee1cf981b041f0749ec381145cd9f6b4397991ef5dafcb6807bba-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1547 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_koji_02/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.841485 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.885487 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/
--rw-rw-r--   0 root         (0) root         (0)      656 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/0219a2f1f9f32af6b7873905269ac1bc27b03e0caf3968c929a49e5a939e8935-updateinfo_01.xml.gz.zck
--rw-rw-r--   0 root         (0) root         (0)     2366 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/04460bfaf6cb5af6b0925d8c99401a44e5192d287796aed4cced5f7ce881761f-comps.f20.xml
--rw-rw-r--   0 root         (0) root         (0)     3775 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/1e12239bf5cb07ec73c74482c35e80dabe30dbe2fdd57bd9e557d987cbacc8c2-primary.sqlite.bz2
--rw-rw-r--   0 root         (0) root         (0)      864 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.gz.zck
--rw-rw-r--   0 root         (0) root         (0)      864 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      932 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/3d6eaa7c77ef92586470dd6a542478e42cc421a85f12e0db93aa783077704cd0-filelists.xml.zck
--rw-rw-r--   0 root         (0) root         (0)     1287 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/490a2a494a3827b8a356f728ac36bc02fb009b0eaea173c890e727bb54219037-primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1519 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/4f4de7d3254a033b84626f330bc6adb8a3c1a4a20f0ddbe30a5692a041318c81-filelists.sqlite.bz2
--rw-rw-r--   0 root         (0) root         (0)    88281 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/4fbad65c641f4f8fb3cec9b1672fcec2357443e1ea6e93541a0bb559c7dc9238-modules.yaml.gz
--rw-rw-r--   0 root         (0) root         (0)      533 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/88514679cb03d8f51e850ad3639c089f899e83407a2380ef9e62873a8eb1db13-updateinfo_01.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1301 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/8b13cba732c1a02b841f43d6791ca68788d45f376787d9f3ccf68e75f01af499-other.sqlite.bz2
--rw-rw-r--   0 root         (0) root         (0)      749 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/ba5a4fdbb20e7b9b70d9a9abd974bcab1065b1e81d711f80e06ad8cae30c4183-filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      850 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/c5582e660ed9a2d3c10ba44f0aeb02f2bb70e85dc3c8cda4266183d4e5235aa7-other.xml.zck
--rw-rw-r--   0 root         (0) root         (0)    86680 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/cb0f4b5df8268f248158e50d66ee1565591bca23ee2dbd84ae9c457962fa3122-modules.yaml.gz.zck
--rw-rw-r--   0 root         (0) root         (0)     1482 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/e9e6ca4765de75cc3b2bf05e6cf631703c6557edd642300748d7747000547365-primary.xml.zck
--rw-rw-r--   0 root         (0) root         (0)      748 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/f9d860ddcb64fbdc88a9b71a14ddb9f5670968d5dd3430412565c13d42b6804d-comps.f20.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      687 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/fd458a424a3f3e0dadc95b806674b79055c24e73637e47ad5a6e57926aa1b9d1-other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     8640 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.841485 createrepo_c-0.21.1/tests/testdata/repo_with_duplicate_packages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.885487 createrepo_c-0.21.1/tests/testdata/repo_with_duplicate_packages/repodata/
--rw-rw-r--   0 root         (0) root         (0)      341 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_duplicate_packages/repodata/filelists.xml.gz
--rw-rw-r--   0 root         (0) root         (0)      405 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_duplicate_packages/repodata/other.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1017 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_duplicate_packages/repodata/primary.xml.gz
--rw-rw-r--   0 root         (0) root         (0)     1354 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repo_with_duplicate_packages/repodata/repomd.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.885487 createrepo_c-0.21.1/tests/testdata/repodata_snippets/
--rw-rw-r--   0 root         (0) root         (0)      436 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repodata_snippets/filelists_ext_snippet_01.xml
--rw-rw-r--   0 root         (0) root         (0)      745 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repodata_snippets/filelists_ext_snippet_02.xml
--rw-rw-r--   0 root         (0) root         (0)      263 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repodata_snippets/filelists_snippet_01.xml
--rw-rw-r--   0 root         (0) root         (0)      471 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repodata_snippets/filelists_snippet_02.xml
--rw-rw-r--   0 root         (0) root         (0)      408 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repodata_snippets/other_snippet_01.xml
--rw-rw-r--   0 root         (0) root         (0)      697 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repodata_snippets/other_snippet_02.xml
--rw-rw-r--   0 root         (0) root         (0)     1918 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repodata_snippets/primary_snippet_01.xml
--rw-rw-r--   0 root         (0) root         (0)     3085 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/repodata_snippets/primary_snippet_02.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.885487 createrepo_c-0.21.1/tests/testdata/specs/
--rwxrwxr-x   0 root         (0) root         (0)       67 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/specs/build.sh
--rw-rw-r--   0 root         (0) root         (0)     1369 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/specs/fake-Archer.spec
--rw-rw-r--   0 root         (0) root         (0)     1023 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/specs/fake-Rimmer.spec
--rw-rw-r--   0 root         (0) root         (0)      571 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/specs/fake-balicek-iso88591.spec
--rw-rw-r--   0 root         (0) root         (0)      594 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/specs/fake-balicek-iso88592.spec
--rw-rw-r--   0 root         (0) root         (0)      653 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/specs/fake-balicek-utf8.spec
--rw-rw-r--   0 root         (0) root         (0)      176 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/specs/fake-empty.spec
--rw-rw-r--   0 root         (0) root         (0)      632 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/specs/fake-fake_bash.spec
--rw-rw-r--   0 root         (0) root         (0)     1236 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/specs/fake-super_kernel.spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.885487 createrepo_c-0.21.1/tests/testdata/test_files/
--rw-rw-r--   0 root         (0) root         (0)     1523 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/test_files/binary_file
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/test_files/empty_file
--rw-rw-r--   0 root         (0) root         (0)    24576 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/test_files/sqlite_file.sqlite
--rw-rw-r--   0 root         (0) root         (0)      910 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/test_files/text_file
--rw-rw-r--   0 root         (0) root         (0)      522 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/test_files/text_file.gz
--rw-rw-r--   0 root         (0) root         (0)      628 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/test_files/text_file.xz
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:37:51.885487 createrepo_c-0.21.1/tests/testdata/updateinfo_files/
--rw-rw-r--   0 root         (0) root         (0)       60 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/updateinfo_files/updateinfo_00.xml
--rw-rw-r--   0 root         (0) root         (0)     1222 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/updateinfo_files/updateinfo_01.xml
--rw-rw-r--   0 root         (0) root         (0)      188 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/updateinfo_files/updateinfo_02.xml.xz
--rw-rw-r--   0 root         (0) root         (0)     4805 2023-04-04 10:30:43.000000 createrepo_c-0.21.1/tests/testdata/updateinfo_files/updateinfo_03.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.747371 createrepo_c-1.0.0/
+-rw-rw-r--   0 root         (0) root         (0)      499 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/AUTHORS
+-rw-rw-r--   0 root         (0) root         (0)     6088 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)    18092 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/COPYING
+-rw-rw-r--   0 root         (0) root         (0)      198 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      811 2023-07-31 05:41:20.747371 createrepo_c-1.0.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    11505 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/README.md
+-rw-rw-r--   0 root         (0) root         (0)       54 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/VERSION.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.675370 createrepo_c-1.0.0/doc/
+-rw-rw-r--   0 root         (0) root         (0)      637 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/doc/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)   114986 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/doc/Doxyfile.in.in
+-rw-rw-r--   0 root         (0) root         (0)     8781 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/doc/createrepo_c.8
+-rw-rw-r--   0 root         (0) root         (0)     1523 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/doc/logo.png
+-rw-rw-r--   0 root         (0) root         (0)    80453 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/doc/logo.xcf
+-rw-rw-r--   0 root         (0) root         (0)     3476 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/doc/mergerepo_c.8
+-rw-rw-r--   0 root         (0) root         (0)     2164 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/doc/modifyrepo_c.8
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.679370 createrepo_c-1.0.0/doc/python/
+-rw-rw-r--   0 root         (0) root         (0)      255 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/doc/python/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     8128 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/doc/python/conf.py
+-rw-rw-r--   0 root         (0) root         (0)      307 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/doc/python/index.rst
+-rw-rw-r--   0 root         (0) root         (0)      550 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/doc/python/lib.rst
+-rw-rw-r--   0 root         (0) root         (0)     1772 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/doc/sqliterepo_c.8
+-rw-rw-r--   0 root         (0) root         (0)      140 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       30 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 05:41:20.747371 createrepo_c-1.0.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2000 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.687370 createrepo_c-1.0.0/src/
+-rw-rw-r--   0 root         (0) root         (0)     4715 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     8242 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/checksum.c
+-rw-rw-r--   0 root         (0) root         (0)     3660 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/checksum.h
+-rw-rw-r--   0 root         (0) root         (0)     4014 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/cleanup.h
+-rw-rw-r--   0 root         (0) root         (0)    29451 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/cmd_parser.c
+-rw-rw-r--   0 root         (0) root         (0)     9165 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/cmd_parser.h
+-rw-rw-r--   0 root         (0) root         (0)    61983 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/compression_wrapper.c
+-rw-rw-r--   0 root         (0) root         (0)     8273 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/compression_wrapper.h
+-rw-rw-r--   0 root         (0) root         (0)     1138 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/constants.h
+-rw-rw-r--   0 root         (0) root         (0)   104217 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/createrepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)     1654 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/createrepo_c.h
+-rw-rw-r--   0 root         (0) root         (0)      353 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/createrepo_c.pc.cmake
+-rw-rw-r--   0 root         (0) root         (0)     9307 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/createrepo_shared.c
+-rw-rw-r--   0 root         (0) root         (0)     4331 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/createrepo_shared.h
+-rw-rw-r--   0 root         (0) root         (0)    27661 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/deltarpms.c
+-rw-rw-r--   0 root         (0) root         (0)     3729 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/deltarpms.h.in
+-rw-rw-r--   0 root         (0) root         (0)    28066 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/dumper_thread.c
+-rw-rw-r--   0 root         (0) root         (0)     6181 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/dumper_thread.h
+-rw-rw-r--   0 root         (0) root         (0)     3441 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/error.c
+-rw-rw-r--   0 root         (0) root         (0)     4036 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/error.h
+-rw-rw-r--   0 root         (0) root         (0)    15382 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/helpers.c
+-rw-rw-r--   0 root         (0) root         (0)     2751 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/helpers.h
+-rw-rw-r--   0 root         (0) root         (0)    11353 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/koji.c
+-rw-rw-r--   0 root         (0) root         (0)     3679 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/koji.h
+-rw-rw-r--   0 root         (0) root         (0)    23784 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/load_metadata.c
+-rw-rw-r--   0 root         (0) root         (0)     5524 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/load_metadata.h
+-rw-rw-r--   0 root         (0) root         (0)    13005 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/locate_metadata.c
+-rw-rw-r--   0 root         (0) root         (0)     5817 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/locate_metadata.h
+-rw-rw-r--   0 root         (0) root         (0)    85235 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/mergerepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)     2547 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/mergerepo_c.h
+-rw-rw-r--   0 root         (0) root         (0)     2356 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/metadata_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    45017 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/misc.c
+-rw-rw-r--   0 root         (0) root         (0)    20339 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/misc.h
+-rw-rw-r--   0 root         (0) root         (0)    11611 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/modifyrepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)    18830 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/modifyrepo_shared.c
+-rw-rw-r--   0 root         (0) root         (0)     2240 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/modifyrepo_shared.h
+-rw-rw-r--   0 root         (0) root         (0)     8081 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/package.c
+-rw-rw-r--   0 root         (0) root         (0)     7680 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/package.h
+-rw-rw-r--   0 root         (0) root         (0)     1303 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/package_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    26867 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/parsehdr.c
+-rw-rw-r--   0 root         (0) root         (0)     2020 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/parsehdr.h
+-rw-rw-r--   0 root         (0) root         (0)     8518 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/parsepkg.c
+-rw-rw-r--   0 root         (0) root         (0)     5467 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/parsepkg.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.695371 createrepo_c-1.0.0/src/python/
+-rw-rw-r--   0 root         (0) root         (0)     2730 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     1473 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/checksum-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1298 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/checksum-py.h
+-rw-rw-r--   0 root         (0) root         (0)     6450 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/compression_wrapper-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1622 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/compression_wrapper-py.h
+-rw-rw-r--   0 root         (0) root         (0)     6696 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/contentstat-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1104 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/contentstat-py.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.695371 createrepo_c-1.0.0/src/python/createrepo_c/
+-rw-rw-r--   0 root         (0) root         (0)    14701 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/createrepo_c/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.699371 createrepo_c-1.0.0/src/python/createrepo_c.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      811 2023-07-31 05:41:20.000000 createrepo_c-1.0.0/src/python/createrepo_c.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20644 2023-07-31 05:41:20.000000 createrepo_c-1.0.0/src/python/createrepo_c.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:41:20.000000 createrepo_c-1.0.0/src/python/createrepo_c.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-07-31 05:41:20.000000 createrepo_c-1.0.0/src/python/createrepo_c.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 05:41:20.000000 createrepo_c-1.0.0/src/python/createrepo_c.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)    12098 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/createrepo_cmodule.c
+-rw-rw-r--   0 root         (0) root         (0)     2517 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/exception-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1307 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/exception-py.h
+-rw-rw-r--   0 root         (0) root         (0)    10077 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/load_metadata-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1043 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/load_metadata-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7280 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/locate_metadata-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1143 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/locate_metadata-py.h
+-rw-rw-r--   0 root         (0) root         (0)     2573 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/misc-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1495 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/misc-py.h
+-rw-rw-r--   0 root         (0) root         (0)    19974 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/package-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1242 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/package-py.h
+-rw-rw-r--   0 root         (0) root         (0)     4047 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/parsepkg-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1444 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/parsepkg-py.h
+-rw-rw-r--   0 root         (0) root         (0)    13961 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/repomd-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1069 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/repomd-py.h
+-rw-rw-r--   0 root         (0) root         (0)    13674 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/repomdrecord-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1168 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/repomdrecord-py.h
+-rw-rw-r--   0 root         (0) root         (0)     5675 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/sqlite-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1023 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/sqlite-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7705 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/typeconversion.c
+-rw-rw-r--   0 root         (0) root         (0)     1849 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/typeconversion.h
+-rw-rw-r--   0 root         (0) root         (0)    10308 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/updatecollection-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1216 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/updatecollection-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7595 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/updatecollectionmodule-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1270 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/updatecollectionmodule-py.h
+-rw-rw-r--   0 root         (0) root         (0)     8365 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/updatecollectionpackage-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1279 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/updatecollectionpackage-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7867 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/updateinfo-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1097 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/updateinfo-py.h
+-rw-rw-r--   0 root         (0) root         (0)    15281 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/updaterecord-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1168 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/updaterecord-py.h
+-rw-rw-r--   0 root         (0) root         (0)     6257 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/updatereference-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1195 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/updatereference-py.h
+-rw-rw-r--   0 root         (0) root         (0)     4938 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/xml_dump-py.c
+-rw-rw-r--   0 root         (0) root         (0)     2121 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/xml_dump-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7503 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/xml_file-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1030 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/xml_file-py.h
+-rw-rw-r--   0 root         (0) root         (0)    27454 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/xml_parser-py.c
+-rw-rw-r--   0 root         (0) root         (0)     3318 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/python/xml_parser-py.h
+-rw-rw-r--   0 root         (0) root         (0)    36316 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/repomd.c
+-rw-rw-r--   0 root         (0) root         (0)    11634 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/repomd.h
+-rw-rw-r--   0 root         (0) root         (0)     1359 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/repomd_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    48112 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/sqlite.c
+-rw-rw-r--   0 root         (0) root         (0)     5768 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/sqlite.h
+-rw-rw-r--   0 root         (0) root         (0)    34362 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/sqliterepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)     5190 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/threads.c
+-rw-rw-r--   0 root         (0) root         (0)     5854 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/threads.h
+-rw-rw-r--   0 root         (0) root         (0)     9476 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/updateinfo.c
+-rw-rw-r--   0 root         (0) root         (0)     5407 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/updateinfo.h
+-rw-rw-r--   0 root         (0) root         (0)     1312 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/version.h.in
+-rw-rw-r--   0 root         (0) root         (0)    10941 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_dump.c
+-rw-rw-r--   0 root         (0) root         (0)     7158 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_dump.h
+-rw-rw-r--   0 root         (0) root         (0)     4453 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_dump_deltapackage.c
+-rw-rw-r--   0 root         (0) root         (0)     3830 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_dump_filelists.c
+-rw-rw-r--   0 root         (0) root         (0)     3198 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_dump_internal.h
+-rw-rw-r--   0 root         (0) root         (0)     4333 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_dump_other.c
+-rw-rw-r--   0 root         (0) root         (0)    12584 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_dump_primary.c
+-rw-rw-r--   0 root         (0) root         (0)     8647 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_dump_repomd.c
+-rw-rw-r--   0 root         (0) root         (0)     9345 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_dump_updateinfo.c
+-rw-rw-r--   0 root         (0) root         (0)    15876 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_file.c
+-rw-rw-r--   0 root         (0) root         (0)    10285 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_file.h
+-rw-rw-r--   0 root         (0) root         (0)     9169 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_parser.c
+-rw-rw-r--   0 root         (0) root         (0)    13838 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_parser.h
+-rw-rw-r--   0 root         (0) root         (0)    14997 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_parser_filelists.c
+-rw-rw-r--   0 root         (0) root         (0)     9269 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_parser_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    17381 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_parser_main_metadata_together.c
+-rw-rw-r--   0 root         (0) root         (0)    13200 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_parser_other.c
+-rw-rw-r--   0 root         (0) root         (0)    27752 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_parser_primary.c
+-rw-rw-r--   0 root         (0) root         (0)    14399 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_parser_repomd.c
+-rw-rw-r--   0 root         (0) root         (0)    20016 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/src/xml_parser_updateinfo.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.699371 createrepo_c-1.0.0/tests/
+-rw-rw-r--   0 root         (0) root         (0)     2887 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.711371 createrepo_c-1.0.0/tests/createrepo/
+-rw-rw-r--   0 root         (0) root         (0)     4715 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     8242 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/checksum.c
+-rw-rw-r--   0 root         (0) root         (0)     3660 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/checksum.h
+-rw-rw-r--   0 root         (0) root         (0)     4014 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/cleanup.h
+-rw-rw-r--   0 root         (0) root         (0)    29451 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/cmd_parser.c
+-rw-rw-r--   0 root         (0) root         (0)     9165 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/cmd_parser.h
+-rw-rw-r--   0 root         (0) root         (0)    61983 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/compression_wrapper.c
+-rw-rw-r--   0 root         (0) root         (0)     8273 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/compression_wrapper.h
+-rw-rw-r--   0 root         (0) root         (0)     1138 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/constants.h
+-rw-rw-r--   0 root         (0) root         (0)   104217 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/createrepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)     1654 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/createrepo_c.h
+-rw-rw-r--   0 root         (0) root         (0)      353 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/createrepo_c.pc.cmake
+-rw-rw-r--   0 root         (0) root         (0)     9307 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/createrepo_shared.c
+-rw-rw-r--   0 root         (0) root         (0)     4331 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/createrepo_shared.h
+-rw-rw-r--   0 root         (0) root         (0)    27661 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/deltarpms.c
+-rw-rw-r--   0 root         (0) root         (0)     3729 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/deltarpms.h.in
+-rw-rw-r--   0 root         (0) root         (0)    28066 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/dumper_thread.c
+-rw-rw-r--   0 root         (0) root         (0)     6181 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/dumper_thread.h
+-rw-rw-r--   0 root         (0) root         (0)     3441 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/error.c
+-rw-rw-r--   0 root         (0) root         (0)     4036 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/error.h
+-rw-rw-r--   0 root         (0) root         (0)    15382 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/helpers.c
+-rw-rw-r--   0 root         (0) root         (0)     2751 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/helpers.h
+-rw-rw-r--   0 root         (0) root         (0)    11353 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/koji.c
+-rw-rw-r--   0 root         (0) root         (0)     3679 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/koji.h
+-rw-rw-r--   0 root         (0) root         (0)    23784 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/load_metadata.c
+-rw-rw-r--   0 root         (0) root         (0)     5524 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/load_metadata.h
+-rw-rw-r--   0 root         (0) root         (0)    13005 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/locate_metadata.c
+-rw-rw-r--   0 root         (0) root         (0)     5817 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/locate_metadata.h
+-rw-rw-r--   0 root         (0) root         (0)    85235 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/mergerepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)     2547 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/mergerepo_c.h
+-rw-rw-r--   0 root         (0) root         (0)     2356 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/metadata_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    45017 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/misc.c
+-rw-rw-r--   0 root         (0) root         (0)    20339 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/misc.h
+-rw-rw-r--   0 root         (0) root         (0)    11611 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/modifyrepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)    18830 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/modifyrepo_shared.c
+-rw-rw-r--   0 root         (0) root         (0)     2240 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/modifyrepo_shared.h
+-rw-rw-r--   0 root         (0) root         (0)     8081 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/package.c
+-rw-rw-r--   0 root         (0) root         (0)     7680 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/package.h
+-rw-rw-r--   0 root         (0) root         (0)     1303 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/package_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    26867 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/parsehdr.c
+-rw-rw-r--   0 root         (0) root         (0)     2020 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/parsehdr.h
+-rw-rw-r--   0 root         (0) root         (0)     8518 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/parsepkg.c
+-rw-rw-r--   0 root         (0) root         (0)     5467 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/parsepkg.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.719371 createrepo_c-1.0.0/tests/createrepo/python/
+-rw-rw-r--   0 root         (0) root         (0)     2730 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)     1473 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/checksum-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1298 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/checksum-py.h
+-rw-rw-r--   0 root         (0) root         (0)     6450 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/compression_wrapper-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1622 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/compression_wrapper-py.h
+-rw-rw-r--   0 root         (0) root         (0)     6696 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/contentstat-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1104 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/contentstat-py.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.719371 createrepo_c-1.0.0/tests/createrepo/python/createrepo_c/
+-rw-rw-r--   0 root         (0) root         (0)    14701 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/createrepo_c/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.719371 createrepo_c-1.0.0/tests/createrepo/python/createrepo_c.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      811 2023-07-31 05:41:20.000000 createrepo_c-1.0.0/tests/createrepo/python/createrepo_c.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20644 2023-07-31 05:41:20.000000 createrepo_c-1.0.0/tests/createrepo/python/createrepo_c.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:41:20.000000 createrepo_c-1.0.0/tests/createrepo/python/createrepo_c.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-07-31 05:41:20.000000 createrepo_c-1.0.0/tests/createrepo/python/createrepo_c.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 05:41:20.000000 createrepo_c-1.0.0/tests/createrepo/python/createrepo_c.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)    12098 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/createrepo_cmodule.c
+-rw-rw-r--   0 root         (0) root         (0)     2517 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/exception-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1307 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/exception-py.h
+-rw-rw-r--   0 root         (0) root         (0)    10077 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/load_metadata-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1043 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/load_metadata-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7280 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/locate_metadata-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1143 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/locate_metadata-py.h
+-rw-rw-r--   0 root         (0) root         (0)     2573 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/misc-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1495 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/misc-py.h
+-rw-rw-r--   0 root         (0) root         (0)    19974 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/package-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1242 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/package-py.h
+-rw-rw-r--   0 root         (0) root         (0)     4047 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/parsepkg-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1444 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/parsepkg-py.h
+-rw-rw-r--   0 root         (0) root         (0)    13961 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/repomd-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1069 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/repomd-py.h
+-rw-rw-r--   0 root         (0) root         (0)    13674 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/repomdrecord-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1168 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/repomdrecord-py.h
+-rw-rw-r--   0 root         (0) root         (0)     5675 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/sqlite-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1023 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/sqlite-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7705 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/typeconversion.c
+-rw-rw-r--   0 root         (0) root         (0)     1849 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/typeconversion.h
+-rw-rw-r--   0 root         (0) root         (0)    10308 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/updatecollection-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1216 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/updatecollection-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7595 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/updatecollectionmodule-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1270 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/updatecollectionmodule-py.h
+-rw-rw-r--   0 root         (0) root         (0)     8365 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/updatecollectionpackage-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1279 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/updatecollectionpackage-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7867 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/updateinfo-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1097 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/updateinfo-py.h
+-rw-rw-r--   0 root         (0) root         (0)    15281 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/updaterecord-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1168 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/updaterecord-py.h
+-rw-rw-r--   0 root         (0) root         (0)     6257 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/updatereference-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1195 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/updatereference-py.h
+-rw-rw-r--   0 root         (0) root         (0)     4938 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/xml_dump-py.c
+-rw-rw-r--   0 root         (0) root         (0)     2121 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/xml_dump-py.h
+-rw-rw-r--   0 root         (0) root         (0)     7503 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/xml_file-py.c
+-rw-rw-r--   0 root         (0) root         (0)     1030 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/xml_file-py.h
+-rw-rw-r--   0 root         (0) root         (0)    27454 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/xml_parser-py.c
+-rw-rw-r--   0 root         (0) root         (0)     3318 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/python/xml_parser-py.h
+-rw-rw-r--   0 root         (0) root         (0)    36316 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/repomd.c
+-rw-rw-r--   0 root         (0) root         (0)    11634 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/repomd.h
+-rw-rw-r--   0 root         (0) root         (0)     1359 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/repomd_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    48112 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/sqlite.c
+-rw-rw-r--   0 root         (0) root         (0)     5768 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/sqlite.h
+-rw-rw-r--   0 root         (0) root         (0)    34362 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/sqliterepo_c.c
+-rw-rw-r--   0 root         (0) root         (0)     5190 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/threads.c
+-rw-rw-r--   0 root         (0) root         (0)     5854 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/threads.h
+-rw-rw-r--   0 root         (0) root         (0)     9476 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/updateinfo.c
+-rw-rw-r--   0 root         (0) root         (0)     5407 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/updateinfo.h
+-rw-rw-r--   0 root         (0) root         (0)     1312 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/version.h.in
+-rw-rw-r--   0 root         (0) root         (0)    10941 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_dump.c
+-rw-rw-r--   0 root         (0) root         (0)     7158 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_dump.h
+-rw-rw-r--   0 root         (0) root         (0)     4453 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_dump_deltapackage.c
+-rw-rw-r--   0 root         (0) root         (0)     3830 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_dump_filelists.c
+-rw-rw-r--   0 root         (0) root         (0)     3198 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_dump_internal.h
+-rw-rw-r--   0 root         (0) root         (0)     4333 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_dump_other.c
+-rw-rw-r--   0 root         (0) root         (0)    12584 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_dump_primary.c
+-rw-rw-r--   0 root         (0) root         (0)     8647 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_dump_repomd.c
+-rw-rw-r--   0 root         (0) root         (0)     9345 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_dump_updateinfo.c
+-rw-rw-r--   0 root         (0) root         (0)    15876 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_file.c
+-rw-rw-r--   0 root         (0) root         (0)    10285 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_file.h
+-rw-rw-r--   0 root         (0) root         (0)     9169 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_parser.c
+-rw-rw-r--   0 root         (0) root         (0)    13838 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_parser.h
+-rw-rw-r--   0 root         (0) root         (0)    14997 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_parser_filelists.c
+-rw-rw-r--   0 root         (0) root         (0)     9269 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_parser_internal.h
+-rw-rw-r--   0 root         (0) root         (0)    17381 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_parser_main_metadata_together.c
+-rw-rw-r--   0 root         (0) root         (0)    13200 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_parser_other.c
+-rw-rw-r--   0 root         (0) root         (0)    27752 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_parser_primary.c
+-rw-rw-r--   0 root         (0) root         (0)    14399 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_parser_repomd.c
+-rw-rw-r--   0 root         (0) root         (0)    20016 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/createrepo/xml_parser_updateinfo.c
+-rw-rw-r--   0 root         (0) root         (0)    11645 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/fixtures.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.719371 createrepo_c-1.0.0/tests/python/
+-rw-rw-r--   0 root         (0) root         (0)       25 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.723371 createrepo_c-1.0.0/tests/python/tests/
+-rw-rw-r--   0 root         (0) root         (0)      167 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/CMakeLists.txt
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7555 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/fixtures.py
+-rwxrwxr-x   0 root         (0) root         (0)      199 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/run_unittests.sh.in
+-rw-rw-r--   0 root         (0) root         (0)     1212 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_checksum.py
+-rw-rw-r--   0 root         (0) root         (0)     3567 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_compression_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     2514 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_contentstat.py
+-rw-rw-r--   0 root         (0) root         (0)     4166 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_crfile.py
+-rw-rw-r--   0 root         (0) root         (0)     3414 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_load_metadata.py
+-rw-rw-r--   0 root         (0) root         (0)     4235 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_locate_metadata.py
+-rw-rw-r--   0 root         (0) root         (0)     3249 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_misc.py
+-rw-rw-r--   0 root         (0) root         (0)    10847 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_package.py
+-rw-rw-r--   0 root         (0) root         (0)     2433 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_parsepkg.py
+-rw-rw-r--   0 root         (0) root         (0)     4875 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_repomd.py
+-rw-rw-r--   0 root         (0) root         (0)     7982 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_repomdrecord.py
+-rw-rw-r--   0 root         (0) root         (0)    10544 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_sqlite.py
+-rw-rw-r--   0 root         (0) root         (0)     3063 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_updatecollection.py
+-rw-rw-r--   0 root         (0) root         (0)      938 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_updatecollectionmodule.py
+-rw-rw-r--   0 root         (0) root         (0)     1760 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_updatecollectionpackage.py
+-rw-rw-r--   0 root         (0) root         (0)    13055 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_updateinfo.py
+-rw-rw-r--   0 root         (0) root         (0)     6315 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_updaterecord.py
+-rw-rw-r--   0 root         (0) root         (0)      710 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_updatereference.py
+-rw-rw-r--   0 root         (0) root         (0)      317 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_version.py
+-rw-rw-r--   0 root         (0) root         (0)    14610 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_xml_file.py
+-rw-rw-r--   0 root         (0) root         (0)    56717 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/python/tests/test_xml_parser.py
+-rwxrwxr-x   0 root         (0) root         (0)      688 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/run_tests.sh.in
+-rw-rw-r--   0 root         (0) root         (0)     5518 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/test_checksum.c
+-rw-rw-r--   0 root         (0) root         (0)    32425 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/test_compression_wrapper.c
+-rw-rw-r--   0 root         (0) root         (0)    14197 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/test_koji.c
+-rw-rw-r--   0 root         (0) root         (0)     8097 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/test_load_metadata.c
+-rw-rw-r--   0 root         (0) root         (0)    10143 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/test_locate_metadata.c
+-rw-rw-r--   0 root         (0) root         (0)    43237 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/test_misc.c
+-rw-rw-r--   0 root         (0) root         (0)     4643 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/test_modifyrepo_shared.c
+-rw-rw-r--   0 root         (0) root         (0)     6301 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/test_sqlite.c
+-rw-rw-r--   0 root         (0) root         (0)     3948 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/test_xml_dump.c
+-rw-rw-r--   0 root         (0) root         (0)    15120 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/test_xml_dump_primary.c
+-rw-rw-r--   0 root         (0) root         (0)     4565 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/test_xml_file.c
+-rw-rw-r--   0 root         (0) root         (0)    16817 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/test_xml_parser_filelists.c
+-rw-rw-r--   0 root         (0) root         (0)    11176 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/test_xml_parser_main_metadata_together.c
+-rw-rw-r--   0 root         (0) root         (0)     4156 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/test_xml_parser_repomd.c
+-rw-rw-r--   0 root         (0) root         (0)    10261 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/test_xml_parser_updateinfo.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.675370 createrepo_c-1.0.0/tests/testdata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.727371 createrepo_c-1.0.0/tests/testdata/compressed_files/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/00_plain.foo0
+-rw-rw-r--   0 root         (0) root         (0)       33 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/00_plain.foo1
+-rw-rw-r--   0 root         (0) root         (0)       14 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/00_plain.foo2
+-rw-rw-r--   0 root         (0) root         (0)       32 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/00_plain.foo3
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/00_plain.foo4
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/00_plain.foo5
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/00_plain.txt
+-rw-rw-r--   0 root         (0) root         (0)       14 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/00_plain.txt.bz2
+-rw-rw-r--   0 root         (0) root         (0)       33 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/00_plain.txt.gz
+-rw-rw-r--   0 root         (0) root         (0)       32 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/00_plain.txt.xz
+-rw-rw-r--   0 root         (0) root         (0)       95 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/00_plain.txt.zck
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/00_plain.txt.zst
+-rw-rw-r--   0 root         (0) root         (0)       56 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/01_plain.foo0
+-rw-rw-r--   0 root         (0) root         (0)       64 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/01_plain.foo1
+-rw-rw-r--   0 root         (0) root         (0)       69 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/01_plain.foo2
+-rw-rw-r--   0 root         (0) root         (0)       96 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/01_plain.foo3
+-rw-rw-r--   0 root         (0) root         (0)      169 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/01_plain.foo4
+-rw-rw-r--   0 root         (0) root         (0)       51 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/01_plain.foo5
+-rw-rw-r--   0 root         (0) root         (0)       56 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/01_plain.txt
+-rw-rw-r--   0 root         (0) root         (0)       69 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/01_plain.txt.bz2
+-rw-rw-r--   0 root         (0) root         (0)       64 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/01_plain.txt.gz
+-rw-rw-r--   0 root         (0) root         (0)       96 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/01_plain.txt.xz
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/01_plain.txt.zck
+-rw-rw-r--   0 root         (0) root         (0)       51 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/compressed_files/01_plain.txt.zst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.727371 createrepo_c-1.0.0/tests/testdata/comps_files/
+-rw-rw-r--   0 root         (0) root         (0)      638 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/comps_files/comps_00.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.731371 createrepo_c-1.0.0/tests/testdata/modified_repo_files/
+-rw-rw-r--   0 root         (0) root         (0)      633 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/bad_file_type-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      570 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/error_00-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      802 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/error_00-other.xml
+-rw-rw-r--   0 root         (0) root         (0)     3174 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/error_00-primary.xml
+-rw-rw-r--   0 root         (0) root         (0)    68135 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/long_primary.xml
+-rw-rw-r--   0 root         (0) root         (0)     1528 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/missing_type-repomd.xml
+-rw-rw-r--   0 root         (0) root         (0)      764 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/multiple_warnings_00-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      985 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/multiple_warnings_00-other.xml
+-rw-rw-r--   0 root         (0) root         (0)     3588 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/multiple_warnings_00-primary.xml
+-rw-rw-r--   0 root         (0) root         (0)      510 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/no_pkgid-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      767 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/no_pkgid-other.xml
+-rw-rw-r--   0 root         (0) root         (0)      405 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/repo_01_ampersand-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      551 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/repo_01_ampersand-other.xml
+-rw-rw-r--   0 root         (0) root         (0)     2239 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/repo_01_ampersand-primary.xml
+-rw-rw-r--   0 root         (0) root         (0)      598 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/repo_02_different_order_filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      608 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_00-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      840 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_00-other.xml
+-rw-rw-r--   0 root         (0) root         (0)     3277 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_00-primary.xml
+-rw-rw-r--   0 root         (0) root         (0)      606 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_01-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      838 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_01-other.xml
+-rw-rw-r--   0 root         (0) root         (0)     3353 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_01-primary.xml
+-rw-rw-r--   0 root         (0) root         (0)      657 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_02-filelists.xml
+-rw-rw-r--   0 root         (0) root         (0)      889 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_02-other.xml
+-rw-rw-r--   0 root         (0) root         (0)     3342 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_02-primary.xml
+-rw-rw-r--   0 root         (0) root         (0)     1277 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/modified_repo_files/updateinfo_ampersand.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.731371 createrepo_c-1.0.0/tests/testdata/other_metadata/
+-rw-rw-r--   0 root         (0) root         (0)      894 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/other_metadata/0402e012013246e7e2f2f638c8a6046efdfd71ae1cbeff9c391d9c1ae5d7d431-comps-f19.xml.bz2
+-rw-rw-r--   0 root         (0) root         (0)     2364 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/other_metadata/36c4f2d6dda3b015b4a7da59552c7c76eff99a59979178513cb51341f6eead44-comps-f19.xml
+-rw-rw-r--   0 root         (0) root         (0)      760 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/other_metadata/71d988ca33b31a18b0d775478d6f59b40583c794ae76393284850ee97bfba4dc-comps-f19.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      804 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/other_metadata/c941e2c77a27cdca324c0e0bc3190e134fddddb36a03fb5517e55d156b955205-comps-f19.xml.xz
+-rw-rw-r--   0 root         (0) root         (0)     2364 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/other_metadata/comps-f19.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.735371 createrepo_c-1.0.0/tests/testdata/packages/
+-rw-rw-r--   0 root         (0) root         (0)     3101 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/packages/Archer-3.4.5-6.x86_64.rpm
+-rw-rw-r--   0 root         (0) root         (0)     3096 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/packages/Rimmer-1.0.2-2.x86_64.rpm
+-rw-rw-r--   0 root         (0) root         (0)     1717 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/packages/balicek-iso88591-1.1.1-1.x86_64.rpm
+-rw-rw-r--   0 root         (0) root         (0)     1741 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/packages/balicek-iso88592-1.1.1-1.x86_64.rpm
+-rw-rw-r--   0 root         (0) root         (0)     1789 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/packages/balicek-utf8-1.1.1-1.x86_64.rpm
+-rw-rw-r--   0 root         (0) root         (0)     1488 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/packages/empty-0-0.src.rpm
+-rw-rw-r--   0 root         (0) root         (0)     1401 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/packages/empty-0-0.x86_64.rpm
+-rw-rw-r--   0 root         (0) root         (0)     2237 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/packages/fake_bash-1.1.1-1.x86_64.rpm
+-rw-rw-r--   0 root         (0) root         (0)     2845 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/packages/super_kernel-6.0.1-2.x86_64.rpm
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.671370 createrepo_c-1.0.0/tests/testdata/repo_00/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.735371 createrepo_c-1.0.0/tests/testdata/repo_00/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      134 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_00/repodata/1cb61ea996355add02b1426ed4c1780ea75ce0c04c5d1107c025c3fbd7d8bcae-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      262 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_00/repodata/2e7db4492173b6c437fd1299dc335e63d09f24cbdadeac5175a61b787c2f7a44-filelists.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      123 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_00/repodata/95a4415d859d7120efb6b3cf964c07bebbff9a5275ca673e6e74a97bcbfb2a5f-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      263 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_00/repodata/a939c4765106655c3f7a13fb41d0f239824efa66bcd6c1e6c044a854012bda75-other.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      269 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_00/repodata/e0ac03cd77e95e724dbf90ded0dba664e233315a8940051dd8882c56b9878595-primary.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      123 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_00/repodata/ef3e20691954c3d1318ec3071a982da339f4ed76967ded668b795c9e070aaab6-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     3381 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_00/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.671370 createrepo_c-1.0.0/tests/testdata/repo_01/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.735371 createrepo_c-1.0.0/tests/testdata/repo_01/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      783 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_01/repodata/6c662d665c24de9a0f62c17d8fa50622307739d7376f0d19097ca96c6d7f5e3e-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      332 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_01/repodata/b752a73d9efd4006d740f943db5fb7c2dd77a8324bd99da92e86bd55a2c126ef-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      273 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_01/repodata/c7db035d0e6f1b2e883a7fa3229e2d2be70c05a8b8d2b57dbb5f9c1a67483b6c-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1497 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_01/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.671370 createrepo_c-1.0.0/tests/testdata/repo_02/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.735371 createrepo_c-1.0.0/tests/testdata/repo_02/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      341 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_02/repodata/3b7e6ecd01af9cb674aff6458186911d7081bb5676d5562a21a963afc8a8bcc7-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      403 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_02/repodata/ab5d3edeea50f9b4ec5ee13e4d25c147e318e3a433dbabc94d3461f58ac28255-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      973 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_02/repodata/bcde64b04916a2a72fdc257d61bc922c70b3d58e953499180585f7a360ce86cf-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1497 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_02/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.671370 createrepo_c-1.0.0/tests/testdata/repo_03/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.739371 createrepo_c-1.0.0/tests/testdata/repo_03/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      134 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_03/repodata/1cb61ea996355add02b1426ed4c1780ea75ce0c04c5d1107c025c3fbd7d8bcae-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      262 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_03/repodata/2e7db4492173b6c437fd1299dc335e63d09f24cbdadeac5175a61b787c2f7a44-filelists.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      123 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_03/repodata/95a4415d859d7120efb6b3cf964c07bebbff9a5275ca673e6e74a97bcbfb2a5f-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1044 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_03/repodata/a850093e240506c728d6ce26a6fc51d6a7fe10730c67988d13afa7dd82df82d5-modules.yaml.xz
+-rw-rw-r--   0 root         (0) root         (0)      263 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_03/repodata/a939c4765106655c3f7a13fb41d0f239824efa66bcd6c1e6c044a854012bda75-other.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      269 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_03/repodata/e0ac03cd77e95e724dbf90ded0dba664e233315a8940051dd8882c56b9878595-primary.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      123 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_03/repodata/ef3e20691954c3d1318ec3071a982da339f4ed76967ded668b795c9e070aaab6-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     3838 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_03/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.675370 createrepo_c-1.0.0/tests/testdata/repo_04/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.739371 createrepo_c-1.0.0/tests/testdata/repo_04/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      987 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_04/repodata/6a5f64dd82a126a161657764fe8f4b4092c0a3b61b9a34bde2af89dc1df112a1-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      397 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_04/repodata/6d0101044d9b4683e4ddc76491b3eb2228cddaace9e1d148c5eb138de9f71c17-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      429 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_04/repodata/d1c632d489f1c72b68b5c0d5de38ed1cb5c7a521380a88bed86771d39fb19538-filelists-ext.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      336 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_04/repodata/d7b8b1b6caa124aa17e4c6a1867e50e6893791ade0ebe212ab6f536695b5ce84-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     2012 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_04/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.675370 createrepo_c-1.0.0/tests/testdata/repo_koji_01/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.739371 createrepo_c-1.0.0/tests/testdata/repo_koji_01/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      816 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_koji_01/repodata/5d039d9ec332d158c69d083f04ac88a187c6b68444472b802eaf0249aec83294-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1007 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_koji_01/repodata/b153f86915d1dacbb89b244da26e50adb204195262fd3562290de26725daa21d-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      487 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_koji_01/repodata/c0e88e9a81f76341e91cd06f8ded80d4c289bdb4977e7624068802654b6da506-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1549 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_koji_01/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.675370 createrepo_c-1.0.0/tests/testdata/repo_koji_02/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.739371 createrepo_c-1.0.0/tests/testdata/repo_koji_02/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      338 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_koji_02/repodata/118e790330a62cfb167ce670478b25f4bfc58d7fc671096e4fd294fe40cee201-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      913 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_koji_02/repodata/ee9261d1d2916d841cf24bb01743198ec63ed596f410784602eca2350e430e17-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      687 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_koji_02/repodata/feb0b5fdcb0ee1cf981b041f0749ec381145cd9f6b4397991ef5dafcb6807bba-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1547 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_koji_02/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.675370 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.743371 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      656 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/0219a2f1f9f32af6b7873905269ac1bc27b03e0caf3968c929a49e5a939e8935-updateinfo_01.xml.gz.zck
+-rw-rw-r--   0 root         (0) root         (0)     2366 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/04460bfaf6cb5af6b0925d8c99401a44e5192d287796aed4cced5f7ce881761f-comps.f20.xml
+-rw-rw-r--   0 root         (0) root         (0)     3775 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/1e12239bf5cb07ec73c74482c35e80dabe30dbe2fdd57bd9e557d987cbacc8c2-primary.sqlite.bz2
+-rw-rw-r--   0 root         (0) root         (0)      864 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.gz.zck
+-rw-rw-r--   0 root         (0) root         (0)      864 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      932 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/3d6eaa7c77ef92586470dd6a542478e42cc421a85f12e0db93aa783077704cd0-filelists.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)     1287 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/490a2a494a3827b8a356f728ac36bc02fb009b0eaea173c890e727bb54219037-primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1519 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/4f4de7d3254a033b84626f330bc6adb8a3c1a4a20f0ddbe30a5692a041318c81-filelists.sqlite.bz2
+-rw-rw-r--   0 root         (0) root         (0)    88281 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/4fbad65c641f4f8fb3cec9b1672fcec2357443e1ea6e93541a0bb559c7dc9238-modules.yaml.gz
+-rw-rw-r--   0 root         (0) root         (0)      533 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/88514679cb03d8f51e850ad3639c089f899e83407a2380ef9e62873a8eb1db13-updateinfo_01.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1301 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/8b13cba732c1a02b841f43d6791ca68788d45f376787d9f3ccf68e75f01af499-other.sqlite.bz2
+-rw-rw-r--   0 root         (0) root         (0)      749 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/ba5a4fdbb20e7b9b70d9a9abd974bcab1065b1e81d711f80e06ad8cae30c4183-filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      850 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/c5582e660ed9a2d3c10ba44f0aeb02f2bb70e85dc3c8cda4266183d4e5235aa7-other.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)    86680 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/cb0f4b5df8268f248158e50d66ee1565591bca23ee2dbd84ae9c457962fa3122-modules.yaml.gz.zck
+-rw-rw-r--   0 root         (0) root         (0)     1482 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/e9e6ca4765de75cc3b2bf05e6cf631703c6557edd642300748d7747000547365-primary.xml.zck
+-rw-rw-r--   0 root         (0) root         (0)      748 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/f9d860ddcb64fbdc88a9b71a14ddb9f5670968d5dd3430412565c13d42b6804d-comps.f20.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      687 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/fd458a424a3f3e0dadc95b806674b79055c24e73637e47ad5a6e57926aa1b9d1-other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     8640 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.675370 createrepo_c-1.0.0/tests/testdata/repo_with_duplicate_packages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.743371 createrepo_c-1.0.0/tests/testdata/repo_with_duplicate_packages/repodata/
+-rw-rw-r--   0 root         (0) root         (0)      341 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_duplicate_packages/repodata/filelists.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)      405 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_duplicate_packages/repodata/other.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1017 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_duplicate_packages/repodata/primary.xml.gz
+-rw-rw-r--   0 root         (0) root         (0)     1354 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repo_with_duplicate_packages/repodata/repomd.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.743371 createrepo_c-1.0.0/tests/testdata/repodata_snippets/
+-rw-rw-r--   0 root         (0) root         (0)      436 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repodata_snippets/filelists_ext_snippet_01.xml
+-rw-rw-r--   0 root         (0) root         (0)      745 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repodata_snippets/filelists_ext_snippet_02.xml
+-rw-rw-r--   0 root         (0) root         (0)      263 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repodata_snippets/filelists_snippet_01.xml
+-rw-rw-r--   0 root         (0) root         (0)      471 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repodata_snippets/filelists_snippet_02.xml
+-rw-rw-r--   0 root         (0) root         (0)      408 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repodata_snippets/other_snippet_01.xml
+-rw-rw-r--   0 root         (0) root         (0)      697 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repodata_snippets/other_snippet_02.xml
+-rw-rw-r--   0 root         (0) root         (0)     1918 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repodata_snippets/primary_snippet_01.xml
+-rw-rw-r--   0 root         (0) root         (0)     3085 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/repodata_snippets/primary_snippet_02.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.747371 createrepo_c-1.0.0/tests/testdata/specs/
+-rwxrwxr-x   0 root         (0) root         (0)       67 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/specs/build.sh
+-rw-rw-r--   0 root         (0) root         (0)     1369 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/specs/fake-Archer.spec
+-rw-rw-r--   0 root         (0) root         (0)     1023 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/specs/fake-Rimmer.spec
+-rw-rw-r--   0 root         (0) root         (0)      571 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/specs/fake-balicek-iso88591.spec
+-rw-rw-r--   0 root         (0) root         (0)      594 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/specs/fake-balicek-iso88592.spec
+-rw-rw-r--   0 root         (0) root         (0)      653 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/specs/fake-balicek-utf8.spec
+-rw-rw-r--   0 root         (0) root         (0)      176 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/specs/fake-empty.spec
+-rw-rw-r--   0 root         (0) root         (0)      632 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/specs/fake-fake_bash.spec
+-rw-rw-r--   0 root         (0) root         (0)     1236 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/specs/fake-super_kernel.spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.747371 createrepo_c-1.0.0/tests/testdata/test_files/
+-rw-rw-r--   0 root         (0) root         (0)     1523 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/test_files/binary_file
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/test_files/empty_file
+-rw-rw-r--   0 root         (0) root         (0)    24576 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/test_files/sqlite_file.sqlite
+-rw-rw-r--   0 root         (0) root         (0)      910 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/test_files/text_file
+-rw-rw-r--   0 root         (0) root         (0)      522 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/test_files/text_file.gz
+-rw-rw-r--   0 root         (0) root         (0)      628 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/test_files/text_file.xz
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:41:20.747371 createrepo_c-1.0.0/tests/testdata/updateinfo_files/
+-rw-rw-r--   0 root         (0) root         (0)       60 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/updateinfo_files/updateinfo_00.xml
+-rw-rw-r--   0 root         (0) root         (0)     1222 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/updateinfo_files/updateinfo_01.xml
+-rw-rw-r--   0 root         (0) root         (0)      188 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/updateinfo_files/updateinfo_02.xml.xz
+-rw-rw-r--   0 root         (0) root         (0)     4805 2023-07-31 05:36:17.000000 createrepo_c-1.0.0/tests/testdata/updateinfo_files/updateinfo_03.xml
```

### Comparing `createrepo_c-0.21.1/CMakeLists.txt` & `createrepo_c-1.0.0/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 
 option(BUILD_LIBCREATEREPO_C_SHARED "Build libcreaterepo_c as a shared library" ON)
 if(NOT BUILD_LIBCREATEREPO_C_SHARED)
   set(CMAKE_POSITION_INDEPENDENT_CODE 1)
 endif()
 
+option(WITH_ZSTD "Build with zstd support" ON)
+
 option(CREATEREPO_C_INSTALL_DEVELOPMENT "Install createrepo_c development files." ON)
 option(CREATEREPO_C_INSTALL_MANPAGES "Install createrepo_c man-pages." ON)
 
 # Add path with own cmake modules
 
 INCLUDE_DIRECTORIES (${CMAKE_SOURCE_DIR})
 set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_SOURCE_DIR}/cmake/Modules/")
@@ -98,14 +100,21 @@
 IF (WITH_LIBMODULEMD)
     pkg_check_modules(LIBMODULEMD REQUIRED modulemd-2.0)
     include_directories(${LIBMODULEMD_INCLUDE_DIRS})
     SET (CMAKE_C_FLAGS          "${CMAKE_C_FLAGS} -DWITH_LIBMODULEMD")
     SET (CMAKE_C_FLAGS_DEBUG    "${CMAKE_C_FLAGS_DEBUG} -DWITH_LIBMODULEMD")
 ENDIF (WITH_LIBMODULEMD)
 
+if (WITH_ZSTD)
+    pkg_check_modules(ZSTD REQUIRED libzstd)
+    include_directories(${ZSTD_INCLUDE_DIRS})
+    SET (CMAKE_C_FLAGS          "${CMAKE_C_FLAGS} -DWITH_ZSTD")
+    SET (CMAKE_C_FLAGS_DEBUG    "${CMAKE_C_FLAGS_DEBUG} -DWITH_ZSTD")
+endif()
+
 # Threaded XZ Compression
 # Note: This option is disabled by default, because Createrepo_c
 # parallelize a lot of tasks (including compression) by default, this
 # only adds extra threads on XZ library level which causes thread bloat
 # and for most usecases doesn't bring any performance boost.
 # On regular hardware (e.g. less-or-equal 4 cores) this option may even
 # cause degradation of performance.
```

### Comparing `createrepo_c-0.21.1/COPYING` & `createrepo_c-1.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/PKG-INFO` & `createrepo_c-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: createrepo_c
-Version: 0.21.1
+Version: 1.0.0
 Summary: C implementation of createrepo
 Home-page: https://github.com/rpm-software-management
 Author: RPM Software Management
 Author-email: rpm-ecosystem@lists.rpm.org
 License: GPLv2+
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `createrepo_c-0.21.1/README.md` & `createrepo_c-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 * python (http://python.org/) - python3-devel/libpython3-dev
 * rpm (http://www.rpm.org/) - rpm-devel/librpm-dev
 * openssl (http://www.openssl.org/) - openssl-devel/libssl-dev
 * sqlite3 (https://sqlite.org/) - sqlite-devel/libsqlite3-dev
 * xz (http://tukaani.org/xz/) - xz-devel/liblzma-dev
 * zchunk (https://github.com/zchunk/zchunk) - zchunk-devel/
 * zlib (http://www.zlib.net/) - zlib-devel/zlib1g-dev
+* libzstd (http://facebook.github.io/zstd/) - libzstd-devel/libzstd-dev
 * *Documentation:* doxygen (http://doxygen.org/) - doxygen/doxygen
 * *Documentation:* sphinx (http://sphinx-doc.org/) - python3-sphinx/python3-sphinx
 * **Test requires:** check (http://check.sourceforge.net/) - check-devel/check
 * **Test requires:** xz (http://tukaani.org/xz/) - xz/
 * **Test requires:** zchunk (https://github.com/zchunk/zchunk) - zchunk/
 
 From your checkout dir:
```

### Comparing `createrepo_c-0.21.1/doc/CMakeLists.txt` & `createrepo_c-1.0.0/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/doc/Doxyfile.in.in` & `createrepo_c-1.0.0/doc/Doxyfile.in.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/doc/createrepo_c.8` & `createrepo_c-1.0.0/doc/createrepo_c.8`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 .sp
 Number of workers to spawn to read rpms.
 .SS \-\-xz
 .sp
 Use xz for repodata compression.
 .SS \-\-compress\-type COMPRESSION_TYPE
 .sp
-Which compression type to use.
+Which compression type to use. Supported compressions are: bzip2, gzip, zck, zstd, xz.
 .SS \-\-general\-compress\-type COMPRESSION_TYPE
 .sp
 Which compression type to use (even for primary, filelists and other xml).
 .SS \-\-zck
 .sp
 Generate zchunk files as well as the standard repodata.
 .SS \-\-zck\-dict\-dir ZCK_DICT_DIR
```

### Comparing `createrepo_c-0.21.1/doc/logo.png` & `createrepo_c-1.0.0/doc/logo.png`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/doc/logo.xcf` & `createrepo_c-1.0.0/doc/logo.xcf`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/doc/mergerepo_c.8` & `createrepo_c-1.0.0/doc/mergerepo_c.8`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/doc/modifyrepo_c.8` & `createrepo_c-1.0.0/doc/modifyrepo_c.8`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/doc/python/conf.py` & `createrepo_c-1.0.0/doc/python/conf.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/doc/python/lib.rst` & `createrepo_c-1.0.0/doc/python/lib.rst`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/doc/sqliterepo_c.8` & `createrepo_c-1.0.0/doc/sqliterepo_c.8`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/setup.py` & `createrepo_c-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/CMakeLists.txt` & `createrepo_c-1.0.0/src/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 TARGET_LINK_LIBRARIES(libcreaterepo_c ${LZMA_LIBRARIES})
 TARGET_LINK_LIBRARIES(libcreaterepo_c ${OPENSSL_LIBRARIES})
 TARGET_LINK_LIBRARIES(libcreaterepo_c ${RPM_LIBRARIES})
 TARGET_LINK_LIBRARIES(libcreaterepo_c ${SQLITE3_LIBRARIES})
 TARGET_LINK_LIBRARIES(libcreaterepo_c ${ZLIB_LIBRARY})
 TARGET_LINK_LIBRARIES(libcreaterepo_c ${ZCK_LIBRARIES})
 TARGET_LINK_LIBRARIES(libcreaterepo_c ${DRPM_LIBRARIES})
+TARGET_LINK_LIBRARIES(libcreaterepo_c ${ZSTD_LIBRARIES})
 
 SET_TARGET_PROPERTIES(libcreaterepo_c PROPERTIES
                       OUTPUT_NAME "createrepo_c"
                       SOVERSION ${CR_MAJOR}
                       VERSION "${VERSION}"
                       COMPILE_DEFINITIONS "G_LOG_DOMAIN=\"${G_LOG_DOMAIN}\"")
```

### Comparing `createrepo_c-0.21.1/src/checksum.c` & `createrepo_c-1.0.0/src/checksum.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/checksum.h` & `createrepo_c-1.0.0/src/checksum.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/cleanup.h` & `createrepo_c-1.0.0/src/cleanup.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/cmd_parser.c` & `createrepo_c-1.0.0/src/cmd_parser.c`

 * *Files 1% similar despite different names*

```diff
@@ -69,17 +69,17 @@
 
         .keep_all_metadata          = TRUE,
         .nevra_duplicates           = CR_ARG_DUP_NEVRA_KEEP_ALL,
     };
 
 
 gboolean
-duplicated_nevra_option_parser(const gchar *,
+duplicated_nevra_option_parser(const gchar *option_name,
                                const gchar *value,
-                               gpointer,
+                               gpointer data,
                                GError **error)
 {
     if (!g_strcmp0(value, "keep"))
         _cmd_options.nevra_duplicates = CR_ARG_DUP_NEVRA_KEEP_ALL;
     else if (!g_strcmp0(value, "keep-last"))
         _cmd_options.nevra_duplicates = CR_ARG_DUP_NEVRA_KEEP_LAST;
     else {
@@ -114,15 +114,15 @@
       "Choose the checksum type used in repomd.xml and for packages in the "
       "metadata. The default is now \"sha256\".", "CHECKSUM_TYPE" },
     { "pretty", 'p', 0, G_OPTION_ARG_NONE, &(_cmd_options.pretty),
       "Make sure all xml generated is formatted (default)", NULL },
     { "database", 'd', 0, G_OPTION_ARG_NONE, &(_cmd_options.database),
       "Generate sqlite databases for use with yum.", NULL },
     { "no-database", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.no_database),
-      "Do not generate sqlite databases in the repository.", NULL },
+      "Do not generate sqlite databases in the repository (default).", NULL },
     { "filelists-ext", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.filelists_ext),
       "Create filelists-ext metadata with file hashes.", NULL },
     { "update", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.update),
       "If metadata already exists in the outputdir and an rpm is unchanged "
       "(based on file size and mtime) since the metadata was generated, reuse "
       "the existing metadata rather than recalculating it. In the case of a "
       "large repository with only a few new or modified rpms "
@@ -176,17 +176,17 @@
       "Output the paths to the pkgs actually read useful with --update.",
       "READ_PKGS_LIST" },
     { "workers", 0, 0, G_OPTION_ARG_INT, &(_cmd_options.workers),
       "Number of workers to spawn to read rpms.", NULL },
     { "xz", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.xz_compression),
       "Use xz for repodata compression.", NULL },
     { "compress-type", 0, 0, G_OPTION_ARG_STRING, &(_cmd_options.compress_type),
-      "Which compression type to use.", "COMPRESSION_TYPE" },
+      "Which compression type to use for additional metadata files (comps, updateinfo, etc). Supported compressions are: bzip2, gzip, zck, zstd, xz.", "COMPRESSION_TYPE" },
     { "general-compress-type", 0, 0, G_OPTION_ARG_STRING, &(_cmd_options.general_compress_type),
-      "Which compression type to use (even for primary, filelists and other xml).",
+      "Which compression type to use (even for primary, filelists and other xml). Supported compressions are: bzip2, gzip, zck, zstd, xz.",
       "COMPRESSION_TYPE" },
 #ifdef WITH_ZCHUNK
     { "zck", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.zck_compression),
       "Generate zchunk files as well as the standard repodata.", NULL },
     { "zck-dict-dir", 0, 0, G_OPTION_ARG_FILENAME, &(_cmd_options.zck_dict_dir),
       "Directory containing compression dictionaries for use by zchunk", "ZCK_DICT_DIR" },
 #endif
@@ -311,14 +311,16 @@
 
     if (!strcmp(compress_str->str, "gz")) {
         *type = CR_CW_GZ_COMPRESSION;
     } else if (!strcmp(compress_str->str, "bz2")) {
         *type = CR_CW_BZ2_COMPRESSION;
     } else if (!strcmp(compress_str->str, "xz")) {
         *type = CR_CW_XZ_COMPRESSION;
+    } else if (!strcmp(compress_str->str, "zstd")) {
+        *type = CR_CW_ZSTD_COMPRESSION;
     } else {
         g_set_error(err, ERR_DOMAIN, CRE_BADARG,
                     "Unknown/Unsupported compression type \"%s\"", type_str);
         return FALSE;
     }
 
     return TRUE;
@@ -382,15 +384,15 @@
                 GError **err)
 {
     assert(!err || *err == NULL);
 
     // Check outputdir
     if (options->outputdir && !g_file_test(options->outputdir, G_FILE_TEST_EXISTS|G_FILE_TEST_IS_DIR)) {
         g_set_error(err, ERR_DOMAIN, CRE_BADARG,
-                    "Specified outputdir \"%s\" doesn't exists",
+                    "Specified outputdir \"%s\" doesn't exist",
                     options->outputdir);
         return FALSE;
     }
 
     // Check workers
     if ((options->workers < 1) || (options->workers > 100)) {
         g_warning("Wrong number of workers - Using 5 workers.");
@@ -494,25 +496,25 @@
             options->groupfile_fullpath = g_strconcat(input_dir,
                                                       options->groupfile,
                                                       NULL);
         }
 
         if (!remote && !g_file_test(options->groupfile_fullpath, G_FILE_TEST_IS_REGULAR)) {
             g_set_error(err, ERR_DOMAIN, CRE_BADARG,
-                        "groupfile %s doesn't exists",
+                        "groupfile %s doesn't exist",
                         options->groupfile_fullpath);
             return FALSE;
         }
     }
 
     // Process pkglist file
     if (options->pkglist) {
         if (!g_file_test(options->pkglist, G_FILE_TEST_IS_REGULAR)) {
             g_set_error(err, ERR_DOMAIN, CRE_BADARG,
-                        "pkglist file \"%s\" doesn't exists", options->pkglist);
+                        "pkglist file \"%s\" doesn't exist", options->pkglist);
             return FALSE;
         } else {
             char *content = NULL;
             GError *tmp_err = NULL;
             if (!g_file_get_contents(options->pkglist, &content, NULL, &tmp_err)) {
                 g_warning("Error while reading pkglist file: %s", tmp_err->message);
                 g_error_free(tmp_err);
```

### Comparing `createrepo_c-0.21.1/src/cmd_parser.h` & `createrepo_c-1.0.0/src/cmd_parser.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/compression_wrapper.c` & `createrepo_c-1.0.0/src/compression_wrapper.c`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 #include <bzlib.h>
 #include <lzma.h>
 #ifdef WITH_ZCHUNK
 #include <zck.h>
 #endif  // WITH_ZCHUNK
 #include "error.h"
 #include "compression_wrapper.h"
+#ifdef WITH_ZSTD
+#include <zstd.h>
+#endif
 
 
 #define ERR_DOMAIN                      CREATEREPO_C_ERROR
 
 /*
 #define Z_CR_CW_NO_COMPRESSION          0
 #define Z_BEST_SPEED                    1
@@ -114,27 +117,38 @@
 
 typedef struct {
     lzma_stream stream;
     FILE *file;
     unsigned char buffer[XZ_BUFFER_SIZE];
 } XzFile;
 
+#ifdef WITH_ZSTD
+#define CR_CW_ZSTD_COMPRESSION_LEVEL    9
+typedef struct {
+    void *buffer;
+    size_t buffer_size;
+    ZSTD_inBuffer zib;
+    ZSTD_outBuffer zob;
+    void * context;     //ZSTD_{C,D}Ctx
+} ZstdFile;
+#endif
+
 cr_CompressionType
 cr_detect_compression(const char *filename, GError **err)
 {
     cr_CompressionType type = CR_CW_UNKNOWN_COMPRESSION;
 
     assert(filename);
     assert(!err || *err == NULL);
 
     if (!g_file_test(filename, G_FILE_TEST_IS_REGULAR)) {
-        g_debug("%s: File %s doesn't exists or not a regular file",
+        g_debug("%s: File %s doesn't exist or not a regular file",
                 __func__, filename);
         g_set_error(err, ERR_DOMAIN, CRE_NOFILE,
-                    "File %s doesn't exists or not a regular file", filename);
+                    "File %s doesn't exist or not a regular file", filename);
         return CR_CW_UNKNOWN_COMPRESSION;
     }
 
     // Try determine compression type via filename suffix
 
     if (g_str_has_suffix(filename, ".gz") ||
         g_str_has_suffix(filename, ".gzip") ||
@@ -147,14 +161,17 @@
         return CR_CW_BZ2_COMPRESSION;
     } else if (g_str_has_suffix(filename, ".xz"))
     {
         return CR_CW_XZ_COMPRESSION;
     } else if (g_str_has_suffix(filename, ".zck"))
     {
         return CR_CW_ZCK_COMPRESSION;
+    } else if (g_str_has_suffix(filename, ".zst"))
+    {
+        return CR_CW_ZSTD_COMPRESSION;
     } else if (g_str_has_suffix(filename, ".xml") ||
                g_str_has_suffix(filename, ".tar") ||
                g_str_has_suffix(filename, ".yaml") ||
                g_str_has_suffix(filename, ".sqlite"))
     {
         return CR_CW_NO_COMPRESSION;
     }
@@ -188,14 +205,19 @@
             g_str_has_prefix(mime_type, "application/x-compress") ||
             g_str_has_prefix(mime_type, "application/x-gunzip") ||
             g_str_has_prefix(mime_type, "multipart/x-gzip"))
         {
             type = CR_CW_GZ_COMPRESSION;
         }
 
+        else if (g_str_has_prefix(mime_type, "application/zstd"))
+        {
+            type = CR_CW_ZSTD_COMPRESSION;
+        }
+
         else if (g_str_has_prefix(mime_type, "application/x-bzip2") ||
                  g_str_has_prefix(mime_type, "application/x-bz2") ||
                  g_str_has_prefix(mime_type, "application/bzip2") ||
                  g_str_has_prefix(mime_type, "application/bz2"))
         {
             type = CR_CW_BZ2_COMPRESSION;
         }
@@ -251,14 +273,16 @@
         type = CR_CW_GZ_COMPRESSION;
     if (!g_strcmp0(name_lower, "bz2") || !g_strcmp0(name_lower, "bzip2"))
         type = CR_CW_BZ2_COMPRESSION;
     if (!g_strcmp0(name_lower, "xz"))
         type = CR_CW_XZ_COMPRESSION;
     if (!g_strcmp0(name_lower, "zck"))
         type = CR_CW_ZCK_COMPRESSION;
+    if (!g_strcmp0(name_lower, "zstd"))
+        type = CR_CW_ZSTD_COMPRESSION;
     g_free(name_lower);
 
     return type;
 }
 
 const char *
 cr_compression_suffix(cr_CompressionType comtype)
@@ -268,14 +292,16 @@
             return ".gz";
         case CR_CW_BZ2_COMPRESSION:
             return ".bz2";
         case CR_CW_XZ_COMPRESSION:
             return ".xz";
         case CR_CW_ZCK_COMPRESSION:
             return ".zck";
+        case CR_CW_ZSTD_COMPRESSION:
+            return ".zst";
         default:
             return NULL;
     }
 }
 
 
 static const char *
@@ -409,14 +435,64 @@
             if (gzbuffer((gzFile) file->FILE, GZ_BUFFER_SIZE) == -1) {
                 g_debug("%s: gzbuffer() call failed", __func__);
                 g_set_error(err, ERR_DOMAIN, CRE_GZ,
                             "gzbuffer() call failed");
             }
             break;
 
+        case (CR_CW_ZSTD_COMPRESSION): { // ------------------------------------
+#ifdef WITH_ZSTD
+            FILE *f = fopen(filename, mode_str);
+
+            if (!f) {
+                g_set_error(err, ERR_DOMAIN, CRE_IO, "fopen(): %s", g_strerror(errno));
+                break;
+            }
+
+            file->INNERFILE = f;
+
+            ZstdFile *zstd_file = g_malloc0(sizeof(ZstdFile));
+
+            if (mode == CR_CW_MODE_WRITE) {
+                if ((zstd_file->context = (void *) ZSTD_createCCtx()) == NULL) {
+                    g_set_error(err, ERR_DOMAIN, CRE_ZSTD, "%s",
+                            "Failed to create ZSTD context.");
+                    g_free(zstd_file);
+                    fclose(f);
+                    break;
+                }
+                size_t ret = ZSTD_CCtx_setParameter(zstd_file->context, ZSTD_c_compressionLevel, CR_CW_ZSTD_COMPRESSION_LEVEL);
+                if (ZSTD_isError(ret)) {
+                    g_set_error(err, ERR_DOMAIN, CRE_ZSTD, "%s",
+                            ZSTD_getErrorName(ret));
+                    g_free(zstd_file);
+                    fclose(f);
+                    break;
+                }
+                zstd_file->buffer_size = ZSTD_CStreamOutSize();
+            } else {
+                if ((zstd_file->context = (void *) ZSTD_createDCtx()) == NULL) {
+                    g_free(zstd_file);
+                    fclose(f);
+                    g_set_error(err, ERR_DOMAIN, CRE_IO, "%s",
+                            "Failed to create ZSTD context.");
+                    break;
+                }
+                zstd_file->buffer_size = ZSTD_DStreamInSize();
+            }
+            zstd_file->buffer = g_malloc(zstd_file->buffer_size);
+            file->FILE = (void *) zstd_file;
+
+            break;
+#else
+            g_set_error(err, ERR_DOMAIN, CRE_IO, "createrepo_c wasn't compiled with zstd support");
+            break;
+#endif // WITH_ZSTD
+        }
+
         case (CR_CW_BZ2_COMPRESSION): { // ------------------------------------
             FILE *f = fopen(filename, mode_str);
             file->INNERFILE = f;
             int bzerror;
 
             if (!f) {
                 g_set_error(err, ERR_DOMAIN, CRE_IO,
@@ -765,14 +841,51 @@
 
                 ret = CRE_GZ;
                 g_set_error(err, ERR_DOMAIN, CRE_GZ,
                     "gzclose(): %s", err_msg);
             }
             break;
 
+        case (CR_CW_ZSTD_COMPRESSION): { // --------------------------------------
+#ifdef WITH_ZSTD
+            ZstdFile * zstd = (ZstdFile *) cr_file->FILE;
+            if (cr_file->mode == CR_CW_MODE_READ) {
+                ZSTD_freeDCtx(zstd->context);
+            } else {
+                size_t remaining;
+                // No more new input just finish flushing compression data
+                ZSTD_inBuffer zip = { NULL, 0, 0 };
+                do {
+                    zstd->zob.dst = zstd->buffer;
+                    zstd->zob.size = zstd->buffer_size;
+                    zstd->zob.pos = 0;
+
+                    remaining = ZSTD_compressStream2(zstd->context, &zstd->zob , &zip, ZSTD_e_end);
+                    if (ZSTD_isError(remaining)) {
+                        g_set_error(err, ERR_DOMAIN, CRE_ZSTD, "%s", ZSTD_getErrorName(remaining));
+                        break;
+                    } else if (zstd->zob.pos != fwrite(zstd->buffer, 1, zstd->zob.pos, cr_file->INNERFILE)) {
+                        g_set_error(err, ERR_DOMAIN, CRE_IO, "cr_close ZSTD fwrite failed");
+                        break;
+                    }
+                } while(remaining != 0);
+                ZSTD_freeCCtx(zstd->context);
+            }
+
+            fclose(cr_file->INNERFILE);
+            g_free(zstd->buffer);
+            g_free(cr_file->FILE);
+
+            ret = CRE_OK;
+            break;
+#else
+            g_set_error(err, ERR_DOMAIN, CRE_IO, "createrepo_c wasn't compiled with zstd support");
+            break;
+#endif // WITH_ZSTD
+        }
         case (CR_CW_BZ2_COMPRESSION): // --------------------------------------
             if (cr_file->mode == CR_CW_MODE_READ)
                 BZ2_bzReadClose(&rc, (BZFILE *) cr_file->FILE);
             else
                 BZ2_bzWriteClose(&rc, (BZFILE *) cr_file->FILE,
                                  BZ2_SKIP_FFLUSH, NULL, NULL);
 
@@ -976,14 +1089,51 @@
             if (ret == -1) {
                 ret = CR_CW_ERR;
                 g_set_error(err, ERR_DOMAIN, CRE_GZ,
                     "fread(): %s", cr_gz_strerror((gzFile) cr_file->FILE));
             }
             break;
 
+        case (CR_CW_ZSTD_COMPRESSION): { // ---------------------------------------
+#ifdef WITH_ZSTD
+            ZstdFile * zstd = (ZstdFile *) cr_file->FILE;
+
+            ZSTD_outBuffer zob = {buffer, len, 0};
+
+            while (zob.pos < zob.size) {
+                // Re-fill compressed data buffer
+                if (zstd->zib.pos >= zstd->zib.size) {
+                    zstd->zib.size = fread(zstd->buffer, 1, zstd->buffer_size, cr_file->INNERFILE);
+                    if (zstd->zib.size == 0) {
+                        break; //EOF
+                    }
+                    zstd->zib.src = zstd->buffer;
+                    zstd->zib.pos = 0;
+                }
+
+                // Decompress chunk
+                int decomp_ret = ZSTD_decompressStream(zstd->context, &zob, &zstd->zib);
+                if (ZSTD_isError(decomp_ret)) {
+                    ret = CR_CW_ERR;
+                    g_set_error(err, ERR_DOMAIN, CRE_ZSTD, "%s", ZSTD_getErrorName(decomp_ret));
+                    break;
+                }
+
+            }
+
+            if (!(err && *err)) {
+                ret = zob.pos;
+            }
+
+            break;
+#else
+            g_set_error(err, ERR_DOMAIN, CRE_IO, "createrepo_c wasn't compiled with zstd support");
+            break;
+#endif // WITH_ZSTD
+        }
         case (CR_CW_BZ2_COMPRESSION): // --------------------------------------
             ret = BZ2_bzRead(&bzerror, (BZFILE *) cr_file->FILE, buffer, len);
             if (!ret && bzerror == BZ_SEQUENCE_ERROR)
                 // Next read after BZ_STREAM_END (EOF)
                 return 0;
 
             if (bzerror != BZ_OK && bzerror != BZ_STREAM_END) {
@@ -1210,14 +1360,53 @@
             if ((ret = gzwrite((gzFile) cr_file->FILE, buffer, len)) == 0) {
                 ret = CR_CW_ERR;
                 g_set_error(err, ERR_DOMAIN, CRE_GZ,
                     "gzwrite(): %s", cr_gz_strerror((gzFile) cr_file->FILE));
             }
             break;
 
+        case (CR_CW_ZSTD_COMPRESSION): { // ---------------------------------------
+#ifdef WITH_ZSTD
+            ZstdFile * zstd = (ZstdFile *) cr_file->FILE;
+            ZSTD_inBuffer zib = {buffer, len, 0};
+
+            while (zib.pos < zib.size) {
+                zstd->zob.dst = zstd->buffer;
+                zstd->zob.size = zstd->buffer_size;
+                zstd->zob.pos = 0;
+
+                // Compress chunk into buffer
+                size_t remaining = ZSTD_compressStream2(zstd->context, &zstd->zob , &zib, ZSTD_e_continue);
+                if (ZSTD_isError(remaining)) {
+                    g_set_error(err, ERR_DOMAIN, CRE_ZSTD, "%s", ZSTD_getErrorName(remaining));
+                    break;
+                }
+
+                // Write compressed buffer
+                if (zstd->zob.pos > 0) {
+                    size_t nw = fwrite(zstd->buffer, 1, zstd->zob.pos, cr_file->INNERFILE);
+                    if (nw != zstd->zob.pos) {
+                        g_set_error(err, ERR_DOMAIN, CRE_IO, "cr_write zstd write failed");
+                        break;
+                    }
+                }
+
+            }
+
+            if (!(err && *err)) {
+                ret = zib.pos;
+            }
+
+            break;
+#else
+            g_set_error(err, ERR_DOMAIN, CRE_IO, "createrepo_c wasn't compiled with zstd support");
+            break;
+#endif // WITH_ZSTD
+        }
+
         case (CR_CW_BZ2_COMPRESSION): // --------------------------------------
             BZ2_bzWrite(&bzerror, (BZFILE *) cr_file->FILE, (void *) buffer, len);
             if (bzerror == BZ_OK) {
                 ret = len;
             } else {
                 const char *err_msg;
                 ret = CR_CW_ERR;
@@ -1357,14 +1546,15 @@
     switch (cr_file->type) {
 
         case (CR_CW_NO_COMPRESSION): // ---------------------------------------
         case (CR_CW_GZ_COMPRESSION): // ---------------------------------------
         case (CR_CW_BZ2_COMPRESSION): // --------------------------------------
         case (CR_CW_XZ_COMPRESSION): // ---------------------------------------
         case (CR_CW_ZCK_COMPRESSION): // --------------------------------------
+        case (CR_CW_ZSTD_COMPRESSION): // --------------------------------------
             len = strlen(str);
             ret = cr_write(cr_file, str, len, err);
             if (ret != (int) len)
                 ret = CR_CW_ERR;
             break;
 
         default: // -----------------------------------------------------------
@@ -1394,14 +1584,15 @@
     }
 
     switch (cr_file->type) {
         case (CR_CW_NO_COMPRESSION): // ---------------------------------------
         case (CR_CW_GZ_COMPRESSION): // ---------------------------------------
         case (CR_CW_BZ2_COMPRESSION): // --------------------------------------
         case (CR_CW_XZ_COMPRESSION): // ---------------------------------------
+        case (CR_CW_ZSTD_COMPRESSION): // ---------------------------------------
             break;
         case (CR_CW_ZCK_COMPRESSION): { // ------------------------------------
 #ifdef WITH_ZCHUNK
             zckCtx *zck = (zckCtx *) cr_file->FILE;
             ssize_t wb = zck_end_chunk(zck);
             if (wb < 0) {
                 g_set_error(err, ERR_DOMAIN, CRE_ZCK,
@@ -1446,14 +1637,15 @@
     }
 
     switch (cr_file->type) {
         case (CR_CW_NO_COMPRESSION): // ---------------------------------------
         case (CR_CW_GZ_COMPRESSION): // ---------------------------------------
         case (CR_CW_BZ2_COMPRESSION): // --------------------------------------
         case (CR_CW_XZ_COMPRESSION): // ---------------------------------------
+        case (CR_CW_ZSTD_COMPRESSION): // ---------------------------------------
             break;
         case (CR_CW_ZCK_COMPRESSION): { // ------------------------------------
 #ifdef WITH_ZCHUNK
             zckCtx *zck = (zckCtx *) cr_file->FILE;
             if (!zck_set_ioption(zck, ZCK_MANUAL_CHUNK, !auto_chunk)) {
                 g_set_error(err, ERR_DOMAIN, CRE_ZCK,
                             "Error setting auto_chunk: %s",
@@ -1520,14 +1712,15 @@
     switch (cr_file->type) {
 
         case (CR_CW_NO_COMPRESSION): // ---------------------------------------
         case (CR_CW_GZ_COMPRESSION): // ---------------------------------------
         case (CR_CW_BZ2_COMPRESSION): // --------------------------------------
         case (CR_CW_XZ_COMPRESSION): // ---------------------------------------
         case (CR_CW_ZCK_COMPRESSION): // --------------------------------------
+        case (CR_CW_ZSTD_COMPRESSION): // --------------------------------------
             tmp_ret = cr_write(cr_file, buf, ret, err);
             if (tmp_ret != (int) ret)
                 ret = CR_CW_ERR;
             break;
 
         default: // -----------------------------------------------------------
             ret = CR_CW_ERR;
```

### Comparing `createrepo_c-0.21.1/src/compression_wrapper.h` & `createrepo_c-1.0.0/src/compression_wrapper.h`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     CR_CW_AUTO_DETECT_COMPRESSION,    /*!< Autodetection */
     CR_CW_UNKNOWN_COMPRESSION,        /*!< Unknown compression */
     CR_CW_NO_COMPRESSION,             /*!< No compression */
     CR_CW_GZ_COMPRESSION,             /*!< Gzip compression */
     CR_CW_BZ2_COMPRESSION,            /*!< BZip2 compression */
     CR_CW_XZ_COMPRESSION,             /*!< XZ compression */
     CR_CW_ZCK_COMPRESSION,            /*!< ZCK compression */
+    CR_CW_ZSTD_COMPRESSION,           /*!< ZSTD compression */
     CR_CW_COMPRESSION_SENTINEL,       /*!< Sentinel of the list */
 } cr_CompressionType;
 
 /** Open modes.
  */
 typedef enum {
     CR_CW_MODE_READ,            /*!< Read mode */
```

### Comparing `createrepo_c-0.21.1/src/constants.h` & `createrepo_c-1.0.0/src/constants.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/createrepo_c.c` & `createrepo_c-1.0.0/src/createrepo_c.c`

 * *Files 2% similar despite different names*

```diff
@@ -378,72 +378,14 @@
         }
     }
 
     g_debug("Cachedir for checksums is %s", cmd_options->checksum_cachedir);
     return TRUE;
 }
 
-/** Adds groupfile cr_RepomdRecords to additional_metadata_rec list.
- *  Groupfile is a special case, because it's the only metadatum
- *  that can be inputed to createrepo_c via command line option.
- *
- * @param group_metadatum           Cr_Metadatum for used groupfile
- * @param additional_metadata_rec   GSList of cr_RepomdRecords
- * @param comp_type                 Groupfile compression type
- * @param repomd_checksum_type
- *
- * @return                          GSList with added cr_RepomdRecords for
- *                                  groupfile
- */
-GSList*
-cr_create_repomd_records_for_groupfile_metadata(const cr_Metadatum *group_metadatum,
-                                                GSList *additional_metadata_rec,
-                                                cr_CompressionType comp_type,
-                                                cr_ChecksumType repomd_checksum_type)
-{
-    GError *tmp_err = NULL;
-    char *compression_suffix = g_strdup(cr_compression_suffix(comp_type));
-    compression_suffix[0] = '_'; //replace '.'
-    additional_metadata_rec = g_slist_prepend(additional_metadata_rec,
-                                              cr_repomd_record_new(
-                                                  group_metadatum->type,
-                                                  group_metadatum->name
-                                              ));
-
-    gchar *compressed_record_type = g_strconcat(group_metadatum->type, compression_suffix, NULL);
-    additional_metadata_rec = g_slist_prepend(additional_metadata_rec,
-                                              cr_repomd_record_new(
-                                                  compressed_record_type,
-                                                  NULL
-                                              ));
-
-    cr_repomd_record_compress_and_fill(additional_metadata_rec->next->data,
-                                       additional_metadata_rec->data,
-                                       repomd_checksum_type,
-                                       comp_type,
-                                       NULL,
-                                       &tmp_err);
-
-    if (tmp_err) {
-        g_critical("Cannot process %s %s: %s",
-                   group_metadatum->type,
-                   group_metadatum->name,
-                   tmp_err->message);
-        g_free(compression_suffix);
-        g_free(compressed_record_type);
-        g_clear_error(&tmp_err);
-        exit(EXIT_FAILURE);
-    }
-
-    g_free(compressed_record_type);
-    g_free(compression_suffix);
-
-    return additional_metadata_rec;
-}
-
 /** Creates list of cr_RepomdRecords from list
  *  of additional metadata (cr_Metadatum)
  *
  * @param additional_metadata       List of cr_Metadatum
  * @param repomd_checksum_type
  *
  * @return                          New GSList of cr_RepomdRecords
@@ -880,17 +822,17 @@
     current_pkglist = NULL;
     GSList *additional_metadata = NULL;
 
     // Setup compression types
     const char *xml_compression_suffix = NULL;
     const char *sqlite_compression_suffix = NULL;
     const char *compression_suffix = NULL;
-    cr_CompressionType xml_compression = CR_CW_GZ_COMPRESSION;
+    cr_CompressionType xml_compression = CR_CW_ZSTD_COMPRESSION;
     cr_CompressionType sqlite_compression = CR_CW_BZ2_COMPRESSION;
-    cr_CompressionType compression = CR_CW_GZ_COMPRESSION;
+    cr_CompressionType compression = CR_CW_ZSTD_COMPRESSION;
 
     if (cmd_options->compression_type != CR_CW_UNKNOWN_COMPRESSION) {
         sqlite_compression = cmd_options->compression_type;
         compression        = cmd_options->compression_type;
     }
 
     if (cmd_options->general_compression_type != CR_CW_UNKNOWN_COMPRESSION) {
@@ -899,21 +841,22 @@
         compression        = cmd_options->general_compression_type;
     }
 
     xml_compression_suffix = cr_compression_suffix(xml_compression);
     sqlite_compression_suffix = cr_compression_suffix(sqlite_compression);
     compression_suffix = cr_compression_suffix(compression);
 
-    cr_Metadatum *new_groupfile_metadatum = NULL;
-
     // Groupfile specified as argument
     if (cmd_options->groupfile_fullpath) {
-        new_groupfile_metadatum = g_malloc0(sizeof(cr_Metadatum));
-        new_groupfile_metadatum->name = cr_copy_metadatum(cmd_options->groupfile_fullpath, tmp_out_repo, &tmp_err);
+        gchar *compressed_path = cr_compress_groupfile(cmd_options->groupfile_fullpath, tmp_out_repo, compression);
+        cr_Metadatum *new_groupfile_metadatum = g_malloc0(sizeof(cr_Metadatum));
+        new_groupfile_metadatum->name = compressed_path;
         new_groupfile_metadatum->type = g_strdup("group");
+        additional_metadata = g_slist_prepend(additional_metadata, new_groupfile_metadatum);
+
         //remove old groupfile(s) (every [compressed] variant)
         if (old_metadata_location){
             GSList *node_iter = old_metadata_location->additional_metadata;
             while (node_iter != NULL){
                 cr_Metadatum *m = node_iter->data;
                 GSList *next = g_slist_next(node_iter);
                 if(g_str_has_prefix(m->type, "group")){
@@ -1074,15 +1017,15 @@
 
     gchar *pri_xml_filename = NULL;
     gchar *fil_xml_filename = NULL;
     gchar *fex_xml_filename = NULL;
     gchar *oth_xml_filename = NULL;
 
     g_message("Temporary output repo path: %s", tmp_out_repo);
-    g_debug("Creating .xml.gz files");
+    g_debug("Creating .xml.%s files", xml_compression_suffix);
 
     pri_xml_filename = g_strconcat(tmp_out_repo, "/primary.xml", xml_compression_suffix, NULL);
     fil_xml_filename = g_strconcat(tmp_out_repo, "/filelists.xml", xml_compression_suffix, NULL);
     if (cmd_options->filelists_ext)
         fex_xml_filename = g_strconcat(tmp_out_repo, "/filelists-ext.xml", xml_compression_suffix, NULL);
     oth_xml_filename = g_strconcat(tmp_out_repo, "/other.xml", xml_compression_suffix, NULL);
 
@@ -1189,15 +1132,15 @@
     gchar *fex_db_filename = NULL;
     gchar *oth_db_filename = NULL;
     cr_SqliteDb *pri_db = NULL;
     cr_SqliteDb *fil_db = NULL;
     cr_SqliteDb *fex_db = NULL;
     cr_SqliteDb *oth_db = NULL;
 
-    if (!cmd_options->no_database) {
+    if (cmd_options->database) {
         _cleanup_file_close_ int pri_db_fd = -1;
         _cleanup_file_close_ int fil_db_fd = -1;
         _cleanup_file_close_ int fex_db_fd = -1;
         _cleanup_file_close_ int oth_db_fd = -1;
 
         g_message("Preparing sqlite DBs");
         if (!cmd_options->local_sqlite) {
@@ -1860,38 +1803,24 @@
                                                 NULL);
     g_thread_pool_push(fill_pool, oth_fill_task, NULL);
 
 
     additional_metadata_rec = cr_create_repomd_records_for_additional_metadata(additional_metadata,
                                                                                cmd_options->repomd_checksum_type);
 
-    if (new_groupfile_metadatum) {
-        additional_metadata_rec = cr_create_repomd_records_for_groupfile_metadata(new_groupfile_metadatum,
-                                                                                  additional_metadata_rec,
-                                                                                  compression,
-                                                                                  cmd_options->repomd_checksum_type);
-
-        //NOTE(amatej): Now we can add groupfile metadata to the additional_metadata list, for unified handlig while zck compressing
-        additional_metadata = g_slist_prepend(additional_metadata, new_groupfile_metadatum);
-        cr_Metadatum *compressed_new_groupfile_metadatum = g_malloc0(sizeof(cr_Metadatum));
-        compressed_new_groupfile_metadatum->name = g_strdup(((cr_RepomdRecord *) additional_metadata_rec->data)->location_real);
-        compressed_new_groupfile_metadatum->type = g_strdup(((cr_RepomdRecord *) additional_metadata_rec->data)->type);
-        additional_metadata = g_slist_prepend(additional_metadata, compressed_new_groupfile_metadatum);
-    }
-
     // Wait till repomd record fill task of xml files ends.
     g_thread_pool_free(fill_pool, FALSE, TRUE);
 
     cr_repomdrecordfilltask_free(pri_fill_task, NULL);
     cr_repomdrecordfilltask_free(fil_fill_task, NULL);
     cr_repomdrecordfilltask_free(fex_fill_task, NULL);
     cr_repomdrecordfilltask_free(oth_fill_task, NULL);
 
     // Sqlite db
-    if (!cmd_options->no_database) {
+    if (cmd_options->database) {
 
         gchar *pri_db_name = g_strconcat(tmp_out_repo, "/primary.sqlite",
                                          sqlite_compression_suffix, NULL);
         gchar *fil_db_name = g_strconcat(tmp_out_repo, "/filelists.sqlite",
                                          sqlite_compression_suffix, NULL);
         gchar *fex_db_name = NULL;
         if (cmd_options->filelists_ext)
@@ -2471,15 +2400,15 @@
 
     // Rename out_repo to "repodata.old.pid.date.microsecs"
     gchar *tmp_dirname = cr_append_pid_and_datetime("repodata.old.", NULL);
     gchar *old_repodata_path = g_build_filename(out_dir, tmp_dirname, NULL);
     g_free(tmp_dirname);
 
     if (!cr_move_recursive(out_repo, old_repodata_path, &tmp_err)) {
-        g_debug("Old repodata doesn't exists: Cannot rename %s -> %s: %s",
+        g_debug("Old repodata doesn't exist: Cannot rename %s -> %s: %s",
                 out_repo, old_repodata_path, tmp_err->message);
     } else {
         g_debug("Renamed %s -> %s", out_repo, old_repodata_path);
         old_repodata_renamed = TRUE;
     }
 
     // Rename tmp_out_repo to out_repo
```

### Comparing `createrepo_c-0.21.1/src/createrepo_c.h` & `createrepo_c-1.0.0/src/createrepo_c.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/createrepo_shared.c` & `createrepo_c-1.0.0/src/createrepo_shared.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/createrepo_shared.h` & `createrepo_c-1.0.0/src/createrepo_shared.h`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 gboolean
 cr_unblock_terminating_signals(GError **err);
 
 
 /**
  * This function does:
  * - Tries to create repo/.repodata/ dir.
- * - If it doesn't exists, it's created and function returns TRUE.
+ * - If it doesn't exist, it's created and function returns TRUE.
  * - If it exists and ignore_lock is FALSE, returns FALSE and err is set.
  * - If it exists and ignore_lock is TRUE it:
  *  - Removes the existing .repodata/ dir and all its content
  *  - Creates (empty) new one (just as a lock dir - place holder)
  *  - Creates .repodata.pid.datetime.usec/ that should be used for
  *    repodata generation
  *
```

### Comparing `createrepo_c-0.21.1/src/deltarpms.c` & `createrepo_c-1.0.0/src/deltarpms.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/deltarpms.h.in` & `createrepo_c-1.0.0/src/deltarpms.h.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/dumper_thread.c` & `createrepo_c-1.0.0/src/dumper_thread.c`

 * *Files 0% similar despite different names*

```diff
@@ -627,18 +627,20 @@
                 // CR_PACKAGE_SINGLE_CHUNK used with the preloaded (old)
                 // metadata.  Create a new per-package chunk.
                 assert (!md->chunk);
                 md->chunk = g_string_chunk_new(1024);
                 md->loadingflags &= ~CR_PACKAGE_SINGLE_CHUNK;
 
                 // We have usable old data, but we have to set proper locations
-                // WARNING! This two lines destructively modifies content of
-                // packages in old metadata.
+                // WARNING! location_href is overidden
+                // location_base is kept by default, unless specified differently
+                //
                 md->location_href = cr_safe_string_chunk_insert(md->chunk, location_href);
-                md->location_base = cr_safe_string_chunk_insert(md->chunk, location_base);
+                if (location_base)
+                    md->location_base = cr_safe_string_chunk_insert(md->chunk, location_base);
                 // ^^^ The location_base and location_href create a new data
                 // chunk, even though the rest of the metadata is stored in the
                 // global chunk (shared with all packages).
             }
         }
     }
```

### Comparing `createrepo_c-0.21.1/src/dumper_thread.h` & `createrepo_c-1.0.0/src/dumper_thread.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/error.c` & `createrepo_c-1.0.0/src/error.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/error.h` & `createrepo_c-1.0.0/src/error.h`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     CRE_DB,     /*!<
         (5) A database error */
     CRE_BADARG, /*!<
         (6) At least one argument of function is bad or non complete */
     CRE_NOFILE, /*!<
         (7) File doesn't exist */
     CRE_NODIR, /*!<
-        (8) Directory doesn't exist (not a dir or path doesn't exists) */
+        (8) Directory doesn't exist (not a dir or path doesn't exist) */
     CRE_EXISTS, /*!<
         (9) File/Directory already exists */
     CRE_UNKNOWNCHECKSUMTYPE, /*!<
         (10) Unknown/Unsupported checksum type */
     CRE_UNKNOWNCOMPRESSION, /*!<
         (11) Unknown/Unsupported compression type */
     CRE_XMLPARSER, /*!<
@@ -94,14 +94,16 @@
         (32) Bad updateinfo.xml file */
     CRE_SIGPROCMASK, /*!<
         (33) Cannot change blocked signals */
     CRE_ZCK, /*!<
         (34) ZCK library related error */
     CRE_MODULEMD, /*!<
         (35) modulemd related error */
+    CRE_ZSTD, /*!<
+        (36) Zstd library related error */
     CRE_SENTINEL, /*!<
         (XX) Sentinel */
 } cr_Error;
 
 /** Converts cr_Error return code to error string.
  * @param rc        cr_Error return code
  * @return          Error string
```

### Comparing `createrepo_c-0.21.1/src/helpers.c` & `createrepo_c-1.0.0/src/helpers.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/helpers.h` & `createrepo_c-1.0.0/src/helpers.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/koji.c` & `createrepo_c-1.0.0/src/koji.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/koji.h` & `createrepo_c-1.0.0/src/koji.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/load_metadata.c` & `createrepo_c-1.0.0/src/load_metadata.c`

 * *Files 5% similar despite different names*

```diff
@@ -696,7 +696,35 @@
 
     ret = cr_metadata_load_xml(md, ml, err);
 
     cr_metadatalocation_free(ml);
 
     return ret;
 }
+
+gchar *
+cr_compress_groupfile(const char *groupfile, const char *dest_dir, cr_CompressionType compression)
+{
+    const char *compression_suffix = cr_compression_suffix(compression);
+    GError *tmp_err = NULL;
+    gchar *compressed_path;
+    cr_CompressionType old_type = cr_detect_compression(groupfile, &tmp_err);
+    if (tmp_err) {
+        compressed_path = g_strconcat(dest_dir, cr_get_filename(groupfile), compression_suffix, NULL);
+        g_debug("Unable to detect compression type of %s, using %s for groupfile.", groupfile, compressed_path);
+        g_clear_error(&tmp_err);
+    } else if (old_type == CR_CW_NO_COMPRESSION) {
+        compressed_path = g_strconcat(dest_dir, cr_get_filename(groupfile), compression_suffix, NULL);
+    } else {
+        // strip compression suffix
+        gchar *tmp_file = g_strndup(groupfile, strlen(groupfile) - strlen(cr_compression_suffix(old_type)));
+        compressed_path = g_strconcat(dest_dir, cr_get_filename(tmp_file), compression_suffix, NULL);
+        g_free(tmp_file);
+    }
+    if (cr_compress_file(groupfile, compressed_path, compression, NULL, 0, &tmp_err) != CRE_OK) {
+        g_critical("Cannot compress file: %s: %s", groupfile,
+                   (tmp_err ? tmp_err->message : "Unknown error"));
+        g_clear_error(&tmp_err);
+        exit(EXIT_FAILURE);
+    }
+    return compressed_path;
+}
```

### Comparing `createrepo_c-0.21.1/src/load_metadata.h` & `createrepo_c-1.0.0/src/load_metadata.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/locate_metadata.c` & `createrepo_c-1.0.0/src/locate_metadata.c`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         g_warning("%s: %s is not a directory", __func__, repopath);
         return ret;
     }
 
     // Create path to repomd.xml and check if it exists
     repomd = g_build_filename(repopath, "repodata", "repomd.xml", NULL);
     if (!g_file_test(repomd, G_FILE_TEST_EXISTS)) {
-        g_debug("%s: %s doesn't exists", __func__, repomd);
+        g_debug("%s: %s doesn't exist", __func__, repomd);
         return ret;
     }
 
     ret = cr_parse_repomd(repomd, repopath, ignore_sqlite);
 
     return ret;
 }
```

### Comparing `createrepo_c-0.21.1/src/locate_metadata.h` & `createrepo_c-1.0.0/src/locate_metadata.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/mergerepo_c.c` & `createrepo_c-1.0.0/src/mergerepo_c.c`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 #define DEFAULT_OUTPUTDIR               "merged_repo/"
 
 #include "mergerepo_c.h"
 
 struct CmdOptions _cmd_options = {
         .db_compression_type = DEFAULT_DB_COMPRESSION_TYPE,
-        .groupfile_compression_type = DEFAULT_GROUPFILE_COMPRESSION_TYPE,
+        .compression_type = DEFAULT_COMPRESSION_TYPE,
         .merge_method = MM_DEFAULT,
         .unique_md_filenames = TRUE,
         .simple_md_filenames = FALSE,
 
         .zck_compression = FALSE,
         .zck_dict_dir = NULL,
     };
@@ -277,19 +277,19 @@
     if (options->compress_type) {
 
         cr_CompressionType type;
         type = cr_compression_type(options->compress_type);
 
         if (type == CR_CW_UNKNOWN_COMPRESSION) {
             g_critical("Compression %s not available: Please choose from: "
-                       "gz or bz2 or xz", options->compress_type);
+                       "gz, bz2, xz or zstd", options->compress_type);
             ret = FALSE;
         } else {
             options->db_compression_type = type;
-            options->groupfile_compression_type = type;
+            options->compression_type = type;
         }
     }
 
     // Merge method
     if (options->merge_method_str) {
         if (options->koji) {
             g_warning("With -k/--koji argument merge method is ignored (--all is implicitly used).");
@@ -325,15 +325,15 @@
 
     if (options->blocked) {
         if (!options->koji) {
             g_critical("-b/--blocked cannot be used without -k/--koji argument");
             ret = FALSE;
         }
         if (!g_file_test(options->blocked, G_FILE_TEST_EXISTS)) {
-            g_critical("File %s doesn't exists", options->blocked);
+            g_critical("File %s doesn't exist", options->blocked);
             ret = FALSE;
         }
     }
 
     if (options->repo_prefix_search || options->repo_prefix_replace) {
         if (options->repo_prefix_search == NULL) {
             g_critical("--repo-prefix-replace must be used together with --repo-prefix-search");
@@ -952,36 +952,40 @@
             g_critical("Error reading zchunk other dict %s: %s",
                        oth_dict_file, tmp_err->message);
             g_clear_error(&tmp_err);
             exit(EXIT_FAILURE);
         }
     }
 
-    const char *groupfile_suffix = cr_compression_suffix(
-                                    cmd_options->groupfile_compression_type);
+    const char *compression_suffix = cr_compression_suffix(
+                                    cmd_options->compression_type);
 
     gchar *pri_xml_filename = g_strconcat(cmd_options->tmp_out_repo,
-                                          "/primary.xml.gz", NULL);
+                                          "/primary.xml",
+                                          compression_suffix, NULL);
     gchar *fil_xml_filename = g_strconcat(cmd_options->tmp_out_repo,
-                                          "/filelists.xml.gz", NULL);
+                                          "/filelists.xml",
+                                          compression_suffix, NULL);
     gchar *fex_xml_filename = NULL;
     if (cmd_options->filelists_ext)
         fex_xml_filename = g_strconcat(cmd_options->tmp_out_repo,
-                                       "/filelists-ext.xml.gz", NULL);
+                                       "/filelists-ext.xml",
+                                       compression_suffix, NULL);
     gchar *oth_xml_filename = g_strconcat(cmd_options->tmp_out_repo,
-                                          "/other.xml.gz", NULL);
+                                          "/other.xml",
+                                          compression_suffix, NULL);
 
     gchar *update_info_filename = NULL;
     if (!cmd_options->noupdateinfo)
         update_info_filename  = g_strconcat(cmd_options->tmp_out_repo,
                                             "/updateinfo.xml",
-                                            groupfile_suffix, NULL);
+                                            compression_suffix, NULL);
 
     pri_f = cr_xmlfile_sopen_primary(pri_xml_filename,
-                                     CR_CW_GZ_COMPRESSION,
+                                     cmd_options->compression_type,
                                      pri_stat,
                                      &tmp_err);
     if (tmp_err) {
         g_critical("Cannot open %s: %s", pri_xml_filename, tmp_err->message);
         cr_contentstat_free(pri_stat, NULL);
         cr_contentstat_free(fil_stat, NULL);
         cr_contentstat_free(fex_stat, NULL);
@@ -1001,15 +1005,15 @@
         g_free(fex_dict);
         g_free(oth_dict);
         cr_xmlfile_close(pri_f, NULL);
         return 0;
     }
 
     fil_f = cr_xmlfile_sopen_filelists(fil_xml_filename,
-                                       CR_CW_GZ_COMPRESSION,
+                                       cmd_options->compression_type,
                                        fil_stat,
                                        &tmp_err);
     if (tmp_err) {
         g_critical("Cannot open %s: %s", fil_xml_filename, tmp_err->message);
         cr_contentstat_free(pri_stat, NULL);
         cr_contentstat_free(fil_stat, NULL);
         cr_contentstat_free(fex_stat, NULL);
@@ -1030,15 +1034,15 @@
         g_free(fex_dict);
         g_free(oth_dict);
         return 0;
     }
 
     if (cmd_options->filelists_ext) {
         fex_f = cr_xmlfile_sopen_filelists(fex_xml_filename,
-                                           CR_CW_GZ_COMPRESSION,
+                                           cmd_options->compression_type,
                                            fex_stat,
                                            &tmp_err);
         if (tmp_err) {
             g_critical("Cannot open %s: %s", fil_xml_filename, tmp_err->message);
             cr_contentstat_free(pri_stat, NULL);
             cr_contentstat_free(fil_stat, NULL);
             cr_contentstat_free(fex_stat, NULL);
@@ -1060,15 +1064,15 @@
             g_free(fex_dict);
             g_free(oth_dict);
             return 0;
         }
     }
 
     oth_f = cr_xmlfile_sopen_other(oth_xml_filename,
-                                   CR_CW_GZ_COMPRESSION,
+                                   cmd_options->compression_type,
                                    oth_stat,
                                    &tmp_err);
     if (tmp_err) {
         g_critical("Cannot open %s: %s", oth_xml_filename, tmp_err->message);
         cr_contentstat_free(pri_stat, NULL);
         cr_contentstat_free(fil_stat, NULL);
         cr_contentstat_free(fex_stat, NULL);
@@ -1238,15 +1242,15 @@
     // Prepare sqlite if needed
 
     cr_SqliteDb *pri_db = NULL;
     cr_SqliteDb *fil_db = NULL;
     cr_SqliteDb *fex_db = NULL;
     cr_SqliteDb *oth_db = NULL;
 
-    if (!cmd_options->no_database) {
+    if (cmd_options->database) {
         gchar *pri_db_filename = NULL;
         gchar *fil_db_filename = NULL;
         gchar *fex_db_filename = NULL;
         gchar *oth_db_filename = NULL;
 
         pri_db_filename = g_strconcat(cmd_options->tmp_out_repo,
                                       "/primary.sqlite", NULL);
@@ -1325,15 +1329,15 @@
                 cr_xmlfile_add_chunk(pri_cr_zck, (const char *) res.primary, NULL);
                 cr_xmlfile_add_chunk(fil_cr_zck, (const char *) res.filelists, NULL);
                 if (cmd_options->filelists_ext)
                     cr_xmlfile_add_chunk(fex_cr_zck, (const char *) res.filelists_ext, NULL);
                 cr_xmlfile_add_chunk(oth_cr_zck, (const char *) res.other, NULL);
             }
 
-            if (!cmd_options->no_database) {
+            if (cmd_options->database) {
                 cr_db_add_pkg(pri_db, pkg, NULL);
                 cr_db_add_pkg(fil_db, pkg, NULL);
                 if (cmd_options->filelists_ext)
                     cr_db_add_pkg(fex_db, pkg, NULL);
                 cr_db_add_pkg(oth_db, pkg, NULL);
             }
 
@@ -1363,15 +1367,15 @@
 
     // Write updateinfo.xml
     // TODO
 
     if (!cmd_options->noupdateinfo) {
         CR_FILE *update_info = cr_open(update_info_filename,
                                        CR_CW_MODE_WRITE,
-                                       cmd_options->groupfile_compression_type,
+                                       cmd_options->compression_type,
                                        &tmp_err);
         if (update_info) {
             cr_puts(update_info,
                     "<?xml version=\"1.0\"?>\n<updates></updates>\n",
                     NULL);
             cr_close(update_info, NULL);
         } else {
@@ -1386,18 +1390,18 @@
 #ifdef WITH_LIBMODULEMD
     // Write modulemd
     g_autofree gchar *modulemd_filename = NULL;
 
     if (module_index) {
         gboolean ret;
         modulemd_filename =
-            g_strconcat(cmd_options->tmp_out_repo, "/modules.yaml.gz", NULL);
+            g_strconcat(cmd_options->tmp_out_repo, "/modules.yaml", compression_suffix, NULL);
         CR_FILE *modulemd = cr_open(modulemd_filename,
                                     CR_CW_MODE_WRITE,
-                                    CR_CW_GZ_COMPRESSION,
+                                    cmd_options->compression_type,
                                     &tmp_err);
         if (modulemd) {
             ret = modulemd_module_index_dump_to_custom(module_index,
                                                        modulemd_write_handler,
                                                        modulemd,
                                                        &tmp_err);
             if (!ret) {
@@ -1429,15 +1433,14 @@
     cr_RepomdRecord *fex_db_rec               = NULL;
     cr_RepomdRecord *oth_db_rec               = NULL;
     cr_RepomdRecord *pri_zck_rec              = NULL;
     cr_RepomdRecord *fil_zck_rec              = NULL;
     cr_RepomdRecord *fex_zck_rec              = NULL;
     cr_RepomdRecord *oth_zck_rec              = NULL;
     cr_RepomdRecord *groupfile_rec            = NULL;
-    cr_RepomdRecord *compressed_groupfile_rec = NULL;
     cr_RepomdRecord *groupfile_zck_rec        = NULL;
     cr_RepomdRecord *update_info_rec          = NULL;
     cr_RepomdRecord *update_info_zck_rec      = NULL;
     cr_RepomdRecord *pkgorigins_rec           = NULL;
     cr_RepomdRecord *pkgorigins_zck_rec       = NULL;
 
 #ifdef WITH_LIBMODULEMD
@@ -1513,21 +1516,19 @@
         }
     }
 #endif /* WITH_LIBMODULEMD */
 
     // Groupfile
 
     if (groupfile) {
-        groupfile_rec = cr_repomd_record_new("group", groupfile);
-        compressed_groupfile_rec = cr_repomd_record_new("group_gz", NULL);
-        cr_repomd_record_compress_and_fill(groupfile_rec,
-                                           compressed_groupfile_rec,
-                                           CR_CHECKSUM_SHA256,
-                                           cmd_options->groupfile_compression_type,
-                                           NULL, NULL);
+        gchar *compressed_path = cr_compress_groupfile(groupfile, cmd_options->tmp_out_repo, cmd_options->compression_type);
+        groupfile_rec = cr_repomd_record_new("group", compressed_path);
+        g_free(compressed_path);
+        cr_repomd_record_fill(groupfile_rec, CR_CHECKSUM_SHA256, NULL);
+
         if (cmd_options->zck_compression) {
             groupfile_zck_rec = cr_repomd_record_new("group_zck", NULL);
             cr_repomd_record_compress_and_fill(groupfile_rec,
                                                groupfile_zck_rec,
                                                CR_CHECKSUM_SHA256,
                                                CR_CW_ZCK_COMPRESSION,
                                                NULL, NULL);
@@ -1581,15 +1582,15 @@
       cr_repomdrecordfilltask_free(mmd_fill_task, NULL);
     }
 #endif
 
 
     // Sqlite db
 
-    if (!cmd_options->no_database) {
+    if (cmd_options->database) {
         const char *db_suffix = cr_compression_suffix(cmd_options->db_compression_type);
 
         // Insert XML checksums into the dbs
         cr_db_dbinfo_update(pri_db, pri_xml_rec->checksum, NULL);
         cr_db_dbinfo_update(fil_db, fil_xml_rec->checksum, NULL);
         if (cmd_options->filelists_ext)
             cr_db_dbinfo_update(fex_db, fil_xml_rec->checksum, NULL);
@@ -1803,15 +1804,14 @@
         cr_repomd_record_rename_file(oth_db_rec, NULL);
         cr_repomd_record_rename_file(pri_zck_rec, NULL);
         cr_repomd_record_rename_file(fil_zck_rec, NULL);
         if (cmd_options->filelists_ext)
             cr_repomd_record_rename_file(fex_zck_rec, NULL);
         cr_repomd_record_rename_file(oth_zck_rec, NULL);
         cr_repomd_record_rename_file(groupfile_rec, NULL);
-        cr_repomd_record_rename_file(compressed_groupfile_rec, NULL);
         cr_repomd_record_rename_file(groupfile_zck_rec, NULL);
         cr_repomd_record_rename_file(update_info_rec, NULL);
         cr_repomd_record_rename_file(update_info_zck_rec, NULL);
         cr_repomd_record_rename_file(pkgorigins_rec, NULL);
         cr_repomd_record_rename_file(pkgorigins_zck_rec, NULL);
 
 #ifdef WITH_LIBMODULEMD
@@ -1836,15 +1836,14 @@
     cr_repomd_set_record(repomd_obj, oth_db_rec);
     cr_repomd_set_record(repomd_obj, pri_zck_rec);
     cr_repomd_set_record(repomd_obj, fil_zck_rec);
     if (cmd_options->filelists_ext)
         cr_repomd_set_record(repomd_obj, fex_zck_rec);
     cr_repomd_set_record(repomd_obj, oth_zck_rec);
     cr_repomd_set_record(repomd_obj, groupfile_rec);
-    cr_repomd_set_record(repomd_obj, compressed_groupfile_rec);
     cr_repomd_set_record(repomd_obj, groupfile_zck_rec);
     cr_repomd_set_record(repomd_obj, update_info_rec);
     cr_repomd_set_record(repomd_obj, update_info_zck_rec);
     cr_repomd_set_record(repomd_obj, pkgorigins_rec);
     cr_repomd_set_record(repomd_obj, pkgorigins_zck_rec);
 
 #ifdef WITH_LIBMODULEMD
@@ -2046,41 +2045,23 @@
             struct cr_MetadataLocation *loc;
             loc = (struct cr_MetadataLocation  *) element->data;
             if (!groupfile){
                 if (loc->additional_metadata){
                     GSList *loc_groupfile = (g_slist_find_custom(loc->additional_metadata, "group", cr_cmp_metadatum_type));
                     if (loc_groupfile) {
                         cr_Metadatum *g = loc_groupfile->data;
-                        if (cr_copy_file(g->name, cmd_options->tmp_out_repo, &tmp_err)) {
-                            groupfile = g_strconcat(cmd_options->tmp_out_repo,
-                                    cr_get_filename(g->name),
-                                    NULL);
-                            g_debug("Using groupfile: %s", groupfile);
-                            break;
-                      } else {
-                            g_warning("Groupfile %s from repo: %s cannot be used: %s\n",
-                                    g->name, loc->original_url, tmp_err->message);
-                            g_clear_error(&tmp_err);
-                        }
+                        groupfile = g_strdup(g->name);
+                        break;
                     }
                 }
             }
         }
     } else {
         // Use groupfile specified by user
-        if (cr_copy_file(cmd_options->groupfile, cmd_options->tmp_out_repo, &tmp_err)) {
-            groupfile = g_strconcat(cmd_options->tmp_out_repo,
-                                    cr_get_filename(cmd_options->groupfile),
-                                    NULL);
-            g_debug("Using user specified groupfile: %s", groupfile);
-        } else {
-            g_critical("Cannot copy groupfile %s: %s",
-                       cmd_options->groupfile, tmp_err->message);
-            return 1;
-        }
+        groupfile = g_strdup(cmd_options->groupfile);
     }
 
     // Load noarch repo
 
     cr_Metadata *noarch_metadata = NULL;
     // cr_metadata_hashtable(noarch_metadata):
     //   Key: CR_HT_KEY_FILENAME aka pkg->location_href
```

### Comparing `createrepo_c-0.21.1/src/mergerepo_c.h` & `createrepo_c-1.0.0/src/mergerepo_c.h`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 #include "compression_wrapper.h"
 
 #define DEFAULT_DB_COMPRESSION_TYPE             CR_CW_BZ2_COMPRESSION
-#define DEFAULT_GROUPFILE_COMPRESSION_TYPE      CR_CW_GZ_COMPRESSION
+#define DEFAULT_COMPRESSION_TYPE                CR_CW_ZSTD_COMPRESSION
 
 typedef enum {
     MM_DEFAULT,
     // NA == Name, Arch
     MM_FIRST_FROM_IDENTICAL_NA = MM_DEFAULT,
     MM_NEWEST_FROM_IDENTICAL_NA,
     MM_WITH_HIGHEST_NEVRA,
@@ -79,15 +79,15 @@
 
     char *out_dir;
     char *out_repo;
     char *tmp_out_repo;
     GSList *repo_list;
     GSList *arch_list;
     cr_CompressionType db_compression_type;
-    cr_CompressionType groupfile_compression_type;
+    cr_CompressionType compression_type;
     MergeMethod merge_method;
 };
 
 #ifdef __cplusplus
 }
 #endif
```

### Comparing `createrepo_c-0.21.1/src/metadata_internal.h` & `createrepo_c-1.0.0/src/metadata_internal.h`

 * *Files 16% similar despite different names*

```diff
@@ -42,14 +42,25 @@
  * @return              cr_Error code
  */
 int
 cr_metadata_load_modulemd(ModulemdModuleIndex **moduleindex,
                           gchar *path_to_md,
                           GError **err);
 
+/** Compress groupfile into dest_dir with specified compression.
+ * @param groupfile     Path to local groupfile, it can be already compressed by
+ *                      some compression.
+ * @param dest_dir      Path to directory where the compressed groupfile should be stored.
+ * @return              Path to the new compressed groupfile. Has to be freed by the caller.
+ */
+gchar *
+cr_compress_groupfile(const char *groupfile,
+                      const char *dest_dir,
+                      cr_CompressionType compression);
+
 
 #endif /* WITH_LIBMODULEMD */
 
 #ifdef __cplusplus
 }
 #endif
```

### Comparing `createrepo_c-0.21.1/src/misc.c` & `createrepo_c-1.0.0/src/misc.c`

 * *Files 4% similar despite different names*

```diff
@@ -236,47 +236,58 @@
         return 1;
     }
 
     return 0;
 }
 */
 
-#define VAL_LEN         4       // Len of numeric values in rpm
+#define VAL_LEN         4       // Len of numeric values in rpm (bytes)
 
 struct cr_HeaderRangeStruct
 cr_get_header_byte_range(const char *filename, GError **err)
 {
-    /* Values readed by fread are 4 bytes long and stored as big-endian.
-     * So there is htonl function to convert this big-endian number into host
-     * byte order.
-     */
-
+    // Lead is 96 bytes.
+    //
+    // Each Header starts like this (16 bytes)
+    // 3 bytes for the magic
+    // 1 byte RPM version number - always 1
+    // 4 reserved bytes (no meaning, just padding)
+    // 4 bytes for the number of entries in the index (u32)
+    // 4 bytes for the length of the data section (u32)
+    //
+    // Next comes a series of index entries. Each index entry is 16 bytes
+    // 4 bytes for the tag (u32)
+    // 4 bytes for the tag data type (u32)
+    // 4 bytes for the offset relative to the beginning of the data store
+    // 4 bytes for the count that contains the number of data items pointed to by the index entry
+    //
+    // After the header entries comes the data section. This stores the data pointed to by
+    // the offsets within each index entry.
+    //
+    // All numeric values are big-endian and need to be converted into host byte order.
     struct cr_HeaderRangeStruct results;
 
     assert(!err || *err == NULL);
 
     results.start = 0;
     results.end   = 0;
 
-
     // Open file
-
     FILE *fp = fopen(filename, "rb");
     if (!fp) {
         const gchar * fopen_error = g_strerror(errno);
         g_debug("%s: Cannot open file %s (%s)", __func__, filename,
                 fopen_error);
         g_set_error(err, ERR_DOMAIN, CRE_IO,
                     "Cannot open %s: %s", filename, fopen_error);
         return results;
     }
 
-
     // Get header range
-
+    // Seek to Lead (96) + 8 bytes and read the number of entries in the signature header, then convert to host byte order
     if (fseek(fp, 104, SEEK_SET) != 0) {
         const gchar * fseek_error = g_strerror(errno);
         g_debug("%s: fseek fail on %s (%s)", __func__, filename, fseek_error);
         g_set_error(err, ERR_DOMAIN, CRE_IO,
                     "Cannot seek over %s: %s", filename, fseek_error);
         fclose(fp);
         return results;
@@ -287,58 +298,61 @@
     if (fread(&sigindex, VAL_LEN, 1, fp) != 1) {
         g_set_error(err, ERR_DOMAIN, CRE_IO,
                     "fread() error on %s: %s", filename, g_strerror(errno));
         fclose(fp);
         return results;
     }
     sigindex = htonl(sigindex);
+    // Read the length of the data section and convert to host byte order
     if (fread(&sigdata, VAL_LEN, 1, fp) != 1) {
         g_set_error(err, ERR_DOMAIN, CRE_IO,
                     "fread() error on %s: %s", filename, g_strerror(errno));
         fclose(fp);
         return results;
     }
     sigdata = htonl(sigdata);
 
+    // Lead (96) + HeaderIndex (16) = 112. Index entries are 16 bytes each. Include padding to align to 8 bytes
     unsigned int sigindexsize = sigindex * 16;
     unsigned int sigsize = sigdata + sigindexsize;
     unsigned int disttoboundary = sigsize % 8;
     if (disttoboundary) {
         disttoboundary = 8 - disttoboundary;
     }
     unsigned int hdrstart = 112 + sigsize + disttoboundary;
 
+    // Seek to start of header (96) + 8 bytes and read the number of entries in the header, then convert to host byte order
     fseek(fp, hdrstart, SEEK_SET);
     fseek(fp, 8, SEEK_CUR);
 
     unsigned int hdrindex = 0;
     unsigned int hdrdata  = 0;
     if (fread(&hdrindex, VAL_LEN, 1, fp) != 1) {
         g_set_error(err, ERR_DOMAIN, CRE_IO,
                     "fread() error on %s: %s", filename, g_strerror(errno));
         fclose(fp);
         return results;
     }
     hdrindex = htonl(hdrindex);
+    // Read the length of the data section and convert to host byte order
     if (fread(&hdrdata, VAL_LEN, 1, fp) != 1) {
         g_set_error(err, ERR_DOMAIN, CRE_IO,
                     "fread() error on %s: %s", filename, g_strerror(errno));
         fclose(fp);
         return results;
     }
     hdrdata = htonl(hdrdata);
+    // Calculate the end of the header
     unsigned int hdrindexsize = hdrindex * 16;
     unsigned int hdrsize = hdrdata + hdrindexsize + 16;
     unsigned int hdrend = hdrstart + hdrsize;
 
     fclose(fp);
 
-
     // Check sanity
-
     if (hdrend < hdrstart) {
         g_debug("%s: sanity check fail on %s (%d > %d))", __func__,
                 filename, hdrstart, hdrend);
         g_set_error(err, ERR_DOMAIN, CRE_ERROR,
                     "sanity check error on %s (hdrstart: %d > hdrend: %d)",
                     filename, hdrstart, hdrend);
         return results;
```

### Comparing `createrepo_c-0.21.1/src/misc.h` & `createrepo_c-1.0.0/src/misc.h`

 * *Files 0% similar despite different names*

```diff
@@ -543,15 +543,15 @@
  */
 void
 cr_nevra_free(cr_NEVRA *nevra);
 
 /** Are the files identical?
  * Different paths could point to the same file.
  * This functions checks if both paths point to the same file or not.
- * If one of the files doesn't exists, the funcion doesn't fail
+ * If one of the files doesn't exist, the funcion doesn't fail
  * and just put FALSE into "indentical" value and returns.
  * @param fn1           First path
  * @param fn2           Second path
  * @param identical     Are the files same or not
  * @param err           GError **
  * @return              FALSE if an error was encountered, TRUE otherwise
  */
```

### Comparing `createrepo_c-0.21.1/src/modifyrepo_c.c` & `createrepo_c-1.0.0/src/modifyrepo_c.c`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
     if (options->remove)
         g_debug("Preparing remove-task for: %s", options->remove);
     else
         g_debug("Preparing task for: %s", metadatapath);
 
     if (metadatapath && !g_file_test(metadatapath, G_FILE_TEST_IS_REGULAR)) {
         g_set_error(err, ERR_DOMAIN, CRE_ERROR,
-                    "File \"%s\" is not regular file or doesn't exists",
+                    "File \"%s\" is not regular file or doesn't exist",
                     metadatapath);
         return FALSE;
     }
 
     if (options->remove)
         metadatapath = options->remove;
```

### Comparing `createrepo_c-0.21.1/src/modifyrepo_shared.c` & `createrepo_c-1.0.0/src/modifyrepo_shared.c`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #include "checksum.h"
 #include "modifyrepo_shared.h"
 #include "compression_wrapper.h"
 #include "threads.h"
 #include "xml_dump.h"
 
 #define ERR_DOMAIN              CREATEREPO_C_ERROR
-#define DEFAULT_COMPRESSION     CR_CW_GZ_COMPRESSION
+#define DEFAULT_COMPRESSION     CR_CW_ZSTD_COMPRESSION
 #define DEFAULT_CHECKSUM        CR_CHECKSUM_SHA256
 
 cr_ModifyRepoTask *
 cr_modifyrepotask_new(void)
 {
     cr_ModifyRepoTask *task = g_new0(cr_ModifyRepoTask, 1);
     task->chunk = g_string_chunk_new(16);
@@ -140,15 +140,15 @@
     }
 
     // Parse repomd.xml
 
     gchar *repomd_path = g_build_filename(repopath, "repomd.xml", NULL);
     if (!g_file_test(repomd_path, G_FILE_TEST_IS_REGULAR)) {
         g_set_error(err, ERR_DOMAIN, CRE_IO,
-                    "Regular file \"%s\" doesn't exists", repomd_path);
+                    "Regular file \"%s\" doesn't exist", repomd_path);
         g_free(repomd_path);
         return FALSE;
     }
 
     cr_Repomd *repomd = cr_repomd_new();
     int rc = cr_xml_parse_repomd(repomd_path, repomd, cr_warning_cb,
                                   "Repomd XML parser", err);
@@ -237,15 +237,15 @@
                     g_debug("%s: New name cannot be empty", __func__);
                     cr_repomd_free(repomd);
                     g_free(repomd_path);
                     return FALSE;
                 }
             }
 
-            // Check if record with this name doesn't exists yet
+            // Check if record with this name doesn't exist yet
             if (cr_repomd_get_record(repomd, task->type))
                 g_warning("Record with type \"%s\" already exists "
                           "in repomd.xml", task->type);
 
         }
     }
```

### Comparing `createrepo_c-0.21.1/src/modifyrepo_shared.h` & `createrepo_c-1.0.0/src/modifyrepo_shared.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/package.c` & `createrepo_c-1.0.0/src/package.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/package.h` & `createrepo_c-1.0.0/src/package.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/package_internal.h` & `createrepo_c-1.0.0/src/package_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/parsehdr.c` & `createrepo_c-1.0.0/src/parsehdr.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/parsehdr.h` & `createrepo_c-1.0.0/src/parsehdr.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/parsepkg.c` & `createrepo_c-1.0.0/src/parsepkg.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/parsepkg.h` & `createrepo_c-1.0.0/src/parsepkg.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/CMakeLists.txt` & `createrepo_c-1.0.0/src/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/checksum-py.c` & `createrepo_c-1.0.0/src/python/checksum-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/checksum-py.h` & `createrepo_c-1.0.0/src/python/checksum-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/compression_wrapper-py.c` & `createrepo_c-1.0.0/src/python/compression_wrapper-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/compression_wrapper-py.h` & `createrepo_c-1.0.0/src/python/compression_wrapper-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/contentstat-py.c` & `createrepo_c-1.0.0/src/python/contentstat-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/contentstat-py.h` & `createrepo_c-1.0.0/src/python/contentstat-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/createrepo_c/__init__.py` & `createrepo_c-1.0.0/src/python/createrepo_c/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 
 #: XZ compression alias
 XZ                      = _createrepo_c.XZ_COMPRESSION
 
 #: Zchunk compression alias
 ZCK                     = _createrepo_c.ZCK_COMPRESSION
 
+#: Zstd compression alias
+ZSTD                     = _createrepo_c.ZSTD_COMPRESSION
+
 HT_KEY_DEFAULT  = _createrepo_c.HT_KEY_DEFAULT  #: Default key (hash)
 HT_KEY_HASH     = _createrepo_c.HT_KEY_HASH     #: Package hash as a key
 HT_KEY_NAME     = _createrepo_c.HT_KEY_NAME     #: Package name as a key
 HT_KEY_FILENAME = _createrepo_c.HT_KEY_FILENAME #: Package filename as a key
 
 HT_DUPACT_KEEPFIRST = _createrepo_c.HT_DUPACT_KEEPFIRST #: If an key is duplicated, keep only the first occurrence
 HT_DUPACT_REMOVEALL = _createrepo_c.HT_DUPACT_REMOVEALL #: If an key is duplicated, discard all occurrences
@@ -103,14 +106,15 @@
 PCOR_ENTRY_PRE     = 5 #: PCOR entry tuple index - pre
 
 
 # Tuple indexes for file entry
 FILE_ENTRY_TYPE = 0 #: File entry tuple index - file type
 FILE_ENTRY_PATH = 1 #: File entry tuple index - path
 FILE_ENTRY_NAME = 2 #: File entry tuple index - file name
+FILE_ENTRY_DIGEST = 3 #: File entry tuple index - file digest, present only in filelists-ext
 
 # Tuple indexes for changelog entry
 CHANGELOG_ENTRY_AUTHOR    = 0 #: Changelog entry tuple index - Author
 CHANGELOG_ENTRY_DATE      = 1 #: Changelog entry tuple index - Date
 CHANGELOG_ENTRY_CHANGELOG = 2 #: Changelog entry tuple index - Changelog
```

### Comparing `createrepo_c-0.21.1/src/python/createrepo_c.egg-info/PKG-INFO` & `createrepo_c-1.0.0/src/python/createrepo_c.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: createrepo-c
-Version: 0.21.1
+Version: 1.0.0
 Summary: C implementation of createrepo
 Home-page: https://github.com/rpm-software-management
 Author: RPM Software Management
 Author-email: rpm-ecosystem@lists.rpm.org
 License: GPLv2+
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `createrepo_c-0.21.1/src/python/createrepo_c.egg-info/SOURCES.txt` & `createrepo_c-1.0.0/src/python/createrepo_c.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -316,29 +316,33 @@
 tests/python/tests/test_xml_file.py
 tests/python/tests/test_xml_parser.py
 tests/testdata/compressed_files/00_plain.foo0
 tests/testdata/compressed_files/00_plain.foo1
 tests/testdata/compressed_files/00_plain.foo2
 tests/testdata/compressed_files/00_plain.foo3
 tests/testdata/compressed_files/00_plain.foo4
+tests/testdata/compressed_files/00_plain.foo5
 tests/testdata/compressed_files/00_plain.txt
 tests/testdata/compressed_files/00_plain.txt.bz2
 tests/testdata/compressed_files/00_plain.txt.gz
 tests/testdata/compressed_files/00_plain.txt.xz
 tests/testdata/compressed_files/00_plain.txt.zck
+tests/testdata/compressed_files/00_plain.txt.zst
 tests/testdata/compressed_files/01_plain.foo0
 tests/testdata/compressed_files/01_plain.foo1
 tests/testdata/compressed_files/01_plain.foo2
 tests/testdata/compressed_files/01_plain.foo3
 tests/testdata/compressed_files/01_plain.foo4
+tests/testdata/compressed_files/01_plain.foo5
 tests/testdata/compressed_files/01_plain.txt
 tests/testdata/compressed_files/01_plain.txt.bz2
 tests/testdata/compressed_files/01_plain.txt.gz
 tests/testdata/compressed_files/01_plain.txt.xz
 tests/testdata/compressed_files/01_plain.txt.zck
+tests/testdata/compressed_files/01_plain.txt.zst
 tests/testdata/comps_files/comps_00.xml
 tests/testdata/modified_repo_files/bad_file_type-filelists.xml
 tests/testdata/modified_repo_files/error_00-filelists.xml
 tests/testdata/modified_repo_files/error_00-other.xml
 tests/testdata/modified_repo_files/error_00-primary.xml
 tests/testdata/modified_repo_files/long_primary.xml
 tests/testdata/modified_repo_files/missing_type-repomd.xml
```

### Comparing `createrepo_c-0.21.1/src/python/createrepo_cmodule.c` & `createrepo_c-1.0.0/src/python/createrepo_cmodule.c`

 * *Files 1% similar despite different names*

```diff
@@ -262,14 +262,15 @@
     PyModule_AddIntConstant(m, "AUTO_DETECT_COMPRESSION", CR_CW_AUTO_DETECT_COMPRESSION);
     PyModule_AddIntConstant(m, "UNKNOWN_COMPRESSION", CR_CW_UNKNOWN_COMPRESSION);
     PyModule_AddIntConstant(m, "NO_COMPRESSION", CR_CW_NO_COMPRESSION);
     PyModule_AddIntConstant(m, "GZ_COMPRESSION", CR_CW_GZ_COMPRESSION);
     PyModule_AddIntConstant(m, "BZ2_COMPRESSION", CR_CW_BZ2_COMPRESSION);
     PyModule_AddIntConstant(m, "XZ_COMPRESSION", CR_CW_XZ_COMPRESSION);
     PyModule_AddIntConstant(m, "ZCK_COMPRESSION", CR_CW_ZCK_COMPRESSION);
+    PyModule_AddIntConstant(m, "ZSTD_COMPRESSION", CR_CW_ZSTD_COMPRESSION);
 
     /* Zchunk support */
 #ifdef WITH_ZCHUNK
     PyModule_AddIntConstant(m, "HAS_ZCK", 1);
 #else
     PyModule_AddIntConstant(m, "HAS_ZCK", 0);
 #endif // WITH_ZCHUNK
```

### Comparing `createrepo_c-0.21.1/src/python/exception-py.c` & `createrepo_c-1.0.0/src/python/exception-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/exception-py.h` & `createrepo_c-1.0.0/src/python/exception-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/load_metadata-py.c` & `createrepo_c-1.0.0/src/python/load_metadata-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/load_metadata-py.h` & `createrepo_c-1.0.0/src/python/load_metadata-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/locate_metadata-py.c` & `createrepo_c-1.0.0/src/python/locate_metadata-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/locate_metadata-py.h` & `createrepo_c-1.0.0/src/python/locate_metadata-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/misc-py.c` & `createrepo_c-1.0.0/src/python/misc-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/misc-py.h` & `createrepo_c-1.0.0/src/python/misc-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/package-py.c` & `createrepo_c-1.0.0/src/python/package-py.c`

 * *Files 1% similar despite different names*

```diff
@@ -427,16 +427,17 @@
     }
     return 0;
 }
 
 static int
 CheckPyPackageFile(PyObject *dep)
 {
-    if (!PyTuple_Check(dep) || PyTuple_Size(dep) != 4) {
-        PyErr_SetString(PyExc_TypeError, "Element of list has to be a tuple with 4 items.");
+    // The fourth element (file checksum) is optional since it is present only in filelists-ext
+    if (!PyTuple_Check(dep) || (PyTuple_Size(dep) != 4 && PyTuple_Size(dep) != 3)) {
+        PyErr_SetString(PyExc_TypeError, "Element of list has to be a tuple with 3 or 4 items.");
         return 1;
     }
     return 0;
 }
 
 static int
 CheckPyChangelogEntry(PyObject *dep)
```

### Comparing `createrepo_c-0.21.1/src/python/package-py.h` & `createrepo_c-1.0.0/src/python/package-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/parsepkg-py.c` & `createrepo_c-1.0.0/src/python/parsepkg-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/parsepkg-py.h` & `createrepo_c-1.0.0/src/python/parsepkg-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/repomd-py.c` & `createrepo_c-1.0.0/src/python/repomd-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/repomd-py.h` & `createrepo_c-1.0.0/src/python/repomd-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/repomdrecord-py.c` & `createrepo_c-1.0.0/src/python/repomdrecord-py.c`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 {
     if (check_RepomdRecordStatus(self))
         return NULL;
     return Object_FromRepomdRecord(cr_repomd_record_copy(self->record));
 }
 
 PyDoc_STRVAR(fill__doc__,
-"fill() -> None\n\n"
+"fill(checksum_type) -> None\n\n"
 "Fill unfilled items in the RepomdRecord (sizes and checksums)");
 
 static PyObject *
 fill(_RepomdRecordObject *self, PyObject *args)
 {
     int checksum_type;
     GError *err = NULL;
```

### Comparing `createrepo_c-0.21.1/src/python/repomdrecord-py.h` & `createrepo_c-1.0.0/src/python/repomdrecord-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/sqlite-py.c` & `createrepo_c-1.0.0/src/python/sqlite-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/sqlite-py.h` & `createrepo_c-1.0.0/src/python/sqlite-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/typeconversion.c` & `createrepo_c-1.0.0/src/python/typeconversion.c`

 * *Files 2% similar despite different names*

```diff
@@ -165,21 +165,26 @@
 }
 
 PyObject *
 PyObject_FromPackageFile(cr_PackageFile *file)
 {
     PyObject *tuple;
 
-    if ((tuple = PyTuple_New(4)) == NULL)
-        return NULL;
+    if (file->digest != NULL) {
+        if ((tuple = PyTuple_New(4)) == NULL)
+            return NULL;
+        PyTuple_SetItem(tuple, 3, PyUnicodeOrNone_FromString(file->digest));
+    } else {
+        if ((tuple = PyTuple_New(3)) == NULL)
+            return NULL;
+    }
 
     PyTuple_SetItem(tuple, 0, PyUnicodeOrNone_FromString(file->type));
     PyTuple_SetItem(tuple, 1, PyUnicodeOrNone_FromString(file->path));
     PyTuple_SetItem(tuple, 2, PyUnicodeOrNone_FromString(file->name));
-    PyTuple_SetItem(tuple, 3, PyUnicodeOrNone_FromString(file->digest));
 
     return tuple;
 }
 
 cr_PackageFile *
 PyObject_ToPackageFile(PyObject *tuple, GStringChunk *chunk)
 {
```

### Comparing `createrepo_c-0.21.1/src/python/typeconversion.h` & `createrepo_c-1.0.0/src/python/typeconversion.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/updatecollection-py.c` & `createrepo_c-1.0.0/src/python/updatecollection-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/updatecollection-py.h` & `createrepo_c-1.0.0/src/python/updatecollection-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/updatecollectionmodule-py.c` & `createrepo_c-1.0.0/src/python/updatecollectionmodule-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/updatecollectionmodule-py.h` & `createrepo_c-1.0.0/src/python/updatecollectionmodule-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/updatecollectionpackage-py.c` & `createrepo_c-1.0.0/src/python/updatecollectionpackage-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/updatecollectionpackage-py.h` & `createrepo_c-1.0.0/src/python/updatecollectionpackage-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/updateinfo-py.c` & `createrepo_c-1.0.0/src/python/updateinfo-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/updateinfo-py.h` & `createrepo_c-1.0.0/src/python/updateinfo-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/updaterecord-py.c` & `createrepo_c-1.0.0/src/python/updaterecord-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/updaterecord-py.h` & `createrepo_c-1.0.0/src/python/updaterecord-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/updatereference-py.c` & `createrepo_c-1.0.0/src/python/updatereference-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/updatereference-py.h` & `createrepo_c-1.0.0/src/python/updatereference-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/xml_dump-py.c` & `createrepo_c-1.0.0/src/python/xml_dump-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/xml_dump-py.h` & `createrepo_c-1.0.0/src/python/xml_dump-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/xml_file-py.c` & `createrepo_c-1.0.0/src/python/xml_file-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/xml_file-py.h` & `createrepo_c-1.0.0/src/python/xml_file-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/xml_parser-py.c` & `createrepo_c-1.0.0/src/python/xml_parser-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/python/xml_parser-py.h` & `createrepo_c-1.0.0/src/python/xml_parser-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/repomd.c` & `createrepo_c-1.0.0/src/repomd.c`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     GError *tmp_err = NULL;
 
     assert(filename);
     assert(!err || *err == NULL);
 
     if (!g_file_test(filename, G_FILE_TEST_IS_REGULAR)) {
         g_set_error(err, ERR_DOMAIN, CRE_NOFILE,
-                    "File %s doesn't exists or not a regular file", filename);
+                    "File %s doesn't exist or not a regular file", filename);
         return NULL;
     }
 
 
     // Open compressed file
     cr_ContentStat *read_stat = g_malloc0(sizeof(cr_ContentStat));
 
@@ -227,18 +227,18 @@
 
     path = md->location_real;
 
     checksum_str = cr_checksum_name_str(checksum_type);
     checksum_t = checksum_type;
 
     if (!g_file_test(path, G_FILE_TEST_IS_REGULAR)) {
-        // File doesn't exists
-        g_warning("%s: File %s doesn't exists", __func__, path);
+        // File doesn't exist
+        g_warning("%s: File %s doesn't exist", __func__, path);
         g_set_error(err, ERR_DOMAIN, CRE_NOFILE,
-                    "File %s doesn't exists or not a regular file", path);
+                    "File %s doesn't exist or not a regular file", path);
         return CRE_NOFILE;
     }
 
     // Compute checksum of compressed file
 
     if (!md->checksum_type || !md->checksum) {
         gchar *chksum;
@@ -366,18 +366,18 @@
     if (!(record->location_real) || !strlen(record->location_real)) {
         g_set_error(err, ERR_DOMAIN, CRE_BADARG,
                     "Empty locations in repomd record object");
         return CRE_BADARG;
     }
 
     if (!g_file_test(record->location_real, G_FILE_TEST_IS_REGULAR)) {
-        // File doesn't exists
-        g_warning("%s: File %s doesn't exists", __func__, record->location_real);
+        // File doesn't exist
+        g_warning("%s: File %s doesn't exist", __func__, record->location_real);
         g_set_error(err, ERR_DOMAIN, CRE_NOFILE,
-                    "File %s doesn't exists or not a regular file",
+                    "File %s doesn't exist or not a regular file",
                     record->location_real);
         return CRE_NOFILE;;
     }
 
     // Paths
 
     suffix = cr_compression_suffix(record_compression);
```

### Comparing `createrepo_c-0.21.1/src/repomd.h` & `createrepo_c-1.0.0/src/repomd.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/repomd_internal.h` & `createrepo_c-1.0.0/src/repomd_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/sqlite.c` & `createrepo_c-1.0.0/src/sqlite.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/sqlite.h` & `createrepo_c-1.0.0/src/sqlite.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/sqliterepo_c.c` & `createrepo_c-1.0.0/src/sqliterepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/threads.c` & `createrepo_c-1.0.0/src/threads.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/threads.h` & `createrepo_c-1.0.0/src/threads.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/updateinfo.c` & `createrepo_c-1.0.0/src/updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/updateinfo.h` & `createrepo_c-1.0.0/src/updateinfo.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/version.h.in` & `createrepo_c-1.0.0/src/version.h.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_dump.c` & `createrepo_c-1.0.0/src/xml_dump.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_dump.h` & `createrepo_c-1.0.0/src/xml_dump.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_dump_deltapackage.c` & `createrepo_c-1.0.0/src/xml_dump_deltapackage.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_dump_filelists.c` & `createrepo_c-1.0.0/src/xml_dump_filelists.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_dump_internal.h` & `createrepo_c-1.0.0/src/xml_dump_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_dump_other.c` & `createrepo_c-1.0.0/src/xml_dump_other.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_dump_primary.c` & `createrepo_c-1.0.0/src/xml_dump_primary.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_dump_repomd.c` & `createrepo_c-1.0.0/src/xml_dump_repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_dump_updateinfo.c` & `createrepo_c-1.0.0/src/xml_dump_updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_file.c` & `createrepo_c-1.0.0/src/xml_file.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_file.h` & `createrepo_c-1.0.0/src/xml_file.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_parser.c` & `createrepo_c-1.0.0/src/xml_parser.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_parser.h` & `createrepo_c-1.0.0/src/xml_parser.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_parser_filelists.c` & `createrepo_c-1.0.0/src/xml_parser_filelists.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_parser_internal.h` & `createrepo_c-1.0.0/src/xml_parser_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_parser_main_metadata_together.c` & `createrepo_c-1.0.0/src/xml_parser_main_metadata_together.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_parser_other.c` & `createrepo_c-1.0.0/src/xml_parser_other.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_parser_primary.c` & `createrepo_c-1.0.0/src/xml_parser_primary.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_parser_repomd.c` & `createrepo_c-1.0.0/src/xml_parser_repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/src/xml_parser_updateinfo.c` & `createrepo_c-1.0.0/src/xml_parser_updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/CMakeLists.txt` & `createrepo_c-1.0.0/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/CMakeLists.txt` & `createrepo_c-1.0.0/tests/createrepo/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 TARGET_LINK_LIBRARIES(libcreaterepo_c ${LZMA_LIBRARIES})
 TARGET_LINK_LIBRARIES(libcreaterepo_c ${OPENSSL_LIBRARIES})
 TARGET_LINK_LIBRARIES(libcreaterepo_c ${RPM_LIBRARIES})
 TARGET_LINK_LIBRARIES(libcreaterepo_c ${SQLITE3_LIBRARIES})
 TARGET_LINK_LIBRARIES(libcreaterepo_c ${ZLIB_LIBRARY})
 TARGET_LINK_LIBRARIES(libcreaterepo_c ${ZCK_LIBRARIES})
 TARGET_LINK_LIBRARIES(libcreaterepo_c ${DRPM_LIBRARIES})
+TARGET_LINK_LIBRARIES(libcreaterepo_c ${ZSTD_LIBRARIES})
 
 SET_TARGET_PROPERTIES(libcreaterepo_c PROPERTIES
                       OUTPUT_NAME "createrepo_c"
                       SOVERSION ${CR_MAJOR}
                       VERSION "${VERSION}"
                       COMPILE_DEFINITIONS "G_LOG_DOMAIN=\"${G_LOG_DOMAIN}\"")
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/checksum.c` & `createrepo_c-1.0.0/tests/createrepo/checksum.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/checksum.h` & `createrepo_c-1.0.0/tests/createrepo/checksum.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/cleanup.h` & `createrepo_c-1.0.0/tests/createrepo/cleanup.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/cmd_parser.c` & `createrepo_c-1.0.0/tests/createrepo/cmd_parser.c`

 * *Files 1% similar despite different names*

```diff
@@ -69,17 +69,17 @@
 
         .keep_all_metadata          = TRUE,
         .nevra_duplicates           = CR_ARG_DUP_NEVRA_KEEP_ALL,
     };
 
 
 gboolean
-duplicated_nevra_option_parser(const gchar *,
+duplicated_nevra_option_parser(const gchar *option_name,
                                const gchar *value,
-                               gpointer,
+                               gpointer data,
                                GError **error)
 {
     if (!g_strcmp0(value, "keep"))
         _cmd_options.nevra_duplicates = CR_ARG_DUP_NEVRA_KEEP_ALL;
     else if (!g_strcmp0(value, "keep-last"))
         _cmd_options.nevra_duplicates = CR_ARG_DUP_NEVRA_KEEP_LAST;
     else {
@@ -114,15 +114,15 @@
       "Choose the checksum type used in repomd.xml and for packages in the "
       "metadata. The default is now \"sha256\".", "CHECKSUM_TYPE" },
     { "pretty", 'p', 0, G_OPTION_ARG_NONE, &(_cmd_options.pretty),
       "Make sure all xml generated is formatted (default)", NULL },
     { "database", 'd', 0, G_OPTION_ARG_NONE, &(_cmd_options.database),
       "Generate sqlite databases for use with yum.", NULL },
     { "no-database", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.no_database),
-      "Do not generate sqlite databases in the repository.", NULL },
+      "Do not generate sqlite databases in the repository (default).", NULL },
     { "filelists-ext", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.filelists_ext),
       "Create filelists-ext metadata with file hashes.", NULL },
     { "update", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.update),
       "If metadata already exists in the outputdir and an rpm is unchanged "
       "(based on file size and mtime) since the metadata was generated, reuse "
       "the existing metadata rather than recalculating it. In the case of a "
       "large repository with only a few new or modified rpms "
@@ -176,17 +176,17 @@
       "Output the paths to the pkgs actually read useful with --update.",
       "READ_PKGS_LIST" },
     { "workers", 0, 0, G_OPTION_ARG_INT, &(_cmd_options.workers),
       "Number of workers to spawn to read rpms.", NULL },
     { "xz", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.xz_compression),
       "Use xz for repodata compression.", NULL },
     { "compress-type", 0, 0, G_OPTION_ARG_STRING, &(_cmd_options.compress_type),
-      "Which compression type to use.", "COMPRESSION_TYPE" },
+      "Which compression type to use for additional metadata files (comps, updateinfo, etc). Supported compressions are: bzip2, gzip, zck, zstd, xz.", "COMPRESSION_TYPE" },
     { "general-compress-type", 0, 0, G_OPTION_ARG_STRING, &(_cmd_options.general_compress_type),
-      "Which compression type to use (even for primary, filelists and other xml).",
+      "Which compression type to use (even for primary, filelists and other xml). Supported compressions are: bzip2, gzip, zck, zstd, xz.",
       "COMPRESSION_TYPE" },
 #ifdef WITH_ZCHUNK
     { "zck", 0, 0, G_OPTION_ARG_NONE, &(_cmd_options.zck_compression),
       "Generate zchunk files as well as the standard repodata.", NULL },
     { "zck-dict-dir", 0, 0, G_OPTION_ARG_FILENAME, &(_cmd_options.zck_dict_dir),
       "Directory containing compression dictionaries for use by zchunk", "ZCK_DICT_DIR" },
 #endif
@@ -311,14 +311,16 @@
 
     if (!strcmp(compress_str->str, "gz")) {
         *type = CR_CW_GZ_COMPRESSION;
     } else if (!strcmp(compress_str->str, "bz2")) {
         *type = CR_CW_BZ2_COMPRESSION;
     } else if (!strcmp(compress_str->str, "xz")) {
         *type = CR_CW_XZ_COMPRESSION;
+    } else if (!strcmp(compress_str->str, "zstd")) {
+        *type = CR_CW_ZSTD_COMPRESSION;
     } else {
         g_set_error(err, ERR_DOMAIN, CRE_BADARG,
                     "Unknown/Unsupported compression type \"%s\"", type_str);
         return FALSE;
     }
 
     return TRUE;
@@ -382,15 +384,15 @@
                 GError **err)
 {
     assert(!err || *err == NULL);
 
     // Check outputdir
     if (options->outputdir && !g_file_test(options->outputdir, G_FILE_TEST_EXISTS|G_FILE_TEST_IS_DIR)) {
         g_set_error(err, ERR_DOMAIN, CRE_BADARG,
-                    "Specified outputdir \"%s\" doesn't exists",
+                    "Specified outputdir \"%s\" doesn't exist",
                     options->outputdir);
         return FALSE;
     }
 
     // Check workers
     if ((options->workers < 1) || (options->workers > 100)) {
         g_warning("Wrong number of workers - Using 5 workers.");
@@ -494,25 +496,25 @@
             options->groupfile_fullpath = g_strconcat(input_dir,
                                                       options->groupfile,
                                                       NULL);
         }
 
         if (!remote && !g_file_test(options->groupfile_fullpath, G_FILE_TEST_IS_REGULAR)) {
             g_set_error(err, ERR_DOMAIN, CRE_BADARG,
-                        "groupfile %s doesn't exists",
+                        "groupfile %s doesn't exist",
                         options->groupfile_fullpath);
             return FALSE;
         }
     }
 
     // Process pkglist file
     if (options->pkglist) {
         if (!g_file_test(options->pkglist, G_FILE_TEST_IS_REGULAR)) {
             g_set_error(err, ERR_DOMAIN, CRE_BADARG,
-                        "pkglist file \"%s\" doesn't exists", options->pkglist);
+                        "pkglist file \"%s\" doesn't exist", options->pkglist);
             return FALSE;
         } else {
             char *content = NULL;
             GError *tmp_err = NULL;
             if (!g_file_get_contents(options->pkglist, &content, NULL, &tmp_err)) {
                 g_warning("Error while reading pkglist file: %s", tmp_err->message);
                 g_error_free(tmp_err);
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/cmd_parser.h` & `createrepo_c-1.0.0/tests/createrepo/cmd_parser.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/compression_wrapper.c` & `createrepo_c-1.0.0/tests/createrepo/compression_wrapper.c`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 #include <bzlib.h>
 #include <lzma.h>
 #ifdef WITH_ZCHUNK
 #include <zck.h>
 #endif  // WITH_ZCHUNK
 #include "error.h"
 #include "compression_wrapper.h"
+#ifdef WITH_ZSTD
+#include <zstd.h>
+#endif
 
 
 #define ERR_DOMAIN                      CREATEREPO_C_ERROR
 
 /*
 #define Z_CR_CW_NO_COMPRESSION          0
 #define Z_BEST_SPEED                    1
@@ -114,27 +117,38 @@
 
 typedef struct {
     lzma_stream stream;
     FILE *file;
     unsigned char buffer[XZ_BUFFER_SIZE];
 } XzFile;
 
+#ifdef WITH_ZSTD
+#define CR_CW_ZSTD_COMPRESSION_LEVEL    9
+typedef struct {
+    void *buffer;
+    size_t buffer_size;
+    ZSTD_inBuffer zib;
+    ZSTD_outBuffer zob;
+    void * context;     //ZSTD_{C,D}Ctx
+} ZstdFile;
+#endif
+
 cr_CompressionType
 cr_detect_compression(const char *filename, GError **err)
 {
     cr_CompressionType type = CR_CW_UNKNOWN_COMPRESSION;
 
     assert(filename);
     assert(!err || *err == NULL);
 
     if (!g_file_test(filename, G_FILE_TEST_IS_REGULAR)) {
-        g_debug("%s: File %s doesn't exists or not a regular file",
+        g_debug("%s: File %s doesn't exist or not a regular file",
                 __func__, filename);
         g_set_error(err, ERR_DOMAIN, CRE_NOFILE,
-                    "File %s doesn't exists or not a regular file", filename);
+                    "File %s doesn't exist or not a regular file", filename);
         return CR_CW_UNKNOWN_COMPRESSION;
     }
 
     // Try determine compression type via filename suffix
 
     if (g_str_has_suffix(filename, ".gz") ||
         g_str_has_suffix(filename, ".gzip") ||
@@ -147,14 +161,17 @@
         return CR_CW_BZ2_COMPRESSION;
     } else if (g_str_has_suffix(filename, ".xz"))
     {
         return CR_CW_XZ_COMPRESSION;
     } else if (g_str_has_suffix(filename, ".zck"))
     {
         return CR_CW_ZCK_COMPRESSION;
+    } else if (g_str_has_suffix(filename, ".zst"))
+    {
+        return CR_CW_ZSTD_COMPRESSION;
     } else if (g_str_has_suffix(filename, ".xml") ||
                g_str_has_suffix(filename, ".tar") ||
                g_str_has_suffix(filename, ".yaml") ||
                g_str_has_suffix(filename, ".sqlite"))
     {
         return CR_CW_NO_COMPRESSION;
     }
@@ -188,14 +205,19 @@
             g_str_has_prefix(mime_type, "application/x-compress") ||
             g_str_has_prefix(mime_type, "application/x-gunzip") ||
             g_str_has_prefix(mime_type, "multipart/x-gzip"))
         {
             type = CR_CW_GZ_COMPRESSION;
         }
 
+        else if (g_str_has_prefix(mime_type, "application/zstd"))
+        {
+            type = CR_CW_ZSTD_COMPRESSION;
+        }
+
         else if (g_str_has_prefix(mime_type, "application/x-bzip2") ||
                  g_str_has_prefix(mime_type, "application/x-bz2") ||
                  g_str_has_prefix(mime_type, "application/bzip2") ||
                  g_str_has_prefix(mime_type, "application/bz2"))
         {
             type = CR_CW_BZ2_COMPRESSION;
         }
@@ -251,14 +273,16 @@
         type = CR_CW_GZ_COMPRESSION;
     if (!g_strcmp0(name_lower, "bz2") || !g_strcmp0(name_lower, "bzip2"))
         type = CR_CW_BZ2_COMPRESSION;
     if (!g_strcmp0(name_lower, "xz"))
         type = CR_CW_XZ_COMPRESSION;
     if (!g_strcmp0(name_lower, "zck"))
         type = CR_CW_ZCK_COMPRESSION;
+    if (!g_strcmp0(name_lower, "zstd"))
+        type = CR_CW_ZSTD_COMPRESSION;
     g_free(name_lower);
 
     return type;
 }
 
 const char *
 cr_compression_suffix(cr_CompressionType comtype)
@@ -268,14 +292,16 @@
             return ".gz";
         case CR_CW_BZ2_COMPRESSION:
             return ".bz2";
         case CR_CW_XZ_COMPRESSION:
             return ".xz";
         case CR_CW_ZCK_COMPRESSION:
             return ".zck";
+        case CR_CW_ZSTD_COMPRESSION:
+            return ".zst";
         default:
             return NULL;
     }
 }
 
 
 static const char *
@@ -409,14 +435,64 @@
             if (gzbuffer((gzFile) file->FILE, GZ_BUFFER_SIZE) == -1) {
                 g_debug("%s: gzbuffer() call failed", __func__);
                 g_set_error(err, ERR_DOMAIN, CRE_GZ,
                             "gzbuffer() call failed");
             }
             break;
 
+        case (CR_CW_ZSTD_COMPRESSION): { // ------------------------------------
+#ifdef WITH_ZSTD
+            FILE *f = fopen(filename, mode_str);
+
+            if (!f) {
+                g_set_error(err, ERR_DOMAIN, CRE_IO, "fopen(): %s", g_strerror(errno));
+                break;
+            }
+
+            file->INNERFILE = f;
+
+            ZstdFile *zstd_file = g_malloc0(sizeof(ZstdFile));
+
+            if (mode == CR_CW_MODE_WRITE) {
+                if ((zstd_file->context = (void *) ZSTD_createCCtx()) == NULL) {
+                    g_set_error(err, ERR_DOMAIN, CRE_ZSTD, "%s",
+                            "Failed to create ZSTD context.");
+                    g_free(zstd_file);
+                    fclose(f);
+                    break;
+                }
+                size_t ret = ZSTD_CCtx_setParameter(zstd_file->context, ZSTD_c_compressionLevel, CR_CW_ZSTD_COMPRESSION_LEVEL);
+                if (ZSTD_isError(ret)) {
+                    g_set_error(err, ERR_DOMAIN, CRE_ZSTD, "%s",
+                            ZSTD_getErrorName(ret));
+                    g_free(zstd_file);
+                    fclose(f);
+                    break;
+                }
+                zstd_file->buffer_size = ZSTD_CStreamOutSize();
+            } else {
+                if ((zstd_file->context = (void *) ZSTD_createDCtx()) == NULL) {
+                    g_free(zstd_file);
+                    fclose(f);
+                    g_set_error(err, ERR_DOMAIN, CRE_IO, "%s",
+                            "Failed to create ZSTD context.");
+                    break;
+                }
+                zstd_file->buffer_size = ZSTD_DStreamInSize();
+            }
+            zstd_file->buffer = g_malloc(zstd_file->buffer_size);
+            file->FILE = (void *) zstd_file;
+
+            break;
+#else
+            g_set_error(err, ERR_DOMAIN, CRE_IO, "createrepo_c wasn't compiled with zstd support");
+            break;
+#endif // WITH_ZSTD
+        }
+
         case (CR_CW_BZ2_COMPRESSION): { // ------------------------------------
             FILE *f = fopen(filename, mode_str);
             file->INNERFILE = f;
             int bzerror;
 
             if (!f) {
                 g_set_error(err, ERR_DOMAIN, CRE_IO,
@@ -765,14 +841,51 @@
 
                 ret = CRE_GZ;
                 g_set_error(err, ERR_DOMAIN, CRE_GZ,
                     "gzclose(): %s", err_msg);
             }
             break;
 
+        case (CR_CW_ZSTD_COMPRESSION): { // --------------------------------------
+#ifdef WITH_ZSTD
+            ZstdFile * zstd = (ZstdFile *) cr_file->FILE;
+            if (cr_file->mode == CR_CW_MODE_READ) {
+                ZSTD_freeDCtx(zstd->context);
+            } else {
+                size_t remaining;
+                // No more new input just finish flushing compression data
+                ZSTD_inBuffer zip = { NULL, 0, 0 };
+                do {
+                    zstd->zob.dst = zstd->buffer;
+                    zstd->zob.size = zstd->buffer_size;
+                    zstd->zob.pos = 0;
+
+                    remaining = ZSTD_compressStream2(zstd->context, &zstd->zob , &zip, ZSTD_e_end);
+                    if (ZSTD_isError(remaining)) {
+                        g_set_error(err, ERR_DOMAIN, CRE_ZSTD, "%s", ZSTD_getErrorName(remaining));
+                        break;
+                    } else if (zstd->zob.pos != fwrite(zstd->buffer, 1, zstd->zob.pos, cr_file->INNERFILE)) {
+                        g_set_error(err, ERR_DOMAIN, CRE_IO, "cr_close ZSTD fwrite failed");
+                        break;
+                    }
+                } while(remaining != 0);
+                ZSTD_freeCCtx(zstd->context);
+            }
+
+            fclose(cr_file->INNERFILE);
+            g_free(zstd->buffer);
+            g_free(cr_file->FILE);
+
+            ret = CRE_OK;
+            break;
+#else
+            g_set_error(err, ERR_DOMAIN, CRE_IO, "createrepo_c wasn't compiled with zstd support");
+            break;
+#endif // WITH_ZSTD
+        }
         case (CR_CW_BZ2_COMPRESSION): // --------------------------------------
             if (cr_file->mode == CR_CW_MODE_READ)
                 BZ2_bzReadClose(&rc, (BZFILE *) cr_file->FILE);
             else
                 BZ2_bzWriteClose(&rc, (BZFILE *) cr_file->FILE,
                                  BZ2_SKIP_FFLUSH, NULL, NULL);
 
@@ -976,14 +1089,51 @@
             if (ret == -1) {
                 ret = CR_CW_ERR;
                 g_set_error(err, ERR_DOMAIN, CRE_GZ,
                     "fread(): %s", cr_gz_strerror((gzFile) cr_file->FILE));
             }
             break;
 
+        case (CR_CW_ZSTD_COMPRESSION): { // ---------------------------------------
+#ifdef WITH_ZSTD
+            ZstdFile * zstd = (ZstdFile *) cr_file->FILE;
+
+            ZSTD_outBuffer zob = {buffer, len, 0};
+
+            while (zob.pos < zob.size) {
+                // Re-fill compressed data buffer
+                if (zstd->zib.pos >= zstd->zib.size) {
+                    zstd->zib.size = fread(zstd->buffer, 1, zstd->buffer_size, cr_file->INNERFILE);
+                    if (zstd->zib.size == 0) {
+                        break; //EOF
+                    }
+                    zstd->zib.src = zstd->buffer;
+                    zstd->zib.pos = 0;
+                }
+
+                // Decompress chunk
+                int decomp_ret = ZSTD_decompressStream(zstd->context, &zob, &zstd->zib);
+                if (ZSTD_isError(decomp_ret)) {
+                    ret = CR_CW_ERR;
+                    g_set_error(err, ERR_DOMAIN, CRE_ZSTD, "%s", ZSTD_getErrorName(decomp_ret));
+                    break;
+                }
+
+            }
+
+            if (!(err && *err)) {
+                ret = zob.pos;
+            }
+
+            break;
+#else
+            g_set_error(err, ERR_DOMAIN, CRE_IO, "createrepo_c wasn't compiled with zstd support");
+            break;
+#endif // WITH_ZSTD
+        }
         case (CR_CW_BZ2_COMPRESSION): // --------------------------------------
             ret = BZ2_bzRead(&bzerror, (BZFILE *) cr_file->FILE, buffer, len);
             if (!ret && bzerror == BZ_SEQUENCE_ERROR)
                 // Next read after BZ_STREAM_END (EOF)
                 return 0;
 
             if (bzerror != BZ_OK && bzerror != BZ_STREAM_END) {
@@ -1210,14 +1360,53 @@
             if ((ret = gzwrite((gzFile) cr_file->FILE, buffer, len)) == 0) {
                 ret = CR_CW_ERR;
                 g_set_error(err, ERR_DOMAIN, CRE_GZ,
                     "gzwrite(): %s", cr_gz_strerror((gzFile) cr_file->FILE));
             }
             break;
 
+        case (CR_CW_ZSTD_COMPRESSION): { // ---------------------------------------
+#ifdef WITH_ZSTD
+            ZstdFile * zstd = (ZstdFile *) cr_file->FILE;
+            ZSTD_inBuffer zib = {buffer, len, 0};
+
+            while (zib.pos < zib.size) {
+                zstd->zob.dst = zstd->buffer;
+                zstd->zob.size = zstd->buffer_size;
+                zstd->zob.pos = 0;
+
+                // Compress chunk into buffer
+                size_t remaining = ZSTD_compressStream2(zstd->context, &zstd->zob , &zib, ZSTD_e_continue);
+                if (ZSTD_isError(remaining)) {
+                    g_set_error(err, ERR_DOMAIN, CRE_ZSTD, "%s", ZSTD_getErrorName(remaining));
+                    break;
+                }
+
+                // Write compressed buffer
+                if (zstd->zob.pos > 0) {
+                    size_t nw = fwrite(zstd->buffer, 1, zstd->zob.pos, cr_file->INNERFILE);
+                    if (nw != zstd->zob.pos) {
+                        g_set_error(err, ERR_DOMAIN, CRE_IO, "cr_write zstd write failed");
+                        break;
+                    }
+                }
+
+            }
+
+            if (!(err && *err)) {
+                ret = zib.pos;
+            }
+
+            break;
+#else
+            g_set_error(err, ERR_DOMAIN, CRE_IO, "createrepo_c wasn't compiled with zstd support");
+            break;
+#endif // WITH_ZSTD
+        }
+
         case (CR_CW_BZ2_COMPRESSION): // --------------------------------------
             BZ2_bzWrite(&bzerror, (BZFILE *) cr_file->FILE, (void *) buffer, len);
             if (bzerror == BZ_OK) {
                 ret = len;
             } else {
                 const char *err_msg;
                 ret = CR_CW_ERR;
@@ -1357,14 +1546,15 @@
     switch (cr_file->type) {
 
         case (CR_CW_NO_COMPRESSION): // ---------------------------------------
         case (CR_CW_GZ_COMPRESSION): // ---------------------------------------
         case (CR_CW_BZ2_COMPRESSION): // --------------------------------------
         case (CR_CW_XZ_COMPRESSION): // ---------------------------------------
         case (CR_CW_ZCK_COMPRESSION): // --------------------------------------
+        case (CR_CW_ZSTD_COMPRESSION): // --------------------------------------
             len = strlen(str);
             ret = cr_write(cr_file, str, len, err);
             if (ret != (int) len)
                 ret = CR_CW_ERR;
             break;
 
         default: // -----------------------------------------------------------
@@ -1394,14 +1584,15 @@
     }
 
     switch (cr_file->type) {
         case (CR_CW_NO_COMPRESSION): // ---------------------------------------
         case (CR_CW_GZ_COMPRESSION): // ---------------------------------------
         case (CR_CW_BZ2_COMPRESSION): // --------------------------------------
         case (CR_CW_XZ_COMPRESSION): // ---------------------------------------
+        case (CR_CW_ZSTD_COMPRESSION): // ---------------------------------------
             break;
         case (CR_CW_ZCK_COMPRESSION): { // ------------------------------------
 #ifdef WITH_ZCHUNK
             zckCtx *zck = (zckCtx *) cr_file->FILE;
             ssize_t wb = zck_end_chunk(zck);
             if (wb < 0) {
                 g_set_error(err, ERR_DOMAIN, CRE_ZCK,
@@ -1446,14 +1637,15 @@
     }
 
     switch (cr_file->type) {
         case (CR_CW_NO_COMPRESSION): // ---------------------------------------
         case (CR_CW_GZ_COMPRESSION): // ---------------------------------------
         case (CR_CW_BZ2_COMPRESSION): // --------------------------------------
         case (CR_CW_XZ_COMPRESSION): // ---------------------------------------
+        case (CR_CW_ZSTD_COMPRESSION): // ---------------------------------------
             break;
         case (CR_CW_ZCK_COMPRESSION): { // ------------------------------------
 #ifdef WITH_ZCHUNK
             zckCtx *zck = (zckCtx *) cr_file->FILE;
             if (!zck_set_ioption(zck, ZCK_MANUAL_CHUNK, !auto_chunk)) {
                 g_set_error(err, ERR_DOMAIN, CRE_ZCK,
                             "Error setting auto_chunk: %s",
@@ -1520,14 +1712,15 @@
     switch (cr_file->type) {
 
         case (CR_CW_NO_COMPRESSION): // ---------------------------------------
         case (CR_CW_GZ_COMPRESSION): // ---------------------------------------
         case (CR_CW_BZ2_COMPRESSION): // --------------------------------------
         case (CR_CW_XZ_COMPRESSION): // ---------------------------------------
         case (CR_CW_ZCK_COMPRESSION): // --------------------------------------
+        case (CR_CW_ZSTD_COMPRESSION): // --------------------------------------
             tmp_ret = cr_write(cr_file, buf, ret, err);
             if (tmp_ret != (int) ret)
                 ret = CR_CW_ERR;
             break;
 
         default: // -----------------------------------------------------------
             ret = CR_CW_ERR;
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/compression_wrapper.h` & `createrepo_c-1.0.0/tests/createrepo/compression_wrapper.h`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     CR_CW_AUTO_DETECT_COMPRESSION,    /*!< Autodetection */
     CR_CW_UNKNOWN_COMPRESSION,        /*!< Unknown compression */
     CR_CW_NO_COMPRESSION,             /*!< No compression */
     CR_CW_GZ_COMPRESSION,             /*!< Gzip compression */
     CR_CW_BZ2_COMPRESSION,            /*!< BZip2 compression */
     CR_CW_XZ_COMPRESSION,             /*!< XZ compression */
     CR_CW_ZCK_COMPRESSION,            /*!< ZCK compression */
+    CR_CW_ZSTD_COMPRESSION,           /*!< ZSTD compression */
     CR_CW_COMPRESSION_SENTINEL,       /*!< Sentinel of the list */
 } cr_CompressionType;
 
 /** Open modes.
  */
 typedef enum {
     CR_CW_MODE_READ,            /*!< Read mode */
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/constants.h` & `createrepo_c-1.0.0/tests/createrepo/constants.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/createrepo_c.c` & `createrepo_c-1.0.0/tests/createrepo/createrepo_c.c`

 * *Files 2% similar despite different names*

```diff
@@ -378,72 +378,14 @@
         }
     }
 
     g_debug("Cachedir for checksums is %s", cmd_options->checksum_cachedir);
     return TRUE;
 }
 
-/** Adds groupfile cr_RepomdRecords to additional_metadata_rec list.
- *  Groupfile is a special case, because it's the only metadatum
- *  that can be inputed to createrepo_c via command line option.
- *
- * @param group_metadatum           Cr_Metadatum for used groupfile
- * @param additional_metadata_rec   GSList of cr_RepomdRecords
- * @param comp_type                 Groupfile compression type
- * @param repomd_checksum_type
- *
- * @return                          GSList with added cr_RepomdRecords for
- *                                  groupfile
- */
-GSList*
-cr_create_repomd_records_for_groupfile_metadata(const cr_Metadatum *group_metadatum,
-                                                GSList *additional_metadata_rec,
-                                                cr_CompressionType comp_type,
-                                                cr_ChecksumType repomd_checksum_type)
-{
-    GError *tmp_err = NULL;
-    char *compression_suffix = g_strdup(cr_compression_suffix(comp_type));
-    compression_suffix[0] = '_'; //replace '.'
-    additional_metadata_rec = g_slist_prepend(additional_metadata_rec,
-                                              cr_repomd_record_new(
-                                                  group_metadatum->type,
-                                                  group_metadatum->name
-                                              ));
-
-    gchar *compressed_record_type = g_strconcat(group_metadatum->type, compression_suffix, NULL);
-    additional_metadata_rec = g_slist_prepend(additional_metadata_rec,
-                                              cr_repomd_record_new(
-                                                  compressed_record_type,
-                                                  NULL
-                                              ));
-
-    cr_repomd_record_compress_and_fill(additional_metadata_rec->next->data,
-                                       additional_metadata_rec->data,
-                                       repomd_checksum_type,
-                                       comp_type,
-                                       NULL,
-                                       &tmp_err);
-
-    if (tmp_err) {
-        g_critical("Cannot process %s %s: %s",
-                   group_metadatum->type,
-                   group_metadatum->name,
-                   tmp_err->message);
-        g_free(compression_suffix);
-        g_free(compressed_record_type);
-        g_clear_error(&tmp_err);
-        exit(EXIT_FAILURE);
-    }
-
-    g_free(compressed_record_type);
-    g_free(compression_suffix);
-
-    return additional_metadata_rec;
-}
-
 /** Creates list of cr_RepomdRecords from list
  *  of additional metadata (cr_Metadatum)
  *
  * @param additional_metadata       List of cr_Metadatum
  * @param repomd_checksum_type
  *
  * @return                          New GSList of cr_RepomdRecords
@@ -880,17 +822,17 @@
     current_pkglist = NULL;
     GSList *additional_metadata = NULL;
 
     // Setup compression types
     const char *xml_compression_suffix = NULL;
     const char *sqlite_compression_suffix = NULL;
     const char *compression_suffix = NULL;
-    cr_CompressionType xml_compression = CR_CW_GZ_COMPRESSION;
+    cr_CompressionType xml_compression = CR_CW_ZSTD_COMPRESSION;
     cr_CompressionType sqlite_compression = CR_CW_BZ2_COMPRESSION;
-    cr_CompressionType compression = CR_CW_GZ_COMPRESSION;
+    cr_CompressionType compression = CR_CW_ZSTD_COMPRESSION;
 
     if (cmd_options->compression_type != CR_CW_UNKNOWN_COMPRESSION) {
         sqlite_compression = cmd_options->compression_type;
         compression        = cmd_options->compression_type;
     }
 
     if (cmd_options->general_compression_type != CR_CW_UNKNOWN_COMPRESSION) {
@@ -899,21 +841,22 @@
         compression        = cmd_options->general_compression_type;
     }
 
     xml_compression_suffix = cr_compression_suffix(xml_compression);
     sqlite_compression_suffix = cr_compression_suffix(sqlite_compression);
     compression_suffix = cr_compression_suffix(compression);
 
-    cr_Metadatum *new_groupfile_metadatum = NULL;
-
     // Groupfile specified as argument
     if (cmd_options->groupfile_fullpath) {
-        new_groupfile_metadatum = g_malloc0(sizeof(cr_Metadatum));
-        new_groupfile_metadatum->name = cr_copy_metadatum(cmd_options->groupfile_fullpath, tmp_out_repo, &tmp_err);
+        gchar *compressed_path = cr_compress_groupfile(cmd_options->groupfile_fullpath, tmp_out_repo, compression);
+        cr_Metadatum *new_groupfile_metadatum = g_malloc0(sizeof(cr_Metadatum));
+        new_groupfile_metadatum->name = compressed_path;
         new_groupfile_metadatum->type = g_strdup("group");
+        additional_metadata = g_slist_prepend(additional_metadata, new_groupfile_metadatum);
+
         //remove old groupfile(s) (every [compressed] variant)
         if (old_metadata_location){
             GSList *node_iter = old_metadata_location->additional_metadata;
             while (node_iter != NULL){
                 cr_Metadatum *m = node_iter->data;
                 GSList *next = g_slist_next(node_iter);
                 if(g_str_has_prefix(m->type, "group")){
@@ -1074,15 +1017,15 @@
 
     gchar *pri_xml_filename = NULL;
     gchar *fil_xml_filename = NULL;
     gchar *fex_xml_filename = NULL;
     gchar *oth_xml_filename = NULL;
 
     g_message("Temporary output repo path: %s", tmp_out_repo);
-    g_debug("Creating .xml.gz files");
+    g_debug("Creating .xml.%s files", xml_compression_suffix);
 
     pri_xml_filename = g_strconcat(tmp_out_repo, "/primary.xml", xml_compression_suffix, NULL);
     fil_xml_filename = g_strconcat(tmp_out_repo, "/filelists.xml", xml_compression_suffix, NULL);
     if (cmd_options->filelists_ext)
         fex_xml_filename = g_strconcat(tmp_out_repo, "/filelists-ext.xml", xml_compression_suffix, NULL);
     oth_xml_filename = g_strconcat(tmp_out_repo, "/other.xml", xml_compression_suffix, NULL);
 
@@ -1189,15 +1132,15 @@
     gchar *fex_db_filename = NULL;
     gchar *oth_db_filename = NULL;
     cr_SqliteDb *pri_db = NULL;
     cr_SqliteDb *fil_db = NULL;
     cr_SqliteDb *fex_db = NULL;
     cr_SqliteDb *oth_db = NULL;
 
-    if (!cmd_options->no_database) {
+    if (cmd_options->database) {
         _cleanup_file_close_ int pri_db_fd = -1;
         _cleanup_file_close_ int fil_db_fd = -1;
         _cleanup_file_close_ int fex_db_fd = -1;
         _cleanup_file_close_ int oth_db_fd = -1;
 
         g_message("Preparing sqlite DBs");
         if (!cmd_options->local_sqlite) {
@@ -1860,38 +1803,24 @@
                                                 NULL);
     g_thread_pool_push(fill_pool, oth_fill_task, NULL);
 
 
     additional_metadata_rec = cr_create_repomd_records_for_additional_metadata(additional_metadata,
                                                                                cmd_options->repomd_checksum_type);
 
-    if (new_groupfile_metadatum) {
-        additional_metadata_rec = cr_create_repomd_records_for_groupfile_metadata(new_groupfile_metadatum,
-                                                                                  additional_metadata_rec,
-                                                                                  compression,
-                                                                                  cmd_options->repomd_checksum_type);
-
-        //NOTE(amatej): Now we can add groupfile metadata to the additional_metadata list, for unified handlig while zck compressing
-        additional_metadata = g_slist_prepend(additional_metadata, new_groupfile_metadatum);
-        cr_Metadatum *compressed_new_groupfile_metadatum = g_malloc0(sizeof(cr_Metadatum));
-        compressed_new_groupfile_metadatum->name = g_strdup(((cr_RepomdRecord *) additional_metadata_rec->data)->location_real);
-        compressed_new_groupfile_metadatum->type = g_strdup(((cr_RepomdRecord *) additional_metadata_rec->data)->type);
-        additional_metadata = g_slist_prepend(additional_metadata, compressed_new_groupfile_metadatum);
-    }
-
     // Wait till repomd record fill task of xml files ends.
     g_thread_pool_free(fill_pool, FALSE, TRUE);
 
     cr_repomdrecordfilltask_free(pri_fill_task, NULL);
     cr_repomdrecordfilltask_free(fil_fill_task, NULL);
     cr_repomdrecordfilltask_free(fex_fill_task, NULL);
     cr_repomdrecordfilltask_free(oth_fill_task, NULL);
 
     // Sqlite db
-    if (!cmd_options->no_database) {
+    if (cmd_options->database) {
 
         gchar *pri_db_name = g_strconcat(tmp_out_repo, "/primary.sqlite",
                                          sqlite_compression_suffix, NULL);
         gchar *fil_db_name = g_strconcat(tmp_out_repo, "/filelists.sqlite",
                                          sqlite_compression_suffix, NULL);
         gchar *fex_db_name = NULL;
         if (cmd_options->filelists_ext)
@@ -2471,15 +2400,15 @@
 
     // Rename out_repo to "repodata.old.pid.date.microsecs"
     gchar *tmp_dirname = cr_append_pid_and_datetime("repodata.old.", NULL);
     gchar *old_repodata_path = g_build_filename(out_dir, tmp_dirname, NULL);
     g_free(tmp_dirname);
 
     if (!cr_move_recursive(out_repo, old_repodata_path, &tmp_err)) {
-        g_debug("Old repodata doesn't exists: Cannot rename %s -> %s: %s",
+        g_debug("Old repodata doesn't exist: Cannot rename %s -> %s: %s",
                 out_repo, old_repodata_path, tmp_err->message);
     } else {
         g_debug("Renamed %s -> %s", out_repo, old_repodata_path);
         old_repodata_renamed = TRUE;
     }
 
     // Rename tmp_out_repo to out_repo
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/createrepo_c.h` & `createrepo_c-1.0.0/tests/createrepo/createrepo_c.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/createrepo_shared.c` & `createrepo_c-1.0.0/tests/createrepo/createrepo_shared.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/createrepo_shared.h` & `createrepo_c-1.0.0/tests/createrepo/createrepo_shared.h`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 gboolean
 cr_unblock_terminating_signals(GError **err);
 
 
 /**
  * This function does:
  * - Tries to create repo/.repodata/ dir.
- * - If it doesn't exists, it's created and function returns TRUE.
+ * - If it doesn't exist, it's created and function returns TRUE.
  * - If it exists and ignore_lock is FALSE, returns FALSE and err is set.
  * - If it exists and ignore_lock is TRUE it:
  *  - Removes the existing .repodata/ dir and all its content
  *  - Creates (empty) new one (just as a lock dir - place holder)
  *  - Creates .repodata.pid.datetime.usec/ that should be used for
  *    repodata generation
  *
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/deltarpms.c` & `createrepo_c-1.0.0/tests/createrepo/deltarpms.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/deltarpms.h.in` & `createrepo_c-1.0.0/tests/createrepo/deltarpms.h.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/dumper_thread.c` & `createrepo_c-1.0.0/tests/createrepo/dumper_thread.c`

 * *Files 0% similar despite different names*

```diff
@@ -627,18 +627,20 @@
                 // CR_PACKAGE_SINGLE_CHUNK used with the preloaded (old)
                 // metadata.  Create a new per-package chunk.
                 assert (!md->chunk);
                 md->chunk = g_string_chunk_new(1024);
                 md->loadingflags &= ~CR_PACKAGE_SINGLE_CHUNK;
 
                 // We have usable old data, but we have to set proper locations
-                // WARNING! This two lines destructively modifies content of
-                // packages in old metadata.
+                // WARNING! location_href is overidden
+                // location_base is kept by default, unless specified differently
+                //
                 md->location_href = cr_safe_string_chunk_insert(md->chunk, location_href);
-                md->location_base = cr_safe_string_chunk_insert(md->chunk, location_base);
+                if (location_base)
+                    md->location_base = cr_safe_string_chunk_insert(md->chunk, location_base);
                 // ^^^ The location_base and location_href create a new data
                 // chunk, even though the rest of the metadata is stored in the
                 // global chunk (shared with all packages).
             }
         }
     }
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/dumper_thread.h` & `createrepo_c-1.0.0/tests/createrepo/dumper_thread.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/error.c` & `createrepo_c-1.0.0/tests/createrepo/error.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/error.h` & `createrepo_c-1.0.0/tests/createrepo/error.h`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     CRE_DB,     /*!<
         (5) A database error */
     CRE_BADARG, /*!<
         (6) At least one argument of function is bad or non complete */
     CRE_NOFILE, /*!<
         (7) File doesn't exist */
     CRE_NODIR, /*!<
-        (8) Directory doesn't exist (not a dir or path doesn't exists) */
+        (8) Directory doesn't exist (not a dir or path doesn't exist) */
     CRE_EXISTS, /*!<
         (9) File/Directory already exists */
     CRE_UNKNOWNCHECKSUMTYPE, /*!<
         (10) Unknown/Unsupported checksum type */
     CRE_UNKNOWNCOMPRESSION, /*!<
         (11) Unknown/Unsupported compression type */
     CRE_XMLPARSER, /*!<
@@ -94,14 +94,16 @@
         (32) Bad updateinfo.xml file */
     CRE_SIGPROCMASK, /*!<
         (33) Cannot change blocked signals */
     CRE_ZCK, /*!<
         (34) ZCK library related error */
     CRE_MODULEMD, /*!<
         (35) modulemd related error */
+    CRE_ZSTD, /*!<
+        (36) Zstd library related error */
     CRE_SENTINEL, /*!<
         (XX) Sentinel */
 } cr_Error;
 
 /** Converts cr_Error return code to error string.
  * @param rc        cr_Error return code
  * @return          Error string
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/helpers.c` & `createrepo_c-1.0.0/tests/createrepo/helpers.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/helpers.h` & `createrepo_c-1.0.0/tests/createrepo/helpers.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/koji.c` & `createrepo_c-1.0.0/tests/createrepo/koji.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/koji.h` & `createrepo_c-1.0.0/tests/createrepo/koji.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/load_metadata.c` & `createrepo_c-1.0.0/tests/createrepo/load_metadata.c`

 * *Files 5% similar despite different names*

```diff
@@ -696,7 +696,35 @@
 
     ret = cr_metadata_load_xml(md, ml, err);
 
     cr_metadatalocation_free(ml);
 
     return ret;
 }
+
+gchar *
+cr_compress_groupfile(const char *groupfile, const char *dest_dir, cr_CompressionType compression)
+{
+    const char *compression_suffix = cr_compression_suffix(compression);
+    GError *tmp_err = NULL;
+    gchar *compressed_path;
+    cr_CompressionType old_type = cr_detect_compression(groupfile, &tmp_err);
+    if (tmp_err) {
+        compressed_path = g_strconcat(dest_dir, cr_get_filename(groupfile), compression_suffix, NULL);
+        g_debug("Unable to detect compression type of %s, using %s for groupfile.", groupfile, compressed_path);
+        g_clear_error(&tmp_err);
+    } else if (old_type == CR_CW_NO_COMPRESSION) {
+        compressed_path = g_strconcat(dest_dir, cr_get_filename(groupfile), compression_suffix, NULL);
+    } else {
+        // strip compression suffix
+        gchar *tmp_file = g_strndup(groupfile, strlen(groupfile) - strlen(cr_compression_suffix(old_type)));
+        compressed_path = g_strconcat(dest_dir, cr_get_filename(tmp_file), compression_suffix, NULL);
+        g_free(tmp_file);
+    }
+    if (cr_compress_file(groupfile, compressed_path, compression, NULL, 0, &tmp_err) != CRE_OK) {
+        g_critical("Cannot compress file: %s: %s", groupfile,
+                   (tmp_err ? tmp_err->message : "Unknown error"));
+        g_clear_error(&tmp_err);
+        exit(EXIT_FAILURE);
+    }
+    return compressed_path;
+}
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/load_metadata.h` & `createrepo_c-1.0.0/tests/createrepo/load_metadata.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/locate_metadata.c` & `createrepo_c-1.0.0/tests/createrepo/locate_metadata.c`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         g_warning("%s: %s is not a directory", __func__, repopath);
         return ret;
     }
 
     // Create path to repomd.xml and check if it exists
     repomd = g_build_filename(repopath, "repodata", "repomd.xml", NULL);
     if (!g_file_test(repomd, G_FILE_TEST_EXISTS)) {
-        g_debug("%s: %s doesn't exists", __func__, repomd);
+        g_debug("%s: %s doesn't exist", __func__, repomd);
         return ret;
     }
 
     ret = cr_parse_repomd(repomd, repopath, ignore_sqlite);
 
     return ret;
 }
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/locate_metadata.h` & `createrepo_c-1.0.0/tests/createrepo/locate_metadata.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/mergerepo_c.c` & `createrepo_c-1.0.0/tests/createrepo/mergerepo_c.c`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 #define DEFAULT_OUTPUTDIR               "merged_repo/"
 
 #include "mergerepo_c.h"
 
 struct CmdOptions _cmd_options = {
         .db_compression_type = DEFAULT_DB_COMPRESSION_TYPE,
-        .groupfile_compression_type = DEFAULT_GROUPFILE_COMPRESSION_TYPE,
+        .compression_type = DEFAULT_COMPRESSION_TYPE,
         .merge_method = MM_DEFAULT,
         .unique_md_filenames = TRUE,
         .simple_md_filenames = FALSE,
 
         .zck_compression = FALSE,
         .zck_dict_dir = NULL,
     };
@@ -277,19 +277,19 @@
     if (options->compress_type) {
 
         cr_CompressionType type;
         type = cr_compression_type(options->compress_type);
 
         if (type == CR_CW_UNKNOWN_COMPRESSION) {
             g_critical("Compression %s not available: Please choose from: "
-                       "gz or bz2 or xz", options->compress_type);
+                       "gz, bz2, xz or zstd", options->compress_type);
             ret = FALSE;
         } else {
             options->db_compression_type = type;
-            options->groupfile_compression_type = type;
+            options->compression_type = type;
         }
     }
 
     // Merge method
     if (options->merge_method_str) {
         if (options->koji) {
             g_warning("With -k/--koji argument merge method is ignored (--all is implicitly used).");
@@ -325,15 +325,15 @@
 
     if (options->blocked) {
         if (!options->koji) {
             g_critical("-b/--blocked cannot be used without -k/--koji argument");
             ret = FALSE;
         }
         if (!g_file_test(options->blocked, G_FILE_TEST_EXISTS)) {
-            g_critical("File %s doesn't exists", options->blocked);
+            g_critical("File %s doesn't exist", options->blocked);
             ret = FALSE;
         }
     }
 
     if (options->repo_prefix_search || options->repo_prefix_replace) {
         if (options->repo_prefix_search == NULL) {
             g_critical("--repo-prefix-replace must be used together with --repo-prefix-search");
@@ -952,36 +952,40 @@
             g_critical("Error reading zchunk other dict %s: %s",
                        oth_dict_file, tmp_err->message);
             g_clear_error(&tmp_err);
             exit(EXIT_FAILURE);
         }
     }
 
-    const char *groupfile_suffix = cr_compression_suffix(
-                                    cmd_options->groupfile_compression_type);
+    const char *compression_suffix = cr_compression_suffix(
+                                    cmd_options->compression_type);
 
     gchar *pri_xml_filename = g_strconcat(cmd_options->tmp_out_repo,
-                                          "/primary.xml.gz", NULL);
+                                          "/primary.xml",
+                                          compression_suffix, NULL);
     gchar *fil_xml_filename = g_strconcat(cmd_options->tmp_out_repo,
-                                          "/filelists.xml.gz", NULL);
+                                          "/filelists.xml",
+                                          compression_suffix, NULL);
     gchar *fex_xml_filename = NULL;
     if (cmd_options->filelists_ext)
         fex_xml_filename = g_strconcat(cmd_options->tmp_out_repo,
-                                       "/filelists-ext.xml.gz", NULL);
+                                       "/filelists-ext.xml",
+                                       compression_suffix, NULL);
     gchar *oth_xml_filename = g_strconcat(cmd_options->tmp_out_repo,
-                                          "/other.xml.gz", NULL);
+                                          "/other.xml",
+                                          compression_suffix, NULL);
 
     gchar *update_info_filename = NULL;
     if (!cmd_options->noupdateinfo)
         update_info_filename  = g_strconcat(cmd_options->tmp_out_repo,
                                             "/updateinfo.xml",
-                                            groupfile_suffix, NULL);
+                                            compression_suffix, NULL);
 
     pri_f = cr_xmlfile_sopen_primary(pri_xml_filename,
-                                     CR_CW_GZ_COMPRESSION,
+                                     cmd_options->compression_type,
                                      pri_stat,
                                      &tmp_err);
     if (tmp_err) {
         g_critical("Cannot open %s: %s", pri_xml_filename, tmp_err->message);
         cr_contentstat_free(pri_stat, NULL);
         cr_contentstat_free(fil_stat, NULL);
         cr_contentstat_free(fex_stat, NULL);
@@ -1001,15 +1005,15 @@
         g_free(fex_dict);
         g_free(oth_dict);
         cr_xmlfile_close(pri_f, NULL);
         return 0;
     }
 
     fil_f = cr_xmlfile_sopen_filelists(fil_xml_filename,
-                                       CR_CW_GZ_COMPRESSION,
+                                       cmd_options->compression_type,
                                        fil_stat,
                                        &tmp_err);
     if (tmp_err) {
         g_critical("Cannot open %s: %s", fil_xml_filename, tmp_err->message);
         cr_contentstat_free(pri_stat, NULL);
         cr_contentstat_free(fil_stat, NULL);
         cr_contentstat_free(fex_stat, NULL);
@@ -1030,15 +1034,15 @@
         g_free(fex_dict);
         g_free(oth_dict);
         return 0;
     }
 
     if (cmd_options->filelists_ext) {
         fex_f = cr_xmlfile_sopen_filelists(fex_xml_filename,
-                                           CR_CW_GZ_COMPRESSION,
+                                           cmd_options->compression_type,
                                            fex_stat,
                                            &tmp_err);
         if (tmp_err) {
             g_critical("Cannot open %s: %s", fil_xml_filename, tmp_err->message);
             cr_contentstat_free(pri_stat, NULL);
             cr_contentstat_free(fil_stat, NULL);
             cr_contentstat_free(fex_stat, NULL);
@@ -1060,15 +1064,15 @@
             g_free(fex_dict);
             g_free(oth_dict);
             return 0;
         }
     }
 
     oth_f = cr_xmlfile_sopen_other(oth_xml_filename,
-                                   CR_CW_GZ_COMPRESSION,
+                                   cmd_options->compression_type,
                                    oth_stat,
                                    &tmp_err);
     if (tmp_err) {
         g_critical("Cannot open %s: %s", oth_xml_filename, tmp_err->message);
         cr_contentstat_free(pri_stat, NULL);
         cr_contentstat_free(fil_stat, NULL);
         cr_contentstat_free(fex_stat, NULL);
@@ -1238,15 +1242,15 @@
     // Prepare sqlite if needed
 
     cr_SqliteDb *pri_db = NULL;
     cr_SqliteDb *fil_db = NULL;
     cr_SqliteDb *fex_db = NULL;
     cr_SqliteDb *oth_db = NULL;
 
-    if (!cmd_options->no_database) {
+    if (cmd_options->database) {
         gchar *pri_db_filename = NULL;
         gchar *fil_db_filename = NULL;
         gchar *fex_db_filename = NULL;
         gchar *oth_db_filename = NULL;
 
         pri_db_filename = g_strconcat(cmd_options->tmp_out_repo,
                                       "/primary.sqlite", NULL);
@@ -1325,15 +1329,15 @@
                 cr_xmlfile_add_chunk(pri_cr_zck, (const char *) res.primary, NULL);
                 cr_xmlfile_add_chunk(fil_cr_zck, (const char *) res.filelists, NULL);
                 if (cmd_options->filelists_ext)
                     cr_xmlfile_add_chunk(fex_cr_zck, (const char *) res.filelists_ext, NULL);
                 cr_xmlfile_add_chunk(oth_cr_zck, (const char *) res.other, NULL);
             }
 
-            if (!cmd_options->no_database) {
+            if (cmd_options->database) {
                 cr_db_add_pkg(pri_db, pkg, NULL);
                 cr_db_add_pkg(fil_db, pkg, NULL);
                 if (cmd_options->filelists_ext)
                     cr_db_add_pkg(fex_db, pkg, NULL);
                 cr_db_add_pkg(oth_db, pkg, NULL);
             }
 
@@ -1363,15 +1367,15 @@
 
     // Write updateinfo.xml
     // TODO
 
     if (!cmd_options->noupdateinfo) {
         CR_FILE *update_info = cr_open(update_info_filename,
                                        CR_CW_MODE_WRITE,
-                                       cmd_options->groupfile_compression_type,
+                                       cmd_options->compression_type,
                                        &tmp_err);
         if (update_info) {
             cr_puts(update_info,
                     "<?xml version=\"1.0\"?>\n<updates></updates>\n",
                     NULL);
             cr_close(update_info, NULL);
         } else {
@@ -1386,18 +1390,18 @@
 #ifdef WITH_LIBMODULEMD
     // Write modulemd
     g_autofree gchar *modulemd_filename = NULL;
 
     if (module_index) {
         gboolean ret;
         modulemd_filename =
-            g_strconcat(cmd_options->tmp_out_repo, "/modules.yaml.gz", NULL);
+            g_strconcat(cmd_options->tmp_out_repo, "/modules.yaml", compression_suffix, NULL);
         CR_FILE *modulemd = cr_open(modulemd_filename,
                                     CR_CW_MODE_WRITE,
-                                    CR_CW_GZ_COMPRESSION,
+                                    cmd_options->compression_type,
                                     &tmp_err);
         if (modulemd) {
             ret = modulemd_module_index_dump_to_custom(module_index,
                                                        modulemd_write_handler,
                                                        modulemd,
                                                        &tmp_err);
             if (!ret) {
@@ -1429,15 +1433,14 @@
     cr_RepomdRecord *fex_db_rec               = NULL;
     cr_RepomdRecord *oth_db_rec               = NULL;
     cr_RepomdRecord *pri_zck_rec              = NULL;
     cr_RepomdRecord *fil_zck_rec              = NULL;
     cr_RepomdRecord *fex_zck_rec              = NULL;
     cr_RepomdRecord *oth_zck_rec              = NULL;
     cr_RepomdRecord *groupfile_rec            = NULL;
-    cr_RepomdRecord *compressed_groupfile_rec = NULL;
     cr_RepomdRecord *groupfile_zck_rec        = NULL;
     cr_RepomdRecord *update_info_rec          = NULL;
     cr_RepomdRecord *update_info_zck_rec      = NULL;
     cr_RepomdRecord *pkgorigins_rec           = NULL;
     cr_RepomdRecord *pkgorigins_zck_rec       = NULL;
 
 #ifdef WITH_LIBMODULEMD
@@ -1513,21 +1516,19 @@
         }
     }
 #endif /* WITH_LIBMODULEMD */
 
     // Groupfile
 
     if (groupfile) {
-        groupfile_rec = cr_repomd_record_new("group", groupfile);
-        compressed_groupfile_rec = cr_repomd_record_new("group_gz", NULL);
-        cr_repomd_record_compress_and_fill(groupfile_rec,
-                                           compressed_groupfile_rec,
-                                           CR_CHECKSUM_SHA256,
-                                           cmd_options->groupfile_compression_type,
-                                           NULL, NULL);
+        gchar *compressed_path = cr_compress_groupfile(groupfile, cmd_options->tmp_out_repo, cmd_options->compression_type);
+        groupfile_rec = cr_repomd_record_new("group", compressed_path);
+        g_free(compressed_path);
+        cr_repomd_record_fill(groupfile_rec, CR_CHECKSUM_SHA256, NULL);
+
         if (cmd_options->zck_compression) {
             groupfile_zck_rec = cr_repomd_record_new("group_zck", NULL);
             cr_repomd_record_compress_and_fill(groupfile_rec,
                                                groupfile_zck_rec,
                                                CR_CHECKSUM_SHA256,
                                                CR_CW_ZCK_COMPRESSION,
                                                NULL, NULL);
@@ -1581,15 +1582,15 @@
       cr_repomdrecordfilltask_free(mmd_fill_task, NULL);
     }
 #endif
 
 
     // Sqlite db
 
-    if (!cmd_options->no_database) {
+    if (cmd_options->database) {
         const char *db_suffix = cr_compression_suffix(cmd_options->db_compression_type);
 
         // Insert XML checksums into the dbs
         cr_db_dbinfo_update(pri_db, pri_xml_rec->checksum, NULL);
         cr_db_dbinfo_update(fil_db, fil_xml_rec->checksum, NULL);
         if (cmd_options->filelists_ext)
             cr_db_dbinfo_update(fex_db, fil_xml_rec->checksum, NULL);
@@ -1803,15 +1804,14 @@
         cr_repomd_record_rename_file(oth_db_rec, NULL);
         cr_repomd_record_rename_file(pri_zck_rec, NULL);
         cr_repomd_record_rename_file(fil_zck_rec, NULL);
         if (cmd_options->filelists_ext)
             cr_repomd_record_rename_file(fex_zck_rec, NULL);
         cr_repomd_record_rename_file(oth_zck_rec, NULL);
         cr_repomd_record_rename_file(groupfile_rec, NULL);
-        cr_repomd_record_rename_file(compressed_groupfile_rec, NULL);
         cr_repomd_record_rename_file(groupfile_zck_rec, NULL);
         cr_repomd_record_rename_file(update_info_rec, NULL);
         cr_repomd_record_rename_file(update_info_zck_rec, NULL);
         cr_repomd_record_rename_file(pkgorigins_rec, NULL);
         cr_repomd_record_rename_file(pkgorigins_zck_rec, NULL);
 
 #ifdef WITH_LIBMODULEMD
@@ -1836,15 +1836,14 @@
     cr_repomd_set_record(repomd_obj, oth_db_rec);
     cr_repomd_set_record(repomd_obj, pri_zck_rec);
     cr_repomd_set_record(repomd_obj, fil_zck_rec);
     if (cmd_options->filelists_ext)
         cr_repomd_set_record(repomd_obj, fex_zck_rec);
     cr_repomd_set_record(repomd_obj, oth_zck_rec);
     cr_repomd_set_record(repomd_obj, groupfile_rec);
-    cr_repomd_set_record(repomd_obj, compressed_groupfile_rec);
     cr_repomd_set_record(repomd_obj, groupfile_zck_rec);
     cr_repomd_set_record(repomd_obj, update_info_rec);
     cr_repomd_set_record(repomd_obj, update_info_zck_rec);
     cr_repomd_set_record(repomd_obj, pkgorigins_rec);
     cr_repomd_set_record(repomd_obj, pkgorigins_zck_rec);
 
 #ifdef WITH_LIBMODULEMD
@@ -2046,41 +2045,23 @@
             struct cr_MetadataLocation *loc;
             loc = (struct cr_MetadataLocation  *) element->data;
             if (!groupfile){
                 if (loc->additional_metadata){
                     GSList *loc_groupfile = (g_slist_find_custom(loc->additional_metadata, "group", cr_cmp_metadatum_type));
                     if (loc_groupfile) {
                         cr_Metadatum *g = loc_groupfile->data;
-                        if (cr_copy_file(g->name, cmd_options->tmp_out_repo, &tmp_err)) {
-                            groupfile = g_strconcat(cmd_options->tmp_out_repo,
-                                    cr_get_filename(g->name),
-                                    NULL);
-                            g_debug("Using groupfile: %s", groupfile);
-                            break;
-                      } else {
-                            g_warning("Groupfile %s from repo: %s cannot be used: %s\n",
-                                    g->name, loc->original_url, tmp_err->message);
-                            g_clear_error(&tmp_err);
-                        }
+                        groupfile = g_strdup(g->name);
+                        break;
                     }
                 }
             }
         }
     } else {
         // Use groupfile specified by user
-        if (cr_copy_file(cmd_options->groupfile, cmd_options->tmp_out_repo, &tmp_err)) {
-            groupfile = g_strconcat(cmd_options->tmp_out_repo,
-                                    cr_get_filename(cmd_options->groupfile),
-                                    NULL);
-            g_debug("Using user specified groupfile: %s", groupfile);
-        } else {
-            g_critical("Cannot copy groupfile %s: %s",
-                       cmd_options->groupfile, tmp_err->message);
-            return 1;
-        }
+        groupfile = g_strdup(cmd_options->groupfile);
     }
 
     // Load noarch repo
 
     cr_Metadata *noarch_metadata = NULL;
     // cr_metadata_hashtable(noarch_metadata):
     //   Key: CR_HT_KEY_FILENAME aka pkg->location_href
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/mergerepo_c.h` & `createrepo_c-1.0.0/tests/createrepo/mergerepo_c.h`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 #include "compression_wrapper.h"
 
 #define DEFAULT_DB_COMPRESSION_TYPE             CR_CW_BZ2_COMPRESSION
-#define DEFAULT_GROUPFILE_COMPRESSION_TYPE      CR_CW_GZ_COMPRESSION
+#define DEFAULT_COMPRESSION_TYPE                CR_CW_ZSTD_COMPRESSION
 
 typedef enum {
     MM_DEFAULT,
     // NA == Name, Arch
     MM_FIRST_FROM_IDENTICAL_NA = MM_DEFAULT,
     MM_NEWEST_FROM_IDENTICAL_NA,
     MM_WITH_HIGHEST_NEVRA,
@@ -79,15 +79,15 @@
 
     char *out_dir;
     char *out_repo;
     char *tmp_out_repo;
     GSList *repo_list;
     GSList *arch_list;
     cr_CompressionType db_compression_type;
-    cr_CompressionType groupfile_compression_type;
+    cr_CompressionType compression_type;
     MergeMethod merge_method;
 };
 
 #ifdef __cplusplus
 }
 #endif
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/metadata_internal.h` & `createrepo_c-1.0.0/tests/createrepo/metadata_internal.h`

 * *Files 16% similar despite different names*

```diff
@@ -42,14 +42,25 @@
  * @return              cr_Error code
  */
 int
 cr_metadata_load_modulemd(ModulemdModuleIndex **moduleindex,
                           gchar *path_to_md,
                           GError **err);
 
+/** Compress groupfile into dest_dir with specified compression.
+ * @param groupfile     Path to local groupfile, it can be already compressed by
+ *                      some compression.
+ * @param dest_dir      Path to directory where the compressed groupfile should be stored.
+ * @return              Path to the new compressed groupfile. Has to be freed by the caller.
+ */
+gchar *
+cr_compress_groupfile(const char *groupfile,
+                      const char *dest_dir,
+                      cr_CompressionType compression);
+
 
 #endif /* WITH_LIBMODULEMD */
 
 #ifdef __cplusplus
 }
 #endif
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/misc.c` & `createrepo_c-1.0.0/tests/createrepo/misc.c`

 * *Files 4% similar despite different names*

```diff
@@ -236,47 +236,58 @@
         return 1;
     }
 
     return 0;
 }
 */
 
-#define VAL_LEN         4       // Len of numeric values in rpm
+#define VAL_LEN         4       // Len of numeric values in rpm (bytes)
 
 struct cr_HeaderRangeStruct
 cr_get_header_byte_range(const char *filename, GError **err)
 {
-    /* Values readed by fread are 4 bytes long and stored as big-endian.
-     * So there is htonl function to convert this big-endian number into host
-     * byte order.
-     */
-
+    // Lead is 96 bytes.
+    //
+    // Each Header starts like this (16 bytes)
+    // 3 bytes for the magic
+    // 1 byte RPM version number - always 1
+    // 4 reserved bytes (no meaning, just padding)
+    // 4 bytes for the number of entries in the index (u32)
+    // 4 bytes for the length of the data section (u32)
+    //
+    // Next comes a series of index entries. Each index entry is 16 bytes
+    // 4 bytes for the tag (u32)
+    // 4 bytes for the tag data type (u32)
+    // 4 bytes for the offset relative to the beginning of the data store
+    // 4 bytes for the count that contains the number of data items pointed to by the index entry
+    //
+    // After the header entries comes the data section. This stores the data pointed to by
+    // the offsets within each index entry.
+    //
+    // All numeric values are big-endian and need to be converted into host byte order.
     struct cr_HeaderRangeStruct results;
 
     assert(!err || *err == NULL);
 
     results.start = 0;
     results.end   = 0;
 
-
     // Open file
-
     FILE *fp = fopen(filename, "rb");
     if (!fp) {
         const gchar * fopen_error = g_strerror(errno);
         g_debug("%s: Cannot open file %s (%s)", __func__, filename,
                 fopen_error);
         g_set_error(err, ERR_DOMAIN, CRE_IO,
                     "Cannot open %s: %s", filename, fopen_error);
         return results;
     }
 
-
     // Get header range
-
+    // Seek to Lead (96) + 8 bytes and read the number of entries in the signature header, then convert to host byte order
     if (fseek(fp, 104, SEEK_SET) != 0) {
         const gchar * fseek_error = g_strerror(errno);
         g_debug("%s: fseek fail on %s (%s)", __func__, filename, fseek_error);
         g_set_error(err, ERR_DOMAIN, CRE_IO,
                     "Cannot seek over %s: %s", filename, fseek_error);
         fclose(fp);
         return results;
@@ -287,58 +298,61 @@
     if (fread(&sigindex, VAL_LEN, 1, fp) != 1) {
         g_set_error(err, ERR_DOMAIN, CRE_IO,
                     "fread() error on %s: %s", filename, g_strerror(errno));
         fclose(fp);
         return results;
     }
     sigindex = htonl(sigindex);
+    // Read the length of the data section and convert to host byte order
     if (fread(&sigdata, VAL_LEN, 1, fp) != 1) {
         g_set_error(err, ERR_DOMAIN, CRE_IO,
                     "fread() error on %s: %s", filename, g_strerror(errno));
         fclose(fp);
         return results;
     }
     sigdata = htonl(sigdata);
 
+    // Lead (96) + HeaderIndex (16) = 112. Index entries are 16 bytes each. Include padding to align to 8 bytes
     unsigned int sigindexsize = sigindex * 16;
     unsigned int sigsize = sigdata + sigindexsize;
     unsigned int disttoboundary = sigsize % 8;
     if (disttoboundary) {
         disttoboundary = 8 - disttoboundary;
     }
     unsigned int hdrstart = 112 + sigsize + disttoboundary;
 
+    // Seek to start of header (96) + 8 bytes and read the number of entries in the header, then convert to host byte order
     fseek(fp, hdrstart, SEEK_SET);
     fseek(fp, 8, SEEK_CUR);
 
     unsigned int hdrindex = 0;
     unsigned int hdrdata  = 0;
     if (fread(&hdrindex, VAL_LEN, 1, fp) != 1) {
         g_set_error(err, ERR_DOMAIN, CRE_IO,
                     "fread() error on %s: %s", filename, g_strerror(errno));
         fclose(fp);
         return results;
     }
     hdrindex = htonl(hdrindex);
+    // Read the length of the data section and convert to host byte order
     if (fread(&hdrdata, VAL_LEN, 1, fp) != 1) {
         g_set_error(err, ERR_DOMAIN, CRE_IO,
                     "fread() error on %s: %s", filename, g_strerror(errno));
         fclose(fp);
         return results;
     }
     hdrdata = htonl(hdrdata);
+    // Calculate the end of the header
     unsigned int hdrindexsize = hdrindex * 16;
     unsigned int hdrsize = hdrdata + hdrindexsize + 16;
     unsigned int hdrend = hdrstart + hdrsize;
 
     fclose(fp);
 
-
     // Check sanity
-
     if (hdrend < hdrstart) {
         g_debug("%s: sanity check fail on %s (%d > %d))", __func__,
                 filename, hdrstart, hdrend);
         g_set_error(err, ERR_DOMAIN, CRE_ERROR,
                     "sanity check error on %s (hdrstart: %d > hdrend: %d)",
                     filename, hdrstart, hdrend);
         return results;
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/misc.h` & `createrepo_c-1.0.0/tests/createrepo/misc.h`

 * *Files 0% similar despite different names*

```diff
@@ -543,15 +543,15 @@
  */
 void
 cr_nevra_free(cr_NEVRA *nevra);
 
 /** Are the files identical?
  * Different paths could point to the same file.
  * This functions checks if both paths point to the same file or not.
- * If one of the files doesn't exists, the funcion doesn't fail
+ * If one of the files doesn't exist, the funcion doesn't fail
  * and just put FALSE into "indentical" value and returns.
  * @param fn1           First path
  * @param fn2           Second path
  * @param identical     Are the files same or not
  * @param err           GError **
  * @return              FALSE if an error was encountered, TRUE otherwise
  */
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/modifyrepo_c.c` & `createrepo_c-1.0.0/tests/createrepo/modifyrepo_c.c`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
     if (options->remove)
         g_debug("Preparing remove-task for: %s", options->remove);
     else
         g_debug("Preparing task for: %s", metadatapath);
 
     if (metadatapath && !g_file_test(metadatapath, G_FILE_TEST_IS_REGULAR)) {
         g_set_error(err, ERR_DOMAIN, CRE_ERROR,
-                    "File \"%s\" is not regular file or doesn't exists",
+                    "File \"%s\" is not regular file or doesn't exist",
                     metadatapath);
         return FALSE;
     }
 
     if (options->remove)
         metadatapath = options->remove;
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/modifyrepo_shared.c` & `createrepo_c-1.0.0/tests/createrepo/modifyrepo_shared.c`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #include "checksum.h"
 #include "modifyrepo_shared.h"
 #include "compression_wrapper.h"
 #include "threads.h"
 #include "xml_dump.h"
 
 #define ERR_DOMAIN              CREATEREPO_C_ERROR
-#define DEFAULT_COMPRESSION     CR_CW_GZ_COMPRESSION
+#define DEFAULT_COMPRESSION     CR_CW_ZSTD_COMPRESSION
 #define DEFAULT_CHECKSUM        CR_CHECKSUM_SHA256
 
 cr_ModifyRepoTask *
 cr_modifyrepotask_new(void)
 {
     cr_ModifyRepoTask *task = g_new0(cr_ModifyRepoTask, 1);
     task->chunk = g_string_chunk_new(16);
@@ -140,15 +140,15 @@
     }
 
     // Parse repomd.xml
 
     gchar *repomd_path = g_build_filename(repopath, "repomd.xml", NULL);
     if (!g_file_test(repomd_path, G_FILE_TEST_IS_REGULAR)) {
         g_set_error(err, ERR_DOMAIN, CRE_IO,
-                    "Regular file \"%s\" doesn't exists", repomd_path);
+                    "Regular file \"%s\" doesn't exist", repomd_path);
         g_free(repomd_path);
         return FALSE;
     }
 
     cr_Repomd *repomd = cr_repomd_new();
     int rc = cr_xml_parse_repomd(repomd_path, repomd, cr_warning_cb,
                                   "Repomd XML parser", err);
@@ -237,15 +237,15 @@
                     g_debug("%s: New name cannot be empty", __func__);
                     cr_repomd_free(repomd);
                     g_free(repomd_path);
                     return FALSE;
                 }
             }
 
-            // Check if record with this name doesn't exists yet
+            // Check if record with this name doesn't exist yet
             if (cr_repomd_get_record(repomd, task->type))
                 g_warning("Record with type \"%s\" already exists "
                           "in repomd.xml", task->type);
 
         }
     }
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/modifyrepo_shared.h` & `createrepo_c-1.0.0/tests/createrepo/modifyrepo_shared.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/package.c` & `createrepo_c-1.0.0/tests/createrepo/package.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/package.h` & `createrepo_c-1.0.0/tests/createrepo/package.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/package_internal.h` & `createrepo_c-1.0.0/tests/createrepo/package_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/parsehdr.c` & `createrepo_c-1.0.0/tests/createrepo/parsehdr.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/parsehdr.h` & `createrepo_c-1.0.0/tests/createrepo/parsehdr.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/parsepkg.c` & `createrepo_c-1.0.0/tests/createrepo/parsepkg.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/parsepkg.h` & `createrepo_c-1.0.0/tests/createrepo/parsepkg.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/CMakeLists.txt` & `createrepo_c-1.0.0/tests/createrepo/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/checksum-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/checksum-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/checksum-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/checksum-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/compression_wrapper-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/compression_wrapper-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/compression_wrapper-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/compression_wrapper-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/contentstat-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/contentstat-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/contentstat-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/contentstat-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/createrepo_c/__init__.py` & `createrepo_c-1.0.0/tests/createrepo/python/createrepo_c/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 
 #: XZ compression alias
 XZ                      = _createrepo_c.XZ_COMPRESSION
 
 #: Zchunk compression alias
 ZCK                     = _createrepo_c.ZCK_COMPRESSION
 
+#: Zstd compression alias
+ZSTD                     = _createrepo_c.ZSTD_COMPRESSION
+
 HT_KEY_DEFAULT  = _createrepo_c.HT_KEY_DEFAULT  #: Default key (hash)
 HT_KEY_HASH     = _createrepo_c.HT_KEY_HASH     #: Package hash as a key
 HT_KEY_NAME     = _createrepo_c.HT_KEY_NAME     #: Package name as a key
 HT_KEY_FILENAME = _createrepo_c.HT_KEY_FILENAME #: Package filename as a key
 
 HT_DUPACT_KEEPFIRST = _createrepo_c.HT_DUPACT_KEEPFIRST #: If an key is duplicated, keep only the first occurrence
 HT_DUPACT_REMOVEALL = _createrepo_c.HT_DUPACT_REMOVEALL #: If an key is duplicated, discard all occurrences
@@ -103,14 +106,15 @@
 PCOR_ENTRY_PRE     = 5 #: PCOR entry tuple index - pre
 
 
 # Tuple indexes for file entry
 FILE_ENTRY_TYPE = 0 #: File entry tuple index - file type
 FILE_ENTRY_PATH = 1 #: File entry tuple index - path
 FILE_ENTRY_NAME = 2 #: File entry tuple index - file name
+FILE_ENTRY_DIGEST = 3 #: File entry tuple index - file digest, present only in filelists-ext
 
 # Tuple indexes for changelog entry
 CHANGELOG_ENTRY_AUTHOR    = 0 #: Changelog entry tuple index - Author
 CHANGELOG_ENTRY_DATE      = 1 #: Changelog entry tuple index - Date
 CHANGELOG_ENTRY_CHANGELOG = 2 #: Changelog entry tuple index - Changelog
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/createrepo_c.egg-info/PKG-INFO` & `createrepo_c-1.0.0/tests/createrepo/python/createrepo_c.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: createrepo-c
-Version: 0.21.1
+Version: 1.0.0
 Summary: C implementation of createrepo
 Home-page: https://github.com/rpm-software-management
 Author: RPM Software Management
 Author-email: rpm-ecosystem@lists.rpm.org
 License: GPLv2+
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/createrepo_c.egg-info/SOURCES.txt` & `createrepo_c-1.0.0/tests/createrepo/python/createrepo_c.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -316,29 +316,33 @@
 tests/python/tests/test_xml_file.py
 tests/python/tests/test_xml_parser.py
 tests/testdata/compressed_files/00_plain.foo0
 tests/testdata/compressed_files/00_plain.foo1
 tests/testdata/compressed_files/00_plain.foo2
 tests/testdata/compressed_files/00_plain.foo3
 tests/testdata/compressed_files/00_plain.foo4
+tests/testdata/compressed_files/00_plain.foo5
 tests/testdata/compressed_files/00_plain.txt
 tests/testdata/compressed_files/00_plain.txt.bz2
 tests/testdata/compressed_files/00_plain.txt.gz
 tests/testdata/compressed_files/00_plain.txt.xz
 tests/testdata/compressed_files/00_plain.txt.zck
+tests/testdata/compressed_files/00_plain.txt.zst
 tests/testdata/compressed_files/01_plain.foo0
 tests/testdata/compressed_files/01_plain.foo1
 tests/testdata/compressed_files/01_plain.foo2
 tests/testdata/compressed_files/01_plain.foo3
 tests/testdata/compressed_files/01_plain.foo4
+tests/testdata/compressed_files/01_plain.foo5
 tests/testdata/compressed_files/01_plain.txt
 tests/testdata/compressed_files/01_plain.txt.bz2
 tests/testdata/compressed_files/01_plain.txt.gz
 tests/testdata/compressed_files/01_plain.txt.xz
 tests/testdata/compressed_files/01_plain.txt.zck
+tests/testdata/compressed_files/01_plain.txt.zst
 tests/testdata/comps_files/comps_00.xml
 tests/testdata/modified_repo_files/bad_file_type-filelists.xml
 tests/testdata/modified_repo_files/error_00-filelists.xml
 tests/testdata/modified_repo_files/error_00-other.xml
 tests/testdata/modified_repo_files/error_00-primary.xml
 tests/testdata/modified_repo_files/long_primary.xml
 tests/testdata/modified_repo_files/missing_type-repomd.xml
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/createrepo_cmodule.c` & `createrepo_c-1.0.0/tests/createrepo/python/createrepo_cmodule.c`

 * *Files 1% similar despite different names*

```diff
@@ -262,14 +262,15 @@
     PyModule_AddIntConstant(m, "AUTO_DETECT_COMPRESSION", CR_CW_AUTO_DETECT_COMPRESSION);
     PyModule_AddIntConstant(m, "UNKNOWN_COMPRESSION", CR_CW_UNKNOWN_COMPRESSION);
     PyModule_AddIntConstant(m, "NO_COMPRESSION", CR_CW_NO_COMPRESSION);
     PyModule_AddIntConstant(m, "GZ_COMPRESSION", CR_CW_GZ_COMPRESSION);
     PyModule_AddIntConstant(m, "BZ2_COMPRESSION", CR_CW_BZ2_COMPRESSION);
     PyModule_AddIntConstant(m, "XZ_COMPRESSION", CR_CW_XZ_COMPRESSION);
     PyModule_AddIntConstant(m, "ZCK_COMPRESSION", CR_CW_ZCK_COMPRESSION);
+    PyModule_AddIntConstant(m, "ZSTD_COMPRESSION", CR_CW_ZSTD_COMPRESSION);
 
     /* Zchunk support */
 #ifdef WITH_ZCHUNK
     PyModule_AddIntConstant(m, "HAS_ZCK", 1);
 #else
     PyModule_AddIntConstant(m, "HAS_ZCK", 0);
 #endif // WITH_ZCHUNK
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/exception-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/exception-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/exception-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/exception-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/load_metadata-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/load_metadata-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/load_metadata-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/load_metadata-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/locate_metadata-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/locate_metadata-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/locate_metadata-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/locate_metadata-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/misc-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/misc-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/misc-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/misc-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/package-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/package-py.c`

 * *Files 1% similar despite different names*

```diff
@@ -427,16 +427,17 @@
     }
     return 0;
 }
 
 static int
 CheckPyPackageFile(PyObject *dep)
 {
-    if (!PyTuple_Check(dep) || PyTuple_Size(dep) != 4) {
-        PyErr_SetString(PyExc_TypeError, "Element of list has to be a tuple with 4 items.");
+    // The fourth element (file checksum) is optional since it is present only in filelists-ext
+    if (!PyTuple_Check(dep) || (PyTuple_Size(dep) != 4 && PyTuple_Size(dep) != 3)) {
+        PyErr_SetString(PyExc_TypeError, "Element of list has to be a tuple with 3 or 4 items.");
         return 1;
     }
     return 0;
 }
 
 static int
 CheckPyChangelogEntry(PyObject *dep)
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/package-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/package-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/parsepkg-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/parsepkg-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/parsepkg-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/parsepkg-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/repomd-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/repomd-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/repomd-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/repomd-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/repomdrecord-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/repomdrecord-py.c`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 {
     if (check_RepomdRecordStatus(self))
         return NULL;
     return Object_FromRepomdRecord(cr_repomd_record_copy(self->record));
 }
 
 PyDoc_STRVAR(fill__doc__,
-"fill() -> None\n\n"
+"fill(checksum_type) -> None\n\n"
 "Fill unfilled items in the RepomdRecord (sizes and checksums)");
 
 static PyObject *
 fill(_RepomdRecordObject *self, PyObject *args)
 {
     int checksum_type;
     GError *err = NULL;
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/repomdrecord-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/repomdrecord-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/sqlite-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/sqlite-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/sqlite-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/sqlite-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/typeconversion.c` & `createrepo_c-1.0.0/tests/createrepo/python/typeconversion.c`

 * *Files 2% similar despite different names*

```diff
@@ -165,21 +165,26 @@
 }
 
 PyObject *
 PyObject_FromPackageFile(cr_PackageFile *file)
 {
     PyObject *tuple;
 
-    if ((tuple = PyTuple_New(4)) == NULL)
-        return NULL;
+    if (file->digest != NULL) {
+        if ((tuple = PyTuple_New(4)) == NULL)
+            return NULL;
+        PyTuple_SetItem(tuple, 3, PyUnicodeOrNone_FromString(file->digest));
+    } else {
+        if ((tuple = PyTuple_New(3)) == NULL)
+            return NULL;
+    }
 
     PyTuple_SetItem(tuple, 0, PyUnicodeOrNone_FromString(file->type));
     PyTuple_SetItem(tuple, 1, PyUnicodeOrNone_FromString(file->path));
     PyTuple_SetItem(tuple, 2, PyUnicodeOrNone_FromString(file->name));
-    PyTuple_SetItem(tuple, 3, PyUnicodeOrNone_FromString(file->digest));
 
     return tuple;
 }
 
 cr_PackageFile *
 PyObject_ToPackageFile(PyObject *tuple, GStringChunk *chunk)
 {
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/typeconversion.h` & `createrepo_c-1.0.0/tests/createrepo/python/typeconversion.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/updatecollection-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/updatecollection-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/updatecollection-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/updatecollection-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/updatecollectionmodule-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/updatecollectionmodule-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/updatecollectionmodule-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/updatecollectionmodule-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/updatecollectionpackage-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/updatecollectionpackage-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/updatecollectionpackage-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/updatecollectionpackage-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/updateinfo-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/updateinfo-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/updateinfo-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/updateinfo-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/updaterecord-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/updaterecord-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/updaterecord-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/updaterecord-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/updatereference-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/updatereference-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/updatereference-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/updatereference-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/xml_dump-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/xml_dump-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/xml_dump-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/xml_dump-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/xml_file-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/xml_file-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/xml_file-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/xml_file-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/xml_parser-py.c` & `createrepo_c-1.0.0/tests/createrepo/python/xml_parser-py.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/python/xml_parser-py.h` & `createrepo_c-1.0.0/tests/createrepo/python/xml_parser-py.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/repomd.c` & `createrepo_c-1.0.0/tests/createrepo/repomd.c`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     GError *tmp_err = NULL;
 
     assert(filename);
     assert(!err || *err == NULL);
 
     if (!g_file_test(filename, G_FILE_TEST_IS_REGULAR)) {
         g_set_error(err, ERR_DOMAIN, CRE_NOFILE,
-                    "File %s doesn't exists or not a regular file", filename);
+                    "File %s doesn't exist or not a regular file", filename);
         return NULL;
     }
 
 
     // Open compressed file
     cr_ContentStat *read_stat = g_malloc0(sizeof(cr_ContentStat));
 
@@ -227,18 +227,18 @@
 
     path = md->location_real;
 
     checksum_str = cr_checksum_name_str(checksum_type);
     checksum_t = checksum_type;
 
     if (!g_file_test(path, G_FILE_TEST_IS_REGULAR)) {
-        // File doesn't exists
-        g_warning("%s: File %s doesn't exists", __func__, path);
+        // File doesn't exist
+        g_warning("%s: File %s doesn't exist", __func__, path);
         g_set_error(err, ERR_DOMAIN, CRE_NOFILE,
-                    "File %s doesn't exists or not a regular file", path);
+                    "File %s doesn't exist or not a regular file", path);
         return CRE_NOFILE;
     }
 
     // Compute checksum of compressed file
 
     if (!md->checksum_type || !md->checksum) {
         gchar *chksum;
@@ -366,18 +366,18 @@
     if (!(record->location_real) || !strlen(record->location_real)) {
         g_set_error(err, ERR_DOMAIN, CRE_BADARG,
                     "Empty locations in repomd record object");
         return CRE_BADARG;
     }
 
     if (!g_file_test(record->location_real, G_FILE_TEST_IS_REGULAR)) {
-        // File doesn't exists
-        g_warning("%s: File %s doesn't exists", __func__, record->location_real);
+        // File doesn't exist
+        g_warning("%s: File %s doesn't exist", __func__, record->location_real);
         g_set_error(err, ERR_DOMAIN, CRE_NOFILE,
-                    "File %s doesn't exists or not a regular file",
+                    "File %s doesn't exist or not a regular file",
                     record->location_real);
         return CRE_NOFILE;;
     }
 
     // Paths
 
     suffix = cr_compression_suffix(record_compression);
```

### Comparing `createrepo_c-0.21.1/tests/createrepo/repomd.h` & `createrepo_c-1.0.0/tests/createrepo/repomd.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/repomd_internal.h` & `createrepo_c-1.0.0/tests/createrepo/repomd_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/sqlite.c` & `createrepo_c-1.0.0/tests/createrepo/sqlite.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/sqlite.h` & `createrepo_c-1.0.0/tests/createrepo/sqlite.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/sqliterepo_c.c` & `createrepo_c-1.0.0/tests/createrepo/sqliterepo_c.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/threads.c` & `createrepo_c-1.0.0/tests/createrepo/threads.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/threads.h` & `createrepo_c-1.0.0/tests/createrepo/threads.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/updateinfo.c` & `createrepo_c-1.0.0/tests/createrepo/updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/updateinfo.h` & `createrepo_c-1.0.0/tests/createrepo/updateinfo.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/version.h.in` & `createrepo_c-1.0.0/tests/createrepo/version.h.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_dump.c` & `createrepo_c-1.0.0/tests/createrepo/xml_dump.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_dump.h` & `createrepo_c-1.0.0/tests/createrepo/xml_dump.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_dump_deltapackage.c` & `createrepo_c-1.0.0/tests/createrepo/xml_dump_deltapackage.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_dump_filelists.c` & `createrepo_c-1.0.0/tests/createrepo/xml_dump_filelists.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_dump_internal.h` & `createrepo_c-1.0.0/tests/createrepo/xml_dump_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_dump_other.c` & `createrepo_c-1.0.0/tests/createrepo/xml_dump_other.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_dump_primary.c` & `createrepo_c-1.0.0/tests/createrepo/xml_dump_primary.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_dump_repomd.c` & `createrepo_c-1.0.0/tests/createrepo/xml_dump_repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_dump_updateinfo.c` & `createrepo_c-1.0.0/tests/createrepo/xml_dump_updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_file.c` & `createrepo_c-1.0.0/tests/createrepo/xml_file.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_file.h` & `createrepo_c-1.0.0/tests/createrepo/xml_file.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_parser.c` & `createrepo_c-1.0.0/tests/createrepo/xml_parser.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_parser.h` & `createrepo_c-1.0.0/tests/createrepo/xml_parser.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_parser_filelists.c` & `createrepo_c-1.0.0/tests/createrepo/xml_parser_filelists.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_parser_internal.h` & `createrepo_c-1.0.0/tests/createrepo/xml_parser_internal.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_parser_main_metadata_together.c` & `createrepo_c-1.0.0/tests/createrepo/xml_parser_main_metadata_together.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_parser_other.c` & `createrepo_c-1.0.0/tests/createrepo/xml_parser_other.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_parser_primary.c` & `createrepo_c-1.0.0/tests/createrepo/xml_parser_primary.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_parser_repomd.c` & `createrepo_c-1.0.0/tests/createrepo/xml_parser_repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/createrepo/xml_parser_updateinfo.c` & `createrepo_c-1.0.0/tests/createrepo/xml_parser_updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/fixtures.h` & `createrepo_c-1.0.0/tests/fixtures.h`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/fixtures.py` & `createrepo_c-1.0.0/tests/python/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_checksum.py` & `createrepo_c-1.0.0/tests/python/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_compression_wrapper.py` & `createrepo_c-1.0.0/tests/python/tests/test_compression_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         self.assertEqual(cr.compression_suffix(cr.NO_COMPRESSION), None)
         self.assertEqual(cr.compression_suffix(123), None)
 
         self.assertEqual(cr.compression_suffix(cr.GZ), ".gz")
         self.assertEqual(cr.compression_suffix(cr.BZ2), ".bz2")
         self.assertEqual(cr.compression_suffix(cr.XZ), ".xz")
         self.assertEqual(cr.compression_suffix(cr.ZCK), ".zck")
+        self.assertEqual(cr.compression_suffix(cr.ZSTD), ".zst")
 
     def test_detect_compression(self):
 
         # no compression
         path = os.path.join(COMPRESSED_FILES_PATH, "01_plain.txt")
         comtype = cr.detect_compression(path)
         self.assertEqual(comtype, cr.NO_COMPRESSION)
@@ -65,16 +66,21 @@
 
         # Disabled because magic module doesn't recognize zchunk files yet
         # Bad suffix - zck compression
         #path = os.path.join(COMPRESSED_FILES_PATH, "01_plain.foo4")
         #comtype = cr.detect_compression(path)
         #self.assertEqual(comtype, cr.ZCK)
 
+        # Bad suffix - zstd compression
+        path = os.path.join(COMPRESSED_FILES_PATH, "01_plain.foo5")
+        comtype = cr.detect_compression(path)
+        self.assertEqual(comtype, cr.ZSTD)
+
     def test_compression_type(self):
         self.assertEqual(cr.compression_type(None), cr.UNKNOWN_COMPRESSION)
         self.assertEqual(cr.compression_type(""), cr.UNKNOWN_COMPRESSION)
         self.assertEqual(cr.compression_type("gz"), cr.GZ)
         self.assertEqual(cr.compression_type("bz2"), cr.BZ2)
         self.assertEqual(cr.compression_type("xz"), cr.XZ)
         self.assertEqual(cr.compression_type("XZ"), cr.XZ)
         self.assertEqual(cr.compression_type("zck"), cr.ZCK)
-
+        self.assertEqual(cr.compression_type("zstd"), cr.ZSTD)
```

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_contentstat.py` & `createrepo_c-1.0.0/tests/python/tests/test_contentstat.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_crfile.py` & `createrepo_c-1.0.0/tests/python/tests/test_crfile.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_load_metadata.py` & `createrepo_c-1.0.0/tests/python/tests/test_load_metadata.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_locate_metadata.py` & `createrepo_c-1.0.0/tests/python/tests/test_locate_metadata.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_misc.py` & `createrepo_c-1.0.0/tests/python/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_package.py` & `createrepo_c-1.0.0/tests/python/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_parsepkg.py` & `createrepo_c-1.0.0/tests/python/tests/test_parsepkg.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         pkg = cr.package_from_rpm(PKG_SUPER_KERNEL_PATH)
         self.assertTrue(pkg)
         self.assertEqual(pkg.name, "super_kernel")
 
         # Test error cases
 
-        # Rpm doesn't exists
+        # Rpm doesn't exist
         self.assertRaises(IOError, cr.package_from_rpm, "this_foo_pkg_should_not_exists.rpm")
 
         # Path is a directory, not a file
         self.assertRaises(IOError, cr.package_from_rpm, "./")
 
         # File is not a rpm
         self.assertRaises(IOError, cr.package_from_rpm, FILE_BINARY_PATH)
@@ -54,15 +54,15 @@
         self.assertTrue(len(xml) == 3)
         self.assertTrue("<name>Archer</name>" in xml[0])
         self.assertTrue('<package pkgid="4e0b775220c67f0f2c1fd2177e626b9c863a098130224ff09778ede25cea9a9e" name="Archer" arch="x86_64">' in xml[1])
         self.assertTrue('<package pkgid="4e0b775220c67f0f2c1fd2177e626b9c863a098130224ff09778ede25cea9a9e" name="Archer" arch="x86_64">' in xml[2])
 
         # Test error cases
 
-        # Rpm doesn't exists
+        # Rpm doesn't exist
         self.assertRaises(IOError, cr.xml_from_rpm, "this_foo_pkg_should_not_exists.rpm")
 
         # Path is a directory, not a file
         self.assertRaises(IOError, cr.xml_from_rpm, "./")
 
         # File is not a rpm
         self.assertRaises(IOError, cr.xml_from_rpm, FILE_BINARY_PATH)
```

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_repomd.py` & `createrepo_c-1.0.0/tests/python/tests/test_repomd.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_repomdrecord.py` & `createrepo_c-1.0.0/tests/python/tests/test_repomdrecord.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_sqlite.py` & `createrepo_c-1.0.0/tests/python/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_updatecollection.py` & `createrepo_c-1.0.0/tests/python/tests/test_updatecollection.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_updatecollectionmodule.py` & `createrepo_c-1.0.0/tests/python/tests/test_updatecollectionmodule.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_updatecollectionpackage.py` & `createrepo_c-1.0.0/tests/python/tests/test_updatecollectionpackage.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_updateinfo.py` & `createrepo_c-1.0.0/tests/python/tests/test_updateinfo.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_updaterecord.py` & `createrepo_c-1.0.0/tests/python/tests/test_updaterecord.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_updatereference.py` & `createrepo_c-1.0.0/tests/python/tests/test_updatereference.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_xml_file.py` & `createrepo_c-1.0.0/tests/python/tests/test_xml_file.py`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/python/tests/test_xml_parser.py` & `createrepo_c-1.0.0/tests/python/tests/test_xml_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                 [('kernel', None, None, None, None, False),
                  ('super_kernel', 'EQ', '0', '5.0.0', None, False),
                  ('super_kernel', 'LT', '0', '4.0.0', None, False)])
         self.assertEqual(pkg.obsoletes,
                 [('kernel', None, None, None, None, False),
                  ('super_kernel', 'EQ', '0', '5.9.0', None, False)])
         self.assertEqual(pkg.files,
-                [(None, '/usr/bin/', 'super_kernel', None)])
+                [(None, '/usr/bin/', 'super_kernel')])
         self.assertEqual(pkg.changelogs, [])
 
     def test_xml_parser_primary_repo01_ampersand(self):
 
         userdata = {
                 "pkgs": [],
                 "pkgcb_calls": 0,
@@ -146,17 +146,17 @@
                 [('kernel', None, None, None, None, False),
                  ('sup&er_kernel', 'EQ', '0', '5.0.0', None, False),
                  ('super_kernel', 'LT', '0', '4.0.0', None, False)])
         self.assertEqual(pkg.obsoletes,
                 [('kernel', None, None, None, None, False),
                  ('super_kernel', 'EQ', '0', '5.9.0', None, False)])
         self.assertEqual(pkg.files,
-                [(None, '/usr/bin&/', 'super_kernel', None),
-                 (None, '/usr/bin/', 'supe&&r_kernel', None),
-                 (None, '/usr/bin/', 'super_kernel', None)])
+                [(None, '/usr/bin&/', 'super_kernel'),
+                 (None, '/usr/bin/', 'supe&&r_kernel'),
+                 (None, '/usr/bin/', 'super_kernel')])
         self.assertEqual(pkg.changelogs, [])
 
     def test_xml_parser_primary_snippet01(self):
 
         userdata = {
                 "pkgs": [],
                 "pkgcb_calls": 0,
@@ -223,15 +223,15 @@
                 [('kernel', None, None, None, None, False),
                  ('super_kernel', 'EQ', '0', '5.0.0', None, False),
                  ('super_kernel', 'LT', '0', '4.0.0', None, False)])
         self.assertEqual(pkg.obsoletes,
                 [('kernel', None, None, None, None, False),
                  ('super_kernel', 'EQ', '0', '5.9.0', None, False)])
         self.assertEqual(pkg.files,
-                [(None, '/usr/bin/', 'super_kernel', None)])
+                [(None, '/usr/bin/', 'super_kernel')])
         self.assertEqual(pkg.changelogs, [])
 
     def test_xml_parser_primary_repo02(self):
 
         userdata = {
                 "pkgs": [],
                 "pkgcb_calls": 0,
@@ -428,16 +428,16 @@
         self.assertEqual(pkg.checksum_type, None)
         self.assertEqual(pkg.files_checksum_type, None)
         self.assertEqual(pkg.requires, [])
         self.assertEqual(pkg.provides, [])
         self.assertEqual(pkg.conflicts, [])
         self.assertEqual(pkg.obsoletes, [])
         self.assertEqual(pkg.files,
-                [(None, '/usr/bin/', 'super_kernel', None),
-                 (None, '/usr/share/man/', 'super_kernel.8.gz', None)])
+                [(None, '/usr/bin/', 'super_kernel'),
+                 (None, '/usr/share/man/', 'super_kernel.8.gz')])
         self.assertEqual(pkg.changelogs, [])
 
     def test_xml_parser_filelists_repo01_ampersand(self):
 
         userdata = {
                 "pkgs": [],
                 "pkgcb_calls": 0,
@@ -490,16 +490,16 @@
         self.assertEqual(pkg.checksum_type, None)
         self.assertEqual(pkg.files_checksum_type, None)
         self.assertEqual(pkg.requires, [])
         self.assertEqual(pkg.provides, [])
         self.assertEqual(pkg.conflicts, [])
         self.assertEqual(pkg.obsoletes, [])
         self.assertEqual(pkg.files,
-                [(None, '/usr/&&bin/', 'super_kernel', None),
-                 (None, '/usr/share/man/', 'super_kernel.8.gz', None)])
+                [(None, '/usr/&&bin/', 'super_kernel'),
+                 (None, '/usr/share/man/', 'super_kernel.8.gz')])
         self.assertEqual(pkg.changelogs, [])
 
     def test_xml_parser_filelists_snippet01(self):
 
         userdata = {
                 "pkgs": [],
                 "pkgcb_calls": 0,
@@ -553,16 +553,16 @@
         self.assertEqual(pkg.checksum_type, None)
         self.assertEqual(pkg.files_checksum_type, None)
         self.assertEqual(pkg.requires, [])
         self.assertEqual(pkg.provides, [])
         self.assertEqual(pkg.conflicts, [])
         self.assertEqual(pkg.obsoletes, [])
         self.assertEqual(pkg.files,
-                [(None, '/usr/bin/', 'super_kernel', None),
-                 (None, '/usr/share/man/', 'super_kernel.8.gz', None)])
+                [(None, '/usr/bin/', 'super_kernel'),
+                 (None, '/usr/share/man/', 'super_kernel.8.gz')])
         self.assertEqual(pkg.changelogs, [])
 
     def test_xml_parser_filelists_repo02(self):
 
         userdata = {
                 "pkgs": [],
                 "pkgcb_calls": 0,
@@ -1211,16 +1211,16 @@
                 [('kernel', None, None, None, None, False),
                  ('super_kernel', 'EQ', '0', '5.0.0', None, False),
                  ('super_kernel', 'LT', '0', '4.0.0', None, False)])
         self.assertEqual(pkg.obsoletes,
                 [('kernel', None, None, None, None, False),
                  ('super_kernel', 'EQ', '0', '5.9.0', None, False)])
         self.assertEqual(pkg.files,
-                [(None, '/usr/bin/', 'super_kernel', None),
-                 (None, '/usr/share/man/', 'super_kernel.8.gz', None)])
+                [(None, '/usr/bin/', 'super_kernel'),
+                 (None, '/usr/share/man/', 'super_kernel.8.gz')])
         self.assertEqual(pkg.changelogs,
                 [('Tomas Mlcoch <tmlcoch@redhat.com> - 6.0.1-1',
                    1334664000,
                   '- First release'),
                  ('Tomas Mlcoch <tmlcoch@redhat.com> - 6.0.1-2',
                    1334664001,
                    '- Second release')])
```

### Comparing `createrepo_c-0.21.1/tests/run_tests.sh.in` & `createrepo_c-1.0.0/tests/run_tests.sh.in`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/test_checksum.c` & `createrepo_c-1.0.0/tests/test_checksum.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/test_compression_wrapper.c` & `createrepo_c-1.0.0/tests/test_compression_wrapper.c`

 * *Files 11% similar despite different names*

```diff
@@ -33,30 +33,34 @@
 
 #define FILE_COMPRESSED_0_CONTENT               ""
 #define FILE_COMPRESSED_0_CONTENT_LEN           0
 #define FILE_COMPRESSED_0_PLAIN                 TEST_COMPRESSED_FILES_PATH"/00_plain.txt"
 #define FILE_COMPRESSED_0_GZ                    TEST_COMPRESSED_FILES_PATH"/00_plain.txt.gz"
 #define FILE_COMPRESSED_0_BZ2                   TEST_COMPRESSED_FILES_PATH"/00_plain.txt.bz2"
 #define FILE_COMPRESSED_0_XZ                    TEST_COMPRESSED_FILES_PATH"/00_plain.txt.xz"
+#define FILE_COMPRESSED_0_ZSTD                  TEST_COMPRESSED_FILES_PATH"/00_plain.txt.zst"
 #define FILE_COMPRESSED_0_PLAIN_BAD_SUFFIX      TEST_COMPRESSED_FILES_PATH"/00_plain.foo0"
 #define FILE_COMPRESSED_0_GZ_BAD_SUFFIX         TEST_COMPRESSED_FILES_PATH"/00_plain.foo1"
 #define FILE_COMPRESSED_0_BZ2_BAD_SUFFIX        TEST_COMPRESSED_FILES_PATH"/00_plain.foo2"
 #define FILE_COMPRESSED_0_XZ_BAD_SUFFIX         TEST_COMPRESSED_FILES_PATH"/00_plain.foo3"
+#define FILE_COMPRESSED_0_ZSTD_BAD_SUFFIX       TEST_COMPRESSED_FILES_PATH"/00_plain.foo5"
 
 #define FILE_COMPRESSED_1_CONTENT               "foobar foobar foobar foobar test test\nfolkjsaflkjsadokf\n"
 #define FILE_COMPRESSED_1_CONTENT_LEN           56
 #define FILE_COMPRESSED_1_PLAIN                 TEST_COMPRESSED_FILES_PATH"/01_plain.txt"
 #define FILE_COMPRESSED_1_GZ                    TEST_COMPRESSED_FILES_PATH"/01_plain.txt.gz"
 #define FILE_COMPRESSED_1_BZ2                   TEST_COMPRESSED_FILES_PATH"/01_plain.txt.bz2"
 #define FILE_COMPRESSED_1_XZ                    TEST_COMPRESSED_FILES_PATH"/01_plain.txt.xz"
+#define FILE_COMPRESSED_1_ZSTD                  TEST_COMPRESSED_FILES_PATH"/01_plain.txt.zst"
 #define FILE_COMPRESSED_1_ZCK                   TEST_COMPRESSED_FILES_PATH"/01_plain.txt.zck"
 #define FILE_COMPRESSED_1_PLAIN_BAD_SUFFIX      TEST_COMPRESSED_FILES_PATH"/01_plain.foo0"
 #define FILE_COMPRESSED_1_GZ_BAD_SUFFIX         TEST_COMPRESSED_FILES_PATH"/01_plain.foo1"
 #define FILE_COMPRESSED_1_BZ2_BAD_SUFFIX        TEST_COMPRESSED_FILES_PATH"/01_plain.foo2"
 #define FILE_COMPRESSED_1_XZ_BAD_SUFFIX         TEST_COMPRESSED_FILES_PATH"/01_plain.foo3"
+#define FILE_COMPRESSED_1_ZSTD_BAD_SUFFIX       TEST_COMPRESSED_FILES_PATH"/01_plain.foo5"
 
 
 static void
 test_cr_contentstat(void)
 {
     cr_ContentStat *cs = NULL;
     GError *tmp_err = NULL;
@@ -94,14 +98,19 @@
     g_assert_cmpstr(suffix, ==, ".gz");
 
     suffix = cr_compression_suffix(CR_CW_BZ2_COMPRESSION);
     g_assert_cmpstr(suffix, ==, ".bz2");
 
     suffix = cr_compression_suffix(CR_CW_XZ_COMPRESSION);
     g_assert_cmpstr(suffix, ==, ".xz");
+
+#ifdef WITH_ZSTD
+    suffix = cr_compression_suffix(CR_CW_ZSTD_COMPRESSION);
+    g_assert_cmpstr(suffix, ==, ".zst");
+#endif // WITH_ZSTD
 }
 
 static void
 test_cr_compression_type(void)
 {
     cr_CompressionType type;
 
@@ -130,14 +139,19 @@
     g_assert_cmpint(type, ==, CR_CW_BZ2_COMPRESSION);
 
     type = cr_compression_type("bzip2");
     g_assert_cmpint(type, ==, CR_CW_BZ2_COMPRESSION);
 
     type = cr_compression_type("xz");
     g_assert_cmpint(type, ==, CR_CW_XZ_COMPRESSION);
+
+#ifdef WITH_ZSTD
+    type = cr_compression_type("zstd");
+    g_assert_cmpint(type, ==, CR_CW_ZSTD_COMPRESSION);
+#endif // WITH_ZSTD
 }
 
 static void
 test_cr_detect_compression(void)
 {
     cr_CompressionType ret;
     GError *tmp_err = NULL;
@@ -173,14 +187,25 @@
 
     ret = cr_detect_compression(FILE_COMPRESSED_0_XZ, &tmp_err);
     g_assert_cmpint(ret, ==, CR_CW_XZ_COMPRESSION);
     g_assert(!tmp_err);
     ret = cr_detect_compression(FILE_COMPRESSED_1_XZ, &tmp_err);
     g_assert_cmpint(ret, ==, CR_CW_XZ_COMPRESSION);
     g_assert(!tmp_err);
+
+#ifdef WITH_ZSTD
+    // Zstd
+
+    ret = cr_detect_compression(FILE_COMPRESSED_0_ZSTD, &tmp_err);
+    g_assert_cmpint(ret, ==, CR_CW_ZSTD_COMPRESSION);
+    g_assert(!tmp_err);
+    ret = cr_detect_compression(FILE_COMPRESSED_1_ZSTD, &tmp_err);
+    g_assert_cmpint(ret, ==, CR_CW_ZSTD_COMPRESSION);
+    g_assert(!tmp_err);
+#endif // WITH_ZSTD
 }
 
 
 static void
 test_cr_detect_compression_bad_suffix(void)
 {
     cr_CompressionType ret;
@@ -217,28 +242,49 @@
 
     ret = cr_detect_compression(FILE_COMPRESSED_0_XZ_BAD_SUFFIX, &tmp_err);
     g_assert_cmpint(ret, ==, CR_CW_XZ_COMPRESSION);
     g_assert(!tmp_err);
     ret = cr_detect_compression(FILE_COMPRESSED_1_XZ_BAD_SUFFIX, &tmp_err);
     g_assert_cmpint(ret, ==, CR_CW_XZ_COMPRESSION);
     g_assert(!tmp_err);
+
+#ifdef WITH_ZSTD
+    // Zstd
+
+    ret = cr_detect_compression(FILE_COMPRESSED_0_ZSTD_BAD_SUFFIX, &tmp_err);
+    g_assert_cmpint(ret, ==, CR_CW_ZSTD_COMPRESSION);
+    g_assert(!tmp_err);
+    ret = cr_detect_compression(FILE_COMPRESSED_1_ZSTD_BAD_SUFFIX, &tmp_err);
+    g_assert_cmpint(ret, ==, CR_CW_ZSTD_COMPRESSION);
+    g_assert(!tmp_err);
+#endif // WITH_ZSTD
 }
 
 
 void
 test_helper_cw_input(const char *filename,
                      cr_CompressionType ctype,
                      const char *content,
                      int len)
 {
     int ret;
     CR_FILE *file;
     char buffer[COMPRESSED_BUFFER_LEN+1];
     GError *tmp_err = NULL;
 
+    if (ctype != CR_CW_AUTO_DETECT_COMPRESSION) {
+        cr_CompressionType detected_type = cr_detect_compression(filename, &tmp_err);
+        g_assert(!tmp_err);
+        if (ctype != detected_type) {
+            printf("detected_type: %i does not match passed type: %i for filename: %s\n",
+                   detected_type, ctype, filename);
+            g_assert(0);
+        }
+    }
+
     file = cr_open(filename, CR_CW_MODE_READ, ctype, &tmp_err);
     g_assert(file);
     g_assert(!tmp_err);
 
     ret = cr_read(file, buffer, COMPRESSED_BUFFER_LEN, &tmp_err);
     g_assert_cmpint(ret, ==, len);
     g_assert(!tmp_err);
@@ -277,14 +323,23 @@
 
     // Xz
 
     test_helper_cw_input(FILE_COMPRESSED_0_XZ, CR_CW_AUTO_DETECT_COMPRESSION,
             FILE_COMPRESSED_0_CONTENT, FILE_COMPRESSED_0_CONTENT_LEN);
     test_helper_cw_input(FILE_COMPRESSED_1_XZ, CR_CW_AUTO_DETECT_COMPRESSION,
             FILE_COMPRESSED_1_CONTENT, FILE_COMPRESSED_1_CONTENT_LEN);
+
+#ifdef WITH_ZSTD
+    // Zstd
+
+    test_helper_cw_input(FILE_COMPRESSED_0_ZSTD, CR_CW_AUTO_DETECT_COMPRESSION,
+            FILE_COMPRESSED_0_CONTENT, FILE_COMPRESSED_0_CONTENT_LEN);
+    test_helper_cw_input(FILE_COMPRESSED_1_ZSTD, CR_CW_AUTO_DETECT_COMPRESSION,
+            FILE_COMPRESSED_1_CONTENT, FILE_COMPRESSED_1_CONTENT_LEN);
+#endif // WITH_ZSTD
 }
 
 
 typedef struct {
     gchar *tmp_filename;
 } Outputtest;
 
@@ -443,14 +498,37 @@
                           FILE_COMPRESSED_1_CONTENT_LEN);
     test_helper_cw_output(OUTPUT_TYPE_PRINTF, outputtest->tmp_filename,
                           CR_CW_XZ_COMPRESSION, FILE_COMPRESSED_0_CONTENT,
                           FILE_COMPRESSED_0_CONTENT_LEN);
     test_helper_cw_output(OUTPUT_TYPE_PRINTF, outputtest->tmp_filename,
                           CR_CW_XZ_COMPRESSION, FILE_COMPRESSED_1_CONTENT,
                           FILE_COMPRESSED_1_CONTENT_LEN);
+
+#ifdef WITH_ZSTD
+    // Zstd
+
+    test_helper_cw_output(OUTPUT_TYPE_WRITE,  outputtest->tmp_filename,
+                          CR_CW_ZSTD_COMPRESSION, FILE_COMPRESSED_0_CONTENT,
+                          FILE_COMPRESSED_0_CONTENT_LEN);
+    test_helper_cw_output(OUTPUT_TYPE_WRITE,  outputtest->tmp_filename,
+                          CR_CW_ZSTD_COMPRESSION, FILE_COMPRESSED_1_CONTENT,
+                          FILE_COMPRESSED_1_CONTENT_LEN);
+    test_helper_cw_output(OUTPUT_TYPE_PUTS,   outputtest->tmp_filename,
+                          CR_CW_ZSTD_COMPRESSION, FILE_COMPRESSED_0_CONTENT,
+                          FILE_COMPRESSED_0_CONTENT_LEN);
+    test_helper_cw_output(OUTPUT_TYPE_PUTS,   outputtest->tmp_filename,
+                          CR_CW_ZSTD_COMPRESSION, FILE_COMPRESSED_1_CONTENT,
+                          FILE_COMPRESSED_1_CONTENT_LEN);
+    test_helper_cw_output(OUTPUT_TYPE_PRINTF, outputtest->tmp_filename,
+                          CR_CW_ZSTD_COMPRESSION, FILE_COMPRESSED_0_CONTENT,
+                          FILE_COMPRESSED_0_CONTENT_LEN);
+    test_helper_cw_output(OUTPUT_TYPE_PRINTF, outputtest->tmp_filename,
+                          CR_CW_ZSTD_COMPRESSION, FILE_COMPRESSED_1_CONTENT,
+                          FILE_COMPRESSED_1_CONTENT_LEN);
+#endif // WITH_ZSTD
 }
 
 
 static void
 test_cr_error_handling(void)
 {
     GError *tmp_err = NULL;
@@ -504,14 +582,23 @@
     f = cr_open("/", CR_CW_MODE_WRITE, CR_CW_XZ_COMPRESSION, &tmp_err);
     g_assert(!f);
     g_assert(tmp_err);
     g_assert_cmpint(tmp_err->code, ==, CRE_XZ);
     g_error_free(tmp_err);
     tmp_err = NULL;
 
+#ifdef WITH_ZSTD
+    f = cr_open("/", CR_CW_MODE_WRITE, CR_CW_ZSTD_COMPRESSION, &tmp_err);
+    g_assert(!f);
+    g_assert(tmp_err);
+    g_assert_cmpint(tmp_err->code, ==, CRE_IO);
+    g_error_free(tmp_err);
+    tmp_err = NULL;
+#endif // WITH_ZSTD
+
     // Opening plain text file as compressed
 
     char buf[256];
     int ret;
 
     // gzread can read compressed as well as uncompressed, so this test
     // is useful.
@@ -546,14 +633,29 @@
     g_assert(tmp_err);
     g_assert_cmpint(tmp_err->code, ==, CRE_XZ);
     g_error_free(tmp_err);
     tmp_err = NULL;
     ret = cr_close(f, &tmp_err);
     g_assert_cmpint(ret, ==, CRE_OK);
     g_assert(!tmp_err);
+
+#ifdef WITH_ZSTD
+    f = cr_open(FILE_COMPRESSED_1_PLAIN, CR_CW_MODE_READ,
+                CR_CW_ZSTD_COMPRESSION, &tmp_err);
+    g_assert(f);
+    ret = cr_read(f, buf, 256, &tmp_err);
+    g_assert_cmpint(ret, ==, -1);
+    g_assert(tmp_err);
+    g_assert_cmpint(tmp_err->code, ==, CRE_ZSTD);
+    g_error_free(tmp_err);
+    tmp_err = NULL;
+    ret = cr_close(f, &tmp_err);
+    g_assert_cmpint(ret, ==, CRE_OK);
+    g_assert(!tmp_err);
+#endif // WITH_ZSTD
 }
 
 
 static void
 test_contentstating_singlewrite(Outputtest *outputtest,
                                 G_GNUC_UNUSED gconstpointer test_data)
 {
@@ -666,14 +768,41 @@
     cr_close(f, &tmp_err);
     g_assert(!tmp_err);
 
     g_assert_cmpint(stat->size, ==, content_len);
     g_assert_cmpstr(stat->checksum, ==, content_sha256);
     cr_contentstat_free(stat, &tmp_err);
     g_assert(!tmp_err);
+
+#ifdef WITH_ZSTD
+    // zstd compression
+    stat = cr_contentstat_new(CR_CHECKSUM_SHA256, &tmp_err);
+    g_assert(stat);
+    g_assert(!tmp_err);
+
+    f = cr_sopen(outputtest->tmp_filename,
+                 CR_CW_MODE_WRITE,
+                 CR_CW_ZSTD_COMPRESSION,
+                 stat,
+                 &tmp_err);
+    g_assert(f);
+    g_assert(!tmp_err);
+
+    ret = cr_write(f, content, content_len, &tmp_err);
+    g_assert_cmpint(ret, ==, content_len);
+    g_assert(!tmp_err);
+
+    cr_close(f, &tmp_err);
+    g_assert(!tmp_err);
+
+    g_assert_cmpint(stat->size, ==, content_len);
+    g_assert_cmpstr(stat->checksum, ==, content_sha256);
+    cr_contentstat_free(stat, &tmp_err);
+    g_assert(!tmp_err);
+#endif // WITH_ZSTD
 }
 
 static void
 test_contentstating_multiwrite(Outputtest *outputtest,
                                G_GNUC_UNUSED gconstpointer test_data)
 {
     CR_FILE *f;
@@ -711,14 +840,46 @@
     cr_close(f, &tmp_err);
     g_assert(!tmp_err);
 
     g_assert_cmpint(stat->size, ==, content_len);
     g_assert_cmpstr(stat->checksum, ==, content_sha256);
     cr_contentstat_free(stat, &tmp_err);
     g_assert(!tmp_err);
+
+#ifdef WITH_ZSTD
+    // Zstd compression
+
+    stat = cr_contentstat_new(CR_CHECKSUM_SHA256, &tmp_err);
+    g_assert(stat);
+    g_assert(!tmp_err);
+
+    f = cr_sopen(outputtest->tmp_filename,
+                 CR_CW_MODE_WRITE,
+                 CR_CW_ZSTD_COMPRESSION,
+                 stat,
+                 &tmp_err);
+    g_assert(f);
+    g_assert(!tmp_err);
+
+    ret = cr_write(f, content, 10, &tmp_err);
+    g_assert_cmpint(ret, ==, 10);
+    g_assert(!tmp_err);
+
+    ret = cr_write(f, content+10, 29, &tmp_err);
+    g_assert_cmpint(ret, ==, 29);
+    g_assert(!tmp_err);
+
+    cr_close(f, &tmp_err);
+    g_assert(!tmp_err);
+
+    g_assert_cmpint(stat->size, ==, content_len);
+    g_assert_cmpstr(stat->checksum, ==, content_sha256);
+    cr_contentstat_free(stat, &tmp_err);
+    g_assert(!tmp_err);
+#endif // WITH_ZSTD
 }
 
 static void
 test_cr_get_zchunk_with_index(void)
 {
     gchar *output;
     CR_FILE *f;
```

### Comparing `createrepo_c-0.21.1/tests/test_koji.c` & `createrepo_c-1.0.0/tests/test_koji.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/test_load_metadata.c` & `createrepo_c-1.0.0/tests/test_load_metadata.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/test_locate_metadata.c` & `createrepo_c-1.0.0/tests/test_locate_metadata.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/test_misc.c` & `createrepo_c-1.0.0/tests/test_misc.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/test_modifyrepo_shared.c` & `createrepo_c-1.0.0/tests/test_modifyrepo_shared.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/test_sqlite.c` & `createrepo_c-1.0.0/tests/test_sqlite.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/test_xml_dump.c` & `createrepo_c-1.0.0/tests/test_xml_dump.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/test_xml_dump_primary.c` & `createrepo_c-1.0.0/tests/test_xml_dump_primary.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/test_xml_file.c` & `createrepo_c-1.0.0/tests/test_xml_file.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/test_xml_parser_filelists.c` & `createrepo_c-1.0.0/tests/test_xml_parser_filelists.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/test_xml_parser_main_metadata_together.c` & `createrepo_c-1.0.0/tests/test_xml_parser_main_metadata_together.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/test_xml_parser_repomd.c` & `createrepo_c-1.0.0/tests/test_xml_parser_repomd.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/test_xml_parser_updateinfo.c` & `createrepo_c-1.0.0/tests/test_xml_parser_updateinfo.c`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/comps_files/comps_00.xml` & `createrepo_c-1.0.0/tests/testdata/comps_files/comps_00.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/bad_file_type-filelists.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/bad_file_type-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/error_00-filelists.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/error_00-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/error_00-other.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/error_00-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/error_00-primary.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/error_00-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/long_primary.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/long_primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/missing_type-repomd.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/missing_type-repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/multiple_warnings_00-filelists.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/multiple_warnings_00-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/multiple_warnings_00-other.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/multiple_warnings_00-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/multiple_warnings_00-primary.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/multiple_warnings_00-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/no_pkgid-other.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/no_pkgid-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/repo_01_ampersand-other.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/repo_01_ampersand-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/repo_01_ampersand-primary.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/repo_01_ampersand-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/repo_02_different_order_filelists.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/repo_02_different_order_filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_00-filelists.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_00-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_00-other.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_00-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_00-primary.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_00-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_01-filelists.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_01-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_01-other.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_01-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_01-primary.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_01-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_02-filelists.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_02-filelists.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_02-other.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_02-other.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/unknown_element_02-primary.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/unknown_element_02-primary.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/modified_repo_files/updateinfo_ampersand.xml` & `createrepo_c-1.0.0/tests/testdata/modified_repo_files/updateinfo_ampersand.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/other_metadata/0402e012013246e7e2f2f638c8a6046efdfd71ae1cbeff9c391d9c1ae5d7d431-comps-f19.xml.bz2` & `createrepo_c-1.0.0/tests/testdata/other_metadata/0402e012013246e7e2f2f638c8a6046efdfd71ae1cbeff9c391d9c1ae5d7d431-comps-f19.xml.bz2`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/other_metadata/36c4f2d6dda3b015b4a7da59552c7c76eff99a59979178513cb51341f6eead44-comps-f19.xml` & `createrepo_c-1.0.0/tests/testdata/other_metadata/36c4f2d6dda3b015b4a7da59552c7c76eff99a59979178513cb51341f6eead44-comps-f19.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/other_metadata/71d988ca33b31a18b0d775478d6f59b40583c794ae76393284850ee97bfba4dc-comps-f19.xml.gz` & `createrepo_c-1.0.0/tests/testdata/other_metadata/71d988ca33b31a18b0d775478d6f59b40583c794ae76393284850ee97bfba4dc-comps-f19.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/other_metadata/c941e2c77a27cdca324c0e0bc3190e134fddddb36a03fb5517e55d156b955205-comps-f19.xml.xz` & `createrepo_c-1.0.0/tests/testdata/other_metadata/c941e2c77a27cdca324c0e0bc3190e134fddddb36a03fb5517e55d156b955205-comps-f19.xml.xz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/other_metadata/comps-f19.xml` & `createrepo_c-1.0.0/tests/testdata/other_metadata/comps-f19.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/packages/Archer-3.4.5-6.x86_64.rpm` & `createrepo_c-1.0.0/tests/testdata/packages/Archer-3.4.5-6.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/packages/Rimmer-1.0.2-2.x86_64.rpm` & `createrepo_c-1.0.0/tests/testdata/packages/Rimmer-1.0.2-2.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/packages/balicek-iso88591-1.1.1-1.x86_64.rpm` & `createrepo_c-1.0.0/tests/testdata/packages/balicek-iso88591-1.1.1-1.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/packages/balicek-iso88592-1.1.1-1.x86_64.rpm` & `createrepo_c-1.0.0/tests/testdata/packages/balicek-iso88592-1.1.1-1.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/packages/balicek-utf8-1.1.1-1.x86_64.rpm` & `createrepo_c-1.0.0/tests/testdata/packages/balicek-utf8-1.1.1-1.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/packages/empty-0-0.src.rpm` & `createrepo_c-1.0.0/tests/testdata/packages/empty-0-0.src.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/packages/empty-0-0.x86_64.rpm` & `createrepo_c-1.0.0/tests/testdata/packages/empty-0-0.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/packages/fake_bash-1.1.1-1.x86_64.rpm` & `createrepo_c-1.0.0/tests/testdata/packages/fake_bash-1.1.1-1.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/packages/super_kernel-6.0.1-2.x86_64.rpm` & `createrepo_c-1.0.0/tests/testdata/packages/super_kernel-6.0.1-2.x86_64.rpm`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_00/repodata/repomd.xml` & `createrepo_c-1.0.0/tests/testdata/repo_00/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_01/repodata/6c662d665c24de9a0f62c17d8fa50622307739d7376f0d19097ca96c6d7f5e3e-primary.xml.gz` & `createrepo_c-1.0.0/tests/testdata/repo_01/repodata/6c662d665c24de9a0f62c17d8fa50622307739d7376f0d19097ca96c6d7f5e3e-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_01/repodata/repomd.xml` & `createrepo_c-1.0.0/tests/testdata/repo_01/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_02/repodata/bcde64b04916a2a72fdc257d61bc922c70b3d58e953499180585f7a360ce86cf-primary.xml.gz` & `createrepo_c-1.0.0/tests/testdata/repo_02/repodata/bcde64b04916a2a72fdc257d61bc922c70b3d58e953499180585f7a360ce86cf-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_02/repodata/repomd.xml` & `createrepo_c-1.0.0/tests/testdata/repo_02/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_03/repodata/a850093e240506c728d6ce26a6fc51d6a7fe10730c67988d13afa7dd82df82d5-modules.yaml.xz` & `createrepo_c-1.0.0/tests/testdata/repo_03/repodata/a850093e240506c728d6ce26a6fc51d6a7fe10730c67988d13afa7dd82df82d5-modules.yaml.xz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_03/repodata/repomd.xml` & `createrepo_c-1.0.0/tests/testdata/repo_03/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_04/repodata/6a5f64dd82a126a161657764fe8f4b4092c0a3b61b9a34bde2af89dc1df112a1-primary.xml.gz` & `createrepo_c-1.0.0/tests/testdata/repo_04/repodata/6a5f64dd82a126a161657764fe8f4b4092c0a3b61b9a34bde2af89dc1df112a1-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_04/repodata/repomd.xml` & `createrepo_c-1.0.0/tests/testdata/repo_04/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_koji_01/repodata/5d039d9ec332d158c69d083f04ac88a187c6b68444472b802eaf0249aec83294-other.xml.gz` & `createrepo_c-1.0.0/tests/testdata/repo_koji_01/repodata/5d039d9ec332d158c69d083f04ac88a187c6b68444472b802eaf0249aec83294-other.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_koji_01/repodata/b153f86915d1dacbb89b244da26e50adb204195262fd3562290de26725daa21d-primary.xml.gz` & `createrepo_c-1.0.0/tests/testdata/repo_koji_01/repodata/b153f86915d1dacbb89b244da26e50adb204195262fd3562290de26725daa21d-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_koji_01/repodata/repomd.xml` & `createrepo_c-1.0.0/tests/testdata/repo_koji_01/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_koji_02/repodata/ee9261d1d2916d841cf24bb01743198ec63ed596f410784602eca2350e430e17-primary.xml.gz` & `createrepo_c-1.0.0/tests/testdata/repo_koji_02/repodata/ee9261d1d2916d841cf24bb01743198ec63ed596f410784602eca2350e430e17-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_koji_02/repodata/feb0b5fdcb0ee1cf981b041f0749ec381145cd9f6b4397991ef5dafcb6807bba-other.xml.gz` & `createrepo_c-1.0.0/tests/testdata/repo_koji_02/repodata/feb0b5fdcb0ee1cf981b041f0749ec381145cd9f6b4397991ef5dafcb6807bba-other.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_koji_02/repodata/repomd.xml` & `createrepo_c-1.0.0/tests/testdata/repo_koji_02/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/0219a2f1f9f32af6b7873905269ac1bc27b03e0caf3968c929a49e5a939e8935-updateinfo_01.xml.gz.zck` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/0219a2f1f9f32af6b7873905269ac1bc27b03e0caf3968c929a49e5a939e8935-updateinfo_01.xml.gz.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/04460bfaf6cb5af6b0925d8c99401a44e5192d287796aed4cced5f7ce881761f-comps.f20.xml` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/04460bfaf6cb5af6b0925d8c99401a44e5192d287796aed4cced5f7ce881761f-comps.f20.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/1e12239bf5cb07ec73c74482c35e80dabe30dbe2fdd57bd9e557d987cbacc8c2-primary.sqlite.bz2` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/1e12239bf5cb07ec73c74482c35e80dabe30dbe2fdd57bd9e557d987cbacc8c2-primary.sqlite.bz2`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.gz.zck` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.gz.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.zck` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/2bbdf70c4394e71c2d3905c143d460009d04359de5a90b72b47cdb9dbdcc079d-comps.f20.xml.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/3d6eaa7c77ef92586470dd6a542478e42cc421a85f12e0db93aa783077704cd0-filelists.xml.zck` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/3d6eaa7c77ef92586470dd6a542478e42cc421a85f12e0db93aa783077704cd0-filelists.xml.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/490a2a494a3827b8a356f728ac36bc02fb009b0eaea173c890e727bb54219037-primary.xml.gz` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/490a2a494a3827b8a356f728ac36bc02fb009b0eaea173c890e727bb54219037-primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/4f4de7d3254a033b84626f330bc6adb8a3c1a4a20f0ddbe30a5692a041318c81-filelists.sqlite.bz2` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/4f4de7d3254a033b84626f330bc6adb8a3c1a4a20f0ddbe30a5692a041318c81-filelists.sqlite.bz2`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/4fbad65c641f4f8fb3cec9b1672fcec2357443e1ea6e93541a0bb559c7dc9238-modules.yaml.gz` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/4fbad65c641f4f8fb3cec9b1672fcec2357443e1ea6e93541a0bb559c7dc9238-modules.yaml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/88514679cb03d8f51e850ad3639c089f899e83407a2380ef9e62873a8eb1db13-updateinfo_01.xml.gz` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/88514679cb03d8f51e850ad3639c089f899e83407a2380ef9e62873a8eb1db13-updateinfo_01.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/8b13cba732c1a02b841f43d6791ca68788d45f376787d9f3ccf68e75f01af499-other.sqlite.bz2` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/8b13cba732c1a02b841f43d6791ca68788d45f376787d9f3ccf68e75f01af499-other.sqlite.bz2`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/ba5a4fdbb20e7b9b70d9a9abd974bcab1065b1e81d711f80e06ad8cae30c4183-filelists.xml.gz` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/ba5a4fdbb20e7b9b70d9a9abd974bcab1065b1e81d711f80e06ad8cae30c4183-filelists.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/c5582e660ed9a2d3c10ba44f0aeb02f2bb70e85dc3c8cda4266183d4e5235aa7-other.xml.zck` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/c5582e660ed9a2d3c10ba44f0aeb02f2bb70e85dc3c8cda4266183d4e5235aa7-other.xml.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/cb0f4b5df8268f248158e50d66ee1565591bca23ee2dbd84ae9c457962fa3122-modules.yaml.gz.zck` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/cb0f4b5df8268f248158e50d66ee1565591bca23ee2dbd84ae9c457962fa3122-modules.yaml.gz.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/e9e6ca4765de75cc3b2bf05e6cf631703c6557edd642300748d7747000547365-primary.xml.zck` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/e9e6ca4765de75cc3b2bf05e6cf631703c6557edd642300748d7747000547365-primary.xml.zck`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/f9d860ddcb64fbdc88a9b71a14ddb9f5670968d5dd3430412565c13d42b6804d-comps.f20.xml.gz` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/f9d860ddcb64fbdc88a9b71a14ddb9f5670968d5dd3430412565c13d42b6804d-comps.f20.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/fd458a424a3f3e0dadc95b806674b79055c24e73637e47ad5a6e57926aa1b9d1-other.xml.gz` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/fd458a424a3f3e0dadc95b806674b79055c24e73637e47ad5a6e57926aa1b9d1-other.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_additional_metadata/repodata/repomd.xml` & `createrepo_c-1.0.0/tests/testdata/repo_with_additional_metadata/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_duplicate_packages/repodata/primary.xml.gz` & `createrepo_c-1.0.0/tests/testdata/repo_with_duplicate_packages/repodata/primary.xml.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repo_with_duplicate_packages/repodata/repomd.xml` & `createrepo_c-1.0.0/tests/testdata/repo_with_duplicate_packages/repodata/repomd.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repodata_snippets/filelists_ext_snippet_02.xml` & `createrepo_c-1.0.0/tests/testdata/repodata_snippets/filelists_ext_snippet_02.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repodata_snippets/other_snippet_02.xml` & `createrepo_c-1.0.0/tests/testdata/repodata_snippets/other_snippet_02.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repodata_snippets/primary_snippet_01.xml` & `createrepo_c-1.0.0/tests/testdata/repodata_snippets/primary_snippet_01.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/repodata_snippets/primary_snippet_02.xml` & `createrepo_c-1.0.0/tests/testdata/repodata_snippets/primary_snippet_02.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/specs/fake-Archer.spec` & `createrepo_c-1.0.0/tests/testdata/specs/fake-Archer.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/specs/fake-Rimmer.spec` & `createrepo_c-1.0.0/tests/testdata/specs/fake-Rimmer.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/specs/fake-balicek-iso88591.spec` & `createrepo_c-1.0.0/tests/testdata/specs/fake-balicek-iso88591.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/specs/fake-balicek-iso88592.spec` & `createrepo_c-1.0.0/tests/testdata/specs/fake-balicek-iso88592.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/specs/fake-balicek-utf8.spec` & `createrepo_c-1.0.0/tests/testdata/specs/fake-balicek-utf8.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/specs/fake-fake_bash.spec` & `createrepo_c-1.0.0/tests/testdata/specs/fake-fake_bash.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/specs/fake-super_kernel.spec` & `createrepo_c-1.0.0/tests/testdata/specs/fake-super_kernel.spec`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/test_files/binary_file` & `createrepo_c-1.0.0/tests/testdata/test_files/binary_file`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/test_files/sqlite_file.sqlite` & `createrepo_c-1.0.0/tests/testdata/test_files/sqlite_file.sqlite`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/test_files/text_file` & `createrepo_c-1.0.0/tests/testdata/test_files/text_file`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/test_files/text_file.gz` & `createrepo_c-1.0.0/tests/testdata/test_files/text_file.gz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/test_files/text_file.xz` & `createrepo_c-1.0.0/tests/testdata/test_files/text_file.xz`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/updateinfo_files/updateinfo_01.xml` & `createrepo_c-1.0.0/tests/testdata/updateinfo_files/updateinfo_01.xml`

 * *Files identical despite different names*

### Comparing `createrepo_c-0.21.1/tests/testdata/updateinfo_files/updateinfo_03.xml` & `createrepo_c-1.0.0/tests/testdata/updateinfo_files/updateinfo_03.xml`

 * *Files identical despite different names*

