# Comparing `tmp/nlptoolssna-0.4.2.tar.gz` & `tmp/nlptoolssna-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.4.2.tar", last modified: Sun Apr 30 11:00:47 2023, max compression
+gzip compressed data, was "nlptoolssna-0.4.3.tar", last modified: Mon May  1 11:18:22 2023, max compression
```

## Comparing `nlptoolssna-0.4.2.tar` & `nlptoolssna-0.4.3.tar`

### file list

```diff
@@ -1,82 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.572275 nlptoolssna-0.4.2/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.4.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.4.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.4.2/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.4.2/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-04-30 11:00:47.572275 nlptoolssna-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.4.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.408929 nlptoolssna-0.4.2/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.4.2/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.379791 nlptoolssna-0.4.2/docs/build/
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.380678 nlptoolssna-0.4.2/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.413973 nlptoolssna-0.4.2/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.2/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.432566 nlptoolssna-0.4.2/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.2/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.4.2/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.2/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.2/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.4.2/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.455494 nlptoolssna-0.4.2/docs/source/
--rw-rw-rw-   0        0        0      318 2023-04-27 09:55:38.000000 nlptoolssna-0.4.2/docs/source/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.458078 nlptoolssna-0.4.2/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.2/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.462438 nlptoolssna-0.4.2/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.474888 nlptoolssna-0.4.2/docs/source/api/morph/
--rw-rw-rw-   0        0        0       48 2023-04-26 20:02:35.000000 nlptoolssna-0.4.2/docs/source/api/morph/charsets.rst
--rw-rw-rw-   0        0        0       66 2023-04-26 20:02:52.000000 nlptoolssna-0.4.2/docs/source/api/morph/lemmatizeSentence.rst
--rw-rw-rw-   0        0        0      127 2023-04-27 18:16:11.000000 nlptoolssna-0.4.2/docs/source/api/morph/morph_tagger.rst
--rw-rw-rw-   0        0        0       65 2023-04-26 20:03:13.000000 nlptoolssna-0.4.2/docs/source/api/morph/tokenizers_words.rst
--rw-rw-rw-   0        0        0      280 2023-04-27 12:17:19.000000 nlptoolssna-0.4.2/docs/source/api/morph.rst
--rw-rw-rw-   0        0        0      140 2023-04-26 20:11:06.000000 nlptoolssna-0.4.2/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.4.2/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.4.2/docs/source/conf.py
--rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.4.2/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.4.2/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.4.2/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.484214 nlptoolssna-0.4.2/nlptools/
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.489584 nlptoolssna-0.4.2/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.4.2/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     2527 2023-04-27 21:39:46.000000 nlptoolssna-0.4.2/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.4.2/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.517729 nlptoolssna-0.4.2/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.4.2/nlptools/arabiner/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.4.2/nlptools/arabiner/data.py
--rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.4.2/nlptools/arabiner/datasets.py
--rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.4.2/nlptools/arabiner/helpers.py
--rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.4.2/nlptools/arabiner/infer.py
--rw-rw-rw-   0        0        0     5092 2023-04-30 06:31:23.000000 nlptoolssna-0.4.2/nlptools/arabiner/transforms.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.4.2/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.521619 nlptoolssna-0.4.2/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.4.2/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.529350 nlptoolssna-0.4.2/nlptools/jaccard/
--rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.4.2/nlptools/jaccard/__init__.py
--rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.4.2/nlptools/jaccard/jaccardFunction.py
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.542662 nlptoolssna-0.4.2/nlptools/morph/
--rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.4.2/nlptools/morph/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.4.2/nlptools/morph/charsets.py
--rw-rw-rw-   0        0        0     7629 2023-04-29 19:50:22.000000 nlptoolssna-0.4.2/nlptools/morph/morph_tagger.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.4.2/nlptools/morph/settings.py
--rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.4.2/nlptools/morph/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.4.2/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.547503 nlptoolssna-0.4.2/nlptools/parse/
--rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.4.2/nlptools/parse/__init__.py
--rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.4.2/nlptools/parse/parser.py
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.554504 nlptoolssna-0.4.2/nlptools/salma/
--rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.4.2/nlptools/salma/__init__.py
--rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.4.2/nlptools/salma/implication.py
--rw-rw-rw-   0        0        0      531 2023-04-18 21:41:47.000000 nlptoolssna-0.4.2/nlptools/salma/tokenizers_words.py
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.567157 nlptoolssna-0.4.2/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-04-30 11:00:47.000000 nlptoolssna-0.4.2/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1653 2023-04-30 11:00:47.000000 nlptoolssna-0.4.2/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 11:00:47.000000 nlptoolssna-0.4.2/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-30 11:00:47.000000 nlptoolssna-0.4.2/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.4.2/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      146 2023-04-30 11:00:47.000000 nlptoolssna-0.4.2/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-30 11:00:47.000000 nlptoolssna-0.4.2/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-04-30 11:00:47.574164 nlptoolssna-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     2099 2023-04-30 11:00:39.000000 nlptoolssna-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 11:00:47.570880 nlptoolssna-0.4.2/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.4.2/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.4.2/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.795696 nlptoolssna-0.4.3/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.4.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.4.3/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.4.3/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-01 11:18:22.796694 nlptoolssna-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.4.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.708425 nlptoolssna-0.4.3/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.4.3/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.669275 nlptoolssna-0.4.3/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.671298 nlptoolssna-0.4.3/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.710430 nlptoolssna-0.4.3/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.3/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.716423 nlptoolssna-0.4.3/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.3/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.4.3/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.3/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.4.3/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.4.3/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.727018 nlptoolssna-0.4.3/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.729035 nlptoolssna-0.4.3/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.4.3/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.732036 nlptoolssna-0.4.3/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.734036 nlptoolssna-0.4.3/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.4.3/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.4.3/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.735035 nlptoolssna-0.4.3/docs/source/api/morph/
+-rw-rw-rw-   0        0        0      127 2023-04-27 18:16:11.000000 nlptoolssna-0.4.3/docs/source/api/morph/morph_tagger.rst
+-rw-rw-rw-   0        0        0      208 2023-05-01 09:05:51.000000 nlptoolssna-0.4.3/docs/source/api/morph.rst
+-rw-rw-rw-   0        0        0      161 2023-05-01 11:08:00.000000 nlptoolssna-0.4.3/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.4.3/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.4.3/docs/source/conf.py
+-rw-rw-rw-   0        0        0      329 2023-04-27 09:52:07.000000 nlptoolssna-0.4.3/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.4.3/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.4.3/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.741037 nlptoolssna-0.4.3/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.745145 nlptoolssna-0.4.3/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.4.3/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     4019 2023-05-01 11:12:31.000000 nlptoolssna-0.4.3/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      134 2023-04-15 18:20:16.000000 nlptoolssna-0.4.3/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.756143 nlptoolssna-0.4.3/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.4.3/nlptools/arabiner/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-04-30 06:31:38.000000 nlptoolssna-0.4.3/nlptools/arabiner/data.py
+-rw-rw-rw-   0        0        0     5061 2023-04-30 06:31:27.000000 nlptoolssna-0.4.3/nlptools/arabiner/datasets.py
+-rw-rw-rw-   0        0        0     3676 2023-03-29 20:23:29.000000 nlptoolssna-0.4.3/nlptools/arabiner/helpers.py
+-rw-rw-rw-   0        0        0     1365 2023-04-30 06:28:09.000000 nlptoolssna-0.4.3/nlptools/arabiner/infer.py
+-rw-rw-rw-   0        0        0     5092 2023-04-30 06:31:23.000000 nlptoolssna-0.4.3/nlptools/arabiner/transforms.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.4.3/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.762244 nlptoolssna-0.4.3/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.4.3/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.765243 nlptoolssna-0.4.3/nlptools/jaccard/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:47:17.000000 nlptoolssna-0.4.3/nlptools/jaccard/__init__.py
+-rw-rw-rw-   0        0        0     7425 2023-04-18 10:15:57.000000 nlptoolssna-0.4.3/nlptools/jaccard/jaccardFunction.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.772926 nlptoolssna-0.4.3/nlptools/morph/
+-rw-rw-rw-   0        0        0        0 2023-04-15 18:29:14.000000 nlptoolssna-0.4.3/nlptools/morph/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.4.3/nlptools/morph/charsets.py
+-rw-rw-rw-   0        0        0     8399 2023-05-01 11:17:10.000000 nlptoolssna-0.4.3/nlptools/morph/morph_tagger.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.4.3/nlptools/morph/settings.py
+-rw-rw-rw-   0        0        0      592 2023-04-15 18:51:58.000000 nlptoolssna-0.4.3/nlptools/morph/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.4.3/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.776152 nlptoolssna-0.4.3/nlptools/parse/
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:45:31.000000 nlptoolssna-0.4.3/nlptools/parse/__init__.py
+-rw-rw-rw-   0        0        0     4517 2023-04-11 20:46:38.000000 nlptoolssna-0.4.3/nlptools/parse/parser.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.781149 nlptoolssna-0.4.3/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.4.3/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0    20593 2023-04-06 21:04:01.000000 nlptoolssna-0.4.3/nlptools/salma/implication.py
+-rw-rw-rw-   0        0        0      531 2023-04-18 21:41:47.000000 nlptoolssna-0.4.3/nlptools/salma/tokenizers_words.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.791699 nlptoolssna-0.4.3/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-01 11:18:22.000000 nlptoolssna-0.4.3/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1579 2023-05-01 11:18:22.000000 nlptoolssna-0.4.3/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 11:18:22.000000 nlptoolssna-0.4.3/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-01 11:18:22.000000 nlptoolssna-0.4.3/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 18:40:32.000000 nlptoolssna-0.4.3/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      146 2023-05-01 11:18:22.000000 nlptoolssna-0.4.3/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-01 11:18:22.000000 nlptoolssna-0.4.3/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-01 11:18:22.797695 nlptoolssna-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     2099 2023-04-30 11:00:39.000000 nlptoolssna-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 11:18:22.794695 nlptoolssna-0.4.3/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.4.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.4.3/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.4.2/CONTRIBUTING.rst` & `nlptoolssna-0.4.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/LICENSE` & `nlptoolssna-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/PKG-INFO` & `nlptoolssna-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.4.2/README.rst` & `nlptoolssna-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/docs/Makefile` & `nlptoolssna-0.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/docs/build/html/_images/download.png` & `nlptoolssna-0.4.3/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/docs/build/html/_static/download.png` & `nlptoolssna-0.4.3/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/docs/make.bat` & `nlptoolssna-0.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/docs/source/_static/download.png` & `nlptoolssna-0.4.3/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/docs/source/conf.py` & `nlptoolssna-0.4.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/docs/source/installation.rst` & `nlptoolssna-0.4.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/nlptools/arabiner/data.py` & `nlptoolssna-0.4.3/nlptools/arabiner/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/nlptools/arabiner/datasets.py` & `nlptoolssna-0.4.3/nlptools/arabiner/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/nlptools/arabiner/helpers.py` & `nlptoolssna-0.4.3/nlptools/arabiner/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/nlptools/arabiner/infer.py` & `nlptoolssna-0.4.3/nlptools/arabiner/infer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/nlptools/arabiner/transforms.py` & `nlptoolssna-0.4.3/nlptools/arabiner/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/nlptools/data/my_data.pickle` & `nlptoolssna-0.4.3/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/nlptools/jaccard/jaccardFunction.py` & `nlptoolssna-0.4.3/nlptools/jaccard/jaccardFunction.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/nlptools/morph/charsets.py` & `nlptoolssna-0.4.3/nlptools/morph/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/nlptools/morph/morph_tagger.py` & `nlptoolssna-0.4.3/nlptools/morph/morph_tagger.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,24 +18,23 @@
        #Load the serialized data from the file
        ALMA_dic = pickle.load(f)
        #print(ALMA_dic)
        return ALMA_dic
 
 def tag(token, language, task):
     """
-    Given a token, this method retrives the possible morphological solutions (lemma, pos, frequency, task and language) filterd by spesific
-    language and task.
+    Given a token, this method retrives the morphological solutions [token, lemma, pos, frequency, task and language] filterd by spesific language and task.
           
     Args:
-        token (str): The Arabic token to be morphologcaly tagged.
-        language (str): The language to filter the results by, [MSA, Pal, ].
-        task (str): The task to filter the results by [lemmatizer, pos, full]. The defualt task if not specisifd is `full`.
+        - token (:obj:`str`): The Arabic token to be morphologcaly tagged.
+        - language (:obj:`str`): The language to filter the results by [MSA, Pal, Lebanese, Iraqi, Libyan, Syrian, Sudanese, Yemeni]. The defualt task if not specisifd is `MSA`.
+        - task (:obj:`str`): The task to filter the results by [lemmatizer, pos, full]. The defualt task if not specisifd is `full`.
 
     Returns:
-        list: A list of [token, lemma, pos_ar, lemma_freq, language, task], where:
+        list (:obj:`list`): A list of [token, lemma, pos_ar, lemma_freq, language, task], where:
             - token: the original input token
             - lemma: the lemma of the token
             - pos_ar: the part of speech of the token in Arabic
             - lemma_freq: the frequency of the lemma in the dictionary
             - language: the input language 
             - task: the input task 
 
@@ -48,133 +47,142 @@
             return  [token, soluation[3], soluation[2],  soluation[-2], soluation[-1]]
         elif soluation[-2] == language and soluation[-1] ==task:
             return [token, soluation[3], soluation[2],  soluation[-2], soluation[-1]]
         return []
     else:
         return []
 
-def lemmatize_sentence(text ,language, task):
+def analyze_morphology(text ,language, task):
    """
