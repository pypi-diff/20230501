# Comparing `tmp/not1mm-23.4.6.tar.gz` & `tmp/not1mm-23.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-23.4.6.tar", last modified: Thu Apr  6 17:36:34 2023, max compression
+gzip compressed data, was "not1mm-23.5.1.tar", last modified: Mon May  1 16:46:02 2023, max compression
```

## Comparing `not1mm-23.4.6.tar` & `not1mm-23.5.1.tar`

### file list

```diff
@@ -1,80 +1,135 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-04-06 17:36:34.554216 not1mm-23.4.6/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.4.6/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12200 2023-04-06 17:36:34.553217 not1mm-23.4.6/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11451 2023-04-06 17:30:46.000000 not1mm-23.4.6/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-04-06 17:36:34.534217 not1mm-23.4.6/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.4.6/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61666 2023-04-06 16:51:30.000000 not1mm-23.4.6/not1mm/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-04-06 17:36:34.546217 not1mm-23.4.6/not1mm/data/
--rw-rw-rw-   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.4.6/not1mm/data/Combinear.qss
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.4.6/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.4.6/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.4.6/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.4.6/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.4.6/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      487 2023-03-21 14:20:18.000000 not1mm-23.4.6/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.4.6/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.4.6/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.4.6/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.4.6/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.4.6/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.4.6/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.4.6/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.4.6/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37714 2023-04-05 21:11:39.000000 not1mm-23.4.6/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16209 2023-04-06 14:33:00.000000 not1mm-23.4.6/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.4.6/not1mm/data/opon.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.4.6/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.4.6/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35558 2023-03-24 21:02:25.000000 not1mm-23.4.6/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4554 2023-02-26 02:19:03.000000 not1mm-23.4.6/not1mm/data/use_qrz_dialog.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-04-06 17:36:34.550217 not1mm-23.4.6/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.4.6/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10342 2023-04-04 19:55:47.000000 not1mm-23.4.6/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.4.6/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    27632 2023-04-06 16:34:21.000000 not1mm-23.4.6/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.4.6/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.4.6/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.4.6/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      734 2023-03-31 15:55:44.000000 not1mm-23.4.6/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.4.6/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.4.6/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1954 2023-03-17 17:01:08.000000 not1mm-23.4.6/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.4.6/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.4.6/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      350 2023-03-06 18:07:06.000000 not1mm-23.4.6/not1mm/lib/qrz_dialog.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.4.6/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-04-06 17:13:12.000000 not1mm-23.4.6/not1mm/lib/version.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    28034 2023-04-05 21:31:54.000000 not1mm-23.4.6/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-04-06 17:36:34.553217 not1mm-23.4.6/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.4.6/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2456 2023-03-28 17:33:53.000000 not1mm-23.4.6/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2459 2023-03-28 17:34:18.000000 not1mm-23.4.6/not1mm/plugins/arrl_dx_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12593 2023-04-05 21:08:37.000000 not1mm-23.4.6/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2464 2023-03-28 17:34:12.000000 not1mm-23.4.6/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2465 2023-03-28 17:34:06.000000 not1mm-23.4.6/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2468 2023-03-28 17:33:59.000000 not1mm-23.4.6/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14651 2023-04-02 16:44:37.000000 not1mm-23.4.6/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14659 2023-04-03 15:09:21.000000 not1mm-23.4.6/not1mm/plugins/cq_wpx_rtty.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14655 2023-04-03 15:09:18.000000 not1mm-23.4.6/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2153 2023-03-28 17:33:25.000000 not1mm-23.4.6/not1mm/plugins/cqww_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2157 2023-03-28 17:33:25.000000 not1mm-23.4.6/not1mm/plugins/cqww_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7177 2023-04-04 14:52:27.000000 not1mm-23.4.6/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13549 2023-04-06 16:32:50.000000 not1mm-23.4.6/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13550 2023-04-06 16:31:42.000000 not1mm-23.4.6/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2725 2023-03-28 17:33:25.000000 not1mm-23.4.6/not1mm/plugins/winter_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3906 2023-03-07 21:13:08.000000 not1mm-23.4.6/not1mm/test.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-04-06 17:36:34.553217 not1mm-23.4.6/not1mm/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2297 2023-03-29 19:50:12.000000 not1mm-23.4.6/not1mm/testing/test.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-04-06 17:36:34.535217 not1mm-23.4.6/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12200 2023-04-06 17:36:34.000000 not1mm-23.4.6/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1801 2023-04-06 17:36:34.000000 not1mm-23.4.6/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-04-06 17:36:34.000000 not1mm-23.4.6/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-04-06 17:36:34.000000 not1mm-23.4.6/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       42 2023-04-06 17:36:34.000000 not1mm-23.4.6/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-04-06 17:36:34.000000 not1mm-23.4.6/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1148 2023-04-06 17:13:25.000000 not1mm-23.4.6/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-04-06 17:36:34.554216 not1mm-23.4.6/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-04-06 17:36:34.553217 not1mm-23.4.6/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.4.6/testing/test.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      861 2023-03-29 19:39:25.000000 not1mm-23.4.6/testing/text2.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.847775 not1mm-23.5.1/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.1/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20878 2023-05-01 16:46:02.847775 not1mm-23.5.1/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20133 2023-05-01 16:41:22.000000 not1mm-23.5.1/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.819775 not1mm-23.5.1/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.1/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    77026 2023-05-01 14:18:20.000000 not1mm-23.5.1/not1mm/__main__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    18617 2023-04-30 04:11:31.000000 not1mm-23.5.1/not1mm/bandmap.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.830775 not1mm-23.5.1/not1mm/data/
+-rw-rw-rw-   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.1/not1mm/data/Combinear.qss
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.1/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.1/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.1/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.1/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.1/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.1/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    31458 2023-04-24 19:59:20.000000 not1mm-23.5.1/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.1/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.1/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.1/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.1/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.1/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.1/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.1/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.1/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.1/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.1/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.1/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43658 2023-05-01 15:38:56.000000 not1mm-23.5.1/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17405 2023-05-01 15:15:03.000000 not1mm-23.5.1/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.1/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.840775 not1mm-23.5.1/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.1/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.1/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.1/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.1/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.1/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.1/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.1/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.1/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.1/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.1/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.1/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.1/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.1/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.1/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.1/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.1/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.1/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.1/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.1/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.1/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.1/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.1/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.1/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.1/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.1/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.1/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.1/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.1/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.1/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.1/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.1/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.1/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.1/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.1/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.1/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.1/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.1/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.1/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.1/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.1/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.1/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.1/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.1/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.1/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.1/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.1/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.1/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.1/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.1/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.1/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.1/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.1/not1mm/data/ssbmacros.txt
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.843775 not1mm-23.5.1/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.1/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.1/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12468 2023-04-25 15:08:00.000000 not1mm-23.5.1/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.1/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32966 2023-04-24 03:05:48.000000 not1mm-23.5.1/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.1/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.1/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.1/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.1/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.1/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.1/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.1/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.1/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.1/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.1/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5414 2023-04-21 15:02:17.000000 not1mm-23.5.1/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-05-01 16:43:25.000000 not1mm-23.5.1/not1mm/lib/version.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    31120 2023-04-29 16:10:36.000000 not1mm-23.5.1/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.846775 not1mm-23.5.1/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13558 2023-05-01 16:14:59.000000 not1mm-23.5.1/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.1/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14348 2023-04-24 14:53:10.000000 not1mm-23.5.1/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14351 2023-04-24 14:53:19.000000 not1mm-23.5.1/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12719 2023-04-24 14:53:32.000000 not1mm-23.5.1/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2590 2023-04-24 14:53:43.000000 not1mm-23.5.1/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2591 2023-04-24 14:53:53.000000 not1mm-23.5.1/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2594 2023-04-24 14:54:04.000000 not1mm-23.5.1/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14755 2023-04-24 14:54:20.000000 not1mm-23.5.1/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14759 2023-04-24 14:54:36.000000 not1mm-23.5.1/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13701 2023-04-24 14:54:47.000000 not1mm-23.5.1/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13772 2023-04-24 14:54:56.000000 not1mm-23.5.1/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14624 2023-04-24 14:52:00.000000 not1mm-23.5.1/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7272 2023-04-24 14:55:06.000000 not1mm-23.5.1/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13650 2023-04-24 14:55:15.000000 not1mm-23.5.1/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13651 2023-04-24 14:55:25.000000 not1mm-23.5.1/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2851 2023-04-24 14:55:37.000000 not1mm-23.5.1/not1mm/plugins/winter_field_day.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.846775 not1mm-23.5.1/not1mm/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2297 2023-03-29 19:50:12.000000 not1mm-23.5.1/not1mm/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.820775 not1mm-23.5.1/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20878 2023-05-01 16:46:02.000000 not1mm-23.5.1/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3354 2023-05-01 16:46:02.000000 not1mm-23.5.1/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-01 16:46:02.000000 not1mm-23.5.1/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-01 16:46:02.000000 not1mm-23.5.1/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-01 16:46:02.000000 not1mm-23.5.1/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-01 16:46:02.000000 not1mm-23.5.1/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1217 2023-05-01 16:43:42.000000 not1mm-23.5.1/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-01 16:46:02.847775 not1mm-23.5.1/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.847775 not1mm-23.5.1/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.1/testing/test.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-21 20:18:16.000000 not1mm-23.5.1/testing/text2.py
```

### Comparing `not1mm-23.4.6/LICENSE` & `not1mm-23.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/__main__.py` & `not1mm-23.5.1/not1mm/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 #!/usr/bin/env python3
 """
 NOT1MM Logger
 """
-# pylint: disable=unused-import, c-extension-no-member, no-member, invalid-name
+# pylint: disable=unused-import, c-extension-no-member, no-member, invalid-name, too-many-lines, no-name-in-module
 
 import importlib
 import logging
 import os
 import pkgutil
+import queue
 import re
 import socket
 import subprocess
-
-# import sqlite3
 import sys
 import threading
+import time
 import uuid
+
 from datetime import datetime
-from json import dumps, loads
+from json import dumps, loads, JSONDecodeError
 from pathlib import Path
 from shutil import copyfile
 from xmlrpc.client import Error, ServerProxy
 
 import psutil
 from PyQt5 import QtCore, QtGui, QtWidgets, uic
 from PyQt5.QtWidgets import QFileDialog
 from PyQt5.QtCore import QPoint  # pylint: disable=no-name-in-module
 from PyQt5.QtCore import QDir, QRect, QSize, Qt
 from PyQt5.QtGui import QFontDatabase  # pylint: disable=no-name-in-module
+import sounddevice as sd
+import soundfile as sf
 
+from not1mm.lib.about import About
 from not1mm.lib.cat_interface import CAT
 from not1mm.lib.cwinterface import CW
 from not1mm.lib.database import DataBase
 from not1mm.lib.edit_macro import EditMacro
 from not1mm.lib.edit_opon import OpOn
 from not1mm.lib.edit_station import EditStation
 from not1mm.lib.select_contest import SelectContest
+from not1mm.lib.settings import Settings
 from not1mm.lib.ham_utility import (
     bearing,
     bearing_with_latlon,
     calculate_wpx_prefix,
     distance,
     distance_with_latlon,
     get_logged_band,
     getband,
     reciprocol,
 )
-from not1mm.lib.lookup import QRZlookup
+from not1mm.lib.lookup import QRZlookup, HamDBlookup, HamQTH
 from not1mm.lib.multicast import Multicast
 from not1mm.lib.new_contest import NewContest
 from not1mm.lib.n1mm import N1MM
-from not1mm.lib.qrz_dialog import UseQRZ
 from not1mm.lib.version import __version__
 
-# os.environ["QT_QPA_PLATFORM"] = "wayland"
 os.environ["QT_QPA_PLATFORMTHEME"] = "gnome"
-# os.environ["QT_STYLE_OVERRIDE"] = "Fusion"
 
 loader = pkgutil.get_loader("not1mm")
 WORKING_PATH = os.path.dirname(loader.get_filename())
 
 if "XDG_DATA_HOME" in os.environ:
     DATA_PATH = os.environ.get("XDG_DATA_HOME")
 else:
@@ -78,16 +80,16 @@
 try:
     os.mkdir(CONFIG_PATH)
 except FileExistsError:
     ...
 
 CTYFILE = {}
 
-with open(WORKING_PATH + "/data/cty.json", "rt", encoding="utf-8") as fd:
-    CTYFILE = loads(fd.read())
+with open(WORKING_PATH + "/data/cty.json", "rt", encoding="utf-8") as c_file:
+    CTYFILE = loads(c_file.read())
 
 DARK_STYLESHEET = ""
 
 with open(WORKING_PATH + "/data/Combinear.qss", encoding="utf-8") as stylefile:
     DARK_STYLESHEET = stylefile.read()
 
 
@@ -117,14 +119,15 @@
 
 class MainWindow(QtWidgets.QMainWindow):
     """
     The main window
     """
 
     pref_ref = {
+        "sounddevice": "default",
         "useqrz": False,
         "lookupusername": "username",
         "lookuppassword": "password",
         "run_state": True,
         "dark_mode": False,
         "command_buttons": False,
         "cw_macros": True,
@@ -142,67 +145,97 @@
         "n1mm_station_name": "20M CW Tent",
         "n1mm_operator": "Bernie",
         "n1mm_ip": "127.0.0.1",
         "n1mm_radioport": 12060,
         "n1mm_contactport": 12061,
         "n1mm_lookupport": 12060,
         "n1mm_scoreport": 12062,
+        "usehamdb": False,
+        "usehamqth": False,
+        "cloudlog": False,
+        "cloudlogapi": "",
+        "cloudlogurl": "",
+        "CAT_ip": "127.0.0.1",
+        "userigctld": True,
+        "useflrig": False,
+        "cwip": "127.0.0.1",
+        "cwport": 6789,
+        "cwtype": 1,
+        "useserver": False,
+        "CAT_port": 4532,
     }
     appstarted = False
+    contact = {}
     contest = None
     contest_settings = {}
     pref = None
     station = {}
     current_op = ""
     current_mode = ""
     current_band = ""
+    cw = None
     look_up = None
     run_state = False
     fkeys = {}
+    about_dialog = None
     qrz_dialog = None
     settings_dialog = None
     edit_macro_dialog = None
     contest_dialog = None
+    configuration_dialog = None
     opon_dialog = None
     dbname = DATA_PATH + "/ham.db"
     radio_state = {}
+    rig_control = None
     server_udp = None
     multicast_group = None
     multicast_port = None
     interface_ip = None
     rig_control = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         logger.info("MainWindow: __init__")
-
+        self._udpwatch = None
+        self.udp_fifo = queue.Queue()
         data_path = WORKING_PATH + "/data/main.ui"
         uic.loadUi(data_path, self)
+        self.leftdot.hide()
+        self.rightdot.hide()
         self.n1mm = N1MM()
         self.next_field = self.other_2
         self.dupe_indicator.hide()
         self.cw_speed.valueChanged.connect(self.cwspeed_spinbox_changed)
 
         self.actionCW_Macros.triggered.connect(self.cw_macros_state_changed)
         self.actionCommand_Buttons.triggered.connect(self.command_buttons_state_change)
         self.actionDark_Mode.triggered.connect(self.dark_mode_state_change)
         self.actionLog_Window.triggered.connect(self.launch_log_window)
+        self.actionBandmap.triggered.connect(self.launch_bandmap_window)
         self.actionRecalculate_Mults.triggered.connect(self.recalculate_mults)
 
         self.actionGenerate_Cabrillo.triggered.connect(self.generate_cabrillo)
         self.actionGenerate_ADIF.triggered.connect(self.generate_adif)
 
