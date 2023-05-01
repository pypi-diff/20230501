# Comparing `tmp/xklb-1.26.14.tar.gz` & `tmp/xklb-1.26.15.tar.gz`

## Comparing `xklb-1.26.14.tar` & `xklb-1.26.15.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.14/.gitattributes
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 xklb-1.26.14/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.14/Windows.md
--rw-r--r--   0        0        0   415271 2020-02-02 00:00:00.000000 xklb-1.26.14/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.14/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.14/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.14/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.14/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 xklb-1.26.14/.github/workflows/push.yaml
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 xklb-1.26.14/sql/restore_listen_count.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/__init__.py
--rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/av.py
--rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/books.py
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/consts.py
--rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/db.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/dl_config.py
--rw-r--r--   0        0        0    14769 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/dl_extract.py
--rw-r--r--   0        0        0    13485 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/fs_extract.py
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/gui.py
--rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/hn_extract.py
--rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/lb.py
--rw-r--r--   0        0        0    35700 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/play_actions.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/playback.py
--rw-r--r--   0        0        0    26435 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/player.py
--rw-r--r--   0        0        0    14621 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/praw_extract.py
--rw-r--r--   0        0        0    16072 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/stats.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/subtitle.py
--rw-r--r--   0        0        0    12107 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/tube_backend.py
--rw-r--r--   0        0        0     6292 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/tube_extract.py
--rw-r--r--   0        0        0    28045 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/utils.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/christen.py
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/mining/nfb_ca.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/mining/reddit_self.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.14/xklb/scripts/mining/words.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.14/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.14/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.14/LICENSE
--rw-r--r--   0        0        0    40448 2020-02-02 00:00:00.000000 xklb-1.26.14/README.md
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 xklb-1.26.14/pyproject.toml
--rw-r--r--   0        0        0    43985 2020-02-02 00:00:00.000000 xklb-1.26.14/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.26.15/.gitattributes
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 xklb-1.26.15/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.26.15/Windows.md
+-rw-r--r--   0        0        0   414011 2020-02-02 00:00:00.000000 xklb-1.26.15/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.26.15/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.26.15/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.26.15/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.26.15/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 xklb-1.26.15/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/__init__.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/av.py
+-rw-r--r--   0        0        0     6859 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/books.py
+-rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/consts.py
+-rw-r--r--   0        0        0     7856 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/db.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/dl_config.py
+-rw-r--r--   0        0        0    14860 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13555 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6067 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/gui.py
+-rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9592 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/lb.py
+-rw-r--r--   0        0        0    35709 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/play_actions.py
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/playback.py
+-rw-r--r--   0        0        0    26512 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/player.py
+-rw-r--r--   0        0        0    14708 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16159 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/stats.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/subtitle.py
+-rw-r--r--   0        0        0    12089 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21697 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28119 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/utils.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9468 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17099 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/mining/nfb_ca.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.26.15/xklb/scripts/mining/words.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.26.15/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.26.15/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.26.15/LICENSE
+-rw-r--r--   0        0        0    40524 2020-02-02 00:00:00.000000 xklb-1.26.15/README.md
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.26.15/pyproject.toml
+-rw-r--r--   0        0        0    44061 2020-02-02 00:00:00.000000 xklb-1.26.15/PKG-INFO
```

### Comparing `xklb-1.26.14/TODO` & `xklb-1.26.15/TODO`

 * *Files identical despite different names*

### Comparing `xklb-1.26.14/Windows.md` & `xklb-1.26.15/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.14/pdm.lock` & `xklb-1.26.15/pdm.lock`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 name = "future"
 version = "0.18.3"
 requires_python = ">=2.6, !=3.0.*, !=3.1.*, !=3.2.*"
 summary = "Clean single-source support for Python 3 and 2"
 
 [[package]]
 name = "gallery-dl"
-version = "1.25.2"
+version = "1.25.3"
 requires_python = ">=3.4"
 summary = "Command-line program to download image galleries and collections from several image hosting sites"
 dependencies = [
     "requests>=2.11.0",
 ]
 
 [[package]]
@@ -384,15 +384,15 @@
     "ipython>=7.31.1; python_version > \"3.6\" and python_version < \"3.11\"",
     "ipython>=7.31.1; python_version >= \"3.11\"",
     "tomli; python_version > \"3.6\" and python_version < \"3.11\"",
 ]
 
 [[package]]
 name = "ipython"
-version = "8.12.0"
+version = "8.12.1"
 requires_python = ">=3.8"
 summary = "IPython: Productive Interactive Computing"
 dependencies = [
     "appnope; sys_platform == \"darwin\"",
     "backcall",
     "colorama; sys_platform == \"win32\"",
     "decorator",
@@ -522,15 +522,15 @@
 name = "olefile"
 version = "0.46"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "Python package to parse, read and write Microsoft OLE2 files (Structured Storage or Compound Document, Microsoft Office)"
 
 [[package]]
 name = "orjson"
-version = "3.8.10"
+version = "3.8.11"
 requires_python = ">= 3.7"
 summary = "Fast, correct Python JSON library supporting dataclasses, datetimes, and numpy"
 
 [[package]]
 name = "packaging"
 version = "23.1"
 requires_python = ">=3.7"
@@ -596,15 +596,15 @@
 name = "pillow"
 version = "9.5.0"
 requires_python = ">=3.7"
 summary = "Python Imaging Library (Fork)"
 
 [[package]]
 name = "platformdirs"
-version = "3.4.0"
+version = "3.5.0"
 requires_python = ">=3.7"
 summary = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 
 [[package]]
 name = "pluggy"
 version = "1.0.0"
 requires_python = ">=3.6"
@@ -816,15 +816,15 @@
     "chardet<4,>=3.0.2",
     "idna<3,>=2.5",
     "urllib3!=1.25.0,!=1.25.1,<1.26,>=1.21.1",
 ]
 
 [[package]]
 name = "rich"
-version = "13.3.4"
+version = "13.3.5"
 requires_python = ">=3.7.0"
 summary = "Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal"
 dependencies = [
     "markdown-it-py<3.0.0,>=2.2.0",
     "pygments<3.0.0,>=2.13.0",
     "typing-extensions<5.0,>=4.0.0; python_version < \"3.9\"",
 ]
@@ -1040,15 +1040,15 @@
 name = "websockets"
 version = "11.0.2"
 requires_python = ">=3.7"
 summary = "An implementation of the WebSocket Protocol (RFC 6455 & 7692)"
 
 [[package]]
 name = "werkzeug"
-version = "2.3.1"
+version = "2.3.2"
 requires_python = ">=3.8"
 summary = "The comprehensive WSGI web application library."
 dependencies = [
     "MarkupSafe>=2.1.1",
 ]
 
 [[package]]
@@ -1108,15 +1108,15 @@
 version = "3.15.0"
 requires_python = ">=3.7"
 summary = "Backport of pathlib-compatible object wrapper for zip files"
 
 [metadata]
 lock_version = "4.2"
 groups = ["default", "all", "deluxe", "dev", "test"]
-content_hash = "sha256:2248e9cec8c6be35ba49143dc7aaf11b704adeda352a5a65568c4e79d4f58962"
+content_hash = "sha256:d045ee536b47a947a35a1dc58eadf67483fb1b64ecaa33bb1ece931eefb8fb1a"
 
 [metadata.files]
 "aiohttp 3.8.4" = [
     {url = "https://files.pythonhosted.org/packages/03/e7/84b65e341b1f45753fea51158d8a9522e57a5ae804acbc6dc34edf07cea0/aiohttp-3.8.4-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:bca5f24726e2919de94f047739d0a4fc01372801a3672708260546aa2601bf57"},
     {url = "https://files.pythonhosted.org/packages/04/03/3ce412b191aba5961b4ada3ee7a93498623e218fb4d50ac6d357da61dc26/aiohttp-3.8.4-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:8189c56eb0ddbb95bfadb8f60ea1b22fcfa659396ea36f6adcc521213cd7b44d"},
     {url = "https://files.pythonhosted.org/packages/05/ee/77b3dc08f41a1bce842e30134233c58b3bbe8c0fa7be121295aa2fad885d/aiohttp-3.8.4-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:17b79c2963db82086229012cff93ea55196ed31f6493bb1ccd2c62f1724324e4"},
     {url = "https://files.pythonhosted.org/packages/07/3c/04c65b5873524a415509cbcf21787be32c31f4e729840fab9866dd197030/aiohttp-3.8.4-cp36-cp36m-musllinux_1_1_i686.whl", hash = "sha256:7c7837fe8037e96b6dd5cfcf47263c1620a9d332a87ec06a6ca4564e56bd0f36"},
@@ -1746,17 +1746,17 @@
 "ftfy 6.1.1" = [
     {url = "https://files.pythonhosted.org/packages/97/16/79c6e17bd3465f6498282dd23813846c68cd0989fe60bfef68bb1918d041/ftfy-6.1.1.tar.gz", hash = "sha256:bfc2019f84fcd851419152320a6375604a0f1459c281b5b199b2cd0d2e727f8f"},
     {url = "https://files.pythonhosted.org/packages/e1/1e/bf736f9576a8979752b826b75cbd83663ff86634ea3055a766e2d8ad3ee5/ftfy-6.1.1-py3-none-any.whl", hash = "sha256:0ffd33fce16b54cccaec78d6ec73d95ad370e5df5a25255c8966a6147bd667ca"},
 ]
 "future 0.18.3" = [
     {url = "https://files.pythonhosted.org/packages/8f/2e/cf6accf7415237d6faeeebdc7832023c90e0282aa16fd3263db0eb4715ec/future-0.18.3.tar.gz", hash = "sha256:34a17436ed1e96697a86f9de3d15a3b0be01d8bc8de9c1dffd59fb8234ed5307"},
 ]
-"gallery-dl 1.25.2" = [
-    {url = "https://files.pythonhosted.org/packages/ac/86/022e5c3a31072a57080ab01e791b82e6746562a0a3b0819053f33626e6e7/gallery_dl-1.25.2.tar.gz", hash = "sha256:4fd3f3be339d70b68eee24f1059c6e71076200f569935fbdc037dca5284805d3"},
-    {url = "https://files.pythonhosted.org/packages/af/9f/94c00008c2c71e2c3ca29c0a1a404e1d8e5d9c64e3a5e9a72153162b7bb4/gallery_dl-1.25.2-py3-none-any.whl", hash = "sha256:860a230d330da0b1939edea0fc19884dfc8036e7643a6ef65281335f3978613d"},
+"gallery-dl 1.25.3" = [
+    {url = "https://files.pythonhosted.org/packages/2d/7b/759ffa14f2b0152b1a71671fb92da305f07bb035d3fb52fddcfe97b3fcc9/gallery_dl-1.25.3-py3-none-any.whl", hash = "sha256:9604690a4584069fb69f220f455a899ea3b323a3eafeb25f173470faf575aaee"},
+    {url = "https://files.pythonhosted.org/packages/be/05/db6932f3f27b24fd33dcc924584bbe8401211120763a8dc0733eaa8bc6a2/gallery_dl-1.25.3.tar.gz", hash = "sha256:6a8b1a03c17c4d5067634333f936d16108d55b91540e24a2a2197feefa97c22b"},
 ]
 "guessit 3.7.1" = [
     {url = "https://files.pythonhosted.org/packages/96/5f/64304acee35bac703cee51656a5caf37bd18c9490561fbff225922f41d39/guessit-3.7.1.tar.gz", hash = "sha256:2c18d982ee6db30db5d59557add0324a2b49bf3940a752947510632a2b58a3c1"},
     {url = "https://files.pythonhosted.org/packages/db/5e/eec6416047845a745b1d2aee181244b380e59158e29d814021d2e511b267/guessit-3.7.1-py3-none-any.whl", hash = "sha256:c3be280ee8ec581a45ca6a654a92e317bf89567fdc55e7167452226f4f5b8b38"},
 ]
 "humanize 4.6.0" = [
     {url = "https://files.pythonhosted.org/packages/06/b1/9e491df2ee1c919d67ee328d8bc9f17b7a9af68e4077f3f5fac83a4488c9/humanize-4.6.0.tar.gz", hash = "sha256:5f1f22bc65911eb1a6ffe7659bd6598e33dcfeeb904eb16ee1e705a09bf75916"},
@@ -1786,17 +1786,17 @@
     {url = "https://files.pythonhosted.org/packages/d7/4b/cbd8e699e64a6f16ca3a8220661b5f83792b3017d0f79807cb8708d33913/iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
     {url = "https://files.pythonhosted.org/packages/ef/a6/62565a6e1cf69e10f5727360368e451d4b7f58beeac6173dc9db836a5b46/iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
 ]
 "ipdb 0.13.13" = [
     {url = "https://files.pythonhosted.org/packages/0c/4c/b075da0092003d9a55cf2ecc1cae9384a1ca4f650d51b00fc59875fe76f6/ipdb-0.13.13-py3-none-any.whl", hash = "sha256:45529994741c4ab6d2388bfa5d7b725c2cf7fe9deffabdb8a6113aa5ed449ed4"},
     {url = "https://files.pythonhosted.org/packages/3d/1b/7e07e7b752017f7693a0f4d41c13e5ca29ce8cbcfdcc1fd6c4ad8c0a27a0/ipdb-0.13.13.tar.gz", hash = "sha256:e3ac6018ef05126d442af680aad863006ec19d02290561ac88b8b1c0b0cfc726"},
 ]
-"ipython 8.12.0" = [
-    {url = "https://files.pythonhosted.org/packages/32/38/123155a40a0837c7627114995bf5f7a0d0b469cb903b9a27051198fad222/ipython-8.12.0.tar.gz", hash = "sha256:a950236df04ad75b5bc7f816f9af3d74dc118fd42f2ff7e80e8e60ca1f182e2d"},
-    {url = "https://files.pythonhosted.org/packages/9d/1c/6001840eceb489e4a3e6ae9b012cb56b109dd6b8ee286d7771166b83d111/ipython-8.12.0-py3-none-any.whl", hash = "sha256:1c183bf61b148b00bcebfa5d9b39312733ae97f6dad90d7e9b4d86c8647f498c"},
+"ipython 8.12.1" = [
+    {url = "https://files.pythonhosted.org/packages/24/fd/0859292b848cdb7f853a97aacc25d70f564465fb6eaf838ecc88e2a866cc/ipython-8.12.1-py3-none-any.whl", hash = "sha256:e3015a1a4aa09b3984fb81b9cef4f0772af5a549878b81efb094cda8bb121993"},
+    {url = "https://files.pythonhosted.org/packages/96/af/2fa34691b249cd6c54d0e20a5a542bc20c05228ae8af3e3c9c96dea62638/ipython-8.12.1.tar.gz", hash = "sha256:2442915417763b62181009259782975fa50bb5eedb97ae97fb614204bf6ecc21"},
 ]
 "isort 5.12.0" = [
     {url = "https://files.pythonhosted.org/packages/0a/63/4036ae70eea279c63e2304b91ee0ac182f467f24f86394ecfe726092340b/isort-5.12.0-py3-none-any.whl", hash = "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"},
     {url = "https://files.pythonhosted.org/packages/a9/c4/dc00e42c158fc4dda2afebe57d2e948805c06d5169007f1724f0683010a9/isort-5.12.0.tar.gz", hash = "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504"},
 ]
 "itsdangerous 2.1.2" = [
     {url = "https://files.pythonhosted.org/packages/68/5f/447e04e828f47465eeab35b5d408b7ebaaaee207f48b7136c5a7267a30ae/itsdangerous-2.1.2-py3-none-any.whl", hash = "sha256:2c2349112351b88699d8d4b6b075022c0808887cb7ad10069318a8b0bc88db44"},
@@ -2078,71 +2078,66 @@
     {url = "https://files.pythonhosted.org/packages/f0/e8/1ea9adebdccaadfc208c7517e09f5145ed5a73069779ff436393085d47a2/numpy-1.24.3-cp311-cp311-win_amd64.whl", hash = "sha256:5342cf6aad47943286afa6f1609cad9b4266a05e7f2ec408e2cf7aea7ff69d80"},
     {url = "https://files.pythonhosted.org/packages/f3/23/7cc851bae09cf4db90d42a701dfe525780883ada86bece45e3da7a07e76b/numpy-1.24.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:3c1104d3c036fb81ab923f507536daedc718d0ad5a8707c6061cdfd6d184e570"},
     {url = "https://files.pythonhosted.org/packages/fa/7d/8dfb40eecbb6bc83ca00ef979f5cdeca5909a250cb8b642dcf1fbd34c078/numpy-1.24.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:202de8f38fc4a45a3eea4b63e2f376e5f2dc64ef0fa692838e31a808520efaf7"},
 ]
 "olefile 0.46" = [
     {url = "https://files.pythonhosted.org/packages/34/81/e1ac43c6b45b4c5f8d9352396a14144bba52c8fec72a80f425f6a4d653ad/olefile-0.46.zip", hash = "sha256:133b031eaf8fd2c9399b78b8bc5b8fcbe4c31e85295749bb17a87cba8f3c3964"},
 ]
-"orjson 3.8.10" = [
-    {url = "https://files.pythonhosted.org/packages/00/12/dd85b1a82a62fe027c027b1ebbd803919186f01bcbdd6dd0feb14bd17c2f/orjson-3.8.10-cp39-cp39-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:b7b0ba074375e25c1594e770e2215941e2017c3cd121889150737fa1123e8bfe"},
-    {url = "https://files.pythonhosted.org/packages/01/cd/07b9afa29f0ade4cb6addeeff451d9fac06f6bc93f3a4bc56ecee201f4d1/orjson-3.8.10-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:979f231e3bad1c835627eef1a30db12a8af58bfb475a6758868ea7e81897211f"},
-    {url = "https://files.pythonhosted.org/packages/07/9c/6528db257e2c99bd10beecaa0a83e8b4ccddc57639fb70ce23c5103a95b7/orjson-3.8.10-cp39-cp39-macosx_10_7_x86_64.whl", hash = "sha256:af7601a78b99f0515af2f8ab12c955c0072ffcc1e437fb2556f4465783a4d813"},
-    {url = "https://files.pythonhosted.org/packages/09/5b/a36898c5b605a3281a2224db9279612adda73c5373c0cfbc0f37853d4d4e/orjson-3.8.10-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:ce49999bcbbc14791c61844bc8a69af44f5205d219be540e074660038adae6bf"},
-    {url = "https://files.pythonhosted.org/packages/0f/4a/51e92f88eaacb80557e39e6f8a45d0ed9d8d26f825ba6f96127750ba86a7/orjson-3.8.10-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:4bf2556ba99292c4dc550560384dd22e88b5cdbe6d98fb4e202e902b5775cf9f"},
-    {url = "https://files.pythonhosted.org/packages/15/ef/0b720c199e2fd4cf139e414f7f6681d73047a306893c24258b4aee91959a/orjson-3.8.10-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:34b6901c110c06ab9e8d7d0496db4bc9a0c162ca8d77f67539d22cb39e0a1ef4"},
-    {url = "https://files.pythonhosted.org/packages/17/7f/b86734aba76339447a2f823772f3cde96b2523246d7af00993514df70913/orjson-3.8.10-cp311-cp311-macosx_10_7_x86_64.whl", hash = "sha256:2073b62822738d6740bd2492f6035af5c2fd34aa198322b803dc0e70559a17b7"},
-    {url = "https://files.pythonhosted.org/packages/18/4f/3a8896a34fd1cb3137ff89939999005fc453a20941c4e3d6f5ecfc30773e/orjson-3.8.10-cp311-cp311-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:b2c4faf20b6bb5a2d7ac0c16f58eb1a3800abcef188c011296d1dc2bb2224d48"},
-    {url = "https://files.pythonhosted.org/packages/20/d8/75f018274702211445090e4641f4fea27538d3bec281a7ab4c76214e46ba/orjson-3.8.10-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:48824649019a25d3e52f6454435cf19fe1eb3d05ee697e65d257f58ae3aa94d9"},
-    {url = "https://files.pythonhosted.org/packages/21/14/e0f12fcf5e9ea20ddc0f65f4e30a89bc992dfce7cb7ed4fdfdc5854984be/orjson-3.8.10-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6fa3a26dcf0f5f2912a8ce8e87273e68b2a9526854d19fd09ea671b154418e88"},
-    {url = "https://files.pythonhosted.org/packages/23/05/298272a9a421e0552fe42030dccd05484ab1e550f635bd6854cf636490da/orjson-3.8.10-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7d27b6182f75896dd8c10ea0f78b9265a3454be72d00632b97f84d7031900dd4"},
-    {url = "https://files.pythonhosted.org/packages/23/09/1f01c425e6cc522be8ab7a1c02518b762bdaa0010a2599c34841ce5f36dd/orjson-3.8.10-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:f3e9ac9483c2b4cd794e760316966b7bd1e6afb52b0218f068a4e80c9b2db4f6"},
-    {url = "https://files.pythonhosted.org/packages/29/cb/56a202dbad43f89724a8c224d27d9f362acb0cc2b9b9765027b900888759/orjson-3.8.10-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:9b23fb0264bbdd7218aa685cb6fc71f0dcecf34182f0a8596a3a0dff010c06f9"},
-    {url = "https://files.pythonhosted.org/packages/2e/d9/e4f39cef546e40f829ce278110c9148e8a9062f85a693d08b84a2d21397f/orjson-3.8.10-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8c1825997232a324911d11c75d91e1e0338c7b723c149cf53a5fc24496c048a4"},
-    {url = "https://files.pythonhosted.org/packages/37/9e/e9556a8758eb31c7fa9ddc7db55ec3aa9f235cd04f3b9396a839dcb78314/orjson-3.8.10-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:a3fdee68c4bb3c5d6f89ed4560f1384b5d6260e48fbf868bae1a245a3c693d4d"},
-    {url = "https://files.pythonhosted.org/packages/3f/0d/824c7073f18537bdd315f6b886d8220dcd63f325500a48a919746a6e086b/orjson-3.8.10-cp310-cp310-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:bc30de5c7b3a402eb59cc0656b8ee53ca36322fc52ab67739c92635174f88336"},
-    {url = "https://files.pythonhosted.org/packages/41/6f/35fd080f429d0a52c2542dcf192410f4804e42fc6fc6fde2f957ada7b00c/orjson-3.8.10-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:27bb26e171e9cfdbec39c7ca4739b6bef8bd06c293d56d92d5e3a3fc017df17d"},
-    {url = "https://files.pythonhosted.org/packages/43/05/c2c2212ac60fb84286247e0e2d2c28441da12cc56379204d22a7a89afe5e/orjson-3.8.10-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:595e1e7d04aaaa3d41113e4eb9f765ab642173c4001182684ae9ddc621bb11c8"},
-    {url = "https://files.pythonhosted.org/packages/47/a5/9a88dadccc93f060fe758a2963936d7d0ecfa156ae0e6d75d54de3a633e4/orjson-3.8.10-cp37-cp37m-macosx_10_7_x86_64.whl", hash = "sha256:11ae68f995a50724032af297c92f20bcde31005e0bf3653b12bff9356394615b"},
-    {url = "https://files.pythonhosted.org/packages/51/6e/ab13d96f1f904fe05493adad842ca7c29d801bce5622803e0bf1561caa42/orjson-3.8.10-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:2b8cdaacecb92997916603ab232bb096d0fa9e56b418ca956b9754187d65ca06"},
-    {url = "https://files.pythonhosted.org/packages/52/d5/cecc86aaa954b105a0e4b6c10e48ad5a9ce8dc0bbac3b34fda05b665b282/orjson-3.8.10-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:e999abca892accada083f7079612307d94dd14cc105a699588a324f843216509"},
-    {url = "https://files.pythonhosted.org/packages/55/a0/b85d00a8404902c49b49eb3c454eefb1d29ddf6149c622ca92737e3ca753/orjson-3.8.10-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:61e2e51cefe7ef90c4fbbc9fd38ecc091575a3ea7751d56fad95cbebeae2a054"},
-    {url = "https://files.pythonhosted.org/packages/56/f2/86cd00c33d468ba74427b91bc41a8d050064f5b5b8ac8f5e9a39a0965ace/orjson-3.8.10-cp311-cp311-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:f7e85d4682f3ed7321d36846cad0503e944ea9579ef435d4c162e1b73ead8ac9"},
-    {url = "https://files.pythonhosted.org/packages/57/98/774c893b0a7480a1af12596066bfe095cf706a4d7ec267b413a79fcd7632/orjson-3.8.10-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:344ea91c556a2ce6423dc13401b83ab0392aa697a97fa4142c2c63a6fd0bbfef"},
-    {url = "https://files.pythonhosted.org/packages/62/e3/07b064ac235aeaa3fd2041dabfadfe7a8097ecf0a36a77f4eafb398b3d1b/orjson-3.8.10-cp37-cp37m-manylinux_2_28_x86_64.whl", hash = "sha256:abce8d319aae800fd2d774db1106f926dee0e8a5ca85998fd76391fcb58ef94f"},
-    {url = "https://files.pythonhosted.org/packages/63/b7/90fa1e1a398406b14311a17cd0d6e2b82dd1a090d94b4f12d01df0822728/orjson-3.8.10-cp310-none-win_amd64.whl", hash = "sha256:3cfe32b1227fe029a5ad989fbec0b453a34e5e6d9a977723f7c3046d062d3537"},
-    {url = "https://files.pythonhosted.org/packages/68/5c/de3ab2cd34c040d73ebc81858eb30f20e49d75ce7b859b5534294fdf8d54/orjson-3.8.10-cp38-cp38-manylinux_2_28_x86_64.whl", hash = "sha256:b6e79d8864794635974b18821b49a7f27859d17b93413d4603efadf2e92da7a5"},
-    {url = "https://files.pythonhosted.org/packages/71/5e/c1a04cb1c9a8d5ddcf2686c143aae5cfcc7a6704195f6d8f0fe75f1cc3f1/orjson-3.8.10-cp37-cp37m-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:45a5afc9cda6b8aac066dd50d8194432fbc33e71f7164f95402999b725232d78"},
-    {url = "https://files.pythonhosted.org/packages/75/47/a4a9637bfb9c90266ea0608f92f361928f0552e3a43a6b3e921241dac486/orjson-3.8.10-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:345e41abd1d9e3ecfb554e1e75ff818cf42e268bd06ad25a96c34e00f73a327e"},
-    {url = "https://files.pythonhosted.org/packages/75/b3/59f475afc874245f7059aa0ef4f65046a9742a3d4e1824e100bed74ad898/orjson-3.8.10-cp310-cp310-macosx_10_7_x86_64.whl", hash = "sha256:4dfe0651e26492d5d929bbf4322de9afbd1c51ac2e3947a7f78492b20359711d"},
-    {url = "https://files.pythonhosted.org/packages/78/e2/9d7bacf7d4457d3a2c50636ff55383f7e9121f9537b5481d43898b44239e/orjson-3.8.10-cp310-cp310-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:bce970f293825e008dbf739268dfa41dfe583aa2a1b5ef4efe53a0e92e9671ea"},
-    {url = "https://files.pythonhosted.org/packages/7c/e2/5be47f91b2e63c2837225f1d94fbcafb8900c6dde2e7c937e06a711dd0dd/orjson-3.8.10-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:c2ef690335b24f9272dbf6639353c1ffc3f196623a92b851063e28e9515cf7dd"},
-    {url = "https://files.pythonhosted.org/packages/7e/51/49757d16d9489c2848f7dfa8e42f5829140671075369860343792e832979/orjson-3.8.10-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4355c9aedfefe60904e8bd7901315ebbc8bb828f665e4c9bc94b1432e67cb6f7"},
-    {url = "https://files.pythonhosted.org/packages/88/55/63a7b35fb25a32456456a2a90b39ef168e33c401cdecc63e983806a26d30/orjson-3.8.10-cp39-none-win_amd64.whl", hash = "sha256:d2874cee6856d7c386b596e50bc517d1973d73dc40b2bd6abec057b5e7c76b2f"},
-    {url = "https://files.pythonhosted.org/packages/8c/25/5943b588710715aed87d7f611f0bb195609fecb0780bf7d27a680621d510/orjson-3.8.10-cp38-cp38-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:1486600bc1dd1db26c588dd482689edba3d72d301accbe4301db4b2b28bd7aa4"},
-    {url = "https://files.pythonhosted.org/packages/8c/ac/4f014e9fc7bf4d33af31a77da3f01cd1b3785c11a900804662d1c7f92a5a/orjson-3.8.10-cp311-cp311-manylinux_2_28_x86_64.whl", hash = "sha256:1810e5446fe68d61732e9743592da0ec807e63972eef076d09e02878c2f5958e"},
-    {url = "https://files.pythonhosted.org/packages/9f/09/7401d6fcfeabb845403d189a7e4c1a5d10a1efa29a5a6cd059747d4edae3/orjson-3.8.10-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:6a286ad379972e4f46579e772f0477e6b505f1823aabcd64ef097dbb4549e1a4"},
-    {url = "https://files.pythonhosted.org/packages/a5/80/9080fb6fbcde111215d0afb08b732a8edde8e0d4d786a6128eaefc107f4a/orjson-3.8.10-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:0826ad2dc1cea1547edff14ce580374f0061d853cbac088c71162dbfe2e52205"},
-    {url = "https://files.pythonhosted.org/packages/a7/2d/2b75783d0da53915acd7584d8ca3e1c9c49a0436aa1531d89fed50272fe9/orjson-3.8.10-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:b1f648ec89c6a426098868460c0ef8c86b457ce1378d7569ff4acb6c0c454048"},
-    {url = "https://files.pythonhosted.org/packages/a9/d5/3ff2daf4a77e95f84463a174cb6c93b90a5bcac318ed936254ef6076c6a1/orjson-3.8.10-cp310-cp310-manylinux_2_28_x86_64.whl", hash = "sha256:0b470d31244a6f647e5402aac7d2abaf7bb4f52379acf67722a09d35a45c9417"},
-    {url = "https://files.pythonhosted.org/packages/ab/fa/7a23802808f4a2ba866050952bb7fdafb1ccb85b1ed14435adeb9e452b8b/orjson-3.8.10-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b88afd662190f19c3bb5036a903589f88b1d2c2608fbb97281ce000db6b08897"},
-    {url = "https://files.pythonhosted.org/packages/ae/77/50471ad2e440e0c251c1eb52c9040856959d53e5cd9782cbc92d61eb8f87/orjson-3.8.10-cp37-cp37m-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:35d879b46b8029e1e01e9f6067928b470a4efa1ca749b6d053232b873c2dcf66"},
-    {url = "https://files.pythonhosted.org/packages/b4/39/e80e6da76cfd9565d80b815373305f7fec9f424f49edfdeaa2622b7564ac/orjson-3.8.10-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a7bce6e61cea6426309259b04c6ee2295b3f823ea51a033749459fe2dd0423b2"},
-    {url = "https://files.pythonhosted.org/packages/bb/f7/e8f06af5c1e3d7dc6f9282fab4b2c2fd8a536b6de048ce43adba3b7322db/orjson-3.8.10-cp39-cp39-manylinux_2_28_x86_64.whl", hash = "sha256:64ffd92328473a2f9af059410bd10c703206a4bbc7b70abb1bedcd8761e39eb8"},
-    {url = "https://files.pythonhosted.org/packages/bc/26/3fa52f91d6df7284e4c32af78c94fc977f0bfc1798bb8a88a276dbafdd06/orjson-3.8.10-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:cb62ec16a1c26ad9487727b529103cb6a94a1d4969d5b32dd0eab5c3f4f5a6f2"},
-    {url = "https://files.pythonhosted.org/packages/c1/db/7f0517a12a7b48271ee4ad056c54f0636053072d72bc2aca061f21ec7fb4/orjson-3.8.10.tar.gz", hash = "sha256:dcf6adb4471b69875034afab51a14b64f1026bc968175a2bb02c5f6b358bd413"},
-    {url = "https://files.pythonhosted.org/packages/d0/d0/4f74f76be448842b5b4f9e2313586fd7371b671882eed83da6199ef23c54/orjson-3.8.10-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:ad632dc330a7b39da42530c8d146f76f727d476c01b719dc6743c2b5701aaf6b"},
-    {url = "https://files.pythonhosted.org/packages/d4/72/4ede0d07f2106eb00d4491a75c6c5c5712a4fa35b981a4faf3a4d1c9eae5/orjson-3.8.10-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c08b426fae7b9577b528f99af0f7e0ff3ce46858dd9a7d1bf86d30f18df89a4c"},
-    {url = "https://files.pythonhosted.org/packages/d5/fe/780ea0b111d24989393bf538fa18b5e9f5c749914337a36fd004cae666ba/orjson-3.8.10-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:ddabc5e44702d13137949adee3c60b7091e73a664f6e07c7b428eebb2dea7bbf"},
-    {url = "https://files.pythonhosted.org/packages/e0/45/05466d703be26a1b2fff5e1ddd9139ffc9771459821205beb0bdfbe5ec57/orjson-3.8.10-cp39-cp39-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:6bbd7b3a3e2030b03c68c4d4b19a2ef5b89081cbb43c05fe2010767ef5e408db"},
-    {url = "https://files.pythonhosted.org/packages/e4/f4/77f41bfa56a32f99229fcb6b8b0c4c68092b609d54fca1af74f430641219/orjson-3.8.10-cp311-none-win_amd64.whl", hash = "sha256:26aee557cf8c93b2a971b5a4a8e3cca19780573531493ce6573aa1002f5c4378"},
-    {url = "https://files.pythonhosted.org/packages/f0/ab/71c01b3c20d6cd9258987e539b1dd6183263ea15e730a0cedb4c6259adc1/orjson-3.8.10-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:faee89e885796a9cc493c930013fa5cfcec9bfaee431ddf00f0fbfb57166a8b3"},
-    {url = "https://files.pythonhosted.org/packages/f9/28/691be2d1aa67669bb7e7d3aa3f6befeead4a8268951a889142c51e54af04/orjson-3.8.10-cp38-cp38-macosx_10_7_x86_64.whl", hash = "sha256:d953e6c2087dcd990e794f8405011369ee11cf13e9aaae3172ee762ee63947f2"},
-    {url = "https://files.pythonhosted.org/packages/fe/2b/2d4ccdd25956c146a99c743fba9c696d4f9057214a7f9cda23bd48b3be34/orjson-3.8.10-cp38-cp38-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:81aa3f321d201bff0bd0f4014ea44e51d58a9a02d8f2b0eeab2cee22611be8e1"},
-    {url = "https://files.pythonhosted.org/packages/ff/14/b52b0cb7735ed025fd7608eef27a268c1fe18706e986e1509bab6ceaf0c6/orjson-3.8.10-cp38-none-win_amd64.whl", hash = "sha256:5a0b1f4e4fa75e26f814161196e365fc0e1a16e3c07428154505b680a17df02f"},
-    {url = "https://files.pythonhosted.org/packages/ff/81/fa72d1ca2fd22549dfe7a6c88f9884b698ce8c78a5b35656ee5e6c010d7f/orjson-3.8.10-cp37-none-win_amd64.whl", hash = "sha256:e5d7f82506212e047b184c06e4bcd48c1483e101969013623cebcf51cf12cad9"},
+"orjson 3.8.11" = [
+    {url = "https://files.pythonhosted.org/packages/00/32/b6fac1a93ac31829f7263dc070551a60a0c710c131b0cb58ba41a200d941/orjson-3.8.11-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:6d7b050135669d2335e40120215ad4120e29958c139f8bab68ce06a1cb1a1b2c"},
+    {url = "https://files.pythonhosted.org/packages/00/8a/ca729b5af5972cff989197681f965c590f6120f43eb64e2e6e9abce96e28/orjson-3.8.11-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:358e515b8b19a275b259f5ee1e0efa2859b1d976b5ed5d016ac59f9e6c8788a3"},
+    {url = "https://files.pythonhosted.org/packages/03/1e/728747da836829b358fcc451c0274a3c38e060eea4654793ca6b74636c85/orjson-3.8.11-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bf48ed8d4b6ab9f23b7ee642462369d7133412d72824bad89f9bf4311c06c6a1"},
+    {url = "https://files.pythonhosted.org/packages/13/1e/c9345602fda75f228179b6d3c1c1292adc4f40e260f4536cb2b4044b7d17/orjson-3.8.11-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:7e4ded77ac7432a155d1d27a83bcadf722750aea3b9e6c4d47f2a92054ab71cb"},
+    {url = "https://files.pythonhosted.org/packages/16/45/a05192669185bd7734ebd64ee636a7b200762c6da67894cd6311d00502dd/orjson-3.8.11-cp37-cp37m-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:71a656f1c62e84c69060093e20cedff6a92e472d53ff5b8b9026b1b298542a68"},
+    {url = "https://files.pythonhosted.org/packages/17/7d/4301a4c3c9908e46a5c1186c5232d83b15af7d265817d7553b70197fd009/orjson-3.8.11-cp39-cp39-manylinux_2_28_x86_64.whl", hash = "sha256:714c3e2be6ed7e4ff6e887926d6e171bfd94fdee76d7d3bfa74ee19237a2d49d"},
+    {url = "https://files.pythonhosted.org/packages/32/7f/2e0b9ad9ab068ea32b57ae140e15e7303c2ecf86e1214ce69c8c3ee9ea9b/orjson-3.8.11-cp37-cp37m-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:b369019e597b59c4b97e9f925a3b725321fa1481c129d76c74c6ea3823f5d1e8"},
+    {url = "https://files.pythonhosted.org/packages/37/b1/4dcae237c6498f0cd2afa990bb2d93eb90c5d41a1056f5ca297d2239aa37/orjson-3.8.11-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:2fc050f8e7f2e4061c8c9968ad0be745b11b03913b77ffa8ceca65914696886c"},
+    {url = "https://files.pythonhosted.org/packages/3c/4b/67d4a9cbb504817c35e7cb31f4ef006195372497a623618665151b3a14d6/orjson-3.8.11-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3afccf7f8684dca7f017837a315de0a1ab5c095de22a4eed206d079f9325ed72"},
+    {url = "https://files.pythonhosted.org/packages/3e/28/71a77cf7db5c9debc152d411f1da0a5c3a3197a3a1e298464e070f37de00/orjson-3.8.11-cp310-cp310-macosx_11_0_x86_64.macosx_11_0_arm64.macosx_11_0_universal2.whl", hash = "sha256:9fa900bdd84b4576c8dd6f3e2a00b35797f29283af328c6e3d70addfa4c2d599"},
+    {url = "https://files.pythonhosted.org/packages/3e/93/08e22637abab902e18780a6b07a7407a68caf9cb872ac79df8e0955d97a5/orjson-3.8.11-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:37f38c8194ce086e6a9816b4b8dde5e7f383feeed92feec0385d99baf64f9b6e"},
+    {url = "https://files.pythonhosted.org/packages/49/f1/f375e5621e79d28ee989cbddf99b4e819b43b741e55ab7935fc9cc6ce08e/orjson-3.8.11-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:7c7b4fae3b8fc69c8e76f1c0694f3decfe8a57f87e7ac7779ebb59cd71135438"},
+    {url = "https://files.pythonhosted.org/packages/52/ae/4c2c3022d8d30cacd87baf955fcee3c986594dd2f103c78631f1c922389f/orjson-3.8.11-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:d47f97b99beb9bcac6e288a76b559543a61e0187443d8089204b757726b1d000"},
+    {url = "https://files.pythonhosted.org/packages/67/28/2a968fe292e85bab916db3cb8dd84a722425f4967cd92dd15f12897c1339/orjson-3.8.11-cp38-cp38-manylinux_2_28_x86_64.whl", hash = "sha256:ef52f1d5a2f89ef9049781c90ea35d5edf74374ed6ed515c286a706d1b290267"},
+    {url = "https://files.pythonhosted.org/packages/68/4c/d6e0c378686fc567790c701ada6a9616b201d4a54552bc45b4dbd2b14545/orjson-3.8.11-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:4118dcd2b5a27a22af5ad92414073f25d93bca1868f1f580056003c84841062f"},
+    {url = "https://files.pythonhosted.org/packages/72/bc/e0cf777c3d81af5be4c08df9dae968a5da14f9d2b97f6f590005c83dbd2d/orjson-3.8.11-cp37-none-win_amd64.whl", hash = "sha256:b68a07794834b7bd53ae2a8b4fe4bf010734cae3f0917d434c83b97acf8e5bce"},
+    {url = "https://files.pythonhosted.org/packages/7c/6c/c7c32c67bd8e4a589a905e1a6131a1b7cfe534cff31e66fdce1c3b11de87/orjson-3.8.11-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:d7d5aecccfaf2052cd07ed5bec8efba9ddfea055682fcd346047b1a3e9da3034"},
+    {url = "https://files.pythonhosted.org/packages/7d/8e/53878064fdc3d63acd8bdda4a161cef7eb2e0409cc0f4849752c9867fd80/orjson-3.8.11-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:0a53b3c02a38aadc5302661c2ca18645093971488992df77ce14fef16f598b2e"},
+    {url = "https://files.pythonhosted.org/packages/83/07/218d156fd331bf024347239492c6c08a2995ecbfa88bccf11947508256a1/orjson-3.8.11-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:1e97fdbb779a3b8f5d9fc7dfddef5325f81ee45897eb7cb4638d5d9734d42514"},
+    {url = "https://files.pythonhosted.org/packages/85/f9/b0a1736100fa455de898ccc57a54c07612c4919f7eaa761bbc1e5e099254/orjson-3.8.11-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:9486963d2e65482c565dacb366adb36d22aa22acf7274b61490244c3d87fa631"},
+    {url = "https://files.pythonhosted.org/packages/86/b1/6042c73cae624793f182f16d7976e42835de2c0421efbe1f431b7f8360d5/orjson-3.8.11-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e14903bfeb591a9117b7d40d81e3ebca9700b4e77bd829d6f22ea57941bb0ebf"},
+    {url = "https://files.pythonhosted.org/packages/87/ea/03502809586741c18fcf6845622ba4a6ca0e77891a3f01ec46281714deae/orjson-3.8.11-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:f4e4a1001933166fd1c257b920b241b35322bef99ed7329338bf266ac053abe7"},
+    {url = "https://files.pythonhosted.org/packages/88/3f/ee2ad2408b1f87b0fef04891151441d2a9951203460953d195c78258860a/orjson-3.8.11-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:c2d3e6b65458ed71b6797f321d6e8bfeeadee9d3d31cac47806a608ea745edd7"},
+    {url = "https://files.pythonhosted.org/packages/88/90/f3c96affce81d08d56434a84c8130da6073fab560622b3a3893c4be59ffa/orjson-3.8.11-cp39-none-win_amd64.whl", hash = "sha256:0bc3d1b93a73b46a698c054697eb2d27bdedbc5ea0d11ec5f1a6bfbec36346b5"},
+    {url = "https://files.pythonhosted.org/packages/8b/90/fd5a7d1a9b1065f3ebae6b227e25fbef8d4454ceac6cd02ae0f9d228f6b3/orjson-3.8.11-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3b65424ceee82b94e3613233b67ef110dc58f9d83b0076ec47a506289552a861"},
+    {url = "https://files.pythonhosted.org/packages/95/00/df4a035a1edba0ee1ae89152312ae837aa0b6cdcc3ac7895409cb1eca6fa/orjson-3.8.11-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f2ef933da50b31c112b252be03d1ef59e0d0552c1a08e48295bd529ce42aaab8"},
+    {url = "https://files.pythonhosted.org/packages/95/4c/61734f64828ac9e0d39382863c0b916e91661d988bb9b654168f34440a3b/orjson-3.8.11-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1103e597c16f82c241e1b02beadc9c91cecd93e60433ca73cb6464dcc235f37c"},
+    {url = "https://files.pythonhosted.org/packages/98/36/3fc17daadc49735a530ac559c037c81edc5dce0763c72b069db401f1dfc0/orjson-3.8.11-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:382f15861a4bf447ab9d07106010e61b217ef6d4245c6cf64af0c12c4c5e2346"},
+    {url = "https://files.pythonhosted.org/packages/98/bc/ad2e5a1411976153621699bc460549691fd19a96eef15faa518162665e5b/orjson-3.8.11-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:5c3b5405edc3a5f9e34516ee1a729f6c46aecf6de960ae07a7b3e95ebdd0e1d9"},
+    {url = "https://files.pythonhosted.org/packages/9e/1d/1e223d0c5eb8093ad9acdaec7f61f5ad041862fe6a27db68dbf4629c4ea1/orjson-3.8.11-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:04b60dfc1251742e79bb075d7a7c4e37078b932a02e6f005c45761bd90c69189"},
+    {url = "https://files.pythonhosted.org/packages/a2/88/90cd28ee83856171f247fca9523857a6c8aad59bad811a25d1388a5c136c/orjson-3.8.11-cp38-cp38-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:98befa717efaab7ddb847ebe47d473f6bd6f0cb53e98e6c3d487c7c58ba2e174"},
+    {url = "https://files.pythonhosted.org/packages/a2/8c/2fb31949136215c828f1ecc266720afbc36b8a80aa299e6e6f3ec9c00632/orjson-3.8.11-cp37-cp37m-manylinux_2_28_x86_64.whl", hash = "sha256:235926b38ed9b76ab2bca99ff26ece79c1c46bc10079b06e660b087aecffbe69"},
+    {url = "https://files.pythonhosted.org/packages/a5/4f/7498b3ec54017a09de2563a4c85c81dcb73894110bc3ecba3580af397445/orjson-3.8.11-cp310-none-win_amd64.whl", hash = "sha256:62eb8bdcf6f4cdbe12743e88ad98696277a75f91a35e8fb93a7ea2b9f4a7000c"},
+    {url = "https://files.pythonhosted.org/packages/a6/85/90b299ff58f851847ba9c149f563c6f18fb9fd054c17f7fe07751eadf844/orjson-3.8.11-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:176d742f53434541e50a5e659694073aa51dcbd8f29a1708a4fa1a320193c615"},
+    {url = "https://files.pythonhosted.org/packages/a9/87/7dd79550c902916ec0aa99c6dd91c5531d48e1d86befa09069ca93848fa8/orjson-3.8.11-cp310-cp310-manylinux_2_28_x86_64.whl", hash = "sha256:3c55065bc2075a5ea6ffb30462d84fd3aa5bbb7ae600855c325ee5753feec715"},
+    {url = "https://files.pythonhosted.org/packages/aa/9f/b6f78ff25edadf02fdb9d521268245f6d554ee20353594e9492a455bd874/orjson-3.8.11-cp311-cp311-macosx_11_0_x86_64.macosx_11_0_arm64.macosx_11_0_universal2.whl", hash = "sha256:982ab319b7a5ece4199caf2a2b3a28e62a8e289cb6418548ef98bced7e2a6cfe"},
+    {url = "https://files.pythonhosted.org/packages/b5/c4/6d6e4d68a789c807f615d5f9ffceead50b3df733ac0c7fc19d47b7a4cbf7/orjson-3.8.11-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0f9415b86ef154bf247fa78a6918aac50089c296e26fb6cf15bc9d7e6402a1f8"},
+    {url = "https://files.pythonhosted.org/packages/b7/43/dffa4fcdcc7d39ccf8509896523359d1c5aa02e25088b1ee2ebaf53118fa/orjson-3.8.11-cp39-cp39-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:3485c458670c0edb79ca149fe201f199dd9ccfe7ca3acbdef617e3c683e7b97f"},
+    {url = "https://files.pythonhosted.org/packages/b8/ef/4bedd95b595776c4745c8bff77aa00f755cc88cc6b94bd9e8b5595dd1a0e/orjson-3.8.11.tar.gz", hash = "sha256:882c77126c42dd93bb35288632d69b1e393863a2b752de3e5fe0112833609496"},
+    {url = "https://files.pythonhosted.org/packages/c4/07/f29b03ddbf98828aa84549a810ba13770a2a61e08621009e581152f19534/orjson-3.8.11-cp311-cp311-manylinux_2_28_x86_64.whl", hash = "sha256:173b8f8c750590f432757292cfb197582e5c14347b913b4017561d47af0e759b"},
+    {url = "https://files.pythonhosted.org/packages/cd/7a/bbcc6b07d078a877dc6bd56aa3b0b97c2e463800986cd7edf26605080a2d/orjson-3.8.11-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:66f0c9e4e8f6641497a7dc50591af3704b11468e9fc90cfb5874f28b0a61edb5"},
+    {url = "https://files.pythonhosted.org/packages/d9/f2/e051be62f8e415edd72328a0a14ee028432ff89cd20f3c808f27587e1fad/orjson-3.8.11-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:1fedcc428416e23a6c9de62a000c22ae33bbe0108302ad5d5935e29ea739bf37"},
+    {url = "https://files.pythonhosted.org/packages/da/c3/5ed5c85029d814408bb841a77b566eb777d6855b13c9c45ddeac87343b64/orjson-3.8.11-cp310-cp310-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:d70b6db9d4e1e6057829cd7fe119c217cebaf989f88d14b2445fa69fc568d03e"},
+    {url = "https://files.pythonhosted.org/packages/dc/7f/2647741a99d42422ad82e8c9424b5ee4443951c2ae5f743d1dd4a6719551/orjson-3.8.11-cp311-none-win_amd64.whl", hash = "sha256:12f647d4da0aab1997e25bed4fa2b76782b5b9d2d1bf3066b5f0a57d34d833c4"},
+    {url = "https://files.pythonhosted.org/packages/ec/5a/6e791896f99ca1f5bb5da5327143cda69b4dc62bfe1088e5e60817f1bc6a/orjson-3.8.11-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:08729e339ff3146e6de56c1166f014c3d2ec3e79ffb76d6c55d52cc892e5e477"},
+    {url = "https://files.pythonhosted.org/packages/ec/db/c9f42566e339faa5cd840c73e7698f439ec916626d79bfee8a4e7c078020/orjson-3.8.11-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cdf201e77d3fac9d8d6f68d872ef45dccfe46f30b268bb88b6c5af5065b433aa"},
+    {url = "https://files.pythonhosted.org/packages/ed/7e/e614a9d5f0a5f35b47a650cb5e01d1dfee83e0b69232f5f5474d1969b94f/orjson-3.8.11-cp39-cp39-macosx_11_0_x86_64.macosx_11_0_arm64.macosx_11_0_universal2.whl", hash = "sha256:c67ac094a4dde914297543af19f22532d7124f3a35245580d8b756c4ff2f5884"},
+    {url = "https://files.pythonhosted.org/packages/f5/d6/366c09102f8a41b168e537db866f1b681cb037c0ceb036c3b908921030ee/orjson-3.8.11-cp311-cp311-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:58c068f93d701f9466f667bf3b5cb4e4946aee940df2b07ca5101f1cf1b60ce4"},
+    {url = "https://files.pythonhosted.org/packages/f7/d5/ca8ab6e8b04bc62f605c488759cdfc3ba815ab9a18573e65d97dd763b409/orjson-3.8.11-cp38-cp38-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:f7aeefac55848aeb29f20b91fa55f9e488f446201bb1bb31dc17480d113d8955"},
+    {url = "https://files.pythonhosted.org/packages/fa/84/bd6533b9c2eeda75df9502c6514e557083f0834daa85ce89fe1c5d5b490b/orjson-3.8.11-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:553fdaf9f4b5060a0dcc517ae0c511c289c184a83d6719d03c5602ed0eef0390"},
+    {url = "https://files.pythonhosted.org/packages/fc/47/1cd81f3a396ef3a3883378c3bad80509c0f14429d62a3100d5b26f82d870/orjson-3.8.11-cp38-none-win_amd64.whl", hash = "sha256:5ff10789cbc08a9fd94507c907ba55b9315e99f20345ff8ef34fac432dacd948"},
 ]
 "packaging 23.1" = [
     {url = "https://files.pythonhosted.org/packages/ab/c3/57f0601a2d4fe15de7a553c00adbc901425661bf048f2a22dfc500caf121/packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
     {url = "https://files.pythonhosted.org/packages/b9/6c/7c6658d258d7971c5eb0d9b69fa9265879ec9a9158031206d47800ae2213/packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 "pandas 2.0.1" = [
     {url = "https://files.pythonhosted.org/packages/16/75/924e3a52c35cb105a152d29622d0f06bb0f48a677e77ddd6e11ef0004164/pandas-2.0.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e09a53a4fe8d6ae2149959a2d02e1ef2f4d2ceb285ac48f74b79798507e468b4"},
@@ -2259,17 +2254,17 @@
     {url = "https://files.pythonhosted.org/packages/d9/0e/7c6f054022235830dc2c37ec83e947d9ca09b0b0361e1e5e29983da92294/Pillow-9.5.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:cb841572862f629b99725ebaec3287fc6d275be9b14443ea746c1dd325053cbd"},
     {url = "https://files.pythonhosted.org/packages/db/5c/ba9e291850f594f89436cdca93d36c6f8610d4fb7833a6c257f4481d4174/Pillow-9.5.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:662da1f3f89a302cc22faa9f14a262c2e3951f9dbc9617609a47521c69dd9f8f"},
     {url = "https://files.pythonhosted.org/packages/e7/2a/f3ed578595f8486ee2cc07434460097d89aedd406a3db849b890ca8ec416/Pillow-9.5.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:a127ae76092974abfbfa38ca2d12cbeddcdeac0fb71f9627cc1135bedaf9d51a"},
     {url = "https://files.pythonhosted.org/packages/ec/7d/01404982db598f271ac7c0d0207860f60ab9288cfacce9872eb567cfbfe3/Pillow-9.5.0-cp37-cp37m-macosx_10_10_x86_64.whl", hash = "sha256:5d4ebf8e1db4441a55c509c4baa7a0587a0210f7cd25fcfe74dbbce7a4bd1906"},
     {url = "https://files.pythonhosted.org/packages/f2/43/0892913d499c8df2c88dee69d59e77de19e0c51754a9be82023880641c09/Pillow-9.5.0-cp39-cp39-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:8aca1152d93dcc27dc55395604dcfc55bed5f25ef4c98716a928bacba90d33a3"},
     {url = "https://files.pythonhosted.org/packages/ff/fc/48a51c0fe2a00d5def57b9981a1e0f8339b516351da7a51500383d833bc8/Pillow-9.5.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:608488bdcbdb4ba7837461442b90ea6f3079397ddc968c31265c1e056964f1ef"},
 ]
-"platformdirs 3.4.0" = [
-    {url = "https://files.pythonhosted.org/packages/5e/ac/26d3d2a99b5fc84852229fc8470ae612595900f7f52c78468fd3f3a15a27/platformdirs-3.4.0.tar.gz", hash = "sha256:a5e1536e5ea4b1c238a1364da17ff2993d5bd28e15600c2c8224008aff6bbcad"},
-    {url = "https://files.pythonhosted.org/packages/6c/fe/f6001fac1337528c14b353298d38748ee2387db0c262587ff4e7c68b5769/platformdirs-3.4.0-py3-none-any.whl", hash = "sha256:01437886022decaf285d8972f9526397bfae2ac55480ed372ed6d9eca048870a"},
+"platformdirs 3.5.0" = [
+    {url = "https://files.pythonhosted.org/packages/91/17/3836ffe140abb245726d0e21c5b9b984e2569e7027c20d12e969ec69bd8a/platformdirs-3.5.0.tar.gz", hash = "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"},
+    {url = "https://files.pythonhosted.org/packages/ce/cf/279b73aae00f7ba9d5d7664156ef323ebbf16fb556285bb223ecc45031aa/platformdirs-3.5.0-py3-none-any.whl", hash = "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4"},
 ]
 "pluggy 1.0.0" = [
     {url = "https://files.pythonhosted.org/packages/9e/01/f38e2ff29715251cf25532b9082a1589ab7e4f571ced434f98d0139336dc/pluggy-1.0.0-py2.py3-none-any.whl", hash = "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"},
     {url = "https://files.pythonhosted.org/packages/a1/16/db2d7de3474b6e37cbb9c008965ee63835bba517e22cdb8c35b5116b5ce1/pluggy-1.0.0.tar.gz", hash = "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159"},
 ]
 "praw 7.7.0" = [
     {url = "https://files.pythonhosted.org/packages/b3/93/55ae62910b94b46ecdd0ee8765289304f8df8deeaa1df7a96b0831c637ff/praw-7.7.0-py3-none-any.whl", hash = "sha256:22155c4b3006733a5ab0754136cf2226917747b61ec037ee335246fe0db5420e"},
@@ -2553,17 +2548,17 @@
     {url = "https://files.pythonhosted.org/packages/fe/68/63349d423d856993cbe1939f9189c826e757a4bb08fda931e6e7bfeb70cd/regex-2023.3.23-cp39-cp39-win32.whl", hash = "sha256:7304863f3a652dab5e68e6fb1725d05ebab36ec0390676d1736e0571ebb713ef"},
     {url = "https://files.pythonhosted.org/packages/fe/b3/afcb0c6fde8c5ee24c7cb5d29d0caafb9b57dd4b1400ca66cfc12d67e2b4/regex-2023.3.23-cp39-cp39-win_amd64.whl", hash = "sha256:54c3fa855a3f7438149de3211738dd9b5f0c733f48b54ae05aa7fce83d48d858"},
 ]
 "requests 2.24.0" = [
     {url = "https://files.pythonhosted.org/packages/45/1e/0c169c6a5381e241ba7404532c16a21d86ab872c9bed8bdcd4c423954103/requests-2.24.0-py2.py3-none-any.whl", hash = "sha256:fe75cc94a9443b9246fc7049224f75604b113c36acb93f87b80ed42c44cbb898"},
     {url = "https://files.pythonhosted.org/packages/da/67/672b422d9daf07365259958912ba533a0ecab839d4084c487a5fe9a5405f/requests-2.24.0.tar.gz", hash = "sha256:b3559a131db72c33ee969480840fff4bb6dd111de7dd27c8ee1f820f4f00231b"},
 ]
-"rich 13.3.4" = [
-    {url = "https://files.pythonhosted.org/packages/31/3b/2360352760b436f822258396e66ffb6d42585518a9cde2f93f142e64c5eb/rich-13.3.4.tar.gz", hash = "sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13f74cf454ccb2f490708b"},
-    {url = "https://files.pythonhosted.org/packages/9d/1a/28117ae737aec7c004ed5067034a8949adab43730420b50312821f466c3f/rich-13.3.4-py3-none-any.whl", hash = "sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a"},
+"rich 13.3.5" = [
+    {url = "https://files.pythonhosted.org/packages/39/03/6de23bdd88f5ee7f8b03f94f6e88108f5d7ffe6d207e95cdb06d9aa4cd57/rich-13.3.5-py3-none-any.whl", hash = "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"},
+    {url = "https://files.pythonhosted.org/packages/3d/0b/8dd34d20929c4b5e474db2e64426175469c2b7fea5ba71c6d4b3397a9729/rich-13.3.5.tar.gz", hash = "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c"},
 ]
 "ruff 0.0.263" = [
     {url = "https://files.pythonhosted.org/packages/08/01/e553109ab71bcef7dbf994b7c935f683857cdd7cef8353a76d6fad962014/ruff-0.0.263-py3-none-win_arm64.whl", hash = "sha256:ddf4503595b560bfa5fae92fa2e4cb09ec465ee4cf88cc248f10ad2e956deec3"},
     {url = "https://files.pythonhosted.org/packages/14/c9/5470c9324095f3b3f603b4f2533e89594ebdd17579f6e1111bb0712aee30/ruff-0.0.263-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:82c41f276106017b6f075dd2f2cc68e1a0b434cc75488f816fc98bd41982628d"},
     {url = "https://files.pythonhosted.org/packages/2a/4b/bea4dc1790bff48b0f5e1fa9e0b1f6d4cdff4eb76b8aa241e4c9ac73261d/ruff-0.0.263-py3-none-win_amd64.whl", hash = "sha256:9af932f665e177de62e172901704257fd6e5bfabb95893867ff7382a851459d3"},
     {url = "https://files.pythonhosted.org/packages/2e/8e/084839c7b3f3548f1985cdb6536770dee4dabab8f40d2ca181c1107b549a/ruff-0.0.263-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:15386933dd8e03aafa3186f9e996d6823105492817311338fbcb64d0ecbcd95f"},
     {url = "https://files.pythonhosted.org/packages/4c/bd/0e66ad872dc598aaead4f9b8cf3e7de07ad97435448be662853dafd6d293/ruff-0.0.263-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ddcee0d91629a4fa4bc9faebf5b94d4615d50d1cd76d1098fa71fbe1c54f4104"},
@@ -2755,17 +2750,17 @@
     {url = "https://files.pythonhosted.org/packages/df/8f/064d879849112d09df9fd2a797668c011fbd33420d15e469435da903dc22/websockets-11.0.2-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e0eeeea3b01c97fd3b5049a46c908823f68b59bf0e18d79b231d8d6764bc81ee"},
     {url = "https://files.pythonhosted.org/packages/e7/55/883b3d2fb2435d4d80cbe39237d0a1ad7f6014f05de21926e3b410a1eae6/websockets-11.0.2-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:13bd5bebcd16a4b5e403061b8b9dcc5c77e7a71e3c57e072d8dff23e33f70fba"},
     {url = "https://files.pythonhosted.org/packages/ea/8a/32116db59137262378ba72a124e5ee28f78f8a3a621281cfbddb6a634b37/websockets-11.0.2-py3-none-any.whl", hash = "sha256:5004c087d17251938a52cce21b3dbdabeecbbe432ce3f5bbbf15d8692c36eac9"},
     {url = "https://files.pythonhosted.org/packages/f0/61/c1a45650b8526b19f2aeb9f3e03532e493e6470bd99c4f67c66f5e20915b/websockets-11.0.2-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b2a573c8d71b7af937852b61e7ccb37151d719974146b5dc734aad350ef55a02"},
     {url = "https://files.pythonhosted.org/packages/f8/cb/1178fe699508fc820eead75a8f1848dbc95acdd9fb2530b784db1e4a8f58/websockets-11.0.2-pp39-pypy39_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:518ed6782d9916c5721ebd61bb7651d244178b74399028302c8617d0620af291"},
     {url = "https://files.pythonhosted.org/packages/f8/e9/885a685ddf6a4f9033b6254cb742e4f2f47acee10e5d068f0a7ea8592e52/websockets-11.0.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:143782041e95b63083b02107f31cda999f392903ae331de1307441f3a4557d51"},
 ]
-"werkzeug 2.3.1" = [
-    {url = "https://files.pythonhosted.org/packages/9b/5a/6259e936ce9b9043293dd8473943f5e6bba244c2cb6e3e5354406dfb0700/Werkzeug-2.3.1-py3-none-any.whl", hash = "sha256:69a4b8fcbb30a4c3fa81a5cebd961541273e4d222a4c08593b0b18312e14f64a"},
-    {url = "https://files.pythonhosted.org/packages/aa/70/3874542be48f8da37cecf59d931c56543a9b5704da26fad48ddf8bd024ae/Werkzeug-2.3.1.tar.gz", hash = "sha256:2d35a28a75ae03727eae14ea7d13627c0f77aed6b9998441e6dae0b387f697fc"},
+"werkzeug 2.3.2" = [
+    {url = "https://files.pythonhosted.org/packages/80/b2/7b7467a8c766121d061bae61f378fc62726c49511c5c8ae435a76d146361/Werkzeug-2.3.2-py3-none-any.whl", hash = "sha256:b7b8bc1609f35ae8e45d48a9b58d7a4eb1e41eec148d37e977e5df6ebf3398b2"},
+    {url = "https://files.pythonhosted.org/packages/fe/1a/2a4da2b4ae4f01522cf01a29d68ddc95a5ff338b56a3cbbd8b77475114cc/Werkzeug-2.3.2.tar.gz", hash = "sha256:2f3278e9ef61511cdf82cc28fc5da0f5b501dd8f01ecf5ef6a5d810048f68702"},
 ]
 "wheel 0.40.0" = [
     {url = "https://files.pythonhosted.org/packages/61/86/cc8d1ff2ca31a312a25a708c891cf9facbad4eae493b3872638db6785eb5/wheel-0.40.0-py3-none-any.whl", hash = "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"},
     {url = "https://files.pythonhosted.org/packages/fc/ef/0335f7217dd1e8096a9e8383e1d472aa14717878ffe07c4772e68b6e8735/wheel-0.40.0.tar.gz", hash = "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873"},
 ]
 "xlrd 1.2.0" = [
     {url = "https://files.pythonhosted.org/packages/aa/05/ec9d4fcbbb74bbf4da9f622b3b61aec541e4eccf31d3c60c5422ec027ce2/xlrd-1.2.0.tar.gz", hash = "sha256:546eb36cee8db40c3eaa46c351e67ffee6eeb5fa2650b71bc4c758a29a1b29b2"},
```

