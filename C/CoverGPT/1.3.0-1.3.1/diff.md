# Comparing `tmp/CoverGPT-1.3.0.tar.gz` & `tmp/CoverGPT-1.3.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoverGPT-1.3.0.tar", last modified: Wed Apr 12 20:30:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

