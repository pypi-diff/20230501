# Comparing `tmp/VDBforGenAI-0.2.tar.gz` & `tmp/VDBforGenAI-0.21-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VDBforGenAI-0.2.tar", last modified: Sat Apr 29 11:31:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

