# Comparing `tmp/pinecone_cli-0.5.1.tar.gz` & `tmp/pinecone_cli-0.5.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone_cli-0.5.1.tar", last modified: Tue Mar 28 18:15:37 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

