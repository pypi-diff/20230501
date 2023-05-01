# Comparing `tmp/mangadex-downloader-2.8.3.tar.gz` & `tmp/mangadex-downloader-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mangadex-downloader-2.8.3.tar", last modified: Tue Mar 14 14:01:05 2023, max compression
+gzip compressed data, was "mangadex-downloader-2.9.0.tar", last modified: Mon May  1 13:06:26 2023, max compression
```

## Comparing `mangadex-downloader-2.8.3.tar` & `mangadex-downloader-2.9.0.tar`

### file list

```diff
@@ -1,103 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:05.570539 mangadex-downloader-2.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-03-14 14:01:05.570539 mangadex-downloader-2.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:05.554539 mangadex-downloader-2.8.3/mangadex_downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/artist_and_author.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:05.558539 mangadex-downloader-2.8.3/mangadex_downloader/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/auth/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/auth/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/auth/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20048 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/chapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:05.558539 mangadex-downloader-2.8.3/mangadex_downloader/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15984 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/cli/args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/cli/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/cli/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/cli/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:05.558539 mangadex-downloader-2.8.3/mangadex_downloader/config/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9881 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/config/auth_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/config/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:05.550539 mangadex-downloader-2.8.3/mangadex_downloader/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:05.558539 mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    23240 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/CREDITS
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:05.562539 mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/otf/
--rw-r--r--   0 runner    (1001) docker     (123)   856800 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSans.otf
--rw-r--r--   0 runner    (1001) docker     (123)   305436 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBold.otf
--rw-r--r--   0 runner    (1001) docker     (123)   233476 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBoldOblique.otf
--rw-r--r--   0 runner    (1001) docker     (123)   473976 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansOblique.otf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:05.566539 mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/ttf/
--rw-r--r--   0 runner    (1001) docker     (123)  1563256 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSans.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   416128 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   342488 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   763696 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansOblique.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:05.570539 mangadex-downloader-2.8.3/mangadex_downloader/format/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22090 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/format/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/format/chinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/format/comic_book.py
--rw-r--r--   0 runner    (1001) docker     (123)    16891 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/format/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)    18146 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/format/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/format/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/format/sevenzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/format/tachiyomi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/format/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/forums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:05.570539 mangadex-downloader-2.8.3/mangadex_downloader/images/
--rw-r--r--   0 runner    (1001) docker     (123)    49604 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/images/mangadex-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/manga.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/mdlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:05.570539 mangadex-downloader-2.8.3/mangadex_downloader/tracker/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:05.570539 mangadex-downloader-2.8.3/mangadex_downloader/tracker/info_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/tracker/info_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/tracker/info_data/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/tracker/info_data/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/tracker/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:05.570539 mangadex-downloader-2.8.3/mangadex_downloader/tracker/sql_files/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/tracker/sql_files/create_ch_info.sql
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/tracker/sql_files/create_file_info.sql
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/tracker/sql_files/create_img_info.sql
--rw-r--r--   0 runner    (1001) docker     (123)     9210 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/tracker/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/tracker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/mangadex_downloader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:01:05.558539 mangadex-downloader-2.8.3/mangadex_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-03-14 14:01:05.000000 mangadex-downloader-2.8.3/mangadex_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-03-14 14:01:05.000000 mangadex-downloader-2.8.3/mangadex_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 14:01:05.000000 mangadex-downloader-2.8.3/mangadex_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-14 14:01:05.000000 mangadex-downloader-2.8.3/mangadex_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-14 14:01:05.000000 mangadex-downloader-2.8.3/mangadex_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-14 14:01:05.000000 mangadex-downloader-2.8.3/mangadex_downloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 14:01:05.570539 mangadex-downloader-2.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-03-14 14:00:46.000000 mangadex-downloader-2.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.660271 mangadex-downloader-2.9.0/mangadex_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/artist_and_author.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.660271 mangadex-downloader-2.9.0/mangadex_downloader/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/auth/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/auth/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/auth/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20378 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/chapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.660271 mangadex-downloader-2.9.0/mangadex_downloader/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21554 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.664271 mangadex-downloader-2.9.0/mangadex_downloader/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/config/auth_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/config/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.656271 mangadex-downloader-2.9.0/mangadex_downloader/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.664271 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    23240 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/CREDITS
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.664271 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/
+-rw-r--r--   0 runner    (1001) docker     (123)   856800 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSans.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   305436 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBold.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   233476 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBoldOblique.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   473976 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansOblique.otf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.668271 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/
+-rw-r--r--   0 runner    (1001) docker     (123)  1563256 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSans.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   416128 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   342488 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   763696 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansOblique.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/mangadex_downloader/format/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22098 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/chinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/comic_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16899 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/sevenzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/tachiyomi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/forums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/mangadex_downloader/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    49604 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/images/mangadex-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/json_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/manga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/mdlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/mangadex_downloader/tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/mangadex_downloader/tracker/info_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/info_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/info_data/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/info_data/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/mangadex_downloader/tracker/sql_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/sql_files/create_ch_info.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/sql_files/create_file_info.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/sql_files/create_img_info.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    10322 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.660271 mangadex-downloader-2.9.0/mangadex_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-01 13:06:26.000000 mangadex-downloader-2.9.0/mangadex_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-01 13:06:26.000000 mangadex-downloader-2.9.0/mangadex_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:06:26.000000 mangadex-downloader-2.9.0/mangadex_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-01 13:06:26.000000 mangadex-downloader-2.9.0/mangadex_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-01 13:06:26.000000 mangadex-downloader-2.9.0/mangadex_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-01 13:06:26.000000 mangadex-downloader-2.9.0/mangadex_downloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/setup.py
```

### Comparing `mangadex-downloader-2.8.3/LICENSE` & `mangadex-downloader-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/PKG-INFO` & `mangadex-downloader-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangadex-downloader
-Version: 2.8.3
+Version: 2.9.0
 Summary: A Command-line tool to download manga from MangaDex, written in Python
 Home-page: https://github.com/mansuf/mangadex-downloader
 Download-URL: https://github.com/mansuf/mangadex-downloader/releases
 Author: Rahman Yusuf
 Author-email: danipart4@gmail.com
 License: MIT
 Keywords: mangadex