### Comparing `xklb-1.26.14/readme.py` & `xklb-1.26.15/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.14/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.26.15/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.14/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.26.15/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.26.14/.github/workflows/push.yaml` & `xklb-1.26.15/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.26.14/xklb/av.py` & `xklb-1.26.15/xklb/av.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,23 +102,23 @@
     import ffmpeg
 
     try:
         probe = ffmpeg.probe(f, show_chapters=None)
     except (KeyboardInterrupt, SystemExit):
         raise SystemExit(130)
     except Exception as e:
-        print(f"[{f}] Failed reading header", file=sys.stderr)
+        log.error(f"[{f}] Failed reading header")
         log.debug(e)
         if args.delete_unplayable:
             utils.trash(f)
         return None
 
     if "format" not in probe:
-        print(f"[{f}] Failed reading format", file=sys.stderr)
-        print(probe)
+        log.error(f"[{f}] Failed reading format")
+        log.warning(probe)
         return None
 
     format_ = probe["format"]
     format_.pop("size", None)
     format_.pop("bit_rate", None)
     format_.pop("format_name", None)
     format_.pop("format_long_name", None)
```

### Comparing `xklb-1.26.14/xklb/books.py` & `xklb-1.26.15/xklb/books.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             "textract is required for text database creation: pip install textract; sudo dnf install libxml2-devel libxslt-devel antiword unrtf poppler-utils tesseract sox-plugins-nonfree sox libjpeg-devel swig",
         )
     try:
         tags = textract.process(f)
         tags = REGEX_SENTENCE_ENDS.split(tags.decode())
     except Exception as e:
         log.warning(e)
