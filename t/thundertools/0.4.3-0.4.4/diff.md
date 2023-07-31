# Comparing `tmp/thundertools-0.4.3.tar.gz` & `tmp/thundertools-0.4.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thundertools-0.4.3.tar", last modified: Tue Jul 18 12:27:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

