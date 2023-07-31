# Comparing `tmp/bsb-hdf5-0.8.1.tar.gz` & `tmp/bsb_hdf5-0.8.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsb-hdf5-0.8.1.tar", last modified: Tue Jun 13 15:03:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

