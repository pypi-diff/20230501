# Comparing `tmp/not1mm-23.5.1.tar.gz` & `tmp/not1mm-23.5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-23.5.1.tar", last modified: Mon May  1 16:46:02 2023, max compression
+gzip compressed data, was "not1mm-23.5.1.1.tar", last modified: Mon May  1 21:18:17 2023, max compression
```

## Comparing `not1mm-23.5.1.tar` & `not1mm-23.5.1.1.tar`

### file list

```diff
@@ -1,135 +1,138 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.847775 not1mm-23.5.1/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.1/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20878 2023-05-01 16:46:02.847775 not1mm-23.5.1/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20133 2023-05-01 16:41:22.000000 not1mm-23.5.1/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.819775 not1mm-23.5.1/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.1/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    77026 2023-05-01 14:18:20.000000 not1mm-23.5.1/not1mm/__main__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    18617 2023-04-30 04:11:31.000000 not1mm-23.5.1/not1mm/bandmap.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.830775 not1mm-23.5.1/not1mm/data/
--rw-rw-rw-   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.1/not1mm/data/Combinear.qss
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.1/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.1/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.1/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.1/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.1/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.1/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    31458 2023-04-24 19:59:20.000000 not1mm-23.5.1/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.1/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.1/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.1/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.1/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.1/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.1/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.1/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.1/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.1/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.1/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.1/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43658 2023-05-01 15:38:56.000000 not1mm-23.5.1/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17405 2023-05-01 15:15:03.000000 not1mm-23.5.1/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.1/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.840775 not1mm-23.5.1/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.1/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.1/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.1/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.1/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.1/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.1/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.1/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.1/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.1/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.1/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.1/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.1/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.1/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.1/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.1/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.1/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.1/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.1/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.1/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.1/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.1/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.1/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.1/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.1/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.1/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.1/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.1/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.1/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.1/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.1/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.1/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.1/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.1/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.1/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.1/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.1/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.1/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.1/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.1/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.1/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.1/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.1/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.1/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.1/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.1/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.1/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.1/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.1/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.1/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.1/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.1/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.1/not1mm/data/ssbmacros.txt
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.843775 not1mm-23.5.1/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.1/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.1/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12468 2023-04-25 15:08:00.000000 not1mm-23.5.1/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.1/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32966 2023-04-24 03:05:48.000000 not1mm-23.5.1/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.1/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.1/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.1/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.1/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.1/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.1/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.1/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.1/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.1/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.1/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5414 2023-04-21 15:02:17.000000 not1mm-23.5.1/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-05-01 16:43:25.000000 not1mm-23.5.1/not1mm/lib/version.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    31120 2023-04-29 16:10:36.000000 not1mm-23.5.1/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.846775 not1mm-23.5.1/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13558 2023-05-01 16:14:59.000000 not1mm-23.5.1/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.1/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14348 2023-04-24 14:53:10.000000 not1mm-23.5.1/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14351 2023-04-24 14:53:19.000000 not1mm-23.5.1/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12719 2023-04-24 14:53:32.000000 not1mm-23.5.1/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2590 2023-04-24 14:53:43.000000 not1mm-23.5.1/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2591 2023-04-24 14:53:53.000000 not1mm-23.5.1/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2594 2023-04-24 14:54:04.000000 not1mm-23.5.1/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14755 2023-04-24 14:54:20.000000 not1mm-23.5.1/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14759 2023-04-24 14:54:36.000000 not1mm-23.5.1/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13701 2023-04-24 14:54:47.000000 not1mm-23.5.1/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13772 2023-04-24 14:54:56.000000 not1mm-23.5.1/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14624 2023-04-24 14:52:00.000000 not1mm-23.5.1/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7272 2023-04-24 14:55:06.000000 not1mm-23.5.1/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13650 2023-04-24 14:55:15.000000 not1mm-23.5.1/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13651 2023-04-24 14:55:25.000000 not1mm-23.5.1/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2851 2023-04-24 14:55:37.000000 not1mm-23.5.1/not1mm/plugins/winter_field_day.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.846775 not1mm-23.5.1/not1mm/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2297 2023-03-29 19:50:12.000000 not1mm-23.5.1/not1mm/testing/test.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.820775 not1mm-23.5.1/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20878 2023-05-01 16:46:02.000000 not1mm-23.5.1/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3354 2023-05-01 16:46:02.000000 not1mm-23.5.1/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-01 16:46:02.000000 not1mm-23.5.1/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-01 16:46:02.000000 not1mm-23.5.1/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-01 16:46:02.000000 not1mm-23.5.1/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-01 16:46:02.000000 not1mm-23.5.1/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1217 2023-05-01 16:43:42.000000 not1mm-23.5.1/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-01 16:46:02.847775 not1mm-23.5.1/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 16:46:02.847775 not1mm-23.5.1/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.1/testing/test.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-21 20:18:16.000000 not1mm-23.5.1/testing/text2.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.148401 not1mm-23.5.1.1/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.1.1/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21192 2023-05-01 21:18:17.147401 not1mm-23.5.1.1/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20445 2023-05-01 21:13:35.000000 not1mm-23.5.1.1/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.121401 not1mm-23.5.1.1/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.1.1/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    77167 2023-05-01 20:02:13.000000 not1mm-23.5.1.1/not1mm/__main__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    18880 2023-05-01 19:53:36.000000 not1mm-23.5.1.1/not1mm/bandmap.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.131401 not1mm-23.5.1.1/not1mm/data/
+-rw-rw-rw-   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.1.1/not1mm/data/Combinear.qss
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.1.1/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.1.1/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.1.1/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.1.1/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.1.1/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.1.1/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39001 2023-05-01 19:49:53.000000 not1mm-23.5.1.1/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.1.1/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.1.1/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.1.1/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.1.1/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.1.1/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.1.1/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.1.1/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.1.1/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.1.1/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.1.1/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.1.1/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43658 2023-05-01 15:38:56.000000 not1mm-23.5.1.1/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17745 2023-05-01 21:11:17.000000 not1mm-23.5.1.1/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.1.1/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.140401 not1mm-23.5.1.1/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.1.1/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.1.1/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.1.1/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.1.1/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.1.1/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.1.1/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.1.1/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.1.1/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.1.1/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.1.1/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.1.1/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.1.1/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.1.1/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.1.1/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.1.1/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.1.1/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.1.1/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.1.1/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.1.1/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.1.1/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.1.1/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.1.1/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.1.1/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.1.1/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.1.1/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.1.1/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.1.1/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.1.1/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.1.1/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.1.1/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.1.1/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.1.1/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.1.1/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.1.1/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.1.1/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.1.1/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.1.1/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.1.1/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.1.1/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.1.1/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.1.1/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.1.1/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.1.1/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.1.1/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.1.1/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.1.1/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.1.1/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.1.1/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.1.1/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.1.1/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.1.1/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.1.1/not1mm/data/ssbmacros.txt
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.143401 not1mm-23.5.1.1/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.1.1/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.1.1/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12468 2023-04-25 15:08:00.000000 not1mm-23.5.1.1/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.1.1/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32966 2023-04-24 03:05:48.000000 not1mm-23.5.1.1/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.1.1/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.1.1/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.1.1/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.1.1/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.1.1/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.1.1/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.1.1/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.1.1/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.1.1/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.1.1/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5781 2023-05-01 19:29:49.000000 not1mm-23.5.1.1/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       48 2023-05-01 21:16:13.000000 not1mm-23.5.1.1/not1mm/lib/version.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    31143 2023-05-01 19:53:26.000000 not1mm-23.5.1.1/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.147401 not1mm-23.5.1.1/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13552 2023-05-01 21:04:22.000000 not1mm-23.5.1.1/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13558 2023-05-01 16:14:59.000000 not1mm-23.5.1.1/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13565 2023-05-01 21:07:00.000000 not1mm-23.5.1.1/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13568 2023-05-01 21:07:03.000000 not1mm-23.5.1.1/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.1.1/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14348 2023-04-24 14:53:10.000000 not1mm-23.5.1.1/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14351 2023-04-24 14:53:19.000000 not1mm-23.5.1.1/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12719 2023-04-24 14:53:32.000000 not1mm-23.5.1.1/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2590 2023-04-24 14:53:43.000000 not1mm-23.5.1.1/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2591 2023-04-24 14:53:53.000000 not1mm-23.5.1.1/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2594 2023-04-24 14:54:04.000000 not1mm-23.5.1.1/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14755 2023-04-24 14:54:20.000000 not1mm-23.5.1.1/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14759 2023-04-24 14:54:36.000000 not1mm-23.5.1.1/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13701 2023-04-24 14:54:47.000000 not1mm-23.5.1.1/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13772 2023-04-24 14:54:56.000000 not1mm-23.5.1.1/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14624 2023-04-24 14:52:00.000000 not1mm-23.5.1.1/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7272 2023-04-24 14:55:06.000000 not1mm-23.5.1.1/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13650 2023-04-24 14:55:15.000000 not1mm-23.5.1.1/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13651 2023-04-24 14:55:25.000000 not1mm-23.5.1.1/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2851 2023-04-24 14:55:37.000000 not1mm-23.5.1.1/not1mm/plugins/winter_field_day.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.147401 not1mm-23.5.1.1/not1mm/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2297 2023-03-29 19:50:12.000000 not1mm-23.5.1.1/not1mm/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.122401 not1mm-23.5.1.1/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    21192 2023-05-01 21:18:17.000000 not1mm-23.5.1.1/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3460 2023-05-01 21:18:17.000000 not1mm-23.5.1.1/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-01 21:18:17.000000 not1mm-23.5.1.1/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-01 21:18:17.000000 not1mm-23.5.1.1/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-01 21:18:17.000000 not1mm-23.5.1.1/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-01 21:18:17.000000 not1mm-23.5.1.1/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1219 2023-05-01 21:16:15.000000 not1mm-23.5.1.1/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-01 21:18:17.148401 not1mm-23.5.1.1/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-01 21:18:17.147401 not1mm-23.5.1.1/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.1.1/testing/test.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-21 20:18:16.000000 not1mm-23.5.1.1/testing/text2.py
```

### Comparing `not1mm-23.5.1/LICENSE` & `not1mm-23.5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/PKG-INFO` & `not1mm-23.5.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.5.1
+Version: 23.5.1.1
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -53,14 +53,15 @@
   - [Selecting an existing contest as the current contest](#selecting-an-existing-contest-as-the-current-contest)
   - [Editing an existing contest parameters](#editing-an-existing-contest-parameters)
   - [Configuration Settings](#configuration-settings)
     - [Lookup](#lookup)
     - [Soundcard](#soundcard)
     - [CAT](#cat)
     - [CW Keyer interface](#cw-keyer-interface)
+    - [Cluster](#cluster)
   - [Hiding screen elements](#hiding-screen-elements)
   - [Editing macro keys](#editing-macro-keys)
     - [Macro substitutions](#macro-substitutions)
     - [Macro use with voice](#macro-use-with-voice)
   - [cty.dat and QRZ lookups for distance and bearing](#ctydat-and-qrz-lookups-for-distance-and-bearing)
   - [Other uses for the call field](#other-uses-for-the-call-field)
   - [Windows](#windows)
@@ -96,28 +97,31 @@
 Feature complete. I'm only one guy, and I'm not what you'd consider to be a contester. So new contests will be sparse.
 
 ![main screen](https://github.com/mbridak/not1mm/raw/master/pic/main.png)
 
 ## List of should be working contests
 
 - General Logging
+- 10 10 Fall CW
 - 10 10 Spring CW
+- 10 10 Summer Phone
+- 10 10 Winter Phone
 - ARRL DX CW
 - ARRL DX SSB
 - CQ WPX CW
 - CQ WPX SSB
 - CQ World Wide CW
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
-- [23-5-1] Added 10 10 Spring CW.
+- [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
 <details>
 
 <summary>April 2023</summary>
 
 - [23-4-29] Added callsign and connect button to the bandmap. Fixed rxmarker not updateing.
 - [23-4-28] Added a bandmap window (WIP) to track spots. Clicked spots now tune radio and sets callsign.
@@ -315,14 +319,18 @@
 
 Under the `CAT` TAB, you can choose either `rigctld` normally with an IP of `127.0.0.1` and a port of `4532`. Or `flrig`, IP normally of `127.0.0.1` and a port of `12345`. `None` is always an option, but is it really?
 
 ### CW Keyer interface
 
 Under the `CW` TAB, There are three options. `cwdaemon`, which normally uses IP `127.0.0.1` and port `6789`. `pywinkeyer` which normally uses IP `127.0.0.1` and port `8000`. Or `None`, if you want to Morse it like it's 1899.
 
+### Cluster
+
+  Under the `Cluster` TAB you can change the default AR Cluster server and port settings used for the bandmap window.
+
 ## Hiding screen elements
 
 You can show or hide certain buttons/indicators by checking and unchecking their boxes under the view menu. You can then resize the screen to make it more compact.
 
 ![View Menu](https://github.com/mbridak/not1mm/raw/master/pic/view_menu.png)
 
 The your choices will be remembered when you relaunch the program.
```

### Comparing `not1mm-23.5.1/README.md` & `not1mm-23.5.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
   - [Selecting an existing contest as the current contest](#selecting-an-existing-contest-as-the-current-contest)
   - [Editing an existing contest parameters](#editing-an-existing-contest-parameters)
   - [Configuration Settings](#configuration-settings)
     - [Lookup](#lookup)
     - [Soundcard](#soundcard)
     - [CAT](#cat)
     - [CW Keyer interface](#cw-keyer-interface)
+    - [Cluster](#cluster)
   - [Hiding screen elements](#hiding-screen-elements)
   - [Editing macro keys](#editing-macro-keys)
     - [Macro substitutions](#macro-substitutions)
     - [Macro use with voice](#macro-use-with-voice)
   - [cty.dat and QRZ lookups for distance and bearing](#ctydat-and-qrz-lookups-for-distance-and-bearing)
   - [Other uses for the call field](#other-uses-for-the-call-field)
   - [Windows](#windows)
@@ -77,28 +78,31 @@
 Feature complete. I'm only one guy, and I'm not what you'd consider to be a contester. So new contests will be sparse.
 
 ![main screen](https://github.com/mbridak/not1mm/raw/master/pic/main.png)
 
 ## List of should be working contests
 
 - General Logging
+- 10 10 Fall CW
 - 10 10 Spring CW
+- 10 10 Summer Phone
+- 10 10 Winter Phone
 - ARRL DX CW
 - ARRL DX SSB
 - CQ WPX CW
 - CQ WPX SSB
 - CQ World Wide CW
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
-- [23-5-1] Added 10 10 Spring CW.
+- [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
 <details>
 
 <summary>April 2023</summary>
 
 - [23-4-29] Added callsign and connect button to the bandmap. Fixed rxmarker not updateing.
 - [23-4-28] Added a bandmap window (WIP) to track spots. Clicked spots now tune radio and sets callsign.
@@ -296,14 +300,18 @@
 
 Under the `CAT` TAB, you can choose either `rigctld` normally with an IP of `127.0.0.1` and a port of `4532`. Or `flrig`, IP normally of `127.0.0.1` and a port of `12345`. `None` is always an option, but is it really?
 
 ### CW Keyer interface
 
 Under the `CW` TAB, There are three options. `cwdaemon`, which normally uses IP `127.0.0.1` and port `6789`. `pywinkeyer` which normally uses IP `127.0.0.1` and port `8000`. Or `None`, if you want to Morse it like it's 1899.
 
+### Cluster
+
+  Under the `Cluster` TAB you can change the default AR Cluster server and port settings used for the bandmap window.
+
 ## Hiding screen elements
 
 You can show or hide certain buttons/indicators by checking and unchecking their boxes under the view menu. You can then resize the screen to make it more compact.
 
 ![View Menu](https://github.com/mbridak/not1mm/raw/master/pic/view_menu.png)
 
 The your choices will be remembered when you relaunch the program.
```

### Comparing `not1mm-23.5.1/not1mm/__main__.py` & `not1mm-23.5.1.1/not1mm/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 from not1mm.lib.lookup import QRZlookup, HamDBlookup, HamQTH
 from not1mm.lib.multicast import Multicast
 from not1mm.lib.new_contest import NewContest
 from not1mm.lib.n1mm import N1MM
 from not1mm.lib.version import __version__
 
 os.environ["QT_QPA_PLATFORMTHEME"] = "gnome"
+# os.environ["QT_STYLE_OVERRIDE"] = "adwaita"
 
 loader = pkgutil.get_loader("not1mm")
 WORKING_PATH = os.path.dirname(loader.get_filename())
 
 if "XDG_DATA_HOME" in os.environ:
     DATA_PATH = os.environ.get("XDG_DATA_HOME")
 else:
@@ -158,14 +159,16 @@
         "userigctld": True,
         "useflrig": False,
         "cwip": "127.0.0.1",
         "cwport": 6789,
         "cwtype": 1,
         "useserver": False,
         "CAT_port": 4532,
+        "cluster_server": "dxc.nc7j.com",
+        "cluster_port": 7373,
     }
     appstarted = False
     contact = {}
     contest = None
     contest_settings = {}
     pref = None
     station = {}
@@ -1922,14 +1925,15 @@
     logger.setLevel(logging.DEBUG)
     logger.debug("debugging on")
 else:
     logger.setLevel(logging.WARNING)
     logger.warning("debugging off")
 
 app = QtWidgets.QApplication(sys.argv)
+app.setStyle("Fusion")
 font_path = WORKING_PATH + "/data"
 families = load_fonts_from_dir(os.fspath(font_path))
 logger.info(families)
 window = MainWindow()
 height = window.pref.get("window_height", 300)
 width = window.pref.get("window_width", 700)
 x = window.pref.get("window_x", -1)
```

### Comparing `not1mm-23.5.1/not1mm/bandmap.py` & `not1mm-23.5.1.1/not1mm/bandmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from datetime import datetime
 from json import JSONDecodeError, loads, dumps
 from pathlib import Path
 
 import logging
 import os
 import pkgutil
-import queue
 import sys
 import sqlite3
 
 from PyQt5 import QtCore, QtGui, Qt
 from PyQt5 import QtNetwork
 from PyQt5 import QtWidgets, uic
 
@@ -44,14 +43,20 @@
     CONFIG_PATH = str(Path.home() / ".config")
 CONFIG_PATH += "/not1mm"
 
 MULTICAST_PORT = 2239
 MULTICAST_GROUP = "224.1.1.1"
 INTERFACE_IP = "0.0.0.0"
 
+PREF = {}
+if os.path.exists(CONFIG_PATH + "/not1mm.json"):
+    with open(CONFIG_PATH + "/not1mm.json", "rt", encoding="utf-8") as file_descriptor:
+        PREF = loads(file_descriptor.read())
+
+
 # CTYFILE = {}
 
 # with open(WORKING_PATH + "/data/cty.json", "rt", encoding="utf-8") as c_file:
 #     CTYFILE = loads(c_file.read())
 
 
 # def cty_lookup(callsign: str):
@@ -188,15 +193,14 @@
     lineitemlist = []
     textItemList = []
     connected = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._udpwatch = None
-        self.udp_fifo = queue.Queue()
         data_path = WORKING_PATH + "/data/bandmap.ui"
         uic.loadUi(data_path, self)
         self.agetime = self.clear_spot_olderSpinBox.value()
         self.clear_spot_olderSpinBox.valueChanged.connect(self.spot_aging_changed)
         self.clearButton.clicked.connect(self.clear_spots)
         self.zoominButton.clicked.connect(self.dec_zoom)
         self.zoomoutButton.clicked.connect(self.inc_zoom)
@@ -231,15 +235,17 @@
         """doc"""
         if self.connected is True:
             self.socket.close()
             self.connected = False
             self.connectButton.setStyleSheet("color: red;")
             self.connectButton.setText("Closed")
             return
-        self.socket.connectToHost("dxc.nc7j.com", 7373)
+        server = PREF.get("cluster_server", "dxc.nc7j.com")
+        port = PREF.get("cluster_port", 7373)
+        self.socket.connectToHost(server, port)
         self.connectButton.setStyleSheet("color: white;")
         self.connectButton.setText("Connecting")
         self.connected = True
 
     def watch_udp(self):
         """doc"""
         while self.udpsocket.hasPendingDatagrams():
@@ -566,12 +572,12 @@
     logger.setLevel(logging.DEBUG)
     logger.debug("debugging on")
 else:
     logger.setLevel(logging.WARNING)
     logger.warning("debugging off")
 
 app = QtWidgets.QApplication(sys.argv)
-
+app.setStyle("Fusion")
 window = MainWindow()
 window.show()
 if __name__ == "__main__":
     run()
```

### Comparing `not1mm-23.5.1/not1mm/data/Combinear.qss` & `not1mm-23.5.1.1/not1mm/data/Combinear.qss`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-23.5.1.1/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/MASTER.SCP` & `not1mm-23.5.1.1/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/about.ui` & `not1mm-23.5.1.1/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/bandmap.ui` & `not1mm-23.5.1.1/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/configuration.ui` & `not1mm-23.5.1.1/not1mm/data/main.ui`

 * *Files 26% similar despite different names*

#### Comparing `not1mm-23.5.1/not1mm/data/configuration.ui` & `not1mm-23.5.1.1/not1mm/data/main.ui`

```diff
@@ -1,1070 +1,1433 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>Dialog</class>
-  <widget class="QDialog" name="Dialog">
+  <class>MainWindow</class>
+  <widget class="QMainWindow" name="MainWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>610</width>
-        <height>437</height>
+        <width>1975</width>
+        <height>366</height>
       </rect>
     </property>
+    <property name="sizePolicy">
+      <sizepolicy hsizetype="Minimum" vsizetype="Minimum">
+        <horstretch>0</horstretch>
+        <verstretch>0</verstretch>
+      </sizepolicy>
+    </property>
     <property name="font">
       <font>
         <family>JetBrains Mono</family>
+        <pointsize>11</pointsize>
       </font>
     </property>
-    <property name="windowTitle">
-      <string>Configuration Settings</string>
+    <property name="focusPolicy">
+      <enum>Qt::NoFocus</enum>
     </property>
-    <property name="styleSheet">
-      <string notr="true"/>
+    <property name="windowTitle">
+      <string>NOT1MM</string>
     </property>
-    <layout class="QGridLayout" name="gridLayout">
-      <item row="0" column="1">
-        <widget class="QTabWidget" name="tabWidget">
-          <property name="enabled">
-            <bool>true</bool>
-          </property>
-          <property name="font">
-            <font>
-              <family>JetBrains Mono</family>
-              <pointsize>12</pointsize>
-              <strikeout>false</strikeout>
-            </font>
-          </property>
-          <property name="tabPosition">
-            <enum>QTabWidget::North</enum>
-          </property>
-          <property name="tabShape">
-            <enum>QTabWidget::Rounded</enum>
-          </property>
-          <property name="currentIndex">
-            <number>2</number>
-          </property>
-          <property name="elideMode">
-            <enum>Qt::ElideNone</enum>
-          </property>
-          <property name="documentMode">
-            <bool>true</bool>
-          </property>
-          <property name="tabsClosable">
-            <bool>false</bool>
-          </property>
-          <property name="movable">
-            <bool>false</bool>
-          </property>
-          <property name="tabBarAutoHide">
-            <bool>false</bool>
-          </property>
-          <widget class="QWidget" name="lookup_tab">
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
-            </property>
-            <attribute name="title">
-              <string>Lookup</string>
-            </attribute>
-            <layout class="QGridLayout" name="gridLayout_2">
-              <item row="2" column="4">
-                <widget class="QRadioButton" name="usehamqth_radioButton">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="styleSheet">
-                    <string notr="true"/>
-                  </property>
-                  <property name="text">
-                    <string>Use HamQTH</string>
-                  </property>
-                  <attribute name="buttonGroup">
-                    <string notr="true">buttonGroup_2</string>
-                  </attribute>
-                </widget>
-              </item>
-              <item row="2" column="1">
-                <widget class="QRadioButton" name="useqrz_radioButton">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                      <bold>false</bold>
-                    </font>
-                  </property>
-                  <property name="autoFillBackground">
-                    <bool>false</bool>
-                  </property>
-                  <property name="styleSheet">
-                    <string notr="true"/>
-                  </property>
-                  <property name="text">
-                    <string>Use QRZ</string>
-                  </property>
-                  <attribute name="buttonGroup">
-                    <string notr="true">buttonGroup_2</string>
-                  </attribute>
-                </widget>
-              </item>
-              <item row="2" column="5">
-                <widget class="QRadioButton" name="radioButton_3">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>None</string>
-                  </property>
-                  <attribute name="buttonGroup">
-                    <string notr="true">buttonGroup_2</string>
-                  </attribute>
-                </widget>
-              </item>
-              <item row="0" column="3" colspan="3">
-                <widget class="QLineEdit" name="lookup_user_name_field">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                      <bold>false</bold>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string/>
-                  </property>
-                  <property name="placeholderText">
-                    <string>W1AW</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="2" column="3">
-                <widget class="QRadioButton" name="usehamdb_radioButton">
-                  <property name="enabled">
-                    <bool>false</bool>
-                  </property>
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="styleSheet">
-                    <string notr="true"/>
-                  </property>
-                  <property name="text">
-                    <string>Use HamDB</string>
-                  </property>
-                  <attribute name="buttonGroup">
-                    <string notr="true">buttonGroup_2</string>
-                  </attribute>
-                </widget>
-              </item>
-              <item row="1" column="1">
-                <widget class="QLabel" name="label_2">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                      <bold>false</bold>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>Password:</string>
-                  </property>
-                  <property name="alignment">
-                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                  </property>
-                </widget>
-              </item>
-              <item row="0" column="1">
-                <widget class="QLabel" name="label">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                      <bold>false</bold>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>User Name:</string>
-                  </property>
-                  <property name="alignment">
-                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                  </property>
-                </widget>
-              </item>
-              <item row="1" column="3" colspan="3">
-                <widget class="QLineEdit" name="lookup_password_field">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                      <bold>false</bold>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string/>
-                  </property>
-                  <property name="placeholderText">
-                    <string>Your Password</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="2" column="0">
-                <spacer name="horizontalSpacer">
-                  <property name="orientation">
-                    <enum>Qt::Horizontal</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>40</width>
-                      <height>20</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-              <item row="2" column="6">
-                <spacer name="horizontalSpacer_2">
-                  <property name="orientation">
-                    <enum>Qt::Horizontal</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>40</width>
-                      <height>20</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-            </layout>
-          </widget>
-          <widget class="QWidget" name="sound_tab">
-            <property name="enabled">
-              <bool>true</bool>
-            </property>
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-                <strikeout>false</strikeout>
-              </font>
-            </property>
-            <attribute name="title">
-              <string>Sound</string>
-            </attribute>
-            <layout class="QGridLayout" name="gridLayout_3">
-              <item row="3" column="0">
-                <spacer name="verticalSpacer_4">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-              <item row="1" column="0">
-                <widget class="QLabel" name="label_4">
-                  <property name="text">
-                    <string>Output Sound Device</string>
-                  </property>
-                  <property name="alignment">
-                    <set>Qt::AlignCenter</set>
-                  </property>
-                </widget>
-              </item>
-              <item row="2" column="0">
-                <widget class="QComboBox" name="sounddevice">
-                  <property name="enabled">
-                    <bool>true</bool>
-                  </property>
-                </widget>
-              </item>
-              <item row="0" column="0">
-                <spacer name="verticalSpacer_5">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-            </layout>
-          </widget>
-          <widget class="QWidget" name="cat_tab">
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-                <strikeout>false</strikeout>
-              </font>
-            </property>
-            <attribute name="title">
-              <string>CAT</string>
-            </attribute>
-            <layout class="QGridLayout" name="gridLayout_4">
-              <item row="1" column="1">
-                <widget class="QLineEdit" name="rigcontrolip_field">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                      <bold>false</bold>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>127.0.0.1</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="3" column="0" colspan="4">
-                <layout class="QHBoxLayout" name="horizontalLayout">
-                  <property name="sizeConstraint">
-                    <enum>QLayout::SetDefaultConstraint</enum>
-                  </property>
-                  <item>
-                    <spacer name="horizontalSpacer_4">
-                      <property name="orientation">
-                        <enum>Qt::Horizontal</enum>
-                      </property>
-                      <property name="sizeHint" stdset="0">
-                        <size>
-                          <width>40</width>
-                          <height>20</height>
-                        </size>
+    <widget class="QWidget" name="centralwidget">
+      <property name="focusPolicy">
+        <enum>Qt::NoFocus</enum>
+      </property>
+      <layout class="QGridLayout" name="gridLayout">
+        <property name="leftMargin">
+          <number>10</number>
+        </property>
+        <property name="rightMargin">
+          <number>10</number>
+        </property>
+        <property name="bottomMargin">
+          <number>0</number>
+        </property>
+        <item row="0" column="0">
+          <layout class="QVBoxLayout" name="verticalLayout" stretch="1,0">
+            <item>
+              <layout class="QHBoxLayout" name="mainsection">
+                <item>
+                  <widget class="QFrame" name="Band_Mode_Frame_CW">
+                    <property name="minimumSize">
+                      <size>
+                        <width>40</width>
+                        <height>0</height>
+                      </size>
+                    </property>
+                    <property name="lineWidth">
+                      <number>0</number>
+                    </property>
+                    <layout class="QVBoxLayout" name="bandmode_vertline">
+                      <property name="leftMargin">
+                        <number>0</number>
                       </property>
-                    </spacer>
-                  </item>
-                  <item>
-                    <widget class="QRadioButton" name="userigctld_radioButton">
-                      <property name="minimumSize">
-                        <size>
-                          <width>0</width>
-                          <height>28</height>
-                        </size>
+                      <property name="topMargin">
+                        <number>27</number>
                       </property>
-                      <property name="font">
-                        <font>
-                          <family>JetBrains Mono</family>
-                          <pointsize>12</pointsize>
-                          <bold>false</bold>
-                        </font>
+                      <property name="rightMargin">
+                        <number>0</number>
                       </property>
-                      <property name="styleSheet">
-                        <string notr="true"/>
+                      <property name="bottomMargin">
+                        <number>0</number>
                       </property>
-                      <property name="text">
-                        <string>rigctld</string>
+                      <item>
+                        <widget class="QLabel" name="mode_cw">
+                          <property name="text">
+                            <string>CW</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="cw_band_160">
+                          <property name="text">
+                            <string>160</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="cw_band_80">
+                          <property name="text">
+                            <string>80</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="cw_band_40">
+                          <property name="text">
+                            <string>40</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="cw_band_20">
+                          <property name="text">
+                            <string>20</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="cw_band_15">
+                          <property name="text">
+                            <string>15</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="cw_band_10">
+                          <property name="text">
+                            <string>10</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <spacer name="verticalSpacer">
+                          <property name="orientation">
+                            <enum>Qt::Vertical</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>20</width>
+                              <height>40</height>
+                            </size>
+                          </property>
+                        </spacer>
+                      </item>
+                    </layout>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QFrame" name="Band_Mode_Frame_SSB">
+                    <property name="minimumSize">
+                      <size>
+                        <width>35</width>
+                        <height>0</height>
+                      </size>
+                    </property>
+                    <property name="frameShape">
+                      <enum>QFrame::NoFrame</enum>
+                    </property>
+                    <property name="frameShadow">
+                      <enum>QFrame::Raised</enum>
+                    </property>
+                    <layout class="QVBoxLayout" name="verticalLayout_4">
+                      <property name="leftMargin">
+                        <number>0</number>
                       </property>
-                      <attribute name="buttonGroup">
-                        <string notr="true">buttonGroup</string>
-                      </attribute>
-                    </widget>
-                  </item>
-                  <item>
-                    <widget class="QRadioButton" name="useflrig_radioButton">
-                      <property name="font">
-                        <font>
-                          <family>JetBrains Mono</family>
-                          <pointsize>12</pointsize>
-                        </font>
+                      <property name="topMargin">
+                        <number>27</number>
                       </property>
-                      <property name="styleSheet">
-                        <string notr="true"/>
+                      <property name="rightMargin">
+                        <number>0</number>
                       </property>
-                      <property name="text">
-                        <string>flrig</string>
+                      <property name="bottomMargin">
+                        <number>0</number>
                       </property>
-                      <attribute name="buttonGroup">
-                        <string notr="true">buttonGroup</string>
-                      </attribute>
-                    </widget>
-                  </item>
-                  <item>
-                    <widget class="QRadioButton" name="radioButton">
-                      <property name="font">
-                        <font>
-                          <family>JetBrains Mono</family>
-                          <pointsize>12</pointsize>
-                        </font>
+                      <item>
+                        <widget class="QLabel" name="mode_ssb">
+                          <property name="text">
+                            <string>SSB</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="ssb_band_160">
+                          <property name="text">
+                            <string>160</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="ssb_band_80">
+                          <property name="text">
+                            <string>80</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="ssb_band_40">
+                          <property name="text">
+                            <string>40</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="ssb_band_20">
+                          <property name="text">
+                            <string>20</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="ssb_band_15">
+                          <property name="text">
+                            <string>15</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="ssb_band_10">
+                          <property name="text">
+                            <string>10</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <spacer name="verticalSpacer_2">
+                          <property name="orientation">
+                            <enum>Qt::Vertical</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>20</width>
+                              <height>40</height>
+                            </size>
+                          </property>
+                        </spacer>
+                      </item>
+                    </layout>
+                  </widget>
+                </item>
+                <item>
+                  <widget class="QFrame" name="Band_Mode_Frame_RTTY">
+                    <property name="minimumSize">
+                      <size>
+                        <width>33</width>
+                        <height>0</height>
+                      </size>
+                    </property>
+                    <property name="frameShape">
+                      <enum>QFrame::NoFrame</enum>
+                    </property>
+                    <property name="frameShadow">
+                      <enum>QFrame::Raised</enum>
+                    </property>
+                    <layout class="QVBoxLayout" name="verticalLayout_3">
+                      <property name="leftMargin">
+                        <number>0</number>
                       </property>
-                      <property name="text">
-                        <string>None</string>
+                      <property name="topMargin">
+                        <number>27</number>
                       </property>
-                      <attribute name="buttonGroup">
-                        <string notr="true">buttonGroup</string>
-                      </attribute>
-                    </widget>
-                  </item>
-                  <item>
-                    <spacer name="horizontalSpacer_3">
-                      <property name="orientation">
-                        <enum>Qt::Horizontal</enum>
+                      <property name="rightMargin">
+                        <number>0</number>
                       </property>
-                      <property name="sizeHint" stdset="0">
-                        <size>
-                          <width>40</width>
-                          <height>20</height>
-                        </size>
+                      <property name="bottomMargin">
+                        <number>0</number>
                       </property>
-                    </spacer>
-                  </item>
-                </layout>
-              </item>
-              <item row="2" column="1" colspan="3">
-                <spacer name="verticalSpacer_2">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-              <item row="1" column="0">
-                <widget class="QLabel" name="label_6">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                      <bold>false</bold>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>Rig Control IP:</string>
-                  </property>
-                  <property name="alignment">
-                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                  </property>
-                </widget>
-              </item>
-              <item row="0" column="2">
-                <spacer name="verticalSpacer">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-              <item row="1" column="2">
-                <widget class="QLabel" name="label_7">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                      <bold>false</bold>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>Port:</string>
-                  </property>
-                  <property name="alignment">
-                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                  </property>
-                </widget>
-              </item>
-              <item row="4" column="0" colspan="4">
-                <spacer name="verticalSpacer_3">
-                  <property name="orientation">
-                    <enum>Qt::Vertical</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>20</width>
-                      <height>40</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-              <item row="1" column="3">
-                <widget class="QLineEdit" name="rigcontrolport_field">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                      <bold>false</bold>
-                    </font>
-                  </property>
-                  <property name="inputMethodHints">
-                    <set>Qt::ImhDigitsOnly</set>
-                  </property>
-                  <property name="text">
-                    <string>4532</string>
-                  </property>
-                </widget>
-              </item>
-            </layout>
-          </widget>
-          <widget class="QWidget" name="cw_tab">
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
-            </property>
-            <attribute name="title">
-              <string>CW</string>
-            </attribute>
-            <layout class="QGridLayout" name="gridLayout_6">
-              <item row="1" column="2" colspan="2">
-                <widget class="QLineEdit" name="cwport_field">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="inputMethodHints">
-                    <set>Qt::ImhDigitsOnly</set>
-                  </property>
-                  <property name="text">
-                    <string>6789</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="1" column="1">
-                <widget class="QLabel" name="label_11">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>CW_Port:</string>
-                  </property>
-                  <property name="alignment">
-                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                  </property>
-                </widget>
-              </item>
-              <item row="2" column="0">
-                <spacer name="horizontalSpacer_5">
-                  <property name="orientation">
-                    <enum>Qt::Horizontal</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>40</width>
-                      <height>20</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-              <item row="2" column="2" alignment="Qt::AlignHCenter">
-                <widget class="QRadioButton" name="usepywinkeyer_radioButton">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>PyWinkeyer</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="2" column="3" alignment="Qt::AlignHCenter">
-                <widget class="QRadioButton" name="radioButton_5">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>None</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="0" column="2" colspan="2">
-                <widget class="QLineEdit" name="cwip_field">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>localhost</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="2" column="1" alignment="Qt::AlignHCenter">
-                <widget class="QRadioButton" name="usecwdaemon_radioButton">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>cwdaemon</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="0" column="1">
-                <widget class="QLabel" name="label_10">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>CW_Address:</string>
-                  </property>
-                  <property name="alignment">
-                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                  </property>
-                </widget>
-              </item>
-              <item row="2" column="4">
-                <spacer name="horizontalSpacer_6">
-                  <property name="orientation">
-                    <enum>Qt::Horizontal</enum>
-                  </property>
-                  <property name="sizeHint" stdset="0">
-                    <size>
-                      <width>40</width>
-                      <height>20</height>
-                    </size>
-                  </property>
-                </spacer>
-              </item>
-            </layout>
-          </widget>
-          <widget class="QWidget" name="group_tab">
-            <property name="enabled">
-              <bool>false</bool>
-            </property>
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
-            </property>
-            <attribute name="title">
-              <string>Group</string>
-            </attribute>
-            <layout class="QGridLayout" name="gridLayout_7">
-              <item row="0" column="0" colspan="2" alignment="Qt::AlignHCenter">
-                <widget class="QCheckBox" name="connect_to_server">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>Connect to server</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="1" column="0">
-                <widget class="QLabel" name="label_3">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>Multicast Group:</string>
-                  </property>
-                  <property name="alignment">
-                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                  </property>
-                </widget>
-              </item>
-              <item row="1" column="1">
-                <widget class="QLineEdit" name="multicast_group">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>224.1.1.1</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="2" column="0">
-                <widget class="QLabel" name="label_9">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>Multicast Port:</string>
-                  </property>
-                  <property name="alignment">
-                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                  </property>
-                </widget>
-              </item>
-              <item row="2" column="1">
-                <widget class="QLineEdit" name="multicast_port">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="inputMethodHints">
-                    <set>Qt::ImhDigitsOnly</set>
-                  </property>
-                  <property name="text">
-                    <string>2239</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="3" column="0">
-                <widget class="QLabel" name="label_12">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>Interface IP:</string>
-                  </property>
-                  <property name="alignment">
-                    <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                  </property>
-                </widget>
-              </item>
-              <item row="3" column="1">
-                <widget class="QLineEdit" name="interface_ip">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                      <pointsize>12</pointsize>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>0.0.0.0</string>
-                  </property>
-                </widget>
-              </item>
-            </layout>
-          </widget>
-          <widget class="QWidget" name="n1mm_tab">
-            <property name="enabled">
-              <bool>false</bool>
-            </property>
-            <property name="font">
-              <font>
-                <family>JetBrains Mono</family>
-              </font>
-            </property>
-            <attribute name="title">
-              <string>N1MM</string>
-            </attribute>
-            <layout class="QGridLayout" name="gridLayout_8">
-              <item row="1" column="0">
-                <widget class="QLabel" name="label_13">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>Station Name:</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="1" column="1" colspan="2">
-                <widget class="QLineEdit" name="n1mm_station_name">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                    </font>
-                  </property>
-                  <property name="placeholderText">
-                    <string/>
-                  </property>
-                </widget>
-              </item>
-              <item row="1" column="3">
-                <widget class="QLabel" name="label_14">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>Operator Name:</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="1" column="4">
-                <widget class="QLineEdit" name="n1mm_operator">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                    </font>
-                  </property>
-                  <property name="placeholderText">
-                    <string/>
-                  </property>
-                </widget>
-              </item>
-              <item row="2" column="0" colspan="2" alignment="Qt::AlignRight">
-                <widget class="QLabel" name="label_15">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>Destination Adderess:</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="4" column="0" colspan="2" alignment="Qt::AlignRight">
-                <widget class="QLabel" name="label_17">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>Contact Port:</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="5" column="1" alignment="Qt::AlignRight">
-                <widget class="QLabel" name="label_18">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>Lookup Port:</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="6" column="1" alignment="Qt::AlignRight">
-                <widget class="QLabel" name="label_19">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>Score Port:</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="0" column="0" colspan="5" alignment="Qt::AlignHCenter">
-                <widget class="QCheckBox" name="send_n1mm_packets">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                    </font>
-                  </property>
-                  <property name="styleSheet">
-                    <string notr="true"/>
-                  </property>
-                  <property name="text">
-                    <string>Send N1MM packets</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="3" column="0" colspan="2" alignment="Qt::AlignRight">
-                <widget class="QLabel" name="label_16">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string>Radio Port:</string>
-                  </property>
-                </widget>
-              </item>
-              <item row="2" column="2" colspan="3">
-                <widget class="QLineEdit" name="n1mm_ip">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                    </font>
-                  </property>
-                  <property name="text">
-                    <string/>
-                  </property>
-                  <property name="placeholderText">
-                    <string/>
-                  </property>
-                </widget>
-              </item>
-              <item row="3" column="2" colspan="3">
-                <widget class="QLineEdit" name="n1mm_radioport">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                    </font>
-                  </property>
-                  <property name="inputMethodHints">
-                    <set>Qt::ImhDigitsOnly</set>
-                  </property>
-                  <property name="text">
-                    <string/>
-                  </property>
-                  <property name="placeholderText">
-                    <string/>
-                  </property>
-                </widget>
-              </item>
-              <item row="4" column="2" colspan="3">
-                <widget class="QLineEdit" name="n1mm_contactport">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                    </font>
-                  </property>
-                  <property name="inputMethodHints">
-                    <set>Qt::ImhDigitsOnly</set>
-                  </property>
-                  <property name="text">
-                    <string/>
-                  </property>
-                  <property name="placeholderText">
-                    <string/>
-                  </property>
-                </widget>
-              </item>
-              <item row="5" column="2" colspan="3">
-                <widget class="QLineEdit" name="n1mm_lookupport">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                    </font>
-                  </property>
-                  <property name="inputMethodHints">
-                    <set>Qt::ImhDigitsOnly</set>
-                  </property>
-                  <property name="text">
-                    <string/>
-                  </property>
-                  <property name="placeholderText">
-                    <string/>
-                  </property>
-                </widget>
-              </item>
-              <item row="6" column="2" colspan="3">
-                <widget class="QLineEdit" name="n1mm_scoreport">
-                  <property name="font">
-                    <font>
-                      <family>JetBrains Mono</family>
-                    </font>
-                  </property>
-                  <property name="inputMethodHints">
-                    <set>Qt::ImhDigitsOnly</set>
-                  </property>
-                  <property name="text">
-                    <string/>
-                  </property>
-                  <property name="placeholderText">
-                    <string/>
-                  </property>
-                </widget>
-              </item>
-            </layout>
-          </widget>
-        </widget>
-      </item>
-      <item row="1" column="1" alignment="Qt::AlignHCenter">
-        <widget class="QDialogButtonBox" name="buttonBox">
-          <property name="sizePolicy">
-            <sizepolicy hsizetype="Maximum" vsizetype="Fixed">
-              <horstretch>0</horstretch>
-              <verstretch>0</verstretch>
-            </sizepolicy>
-          </property>
-          <property name="font">
-            <font>
-              <family>JetBrains Mono</family>
-              <pointsize>12</pointsize>
-              <bold>false</bold>
-            </font>
-          </property>
-          <property name="layoutDirection">
-            <enum>Qt::LeftToRight</enum>
-          </property>
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-          <property name="standardButtons">
-            <set>QDialogButtonBox::Cancel|QDialogButtonBox::Save</set>
-          </property>
-          <property name="centerButtons">
-            <bool>true</bool>
-          </property>
-        </widget>
-      </item>
-    </layout>
+                      <item>
+                        <widget class="QLabel" name="mode_rtty">
+                          <property name="text">
+                            <string>RTTY</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="rtty_band_160">
+                          <property name="text">
+                            <string>160</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="rtty_band_80">
+                          <property name="text">
+                            <string>80</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="rtty_band_40">
+                          <property name="text">
+                            <string>40</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="rtty_band_20">
+                          <property name="text">
+                            <string>20</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="rtty_band_15">
+                          <property name="text">
+                            <string>15</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <widget class="QLabel" name="rtty_band_10">
+                          <property name="text">
+                            <string>10</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignCenter</set>
+                          </property>
+                        </widget>
+                      </item>
+                      <item>
+                        <spacer name="verticalSpacer_3">
+                          <property name="orientation">
+                            <enum>Qt::Vertical</enum>
+                          </property>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>20</width>
+                              <height>40</height>
+                            </size>
+                          </property>
+                        </spacer>
+                      </item>
+                    </layout>
+                  </widget>
+                </item>
+                <item>
+                  <layout class="QVBoxLayout" name="main_dialog" stretch="0,0,0,0,0,0">
+                    <item>
+                      <layout class="QHBoxLayout" name="horizontalLayout" stretch="2,1,1,2,2">
+                        <item>
+                          <widget class="QFrame" name="callsignfield">
+                            <layout class="QVBoxLayout" name="input_call">
+                              <item>
+                                <widget class="QLabel" name="callsign_label">
+                                  <property name="text">
+                                    <string>Callsign</string>
+                                  </property>
+                                </widget>
+                              </item>
+                              <item>
+                                <widget class="QLineEdit" name="callsign">
+                                  <property name="font">
+                                    <font>
+                                      <family>JetBrains Mono</family>
+                                      <pointsize>20</pointsize>
+                                    </font>
+                                  </property>
+                                  <property name="focusPolicy">
+                                    <enum>Qt::ClickFocus</enum>
+                                  </property>
+                                  <property name="styleSheet">
+                                    <string notr="true">text-transform: uppercase;</string>
+                                  </property>
+                                </widget>
+                              </item>
+                            </layout>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QFrame" name="field1">
+                            <layout class="QVBoxLayout" name="input_snt">
+                              <item>
+                                <widget class="QLabel" name="snt_label">
+                                  <property name="text">
+                                    <string>SNT</string>
+                                  </property>
+                                  <property name="alignment">
+                                    <set>Qt::AlignBottom|Qt::AlignLeading|Qt::AlignLeft</set>
+                                  </property>
+                                </widget>
+                              </item>
+                              <item>
+                                <widget class="QLineEdit" name="sent">
+                                  <property name="font">
+                                    <font>
+                                      <family>JetBrains Mono</family>
+                                      <pointsize>20</pointsize>
+                                    </font>
+                                  </property>
+                                  <property name="focusPolicy">
+                                    <enum>Qt::ClickFocus</enum>
+                                  </property>
+                                  <property name="styleSheet">
+                                    <string notr="true">text-transform: uppercase;</string>
+                                  </property>
+                                </widget>
+                              </item>
+                            </layout>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QFrame" name="field2">
+                            <layout class="QVBoxLayout" name="input_rcv">
+                              <item>
+                                <widget class="QLabel" name="rcv_label">
+                                  <property name="text">
+                                    <string>RCV</string>
+                                  </property>
+                                  <property name="alignment">
+                                    <set>Qt::AlignBottom|Qt::AlignLeading|Qt::AlignLeft</set>
+                                  </property>
+                                </widget>
+                              </item>
+                              <item>
+                                <widget class="QLineEdit" name="receive">
+                                  <property name="font">
+                                    <font>
+                                      <family>JetBrains Mono</family>
+                                      <pointsize>20</pointsize>
+                                    </font>
+                                  </property>
+                                  <property name="focusPolicy">
+                                    <enum>Qt::ClickFocus</enum>
+                                  </property>
+                                  <property name="styleSheet">
+                                    <string notr="true">text-transform: uppercase;</string>
+                                  </property>
+                                </widget>
+                              </item>
+                            </layout>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QFrame" name="field3">
+                            <layout class="QVBoxLayout" name="input_other">
+                              <item>
+                                <widget class="QLabel" name="other_label">
+                                  <property name="text">
+                                    <string>OTHER_1</string>
+                                  </property>
+                                  <property name="alignment">
+                                    <set>Qt::AlignBottom|Qt::AlignLeading|Qt::AlignLeft</set>
+                                  </property>
+                                </widget>
+                              </item>
+                              <item>
+                                <widget class="QLineEdit" name="other_1">
+                                  <property name="font">
+                                    <font>
+                                      <family>JetBrains Mono</family>
+                                      <pointsize>20</pointsize>
+                                    </font>
+                                  </property>
+                                  <property name="focusPolicy">
+                                    <enum>Qt::ClickFocus</enum>
+                                  </property>
+                                  <property name="styleSheet">
+                                    <string notr="true">text-transform: uppercase;</string>
+                                  </property>
+                                </widget>
+                              </item>
+                            </layout>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QFrame" name="field4">
+                            <layout class="QVBoxLayout" name="verticalLayout_2">
+                              <property name="sizeConstraint">
+                                <enum>QLayout::SetDefaultConstraint</enum>
+                              </property>
+                              <item>
+                                <widget class="QLabel" name="label">
+                                  <property name="text">
+                                    <string>OTHER_2</string>
+                                  </property>
+                                  <property name="textFormat">
+                                    <enum>Qt::AutoText</enum>
+                                  </property>
+                                  <property name="alignment">
+                                    <set>Qt::AlignBottom|Qt::AlignLeading|Qt::AlignLeft</set>
+                                  </property>
+                                  <property name="buddy">
+                                    <cstring>field4</cstring>
+                                  </property>
+                                </widget>
+                              </item>
+                              <item>
+                                <widget class="QLineEdit" name="other_2">
+                                  <property name="font">
+                                    <font>
+                                      <family>JetBrains Mono</family>
+                                      <pointsize>20</pointsize>
+                                    </font>
+                                  </property>
+                                  <property name="focusPolicy">
+                                    <enum>Qt::ClickFocus</enum>
+                                  </property>
+                                  <property name="styleSheet">
+                                    <string notr="true">text-transform: uppercase;</string>
+                                  </property>
+                                </widget>
+                              </item>
+                            </layout>
+                          </widget>
+                        </item>
+                      </layout>
+                    </item>
+                    <item>
+                      <layout class="QHBoxLayout" name="run_vs_sanp">
+                        <property name="spacing">
+                          <number>6</number>
+                        </property>
+                        <property name="sizeConstraint">
+                          <enum>QLayout::SetDefaultConstraint</enum>
+                        </property>
+                        <item>
+                          <widget class="QLabel" name="leftdot">
+                            <property name="text">
+                              <string/>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="rightdot">
+                            <property name="text">
+                              <string/>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QRadioButton" name="radioButton_run">
+                            <property name="focusPolicy">
+                              <enum>Qt::NoFocus</enum>
+                            </property>
+                            <property name="text">
+                              <string>Run</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QRadioButton" name="radioButton_sp">
+                            <property name="focusPolicy">
+                              <enum>Qt::NoFocus</enum>
+                            </property>
+                            <property name="text">
+                              <string>S&amp;&amp;P</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QSpinBox" name="cw_speed">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="focusPolicy">
+                              <enum>Qt::NoFocus</enum>
+                            </property>
+                            <property name="wrapping">
+                              <bool>false</bool>
+                            </property>
+                            <property name="frame">
+                              <bool>true</bool>
+                            </property>
+                            <property name="alignment">
+                              <set>Qt::AlignCenter</set>
+                            </property>
+                            <property name="buttonSymbols">
+                              <enum>QAbstractSpinBox::UpDownArrows</enum>
+                            </property>
+                            <property name="suffix">
+                              <string/>
+                            </property>
+                            <property name="prefix">
+                              <string/>
+                            </property>
+                            <property name="minimum">
+                              <number>5</number>
+                            </property>
+                            <property name="maximum">
+                              <number>40</number>
+                            </property>
+                            <property name="value">
+                              <number>20</number>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <widget class="QLabel" name="dupe_indicator">
+                            <property name="enabled">
+                              <bool>true</bool>
+                            </property>
+                            <property name="font">
+                              <font>
+                                <family>JetBrains Mono</family>
+                                <pointsize>20</pointsize>
+                                <bold>true</bold>
+                              </font>
+                            </property>
+                            <property name="styleSheet">
+                              <string notr="true">color: rgb(246, 10, 10);</string>
+                            </property>
+                            <property name="text">
+                              <string>Dupe</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item>
+                          <spacer name="horizontalSpacer_3">
+                            <property name="orientation">
+                              <enum>Qt::Horizontal</enum>
+                            </property>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>40</width>
+                                <height>20</height>
+                              </size>
+                            </property>
+                          </spacer>
+                        </item>
+                      </layout>
+                    </item>
+                    <item>
+                      <widget class="QFrame" name="Button_Row1">
+                        <layout class="QHBoxLayout" name="ButtonRow1">
+                          <property name="sizeConstraint">
+                            <enum>QLayout::SetNoConstraint</enum>
+                          </property>
+                          <property name="leftMargin">
+                            <number>0</number>
+                          </property>
+                          <property name="topMargin">
+                            <number>0</number>
+                          </property>
+                          <property name="rightMargin">
+                            <number>0</number>
+                          </property>
+                          <property name="bottomMargin">
+                            <number>0</number>
+                          </property>
+                          <item>
+                            <widget class="QPushButton" name="F1">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>F1:</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="F2">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>F2:</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="F3">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>F3:</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="F4">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>F4:</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="F5">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>F5:</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="F6">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>F6:</string>
+                              </property>
+                            </widget>
+                          </item>
+                        </layout>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QFrame" name="Button_Row2">
+                        <property name="lineWidth">
+                          <number>0</number>
+                        </property>
+                        <layout class="QHBoxLayout" name="ButtonRow2">
+                          <property name="leftMargin">
+                            <number>0</number>
+                          </property>
+                          <property name="topMargin">
+                            <number>0</number>
+                          </property>
+                          <property name="rightMargin">
+                            <number>0</number>
+                          </property>
+                          <property name="bottomMargin">
+                            <number>0</number>
+                          </property>
+                          <item>
+                            <widget class="QPushButton" name="F7">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>F7:</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="F8">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>F8:</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="F9">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>F9:</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="F10">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>F10:</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="F11">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>F11:</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="F12">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>F12:</string>
+                              </property>
+                            </widget>
+                          </item>
+                        </layout>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QFrame" name="Command_Buttons">
+                        <layout class="QHBoxLayout" name="ButtonRow3">
+                          <property name="leftMargin">
+                            <number>0</number>
+                          </property>
+                          <property name="topMargin">
+                            <number>0</number>
+                          </property>
+                          <property name="rightMargin">
+                            <number>0</number>
+                          </property>
+                          <property name="bottomMargin">
+                            <number>0</number>
+                          </property>
+                          <item>
+                            <widget class="QPushButton" name="esc_stop">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>Esc: STOP</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="wipe">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>Wipe</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="log_it">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>Log It</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="edit">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>Edit</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="mark">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>Mark</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="store">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>Store</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="spot_it">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>Spot It</string>
+                              </property>
+                            </widget>
+                          </item>
+                          <item>
+                            <widget class="QPushButton" name="qrz">
+                              <property name="focusPolicy">
+                                <enum>Qt::NoFocus</enum>
+                              </property>
+                              <property name="text">
+                                <string>QRZ</string>
+                              </property>
+                            </widget>
+                          </item>
+                        </layout>
+                      </widget>
+                    </item>
+                    <item>
+                      <layout class="QHBoxLayout" name="horizontalLayout_6">
+                        <property name="sizeConstraint">
+                          <enum>QLayout::SetDefaultConstraint</enum>
+                        </property>
+                        <item>
+                          <widget class="QLabel" name="heading_distance">
+                            <property name="text">
+                              <string>Heading and Distance</string>
+                            </property>
+                          </widget>
+                        </item>
+                      </layout>
+                    </item>
+                  </layout>
+                </item>
+              </layout>
+            </item>
+            <item>
+              <layout class="QHBoxLayout" name="StatusLine">
+                <property name="sizeConstraint">
+                  <enum>QLayout::SetDefaultConstraint</enum>
+                </property>
+                <item>
+                  <widget class="QLabel" name="dx_entity">
+                    <property name="sizePolicy">
+                      <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
+                        <horstretch>0</horstretch>
+                        <verstretch>0</verstretch>
+                      </sizepolicy>
+                    </property>
+                    <property name="text">
+                      <string>dxentity</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <spacer name="horizontalSpacer">
+                    <property name="orientation">
+                      <enum>Qt::Horizontal</enum>
+                    </property>
+                    <property name="sizeHint" stdset="0">
+                      <size>
+                        <width>40</width>
+                        <height>20</height>
+                      </size>
+                    </property>
+                  </spacer>
+                </item>
+                <item>
+                  <widget class="QLabel" name="mults">
+                    <property name="text">
+                      <string>mults</string>
+                    </property>
+                  </widget>
+                </item>
+                <item>
+                  <spacer name="horizontalSpacer_2">
+                    <property name="orientation">
+                      <enum>Qt::Horizontal</enum>
+                    </property>
+                    <property name="sizeHint" stdset="0">
+                      <size>
+                        <width>40</width>
+                        <height>20</height>
+                      </size>
+                    </property>
+                  </spacer>
+                </item>
+                <item>
+                  <widget class="QLabel" name="score">
+                    <property name="text">
+                      <string>Score</string>
+                    </property>
+                  </widget>
+                </item>
+              </layout>
+            </item>
+          </layout>
+        </item>
+      </layout>
+    </widget>
+    <widget class="QMenuBar" name="menubar">
+      <property name="geometry">
+        <rect>
+          <x>0</x>
+          <y>0</y>
+          <width>1975</width>
+          <height>30</height>
+        </rect>
+      </property>
+      <widget class="QMenu" name="menuFile">
+        <property name="title">
+          <string>File</string>
+        </property>
+        <addaction name="actionNew_Database"/>
+        <addaction name="actionOpen_Database"/>
+        <addaction name="separator"/>
+        <addaction name="actionNew_Contest"/>
+        <addaction name="actionOpen_Contest"/>
+        <addaction name="actionEdit_Current_Contest"/>
+        <addaction name="separator"/>
+        <addaction name="actionGenerate_Cabrillo"/>
+        <addaction name="actionGenerate_ADIF"/>
+        <addaction name="separator"/>
+        <addaction name="actionConfiguration_Settings"/>
+        <addaction name="actionStationSettings"/>
+        <addaction name="separator"/>
+        <addaction name="actionEdit_Macros"/>
+      </widget>
+      <widget class="QMenu" name="menuHelp">
+        <property name="title">
+          <string>Help</string>
+        </property>
+        <addaction name="actionAbout"/>
+      </widget>
+      <widget class="QMenu" name="menuView">
+        <property name="title">
+          <string>View</string>
+        </property>
+        <addaction name="actionCommand_Buttons"/>
+        <addaction name="actionCW_Macros"/>
+        <addaction name="actionDark_Mode"/>
+      </widget>
+      <widget class="QMenu" name="menuWindow">
+        <property name="title">
+          <string>Window</string>
+        </property>
+        <addaction name="actionLog_Window"/>
+        <addaction name="actionBandmap"/>
+      </widget>
+      <widget class="QMenu" name="menuOther">
+        <property name="title">
+          <string>Misc</string>
+        </property>
+        <addaction name="actionRecalculate_Mults"/>
+      </widget>
+      <addaction name="menuFile"/>
+      <addaction name="menuView"/>
+      <addaction name="menuWindow"/>
+      <addaction name="menuOther"/>
+      <addaction name="menuHelp"/>
+    </widget>
+    <action name="actionAbout">
+      <property name="enabled">
+        <bool>true</bool>
+      </property>
+      <property name="text">
+        <string>About</string>
+      </property>
+      <property name="font">
+        <font>
+          <family>JetBrains Mono</family>
+        </font>
+      </property>
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
+    </action>
+    <action name="actionCommand_Buttons">
+      <property name="checkable">
+        <bool>true</bool>
+      </property>
+      <property name="checked">
+        <bool>true</bool>
+      </property>
+      <property name="text">
+        <string>Command Buttons</string>
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
+    <action name="actionCW_Macros">
+      <property name="checkable">
+        <bool>true</bool>
+      </property>
+      <property name="checked">
+        <bool>true</bool>
+      </property>
+      <property name="text">
+        <string>CW Macros</string>
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
+    <action name="actionMode_and_Bands">
+      <property name="checkable">
+        <bool>true</bool>
+      </property>
+      <property name="checked">
+        <bool>true</bool>
+      </property>
+      <property name="text">
+        <string>Mode and Bands</string>
+      </property>
+      <property name="font">
+        <font>
+          <family>JetBrains Mono</family>
+        </font>
+      </property>
+    </action>
+    <action name="actionDark_Mode">
+      <property name="checkable">
+        <bool>true</bool>
+      </property>
+      <property name="checked">
+        <bool>true</bool>
+      </property>
+      <property name="text">
+        <string>Force Dark Mode</string>
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
+    <action name="actionStationSettings">
+      <property name="text">
+        <string>Station Settings</string>
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
+    <action name="actionQRZ_Settings">
+      <property name="text">
+        <string>QRZ Settings</string>
+      </property>
+      <property name="font">
+        <font>
+          <family>JetBrains Mono</family>
+        </font>
+      </property>
+    </action>
+    <action name="actionConfiguration_Settings">
+      <property name="text">
+        <string>Configuration Settings</string>
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
+    <action name="actionGenerate_Cabrillo">
+      <property name="text">
+        <string>Generate Cabrillo</string>
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
+    <action name="actionLog_Window">
+      <property name="text">
+        <string>Log Window</string>
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
+    <action name="actionGenerate_ADIF">
+      <property name="text">
+        <string>Generate ADIF</string>
+      </property>
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
+    </action>
+    <action name="actionRecalculate_Mults">
+      <property name="text">
+        <string>Recalculate Mults</string>
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
+    <action name="actionNew_Contest">
+      <property name="text">
+        <string>New Contest</string>
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
+    <action name="actionNew_Database">
+      <property name="text">
+        <string>New Database</string>
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
+    <action name="actionOpen_Database">
+      <property name="text">
+        <string>Open Database</string>
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
+    <action name="actionOpen_Contest">
+      <property name="text">
+        <string>Open Contest</string>
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
+    </action>
   </widget>
   <resources/>
-  <connections>
-    <connection>
-      <sender>buttonBox</sender>
-      <signal>accepted()</signal>
-      <receiver>Dialog</receiver>
-      <slot>accept()</slot>
-      <hints>
-        <hint type="sourcelabel">
-          <x>248</x>
-          <y>254</y>
-        </hint>
-        <hint type="destinationlabel">
-          <x>157</x>
-          <y>274</y>
-        </hint>
-      </hints>
-    </connection>
-    <connection>
-      <sender>buttonBox</sender>
-      <signal>rejected()</signal>
-      <receiver>Dialog</receiver>
-      <slot>reject()</slot>
-      <hints>
-        <hint type="sourcelabel">
-          <x>316</x>
-          <y>260</y>
-        </hint>
-        <hint type="destinationlabel">
-          <x>286</x>
-          <y>274</y>
-        </hint>
-      </hints>
-    </connection>
-  </connections>
-  <buttongroups>
-    <buttongroup name="buttonGroup_2"/>
-    <buttongroup name="buttonGroup"/>
-  </buttongroups>
+  <connections/>
 </ui>
```

### Comparing `not1mm-23.5.1/not1mm/data/contests.sql` & `not1mm-23.5.1.1/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/cty.json` & `not1mm-23.5.1.1/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/editcontact.ui` & `not1mm-23.5.1.1/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/editmacro.ui` & `not1mm-23.5.1.1/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/k6gte.not1mm-128.png` & `not1mm-23.5.1.1/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/k6gte.not1mm-32.png` & `not1mm-23.5.1.1/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/k6gte.not1mm-64.png` & `not1mm-23.5.1.1/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/logwindow.ui` & `not1mm-23.5.1.1/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/new_contest.ui` & `not1mm-23.5.1.1/not1mm/data/new_contest.ui`

 * *Files 2% similar despite different names*

#### Comparing `not1mm-23.5.1/not1mm/data/new_contest.ui` & `not1mm-23.5.1.1/not1mm/data/new_contest.ui`

```diff
@@ -159,19 +159,34 @@
           <item>
             <property name="text">
               <string>General Logging</string>
             </property>
           </item>
           <item>
             <property name="text">
+              <string>10 10 FALL CW</string>
+            </property>
+          </item>
+          <item>
+            <property name="text">
               <string>10 10 SPRING CW</string>
             </property>
           </item>
           <item>
             <property name="text">
+              <string>10 10 SUMMER PHONE</string>
+            </property>
+          </item>
+          <item>
+            <property name="text">
+              <string>10 10 WINTER PHONE</string>
+            </property>
+          </item>
+          <item>
+            <property name="text">
               <string>ARRL DX CW</string>
             </property>
           </item>
           <item>
             <property name="text">
               <string>ARRL DX SSB</string>
             </property>
@@ -223,15 +238,15 @@
           </item>
         </widget>
       </item>
       <item row="2" column="2">
         <widget class="QDateTimeEdit" name="dateTimeEdit">
           <property name="time">
             <time>
-              <hour>0</hour>
+              <hour>8</hour>
               <minute>0</minute>
               <second>0</second>
             </time>
           </property>
           <property name="maximumDateTime">
             <datetime>
               <hour>7</hour>
```

### Comparing `not1mm-23.5.1/not1mm/data/opon.ui` & `not1mm-23.5.1.1/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/0.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/1.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/2.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/3.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/4.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/5.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/6.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/7.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/73.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/8.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/9.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/a.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/again.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/b.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/c.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/contest.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/cq.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/d.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/e.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/f.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/g.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/h.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/i.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/j.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/k.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/k6gte.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/l.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/m.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/mynumber.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/n.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/nil.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/o.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/p.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/q.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/r.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/roger.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/s.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/space.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/t.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/thankyou.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/u.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/v.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/w.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/x.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/y.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/yourcall.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/phonetics/z.wav` & `not1mm-23.5.1.1/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/pickcontest.ui` & `not1mm-23.5.1.1/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/reddot.png` & `not1mm-23.5.1.1/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/data/settings.ui` & `not1mm-23.5.1.1/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/lib/cat_interface.py` & `not1mm-23.5.1.1/not1mm/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/lib/cwinterface.py` & `not1mm-23.5.1.1/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/lib/database.py` & `not1mm-23.5.1.1/not1mm/lib/database.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/lib/edit_macro.py` & `not1mm-23.5.1.1/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/lib/edit_station.py` & `not1mm-23.5.1.1/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/lib/ham_utility.py` & `not1mm-23.5.1.1/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/lib/lookup.py` & `not1mm-23.5.1.1/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/lib/multicast.py` & `not1mm-23.5.1.1/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/lib/n1mm.py` & `not1mm-23.5.1.1/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/lib/settings.py` & `not1mm-23.5.1.1/not1mm/lib/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,18 @@
         )
         self.n1mm_operator.setText(str(self.preference.get("n1mm_operator", "")))
         self.n1mm_ip.setText(str(self.preference.get("n1mm_ip", "")))
         self.n1mm_radioport.setText(str(self.preference.get("n1mm_radioport", "")))
         self.n1mm_contactport.setText(str(self.preference.get("n1mm_contactport", "")))
         self.n1mm_lookupport.setText(str(self.preference.get("n1mm_lookupport", "")))
         self.n1mm_scoreport.setText(str(self.preference.get("n1mm_scoreport", "")))
+        self.cluster_server_field.setText(
+            str(self.preference.get("cluster_server", "dxc.nc7j.com"))
+        )
+        self.cluster_port_field.setText(str(self.preference.get("cluster_port", 7373)))
 
     def save_changes(self):
         """
         Write preferences to json file.
         """
         self.preference["sounddevice"] = self.sounddevice.currentText()
         self.preference["useqrz"] = self.useqrz_radioButton.isChecked()
@@ -104,7 +108,9 @@
         self.preference["n1mm_station_name"] = self.n1mm_station_name.text()
         self.preference["n1mm_operator"] = self.n1mm_operator.text()
         self.preference["n1mm_ip"] = self.n1mm_ip.text()
         self.preference["n1mm_radioport"] = self.n1mm_radioport.text()
         self.preference["n1mm_contactport"] = self.n1mm_contactport.text()
         self.preference["n1mm_lookupport"] = self.n1mm_lookupport.text()
         self.preference["n1mm_scoreport"] = self.n1mm_scoreport.text()
+        self.preference["cluster_server"] = self.cluster_server_field.text()
+        self.preference["cluster_port"] = int(self.cluster_port_field.text())
```

### Comparing `not1mm-23.5.1/not1mm/logwindow.py` & `not1mm-23.5.1.1/not1mm/logwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -731,14 +731,15 @@
     logger.setLevel(logging.DEBUG)
     logger.debug("debugging on")
 else:
     logger.setLevel(logging.WARNING)
     logger.warning("debugging off")
 
 app = QtWidgets.QApplication(sys.argv)
+app.setStyle("Fusion")
 font_path = WORKING_PATH + "/data"
 _families = load_fonts_from_dir(os.fspath(font_path))
 window = MainWindow()
 # window.setWindowTitle("Log Display")
 window.show()
 timer = QtCore.QTimer()
 timer.timeout.connect(window.check_udp_traffic)
```

### Comparing `not1mm-23.5.1/not1mm/plugins/10_10_spring_cw.py` & `not1mm-23.5.1.1/not1mm/plugins/10_10_spring_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/plugins/arrl_dx_cw.py` & `not1mm-23.5.1.1/not1mm/plugins/arrl_dx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-23.5.1.1/not1mm/plugins/arrl_dx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/plugins/arrl_field_day.py` & `not1mm-23.5.1.1/not1mm/plugins/arrl_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-23.5.1.1/not1mm/plugins/arrl_rtty_ru.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/plugins/arrl_ss_cw.py` & `not1mm-23.5.1.1/not1mm/plugins/arrl_ss_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/plugins/arrl_ss_phone.py` & `not1mm-23.5.1.1/not1mm/plugins/arrl_ss_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/plugins/cq_wpx_cw.py` & `not1mm-23.5.1.1/not1mm/plugins/cq_wpx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-23.5.1.1/not1mm/plugins/cq_wpx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/plugins/cq_ww_cw.py` & `not1mm-23.5.1.1/not1mm/plugins/cq_ww_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/plugins/cq_ww_ssb.py` & `not1mm-23.5.1.1/not1mm/plugins/cq_ww_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/plugins/cwt.py` & `not1mm-23.5.1.1/not1mm/plugins/cwt.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/plugins/general_logging.py` & `not1mm-23.5.1.1/not1mm/plugins/general_logging.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/plugins/jidx_cw.py` & `not1mm-23.5.1.1/not1mm/plugins/jidx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/plugins/jidx_ph.py` & `not1mm-23.5.1.1/not1mm/plugins/jidx_ph.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/plugins/winter_field_day.py` & `not1mm-23.5.1.1/not1mm/plugins/winter_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm/testing/test.py` & `not1mm-23.5.1.1/not1mm/testing/test.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.1/not1mm.egg-info/PKG-INFO` & `not1mm-23.5.1.1/not1mm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.5.1
+Version: 23.5.1.1
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -53,14 +53,15 @@
   - [Selecting an existing contest as the current contest](#selecting-an-existing-contest-as-the-current-contest)
   - [Editing an existing contest parameters](#editing-an-existing-contest-parameters)
   - [Configuration Settings](#configuration-settings)
     - [Lookup](#lookup)
     - [Soundcard](#soundcard)
     - [CAT](#cat)
     - [CW Keyer interface](#cw-keyer-interface)
+    - [Cluster](#cluster)
   - [Hiding screen elements](#hiding-screen-elements)
   - [Editing macro keys](#editing-macro-keys)
     - [Macro substitutions](#macro-substitutions)
     - [Macro use with voice](#macro-use-with-voice)
   - [cty.dat and QRZ lookups for distance and bearing](#ctydat-and-qrz-lookups-for-distance-and-bearing)
   - [Other uses for the call field](#other-uses-for-the-call-field)
   - [Windows](#windows)
@@ -96,28 +97,31 @@
 Feature complete. I'm only one guy, and I'm not what you'd consider to be a contester. So new contests will be sparse.
 
 ![main screen](https://github.com/mbridak/not1mm/raw/master/pic/main.png)
 
 ## List of should be working contests
 
 - General Logging
+- 10 10 Fall CW
 - 10 10 Spring CW
+- 10 10 Summer Phone
+- 10 10 Winter Phone
 - ARRL DX CW
 - ARRL DX SSB
 - CQ WPX CW
 - CQ WPX SSB
 - CQ World Wide CW
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
-- [23-5-1] Added 10 10 Spring CW.
+- [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
 <details>
 
 <summary>April 2023</summary>
 
 - [23-4-29] Added callsign and connect button to the bandmap. Fixed rxmarker not updateing.
 - [23-4-28] Added a bandmap window (WIP) to track spots. Clicked spots now tune radio and sets callsign.
@@ -315,14 +319,18 @@
 
 Under the `CAT` TAB, you can choose either `rigctld` normally with an IP of `127.0.0.1` and a port of `4532`. Or `flrig`, IP normally of `127.0.0.1` and a port of `12345`. `None` is always an option, but is it really?
 
 ### CW Keyer interface
 
 Under the `CW` TAB, There are three options. `cwdaemon`, which normally uses IP `127.0.0.1` and port `6789`. `pywinkeyer` which normally uses IP `127.0.0.1` and port `8000`. Or `None`, if you want to Morse it like it's 1899.
 
+### Cluster
+
+  Under the `Cluster` TAB you can change the default AR Cluster server and port settings used for the bandmap window.
+
 ## Hiding screen elements
 
 You can show or hide certain buttons/indicators by checking and unchecking their boxes under the view menu. You can then resize the screen to make it more compact.
 
 ![View Menu](https://github.com/mbridak/not1mm/raw/master/pic/view_menu.png)
 
 The your choices will be remembered when you relaunch the program.
```

### Comparing `not1mm-23.5.1/not1mm.egg-info/SOURCES.txt` & `not1mm-23.5.1.1/not1mm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,18 @@
 not1mm/lib/lookup.py
 not1mm/lib/multicast.py
 not1mm/lib/n1mm.py
 not1mm/lib/new_contest.py
 not1mm/lib/select_contest.py
 not1mm/lib/settings.py
 not1mm/lib/version.py
+not1mm/plugins/10_10_fall_cw.py
 not1mm/plugins/10_10_spring_cw.py
+not1mm/plugins/10_10_summer_phone.py
+not1mm/plugins/10_10_winter_phone.py
 not1mm/plugins/__init__.py
 not1mm/plugins/arrl_dx_cw.py
 not1mm/plugins/arrl_dx_ssb.py
 not1mm/plugins/arrl_field_day.py
 not1mm/plugins/arrl_rtty_ru.py
 not1mm/plugins/arrl_ss_cw.py
 not1mm/plugins/arrl_ss_phone.py
```

### Comparing `not1mm-23.5.1/pyproject.toml` & `not1mm-23.5.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "23.5.1"
+version = "23.5.1.1"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

### Comparing `not1mm-23.5.1/testing/test.py` & `not1mm-23.5.1.1/testing/test.py`

 * *Files identical despite different names*

