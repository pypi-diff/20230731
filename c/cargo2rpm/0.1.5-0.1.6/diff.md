# Comparing `tmp/cargo2rpm-0.1.5.tar.gz` & `tmp/cargo2rpm-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cargo2rpm-0.1.5.tar", last modified: Tue Jun 13 00:10:08 2023, max compression
+gzip compressed data, was "cargo2rpm-0.1.6.tar", last modified: Mon Jul 31 09:29:23 2023, max compression
```

## Comparing `cargo2rpm-0.1.5.tar` & `cargo2rpm-0.1.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-06-13 00:10:08.660513 cargo2rpm-0.1.5/
--rw-r--r--   0 deca      (1000) deca      (1000)     1059 2023-02-02 16:39:47.000000 cargo2rpm-0.1.5/LICENSE
--rw-rw-r--   0 deca      (1000) deca      (1000)       50 2023-02-06 21:47:33.000000 cargo2rpm-0.1.5/MANIFEST.in
--rw-r--r--   0 deca      (1000) deca      (1000)     1920 2023-06-13 00:10:08.660513 cargo2rpm-0.1.5/PKG-INFO
--rw-r--r--   0 deca      (1000) deca      (1000)     1142 2023-02-12 23:57:41.000000 cargo2rpm-0.1.5/README.md
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-06-13 00:10:08.657513 cargo2rpm-0.1.5/cargo2rpm/
--rw-r--r--   0 deca      (1000) deca      (1000)      497 2023-06-13 00:08:14.000000 cargo2rpm-0.1.5/cargo2rpm/__init__.py
--rw-r--r--   0 deca      (1000) deca      (1000)     7132 2023-02-14 13:59:22.000000 cargo2rpm-0.1.5/cargo2rpm/__main__.py
--rw-r--r--   0 deca      (1000) deca      (1000)     5010 2023-04-15 10:37:18.000000 cargo2rpm-0.1.5/cargo2rpm/cli.py
--rw-r--r--   0 deca      (1000) deca      (1000)    24552 2023-03-03 16:38:35.000000 cargo2rpm-0.1.5/cargo2rpm/metadata.py
--rw-r--r--   0 deca      (1000) deca      (1000)    15915 2023-06-12 23:49:45.000000 cargo2rpm-0.1.5/cargo2rpm/rpm.py
--rw-r--r--   0 deca      (1000) deca      (1000)    17634 2023-02-12 22:52:52.000000 cargo2rpm-0.1.5/cargo2rpm/semver.py
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-06-13 00:10:08.660513 cargo2rpm-0.1.5/cargo2rpm/testdata/
--rw-r--r--   0 deca      (1000) deca      (1000)     6403 2023-02-04 15:25:02.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/ahash-0.8.3.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2134 2023-06-12 20:40:02.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/aho-corasick-1.0.2.json
--rw-r--r--   0 deca      (1000) deca      (1000)     4690 2023-02-04 15:26:13.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/assert_cmd-2.0.8.json
--rw-r--r--   0 deca      (1000) deca      (1000)     3989 2023-02-04 15:27:28.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/assert_fs-1.0.10.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2177 2023-02-04 11:54:43.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/autocfg-1.1.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     4792 2023-02-04 15:28:23.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/bstr-1.2.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2078 2023-02-04 11:53:09.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/cfg-if-1.0.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)    21085 2023-02-04 15:28:56.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/clap-4.1.4.json
--rw-r--r--   0 deca      (1000) deca      (1000)    19710 2023-02-07 16:19:07.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/fapolicy-analyzer-0.6.8.json
--rw-r--r--   0 deca      (1000) deca      (1000)     6679 2023-02-04 15:29:26.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/gstreamer-0.19.7.json
--rw-r--r--   0 deca      (1000) deca      (1000)     3706 2023-02-04 15:30:03.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/human-panic-1.1.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     7484 2023-02-08 15:04:25.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/hyperfine-1.15.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     5189 2023-06-12 20:41:15.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/iri-string-0.7.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     7821 2023-02-07 16:31:01.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/libblkio-1.2.2.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2126 2023-02-04 11:52:04.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/libc-0.2.139.json
--rw-r--r--   0 deca      (1000) deca      (1000)     4674 2023-02-04 15:30:40.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/predicates-2.1.5.json
--rw-r--r--   0 deca      (1000) deca      (1000)     3363 2023-02-04 11:53:39.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/proc-macro2-1.0.50.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2537 2023-02-04 11:52:34.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/quote-1.0.23.json
--rw-r--r--   0 deca      (1000) deca      (1000)     3523 2023-02-04 11:44:15.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/rand-0.8.5.json
--rw-r--r--   0 deca      (1000) deca      (1000)     1963 2023-02-04 11:45:17.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/rand_core-0.6.4.json
--rw-r--r--   0 deca      (1000) deca      (1000)     6593 2023-06-12 20:40:35.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/regex-1.8.4.json
--rw-r--r--   0 deca      (1000) deca      (1000)     1816 2023-06-12 20:40:57.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/regex-syntax-0.7.2.json
--rw-r--r--   0 deca      (1000) deca      (1000)     4188 2023-02-07 16:26:50.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/rpm-sequoia-1.2.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     9928 2023-02-04 15:31:49.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/rust_decimal-1.28.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)    10741 2023-02-08 12:38:58.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/rustix-0.36.8.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2116 2023-02-04 11:54:11.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/serde-1.0.152.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2562 2023-02-10 16:01:12.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/serde_derive-1.0.152.json
--rw-r--r--   0 deca      (1000) deca      (1000)    10844 2023-02-04 11:36:50.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/syn-1.0.107.json
--rw-r--r--   0 deca      (1000) deca      (1000)     6240 2023-02-04 15:32:38.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/time-0.3.17.json
--rw-r--r--   0 deca      (1000) deca      (1000)    32900 2023-02-08 13:03:00.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/tokio-1.25.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2131 2023-02-04 11:55:18.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/unicode-xid-0.2.4.json
--rw-r--r--   0 deca      (1000) deca      (1000)    12152 2023-02-04 15:33:09.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/zbus-3.8.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)    41849 2023-02-04 15:42:40.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/zola-0.16.1.json
--rw-r--r--   0 deca      (1000) deca      (1000)     6485 2023-02-08 15:04:53.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/zoxide-0.9.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)      766 2023-02-12 21:25:39.000000 cargo2rpm-0.1.5/cargo2rpm/utils.py
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-06-13 00:10:08.657513 cargo2rpm-0.1.5/cargo2rpm.egg-info/
--rw-r--r--   0 deca      (1000) deca      (1000)     1920 2023-06-13 00:10:08.000000 cargo2rpm-0.1.5/cargo2rpm.egg-info/PKG-INFO
--rw-r--r--   0 deca      (1000) deca      (1000)     1697 2023-06-13 00:10:08.000000 cargo2rpm-0.1.5/cargo2rpm.egg-info/SOURCES.txt
--rw-r--r--   0 deca      (1000) deca      (1000)        1 2023-06-13 00:10:08.000000 cargo2rpm-0.1.5/cargo2rpm.egg-info/dependency_links.txt
--rw-r--r--   0 deca      (1000) deca      (1000)       54 2023-06-13 00:10:08.000000 cargo2rpm-0.1.5/cargo2rpm.egg-info/entry_points.txt
--rw-r--r--   0 deca      (1000) deca      (1000)       10 2023-06-13 00:10:08.000000 cargo2rpm-0.1.5/cargo2rpm.egg-info/top_level.txt
--rw-r--r--   0 deca      (1000) deca      (1000)      161 2023-02-02 00:36:19.000000 cargo2rpm-0.1.5/pyproject.toml
--rw-r--r--   0 deca      (1000) deca      (1000)      893 2023-06-13 00:10:08.660513 cargo2rpm-0.1.5/setup.cfg
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-07-31 09:29:23.578802 cargo2rpm-0.1.6/
+-rw-r--r--   0 deca      (1000) deca      (1000)     1059 2023-02-02 16:39:47.000000 cargo2rpm-0.1.6/LICENSE
+-rw-rw-r--   0 deca      (1000) deca      (1000)       50 2023-02-06 21:47:33.000000 cargo2rpm-0.1.6/MANIFEST.in
+-rw-r--r--   0 deca      (1000) deca      (1000)     1920 2023-07-31 09:29:23.578802 cargo2rpm-0.1.6/PKG-INFO
+-rw-r--r--   0 deca      (1000) deca      (1000)     1142 2023-02-12 23:57:41.000000 cargo2rpm-0.1.6/README.md
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-07-31 09:29:23.575802 cargo2rpm-0.1.6/cargo2rpm/
+-rw-r--r--   0 deca      (1000) deca      (1000)      497 2023-07-31 09:27:31.000000 cargo2rpm-0.1.6/cargo2rpm/__init__.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     7132 2023-07-31 09:27:15.000000 cargo2rpm-0.1.6/cargo2rpm/__main__.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     5010 2023-04-15 10:37:18.000000 cargo2rpm-0.1.6/cargo2rpm/cli.py
+-rw-r--r--   0 deca      (1000) deca      (1000)    24552 2023-03-03 16:38:35.000000 cargo2rpm-0.1.6/cargo2rpm/metadata.py
+-rw-r--r--   0 deca      (1000) deca      (1000)    15915 2023-06-12 23:49:45.000000 cargo2rpm-0.1.6/cargo2rpm/rpm.py
+-rw-r--r--   0 deca      (1000) deca      (1000)    23295 2023-07-31 09:05:15.000000 cargo2rpm-0.1.6/cargo2rpm/semver.py
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-07-31 09:29:23.578802 cargo2rpm-0.1.6/cargo2rpm/testdata/
+-rw-r--r--   0 deca      (1000) deca      (1000)     6403 2023-02-04 15:25:02.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/ahash-0.8.3.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2134 2023-06-12 20:40:02.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/aho-corasick-1.0.2.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     4690 2023-02-04 15:26:13.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/assert_cmd-2.0.8.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     3989 2023-02-04 15:27:28.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/assert_fs-1.0.10.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2177 2023-02-04 11:54:43.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/autocfg-1.1.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     4792 2023-02-04 15:28:23.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/bstr-1.2.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2078 2023-02-04 11:53:09.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/cfg-if-1.0.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    21085 2023-02-04 15:28:56.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/clap-4.1.4.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    19710 2023-02-07 16:19:07.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/fapolicy-analyzer-0.6.8.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     6679 2023-02-04 15:29:26.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/gstreamer-0.19.7.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     3706 2023-02-04 15:30:03.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/human-panic-1.1.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     7484 2023-02-08 15:04:25.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/hyperfine-1.15.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     5189 2023-06-12 20:41:15.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/iri-string-0.7.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     7821 2023-02-07 16:31:01.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/libblkio-1.2.2.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2126 2023-02-04 11:52:04.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/libc-0.2.139.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     4674 2023-02-04 15:30:40.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/predicates-2.1.5.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     3363 2023-02-04 11:53:39.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/proc-macro2-1.0.50.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2537 2023-02-04 11:52:34.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/quote-1.0.23.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     3523 2023-02-04 11:44:15.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/rand-0.8.5.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     1963 2023-02-04 11:45:17.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/rand_core-0.6.4.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     6593 2023-06-12 20:40:35.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/regex-1.8.4.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     1816 2023-06-12 20:40:57.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/regex-syntax-0.7.2.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     4188 2023-02-07 16:26:50.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/rpm-sequoia-1.2.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     9928 2023-02-04 15:31:49.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/rust_decimal-1.28.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    10741 2023-02-08 12:38:58.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/rustix-0.36.8.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2116 2023-02-04 11:54:11.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/serde-1.0.152.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2562 2023-02-10 16:01:12.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/serde_derive-1.0.152.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    10844 2023-02-04 11:36:50.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/syn-1.0.107.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     6240 2023-02-04 15:32:38.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/time-0.3.17.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    32900 2023-02-08 13:03:00.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/tokio-1.25.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2131 2023-02-04 11:55:18.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/unicode-xid-0.2.4.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    12152 2023-02-04 15:33:09.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/zbus-3.8.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    41849 2023-02-04 15:42:40.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/zola-0.16.1.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     6485 2023-02-08 15:04:53.000000 cargo2rpm-0.1.6/cargo2rpm/testdata/zoxide-0.9.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)      766 2023-02-12 21:25:39.000000 cargo2rpm-0.1.6/cargo2rpm/utils.py
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-07-31 09:29:23.575802 cargo2rpm-0.1.6/cargo2rpm.egg-info/
+-rw-r--r--   0 deca      (1000) deca      (1000)     1920 2023-07-31 09:29:23.000000 cargo2rpm-0.1.6/cargo2rpm.egg-info/PKG-INFO
+-rw-r--r--   0 deca      (1000) deca      (1000)     1697 2023-07-31 09:29:23.000000 cargo2rpm-0.1.6/cargo2rpm.egg-info/SOURCES.txt
+-rw-r--r--   0 deca      (1000) deca      (1000)        1 2023-07-31 09:29:23.000000 cargo2rpm-0.1.6/cargo2rpm.egg-info/dependency_links.txt
+-rw-r--r--   0 deca      (1000) deca      (1000)       54 2023-07-31 09:29:23.000000 cargo2rpm-0.1.6/cargo2rpm.egg-info/entry_points.txt
+-rw-r--r--   0 deca      (1000) deca      (1000)       10 2023-07-31 09:29:23.000000 cargo2rpm-0.1.6/cargo2rpm.egg-info/top_level.txt
+-rw-r--r--   0 deca      (1000) deca      (1000)      161 2023-02-02 00:36:19.000000 cargo2rpm-0.1.6/pyproject.toml
+-rw-r--r--   0 deca      (1000) deca      (1000)      893 2023-07-31 09:29:23.578802 cargo2rpm-0.1.6/setup.cfg
```

### Comparing `cargo2rpm-0.1.5/LICENSE` & `cargo2rpm-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/PKG-INFO` & `cargo2rpm-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cargo2rpm
-Version: 0.1.5
+Version: 0.1.6
 Summary: Translation layer between cargo and RPM
 Home-page: https://pagure.io/fedora-rust/cargo2rpm
 Author: Fedora Rust SIG
 Author-email: rust@lists.fedoraproject.org
 License: MIT
 Keywords: rpm,cargo,rust
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cargo2rpm-0.1.5/README.md` & `cargo2rpm-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/__main__.py` & `cargo2rpm-0.1.6/cargo2rpm/__main__.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/cli.py` & `cargo2rpm-0.1.6/cargo2rpm/cli.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/metadata.py` & `cargo2rpm-0.1.6/cargo2rpm/metadata.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/rpm.py` & `cargo2rpm-0.1.6/cargo2rpm/rpm.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/semver.py` & `cargo2rpm-0.1.6/cargo2rpm/semver.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This module is a partial Python port of the "semver" crate:
 <https://docs.rs/semver>
 """
 
 from enum import Enum
+import itertools
 import re
 from typing import Optional
 
 
 VERSION_REGEX = re.compile(
     r"""
     ^
