# Comparing `tmp/YMS-0.63.tar.gz` & `tmp/YMS-0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YMS-0.63.tar", last modified: Sun Apr  2 11:42:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