+        self.actionConfiguration_Settings.triggered.connect(
+            self.edit_configuration_settings
+        )
         self.actionStationSettings.triggered.connect(self.edit_station_settings)
-        self.actionQRZ_Settings.triggered.connect(self.qrz_preference_selected)
 
         self.actionNew_Contest.triggered.connect(self.new_contest_dialog)
         self.actionOpen_Contest.triggered.connect(self.open_contest)
+        self.actionEdit_Current_Contest.triggered.connect(self.edit_contest)
+
         self.actionNew_Database.triggered.connect(self.new_database)
         self.actionOpen_Database.triggered.connect(self.open_database)
 
+        self.actionEdit_Macros.triggered.connect(self.edit_cw_macros)
+
+        self.actionAbout.triggered.connect(self.show_about_dialog)
+
         self.radioButton_run.clicked.connect(self.run_sp_buttons_clicked)
         self.radioButton_sp.clicked.connect(self.run_sp_buttons_clicked)
         self.score.setText("0")
         self.callsign.textEdited.connect(self.callsign_changed)
         self.callsign.returnPressed.connect(self.save_contact)
         self.sent.returnPressed.connect(self.save_contact)
         self.receive.returnPressed.connect(self.save_contact)
@@ -261,36 +294,22 @@
             self.station = {}
             self.edit_station_settings()
             self.station = self.database.fetch_station()
             if self.station is None:
                 self.station = {}
         self.contact = self.database.empty_contact
         self.current_op = self.station.get("Call", "")
+        self.make_op_dir()
         if self.pref.get("contest"):
             self.load_contest()
 
-        self.cw = CW(1, "127.0.0.1", 6789)
-        # self.cw = CW(2, "127.0.0.1", 8000)
-
         self.read_cw_macros()
         self.clearinputs()
         # self.launch_log_window()
 
-        self.rig_control = None
-        local_flrig = self.check_process("flrig")
-        local_rigctld = self.check_process("rigctld")
-        if local_flrig:
-            logger.debug("Found flrig")
-            address, port = "localhost", "12345"
-            self.rig_control = CAT("flrig", address, int(port))
-        if local_rigctld:
-            logger.debug("Found rigctld")
-            address, port = "localhost", "4532"
-            self.rig_control = CAT("rigctld", address, int(port))
-
         self.band_indicators_cw = {
             "160": self.cw_band_160,
             "80": self.cw_band_80,
             "40": self.cw_band_40,
             "20": self.cw_band_20,
             "15": self.cw_band_15,
             "10": self.cw_band_10,
@@ -315,23 +334,60 @@
         }
 
         self.all_mode_indicators = {
             "CW": self.band_indicators_cw,
             "SSB": self.band_indicators_ssb,
             "RTTY": self.band_indicators_rtty,
         }
+        if self._udpwatch is None:
+            self._udpwatch = threading.Thread(
+                target=self.watch_udp,
+                daemon=True,
+            )
+            self._udpwatch.start()
 
     @staticmethod
     def check_process(name: str) -> bool:
         """checks to see if program of name is in the active process list"""
         for proc in psutil.process_iter():
             if bool(re.match(name, proc.name().lower())):
                 return True
         return False
 
+    def show_message_box(self, message: str) -> None:
+        """doc"""
+        message_box = QtWidgets.QMessageBox()
+        message_box.setIcon(QtWidgets.QMessageBox.Information)
+        message_box.setText(message)
+        message_box.setWindowTitle("Information")
+        message_box.setStandardButtons(QtWidgets.QMessageBox.Ok)
+        _ = message_box.exec_()
+
+    def show_about_dialog(self):
+        """Show about dialog"""
+        self.about_dialog = About(WORKING_PATH)
+        if self.pref.get("dark_mode"):
+            self.about_dialog.setStyleSheet(DARK_STYLESHEET)
+        self.about_dialog.open()
+
+    def edit_configuration_settings(self):
+        """Configuration Settings was clicked"""
+        self.configuration_dialog = Settings(WORKING_PATH, CONFIG_PATH, self.pref)
+        self.configuration_dialog.usehamdb_radioButton.hide()
+        # self.configuration_dialog.n1mm_tab.hide()
+        self.configuration_dialog.show()
+        self.configuration_dialog.accepted.connect(self.edit_configuration_return)
+
+    def edit_configuration_return(self):
+        """Returns here when configuration dialog closed with okay."""
+        self.configuration_dialog.save_changes()
+        self.write_preference()
+        logger.debug("%s", f"{self.pref}")
+        self.readpreferences()
+
     def new_database(self):
         """Create new database."""
         filename = self.filepicker("new")
         if filename:
             if filename[-3:] != ".db":
                 filename += ".db"
             self.pref["current_database"] = filename.split("/")[-1:][0]
@@ -339,14 +395,15 @@
             self.dbname = DATA_PATH + "/" + self.pref.get("current_database", "ham.db")
             self.database = DataBase(self.dbname, WORKING_PATH)
             self.contact = self.database.empty_contact
             self.station = self.database.fetch_station()
             if self.station is None:
                 self.station = {}
             self.current_op = self.station.get("Call", "")
+            self.make_op_dir()
             cmd = {}
             cmd["cmd"] = "NEWDB"
             self.multicast_interface.send_as_json(cmd)
             self.clearinputs()
             self.edit_station_settings()
 
     def open_database(self):
@@ -360,14 +417,15 @@
             self.contact = self.database.empty_contact
             self.station = self.database.fetch_station()
             if self.station is None:
                 self.station = {}
             if self.station.get("Call", "") == "":
                 self.edit_station_settings()
             self.current_op = self.station.get("Call", "")
+            self.make_op_dir()
             cmd = {}
             cmd["cmd"] = "NEWDB"
             self.multicast_interface.send_as_json(cmd)
             self.clearinputs()
 
     def new_contest(self):
         """Create new contest in existing database."""
@@ -422,29 +480,120 @@
         selected_row = self.contest_dialog.contest_list.currentRow()
         contest = self.contest_dialog.contest_list.item(selected_row, 0).text()
         self.pref["contest"] = contest
         self.write_preference()
         logger.debug("Selected contest: %s", f"{contest}")
         self.load_contest()
 
+    def refill_dropdown(self, target, source):
+        """Refill QCombobox widget with value."""
+        index = target.findText(source)
+        target.setCurrentIndex(index)
+
+    def edit_contest(self):
+        """Edit the current contest"""
+        logger.debug("Edit contest Dialog")
+        if self.contest_settings is None:
+            return
+        self.contest_dialog = NewContest(WORKING_PATH)
+        self.contest_dialog.setWindowTitle("Edit Contest")
+        self.contest_dialog.title.setText("")
+        self.contest_dialog.accepted.connect(self.save_edited_contest)
+        if self.pref.get("dark_mode"):
+            self.contest_dialog.setStyleSheet(DARK_STYLESHEET)
+
+        value = self.contest_settings.get("ContestName").upper().replace("_", " ")
+        if value == "GENERAL LOGGING":
+            value = "General Logging"
+        self.refill_dropdown(self.contest_dialog.contest, value)
+        value = self.contest_settings.get("OperatorCategory")
+        self.refill_dropdown(self.contest_dialog.operator_class, value)
+        value = self.contest_settings.get("BandCategory")
+        self.refill_dropdown(self.contest_dialog.band, value)
+        value = self.contest_settings.get("PowerCategory")
+        self.refill_dropdown(self.contest_dialog.power, value)
+        value = self.contest_settings.get("ModeCategory")
+        self.refill_dropdown(self.contest_dialog.mode, value)
+        value = self.contest_settings.get("OverlayCategory")
+        self.refill_dropdown(self.contest_dialog.overlay, value)
+        self.contest_dialog.operators.setText(self.contest_settings.get("Operators"))
+        self.contest_dialog.soapbox.setPlainText(self.contest_settings.get("Soapbox"))
+        self.contest_dialog.exchange.setText(self.contest_settings.get("SentExchange"))
+        value = self.contest_settings.get("StationCategory")
+        self.refill_dropdown(self.contest_dialog.station, value)
+        value = self.contest_settings.get("AssistedCategory")
+        self.refill_dropdown(self.contest_dialog.assisted, value)
+        value = self.contest_settings.get("TransmitterCategory")
+        self.refill_dropdown(self.contest_dialog.transmitter, value)
+        value = self.contest_settings.get("StartDate")
+        the_date, the_time = value.split()
+        self.contest_dialog.dateTimeEdit.setDate(
+            QtCore.QDate.fromString(the_date, "yyyy-MM-dd")
+        )
+        self.contest_dialog.dateTimeEdit.setCalendarPopup(True)
+        self.contest_dialog.dateTimeEdit.setTime(
+            QtCore.QTime.fromString(the_time, "hh:mm:ss")
+        )
+        self.contest_dialog.open()
+
+    def save_edited_contest(self):
+        """Save the edited contest"""
+        contest = {}
+        contest["ContestName"] = (
+            self.contest_dialog.contest.currentText().lower().replace(" ", "_")
+        )
+        contest["StartDate"] = self.contest_dialog.dateTimeEdit.dateTime().toString(
+            "yyyy-MM-dd hh:mm:ss"
+        )
+        contest["OperatorCategory"] = self.contest_dialog.operator_class.currentText()
+        contest["BandCategory"] = self.contest_dialog.band.currentText()
+        contest["PowerCategory"] = self.contest_dialog.power.currentText()
+        contest["ModeCategory"] = self.contest_dialog.mode.currentText()
+        contest["OverlayCategory"] = self.contest_dialog.overlay.currentText()
+        contest["Operators"] = self.contest_dialog.operators.text()
+        contest["Soapbox"] = self.contest_dialog.soapbox.toPlainText()
+        contest["SentExchange"] = self.contest_dialog.exchange.text()
+        contest["ContestNR"] = self.pref.get("contest", 1)
+        contest["StationCategory"] = self.contest_dialog.station.currentText()
+        contest["AssistedCategory"] = self.contest_dialog.assisted.currentText()
+        contest["TransmitterCategory"] = self.contest_dialog.transmitter.currentText()
+
+        logger.debug("%s", f"{contest}")
+        self.database.update_contest(contest)
+        self.write_preference()
+        self.load_contest()
+
     def load_contest(self):
         """load a contest"""
         if self.pref.get("contest"):
             self.contest_settings = self.database.fetch_contest_by_id(
                 self.pref.get("contest")
             )
-            self.database.current_contest = self.pref.get("contest")
-            if self.contest_settings.get("ContestName"):
-                self.contest = doimp(self.contest_settings.get("ContestName"))
-                logger.debug("Loaded Contest Name = %s", self.contest.name)
-                self.contest.init_contest(self)
-                self.hide_band_mode(self.contest_settings.get("ModeCategory", ""))
-            cmd = {}
-            cmd["cmd"] = "NEWDB"
-            self.multicast_interface.send_as_json(cmd)
+            if self.contest_settings:
+                self.database.current_contest = self.pref.get("contest")
+                if self.contest_settings.get("ContestName"):
+                    self.contest = doimp(self.contest_settings.get("ContestName"))
+                    logger.debug("Loaded Contest Name = %s", self.contest.name)
+                    self.contest.init_contest(self)
+                    self.hide_band_mode(self.contest_settings.get("ModeCategory", ""))
+
+                if hasattr(self.contest, "mode"):
+                    if self.contest.mode in ["CW", "BOTH"]:
+                        self.cw_speed.show()
+                    else:
+                        self.cw_speed.hide()
+
+                cmd = {}
+                cmd["cmd"] = "NEWDB"
+                self.multicast_interface.send_as_json(cmd)
+                if hasattr(self.contest, "columns"):
+                    cmd = {}
+                    cmd["cmd"] = "SHOWCOLUMNS"
+                    cmd["COLUMNS"] = self.contest.columns
+                    self.multicast_interface.send_as_json(cmd)
 
     def hide_band_mode(self, the_mode: str) -> None:
         """hide"""
         logger.debug("%s", f"{the_mode}")
         self.Band_Mode_Frame_CW.hide()
         self.Band_Mode_Frame_SSB.hide()
         self.Band_Mode_Frame_RTTY.hide()
@@ -499,14 +648,19 @@
         self.contest.recalculate_mults(self)
 
     def launch_log_window(self):
         """launch the Log Window"""
         if not check_process("logwindow.py"):
             _ = subprocess.Popen([sys.executable, WORKING_PATH + "/logwindow.py"])
 
+    def launch_bandmap_window(self):
+        """launch the Log Window"""
+        if not check_process("bandmap.py"):
+            _ = subprocess.Popen([sys.executable, WORKING_PATH + "/bandmap.py"])
+
     def clear_band_indicators(self):
         """Clear the indicators"""
         for _, indicators in self.all_mode_indicators.items():
             for _, indicator in indicators.items():
                 indicator.setFrameShape(QtWidgets.QFrame.NoFrame)
 
     def set_band_indicator(self, band: str) -> None:
@@ -686,16 +840,16 @@
             f"- Not1MM v{__version__}"
         )
 
     def clearinputs(self):
         """Clears the text input fields and sets focus to callsign field."""
         self.dupe_indicator.hide()
         self.contact = self.database.empty_contact
-        self.heading_distance.setText("No Heading")
-        self.dx_entity.setText("dxentity")
+        self.heading_distance.setText("")
+        self.dx_entity.setText("")
         if self.contest:
             mults = self.contest.show_mults(self)
             qsos = self.contest.show_qso(self)
             multstring = f"{qsos}/{mults}"
             self.mults.setText(multstring)
             score = self.contest.calc_score(self)
             self.score.setText(str(score))
@@ -779,35 +933,14 @@
         # self.contact["GridSquare"]
         # self.contact["Continent"]
         # self.contact["RoverLocation"]
         # self.contact["RadioInterfaced"]
         # self.contact["NetworkedCompNr"]
         # self.contact["CLAIMEDQSO"]
 
-    def qrz_preference_selected(self):
-        """Show QRZ settings dialog"""
-        logger.debug("QRZ preference selected")
-        self.qrz_dialog = UseQRZ(WORKING_PATH)
-        self.qrz_dialog.accepted.connect(self.save_qrz_settings)
-        if self.pref.get("dark_mode"):
-            self.qrz_dialog.setStyleSheet(DARK_STYLESHEET)
-        self.qrz_dialog.useqrz.setChecked(self.pref.get("useqrz", False))
-        self.qrz_dialog.username.setText(self.pref.get("lookupusername", ""))
-        self.qrz_dialog.password.setText(self.pref.get("lookuppassword", ""))
-        self.qrz_dialog.open()
-
-    def save_qrz_settings(self):
-        """Save QRZ settings"""
-        self.pref["useqrz"] = self.qrz_dialog.useqrz.isChecked()
-        self.pref["lookupusername"] = self.qrz_dialog.username.text()
-        self.pref["lookuppassword"] = self.qrz_dialog.password.text()
-        self.qrz_dialog.close()
-        self.write_preference()
-        self.readpreferences()
-
     def new_contest_dialog(self):
         """Show new contest dialog"""
         logger.debug("New contest Dialog")
         self.contest_dialog = NewContest(WORKING_PATH)
         self.contest_dialog.accepted.connect(self.save_contest)
         if self.pref.get("dark_mode"):
             self.contest_dialog.setStyleSheet(DARK_STYLESHEET)
@@ -909,14 +1042,15 @@
         self.station["RoverQTH"] = self.settings_dialog.RoverQTH.text()
         self.station["Club"] = self.settings_dialog.Club.text().title()
         self.station["Email"] = self.settings_dialog.Email.text()
         self.database.add_station(self.station)
         self.settings_dialog.close()
         if self.current_op == "":
             self.current_op = self.station.get("Call", "")
