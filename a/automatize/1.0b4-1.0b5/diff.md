# Comparing `tmp/automatize-1.0b4.tar.gz` & `tmp/automatize-1.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automatize-1.0b4.tar", last modified: Mon May  1 02:32:15 2023, max compression
+gzip compressed data, was "automatize-1.0b5.tar", last modified: Mon May  1 02:57:39 2023, max compression
```

## Comparing `automatize-1.0b4.tar` & `automatize-1.0b5.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.558693 automatize-1.0b4/
--rwx------   0 tarlisportela   (501) staff       (20)      212 2023-04-29 19:11:36.000000 automatize-1.0b4/Dockerfile
--rwx------   0 tarlisportela   (501) staff       (20)    35721 2022-04-12 17:20:02.000000 automatize-1.0b4/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)      169 2023-04-30 05:29:46.000000 automatize-1.0b4/MANIFEST.in
--rw-r--r--   0 tarlisportela   (501) staff       (20)    12793 2023-05-01 02:32:15.558497 automatize-1.0b4/PKG-INFO
--rwx------   0 tarlisportela   (501) staff       (20)    10832 2023-04-29 20:00:41.000000 automatize-1.0b4/README.md
--rwx------   0 tarlisportela   (501) staff       (20)      982 2023-05-01 02:25:33.000000 automatize-1.0b4/Steps to Build.txt
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.495019 automatize-1.0b4/automatize/
--rwx------   0 tarlisportela   (501) staff       (20)    10832 2023-04-29 20:00:41.000000 automatize-1.0b4/automatize/README.md
--rwx------   0 tarlisportela   (501) staff       (20)        0 2023-04-30 01:10:26.000000 automatize-1.0b4/automatize/__init__.py
--rwx------   0 tarlisportela   (501) staff       (20)     8206 2022-11-28 21:43:58.000000 automatize-1.0b4/automatize/analysis.py
--rwx------   0 tarlisportela   (501) staff       (20)     7365 2023-04-30 02:04:46.000000 automatize-1.0b4/automatize/app.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.497531 automatize-1.0b4/automatize/assets/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b4/automatize/assets/__init__.py
--rwx------   0 tarlisportela   (501) staff       (20)     3164 2023-04-30 03:33:48.000000 automatize-1.0b4/automatize/assets/app_base.py
--rwx------   0 tarlisportela   (501) staff       (20)     8715 2023-01-17 18:34:22.000000 automatize-1.0b4/automatize/assets/appstyle.css
--rw-r--r--   0 tarlisportela   (501) staff       (20)      437 2022-06-23 16:25:27.000000 automatize-1.0b4/automatize/assets/citation.bib
--rwx------   0 tarlisportela   (501) staff       (20)     1989 2023-05-01 02:31:30.000000 automatize-1.0b4/automatize/assets/config.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.519561 automatize-1.0b4/automatize/assets/examples/
--rw-r--r--   0 tarlisportela   (501) staff       (20)  4340421 2022-11-28 22:55:33.000000 automatize-1.0b4/automatize/assets/examples/Automatize_Sample_Code.html
--rwx------   0 tarlisportela   (501) staff       (20)  3914737 2022-11-28 22:54:28.000000 automatize-1.0b4/automatize/assets/examples/Automatize_Sample_Code.ipynb
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.519719 automatize-1.0b4/automatize/assets/examples/Example/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b4/automatize/assets/examples/Example/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.523912 automatize-1.0b4/automatize/assets/examples/Example/data/
--rwx------   0 tarlisportela   (501) staff       (20)     1301 2022-06-07 11:28:16.000000 automatize-1.0b4/automatize/assets/examples/Example/data/Descriptor.json
--rwx------   0 tarlisportela   (501) staff       (20)     1223 2022-06-07 11:28:36.000000 automatize-1.0b4/automatize/assets/examples/Example/data/Descriptor_hp.json
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b4/automatize/assets/examples/Example/data/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3000 2022-06-07 11:34:59.000000 automatize-1.0b4/automatize/assets/examples/Example/data/test.csv
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3029 2022-06-09 17:42:27.000000 automatize-1.0b4/automatize/assets/examples/Example/data/test.mat
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3754 2022-06-09 17:42:27.000000 automatize-1.0b4/automatize/assets/examples/Example/data/test.zip
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2955 2022-06-07 11:34:50.000000 automatize-1.0b4/automatize/assets/examples/Example/data/train.csv
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3020 2022-06-09 17:42:27.000000 automatize-1.0b4/automatize/assets/examples/Example/data/train.mat
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3736 2022-06-09 17:42:27.000000 automatize-1.0b4/automatize/assets/examples/Example/data/train.zip
--rw-rw-r--   0 tarlisportela   (501) staff       (20)  7716732 2021-02-10 16:01:46.000000 automatize-1.0b4/automatize/assets/examples/Foursquare_Example.csv
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b4/automatize/assets/examples/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.524466 automatize-1.0b4/automatize/assets/examples/css/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b4/automatize/assets/examples/css/__init__.py
--rwx------   0 tarlisportela   (501) staff       (20)     4680 2020-01-03 17:28:58.000000 automatize-1.0b4/automatize/assets/examples/css/colorful.css
--rwx------   0 tarlisportela   (501) staff       (20)    13108 2020-01-03 17:28:58.000000 automatize-1.0b4/automatize/assets/examples/css/notebook.css
--rwx------   0 tarlisportela   (501) staff       (20)    24364 2023-01-05 15:37:21.000000 automatize-1.0b4/automatize/assets/experimental_history.csv
--rwx------   0 tarlisportela   (501) staff       (20)     2956 2022-01-03 15:20:50.000000 automatize-1.0b4/automatize/assets/favicon.ico
--rw-r--r--   0 tarlisportela   (501) staff       (20)    40902 2022-06-21 12:21:11.000000 automatize-1.0b4/automatize/assets/mat.svg
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.529587 automatize-1.0b4/automatize/assets/method/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     1125 2023-04-30 14:14:47.000000 automatize-1.0b4/automatize/assets/method/BITULER.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)      883 2023-04-30 13:58:14.000000 automatize-1.0b4/automatize/assets/method/DeepeST.md
--rwx------   0 tarlisportela   (501) staff       (20)     1014 2023-04-30 13:31:13.000000 automatize-1.0b4/automatize/assets/method/Dodge.md
--rwx------   0 tarlisportela   (501) staff       (20)     2569 2023-04-30 13:39:25.000000 automatize-1.0b4/automatize/assets/method/HIPERMovelets.md
--rwx------   0 tarlisportela   (501) staff       (20)     1195 2023-04-30 14:15:26.000000 automatize-1.0b4/automatize/assets/method/MARC.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)   209722 2023-04-30 12:37:42.000000 automatize-1.0b4/automatize/assets/method/MASTERMovelets.jar
--rwx------   0 tarlisportela   (501) staff       (20)     1482 2023-04-30 13:39:16.000000 automatize-1.0b4/automatize/assets/method/MASTERMovelets.md
--rwx------   0 tarlisportela   (501) staff       (20)     1414 2023-04-30 13:39:07.000000 automatize-1.0b4/automatize/assets/method/Movelets.md
--rwx------   0 tarlisportela   (501) staff       (20)       36 2022-04-26 15:11:35.000000 automatize-1.0b4/automatize/assets/method/POIF.md
--rwx------   0 tarlisportela   (501) staff       (20)     1739 2023-04-30 14:13:48.000000 automatize-1.0b4/automatize/assets/method/POIS.md
--rwx------   0 tarlisportela   (501) staff       (20)     1460 2023-04-30 13:38:04.000000 automatize-1.0b4/automatize/assets/method/SUPERMovelets.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)      921 2023-04-30 13:59:58.000000 automatize-1.0b4/automatize/assets/method/TRF.md
--rwx------   0 tarlisportela   (501) staff       (20)     1171 2023-04-30 14:15:58.000000 automatize-1.0b4/automatize/assets/method/TULVAE.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)     1048 2023-04-30 14:00:02.000000 automatize-1.0b4/automatize/assets/method/TXGB.md
--rwx------   0 tarlisportela   (501) staff       (20)      982 2023-04-30 13:37:51.000000 automatize-1.0b4/automatize/assets/method/Xiao.md
--rwx------   0 tarlisportela   (501) staff       (20)      975 2023-04-30 13:37:38.000000 automatize-1.0b4/automatize/assets/method/Zheng.md
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b4/automatize/assets/method/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.531078 automatize-1.0b4/automatize/assets/pages/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b4/automatize/assets/pages/__init__.py
--rwx------   0 tarlisportela   (501) staff       (20)      270 2022-06-21 12:16:55.000000 automatize-1.0b4/automatize/assets/pages/datasets.md
--rwx------   0 tarlisportela   (501) staff       (20)      126 2022-03-01 17:59:17.000000 automatize-1.0b4/automatize/assets/pages/experiments.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)     7031 2022-06-21 12:27:07.000000 automatize-1.0b4/automatize/assets/pages/mat.md
--rwx------   0 tarlisportela   (501) staff       (20)     5870 2023-04-30 13:36:07.000000 automatize-1.0b4/automatize/assets/pages/methods.md
--rwx------   0 tarlisportela   (501) staff       (20)     3118 2022-02-26 16:09:56.000000 automatize-1.0b4/automatize/assets/pages/publications.md
--rwx------   0 tarlisportela   (501) staff       (20)       23 2022-02-26 15:58:33.000000 automatize-1.0b4/automatize/assets/pages/results.md
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.533553 automatize-1.0b4/automatize/assets/routes/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b4/automatize/assets/routes/__init__.py
--rwx------   0 tarlisportela   (501) staff       (20)    18663 2023-04-30 01:58:18.000000 automatize-1.0b4/automatize/assets/routes/page_analysis.py
--rwx------   0 tarlisportela   (501) staff       (20)    14488 2023-04-30 05:23:03.000000 automatize-1.0b4/automatize/assets/routes/page_datasets.py
--rwx------   0 tarlisportela   (501) staff       (20)    29000 2023-04-30 12:55:38.000000 automatize-1.0b4/automatize/assets/routes/page_experiments.py
--rwx------   0 tarlisportela   (501) staff       (20)    36787 2023-04-30 01:58:40.000000 automatize-1.0b4/automatize/assets/routes/page_results.py
--rwx------   0 tarlisportela   (501) staff       (20)    17012 2022-09-16 22:07:24.000000 automatize-1.0b4/automatize/assets/routes/subpage_models.py
--rwx------   0 tarlisportela   (501) staff       (20)     9075 2022-08-19 12:45:53.000000 automatize-1.0b4/automatize/assets/routes/subpage_trajectories.py
--rwx------   0 tarlisportela   (501) staff       (20)       37 2022-04-28 17:41:53.000000 automatize-1.0b4/automatize/automatize-web
--rw-r--r--   0 tarlisportela   (501) staff       (20)    26418 2022-11-25 23:46:01.000000 automatize-1.0b4/automatize/generator.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    15021 2023-02-14 17:55:30.000000 automatize-1.0b4/automatize/graphics.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.534554 automatize-1.0b4/automatize/inc/
--rwx------   0 tarlisportela   (501) staff       (20)    14694 2022-10-21 19:18:34.000000 automatize-1.0b4/automatize/inc/CDDiagram.py
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b4/automatize/inc/__init__.py
--rwx------   0 tarlisportela   (501) staff       (20)     4962 2023-04-30 04:32:59.000000 automatize-1.0b4/automatize/inc/datasets_def.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.535821 automatize-1.0b4/automatize/inc/io/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b4/automatize/inc/io/__init__.py
--rwx------   0 tarlisportela   (501) staff       (20)    13756 2022-07-31 10:13:08.000000 automatize-1.0b4/automatize/inc/io/converter.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    41550 2023-02-08 21:49:07.000000 automatize-1.0b4/automatize/inc/io/results_read.py
--rwx------   0 tarlisportela   (501) staff       (20)    52635 2022-04-12 17:26:09.000000 automatize-1.0b4/automatize/inc/io/ts_io.py
--rwx------   0 tarlisportela   (501) staff       (20)    10597 2023-04-30 13:11:28.000000 automatize-1.0b4/automatize/inc/script_def.py
--rwx------   0 tarlisportela   (501) staff       (20)    26507 2023-04-30 02:57:15.000000 automatize-1.0b4/automatize/main.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.536624 automatize-1.0b4/automatize/methods/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b4/automatize/methods/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.537914 automatize-1.0b4/automatize/methods/_lib/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2022-04-26 11:54:30.000000 automatize-1.0b4/automatize/methods/_lib/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    15014 2022-11-28 22:46:30.000000 automatize-1.0b4/automatize/methods/_lib/datahandler.py
--rwx------   0 tarlisportela   (501) staff       (20)     1793 2022-11-26 15:29:33.000000 automatize-1.0b4/automatize/methods/_lib/geohash.py
--rwx------   0 tarlisportela   (501) staff       (20)     1804 2022-11-27 00:47:22.000000 automatize-1.0b4/automatize/methods/_lib/logger.py
--rwx------   0 tarlisportela   (501) staff       (20)    10704 2022-11-28 21:10:26.000000 automatize-1.0b4/automatize/methods/_lib/metrics.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.488486 automatize-1.0b4/automatize/methods/_lib/pymove/
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.539653 automatize-1.0b4/automatize/methods/_lib/pymove/core/
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/core/__init__.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)     1220 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/core/db.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.540063 automatize-1.0b4/automatize/methods/_lib/pymove/core/dirutils/
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/core/dirutils/__init__.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)     1001 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/core/dirutils/geohash.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)     4909 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/core/dirutils/metrics.py
--rw-rw-r--   0 tarlisportela   (501) staff       (20)     1317 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/core/labels.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)     4597 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/core/mem.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)     1837 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/core/mem_usage.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)     3125 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/core/notity.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)     3144 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/core/osmutils.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)    13613 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/core/utils.py
--rw-rw-r--   0 tarlisportela   (501) staff       (20)      160 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/core/video.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.540550 automatize-1.0b4/automatize/methods/_lib/pymove/models/
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/models/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.541983 automatize-1.0b4/automatize/methods/_lib/pymove/models/classification/
--rw-rw-r--   0 tarlisportela   (501) staff       (20)    11103 2022-11-27 17:41:31.000000 automatize-1.0b4/automatize/methods/_lib/pymove/models/classification/DeepestST.py
--rw-rw-r--   0 tarlisportela   (501) staff       (20)     2067 2022-07-30 23:09:20.000000 automatize-1.0b4/automatize/methods/_lib/pymove/models/classification/RandomForest.py
--rw-rw-r--   0 tarlisportela   (501) staff       (20)     9846 2022-11-27 17:43:07.000000 automatize-1.0b4/automatize/methods/_lib/pymove/models/classification/Tuler.py
--rw-rw-r--   0 tarlisportela   (501) staff       (20)     6809 2022-11-27 17:44:04.000000 automatize-1.0b4/automatize/methods/_lib/pymove/models/classification/Tulvae.py
--rw-rw-r--   0 tarlisportela   (501) staff       (20)     3372 2022-12-06 16:32:09.000000 automatize-1.0b4/automatize/methods/_lib/pymove/models/classification/XGBoost.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/models/classification/__init__.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)     5718 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/models/lossutils.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)     6891 2022-11-26 19:35:39.000000 automatize-1.0b4/automatize/methods/_lib/pymove/models/metrics.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.543421 automatize-1.0b4/automatize/methods/_lib/pymove/processing/
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)    10032 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/processing/compression.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)     3366 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/processing/geoutils.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)     7841 2022-07-30 23:11:51.000000 automatize-1.0b4/automatize/methods/_lib/pymove/processing/gridutils.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)    19465 2022-07-30 23:12:19.000000 automatize-1.0b4/automatize/methods/_lib/pymove/processing/segment.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)     8737 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/processing/semantic.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)    54422 2022-07-30 23:11:20.000000 automatize-1.0b4/automatize/methods/_lib/pymove/processing/trajutils.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.544495 automatize-1.0b4/automatize/methods/_lib/pymove/visualization/
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/visualization/__init__.py
--rwxr-xr-x   0 tarlisportela   (501) staff       (20)    36328 2020-11-23 14:20:06.000000 automatize-1.0b4/automatize/methods/_lib/pymove/visualization/maputils.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      357 2022-07-29 10:09:06.000000 automatize-1.0b4/automatize/methods/_lib/utils.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.544961 automatize-1.0b4/automatize/methods/deepest/
--rw-rw-r--   0 tarlisportela   (501) staff       (20)    12530 2022-12-13 16:29:31.000000 automatize-1.0b4/automatize/methods/deepest/DeepestST.py
--rwx------   0 tarlisportela   (501) staff       (20)        0 2022-04-26 11:54:30.000000 automatize-1.0b4/automatize/methods/deepest/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.545184 automatize-1.0b4/automatize/methods/marc/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2022-04-26 11:54:30.000000 automatize-1.0b4/automatize/methods/marc/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    17730 2022-11-29 00:50:57.000000 automatize-1.0b4/automatize/methods/marc/marc_nn.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.488822 automatize-1.0b4/automatize/methods/marc/src_marc/
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.545935 automatize-1.0b4/automatize/methods/marc/src_marc/core/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-27 20:05:17.000000 automatize-1.0b4/automatize/methods/marc/src_marc/core/__init__.py
--rwx------   0 tarlisportela   (501) staff       (20)     1805 2022-04-12 17:21:10.000000 automatize-1.0b4/automatize/methods/marc/src_marc/core/logger.py
--rwx------   0 tarlisportela   (501) staff       (20)     1868 2020-08-27 20:05:17.000000 automatize-1.0b4/automatize/methods/marc/src_marc/core/logger.pyc
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.547109 automatize-1.0b4/automatize/methods/marc/src_marc/core/utils/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-27 20:05:17.000000 automatize-1.0b4/automatize/methods/marc/src_marc/core/utils/__init__.py
--rwx------   0 tarlisportela   (501) staff       (20)     1869 2022-04-12 17:20:57.000000 automatize-1.0b4/automatize/methods/marc/src_marc/core/utils/geohash.py
--rwx------   0 tarlisportela   (501) staff       (20)     2179 2020-08-27 20:05:17.000000 automatize-1.0b4/automatize/methods/marc/src_marc/core/utils/geohash.pyc
--rwx------   0 tarlisportela   (501) staff       (20)     5794 2022-04-12 17:21:01.000000 automatize-1.0b4/automatize/methods/marc/src_marc/core/utils/metrics.py
--rwx------   0 tarlisportela   (501) staff       (20)     4998 2020-08-27 20:05:17.000000 automatize-1.0b4/automatize/methods/marc/src_marc/core/utils/metrics.pyc
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.547755 automatize-1.0b4/automatize/methods/movelet/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2022-04-26 11:54:30.000000 automatize-1.0b4/automatize/methods/movelet/__init__.py
--rwx------   0 tarlisportela   (501) staff       (20)     7580 2022-08-07 19:09:08.000000 automatize-1.0b4/automatize/methods/movelet/classification.py
--rwx------   0 tarlisportela   (501) staff       (20)    16942 2022-11-28 21:12:53.000000 automatize-1.0b4/automatize/methods/movelet/moveletml.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.549000 automatize-1.0b4/automatize/methods/pois/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b4/automatize/methods/pois/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    13846 2022-12-15 19:53:21.000000 automatize-1.0b4/automatize/methods/pois/model_poifreq.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    17523 2022-07-30 16:09:19.000000 automatize-1.0b4/automatize/methods/pois/poifreq.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.549833 automatize-1.0b4/automatize/methods/rf/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2022-04-26 11:54:30.000000 automatize-1.0b4/automatize/methods/rf/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    11857 2022-11-28 22:58:43.000000 automatize-1.0b4/automatize/methods/rf/randomforrest.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.550655 automatize-1.0b4/automatize/methods/tec/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b4/automatize/methods/tec/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.551943 automatize-1.0b4/automatize/methods/tec/models/
--rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b4/automatize/methods/tec/models/__init__.py
--rwx------   0 tarlisportela   (501) staff       (20)    18808 2022-11-28 21:28:07.000000 automatize-1.0b4/automatize/methods/tec/models/marc.py
--rwx------   0 tarlisportela   (501) staff       (20)     5853 2022-04-12 15:10:22.000000 automatize-1.0b4/automatize/methods/tec/models/movelets.py
--rwx------   0 tarlisportela   (501) staff       (20)     6164 2022-04-12 15:09:31.000000 automatize-1.0b4/automatize/methods/tec/models/randomforrest.py
--rwx------   0 tarlisportela   (501) staff       (20)     7502 2022-04-12 15:09:34.000000 automatize-1.0b4/automatize/methods/tec/models/randomforresthp.py
--rwx------   0 tarlisportela   (501) staff       (20)    13090 2022-11-29 00:51:41.000000 automatize-1.0b4/automatize/methods/tec/tec.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.553000 automatize-1.0b4/automatize/methods/tuler/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     9724 2022-11-28 23:01:03.000000 automatize-1.0b4/automatize/methods/tuler/BITULER.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    11440 2022-11-28 23:00:52.000000 automatize-1.0b4/automatize/methods/tuler/TULVAE.py
--rwx------   0 tarlisportela   (501) staff       (20)        0 2022-04-26 11:54:30.000000 automatize-1.0b4/automatize/methods/tuler/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.553923 automatize-1.0b4/automatize/methods/xgboost/
--rw-r--r--   0 tarlisportela   (501) staff       (20)    10222 2022-12-06 16:32:06.000000 automatize-1.0b4/automatize/methods/xgboost/XGBoost.py
--rwx------   0 tarlisportela   (501) staff       (20)        0 2022-04-26 11:54:30.000000 automatize-1.0b4/automatize/methods/xgboost/__init__.py
--rwx------   0 tarlisportela   (501) staff       (20)    40048 2022-09-16 22:29:54.000000 automatize-1.0b4/automatize/movelets.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      211 2022-11-30 20:27:57.000000 automatize-1.0b4/automatize/optionals.txt
--rwx------   0 tarlisportela   (501) staff       (20)    34359 2022-11-29 02:05:09.000000 automatize-1.0b4/automatize/preprocessing.py
--rwx------   0 tarlisportela   (501) staff       (20)     2566 2023-05-01 02:31:44.000000 automatize-1.0b4/automatize/pyproject.toml
--rwx------   0 tarlisportela   (501) staff       (20)      160 2022-11-30 20:27:52.000000 automatize-1.0b4/automatize/requirements.txt
--rwx------   0 tarlisportela   (501) staff       (20)    46515 2023-02-08 20:46:01.000000 automatize-1.0b4/automatize/results.py
--rwx------   0 tarlisportela   (501) staff       (20)    19926 2022-07-30 15:25:32.000000 automatize-1.0b4/automatize/run.py
--rwx------   0 tarlisportela   (501) staff       (20)    30273 2023-04-30 13:05:49.000000 automatize-1.0b4/automatize/script.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.558263 automatize-1.0b4/automatize/scripts/
--rwx------   0 tarlisportela   (501) staff       (20)     5246 2023-04-30 14:16:27.000000 automatize-1.0b4/automatize/scripts/MARC.py
--rwx------   0 tarlisportela   (501) staff       (20)     1447 2023-04-30 00:30:36.000000 automatize-1.0b4/automatize/scripts/MAT-CheckRun.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2297 2023-04-30 14:16:33.000000 automatize-1.0b4/automatize/scripts/MAT-ExportMovelets.py
--rwx------   0 tarlisportela   (501) staff       (20)     2914 2023-04-30 14:16:37.000000 automatize-1.0b4/automatize/scripts/MAT-ExportResults.py
--rwx------   0 tarlisportela   (501) staff       (20)     2226 2023-04-30 14:16:40.000000 automatize-1.0b4/automatize/scripts/MAT-MC.py
--rwx------   0 tarlisportela   (501) staff       (20)     1571 2023-04-30 14:16:43.000000 automatize-1.0b4/automatize/scripts/MAT-MergeDatasets.py
--rwx------   0 tarlisportela   (501) staff       (20)     1700 2023-04-30 14:16:46.000000 automatize-1.0b4/automatize/scripts/MAT-MoveDatasets.py
--rwx------   0 tarlisportela   (501) staff       (20)     2054 2023-04-30 14:16:48.000000 automatize-1.0b4/automatize/scripts/MAT-PrintResults.py
--rwx------   0 tarlisportela   (501) staff       (20)     2190 2023-04-30 14:16:50.000000 automatize-1.0b4/automatize/scripts/MAT-ResultsCheck.py
--rwx------   0 tarlisportela   (501) staff       (20)     2693 2023-04-30 14:16:52.000000 automatize-1.0b4/automatize/scripts/MAT-ResultsTo.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2895 2023-04-30 14:16:55.000000 automatize-1.0b4/automatize/scripts/MAT-TC.py
--rwx------   0 tarlisportela   (501) staff       (20)     2545 2023-04-30 14:16:56.000000 automatize-1.0b4/automatize/scripts/MAT-TEC.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     1761 2023-04-30 04:19:35.000000 automatize-1.0b4/automatize/scripts/MAT.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2946 2023-04-30 14:17:00.000000 automatize-1.0b4/automatize/scripts/POIS-TC.py
--rwx------   0 tarlisportela   (501) staff       (20)     3521 2023-04-30 14:10:42.000000 automatize-1.0b4/automatize/scripts/POIS.py
--rwx------   0 tarlisportela   (501) staff       (20)        0 2022-07-25 14:59:03.000000 automatize-1.0b4/automatize/scripts/__init__.py
--rwx------   0 tarlisportela   (501) staff       (20)     2861 2023-05-01 02:26:40.000000 automatize-1.0b4/automatize/setup.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:32:15.495695 automatize-1.0b4/automatize.egg-info/
--rw-r--r--   0 tarlisportela   (501) staff       (20)    12793 2023-05-01 02:32:15.000000 automatize-1.0b4/automatize.egg-info/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)     6831 2023-05-01 02:32:15.000000 automatize-1.0b4/automatize.egg-info/SOURCES.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2023-05-01 02:32:15.000000 automatize-1.0b4/automatize.egg-info/dependency_links.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)      401 2023-05-01 02:32:15.000000 automatize-1.0b4/automatize.egg-info/requires.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)       11 2023-05-01 02:32:15.000000 automatize-1.0b4/automatize.egg-info/top_level.txt
--rwx------   0 tarlisportela   (501) staff       (20)     2566 2023-05-01 02:31:44.000000 automatize-1.0b4/pyproject.toml
--rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2023-05-01 02:32:15.558735 automatize-1.0b4/setup.cfg
--rwx------   0 tarlisportela   (501) staff       (20)     2861 2023-05-01 02:26:40.000000 automatize-1.0b4/setup.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.993234 automatize-1.0b5/
+-rwx------   0 tarlisportela   (501) staff       (20)      212 2023-04-29 19:11:36.000000 automatize-1.0b5/Dockerfile
+-rwx------   0 tarlisportela   (501) staff       (20)    35721 2022-04-12 17:20:02.000000 automatize-1.0b5/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      169 2023-04-30 05:29:46.000000 automatize-1.0b5/MANIFEST.in
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    12793 2023-05-01 02:57:39.993043 automatize-1.0b5/PKG-INFO
+-rwx------   0 tarlisportela   (501) staff       (20)    10832 2023-04-29 20:00:41.000000 automatize-1.0b5/README.md
+-rwx------   0 tarlisportela   (501) staff       (20)      982 2023-05-01 02:25:33.000000 automatize-1.0b5/Steps to Build.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.931645 automatize-1.0b5/automatize/
+-rwx------   0 tarlisportela   (501) staff       (20)    10832 2023-04-29 20:00:41.000000 automatize-1.0b5/automatize/README.md
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2023-04-30 01:10:26.000000 automatize-1.0b5/automatize/__init__.py
+-rwx------   0 tarlisportela   (501) staff       (20)     8206 2022-11-28 21:43:58.000000 automatize-1.0b5/automatize/analysis.py
+-rwx------   0 tarlisportela   (501) staff       (20)     7365 2023-04-30 02:04:46.000000 automatize-1.0b5/automatize/app.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.934394 automatize-1.0b5/automatize/assets/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b5/automatize/assets/__init__.py
+-rwx------   0 tarlisportela   (501) staff       (20)     3164 2023-04-30 03:33:48.000000 automatize-1.0b5/automatize/assets/app_base.py
+-rwx------   0 tarlisportela   (501) staff       (20)     8715 2023-01-17 18:34:22.000000 automatize-1.0b5/automatize/assets/appstyle.css
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      437 2022-06-23 16:25:27.000000 automatize-1.0b5/automatize/assets/citation.bib
+-rwx------   0 tarlisportela   (501) staff       (20)     2095 2023-05-01 02:55:17.000000 automatize-1.0b5/automatize/assets/config.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.954083 automatize-1.0b5/automatize/assets/examples/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)  4340421 2022-11-28 22:55:33.000000 automatize-1.0b5/automatize/assets/examples/Automatize_Sample_Code.html
+-rwx------   0 tarlisportela   (501) staff       (20)  3914737 2022-11-28 22:54:28.000000 automatize-1.0b5/automatize/assets/examples/Automatize_Sample_Code.ipynb
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.954239 automatize-1.0b5/automatize/assets/examples/Example/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b5/automatize/assets/examples/Example/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.959093 automatize-1.0b5/automatize/assets/examples/Example/data/
+-rwx------   0 tarlisportela   (501) staff       (20)     1301 2022-06-07 11:28:16.000000 automatize-1.0b5/automatize/assets/examples/Example/data/Descriptor.json
+-rwx------   0 tarlisportela   (501) staff       (20)     1223 2022-06-07 11:28:36.000000 automatize-1.0b5/automatize/assets/examples/Example/data/Descriptor_hp.json
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b5/automatize/assets/examples/Example/data/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3000 2022-06-07 11:34:59.000000 automatize-1.0b5/automatize/assets/examples/Example/data/test.csv
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3029 2022-06-09 17:42:27.000000 automatize-1.0b5/automatize/assets/examples/Example/data/test.mat
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3754 2022-06-09 17:42:27.000000 automatize-1.0b5/automatize/assets/examples/Example/data/test.zip
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2955 2022-06-07 11:34:50.000000 automatize-1.0b5/automatize/assets/examples/Example/data/train.csv
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3020 2022-06-09 17:42:27.000000 automatize-1.0b5/automatize/assets/examples/Example/data/train.mat
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3736 2022-06-09 17:42:27.000000 automatize-1.0b5/automatize/assets/examples/Example/data/train.zip
+-rw-rw-r--   0 tarlisportela   (501) staff       (20)  7716732 2021-02-10 16:01:46.000000 automatize-1.0b5/automatize/assets/examples/Foursquare_Example.csv
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b5/automatize/assets/examples/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.959802 automatize-1.0b5/automatize/assets/examples/css/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b5/automatize/assets/examples/css/__init__.py
+-rwx------   0 tarlisportela   (501) staff       (20)     4680 2020-01-03 17:28:58.000000 automatize-1.0b5/automatize/assets/examples/css/colorful.css
+-rwx------   0 tarlisportela   (501) staff       (20)    13108 2020-01-03 17:28:58.000000 automatize-1.0b5/automatize/assets/examples/css/notebook.css
+-rwx------   0 tarlisportela   (501) staff       (20)    24364 2023-01-05 15:37:21.000000 automatize-1.0b5/automatize/assets/experimental_history.csv
+-rwx------   0 tarlisportela   (501) staff       (20)     2956 2022-01-03 15:20:50.000000 automatize-1.0b5/automatize/assets/favicon.ico
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    40902 2022-06-21 12:21:11.000000 automatize-1.0b5/automatize/assets/mat.svg
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.965710 automatize-1.0b5/automatize/assets/method/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1125 2023-04-30 14:14:47.000000 automatize-1.0b5/automatize/assets/method/BITULER.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      883 2023-04-30 13:58:14.000000 automatize-1.0b5/automatize/assets/method/DeepeST.md
+-rwx------   0 tarlisportela   (501) staff       (20)     1014 2023-04-30 13:31:13.000000 automatize-1.0b5/automatize/assets/method/Dodge.md
+-rwx------   0 tarlisportela   (501) staff       (20)     2569 2023-04-30 13:39:25.000000 automatize-1.0b5/automatize/assets/method/HIPERMovelets.md
+-rwx------   0 tarlisportela   (501) staff       (20)     1195 2023-04-30 14:15:26.000000 automatize-1.0b5/automatize/assets/method/MARC.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)   209722 2023-04-30 12:37:42.000000 automatize-1.0b5/automatize/assets/method/MASTERMovelets.jar
+-rwx------   0 tarlisportela   (501) staff       (20)     1482 2023-04-30 13:39:16.000000 automatize-1.0b5/automatize/assets/method/MASTERMovelets.md
+-rwx------   0 tarlisportela   (501) staff       (20)     1414 2023-04-30 13:39:07.000000 automatize-1.0b5/automatize/assets/method/Movelets.md
+-rwx------   0 tarlisportela   (501) staff       (20)       36 2022-04-26 15:11:35.000000 automatize-1.0b5/automatize/assets/method/POIF.md
+-rwx------   0 tarlisportela   (501) staff       (20)     1739 2023-04-30 14:13:48.000000 automatize-1.0b5/automatize/assets/method/POIS.md
+-rwx------   0 tarlisportela   (501) staff       (20)     1460 2023-04-30 13:38:04.000000 automatize-1.0b5/automatize/assets/method/SUPERMovelets.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      921 2023-04-30 13:59:58.000000 automatize-1.0b5/automatize/assets/method/TRF.md
+-rwx------   0 tarlisportela   (501) staff       (20)     1171 2023-04-30 14:15:58.000000 automatize-1.0b5/automatize/assets/method/TULVAE.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1048 2023-04-30 14:00:02.000000 automatize-1.0b5/automatize/assets/method/TXGB.md
+-rwx------   0 tarlisportela   (501) staff       (20)      982 2023-04-30 13:37:51.000000 automatize-1.0b5/automatize/assets/method/Xiao.md
+-rwx------   0 tarlisportela   (501) staff       (20)      975 2023-04-30 13:37:38.000000 automatize-1.0b5/automatize/assets/method/Zheng.md
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b5/automatize/assets/method/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.967219 automatize-1.0b5/automatize/assets/pages/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b5/automatize/assets/pages/__init__.py
+-rwx------   0 tarlisportela   (501) staff       (20)      270 2022-06-21 12:16:55.000000 automatize-1.0b5/automatize/assets/pages/datasets.md
+-rwx------   0 tarlisportela   (501) staff       (20)      126 2022-03-01 17:59:17.000000 automatize-1.0b5/automatize/assets/pages/experiments.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     7031 2022-06-21 12:27:07.000000 automatize-1.0b5/automatize/assets/pages/mat.md
+-rwx------   0 tarlisportela   (501) staff       (20)     5870 2023-04-30 13:36:07.000000 automatize-1.0b5/automatize/assets/pages/methods.md
+-rwx------   0 tarlisportela   (501) staff       (20)     3118 2022-02-26 16:09:56.000000 automatize-1.0b5/automatize/assets/pages/publications.md
+-rwx------   0 tarlisportela   (501) staff       (20)       23 2022-02-26 15:58:33.000000 automatize-1.0b5/automatize/assets/pages/results.md
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.969625 automatize-1.0b5/automatize/assets/routes/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b5/automatize/assets/routes/__init__.py
+-rwx------   0 tarlisportela   (501) staff       (20)    18663 2023-04-30 01:58:18.000000 automatize-1.0b5/automatize/assets/routes/page_analysis.py
+-rwx------   0 tarlisportela   (501) staff       (20)    14488 2023-04-30 05:23:03.000000 automatize-1.0b5/automatize/assets/routes/page_datasets.py
+-rwx------   0 tarlisportela   (501) staff       (20)    29000 2023-04-30 12:55:38.000000 automatize-1.0b5/automatize/assets/routes/page_experiments.py
+-rwx------   0 tarlisportela   (501) staff       (20)    36787 2023-04-30 01:58:40.000000 automatize-1.0b5/automatize/assets/routes/page_results.py
+-rwx------   0 tarlisportela   (501) staff       (20)    17012 2022-09-16 22:07:24.000000 automatize-1.0b5/automatize/assets/routes/subpage_models.py
+-rwx------   0 tarlisportela   (501) staff       (20)     9075 2022-08-19 12:45:53.000000 automatize-1.0b5/automatize/assets/routes/subpage_trajectories.py
+-rwx------   0 tarlisportela   (501) staff       (20)       37 2022-04-28 17:41:53.000000 automatize-1.0b5/automatize/automatize-web
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    26418 2022-11-25 23:46:01.000000 automatize-1.0b5/automatize/generator.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    15021 2023-02-14 17:55:30.000000 automatize-1.0b5/automatize/graphics.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.970642 automatize-1.0b5/automatize/inc/
+-rwx------   0 tarlisportela   (501) staff       (20)    14694 2022-10-21 19:18:34.000000 automatize-1.0b5/automatize/inc/CDDiagram.py
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b5/automatize/inc/__init__.py
+-rwx------   0 tarlisportela   (501) staff       (20)     4962 2023-04-30 04:32:59.000000 automatize-1.0b5/automatize/inc/datasets_def.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.971908 automatize-1.0b5/automatize/inc/io/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b5/automatize/inc/io/__init__.py
+-rwx------   0 tarlisportela   (501) staff       (20)    13756 2022-07-31 10:13:08.000000 automatize-1.0b5/automatize/inc/io/converter.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    41550 2023-02-08 21:49:07.000000 automatize-1.0b5/automatize/inc/io/results_read.py
+-rwx------   0 tarlisportela   (501) staff       (20)    52635 2022-04-12 17:26:09.000000 automatize-1.0b5/automatize/inc/io/ts_io.py
+-rwx------   0 tarlisportela   (501) staff       (20)    10597 2023-04-30 13:11:28.000000 automatize-1.0b5/automatize/inc/script_def.py
+-rwx------   0 tarlisportela   (501) staff       (20)    26507 2023-04-30 02:57:15.000000 automatize-1.0b5/automatize/main.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.972733 automatize-1.0b5/automatize/methods/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b5/automatize/methods/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.974033 automatize-1.0b5/automatize/methods/_lib/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2022-04-26 11:54:30.000000 automatize-1.0b5/automatize/methods/_lib/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    15014 2022-11-28 22:46:30.000000 automatize-1.0b5/automatize/methods/_lib/datahandler.py
+-rwx------   0 tarlisportela   (501) staff       (20)     1793 2022-11-26 15:29:33.000000 automatize-1.0b5/automatize/methods/_lib/geohash.py
+-rwx------   0 tarlisportela   (501) staff       (20)     1804 2022-11-27 00:47:22.000000 automatize-1.0b5/automatize/methods/_lib/logger.py
+-rwx------   0 tarlisportela   (501) staff       (20)    10704 2022-11-28 21:10:26.000000 automatize-1.0b5/automatize/methods/_lib/metrics.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.924405 automatize-1.0b5/automatize/methods/_lib/pymove/
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.975785 automatize-1.0b5/automatize/methods/_lib/pymove/core/
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/core/__init__.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)     1220 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/core/db.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.976206 automatize-1.0b5/automatize/methods/_lib/pymove/core/dirutils/
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/core/dirutils/__init__.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)     1001 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/core/dirutils/geohash.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)     4909 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/core/dirutils/metrics.py
+-rw-rw-r--   0 tarlisportela   (501) staff       (20)     1317 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/core/labels.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)     4597 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/core/mem.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)     1837 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/core/mem_usage.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)     3125 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/core/notity.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)     3144 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/core/osmutils.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)    13613 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/core/utils.py
+-rw-rw-r--   0 tarlisportela   (501) staff       (20)      160 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/core/video.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.976772 automatize-1.0b5/automatize/methods/_lib/pymove/models/
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/models/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.978224 automatize-1.0b5/automatize/methods/_lib/pymove/models/classification/
+-rw-rw-r--   0 tarlisportela   (501) staff       (20)    11103 2022-11-27 17:41:31.000000 automatize-1.0b5/automatize/methods/_lib/pymove/models/classification/DeepestST.py
+-rw-rw-r--   0 tarlisportela   (501) staff       (20)     2067 2022-07-30 23:09:20.000000 automatize-1.0b5/automatize/methods/_lib/pymove/models/classification/RandomForest.py
+-rw-rw-r--   0 tarlisportela   (501) staff       (20)     9846 2022-11-27 17:43:07.000000 automatize-1.0b5/automatize/methods/_lib/pymove/models/classification/Tuler.py
+-rw-rw-r--   0 tarlisportela   (501) staff       (20)     6809 2022-11-27 17:44:04.000000 automatize-1.0b5/automatize/methods/_lib/pymove/models/classification/Tulvae.py
+-rw-rw-r--   0 tarlisportela   (501) staff       (20)     3372 2022-12-06 16:32:09.000000 automatize-1.0b5/automatize/methods/_lib/pymove/models/classification/XGBoost.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/models/classification/__init__.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)     5718 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/models/lossutils.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)     6891 2022-11-26 19:35:39.000000 automatize-1.0b5/automatize/methods/_lib/pymove/models/metrics.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.979761 automatize-1.0b5/automatize/methods/_lib/pymove/processing/
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)    10032 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/processing/compression.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)     3366 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/processing/geoutils.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)     7841 2022-07-30 23:11:51.000000 automatize-1.0b5/automatize/methods/_lib/pymove/processing/gridutils.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)    19465 2022-07-30 23:12:19.000000 automatize-1.0b5/automatize/methods/_lib/pymove/processing/segment.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)     8737 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/processing/semantic.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)    54422 2022-07-30 23:11:20.000000 automatize-1.0b5/automatize/methods/_lib/pymove/processing/trajutils.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.980898 automatize-1.0b5/automatize/methods/_lib/pymove/visualization/
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/visualization/__init__.py
+-rwxr-xr-x   0 tarlisportela   (501) staff       (20)    36328 2020-11-23 14:20:06.000000 automatize-1.0b5/automatize/methods/_lib/pymove/visualization/maputils.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      357 2022-07-29 10:09:06.000000 automatize-1.0b5/automatize/methods/_lib/utils.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.981415 automatize-1.0b5/automatize/methods/deepest/
+-rw-rw-r--   0 tarlisportela   (501) staff       (20)    12530 2022-12-13 16:29:31.000000 automatize-1.0b5/automatize/methods/deepest/DeepestST.py
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2022-04-26 11:54:30.000000 automatize-1.0b5/automatize/methods/deepest/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.981670 automatize-1.0b5/automatize/methods/marc/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2022-04-26 11:54:30.000000 automatize-1.0b5/automatize/methods/marc/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    17730 2022-11-29 00:50:57.000000 automatize-1.0b5/automatize/methods/marc/marc_nn.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.924739 automatize-1.0b5/automatize/methods/marc/src_marc/
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.982459 automatize-1.0b5/automatize/methods/marc/src_marc/core/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-27 20:05:17.000000 automatize-1.0b5/automatize/methods/marc/src_marc/core/__init__.py
+-rwx------   0 tarlisportela   (501) staff       (20)     1805 2022-04-12 17:21:10.000000 automatize-1.0b5/automatize/methods/marc/src_marc/core/logger.py
+-rwx------   0 tarlisportela   (501) staff       (20)     1868 2020-08-27 20:05:17.000000 automatize-1.0b5/automatize/methods/marc/src_marc/core/logger.pyc
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.983730 automatize-1.0b5/automatize/methods/marc/src_marc/core/utils/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-27 20:05:17.000000 automatize-1.0b5/automatize/methods/marc/src_marc/core/utils/__init__.py
+-rwx------   0 tarlisportela   (501) staff       (20)     1869 2022-04-12 17:20:57.000000 automatize-1.0b5/automatize/methods/marc/src_marc/core/utils/geohash.py
+-rwx------   0 tarlisportela   (501) staff       (20)     2179 2020-08-27 20:05:17.000000 automatize-1.0b5/automatize/methods/marc/src_marc/core/utils/geohash.pyc
+-rwx------   0 tarlisportela   (501) staff       (20)     5794 2022-04-12 17:21:01.000000 automatize-1.0b5/automatize/methods/marc/src_marc/core/utils/metrics.py
+-rwx------   0 tarlisportela   (501) staff       (20)     4998 2020-08-27 20:05:17.000000 automatize-1.0b5/automatize/methods/marc/src_marc/core/utils/metrics.pyc
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.984403 automatize-1.0b5/automatize/methods/movelet/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2022-04-26 11:54:30.000000 automatize-1.0b5/automatize/methods/movelet/__init__.py
+-rwx------   0 tarlisportela   (501) staff       (20)     7580 2022-08-07 19:09:08.000000 automatize-1.0b5/automatize/methods/movelet/classification.py
+-rwx------   0 tarlisportela   (501) staff       (20)    16942 2022-11-28 21:12:53.000000 automatize-1.0b5/automatize/methods/movelet/moveletml.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.985434 automatize-1.0b5/automatize/methods/pois/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b5/automatize/methods/pois/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    13846 2022-12-15 19:53:21.000000 automatize-1.0b5/automatize/methods/pois/model_poifreq.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    17523 2022-07-30 16:09:19.000000 automatize-1.0b5/automatize/methods/pois/poifreq.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.985924 automatize-1.0b5/automatize/methods/rf/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2022-04-26 11:54:30.000000 automatize-1.0b5/automatize/methods/rf/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    11857 2022-11-28 22:58:43.000000 automatize-1.0b5/automatize/methods/rf/randomforrest.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.986335 automatize-1.0b5/automatize/methods/tec/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b5/automatize/methods/tec/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.987715 automatize-1.0b5/automatize/methods/tec/models/
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2020-08-10 12:36:53.000000 automatize-1.0b5/automatize/methods/tec/models/__init__.py
+-rwx------   0 tarlisportela   (501) staff       (20)    18808 2022-11-28 21:28:07.000000 automatize-1.0b5/automatize/methods/tec/models/marc.py
+-rwx------   0 tarlisportela   (501) staff       (20)     5853 2022-04-12 15:10:22.000000 automatize-1.0b5/automatize/methods/tec/models/movelets.py
+-rwx------   0 tarlisportela   (501) staff       (20)     6164 2022-04-12 15:09:31.000000 automatize-1.0b5/automatize/methods/tec/models/randomforrest.py
+-rwx------   0 tarlisportela   (501) staff       (20)     7502 2022-04-12 15:09:34.000000 automatize-1.0b5/automatize/methods/tec/models/randomforresthp.py
+-rwx------   0 tarlisportela   (501) staff       (20)    13090 2022-11-29 00:51:41.000000 automatize-1.0b5/automatize/methods/tec/tec.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.988744 automatize-1.0b5/automatize/methods/tuler/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     9724 2022-11-28 23:01:03.000000 automatize-1.0b5/automatize/methods/tuler/BITULER.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    11440 2022-11-28 23:00:52.000000 automatize-1.0b5/automatize/methods/tuler/TULVAE.py
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2022-04-26 11:54:30.000000 automatize-1.0b5/automatize/methods/tuler/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.989128 automatize-1.0b5/automatize/methods/xgboost/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    10222 2022-12-06 16:32:06.000000 automatize-1.0b5/automatize/methods/xgboost/XGBoost.py
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2022-04-26 11:54:30.000000 automatize-1.0b5/automatize/methods/xgboost/__init__.py
+-rwx------   0 tarlisportela   (501) staff       (20)    40048 2022-09-16 22:29:54.000000 automatize-1.0b5/automatize/movelets.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      211 2022-11-30 20:27:57.000000 automatize-1.0b5/automatize/optionals.txt
+-rwx------   0 tarlisportela   (501) staff       (20)    34359 2022-11-29 02:05:09.000000 automatize-1.0b5/automatize/preprocessing.py
+-rwx------   0 tarlisportela   (501) staff       (20)     2566 2023-05-01 02:57:05.000000 automatize-1.0b5/automatize/pyproject.toml
+-rwx------   0 tarlisportela   (501) staff       (20)      160 2022-11-30 20:27:52.000000 automatize-1.0b5/automatize/requirements.txt
+-rwx------   0 tarlisportela   (501) staff       (20)    46515 2023-02-08 20:46:01.000000 automatize-1.0b5/automatize/results.py
+-rwx------   0 tarlisportela   (501) staff       (20)    19926 2022-07-30 15:25:32.000000 automatize-1.0b5/automatize/run.py
+-rwx------   0 tarlisportela   (501) staff       (20)    30273 2023-04-30 13:05:49.000000 automatize-1.0b5/automatize/script.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.992831 automatize-1.0b5/automatize/scripts/
+-rwx------   0 tarlisportela   (501) staff       (20)     5246 2023-04-30 14:16:27.000000 automatize-1.0b5/automatize/scripts/MARC.py
+-rwx------   0 tarlisportela   (501) staff       (20)     1447 2023-04-30 00:30:36.000000 automatize-1.0b5/automatize/scripts/MAT-CheckRun.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2297 2023-04-30 14:16:33.000000 automatize-1.0b5/automatize/scripts/MAT-ExportMovelets.py
+-rwx------   0 tarlisportela   (501) staff       (20)     2914 2023-04-30 14:16:37.000000 automatize-1.0b5/automatize/scripts/MAT-ExportResults.py
+-rwx------   0 tarlisportela   (501) staff       (20)     2226 2023-04-30 14:16:40.000000 automatize-1.0b5/automatize/scripts/MAT-MC.py
+-rwx------   0 tarlisportela   (501) staff       (20)     1571 2023-04-30 14:16:43.000000 automatize-1.0b5/automatize/scripts/MAT-MergeDatasets.py
+-rwx------   0 tarlisportela   (501) staff       (20)     1700 2023-04-30 14:16:46.000000 automatize-1.0b5/automatize/scripts/MAT-MoveDatasets.py
+-rwx------   0 tarlisportela   (501) staff       (20)     2054 2023-04-30 14:16:48.000000 automatize-1.0b5/automatize/scripts/MAT-PrintResults.py
+-rwx------   0 tarlisportela   (501) staff       (20)     2190 2023-04-30 14:16:50.000000 automatize-1.0b5/automatize/scripts/MAT-ResultsCheck.py
+-rwx------   0 tarlisportela   (501) staff       (20)     2693 2023-04-30 14:16:52.000000 automatize-1.0b5/automatize/scripts/MAT-ResultsTo.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2895 2023-04-30 14:16:55.000000 automatize-1.0b5/automatize/scripts/MAT-TC.py
+-rwx------   0 tarlisportela   (501) staff       (20)     2545 2023-04-30 14:16:56.000000 automatize-1.0b5/automatize/scripts/MAT-TEC.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1761 2023-04-30 04:19:35.000000 automatize-1.0b5/automatize/scripts/MAT.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2946 2023-04-30 14:17:00.000000 automatize-1.0b5/automatize/scripts/POIS-TC.py
+-rwx------   0 tarlisportela   (501) staff       (20)     3521 2023-04-30 14:10:42.000000 automatize-1.0b5/automatize/scripts/POIS.py
+-rwx------   0 tarlisportela   (501) staff       (20)        0 2022-07-25 14:59:03.000000 automatize-1.0b5/automatize/scripts/__init__.py
+-rwx------   0 tarlisportela   (501) staff       (20)     2861 2023-05-01 02:26:40.000000 automatize-1.0b5/automatize/setup.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2023-05-01 02:57:39.932401 automatize-1.0b5/automatize.egg-info/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    12793 2023-05-01 02:57:39.000000 automatize-1.0b5/automatize.egg-info/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     6831 2023-05-01 02:57:39.000000 automatize-1.0b5/automatize.egg-info/SOURCES.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2023-05-01 02:57:39.000000 automatize-1.0b5/automatize.egg-info/dependency_links.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      401 2023-05-01 02:57:39.000000 automatize-1.0b5/automatize.egg-info/requires.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       11 2023-05-01 02:57:39.000000 automatize-1.0b5/automatize.egg-info/top_level.txt
+-rwx------   0 tarlisportela   (501) staff       (20)     2566 2023-05-01 02:57:05.000000 automatize-1.0b5/pyproject.toml
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2023-05-01 02:57:39.993273 automatize-1.0b5/setup.cfg
+-rwx------   0 tarlisportela   (501) staff       (20)     2861 2023-05-01 02:26:40.000000 automatize-1.0b5/setup.py
```

### Comparing `automatize-1.0b4/LICENSE` & `automatize-1.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/PKG-INFO` & `automatize-1.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatize
-Version: 1.0b4
+Version: 1.0b5
 Summary: Automatize: A Multiple Aspect Trajectory Data Mining Tool Library
 Home-page: https://github.com/ttportela/automatize
 Author: Tarlis Tortelli Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
 Project-URL: Homepage, https://github.com/ttportela/automatize
