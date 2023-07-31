# Comparing `tmp/staticmap-0.5.5.tar.gz` & `tmp/staticmap-0.5.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staticmap-0.5.5.tar", last modified: Mon Feb 22 09:50:18 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