+            self.make_op_dir()
         contest_count = self.database.fetch_all_contests()
         if len(contest_count) == 0:
             self.new_contest_dialog()
 
     def edit_macro(self, function_key):
         """Show edit macro dialog"""
         self.edit_macro_dialog = EditMacro(function_key, WORKING_PATH)
@@ -930,15 +1064,14 @@
         self.edit_macro_dialog.function_key.setText(
             self.edit_macro_dialog.macro_label.text()
         )
         self.edit_macro_dialog.function_key.setToolTip(
             self.edit_macro_dialog.the_macro.text()
         )
         self.edit_macro_dialog.close()
-        # logger.debug(f"{self.current_op}")
 
     def edit_F1(self):
         """stub"""
         logger.debug("F1 Right Clicked.")
         self.edit_macro(self.F1)
 
     def edit_F2(self):
@@ -995,91 +1128,186 @@
         """stub"""
         logger.debug("F12 Right Clicked.")
         self.edit_macro(self.F12)
 
     def process_macro(self, macro: str) -> str:
         """Process CW macro substitutions"""
         macro = macro.upper()
-        macro = macro.replace("{MYCALL}", self.station.get("Call"))
+        macro = macro.replace("{MYCALL}", self.station.get("Call", ""))
         macro = macro.replace("{HISCALL}", self.callsign.text())
-        macro = macro.replace("{SNT}", self.sent.text().replace("9", "n"))  # FIXME
+        if self.radio_state.get("mode") == "CW":
+            macro = macro.replace("{SNT}", self.sent.text().replace("9", "n"))
+        else:
+            macro = macro.replace("{SNT}", self.sent.text())
         macro = macro.replace("{SENTNR}", self.other_1.text())
+        macro = macro.replace(
+            "{EXCH}", self.contest_settings.get("SentExchange", "xxx")
+        )
         return macro
 
+    def voice_string(self, the_string: str) -> None:
+        """voices string using nato phonetics"""
+        logger.debug("Voicing: %s", the_string)
+        op_path = Path(DATA_PATH) / self.current_op
+        if "[" in the_string:
+            sub_string = the_string.strip("[]").lower()
+            filename = f"{str(op_path)}/{sub_string}.wav"
+            if Path(filename).is_file():
+                logger.debug("Voicing: %s", filename)
+                data, _fs = sf.read(filename, dtype="float32")
+                self.ptt_on()
+                try:
+                    sd.default.device = self.pref.get("sounddevice", "default")
+                    sd.default.samplerate = 44100.0
+                    sd.play(data)
+                    _status = sd.wait()
+                    # https://snyk.io/advisor/python/sounddevice/functions/sounddevice.PortAudioError
+                except sd.PortAudioError as err:
+                    logger.debug("%s", f"{err}")
+
+                self.ptt_off()
+            return
+        self.ptt_on()
+        for letter in the_string.lower():
+            if letter in "abcdefghijklmnopqrstuvwxyz 1234567890":
+                if letter == " ":
+                    letter = "space"
+                filename = f"{str(op_path)}/{letter}.wav"
+                if Path(filename).is_file():
+                    logger.debug("Voicing: %s", filename)
+                    data, _fs = sf.read(filename, dtype="float32")
+                    try:
+                        sd.default.device = self.pref.get("sounddevice", "default")
+                        sd.default.samplerate = 44100.0
+                        sd.play(data)
+                        logger.debug("%s", f"{sd.wait()}")
+                    except sd.PortAudioError as err:
+                        logger.debug("%s", f"{err}")
+        self.ptt_off()
+
+    def ptt_on(self):
+        """turn on ptt"""
+        if self.rig_control:
+            self.leftdot.setPixmap(self.greendot)
+            app.processEvents()
+            self.rig_control.ptt_on()
+
+    def ptt_off(self):
+        """turn off ptt"""
+        self.leftdot.setPixmap(self.reddot)
+        app.processEvents()
+        self.rig_control.ptt_off()
+
     def sendf1(self):
         """stub"""
         logger.debug("F1 Clicked")
+        if self.radio_state.get("mode") in ["USB", "SSB"]:
+            self.voice_string(self.process_macro(self.F1.toolTip()))
+            return
         if self.cw:
             # if self.preference.get("send_n1mm_packets"):
             #     self.n1mm.radio_info["FunctionKeyCaption"] = self.F1.text()
             self.cw.sendcw(self.process_macro(self.F1.toolTip()))
 
     def sendf2(self):
         """stub"""
         logger.debug("F2 Clicked")
+        if self.radio_state.get("mode") in ["USB", "SSB"]:
+            self.voice_string(self.process_macro(self.F2.toolTip()))
+            return
         if self.cw:
             self.cw.sendcw(self.process_macro(self.F2.toolTip()))
 
     def sendf3(self):
         """stub"""
         logger.debug("F3 Clicked")
+        if self.radio_state.get("mode") in ["USB", "SSB"]:
+            self.voice_string(self.process_macro(self.F3.toolTip()))
+            return
         if self.cw:
             self.cw.sendcw(self.process_macro(self.F3.toolTip()))
 
     def sendf4(self):
         """stub"""
         logger.debug("F4 Clicked")
+        if self.radio_state.get("mode") in ["USB", "SSB"]:
+            self.voice_string(self.process_macro(self.F4.toolTip()))
+            return
         if self.cw:
             self.cw.sendcw(self.process_macro(self.F4.toolTip()))
 
     def sendf5(self):
         """stub"""
         logger.debug("F5 Clicked")
+        if self.radio_state.get("mode") in ["USB", "SSB"]:
+            self.voice_string(self.process_macro(self.F5.toolTip()))
+            return
         if self.cw:
             self.cw.sendcw(self.process_macro(self.F5.toolTip()))
 
     def sendf6(self):
         """stub"""
         logger.debug("F6 Clicked")
+        if self.radio_state.get("mode") in ["USB", "SSB"]:
+            self.voice_string(self.process_macro(self.F6.toolTip()))
+            return
         if self.cw:
             self.cw.sendcw(self.process_macro(self.F6.toolTip()))
 
     def sendf7(self):
         """stub"""
         logger.debug("F7 Clicked")
+        if self.radio_state.get("mode") in ["USB", "SSB"]:
+            self.voice_string(self.process_macro(self.F7.toolTip()))
+            return
         if self.cw:
             self.cw.sendcw(self.process_macro(self.F7.toolTip()))
 
     def sendf8(self):
         """stub"""
         logger.debug("F8 Clicked")
+        if self.radio_state.get("mode") in ["USB", "SSB"]:
+            self.voice_string(self.process_macro(self.F8.toolTip()))
+            return
         if self.cw:
             self.cw.sendcw(self.process_macro(self.F8.toolTip()))
 
     def sendf9(self):
         """stub"""
         logger.debug("F9 Clicked")
+        if self.radio_state.get("mode") in ["USB", "SSB"]:
+            self.voice_string(self.process_macro(self.F9.toolTip()))
+            return
         if self.cw:
             self.cw.sendcw(self.process_macro(self.F9.toolTip()))
 
     def sendf10(self):
         """stub"""
         logger.debug("F10 Clicked")
+        if self.radio_state.get("mode") in ["USB", "SSB"]:
+            self.voice_string(self.process_macro(self.F10.toolTip()))
+            return
         if self.cw:
             self.cw.sendcw(self.process_macro(self.F10.toolTip()))
 
     def sendf11(self):
         """stub"""
         logger.debug("F11 Clicked")
+        if self.radio_state.get("mode") in ["USB", "SSB"]:
+            self.voice_string(self.process_macro(self.F11.toolTip()))
+            return
         if self.cw:
             self.cw.sendcw(self.process_macro(self.F11.toolTip()))
 
     def sendf12(self):
         """stub"""
         logger.debug("F12 Clicked")
+        if self.radio_state.get("mode") in ["USB", "SSB"]:
+            self.voice_string(self.process_macro(self.F12.toolTip()))
+            return
         if self.cw:
             self.cw.sendcw(self.process_macro(self.F12.toolTip()))
 
     def run_sp_buttons_clicked(self):
         """Handle run/s&p mode"""
         self.pref["run_state"] = self.radioButton_run.isChecked()
         self.write_preference()
@@ -1115,21 +1343,29 @@
                     CONFIG_PATH + "/not1mm.json", "wt", encoding="utf-8"
                 ) as file_descriptor:
                     self.pref = self.pref_ref.copy()
                     file_descriptor.write(dumps(self.pref, indent=4))
                     logger.info("%s", self.pref)
         except IOError as exception:
             logger.critical("Error: %s", exception)
+
+        self.look_up = None
         if self.pref.get("useqrz"):
             self.look_up = QRZlookup(
                 self.pref.get("lookupusername"),
                 self.pref.get("lookuppassword"),
             )
-        else:
-            self.look_up = None
+        # if self.pref.get("usehamdb"):
+        #     self.look_up = HamDBlookup()
+        if self.pref.get("usehamqth"):
+            self.look_up = HamQTH(
+                self.pref.get("lookupusername"),
+                self.pref.get("lookuppassword"),
+            )
+
         if self.pref.get("run_state"):
             self.radioButton_run.setChecked(True)
         else:
             self.radioButton_sp.setChecked(True)
 
         if self.pref.get("dark_mode"):
             self.actionDark_Mode.setChecked(True)
@@ -1154,19 +1390,100 @@
         multicast_group = self.pref.get("multicast_group", "224.1.1.1")
         multicast_port = self.pref.get("multicast_port", 2239)
         interface_ip = self.pref.get("interface_ip", "0.0.0.0")
         self.multicast_interface = Multicast(
             multicast_group, multicast_port, interface_ip
         )
 
+        self.rig_control = None
+
+        if self.pref.get("useflrig", False):
+            logger.debug(
+                "Using flrig: %s",
+                f"{self.pref.get('CAT_ip')} {self.pref.get('CAT_port')}",
+            )
+            self.rig_control = CAT(
+                "flrig",
+                self.pref.get("CAT_ip", "127.0.0.1"),
+                int(self.pref.get("CAT_port", 12345)),
+            )
+        if self.pref.get("userigctld", False):
+            logger.debug(
+                "Using rigctld: %s",
+                f"{self.pref.get('CAT_ip')} {self.pref.get('CAT_port')}",
+            )
+            self.rig_control = CAT(
+                "rigctld",
+                self.pref.get("CAT_ip", "127.0.0.1"),
+                int(self.pref.get("CAT_port", 4532)),
+            )
+
+        if self.pref.get("cwtype", 0) == 0:
+            self.cw = None
+        else:
+            self.cw = CW(
+                int(self.pref.get("cwtype")),
+                self.pref.get("cwip"),
+                int(self.pref.get("cwport", 6789)),
+            )
+            self.cw.speed = 20
+
         self.dark_mode()
         self.show_command_buttons()
         self.show_CW_macros()
         # self.show_band_mode()
 
+    def watch_udp(self):
+        """Puts UDP datagrams in a FIFO queue"""
+        while True:
+            try:
+                datagram = self.multicast_interface.server_udp.recv(1500)
+                logger.debug(datagram.decode())
+            except socket.timeout:
+                time.sleep(0.1)
+                continue
+            if datagram:
+                self.udp_fifo.put(datagram)
+
+    def check_udp_traffic(self):
+        """Checks UDP Traffic"""
+        while not self.udp_fifo.empty():
+            datagram = self.udp_fifo.get()
+            try:
+                debug_info = f"{datagram.decode()}"
+                logger.debug(debug_info)
+                json_data = loads(datagram.decode())
+            except UnicodeDecodeError as err:
+                the_error = f"Not Unicode: {err}\n{datagram}"
+                logger.debug(the_error)
+                continue
+            except JSONDecodeError as err:
+                the_error = f"Not JSON: {err}\n{datagram}"
+                logger.debug(the_error)
+                continue
+            if json_data.get("cmd", "") == "GETCOLUMNS":
+                if hasattr(self.contest, "columns"):
+                    cmd = {}
+                    cmd["cmd"] = "SHOWCOLUMNS"
+                    cmd["COLUMNS"] = self.contest.columns
+                    self.multicast_interface.send_as_json(cmd)
+            if json_data.get("cmd", "") == "TUNE":
+                # b'{"cmd": "TUNE", "freq": 7.0235, "spot": "MM0DGI"}'
+                vfo = json_data.get("freq")
+                vfo = float(vfo) * 1000000
+                self.radio_state["vfoa"] = int(vfo)
+                if self.rig_control:
+                    self.rig_control.set_vfo(int(vfo))
+                spot = json_data.get("spot", "")
+                self.callsign.setText(spot)
+                self.callsign_changed()
+                self.callsign.setFocus()
+                self.callsign.activateWindow()
+                window.raise_()
+
     def dark_mode_state_change(self):
         """darkmode dropdown checkmark changed"""
         self.pref["dark_mode"] = self.actionDark_Mode.isChecked()
         self.write_preference()
         self.dark_mode()
 
     def dark_mode(self):
@@ -1200,27 +1517,14 @@
     def show_command_buttons(self):
         """command button state change"""
         if self.pref.get("command_buttons"):
             self.Command_Buttons.show()
         else:
             self.Command_Buttons.hide()
 
-    # def show_band_mode_state_change(self):
-    #     """Called when the mode and bads menu item changes"""
-    #     self.pref["bands_modes"] = self.actionMode_and_Bands.isChecked()
-    #     self.write_preference()
-    #     self.show_band_mode()
-
-    # def show_band_mode(self):
-    #     """Hide or show band/mode indicator"""
-    #     if self.actionMode_and_Bands.isChecked():
-    #         self.Band_Mode_Frame.show()
-    #     else:
-    #         self.Band_Mode_Frame.hide()
-
     def is_floatable(self, item: str) -> bool:
         """check to see if string can be a float"""
         if item.isnumeric():
             return True
         try:
             _test = float(item)
         except ValueError:
@@ -1241,14 +1545,15 @@
                 self.setmode("CW")
                 self.radio_state["mode"] = "CW"
                 if self.rig_control:
                     if self.rig_control.online:
                         self.rig_control.set_mode("CW")
                 self.set_window_title()
                 self.clearinputs()
+                self.read_cw_macros()
                 return
             if stripped_text == "RTTY":
                 self.setmode("RTTY")
                 if self.rig_control:
                     if self.rig_control.online:
                         self.rig_control.set_mode("RTTY")
                     else:
@@ -1262,19 +1567,24 @@
                     self.radio_state["mode"] = "USB"
                 else:
                     self.radio_state["mode"] = "LSB"
                 self.set_window_title()
                 if self.rig_control:
                     self.rig_control.set_mode(self.radio_state.get("mode"))
                 self.clearinputs()
+                self.read_cw_macros()
                 return
             if stripped_text == "OPON":
                 self.get_opon()
                 self.clearinputs()
                 return
+            if stripped_text == "TEST":
+                self.show_message_box("This is a test")
+                self.clearinputs()
+                return
             if self.is_floatable(stripped_text):
                 vfo = float(stripped_text)
                 vfo = int(vfo * 1000)
                 band = getband(str(vfo))
                 self.set_band_indicator(band)
                 # self.contact["Band"] = get_logged_band(str(self.radio_state.get("vfoa", 0.0)))
                 self.radio_state["vfoa"] = vfo
@@ -1329,15 +1639,16 @@
                 self.contact["CountryPrefix"] = primary_pfx
                 self.contact["ZN"] = int(cq)
                 self.contact["Continent"] = continent
                 self.dx_entity.setText(
                     f"{primary_pfx}: {continent}/{entity} cq:{cq} itu:{itu}"
                 )
                 if len(callsign) > 2:
