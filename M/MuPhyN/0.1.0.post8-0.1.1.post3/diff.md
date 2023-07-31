# Comparing `tmp/MuPhyN-0.1.0.post8.tar.gz` & `tmp/MuPhyN-0.1.1.post3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MuPhyN-0.1.0.post8.tar", last modified: Fri Feb  3 15:52:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

