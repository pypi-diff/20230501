# Comparing `tmp/nlptoolssna-0.4.4.tar.gz` & `tmp/nlptoolssna-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.4.4.tar", last modified: Mon May  1 12:37:36 2023, max compression
+gzip compressed data, was "nlptoolssna-0.4.5.tar", last modified: Mon May  1 12:50:12 2023, max compression
```

## Comparing `nlptoolssna-0.4.4.tar` & `nlptoolssna-0.4.5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:36.027717 nlptoolssna-0.4.4/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.4.4/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.4.4/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.4.4/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.4.4/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-01 12:37:36.028710 nlptoolssna-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.4.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.905602 nlptoolssna-0.4.4/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.4.4/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.858264 nlptoolssna-0.4.4/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.859263 nlptoolssna-0.4.4/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.907595 nlptoolssna-0.4.4/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.4/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.915881 nlptoolssna-0.4.4/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.4/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.4.4/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.4/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.4/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.4.4/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.935572 nlptoolssna-0.4.4/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.936570 nlptoolssna-0.4.4/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.4/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.940569 nlptoolssna-0.4.4/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.941568 nlptoolssna-0.4.4/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.4.4/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.4.4/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.943142 nlptoolssna-0.4.4/docs/source/api/morph/
--rw-rw-rw-   0        0        0      127 2023-04-27 18:16:11.000000 nlptoolssna-0.4.4/docs/source/api/morph/morph_tagger.rst
--rw-rw-rw-   0        0        0      208 2023-05-01 09:05:51.000000 nlptoolssna-0.4.4/docs/source/api/morph.rst
--rw-rw-rw-   0        0        0      161 2023-05-01 11:08:00.000000 nlptoolssna-0.4.4/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.4.4/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.4.4/docs/source/conf.py
--rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.4.4/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.4.4/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.4.4/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.957590 nlptoolssna-0.4.4/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.963302 nlptoolssna-0.4.4/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.4.4/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     4019 2023-05-01 11:12:31.000000 nlptoolssna-0.4.4/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.4.4/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.974799 nlptoolssna-0.4.4/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.4.4/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.4.4/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.4.4/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.4.4/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.4.4/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.4.4/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.4.4/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.977165 nlptoolssna-0.4.4/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.4.4/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.979167 nlptoolssna-0.4.4/nlptools/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.4.4/nlptools/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.4.4/nlptools/jaccard/jaccardFunction.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.988157 nlptoolssna-0.4.4/nlptools/morph/
--rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.4.4/nlptools/morph/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.4.4/nlptools/morph/charsets.py
--rw-rw-rw-   0        0        0     7939 2023-05-01 12:37:15.000000 nlptoolssna-0.4.4/nlptools/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.4.4/nlptools/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.4.4/nlptools/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.4.4/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:35.992325 nlptoolssna-0.4.4/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.4.4/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.4.4/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:36.000179 nlptoolssna-0.4.4/nlptools/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.4.4/nlptools/salma/__init__.py
--rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.4.4/nlptools/salma/implication.py
--rw-rw-rw-   0        0        0      531 2023-04-18 21:41:47.000000 nlptoolssna-0.4.4/nlptools/salma/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:36.020073 nlptoolssna-0.4.4/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-01 12:37:35.000000 nlptoolssna-0.4.4/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1579 2023-05-01 12:37:35.000000 nlptoolssna-0.4.4/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 12:37:35.000000 nlptoolssna-0.4.4/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-01 12:37:35.000000 nlptoolssna-0.4.4/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.4.4/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      146 2023-05-01 12:37:35.000000 nlptoolssna-0.4.4/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-01 12:37:35.000000 nlptoolssna-0.4.4/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-01 12:37:36.030710 nlptoolssna-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0     2099 2023-04-30 11:00:39.000000 nlptoolssna-0.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:37:36.026728 nlptoolssna-0.4.4/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.4.4/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.4.4/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.373019 nlptoolssna-0.4.5/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.4.5/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.4.5/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.4.5/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-01 12:50:12.374026 nlptoolssna-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.4.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.195674 nlptoolssna-0.4.5/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.4.5/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.163285 nlptoolssna-0.4.5/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.164287 nlptoolssna-0.4.5/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.200686 nlptoolssna-0.4.5/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.5/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.221001 nlptoolssna-0.4.5/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.5/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.4.5/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.5/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.5/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.4.5/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.237844 nlptoolssna-0.4.5/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.240845 nlptoolssna-0.4.5/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.5/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.249845 nlptoolssna-0.4.5/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.251982 nlptoolssna-0.4.5/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.4.5/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.4.5/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.283798 nlptoolssna-0.4.5/docs/source/api/morph/
+-rw-rw-rw-   0        0        0      127 2023-04-27 18:16:11.000000 nlptoolssna-0.4.5/docs/source/api/morph/morph_tagger.rst
+-rw-rw-rw-   0        0        0      208 2023-05-01 09:05:51.000000 nlptoolssna-0.4.5/docs/source/api/morph.rst
+-rw-rw-rw-   0        0        0      161 2023-05-01 11:08:00.000000 nlptoolssna-0.4.5/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.4.5/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.4.5/docs/source/conf.py
+-rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.4.5/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.4.5/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.4.5/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.295041 nlptoolssna-0.4.5/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.301045 nlptoolssna-0.4.5/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.4.5/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     4019 2023-05-01 11:12:31.000000 nlptoolssna-0.4.5/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.4.5/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.320635 nlptoolssna-0.4.5/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.4.5/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.4.5/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.4.5/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.4.5/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.4.5/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-05-01 11:40:47.000000 nlptoolssna-0.4.5/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.4.5/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.324519 nlptoolssna-0.4.5/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.4.5/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.329621 nlptoolssna-0.4.5/nlptools/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.4.5/nlptools/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.4.5/nlptools/jaccard/jaccardFunction.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.342253 nlptoolssna-0.4.5/nlptools/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.4.5/nlptools/morph/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.4.5/nlptools/morph/charsets.py
+-rw-rw-rw-   0        0        0     7939 2023-05-01 12:37:15.000000 nlptoolssna-0.4.5/nlptools/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.4.5/nlptools/morph/settings.py
+-rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.4.5/nlptools/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.4.5/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.347824 nlptoolssna-0.4.5/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.4.5/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.4.5/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.353822 nlptoolssna-0.4.5/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.4.5/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.4.5/nlptools/salma/implication.py
+-rw-rw-rw-   0        0        0      531 2023-04-18 21:41:47.000000 nlptoolssna-0.4.5/nlptools/salma/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.367437 nlptoolssna-0.4.5/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-01 12:50:11.000000 nlptoolssna-0.4.5/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1579 2023-05-01 12:50:12.000000 nlptoolssna-0.4.5/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 12:50:11.000000 nlptoolssna-0.4.5/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-01 12:50:11.000000 nlptoolssna-0.4.5/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.4.5/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      146 2023-05-01 12:50:11.000000 nlptoolssna-0.4.5/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 12:50:11.000000 nlptoolssna-0.4.5/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-01 12:50:12.376963 nlptoolssna-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     2099 2023-05-01 12:50:00.000000 nlptoolssna-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 12:50:12.372023 nlptoolssna-0.4.5/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.4.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.4.5/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.4.4/CONTRIBUTING.rst` & `nlptoolssna-0.4.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/LICENSE` & `nlptoolssna-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/PKG-INFO` & `nlptoolssna-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.4.4/README.rst` & `nlptoolssna-0.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/docs/Makefile` & `nlptoolssna-0.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/docs/build/html/_images/download.png` & `nlptoolssna-0.4.5/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/docs/build/html/_static/download.png` & `nlptoolssna-0.4.5/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/docs/make.bat` & `nlptoolssna-0.4.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/docs/source/_static/download.png` & `nlptoolssna-0.4.5/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/docs/source/conf.py` & `nlptoolssna-0.4.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/docs/source/installation.rst` & `nlptoolssna-0.4.5/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.4.5/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/nlptools/arabiner/data.py` & `nlptoolssna-0.4.5/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/nlptools/arabiner/datasets.py` & `nlptoolssna-0.4.5/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/nlptools/arabiner/helpers.py` & `nlptoolssna-0.4.5/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/nlptools/arabiner/infer.py` & `nlptoolssna-0.4.5/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/nlptools/arabiner/transforms.py` & `nlptoolssna-0.4.5/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/nlptools/data/my_data.pickle` & `nlptoolssna-0.4.5/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/nlptools/jaccard/jaccardFunction.py` & `nlptoolssna-0.4.5/nlptools/jaccard/jaccardFunction.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/nlptools/morph/charsets.py` & `nlptoolssna-0.4.5/nlptools/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/nlptools/morph/morph_tagger.py` & `nlptoolssna-0.4.5/nlptools/morph/morph_tagger.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/nlptools/morph/tokenizers_words.py` & `nlptoolssna-0.4.5/nlptools/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/nlptools/parse/parser.py` & `nlptoolssna-0.4.5/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/nlptools/salma/implication.py` & `nlptoolssna-0.4.5/nlptools/salma/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/nlptools/salma/tokenizers_words.py` & `nlptoolssna-0.4.5/nlptools/salma/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.4.5/nlptoolssna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.4.4/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.4.5/nlptoolssna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/setup.cfg` & `nlptoolssna-0.4.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.4/setup.py` & `nlptoolssna-0.4.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 requirements = [
     'six',
     'farasapy',
     'tqdm',
     'requests',
     'regex',
     'pathlib',
-    'torch==1.13.0',
+    'torch==1.13.1',
     'transformers==4.24.0',
     'torchtext==0.14.0',
     'torchvision==0.14.0',
     'torchdata==0.5.1',
     'seqeval==1.2.2'
 
 ]
```