-                    self.contest.prefill(self)
+                    if self.contest:
+                        self.contest.prefill(self)
 
     def check_callsign2(self, callsign):
         """Check call once entered"""
         callsign = callsign.strip()
         debug_lookup = f"{self.look_up}"
         logger.debug("%s, %s", callsign, debug_lookup)
         if hasattr(self.look_up, "session"):
@@ -1358,14 +1669,15 @@
                         )
                     # self.dx_entity.setText(f"{theircountry}")
                 # else:
                 # self.heading_distance.setText("Lookup failed.")
 
     def check_dupe(self, call: str) -> bool:
         """Checks if a callsign is a dupe on current band/mode."""
+        self.contest.predupe(self)
         band = float(get_logged_band(str(self.radio_state.get("vfoa", 0.0))))
         mode = self.radio_state.get("mode", "")
         debugline = (
             f"Call: {call} Band: {band} Mode: {mode} Dupetype: {self.contest.dupe_type}"
         )
         logger.debug("%s", debugline)
         if self.contest.dupe_type == 1:
@@ -1383,20 +1695,22 @@
     def setmode(self, mode: str) -> None:
         """stub for when the mode changes."""
         if mode == "CW":
             self.current_mode = "CW"
             # self.mode.setText("CW")
             self.sent.setText("599")
             self.receive.setText("599")
+            self.read_cw_macros()
             return
         if mode == "SSB":
             self.current_mode = "SSB"
             # self.mode.setText("SSB")
             self.sent.setText("59")
             self.receive.setText("59")
+            self.read_cw_macros()
         if mode == "RTTY":
             self.current_mode = "RTTY"
             # self.mode.setText("RTTY")
             self.sent.setText("59")
             self.receive.setText("59")
 
     def get_opon(self):
@@ -1405,51 +1719,96 @@
         self.opon_dialog.accepted.connect(self.new_op)
         self.opon_dialog.open()
 
     def new_op(self):
         """Save new OP"""
         if self.opon_dialog.NewOperator.text():
             self.current_op = self.opon_dialog.NewOperator.text().upper()
-
         self.opon_dialog.close()
         logger.debug("New Op: %s", self.current_op)
+        self.make_op_dir()
+
+    def make_op_dir(self):
+        """Create OP directory if it does not exist."""
+        if self.current_op:
+            op_path = Path(DATA_PATH) / self.current_op
+            logger.debug("op_path: %s", str(op_path))
+            if op_path.is_dir() is False:
+                logger.debug("Creating Op Directory: %s", str(op_path))
+                os.mkdir(str(op_path))
+            if op_path.is_dir():
+                source_path = Path(WORKING_PATH) / "data" / "phonetics"
+                logger.debug("source_path: %s", str(source_path))
+                for child in source_path.iterdir():
+                    destination_file = op_path / child.name
+                    logger.debug("Destination: %s", str(destination_file))
+                    if destination_file.is_file() is False:
+                        destination_file.write_bytes(child.read_bytes())
 
     def poll_radio(self):
         """stub"""
         if self.rig_control:
             if self.rig_control.online:
                 vfo = self.rig_control.get_vfo()
                 mode = self.rig_control.get_mode()
+                self.radio_state["ptt"] = self.rig_control.get_ptt()
+                # if self.radio_state.get("ptt", 0) == 1:
+                #     self.leftdot.setPixmap(self.greendot)
+                # else:
+                #     self.leftdot.setPixmap(self.reddot)
                 if mode == "CW":
                     self.setmode(mode)
                 if mode == "LSB" or mode == "USB":
                     self.setmode("SSB")
                 if mode == "RTTY":
                     self.setmode("RTTY")
                 self.radio_state["vfoa"] = vfo
                 band = getband(str(vfo))
+                self.radio_state["band"] = band
                 self.contact["Band"] = get_logged_band(str(vfo))
                 self.set_band_indicator(band)
                 self.radio_state["mode"] = mode
                 # logger.debug("VFO: %s  MODE: %s", vfo, mode)
                 self.set_window_title()
+                cmd = {}
+                cmd["cmd"] = "RADIO_STATE"
+                cmd["band"] = band
+                cmd["vfoa"] = vfo
+                cmd["mode"] = mode
+                self.multicast_interface.send_as_json(cmd)
+
+    def edit_cw_macros(self) -> None:
+        """
+        Calls the default text editor to edit the CW macro file.
+        """
+        if self.radio_state.get("mode") == "CW":
+            macro_file = "/cwmacros.txt"
+        else:
+            macro_file = "/ssbmacros.txt"
+        if not Path(DATA_PATH + macro_file).exists():
+            logger.debug("read_cw_macros: copying default macro file.")
+            copyfile(WORKING_PATH + "/data" + macro_file, DATA_PATH + macro_file)
+        os.system(f"xdg-open {DATA_PATH}{macro_file}")
 
     def read_cw_macros(self) -> None:
         """
         Reads in the CW macros, firsts it checks to see if the file exists. If it does not,
         and this has been packaged with pyinstaller it will copy the default file from the
         temp directory this is running from... In theory.
         """
 
-        if not Path(DATA_PATH + "/cwmacros.txt").exists():
+        if self.radio_state.get("mode") == "CW":
+            macro_file = "/cwmacros.txt"
+        else:
+            macro_file = "/ssbmacros.txt"
+
+        if not Path(DATA_PATH + macro_file).exists():
             logger.debug("read_cw_macros: copying default macro file.")
-            copyfile(WORKING_PATH + "/data/cwmacros.txt", DATA_PATH + "/cwmacros.txt")
-        with open(
-            DATA_PATH + "/cwmacros.txt", "r", encoding="utf-8"
-        ) as file_descriptor:
+            copyfile(WORKING_PATH + "/data" + macro_file, DATA_PATH + macro_file)
+        with open(DATA_PATH + macro_file, "r", encoding="utf-8") as file_descriptor:
             for line in file_descriptor:
                 try:
                     mode, fkey, buttonname, cwtext = line.split("|")
                     if mode.strip().upper() == "R" and self.pref.get("run_state"):
                         self.fkeys[fkey.strip()] = (buttonname.strip(), cwtext.strip())
                     if mode.strip().upper() != "R" and not self.pref.get("run_state"):
                         self.fkeys[fkey.strip()] = (buttonname.strip(), cwtext.strip())
@@ -1541,14 +1900,15 @@
 def run():
     """
     Main Entry
     """
 
     install_icons()
     timer.start(1000)
