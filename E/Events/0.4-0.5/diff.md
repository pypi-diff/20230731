# Comparing `tmp/Events-0.4.tar.gz` & `tmp/Events-0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Events-0.4.tar", last modified: Sat Oct 31 12:03:26 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

