# Comparing `tmp/ovos-cli-client-0.0.1.tar.gz` & `tmp/ovos_cli_client-0.0.1a1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-cli-client-0.0.1.tar", last modified: Tue Mar 22 15:09:06 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