@@ -31,14 +32,116 @@
     (-(?P<pre>(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*)(?:\.(?:0|[1-9]\d*|\d*[a-zA-Z-][0-9a-zA-Z-]*))*))?
     $
     """,
     re.VERBOSE,
 )
 
 
+class PreRelease:
+    """
+    Pre-release part of a Version.
+    """
+
+    def __init__(self, parts: list[str | int]):
+        self.parts: list[str | int] = parts
+
+    @staticmethod
+    def parse(prerelease: str) -> "PreRelease":
+        parts = [int(part) if part.isdecimal() else part for part in prerelease.split(".")]
+
+        return PreRelease(parts)
+
+    def __str__(self):
+        return ".".join([str(part) for part in self.parts])
+
+    def __repr__(self):
+        return repr(str(self))
+
+    def __eq__(self, other):
+        if not isinstance(other, PreRelease):
+            return False  # pragma nocover
+
+        return self.parts == other.parts
+
+    def __lt__(self, other):
+        """
+        Algorithm for determining precedence between pre-releases based on the semver.org spec.
+        """
+
+        if not isinstance(other, PreRelease):
+            return False  # pragma nocover
+
+        for (lpart, rpart) in itertools.zip_longest(self.parts, other.parts):
+            match lpart, rpart:
+                # all previous parts were equal and the left pre-release has more parts
+                case l, None:
+                    return False
+
+                # all previous parts were equal and the right pre-release has more parts
+                case None, r:
+                    return True
+
+                # compare nonempty parts depending on value type
+                case l, r:
+                    match isinstance(l, int), isinstance(r, int):
+                        # both parts are numbers: compare numerically
+                        case True, True:
+                            if l < r:
+                                return True
+                            elif l == r:
+                                continue
+                            else:
+                                return False
+
+                        # both parts are strings: compare lexicographically
+                        case False, False:
+                            if l < r:
+                                return True
+                            elif l == r:
+                                continue
+                            else:
+                                return False
+
+                        # number and string: string takes precedence
+                        case True, False:
+                            return True
+
+                        # string and number: string takes precedence
+                        case False, True:
+                            return False
+
+                        case _:  # pragma nocover
+                            raise RuntimeError("Unreachable: This should never happen.")
+
+                case _:  # pragma nocover
+                    raise RuntimeError("Unreachable: This should never happen.")
+
+        # both pre-releases have equal numbers of parts and all pairs of parts are equal
+        else:
+            return False
+
+    def __le__(self, other):
+        if not isinstance(other, PreRelease):
+            return False  # pragma nocover
+
+        return (self == other) or (self < other)
+
+    def __gt__(self, other):
+        if not isinstance(other, PreRelease):
+            return False  # pragma nocover
+
+        return other < self
+
+    def __ge__(self, other):
+        if not isinstance(other, PreRelease):
+            return False  # pragma nocover
+
+        return (self == other) or (self > other)
+
+
 class Version:
     """
     Version that adheres to the "semantic versioning" format.
     """
 
     def __init__(self, major: int, minor: int, patch: int, pre: Optional[str] = None, build: Optional[str] = None):
         self.major: int = major
@@ -83,21 +186,60 @@
     def __repr__(self):
         return repr(str(self))
 
     def __eq__(self, other):
         if not isinstance(other, Version):
             return False  # pragma nocover
 
-        return (
-            self.major == other.major
-            and self.minor == other.minor
-            and self.patch == other.patch
-            and self.pre == other.pre
-            and self.build == other.build
-        )
+        return (self.major == other.major) and (self.minor == other.minor) and (self.patch == other.patch) and (self.pre == other.pre)
+
+    def __lt__(self, other):
+        """
+        Algorithm for determining precedence between versions based on the semver.org spec.
+        """
+
+        if not isinstance(other, Version):
+            return False  # pragma nocover
+
+        if self.major < other.major:
+            return True
+        if self.minor < other.minor:
+            return True
+        if self.patch < other.patch:
+            return True
+
+        match self.pre, other.pre:
+            case None, None:
+                return False
+            case spre, None:
+                return True
+            case None, opre:
+                return False
+            case spre, opre:
+                return PreRelease.parse(spre) < PreRelease.parse(opre)
+            case _:  # pragma nocover
+                raise RuntimeError("Unreachable: This should never happen.")
+
+    def __le__(self, other):
+        if not isinstance(other, Version):
+            return False  # pragma nocover
+
+        return (self == other) or (self < other)
+
+    def __gt__(self, other):
+        if not isinstance(other, Version):
+            return False  # pragma nocover
+
+        return other < self
+
+    def __ge__(self, other):
+        if not isinstance(other, Version):
+            return False  # pragma nocover
+
+        return (self == other) or (self > other)
 
     def to_rpm(self) -> str:
         """
         Formats the `Version` object as an equivalent RPM version string.
         Characters that are invalid in RPM versions are replaced ("-" -> "_")
 
         Build metadata (the optional `Version.build` attribute) is dropped, so
