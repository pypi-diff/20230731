# Comparing `tmp/pyjson5-1.6.3.tar.gz` & `tmp/pyjson5-1.6.4-cp311-cp311-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjson5-1.6.3.tar", last modified: Fri Jun 23 22:35:50 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