-        print(f"[{f}] Failed reading file", file=sys.stderr)
+        log.error(f"[{f}] Failed reading file")
         tags = []
     return {**media, "tags": combine(tags)}
 
 
 munge_book_tags_fast = utils.with_timeout(70)(munge_book_tags)
 munge_book_tags_slow = utils.with_timeout(350)(munge_book_tags)
```

### Comparing `xklb-1.26.14/xklb/consts.py` & `xklb-1.26.15/xklb/consts.py`

 * *Files 10% similar despite different names*

```diff
@@ -104,85 +104,79 @@
         Frequency.Quarterly: "year",
         Frequency.Yearly: "year",
     }
 
     return mapper[frequency]
 
 
-def get_text_files(path: Path, OCR=False, speech_recognition=False) -> List[str]:
-    TEXTRACT_EXTENSIONS = "csv|tab|tsv|doc|docx|eml|epub|json|htm|html|msg|odt|pdf|pptx|ps|rtf|txt|log|xlsx|xls"
-    if OCR:
-        ocr_only = "|gif|jpg|jpeg|png|tif|tff|tiff"
-        TEXTRACT_EXTENSIONS += ocr_only
-    if speech_recognition:
-        speech_recognition_only = "|mp3|ogg|wav"
-        TEXTRACT_EXTENSIONS += speech_recognition_only
-
-    TEXTRACT_EXTENSIONS = TEXTRACT_EXTENSIONS.split("|")
-    text_files = []
-    for f in path.rglob("*"):
-        if f.is_file() and (f.suffix[1:].lower() in TEXTRACT_EXTENSIONS):
-            text_files.append(str(f))
-
-    return text_files
-
-
-def get_media_files(path: Path, audio=False) -> List[str]:
-    FFMPEG_EXTENSIONS = (
-        "str|aa|aax|acm|adf|adp|dtk|ads|ss2|adx|aea|afc|aix|al|apl"
-        "|mac|aptx|aptxhd|aqt|ast|obu|avi|avr|avs|avs2|avs3|bfstm|bcstm|binka"
-        "|bit|bmv|brstm|cdg|cdxl|xl|c2|302|daud|str|adp|dav|dss|dts|dtshd|dv"
-        "|dif|divx|cdata|eac3|paf|fap|flm|flv|fsb|fwse|g722|722|tco|rco"
-        "|g723_1|g729|genh|gsm|h261|h26l|h264|264|avc|hca|hevc|h265|265|idf"
-        "|ifv|cgi|ipu|sf|ircam|ivr|kux|669|abc|amf|ams|dbm|dmf|dsm|far|it|mdl"
-        "|med|mid|mod|mt2|mtm|okt|psm|ptm|s3m|stm|ult|umx|xm|itgz|itr|itz"
-        "|mdgz|mdr|mdz|s3gz|s3r|s3z|xmgz|xmr|xmz|669|amf|ams|dbm|digi|dmf"
-        "|dsm|dtm|far|gdm|ice|imf|it|j2b|m15|mdl|med|mmcmp|mms|mo3|mod|mptm"
-        "|mt2|mtm|nst|okt|ogm|ogv|plm|ppm|psm|pt36|ptm|s3m|sfx|sfx2|st26|stk|stm"
-        "|stp|ult|umx|wow|xm|xpk|flv|dat|lvf|m4v|mkv|mk3d|mka|mks|webm|mca|mcc"
-        "|mjpg|mjpeg|mpg|mpo|j2k|mlp|mods|moflex|mov|mp4|3gp|3g2|mj2|psp|m4b"
-        "|ism|ismv|isma|f4v|mp2|mpa|mpc|mjpg|mpl2|msf|mtaf|ul|musx|mvi|mxg"
-        "|v|nist|sph|nsp|nut|obu|oma|omg|pjs|pvf|yuv|cif|qcif|rgb|rt|rsd|rmvb|rm"
-        "|rsd|rso|sw|sb|sami|sbc|msbc|sbg|scc|sdr2|sds|sdx|ser|sga|shn|vb|son|imx"
-        "|sln|mjpg|stl|sup|svag|svs|tak|thd|tta|ans|art|asc|diz|ice|vt|ty|ty+|uw|ub"
-        "|v210|yuv10|vag|vc1|rcv|vob|viv|vpk|vqf|vql|vqe|wmv|wsd|xmv|xvag|yop|y4m"
-    )
-    if audio:
-        audio_only = "|opus|oga|ogg|mp3|m2a|mpga|m4a|flac|wav|wma|aac|aa3|ac3|ape"
-        FFMPEG_EXTENSIONS += audio_only
-
-    FFMPEG_EXTENSIONS = FFMPEG_EXTENSIONS.split("|")
-    media_files = []
-    for f in path.rglob("*"):
-        if f.is_file() and (f.suffix[1:].lower() in FFMPEG_EXTENSIONS):
-            media_files.append(str(f))
+TEXTRACT_EXTENSIONS = "csv|tab|tsv|doc|docx|eml|epub|json|htm|html|msg|odt|pdf|pptx|ps|rtf|txt|log|xlsx|xls".split("|")
+SPEECH_RECOGNITION_EXTENSIONS = "mp3|ogg|wav".split("|")
+OCR_EXTENSIONS = "gif|jpg|jpeg|png|tif|tff|tiff".split("|")
+AUDIO_ONLY_EXTENSIONS = "opus|oga|ogg|mp3|m2a|mpga|m4a|flac|wav|wma|aac|aa3|ac3|ape".split("|")
+VIDEO_EXTENSIONS = (
+    "str|aa|aax|acm|adf|adp|dtk|ads|ss2|adx|aea|afc|aix|al|apl"
+    "|mac|aptx|aptxhd|aqt|ast|obu|avi|avr|avs|avs2|avs3|bfstm|bcstm|binka"
+    "|bit|bmv|brstm|cdg|cdxl|xl|c2|302|daud|str|adp|dav|dss|dts|dtshd|dv"
+    "|dif|divx|cdata|eac3|paf|fap|flm|flv|fsb|fwse|g722|722|tco|rco"
+    "|g723_1|g729|genh|gsm|h261|h26l|h264|264|avc|hca|hevc|h265|265|idf"
+    "|ifv|cgi|ipu|sf|ircam|ivr|kux|669|abc|amf|ams|dbm|dmf|dsm|far|it|mdl"
+    "|med|mid|mod|mt2|mtm|okt|psm|ptm|s3m|stm|ult|umx|xm|itgz|itr|itz"
+    "|mdgz|mdr|mdz|s3gz|s3r|s3z|xmgz|xmr|xmz|669|amf|ams|dbm|digi|dmf"
+    "|dsm|dtm|far|gdm|ice|imf|it|j2b|m15|mdl|med|mmcmp|mms|mo3|mod|mptm"
+    "|mt2|mtm|nst|okt|ogm|ogv|plm|ppm|psm|pt36|ptm|s3m|sfx|sfx2|st26|stk|stm"
+    "|stp|ult|umx|wow|xm|xpk|flv|dat|lvf|m4v|mkv|mk3d|mka|mks|webm|mca|mcc"
+    "|mjpg|mjpeg|mpg|mpo|j2k|mlp|mods|moflex|mov|mp4|3gp|3g2|mj2|psp|m4b"
+    "|ism|ismv|isma|f4v|mp2|mpa|mpc|mjpg|mpl2|msf|mtaf|ul|musx|mvi|mxg"
+    "|v|nist|sph|nsp|nut|obu|oma|omg|pjs|pvf|yuv|cif|qcif|rgb|rt|rsd|rmvb|rm"
+    "|rsd|rso|sw|sb|sami|sbc|msbc|sbg|scc|sdr2|sds|sdx|ser|sga|shn|vb|son|imx"
+    "|sln|mjpg|stl|sup|svag|svs|tak|thd|tta|ans|art|asc|diz|ice|vt|ty|ty+|uw|ub"
+    "|v210|yuv10|vag|vc1|rcv|vob|viv|vpk|vqf|vql|vqe|wmv|wsd|xmv|xvag|yop|y4m"
+).split("|")
+IMAGE_EXTENSIONS = (
+    "pdf|ai|ait|png|jng|mng|arq|arw|cr2|cs1|dcp|dng|eps|epsf|ps|erf|exv|fff"
+    "|gpr|hdp|wdp|jxr|iiq|insp|jpeg|jpg|jpe|mef|mie|mos|mpo|mrw|nef|nrw|orf"
+    "|ori|pef|psd|psb|psdt|raf|raw|rw2|rwl|sr2|srw|thm|tiff|tif|x3f|flif|gif"
+    "|icc|icm|avif|heic|heif|hif|jp2|jpf|jpm|jpx|j2c|j2k|jpc|3fr|btf|dcr|k25"
+    "|kdc|miff|mif|rwz|srf|xcf|bpg|doc|dot|fla|fpx|max|ppt|pps|pot|vsd|xls"
+    "|xlt|pict|pct|360|3g2|3gp2|3gp|3gpp|aax|dvb|f4a|f4b|f4p|f4v|lrv|m4b"
+    "|m4p|m4v|mov|qt|mqv|qtif|qti|qif|cr3|crm|jxl|crw|ciff|ind|indd|indt"
+    "|nksc|vrd|xmp|la|ofr|pac|riff|rif|wav|webp|wv|asf|divx|djvu|djv|dvr-ms"
+    "|flv|insv|inx|swf|wma|wmv|exif|eip|psp|pspimage"
+).split("|")
+
+
+def get_files(base_dir: Path, extensions: List[str]) -> List[str]:
+    files = []
+    for f in base_dir.rglob("*"):
+        if f.is_file() and f.suffix[1:].lower() in extensions:
+            files.append(str(f))
 