-    This method takes a text as input and returns a morphological solution for each token in this text, Based on the input language and task, such that:
+    This method takes a text as input and returns a morphological solution for each token in this text, Based on the input language and task, such that,
     if:
-         - task is lemmatizaer, then the morphological soltuion is only the lemma.
-         - task is pos, then the morphological soltuion is only the pos.
-         - task is full, the the morphological soltuion is both the lemma and the pos.
+         - the task is lemmatizer, then the morphological soltuion is only the lemma.
+         - the task is pos, then the morphological soltuion is only the pos.
+         - the task is full, the the morphological soltuion is both the lemma and the pos.
      
-    The language arguemet is used to help the morphological analysis to return more accurate solutions, for example if the text is MSA, or dialects (Palestinian dilect, pppp).
-   
+    The language argument helps the morphological analysis to return more accurate solutions based on the specific variety of Arabic used in the input text, including MSA and various dialects such as Pal, Lebanese, Iraqi, Libyan, Syrian, Sudanese, and Yemeni. 
+
     Args:
-          - text (str): The input text to morphologicaly analyzed.
-          - language (str): The language of the input text (e.g., `MSA`).
-          - task (str): The type of task being performed (e.g., `lemmatizer`, `pos`, or `full`).
+         - text (:obj:`str`): The input text to be morphologicaly analyzed.
+         - language (:obj:`str`): The language of the input text (e.g., `MSA`).
+         - task (:obj:`str`): The type of task being performed (e.g., `lemmatizer`, `pos`, or `full`).
          
     Returns:
-          - output_list (list): A list of morphological solution for each token in the input text.
-
-    **Example:**
-
-    .. highlight:: python
-    .. code-block:: python
-
-         from nlptools.morph import morph_tagger
-      
-         # Return the morpological solution for each token in this text
-         morph_tagger.tagger('ذهب الولد الى المدرسة')
+          - output_list (:obj:`list`): A list of morphological solution for each token in the input text.
     """
 
    output_list = []
    # tokenize sentence into words
-   words = simple_word_tokenize(text)
-   # create tqdm progress bar
-   progress_bar = tqdm(words, desc='Lemmatizing Sentence', leave=False)
-   # for each word 
-   for word in progress_bar:
-         result_word =[]
+   tokens = simple_word_tokenize(text)
+
+   # for each token 
+   for token in tokens:
+         result_token =[]
          # Trim spaces 
-         word = word.strip()
+         token = token.strip()
          # Remove smallDiac
-         word = arStrip(word , False , True , False , False , False , False) 
+         token = arStrip(token , False , True , False , False , False , False) 
          # Unify ٱ 
-         word = re.sub('[ٱ]','ﺍ',word)
-         # Initialize solution [word, lemma, pos]
-         solution = [word,word+"_0","",0]
+         token = re.sub('[ٱ]','ﺍ',token)
+         # Initialize solution [token, lemma, pos]
+         solution = [token,token+"_0","",0]
          
-         # if word is digit, update pos to be digit 
-         if word.isdigit():
+         # if token is digit, update pos to be digit 
+         if token.isdigit():
             solution[2] = "digit"
 
-         # if word is english, update pos to be ENGLISH
-         elif re.match("^[a-zA-Z]*$", word):
+         # if token is english, update pos to be ENGLISH
+         elif re.match("^[a-zA-Z]*$", token):
             solution[2] = "ENGLISH"
 
          else:
-            # search for a word (as is) in ALMA dictionary   
-            result_word = tag(word,language, task)
+            # search for a token (as is) in the dictionary   
+            result_token = tag(token,language, task)
             
-            if len(re.sub(r'^[ﻝ]','',re.sub(r'^[ﺍ]','',word))) > 5 and result_word == []:
-               # try with remove remove AL
-               result_word = tag(re.sub(r'^[ﻝ]','',re.sub(r'^[ﺍ]','',word)), language, task)
+            if len(re.sub(r'^[ﻝ]','',re.sub(r'^[ﺍ]','',token))) > 5 and result_token == []:
+               # try with remove AL
+               result_token = tag(re.sub(r'^[ﻝ]','',re.sub(r'^[ﺍ]','',token)), language, task)
 
-            if result_word == []:
+            if result_token == []:
               # try with replace ﻩ with ﺓ
-               result_word = tag(re.sub(r'[ﻩ]$','ﺓ',word), language, task)
+               result_token = tag(re.sub(r'[ﻩ]$','ﺓ',token), language, task)
 
-            if result_word == []:
+            if result_token == []:
                # try with unify Alef
-               word_with_unify_alef = arStrip(word , False , False , False , False , True , False) # Unify Alef
-               result_word = tag(word_with_unify_alef, language, task)
+               word_with_unify_alef = arStrip(token , False , False , False , False , True , False) # Unify Alef
+               result_token = tag(word_with_unify_alef, language, task)
             
-            if result_word == []:
+            if result_token == []:
                # try with remove diac
-               word_undiac = arStrip(word , True , False , True , True , False , False) # remove diacs, shaddah ,  digit
-               result_word = tag(word_undiac, language, task)
+               word_undiac = arStrip(token , True , False , True , True , False , False) # remove diacs, shaddah ,  digit
+               result_token = tag(word_undiac, language, task)
 
-            if result_word == []:
+            if result_token == []:
                # try with remove diac and unify alef
-               word_undiac = arStrip(word , True , True , True , False, True , False) # diacs , smallDiacs , shaddah ,  alif
-               result_word = tag(word_undiac, language, task)
+               word_undiac = arStrip(token , True , True , True , False, True , False) # diacs , smallDiacs , shaddah ,  alif
+               result_token = tag(word_undiac, language, task)
 
-         if result_word != []:
+         if result_token != []:
+               #[token, lemma, pos, frequency, task and language]
                # if solution found
-               tmp_solution = [word,word+"_0","",0]               
-               tmp_solution[1] = result_word[2] # lemma
-               tmp_solution[2] = result_word[1] # pos_ar
-               tmp_solution[3] = result_word[3] # lemma_freq
+               tmp_solution = [token,token+"_0","",0] 
+               tmp_solution[1] = result_token[0] # token              
+               tmp_solution[2] = result_token[1] # lemma
+               tmp_solution[3] = result_token[2] # pos_ar
+               tmp_solution[4] = result_token[4] # lemma_freq
+               tmp_solution[5] = result_token[5] # task
+               tmp_solution[6] = result_token[6] # language
                output_list.append(tmp_solution)
          else:
             # if no solution is found
             output_list.append(solution)
 
    return output_list               
         
-def tagger(text: str, task = 'full', language = 'MSA') -> list:
+def tagger(text: str, task = 'full', language = 'MSA'):
 
     """
     This method takes an Arabic text as input, tokenize it into tokens and calles the morphological tagger to return the morpological solution for each token in this text.
     There is no limit for the text size, but one should be resonable based on the available resources (computational power).
     
         Args:
-            - text (str): The input Arabic text to be morphologically analyzed and tagged.
-            - task (str): The type of morphological analysis and tagging to be performed. Default is `full`.
-            - language (str): The language of the input text. Default is 'MSA' (Modern Standard Arabic).
+            - text (:obj:`str`): The input Arabic text to be morphologically analyzed and tagged.
+            - task (:obj:`str`): The type of morphological analysis and tagging to be performed (the default is `full`).
+            - language (:obj:`str`): The language of the input text (the default is 'MSA' (Modern Standard Arabic)).
         
     Returns:
-        list: A list of lists, where each sublist contains information about a token in the input text, including the original tokem, its lemma, its part of speech (POS) tag, its lemma frequency, the task and the language.
+           - output_list list(:obj:`list`): A list of lists, where each sublist contains information about a token in the input text, including the original token, its lemma, its part of speech (POS) tag, its lemma frequency, the task and the language.
+
+    **Example:**
+
+    .. highlight:: python
+    .. code-block:: python
+
+         from nlptools.morph import morph_tagger
+      
+         # Return the morpological solution for each token in this text
+         morph_tagger.tagger('ذهب الولد الى المدرسة')
+
+         # the output
+            [['ذهب', 349890, 'فعل', 'MSA'],
+            ['الولد', 320244, 'اسم', 'MSA'],
+            ['الى', 20215999, 'كلمة وظيفية', 'MSA'],
+            ['المدرسة', 561184, 'اسم', 'MSA']]
     """
     
     # Check if the ALMA dictionary has been loaded
     if settings.flag == True:
         settings.flag = False
-    settings.div_dic = load_ALMA_dic()
+        settings.div_dic = load_ALMA_dic()
    
     
-    # Perform lemmatization on the input sentence
-    output_list = lemmatize_sentence(text,language, task)
+    # Perform morphological tagging for the input text
+    output_list = analyze_morphology(text,language, task)
     
-    # Return the list of lemmatized words
+    # Return a list of morphological solution for each token in the input text
     return output_list
```

### Comparing `nlptoolssna-0.4.2/nlptools/morph/tokenizers_words.py` & `nlptoolssna-0.4.3/nlptools/morph/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/nlptools/parse/parser.py` & `nlptoolssna-0.4.3/nlptools/parse/parser.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/nlptools/salma/implication.py` & `nlptoolssna-0.4.3/nlptools/salma/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/nlptools/salma/tokenizers_words.py` & `nlptoolssna-0.4.3/nlptools/salma/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.4.3/nlptoolssna.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.4.2/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.4.3/nlptoolssna.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,25 @@
 docs/Makefile
 docs/make.bat
 docs/build/html/_images/download.png
 docs/build/html/_static/download.png
 docs/build/html/_static/file.png
 docs/build/html/_static/minus.png
 docs/build/html/_static/plus.png
-docs/source/DataDownload.rst
 docs/source/api.rst
 docs/source/authors.rst
 docs/source/conf.py
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/readme.rst
 docs/source/_static/download.png
+docs/source/api/DataDownload.rst
 docs/source/api/morph.rst
-docs/source/api/morph/charsets.rst
-docs/source/api/morph/lemmatizeSentence.rst
+docs/source/api/DataDownload/downloader.rst
 docs/source/api/morph/morph_tagger.rst
-docs/source/api/morph/tokenizers_words.rst
 nlptools/__init__.py
 nlptools/cli.py
 nlptools/nlptools.py
 nlptools/DataDownload/__init__.py
 nlptools/DataDownload/downloader.py
 nlptools/arabiner/__init__.py
 nlptools/arabiner/data.py
```

### Comparing `nlptoolssna-0.4.2/setup.cfg` & `nlptoolssna-0.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.4.2/setup.py` & `nlptoolssna-0.4.3/setup.py`

 * *Files identical despite different names*