@@ -262,60 +404,72 @@
                         comparators.append(Comparator(Op.GREATER_EQ, self.major, 0, 0, None))
                         comparators.append(Comparator(Op.LESS, self.major + 1, 0, 0, None))
                     case (minor, None):
                         comparators.append(Comparator(Op.GREATER_EQ, self.major, minor, 0, None))
                         comparators.append(Comparator(Op.LESS, self.major, minor + 1, 0, None))
                     case (minor, patch):
                         comparators.append(Comparator(Op.EXACT, self.major, minor, patch, self.pre))
+                    case _:  # pragma nocover
+                        raise RuntimeError("Unreachable: This should never happen.")
 
             case Op.GREATER:
                 match (self.minor, self.patch):
                     case (None, None):
                         comparators.append(Comparator(Op.GREATER_EQ, self.major + 1, 0, 0, None))
                     case (minor, None):
                         comparators.append(Comparator(Op.GREATER_EQ, self.major, minor + 1, 0, None))
                     case (minor, patch):
                         comparators.append(Comparator(Op.GREATER, self.major, minor, patch, self.pre))
+                    case _:  # pragma nocover
+                        raise RuntimeError("Unreachable: This should never happen.")
 
             case Op.GREATER_EQ:
                 match (self.minor, self.patch):
                     case (None, None):
                         comparators.append(Comparator(Op.GREATER_EQ, self.major, 0, 0, None))
                     case (minor, None):
                         comparators.append(Comparator(Op.GREATER_EQ, self.major, minor, 0, None))
                     case (minor, patch):
                         comparators.append(Comparator(Op.GREATER_EQ, self.major, minor, patch, self.pre))