+    timer2.start(1000)
 
     sys.exit(app.exec())
 
 
 logger = logging.getLogger("__main__")
 handler = logging.StreamHandler()
 formatter = logging.Formatter(
@@ -1576,11 +1936,12 @@
 y = window.pref.get("window_y", -1)
 window.setGeometry(x, y, width, height)
 window.setWindowTitle(f"Not1MM v{__version__}")
 window.callsign.setFocus()
 window.show()
 timer = QtCore.QTimer()
 timer.timeout.connect(window.poll_radio)
-
+timer2 = QtCore.QTimer()
+timer2.timeout.connect(window.check_udp_traffic)
 
 if __name__ == "__main__":
     run()
```

### Comparing `not1mm-23.4.6/not1mm/data/Combinear.qss` & `not1mm-23.5.1/not1mm/data/Combinear.qss`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-23.5.1/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/data/MASTER.SCP` & `not1mm-23.5.1/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/data/contests.sql` & `not1mm-23.5.1/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/data/cty.json` & `not1mm-23.5.1/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/data/editcontact.ui` & `not1mm-23.5.1/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/data/editmacro.ui` & `not1mm-23.5.1/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/data/k6gte.not1mm-128.png` & `not1mm-23.5.1/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/data/k6gte.not1mm-32.png` & `not1mm-23.5.1/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/data/k6gte.not1mm-64.png` & `not1mm-23.5.1/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/data/logwindow.ui` & `not1mm-23.5.1/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/data/main.ui` & `not1mm-23.5.1/not1mm/data/main.ui`

 * *Files 6% similar despite different names*

#### Comparing `not1mm-23.4.6/not1mm/data/main.ui` & `not1mm-23.5.1/not1mm/data/main.ui`

```diff
@@ -403,14 +403,17 @@
                                       <family>JetBrains Mono</family>
                                       <pointsize>20</pointsize>
                                     </font>
                                   </property>
                                   <property name="focusPolicy">
                                     <enum>Qt::ClickFocus</enum>
                                   </property>
+                                  <property name="styleSheet">
+                                    <string notr="true">text-transform: uppercase;</string>
+                                  </property>
                                 </widget>
                               </item>
                             </layout>
                           </widget>
                         </item>
                         <item>
                           <widget class="QFrame" name="field1">
@@ -432,14 +435,17 @@
                                       <family>JetBrains Mono</family>
                                       <pointsize>20</pointsize>
                                     </font>
                                   </property>
                                   <property name="focusPolicy">
                                     <enum>Qt::ClickFocus</enum>
                                   </property>
+                                  <property name="styleSheet">
+                                    <string notr="true">text-transform: uppercase;</string>
+                                  </property>
                                 </widget>
                               </item>
                             </layout>
                           </widget>
                         </item>
                         <item>
                           <widget class="QFrame" name="field2">
@@ -461,14 +467,17 @@
                                       <family>JetBrains Mono</family>
                                       <pointsize>20</pointsize>
                                     </font>
                                   </property>
                                   <property name="focusPolicy">
                                     <enum>Qt::ClickFocus</enum>
                                   </property>
+                                  <property name="styleSheet">
+                                    <string notr="true">text-transform: uppercase;</string>
+                                  </property>
                                 </widget>
                               </item>
                             </layout>
                           </widget>
                         </item>
                         <item>
                           <widget class="QFrame" name="field3">
@@ -490,14 +499,17 @@
                                       <family>JetBrains Mono</family>
                                       <pointsize>20</pointsize>
                                     </font>
                                   </property>
                                   <property name="focusPolicy">
                                     <enum>Qt::ClickFocus</enum>
                                   </property>
+                                  <property name="styleSheet">
+                                    <string notr="true">text-transform: uppercase;</string>
+                                  </property>
                                 </widget>
                               </item>
                             </layout>
                           </widget>
                         </item>
                         <item>
                           <widget class="QFrame" name="field4">
@@ -528,14 +540,17 @@
                                       <family>JetBrains Mono</family>
                                       <pointsize>20</pointsize>
                                     </font>
                                   </property>
                                   <property name="focusPolicy">
                                     <enum>Qt::ClickFocus</enum>
                                   </property>
+                                  <property name="styleSheet">
+                                    <string notr="true">text-transform: uppercase;</string>
+                                  </property>
                                 </widget>
                               </item>
                             </layout>
                           </widget>
                         </item>
                       </layout>
                     </item>
@@ -1012,22 +1027,23 @@
           <string>File</string>
         </property>
         <addaction name="actionNew_Database"/>
         <addaction name="actionOpen_Database"/>
         <addaction name="separator"/>
         <addaction name="actionNew_Contest"/>
         <addaction name="actionOpen_Contest"/>
+        <addaction name="actionEdit_Current_Contest"/>
         <addaction name="separator"/>
         <addaction name="actionGenerate_Cabrillo"/>
         <addaction name="actionGenerate_ADIF"/>
         <addaction name="separator"/>
-        <addaction name="actionConnection_Settings"/>
+        <addaction name="actionConfiguration_Settings"/>
         <addaction name="actionStationSettings"/>
-        <addaction name="actionQRZ_Settings"/>
         <addaction name="separator"/>
+        <addaction name="actionEdit_Macros"/>
       </widget>
       <widget class="QMenu" name="menuHelp">
         <property name="title">
           <string>Help</string>
         </property>
         <addaction name="actionAbout"/>
       </widget>
@@ -1040,36 +1056,52 @@
         <addaction name="actionDark_Mode"/>
       </widget>
       <widget class="QMenu" name="menuWindow">
         <property name="title">
           <string>Window</string>
         </property>
         <addaction name="actionLog_Window"/>
+        <addaction name="actionBandmap"/>
       </widget>
       <widget class="QMenu" name="menuOther">
         <property name="title">
           <string>Misc</string>
         </property>
         <addaction name="actionRecalculate_Mults"/>
       </widget>
       <addaction name="menuFile"/>
       <addaction name="menuView"/>
       <addaction name="menuWindow"/>
       <addaction name="menuOther"/>
       <addaction name="menuHelp"/>
     </widget>
     <action name="actionAbout">
+      <property name="enabled">
+        <bool>true</bool>
+      </property>
       <property name="text">
         <string>About</string>
       </property>
       <property name="font">
         <font>
           <family>JetBrains Mono</family>
         </font>
       </property>
+      <property name="autoRepeat">
+        <bool>false</bool>
+      </property>
+      <property name="visible">
+        <bool>true</bool>
+      </property>
+      <property name="iconVisibleInMenu">
+        <bool>false</bool>
+      </property>
+      <property name="shortcutVisibleInContextMenu">
+        <bool>false</bool>
+      </property>
     </action>
     <action name="actionCommand_Buttons">
       <property name="checkable">
         <bool>true</bool>
       </property>
       <property name="checked">
         <bool>true</bool>
@@ -1078,14 +1110,23 @@
         <string>Command Buttons</string>
       </property>
       <property name="font">
         <font>
           <family>JetBrains Mono</family>
         </font>
       </property>
+      <property name="autoRepeat">
+        <bool>false</bool>
+      </property>
+      <property name="iconVisibleInMenu">
+        <bool>false</bool>
+      </property>
+      <property name="shortcutVisibleInContextMenu">
+        <bool>false</bool>
+      </property>
     </action>
     <action name="actionCW_Macros">
       <property name="checkable">
         <bool>true</bool>
       </property>
       <property name="checked">
         <bool>true</bool>
@@ -1094,14 +1135,23 @@
         <string>CW Macros</string>
       </property>
       <property name="font">
         <font>
           <family>JetBrains Mono</family>
         </font>
       </property>
+      <property name="autoRepeat">
+        <bool>false</bool>
+      </property>
+      <property name="iconVisibleInMenu">
+        <bool>false</bool>
+      </property>
+      <property name="shortcutVisibleInContextMenu">
+        <bool>false</bool>
+      </property>
     </action>
     <action name="actionMode_and_Bands">
       <property name="checkable">
         <bool>true</bool>
       </property>
       <property name="checked">
         <bool>true</bool>
@@ -1126,82 +1176,258 @@
         <string>Force Dark Mode</string>
       </property>
       <property name="font">
         <font>
           <family>JetBrains Mono</family>
         </font>
       </property>
+      <property name="autoRepeat">
+        <bool>false</bool>
+      </property>
+      <property name="iconVisibleInMenu">
+        <bool>false</bool>
+      </property>
+      <property name="shortcutVisibleInContextMenu">
+        <bool>false</bool>
+      </property>
     </action>
     <action name="actionStationSettings">
       <property name="text">
         <string>Station Settings</string>
       </property>
       <property name="font">
         <font>
           <family>JetBrains Mono</family>
         </font>
       </property>
+      <property name="autoRepeat">
+        <bool>false</bool>
+      </property>
+      <property name="iconVisibleInMenu">
+        <bool>false</bool>
+      </property>
+      <property name="shortcutVisibleInContextMenu">
+        <bool>false</bool>
+      </property>
     </action>
     <action name="actionQRZ_Settings">
       <property name="text">
         <string>QRZ Settings</string>
       </property>
       <property name="font">
         <font>
           <family>JetBrains Mono</family>
         </font>
       </property>
     </action>
-    <action name="actionConnection_Settings">
+    <action name="actionConfiguration_Settings">
       <property name="text">
-        <string>Connection Settings</string>
+        <string>Configuration Settings</string>
       </property>
       <property name="font">
         <font>
           <family>JetBrains Mono</family>
         </font>
       </property>
+      <property name="autoRepeat">
+        <bool>false</bool>
+      </property>
+      <property name="iconVisibleInMenu">
+        <bool>false</bool>
+      </property>
+      <property name="shortcutVisibleInContextMenu">
+        <bool>false</bool>
+      </property>
     </action>
     <action name="actionGenerate_Cabrillo">
       <property name="text">
         <string>Generate Cabrillo</string>
       </property>
+      <property name="font">
+        <font>
+          <family>JetBrains Mono</family>
+        </font>
+      </property>
+      <property name="autoRepeat">
+        <bool>false</bool>
+      </property>
+      <property name="iconVisibleInMenu">
+        <bool>false</bool>
+      </property>
+      <property name="shortcutVisibleInContextMenu">
+        <bool>false</bool>
+      </property>
     </action>
     <action name="actionLog_Window">
       <property name="text">
         <string>Log Window</string>
       </property>
+      <property name="font">
+        <font>
+          <family>JetBrains Mono</family>
+        </font>
+      </property>
+      <property name="autoRepeat">
+        <bool>false</bool>
+      </property>
+      <property name="iconVisibleInMenu">
+        <bool>false</bool>
+      </property>
+      <property name="shortcutVisibleInContextMenu">
+        <bool>false</bool>
+      </property>
     </action>
     <action name="actionGenerate_ADIF">
       <property name="text">
         <string>Generate ADIF</string>
       </property>
+      <property name="font">
+        <font>
+          <family>JetBrains Mono</family>
+        </font>
+      </property>
+      <property name="shortcut">
+        <string/>
+      </property>
+      <property name="autoRepeat">
+        <bool>false</bool>
+      </property>
+      <property name="iconVisibleInMenu">
+        <bool>false</bool>
+      </property>
+      <property name="shortcutVisibleInContextMenu">
+        <bool>false</bool>
+      </property>
     </action>
     <action name="actionRecalculate_Mults">
       <property name="text">
         <string>Recalculate Mults</string>
       </property>
+      <property name="font">
+        <font>
+          <family>JetBrains Mono</family>
+        </font>
+      </property>
+      <property name="autoRepeat">
+        <bool>false</bool>
+      </property>
+      <property name="iconVisibleInMenu">
+        <bool>false</bool>
+      </property>
+      <property name="shortcutVisibleInContextMenu">
+        <bool>false</bool>
+      </property>
     </action>
     <action name="actionNew_Contest">
       <property name="text">
         <string>New Contest</string>
       </property>
+      <property name="font">
+        <font>
+          <family>JetBrains Mono</family>
+        </font>
+      </property>
+      <property name="autoRepeat">
+        <bool>false</bool>
+      </property>
+      <property name="iconVisibleInMenu">
+        <bool>false</bool>
+      </property>
+      <property name="shortcutVisibleInContextMenu">
+        <bool>false</bool>
+      </property>
     </action>
     <action name="actionNew_Database">
       <property name="text">
         <string>New Database</string>
       </property>
+      <property name="font">
+        <font>
+          <family>JetBrains Mono</family>
+        </font>
+      </property>
+      <property name="autoRepeat">
+        <bool>false</bool>
+      </property>
+      <property name="iconVisibleInMenu">
+        <bool>false</bool>
+      </property>
+      <property name="shortcutVisibleInContextMenu">
+        <bool>false</bool>
+      </property>
     </action>
     <action name="actionOpen_Database">
       <property name="text">
         <string>Open Database</string>
       </property>
+      <property name="font">
+        <font>
+          <family>JetBrains Mono</family>
+        </font>
+      </property>
+      <property name="autoRepeat">
+        <bool>false</bool>
+      </property>
+      <property name="iconVisibleInMenu">
+        <bool>false</bool>
+      </property>
+      <property name="shortcutVisibleInContextMenu">
+        <bool>false</bool>
+      </property>
     </action>
     <action name="actionOpen_Contest">
       <property name="text">
         <string>Open Contest</string>
       </property>
+      <property name="font">
+        <font>
+          <family>JetBrains Mono</family>
+        </font>
+      </property>
+      <property name="autoRepeat">
+        <bool>false</bool>
+      </property>
+      <property name="iconVisibleInMenu">
+        <bool>false</bool>
+      </property>
+      <property name="shortcutVisibleInContextMenu">
+        <bool>false</bool>
+      </property>
+    </action>
+    <action name="actionEdit_Macros">
+      <property name="text">
+        <string>Edit Macros</string>
+      </property>
+      <property name="font">
+        <font>
+          <family>JetBrains Mono</family>
+        </font>
+      </property>
+      <property name="autoRepeat">
+        <bool>false</bool>
+      </property>
+      <property name="iconVisibleInMenu">
+        <bool>false</bool>
+      </property>
+      <property name="shortcutVisibleInContextMenu">
+        <bool>false</bool>
+      </property>
+    </action>
+    <action name="actionEdit_Current_Contest">
+      <property name="text">
+        <string>Edit Current Contest</string>
+      </property>
+    </action>
+    <action name="actionBandmap">
+      <property name="text">
+        <string>Bandmap</string>
+      </property>
+      <property name="font">
+        <font>
+          <family>JetBrains Mono</family>
+        </font>
+      </property>
     </action>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `not1mm-23.4.6/not1mm/data/new_contest.ui` & `not1mm-23.5.1/not1mm/data/new_contest.ui`

 * *Files 6% similar despite different names*

#### Comparing `not1mm-23.4.6/not1mm/data/new_contest.ui` & `not1mm-23.5.1/not1mm/data/new_contest.ui`

```diff
@@ -63,15 +63,19 @@
             <property name="text">
               <string>NON-ASSISTED</string>
             </property>
           </item>
         </widget>
       </item>
       <item row="12" column="2" rowspan="2">
-        <widget class="QLineEdit" name="exchange"/>
+        <widget class="QLineEdit" name="exchange">
+          <property name="styleSheet">
+            <string notr="true">text-transform: uppercase;</string>
+          </property>
+        </widget>
       </item>
       <item row="7" column="2" colspan="2">
         <widget class="QComboBox" name="mode">
           <item>
             <property name="text">
               <string>CW</string>
             </property>
@@ -130,15 +134,15 @@
           </property>
           <property name="alignment">
             <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
           </property>
         </widget>
       </item>
       <item row="0" column="0" colspan="4">
-        <widget class="QLabel" name="label">
+        <widget class="QLabel" name="title">
           <property name="font">
             <font>
               <family>JetBrains Mono</family>
               <pointsize>14</pointsize>
               <bold>true</bold>
             </font>
           </property>
@@ -155,30 +159,55 @@
           <item>
             <property name="text">
               <string>General Logging</string>
             </property>
           </item>
           <item>
             <property name="text">
+              <string>10 10 SPRING CW</string>
+            </property>
+          </item>
+          <item>
+            <property name="text">
+              <string>ARRL DX CW</string>
+            </property>
+          </item>
+          <item>
+            <property name="text">
+              <string>ARRL DX SSB</string>
+            </property>
+          </item>
+          <item>
+            <property name="text">
               <string>ARRL Field Day</string>
             </property>
           </item>
           <item>
             <property name="text">
               <string>CQ WPX CW</string>
             </property>
           </item>
           <item>
             <property name="text">
-              <string>CQ WPX RTTY</string>
+              <string>CQ WPX SSB</string>
             </property>
           </item>
           <item>
             <property name="text">
-              <string>CQ WPX SSB</string>
+              <string>CQ WW CW</string>
+            </property>
+          </item>
+          <item>
+            <property name="text">
+              <string>CQ WW SSB</string>
+            </property>
+          </item>
+          <item>
+            <property name="text">
+              <string>CWT</string>
             </property>
           </item>
           <item>
             <property name="text">
               <string>JIDX CW</string>
             </property>
           </item>
@@ -551,15 +580,19 @@
             <property name="text">
               <string>ROOKIE</string>
             </property>
           </item>
         </widget>
       </item>
       <item row="14" column="2" colspan="2">
-        <widget class="QLineEdit" name="operators"/>
+        <widget class="QLineEdit" name="operators">
+          <property name="styleSheet">
+            <string notr="true">text-transform: uppercase;</string>
+          </property>
+        </widget>
       </item>
       <item row="4" column="0">
         <widget class="QLabel" name="label_4">
           <property name="text">
             <string>Operator</string>
           </property>
           <property name="alignment">
@@ -645,14 +678,29 @@
           <property name="orientation">
             <enum>Qt::Horizontal</enum>
           </property>
         </widget>
       </item>
     </layout>
   </widget>
+  <tabstops>
+    <tabstop>contest</tabstop>
+    <tabstop>dateTimeEdit</tabstop>
+    <tabstop>operator_class</tabstop>
+    <tabstop>band</tabstop>
+    <tabstop>power</tabstop>
+    <tabstop>mode</tabstop>
+    <tabstop>overlay</tabstop>
+    <tabstop>station</tabstop>
+    <tabstop>assisted</tabstop>
+    <tabstop>transmitter</tabstop>
+    <tabstop>exchange</tabstop>
+    <tabstop>operators</tabstop>
+    <tabstop>soapbox</tabstop>
+  </tabstops>
   <resources/>
   <connections>
     <connection>
       <sender>buttonBox</sender>
       <signal>accepted()</signal>
       <receiver>Dialog</receiver>
       <slot>accept()</slot>
```

### Comparing `not1mm-23.4.6/not1mm/data/opon.ui` & `not1mm-23.5.1/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/data/pickcontest.ui` & `not1mm-23.5.1/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/data/reddot.png` & `not1mm-23.5.1/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/data/settings.ui` & `not1mm-23.5.1/not1mm/data/settings.ui`

 * *Files 0% similar despite different names*

#### Comparing `not1mm-23.4.6/not1mm/data/settings.ui` & `not1mm-23.5.1/not1mm/data/settings.ui`

```diff
@@ -12,15 +12,15 @@
     </property>
     <property name="font">
       <font>
         <family>JetBrains Mono</family>
       </font>
     </property>
     <property name="windowTitle">
-      <string>Settings</string>
+      <string>Station Settings</string>
     </property>
     <layout class="QGridLayout" name="gridLayout" columnstretch="0,10,0,0,10,0,10">
       <item row="6" column="3">
         <widget class="QLabel" name="label_15">
           <property name="text">
             <string>State</string>
           </property>
```

### Comparing `not1mm-23.4.6/not1mm/lib/cat_interface.py` & `not1mm-23.5.1/not1mm/lib/cat_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -310,7 +310,76 @@
             try:
                 self.online = True
                 self.rigctrlsocket.send(rig_cmd)
                 _ = self.rigctrlsocket.recv(1024).decode().strip()
             except socket.error:
                 self.online = False
                 self.rigctrlsocket = None
+
+    def ptt_on(self):
+        """turn ptt on/off"""
+        if self.interface == "flrig":
+            return self.__ptt_on_flrig()
+        if self.interface == "rigctld":
+            return self.__ptt_on_rigctld()
+        return False
+
+    def __ptt_on_rigctld(self):
+        """Toggle PTT state on"""
+
+        # T, set_ptt 'PTT'
+        # Set 'PTT'.
+        # PTT is a value: ‘0’ (RX), ‘1’ (TX), ‘2’ (TX mic), or ‘3’ (TX data).
+
+        # t, get_ptt
+        # Get 'PTT' status.
+        # Returns PTT as a value in set_ptt above.
+
+        rig_cmd = bytes("T 1\n", "utf-8")
+        logger.debug("%s", f"{rig_cmd}")
+        try:
+            self.online = True
+            self.rigctrlsocket.send(rig_cmd)
+            _ = self.rigctrlsocket.recv(1024).decode().strip()
+        except socket.error:
+            self.online = False
+            self.rigctrlsocket = None
+
+    def __ptt_on_flrig(self):
+        """Toggle PTT state on"""
+        try:
+            self.online = True
+            return self.server.rig.set_ptt(1)
+        except ConnectionRefusedError as exception:
+            self.online = False
+            logger.debug("%s", exception)
+        return "0"
+
+    def ptt_off(self):
+        """turn ptt on/off"""
+        if self.interface == "flrig":
+            return self.__ptt_off_flrig()
+        if self.interface == "rigctld":
+            return self.__ptt_off_rigctld()
+        return False
+
+    def __ptt_off_rigctld(self):
+        """Toggle PTT state off"""
+        rig_cmd = bytes("T 0\n", "utf-8")
+        logger.debug("%s", f"{rig_cmd}")
+        try:
+            self.online = True
+            self.rigctrlsocket.send(rig_cmd)
+            _ = self.rigctrlsocket.recv(1024).decode().strip()
+        except socket.error:
+            self.online = False
+            self.rigctrlsocket = None
+
+    def __ptt_off_flrig(self):
+        """Toggle PTT state off"""
+        try:
+            self.online = True
+            return self.server.rig.set_ptt(0)
+        except ConnectionRefusedError as exception:
+            self.online = False
+            logger.debug("%s", exception)
+        return "0"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `not1mm-23.4.6/not1mm/lib/cwinterface.py` & `not1mm-23.5.1/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/lib/database.py` & `not1mm-23.5.1/not1mm/lib/database.py`

 * *Files 14% similar despite different names*

```diff
@@ -361,14 +361,30 @@
                 logger.info("%s", sql)
                 cur = conn.cursor()
                 cur.execute(sql, tuple(values))
                 conn.commit()
         except sqlite3.Error as exception:
             logger.info("DataBase add_contest: %s", exception)
 
+    def update_contest(self, contest: dict) -> None:
+        """Update an existing contest"""
+        pre = "UPDATE ContestInstance set "
+        for key in contest.keys():
+            pre += f"{key} = '{contest[key]}',"
+        sql = f"{pre[:-1]} where ContestNR='{contest['ContestNR']}';"
+
+        try:
+            with sqlite3.connect(self.database) as conn:
+                logger.info("%s\n%s", sql, contest)
+                cur = conn.cursor()
+                cur.execute(sql)
+                conn.commit()
+        except sqlite3.Error as exception:
+            logger.info("DataBase update_contest: %s", exception)
+
     def fetch_all_contests(self) -> list:
         """returns a list of dicts with contests in the database."""
         try:
             with sqlite3.connect(self.database) as conn:
                 conn.row_factory = self.row_factory
                 cursor = conn.cursor()
                 cursor.execute("select * from ContestInstance;")
@@ -481,14 +497,79 @@
                 cursor = conn.cursor()
                 cursor.execute(f"select * from dxlog where ID='{uuid}';")
                 return cursor.fetchone()
         except sqlite3.OperationalError as exception:
             logger.debug("%s", exception)
             return {}
 
+    def fetch_cqzn_exists(self, number) -> dict:
+        """returns a dict key of nr_count"""
+        try:
+            with sqlite3.connect(self.database) as conn:
+                conn.row_factory = self.row_factory
+                cursor = conn.cursor()
+                cursor.execute(
+                    f"select count(*) as zn_count from dxlog where ZN = '{number}' and ContestNR = {self.current_contest};"
+                )
+                return cursor.fetchone()
+        except sqlite3.OperationalError as exception:
+            logger.debug("%s", exception)
+            return {}
+
+    def fetch_zn_band_count(self) -> dict:
+        """
+        returns dict with count of unique NR.
+        {nr_count: count}
+        """
+        try:
+            with sqlite3.connect(self.database) as conn:
+                conn.row_factory = self.row_factory
+                cursor = conn.cursor()
+                cursor.execute(
+                    f"select count(DISTINCT(ZN || ':' || Band)) as zb_count from dxlog where ContestNR = {self.current_contest};"
+                )
+                return cursor.fetchone()
+        except sqlite3.OperationalError as exception:
+            logger.debug("%s", exception)
+            return {}
+
+    def fetch_country_band_count(self) -> dict:
+        """
+        returns dict with count of unique NR.
+        {nr_count: count}
+        """
+        try:
+            with sqlite3.connect(self.database) as conn:
+                conn.row_factory = self.row_factory
+                cursor = conn.cursor()
+                cursor.execute(
+                    f"select count(DISTINCT(CountryPrefix || ':' || Band)) as cb_count from dxlog where ContestNR = {self.current_contest};"
+                )
+                return cursor.fetchone()
+        except sqlite3.OperationalError as exception:
+            logger.debug("%s", exception)
+            return {}
+
+    def fetch_arrldx_country_band_count(self) -> dict:
+        """
+        returns dict with count of unique NR.
+        {nr_count: count}
+        """
+        try:
+            with sqlite3.connect(self.database) as conn:
+                conn.row_factory = self.row_factory
+                cursor = conn.cursor()
+                cursor.execute(
+                    f"select count(DISTINCT(CountryPrefix || ':' || Band)) as cb_count from dxlog where ContestNR = {self.current_contest} and points = 3;"
+                )
+                return cursor.fetchone()
+        except sqlite3.OperationalError as exception:
+            logger.debug("%s", exception)
+            return {}
+
     def fetch_nr_count(self) -> dict:
         """
         returns dict with count of unique NR.
         {nr_count: count}
         """
         try:
             with sqlite3.connect(self.database) as conn:
@@ -512,28 +593,59 @@
                     f"select count(*) as nr_count from dxlog where NR = '{number}' and ContestNR = {self.current_contest};"
                 )
                 return cursor.fetchone()
         except sqlite3.OperationalError as exception:
             logger.debug("%s", exception)
             return {}
 
+    def fetch_call_exists(self, call) -> dict:
+        """returns a dict key of nr_count"""
+        try:
+            with sqlite3.connect(self.database) as conn:
+                conn.row_factory = self.row_factory
+                cursor = conn.cursor()
+                cursor.execute(
+                    f"select count(*) as call_count from dxlog where Call = '{call}' and ContestNR = {self.current_contest};"
+                )
+                return cursor.fetchone()
+        except sqlite3.OperationalError as exception:
+            logger.debug("%s", exception)
+            return {}
+
     def fetch_nr_exists_before_me(self, number, time_stamp) -> dict:
         """returns a dict key of nr_count"""
         try:
             with sqlite3.connect(self.database) as conn:
                 conn.row_factory = self.row_factory
                 cursor = conn.cursor()
                 cursor.execute(
                     f"select count(*) as nr_count from dxlog where  TS < '{time_stamp}' and NR = '{number}' and ContestNR = {self.current_contest};"
                 )
                 return cursor.fetchone()
         except sqlite3.OperationalError as exception:
             logger.debug("%s", exception)
             return {}
 
+    def fetch_call_count(self) -> dict:
+        """
+        returns dict with count of unique calls.
+        {call_count: count}
+        """
+        try:
+            with sqlite3.connect(self.database) as conn:
+                conn.row_factory = self.row_factory
+                cursor = conn.cursor()
+                cursor.execute(
+                    f"select count(DISTINCT Call) as call_count from dxlog where ContestNR = {self.current_contest};"
+                )
+                return cursor.fetchone()
+        except sqlite3.OperationalError as exception:
+            logger.debug("%s", exception)
+            return {}
+
     def fetch_wpx_count(self) -> dict:
         """
         returns dict with count of unique WPXPrefix.
         {wpx_count: count}
         """
         try:
             with sqlite3.connect(self.database) as conn:
@@ -656,15 +768,15 @@
                 )
                 return cursor.fetchall()
         except sqlite3.OperationalError as exception:
             logger.debug("%s", exception)
             return ()
 
     def get_serial(self) -> dict:
-        """Return serial number"""
+        """Return next serial number"""
         try:
             with sqlite3.connect(self.database) as conn:
                 conn.row_factory = self.row_factory
                 cursor = conn.cursor()
                 cursor.execute(
                     f"select max(SentNR) + 1 as serial_nr from DXLOG where ContestNR = {self.current_contest};"
                 )
@@ -686,7 +798,31 @@
                 cursor.execute(
                     f"select DISTINCT band, mode, count(*) as mult from dxlog where ContestNR = {self.current_contest};"
                 )
                 return cursor.fetchone()
         except sqlite3.OperationalError as exception:
             logger.debug("%s", exception)
             return {}
+
+    def exec_sql(self, query: str) -> dict:
+        """Exec one off queries returning one dict"""
+        try:
+            with sqlite3.connect(self.database) as conn:
+                conn.row_factory = self.row_factory
+                cursor = conn.cursor()
+                cursor.execute(query)
+                return cursor.fetchone()
+        except sqlite3.OperationalError as exception:
+            logger.debug("%s", exception)
+            return {}
+
+    def exec_sql_mult(self, query: str) -> list:
+        """Exec one off queries returning list of dicts"""
+        try:
+            with sqlite3.connect(self.database) as conn:
+                conn.row_factory = self.row_factory
+                cursor = conn.cursor()
+                cursor.execute(query)
+                return cursor.fetchall()
+        except sqlite3.OperationalError as exception:
+            logger.debug("%s", exception)
+            return ()
```

### Comparing `not1mm-23.4.6/not1mm/lib/edit_macro.py` & `not1mm-23.5.1/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/lib/ham_utility.py` & `not1mm-23.5.1/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/lib/lookup.py` & `not1mm-23.5.1/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/lib/multicast.py` & `not1mm-23.5.1/not1mm/lib/multicast.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,15 @@
             socket.IPPROTO_IP, socket.IP_ADD_MEMBERSHIP, bytes(mreq)
         )
         self.server_udp.settimeout(0.01)
 
     def send_as_json(self, dict_object: dict):
         """Send dict as json encoded packet"""
         bytes_to_send = bytes(dumps(dict_object), encoding="ascii")