@@ -48,15 +48,15 @@
 - [Contributing](#contributing)
 - [Donation](#donation)
 - [Links](#links)
 - [Disclaimer](#disclaimer)
 
 ## Key Features <a id="key-features"></a>
 
-- Download manga, chapter, or list directly from MangaDex
+- Download manga, cover manga, chapter, or list directly from MangaDex
 - Download manga or list from user library
 - Find and download MangaDex URLs from MangaDex forums ([https://forums.mangadex.org/](https://forums.mangadex.org/))
 - Batch download support
 - Old MangaDex url support
 - Scanlation groups filter support
 - Authentication support
 - Control how many chapters and pages you want to download
@@ -176,14 +176,15 @@
 See [CONTRIBUTING.md](https://github.com/mansuf/mangadex-downloader/blob/main/CONTRIBUTING.md) for more info
 
 ## Donation <a id="donation"></a>
 
 If you like this project, please consider donate to one of these websites:
 
 - [Sociabuzz](https://sociabuzz.com/mansuf/donate)
+- [Ko-fi](https://ko-fi.com/rahmanyusuf)
 - [Github Sponsor](https://github.com/sponsors/mansuf)
 
 Any donation amount will be appreciated 💖
 
 ## Links <a id="links"></a>
 
 - [PyPI](https://pypi.org/project/mangadex-downloader/)
```

### Comparing `mangadex-downloader-2.8.3/README.md` & `mangadex-downloader-2.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 - [Contributing](#contributing)
 - [Donation](#donation)
 - [Links](#links)
 - [Disclaimer](#disclaimer)
 
 ## Key Features <a id="key-features"></a>
 
-- Download manga, chapter, or list directly from MangaDex
+- Download manga, cover manga, chapter, or list directly from MangaDex
 - Download manga or list from user library
 - Find and download MangaDex URLs from MangaDex forums ([https://forums.mangadex.org/](https://forums.mangadex.org/))
 - Batch download support
 - Old MangaDex url support
 - Scanlation groups filter support
 - Authentication support
 - Control how many chapters and pages you want to download
@@ -151,14 +151,15 @@
 See [CONTRIBUTING.md](https://github.com/mansuf/mangadex-downloader/blob/main/CONTRIBUTING.md) for more info
 
 ## Donation <a id="donation"></a>
 
 If you like this project, please consider donate to one of these websites:
 
 - [Sociabuzz](https://sociabuzz.com/mansuf/donate)
+- [Ko-fi](https://ko-fi.com/rahmanyusuf)
 - [Github Sponsor](https://github.com/sponsors/mansuf)
 
 Any donation amount will be appreciated 💖
 
 ## Links <a id="links"></a>
 
 - [PyPI](https://pypi.org/project/mangadex-downloader/)
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/__main__.py` & `mangadex-downloader-2.9.0/mangadex_downloader/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/artist_and_author.py` & `mangadex-downloader-2.9.0/mangadex_downloader/artist_and_author.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/auth/base.py` & `mangadex-downloader-2.9.0/mangadex_downloader/auth/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/auth/legacy.py` & `mangadex-downloader-2.9.0/mangadex_downloader/auth/legacy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/auth/oauth2.py` & `mangadex-downloader-2.9.0/mangadex_downloader/auth/oauth2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/chapter.py` & `mangadex-downloader-2.9.0/mangadex_downloader/chapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -414,14 +414,17 @@
         self.log_cache = True if log_cache else False
 
         if Net.mangadex.check_login():
             self._unread_chapters = get_unread_chapters(manga.id)["data"]
         else:
             self._unread_chapters = []
 
+        # To show error message when chapters in specified language is not found
+        self._first_run = True
+
         self._fill_data()
 
     def _parse_groups(self, ids):
         groups = []
 
         for _id in ids:
             group = None
@@ -592,16 +595,22 @@
         return True
 
     def _get_next_chapter(self):
         # Get chapter
         try:
             chap = self.queue.get_nowait()
         except queue.Empty:
+            if self._first_run:
+                raise ChapterNotFound(
+                    f"Manga '{self.manga.title}' has no {self.language.name} chapters"
+                )
+
             raise StopIteration()
 
+        self._first_run = False
         return chap
 
     def __iter__(self) -> "IteratorChapter":
         return self
 
     def __next__(self):
         while True:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/cli/__init__.py` & `mangadex-downloader-2.9.0/mangadex_downloader/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 from ..errors import MangaDexException
 from ..format import deprecated_formats
 
 _deprecated_opts = {
     # I know this isn't deprecated
     # But i need the warning feature, hehe
     "range": "--range is disabled, because it's broken and need to rework",
-    "no_chapter_info": "--no-chapter-info is deprecated and will be removed in v2.9.0. " \
-                       "Please use --use-chapter-cover to enable chapter info (cover) creation"
 }
 
 def check_deprecated_options(log, args):
     for arg, msg in _deprecated_opts.items():
         deprecated = getattr(args, arg)
         if deprecated:
             log.warning(msg)
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/cli/args_parser.py` & `mangadex-downloader-2.9.0/mangadex_downloader/cli/args_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -220,24 +220,14 @@
         '-uct',
         action='store_true',
         help='Use chapter title for each chapters. ' \
              'NOTE: This option is useless if used with any single and volume format.',
         default=config.use_chapter_title
     )
     chap_group.add_argument(
-        '--no-chapter-info',
-        '-nci',
-        action='store_true',
-        help="[Deprecated] Use --use-chapter-cover to enable creation of chapter info. " \
-             "Previously, this option is used to disable creation of chapter info. " \
-             "Because it was automatically enabled when you downloading with any single or volume formats. " \
-             "Now, by default it was disabled. You must use --use-chapter-cover to enable " \
-             "creation of chapter info."
-    )
-    chap_group.add_argument(
         '--range',
         '-rg',
         help='[DISABLED] A range pattern to download specific chapters'
     )
     chap_group.add_argument(
         '--sort-by',
         help='Download sorting method, by default it\'s selected to "volume"',
@@ -452,14 +442,24 @@
     fetch_library_follows_list = urls.startswith('followed-list')
     random = urls.startswith('random')
     group = urls.startswith('group')
     file = urls.startswith('file')
     seasonal = urls.startswith('seasonal')
     thread = is_forum_thread
 
+    cover_art_512px = None
+    cover_art_256px = None
+    cover_art = None
+
+    # Lifehack
+    if urls.startswith('cover'):
+        cover_art_512px = urls.startswith('cover-512px')
+        cover_art_256px = urls.startswith('cover-256px')
+        cover_art = not any([cover_art_256px, cover_art_512px])
+
     # TODO: Add extra checking for -pipe and --search options
 
     setattr(args, "URL", urls)
     setattr(args, 'fetch_library_manga', fetch_library_manga)
     setattr(args, 'fetch_library_list', fetch_library_list)
     setattr(
         args,
@@ -467,9 +467,12 @@
         fetch_library_follows_list
     )
     setattr(args, 'random', random)
     setattr(args, 'fetch_group', group)
     setattr(args, 'file', file)
     setattr(args, 'seasonal', seasonal)
     setattr(args, 'thread', thread)
+    setattr(args, 'cover_art', cover_art)
+    setattr(args, 'cover_art_512px', cover_art_512px)
+    setattr(args, 'cover_art_256px', cover_art_256px)
 
     return parser, args
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/cli/auth.py` & `mangadex-downloader-2.9.0/mangadex_downloader/cli/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/cli/command.py` & `mangadex-downloader-2.9.0/mangadex_downloader/iterator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,573 +16,538 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import sys
+import logging
+import queue
 
-import requests
-from .utils import (
-    Paginator, 
-    dynamic_bars, 
-    IteratorEmpty, 
-    get_key_value, 
-    split_comma_separated
+from .mdlist import MangaDexList
+from .errors import HTTPException, MangaDexException, NotLoggedIn
+from .network import Net, base_url
+from .manga import Manga
+from .fetcher import (
+    get_list,
+    get_legacy_id
 )
-from ..iterator import (
-    IteratorManga,
-    IteratorMangaFromList,
-    IteratorSeasonalManga,
-    IteratorUserLibraryFollowsList,
-    IteratorUserLibraryList,
-    IteratorUserLibraryManga,
-    IteratorUserList,
-    iter_random_manga,
-    ForumThreadMangaDexURLIterator
-)
-from ..forums import (
-    get_thread_title_owner_and_post_owner,
-    get_post_id_forum_thread,
-    validate_forum_thread_url
-)
-from .. import __repository__
-from ..utils import input_handle, validate_url, get_cover_art_url
-from ..errors import InvalidURL, MangaDexException, PillowNotInstalled
-from ..network import Net
-from ..manga import Manga
-from ..chapter import Chapter
-from ..mdlist import MangaDexList
-from ..group import Group
-
-def preview_chapter(chapter: Chapter):
-    try:
-        from PIL import Image
-    except ImportError:
-        raise PillowNotInstalled("Pillow is not installed") from None
-
-    # we're just gonna use chapter info (cover)
-    url = f"https://og.mangadex.org/og-image/chapter/{chapter.id}"
-    r = Net.mangadex.get(url, stream=True)
-    im = Image.open(r.raw)
-
-    print("\nCLOSE THE IMAGE PREVIEW TO CONTINUE\n")
-
-    im.show(str(chapter))
-    im.close()
-
-    pass
-
-def preview_cover_manga(manga):
-    try:
-        from PIL import Image
-    except ImportError:
-        raise PillowNotInstalled("Pillow is not installed") from None
-
-    cover_art_url = get_cover_art_url(manga, manga.cover, "original")
-    r = Net.mangadex.get(cover_art_url, stream=True)
-    im = Image.open(r.raw)
-
-    print("\nCLOSE THE IMAGE PREVIEW TO CONTINUE\n")
-
-    im.show(manga.title)
-    im.close()
-
-def preview_list(mdlist):
-    text_init = f'List of mangas from MangaDex list \"{mdlist.name}\"'
-
-    print('\n')
-    print(text_init)
-    print(dynamic_bars(text_init))
-    for manga in mdlist.iter_manga():
-        print(manga.title)
-    print('\n\n')
-
-class BaseCommand:
-    """A base class that will handle command prompt"""
-    def __init__(self, parser, args, iterator, text, limit=10):
-        self.args_parser = parser
-        self.args = args
-        self.text = text
-        self.paginator = Paginator(iterator, limit)
-        self._text_choices = ""
-
-    def _error(self, message, exit=False):
-        """Function to print error, yes"""
-        msg = f'\nError: {message}\n'
-        if exit:
-            self.args_parser.error(message)
-        else:
-            print(msg)
-
-    def _insert_choices(self, choices, action='next'):
-        text = ""
-        func = getattr(self.paginator, action)
-
-        for pos, item in func():
-            choices[str(pos)] = item
-            text += f"({pos}). {item}\n" 
-
-        self._text_choices = text
-
-    def _print_choices(self):
-        header = dynamic_bars(self.text) + "\n"
-
-        final_text = ""
-        # Title with bars header
-        final_text += header
-        final_text += self.text + "\n"
-        final_text += header
-
-        # Choices
-        final_text += self._text_choices
-
-        # Empty line for separator
-        final_text += "\n"
-
-        # Prompt instruction
-        final_text += 'type "next" to show next results\n'
-        final_text += 'type "previous" to show previous results'
-        if self.preview():
-            final_text += '\ntype "preview NUMBER" to show more details about selected result. ' \
-                          'For example: "preview 2"'
-        
-        print(final_text)
-
-    def preview(self):
-        """Check if this command support preview.
-        
-        Must return ``True`` or ``False``.
-        """
-        return False
-
-    def on_empty_error(self):
-        """This function will be called if :attr:`BaseCommand.iterator` 
-        returns nothing on first prompt.
-        """
-        pass
+from .user import User
+from .filters import Filter
+from .utils import check_blacklisted_tags_manga
+from .cover import CoverArt
+from .forums import iter_md_urls_from_forum_thread
+from .chapter import Chapter
+
+log = logging.getLogger(__name__)
+
+class BaseIterator:
+    def __init__(self):
+        self.queue = queue.Queue()
+        self.offset = 0
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        if self.queue.empty():
+            # Maximum number of results from MangaDex API
+            if self.offset >= 10000:
+                raise StopIteration()
+            else:
+                self.fill_data()
 
-    def on_preview(self, item):
-        """This function is called when command ``preview`` is selected.
-        
-        :func:`BaseCommand.preview()` must return ``True`` in order to get this called.
-        """
-        pass
+        try:
+            return self.next()
+        except queue.Empty:
+            raise StopIteration()
 
-    def _return_from(self, pos):
-        choices = {}
+    def fill_data(self):
+        raise NotImplementedError
 
-        try:
-            self._insert_choices(choices)
-        except IteratorEmpty:
-            self.on_empty_error()
-            return None
+    def next(self):
+        return self.queue.get_nowait()
 
+class MangaIterator(BaseIterator):
+    """Iterator specialized for manga that has abilities like
+    
+    - Filter tags based on environment MANGADEXDL_TAGS_BLACKLIST
+    """
+    def next(self):
         while True:
+            manga = super().next()
 
-            try:
-                result = choices[pos]
-            except KeyError:
-                result = None
-            
-            if result is not None:
-                yield result
-                break
-            elif pos == "*":
-                for item in choices.values():
-                    yield item
-                choices.clear()
-            try:
-                self._insert_choices(choices)
-            except IteratorEmpty:
-                self._error("There are no more results", exit=True)
-            except IndexError:
-                self._error("Choices are out of range, try again")
-
-    def prompt(self, input_pos=None):
-        """Begin ask question to user"""
-        choices = {}
-
-        if input_pos:
-            return self._return_from(input_pos)
+            blacklisted, tags = check_blacklisted_tags_manga(manga)
 
-        # Begin inserting choices for question
-        try:
-            self._insert_choices(choices)
-        except IteratorEmpty:
-            self.on_empty_error()
-            return
+            if blacklisted:
+                log.debug(
+                    f'Not showing manga "{manga.title}", ' \
+                    f'since it contain one or more blacklisted tags {tags}'
+                )
+                continue
+
+            return manga
+
+class SearchFilterError(MangaDexException):
+    def __init__(self, key, msg):
+        text = f"Search filter error '{key}' = {msg}"
+
+        super().__init__(text)
+
+class IteratorManga(MangaIterator):
+    def __init__(
+        self,
+        title,
+        **filters
+    ):
+        super().__init__()
+
+        self.limit = 100
+        self.title = title
+
+        f = Filter()
+        self._param_init = f.get_request_params(**filters)
+
+    def _get_params(self):
+        includes = ['author', 'artist', 'cover_art']
+
+        params = {
+            'includes[]': includes,
+            'title': self.title,
+            'limit': self.limit,
+            'offset': self.offset,
+        }
+        params.update(self._param_init.copy())
+
+        return params
+
+    def fill_data(self):
+        params = self._get_params()
+        url = f'{base_url}/manga'
+        r = Net.mangadex.get(url, params=params)
+        data = r.json()
+
+        if r.status_code >= 400:
+            err = data['errors'][0]['detail']
+            raise MangaDexException(err)
 
-        answer = None
-        while True:
-            if answer is not None:
-                if answer.startswith('preview') and self.preview():
-                    answer_item = answer.split('preview', maxsplit=1)[1].strip()
-                    try:
-                        item = choices[answer_item]
-                    except KeyError:
-                        self._error("Invalid choice, try again")
-                    else:
-                        self.on_preview(item)
-
-                    answer = None
-                    continue
-
-                elif answer.startswith("next"):
-                    action = "next"
-                elif answer.startswith("previous"):
-                    action = "previous"
-                else:
-                    try:
-                        item = choices[answer]
-                    except KeyError:
-                        self._error("Invalid choice, try again")
-                        answer = None
-                    else:
-                        return item
-                
-                if answer is not None:
-                    try:
-                        self._insert_choices(choices, action)
-                    except IteratorEmpty:
-                        self._error("There are no more results")
-                    except IndexError:
-                        self._error("Choices are out of range, try again")
+        items = data['data']
         
-            self._print_choices()
-            answer = input_handle("=> ")
+        for item in items:
+            self.queue.put(Manga(data=item))
 
-class MangaDexCommand(BaseCommand):
-    """Command specialized for MangaDex"""
-    def prompt(self, input_pos=None):
-        answer = super().prompt(input_pos=input_pos)
-
-        def yield_ids():
-            for item in answer:
-                item_id = getattr(item, "id", None)
-                if item_id:
-                    yield item_id
-                else:
-                    yield item
-
-        # "input_pos" argument from prompt() is used
-        if input_pos:
-            return yield_ids()
-        else:
-            return [answer.id]
+        self.offset += len(items)
 
-class MangaCommand(MangaDexCommand):
-    """Command specialized for manga related"""
-    def preview(self):
-        return True
+class IteratorUserLibraryManga(MangaIterator):
+    statuses = [
+        'reading',
+        'on_hold',
+        'plan_to_read',
+        'dropped',
+        're_reading',
+        'completed'
+    ]
 
-    def on_preview(self, item):
-        preview_cover_manga(item)
+    def __init__(self, status=None):
+        super().__init__()
 
-class MDListCommand(MangaDexCommand):
-    """Command specialized for MangaDex list related"""
-    def preview(self):
-        return True
+        self.limit = 100
+        self.offset = 0
 
-    def on_preview(self, item):
-        preview_list(item)
+        if status is not None and status not in self.statuses:
+            raise MangaDexException(f"{status} are not valid status, choices are {set(self.statuses)}")
 
-class MangaLibraryCommand(MangaCommand):
-    """A command that will prompt user to select which manga want to download from user library"""
+        self.status = status
 
-    def __init__(self, parser, args, input_text):
-        _, status = get_key_value(input_text, sep=':')
+        lib = {}
+        for stat in self.statuses:
+            lib[stat] = []
+        self.library = lib
 
-        if not status:
-            # To prevent error "invalid value"
-            status = None
-        elif status == "help":
-            text = "List of statuses filter for user library manga"
+        logged_in = Net.mangadex.check_login()
+        if not logged_in:
+            raise NotLoggedIn("Retrieving user library require login")
 
-            bars = dynamic_bars(text)
+        self._parse_reading_status()
 
-            print(f"{bars}\n{text}\n{bars}")
-            for item in IteratorUserLibraryManga.statuses:
-                print(item)
-            parser.exit(0)
+    def _parse_reading_status(self):
+        r = Net.mangadex.get(f'{base_url}/manga/status')
+        data = r.json()
 
-        user = Net.mangadex.user
+        for manga_id, status in data['statuses'].items():
+            self.library[status].append(manga_id)
 
-        super().__init__(
-            parser,
-            args,
-            IteratorUserLibraryManga(status),
-            f'List of manga from user library "{user.name}"'
-        )
+    def _check_status(self, manga):
+        if self.status is None:
+            return True
 
-        self.user = user
+        manga_ids = self.library[self.status]
+        return manga.id in manga_ids
 
-    def on_empty_error(self):
-        self.args_parser.error(f'User "{self.user.name}"')
+    def next(self) -> Manga:
+        while True:
+            manga = super().next()
 
-class ListLibraryCommand(MDListCommand):
-    """A command that will prompt user to select which list want to download from user library"""
-    def __init__(self, parser, args, input_text):
-        _, user = get_key_value(input_text, sep=':')
+            if not self._check_status(manga):
+                # Filter is used
+                continue
+            
+            return manga
 
-        user_id = None
-        if user:
-            try:
-                user_id = validate_url(user)
-            except InvalidURL as e:
-                parser.error(f'"{user}" is not a valid user')
+    def fill_data(self):
+        includes = [
+            'artist', 'author', 'cover_art'
+        ]
+        params = {
+            'includes[]': includes,
+            'limit': self.limit,
+            'offset': self.offset,
+        }
+        url = f'{base_url}/user/follows/manga'
+        r = Net.mangadex.get(url, params=params)
+        data = r.json()
+
+        items = data['data']
+
+        for item in items:
+            self.queue.put(Manga(data=item))
         
-        if user:
-            iterator = IteratorUserList(user_id)
+        self.offset += len(items)
+
+class IteratorMangaFromList(MangaIterator):
+    def __init__(self, _id=None, data=None):
+        if _id is None and data is None:
+            raise ValueError("atleast provide _id or data")
+        elif _id and data:
+            raise ValueError("_id and data cannot be together")
+
+        super().__init__()
+
+        self.id = _id
+        self.data = data
+        self.limit = 100
+        self.name = None # type: str
+        self.user = None # type: User
+
+        self.manga_ids = []
+
+        self._parse_list()
+
+    def _parse_list(self):
+        if self.id:
+            data = get_list(self.id)['data']
         else:
-            iterator = IteratorUserLibraryList()
-        
-        try:
-            user = iterator.user
-        except AttributeError:
-            # Logged in user
-            user = Net.mangadex.user
-
-        super().__init__(
-            parser,
-            args,
-            iterator,
-            f'List of saved MDList from user "{user.name}"'
-        )
+            data = self.data
 
-        self.user = user
+        self.name = data['attributes']['name']
+        
+        for rel in data['relationships']:
+            _type = rel['type']
+            _id = rel['id']
+            if _type == 'manga':
+                self.manga_ids.append(_id)
+            elif _type == 'user':
+                self.user = User(_id)
     
-    def on_empty_error(self):
-        self.args_parser.error(f'User "{self.user.name} has no saved lists"')
-
-class FollowedListLibraryCommand(MDListCommand):
-    """A command that will prompt user to select which list want to download from followed lists user """
+    def fill_data(self):
+        ids = self.manga_ids
+        includes = ['author', 'artist', 'cover_art']
+        content_ratings = [
+            'safe',
+            'suggestive',
+            'erotica',
+            'pornographic' # Filter porn content will be done in next()
+        ]
+
+        limit = self.limit
+        if ids:
+            param_ids = ids[:limit]
+            del ids[:len(param_ids)]
+            params = {
+                'includes[]': includes,
+                'limit': limit,
+                'contentRating[]': content_ratings,
+                'ids[]': param_ids
+            }
+            url = f'{base_url}/manga'
+            r = Net.mangadex.get(url, params=params)
+            data = r.json()
+
+            notexist_ids = param_ids.copy()
+            copy_data = data.copy()
+            for manga_data in copy_data['data']:
+                manga = Manga(data=manga_data)
+                if manga.id in notexist_ids:
+                    notexist_ids.remove(manga.id)
+            
+            if notexist_ids:
+                for manga_id in notexist_ids:
+                    log.warning(f'There is ghost (not exist) manga = {manga_id} in list {self.name}')
+
+            for manga_data in data['data']:
+                self.queue.put(Manga(data=manga_data))
+
+class IteratorUserLibraryList(BaseIterator):
+    def __init__(self):
+        super().__init__()
+
+        self.limit = 100
+        self.offset = 0
+
+        logged_in = Net.mangadex.check_login()
+        if not logged_in:
+            raise NotLoggedIn("Retrieving user library require login")
+
+    def fill_data(self):
+        params = {
+            'limit': self.limit,
+            'offset': self.offset,
+        }
+        url = f'{base_url}/user/list'
+        r = Net.mangadex.get(url, params=params)
+        data = r.json()
 
-    def __init__(self, parser, args, input_text):
-        iterator = IteratorUserLibraryFollowsList()
+        items = data['data']
 
-        user = Net.mangadex.user
+        for item in items:
+            self.queue.put(MangaDexList(data=item))
+        
+        self.offset += len(items)
 
-        super().__init__(
-            parser,
-            args,
-            iterator,
-            f'List of followed MDlist from user "{user.name}"'
-        )
+class IteratorUserList(BaseIterator):
+    def __init__(self, _id=None):
+        super().__init__()
 
-        self.user = user
+        self.limit = 100
+        self.user = User(_id)
     
-    def on_empty_error(self):
-        self.args_parser.error(f'User "{self.user.name}" has no followed lists')
+    def fill_data(self):
+        params = {
+            'limit': self.limit,
+            'offset': self.offset,
+            
+        }
+        url = f'{base_url}/user/{self.user.id}/list'
+        try:
+            r = Net.mangadex.get(url, params=params)
+        except HTTPException:
+            # Some users are throwing server error (Bad gateway)
+            # MD devs said it was cache and headers issues
+            # Reference: https://api.mangadex.org/user/10dbf775-1935-4f89-87a5-a1f4e64d9d94/list
+            # For now the app will throw error and tell the user cannot be fetched until it's get fixed
+
+            # HTTPException from session only giving "server throwing ... code" message
+            raise HTTPException(
+                f"An error occured when getting mdlists from user \"{self.user.id}\". " \
+                f"The app cannot fetch all MangaDex lists from user \"{self.user.id}\" " \
+                "because of server error. The only solution is to wait until this get fixed " \
+                "from MangaDex itself."
+            ) from None
 
-class FilterEnabled:
-    @classmethod
-    def parse_filter(cls, args):
-        # Parse filters
-        orders = {}
-        filter_kwargs = {}
-        filters = args.filter or []
-        for f in filters:
-            key, value  = get_key_value(f)
-            try:
-                value_filter_kwargs = filter_kwargs[key]
-            except KeyError:
-                filter_kwargs[key] = split_comma_separated(value)
-            else:
-                # Found duplicate filter with different value
-                if isinstance(value_filter_kwargs, str):
-                    new_values = [value_filter_kwargs]
-                else:
-                    new_values = value_filter_kwargs
-
-                values = split_comma_separated(value, single_value_to_list=True)
-                new_values.extend(values)
-
-                filter_kwargs[key] = new_values
-
-        # We cannot put "order[key]" into function parameters
-        # that would cause syntax error
-        for key in filter_kwargs.keys():
-            if 'order' in key:
-                orders[key] = filter_kwargs[key]
-
-        # Remove "order[key]" from filter_kwargs
-        # to avoid syntax error
-        for key in orders.keys():
-            filter_kwargs.pop(key)
-
-        # This much safer
-        if orders:
-            filter_kwargs['order'] = orders
-
-        return filter_kwargs
-
-class SearchMangaCommand(MangaCommand, FilterEnabled):
-    """A command that will prompt user to select which manga to download (from search)"""
-    def __init__(self, parser, args, input_text):
-        filter_kwargs = self.parse_filter(args)
-
-        iterator = IteratorManga(input_text, **filter_kwargs)
-        super().__init__(
-            parser,
-            args,
-            iterator,
-            f'Manga search results for "{input_text}"'
-        )
+        data = r.json()
+
+        items = data['data']
+
+        for item in items:
+            self.queue.put(MangaDexList(data=item))
         
-        self.input_text = input_text
-    
-    def on_empty_error(self):
-        self.args_parser.error(f'Manga search results for "{self.input_text}" are empty')
+        self.offset += len(items)
+
+class IteratorUserLibraryFollowsList(BaseIterator):
+    def __init__(self):
+        super().__init__()
+
+        self.limit = 100
+
+        logged_in = Net.mangadex.check_login()
+        if not logged_in:
+            raise NotLoggedIn("Retrieving user library require login")
+
+    def fill_data(self):
+        params = {
+            'limit': self.limit,
+            'offset': self.offset,
+        }
+        url = f'{base_url}/user/follows/list'
+        r = Net.mangadex.get(url, params=params)
+        data = r.json()
 
-class GroupMangaCommand(MangaCommand):
-    """A command that will prompt user to select which manga to download (from scanlator group)"""
-    def __init__(self, parser, args, input_text):
-        # Getting group id
-        _, group_id = get_key_value(input_text, sep=':')
-        if not group_id:
-            parser.error("group id or url are required")
+        items = data['data']
+
+        for item in items:
+            self.queue.put(MangaDexList(data=item))
         
-        group_id = validate_url(group_id)
-        group = Group(group_id)
+        self.offset += len(items)
+
+class IteratorSeasonalManga(IteratorMangaFromList):
+    owner_list = 'd2ae45e0-b5e2-4e7f-a688-17925c2d7d6b'
 
-        iterator = IteratorManga(None, group=group.id)
-        text = f'List of manga from group "{group.name}"'
+    def __init__(self, season):
+        seasons = self._get_seasons()
 
-        super().__init__(
-            parser,
-            args,
-            iterator,
-            text
-        )
+        try:
+            mdlist = seasons[season]
+        except KeyError:
+            raise MangaDexException(f"invalid season, available choices are {list(seasons.keys())}")
         
-        self.group = group
+        super().__init__(mdlist.id)
 
-    def on_empty_error(self):
-        self.args_parser.error(f'Group "{self.group.name}" has no uploaded mangas')
+    @classmethod
+    def _get_seasons(self):
+        seasons = {}
+        for mdlist in IteratorUserList(self.owner_list):
+            name = mdlist.name.lower().replace('seasonal: ', '')
+            seasons[name] = mdlist
+        
+        return seasons
 
-class RandomMangaCommand(MangaCommand, FilterEnabled):
-    def __init__(self, parser, args, input_text):
-        _, value = get_key_value(input_text, sep=':')
-
-        if value:
-            raise MangaDexException(
-                "Syntax 'random:<content_rating>' are no longer supported, " \
-                "use --filter or -ft instead."
+def iter_random_manga(**filters):
+    ids = []
+    f = Filter([
+        'content_rating',
+        'included_tags',
+        'included_tags_mode',
+        'excluded_tags',
+        'excluded_tags_mode'
+    ])
+    filter_params = f.get_request_params(**filters)
+    while True:
+        params = {
+            'includes[]': ['author', 'artist', 'cover_art'],
+        }
+        params.update(**filter_params)
+        r = Net.mangadex.get(f'{base_url}/manga/random', params=params)
+        data = r.json()['data']
+        manga = Manga(data=data)
+
+        blacklisted, tags = check_blacklisted_tags_manga(manga)
+
+        if blacklisted:
+            log.debug(
+                f'Not showing manga "{manga.title}", ' \
+                f'since it contain one or more blacklisted tags {tags}'
             )
+            continue
+
+        if manga.id not in ids:
+            # Make sure it's not duplicated manga
+            ids.append(manga.id)
+            yield manga
+
+        continue
+
+# For some reason, "/cover" endpoint has result limit for each responses.
+# This class is used for getting all covers while respecting result limit.
+# Of course, the results will be cached to prevent repeated requests.
+class CoverArtIterator(BaseIterator):
+    cache = {}
 
-        filters = self.parse_filter(args)
+    def __init__(self, manga_id):
+        super().__init__()
 
-        iterator = iter_random_manga(**filters)
-        text = f'Found random manga'
-        super().__init__(
-            parser,
-            args,
-            iterator,
-            text,
-            limit=5
-        )
+        self.limit = 100
+        self.manga_id = manga_id
+        
+        if self.cache.get(manga_id) is None:
+            # Data is not cached
+            self.cache[manga_id] = []
     
-    def on_empty_error(self):
-        # This should never happened
-        self.args_parser.error('Unknown error when fetching random manga')
-
-class SeasonalMangaCommand(MangaCommand):
-    def __init__(self, parser, args, input_text):
-        # Get season
-        _, season = get_key_value(input_text, sep=':')
-
-        season = season.lower().strip()
-
-        if season == "list":
-            self._print_help()
-        elif not season:
-            # Current season
-            r = Net.requests.get(f'https://raw.githubusercontent.com/{__repository__}/main/seasonal_manga_now.txt')
-            try:
-                r.raise_for_status()
-            except requests.HTTPError as e:
-                raise MangaDexException(f"failed to get current seasonal manga, reason: {e}")
-            
-            season_list_id = validate_url(r.text)
-            iterator = IteratorMangaFromList(season_list_id)
-            season = iterator.name
+    def _make_cache_iterator(self):
+        for item in self.cache.get(self.manga_id):
+            yield item
+
+    def __iter__(self):
+        cache = self.cache.get(self.manga_id)
+        if cache:
+            # Return cached data instead
+            return self._make_cache_iterator()
         else:
-            season = f'Seasonal: {season.capitalize()}'
-            iterator = IteratorSeasonalManga(season)
+            return self
 
-        text = f"List of manga from {season}"
-        super().__init__(
-            parser,
-            args,
-            iterator,
-            text
-        )
+    def fill_data(self):
+        # If it's already cached
+        # DO NOT FETCH IT AGAIN
+        if self.cache.get(self.manga_id):
+            return
 
-    def _print_help(self):
-        header = "Available seasons"
+        # One-shot filling covers in single function call
+        # So cache can be used
+        while True:
+            params = {
+                "manga[]": self.manga_id,
+                "offset": self.offset,
+                "limit": self.limit
+            }
+
+            url = f"{base_url}/cover"
+            r = Net.mangadex.get(url, params=params)
+            items = r.json()["data"]
 
-        print(header)
-        print(dynamic_bars(header), end='\n\n')
+            if not items:
+                break
 
-        for season in IteratorSeasonalManga._get_seasons():
-            print(season)
-        
-        sys.exit(0)
+            for item in items:
+                cover = CoverArt(data=item)
+                self.queue.put(cover)
 
-    def on_empty_error(self):
-        # This should never happened
-        self.args_parser.error('Unknown error when fetching seasonal manga')
-
-class ForumThreadCommand(MangaDexCommand):
-    def preview(self):
-        return True
-
-    def on_preview(self, item):
-        if isinstance(item, Manga):
-            preview_cover_manga(item)
-        elif isinstance(item, Chapter):
-            preview_chapter(item)
-        elif isinstance(item, MangaDexList):
-            preview_list(item)
-
-    def __init__(self, parser, args, input_text):
-        iterator = ForumThreadMangaDexURLIterator(input_text, True)
-
-        post_id = get_post_id_forum_thread(input_text)
-        result = get_thread_title_owner_and_post_owner(thread_url=input_text, post_id=post_id)
-        thread_title, thread_owner, post_owner = result
-
-        text = f"List of URLs from thread '{thread_title}' by '{thread_owner}'"
-
-        if post_owner:
-            text += f" post by '{post_owner}'"
-
-        super().__init__(
-            parser,
-            args,
-            iterator,
-            text,
-            limit=5
-        )
-
-    def _return_from(self, pos):
-        # We don't want to fetch the entire URLs returned from forum thread
-        # when --input-pos is used
-        self.paginator.iterator.fetch = False
+                # Add it to cache
+                self.cache[self.manga_id].append(cover)
+            
+            self.offset += len(items)
 
-        return super()._return_from(pos)
+class ForumThreadMangaDexURLIterator(BaseIterator):
+    """If `Fetch` parameter is `True`, it will return object based on returned type URLs. 
+    For example:
+
+    - manga = :class:`mangadex_downloader.manga.Manga`
+    - chapter = :class:`mangadex_downloader.chapter.Chapter`
+    - list = :class:`mangadex_downloader.mdlist.MangaDexList`
+    - etc
     
-    def on_empty_error(self):
-        self.args_parser.error("No MangaDex urls found in the forum thread")
+    Otherwise it will return the ids only.
+    """
+    def __init__(self, thread_id, fetch=False):
+        super().__init__()
+
+        self.thread_id = thread_id
+        self.fetch = fetch
+        self.limit = 5 # We don't want to slow down the application
+
+        self.iterator = iter_md_urls_from_forum_thread(thread_id)
+
+    def _make_item_obj(self, item_id, item_type):
+        if item_type == "legacy-manga":
+            new_id = get_legacy_id("manga", item_id)
+            obj = Manga(_id=new_id)
+        elif item_type == "legacy-chapter":
+            new_id = get_legacy_id("chapter", item_id)
+            obj = Chapter(_id=new_id)
+        elif item_type == "list":
+            obj = MangaDexList(_id=item_id)
+        elif item_type == "manga":
+            obj = Manga(_id=item_id)
+        elif item_type == "chapter":
+            obj = Chapter(_id=item_id)
+        else:
+            # This should be impossible
+            # because `item_type` value is from `utils.valid_url_types`
+            raise RuntimeError(f"item_type '{item_type}' unknown, item_id = {item_id}")
+        
+        return obj
+
+    def fill_data(self):
+        current_limit = 0
+        while current_limit < self.limit:
+            try:
+                raw_item = next(self.iterator)
+            except StopIteration:
+                return
 
-registered_commands = {
-    "search": SearchMangaCommand,
-    "fetch_library_manga": MangaLibraryCommand,
-    "fetch_library_list": ListLibraryCommand,
-    "fetch_library_follows_list": FollowedListLibraryCommand,
-    "random": RandomMangaCommand,
-    "fetch_group": GroupMangaCommand,
-    "seasonal": SeasonalMangaCommand,
-    "thread": ForumThreadCommand
-}
+            item_id, item_type = raw_item
+
+            if self.fetch:
+                item = self._make_item_obj(item_id, item_type)
+            else:
+                item = item_id
+            
+            self.queue.put(item)
+            current_limit += 1
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/cli/config.py` & `mangadex-downloader-2.9.0/mangadex_downloader/cli/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/cli/download.py` & `mangadex-downloader-2.9.0/mangadex_downloader/cli/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/cli/update.py` & `mangadex-downloader-2.9.0/mangadex_downloader/cli/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/cli/url.py` & `mangadex-downloader-2.9.0/mangadex_downloader/cli/url.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -37,15 +37,16 @@
     valid_url_types
 )
 from ..main import (
     download as dl_manga,
     download_chapter as dl_chapter,
     download_list as dl_list,
     download_legacy_chapter as dl_legacy_chapter,
-    download_legacy_manga as dl_legacy_manga
+    download_legacy_manga as dl_legacy_manga,
+    download_cover_art_manga as dl_cover_art
 )
 
 log = logging.getLogger(__name__)
 
 def download_manga(url, args, legacy=False):
     check_group_all(args)
 
@@ -140,14 +141,17 @@
 
     dl_list(
         url,
         args.replace,
         args.group,
     )
 
+def download_cover(url, args):
+    dl_cover_art(url, args.replace)
+
 # Legacy support
 download_legacy_manga = lambda url, args: download_manga(url, args, True)
 download_legacy_chapter = lambda url, args: download_chapter(url, args, True)
 
 funcs = {i: globals()['download_%s' % i.replace('-', '_')] for i in valid_url_types}
 
 class URL:
@@ -163,15 +167,16 @@
     def __repr__(self) -> str:
         return '<URL func = "%s" id = "%s">' % (
             self.func.__name__,
             self.id
         )
 
 def build_URL_from_type(_type, _id):
-    return URL(funcs[_type], _id)
+    parsed_id = get_uuid(_id)
+    return URL(funcs[_type], parsed_id)
 
 def smart_select_url(url):
     """Wisely determine type url. The process is checking given url one by one"""
     log.info(f"Checking url = {url}")
     func = None
     _id = None
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/cli/utils.py` & `mangadex-downloader-2.9.0/mangadex_downloader/cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/config/auth_cache.py` & `mangadex-downloader-2.9.0/mangadex_downloader/config/auth_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,25 +18,25 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import threading
 import base64
-import json
 import binascii
 import logging
 import traceback
 import sys
 import jwt
 from datetime import datetime
 
 from .env import *
 from .config import *
 from ..errors import MangaDexException
+from .. import json_op
 
 log = logging.getLogger(__name__)
 
 __all__ = ("login_cache",)
 
 class AuthCacheManager:
     path = base_path / 'auth.cache'
@@ -83,20 +83,20 @@
             )
 
         data['refresh']['exp'] = parsed_exp_refresh_token
         data['session']['exp'] = parsed_exp_session_token
 
     def _read(self):
         if not self.path.exists():
-            data = base64.b64encode(json.dumps(self.default).encode())
+            data = base64.b64encode(json_op.dumps(self.default, convert_str=False))
             self.path.write_bytes(data)
 
         data = self.path.read_bytes()
         decoded = base64.b64decode(data)
-        final_data = json.loads(decoded)
+        final_data = json_op.loads(decoded)
         self._parse_expired_time(final_data)
         return final_data
 
     def _serialize_exp_time(self, obj):
         """Convert :class:`datetime.datetime` to formatted string"""
         exp_refresh_token = obj['refresh']['exp']
         exp_session_token = obj['session']['exp']
@@ -110,15 +110,15 @@
             serialized_exp_session_token = exp_session_token.strftime(self.fmt_exp_datetime)
 
         obj['refresh']['exp'] = serialized_exp_refresh_token
         obj['session']['exp'] = serialized_exp_session_token
 
     def _write(self, obj):
         self._serialize_exp_time(obj)
-        data = json.dumps(obj).encode()
+        data = json_op.dumps(obj, convert_str=False)
         self.path.write_bytes(base64.b64encode(data))
         self._parse_expired_time(obj)
         self._data = obj
 
     def _load(self):
         if not config_enabled or not config.login_cache:
             self._data = self.default.copy()
@@ -135,15 +135,15 @@
                 err = e
                 # Failed to decode base64
                 log.error(
                     f"Failed to decode auth cache file, reason: {e}. " \
                     "Authentication cache file will be re-created and previous auth cached will be lost. " \
                     f"Recreating... (attempt: {attempt})"
                 )
-            except json.JSONDecodeError as e:
+            except json_op.JSONDecodeError as e:
                 err = e
                 # Failed to deserialize json
                 log.error(
                     f"Failed to deserialize json auth cache file, reason: {e}. " \
                     "Authentication cache file will be re-created and previous auth cached will be lost. " \
                     f"Recreating... (attempt: {attempt})"
                 )
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/config/config.py` & `mangadex-downloader-2.9.0/mangadex_downloader/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,20 +18,19 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import threading
 import logging
-import json
 from requests_doh import get_all_dns_provider
 
 from .env import base_path, config_enabled, init
 from .utils import *
-from .. import format as fmt
+from .. import format as fmt, json_op
 from ..cover import default_cover_type, valid_cover_types
 from ..language import Language
 from ..errors import MangaDexException
 
 # Fix #28
 _doh_providers = [None]
 _doh_providers.extend(get_all_dns_provider())
@@ -169,15 +168,15 @@
                     f"reason: {e}. Falling back to default value"
                 )
                 data[conf_key] = default_value
 
         self._data = data
 
         if config_enabled and write_to_path:
-            self.path.write_text(json.dumps(data))
+            self.path.write_text(json_op.dumps(data))
 
     def _write_default(self):
         self._write(self.default_conf)
 
     def _load(self):
         # Initialize config
         if config_enabled:
@@ -200,16 +199,16 @@
 
             # Very tricky lmao
             for attempt, _ in enumerate(range(5), start=1):
                 try:
                     if not self.path.exists():
                         self._write_default()
 
-                    data = json.loads(self.path.read_bytes())
-                except json.JSONDecodeError as e:
+                    data = json_op.loads(self.path.read_bytes())
+                except json_op.JSONDecodeError as e:
                     err = e
                     log.error(
                         f'Failed to decode json data from config file = {self.path.resolve()} ' \
                         f'reason: {e}, retrying... (attempt: {attempt})'
                     )
                     # If somehow failed to decode JSON data, delete it and try it again
                     self.path.unlink(missing_ok=True)
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/config/env.py` & `mangadex-downloader-2.9.0/mangadex_downloader/config/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/config/utils.py` & `mangadex-downloader-2.9.0/mangadex_downloader/config/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/cover.py` & `mangadex-downloader-2.9.0/mangadex_downloader/cover.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,21 +20,22 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from .fetcher import get_cover_art
 from .language import get_language
 from .utils import convert_int_or_float
 
-valid_cover_types = [
+cover_qualities = [
     "original",
     "512px",
     "256px",
-    "none"
 ]
 
+valid_cover_types = cover_qualities + ["none"]
+
 default_cover_type = "original"
 
 class CoverArt:
     def __init__(self, cover_id=None, data=None):
         if not data:
             self.data = get_cover_art(cover_id)["data"]
         else:
@@ -48,14 +49,31 @@
 
         # File cover
         self.file = attr["fileName"]
 
         # Locale
         self.locale = get_language(attr["locale"])
 
+        # Manga and user id
+        self.manga_id = None
+        self.user_id = None
+        try:
+            rels = self.data["relationships"]
+            for rel in rels:
+                if rel["type"] == "manga":
+                    self.manga_id = rel["id"]
+                elif rel["type"] == "user":
+                    self.user_id = rel["id"]
+        except KeyError:
+            # There is no relationships in API data
+            pass
+
+    def __str__(self) -> str:
+        return f"Cover volume {self.volume}"
+
     @property
     def volume(self):
         vol = self.data["attributes"]["volume"]
         if vol is not None:
             # As far as i know
             # Volume manga are integer numbers, not float
             try:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/downloader.py` & `mangadex-downloader-2.9.0/mangadex_downloader/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/errors.py` & `mangadex-downloader-2.9.0/mangadex_downloader/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,14 +16,22 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+from . import __repository__, __url_repository__
+
+class UnhandledException(Exception):
+    """Some errors that the application are unable to handle"""
+    def __init__(self, msg):
+        super().__init__(str(msg) + 
+                        f". Please report this issue to {__url_repository__}/{__repository__}/issues")
+
 class MangaDexException(Exception):
     """Base exception for MangaDex errors"""
     pass
 
 class UnhandledHTTPError(MangaDexException):
     """Raised when we unable to handle HTTP errors"""
     pass
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/fetcher.py` & `mangadex-downloader-2.9.0/mangadex_downloader/fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/filters.py` & `mangadex-downloader-2.9.0/mangadex_downloader/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/AUTHORS` & `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/AUTHORS`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/COPYING` & `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/COPYING`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/CREDITS` & `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/CREDITS`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/README` & `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/README`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSans.otf` & `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSans.otf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBold.otf` & `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBold.otf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBoldOblique.otf` & `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBoldOblique.otf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansOblique.otf` & `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansOblique.otf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSans.ttf` & `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSans.ttf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBold.ttf` & `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBold.ttf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBoldOblique.ttf` & `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansOblique.ttf` & `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansOblique.ttf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/format/__init__.py` & `mangadex-downloader-2.9.0/mangadex_downloader/format/__init__.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/format/base.py` & `mangadex-downloader-2.9.0/mangadex_downloader/format/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/format/chinfo.py` & `mangadex-downloader-2.9.0/mangadex_downloader/format/chinfo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+# MIT License
+
+# Copyright (c) 2022-present Rahman Yusuf
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 import sys
 import textwrap
 from pathlib import Path
 
 from ..utils import get_cover_art_url
 from ..network import Net
 
@@ -66,15 +88,15 @@
         fill=rgb_white,
         font=font,
         align="left"
     )
     return draw.multiline_textbbox((width_pos, height_pos), new_text, font, align="left")
 
 def get_chapter_info(manga, cover, chapter):
-    cover_url = get_cover_art_url(manga, cover, "original")
+    cover_url = get_cover_art_url(manga.id, cover, "original")
     r = Net.mangadex.get(cover_url, stream=True)
     image = Image.open(r.raw)
     image = image.convert("RGBA")
 
     # resize image to fixed 1000px width (keeping aspect ratio) so font sizes and text heights match for all covers
     aspect_ratio = image.height / image.width
     new_width = 1000
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/format/comic_book.py` & `mangadex-downloader-2.9.0/mangadex_downloader/format/comic_book.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/format/epub.py` & `mangadex-downloader-2.9.0/mangadex_downloader/format/epub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/format/pdf.py` & `mangadex-downloader-2.9.0/mangadex_downloader/format/pdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -100,24 +100,29 @@
         img.load()
 
         return True
 
     def _save_all(self, im, fp, filename):
         self._save(im, fp, filename, save_all=True)
 
-    # This was modified version of Pillow/PdfImagePlugin.py version 9.3.0
+    # This was modified version of Pillow/PdfImagePlugin.py version 9.5.0
     # The images will be automatically converted to RGB and closed when done converting to PDF
     def _save(self, im, fp, filename, save_all=False):
         is_appending = im.encoderinfo.get("append", False)
         if is_appending:
             existing_pdf = PdfParser.PdfParser(f=fp, filename=filename, mode="r+b")
         else:
             existing_pdf = PdfParser.PdfParser(f=fp, filename=filename, mode="w+b")
 
-        resolution = im.encoderinfo.get("resolution", 72.0)
+        dpi = im.encoderinfo.get("dpi")
+        if dpi:
+            x_resolution = dpi[0]
+            y_resolution = dpi[1]
+        else:
+            x_resolution = y_resolution = im.encoderinfo.get("resolution", 72.0)
 
         info = {
             "title": None
             if is_appending
             else os.path.splitext(os.path.basename(filename))[0],
             "author": None,
             "subject": None,
@@ -249,21 +254,26 @@
                         PdfParser.PdfBinary(palette),
                     ]
                     procset = "ImageI"  # indexed color
                 elif im.mode == "RGB":
                     filter = "DCTDecode"
                     colorspace = PdfParser.PdfName("DeviceRGB")
                     procset = "ImageC"  # color images
+                elif im.mode == "RGBA":
+                    filter = "JPXDecode"
+                    colorspace = PdfParser.PdfName("DeviceRGB")
+                    procset = "ImageC"  # color images
                 elif im.mode == "CMYK":
                     filter = "DCTDecode"
                     colorspace = PdfParser.PdfName("DeviceCMYK")
                     procset = "ImageC"  # color images
                     decode = [1, 0, 1, 0, 1, 0, 1, 0]
                 else:
-                    raise ValueError(f"cannot save mode {im.mode}")
+                    msg = f"cannot save mode {im.mode}"
+                    raise ValueError(msg)
 
                 #
                 # image
 
                 op = io.BytesIO()
 
                 if filter == "ASCIIHexDecode":
@@ -274,35 +284,38 @@
                         "TIFF",
                         compression="group4",
                         # use a single strip
                         strip_size=math.ceil(im.width / 8) * im.height,
                     )
                 elif filter == "DCTDecode":
                     Image.SAVE["JPEG"](im, op, filename)
+                elif filter == "JPXDecode":
+                    Image.SAVE["JPEG2000"](im, op, filename)
                 elif filter == "FlateDecode":
                     ImageFile._save(im, op, [("zip", (0, 0) + im.size, 0, im.mode)])
                 elif filter == "RunLengthDecode":
                     ImageFile._save(im, op, [("packbits", (0, 0) + im.size, 0, im.mode)])
                 else:
-                    raise ValueError(f"unsupported PDF filter ({filter})")
+                    msg = f"unsupported PDF filter ({filter})"
+                    raise ValueError(msg)
 
                 stream = op.getvalue()
                 if filter == "CCITTFaxDecode":
                     stream = stream[8:]
                     filter = PdfParser.PdfArray([PdfParser.PdfName(filter)])
                 else:
                     filter = PdfParser.PdfName(filter)
 
                 existing_pdf.write_obj(
                     image_refs[page_number],
                     stream=stream,
                     Type=PdfParser.PdfName("XObject"),
                     Subtype=PdfParser.PdfName("Image"),
-                    Width=width,  # * 72.0 / resolution,
-                    Height=height,  # * 72.0 / resolution,
+                    Width=width,  # * 72.0 / x_resolution,
+                    Height=height,  # * 72.0 / y_resolution,
                     Filter=filter,
                     BitsPerComponent=bits,
                     Decode=decode,
                     DecodeParms=params,
                     ColorSpace=colorspace,
                 )
 
@@ -314,26 +327,26 @@
                     Resources=PdfParser.PdfDict(
                         ProcSet=[PdfParser.PdfName("PDF"), PdfParser.PdfName(procset)],
                         XObject=PdfParser.PdfDict(image=image_refs[page_number]),
                     ),
                     MediaBox=[
                         0,
                         0,
-                        width * 72.0 / resolution,
-                        height * 72.0 / resolution,
+                        width * 72.0 / x_resolution,
+                        height * 72.0 / y_resolution,
                     ],
                     Contents=contents_refs[page_number],
                 )
 
                 #
                 # page contents
 
                 page_contents = b"q %f 0 0 %f 0 0 cm /image Do Q\n" % (
-                    width * 72.0 / resolution,
-                    height * 72.0 / resolution,
+                    width * 72.0 / x_resolution,
+                    height * 72.0 / y_resolution,
                 )
 
                 existing_pdf.write_obj(contents_refs[page_number], stream=page_contents)
 
                 self.tqdm.update(1)
                 page_number += 1
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/format/raw.py` & `mangadex-downloader-2.9.0/mangadex_downloader/format/raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/format/sevenzip.py` & `mangadex-downloader-2.9.0/mangadex_downloader/format/sevenzip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/format/tachiyomi.py` & `mangadex-downloader-2.9.0/mangadex_downloader/format/tachiyomi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/format/utils.py` & `mangadex-downloader-2.9.0/mangadex_downloader/format/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,26 +17,25 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import hashlib
-import json
 import logging
 import os
 import re
 import threading
 import time
 
 from enum import Enum
 from .chinfo import get_chapter_info as get_chinfo
 from ..downloader import FileDownloader
 from ..utils import get_cover_art_url
-from .. import __repository__, __url_repository__
+from .. import __repository__, __url_repository__, json_op
 
 log = logging.getLogger(__name__)
 
 def get_chapter_info(manga, chapter, path):
     log.info(f"Creating chapter info for '{chapter.get_name()}'")
 
     vol_cover = get_volume_cover(
@@ -77,15 +76,15 @@
         if download:
             log.warning(
                 f"Failed to find volume cover for volume {volume}. " \
                 "Falling back to manga cover..."
             )
         cover = manga.cover
 
-    url = get_cover_art_url(manga, cover, "original")
+    url = get_cover_art_url(manga.id, cover, "original")
 
     if download:
         fd = FileDownloader(
             url,
             path,
             progress_bar=not config.no_progress_bar,
             replace=replace
@@ -247,15 +246,15 @@
         "2 = Completed",
         "3 = Licensed",
         "4 = Publishing finished",
         "5 = Cancelled",
         "6 = On hiatus"
     ]
     with open(path, 'w') as writer:
-        writer.write(json.dumps(data))
+        writer.write(json_op.dumps(data))
 
 class QueueWorkerReadMarker(threading.Thread):
     """A queue-based worker run in another thread for ChapterReadMarker
     
     This class will mark chapter as read for every 20 chapters
     and will be done asynchronously (in another thread)
     """
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/forums.py` & `mangadex-downloader-2.9.0/mangadex_downloader/forums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -22,16 +22,15 @@
 
 import re
 import logging
 from bs4 import BeautifulSoup
 from dataclasses import dataclass
 from typing import Union
 
-from . import __repository__, __url_repository__
-from .errors import InvalidURL, MangaDexException
+from .errors import InvalidURL, MangaDexException, UnhandledException
 from .network import Net, forums_url
 from .utils import find_md_urls
 
 log = logging.getLogger(__name__)
 
 @dataclass
 class _ResultValidationForumThreadURL:
@@ -127,27 +126,25 @@
         r = Net.mangadex.get(thread_url)
         parser = BeautifulSoup(r.text, "html.parser")
 
     # Finding thread owner
     thread_owner = parser.find("a", attrs={"class": ["username"], "data-xf-init": "member-tooltip"})
     if thread_owner is None:
         # Hmmmm, there is no thread owner in a forum thread ? sus
-        raise MangaDexException(
-            f"No thread owner in forum thread {thread_url}. " \
-            f"Please report this issue to {__url_repository__}/{__repository__}/issues"
+        raise UnhandledException(
+            f"No thread owner in forum thread {thread_url}"
         )
     thread_owner = thread_owner.get_text(strip=True)
 
     # Finding thread title
     thread_title = parser.find("h1", attrs={"class": ["p-title-value"]})
     if thread_title is None:
         # No thread title ? VERY SUS
-        raise MangaDexException(
-            f"No thread title in forum thread {thread_url}. " \
-            f"Please report this issue to {__url_repository__}/{__repository__}/issues"
+        raise UnhandledException(
+            f"No thread title in forum thread {thread_url}"
         )
     thread_title = thread_title.get_text(strip=True)
 
     if post_id:
         article = parser.find("article", attrs={"data-content": f"post-{post_id}"})
         if article:
             post_owner = article.attrs["data-author"]
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/group.py` & `mangadex-downloader-2.9.0/mangadex_downloader/group.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/images/mangadex-logo.png` & `mangadex-downloader-2.9.0/mangadex_downloader/images/mangadex-logo.png`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/language.py` & `mangadex-downloader-2.9.0/mangadex_downloader/language.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/main.py` & `mangadex-downloader-2.9.0/mangadex_downloader/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,22 +17,27 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import logging
+import re
+import os
+from pathlib import Path
+from .errors import UnhandledException
 from .utils import (
     comma_separated_text,
     create_directory,
     check_blacklisted_tags_manga,
     get_cover_art_url
 )
 from .language import Language, get_language
 from .fetcher import *
+from .iterator import CoverArtIterator
 from .mdlist import MangaDexList
 from .manga import Manga
 from .chapter import Chapter
 from .format import get_format
 from .downloader import FileDownloader
 from .config import config
 from .tracker import get_tracker
@@ -84,15 +89,15 @@
     base_path = create_directory(manga.title, config.path)
 
     # Cover path
     cover_path = base_path / 'cover.jpg'
     log.info('Downloading cover manga %s' % manga.title)
 
     # Determine cover art quality
-    cover_url = get_cover_art_url(manga, manga.cover, cover)
+    cover_url = get_cover_art_url(manga.id, manga.cover, cover)
     
     # Download the cover art
     if cover == 'none':
         log.info('Not downloading cover manga, since "cover" is none')
     elif cover_url is None:
         # The manga doesn't have cover
         log.info(f"Not downloading cover manga, since manga '{manga.title}' doesn\'t have cover")
@@ -249,8 +254,64 @@
     log.warning(
         'Old MangaDex URL are deprecated and will be removed any time soon. ' \
         'Please use the new MangaDex URL'
     )
 
     new_id = get_legacy_id('chapter', legacy_id)
     manga = download_chapter(new_id, *args, **kwargs)
-    return manga
+    return manga
+
+def download_cover_art_manga(url, replace=False):
+    # This is hack actually
+    # Since the covers URL are not including cover id
+    # (https://mangadex.org/covers/{manga_id}/{filename})
+    # We gonna find filename cover in list of covers
+    log.info("Getting manga id from cover url")
+    regex = r".+(mangadex\.org|uploads\.mangadex\.org)\/covers\/" \
+            r"(?P<manga_id>[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12})\/" \
+            r"(?P<filename>[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}\.[a-zA-Z]{1,}.+)"
+    result = re.search(regex, url)
+    if result is None:
+        raise UnhandledException(f"Cannot find manga id in cover URL = {url}")
+
+    log.info("Finding matching cover from filename")
+    iterator = CoverArtIterator(result.group("manga_id"))
+    cover = None
+    filename = result.group("filename")
+
+    for cv in iterator:
+        if cv.file in filename:
+            cover = cv
+            break
+
+    if cover is None:
+        raise MangaDexException(f"Cannot find matching cover from filename {filename}")
+
+    manga = Manga(_id=cover.manga_id)
+    if cover.volume is None:
+        cover_name = "No volume cover"
+    else:
+        cover_name = f"Volume {cover.volume} cover"
+    log.info(f"Found {cover_name} from '{manga.title}', downloading...")
+
+    # Merge file ext with new filename
+    _, file_ext = filename.split(".", maxsplit=1)
+    filename = cover_name + "." +  file_ext
+    base_path = create_directory(manga.title, path=config.path)
+    path = base_path / filename
+    log.info(f"Download directory is set to {base_path}")
+
+    def handle_error(err, resp):
+        if not resp.ok:
+            filename = result.group("filename")
+            raise MangaDexException(f"Cover file '{filename}' is not found on MangaDex")
+
+    log.info(f"Downloading file '{filename}'")
+    fd = FileDownloader(
+        url=url,
+        file=path,
+        progress_bar=not config.no_progress_bar,
+        replace=replace
+    )
+    fd.on_error = handle_error
+    fd.download()
+    fd.cleanup()
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/manga.py` & `mangadex-downloader-2.9.0/mangadex_downloader/manga.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/mdlist.py` & `mangadex-downloader-2.9.0/mangadex_downloader/mdlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/network.py` & `mangadex-downloader-2.9.0/mangadex_downloader/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -25,41 +25,33 @@
 import requests
 import itertools
 import urllib.parse
 import time
 import logging
 import sys
 import threading
-from . import __version__, __repository__
+from . import __version__, __repository__, json_op
 from .errors import (
     AlreadyLoggedIn,
     HTTPException,
     LoginFailed,
     MangaDexException,
     NotLoggedIn,
     UnhandledHTTPError
 )
 from .auth import OAuth2, LegacyAuth
 from .utils import QueueWorker
 from requests_doh import DNSOverHTTPSAdapter, set_dns_provider
 from concurrent.futures import Future, TimeoutError
 
-try:
-    import orjson
-except ImportError:
-    have_orjson = False
-else:
-    have_orjson = True
-
-# Apply json loader into :class:`requests.Response`
 def loads_json(self):
-    return orjson.loads(self.content)
+    return json_op.loads(self.content)
 
-if have_orjson:
-    requests.Response.json = loads_json
+# Apply custom json loader into :class:`requests.Response`
+requests.Response.json = loads_json
 
 DEFAULT_RATE_LIMITED_TIMEOUT = 120
 
 log = logging.getLogger(__name__)
 
 __all__ = (
     'Net', 'NetworkManager',
@@ -287,15 +279,15 @@
         self._session_token = session_token
         self.headers['Authorization'] = 'Bearer %s' % session_token
 
         self._login_cache.set_refresh_token(refresh_token)
         self._login_cache.set_session_token(session_token)
 
     def _is_token_cached(self):
-        return bool(self._login_cache.get_session_token or self._login_cache.get_refresh_token())
+        return bool(self._login_cache.get_session_token() or self._login_cache.get_refresh_token())
 
     def _reset_token(self):
         self._refresh_token = None
         self._session_token = None
         self.headers.pop('Authorization')
 
     def _notify_login_fut(self):
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/range.py` & `mangadex-downloader-2.9.0/mangadex_downloader/range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/tag.py` & `mangadex-downloader-2.9.0/mangadex_downloader/tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/tracker/__init__.py` & `mangadex-downloader-2.9.0/mangadex_downloader/tracker/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+# MIT License
+
+# Copyright (c) 2022-present Rahman Yusuf
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 import logging
 from tqdm import tqdm
 from pathlib import Path
 
 from .legacy import DownloadTrackerJSON, FileInfo, ChapterInfo, ImageInfo
 from .sqlite import DownloadTrackerSQLite
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/tracker/legacy.py` & `mangadex-downloader-2.9.0/mangadex_downloader/tracker/legacy.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/tracker/sql_files/create_ch_info.sql` & `mangadex-downloader-2.9.0/mangadex_downloader/tracker/sql_files/create_ch_info.sql`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/tracker/sql_files/create_file_info.sql` & `mangadex-downloader-2.9.0/mangadex_downloader/tracker/sql_files/create_file_info.sql`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/tracker/sql_files/create_img_info.sql` & `mangadex-downloader-2.9.0/mangadex_downloader/tracker/sql_files/create_img_info.sql`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/tracker/sqlite.py` & `mangadex-downloader-2.9.0/mangadex_downloader/tracker/sqlite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+# MIT License
+
+# Copyright (c) 2022-present Rahman Yusuf
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 import sqlite3
 import logging
 import threading
 from pathlib import Path
 from typing import Union
 from datetime import datetime
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/update.py` & `mangadex-downloader-2.9.0/mangadex_downloader/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/user.py` & `mangadex-downloader-2.9.0/mangadex_downloader/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader/utils.py` & `mangadex-downloader-2.9.0/mangadex_downloader/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-# Copyright (c) 2022 Rahman Yusuf
+# Copyright (c) 2022-present Rahman Yusuf
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -245,15 +245,15 @@
         found_tags.append(manga_tag)
 
     if found_tags:
         return True, found_tags
     else:
         return False, found_tags
 
-def get_cover_art_url(manga, cover, quality):
+def get_cover_art_url(manga_id, cover, quality):
     if quality == "none" or cover is None:
         return None
 
     # "Circular Imports" problem
     from .network import uploads_url
 
     if quality == "original":
@@ -261,37 +261,43 @@
     elif quality == "512px":
         additional_file_ext = ".512.jpg"
     elif quality == "256px":
         additional_file_ext = ".256.jpg"
     
     return "{0}/covers/{1}/{2}{3}".format(
         uploads_url,
-        manga.id,
+        manga_id,
         cover.file,
         additional_file_ext
     )
 
 def _build_url_regex(type):
     # Legacy support
     if 'legacy-manga' in type:
         regex = r'mangadex\.org\/(title|manga)\/(?P<id>[0-9]{1,})'
     elif 'legacy-chapter' in type:
         regex = r'mangadex\.org\/chapter\/(?P<id>[0-9]{1,})'
     elif type == 'manga':
         regex = r'mangadex\.org\/(title|manga)\/(?P<id>[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12})'
+    elif type == 'cover':
+        regex = r'(?P<id>.+(mangadex\.org|uploads\.mangadex\.org)\/covers\/' \
+                r'([a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}' \
+                r'-[a-z0-9]{12})\/([a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]' \
+                r'{4}-[a-z0-9]{12})(\.[a-zA-Z]{1,})(\..+|))'
     else:
         regex = r"mangadex\.org\/%s\/(?P<id>[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12})" % type
     return regex
 
 valid_url_types = [
     "manga",
     "list",
     "chapter",
     "legacy-manga",
-    "legacy-chapter"
+    "legacy-chapter",
+    "cover",
 ]
 
 _urL_regexs = {i: _build_url_regex(i) for i in valid_url_types}
 
 def find_md_urls(text):
     for type, regex in _urL_regexs.items():
         # Match pattern regex
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader.egg-info/PKG-INFO` & `mangadex-downloader-2.9.0/mangadex_downloader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangadex-downloader
-Version: 2.8.3
+Version: 2.9.0
 Summary: A Command-line tool to download manga from MangaDex, written in Python
 Home-page: https://github.com/mansuf/mangadex-downloader
 Download-URL: https://github.com/mansuf/mangadex-downloader/releases
 Author: Rahman Yusuf
 Author-email: danipart4@gmail.com
 License: MIT
 Keywords: mangadex
@@ -48,15 +48,15 @@
 - [Contributing](#contributing)
 - [Donation](#donation)
 - [Links](#links)
 - [Disclaimer](#disclaimer)
 
 ## Key Features <a id="key-features"></a>
 
-- Download manga, chapter, or list directly from MangaDex
+- Download manga, cover manga, chapter, or list directly from MangaDex
 - Download manga or list from user library
 - Find and download MangaDex URLs from MangaDex forums ([https://forums.mangadex.org/](https://forums.mangadex.org/))
 - Batch download support
 - Old MangaDex url support
 - Scanlation groups filter support
 - Authentication support
 - Control how many chapters and pages you want to download
@@ -176,14 +176,15 @@
 See [CONTRIBUTING.md](https://github.com/mansuf/mangadex-downloader/blob/main/CONTRIBUTING.md) for more info
 
 ## Donation <a id="donation"></a>
 
 If you like this project, please consider donate to one of these websites:
 
 - [Sociabuzz](https://sociabuzz.com/mansuf/donate)
+- [Ko-fi](https://ko-fi.com/rahmanyusuf)
 - [Github Sponsor](https://github.com/sponsors/mansuf)
 
 Any donation amount will be appreciated 💖
 
 ## Links <a id="links"></a>
 
 - [PyPI](https://pypi.org/project/mangadex-downloader/)
```

### Comparing `mangadex-downloader-2.8.3/mangadex_downloader.egg-info/SOURCES.txt` & `mangadex-downloader-2.9.0/mangadex_downloader.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 mangadex_downloader/downloader.py
 mangadex_downloader/errors.py
 mangadex_downloader/fetcher.py
 mangadex_downloader/filters.py
 mangadex_downloader/forums.py
 mangadex_downloader/group.py
 mangadex_downloader/iterator.py
+mangadex_downloader/json_op.py
 mangadex_downloader/language.py
 mangadex_downloader/main.py
 mangadex_downloader/manga.py
 mangadex_downloader/mdlist.py
 mangadex_downloader/network.py
 mangadex_downloader/range.py
 mangadex_downloader/tag.py
```

### Comparing `mangadex-downloader-2.8.3/setup.py` & `mangadex-downloader-2.9.0/setup.py`

 * *Files identical despite different names*

