# Comparing `tmp/xcsf-1.2.6.post1.tar.gz` & `tmp/xcsf-1.2.7-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcsf-1.2.6.post1.tar", last modified: Sun Apr 23 22:55:36 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