+        logger.debug("%s", f"{dict_object}")
         try:
             self.server_udp.sendto(
                 bytes_to_send,
                 (self.multicast_group, int(self.multicast_port)),
             )
         except OSError as err:
             logger.warning("%s", err)
```

### Comparing `not1mm-23.4.6/not1mm/lib/n1mm.py` & `not1mm-23.5.1/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/not1mm/logwindow.py` & `not1mm-23.5.1/not1mm/logwindow.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
 from not1mm.lib.database import DataBase
 from not1mm.lib.multicast import Multicast
 from not1mm.lib.edit_contact import EditContact
 
 # from not1mm.lib.n1mm import N1MM
 
+os.environ["QT_QPA_PLATFORMTHEME"] = "gnome"
+
 loader = pkgutil.get_loader("not1mm")
 WORKING_PATH = os.path.dirname(loader.get_filename())
 
 if "XDG_DATA_HOME" in os.environ:
     DATA_PATH = os.environ.get("XDG_DATA_HOME")
 else:
     DATA_PATH = str(Path.home() / ".local" / "share")
@@ -72,16 +74,16 @@
         self.database.current_contest = self.pref.get("contest", 0)
         self.contact = self.database.empty_contact
         data_path = WORKING_PATH + "/data/logwindow.ui"
         uic.loadUi(data_path, self)
         self.setWindowTitle(
             f"Log Display - {self.pref.get('current_database', 'ham.db')}"
         )
