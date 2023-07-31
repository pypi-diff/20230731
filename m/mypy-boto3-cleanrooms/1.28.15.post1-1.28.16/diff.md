# Comparing `tmp/mypy-boto3-cleanrooms-1.28.15.post1.tar.gz` & `tmp/mypy_boto3_cleanrooms-1.28.16-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cleanrooms-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