+                    case _:  # pragma nocover
+                        raise RuntimeError("Unreachable: This should never happen.")
 
             case Op.LESS:
                 match (self.minor, self.patch):
                     case (None, None):
                         comparators.append(Comparator(Op.LESS, self.major, 0, 0, None))
                     case (minor, None):
                         comparators.append(Comparator(Op.LESS, self.major, minor, 0, None))
                     case (minor, patch):
                         comparators.append(Comparator(Op.LESS, self.major, minor, patch, self.pre))
+                    case _:  # pragma nocover
+                        raise RuntimeError("Unreachable: This should never happen.")
 
             case Op.LESS_EQ:
                 match (self.minor, self.patch):
                     case (None, None):
                         comparators.append(Comparator(Op.LESS, self.major + 1, 0, 0, None))
                     case (minor, None):
                         comparators.append(Comparator(Op.LESS, self.major, minor + 1, 0, None))
                     case (minor, patch):
                         comparators.append(Comparator(Op.LESS_EQ, self.major, minor, patch, self.pre))
+                    case _:  # pragma nocover
+                        raise RuntimeError("Unreachable: This should never happen.")
 
             case Op.TILDE:
                 match (self.minor, self.patch):
                     case (None, None):
                         comparators.extend(Comparator(Op.EXACT, self.major, None, None, None).normalize())
                     case (minor, None):
                         comparators.extend(Comparator(Op.EXACT, self.major, minor, None, None).normalize())
                     case (minor, patch):
                         comparators.append(Comparator(Op.GREATER_EQ, self.major, minor, patch, self.pre))
                         comparators.append(Comparator(Op.LESS, self.major, minor + 1, 0, None))