-        self.generalLog.setColumnCount(16)
-        self.focusedLog.setColumnCount(16)
+        self.generalLog.setColumnCount(19)
+        self.focusedLog.setColumnCount(19)
         icon_path = WORKING_PATH + "/data/"
         self.checkmark = QtGui.QPixmap(icon_path + "check.png")
         self.checkicon = QtGui.QIcon()
         self.checkicon.addPixmap(self.checkmark)
         self.generalLog.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
         self.generalLog.customContextMenuRequested.connect(self.edit_contact_selected)
         self.generalLog.setHorizontalHeaderItem(
@@ -97,36 +99,44 @@
 
         self.generalLog.setHorizontalHeaderItem(
             7, QtWidgets.QTableWidgetItem("Exchange1")
         )
         self.generalLog.setHorizontalHeaderItem(8, QtWidgets.QTableWidgetItem("Sect"))
 
         self.generalLog.setHorizontalHeaderItem(9, QtWidgets.QTableWidgetItem("WPX"))
-        self.generalLog.setHorizontalHeaderItem(10, QtWidgets.QTableWidgetItem("M1"))
-        self.generalLog.setHorizontalHeaderItem(11, QtWidgets.QTableWidgetItem("ZN"))
-        self.generalLog.setHorizontalHeaderItem(12, QtWidgets.QTableWidgetItem("M2"))
-        self.generalLog.setHorizontalHeaderItem(13, QtWidgets.QTableWidgetItem("PFX"))
-        self.generalLog.setHorizontalHeaderItem(14, QtWidgets.QTableWidgetItem("PTS"))
-        self.generalLog.setHorizontalHeaderItem(15, QtWidgets.QTableWidgetItem("UUID"))
+        self.generalLog.setHorizontalHeaderItem(10, QtWidgets.QTableWidgetItem("Power"))
+        self.generalLog.setHorizontalHeaderItem(11, QtWidgets.QTableWidgetItem("M1"))
+        self.generalLog.setHorizontalHeaderItem(12, QtWidgets.QTableWidgetItem("ZN"))
+        self.generalLog.setHorizontalHeaderItem(13, QtWidgets.QTableWidgetItem("M2"))
+        self.generalLog.setHorizontalHeaderItem(14, QtWidgets.QTableWidgetItem("PFX"))
+        self.generalLog.setHorizontalHeaderItem(15, QtWidgets.QTableWidgetItem("PTS"))
+        self.generalLog.setHorizontalHeaderItem(16, QtWidgets.QTableWidgetItem("Name"))
+        self.generalLog.setHorizontalHeaderItem(
+            17, QtWidgets.QTableWidgetItem("Comment")
+        )
+        self.generalLog.setHorizontalHeaderItem(18, QtWidgets.QTableWidgetItem("UUID"))
         self.generalLog.setColumnWidth(0, 200)
         self.generalLog.setColumnWidth(3, 50)
         self.generalLog.setColumnWidth(4, 50)
         self.generalLog.setColumnWidth(5, 75)
         self.generalLog.setColumnWidth(6, 75)
 
         self.generalLog.setColumnWidth(9, 50)
         self.generalLog.setColumnWidth(10, 50)
         self.generalLog.setColumnWidth(11, 50)
-        self.generalLog.setColumnWidth(14, 50)
+        self.generalLog.setColumnWidth(12, 50)
+        self.generalLog.setColumnWidth(15, 50)
+        self.generalLog.setColumnWidth(16, 75)
+        self.generalLog.setColumnWidth(17, 200)
         self.generalLog.cellDoubleClicked.connect(self.double_clicked)
         self.generalLog.cellChanged.connect(self.cell_changed)
         # self.generalLog.setColumnHidden(11, True)
         # self.generalLog.setColumnHidden(12, True)
         # self.generalLog.setColumnHidden(13, True)
-        self.generalLog.setColumnHidden(15, True)
+        self.generalLog.setColumnHidden(18, True)
 
         self.focusedLog.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
         self.focusedLog.customContextMenuRequested.connect(
             self.edit_focused_contact_selected
         )
         self.focusedLog.setHorizontalHeaderItem(
             0, QtWidgets.QTableWidgetItem("YYYY-MM-DD HH:MM:SS")
@@ -135,54 +145,64 @@
         self.focusedLog.setHorizontalHeaderItem(1, QtWidgets.QTableWidgetItem("Call"))
         self.focusedLog.setHorizontalHeaderItem(2, QtWidgets.QTableWidgetItem("Freq"))
         self.focusedLog.setHorizontalHeaderItem(3, QtWidgets.QTableWidgetItem("Snt"))
         self.focusedLog.setHorizontalHeaderItem(4, QtWidgets.QTableWidgetItem("Rcv"))
         self.focusedLog.setHorizontalHeaderItem(5, QtWidgets.QTableWidgetItem("SentNr"))
         self.focusedLog.setHorizontalHeaderItem(6, QtWidgets.QTableWidgetItem("RcvNr"))
 
-        self.generalLog.setHorizontalHeaderItem(
+        self.focusedLog.setHorizontalHeaderItem(
             7, QtWidgets.QTableWidgetItem("Exchange1")
         )
-        self.generalLog.setHorizontalHeaderItem(8, QtWidgets.QTableWidgetItem("Sect"))
+        self.focusedLog.setHorizontalHeaderItem(8, QtWidgets.QTableWidgetItem("Sect"))
 
         self.focusedLog.setHorizontalHeaderItem(9, QtWidgets.QTableWidgetItem("WPX"))
-        self.focusedLog.setHorizontalHeaderItem(10, QtWidgets.QTableWidgetItem("M1"))
-        self.focusedLog.setHorizontalHeaderItem(11, QtWidgets.QTableWidgetItem("ZN"))
-        self.focusedLog.setHorizontalHeaderItem(12, QtWidgets.QTableWidgetItem("M2"))
-        self.focusedLog.setHorizontalHeaderItem(13, QtWidgets.QTableWidgetItem("PFX"))
-        self.focusedLog.setHorizontalHeaderItem(14, QtWidgets.QTableWidgetItem("PTS"))
-        self.focusedLog.setHorizontalHeaderItem(15, QtWidgets.QTableWidgetItem("UUID"))
+        self.focusedLog.setHorizontalHeaderItem(10, QtWidgets.QTableWidgetItem("Power"))
+        self.focusedLog.setHorizontalHeaderItem(11, QtWidgets.QTableWidgetItem("M1"))
+        self.focusedLog.setHorizontalHeaderItem(12, QtWidgets.QTableWidgetItem("ZN"))
+        self.focusedLog.setHorizontalHeaderItem(13, QtWidgets.QTableWidgetItem("M2"))
+        self.focusedLog.setHorizontalHeaderItem(14, QtWidgets.QTableWidgetItem("PFX"))
+        self.focusedLog.setHorizontalHeaderItem(15, QtWidgets.QTableWidgetItem("PTS"))
+        self.focusedLog.setHorizontalHeaderItem(16, QtWidgets.QTableWidgetItem("Name"))
+        self.focusedLog.setHorizontalHeaderItem(
+            17, QtWidgets.QTableWidgetItem("Comment")
+        )
+        self.focusedLog.setHorizontalHeaderItem(18, QtWidgets.QTableWidgetItem("UUID"))
         self.focusedLog.setColumnWidth(0, 200)
         self.focusedLog.setColumnWidth(3, 50)
         self.focusedLog.setColumnWidth(4, 50)
         self.focusedLog.setColumnWidth(5, 75)
         self.focusedLog.setColumnWidth(6, 75)
 
         self.focusedLog.setColumnWidth(9, 50)
         self.focusedLog.setColumnWidth(10, 50)
         self.focusedLog.setColumnWidth(11, 50)
-        self.focusedLog.setColumnWidth(14, 50)
+        self.focusedLog.setColumnWidth(12, 50)
+        self.focusedLog.setColumnWidth(15, 50)
+        self.focusedLog.setColumnWidth(16, 75)
+        self.focusedLog.setColumnWidth(17, 200)
         # self.focusedLog.cellDoubleClicked.connect(self.double_clicked)
         # self.focusedLog.cellChanged.connect(self.cell_changed)
         # self.focusedLog.setColumnHidden(11, True)
         # self.focusedLog.setColumnHidden(12, True)
         # self.focusedLog.setColumnHidden(13, True)
-        self.focusedLog.setColumnHidden(15, True)
+        self.focusedLog.setColumnHidden(18, True)
         self.get_log()
         self.multicast_interface = Multicast(
             MULTICAST_GROUP, MULTICAST_PORT, INTERFACE_IP
         )
 
         if self._udpwatch is None:
             self._udpwatch = threading.Thread(
                 target=self.watch_udp,
                 daemon=True,
             )
             self._udpwatch.start()
-
+        cmd = {}
+        cmd["cmd"] = "GETCOLUMNS"
+        self.multicast_interface.send_as_json(cmd)
         # self.n1mm = N1MM(
         #     ip_address=self.preference.get("n1mm_ip"),
         #     radioport=self.preference.get("n1mm_radioport"),
         #     contactport=self.preference.get("n1mm_contactport"),
         # )
 
     def load_pref(self):
@@ -229,40 +249,43 @@
             "SNT": self.generalLog.item(row, 3).text(),
             "RCV": self.generalLog.item(row, 4).text(),
             "SentNr": self.generalLog.item(row, 5).text(),
             "NR": self.generalLog.item(row, 6).text(),
             "Exchange1": self.generalLog.item(row, 7).text(),
             "Sect": self.generalLog.item(row, 8).text(),
             "WPXPrefix": self.generalLog.item(row, 9).text(),
-            "IsMultiplier1": self.generalLog.item(row, 10).text(),
-            "ZN": self.generalLog.item(row, 11).text(),
-            "IsMultiplier2": self.generalLog.item(row, 12).text().upper(),
-            "CountryPrefix": self.generalLog.item(row, 13).text(),
-            "Points": self.generalLog.item(row, 14).text(),
-            "ID": self.generalLog.item(row, 15).text(),
+            "Power": self.generalLog.item(row, 10).text(),
+            "IsMultiplier1": self.generalLog.item(row, 11).text(),
+            "ZN": self.generalLog.item(row, 12).text(),
+            "IsMultiplier2": self.generalLog.item(row, 13).text().upper(),
+            "CountryPrefix": self.generalLog.item(row, 14).text(),
+            "Points": self.generalLog.item(row, 15).text(),
+            "Name": self.generalLog.item(row, 16).text(),
+            "Comment": self.generalLog.item(row, 17).text(),
+            "ID": self.generalLog.item(row, 18).text(),
         }
         self.database.change_contact(db_record)
         self.get_log()
         self.generalLog.scrollToItem(self.generalLog.item(row, column))
 
     def dummy(self):
         """the dummy"""
 
     def edit_focused_contact_selected(self, clicked_cell):
         """Show edit contact dialog"""
         logger.debug("Opening EditContact dialog")
         item = self.focusedLog.itemAt(clicked_cell)
-        uuid = self.focusedLog.item(item.row(), 15).text()
+        uuid = self.focusedLog.item(item.row(), 18).text()
         self.edit_contact(uuid)
 
     def edit_contact_selected(self, clicked_cell):
         """Show edit contact dialog"""
         logger.debug("Opening EditContact dialog")
         item = self.generalLog.itemAt(clicked_cell)
-        uuid = self.generalLog.item(item.row(), 15).text()
+        uuid = self.generalLog.item(item.row(), 18).text()
         self.edit_contact(uuid)
 
     def edit_contact(self, uuid):
         """Show edit contact dialog"""
         logger.debug("Edit: %s", uuid)
         self.edit_contact_dialog = EditContact(WORKING_PATH)
         self.edit_contact_dialog.accepted.connect(self.save_edited_contact)
@@ -369,31 +392,30 @@
         self.edit_contact_dialog.close()
         self.get_log()
         self.show_like_calls(self.contact.get("Call", ""))
 
     def get_log(self):
         """Get Log, Show it."""
 
-        """
-            The horizontal flags are:
+        # The horizontal flags are:
+
+        # Constant	Value	Description
+        # Qt::AlignLeft	0x0001	Aligns with the left edge.
+        # Qt::AlignRight	0x0002	Aligns with the right edge.
+        # Qt::AlignHCenter	0x0004	Centers horizontally in the available space.
+        # Qt::AlignJustify	0x0008	Justifies the text in the available space.
+
+        # The vertical flags are:
+
+        # Constant	Value	Description
+        # Qt::AlignTop	0x0020	Aligns with the top.
+        # Qt::AlignBottom	0x0040	Aligns with the bottom.
+        # Qt::AlignVCenter	0x0080	Centers vertically in the available space.
+        # Qt::AlignBaseline	0x0100	Aligns with the baseline.
 
-            Constant	Value	Description
-            Qt::AlignLeft	0x0001	Aligns with the left edge.
-            Qt::AlignRight	0x0002	Aligns with the right edge.
-            Qt::AlignHCenter	0x0004	Centers horizontally in the available space.
-            Qt::AlignJustify	0x0008	Justifies the text in the available space.
-            
-            The vertical flags are:
-
-            Constant	Value	Description
-            Qt::AlignTop	0x0020	Aligns with the top.
-            Qt::AlignBottom	0x0040	Aligns with the bottom.
-            Qt::AlignVCenter	0x0080	Centers vertically in the available space.
-            Qt::AlignBaseline	0x0100	Aligns with the baseline.
-        """
         self.generalLog.cellChanged.connect(self.dummy)
         self.table_loading = True
         current_log = self.database.fetch_all_contacts_asc()
         self.generalLog.setRowCount(0)
         for log_item in current_log:
             number_of_rows = self.generalLog.rowCount()
             self.generalLog.insertRow(number_of_rows)
@@ -445,48 +467,63 @@
                 QtWidgets.QTableWidgetItem(str(log_item.get("Sect", ""))),
             )
             self.generalLog.setItem(
                 number_of_rows,
                 9,
                 QtWidgets.QTableWidgetItem(str(log_item.get("WPXPrefix", ""))),
             )
+            self.generalLog.setItem(
+                number_of_rows,
+                10,
+                QtWidgets.QTableWidgetItem(str(log_item.get("Power", ""))),
+            )
             item = QtWidgets.QTableWidgetItem()
             if log_item.get("IsMultiplier1", False):
                 item.setIcon(self.checkicon)
             self.generalLog.setItem(
                 number_of_rows,
-                10,
+                11,
                 item,
             )
             self.generalLog.setItem(
                 number_of_rows,
-                11,
+                12,
                 QtWidgets.QTableWidgetItem(str(log_item.get("ZN", ""))),
             )
             item = QtWidgets.QTableWidgetItem()
             if log_item.get("IsMultiplier2", False):
                 item.setIcon(self.checkicon)
             self.generalLog.setItem(
                 number_of_rows,
-                12,
+                13,
                 item,
             )
             self.generalLog.setItem(
                 number_of_rows,
-                13,
+                14,
                 QtWidgets.QTableWidgetItem(str(log_item.get("CountryPrefix", ""))),
             )
             self.generalLog.setItem(
                 number_of_rows,
-                14,
+                15,
                 QtWidgets.QTableWidgetItem(str(log_item.get("Points", ""))),
             )
             self.generalLog.setItem(
                 number_of_rows,
-                15,
+                16,
+                QtWidgets.QTableWidgetItem(str(log_item.get("Name", ""))),
+            )
+            self.generalLog.setItem(
+                number_of_rows,
+                17,
+                QtWidgets.QTableWidgetItem(str(log_item.get("Comment", ""))),
+            )
+            self.generalLog.setItem(
+                number_of_rows,
+                18,
                 QtWidgets.QTableWidgetItem(str(log_item.get("ID", ""))),
             )
         self.table_loading = False
         self.generalLog.cellChanged.connect(self.cell_changed)
 
     # def testing(self, a):
     #     """ignore"""
@@ -561,51 +598,75 @@
                 number_of_rows,
                 6,
                 QtWidgets.QTableWidgetItem(str(log_item.get("NR", ""))),
             )
             self.focusedLog.setItem(
                 number_of_rows,
                 7,
+                QtWidgets.QTableWidgetItem(str(log_item.get("Exchange1", ""))),
+            )
+            self.focusedLog.setItem(
+                number_of_rows,
+                8,
+                QtWidgets.QTableWidgetItem(str(log_item.get("Sect", ""))),
+            )
+            self.focusedLog.setItem(
+                number_of_rows,
+                9,
                 QtWidgets.QTableWidgetItem(str(log_item.get("WPXPrefix", ""))),
             )
-
+            self.focusedLog.setItem(
+                number_of_rows,
+                10,
+                QtWidgets.QTableWidgetItem(str(log_item.get("Power", ""))),
+            )
             item = QtWidgets.QTableWidgetItem()
             if log_item.get("IsMultiplier1", False):
                 item.setIcon(self.checkicon)
             self.focusedLog.setItem(
                 number_of_rows,
-                8,
+                11,
                 item,
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                9,
+                12,
                 QtWidgets.QTableWidgetItem(str(log_item.get("ZN", ""))),
             )
             item = QtWidgets.QTableWidgetItem()
             if log_item.get("IsMultiplier2", False):
                 item.setIcon(self.checkicon)
             self.focusedLog.setItem(
                 number_of_rows,
-                10,
+                13,
                 item,
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                11,
+                14,
                 QtWidgets.QTableWidgetItem(str(log_item.get("CountryPrefix", ""))),
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                12,
+                15,
                 QtWidgets.QTableWidgetItem(str(log_item.get("Points", ""))),
             )
             self.focusedLog.setItem(
                 number_of_rows,
-                13,
+                16,
+                QtWidgets.QTableWidgetItem(str(log_item.get("Name", ""))),
+            )
+            self.focusedLog.setItem(
+                number_of_rows,
+                17,
+                QtWidgets.QTableWidgetItem(str(log_item.get("Comment", ""))),
+            )
+            self.focusedLog.setItem(
+                number_of_rows,
+                18,
                 QtWidgets.QTableWidgetItem(str(log_item.get("ID", ""))),
             )
 
     def check_udp_traffic(self):
         """Checks UDP Traffic"""
         while not self.udp_fifo.empty():
             datagram = self.udp_fifo.get()
@@ -625,14 +686,23 @@
                 logger.debug("External refresh command.")
                 self.get_log()
             if json_data.get("cmd", "") == "CALLCHANGED":
                 call = json_data.get("call", "")
                 self.show_like_calls(call)
             if json_data.get("cmd", "") == "NEWDB":
                 self.load_new_db()
+            if json_data.get("cmd", "") == "SHOWCOLUMNS":
+                columns_to_show = json_data.get("COLUMNS", [])
+                for column in range(18):
+                    if column in columns_to_show:
+                        self.generalLog.setColumnHidden(column, False)
+                        self.focusedLog.setColumnHidden(column, False)
+                    else:
+                        self.generalLog.setColumnHidden(column, True)
+                        self.focusedLog.setColumnHidden(column, True)
 
 
 def load_fonts_from_dir(directory: str) -> set:
     """
     Well it loads fonts from a directory...
     """
     font_families = set()
```

### Comparing `not1mm-23.4.6/not1mm/plugins/arrl_dx_cw.py` & `not1mm-23.5.1/not1mm/plugins/arrl_rtty_ru.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """ARRL plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 from PyQt5 import QtWidgets
 
-name = "ARRL DX CW"
+name = "ARRL RTTY Round Up"
 mode = "BOTH"  # CW SSB BOTH RTTY
+columns = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 4
 
 
 def init_contest(self):
     """setup plugin"""
@@ -56,14 +57,18 @@
     }
 
 
 def set_contact_vars(self):
     """Contest Specific"""
 
 
+def predupe(self):
+    """called after callsign entered"""
+
+
 def prefill(self):
     """Fill SentNR"""
 
 
 def points(self):
     """Calc point"""
```

### Comparing `not1mm-23.4.6/not1mm/plugins/arrl_dx_phone.py` & `not1mm-23.5.1/not1mm/plugins/arrl_ss_cw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """ARRL plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 from PyQt5 import QtWidgets
 
-name = "ARRL DX Phone"
+name = "ARRL Sweepstakes CW"
 mode = "BOTH"  # CW SSB BOTH RTTY
+columns = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 4
 
 
 def init_contest(self):
     """setup plugin"""
@@ -56,14 +57,18 @@
     }
 
 
 def set_contact_vars(self):
     """Contest Specific"""
 
 
+def predupe(self):
+    """called after callsign entered"""
+
+
 def prefill(self):
     """Fill SentNR"""
 
 
 def points(self):
     """Calc point"""
```

### Comparing `not1mm-23.4.6/not1mm/plugins/arrl_field_day.py` & `not1mm-23.5.1/not1mm/plugins/arrl_field_day.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
 name = "ARRL Field Day"
 mode = "BOTH"  # CW SSB BOTH RTTY
 cabrillo_name = "ARRL-FD"
+columns = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 3
 
 
 def init_contest(self):
     """setup plugin"""
@@ -73,14 +74,18 @@
     """Contest Specific"""
     self.contact["SNT"] = self.sent.text()
     self.contact["RCV"] = self.receive.text()
     self.contact["Exchange1"] = self.other_1.text().upper()
     self.contact["Sect"] = self.other_2.text().upper()
 
 
+def predupe(self):
+    """called after callsign entered"""
+
+
 def prefill(self):
     """Fill SentNR"""
 
 
 def points(self):
     """Calc point"""
     _mode = self.contact.get("Mode", "")