```

### Comparing `automatize-1.0b4/README.md` & `automatize-1.0b5/README.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/Steps to Build.txt` & `automatize-1.0b5/Steps to Build.txt`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/README.md` & `automatize-1.0b5/automatize/README.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/analysis.py` & `automatize-1.0b5/automatize/analysis.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/app.py` & `automatize-1.0b5/automatize/app.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/app_base.py` & `automatize-1.0b5/automatize/assets/app_base.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/appstyle.css` & `automatize-1.0b5/automatize/assets/appstyle.css`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/config.py` & `automatize-1.0b5/automatize/assets/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,26 +5,30 @@
 The present application offers a tool, to support the user in the classification task of multiple aspect trajectories, specifically for extracting and visualizing the movelets, the parts of the trajectory that better discriminate a class. It integrates into a unique platform the fragmented approaches available for multiple aspects trajectories and in general for multidimensional sequence classification into a unique web-based and python library system. Offers both movelets visualization and a complete configuration of classification experimental settings.
 
 Created on Dec, 2021
 Copyright (C) 2022, License GPL Version 3 or superior (see LICENSE file)
 
 @author: Tarlis Portela
 '''
+import os
+from pathlib import Path
 import configparser
 config = configparser.ConfigParser()
 config.read('automatize/pyproject.toml')
 
-#VERSION = config['project']['version'].replace("'", "")
+VERSION = '1.0' #config['project']['version'].replace("'", "")
 PACKAGE_NAME = 'automatize' #config['project']['name'].replace("'", "")
 
 DATA_PATH = '../datasets'    
 EXP_PATH  = '../../results'
 README    = PACKAGE_NAME+'/README.md'
 
-PAGES_ROUTE  = PACKAGE_NAME+'/'
+ROOT = str(Path(__file__).parents[2])
+
+PAGES_ROUTE  = os.path.join(ROOT, PACKAGE_NAME)+'/'
 ASSETS_ROUTE = PAGES_ROUTE + 'assets/'
 
 RESULTS_FILE    = ASSETS_ROUTE+'experimental_history.csv'
 
 # page_title = 'Tarlis\'s Multiple Aspect Trajectory Analysis'
 page_title = PACKAGE_NAME.capitalize()
 
@@ -38,13 +42,12 @@
 def alert(msg, mtype="info"):
     import dash_bootstrap_components as dbc
     return dbc.Alert(msg, color=mtype, style = {'margin':10})
 
 def render_markdown_file(file, div=False):
     from dash import html
     from dash import dcc
-    import os
-    f = open(file, "r")
+    f = open(os.path.join(ROOT, file), "r")
     if div:
         return html.Div(dcc.Markdown(f.read()), style={'margin': '20px'}, className='markdown')
     else:
         return dcc.Markdown(f.read())
```

### Comparing `automatize-1.0b4/automatize/assets/examples/Automatize_Sample_Code.html` & `automatize-1.0b5/automatize/assets/examples/Automatize_Sample_Code.html`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/examples/Automatize_Sample_Code.ipynb` & `automatize-1.0b5/automatize/assets/examples/Automatize_Sample_Code.ipynb`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/examples/Example/data/Descriptor.json` & `automatize-1.0b5/automatize/assets/examples/Example/data/Descriptor.json`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/examples/Example/data/Descriptor_hp.json` & `automatize-1.0b5/automatize/assets/examples/Example/data/Descriptor_hp.json`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/examples/Example/data/test.csv` & `automatize-1.0b5/automatize/assets/examples/Example/data/test.csv`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/examples/Example/data/test.mat` & `automatize-1.0b5/automatize/assets/examples/Example/data/test.mat`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/examples/Example/data/test.zip` & `automatize-1.0b5/automatize/assets/examples/Example/data/test.zip`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/examples/Example/data/train.csv` & `automatize-1.0b5/automatize/assets/examples/Example/data/train.csv`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/examples/Example/data/train.mat` & `automatize-1.0b5/automatize/assets/examples/Example/data/train.mat`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/examples/Example/data/train.zip` & `automatize-1.0b5/automatize/assets/examples/Example/data/train.zip`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/examples/Foursquare_Example.csv` & `automatize-1.0b5/automatize/assets/examples/Foursquare_Example.csv`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/examples/css/colorful.css` & `automatize-1.0b5/automatize/assets/examples/css/colorful.css`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/examples/css/notebook.css` & `automatize-1.0b5/automatize/assets/examples/css/notebook.css`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/experimental_history.csv` & `automatize-1.0b5/automatize/assets/experimental_history.csv`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/favicon.ico` & `automatize-1.0b5/automatize/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/mat.svg` & `automatize-1.0b5/automatize/assets/mat.svg`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/method/BITULER.md` & `automatize-1.0b5/automatize/assets/method/BITULER.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/method/DeepeST.md` & `automatize-1.0b5/automatize/assets/method/DeepeST.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/method/Dodge.md` & `automatize-1.0b5/automatize/assets/method/Dodge.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/method/HIPERMovelets.md` & `automatize-1.0b5/automatize/assets/method/HIPERMovelets.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/method/MARC.md` & `automatize-1.0b5/automatize/assets/method/MARC.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/method/MASTERMovelets.jar` & `automatize-1.0b5/automatize/assets/method/MASTERMovelets.jar`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/method/MASTERMovelets.md` & `automatize-1.0b5/automatize/assets/method/MASTERMovelets.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/method/Movelets.md` & `automatize-1.0b5/automatize/assets/method/Movelets.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/method/POIS.md` & `automatize-1.0b5/automatize/assets/method/POIS.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/method/SUPERMovelets.md` & `automatize-1.0b5/automatize/assets/method/SUPERMovelets.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/method/TRF.md` & `automatize-1.0b5/automatize/assets/method/TRF.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/method/TULVAE.md` & `automatize-1.0b5/automatize/assets/method/TULVAE.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/method/TXGB.md` & `automatize-1.0b5/automatize/assets/method/TXGB.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/method/Xiao.md` & `automatize-1.0b5/automatize/assets/method/Xiao.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/method/Zheng.md` & `automatize-1.0b5/automatize/assets/method/Zheng.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/pages/mat.md` & `automatize-1.0b5/automatize/assets/pages/mat.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/pages/methods.md` & `automatize-1.0b5/automatize/assets/pages/methods.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/pages/publications.md` & `automatize-1.0b5/automatize/assets/pages/publications.md`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/routes/page_analysis.py` & `automatize-1.0b5/automatize/assets/routes/page_analysis.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/routes/page_datasets.py` & `automatize-1.0b5/automatize/assets/routes/page_datasets.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/routes/page_experiments.py` & `automatize-1.0b5/automatize/assets/routes/page_experiments.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/routes/page_results.py` & `automatize-1.0b5/automatize/assets/routes/page_results.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/routes/subpage_models.py` & `automatize-1.0b5/automatize/assets/routes/subpage_models.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/assets/routes/subpage_trajectories.py` & `automatize-1.0b5/automatize/assets/routes/subpage_trajectories.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/generator.py` & `automatize-1.0b5/automatize/generator.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/graphics.py` & `automatize-1.0b5/automatize/graphics.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/inc/CDDiagram.py` & `automatize-1.0b5/automatize/inc/CDDiagram.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/inc/datasets_def.py` & `automatize-1.0b5/automatize/inc/datasets_def.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/inc/io/converter.py` & `automatize-1.0b5/automatize/inc/io/converter.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/inc/io/results_read.py` & `automatize-1.0b5/automatize/inc/io/results_read.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/inc/io/ts_io.py` & `automatize-1.0b5/automatize/inc/io/ts_io.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/inc/script_def.py` & `automatize-1.0b5/automatize/inc/script_def.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/main.py` & `automatize-1.0b5/automatize/main.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/datahandler.py` & `automatize-1.0b5/automatize/methods/_lib/datahandler.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/geohash.py` & `automatize-1.0b5/automatize/methods/_lib/geohash.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/logger.py` & `automatize-1.0b5/automatize/methods/_lib/logger.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/metrics.py` & `automatize-1.0b5/automatize/methods/_lib/metrics.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/core/db.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/core/db.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/core/dirutils/geohash.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/core/dirutils/geohash.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/core/dirutils/metrics.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/core/dirutils/metrics.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/core/labels.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/core/labels.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/core/mem.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/core/mem.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/core/mem_usage.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/core/mem_usage.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/core/notity.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/core/notity.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/core/osmutils.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/core/osmutils.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/core/utils.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/core/utils.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/models/classification/DeepestST.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/models/classification/DeepestST.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/models/classification/RandomForest.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/models/classification/RandomForest.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/models/classification/Tuler.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/models/classification/Tuler.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/models/classification/Tulvae.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/models/classification/Tulvae.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/models/classification/XGBoost.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/models/classification/XGBoost.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/models/lossutils.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/models/lossutils.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/models/metrics.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/models/metrics.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/processing/compression.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/processing/compression.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/processing/geoutils.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/processing/geoutils.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/processing/gridutils.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/processing/gridutils.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/processing/segment.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/processing/segment.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/processing/semantic.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/processing/semantic.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/processing/trajutils.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/processing/trajutils.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/_lib/pymove/visualization/maputils.py` & `automatize-1.0b5/automatize/methods/_lib/pymove/visualization/maputils.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/deepest/DeepestST.py` & `automatize-1.0b5/automatize/methods/deepest/DeepestST.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/marc/marc_nn.py` & `automatize-1.0b5/automatize/methods/marc/marc_nn.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/marc/src_marc/core/logger.py` & `automatize-1.0b5/automatize/methods/marc/src_marc/core/logger.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/marc/src_marc/core/logger.pyc` & `automatize-1.0b5/automatize/methods/marc/src_marc/core/logger.pyc`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/marc/src_marc/core/utils/geohash.py` & `automatize-1.0b5/automatize/methods/marc/src_marc/core/utils/geohash.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/marc/src_marc/core/utils/geohash.pyc` & `automatize-1.0b5/automatize/methods/marc/src_marc/core/utils/geohash.pyc`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/marc/src_marc/core/utils/metrics.py` & `automatize-1.0b5/automatize/methods/marc/src_marc/core/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/marc/src_marc/core/utils/metrics.pyc` & `automatize-1.0b5/automatize/methods/marc/src_marc/core/utils/metrics.pyc`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/movelet/classification.py` & `automatize-1.0b5/automatize/methods/movelet/classification.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/movelet/moveletml.py` & `automatize-1.0b5/automatize/methods/movelet/moveletml.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/pois/model_poifreq.py` & `automatize-1.0b5/automatize/methods/pois/model_poifreq.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/pois/poifreq.py` & `automatize-1.0b5/automatize/methods/pois/poifreq.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/rf/randomforrest.py` & `automatize-1.0b5/automatize/methods/rf/randomforrest.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/tec/models/marc.py` & `automatize-1.0b5/automatize/methods/tec/models/marc.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/tec/models/movelets.py` & `automatize-1.0b5/automatize/methods/tec/models/movelets.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/tec/models/randomforrest.py` & `automatize-1.0b5/automatize/methods/tec/models/randomforrest.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/tec/models/randomforresthp.py` & `automatize-1.0b5/automatize/methods/tec/models/randomforresthp.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/tec/tec.py` & `automatize-1.0b5/automatize/methods/tec/tec.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/tuler/BITULER.py` & `automatize-1.0b5/automatize/methods/tuler/BITULER.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/tuler/TULVAE.py` & `automatize-1.0b5/automatize/methods/tuler/TULVAE.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/methods/xgboost/XGBoost.py` & `automatize-1.0b5/automatize/methods/xgboost/XGBoost.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/movelets.py` & `automatize-1.0b5/automatize/movelets.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/preprocessing.py` & `automatize-1.0b5/automatize/preprocessing.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/pyproject.toml` & `automatize-1.0b5/automatize/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'automatize'
-version = '1.0b4'
+version = '1.0b5'
 description = "Automatize: A Multiple Aspect Trajectory Data Mining Tool Library"
 authors = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
 maintainers = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
```

### Comparing `automatize-1.0b4/automatize/results.py` & `automatize-1.0b5/automatize/results.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/run.py` & `automatize-1.0b5/automatize/run.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/script.py` & `automatize-1.0b5/automatize/script.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/scripts/MARC.py` & `automatize-1.0b5/automatize/scripts/MARC.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/scripts/MAT-CheckRun.py` & `automatize-1.0b5/automatize/scripts/MAT-CheckRun.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/scripts/MAT-ExportMovelets.py` & `automatize-1.0b5/automatize/scripts/MAT-ExportMovelets.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/scripts/MAT-ExportResults.py` & `automatize-1.0b5/automatize/scripts/MAT-ExportResults.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/scripts/MAT-MC.py` & `automatize-1.0b5/automatize/scripts/MAT-MC.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/scripts/MAT-MergeDatasets.py` & `automatize-1.0b5/automatize/scripts/MAT-MergeDatasets.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/scripts/MAT-MoveDatasets.py` & `automatize-1.0b5/automatize/scripts/MAT-MoveDatasets.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/scripts/MAT-PrintResults.py` & `automatize-1.0b5/automatize/scripts/MAT-PrintResults.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/scripts/MAT-ResultsCheck.py` & `automatize-1.0b5/automatize/scripts/MAT-ResultsCheck.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/scripts/MAT-ResultsTo.py` & `automatize-1.0b5/automatize/scripts/MAT-ResultsTo.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/scripts/MAT-TC.py` & `automatize-1.0b5/automatize/scripts/MAT-TC.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/scripts/MAT-TEC.py` & `automatize-1.0b5/automatize/scripts/MAT-TEC.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/scripts/MAT.py` & `automatize-1.0b5/automatize/scripts/MAT.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/scripts/POIS-TC.py` & `automatize-1.0b5/automatize/scripts/POIS-TC.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/scripts/POIS.py` & `automatize-1.0b5/automatize/scripts/POIS.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize/setup.py` & `automatize-1.0b5/automatize/setup.py`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/automatize.egg-info/PKG-INFO` & `automatize-1.0b5/automatize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automatize
-Version: 1.0b4
+Version: 1.0b5
 Summary: Automatize: A Multiple Aspect Trajectory Data Mining Tool Library
 Home-page: https://github.com/ttportela/automatize
 Author: Tarlis Tortelli Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
 Project-URL: Homepage, https://github.com/ttportela/automatize
```

### Comparing `automatize-1.0b4/automatize.egg-info/SOURCES.txt` & `automatize-1.0b5/automatize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automatize-1.0b4/pyproject.toml` & `automatize-1.0b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'automatize'
-version = '1.0b4'
+version = '1.0b5'
 description = "Automatize: A Multiple Aspect Trajectory Data Mining Tool Library"
 authors = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
 maintainers = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
```

### Comparing `automatize-1.0b4/setup.py` & `automatize-1.0b5/setup.py`

 * *Files identical despite different names*

