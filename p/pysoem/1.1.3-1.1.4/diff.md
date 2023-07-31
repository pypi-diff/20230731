# Comparing `tmp/pysoem-1.1.3.tar.gz` & `tmp/pysoem-1.1.4-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysoem-1.1.3.tar", last modified: Sat Jul 15 07:30:01 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