```

### Comparing `not1mm-23.4.6/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-23.5.1/not1mm/plugins/arrl_ss_phone.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """ARRL plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 from PyQt5 import QtWidgets
 
-name = "ARRL RTTY Round Up"
+name = "ARRL Sweepstakes Phone"
 mode = "BOTH"  # CW SSB BOTH RTTY
+columns = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 4
 
 
 def init_contest(self):
     """setup plugin"""
@@ -56,14 +57,18 @@
     }
 
 
 def set_contact_vars(self):
     """Contest Specific"""
 
 
+def predupe(self):
+    """called after callsign entered"""
+
+
 def prefill(self):
     """Fill SentNR"""
 
 
 def points(self):
     """Calc point"""
```

### Comparing `not1mm-23.4.6/not1mm/plugins/arrl_ss_cw.py` & `not1mm-23.5.1/not1mm/plugins/winter_field_day.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-"""ARRL plugin"""
+"""Winter Field Day plugin"""
 
 # pylint: disable=invalid-name, unused-argument, unused-variable
 
 from PyQt5 import QtWidgets
 
-name = "ARRL Sweepstakes CW"
-mode = "BOTH"  # CW SSB BOTH RTTY
-
+name = "Winter Field Day"
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
+mode = "BOTH"  # CW SSB BOTH RTTY
+columns = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]
 dupe_type = 4
 
 
 def init_contest(self):
     """setup plugin"""
     set_tab_next(self)
     set_tab_prev(self)
     interface(self)
 
 
 def interface(self):
     """Setup user interface"""
+    self.field1.hide()
+    self.field2.hide()
+    self.field3.show()
+    self.field4.show()
+    label = self.field3.findChild(QtWidgets.QLabel)
+    label.setText("Class")
+    label = self.field4.findChild(QtWidgets.QLabel)
+    label.setText("Section")
 
 
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
@@ -56,14 +64,18 @@
     }
 
 
 def set_contact_vars(self):
     """Contest Specific"""
 
 
+def predupe(self):
+    """called after callsign entered"""
+
+
 def prefill(self):
     """Fill SentNR"""
 
 
 def points(self):
     """Calc point"""
```

### Comparing `not1mm-23.4.6/not1mm/plugins/cq_wpx_cw.py` & `not1mm-23.5.1/not1mm/plugins/cq_wpx_cw.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
 name = "CQ WPX CW"
 cabrillo_name = "CQ-WPX-CW"
 mode = "CW"  # CW SSB BOTH RTTY
+columns = [0, 1, 2, 3, 4, 5, 6, 9, 11, 15]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 2
 
 
 def init_contest(self):
     """setup plugin"""
@@ -82,14 +83,18 @@
         result = self.database.fetch_wpx_exists(self.contact.get("WPXPrefix", ""))
         if result.get("wpx_count"):
             self.contact["IsMultiplier1"] = 0
         else:
             self.contact["IsMultiplier1"] = 1
 
 
+def predupe(self):
+    """called after callsign entered"""
+
+
 def prefill(self):
     """Fill SentNR"""
     result = self.database.get_serial()
     serial_nr = str(result.get("serial_nr", "1"))
     if serial_nr == "None":
         serial_nr = "1"
     field = self.field3.findChild(QtWidgets.QLineEdit)
```

### Comparing `not1mm-23.4.6/not1mm/plugins/cq_wpx_rtty.py` & `not1mm-23.5.1/not1mm/plugins/cq_wpx_ssb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-"""CQ WPX RTTY plugin"""
+"""CQ WPX SSB plugin"""
 
 # pylint: disable=invalid-name
 import logging
 from pathlib import Path
 
 from PyQt5 import QtWidgets
 
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
-name = "CQ WPX RTTY"
-cabrillo_name = "CQ-WPX-RTTY"
-mode = "RTTY"  # CW SSB BOTH RTTY
+name = "CQ WPX SSB"
+cabrillo_name = "CQ-WPX-SSB"
+mode = "SSB"  # CW SSB BOTH RTTY
+columns = [0, 1, 2, 3, 4, 5, 6, 9, 11, 15]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 2
 
 
 def init_contest(self):
     """setup plugin"""
@@ -82,14 +83,18 @@
         result = self.database.fetch_wpx_exists(self.contact.get("WPXPrefix", ""))
         if result.get("wpx_count"):
             self.contact["IsMultiplier1"] = 0
         else:
             self.contact["IsMultiplier1"] = 1
 
 
+def predupe(self):
+    """called after callsign entered"""
+
+
 def prefill(self):
     """Fill SentNR"""
     result = self.database.get_serial()
     serial_nr = str(result.get("serial_nr", "1"))
     if serial_nr == "None":
         serial_nr = "1"
     field = self.field3.findChild(QtWidgets.QLineEdit)
```

### Comparing `not1mm-23.4.6/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-23.5.1/not1mm/plugins/arrl_dx_cw.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-"""CQ WPX SSB plugin"""
+"""ARRL plugin"""
+
+# pylint: disable=invalid-name, unused-argument, unused-variable
 
-# pylint: disable=invalid-name
 import logging
 from pathlib import Path
 
 from PyQt5 import QtWidgets
-
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
-name = "CQ WPX SSB"
-cabrillo_name = "CQ-WPX-SSB"
-mode = "SSB"  # CW SSB BOTH RTTY
+name = "ARRL DX CW"
+cabrillo_name = "ARRL-DX-CW"
+mode = "CW"  # CW SSB BOTH RTTY
+columns = [0, 1, 2, 3, 4, 10, 11, 14, 15]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 2
 
 
 def init_contest(self):
     """setup plugin"""
@@ -26,35 +27,31 @@
     self.next_field = self.other_2
 
 
 def interface(self):
     """Setup user interface"""
     self.field1.show()
     self.field2.show()
-    self.field3.show()
+    self.field3.hide()
     self.field4.show()
-    label = self.field3.findChild(QtWidgets.QLabel)
-    label.setText("SentNR")
     label = self.field4.findChild(QtWidgets.QLabel)
-    label.setText("RcvNR")
+    label.setText("Power")
 
 
 def set_tab_next(self):
     """Set TAB Advances"""
     self.tab_next = {
         self.callsign: self.field1.findChild(QtWidgets.QLineEdit),
         self.field1.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
-        self.field2.findChild(QtWidgets.QLineEdit): self.field3.findChild(
-            QtWidgets.QLineEdit
-        ),
-        self.field3.findChild(QtWidgets.QLineEdit): self.field4.findChild(
+        self.field2.findChild(QtWidgets.QLineEdit): self.field4.findChild(
             QtWidgets.QLineEdit
         ),
+        self.field3.findChild(QtWidgets.QLineEdit): self.callsign,
         self.field4.findChild(QtWidgets.QLineEdit): self.callsign,
     }
 
 
 def set_tab_prev(self):
     """Set TAB Advances"""
     self.tab_prev = {
@@ -62,79 +59,67 @@
         self.field1.findChild(QtWidgets.QLineEdit): self.callsign,
         self.field2.findChild(QtWidgets.QLineEdit): self.field1.findChild(
             QtWidgets.QLineEdit
         ),
         self.field3.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
-        self.field4.findChild(QtWidgets.QLineEdit): self.field3.findChild(
+        self.field4.findChild(QtWidgets.QLineEdit): self.field2.findChild(
             QtWidgets.QLineEdit
         ),
     }
 
 
 def set_contact_vars(self):
     """Contest Specific"""
     self.contact["SNT"] = self.sent.text()
     self.contact["RCV"] = self.receive.text()
-    self.contact["SentNr"] = self.other_1.text()
-    self.contact["NR"] = self.other_2.text()
-    if self.contact.get("WPXPrefix"):
-        result = self.database.fetch_wpx_exists(self.contact.get("WPXPrefix", ""))
-        if result.get("wpx_count"):
-            self.contact["IsMultiplier1"] = 0
-        else:
-            self.contact["IsMultiplier1"] = 1
+    self.contact["Power"] = self.other_2.text().upper()
+    self.contact["NR"] = self.other_2.text().upper()
+    self.contact["SentNr"] = self.contest_settings.get("SentExchange", 0)
+
+
+def predupe(self):
+    """called after callsign entered"""
 
 
 def prefill(self):
-    """Fill SentNR"""
-    result = self.database.get_serial()
-    serial_nr = str(result.get("serial_nr", "1"))
-    if serial_nr == "None":
-        serial_nr = "1"
-    field = self.field3.findChild(QtWidgets.QLineEdit)
-    if len(field.text()) == 0:
-        field.setText(serial_nr)
+    """Fill sentnr"""
+    # if len(self.other_2.text()) == 0:
+    #     self.other_2.setText(str(self.contact.get("ZN", "")))
+    self.other_1.setText(str(self.contest_settings.get("SentExchange", 0)))
 
 
 def points(self):
     """Calc point"""
     result = self.cty_lookup(self.station.get("Call", ""))
     if result:
         for item in result.items():
             mycountry = item[1].get("entity", "")
-            mycontinent = item[1].get("continent", "")
+            # mycontinent = item[1].get("continent", "")
     result = self.cty_lookup(self.contact.get("Call", ""))
-    band = int(int(float(self.contact.get("Freq"))) / 1000)
     if result:
         for item in result.items():
             entity = item[1].get("entity", "")
-            continent = item[1].get("continent", "")
-            if mycountry.upper() == entity.upper():
-                return 1
-            if mycontinent and continent == "NA":
-                if band in [28, 21, 14]:
-                    return 2
-                return 4
-            if mycontinent == continent:
-                if band in [28, 21, 14]:
-                    return 1
-                return 2
-            if band in [28, 21, 14]:
+            # continent = item[1].get("continent", "")
+            if mycountry in ["K", "VE"]:
+                if entity in ["K", "VE"]:
+                    return 0
                 return 3
-            return 6
+            if entity in ["K", "VE"]:
+                return 3
+            return 0
     return 0
 
 
 def show_mults(self):
     """Return display string for mults"""
-    result = self.database.fetch_wpx_count()
+    result = self.database.fetch_arrldx_country_band_count()
     if result:
-        return int(result.get("wpx_count", 0))
+        return int(result.get("cb_count", 0))
     return 0
 
 
 def show_qso(self):
     """Return qso count"""
     result = self.database.fetch_qso_count()
     if result:
@@ -154,16 +139,15 @@
     """Return calculated score"""
     result = self.database.fetch_points()
     if result is not None:
         score = result.get("Points", "0")
         if score is None:
             score = "0"
         contest_points = int(score)
-        result = self.database.fetch_wpx_count()
-        mults = int(result.get("wpx_count", 0))
+        mults = show_mults(self)
         return contest_points * mults
     return 0
 
 
 def adif(self):
     """
     Creates an ADIF file of the contacts made.
@@ -182,16 +166,16 @@
                 hiscall = contact.get("Call", "")
                 the_date_and_time = contact.get("TS")
                 # band = contact.get("Band")
                 themode = contact.get("Mode")
                 frequency = str(contact.get("Freq", 0) / 1000)
                 sentrst = contact.get("SNT", "")
                 rcvrst = contact.get("RCV", "")
-                sentnr = str(contact.get("SentNr", "59"))
-                rcvnr = str(contact.get("NR", "59"))
+                sentnr = str(contact.get("SentNr", ""))
+                rcvnr = str(contact.get("NR", ""))
                 grid = contact.get("GridSquare", "")
                 comment = contact.get("ContestName", "")
                 loggeddate = the_date_and_time[:10]
                 loggedtime = the_date_and_time[11:13] + the_date_and_time[14:16]
                 print(
                     f"<QSO_DATE:{len(''.join(loggeddate.split('-')))}:d>"
                     f"{''.join(loggeddate.split('-'))}",
@@ -353,15 +337,15 @@
 
             print(
                 f"CLAIMED-SCORE: {calc_score(self)}",
                 end="\r\n",
                 file=file_descriptor,
             )
             print(
-                "OPERATORS: ",
+                f"OPERATORS: {self.contest_settings.get('Operators','')}",
                 end="\r\n",
                 file=file_descriptor,
             )
             print(
                 f"NAME: {self.station.get('Name', '')}",
                 end="\r\n",
                 file=file_descriptor,
@@ -420,18 +404,24 @@
     except IOError as exception:
         logger.critical("cabrillo: IO error: %s, writing to %s", exception, filename)
         return
 
 
 def recalculate_mults(self):
     """Recalculates multipliers after change in logged qso."""
+
     all_contacts = self.database.fetch_all_contacts_asc()
     for contact in all_contacts:
         time_stamp = contact.get("TS")
-        wpx = contact.get("WPXPrefix")
-        result = self.database.fetch_wpx_exists_before_me(wpx, time_stamp)
-        wpx_count = result.get("wpx_count", 1)
-        if wpx_count == 0:
+        entity = contact.get("CountryPrefix")
+        query = (
+            f"select count(*) as prefix_count from dxlog where  TS < '{time_stamp}' "
+            f"and CountryPrefix = '{entity}' "
+            f"and ContestNR = {self.pref.get('contest', '1')};"
+        )
+        result = self.database.exec_sql(query)
+        count = result.get("prefix_count", 1)
+        if count == 0 and contact.get("Points", 0) == 3:
             contact["IsMultiplier1"] = 1
         else:
             contact["IsMultiplier1"] = 0
         self.database.change_contact(contact)
```

### Comparing `not1mm-23.4.6/not1mm/plugins/general_logging.py` & `not1mm-23.5.1/not1mm/plugins/general_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
 name = "General Logging"
 cabrillo_name = "General-Logging"
 mode = "BOTH"  # CW SSB BOTH RTTY
+columns = [0, 1, 2, 3, 4, 16, 17]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 4
 
 
 def init_contest(self):
     """setup plugin"""
@@ -76,14 +77,18 @@
     """Contest Specific"""
     self.contact["SNT"] = self.sent.text()
     self.contact["RCV"] = self.receive.text()
     self.contact["Name"] = self.other_1.text()
     self.contact["Comment"] = self.other_2.text()
 
 
+def predupe(self):
+    """called after callsign entered"""
+
+
 def prefill(self):
     """Fill SentNR"""
 
 
 def points(self):
     """Calc point"""
```

### Comparing `not1mm-23.4.6/not1mm/plugins/jidx_cw.py` & `not1mm-23.5.1/not1mm/plugins/jidx_cw.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
 name = "JIDX CW"
 cabrillo_name = "JIDX-CW"
 mode = "CW"  # CW SSB BOTH RTTY
+columns = [0, 1, 2, 3, 4, 5, 6, 11, 15]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 2
 
 
 def init_contest(self):
     """setup plugin"""
@@ -82,14 +83,18 @@
         result = self.database.fetch_nr_exists(self.contact.get("NR", ""))
         if result.get("nr_count"):
             self.contact["IsMultiplier1"] = 0
         else:
             self.contact["IsMultiplier1"] = 1
 
 
+def predupe(self):
+    """called after callsign entered"""
+
+
 def prefill(self):
     """Fill SentNR"""
     SentExchange = self.contest_settings.get("SentExchange", "")
     if "#" in SentExchange:
         result = self.database.get_serial()
         serial_nr = str(result.get("serial_nr", "1"))
         if serial_nr == "None":
```

### Comparing `not1mm-23.4.6/not1mm/plugins/jidx_ph.py` & `not1mm-23.5.1/not1mm/plugins/jidx_ph.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from not1mm.lib.version import __version__
 
 logger = logging.getLogger("__main__")
 
 name = "JIDX PH"
 cabrillo_name = "JIDX-PH"
 mode = "SSB"  # CW SSB BOTH RTTY
+columns = [0, 1, 2, 3, 4, 5, 6, 11, 15]
 
 # 1 once per contest, 2 work each band, 3 each band/mode, 4 no dupe checking
 dupe_type = 2
 
 
 def init_contest(self):
     """setup plugin"""
@@ -82,14 +83,18 @@
         result = self.database.fetch_nr_exists(self.contact.get("NR", ""))
         if result.get("nr_count"):
             self.contact["IsMultiplier1"] = 0
         else:
             self.contact["IsMultiplier1"] = 1
 
 
+def predupe(self):
+    """called after callsign entered"""
+
+
 def prefill(self):
     """Fill SentNR"""
     SentExchange = self.contest_settings.get("SentExchange", "")
     if "#" in SentExchange:
         result = self.database.get_serial()
         serial_nr = str(result.get("serial_nr", "1"))
         if serial_nr == "None":
```

### Comparing `not1mm-23.4.6/not1mm/testing/test.py` & `not1mm-23.5.1/not1mm/testing/test.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.4.6/pyproject.toml` & `not1mm-23.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "23.4.6"
+version = "23.5.1"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
     "PyQt5",
     "requests",
     "dicttoxml",
     "xmltodict",
     "psutil",
+    "sounddevice",
+    "soundfile",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
-    "Development Status :: 1 - Planning",
+    "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Environment :: X11 Applications :: Qt",
     "Operating System :: POSIX :: Linux",
     "Intended Audience :: End Users/Desktop",
     "Natural Language :: English",
     "Topic :: Communications :: Ham Radio",
 ]
@@ -34,11 +36,12 @@
 "Bug Tracker" = "https://github.com/mbridak/not1mm/issues"
 
 [tool.setuptools.packages.find]
 where = ["."]
 
 [tool.setuptools.package-data]
 "not1mm.data" = ["*.json", "*.txt", "*.SCP", "*.ui", "*.ttf", "*.desktop", "*.png", "*.qss", "*.sql",]
+"not1mm.data.phonetics" = ["*.wav",]
 "not1mm.icon" = ["*.png",]
 
 [project.scripts]
 not1mm = "not1mm.__main__:run"
```

### Comparing `not1mm-23.4.6/testing/test.py` & `not1mm-23.5.1/testing/test.py`

 * *Files identical despite different names*