+                    case _:  # pragma nocover
+                        raise RuntimeError("Unreachable: This should never happen.")
 
             case Op.CARET:
                 match (self.major, self.minor, self.patch):
                     case (major, None, None):
                         comparators.extend(Comparator(Op.EXACT, major, None, None, None).normalize())
                     case (0, 0, None):
                         comparators.extend(Comparator(Op.EXACT, 0, 0, None, None).normalize())
@@ -325,21 +479,25 @@
                         comparators.extend(Comparator(Op.EXACT, 0, 0, patch, self.pre).normalize())
                     case (0, minor, patch):
                         comparators.append(Comparator(Op.GREATER_EQ, 0, minor, patch, self.pre))
                         comparators.append(Comparator(Op.LESS, 0, minor + 1, 0, None))
                     case (major, minor, patch):
                         comparators.append(Comparator(Op.GREATER_EQ, major, minor, patch, self.pre))
                         comparators.append(Comparator(Op.LESS, major + 1, 0, 0, None))
+                    case _:  # pragma nocover
+                        raise RuntimeError("Unreachable: This should never happen.")
 
             case Op.WILDCARD:
                 match (self.minor, self.patch):
                     case (None, None):
                         comparators.extend(Comparator(Op.EXACT, self.major, None, None, None).normalize())
                     case (minor, None):
                         comparators.extend(Comparator(Op.EXACT, self.major, minor, None, None).normalize())
