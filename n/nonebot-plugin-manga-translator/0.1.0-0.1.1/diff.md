# Comparing `tmp/nonebot_plugin_manga_translator-0.1.0.tar.gz` & `tmp/nonebot_plugin_manga_translator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_manga_translator-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_manga_translator-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_manga_translator-0.1.0.tar` & `nonebot_plugin_manga_translator-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1086 2023-04-28 09:59:46.794856 nonebot_plugin_manga_translator-0.1.0/LICENSE
--rw-r--r--   0        0        0     3124 2023-04-28 10:19:02.057639 nonebot_plugin_manga_translator-0.1.0/nonebot_plugin_manga_translator/__init__.py
--rw-r--r--   0        0        0     3748 2023-04-28 09:32:32.991725 nonebot_plugin_manga_translator-0.1.0/nonebot_plugin_manga_translator/utils.py
--rw-r--r--   0        0        0      529 2023-04-28 10:20:01.091564 nonebot_plugin_manga_translator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3557 2023-04-28 10:24:17.537666 nonebot_plugin_manga_translator-0.1.0/README.md
--rw-r--r--   0        0        0     4214 1970-01-01 00:00:00.000000 nonebot_plugin_manga_translator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-01 18:17:10.001242 nonebot_plugin_manga_translator-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5717 2023-05-01 18:17:10.001242 nonebot_plugin_manga_translator-0.1.1/README.md
+-rw-r--r--   0        0        0     3999 2023-05-01 18:17:10.001242 nonebot_plugin_manga_translator-0.1.1/nonebot_plugin_manga_translator/__init__.py
+-rw-r--r--   0        0        0     5511 2023-05-01 18:17:10.001242 nonebot_plugin_manga_translator-0.1.1/nonebot_plugin_manga_translator/utils.py
+-rw-r--r--   0        0        0      529 2023-05-01 18:17:10.001242 nonebot_plugin_manga_translator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6515 1970-01-01 00:00:00.000000 nonebot_plugin_manga_translator-0.1.1/PKG-INFO
```