-    return media_files
+    return files
 
 
 def get_image_files(path: Path) -> List[str]:
-    IMAGE_EXTENSIONS = (
-        "pdf|ai|ait|png|jng|mng|arq|arw|cr2|cs1|dcp|dng|eps|epsf|ps|erf|exv|fff"
-        "|gpr|hdp|wdp|jxr|iiq|insp|jpeg|jpg|jpe|mef|mie|mos|mpo|mrw|nef|nrw|orf"
-        "|ori|pef|psd|psb|psdt|raf|raw|rw2|rwl|sr2|srw|thm|tiff|tif|x3f|flif|gif"
-        "|icc|icm|avif|heic|heif|hif|jp2|jpf|jpm|jpx|j2c|j2k|jpc|3fr|btf|dcr|k25"
-        "|kdc|miff|mif|rwz|srf|xcf|bpg|doc|dot|fla|fpx|max|ppt|pps|pot|vsd|xls"
-        "|xlt|pict|pct|360|3g2|3gp2|3gp|3gpp|aax|dvb|f4a|f4b|f4p|f4v|lrv|m4b"
-        "|m4p|m4v|mov|qt|mqv|qtif|qti|qif|cr3|crm|jxl|crw|ciff|ind|indd|indt"
-        "|nksc|vrd|xmp|la|ofr|pac|riff|rif|wav|webp|wv|asf|divx|djvu|djv|dvr-ms"
-        "|flv|insv|inx|swf|wma|wmv|exif|eip|psp|pspimage"
-    )
-
-    IMAGE_EXTENSIONS = IMAGE_EXTENSIONS.split("|")
-    image_files = []
-    for f in path.rglob("*"):
-        if f.is_file() and (f.suffix[1:].lower() in IMAGE_EXTENSIONS):
-            image_files.append(str(f))
+    return get_files(path, IMAGE_EXTENSIONS)
+
+
+def get_audio_files(path: Path) -> List[str]:
+    return get_files(path, [*VIDEO_EXTENSIONS, *AUDIO_ONLY_EXTENSIONS])
+
+
+def get_video_files(path: Path) -> List[str]:
+    return get_files(path, VIDEO_EXTENSIONS)
+
+
+def get_text_files(path: Path, image_recognition=False, speech_recognition=False) -> List[str]:
+    extensions = [*TEXTRACT_EXTENSIONS]
+    if image_recognition:
+        extensions.extend(OCR_EXTENSIONS)
+    if speech_recognition:
+        extensions.extend(SPEECH_RECOGNITION_EXTENSIONS)
 