+                    case _:  # pragma nocover
+                        raise RuntimeError("Unreachable: This should never happen.")
 
             case _:  # pragma nocover
                 raise ValueError(f"Unknown operator: {self.op} (this should never happen)")
 
         return comparators
 
     def to_rpm(self, crate: str, feature: Optional[str]) -> str:
```

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/ahash-0.8.3.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/ahash-0.8.3.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/aho-corasick-1.0.2.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/aho-corasick-1.0.2.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/assert_cmd-2.0.8.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/assert_cmd-2.0.8.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/assert_fs-1.0.10.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/assert_fs-1.0.10.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/autocfg-1.1.0.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/autocfg-1.1.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/bstr-1.2.0.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/bstr-1.2.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/cfg-if-1.0.0.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/cfg-if-1.0.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/clap-4.1.4.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/clap-4.1.4.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/fapolicy-analyzer-0.6.8.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/fapolicy-analyzer-0.6.8.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/gstreamer-0.19.7.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/gstreamer-0.19.7.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/human-panic-1.1.0.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/human-panic-1.1.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/hyperfine-1.15.0.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/hyperfine-1.15.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/iri-string-0.7.0.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/iri-string-0.7.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/libblkio-1.2.2.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/libblkio-1.2.2.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/libc-0.2.139.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/libc-0.2.139.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/predicates-2.1.5.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/predicates-2.1.5.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/proc-macro2-1.0.50.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/proc-macro2-1.0.50.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/quote-1.0.23.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/quote-1.0.23.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/rand-0.8.5.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/rand-0.8.5.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/rand_core-0.6.4.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/rand_core-0.6.4.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/regex-1.8.4.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/regex-1.8.4.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/regex-syntax-0.7.2.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/regex-syntax-0.7.2.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/rpm-sequoia-1.2.0.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/rpm-sequoia-1.2.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/rust_decimal-1.28.0.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/rust_decimal-1.28.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/rustix-0.36.8.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/rustix-0.36.8.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/serde-1.0.152.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/serde-1.0.152.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/serde_derive-1.0.152.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/serde_derive-1.0.152.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/syn-1.0.107.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/syn-1.0.107.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/time-0.3.17.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/time-0.3.17.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/tokio-1.25.0.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/tokio-1.25.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/unicode-xid-0.2.4.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/unicode-xid-0.2.4.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/zbus-3.8.0.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/zbus-3.8.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/zola-0.16.1.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/zola-0.16.1.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/testdata/zoxide-0.9.0.json` & `cargo2rpm-0.1.6/cargo2rpm/testdata/zoxide-0.9.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm/utils.py` & `cargo2rpm-0.1.6/cargo2rpm/utils.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/cargo2rpm.egg-info/PKG-INFO` & `cargo2rpm-0.1.6/cargo2rpm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cargo2rpm
-Version: 0.1.5
+Version: 0.1.6
 Summary: Translation layer between cargo and RPM
 Home-page: https://pagure.io/fedora-rust/cargo2rpm
 Author: Fedora Rust SIG
 Author-email: rust@lists.fedoraproject.org
 License: MIT
 Keywords: rpm,cargo,rust
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cargo2rpm-0.1.5/cargo2rpm.egg-info/SOURCES.txt` & `cargo2rpm-0.1.6/cargo2rpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.5/setup.cfg` & `cargo2rpm-0.1.6/setup.cfg`

 * *Files identical despite different names*

