# Comparing `tmp/abstract_gui-0.0.51.1.tar.gz` & `tmp/abstract_gui-0.0.51.11-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.51.1.tar", last modified: Sun Jul 30 20:53:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

