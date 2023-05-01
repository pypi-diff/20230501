# Comparing `tmp/scarfer-0.3.4.tar.gz` & `tmp/scarfer-0.3.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scarfer-0.3.4.tar", last modified: Tue Jan 24 20:05:51 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

