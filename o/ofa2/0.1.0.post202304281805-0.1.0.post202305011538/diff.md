# Comparing `tmp/ofa2-0.1.0.post202304281805.tar.gz` & `tmp/ofa2-0.1.0.post202305011538-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofa2-0.1.0.post202304281805.tar", last modified: Fri Apr 28 21:05:33 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