-    return image_files
+    return get_files(path, extensions)
 
 
 TUBE_IGNORE_KEYS = (
     "thumbnail",
     "thumbnails",
     "availability",
     "playable_in_embed",
```

### Comparing `xklb-1.26.14/xklb/db.py` & `xklb-1.26.15/xklb/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from xklb import consts, utils
 from xklb.utils import log
 
 
 def tracer(sql, params) -> None:
     sql = utils.remove_consecutives(dedent(sql), "\n")
-    print(f"SQL: {sql} - params: {params}")
+    log.info(f"SQL: {sql} - params: {params}")
 
 
 def connect(args, conn=None, **kwargs):
     from sqlite_utils import Database
 
     sqlite3.enable_callback_tracebacks(True)
 
@@ -65,15 +65,15 @@
     return db
 
 
 def optimize(args) -> None:
     if not hasattr(args, "force"):
         args.force = False
 
-    print("\nOptimizing database")
+    log.info("\nOptimizing database")
     from sqlite_utils import Database
 
     db: Database = args.db
 
     config = {
         "media": {
             "search_columns": ["path", "title", "tags", "mood", "genre", "description", "artist", "album"],
```

### Comparing `xklb-1.26.14/xklb/dl_config.py` & `xklb-1.26.15/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.14/xklb/dl_extract.py` & `xklb-1.26.15/xklb/dl_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 
 from xklb import consts, db, play_actions, player, tube_backend, utils
 from xklb.consts import SC, DBType
 from xklb.utils import log
 
 
 def parse_args(action, usage):
-    parser = argparse.ArgumentParser(prog="library " + action, usage=usage)
+    parser = argparse.ArgumentParser(
+        prog="library " + action,
+        usage=usage,
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
 
     subp_profile = parser.add_mutually_exclusive_group()
     subp_profile.add_argument(
         "--audio",
         "-A",
         action="store_const",
         dest="profile",
@@ -79,15 +83,15 @@
     args = parser.parse_intermixed_args()
 
     if action == SC.download:
         if args.duration:
             args.duration = utils.parse_human_to_sql(utils.human_to_seconds, "duration", args.duration)
 
         if not args.profile and not args.print:
-            print("Download profile must be specified. Use one of: --video --audio")
+            log.error("Download profile must be specified. Use one of: --video --audio")
             raise SystemExit(1)
 
     if args.db:
         args.database = args.db
     args.db = db.connect(args)
 
     args.playlists = utils.conform(args.playlists)
```

### Comparing `xklb-1.26.14/xklb/fs_extract.py` & `xklb-1.26.15/xklb/fs_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     args.db = db.connect(args)
     if hasattr(args, "paths"):
         args.paths = utils.conform(args.paths)
     args.io_multiplier = float(args.io_multiplier)
     log.info(utils.dict_filter_bool(args.__dict__))
 
     if args.profile in (DBType.audio, DBType.video) and not which("ffprobe"):
-        print("ffmpeg is not installed. Install it with your package manager.")
+        log.error("ffmpeg is not installed. Install it with your package manager.")
         raise SystemExit(3)
 
     return args
 
 
 def calculate_sparseness(stat) -> int:
     if stat.st_size == 0:
@@ -118,15 +118,15 @@
     return sparseness
 
 
 def extract_metadata(mp_args, f) -> Optional[Dict[str, int]]:
     log.debug(f)
 
     try:
-        stat = os.stat(f)
+        stat = Path(f).stat()
     except FileNotFoundError:
         return None
     except OSError:
         log.error(f"[{f}] IOError: possible filesystem corruption; check dmesg")
         return None
     except Exception as e:
         log.error(f"[{f}] %s", e)
@@ -145,15 +145,15 @@
         "ie_key": "Local",
     }
 
     if hasattr(stat, "st_blocks"):
         media = {**media, "sparseness": calculate_sparseness(stat)}
 
     if mp_args.profile == DBType.filesystem:
-        media = {**media, "is_dir": os.path.isdir(f)}
+        media = {**media, "is_dir": Path(f).is_dir()}
 
     if mp_args.profile in (DBType.audio, DBType.video):
         return av.munge_av_tags(mp_args, media, f)
 
     if mp_args.profile == DBType.text:
         try:
             start = timer()
@@ -198,19 +198,21 @@
     try:
         if args.scan_all_files:
             # thanks to these people for making rglob fast https://bugs.python.org/issue26032
             scanned_files = [str(p) for p in path.rglob("*") if p.is_file()]
         elif args.profile == DBType.filesystem:
             scanned_files = [str(p) for p in path.rglob("*")]
         elif args.profile == DBType.audio:
-            scanned_files = consts.get_media_files(path, audio=True)
+            scanned_files = consts.get_audio_files(path)
         elif args.profile == DBType.video:
-            scanned_files = consts.get_media_files(path)
+            scanned_files = consts.get_video_files(path)
         elif args.profile == DBType.text:
-            scanned_files = consts.get_text_files(path, OCR=args.ocr, speech_recognition=args.speech_recognition)
+            scanned_files = consts.get_text_files(
+                path, image_recognition=args.ocr, speech_recognition=args.speech_recognition
+            )
         elif args.profile == DBType.image:
             scanned_files = consts.get_image_files(path)
         else:
             raise Exception(f"fs_extract for profile {args.profile} not implemented")
     except FileNotFoundError:
         print(f"[{path}] Not found")
         return []
@@ -291,18 +293,18 @@
         elif args.profile in (DBType.image):
             batch_count = consts.SQLITE_PARAM_LIMIT // 20
         else:
             batch_count = consts.SQLITE_PARAM_LIMIT // 100
         chunks_count = math.ceil(len(new_files) / batch_count)
         df_chunked = utils.chunks(new_files, batch_count)
         with Parallel(n_jobs, prefer="threads" if args.profile in threadsafe else None) as parallel:
-            for idx, l in enumerate(df_chunked):
-                percent = ((batch_count * idx) + len(l)) / len(new_files) * 100
+            for idx, chunk_paths in enumerate(df_chunked):
+                percent = ((batch_count * idx) + len(chunk_paths)) / len(new_files) * 100
                 print(f"[{path}] Extracting metadata {percent:3.1f}% (chunk {idx + 1} of {chunks_count})")
-                extract_chunk(args, parallel, l)
+                extract_chunk(args, parallel, chunk_paths)
 
     _add_folder(args, path)
 
     return len(new_files)
 
 
 def extractor(args, paths) -> None:
```

### Comparing `xklb-1.26.14/xklb/gui.py` & `xklb-1.26.15/xklb/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         style.theme_use("clam")
 
         photo = PhotoImage(file="assets/kotobago.png")
         self.root.wm_iconphoto(False, photo)
         self.root.wm_attributes("-topmost", 1)
 
         for keyseq in ("<Escape>", "<Control-c>", "<Control-q>"):
-            self.root.bind(keyseq, lambda _ev: self.quit())
+            self.root.bind(keyseq, lambda _ev: self.user_quit())
 
         # menu left
         self.menu_left = Frame(self.root, width=150)
         self.menu_left_upper = Frame(self.menu_left, width=150, height=150)
         self.menu_left_lower = Frame(self.menu_left, width=150)
 
         true_btn = Button(self.menu_left_upper, text=true_action.title(), command=self.return_true, cursor="heart")
@@ -87,15 +87,15 @@
         # bind first letter key
         self.root.bind(true_action[0], lambda _ev: self.return_true())
         self.root.bind(false_action[0], lambda _ev: self.return_false())
 
         self.move_window(*(geom_data or []))
         self.root.mainloop()
 
-    def quit(self):
+    def user_quit(self):
         raise UserQuit
 
     def return_true(self):
         self.action = True
         self.root.destroy()
 
     def return_false(self):
@@ -137,21 +137,21 @@
         # monitors to find the pixel offset within the framebuffer for the window to show up in
         # that monitor but I have some doubts about whether this will work at all as well as
         # the portability of this solution. I cycle through five different monitors throughout
         # the day but I never use more than one simultaneously so I will stop over-optimizing here:
         raise NotImplementedError
 
     @staticmethod
-    def get_monitor_from_coord(X, Y):
+    def get_monitor_from_coord(coord_x, coord_y):
         import screeninfo
 
         monitors = screeninfo.get_monitors()
 
         for m in reversed(monitors):
-            if m.x <= X <= m.width + m.x and m.y <= Y <= m.height + m.y:
+            if m.x <= coord_x <= m.width + m.x and m.y <= coord_y <= m.height + m.y:
                 return m
         return monitors[0]
 
 
 def askkeep(*args, **kwargs):
     return MrSuperDialogue(*args, **kwargs).action
```

### Comparing `xklb-1.26.14/xklb/hn_extract.py` & `xklb-1.26.15/xklb/hn_extract.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,18 +96,21 @@
     sem = asyncio.Semaphore(N)
 
     async with aiohttp.ClientSession() as session:
         hn_ids = range(args.oldest_id + 1, args.latest_id)
         if not args.oldest:
             hn_ids = reversed(hn_ids)
 
+        background_tasks = set()
         for hn_id in hn_ids:
             log.debug("Getting item %s", hn_id)
             await sem.acquire()
-            asyncio.create_task(get_hn_item(session, db_queue, sem, hn_id))
+            task = asyncio.create_task(get_hn_item(session, db_queue, sem, hn_id))
+            background_tasks.add(task)
+            task.add_done_callback(background_tasks.discard)
 
         for _i in range(N):
             await sem.acquire()
 
 
 def hacker_news_add() -> None:
     args = parse_args(
@@ -127,15 +130,15 @@
 
         library hnadd --oldest hn.db
     """,
     )
     try:
         import aiohttp
     except ModuleNotFoundError as e:
-        print("aiohttp is required for hn_extract. Install with pip install aiohttp or pip install xklb[full]")
+        log.error("aiohttp is required for hn_extract. Install with pip install aiohttp or pip install xklb[full]")
         raise e
 
     args.db.enable_wal()
 
     max_item_id = get("https://hacker-news.firebaseio.com/v0/maxitem.json")
     tables = args.db.table_names()
     r = list(
```

### Comparing `xklb-1.26.14/xklb/lb.py` & `xklb-1.26.15/xklb/lb.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,31 +26,33 @@
       lb watch                 Watch local and online media
       lb read                  Read books
       lb view                  View images
 
       lb bigdirs               Discover folders which take much room
       lb dedupe                Deduplicate local db files
       lb relmv                 Move files/folders while preserving relative paths
+      lb christen              Cleanse files by giving them a new name
+
       lb mv-list               Reach a target free space by moving data across mount points
       lb scatter               Scatter files across multiple mountpoints (mergerfs balance)
 
-      lb christen              Cleanse files by giving them a new name
+      lb merge-dbs             Merge multiple SQLITE files
+      lb copy-play-counts      Copy play counts from multiple SQLITE files
 
     online media:
       lb tubeadd               Create a tube database; Add playlists
       lb tubeupdate            Fetch new videos from saved playlists
 
       lb redditadd             Create a reddit database; Add subreddits
       lb redditupdate          Fetch new posts from saved subreddits
 
     downloads:
       lb download              Download media
       lb redownload            Redownload missing media
       lb block                 Prevent downloading specific URLs
-      lb merge-dbs             Merge multiple SQLITE files
       lb merge-online-local    Merge local and online metadata
 
     playback:
       lb now                   Print what is currently playing
       lb next                  Play next file
       lb stop                  Stop all playback
       lb pause                 Pause all playback
@@ -124,25 +126,30 @@
 
     subp_bigdirs = add_parser(subparsers, "bigdirs", ["largefolders", "large_folders"])
     subp_bigdirs.set_defaults(func=scripts.bigdirs)
     subp_move_list = add_parser(subparsers, "mv-list", ["movelist", "move-list", "move_list"])
     subp_move_list.set_defaults(func=scripts.move_list)
     subp_relmv = add_parser(subparsers, "relmv", ["rel-mv", "mvrel", "mv-rel"])
     subp_relmv.set_defaults(func=scripts.relmv)
-    subp_dedupe = add_parser(subparsers, "dedupe")
-    subp_dedupe.set_defaults(func=scripts.dedupe)
+
     subp_scatter = add_parser(subparsers, "scatter")
     subp_scatter.set_defaults(func=scripts.scatter)
     subp_christen = add_parser(subparsers, "christen")
     subp_christen.set_defaults(func=scripts.christen)
-    subp_merge_db = add_parser(subparsers, "merge-dbs")
+
+    subp_merge_db = add_parser(subparsers, "merge-dbs", ["merge-db", "mergedb", "mergedbs", "merge_db", "merge_dbs"])
     subp_merge_db.set_defaults(func=scripts.merge_dbs)
+    subp_merge_db = add_parser(subparsers, "copy-play-counts")
+    subp_merge_db.set_defaults(func=scripts.copy_play_counts)
+
+    subp_dedupe = add_parser(subparsers, "dedupe")
+    subp_dedupe.set_defaults(func=scripts.dedupe)
     subp_dedupe_local = add_parser(subparsers, "merge-online-local")
     subp_dedupe_local.set_defaults(func=scripts.merge_online_local)
-    subp_optimize = add_parser(subparsers, "optimize")
+    subp_optimize = add_parser(subparsers, "optimize", ["optimize-db"])
     subp_optimize.set_defaults(func=scripts.optimize_db)
 
     subp_tubeadd = add_parser(subparsers, "tubeadd", ["dladd", "ta", "da", "xt"])
     subp_tubeadd.set_defaults(func=tube_add)
     subp_tubeupdate = add_parser(subparsers, "tubeupdate", ["dlupdate", "tu"])
     subp_tubeupdate.set_defaults(func=tube_update)
 
@@ -186,15 +193,15 @@
     subp_surf = add_parser(subparsers, "surf", ["browse", "load"])
     subp_surf.set_defaults(func=scripts.streaming_tab_loader)
 
     subp_nouns = add_parser(subparsers, "nouns")
     subp_nouns.set_defaults(func=scripts.nouns)
 
     subp_reddit_selftext = add_parser(subparsers, "reddit-selftext", ["rst"])
-    subp_reddit_selftext.set_defaults(func=scripts.parse_reddit_selftext)
+    subp_reddit_selftext.set_defaults(func=scripts.reddit_selftext)
     subp_nfb_directors = add_parser(subparsers, "nfb-films")
     subp_nfb_directors.set_defaults(func=scripts.nfb_films)
 
     parser.add_argument("--version", "-V", action="store_true")
     return parser
 
 
@@ -214,17 +221,17 @@
         del sys.argv[1]
 
     if hasattr(args, "func"):
         args.func()
         return None
     else:
         try:
-            print("Subcommand", original_argv[1], "not found")
+            log.error("Subcommand %s not found", original_argv[1])
         except Exception:
-            print("Invalid args. I see:", original_argv)
+            log.error("Invalid args. I see: %s", original_argv)
 
         print_help(parser)
         return None
 
 
 if __name__ == "__main__":
     library()
```

### Comparing `xklb-1.26.14/xklb/play_actions.py` & `xklb-1.26.15/xklb/play_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -748,15 +748,15 @@
     elif args.interdimensional_cable:
         player.socket_play(args, m)
         return
 
     else:
         r = player.local_player(args, m)
         if r.returncode != 0:
-            print("Player exited with code", r.returncode)
+            log.warning("Player exited with code %s", r.returncode)
             if args.ignore_errors:
                 return
             else:
                 raise SystemExit(r.returncode)
 
     m_columns = args.db["media"].columns_dict
     if "playhead" in m_columns:
```

### Comparing `xklb-1.26.14/xklb/playback.py` & `xklb-1.26.15/xklb/playback.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 from pathlib import Path
 
 from xklb import consts, utils
 from xklb.utils import cmd, log
 
 
 def parse_args(action) -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog=f"library {action}")
+    parser = argparse.ArgumentParser(
+        prog=f"library {action}",
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
     parser.add_argument("--mpv-socket", default=consts.DEFAULT_MPV_SOCKET)
     parser.add_argument("--chromecast-device", "--cast-to", "-t")
 
     if action == "next":
         parser.add_argument("--delete", action="store_true")
 
     parser.add_argument("--verbose", "-v", action="count", default=0)
@@ -43,17 +46,17 @@
     if path.startswith("http"):
         text = path
     else:
         text = (
             path
             + "\n"
             + "\n".join(
-                l
-                for l in cmd("ffprobe", "-hide_banner", "-loglevel", "info", path).stderr.splitlines()
-                if path not in l
+                line
+                for line in cmd("ffprobe", "-hide_banner", "-loglevel", "info", path).stderr.splitlines()
+                if path not in line
             )
         )
 
     try:
         text.encode()
         return text
     except UnicodeEncodeError:
@@ -86,15 +89,15 @@
         args.mpv.terminate()
 
     elif playing["catt"]:
         path = playing["catt"]
         print(now_playing(path))
 
     else:
-        print("Nothing seems to be playing. You may need to specify --mpv-socket or --chromecast-device")
+        log.error("Nothing seems to be playing. You may need to specify --mpv-socket or --chromecast-device")
 
 
 def catt_stop(args) -> None:
     catt_device = []
     if args.chromecast_device:
         catt_device = ["-d", args.chromecast_device]
     cmd("catt", *catt_device, "stop")
```

### Comparing `xklb-1.26.14/xklb/player.py` & `xklb-1.26.15/xklb/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,23 +159,23 @@
 
 
 def moved_media(args, moved_files: Union[str, list], base_from, base_to) -> int:
     moved_files = utils.conform(moved_files)
     modified_row_count = 0
     if moved_files:
         df_chunked = utils.chunks(moved_files, consts.SQLITE_PARAM_LIMIT)
-        for l in df_chunked:
+        for chunk_paths in df_chunked:
             with args.db.conn:
                 cursor = args.db.conn.execute(
                     f"""UPDATE media
                     SET path=REPLACE(path, '{quote(base_from)}', '{quote(base_to)}')
                     where path in ("""
-                    + ",".join(["?"] * len(l))
+                    + ",".join(["?"] * len(chunk_paths))
                     + ")",
-                    (*l,),
+                    (*chunk_paths,),
                 )
                 modified_row_count += cursor.rowcount
 
     return modified_row_count
 
 
 def set_playhead(args, path: str, playhead: int) -> int:
@@ -191,45 +191,45 @@
 
 
 def mark_media_watched(args, files) -> int:
     files = utils.conform(files)
     modified_row_count = 0
     if files:
         df_chunked = utils.chunks(files, consts.SQLITE_PARAM_LIMIT)
-        for l in df_chunked:
+        for chunk_paths in df_chunked:
             with args.db.conn:
                 cursor = args.db.conn.execute(
                     """UPDATE media
                     SET play_count = play_count + 1
                     , time_played = cast(STRFTIME('%s') as int)
                     WHERE path in ("""
-                    + ",".join(["?"] * len(l))
+                    + ",".join(["?"] * len(chunk_paths))
                     + ")",
-                    (*l,),
+                    (*chunk_paths,),
                 )
                 modified_row_count += cursor.rowcount
 
     return modified_row_count
 
 
 def mark_media_deleted(args, paths) -> int:
     paths = utils.conform(paths)
 
     modified_row_count = 0
     if paths:
         df_chunked = utils.chunks(paths, consts.SQLITE_PARAM_LIMIT)
-        for l in df_chunked:
+        for chunk_paths in df_chunked:
             with args.db.conn:
                 cursor = args.db.conn.execute(
                     f"""update media
                     set time_deleted={consts.APPLICATION_START}
                     where path in ("""
-                    + ",".join(["?"] * len(l))
+                    + ",".join(["?"] * len(chunk_paths))
                     + ")",
-                    (*l,),
+                    (*chunk_paths,),
                 )
                 modified_row_count += cursor.rowcount
 
     return modified_row_count
 
 
 def mark_media_deleted_like(args, paths) -> int:
@@ -638,15 +638,15 @@
                     if media:
                         players.append(_create_player(args, player_hole, media))
                 else:
                     log.debug("%s Check if still running", t_idx)
                     if m["process"].poll() is not None:
                         r = utils.Pclose(m["process"])
                         if r.returncode != 0:
-                            print("Player exited with code", r.returncode)
+                            log.warning("Player exited with code %s", r.returncode)
                             log.debug(join(r.args))
                             if not args.ignore_errors:
                                 raise SystemExit(r.returncode)
 
                         post_act(args, m["path"], geom_data=geom_data, media=media)
 
                         if media:
@@ -707,18 +707,18 @@
                     D[f"sum_{c}"] = sum((d[c] or 0) for d in media)
                     D[f"avg_{c}"] = sum((d[c] or 0) for d in media) / len(media)
         media = [D]
 
     else:
         if "d" in args.print:
             marked = mark_media_deleted(args, list(map(operator.itemgetter("path"), media)))
-            print(f"Marked {marked} metadata records as deleted", file=sys.stderr)
+            log.warning(f"Marked {marked} metadata records as deleted")
         if "w" in args.print:
             marked = mark_media_watched(args, list(map(operator.itemgetter("path"), media)))
-            print(f"Marked {marked} metadata records as watched", file=sys.stderr)
+            log.warning(f"Marked {marked} metadata records as watched")
 
     if "f" in args.print:
         if args.limit == 1:
             f = media[0]["path"]
             if not Path(f).exists():
                 mark_media_deleted(args, f)
                 raise FileNotFoundError
```

### Comparing `xklb-1.26.14/xklb/praw_extract.py` & `xklb-1.26.15/xklb/praw_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,19 @@
 - Windows: %APPDATA%\praw.ini
 
 More details: https://praw.readthedocs.io/en/stable/getting_started/configuration/prawini.html
 """
 
 
 def parse_args(action, usage) -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library " + action, usage=usage)
+    parser = argparse.ArgumentParser(
+        prog="library " + action,
+        usage=usage,
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
     parser.add_argument("--limit", default=1000, type=int)
     parser.add_argument("--lookback", default=4, type=int, help="Number of days to look back")
     parser.add_argument("--praw-site", default="bot1")
 
     parser.add_argument("--subreddits", action="store_true")
     parser.add_argument("--redditors", action="store_true")
```

### Comparing `xklb-1.26.14/xklb/stats.py` & `xklb-1.26.15/xklb/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 
 from xklb import consts, db, dl_extract, play_actions, tube_backend, utils
 from xklb.player import delete_playlists
 from xklb.utils import human_time, log, pipe_print
 
 
 def parse_args(prog, usage):
-    parser = argparse.ArgumentParser(prog, usage)
+    parser = argparse.ArgumentParser(
+        prog,
+        usage,
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
     parser.add_argument("--fields", "-f", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--aggregate", "-a", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--json", "-j", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--sort", "-u", nargs="+", help=argparse.SUPPRESS)
     parser.add_argument("--where", "-w", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
```

### Comparing `xklb-1.26.14/xklb/subtitle.py` & `xklb-1.26.15/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.14/xklb/tabs_actions.py` & `xklb-1.26.15/xklb/tabs_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from xklb.utils import cmd, flatten, log
 
 
 def parse_args(action) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library tabs",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        usage="""library tabs [database] [optional args]
+        usage="""library tabs DATABASE
 
     Tabs is meant to run **once per day**. Here is how you would configure it with `crontab`:
 
         45 9 * * * DISPLAY=:0 library tabs /home/my/tabs.db
 
     If things aren't working you can use `at` to simulate a similar environment as `cron`
```

### Comparing `xklb-1.26.14/xklb/tabs_extract.py` & `xklb-1.26.15/xklb/tabs_extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from xklb.consts import Frequency
 from xklb.utils import argparse_enum, log, sanitize_url
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog="library tabsadd",
-        usage=r"""library tabsadd --frequency {daily,weekly,monthly,quarterly,yearly} --category CATEGORY [--no-sanitize] [database] paths ...
+        usage=r"""library tabsadd [--frequency daily weekly (monthly) quarterly yearly] [--category CATEGORY] [--no-sanitize] DATABASE URLS ...
 
     Adding one URL:
 
         library tabsadd -f monthly -c travel ~/lb/tabs.db https://old.reddit.com/r/Colombia/top/?sort=top&t=month
 
         Depending on your shell you may need to escape the URL (add quotes)
```

### Comparing `xklb-1.26.14/xklb/tube_backend.py` & `xklb-1.26.15/xklb/tube_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -434,27 +434,27 @@
         )
 
         if args.extra:
             log.warning("[%s]: Getting extra metadata", d["path"])
             get_extra_metadata(args, d["path"], playlist_dl_opts=d.get("dl_config", "{}"))
 
 
-def save_tube_entry(args, m, info: Optional[dict] = None, error=None, URE=False) -> None:
+def save_tube_entry(args, m, info: Optional[dict] = None, error=None, unrecoverable_error=False) -> None:
     webpath = m["path"]
 
     v_id = m.get("id")
     if v_id:
         error = None if not error else error.replace(v_id, "").replace(" :", ":")
 
     if not info:  # not downloaded or already downloaded
         entry = {
             "path": webpath,
             "time_downloaded": 0,
             "time_modified": consts.now(),
-            "time_deleted": consts.APPLICATION_START if URE else 0,
+            "time_deleted": consts.APPLICATION_START if unrecoverable_error else 0,
             "error": error,
         }
         args.db["media"].upsert(utils.dict_filter_bool(entry), pk="path", alter=True)  # type: ignore
         return
 
     assert info["local_path"] != ""
     if Path(info["local_path"]).exists():
@@ -478,15 +478,15 @@
 
     entry = {
         **tube_entry,
         **fs_tags,
         "webpath": webpath,
         "time_modified": consts.now(),
         "time_downloaded": 0 if error else consts.APPLICATION_START,
-        "time_deleted": consts.APPLICATION_START if URE else 0,
+        "time_deleted": consts.APPLICATION_START if unrecoverable_error else 0,
         "error": error,
     }
     args.db["media"].upsert(utils.dict_filter_bool(entry), pk="path", alter=True)  # type: ignore
 
     if fs_tags:
         try:
             args.db["media"].delete(webpath)  # from sqlite_utils.db import NotFoundError
@@ -601,27 +601,29 @@
         else:
             if args.profile == DBType.audio:
                 info["local_path"] = ydl.prepare_filename({**info, "ext": args.ext})
             else:
                 info["local_path"] = ydl.prepare_filename(info)
 
     ydl_errors = ydl_log["error"] + ydl_log["warning"]
-    ydl_errors = "\n".join([l for l in ydl_errors if not yt_meaningless_errors.match(l)])
+    ydl_errors = "\n".join([line for line in ydl_errors if not yt_meaningless_errors.match(line)])
     ydl_full_log = ydl_log["error"] + ydl_log["warning"] + ydl_log["info"]
 
     if not ydl_log["error"] and info:
         log.debug("[%s]: No news is good news", m["path"])
         save_tube_entry(args, m, info)
-    elif any(yt_recoverable_errors.match(l) for l in ydl_full_log):
+    elif any(yt_recoverable_errors.match(line) for line in ydl_full_log):
         log.info("[%s]: Recoverable error matched (will try again later). %s", m["path"], ydl_errors)
         save_tube_entry(args, m, info, error=ydl_errors)
-    elif any(yt_unrecoverable_errors.match(l) for l in ydl_full_log):
-        matched_error = [m.string for m in utils.conform([yt_unrecoverable_errors.match(l) for l in ydl_full_log])]
+    elif any(yt_unrecoverable_errors.match(line) for line in ydl_full_log):
+        matched_error = [
+            m.string for m in utils.conform([yt_unrecoverable_errors.match(line) for line in ydl_full_log])
+        ]
         log.debug("[%s]: Unrecoverable error matched. %s", m["path"], ydl_errors or utils.combine(matched_error))
-        save_tube_entry(args, m, info, error=ydl_errors, URE=True)
-    elif any(prefix_unrecoverable_errors.match(l) for l in ydl_full_log):
+        save_tube_entry(args, m, info, error=ydl_errors, unrecoverable_error=True)
+    elif any(prefix_unrecoverable_errors.match(line) for line in ydl_full_log):
         log.warning("[%s]: Prefix error. %s", m["path"], ydl_errors)
         raise SystemExit(28)
     else:
         if ydl_errors != "":
             log.error("[%s]: Unknown error. %s", m["path"], ydl_errors)
         save_tube_entry(args, m, info, error=ydl_errors)
```

### Comparing `xklb-1.26.14/xklb/tube_extract.py` & `xklb-1.26.15/xklb/tube_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 
 from xklb import db, tube_backend, utils
 from xklb.consts import SC
 from xklb.utils import log
 
 
 def parse_args(action, usage) -> argparse.Namespace:
-    parser = argparse.ArgumentParser(prog="library " + action, usage=usage)
+    parser = argparse.ArgumentParser(
+        prog="library " + action,
+        usage=usage,
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
 
     parser.add_argument(
         "--dl-config",
         "-dl-config",
         nargs=1,
         action=utils.argparse_dict,
         default={},
```

### Comparing `xklb-1.26.14/xklb/utils.py` & `xklb-1.26.15/xklb/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,35 +20,67 @@
     import ipdb
 except ModuleNotFoundError:
     pass
 else:
     sys.breakpointhook = ipdb.set_trace
 
 
-def exit_nicely(_signal, _frame) -> NoReturn:
-    print("\nExiting... (Ctrl+C)")
-    raise SystemExit(130)
-
-
-signal.signal(signal.SIGINT, exit_nicely)
-
-
 def run_once(f):  # noqa: ANN201
     @wraps(f)
     def wrapper(*args, **kwargs):
         if not f.has_run:
             result = f(*args, **kwargs)
             f.has_run = True
             return result
         return None
 
     f.has_run = False
     return wrapper
 
 
+@run_once
+def argparse_log() -> logging.Logger:
+    parser = argparse.ArgumentParser(add_help=False)
+    parser.add_argument("-v", "--verbose", action="count", default=0)
+    args, _unknown = parser.parse_known_args()
+
+    try:
+        if args.verbose > 0 and os.getpgrp() == os.tcgetpgrp(sys.stdout.fileno()):
+            sys.excepthook = ultratb.FormattedTB(
+                mode="Context",
+                color_scheme="Neutral",
+                call_pdb=True,
+                debugger_cls=TerminalPdb,
+            )
+        else:
+            pass
+    except Exception:
+        pass
+
+    log_levels = [logging.WARNING, logging.INFO, logging.DEBUG]
+    logging.root.handlers = []  # clear any existing handlers
+    logging.basicConfig(
+        level=log_levels[min(len(log_levels) - 1, args.verbose)],
+        format="%(message)s",
+        handlers=[RichHandler(show_time=False, show_level=False, show_path=False)],
+    )
+    return logging.getLogger()
+
+
+log = argparse_log()
+
+
+def exit_nicely(_signal, _frame) -> NoReturn:
+    log.warning("\nExiting... (Ctrl+C)")
+    raise SystemExit(130)
+
+
+signal.signal(signal.SIGINT, exit_nicely)
+
+
 def repeat_until_same(fn):  # noqa: ANN201
     def wrapper(*args, **kwargs):
         p = args[0]
         while True:
             p1 = p
             p = fn(p, *args[1:], **kwargs)
             # print(fn.__name__, p)
@@ -83,46 +115,14 @@
     else:
         # CREATE_NEW_PROCESS_GROUP = 0x00000200
         # DETACHED_PROCESS = 0x00000008
         # os_kwargs = dict(creationflags=DETACHED_PROCESS | CREATE_NEW_PROCESS_GROUP)
         return {}
 
 
-@run_once
-def argparse_log() -> logging.Logger:
-    parser = argparse.ArgumentParser(add_help=False)
-    parser.add_argument("-v", "--verbose", action="count", default=0)
-    args, _unknown = parser.parse_known_args()
-
-    try:
-        if args.verbose > 0 and os.getpgrp() == os.tcgetpgrp(sys.stdout.fileno()):
-            sys.excepthook = ultratb.FormattedTB(
-                mode="Context",
-                color_scheme="Neutral",
-                call_pdb=True,
-                debugger_cls=TerminalPdb,
-            )
-        else:
-            pass
-    except Exception:
-        pass
-
-    log_levels = [logging.WARNING, logging.INFO, logging.DEBUG]
-    logging.root.handlers = []  # clear any existing handlers
-    logging.basicConfig(
-        level=log_levels[min(len(log_levels) - 1, args.verbose)],
-        format="%(message)s",
-        handlers=[RichHandler(show_time=False, show_level=False, show_path=False)],
-    )
-    return logging.getLogger()
-
-
-log = argparse_log()
-
-
 def flatten(xs: Iterable) -> Generator:
     for x in xs:
         if isinstance(x, Iterable) and not isinstance(x, (str, bytes)):
             yield from flatten(x)
         elif isinstance(x, bytes):
             yield x.decode("utf-8")
         else:
@@ -199,15 +199,15 @@
             raise SystemExit(124)
 
         signal.signal(signal.SIGALRM, exit_timeout)
         signal.alarm(seconds)
 
 
 def no_media_found() -> NoReturn:
-    print("No media found")
+    log.error("No media found")
     raise SystemExit(2)
 
 
 def sanitize_url(args, path: str) -> str:
     matches = consts.REGEX_SUBREDDIT.match(path)
     if matches:
         subreddit = conform(matches.groups())[0]
@@ -353,24 +353,24 @@
     p = b.decode("utf-8", "backslashreplace")
     p = ftfy.fix_text(p, explain=False)
     path = Path(p)
     ext = path.suffix
 
     parent = [clean_string(part) for part in path.parent.parts]
     stem = clean_string(path.stem)
-    # print('cleaned',parent, stem)
+    log.debug("cleaned %s %s", parent, stem)
 
     parent = [remove_prefixes(part, [" ", "-"]) for part in parent]
-    # print('parent_prefixes', parent, stem)
+    log.debug("parent_prefixes %s %s", parent, stem)
     parent = [remove_suffixes(part, [" ", "-", "_", "."]) for part in parent]
-    # print('parent_suffixes', parent, stem)
+    log.debug("parent_suffixes %s %s", parent, stem)
 
     stem = remove_prefixes(stem, [" ", "-"])
     stem = remove_suffixes(stem, [" ", "-", "."])
-    # print('stem', parent, stem)
+    log.debug("stem %s %s", parent, stem)
 
     parent = ["_" if part == "" else part for part in parent]
     p = str(Path(*parent) / stem[:1024])
 
     if dot_space:
         p = p.replace(" ", ".")
 
@@ -397,15 +397,15 @@
 
 def get_ip_of_chromecast(device_name) -> str:
     from pychromecast import discovery
 
     cast_infos, browser = discovery.discover_listed_chromecasts(friendly_names=[device_name])
     browser.stop_discovery()
     if not cast_infos:
-        print("Target chromecast device not found")
+        log.error("Target chromecast device not found")
         raise SystemExit(53)
 
     return cast_infos[0].host
 
 
 def path_to_mpv_watchlater_md5(path: str):
     return hashlib.md5(path.encode("utf-8")).hexdigest().upper()
@@ -762,19 +762,19 @@
     return
 
 
 def filter_file(path, sieve) -> None:
     with open(path) as fr:
         lines = fr.readlines()
         with tempfile.NamedTemporaryFile(mode="w", delete=False) as temp:
-            temp.writelines(l for l in lines if l.rstrip() not in sieve)
+            temp.writelines(line for line in lines if line.rstrip() not in sieve)
             temp.flush()
             os.fsync(temp.fileno())
     shutil.copy(temp.name, path)
-    os.remove(temp.name)
+    Path(temp.name).unlink()
 
 
 def get_mount_stats(src_mounts) -> List[Dict[str, Union[str, int]]]:
     mount_space = []
     total_used = 1
     total_free = 1
     grand_total = 1
@@ -798,15 +798,15 @@
 
     print("\nRelative free space:")
     for d in space:
         print(f"{d['mount']}: {'#' * int(d['free'] * 80)} {d['free']:.1%}")
 
 
 def mount_stats() -> None:
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(add_help=False)
     parser.add_argument("-v", "--verbose", action="count", default=0)
     parser.add_argument("mounts", nargs="+")
     args = parser.parse_args()
     print_mount_stats(get_mount_stats(args.mounts))
 
 
 def human_to_bytes(input_str) -> int:
```

### Comparing `xklb-1.26.14/xklb/scripts/bigdirs.py` & `xklb-1.26.15/xklb/scripts/bigdirs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,26 @@
 from tabulate import tabulate
 
 from xklb import db, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(
+        prog="library bigdirs",
+        usage="""library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by-deleted] [--size=+5MB]
+
+    See what folders take up space
+
+        lb bigdirs video.db
+        lb bigdirs audio.db
+        lb bigdirs fs.db
+""",
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
     parser.add_argument("--sort-by-deleted", action="store_true")
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default="4000")
     parser.add_argument("--depth", "-d", default=0, type=int, help="Depth of folders")
     parser.add_argument("--lower", type=int, help="Number of files per folder lower limit")
     parser.add_argument("--upper", type=int, help="Number of files per folder upper limit")
     parser.add_argument(
         "--size",
```

### Comparing `xklb-1.26.14/xklb/scripts/christen.py` & `xklb-1.26.15/xklb/scripts/christen.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,33 @@
 from pathlib import Path
 
 from xklb import utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(
+        prog="library christen",
+        usage="""library christen DATABASE [--run]
+
+    Rename files to be somewhat normalized
+
+    Default mode is dry-run
+
+        lb christen fs.db
+
+    To actually do stuff use the run flag
+
+        lb christen audio.db --run
+
+    You can optionally replace all the spaces in your filenames with dots
+
+        lb christen --dot-space video.db
+""",
+    )
     parser.add_argument("paths", nargs="*")
     parser.add_argument("--dot-space", action="store_true")
     parser.add_argument("--overwrite", "-f", action="store_true")
     parser.add_argument("--run", "-r", action="store_true")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     args = parser.parse_args()
```

### Comparing `xklb-1.26.14/xklb/scripts/dedupe.py` & `xklb-1.26.15/xklb/scripts/dedupe.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,21 @@
 
 from xklb import db, player, utils
 from xklb.consts import DBType
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(
+        prog="library dedupe",
+        usage="""library [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
+
+    Dedupe your files
+""",
+    )
 
     profile = parser.add_mutually_exclusive_group()
     profile.add_argument(
         "--audio",
         action="store_const",
         dest="profile",
         const=DBType.audio,
@@ -39,21 +45,29 @@
     profile.add_argument(
         "--filesystem",
         action="store_const",
         dest="profile",
         const=DBType.filesystem,
         help="Dedupe filesystem database",
     )
-    profile.add_argument("--text", action="store_const", dest="profile", const=DBType.text, help="Dedupe text database")
+    profile.add_argument(
+        "--text",
+        action="store_const",
+        dest="profile",
+        const=DBType.text,
+        help=argparse.SUPPRESS,
+        #  "Dedupe text database",
+    )
     profile.add_argument(
         "--image",
         action="store_const",
         dest="profile",
         const=DBType.image,
-        help="Dedupe image database",
+        help=argparse.SUPPRESS,
+        # "Dedupe image database",
     )
 
     parser.add_argument("--only-soft-delete", action="store_true")
     parser.add_argument("--force", "-f", action="store_true")
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default=100)
     parser.add_argument("--verbose", "-v", action="count", default=0)
 
@@ -219,15 +233,15 @@
             continue
 
         deletion_paths.append(d["duplicate_path"])
         deletion_candidates.append(d)
     duplicates = deletion_candidates
 
     if not duplicates:
-        print("No duplicates found")
+        log.error("No duplicates found")
         return
 
     tbl = deepcopy(duplicates)
     tbl = tbl[: int(args.limit)]
     tbl = utils.col_resize(tbl, "keep_path", 30)
     tbl = utils.col_resize(tbl, "duplicate_path", 30)
     tbl = utils.col_naturalsize(tbl, "duplicate_size")
@@ -245,15 +259,15 @@
     except ModuleNotFoundError:
         pass
 
     duplicates_size = sum(filter(None, map(operator.itemgetter("duplicate_size"), duplicates)))
     print(f"Approx. space savings: {humanize.naturalsize(duplicates_size // 2)}")
 
     if duplicates and (args.force or utils.confirm("Delete duplicates?")):  # type: ignore
-        print("Deleting...")
+        log.info("Deleting...")
         for d in duplicates:
             path = d["duplicate_path"]
             if not path.startswith("http") and not args.only_soft_delete:
                 utils.trash(path, detach=False)
             player.mark_media_deleted(args, path)
```

### Comparing `xklb-1.26.14/xklb/scripts/merge_dbs.py` & `xklb-1.26.15/xklb/scripts/merge_dbs.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,26 @@
 from pathlib import Path
 
 from xklb import db, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(
+        prog="library merge-dbs",
+        usage="""library merge-dbs DEST_DB SOURCE_DB ... [--upsert pk1[,pk2]]
+
+    Merge database data and tables
+
+        lb merge-dbs video.db tv.db movies.db
+        lb merge-dbs audio.db music.db podcasts.db
+""",
+    )
     parser.add_argument("database")
-    parser.add_argument("dbs", nargs="*")
+    parser.add_argument("source_dbs", nargs="+")
     parser.add_argument("--upsert")
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
     parser.add_argument("--verbose", "-v", action="count", default=0)
     args = parser.parse_intermixed_args()
 
     if args.db:
         args.database = args.db
@@ -36,13 +45,13 @@
                 args.db[table].upsert_all(data, pk=args.upsert.split(","), alter=True)
             else:
                 args.db[table].insert_all(data, alter=True, replace=True)
 
 
 def merge_dbs():
     args = parse_args()
-    for s_db in args.dbs:
+    for s_db in args.source_dbs:
         merge_db(args, s_db)
 
 
 if __name__ == "__main__":
     merge_dbs()
```

### Comparing `xklb-1.26.14/xklb/scripts/merge_online_local.py` & `xklb-1.26.15/xklb/scripts/merge_online_local.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 from xklb import consts, db, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
-        usage="""library merge-online-local database
+        prog="library merge-online-local",
+        usage="""library merge-online-local DATABASE
 
     If you have previously downloaded YouTube or other online media, you can dedupe
     your database and combine the online and local media records as long as your
     files have the youtube-dl / yt-dlp id in the filename.
     """,
     )
     parser.add_argument("database")
@@ -89,15 +90,15 @@
     tbl = utils.col_resize(tbl, "keep_path", 30)
     tbl = utils.col_resize(tbl, "duplicate_path", 30)
     tbl = utils.col_naturalsize(tbl, "duplicate_size")
     print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
 
     print(f"{duplicates_count} duplicates found (showing first {args.limit})")
     if duplicates and utils.confirm("Merge duplicates?"):  # type: ignore
-        print("Merging...")
+        log.info("Merging...")
 
         merged = []
         for d in duplicates:
             fspath = d["keep_path"]
             webpath = d["duplicate_path"]
             if webpath in merged or fspath == webpath:
                 continue
```

### Comparing `xklb-1.26.14/xklb/scripts/move_list.py` & `xklb-1.26.15/xklb/scripts/move_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 from tabulate import tabulate
 
 from xklb import db, player, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(
+        prog="library mv-list",
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default="25")
     parser.add_argument("--lower", default=4, type=int, help="Number of files per folder lower limit")
     parser.add_argument("--upper", default=4000, type=int, help="Number of files per folder upper limit")
     parser.add_argument("--verbose", "-v", action="count", default=0)
 
     parser.add_argument("mount_point")
     parser.add_argument("database")
```

### Comparing `xklb-1.26.14/xklb/scripts/optimize_db.py` & `xklb-1.26.15/xklb/scripts/optimize_db.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import argparse
 
 from xklb import db, utils
 from xklb.utils import log
 
 
 def optimize_db():
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(
+        prog="library optimize",
+        usage="""library optimize DATABASE [--force]
+
+    Optimize library databases
+
+    The force flag is usually unnecessary and it can take much longer
+""",
+    )
     parser.add_argument("--force", "-f", action="store_true")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
     parser.add_argument("database")
     args = parser.parse_args()
     if args.db:
         args.database = args.db
```

### Comparing `xklb-1.26.14/xklb/scripts/redownload.py` & `xklb-1.26.15/xklb/scripts/redownload.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 from xklb import consts, db, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
-        usage="""library redownload database
+        prog="library redownload",
+        usage="""library redownload DATABASE
 
     If you have previously downloaded YouTube or other online media, but your
     hard drive failed or you accidentally deleted something, and if that media
     is still accessible from the same URL, this script can help to redownload
     everything that was scanned-as-deleted between two timestamps.
 
     List deletions:
@@ -44,14 +45,15 @@
         ...
 
     ...or between two timestamps inclusive:
 
         $ library redownload city.db 2023-01-26T19:54:42 2023-01-26T20:45:24
 
     """,
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("--download-archive", default="~/.local/share/yt_archive.txt")
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default=100)
     parser.add_argument("--verbose", "-v", action="count", default=0)
 
     parser.add_argument("database")
     parser.add_argument("deleted_at", nargs="?")
```

### Comparing `xklb-1.26.14/xklb/scripts/relmv.py` & `xklb-1.26.15/xklb/scripts/relmv.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from xklb import utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
+        prog="library relmv",
         usage="""library relmv [--dry-run] SOURCE ... DEST
 
     Move files/folders without losing hierarchy metadata
 """,
     )
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--test", "--dry-run", action="store_true")
@@ -36,15 +37,15 @@
             relpath = str(abspath.relative_to(Path(rel_prefix).parent))
         target_dir = (dest / relpath).parent
 
         # remove duplicate path parts
         target_dir = Path(*OrderedDict.fromkeys(target_dir.parts).keys())
 
         if args.test:
-            print("mv", shlex.quote(str(abspath)), shlex.quote(str(target_dir)))
+            log.warning("mv %s %s", shlex.quote(str(abspath)), shlex.quote(str(target_dir)))
             continue
 
         target_dir.mkdir(parents=True, exist_ok=True)
         try:
             new_path = target_dir / abspath.name
             log.info("%s -> %s", abspath, new_path)
             abspath.rename(new_path)
```

### Comparing `xklb-1.26.14/xklb/scripts/scatter.py` & `xklb-1.26.15/xklb/scripts/scatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,19 @@
     Scatter without mountpoints (limited functionality; only good for balancing fs inodes)
 
         $ library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
 """
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser(usage=scatter_usage)
+    parser = argparse.ArgumentParser(
+        prog="library scatter",
+        usage=scatter_usage,
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
     parser.add_argument("--limit", "-L", "-l", "-queue", "--queue")
     parser.add_argument("--policy", "-p")
     parser.add_argument("--group", "-g")
     parser.add_argument("--sort", "-s", default="random()", help="Sort files before moving")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--srcmounts", "-m", help="/mnt/d1:/mnt/d2")
```

### Comparing `xklb-1.26.14/xklb/scripts/streaming_tab_loader.py` & `xklb-1.26.15/xklb/scripts/streaming_tab_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     You will likely want to use this setting in `about:config`
 
         browser.tabs.loadDivertedInBackground = True
 
     If you prefer GUI, check out https://unli.xyz/tabsender/
     """,
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     parser.add_argument("database")
     parser.add_argument("--count", "-n", default=2, type=int)
     parser.add_argument("--target-hosts", "--target", default=None, help="Target hosts IP:Port")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     args = parser.parse_args()
 
@@ -69,17 +70,17 @@
             if current_count < initial_count + args.count:
                 log.debug("[%s < %s]: Opening tab", current_count, initial_count + args.count)
                 fill_count = args.count - (current_count - initial_count)
                 urls = [sys.stdin.readline().rstrip() for _ in range(fill_count)]
                 try:
                     open_tabs(args, urls)
                 except ConnectionResetError:
-                    print("open_tabs ConnectionResetError")
+                    log.error("open_tabs:ConnectionResetError... trying again")
 
                 tabs_opened += fill_count
             sleep(0.1)
     finally:
-        print("Opened", tabs_opened, "tabs")
+        log.warning("Opened %s tabs", tabs_opened)
 
 
 if __name__ == "__main__":
     streaming_tab_loader()
```

### Comparing `xklb-1.26.14/xklb/scripts/mining/nfb_ca.py` & `xklb-1.26.15/xklb/scripts/mining/nfb_ca.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,18 +22,18 @@
     for el in film_list:
         pipe_print(el)
 
 
 def nfb_films() -> None:
     import sys
 
-    for l in sys.stdin:
-        l = l.rstrip("\n")
-        if l in ["", '""', "\n"]:
+    for line in sys.stdin:
+        line = line.rstrip("\n")
+        if line in ["", '""', "\n"]:
             continue
 
-        get_page_links(l)
+        get_page_links(line)
 
 
 if __name__ == "__main__":
     # echo $directors | python scripts/mining/nfb.ca.py | tee -a ~/.jobs/todo/71_Mealtime_Videos
     nfb_films()
```

### Comparing `xklb-1.26.14/xklb/scripts/mining/nouns.py` & `xklb-1.26.15/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.14/xklb/scripts/mining/pushshift.py` & `xklb-1.26.15/xklb/scripts/mining/pushshift.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,23 +64,23 @@
     )
 
     args.db.enable_wal()
 
     count = 0
     reddit_posts = []
     media = []
-    for l in sys.stdin:
-        l = l.rstrip("\n")
-        if l in ["", '""', "\n"]:
+    for line in sys.stdin:
+        line = line.rstrip("\n")
+        if line in ["", '""', "\n"]:
             continue
 
         try:
-            post_dict = orjson.loads(l)
+            post_dict = orjson.loads(line)
         except Exception:
-            print("Skipping unreadable line", l)
+            log.warning("Skipping unreadable line: %s", line)
             continue
 
         slim_dict = utils.dict_filter_bool(slim_post_data(post_dict, post_dict.get("subreddit")))
         if slim_dict:
             if "selftext" in slim_dict:
                 reddit_posts.append(slim_dict)
             elif "path" in slim_dict:
```

### Comparing `xklb-1.26.14/xklb/scripts/mining/reddit_self.py` & `xklb-1.26.15/xklb/scripts/mining/reddit_selftext.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 from urllib.parse import urlparse
 
 from xklb import db, utils
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(
+        prog="library reddit-selftext",
+        usage="""library reddit-selftext DATABASE
+
+    Extract URLs from reddit selftext from the reddit_posts table to the media table
+""",
+    )
     parser.add_argument("database")
     parser.add_argument("--verbose", "-v", action="count", default=0)
     args = parser.parse_args()
 
     args.db = db.connect(args)
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
@@ -33,15 +39,15 @@
                     external_links.add(a["href"])
             else:
                 utils.log.debug(a["href"])
 
     return internal_links, external_links
 
 
-def parse_reddit_selftext() -> None:
+def reddit_selftext() -> None:
     from markdown import markdown
 
     args = parse_args()
     m_columns = args.db["media"].columns_dict
 
     reddit_posts = list(
         args.db.query(
@@ -62,8 +68,8 @@
                 log.info(i_link)
 
         for e_link in external_links:
             args.db["media"].upsert({**d, "path": e_link, "webpage": d["path"]}, pk="path", alter=True)
 
 
 if __name__ == "__main__":
-    parse_reddit_selftext()
+    reddit_selftext()
```

### Comparing `xklb-1.26.14/xklb/scripts/mining/words.py` & `xklb-1.26.15/xklb/scripts/mining/words.py`

 * *Files identical despite different names*

### Comparing `xklb-1.26.14/assets/kotobago.png` & `xklb-1.26.15/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.26.14/.gitignore` & `xklb-1.26.15/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.26.14/LICENSE` & `xklb-1.26.15/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.26.14/README.md` & `xklb-1.26.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,45 +17,47 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.014)
+    xk media library subcommands (v1.26.015)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
       lb read                  Read books
       lb view                  View images
 
       lb bigdirs               Discover folders which take much room
       lb dedupe                Deduplicate local db files
       lb relmv                 Move files/folders while preserving relative paths
+      lb christen              Cleanse files by giving them a new name
+
       lb mv-list               Reach a target free space by moving data across mount points
       lb scatter               Scatter files across multiple mountpoints (mergerfs balance)
 
-      lb christen              Cleanse files by giving them a new name
+      lb merge-dbs             Merge multiple SQLITE files
+      lb copy-play-counts      Copy play counts from multiple SQLITE files
 
     online media:
       lb tubeadd               Create a tube database; Add playlists
       lb tubeupdate            Fetch new videos from saved playlists
 
       lb redditadd             Create a reddit database; Add subreddits
       lb redditupdate          Fetch new posts from saved subreddits
 
     downloads:
       lb download              Download media
       lb redownload            Redownload missing media
       lb block                 Prevent downloading specific URLs
-      lb merge-dbs             Merge multiple SQLITE files
       lb merge-online-local    Merge local and online metadata
 
     playback:
       lb now                   Print what is currently playing
       lb next                  Play next file
       lb stop                  Stop all playback
       lb pause                 Pause all playback
```

### Comparing `xklb-1.26.14/pyproject.toml` & `xklb-1.26.15/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 authors = [
   {name = "Jacob Chapman", email = "7908073+chapmanjacobd@users.noreply.github.com"},
 ]
 dependencies = [
   'sqlite-utils >=3.30',
-  'Markdown',
   'catt',
   'ffmpeg-python',
   'ftfy',
   'gallery-dl',
   'humanize',
   'ipython',
   'joblib',
+  'Markdown',
   'mutagen',
   'natsort',
   'praw',
   'pysubs2',
   'python-mpv-jsonipc',
   'regex',
   'rich',
@@ -82,32 +82,49 @@
 "__init__.py" = ["F401"]
 "tests/*" = ["ANN201", "PLR2004"]
 
 [tool.ruff]
 ignore = [
   "ANN001",
   "ANN002",
+  "ANN003",
   "ANN101",
+  "BLE001",
   "D100",
   "D101",
   "D102",
   "D103",
+  "D104",
   "D211",
   "D212",
   "E401",
   "E501",
+  "EM101",
   "ERA001",
+  "FBT002",
   "I001",
+  "N806",
   "PGH003",
+  "PGH004",
   "PLW2901",
+  "PTH109",
+  "PTH123",
   "RET504",
+  "RET505",
+  "RET507",
   "RUF001",
   "S101",
   "S311",
+  "S324",
+  "S606",
+  "SIM103",
   "SIM105",
+  "SIM108",
+  "T201",
+  "TRY003",
 ]
 line-length = 120
 select = ["ALL"]
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 show-fixes = true
```

### Comparing `xklb-1.26.14/PKG-INFO` & `xklb-1.26.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.26.14
+Version: 1.26.15
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -100,45 +100,47 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.26.014)
+    xk media library subcommands (v1.26.015)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
       lb read                  Read books
       lb view                  View images
 
       lb bigdirs               Discover folders which take much room
       lb dedupe                Deduplicate local db files
       lb relmv                 Move files/folders while preserving relative paths
+      lb christen              Cleanse files by giving them a new name
+
       lb mv-list               Reach a target free space by moving data across mount points
       lb scatter               Scatter files across multiple mountpoints (mergerfs balance)
 
-      lb christen              Cleanse files by giving them a new name
+      lb merge-dbs             Merge multiple SQLITE files
+      lb copy-play-counts      Copy play counts from multiple SQLITE files
 
     online media:
       lb tubeadd               Create a tube database; Add playlists
       lb tubeupdate            Fetch new videos from saved playlists
 
       lb redditadd             Create a reddit database; Add subreddits
       lb redditupdate          Fetch new posts from saved subreddits
 
     downloads:
       lb download              Download media
       lb redownload            Redownload missing media
       lb block                 Prevent downloading specific URLs
-      lb merge-dbs             Merge multiple SQLITE files
       lb merge-online-local    Merge local and online metadata
 
     playback:
       lb now                   Print what is currently playing
       lb next                  Play next file
       lb stop                  Stop all playback
       lb pause                 Pause all playback
```

